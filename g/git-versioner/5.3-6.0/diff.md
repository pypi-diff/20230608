# Comparing `tmp/git_versioner-5.3-py3-none-any.whl.zip` & `tmp/git_versioner-6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9391 bytes, number of entries: 7
--rw-r--r--  2.0 unx    17004 b- defN 23-Mar-31 04:09 __version__.py
--rw-rw-rw-  2.0 unx     1063 b- defN 23-Mar-31 04:09 git_versioner-5.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     5681 b- defN 23-Mar-31 04:09 git_versioner-5.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-31 04:09 git_versioner-5.3.dist-info/WHEEL
--rw-r--r--  2.0 unx      125 b- defN 23-Mar-31 04:09 git_versioner-5.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Mar-31 04:09 git_versioner-5.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      578 b- defN 23-Mar-31 04:09 git_versioner-5.3.dist-info/RECORD
-7 files, 24555 bytes uncompressed, 8363 bytes compressed:  65.9%
+Zip file size: 11053 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    19437 b- defN 23-Jun-08 00:35 __version__.py
+-rw-rw-rw-  2.0 unx     1063 b- defN 23-Jun-08 00:35 git_versioner-6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8080 b- defN 23-Jun-08 00:35 git_versioner-6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 00:35 git_versioner-6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      263 b- defN 23-Jun-08 00:35 git_versioner-6.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-08 00:35 git_versioner-6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      578 b- defN 23-Jun-08 00:35 git_versioner-6.0.dist-info/RECORD
+7 files, 29525 bytes uncompressed, 10025 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: __version__.py
 Comment: 
 
-Filename: git_versioner-5.3.dist-info/LICENSE
+Filename: git_versioner-6.0.dist-info/LICENSE
 Comment: 
 
-Filename: git_versioner-5.3.dist-info/METADATA
+Filename: git_versioner-6.0.dist-info/METADATA
 Comment: 
 
-Filename: git_versioner-5.3.dist-info/WHEEL
+Filename: git_versioner-6.0.dist-info/WHEEL
 Comment: 
 
-Filename: git_versioner-5.3.dist-info/entry_points.txt
+Filename: git_versioner-6.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: git_versioner-5.3.dist-info/top_level.txt
+Filename: git_versioner-6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: git_versioner-5.3.dist-info/RECORD
+Filename: git_versioner-6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## __version__.py

```diff
@@ -9,89 +9,139 @@
 import tempfile
 import argparse
 import setuptools
 import subprocess
 from pathlib import Path
 import traceback
 
+__all__ = [
+    "version",
+    "version_short",
+    "git_hash",
+    "on_tag",
+    "dirty",
+    "version_py",
+    "version_py_short",
+]
+
 
 # Set environment variable "VERSION_INCREMENT" to set next version jump
 VERSION_INCREMENT_ENV = "VERSION_INCREMENT"
 
 PROJECT_ROOT_ENV = "PROJECT_ROOT"
 
-VERSION_INCREMENT_PATCH = 'patch'
-VERSION_INCREMENT_MINOR = 'minor'
-VERSION_INCREMENT_MAJOR = 'major'
+VERSION_INCREMENT_PATCH = "patch"
+VERSION_INCREMENT_MINOR = "minor"
+VERSION_INCREMENT_MAJOR = "major"
 
 SUPPORT_PATCH = os.environ.get("VERSION_SUPPORT_PATCH", False)
 
-repo_dir = os.environ.get(PROJECT_ROOT_ENV, '.')
-
-
 VERBOSE = False
 
 # These are the main attributes tracked by git-versioner
 version = "0.0-new"
 version_short = "0.0.0" if SUPPORT_PATCH else "v0.0"
-git_hash = ''
+git_hash = ""
 on_tag = False
 dirty = True
 version_py = "0.0+new"
 version_py_short = "0.0"
 
 
 # Load snapshot of attributes if one exists
 try:
-    from _version import version, version_short, git_hash, on_tag, dirty, SUPPORT_PATCH
+
+    from _version import (  # type: ignore[no-redef]
+        version,
+        version_short,
+        git_hash,
+        on_tag,
+        dirty,
+        SUPPORT_PATCH,
+    )
+
     ignore_missing_git = True
-except:
+except ImportError:
     ignore_missing_git = False
 
 
-__git_safe_directory_cfg = None
+__repo_dir = None
+
+
+def repo_dir():
+    global __repo_dir
+    if __repo_dir is not None:
+        return __repo_dir
+
+    __repo_dir = os.environ.get(PROJECT_ROOT_ENV, None)
+
+    if not __repo_dir:
+        if not ignore_missing_git:
+            try:
+                __repo_dir = (
+                    subprocess.run(["git", "rev-parse", "--show-toplevel"], capture_output=True)
+                    .stdout.strip()
+                    .decode()
+                )
+            except:  # noqa: E722
+                pass
+    if not __repo_dir:
+        __repo_dir = "."
+
+    return __repo_dir
 
 
 def __git_safe_directory():
     global __git_safe_directory_cfg
-    if os.geteuid() == 0:
+    if hasattr(os, "geteuid") and os.geteuid() == 0:
         # running as root, likely inside container. Allow git to read repos from other users.
 
         if not __git_safe_directory_cfg:
-            real_gitconfig_file = Path(os.environ.get("GIT_CONFIG_GLOBAL", Path.home() / ".gitconfig"))
+            real_gitconfig_file = Path(
+                os.environ.get("GIT_CONFIG_GLOBAL", Path.home() / ".gitconfig")
+            )
             __git_safe_directory_cfg = tempfile.NamedTemporaryFile(prefix=".gitconfig_")
             if real_gitconfig_file.exists():
                 __git_safe_directory_cfg.write(real_gitconfig_file.read_bytes())
                 __git_safe_directory_cfg.flush()
 
             os.environ["GIT_CONFIG_GLOBAL"] = __git_safe_directory_cfg.name
             subprocess.check_output(["git", "config", "--global", "--add", "safe.directory", "*"])
 
 
+__git_safe_directory_cfg = None
 __git_safe_directory()
 
 
 def vers_split(vers):
     try:
-        return list(re.search(r"v?(\d+\.\d+(\.\d+)?)", vers).group(1).split('.'))
+        return list(re.search(r"v?(\d+\.\d+(\.\d+)?)", vers).group(1).split("."))
     except:
         print("Could not parse version from:", vers, file=sys.stderr)
         raise
 
 
 def get_version_info_from_git():
     global SUPPORT_PATCH
     fail_ret = None, None, None, None, True
     # Note: git describe doesn't work if no tag is available
-    current_commit = None
+    current_commit = ""
     try:
-        current_commit = subprocess.check_output(["git","rev-parse", "--short", "HEAD"],
-                                          cwd=repo_dir, stderr=subprocess.STDOUT, universal_newlines=True).strip()
-        git_describe = subprocess.check_output(["git", "describe", "--long", "--tags", "--dirty", "--always"],
-                                          cwd=repo_dir, stderr=subprocess.STDOUT, universal_newlines=True).strip()
+        current_commit = subprocess.check_output(
+            ["git", "rev-parse", "--short", "HEAD"],
+            cwd=repo_dir(),
+            stderr=subprocess.STDOUT,
+            universal_newlines=True,
+        ).strip()
+        git_describe = subprocess.check_output(
+            ["git", "describe", "--long", "--tags", "--dirty", "--always"],
+            cwd=repo_dir(),
+            stderr=subprocess.STDOUT,
+            universal_newlines=True,
+        ).strip()
     except subprocess.CalledProcessError as er:
         if VERBOSE:
             traceback.print_exc()
         if er.returncode == 128:
             # git exit code of 128 means no repository found
             return fail_ret
         git_describe = ""
@@ -99,48 +149,57 @@
         if VERBOSE:
             traceback.print_exc()
         return fail_ret
 
     if git_describe.startswith(current_commit):
         # No tags yet, new repo
         git_hash = current_commit
-        parts = re.match(r'(^[a-f0-9]*?)(-dirty)?$', git_describe.lower())
+        parts = re.match(r"(^[a-f0-9]*?)(-dirty)?$", git_describe.lower())
         git_dirty = parts.group(2)
         tag_name = ""
         if SUPPORT_PATCH:
-            git_tag_parts = ['0', '0', '0']
+            git_tag_parts = ["0", "0", "0"]
         else:
-            git_tag_parts = ['0', '0']
+            git_tag_parts = ["0", "0"]
         on_tag = False
 
     else:
-        desc_parts = re.match(r'(^.*?)-(\d+)-g([a-f0-9]+?)(-dirty)?$', git_describe)
+        desc_parts = re.match(r"(^.*?)-(\d+)-g([a-f0-9]+?)(-dirty)?$", git_describe)
         tag_name = desc_parts.group(1)
-        num_commits = desc_parts.group(2)
+        desc_parts.group(2)
         git_hash = desc_parts.group(3)
         git_dirty = desc_parts.group(4)
 
         git_tag_parts = vers_split(git_describe)
 
         if len(git_tag_parts) == 3:
             SUPPORT_PATCH = True
 
         try:
             # Find all tags on the commit and get the largest version if there are multiple
-            tag_sha = subprocess.check_output(["git", "rev-list", "-n", "1", tag_name],
-                                              cwd=repo_dir, stderr=subprocess.STDOUT, universal_newlines=True).strip()
+            tag_sha = subprocess.check_output(
+                ["git", "rev-list", "-n", "1", tag_name],
+                cwd=repo_dir(),
+                stderr=subprocess.STDOUT,
+                universal_newlines=True,
+            ).strip()
+
+            sha_tags = subprocess.check_output(
+                ["git", "tag", "--points-at", tag_sha],
+                cwd=repo_dir(),
+                stderr=subprocess.STDOUT,
+                universal_newlines=True,
+            ).strip()
 
-            sha_tags = subprocess.check_output(["git", "tag", "--points-at", tag_sha],
-                                               cwd=repo_dir, stderr=subprocess.STDOUT, universal_newlines=True).strip()
-
-            sha_tags = {tuple(vers_split(t)):t for t in sha_tags.split('\n')}
+            sha_tags = {tuple(vers_split(t)): t for t in sha_tags.split("\n")}
             git_tag_parts = max(sha_tags)
             tag_name = sha_tags[git_tag_parts]
 
-        except subprocess.CalledProcessError as er:
+        except subprocess.CalledProcessError:
+            tag_sha = ""
             if VERBOSE:
                 traceback.print_exc()
 
         except OSError:
             if VERBOSE:
                 traceback.print_exc()
             return fail_ret
@@ -154,35 +213,47 @@
     try:
         index = {
             VERSION_INCREMENT_PATCH: 2,
             VERSION_INCREMENT_MINOR: 1,
             VERSION_INCREMENT_MAJOR: 0,
         }[increment]
     except KeyError:
-        raise SystemExit("change: %s must be one of '%s', '%s' or '%s'" %
-                         (increment, VERSION_INCREMENT_MAJOR,
-                          VERSION_INCREMENT_MINOR, VERSION_INCREMENT_PATCH))
+        raise SystemExit(
+            "change: %s must be one of '%s', '%s' or '%s'"
+            % (
+                increment,
+                VERSION_INCREMENT_MAJOR,
+                VERSION_INCREMENT_MINOR,
+                VERSION_INCREMENT_PATCH,
+            )
+        )
     return index
 
 
 def increment_from_messages(tag_name):
     # Increment version
     increment = []
 
     # Check git logs between last tag and now
     try:
         git_range = "%s..HEAD" % tag_name if tag_name else "HEAD"
-        commit_messages = subprocess.check_output(["git", "log", git_range],
-                                cwd=repo_dir, stderr=subprocess.STDOUT, universal_newlines=True).strip()
+        commit_messages = subprocess.check_output(
+            ["git", "log", git_range],
+            cwd=repo_dir(),
+            stderr=subprocess.STDOUT,
+            universal_newlines=True,
+        ).strip()
     except subprocess.CalledProcessError:
-        commit_messages = ''
+        commit_messages = ""
 
-    for match in re.findall(r'CHANGE: *(%s|%s|%s)' % (
-        VERSION_INCREMENT_MAJOR, VERSION_INCREMENT_MINOR, VERSION_INCREMENT_PATCH
-    ), commit_messages):
+    for match in re.findall(
+        r"CHANGE: *(%s|%s|%s)"
+        % (VERSION_INCREMENT_MAJOR, VERSION_INCREMENT_MINOR, VERSION_INCREMENT_PATCH),
+        commit_messages,
+    ):
         try:
             increment.append(increment_index(match))
         except SystemExit as ex:
             print(ex.args, file=sys.stderr)
     if increment:
         return min(increment)
     return None
@@ -193,49 +264,57 @@
     parts, tag_name, g_hash, on_tag, dirty = get_version_info_from_git()
     if not parts:
         if ignore_missing_git:
             raise ResourceWarning()
         raise SystemExit("Error: Could not read git repo commit / details")
     try:
         if not (on_tag and not dirty):
-
             index = increment_from_messages(tag_name)
 
             # Fallback to checking env for increment if commit messages don't specify
             if index is None:
                 increment = os.environ.get(VERSION_INCREMENT_ENV, VERSION_INCREMENT_MINOR).lower()
                 index = increment_index(increment)
             if len(parts) < 2:
                 if VERBOSE:
-                    print("Adding minor version to scheme that previously had only major", file=sys.stderr)
-                parts.append('0')
+                    print(
+                        "Adding minor version to scheme that previously had only major",
+                        file=sys.stderr,
+                    )
+                parts.append("0")
             if len(parts) < 3 and (
-                SUPPORT_PATCH or
-                index == increment_index(VERSION_INCREMENT_PATCH)
+                SUPPORT_PATCH or index == increment_index(VERSION_INCREMENT_PATCH)
             ):
                 if VERBOSE:
-                    print("Adding patch version to scheme that is currently only <major>.<minor>", file=sys.stderr)
+                    print(
+                        "Adding patch version to scheme that is currently only <major>.<minor>",
+                        file=sys.stderr,
+                    )
                 SUPPORT_PATCH = True
-                parts.append('0')
+                parts.append("0")
 
             max_index = 2 if SUPPORT_PATCH else 1
 
-            parts = parts[0:index] + [str(int(parts[index]) + 1)] + (['0'] * max(0, (max_index - index)))
+            parts = (
+                parts[0:index]
+                + [str(int(parts[index]) + 1)]
+                + (["0"] * max(0, (max_index - index)))
+            )
 
     except (IndexError, ValueError, AttributeError) as ex:
         if "'NoneType' object has no attribute 'group'" in str(ex):  # regex fail
             print("Parsing version number failed:", tag_name, file=sys.stderr)
         else:
             print("Could not increment %s : %s" % (tag_name, ex), file=sys.stderr)
 
     vers_short = "v" + ".".join(parts)
     if on_tag and not dirty:
         vers_long = on_tag
     else:
-        vers_long = vers_short + '-g' + g_hash
+        vers_long = vers_short + "-g" + g_hash
         if dirty:
             vers_long += "-dirty"
 
     return vers_short, vers_long, g_hash, on_tag, dirty
 
 
 def py_version():
@@ -259,40 +338,42 @@
     vers = pv_short
     if local_parts:
         vers = "+".join((vers, ".".join(local_parts)))
 
     # normalise the version to suitable package version
     try:
         from setuptools.extern import packaging
+
         vers = str(packaging.version.Version(vers))
-    except:
+    except:  # noqa: E722
         pass
 
     return vers, pv_short
 
 
 def save(dest=None):
-    import json
-    dest = dest or Path(repo_dir)
+
+    dest = dest or Path(repo_dir())
     if dest.is_dir():
-        dest /= '_version.py'
+        dest /= "_version.py"
     dest.write_text(
-        '# Version managed by git-versioner\n'
+        "# Version managed by git-versioner\n"
         f'version = "{version}"\n'
         f'version_short = "{version_short}"\n'
         f'git_hash = "{git_hash}"\n'
-        f'on_tag = {repr(on_tag)}\n'
-        f'dirty = {True if dirty else False}\n'
-        f'SUPPORT_PATCH = {True if SUPPORT_PATCH else False}\n'
+        f"on_tag = {repr(on_tag)}\n"
+        f"dirty = {True if dirty else False}\n"
+        f"SUPPORT_PATCH = {True if SUPPORT_PATCH else False}\n"
     )
 
 
 def rename_file(pattern, short):
     global version, version_short
     import glob
+
     for f in glob.glob(pattern):
         f = Path(f)
         newname = f.name.format(
             version=version,
             version_short=version_short,
             git_hash=git_hash,
         )
@@ -304,32 +385,31 @@
 
 
 def fill_file(template_file, output_file):
     template_file = Path(template_file)
     output_file = Path(output_file)
     template = template_file.read_text()
     output = template.format(
-            version=version,
-            version_short=version_short,
-            git_hash=git_hash,
-        )
+        version=version,
+        version_short=version_short,
+        git_hash=git_hash,
+    )
     output_file.write_text(output)
     print("Written:", output_file)
 
 
 ## Set the global version values
 error = None
 
 # Check for static vars in env first
 if any((key for key in os.environ if key.startswith("GIT_VERSIONER"))):
+
     def parse_bool_str(v):
         return (
-            True if v.lower() in ["true", "1"] else
-            False if v.lower() in ["false", "0", ""] else
-            v
+            True if v.lower() in ["true", "1"] else False if v.lower() in ["false", "0", ""] else v
         )
 
     version = os.environ.get("GIT_VERSIONER_VERSION", version)
     version_short = os.environ.get("GIT_VERSIONER_VERSION_SHORT", version_short)
     git_hash = os.environ.get("GIT_VERSIONER_GIT_HASH", git_hash)
     on_tag = parse_bool_str(os.environ.get("GIT_VERSIONER_ON_TAG", repr(on_tag)))
     dirty = parse_bool_str(os.environ.get("GIT_VERSIONER_DIRTY", repr(dirty)))
@@ -342,86 +422,124 @@
         pass
     except Exception as ex:
         error = str(ex)
 
     version_py, version_py_short = py_version()
 
 
-def setup_keyword(dist: setuptools.Distribution, keyword, value):
+def setuptools_finalize(dist: setuptools.Distribution):
+    settings = None
+    # read settings from toml
+    pyproject = Path(repo_dir()) / "pyproject.toml"
+    if pyproject.exists():
+        toml_settings = []
+        try:
+            import tomllib
+        except ImportError:
+            import tomli as tomllib
+        with pyproject.open("rb") as t:
+            parsed = tomllib.load(t)
+        config = parsed.get("tool", {}).get("git-versioner", {})
+        for setting in (
+            "snapshot",
+            "desc",
+            "gitlab",
+            "short",
+        ):
+            if config.get(setting, False):
+                toml_settings.append(setting)
+        settings = ",".join(toml_settings)
+
+    if not settings:
+        # read settings from setup.py
+        settings = getattr(dist, "use_git_versioner", None)
+
+    setup_keyword(dist, value=settings)
+
+
+distribution_verson = setuptools_finalize
+
+
+def setup_keyword(dist: setuptools.Distribution, keyword=None, value=None):
     global version_py, version_py_short, setuptools
     if not value:
         return
 
     # setuptools command to save a static __version__.py in the build package
     class VersionCommand(setuptools.Command):
         def initialize_options(self):
             pass
 
         def finalize_options(self):
             pass
 
         def run(self):
-            build = self.distribution.command_obj.get('build')
+            build = self.distribution.command_obj.get("build")
             if build and self.distribution.packages:
                 for package in self.distribution.packages:
                     dest = Path(build.build_lib) / package
                     if dest.exists():
                         save(dest / "__version__.py")
 
-            sdist = self.distribution.command_obj.get('sdist')
+            sdist = self.distribution.command_obj.get("sdist")
             if sdist and sdist.filelist:
                 save()
                 sdist.filelist.files.append("_version.py")
 
-
-    command = 'git-versioner'
+    command = "git-versioner"
     try:
         import pkg_resources
+
         command += ":" + pkg_resources.get_distribution("git-versioner").version
-    except:
+    except:  # noqa: E722
         pass
 
     dist.cmdclass[command] = VersionCommand
 
     # set the package version
     dist.metadata.version = version_py
 
-    if "sdist" in dist.script_args:
+    if dist.script_args and "sdist" in dist.script_args:
         try:
-            from setuptools.command import sdist
+            from setuptools.command import sdist  # type: ignore[no-redef]
         except ImportError:
-            from distutils.command import sdist
+            from distutils.command import sdist  # type: ignore[no-redef]
         sdist.sdist.sub_commands.append((command, None))
 
     # Cache the version in env for isolated builds
     if not any((key for key in os.environ if key.startswith("GIT_VERSIONER"))):
         os.environ["GIT_VERSIONER_VERSION"] = version
         os.environ["GIT_VERSIONER_VERSION_SHORT"] = version_short
-        os.environ["GIT_VERSIONER_GIT_HASH"] = git_hash
+        os.environ["GIT_VERSIONER_GIT_HASH"] = str(git_hash)
         os.environ["GIT_VERSIONER_ON_TAG"] = repr(on_tag)
         os.environ["GIT_VERSIONER_DIRTY"] = "True" if dirty else "False"
         os.environ["GIT_VERSIONER_VERSION_PY"] = version_py
         os.environ["GIT_VERSIONER_VERSION_PY_SHORT"] = version_py_short
 
     # Handle options
     if not isinstance(value, str):
         return
 
     if "snapshot" in value:
         try:
-            from setuptools.command import build
+            from setuptools.command import build  # type: ignore[no-redef]
         except ImportError:
-            from distutils.command import build
+            from distutils.command import build  # type: ignore[no-redef]
         build.build.sub_commands.append((command, None))
 
     if "desc" in value:
         # function can be run multiple times, ensure we only append once.
+        if not dist.metadata.long_description:
+            dist.metadata.long_description = ""
         if not dist.metadata.long_description.strip().endswith(version_py):
             dist.metadata.long_description += f"\n\nversion: {version_py}"
 
+    if "short" in value:
+        dist.metadata.version = version_py_short
+
     if "gitlab" in value:
         # Long (PEP440 local) number schemes aren't allowed on PyPI
         # This scheme uses short version when building from default branch
         # or on tags.
         ci_commit_tag = os.environ.get("CI_COMMIT_TAG")
         if ci_commit_tag:
             dist.metadata.version = version_py_short
@@ -431,42 +549,49 @@
             ci_default_branch = os.environ["CI_DEFAULT_BRANCH"]
             if ci_commit_branch == ci_default_branch:
                 dist.metadata.version = version_py_short
         except KeyError:
             # No env CI_DEFAULT_BRANCH, not running in Gitlab CI.
             pass
 
-    elif "short" in value:
-        dist.metadata.version = version_py_short
-
 
 def main():
     global version, version_short, git_hash, on_tag, dirty, VERBOSE
 
-    parser = argparse.ArgumentParser(description='Mange current/next version.')
-    parser.add_argument('--save', action='store_true', help='Store in _version.py')
-    parser.add_argument('--short', action='store_true', help='Print the short version string')
-    parser.add_argument('--git', action='store_true', help='Print the release git hash')
-    parser.add_argument('--python', action='store_true', help='display the python formatted version strings')
-    parser.add_argument('--rename', help='Add version numbers to filename(s)')
-    parser.add_argument('--template', metavar=('template', 'output'), type=Path, nargs=2,
-                        help='Add version to <template> and write result to <output>')
-    parser.add_argument('--tag', action='store_true', help='Creates git tag to release the current commit')
-    parser.add_argument('--verbose', action='store_true', help='provide more detail on error')
+    parser = argparse.ArgumentParser(description="Mange current/next version.")
+    parser.add_argument("--save", action="store_true", help="Store in _version.py")
+    parser.add_argument("--short", action="store_true", help="Print the short version string")
+    parser.add_argument("--git", action="store_true", help="Print the release git hash")
+    parser.add_argument(
+        "--python", action="store_true", help="display the python formatted version strings"
+    )
+    parser.add_argument("--rename", help="Add version numbers to filename(s)")
+    parser.add_argument(
+        "--template",
+        metavar=("template", "output"),
+        type=Path,
+        nargs=2,
+        help="Add version to <template> and write result to <output>",
+    )
+    parser.add_argument(
+        "--tag", action="store_true", help="Creates git tag to release the current commit"
+    )
+    parser.add_argument("--verbose", action="store_true", help="provide more detail on error")
     args = parser.parse_args()
 
     VERBOSE = args.verbose
 
     if error:
         # if there was an error during initial processing
         # above, try re-running it here.
         try:
             version_short, version, git_hash, on_tag, dirty = git_version()
-        except:
+        except:  # noqa: E722
             import traceback
+
             traceback.print_exc()
     if args.save:
         save()
 
     if args.rename:
         rename_file(args.rename, args.short)
         return
@@ -476,15 +601,15 @@
 
     if args.tag:
         if on_tag:
             raise SystemExit("Already on tag", on_tag)
         if dirty:
             raise SystemExit("Git dirty, cannot tag")
         print(version_short)
-        subprocess.run(["git", "tag", version_short], cwd=repo_dir)
+        subprocess.run(["git", "tag", version_short], cwd=repo_dir())
 
     if args.short:
         if args.python:
             print(version_py_short)
         else:
             print(version_short)
     elif args.git:
```

## Comparing `git_versioner-5.3.dist-info/LICENSE` & `git_versioner-6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `git_versioner-5.3.dist-info/METADATA` & `git_versioner-6.0.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,143 +1,223 @@
 Metadata-Version: 2.1
 Name: git-versioner
-Version: 5.3
+Version: 6.0
 Summary: Manage current / next version for project
-Home-page: https://gitlab.com/alelec/__version__
-Author: Andrew Leech
-Author-email: andrew@alelec.net
-License: MIT
+Author-email: Andrew Leech <andrew@alelec.net>
+License: MIT License
+        
+        Copyright (c) 2022 alelec
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://gitlab.com/alelec/__version__
+Project-URL: Documentation, https://gitlab.com/alelec/__version__/-/blob/main/README.md
+Project-URL: Repository, https://gitlab.com/alelec/__version__
+Project-URL: Changelog, https://gitlab.com/alelec/__version__/-/commits/main?ref_type=heads
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: tomli ; python_version < "3.11"
 
-=============
-git-versioner
-=============
+# git-versioner
 
-Manages the version number for the project based on git tags. The goal of this packages versioning scheme is to
-avoid ever needing to manually create versions numbers or update version details in files that need to
+Manages the version number for the project based on git tags. The goal
+of this packages versioning scheme is to avoid ever needing to manually
+create versions numbers or update version details in files that need to
 be committed to the repository.
 
 The general rule is:
 
-- If on a tag, report that as-is.
-- When changes are made / git commits added, auto-increment the appropriate level of the semantic version.
+*   If on a tag, report that as-is.
+*   When changes are made / git commits added, auto-increment the
+    appropriate level of the semantic version.
+
+When on a git tag like `v1.2` the version will be reported as `v1.2` in
+short form or `v1.2-g<githash>` in the (default) long form, eg.
+`v1.2-ga1b2c3`
+
+After editing you working tree, by default the minor version attribute
+will be updated, eg `v1.2` -\> `v1.3` or `1.2.3` -\> `1.3.0`
+
+## Version Increments
+
+The increment can be changed by adding one of the following footers to
+any commit since the previous tag:
+
+> `CHANGE: major` 
+
+> `CHANGE: minor`  
+
+> `CHANGE: patch`  
+
+Then the most significant increment specified in any commit will be
+used.
+
+Alternatively this can be overridden at runtime by setting the
+environment variable `VERSION_INCREMENT` to one of `major`, `minor` or
+`patch`
+
+By default on new projects a 2 point version scheme will be used, eg
+v1.2, however the patch level (v1.2.3) will be used if either: 
+* the previous tag includes it 
+* patch level increment is set via commit footer or  `VERSION_INCREMENT` env 
+* the following env variable is
+configured: `VERSION_SUPPORT_PATCH=1`
+
+This setting will be persisted if saved, eg
+`VERSION_SUPPORT_PATCH=1 python -m __version__ --save`
+
+## Project Version
+
+The overall goal is for any commit to be suitable as a potential
+release. As such you can build away, testing your main branch builds and
+as soon as one of them is ready to go simply run
+`python -m __version__ --tag` to have it tagged off with the same
+version number the build already had. Indeed this step can be done in
+CI, take at a look at this projects
+[.gitlab-ci.yml](https://gitlab.com/alelec/__version__/-/blob/main/.gitlab-ci.yml)
+for an example of a manual CI task to \"release this commit\".
+
+gitlab-versioner can be used to provide dynamic versioning in
+setuptools, with support for both `pyproject.toml` and the
+older `setup.py`
+
+For `pyproject.toml` usage; enable dynamic versions in the project section, add `git-versioner` to the build requirements list and add a `[tool.git-versioner]` section to enable git-versioner. Settings 
+
+``` toml
+[project]
+name = "my-project"
+...
+dynamic = ["version"]
+
+[build-system]
+requires = [ "setuptools\>=57", "wheel", "git-versioner>=6.0"]
+build-backend = "setuptools.build_meta"
+
+[tool.git-versioner] 
+```
+
+Alternatively for `setup.py`; add the kwarg
+`use_git_versioner=<True or settings>` and include `git-versioner` in
+the `setup_requires` list:
+
+``` python
+setup(
+    name="my-project",
+    author="Andrew Leech",
+    author_email="andrew@alelec.net",
+    use_git_versioner=True,
+    setup_requires=["git-versioner"],
+    ...
+)
+```
+
+## Dynamic package version options
+
+If no extra settings are added to the `pyproject.toml` / `[tool.git-versioner]`
+section, or `use_git_versioner=True` is set in `setup.py` then default
+version format will be used.  
+This will be the full / long version following
+[PEP440](https://peps.python.org/pep-0440/#local-version-identifiers)
+local version format.
+
+If you want to push the package to PyPI however the short version must
+be used which can be specified with :
+
+``` toml
+[tool.git-versioner]
+short = true
+```
+or
+``` python
+use_git_versioner="short"
+```
+
+The full python version number can also added to the description, which
+can be especially useful when the package is published with the short
+number. Do enable this you can use `desc = true` /
+`use_git_versioner="desc"` in which case a line like
+`version: 1.2.3+ga1b2c3d` will be added to the bottom of the "long
+description" metadata.
+
+When building a package, the version details can be automatically saved
+into `<package>.__version__.py` in the built wheel with the setting
+`snapshot = true` / `use_git_versioner="snapshot"`.
+
+If being used in Gitlab CI for builds an automated versioning scheme can
+be specified with `gitlab = true` / `use_git_versioner="gitlab"`. In
+this mode, potential release builds from the default / main branch or
+from tags will use the short version, with anything else (eg. dev
+branches, pr\'s, local builds) using the long version scheme.
 
-When on a git tag like ``v1.2`` the version will be reported as ``v1.2`` in short form or
-``v1.2-g<githash>`` in the (default) long form, eg. ``v1.2-ga1b2c3``
+Multiple settings can be combined in `setup.py` but including them all
+in the settings string, eg `use_git_versioner="short,desc,snapshot"`.
 
+## Runtime Access
 
-After editing you working tree, by default the minor version attribute will be updated, eg ``v1.2`` -> ``v1.3``
-or ``1.2.3`` -> ``1.3.0``
-
-Version Increments
-------------------
-
-The increment can be changed by adding one of the following footers to any commit since the previous tag:
-
-- ``CHANGE: major``
-- ``CHANGE: minor``
-- ``CHANGE: patch``
-
-Then the most significant increment specified in any commit will be used.
-
-Alternatively this can be overridden at runtime by setting the environment variable ``VERSION_INCREMENT`` to
-one of ``major``, ``minor`` or ``patch``
-
-By default on new projects a 2 point version scheme will be used, eg v1.2, however the patch level (v1.2.3)
-will be used if either:
-* the previous tag includes it
-* patch level increment is set via commit footer or ``VERSION_INCREMENT`` env
-* the following env variable is configured: ``VERSION_SUPPORT_PATCH=1``
-
-This setting will be persisted if saved, eg ``VERSION_SUPPORT_PATCH=1 python -m __version__ --save``
-
-Project Version
----------------
-
-The overall goal is for any commit to be suitable as a potential release. As such you can build away, testing your main
-branch builds and as soon as one of them is ready to go simply run ``python -m __version__ --tag`` to have it tagged off
-with the same version number the build already had. Indeed this step can be done in CI, take at a look at this projects'
-`.gitlab-ci.yml
-<https://gitlab.com/alelec/__version__/-/blob/main/.gitlab-ci.yml>`_ for an example of a manual CI task
-to "release this commit".
-
-To use this to auto-version python packages, this projects' ``setup.py`` the following pattern can be followed: ::
-
-    setup(
-        name="git-versioner",
-        author="Andrew Leech",
-        author_email="andrew@alelec.net",
-        use_git_versioner=True,
-        setup_requires=["git-versioner"],
-        ...
-    )
-
-By default the full / long version is provided in this case in [PEP440](https://peps.python.org/pep-0440/#local-version-identifiers) local version format.
-If you want to push the package to PyPI however the short version must be used which can be specified with
-``use_git_versioner="short"``.
-
-The full python version number can also added to the description, which can be especially useful when the package is
-published with the short number. Do enable this you can use ``use_git_versioner="desc"`` in which case a line like
-``version: 1.2.3+ga1b2c3d`` will be added to the bottom of the long description metadata.
-
-When building a package, the version details can be automatically saved into ``<package>.__version__.py`` in the
-built wheel with the setting ``use_git_versioner="snapshot"``.
-
-Multiple settings can be combined, eg ``use_git_versioner="short:desc:snapshot"``.
-
-If being used in Gitlab CI for builds an automated versioning scheme can be specified with ``use_git_versioner="gitlab"``
-(and/or ``use_git_versioner="gitlab:desc"``). In this mode, builds from the default / main branch or from tags will
-use the short version, with anything else (eg. pr's, local builds) using the long version scheme.
-
-
-Runtime Access
---------------
 To access the version in your project at runtime you can either:
 
-* auto-calculate each run::
-
+*   auto-calculate each run:
+    ``` python
     from __version__ import version, version_short, git_hash, on_tag
+    ```
 
-* get the details from previous run of ``python __version__ --save``::
-
+*   get the details from previous run of `python __version__ --save`:
+    ``` python
     from _version import version, version_short, git_hash, on_tag
+    ```
 
-* In an installed package originally built with ``use_git_versioner="snapshot"``::
-
+*   In an installed package originally built with
+    `use_git_versioner="snapshot"`:
+    ``` python
     from .__version__ import version, version_short, git_hash, on_tag
+    ```
 
-Testing
--------
-The version number can be overridden with the following envirinment variables.
-If any / some of these are set, the rest will fallback to null / invalid values so
-ensure you set all the ones that may be needed. ::
-
-    GIT_VERSIONER_VERSION
-    GIT_VERSIONER_VERSION_SHORT
-    GIT_VERSIONER_GIT_HASH
-    GIT_VERSIONER_ON_TAG
-    GIT_VERSIONER_DIRTY
-    GIT_VERSIONER_VERSION_PY
-    GIT_VERSIONER_VERSION_PY_SHORT
-
-Command Line
-------------
-Can also be used as command line tool to generate ``_version.py``, print version, rename files or fill a
-template file with version details.::
-
-
-    usage: __version__.py [-h] [--save] [--short] [--git] [--rename RENAME] [--template template output]
-
-    Mange current/next version.
-
-    optional arguments:
-      -h, --help            show this help message and exit
-      --save                Store in _version.py
-      --short               Print the short version string
-      --git                 Print the release git hash
-      --rename RENAME       Add version numbers to filename(s)
-      --template template output
-                            Add version to <template> and write result to <output>
-      --tag                 Creates git tag to release the current commit
-
+## Testing
 
-version: 5.3+gf03a534
+The version number can be overridden with the following envirinment
+variables. If any / some of these are set, the rest will fallback to
+null / invalid values so ensure you set all the ones that may be needed.
+```
+GIT_VERSIONER_VERSION
+GIT_VERSIONER_VERSION_SHORT
+GIT_VERSIONER_GIT_HASH
+GIT_VERSIONER_ON_TAG
+GIT_VERSIONER_DIRTY
+GIT_VERSIONER_VERSION_PY
+GIT_VERSIONER_VERSION_PY_SHORT
+```
+## Command Line
+
+Can also be used as command line tool to generate `_version.py`, print
+version, rename files or fill a template file with version details.
+```
+usage: __version__.py [-h] [--save] [--short] [--git] [--rename RENAME] [--template template output]
+
+Mange current/next version.
+
+optional arguments:
+    -h, --help            show this help message and exit
+    --save                Store in _version.py
+    --short               Print the short version string
+    --git                 Print the release git hash
+    --rename RENAME       Add version numbers to filename(s)
+    --template template output
+                        Add version to <template> and write result to <output>
+    --tag                 Creates git tag to release the current commit
+```
```

