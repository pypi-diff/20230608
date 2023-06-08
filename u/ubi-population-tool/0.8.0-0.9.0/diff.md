# Comparing `tmp/ubi-population-tool-0.8.0.tar.gz` & `tmp/ubi-population-tool-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubi-population-tool-0.8.0.tar", last modified: Tue Sep 21 10:10:06 2021, max compression
+gzip compressed data, was "ubi-population-tool-0.9.0.tar", last modified: Wed Sep 29 08:21:38 2021, max compression
```

## Comparing `ubi-population-tool-0.8.0.tar` & `ubi-population-tool-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-21 10:10:06.339893 ubi-population-tool-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2021-09-21 10:09:54.000000 ubi-population-tool-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    35148 2021-09-21 10:09:54.000000 ubi-population-tool-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-09-21 10:09:54.000000 ubi-population-tool-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2021-09-21 10:10:06.339893 ubi-population-tool-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2021-09-21 10:09:54.000000 ubi-population-tool-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      132 2021-09-21 10:09:54.000000 ubi-population-tool-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-21 10:10:06.339893 ubi-population-tool-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2021-09-21 10:09:54.000000 ubi-population-tool-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-21 10:10:06.335893 ubi-population-tool-0.8.0/ubi_population_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2021-09-21 10:10:05.000000 ubi-population-tool-0.8.0/ubi_population_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      420 2021-09-21 10:10:06.000000 ubi-population-tool-0.8.0/ubi_population_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-21 10:10:05.000000 ubi-population-tool-0.8.0/ubi_population_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-09-21 10:10:05.000000 ubi-population-tool-0.8.0/ubi_population_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-09-21 10:10:05.000000 ubi-population-tool-0.8.0/ubi_population_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-09-21 10:10:05.000000 ubi-population-tool-0.8.0/ubi_population_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-21 10:10:06.339893 ubi-population-tool-0.8.0/ubipop/
--rw-r--r--   0 runner    (1001) docker     (121)    24003 2021-09-21 10:09:54.000000 ubi-population-tool-0.8.0/ubipop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18122 2021-09-21 10:09:54.000000 ubi-population-tool-0.8.0/ubipop/_matcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     6777 2021-09-21 10:09:54.000000 ubi-population-tool-0.8.0/ubipop/_pulp_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5068 2021-09-21 10:09:54.000000 ubi-population-tool-0.8.0/ubipop/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3646 2021-09-21 10:09:54.000000 ubi-population-tool-0.8.0/ubipop/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 08:21:38.593336 ubi-population-tool-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     2647 2021-09-29 08:21:30.000000 ubi-population-tool-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)    35148 2021-09-29 08:21:30.000000 ubi-population-tool-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-09-29 08:21:30.000000 ubi-population-tool-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1937 2021-09-29 08:21:38.593336 ubi-population-tool-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1756 2021-09-29 08:21:30.000000 ubi-population-tool-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2021-09-29 08:21:30.000000 ubi-population-tool-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-29 08:21:38.593336 ubi-population-tool-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1407 2021-09-29 08:21:30.000000 ubi-population-tool-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 08:21:38.589336 ubi-population-tool-0.9.0/ubi_population_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1937 2021-09-29 08:21:38.000000 ubi-population-tool-0.9.0/ubi_population_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      420 2021-09-29 08:21:38.000000 ubi-population-tool-0.9.0/ubi_population_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 08:21:38.000000 ubi-population-tool-0.9.0/ubi_population_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2021-09-29 08:21:38.000000 ubi-population-tool-0.9.0/ubi_population_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-09-29 08:21:38.000000 ubi-population-tool-0.9.0/ubi_population_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-09-29 08:21:38.000000 ubi-population-tool-0.9.0/ubi_population_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 08:21:38.593336 ubi-population-tool-0.9.0/ubipop/
+-rw-r--r--   0 runner    (1001) docker     (121)    24395 2021-09-29 08:21:30.000000 ubi-population-tool-0.9.0/ubipop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18122 2021-09-29 08:21:30.000000 ubi-population-tool-0.9.0/ubipop/_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6777 2021-09-29 08:21:30.000000 ubi-population-tool-0.9.0/ubipop/_pulp_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5068 2021-09-29 08:21:30.000000 ubi-population-tool-0.9.0/ubipop/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3646 2021-09-29 08:21:30.000000 ubi-population-tool-0.9.0/ubipop/cli.py
```

### Comparing `ubi-population-tool-0.8.0/CHANGELOG.md` & `ubi-population-tool-0.9.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 - n/a
 
+## [0.9.0]
+
+### Changed
+- Publishing UBI repositories is now non-blocking
+
 ## [0.8.0]
 
 ### Added
 - New cli options --version and --content-set-regex
 
 ### Changed
 - Queries for current content use Matcher class now
@@ -63,15 +68,16 @@
 
 ## [0.1.19] - 2019-06-25
 
 ### Fixed 
 - py26 compatibility issue on travis
 - rpm-py-installer requirement was made conditional  
 
-[Unreleased]: https://github.com/release-engineering/ubi-population-tool/compare/v0.8.0...HEAD
+[Unreleased]: https://github.com/release-engineering/ubi-population-tool/compare/v0.9.0...HEAD
+[0.9.0]: https://github.com/release-engineering/ubi-population-tool/compare/v0.8.0...0.9.0
 [0.8.0]: https://github.com/release-engineering/ubi-population-tool/compare/v0.7.0...0.8.0
 [0.7.0]: https://github.com/release-engineering/ubi-population-tool/compare/v0.6.0...0.7.0
 [0.6.0]: https://github.com/release-engineering/ubi-population-tool/compare/v0.5.0...0.6.0
 [0.5.0]: https://github.com/release-engineering/ubi-population-tool/compare/v0.4.0...0.5.0
 [0.4.0]: https://github.com/release-engineering/ubi-population-tool/compare/v0.3.1...0.4.0
 [0.3.1]: https://github.com/release-engineering/ubi-population-tool/compare/v0.3.0...0.3.1
 [0.3.0]: https://github.com/release-engineering/ubi-population-tool/compare/v0.2.0...0.3.0
```

### Comparing `ubi-population-tool-0.8.0/LICENSE` & `ubi-population-tool-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ubi-population-tool-0.8.0/PKG-INFO` & `ubi-population-tool-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: ubi-population-tool
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tool for populating ubi repositories
 Home-page: https://github.com/release-engineering/ubi-population-tool
 Author: 
 Author-email: 
 License: GNU General Public License
 Description: 
         
-        
         A command-line tool for populating ubi repositories.
         
         # Cli usage
         
         Cli can be run by *ubipop* with arguments:
         
         - positional arguments:
```

### Comparing `ubi-population-tool-0.8.0/README.md` & `ubi-population-tool-0.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # **ubi-population-tool**
-[![Build Status](https://travis-ci.org/release-engineering/ubi-population-tool.svg?branch=master)](https://travis-ci.org/release-engineering/ubi-population-tool)
-[![Coverage Status](https://coveralls.io/repos/github/release-engineering/ubi-population-tool/badge.svg?branch=master)](https://coveralls.io/github/release-engineering/ubi-population-tool?branch=master)
-
+[![Build Status](https://github.com/release-engineering/ubi-population-tool/actions/workflows/tox-test.yml/badge.svg)](https://github.com/release-engineering/ubi-population-tool/actions/workflows/tox-test.yml)
+[![codecov](https://codecov.io/gh/release-engineering/ubi-population-tool/branch/master/graph/badge.svg?token=APniN2wa2U)](https://codecov.io/gh/release-engineering/ubi-population-tool/)
+[![Source](https://badgen.net/badge/icon/source?icon=github&label)](https://github.com/release-engineering/ubi-population-tool/)
+[![Documentation](https://github.com/release-engineering/ubi-population-tool/actions/workflows/docs.yml/badge.svg)](https://release-engineering.github.io/ubi-population-tool/)
+[![PyPI version](https://badgen.net/pypi/v/ubi-population-tool?color=blue)](https://pypi.org/project/ubi-population-tool/)
 
 A command-line tool for populating ubi repositories.
 
 # Cli usage
 
 Cli can be run by *ubipop* with arguments:
```

### Comparing `ubi-population-tool-0.8.0/setup.py` & `ubi-population-tool-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_requirements():
     with open("requirements.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="ubi-population-tool",
-    version="0.8.0",
+    version="0.9.0",
     license="GNU General Public License",
     author="",
     author_email="",
     description=get_description(),
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `ubi-population-tool-0.8.0/ubi_population_tool.egg-info/PKG-INFO` & `ubi-population-tool-0.9.0/ubi_population_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: ubi-population-tool
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tool for populating ubi repositories
 Home-page: https://github.com/release-engineering/ubi-population-tool
 Author: 
 Author-email: 
 License: GNU General Public License
 Description: 
         
-        
         A command-line tool for populating ubi repositories.
         
         # Cli usage
         
         Cli can be run by *ubipop* with arguments:
         
         - positional arguments:
```

### Comparing `ubi-population-tool-0.8.0/ubipop/__init__.py` & `ubi-population-tool-0.9.0/ubipop/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,14 +274,16 @@
     def populate_ubi_repos(self):
         out_repos = set()
         used_content_sets = set()
         # since repos are searched by content sets, same repo could be searched and populated
         # multiple times, to avoid that, cache the content sets already used and skip the config
         # whose content sets are all in the cache
 
+        awaited_repos_publishes = []
+
         for config in sorted(self.ubiconfig_list, key=str):
             content_sets = [
                 config.content_sets.rpm.output,
                 config.content_sets.srpm.output,
                 config.content_sets.debuginfo.output,
             ]
 
@@ -302,24 +304,32 @@
                 _LOG.warning("Skipping current content triplet, some repos are missing")
                 continue
 
             for repo_set in repo_pairs:
                 right_config = self._get_config(
                     repo_set.out_repos.rpm.ubi_config_version, config
                 )
-                UbiPopulateRunner(
+
+                repos_publishes = UbiPopulateRunner(
                     self.pulp,
                     self.pulp_client,
                     repo_set,
                     right_config,
                     self.dry_run,
                     self._executor,
                 ).run_ubi_population()
 
                 out_repos.update(repo_set.get_output_repo_ids())
+                # in case of dry-run there are no publications expected
+                if repos_publishes:
+                    awaited_repos_publishes.extend(repos_publishes)
+
+        # wait until publication of all repos is finished
+        if awaited_repos_publishes:
+            f_sequence(awaited_repos_publishes).result()
 
         if self.output_repos:
             with open(self.output_repos, "w") as f:
                 for repo in out_repos:
                     f.write(repo.strip() + "\n")
 
     def _get_ubi_repo_sets(self, ubi_binary_cs):
@@ -521,14 +531,15 @@
 
         attrs_list_2 = [diff_attr(obj) for obj in list_2]
         diff = [obj for obj in list_1 if diff_attr(obj) not in attrs_list_2]
 
         return diff
 
     def run_ubi_population(self):
+
         current_content = self._get_current_content()
         # start async querying for modulemds and modular and non-modular packages
         mm = ModularMatcher(self.repos.in_repos, self.ubiconfig.modules).run()
         rm = RpmMatcher(self.repos.in_repos, self.ubiconfig).run()
 
         self.repos.modules = mm.modules
         self.repos.module_defaults = mm.modulemd_defaults
@@ -560,16 +571,16 @@
             # wait for associate/unassociate tasks
             self._wait_pulp(fts)
 
             self._associate_unassociate_md_defaults(
                 (mdd_association,), (mdd_unassociation,)
             )
 
-            # wait repo publication
-            f_sequence(self._publish_out_repos()).result()
+            # return list of futures with repo publishes
+            return self._publish_out_repos()
 
     def _associate_unassociate_units(self, action_list):
         fts = []
         for action in action_list:
             if action.units:
                 fts.extend(
                     [self._executor.submit(*a) for a in action.get_actions(self.pulp)]
@@ -694,13 +705,12 @@
     def _publish_out_repos(self):
         fts = []
         repos_to_publish = (
             self.repos.out_repos.rpm,
             self.repos.out_repos.debug,
             self.repos.out_repos.source,
         )
-
         options = PublishOptions(clean=True)
         for repo in repos_to_publish:
             if repo.result():
                 fts.append(repo.publish(options))
         return fts
```

### Comparing `ubi-population-tool-0.8.0/ubipop/_matcher.py` & `ubi-population-tool-0.9.0/ubipop/_matcher.py`

 * *Files identical despite different names*

### Comparing `ubi-population-tool-0.8.0/ubipop/_pulp_client.py` & `ubi-population-tool-0.9.0/ubipop/_pulp_client.py`

 * *Files identical despite different names*

### Comparing `ubi-population-tool-0.8.0/ubipop/_utils.py` & `ubi-population-tool-0.9.0/ubipop/_utils.py`

 * *Files identical despite different names*

### Comparing `ubi-population-tool-0.8.0/ubipop/cli.py` & `ubi-population-tool-0.9.0/ubipop/cli.py`

 * *Files identical despite different names*

