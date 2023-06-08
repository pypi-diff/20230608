# Comparing `tmp/git_theta-0.0.2.tar.gz` & `tmp/git_theta-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/git-theta/git-theta/dist/.tmp-635xuqjt/git_theta-0.0.2.tar", last modified: Mon Jan 30 20:40:33 2023, max compression
+gzip compressed data, was "git_theta-0.1.1.tar", last modified: Wed Jun  7 20:07:03 2023, max compression
```

## Comparing `git_theta-0.0.2.tar` & `git_theta-0.1.1.tar`

### file list

```diff
@@ -1,53 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:40:33.000000 git_theta-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-30 20:40:24.000000 git_theta-0.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-01-30 20:40:33.000000 git_theta-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-01-30 20:40:24.000000 git_theta-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:40:33.000000 git_theta-0.0.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5728 2023-01-30 20:40:24.000000 git_theta-0.0.2/bin/git-theta
--rwxr-xr-x   0 runner    (1001) docker     (123)     6064 2023-01-30 20:40:24.000000 git_theta-0.0.2/bin/git-theta-filter
--rwxr-xr-x   0 runner    (1001) docker     (123)    12589 2023-01-30 20:40:24.000000 git_theta-0.0.2/bin/git-theta-merge
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:40:33.000000 git_theta-0.0.2/git_theta/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/async_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:40:33.000000 git_theta-0.0.2/git_theta/checkpoints/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/checkpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/checkpoints/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/checkpoints/flax_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/checkpoints/pickled_dict_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/checkpoints/tensorflow_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/git_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:40:33.000000 git_theta-0.0.2/git_theta/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      303 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/hooks/post-commit
--rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/hooks/pre-push
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:40:33.000000 git_theta-0.0.2/git_theta/lsh/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/lsh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/lsh/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/lsh/euclidean_lsh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/lsh/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/lsh/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:40:33.000000 git_theta-0.0.2/git_theta/merges/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/merges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/merges/average.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/merges/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/merges/take.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:40:33.000000 git_theta-0.0.2/git_theta/updates/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/updates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/updates/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/updates/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/updates/low_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/updates/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-01-30 20:40:24.000000 git_theta-0.0.2/git_theta/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:40:33.000000 git_theta-0.0.2/git_theta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-01-30 20:40:33.000000 git_theta-0.0.2/git_theta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-01-30 20:40:33.000000 git_theta-0.0.2/git_theta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 20:40:33.000000 git_theta-0.0.2/git_theta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-01-30 20:40:33.000000 git_theta-0.0.2/git_theta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-30 20:40:33.000000 git_theta-0.0.2/git_theta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-30 20:40:33.000000 git_theta-0.0.2/git_theta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-30 20:40:24.000000 git_theta-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 20:40:33.000000 git_theta-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-01-30 20:40:24.000000 git_theta-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:07:03.649758 git_theta-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 20:06:44.000000 git_theta-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    23312 2023-06-07 20:07:03.649758 git_theta-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-06-07 20:06:44.000000 git_theta-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:07:03.641758 git_theta-0.1.1/git_theta/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:07:03.645758 git_theta-0.1.1/git_theta/checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/checkpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/checkpoints/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/checkpoints/flax_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/checkpoints/pickled_dict_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/checkpoints/tensorflow_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/git_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:07:03.645758 git_theta-0.1.1/git_theta/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      303 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/hooks/post-commit
+-rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/hooks/pre-push
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:07:03.645758 git_theta-0.1.1/git_theta/lsh/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/lsh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/lsh/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/lsh/euclidean_lsh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/lsh/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/lsh/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:07:03.649758 git_theta-0.1.1/git_theta/merges/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/merges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/merges/average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/merges/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/merges/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/merges/take.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:07:03.649758 git_theta-0.1.1/git_theta/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6577 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/scripts/git_theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/scripts/git_theta_diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7858 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/scripts/git_theta_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15207 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/scripts/git_theta_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:07:03.649758 git_theta-0.1.1/git_theta/updates/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/updates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/updates/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/updates/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/updates/ia3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/updates/low_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/updates/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-07 20:06:44.000000 git_theta-0.1.1/git_theta/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:07:03.645758 git_theta-0.1.1/git_theta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23312 2023-06-07 20:07:03.000000 git_theta-0.1.1/git_theta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-07 20:07:03.000000 git_theta-0.1.1/git_theta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:07:03.000000 git_theta-0.1.1/git_theta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-07 20:07:03.000000 git_theta-0.1.1/git_theta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-07 20:07:03.000000 git_theta-0.1.1/git_theta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 20:07:03.000000 git_theta-0.1.1/git_theta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-07 20:06:44.000000 git_theta-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:07:03.649758 git_theta-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-06-07 20:06:44.000000 git_theta-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `git_theta-0.0.2/LICENSE.md` & `git_theta-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `git_theta-0.0.2/bin/git-theta` & `git_theta-0.1.1/git_theta/scripts/git_theta.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-#!/usr/bin/env python
+"""Installation and .git manipulation scripts."""
 
 import argparse
-import sys
-import git
+import fnmatch
 import logging
 import re
-import fnmatch
+import sys
+
+import git
+
+if sys.version_info < (3, 10):
+    from importlib_metadata import entry_points
+else:
+    from importlib.metadata import entry_points
 
-from git_theta import git_utils, utils, theta, metadata, async_utils
+from git_theta import async_utils, git_utils, metadata, theta, utils
 
 logging.basicConfig(
     level=logging.DEBUG,
     format="git-theta: [%(asctime)s] [%(funcName)s] %(levelname)s - %(message)s",
 )
 
 
@@ -49,19 +55,21 @@
     )
     track_parser.add_argument(
         "file", help="model checkpoint file or file pattern to track"
     )
     track_parser.set_defaults(func=track)
 
     add_parser = subparsers.add_parser("add", help="add command used to stage files.")
+    add_parser.add_argument("file", help="The file we are git adding.")
     add_parser.add_argument(
         "--update-type",
-        choices=["dense", "sparse", "low-rank"],
+        choices=[e.name for e in entry_points(group="git_theta.plugins.updates")],
         help="Type of update being applied",
     )
+    add_parser.add_argument("--update-data", help="Where update data is stored.")
     add_parser.set_defaults(func=add)
 
     args = parser.parse_known_args()
     return args
 
 
 def post_commit(args):
@@ -123,14 +131,15 @@
         git.config.get_config_path("global"), config_level="global", read_only=False
     )
     config_writer.set_value('filter "theta"', "clean", "git-theta-filter clean %f")
     config_writer.set_value('filter "theta"', "smudge", "git-theta-filter smudge %f")
     config_writer.set_value('filter "theta"', "required", "true")
     config_writer.set_value('merge "theta"', "name", "Merge Models with Git-Theta")
     config_writer.set_value('merge "theta"', "driver", "git-theta-merge %O %A %B %P")
+    config_writer.set_value('diff "theta"', "command", "git-theta-diff")
     config_writer.release()
 
 
 def track(args):
     """
     Track a particular model checkpoint file with git-theta
     """
@@ -144,20 +153,32 @@
 
     git_utils.write_gitattributes(gitattributes_file, new_gitattributes)
     git_utils.add_file(gitattributes_file, repo)
 
 
 def add(args, unparsed_args):
     repo = git_utils.get_git_repo()
-    env_vars = {utils.EnvVarConstants.UPDATE_TYPE: args.update_type}
+    env_vars = {
+        "GIT_THETA_UPDATE_TYPE": args.update_type,
+        "GIT_THETA_UPDATE_DATA_PATH": args.update_data,
+    }
+    # The most common use for `git theta add` is when you have side-loaded
+    # information and thus the main checkpoint file has not been modified. This
+    # results in git not running the add command as the modification time has
+    # not changed. We touch the file so it will actually get added.
+    utils.touch(args.file)
     with repo.git.custom_environment(**env_vars):
-        repo.git.add(*unparsed_args)
+        repo.git.add(args.file, *unparsed_args)
 
 
-if __name__ == "__main__":
+def main():
     args, unparsed_args = parse_args()
     if not args.func == install:
         git_utils.set_hooks()
     if args.func == add:
         args.func(args, unparsed_args)
     else:
         args.func(args)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `git_theta-0.0.2/bin/git-theta-filter` & `git_theta-0.1.1/git_theta/scripts/git_theta_filter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,178 +1,209 @@
-#!/usr/bin/env python
+"""Clean and Smudge filters for version controlling machine learning models."""
 
 import argparse
-import sys
 import logging
+import os
+import sys
+import tempfile
+
+import git
 import numpy as np
 
 from git_theta import (
-    git_utils,
+    async_utils,
     checkpoints,
-    params,
+    git_utils,
+    lsh,
     metadata,
+    params,
     updates,
-    async_utils,
-    lsh,
 )
 from git_theta.utils import EnvVarConstants
 
-
 logging.basicConfig(
     level=logging.DEBUG,
     # Log to a file for clean/smudge as they don't appear on the console when called via git.
-    filename="/tmp/git-theta.log",
+    filename=os.path.join(tempfile.gettempdir(), "git-theta.log"),
     format="git-theta-filter: [%(asctime)s] [%(funcName)s] %(levelname)s - %(message)s",
 )
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="git-theta filter program")
     subparsers = parser.add_subparsers(title="Commands", dest="command")
     subparsers.required = True
 
     clean_parser = subparsers.add_parser("clean", help="clean filter")
     clean_parser.add_argument("file", help="file being passed to clean filter")
-    clean_parser.set_defaults(func=clean)
+    clean_parser.set_defaults(func=run_clean)
 
     smudge_parser = subparsers.add_parser("smudge", help="smudge filter")
     smudge_parser.add_argument("file", help="file being passed to smudge filter")
-    smudge_parser.set_defaults(func=smudge)
+    smudge_parser.set_defaults(func=run_smudge)
 
     args = parser.parse_args()
     return args
 
 
-def clean(args):
-    """
-    Implements clean filter for model files
-    Metadata file looks as follows:
-    {
-    "model/scoping/to/param/1-weight": {
-        "tensor_metadata": {
-            "shape": List[str],
-            "dtype": str,
-            "hash": str,
-        },
-    },
-    ...,
-    "model/scoping/to/param/2-bias": {
-        "tensor_metadata": {
-            "shape": List[str],
-            "dtype": str,
-            "hash": str,
-        },
-    },
-    ...,
-    }
-    """
-    logging.debug(f"Running clean filter on {args.file}")
-    repo = git_utils.get_git_repo()
-    checkpoint_handler = checkpoints.get_checkpoint_handler()
-    model_checkpoint = checkpoint_handler.from_file(sys.stdin.buffer)
-
-    # Note: If the update serializer is configurable per-parameter, it will need to be created inside _clean
+# TODO: Move to a `filters.py` file.
+def clean(
+    checkpoint: checkpoints.Checkpoint, repo: git.Repo, path: str
+) -> metadata.Metadata:
+    """Convert a `Checkpoint` to cleaned `Metadata`."""
+    # Note: If the update serializer is configurable per-parameter, it will
+    # need to be created inside _clean
     update_serializer = params.get_update_serializer()
-    prev_metadata = metadata.Metadata.from_commit(repo, args.file, "HEAD").flatten()
+    # Create an update handler based on user input.
+    update_handler = updates.get_update_handler()(
+        update_serializer, EnvVarConstants.UPDATE_DATA_PATH
+    )
+    prev_metadata = metadata.Metadata.from_commit(repo, path, "HEAD").flatten()
 
     async def _clean(param_keys, new_param):
         logging.debug(f"Cleaning {'/'.join(param_keys)}")
+        # Get the metadata from the previous version of the parameter
         param_metadata = prev_metadata.get(param_keys)
+        # Create new metadata from the current value
         new_tensor_metadata = metadata.TensorMetadata.from_tensor(new_param)
 
         # If the parameter tensor has not changed, just keep the metadata the same
+        # TODO: Encapsulate this parameter check within an equality check.
         if (
             param_metadata
             and param_metadata.tensor_metadata.shape == new_tensor_metadata.shape
             and param_metadata.tensor_metadata.dtype == new_tensor_metadata.dtype
+            # A parameter with a side-loaded update will not have changed in the
+            # normal checkpoint, so ask the updater if it will be updated with
+            # side-loaded information.
+            and not update_handler.will_update(param_keys)
         ):
+            # Compare the parameters using the LSH
             hasher = lsh.get_lsh()
+            # TODO: Is is possible to make this comparison async?
             hash_distance = hasher.distance(
                 param_metadata.tensor_metadata.hash, new_tensor_metadata.hash
             )
-            # If hash_distance < PARAMETER_ATOL, assume the tensors pass np.allclose and parameter hasn't changed
+            # If hash_distance < PARAMETER_ATOL, assume the tensors pass
+            # np.allclose and parameter hasn't changed
             if hash_distance < EnvVarConstants.PARAMETER_ATOL:
                 return param_keys, param_metadata
-            # If PARAMETER_ATOL < hash_distance < LSH_THRESHOLD, load parameters and check if parameter has changed with np.allclose
+            # If PARAMETER_ATOL < hash_distance < LSH_THRESHOLD, load parameters
+            # and check if parameter has changed with np.allclose
             elif hash_distance < EnvVarConstants.LSH_THRESHOLD:
-                update_handler = updates.get_update_handler(
+                # Load the previous parameter using the specific update handler
+                # for that parameter.
+                param_update_handler = updates.get_update_handler(
                     param_metadata.theta_metadata.update_type
                 )(update_serializer)
-                param = await update_handler.apply(
-                    param_metadata, param_keys, repo=repo, path=args.file
+                param = await param_update_handler.apply(
+                    param_metadata, param_keys, repo=repo, path=path
                 )
                 if np.allclose(
                     param,
                     new_param,
                     rtol=EnvVarConstants.PARAMETER_RTOL,
                     atol=EnvVarConstants.PARAMETER_ATOL,
                 ):
                     return param_keys, param_metadata
 
-        update_handler = updates.get_update_handler()(update_serializer)
+        # Create git-theta metadata for the new parameter.
         new_theta_metadata = metadata.ThetaMetadata(
             update_type=update_handler.name, last_commit=git_utils.get_head(repo)
         )
-        lfs_metadata = await update_handler.write(
+        # Write the new parameter into git-lfs
+        lfs_metadata, param_hash = await update_handler.write(
             new_param,
             param_keys,
             prev_metadata=param_metadata,
             repo=repo,
-            path=args.file,
+            path=path,
         )
-
+        # If we are an IncrementalUpdate, we need to re-calculate the hash
+        # so it is based on the updated value, not the old one.
+        if param_hash is not None:
+            new_tensor_metadata.hash = param_hash
+        # Combine metadata into single paramtere metadata blob
         new_param_metadata = metadata.ParamMetadata(
             lfs_metadata=lfs_metadata,
             tensor_metadata=new_tensor_metadata,
             theta_metadata=new_theta_metadata,
         )
         return param_keys, new_param_metadata
 
     # Sort the keys so we don't get changing diffs based on serialization order.
-    sorted_checkpoint = dict(sorted(model_checkpoint.flatten().items()))
-    new_metadata = metadata.Metadata(
+    sorted_checkpoint = dict(sorted(checkpoint.flatten().items()))
+    return metadata.Metadata(
         **async_utils.run(
             async_utils.run_map(
                 sorted_checkpoint,
                 _clean,
                 max_concurrency=EnvVarConstants.MAX_CONCURRENCY,
             )
         )
-    )
+    ).unflatten()
 
-    new_metadata.unflatten().write(sys.stdout)
 
-
-def smudge(args):
+def run_clean(args):
     """
-    Implements smudge filter for model files
+    Implements clean filter for model files
     """
-    logging.debug(f"Running smudge filter on {args.file}")
-
+    logging.debug(f"Running clean filter on {args.file}")
     repo = git_utils.get_git_repo()
-    curr_metadata = metadata.Metadata.from_file(sys.stdin).flatten()
+    checkpoint_handler = checkpoints.get_checkpoint_handler()
+    model_checkpoint = checkpoint_handler.from_file(sys.stdin.buffer)
+    new_metadata = clean(model_checkpoint, repo, args.file)
+    new_metadata.write(sys.stdout)
+    # If we had side-loaded information, write it out so we don't get false
+    # positives for `git status`
+    if EnvVarConstants.UPDATE_DATA_PATH:
+        smudge(new_metadata, repo, args.file)
+
+
+# TODO: Now that we have this as a separate function, us it (instead of
+# `subprocess.run`) in the manual merge escape hatch.
+def smudge(
+    cleaned_metadata: metadata.Metadata, repo: git.Repo, path: str
+) -> checkpoints.Checkpoint:
+    """Convert cleaned `Metadata` to a `Checkpoint`."""
+    curr_metadata = cleaned_metadata.flatten()
 
     async def _smudge(param_keys, param_metadata):
         logging.debug(f"Smudging {'/'.join(param_keys)}")
         update_handler = updates.get_update_handler(
             param_metadata.theta_metadata.update_type
         )(params.get_update_serializer())
         param_value = await update_handler.apply(
-            param_metadata, param_keys, repo=repo, path=args.file
+            param_metadata, param_keys, repo=repo, path=path
         )
         return param_keys, param_value
 
     model_dict = async_utils.run(
         async_utils.run_map(
             curr_metadata, _smudge, max_concurrency=EnvVarConstants.MAX_CONCURRENCY
         )
     )
 
     checkpoint_handler = checkpoints.get_checkpoint_handler()
-    model_checkpoint = checkpoint_handler(model_dict).unflatten()
+    return checkpoint_handler(model_dict).unflatten()
+
+
+def run_smudge(args):
+    """
+    Implements smudge filter for model files
+    """
+    logging.debug(f"Running smudge filter on {args.file}")
+
+    repo = git_utils.get_git_repo()
+    curr_metadata = metadata.Metadata.from_file(sys.stdin)
+    model_checkpoint = smudge(curr_metadata, repo, args.file)
     model_checkpoint.save(sys.stdout.buffer)
 
 
-if __name__ == "__main__":
+def main():
     args = parse_args()
     git_utils.set_hooks()
     args.func(args)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `git_theta-0.0.2/bin/git-theta-merge` & `git_theta-0.1.1/git_theta/scripts/git_theta_merge.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-#!/usr/bin/env python
-
+"""Custom git-theta merge tool."""
 
 import argparse
+import asyncio
+import functools
 import itertools
 import logging
+import os
 import sys
-import functools
-from typing import Optional, Dict, Any, List, FrozenSet, Union
-from prompt_toolkit import PromptSession, print_formatted_text
-from prompt_toolkit.formatted_text import HTML
-from prompt_toolkit.validation import Validator, ValidationError
+import tempfile
+from typing import Any, Dict, FrozenSet, List, Optional, Union
+
+from prompt_toolkit import PromptSession, print_formatted_text, prompt
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
-from git_theta import metadata
-from git_theta import merges
-from git_theta.utils import DiffState, Trie, TEXT_STYLE
+from prompt_toolkit.formatted_text import HTML
+from prompt_toolkit.validation import ValidationError, Validator
 
+from git_theta import async_utils, merges, metadata
+from git_theta.utils import TEXT_STYLE, DiffState, EnvVarConstants, NoResult, Trie
 
 logging.basicConfig(
     level=logging.DEBUG,
     # Log to a file for clean/smudge as they don't appear on the console when called via git.
-    filename="/tmp/git-theta.log",
+    filename=os.path.join(tempfile.gettempdir(), "git-theta.log"),
     format="git-theta-merge: [%(asctime)s] %(levelname)s - %(message)s",
 )
 
 
 def infer_state(
     ancestor: Optional[metadata.ParamMetadata],
     current: Optional[metadata.ParamMetadata],
@@ -167,14 +169,47 @@
     for kb, action in actions.items():
         menu.append(f"{kb:>{longest_kb}})  {action}")
     # Add a small indent to each action.
     menu = [f"{'':>{indent}}{m}" for m in menu]
     return menu
 
 
+def manual_merge(args):
+    logging.info(f"Writing model weights from {args.path} for manual merging.")
+
+    # TODO: Update smudge API to make it easier to call programatically.
+    async def load(name, path):
+        with open(path, "rb") as f:
+            raw_weights = (
+                await async_utils.subprocess_run(
+                    ["git-theta-filter", "smudge", args.path],
+                    f.read(),
+                    capture_output=True,
+                )
+            ).stdout
+        return name, raw_weights
+
+    checkpoints = {
+        "ours": args.current,
+        "theirs": args.other,
+        "ancestor": args.ancestor,
+    }
+
+    checkpoints = async_utils.run(async_utils.run_map(checkpoints, load))
+    for name, raw_weights in checkpoints.items():
+        with open(f"{name}.ckpt", "wb") as wf:
+            logging.info(f"Saving {name} model to {name}.ckpt")
+            wf.write(raw_weights)
+    logging.info(
+        "Manual Merging: Combine checkpoints as you wish, save the "
+        f"result to {args.path} and continue the merge."
+    )
+    sys.exit(1)
+
+
 def merge(args):
     """git-theta checkpoint aware merging."""
     print_formatted_text(
         HTML(f"<b>Fixing Merge Conflicts in {TEXT_STYLE.format_model(args.path)}</b>")
     )
     logging.debug(f"Running merge driver on {args.path}")
     # Load the `cleaned` metadata file for the ancestor commit.
@@ -182,23 +217,27 @@
     ancestor = ancestor.flatten()
     # Load the `cleaned` metadata file for commit on our branch.
     current = metadata.Metadata.from_file(args.current)
     current = current.flatten()
     # Load the `cleaned` metadata file for commit on the other branch.
     other = metadata.Metadata.from_file(args.other)
     other = other.flatten()
+
     # Collect the list of all parameter names. NB: Names are collected from all
     # models as they may have been deleted/added on different branches.
     all_params = sorted(
         list(set(itertools.chain(ancestor.keys(), current.keys(), other.keys())))
     )
     # Load all merge handlers and assign each one a kb shortcut.
     handlers = merges.all_merge_handlers()
     short_cuts = make_short_cuts(handlers)
 
+    # Trigger the context merge for summary of branches.
+    handlers["context"]().merge()
+
     # A place to aggregate metadata for the merged model.
     merged_model = {}
     # A place to store loaded parameters to enable reuse/caching. Currently
     # modified in-place :(
     partial_current = {}
     partial_other = {}
     partial_ancestor = {}
@@ -254,68 +293,100 @@
         # An info box at the bottom of the cli, helps remind users of the context
         # they are working on.
         context = HTML(
             f'Merging parameter: <b><style bg="{TEXT_STYLE.param}">{name}</style></b>'
             f' in model <i><style bg="{TEXT_STYLE.model}">{args.path}</style></i>'
         )
 
-        # User action selection.
-        action = session.prompt(
-            # Show the menu
-            text,
-            # Show the merge context
-            bottom_toolbar=context,
-            # Validate that their input is either a valid action or is the
-            # prefix of a valid action. This lets us alert early if their input
-            # is not in the autocomplete menu.
-            validator=CommandValidator(available_actions, available_prefixes),
-            # Suggest completions they have used before, accept with ->
-            auto_suggest=FilteredAutoSuggestFromHistory(
-                valid_suggestions=available_actions
-            ),
-            # Give them a list of autocomplete actions based on the valid actions.
-            completer=WordCompleter(available_actions),
-            # Pop up the completion list as they type.
-            complete_while_typing=True,
-        )
-        action = action.strip()
-        logging.debug(f"User Input: {action}")
-        if action == "q":
-            logging.debug("User quit the merge tool. Leaving merge files as they are.")
-            sys.exit(1)
-        # Dispatch based on action
-        # TODO: When should these objects be initialized?
-        # TODO: How should we configure these actions?
-        # TODO: Move to a verb object compositional approach?
-        # TODO: Move to async for actions?
-        merged_parameter = available_actions[action]()(
-            param_name,
-            current_param,
-            other_param,
-            ancestor_param,
-            current,
-            other,
-            ancestor,
-            # TODO: Update API so these don't need to be in-place updates?
-            partial_current,
-            partial_other,
-            partial_ancestor,
-            # The path to where the model actually lives.
-            args.path,
-        )
+        merged_parameter = NoResult
+        while merged_parameter is NoResult:
+            # User action selection.
+            action = session.prompt(
+                # Show the menu
+                text,
+                # Show the merge context
+                bottom_toolbar=context,
+                # Validate that their input is either a valid action or is the
+                # prefix of a valid action. This lets us alert early if their input
+                # is not in the autocomplete menu.
+                validator=CommandValidator(available_actions, available_prefixes),
+                # Suggest completions they have used before, accept with ->
+                auto_suggest=FilteredAutoSuggestFromHistory(
+                    valid_suggestions=available_actions
+                ),
+                # Give them a list of autocomplete actions based on the valid actions.
+                completer=WordCompleter(available_actions),
+                # Pop up the completion list as they type.
+                complete_while_typing=True,
+            )
+            action = action.strip()
+            logging.debug(f"User Input: {action}")
+            if action == "q":
+                logging.debug(
+                    "User quit the merge tool. Leaving merge files as they are."
+                )
+                sys.exit(1)
+
+            # Collect any arguments that the merge action requires.
+            action_arguments = {}
+            for merge_argument in available_actions[action].merge_arguments():
+                param_text = HTML(
+                    "\n".join(
+                        [
+                            merge_argument.description,
+                            f"<b>{TEXT_STYLE.format_argument(merge_argument.name)}</b>: ",
+                        ]
+                    )
+                )
+                validator = Validator.from_callable(merge_argument.validator)
+                argument_value = prompt(param_text, validator=validator)
+                # TODO: Add backend validation of the argument value
+                action_arguments[merge_argument.name] = merge_argument.type(
+                    argument_value
+                )
+
+            # Dispatch based on action
+            # TODO: When should these objects be initialized?
+            # TODO: How should we configure these actions?
+            # TODO: Move to a verb object compositional approach?
+            # TODO: Move to async for actions?
+            merged_parameter = available_actions[action]()(
+                param_name,
+                current_param,
+                other_param,
+                ancestor_param,
+                current,
+                other,
+                ancestor,
+                # TODO: Update API so these don't need to be in-place updates?
+                partial_current,
+                partial_other,
+                partial_ancestor,
+                # The path to where the model actually lives.
+                args.path,
+                # Merge action-specific parameters
+                **action_arguments,
+            )
         # Some of the actions result in deleting a parameter (it has a value of
         # None) so if we see that, don't add this parameter name to the merged
         # model.
         if merged_parameter is None:
             continue
         merged_model[param_name] = merged_parameter
 
     merged_model = metadata.Metadata(**merged_model).unflatten()
     # Save merged_model to args.current %A
     merged_model.write(args.current)
     # Exit with 0 to signal the merge was good.
     return 0
 
 
-if __name__ == "__main__":
+def main():
     args = parse_args()
-    merge(args)
+    if EnvVarConstants.MANUAL_MERGE:
+        manual_merge(args)
+    else:
+        merge(args)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `git_theta-0.0.2/git_theta/async_utils.py` & `git_theta-0.1.1/git_theta/async_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 """Utilities for running I/O-bound operations asyncronously."""
 
 import asyncio
 import dataclasses
 import functools
 import sys
-from typing import (
-    Any,
-    Dict,
-    Tuple,
-    TypeVar,
-    Awaitable,
-    Union,
-    Optional,
-    Sequence,
-)
+from typing import Any, Awaitable, Dict, Optional, Sequence, Tuple, TypeVar, Union
+
 import six
 
 if sys.version_info >= (3, 8):
     from typing import Protocol
 else:
     from typing_extensions import Protocol
 
 
 def run(*args, **kwargs):
     """Run an awaitable to completion, dispatch based on python version."""
-    # TODO(bdlester): Remove if we bump to python 3.7
-    if sys.version_info < (3, 7):
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(*args, **kwargs)
+    if sys.version_info < (3, 8):
+        if sys.platform in ("win32", "cygwin"):
+            asyncio.set_event_loop_policy(asyncio.WindowsProactorEventLoopPolicy())
     return asyncio.run(*args, **kwargs)
 
 
 # A type variable to indicate that the keys of the dict will not change.
 K = TypeVar("K")
 # A type variable to indicate that the async task is called with K, V tuples.
 V = TypeVar("V")
```

### Comparing `git_theta-0.0.2/git_theta/checkpoints/base.py` & `git_theta-0.1.1/git_theta/checkpoints/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """Base class and utilities for different checkpoint format backends."""
 
-from abc import ABCMeta, abstractmethod
 import os
 import sys
+from abc import ABCMeta, abstractmethod
 from typing import Optional
+
 import numpy as np
 
 if sys.version_info < (3, 10):
     from importlib_metadata import entry_points
 else:
     from importlib.metadata import entry_points
 
 from git_theta import utils
 
 
+@utils.abstract_classattributes("name")
 class Checkpoint(dict, metaclass=ABCMeta):
     """Abstract base class for wrapping checkpoint formats."""
 
-    @property
-    @abstractmethod
-    def name(self):
-        """The name of this checkpoint handler, can be used to lookup the plugin."""
+    name: str = NotImplemented  # The name of this checkpoint handler, can be used to lookup the plugin.
 
     @classmethod
     def from_file(cls, checkpoint_path):
         """Create a new Checkpoint object.
 
         Parameters
         ----------
@@ -62,14 +61,50 @@
 
     def flatten(self):
         return utils.flatten(self, is_leaf=lambda v: isinstance(v, np.ndarray))
 
     def unflatten(self):
         return utils.unflatten(self)
 
+    @classmethod
+    def diff(cls, m1: "Checkpoint", m2: "Checkpoint") -> "Checkpoint":
+        """Compute the diff between two checkpoints.
+
+        Parameters
+        ----------
+        m1 : Checkpoint
+            The new checkpoint
+        m2 : Checkpoint
+            The old checkpoint
+
+        Returns
+        -------
+        added : Checkpoint
+            Checkpoint containing the parameter groups added to m1
+        removed : Checkpoint
+            Checkpoint containing the parameter groups removed from m2
+        modified : Checkpoint
+            Checkpoint containing the parameter groups modified between m1 and m2
+        """
+        m1_flat = m1.flatten()
+        m2_flat = m2.flatten()
+        # N.b.: This is actually faster than set operations on m1 and m2's keys
+        added = cls({k: v for k, v in m1_flat.items() if k not in m2_flat}).unflatten()
+        removed = cls(
+            {k: v for k, v in m2_flat.items() if k not in m1_flat}
+        ).unflatten()
+        modified = cls(
+            {
+                k: v
+                for k, v in m1_flat.items()
+                if k in m2_flat and not np.allclose(v, m2_flat[k])
+            }
+        ).unflatten()
+        return added, removed, modified
+
 
 def get_checkpoint_handler_name(checkpoint_type: Optional[str] = None) -> str:
     """Get the name of the checkpoint handler to use.
 
     Order of precedence is
     1. `checkpoint_type` argument
     2. `$GIT_THETA_CHECKPOINT_TYPE` environment variable
```

### Comparing `git_theta-0.0.2/git_theta/checkpoints/pickled_dict_checkpoint.py` & `git_theta-0.1.1/git_theta/checkpoints/pickled_dict_checkpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 #!/usr/bin/env python3
 
 
 import io
+
 import torch
+
 from git_theta.checkpoints import Checkpoint
 
 
 class PickledDictCheckpoint(Checkpoint):
     """Class for wrapping picked dict checkpoints, commonly used with PyTorch."""
 
+    name: str = "pickled_dict"
+
     @classmethod
     def load(cls, checkpoint_path):
         """Load a checkpoint into a dict format.
 
         Parameters
         ----------
         checkpoint_path : str or file-like object
```

### Comparing `git_theta-0.0.2/git_theta/checkpoints/tensorflow_checkpoint.py` & `git_theta-0.1.1/git_theta/checkpoints/tensorflow_checkpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """A Checkpoint backend for tensorflow models."""
 
 
 import numpy as np
 import tensorflow as tf
-from git_theta.checkpoints import Checkpoint
+
 from git_theta import utils
+from git_theta.checkpoints import Checkpoint
 
 
 class DynamicNetwork(tf.keras.Model):
     """A keras model that can dynamically build itself from a map of params for tf saving."""
 
     def __init__(self, params):
         super().__init__()
@@ -22,20 +23,17 @@
             # Save the variable (or sub-model) to an attribute so it will get tracked.
             self.__setattr__(name, param)
 
 
 class TensorFlowCheckpoint(Checkpoint):
     """Process a TensorFlow checkpoint via `tf.keras.Model.save_weights`. (no computation graph included)."""
 
+    name: str = "tensorflow-checkpoint"
     VALUE_STRING = ".ATTRIBUTES/VARIABLE_VALUE"
 
-    @property
-    def name(self):
-        return "tensorflow-checkpoint"
-
     @staticmethod
     def is_parameter(param_name: str) -> bool:
         return param_name.endswith(TensorFlowCheckpoint.VALUE_STRING)
 
     @staticmethod
     def normalize_name(param_name: str) -> str:
         param_name = utils.remove_suffix(param_name, TensorFlowCheckpoint.VALUE_STRING)
@@ -58,17 +56,15 @@
         model.save_weights(checkpoint_path)
 
 
 # TODO
 class TensorFlowSavedModel(Checkpoint):
     """Process a TensorFlow SavedModel (computation graph included)."""
 
-    @property
-    def name(self):
-        return "tensorflow-savedmodel"
+    name: str = "tensorflow-savedmodel"
 
     @classmethod
     def load(cls, checkpoint_path: str):
         raise ValueError("Sorry, SavedModel support is a work in progress.")
 
     def save(self, checkpoint_path: str):
         raise ValueError("Sorry, SavedModel support is a work in progress.")
```

### Comparing `git_theta-0.0.2/git_theta/git_utils.py` & `git_theta-0.1.1/git_theta/git_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Utilities for manipulating git."""
 
+import filecmp
 import fnmatch
-import git
-import os
+import io
 import json
 import logging
-import io
+import os
 import re
-from typing import List, Union, Sequence
-import subprocess
 import shutil
-import filecmp
+import subprocess
 import sys
+from typing import List, Sequence, Union
+
+import git
 
 # TODO(bdlester): importlib.resources doesn't have the `.files` API until python
 # version `3.9` so use the backport even if using a python version that has
 # `importlib.resources`.
 if sys.version_info < (3, 9):
     import importlib_resources
 else:
@@ -172,19 +173,21 @@
             # to that.
             if fnmatch.fnmatchcase(path, match.group("pattern")):
                 pattern_found = True
                 if not "filter=theta" in match.group("attributes"):
                     line = f"{line.rstrip()} filter=theta"
                 if not "merge=theta" in match.group("attributes"):
                     line = f"{line.rstrip()} merge=theta"
+                if not "diff=theta" in match.group("attributes"):
+                    line = f"{line.rstrip()} diff=theta"
         new_gitattributes.append(line)
     # If we don't find a matching pattern, add a new line that covers just this
     # specific file.
     if not pattern_found:
-        new_gitattributes.append(f"{path} filter=theta merge=theta")
+        new_gitattributes.append(f"{path} filter=theta merge=theta diff=theta")
     return new_gitattributes
 
 
 def get_gitattributes_tracked_patterns(gitattributes_file):
     gitattributes = read_gitattributes(gitattributes_file)
     theta_attributes = [
         attribute for attribute in gitattributes if "filter=theta" in attribute
```

### Comparing `git_theta-0.0.2/git_theta/lsh/base.py` & `git_theta-0.1.1/git_theta/lsh/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Base class for computing locality-sensitive hashes"""
 
 import abc
-from git_theta.lsh import RandomnessPool
-from git_theta.lsh.types import Signature, Parameter
+
+from git_theta.lsh.pool import RandomnessPool
+from git_theta.lsh.types import Parameter, Signature
 
 
 class HashFamily(metaclass=abc.ABCMeta):
     def __init__(self, signature_size: int):
         self._signature_size = signature_size
         self.pool = RandomnessPool(signature_size)
```

### Comparing `git_theta-0.0.2/git_theta/lsh/euclidean_lsh.py` & `git_theta-0.1.1/git_theta/lsh/euclidean_lsh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Classes for computing Euclidean locality-sensitive hashes"""
 
-import numpy as np
-import numba as nb
 import os
 
-from git_theta.lsh import HashFamily, RandomnessPool
-from git_theta.lsh.types import Signature, Parameter
+import numba as nb
+import numpy as np
+
+from git_theta.lsh import HashFamily
+from git_theta.lsh.pool import RandomnessPool
+from git_theta.lsh.types import Parameter, Signature
 from git_theta.utils import EnvVarConstants
 
 
 class EuclideanLSH(HashFamily):
     """
     Class for performing the Euclidean l2 LSH (E2LSH) algorithm described in https://www.cs.princeton.edu/courses/archive/spring05/cos598E/bib/p253-datar.pdf
     with a pre-computed randomness pool as described in Section 3 of http://personal.denison.edu/~lalla/papers/online-lsh.pdf
```

### Comparing `git_theta-0.0.2/git_theta/lsh/pool.py` & `git_theta-0.1.1/git_theta/lsh/pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Class for deterministically supplying pre-computed random values"""
 
-import numpy as np
-from numpy.random import Generator, MT19937
-import numba as nb
 import sys
 
-from git_theta.utils import EnvVarConstants
+import numba as nb
+import numpy as np
+from numpy.random import MT19937, Generator
 
+from git_theta.utils import EnvVarConstants
 
 spec = [("pool", nb.float64[:]), ("signature_offsets", nb.int64[:])]
 
 
 @nb.experimental.jitclass(spec)
 class RandomnessPool:
     def __init__(self, signature_size):
```

### Comparing `git_theta-0.0.2/git_theta/merges/average.py` & `git_theta-0.1.1/git_theta/merges/average.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """Merge parameters by averaging them."""
 
-from typing import Dict, Any, Sequence
+from typing import Any, Dict, List, Sequence
+
 import numpy as np
-from git_theta import metadata
-from git_theta.merges import Merge
-from git_theta.utils import DiffState, TEXT_STYLE
-from git_theta.types import ParamName
-from git_theta import updates
-from git_theta import params
-from git_theta import async_utils
-from git_theta import git_utils
 
+from git_theta import async_utils, git_utils, metadata, params, updates
+from git_theta.merges import Merge, MergeArgument
+from git_theta.types import ParamName
+from git_theta.utils import TEXT_STYLE, DiffState
 
 PartialModel = Dict[ParamName, Any]
 Parameter = Any
 
 
 # TODO: Add configurable interpolation parameters.
 # TODO: Control this class explosion, Average Merge can have it's own menu?
@@ -75,22 +72,35 @@
         metadataA: metadata.Metadata,
         metadataB: metadata.Metadata,
         metadataO: metadata.Metadata,
         modelA: PartialModel,
         modelB: PartialModel,
         modelO: PartialModel,
         path: str,
+        alpha: float,
     ) -> metadata.ParamMetadata:
         # Load the current parameter
         paramA = self.read_parameter(paramA, param_name, path)
         # Load the other parameter
         paramB = self.read_parameter(paramB, param_name, path)
-        result = self.average(paramA, paramB)
+        result = self.average(alpha * paramA, (1 - alpha) * paramB)
         return self.write_merged(result, param_name)
 
+    @classmethod
+    def merge_arguments(self) -> List[MergeArgument]:
+        """Returns a `MergeArgument` for the interpolation parameter"""
+        return [
+            MergeArgument(
+                name="alpha",
+                description=f"Average two parameters with <b>{TEXT_STYLE.format_argument('alpha')}*{TEXT_STYLE.format_who('our')} + (1 - {TEXT_STYLE.format_argument('alpha')})*{TEXT_STYLE.format_who('their')}</b>",
+                type=float,
+                range=(0, 1),
+            )
+        ]
+
 
 class AverageAll(Average):
     DESCRIPTION = f"Average {TEXT_STYLE.format_who('our')} change, {TEXT_STYLE.format_who('their')} change, and the {TEXT_STYLE.format_who('original')} parameter together."
     NAME = "average-all"
     SHORT_CUT = "avg-all"
     INACTIVE_STATES = frozenset(
         {
@@ -116,24 +126,46 @@
         metadataA: metadata.Metadata,
         metadataB: metadata.Metadata,
         metadataO: metadata.Metadata,
         modelA: PartialModel,
         modelB: PartialModel,
         modelO: PartialModel,
         path: str,
+        alpha1: float,
+        alpha2: float,
     ) -> metadata.ParamMetadata:
         # Load the current parameter
         paramA = self.read_parameter(paramA, param_name, path)
         # Load the other parameter
         paramB = self.read_parameter(paramB, param_name, path)
         # Load the original parameter
         paramO = self.read_parameter(paramO, param_name, path)
-        result = self.average(paramA, paramB, paramO)
+        result = self.average(
+            alpha1 * paramA, alpha2 * paramB, (1 - alpha1 - alpha2) * paramO
+        )
         return self.write_merged(result, param_name)
 
+    @classmethod
+    def merge_arguments(self) -> List[MergeArgument]:
+        """Returns a `MergeArgument` for the interpolation parameter"""
+        return [
+            MergeArgument(
+                name="alpha1",
+                description=f"Average two parameters with <b>{TEXT_STYLE.format_argument('alpha1')}*{TEXT_STYLE.format_who('our')} + {TEXT_STYLE.format_argument('alpha2')}*{TEXT_STYLE.format_who('their')} + (1 - {TEXT_STYLE.format_argument('alpha1')} - {TEXT_STYLE.format_argument('alpha2')})*{TEXT_STYLE.format_who('original')}</b>",
+                type=float,
+                range=(0, 1),
+            ),
+            MergeArgument(
+                name="alpha2",
+                description=f"Average two parameters with <b>{TEXT_STYLE.format_argument('alpha1')}*{TEXT_STYLE.format_who('our')} + {TEXT_STYLE.format_argument('alpha2')}*{TEXT_STYLE.format_who('their')} + (1 - {TEXT_STYLE.format_argument('alpha1')} - {TEXT_STYLE.format_argument('alpha2')})*{TEXT_STYLE.format_who('original')}</b>",
+                type=float,
+                range=(0, 1),
+            ),
+        ]
+
 
 class AverageOursOriginal(Average):
     DESCRIPTION = f"Average {TEXT_STYLE.format_who('our')} change and the {TEXT_STYLE.format_who('original')} parameter together."
     NAME = "average-ours-original"
     SHORT_CUT = "avg-ao"
     INACTIVE_STATES = frozenset(
         {
@@ -159,22 +191,35 @@
         metadataA: metadata.Metadata,
         metadataB: metadata.Metadata,
         metadataO: metadata.Metadata,
         modelA: PartialModel,
         modelB: PartialModel,
         modelO: PartialModel,
         path: str,
+        alpha: float,
     ) -> metadata.ParamMetadata:
         # Load the current parameter
         paramA = self.read_parameter(paramA, param_name, path)
         # Load the original parameter
         paramO = self.read_parameter(paramO, param_name, path)
-        result = self.average(paramA, paramO)
+        result = self.average(alpha * paramA, (1 - alpha) * paramO)
         return self.write_merged(result, param_name)
 
+    @classmethod
+    def merge_arguments(self) -> List[MergeArgument]:
+        """Returns a `MergeArgument` for the interpolation parameter"""
+        return [
+            MergeArgument(
+                name="alpha",
+                description=f"Average two parameters with <b>{TEXT_STYLE.format_argument('alpha')}*{TEXT_STYLE.format_who('our')} + (1 - {TEXT_STYLE.format_argument('alpha')})*{TEXT_STYLE.format_who('original')}</b>",
+                type=float,
+                range=(0, 1),
+            )
+        ]
+
 
 class AverageTheirsOriginal(Average):
     DESCRIPTION = f"Average {TEXT_STYLE.format_who('their')} change and the {TEXT_STYLE.format_who('original')} parameter together."
     NAME = "average-theirs-original"
     SHORT_CUT = "avg-to"
     INACTIVE_STATES = frozenset(
         {
@@ -200,14 +245,27 @@
         metadataA: metadata.Metadata,
         metadataB: metadata.Metadata,
         metadataO: metadata.Metadata,
         modelA: PartialModel,
         modelB: PartialModel,
         modelO: PartialModel,
         path: str,
+        alpha: float,
     ) -> metadata.ParamMetadata:
         # Load the other parameter
         paramB = self.read_parameter(paramB, param_name, path)
         # Load the original parameter
         paramO = self.read_parameter(paramO, param_name, path)
-        result = self.average(paramB, paramO)
+        result = self.average(alpha * paramB, (1 - alpha) * paramO)
         return self.write_merged(result, param_name)
+
+    @classmethod
+    def merge_arguments(self) -> List[MergeArgument]:
+        """Returns a `MergeArgument` for the interpolation parameter"""
+        return [
+            MergeArgument(
+                name="alpha",
+                description=f"Average two parameters with <b>{TEXT_STYLE.format_argument('alpha')}*{TEXT_STYLE.format_who('their')} + (1 - {TEXT_STYLE.format_argument('alpha')})*{TEXT_STYLE.format_who('original')}</b>",
+                type=float,
+                range=(0, 1),
+            )
+        ]
```

### Comparing `git_theta-0.0.2/git_theta/merges/base.py` & `git_theta-0.1.1/git_theta/merges/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,53 +3,82 @@
 Note:
   In order to dynamically create the menu of possible actions that describe what
   each plug-in does, the plugins get imported at the start of the merge tool.
   Therefore, plug-ins must not have slow side-effects that happen at import-time.
 """
 
 
-from abc import ABCMeta, abstractmethod
 import logging
 import sys
-from typing import FrozenSet, Dict, Tuple, Any
+from abc import ABCMeta, abstractmethod
+from dataclasses import dataclass
+from typing import Any, Dict, FrozenSet, List, Optional, Tuple, Type, Union
 
 if sys.version_info < (3, 10):
     from importlib_metadata import entry_points
 else:
     from importlib.metadata import entry_points
 
-from git_theta import metadata
-from git_theta import utils
-
+from git_theta import metadata, utils
 
 ParamName = Tuple[str, ...]
 Parameter = Any
 PartialModel = Dict[ParamName, Parameter]
 
 
+@dataclass
+class MergeArgument:
+    """Metadata for how to describe and validate a user-specified merge-strategy-specific argument"""
+
+    name: str
+    description: str
+    type: Type
+    range: Optional[Tuple[Union[float, int], Union[float, int]]]
+
+    @property
+    def validator(self):
+        """Returns a function checking whether a given string is a valid input for this argument"""
+
+        def is_valid(x):
+            # TODO: May need to support non-numeric types at some point
+            try:
+                x = self.type(x)
+                if self.range:
+                    return x >= self.range[0] and x <= self.range[1]
+                return False
+            except:
+                return False
+
+        return is_valid
+
+
 class PrintableABCMeta(ABCMeta):
     """Add custom `str` to /classes/, not objects."""
 
     def __str__(cls):
         return f"{cls.NAME}: {cls.DESCRIPTION}"
 
 
+@utils.abstract_classattributes("DESCRIPTION", "NAME", "SHORT_CUT", "INACTIVE_STATES")
 class Merge(metaclass=PrintableABCMeta):
     """A Plug-in that handles parameter merging.
 
     Note:
       Informational string about the plugin can contain `prompt_toolkit`
       supported HTML markup for styling and coloring text.
     """
 
-    DESCRIPTION: str = "Description of Merge Action, shown in menu."
-    NAME: str = "Unique name of the merge, to look up the plugin with."
-    SHORT_CUT: str = "A Request keyboard shortcut to use during merging."
-    # States where this action will not appear in the menu.
-    INACTIVE_STATES: FrozenSet[utils.DiffState] = frozenset()
+    DESCRIPTION: str = NotImplemented  # Description of Merge Action, shown in menu.
+    NAME: str = NotImplemented  # Unique name of the merge, to look up the plugin with.
+    SHORT_CUT: str = (
+        NotImplemented  # A Request keyboard shortcut to use during merging.
+    )
+    INACTIVE_STATES: FrozenSet[
+        utils.DiffState
+    ] = frozenset()  # States where this action will not appear in the menu.
 
     def __call__(self, param_name, *args, **kwargs):
         logging.info(f"Running {self.NAME} merge on parameter {'/'.join(param_name,)}")
         return self.merge(param_name, *args, **kwargs)
 
     @abstractmethod
     def merge(
@@ -61,19 +90,20 @@
         metadataA: metadata.Metadata,
         metadataB: metadata.Metadata,
         metadataO: metadata.Metadata,
         modelA: PartialModel,
         modelB: PartialModel,
         modelO: PartialModel,
         path: str,
+        **kwargs,
     ) -> metadata.ParamMetadata:
         """Merge parameters parameters.
 
-        Arguments
-        ---------
+        Parameters
+        ----------
             param_name: The name of the parameter we are looking at.
             paramA: The parameter metadata from branch A (current).
             paramB: The parameter metadata from branch B (other).
             paramO: The parameter metadata from the ancestor.
             metadataA: The full model metadata from branch A (current).
             metadataB: The full model metadata from branch B (other).
             metadataO: The full model metadata from the ancestor.
@@ -83,15 +113,26 @@
             modelB: A partially filled in model of real parameter values from
                 branch B (other). Allows caching and reuse for any sort of
                 "full model" merging method.
             modelO: A partially filled in model of real parameter values from
                 the ancestor. Allows caching and reuse for any sort of
                 "full model" merging method.
             path: The path to where the model actually lives.
+            kwargs: Merge-strategy-specific arguments.
+        """
+
+    @classmethod
+    def merge_arguments(self) -> List[MergeArgument]:
+        """Returns a list of `MergeArgument`s that provide information about the arguments specific to each merge strategy
+        Each `MergeArgument` contains:
+            1. The name of the merge argument
+            2. A text description of what the argument does
+            3. The type of the argument
         """
+        return []
 
 
 def all_merge_handlers() -> Dict[str, Merge]:
     """Enumerate and Load (import) all merge plugins."""
     discovered_plugins = entry_points(group="git_theta.plugins.merges")
     loaded_plugins = {ep.name: ep.load() for ep in discovered_plugins}
     return loaded_plugins
```

### Comparing `git_theta-0.0.2/git_theta/merges/take.py` & `git_theta-0.1.1/git_theta/merges/take.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Merge operations that select one version or another."""
 
 from git_theta import metadata
 from git_theta.merges import Merge
-from git_theta.utils import DiffState, TEXT_STYLE
 from git_theta.types import ParamName
+from git_theta.utils import TEXT_STYLE, DiffState
 
 
 class TakeUs(Merge):
     DESCRIPTION = f"Use {TEXT_STYLE.format_who('our')} change to the parameter."
     NAME = "take_us"
     SHORT_CUT = "tu"
     # If only they made a change take "us" doesn't make sense.
```

### Comparing `git_theta-0.0.2/git_theta/metadata.py` & `git_theta-0.1.1/git_theta/metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Classes representing checkpoint metadata files"""
 
 from __future__ import annotations
-import hashlib
+
 import dataclasses
-from collections import OrderedDict
-import re
+import hashlib
 import json
-from typing import ClassVar
-import numpy as np
-import git
-from typing import Union, TextIO, Dict, Tuple, Any
+import re
+from collections import OrderedDict
+from typing import Any, ClassVar, Dict, TextIO, Tuple, Union
 
-from git_theta import git_utils, utils, lsh
+import git
+import numpy as np
 from file_or_name import file_or_name
 
+from git_theta import git_utils, lsh, utils
+
 
 @dataclasses.dataclass(eq=True)
 class MetadataField:
     def serialize(self) -> Dict[str, Any]:
         return dataclasses.asdict(self, dict_factory=OrderedDict)
```

### Comparing `git_theta-0.0.2/git_theta/params.py` & `git_theta-0.1.1/git_theta/params.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Classes for serializing model updates."""
 
 from abc import ABCMeta, abstractmethod
-from collections import defaultdict
+
+import msgpack
 import tensorstore as ts
-import io
-import tarfile
-import posixpath
 
 
 class TensorSerializer(metaclass=ABCMeta):
     """Serialize/Deserialize tensors."""
 
     @abstractmethod
     async def serialize(self, tensor):
@@ -55,39 +53,20 @@
         """Combine multiple byte steams into one."""
 
     @abstractmethod
     def split(self, file):
         """Split a combined byte stream into original bytes."""
 
 
-class TarCombiner(FileCombiner):
+class MsgPackCombiner(FileCombiner):
     def combine(self, files):
-        tarred_file = io.BytesIO()
-        with tarfile.open(fileobj=tarred_file, mode="w") as archive:
-            for param_name, param_file in files.items():
-                for filename, file_bytes in param_file.items():
-                    # N.b. posixpath is used to create the "virtual path" in the tar file to each underlying parameter file
-                    # Ensures consistent reading/writing of virtual paths across platforms
-                    tarinfo = tarfile.TarInfo(posixpath.join(param_name, filename))
-                    tarinfo.size = len(file_bytes)
-                    archive.addfile(tarinfo, io.BytesIO(file_bytes))
-
-        tarred_file.seek(0)
-        return tarred_file.read()
+        return msgpack.packb(files, use_bin_type=True)
 
     def split(self, file):
-        file = io.BytesIO(file)
-        param_files = defaultdict(dict)
-        with tarfile.open(fileobj=file, mode="r") as archive:
-            for file_in_archive in archive.getnames():
-                param_name, filename = posixpath.split(file_in_archive)
-                param_files[param_name][filename] = archive.extractfile(
-                    file_in_archive
-                ).read()
-        return param_files
+        return msgpack.unpackb(file, raw=False)
 
 
 class Serializer(metaclass=ABCMeta):
     """Serialize/Deserialize parameters, even when represented with multiple tensors."""
 
     @abstractmethod
     async def serialize(self, params):
@@ -116,9 +95,10 @@
             name: await self.serializer.deserialize(serialized_param)
             for name, serialized_param in serialized_params.items()
         }
         return update_params
 
 
 def get_update_serializer():
-    # TODO: Right now this just returns a tensorstore/tar serializer but in the future we can implement other Serializers and/or support user plugins
-    return UpdateSerializer(TensorStoreSerializer(), TarCombiner())
+    # TODO: Right now this just returns a tensorstore/msgpack serializer but in
+    # the future we can implement other Serializers and/or support user plugins
+    return UpdateSerializer(TensorStoreSerializer(), MsgPackCombiner())
```

### Comparing `git_theta-0.0.2/git_theta/theta.py` & `git_theta-0.1.1/git_theta/theta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module for reading and writing to .git/theta"""
 
-import os
+import functools
 import json
-import re
 import logging
-import functools
+import os
+import re
+
 from file_or_name import file_or_name
 
 from git_theta import utils
 
 
 class CommitInfo:
     def __init__(self, oids):
```

### Comparing `git_theta-0.0.2/git_theta/updates/base.py` & `git_theta-0.1.1/git_theta/updates/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,89 @@
 """Base class for parameter update plugins."""
 
-from abc import ABCMeta, abstractmethod
 import os
 import sys
+from abc import ABCMeta, abstractmethod
 
 if sys.version_info < (3, 10):
     from importlib_metadata import entry_points
 else:
     from importlib.metadata import entry_points
 
 import logging
-from typing import Optional, Tuple
+from typing import Dict, FrozenSet, Optional, Tuple
 
 import numpy as np
 
-from git_theta import git_utils, utils, params, metadata
-
+from git_theta import checkpoints, git_utils, lsh, metadata, params, utils
+from git_theta.lsh.types import Signature
 
 Parameter = np.ndarray
 
 
+@utils.abstract_classattributes("name")
 class Update(metaclass=ABCMeta):
     """Base class for parameter update plugins."""
 
-    def __init__(self, serializer: params.Serializer):
-        self.serializer = serializer
+    name: str = NotImplemented  # The name used to lookup the plug-in.
 
-    @property
-    @abstractmethod
-    def name(self) -> str:
-        """The name used to lookup the plug-in."""
+    def __init__(self, serializer: params.Serializer, *args, **kwargs):
+        self.serializer = serializer
 
     async def read(self, param_metadata: metadata.ParamMetadata) -> Parameter:
         """Read in and deserialize a single parameter value based metadata."""
         lfs_pointer = param_metadata.lfs_metadata.lfs_pointer
         serialized_param = await git_utils.git_lfs_smudge(lfs_pointer)
         param = await self.serializer.deserialize(serialized_param)
         return param.get("parameter", param)
 
+    def will_update(self, param_keys: Tuple[str]) -> bool:
+        return False
+
     @abstractmethod
     async def write(
         self, param: Parameter, param_keys: Tuple[str], **kwargs
-    ) -> metadata.LfsMetadata:
+    ) -> Tuple[metadata.LfsMetadata, Signature]:
         """Serialize and save a parameter with git-lfs."""
 
     @abstractmethod
     async def apply(
         self, param_metadata: metadata.ParamMetadata, param_keys: Tuple[str], **kwargs
     ) -> Parameter:
         """Get the final parameter value, including fetching previous values."""
 
 
+# TODO: Fix this for inheritance so we don't need to dup "name" here.
+@utils.abstract_classattributes("name", "required_keys")
 class IncrementalUpdate(Update):
     """Base class for parameter updates that depend on the previous value."""
 
+    required_keys: FrozenSet[str] = NotImplemented  # Names for side-loaded information.
+
+    def __init__(self, serializer: params.Serializer, update_data: str = ""):
+        super().__init__(serializer)
+        self.update_information: Dict[str, np.ndarray] = None
+        self.update_names: utils.Trie = None
+        # Flatten the side-loaded information into a of string keys to arrays.
+        if update_data:
+            self.update_information = {
+                "/".join(k): v
+                for k, v in checkpoints.get_checkpoint_handler()
+                .from_file(update_data)
+                .flatten()
+                .items()
+            }
+            self.update_names = utils.Trie.from_iterable(self.update_information.keys())
+
+    def will_update(self, param_keys: Tuple[str]) -> bool:
+        if self.update_information is not None:
+            param_keys = "/".join(param_keys)
+            return self.update_names.prefix(param_keys)
+        return False
+
     async def get_previous_metadata(
         self,
         param_metadata: metadata.ParamMetadata,
         param_keys: Tuple[str],
         repo,
         path: str,
     ) -> metadata.ParamMetadata:
@@ -101,18 +127,29 @@
 
     @abstractmethod
     async def calculate_update(
         self, parameter: Parameter, previous_parameter: Parameter
     ) -> Parameter:
         """Calculate the update required to go from previous_parameter -> parameter."""
 
+    async def read_update(self, param_keys) -> Parameter:
+        return {
+            k: self.update_information["/".join(param_keys + (k,))]
+            for k in self.required_keys
+        }
+
+    @classmethod
     @abstractmethod
-    async def apply_update(self, update: Parameter, previous: Parameter) -> Parameter:
+    async def apply_update(cls, update: Parameter, previous: Parameter) -> Parameter:
         """Apply the update to the previous value to get the new value."""
 
+    @abstractmethod
+    def format_update(self, param: Parameter, *args, **kwargs) -> Parameter:
+        """A user-facing helper function to help format an update for git-theta."""
+
     async def write_update(self, update: Parameter) -> metadata.LfsMetadata:
         """Save and serialize (just) the update weights."""
         if not isinstance(update, dict):
             update = {"parameter": update}
         serialized_update = await self.serializer.serialize(update)
         lfs_pointer = await git_utils.git_lfs_clean(serialized_update)
         return metadata.LfsMetadata.from_pointer(lfs_pointer)
@@ -133,16 +170,24 @@
         **kwargs,
     ) -> metadata.LfsMetadata:
         """Serialize and save a parameter with git-lfs as a delta from the previous value."""
         logging.debug(f"Writing {self.name} update for {'/'.join(param_keys)}")
         previous_value = await self.get_previous_value(
             prev_metadata, param_keys, repo=repo, path=path
         )
-        update_value = await self.calculate_update(param, previous_value)
-        return await self.write_update(update_value)
+        if self.update_information is not None and self.will_update(param_keys):
+            update_value = await self.read_update(param_keys)
+            # Calculate and hash the *new* value so that we can update the
+            # metadata when using side-loaded information.
+            new_value = await self.apply_update(update_value, previous_value)
+            new_hash = lsh.get_lsh().hash(new_value)
+            return await self.write_update(update_value), new_hash
+        else:
+            update_value = await self.calculate_update(param, previous_value)
+            return await self.write_update(update_value), None
 
     async def apply(
         self,
         param_metadata: metadata.ParamMetadata,
         param_keys: Tuple[str],
         *,
         repo,
```

### Comparing `git_theta-0.0.2/git_theta/updates/dense.py` & `git_theta-0.1.1/git_theta/updates/dense.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Class managing dense parameter updates."""
 
 import logging
-from typing import Optional, Any
+from typing import Any, Optional
+
 from git_theta import git_utils, metadata
 from git_theta.updates import Update
 
-
 Parameter = Any
 
 
 class DenseUpdate(Update):
     """An update where all parameters are changed."""
 
-    @property
-    def name(self):
-        return "dense"
+    name: str = "dense"
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
     async def apply(self, param_metadata, param_keys, *args, **kwargs) -> Parameter:
         logging.debug(f"Reading Dense update for {'/'.join(param_keys)}")
         return await self.read(param_metadata)
 
     async def write(self, param, param_keys, *args, **kwargs) -> metadata.LfsMetadata:
         logging.debug(f"Writing Dense update for {'/'.join(param_keys)}")
         serialized = await self.serializer.serialize({"parameter": param})
         lfs_pointer = await git_utils.git_lfs_clean(serialized)
-        return metadata.LfsMetadata.from_pointer(lfs_pointer)
+        return metadata.LfsMetadata.from_pointer(lfs_pointer), None
```

### Comparing `git_theta-0.0.2/git_theta/updates/low_rank.py` & `git_theta-0.1.1/git_theta/updates/low_rank.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 """An update type where the update is stored as 2 low-rank matrices."""
 
 
 import logging
-from typing import Any, Optional
+from typing import Any, FrozenSet, Optional
+
 import numpy as np
+
 from git_theta.updates import IncrementalUpdate
 
 Parameter = Any
 
 
 class LowRankUpdate(IncrementalUpdate):
     """An update make for 2 low rank matrices."""
 
+    name: str = "low-rank"
+    required_keys: FrozenSet[str] = frozenset(("R", "C"))
+
     # TODO: Make these configuration options easy set.
     def __init__(
         self, *args, K: Optional[int] = None, threshold: float = 1e-11, **kwargs
     ):
         super().__init__(*args, **kwargs)
         self.K = K
         self.threshold = threshold
 
-    @property
-    def name(self):
-        return "low-rank"
+    @classmethod
+    def format_update(
+        cls, param1: Parameter, param2: Parameter, *args, **kwargs
+    ) -> Parameter:
+        return {
+            "R": param1,
+            "C": param2,
+        }
 
     async def calculate_update(
         self, parameter: Parameter, previous_parameter: Parameter
     ) -> Parameter:
         update = parameter - previous_parameter
         if update.ndim < 2:
             return update
```

### Comparing `git_theta-0.0.2/git_theta/updates/sparse.py` & `git_theta-0.1.1/git_theta/updates/sparse.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 """A class for handling sparse updates to parameters."""
 
 import logging
-from typing import Optional, Any
-from git_theta.updates import IncrementalUpdate
-from git_theta import params
-import scipy.sparse
+from typing import Any, FrozenSet, Optional
+
 import numpy as np
+import scipy.sparse
+
+from git_theta import params
+from git_theta.updates import IncrementalUpdate
 
 Parameter = Any
 
 
 class SparseUpdate(IncrementalUpdate):
     """An update where only some parameters are touched."""
 
-    def __init__(self, serializer: params.Serializer, threshold: float = 1e-12):
+    name: str = "sparse"
+    required_keys: FrozenSet[str] = frozenset(("data", "indices", "indptr", "shape"))
+
+    def __init__(
+        self,
+        serializer: params.Serializer,
+        update_data: str = "",
+        threshold: float = 1e-12,
+    ):
         # TODO: Make threshold configurable
-        super().__init__(serializer)
+        super().__init__(serializer, update_data)
         self.threshold = threshold
 
-    @property
-    def name(self):
-        return "sparse"
+    @classmethod
+    def format_update(cls, param: Parameter, *args, **kwargs) -> Parameter:
+        """User-facing helper to convert an array to sparse storage."""
+        update = scipy.sparse.csr_matrix(np.reshape(param, (1, -1)))
+        return {
+            "data": update.data,
+            "indices": update.indices,
+            "indptr": update.indptr,
+            "shape": np.array(param.shape),
+        }
 
     async def calculate_update(
         self, parameter: Parameter, previous_parameter: Parameter
     ) -> Parameter:
         diff = parameter - previous_parameter
         diff[np.abs(diff) < self.threshold] = 0
         # csr_matrix looks for actual zeros in diff tensor. We added a configurable threshold to have the diff tensor (the update) be really sparse
```

### Comparing `git_theta-0.0.2/git_theta/utils.py` & `git_theta-0.1.1/git_theta/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """Utilities for git theta."""
 
 import dataclasses
-from enum import Enum
+import datetime
 import functools
+import inspect
+import os
 import re
 import subprocess
-from types import MethodType
-from typing import Dict, Any, Tuple, Union, Callable, Iterable, Optional
 from dataclasses import dataclass
-import os
+from enum import Enum
+from types import MethodType
+from typing import Any, Callable, Dict, Iterable, Optional, Tuple, Union
 
 
 def _format(self, value, tag):
     """Wrap `value` in HTML like <tag>s."""
     return f"<{getattr(self, tag)}>{value}</{getattr(self, tag)}>"
 
 
 # TODO: Make configurable
 @dataclasses.dataclass
 class TextStyle:
     param: str = "purple"
     model: str = "cyan"
+    argument: str = "Salmon"
     who: str = "u"
     changed: str = "yellow"
     added: str = "green"
     deleted: str = "red"
 
     # TODO: Move this to classlevel code gen?
     def __post_init__(self):
@@ -49,33 +52,39 @@
     DELETED_B = f"{TEXT_STYLE.format_who('They')} <b>{TEXT_STYLE.format_deleted('deleted')}</b> this parameter."
     DELETED_BOTH = f"{TEXT_STYLE.format_who('Both')} them and us <b>{TEXT_STYLE.format_deleted('deleted')}</b> this parameter."
     ADDED_A = f"{TEXT_STYLE.format_who('We')} <b>{TEXT_STYLE.format_added('added')}</b> this parameter."
     ADDED_B = f"{TEXT_STYLE.format_who('They')} <b>{TEXT_STYLE.format_added('added')}</b> this parameter."
     ADDED_BOTH = f"{TEXT_STYLE.format_who('Both')} them and us <b>{TEXT_STYLE.format_added('added')}</b> this parameter."
 
 
+class NoResult:
+    """A sentinel class used to mark no-action choices."""
+
+
 @dataclass
 class EnvVar:
     name: str
     default: Any
 
     def __get__(self, obj, objtype=None):
         value = os.environ.get(self.name)
         return type(self.default)(value) if value else self.default
 
 
 class EnvVarConstants:
     CHECKPOINT_TYPE = EnvVar(name="GIT_THETA_CHECKPOINT_TYPE", default="pytorch")
     UPDATE_TYPE = EnvVar(name="GIT_THETA_UPDATE_TYPE", default="dense")
+    UPDATE_DATA_PATH = EnvVar(name="GIT_THETA_UPDATE_DATA_PATH", default="update.pt")
     PARAMETER_ATOL = EnvVar(name="GIT_THETA_PARAMETER_ATOL", default=1e-8)
     PARAMETER_RTOL = EnvVar(name="GIT_THETA_PARAMETER_RTOL", default=1e-5)
     LSH_SIGNATURE_SIZE = EnvVar(name="GIT_THETA_LSH_SIGNATURE_SIZE", default=16)
     LSH_THRESHOLD = EnvVar(name="GIT_THETA_LSH_THRESHOLD", default=1e-6)
     LSH_POOL_SIZE = EnvVar(name="GIT_THETA_LSH_POOL_SIZE", default=10_000)
     MAX_CONCURRENCY = EnvVar(name="GIT_THETA_MAX_CONCURRENCY", default=-1)
+    MANUAL_MERGE = EnvVar(name="GIT_THETA_MANUAL_MERGE", default=False)
 
 
 def flatten(
     d: Dict[str, Any],
     is_leaf: Callable[[Any], bool] = lambda v: not isinstance(v, dict),
 ) -> Dict[Tuple[str, ...], Any]:
     """Flatten a nested dictionary.
@@ -228,7 +237,68 @@
         root = cls()
         for word in words:
             root.insert(word)
         return root
 
     def __str__(self):
         return f"{self.__class__.__name__}(char={self.char}, is_word={self.is_word}, next={self.next.keys()})"
+
+
+def abstract_classattributes(*attributes):
+    """Force subclasses to define some class attributes."""
+
+    # Note, we are modifying the class with the decorator, not wrapping it so we
+    # don't need @functools.wraps to maintain information about our class.
+    def inner(base_cls):
+        # First set all attributes (on the base class) to NotImplemented
+        # so the subclasses will inherit them and give us something to compare to.
+        for attribute in attributes:
+            setattr(base_cls, attribute, NotImplemented)
+
+        # Save the original verson of the init, this lets us exectue it to make
+        # sure we preserve any functionality defined by the base class.
+        og_init_subclass = base_cls.__init_subclass__
+
+        # A new version of __init_subclass__ that checks for our attributes.
+        # TODO: How does this change things like __doc__ and __name__?
+        def enforcing_init_subclass(cls, **kwargs):
+            # Call the original one, if they didn't override the implementation it
+            # doesn't take cls as an argument. Just try each version to see what works.
+            try:
+                og_init_subclass(cls, **kwargs)
+            except TypeError:
+                og_init_subclass(**kwargs)
+
+            # Collect all attributes on the subclass now, that still have their
+            # default (inherited) value.
+            missing_attributes = []
+            for attribute in attributes:
+                if getattr(cls, attribute, NotImplemented) is NotImplemented:
+                    missing_attributes.append(attribute)
+
+            # Error out if they are a concrete class and missing things.
+            if missing_attributes and not inspect.isabstract(cls):
+                missing = [f'"{attr}"' for attr in missing_attributes]
+                plural = ""
+                # Make it look pretty and handle pluralization.
+                if len(missing) > 1:
+                    missing[-1] = f"and {missing[-1]}"
+                    plural = "s"
+                missing = ", ".join(missing)
+                raise NotImplementedError(
+                    f"Abstract Attribute{plural} {missing} missing "
+                    f"on class {cls.__name__}"
+                )
+
+            return cls
+
+        # Set this as the new __init_subclass__ and make sure it is a class method.
+        base_cls.__init_subclass__ = classmethod(enforcing_init_subclass)
+        return base_cls
+
+    return inner
+
+
+def touch(path: str):
+    """Update the access and modify time of `path`."""
+    dt_epoch = datetime.datetime.now().timestamp()
+    os.utime(path, (dt_epoch, dt_epoch))
```

### Comparing `git_theta-0.0.2/git_theta.egg-info/SOURCES.txt` & `git_theta-0.1.1/git_theta.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 LICENSE.md
 README.md
 pyproject.toml
 setup.py
-bin/git-theta
-bin/git-theta-filter
-bin/git-theta-merge
 git_theta/__init__.py
 git_theta/async_utils.py
 git_theta/git_utils.py
 git_theta/metadata.py
 git_theta/params.py
 git_theta/theta.py
 git_theta/types.py
@@ -30,13 +27,20 @@
 git_theta/lsh/base.py
 git_theta/lsh/euclidean_lsh.py
 git_theta/lsh/pool.py
 git_theta/lsh/types.py
 git_theta/merges/__init__.py
 git_theta/merges/average.py
 git_theta/merges/base.py
+git_theta/merges/context.py
 git_theta/merges/take.py
+git_theta/scripts/__init__.py
+git_theta/scripts/git_theta.py
+git_theta/scripts/git_theta_diff.py
+git_theta/scripts/git_theta_filter.py
+git_theta/scripts/git_theta_merge.py
 git_theta/updates/__init__.py
 git_theta/updates/base.py
 git_theta/updates/dense.py
+git_theta/updates/ia3.py
 git_theta/updates/low_rank.py
 git_theta/updates/sparse.py
```

### Comparing `git_theta-0.0.2/git_theta.egg-info/entry_points.txt` & `git_theta-0.1.1/git_theta.egg-info/entry_points.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+[console_scripts]
+git-theta = git_theta.scripts.git_theta:main
+git-theta-diff = git_theta.scripts.git_theta_diff:main
+git-theta-filter = git_theta.scripts.git_theta_filter:main
+git-theta-merge = git_theta.scripts.git_theta_merge:main
+
 [git_theta.plugins.checkpoints]
 flax = git_theta.checkpoints.flax_checkpoint:FlaxCheckpoint
 pickled-dict = git_theta.checkpoints.pickled_dict_checkpoint:PickledDictCheckpoint
 pytorch = git_theta.checkpoints.pickled_dict_checkpoint:PickledDictCheckpoint
 tensorflow = git_theta.checkpoints.tensorflow_checkpoint:TensorFlowCheckpoint
 tensorflow-checkpoint = git_theta.checkpoints.tensorflow_checkpoint:TensorFlowCheckpoint
 tensorflow-savedmodel = git_theta.checkpoints.tensorflow_checkpoint:TensorFlowSavedModel
@@ -9,15 +15,17 @@
 tf-savedmodel = git_theta.checkpoints.tensorflow_checkpoint:TensorFlowSavedModel
 
 [git_theta.plugins.merges]
 average-all = git_theta.merges.average:AverageAll
 average-ours-original = git_theta.merges.average:AverageOursOriginal
 average-ours-theirs = git_theta.merges.average:Average
 average-theirs-original = git_theta.merges.average:AverageTheirsOriginal
+context = git_theta.merges.context:Context
 take_original = git_theta.merges.take:TakeOriginal
 take_them = git_theta.merges.take:TakeThem
 take_us = git_theta.merges.take:TakeUs
 
 [git_theta.plugins.updates]
 dense = git_theta.updates.dense:DenseUpdate
+ia3 = git_theta.updates.ia3:IA3Update
 low-rank = git_theta.updates.low_rank:LowRankUpdate
 sparse = git_theta.updates.sparse:SparseUpdate
```

### Comparing `git_theta-0.0.2/setup.py` & `git_theta-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Install the git-theta package."""
 
 import ast
 import itertools
-from setuptools import setup, find_packages
+from pathlib import Path
+
+from setuptools import find_packages, setup
 
 
 def get_version(file_name: str, version_variable: str = "__version__") -> str:
     """Find the version by walking the AST to avoid duplication.
 
     Parameters
     ----------
@@ -43,73 +45,96 @@
 frameworks_require = {
     "pytorch": ["torch"],
     "tensorflow": ["tensorflow"],
     "flax": ["flax"],
 }
 
 
+with open(Path(__file__).parent / "README.md", encoding="utf-8") as f:
+    LONG_DESCRIPTION = f.read()
+
+
 setup(
     name="git_theta",
     version=get_version("git_theta/__init__.py"),
-    description="Version control system for model checkpoints.",
+    description="Version control system for machine learning model checkpoints.",
+    long_description=LONG_DESCRIPTION,
+    long_description_content_type="text/markdown",
     author="Colin Raffel",
     author_email="craffel@gmail.com",
-    url="https://github.com/r-three/checkpoint-vcs",
+    url="https://github.com/r-three/git-theta",
     packages=find_packages(),
+    include_package_data=True,
     package_data={"git_theta": ["hooks/post-commit", "hooks/pre-push"]},
-    scripts=["bin/git-theta", "bin/git-theta-filter", "bin/git-theta-merge"],
-    long_description="Version control system for model checkpoints.",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 4 - Beta",
+        "Environment :: Console",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Version Control",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+        "Programming Language :: Python :: 3 :: Only",
+        "Natural Language :: English",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: POSIX :: Linux",
     ],
     keywords="git vcs machine-learning",
     license="MIT",
     install_requires=[
         "GitPython",
         "tensorstore >= 0.1.14",
         "file-or-name",
         "six",
         "scipy",
         "numba",
+        "msgpack",
         'importlib_resources; python_version < "3.9.0"',
         'importlib_metadata; python_version < "3.10.0"',
         'typing_extensions; python_version < "3.8.0"',
     ],
     extras_require={
         **frameworks_require,
         # Install all framework deps with the all target.
         "test": ["pytest"],
         "all": list(set(itertools.chain(*frameworks_require.values()))),
+        "docs": ["sphinx", "numpydoc"],
     },
-    # TODO: Can we auto register these?
     entry_points={
+        "console_scripts": [
+            "git-theta = git_theta.scripts.git_theta:main",
+            "git-theta-filter = git_theta.scripts.git_theta_filter:main",
+            "git-theta-merge = git_theta.scripts.git_theta_merge:main",
+            "git-theta-diff = git_theta.scripts.git_theta_diff:main",
+        ],
         "git_theta.plugins.checkpoints": [
             "pytorch = git_theta.checkpoints.pickled_dict_checkpoint:PickledDictCheckpoint",
             "pickled-dict = git_theta.checkpoints.pickled_dict_checkpoint:PickledDictCheckpoint",
             "tf = git_theta.checkpoints.tensorflow_checkpoint:TensorFlowCheckpoint",
             "tensorflow = git_theta.checkpoints.tensorflow_checkpoint:TensorFlowCheckpoint",
             "tensorflow-checkpoint = git_theta.checkpoints.tensorflow_checkpoint:TensorFlowCheckpoint",
             "tf-savedmodel = git_theta.checkpoints.tensorflow_checkpoint:TensorFlowSavedModel",
             "tensorflow-savedmodel = git_theta.checkpoints.tensorflow_checkpoint:TensorFlowSavedModel",
             "flax = git_theta.checkpoints.flax_checkpoint:FlaxCheckpoint",
         ],
         "git_theta.plugins.updates": [
             "dense = git_theta.updates.dense:DenseUpdate",
             "sparse = git_theta.updates.sparse:SparseUpdate",
             "low-rank = git_theta.updates.low_rank:LowRankUpdate",
+            "ia3 = git_theta.updates.ia3:IA3Update",
         ],
         "git_theta.plugins.merges": [
             "take_us = git_theta.merges.take:TakeUs",
             "take_them = git_theta.merges.take:TakeThem",
             "take_original = git_theta.merges.take:TakeOriginal",
             "average-ours-theirs = git_theta.merges.average:Average",
             "average-all = git_theta.merges.average:AverageAll",
             "average-ours-original = git_theta.merges.average:AverageOursOriginal",
             "average-theirs-original = git_theta.merges.average:AverageTheirsOriginal",
+            "context = git_theta.merges.context:Context",
         ],
     },
 )
```

