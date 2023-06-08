# Comparing `tmp/altparse-0.2.1.tar.gz` & `tmp/altparse-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altparse-0.2.1.tar", last modified: Sun Apr 16 01:28:10 2023, max compression
+gzip compressed data, was "altparse-0.3.0.tar", last modified: Thu Jun  8 05:28:08 2023, max compression
```

## Comparing `altparse-0.2.1.tar` & `altparse-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 01:28:10.168700 altparse-0.2.1/
--rw-rw-rw-   0        0        0       66 2022-05-23 21:26:59.000000 altparse-0.2.1/.gitattributes
--rw-rw-rw-   0        0        0     1447 2022-06-03 19:24:20.000000 altparse-0.2.1/.gitignore
--rw-rw-rw-   0        0        0        0 2022-11-30 22:58:46.000000 altparse-0.2.1/CHANGES.md
--rw-rw-rw-   0        0        0     1086 2022-05-23 21:26:59.000000 altparse-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2022-11-30 22:59:45.000000 altparse-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2429 2023-04-16 01:28:10.168198 altparse-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-02-26 04:17:54.000000 altparse-0.2.1/README.md
--rw-rw-rw-   0        0        0     1018 2023-04-16 01:26:48.000000 altparse-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 01:28:10.169200 altparse-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0       71 2022-12-01 01:01:54.000000 altparse-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 01:28:10.063699 altparse-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 01:28:10.095699 altparse-0.2.1/src/altparse/
--rw-rw-rw-   0        0        0      155 2022-12-06 02:28:59.000000 altparse-0.2.1/src/altparse/__init__.py
--rw-rw-rw-   0        0        0    13618 2023-04-16 01:10:40.000000 altparse-0.2.1/src/altparse/core.py
--rw-rw-rw-   0        0        0      615 2023-03-28 23:48:04.000000 altparse-0.2.1/src/altparse/errors.py
--rw-rw-rw-   0        0        0     3101 2022-12-06 07:19:15.000000 altparse-0.2.1/src/altparse/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-16 01:28:10.131697 altparse-0.2.1/src/altparse/ipautil/
--rw-rw-rw-   0        0        0      156 2022-12-06 07:29:32.000000 altparse-0.2.1/src/altparse/ipautil/__init__.py
--rw-rw-rw-   0        0        0     3493 2023-04-15 22:08:19.000000 altparse-0.2.1/src/altparse/ipautil/core.py
--rw-rw-rw-   0        0        0      603 2022-12-06 07:12:17.000000 altparse-0.2.1/src/altparse/ipautil/errors.py
--rw-rw-rw-   0        0        0     5074 2023-04-16 01:16:54.000000 altparse-0.2.1/src/altparse/ipautil/helpers.py
--rw-rw-rw-   0        0        0     4150 2023-04-15 22:11:00.000000 altparse-0.2.1/src/altparse/ipautil/model.py
--rw-rw-rw-   0        0        0    27402 2023-04-16 01:19:43.000000 altparse-0.2.1/src/altparse/model.py
--rw-rw-rw-   0        0        0    14271 2023-04-16 01:26:02.000000 altparse-0.2.1/src/altparse/parsers.py
-drwxrwxrwx   0        0        0        0 2023-04-16 01:28:10.122698 altparse-0.2.1/src/altparse.egg-info/
--rw-rw-rw-   0        0        0     2429 2023-04-16 01:28:09.000000 altparse-0.2.1/src/altparse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      720 2023-04-16 01:28:10.000000 altparse-0.2.1/src/altparse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 01:28:09.000000 altparse-0.2.1/src/altparse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-16 01:28:09.000000 altparse-0.2.1/src/altparse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-16 01:28:09.000000 altparse-0.2.1/src/altparse.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 01:28:10.166198 altparse-0.2.1/tests/
--rw-rw-rw-   0        0        0   357189 2022-12-06 04:50:45.000000 altparse-0.2.1/tests/XPatcher_2.2.ipa
--rw-rw-rw-   0        0        0        1 2022-12-01 07:44:32.000000 altparse-0.2.1/tests/__init__.py
--rw-rw-rw-   0        0        0      987 2022-12-06 07:11:28.000000 altparse-0.2.1/tests/example_ipa_upload.py
--rw-rw-rw-   0        0        0     6199 2023-04-16 00:40:19.000000 altparse-0.2.1/tests/example_update.py
--rw-rw-rw-   0        0        0   210229 2023-04-16 00:44:35.000000 altparse-0.2.1/tests/quantumsource.json
--rw-rw-rw-   0        0        0      623 2022-12-06 07:31:59.000000 altparse-0.2.1/tests/test_create_altsource_obj.py
+drwxrwxrwx   0        0        0        0 2023-06-08 05:28:08.631998 altparse-0.3.0/
+-rw-rw-rw-   0        0        0       66 2022-05-23 21:26:59.000000 altparse-0.3.0/.gitattributes
+-rw-rw-rw-   0        0        0     1447 2022-06-03 19:24:20.000000 altparse-0.3.0/.gitignore
+-rw-rw-rw-   0        0        0        0 2022-11-30 22:58:46.000000 altparse-0.3.0/CHANGES.md
+-rw-rw-rw-   0        0        0     1086 2022-05-23 21:26:59.000000 altparse-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2022-11-30 22:59:45.000000 altparse-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2429 2023-06-08 05:28:08.631499 altparse-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-02-26 04:17:54.000000 altparse-0.3.0/README.md
+-rw-rw-rw-   0        0        0     1018 2023-06-08 05:27:47.000000 altparse-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 05:28:08.631998 altparse-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       71 2022-12-01 01:01:54.000000 altparse-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 05:28:08.518502 altparse-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-08 05:28:08.561499 altparse-0.3.0/src/altparse/
+-rw-rw-rw-   0        0        0      155 2022-12-06 02:28:59.000000 altparse-0.3.0/src/altparse/__init__.py
+-rw-rw-rw-   0        0        0    14325 2023-06-08 02:22:10.000000 altparse-0.3.0/src/altparse/core.py
+-rw-rw-rw-   0        0        0      615 2023-03-28 23:48:04.000000 altparse-0.3.0/src/altparse/errors.py
+-rw-rw-rw-   0        0        0     4187 2023-06-06 19:28:54.000000 altparse-0.3.0/src/altparse/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-08 05:28:08.595002 altparse-0.3.0/src/altparse/ipautil/
+-rw-rw-rw-   0        0        0      156 2022-12-06 07:29:32.000000 altparse-0.3.0/src/altparse/ipautil/__init__.py
+-rw-rw-rw-   0        0        0     4327 2023-06-06 19:38:09.000000 altparse-0.3.0/src/altparse/ipautil/core.py
+-rw-rw-rw-   0        0        0      603 2022-12-06 07:12:17.000000 altparse-0.3.0/src/altparse/ipautil/errors.py
+-rw-rw-rw-   0        0        0     5074 2023-06-06 02:48:28.000000 altparse-0.3.0/src/altparse/ipautil/helpers.py
+-rw-rw-rw-   0        0        0     9389 2023-06-01 21:09:18.000000 altparse-0.3.0/src/altparse/ipautil/model.py
+-rw-rw-rw-   0        0        0    41725 2023-06-08 05:16:37.000000 altparse-0.3.0/src/altparse/model.py
+-rw-rw-rw-   0        0        0    15318 2023-06-08 00:25:01.000000 altparse-0.3.0/src/altparse/parsers.py
+drwxrwxrwx   0        0        0        0 2023-06-08 05:28:08.585999 altparse-0.3.0/src/altparse.egg-info/
+-rw-rw-rw-   0        0        0     2429 2023-06-08 05:28:08.000000 altparse-0.3.0/src/altparse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      720 2023-06-08 05:28:08.000000 altparse-0.3.0/src/altparse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 05:28:08.000000 altparse-0.3.0/src/altparse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-08 05:28:08.000000 altparse-0.3.0/src/altparse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 05:28:08.000000 altparse-0.3.0/src/altparse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 05:28:08.630000 altparse-0.3.0/tests/
+-rw-rw-rw-   0        0        0   357189 2022-12-06 04:50:45.000000 altparse-0.3.0/tests/XPatcher_2.2.ipa
+-rw-rw-rw-   0        0        0        1 2022-12-01 07:44:32.000000 altparse-0.3.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      987 2022-12-06 07:11:28.000000 altparse-0.3.0/tests/example_ipa_upload.py
+-rw-rw-rw-   0        0        0     6199 2023-06-07 07:31:42.000000 altparse-0.3.0/tests/example_update.py
+-rw-rw-rw-   0        0        0   294916 2023-06-08 05:27:47.000000 altparse-0.3.0/tests/quantumsource.json
+-rw-rw-rw-   0        0        0      623 2022-12-06 07:31:59.000000 altparse-0.3.0/tests/test_create_altsource_obj.py
```

### Comparing `altparse-0.2.1/.gitignore` & `altparse-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `altparse-0.2.1/LICENSE.txt` & `altparse-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `altparse-0.2.1/PKG-INFO` & `altparse-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altparse
-Version: 0.2.1
+Version: 0.3.0
 Summary: Designed to aid in creating and maintaining AltSources
 Author-email: Noah Keck <noahkeck@mindspring.com>
 License: MIT License
         
         Copyright (c) 2022 Noah Keck
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `altparse-0.2.1/pyproject.toml` & `altparse-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "altparse"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
     {name = "Noah Keck", email="noahkeck@mindspring.com"}
 ]
 license = {file = "LICENSE.txt"}
 description = "Designed to aid in creating and maintaining AltSources"
 readme = "README.md"
 keywords = ["altstore", "altsource", "ios", "developer"]
```

### Comparing `altparse-0.2.1/src/altparse/core.py` & `altparse-0.3.0/src/altparse/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 import requests
 from packaging import version
 
 from altparse.errors import *
 from altparse.helpers import *
 from altparse.ipautil import extract_altstore_metadata
 from altparse.ipautil.helpers import download_tempfile
-from altparse.model import AltSource
+from altparse.model import AltSource, update_props_from_new_version
 from altparse.parsers import Parser
 
 
 class AltSourceManager:
-    def __init__(self, src: AltSource | None = None, sources_data: list[dict[str]] | None = None):
+    def __init__(self, src: AltSource | None = None, sources_data: list[dict[str]] | None = None, **kwargs):
         """Creates a new AltSourceManager instance to maintain an AltSource.
 
         If no filepath is provided, a brand new blank source is created.
 
         Args:
             filepath (Path | str | None, optional): The location of the source to be parsed. Defaults to None.
             sources_data (list | None, optional): A list of sources stored in a dictionary format to be used for adding/updating apps, see examples. Defaults to None.
@@ -38,15 +38,15 @@
         self.src_data = sources_data
 
         if src is None:
             self.src = AltSource(path=(Path.cwd / "altsource.json"))
         else:
             self.src = src
 
-    def create_app(self, download_url: str = "", ipa_path: Path | str = None) -> AltSource.App:
+    def create_app(self, download_url: str = "", ipa_path: Path | str = None, **kwargs) -> AltSource.App:
         if download_url=="":
             logging.warning("Users will be unable to download to download the app until a valid download url is set.")
         if not ipa_path and is_url(download_url):
             ipa_path = download_tempfile(download_url)
         if ipa_path:
             if isinstance(str, ipa_path):
                 ipa_path = Path(ipa_path)
@@ -75,15 +75,15 @@
                 logging.error("No bundleIdentifier found in IPA.")
 
             app = AltSource.App(metadata)
             app.add_version(new_ver)
             return app
         return None
 
-    def add(self, app: AltSource.App):
+    def add(self, app: AltSource.App, **kwargs):
         if not isinstance(app, AltSource.App):
             logging.error("No app added.")
             return
         
         if app.appID is None:
             app.appID = app.bundleIdentifier
             
@@ -91,24 +91,24 @@
             logging.error("App is invalid.")
         elif app.appID in [app.appID or app.bundleIdentifier for app in self.src.apps]:
             logging.error("Could not add app. Bundle Identifier already exists in AltSource.")
         else:
             self.src.apps.append(app)
             logging.info(f"Adding {app.name} to {self.src.name}")
 
-    def update(self):
+    def update(self, **kwargs):
         """Updates the primary AltSource using the source data provided to the AltSourceManager.
 
         Raises:
             ArgumentTypeError: the source data / config has incorrect values
             NotImplementedError: only raised if anything other than exactly one bundleID has been passed to a GithubParser
         """
         logging.info(f"Starting on {self.src.name}")
         existingAppIDs = [app.appID or app.bundleIdentifier for app in self.src.apps]
-        existingNewsIDs = [article.newsID for article in self.src.news]
+        existingNewsIDs = [article.identifier for article in self.src.news]
         updatedAppsCount = addedAppsCount = addedNewsCount = 0
 
         for data in self.src_data:
             try:
                 cls = data["parser"].value
                 parser = cls(**data["kwargs"])
 
@@ -116,29 +116,30 @@
                 if isinstance(parser, Parser.ALTSOURCE.value):
                     apps = parser.parse_apps(None if data.get("getAllApps") else data.get("ids"))
                     for app in apps:
                         bundleID = app.appID
                         if bundleID in existingAppIDs:
                             # save the old versions property to ensure old versions aren't lost even if the other AltSource isn't tracking them
                             old_app = self.src.apps[existingAppIDs.index(bundleID)]
-                            # version.parse() will be a lower value if the version is 'older'
+                            # version will be a lower value if the version is 'older'
                             new_ver = app.latest_version()
-                            if version.parse(new_ver.version) > version.parse(self.src.apps[existingAppIDs.index(bundleID)].latest_version().version):
+                            if new_ver > old_app.latest_version():
                                 updatedAppsCount += 1
+                                update_props_from_new_version(old_app, new_ver) # handles incompatibilities with older format AltSources
                                 old_app.add_version(new_ver)
                             app._src = old_app._src # use the _src property to avoid overwrite warnings
                             self.src.apps[existingAppIDs.index(bundleID)] = app # note that this actually updates the app regardless of whether the version is newer
                         else:
                             addedAppsCount += 1
                             self.src.apps.append(app)
 
                     if not data.get("ignoreNews"):
                         news = parser.parse_news(None if data.get("getAllNews") else data.get("ids"))
                         for article in news:
-                            newsID = article.newsID
+                            newsID = article.identifier
                             if newsID in existingNewsIDs:
                                 self.src.news[existingNewsIDs.index(newsID)] = article # overwrite existing news article
                             else:
                                 addedNewsCount += 1
                                 self.src.news.append(article)
 
                 elif isinstance(parser, Parser.GITHUB.value) or isinstance(parser, Parser.UNC0VER.value):
@@ -159,40 +160,45 @@
                         if id not in existingAppIDs:
                             logging.warning(f"{id} not found in {self.src.name}. Create an app entry with this bundleID first.")
                             continue
 
                         app = self.src.apps[existingAppIDs.index(id)]
                         
                         # try to use absoluteVersion if the App contains it
-                        if version.parse(app.versions[0].absoluteVersion if app.versions[0].absoluteVersion else app.versions[0].version) < version.parse(parser.version) or (parser.prefer_date and parse_github_datetime(app.versions[0].date) < parse_github_datetime(parser.versionDate)): 
+                        new_ver = {
+                            "absoluteVersion": parser.version,
+                            "version": parser.version,
+                            "date": parser.versionDate,
+                            "size": 0,
+                            "downloadURL": parser.downloadURL
+                        }
+                        
+                        new_ver = AltSource.App.Version(new_ver)
+                        
+                        if app.latest_version() < new_ver or (parser.prefer_date and parse_github_datetime(app.latest_version(True).date) < parse_github_datetime(new_ver.date)): 
                             metadata = parser.get_asset_metadata()
                             
-                            new_ver = {
-                                "absoluteVersion": parser.version,
-                                "date": parser.versionDate,
-                                "localizedDescription": parser.versionDescription,
-                                "size": metadata.get("size"),
-                                "sha256": metadata.get("sha256"),
-                                "version": metadata.get("version") or parser.version,
-                                "downloadURL": metadata.get("downloadURL")
-                            }
-                            
-                            new_ver = AltSource.App.Version(new_ver)
+                            new_ver.version = metadata.get("version") or parser.version
+                            new_ver.buildVersion = metadata.get("buildVersion")
+                            new_ver.size = metadata.get("size")
+                            new_ver.sha256 = metadata.get("sha256")
+                            new_ver.localizedDescription = parser.versionDescription
                             
                             if not metadata.get("bundleIdentifier"):
                                 logging.error("No bundleIdentifier found in IPA.")
                             elif metadata["bundleIdentifier"] != app.bundleIdentifier:
-                                logging.warning(app.name + " BundleID has changed to " + metadata["bundleIdentifier"])
+                                logging.warning(app.name + " BundleID changed. This may cause issues with automatic updates.")
                                 app.bundleIdentifier = metadata["bundleIdentifier"]
                                 new_ver.localizedDescription += "\n\nNOTE: BundleIdentifier changed in this version and automatic updates have been disabled until manual install occurs."
 
                             if app.appID is None:
                                 app.appID = id
                             
                             app.add_version(new_ver)
+                            app.appPermissions = AltSource.App.Permissions(metadata.get("appPermissions"))
                             updatedAppsCount += 1
                 else:
                     raise NotImplementedError("The specified parser class is not supported.")
             except json.JSONDecodeError as err:
                 logging.error(f"Unable to process {data.get('ids')}.")
                 errstr = str(err).replace('\n', '\n\t') #indent newlines for prettier printing
                 logging.error(f"{type(err).__name__}: {errstr[:300]}...") #only print first 300 chars
@@ -218,14 +224,15 @@
             only_latest (bool, optional): Only updates missing hashes for the latest version. Defaults to True.
             force_update (bool, optional): Forces every app, every version to update its hash. Defaults to False.
         """
         for app in self.src.apps:
             if only_latest:
                 latest_ver = app.latest_version()
                 if force_update or latest_ver.sha256 is None:
+                    logging.debug(f"Updating {app.name} sha256 checksum.")
                     latest_ver.calculate_sha256()
             else:
                 for ver in app.versions:
                     if force_update or ver.sha256 is None:
                         ver.calculate_sha256()
 
     def alter_app_info(self, alternate_data: dict[str, dict[str, any]]):
@@ -235,26 +242,29 @@
         
         alternate_data (dict | None, optional): A dictionary containing preferred AltStore app metadata using the bundleID as the key. Defaults to None.
         """
         for i in range(len(self.src.apps)):
             bundleID = self.src.apps[i].appID
             if bundleID in alternate_data.keys():
                 for key in alternate_data[bundleID].keys():
-                    if key == "permissions":
-                        self.src.apps[i]._src[key] = [AltSource.App.Permission(perm) for perm in alternate_data[bundleID][key]]
+                    if key == "appPermissions":
+                        self.src.apps[i]._src[key] = AltSource.App.Permissions(alternate_data[bundleID][key])
                     elif key == "versions":
                         self.src.apps[i]._src[key] = [AltSource.App.Version(ver) for ver in alternate_data[bundleID][key]]
                     else:
                         self.src.apps[i]._src[key] = alternate_data[bundleID][key]
 
-    def save(self, alternate_dir: Path | str | None = None, prettify: bool = True):
+    def save(self, alternate_dir: Path | str | None = None, prettify: bool = True, only_standard_props: bool = True):
         """Saves the AltSource the manager is in charge of to file.
 
         Args:
             prettify (bool, optional): If False, the file will saved as a minified file. Defaults to True.
             alternate_dir (Path | str | None, optional): _description_. Defaults to None.
+            only_standard_props (bool, optional): If False, the entire dict used as the backend storage will be output instead of only "normal" AltSource properties. Defaults to True.
         """
-        full_src = self.src.to_dict()
+        full_src = dict(self.src) if only_standard_props else self.src.to_dict() 
         with open(alternate_dir or self.src.path, "w", encoding="utf-8") as fp:
-            json.dump(full_src, fp, indent = 2 if prettify else None)
+            if prettify:
+                json.dump(full_src, fp, sort_keys=False, indent=2)
+            else:
+                json.dump(full_src, fp)
             fp.write("\n") # add missing newline to EOF
-
```

### Comparing `altparse-0.2.1/src/altparse/errors.py` & `altparse-0.3.0/src/altparse/errors.py`

 * *Files identical despite different names*

### Comparing `altparse-0.2.1/src/altparse/helpers.py` & `altparse-0.3.0/src/altparse/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -72,7 +72,47 @@
     Returns:
         dict[str, str] | None: A dict that allows conversion from key:`appID` to value:`bundleID` based on the list of ids given.
     """
     convert_ids = [dic for dic in ids if isinstance(dic, dict)]
     if convert_ids is not None:
         return {k: v for d in convert_ids for k, v in d.items()} # combine into one dict
     return None
+
+def equal_ignore_order(a, b):
+    """ Use only when elements are neither hashable nor sortable! """
+    unmatched = list(b)
+    for element in a:
+        try:
+            unmatched.remove(element)
+        except ValueError:
+            return False
+    return not unmatched
+
+def class_properties(cls: type) -> list[str]:
+    """Collects only the @property methods on the passed class.
+
+    Args:
+        cls (type): The object class type
+
+    Returns:
+        list[str]: A list of string keys for the classes properties
+    """
+    return [
+        key
+        for key, value in cls.__dict__.items()
+        if isinstance(value, property)
+    ]
+
+def all_class_properties(cls: type) -> list[str]:
+    """Collects all the @property methods on the passed class and all of the classes it inherited from.
+
+    Args:
+        cls (type): The object class type
+
+    Returns:
+        list[str]: A list of string keys for the classes properties
+    """
+    props = []
+    for kls in cls.mro():
+        props += class_properties(kls)
+    
+    return props
```

### Comparing `altparse-0.2.1/src/altparse/ipautil/errors.py` & `altparse-0.3.0/src/altparse/ipautil/errors.py`

 * *Files identical despite different names*

### Comparing `altparse-0.2.1/src/altparse/ipautil/helpers.py` & `altparse-0.3.0/src/altparse/ipautil/helpers.py`

 * *Files identical despite different names*

### Comparing `altparse-0.2.1/src/altparse/model.py` & `altparse-0.3.0/src/altparse/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,103 +7,297 @@
 MIT License
 Copyright (c) 2022
 :------------------------------------------------------------------------------:
 """
 
 import json
 import logging
+from abc import ABC
+from functools import total_ordering
 from pathlib import Path
 
+from packaging import version
+
 from altparse.errors import *
-from altparse.helpers import fmt_github_datetime, utcnow, parse_github_datetime
-from altparse.ipautil.helpers import extract_sha256, download_tempfile
+from altparse.helpers import (all_class_properties, fmt_github_datetime,
+                              parse_github_datetime, utcnow, equal_ignore_order)
+from altparse.ipautil.helpers import download_tempfile, extract_sha256 
+from altparse.ipautil.core import extract_permissions
 
 # Create a helper class in the namespace that acts as an intermediary to the logging.info to optionally silence the AltSource creation help text
 # OR remove the info help text from the model entirely and place in the cli instead
 
-class AltSource:
-    class App:
-        class Permission:
-            _validTypes = ["photos", "camera", "location", "contacts", "reminders", "music", "microphone", "speech-recognition", "background-audio", "background-fetch", "bluetooth", "network", "calendars", "faceid", "siri", "motion"]
-            _requiredKeys = ["type", "usageDescription"]
+
+class Base(ABC):
+    _src = {}
+    _required_keys = []
+    _deprecated_keys = []
+    
+    def __eq__(self, other):
+        if isinstance(other, self.__class__):
+            for key in all_class_properties(self.__class__):
+                if key in self._deprecated_keys: continue
+                value = getattr(self, key)
+                other_value = getattr(other, key)
+                if isinstance(value, list) and equal_ignore_order(value, other_value): return False
+                elif getattr(self, key) != getattr(other, key): return False
+            return True
+        return NotImplemented
+
+    def __iter__(self):
+        for key in all_class_properties(self.__class__):
+            if key in self._deprecated_keys: continue
+            value = getattr(self, key)
+            if value is None: continue
+            if isinstance(value, list) and len(value)>0 and issubclass(value[0].__class__, Base): 
+                yield (key, [dict(item) for item in value])
+            elif issubclass(value.__class__, Base):  yield (key, dict(value))
+            else: yield (key, value)
+            
+    def __str__(self):
+        return str(dict(self))
+
+class AltSource(Base):
+    class App(Base):
+        
+        class Permissions(Base):
+            class Entitlement(Base):
+                _required_keys = ["name"]
+                
+                def __init__(self, src: dict[str] | None = None):
+                    if src is not None:
+                        self._src = src
+                        
+                        missing_keys = self.missing_keys()
+                        if missing_keys:
+                            logging.warning(f"Missing required AltSource.App.Entitlement keys: {missing_keys}")
+                    else:
+                        logging.info(f"Brand new AltSource.App.Entitlement created. Please remember to set the following properties: {self._required_keys}")
+                        self._src = {}
+                
+                def to_dict(self) -> dict[str]:
+                    ret = self._src.copy()
+                    ret = {k:v for (k,v) in ret.items() if ret.get(k) is not None}
+                    return ret
+                
+                def missing_keys(self) -> list[str]:
+                    """Checks to see if the Entitlement has all the required values and returns the missing keys.
+                    
+                    Note that if the list is empty, it will evaluate as False.
+
+                    Returns:
+                        list[str]: The list of required keys that are missing. If the Entitlement is valid, the list will be empty.
+                    """
+                    missing_keys = list()
+                    for key in self._required_keys:
+                        if key not in self._src.keys():
+                            missing_keys.append(key)
+                    return missing_keys
+                
+                def is_valid(self) -> bool:
+                    """Checks to see if the AltSource.App.Entitlement is valid and contains all the required information.
+
+                    Returns:
+                        bool: True if the `Entitlement` is a valid AltSource.App.Entitlement.
+                    """
+                    return not self.missing_keys()
+                
+                @property 
+                def name(self) -> str:
+                    return self._src.get("name")
+                @name.setter
+                def name(self, value: str):
+                    self._src["name"] = value
+            # End class Entitlement
+            class Privacy(Base):
+                # this is not an all-inclusive list, but is the most common privacy permissions that an app can request / utilize
+                _valid_types = ["BluetoothAlways", "BluetoothPeripheral", "Calendars", "Reminders", "Camera", "Microphone", "Contacts", "FaceID", "DesktopFolder", "DocumentsFolder", "DownloadsFolder", "NetworkVolumes", "RemovableVolumes", "FileProviderDomain", "GKFriendList", "HealthClinicalHealthRecordsShare", "HealthShare", "HealthUpdate", "HomeKit", "LocationAlwaysAndWhenInUse", "Location", "LocationWhenInUse", "LocationAlways", "AppleMusic", "Motion", "FallDetection", "LocalNetwork", "NearbyInteraction", "NearbyInteractionAllowOnce", "NFCReader", "PhotoLibraryAdd", "PhotoLibrary", "UserTracking", "AppleEvents", "SystemAdministration", "SensorKit", "Siri", "SpeechRecognition", "VideoSubscriberAccount", "Identity"]
+                _required_keys = ["name", "usageDescription"]
+                
+                def __init__(self, src: dict[str] | None = None):
+                    if src is not None:
+                        self._src = src
+                        missing_keys = self.missing_keys()
+                        if missing_keys:
+                            logging.warning(f"Missing required AltSource.App.Permissions.Privacy keys: {missing_keys}")
+                        if not self.is_valid_type():
+                            logging.warning(f"Privacy name not found in valid types.")
+                    else:
+                        logging.info(f"Brand new AltSource.App.Permissions.Privacy created. Please remember to set the following properties: {self._required_keys}")
+                        self._src = {}
+                
+                def to_dict(self) -> dict[str]:
+                    ret = self._src.copy()
+                    ret = {k:v for (k,v) in ret.items() if ret.get(k) is not None}
+                    return ret
+                
+                def missing_keys(self) -> list[str]:
+                    """Checks to see if the PrivacyPermission has all the required values and returns the missing keys.
+                    
+                    Note that if the list is empty, it will evaluate as False.
+
+                    Returns:
+                        list[str]: The list of required keys that are missing. If the PrivacyPermission is valid, the list will be empty.
+                    """
+                    missing_keys = list()
+                    for key in self._required_keys:
+                        if key not in self._src.keys():
+                            missing_keys.append(key)
+                    return missing_keys
+                
+                def is_valid(self) -> bool:
+                    """Checks to see if the AltSource.App.PrivacyPermission is valid and contains all the required information.
+
+                    Returns:
+                        bool: True if the `PrivacyPermission` is a valid AltSource.App.PrivacyPermission.
+                    """
+                    return not self.missing_keys()
+                
+                def is_valid_type(self) -> bool:
+                    """Checks to see if the PrivacyPermission name is a valid type.
+
+                    Returns:
+                        bool: True if the listed name is valid
+                    """
+                    return self.name in self._valid_types
+                
+                @property 
+                def name(self) -> str:
+                    return self._src.get("name")
+                @name.setter
+                def name(self, value: str):
+                    if value not in self._valid_types:
+                        logging.warning("PrivacyPermission name is not found in the list of valid types.")
+                    self._src["name"] = value
+                    
+                @property 
+                def usageDescription(self) -> str:
+                    return self._src.get("usageDescription")
+                @usageDescription.setter
+                def usageDescription(self, value: str):
+                    self._src["usageDescription"] = value
+            # End class Privacy
             
-            def __init__(self, src: dict[str] | None = None):
+            _required_keys = []
+            
+            def __init__(self, src: dict[str,list] | None = None):
                 if src is not None:
                     self._src = src
-                    if not all(x in src.keys() for x in self._requiredKeys):
-                        logging.warning(f"Missing required AltSource.App.Permission keys. Must have both `type` and `usageDescription`.")
-                    if "type" in src.keys() and not self.is_valid_type():
-                        logging.warning(f"Permission type not found in valid permission types.")
+                    if "entitlements" in src.keys():
+                        self._src["entitlements"] = [AltSource.App.Permissions.Entitlement(title) for title in src["entitlements"]]
+                    if "privacy" in src.keys():
+                        self._src["privacy"] = [AltSource.App.Permissions.Privacy(perm) for perm in src["privacy"]]
+                        
+                    missing_keys = self.missing_keys()
+                    if missing_keys:
+                        logging.warning(f"Missing required AltSource.App.Permissions keys: {missing_keys}")
                 else:
-                    logging.info(f"Brand new AltSource.App.Permission created. Please remember to set the following properties: {self._requiredKeys}")
-                    src = {}
+                    logging.info(f"Brand new AltSource.App.Permissions created. Please remember to add all the entitlements and privacy permissions that your app uses.")
+                    self._src = {
+                        "entitlements": [],
+                        "privacy": []
+                    }
             
             def to_dict(self) -> dict[str]:
                 ret = self._src.copy()
+                if "entitlements" in self._src.keys():
+                    ret["entitlements"] = [title.to_dict() for title in self.entitlements]
+                if "privacy" in self._src.keys():
+                    ret["privacy"] = [perm.to_dict() for perm in self.privacy]
                 ret = {k:v for (k,v) in ret.items() if ret.get(k) is not None}
                 return ret
             
             def missing_keys(self) -> list[str]:
-                """Checks to see if the Permission has all the required values and returns the missing keys.
+                """Checks to see if the Permissions has all the required values and returns the missing keys.
                 
                 Note that if the list is empty, it will evaluate as False.
 
                 Returns:
-                    list[str]: The list of required keys that are missing. If the Permission is valid, the list will be empty.
+                    list[str]: The list of required keys that are missing. If the Permissions is valid, the list will be empty.
                 """
                 missing_keys = list()
-                for key in self._requiredKeys:
+                for key in self._required_keys:
                     if key not in self._src.keys():
                         missing_keys.append(key)
                 return missing_keys
             
             def is_valid(self) -> bool:
-                """Checks to see if the AltSource.App.Permission is valid and contains all the required information.
+                """Checks to see if the AltSource.App.Permissions is valid and contains all the required information.
 
                 Returns:
-                    bool: True if the `Permission` is a valid AltSource.App.Permission.
+                    bool: True if the `Permissions` is a valid AltSource.App.Permissions.
                 """
-                return not self.missing_keys() and self.is_valid_type()
-            
-            def is_valid_type(self) -> bool:
-                """Checks to see if the Permission type is valid.
-
-                Returns:
-                    bool: True if the listed type is valid
-                """
-                return self._src.get("type") in self._validTypes
+                return not self.missing_keys()
             
             @property 
-            def type(self) -> str:
-                return self._src.get("type")
-            @type.setter
-            def type(self, value: str):
-                if value in self._validTypes:
-                    self._src["type"] = value
-                else:
-                    raise ValueError("Invalid permission type.")
+            def entitlements(self) -> list[Entitlement]:
+                return self._src.get("entitlements",[])
+            @entitlements.setter
+            def entitlements(self, value: list[Entitlement]):
+                if self.entitlements is not None:
+                    logging.warning(f"Entire `entitlements` section has been replaced.")
+                self._src["entitlements"] = value
                 
             @property 
-            def usageDescription(self) -> str:
-                return self._src.get("usageDescription")
-            @usageDescription.setter
-            def usageDescription(self, value: str):
-                self._src["usageDescription"] = value
-        # End class Permission
-        class Version:
-            _requiredKeys = ['version', 'date', 'downloadURL', 'size']
+            def privacy(self) -> list[Privacy]:
+                return self._src.get("privacy",[])
+            @privacy.setter
+            def privacy(self, value: list[Privacy]):
+                if self.privacy is not None:
+                    logging.warning(f"Entire `privacy` section has been replaced.")
+                self._src["privacy"] = value
+        # End class Permissions
+        
+        @total_ordering
+        class Version(Base):
+            _required_keys = ['version', 'date', 'downloadURL', 'size']
             
             def __init__(self, src: dict[str] | None = None):
                 if src is not None:
                     self._src = src
-                    if not all(x in src.keys() for x in self._requiredKeys):
-                        logging.warning(f"Missing required AltSource.App.Permission keys.")
+                    missing_keys = self.missing_keys()
+                    if missing_keys:
+                        logging.warning(f"Missing required AltSource.App.Version keys: {missing_keys}")
                 else:
-                    logging.info(f"Brand new AltSource.App.Version created. Please remember to set the following properties: {self._requiredKeys}")
-                    src = {}
+                    logging.info(f"Brand new AltSource.App.Version created. Please remember to set the following properties: {self._required_keys}")
+                    src = {
+                        "version": "",
+                        "date": "",
+                        "downloadURL": "",
+                        "size": 0
+                    }
+            
+            def __lt__(self, other):
+                if isinstance(other, self.__class__):
+                    if self.absoluteVersion is not None and other.absoluteVersion is not None:
+                        if version.parse(self.absoluteVersion) < version.parse(other.absoluteVersion): return True
+                        else: return False
+                    
+                    if (version.parse(self.version) < version.parse(other.version)): return True
+                    
+                    if (version.parse(self.version) == version.parse(other.version) and 
+                        self.buildVersion is not None and other.buildVersion is not None and 
+                        version.parse(self.buildVersion) < version.parse(other.buildVersion)): return True
+                    
+                    return False
+                return NotImplemented
+            
+            def __gt__(self, other):
+                if isinstance(other, self.__class__):
+                    if (self.absoluteVersion is not None and other.absoluteVersion is not None and 
+                        version.parse(self.absoluteVersion) > version.parse(other.absoluteVersion)): return True
+                    
+                    if (version.parse(self.version) > version.parse(other.version)): return True
+                    
+                    if (version.parse(self.version) == version.parse(other.version) and 
+                        self.buildVersion is not None and other.buildVersion is not None and 
+                        version.parse(self.buildVersion) > version.parse(other.buildVersion)): return True
+                    
+                    return False
+                return NotImplemented
             
             def to_dict(self) -> dict[str]:
                 ret = self._src.copy()
                 ret = {k:v for (k,v) in ret.items() if ret.get(k) is not None}
                 return ret
             
             def missing_keys(self) -> list[str]:
@@ -111,169 +305,196 @@
                 
                 Note that if the list is empty, it will evaluate as False.
 
                 Returns:
                     list[str]: The list of required keys that are missing. If the Version is valid, the list will be empty.
                 """
                 missing_keys = list()
-                for key in self._requiredKeys:
+                for key in self._required_keys:
                     if key not in self._src.keys():
                         missing_keys.append(key)
                 return missing_keys
             
             def is_valid(self) -> bool:
                 """Checks to see if the AltSource.App.Permission is valid and contains all the required information.
 
                 Returns:
                     bool: True if the `Permission` is a valid AltSource.App.Permission.
                 """
                 return not self.missing_keys()
             
-            def calculate_sha256(self):
-                """Calculates the sha256 hash based on the downloadURL object and sets the property.
+            def calculate_sha256(self, ipa_path: Path | None):
+                """Calculates the sha256 hash based on the downloadURL or passed `ipa_path` argument and sets the property.
                 """
                 if self.downloadURL is not None:
-                    ipa_path = download_tempfile(self.downloadURL)
+                    if ipa_path is None: 
+                        ipa_path = download_tempfile(self.downloadURL)
                     if ipa_path is not None:
                         self.sha256 = extract_sha256(ipa_path)
             
+            ### Unofficial property ###
+            @property 
+            def absoluteVersion(self) -> str:
+                return self._src.get("absoluteVersion")
+            @absoluteVersion.setter
+            def absoluteVersion(self, value: str):
+                self._src["absoluteVersion"] = value
+        
             @property 
             def version(self) -> str:
                 return self._src.get("version")
             @version.setter
             def version(self, value: str):
                 self._src["version"] = value
                 
             @property 
+            def buildVersion(self) -> str:
+                return self._src.get("buildVersion")
+            @buildVersion.setter
+            def buildVersion(self, value: str):
+                self._src["buildVersion"] = value
+                
+            @property 
             def date(self) -> str:
                 return self._src.get("date")
             @date.setter
             def date(self, value: str):
                 self._src["date"] = value
                 
             @property 
+            def localizedDescription(self) -> str:
+                return self._src.get("localizedDescription")
+            @localizedDescription.setter
+            def localizedDescription(self, value: str):
+                self._src["localizedDescription"] = value
+                
+            @property 
             def downloadURL(self) -> str:
                 return self._src.get("downloadURL")
             @downloadURL.setter
             def downloadURL(self, value: str):
                 self._src["downloadURL"] = value
                 
             @property 
-            def size(self) -> str:
+            def size(self) -> int:
                 return self._src.get("size")
             @size.setter
-            def size(self, value: str):
+            def size(self, value: int):
                 self._src["size"] = value
                 
             @property 
             def sha256(self) -> str:
                 return self._src.get("sha256")
             @sha256.setter
             def sha256(self, value: str):
                 self._src["sha256"] = value
                 
             @property 
-            def localizedDescription(self) -> str:
-                return self._src.get("localizedDescription")
-            @localizedDescription.setter
-            def localizedDescription(self, value: str):
-                self._src["localizedDescription"] = value
-
-            # Start unofficial AltSource properties
-            
+            def minOSVersion(self) -> str:
+                return self._src.get("minOSVersion")
+            @minOSVersion.setter
+            def minOSVersion(self, value: str):
+                self._src["minOSVersion"] = value
+                
             @property 
-            def buildVersion(self) -> str:
-                return self._src.get("buildVersion")
-            @buildVersion.setter
-            def buildVersion(self, value: str):
-                self._src["buildVersion"] = value
+            def maxOSVersion(self) -> str:
+                return self._src.get("maxOSVersion")
+            @maxOSVersion.setter
+            def maxOSVersion(self, value: str):
+                self._src["maxOSVersion"] = value
             
-            @property 
-            def absoluteVersion(self) -> str:
-                return self._src.get("absoluteVersion")
-            @absoluteVersion.setter
-            def absoluteVersion(self, value: str):
-                self._src["absoluteVersion"] = value
-
         # End class Version
         
-        _requiredKeys = ["name", "bundleIdentifier", "developerName", "versions", "localizedDescription", "iconURL"]
+        _required_keys = ["name", "bundleIdentifier", "developerName", "versions", "localizedDescription", "iconURL"]
+        _deprecated_keys = ["version", "versionDate", "versionDescription", "downloadURL", "size", "permissions"]
         
         def __init__(self, src: dict[str] | None = None):
-            if src is None:
-                logging.info(f"Brand new AltSource.App created. Please remember to set the following properties: {self._requiredKeys}")
-                self._src = {
-                    "name": "Example App", 
-                    "bundleIdentifier": "com.example.app", 
-                    "developerName": "Example.com", 
-                    "versions": [],
-                    "localizedDescription": "An app that is an example.",
-                    "iconURL": "https://example.com/icon.png"
-                    }
-            else:
+            if src is not None:
                 self._src = src
-                if "permissions" in src.keys():
-                    self._src["permissions"] = [self.Permission(perm) for perm in src["permissions"]]
+                if "appPermissions" in src.keys():
+                    self._src["appPermissions"] = AltSource.App.Permissions(src["appPermissions"])
                 if "versions" in src.keys():
                     self._src["versions"] = [AltSource.App.Version(ver) for ver in src["versions"]]
-                else: # create the first Version 
+                else: # create the first Version by attempting to convert from old AltSource API
                     self._src["versions"] = [AltSource.App.Version({
                         "version": src.get("version"),
                         "date": src.get("versionDate"),
                         "downloadURL": src.get("downloadURL"),
                         "localizedDescription": src.get("versionDescription"),
-                        "size": src.get("size"),
-                        "sha256": src.get("sha256"),
-                        "absoluteVersion": src.get("absoluteVersion")
+                        "size": src.get("size")
                     })]
+                    
                 missing_keys = self.missing_keys()
                 if missing_keys:
                     logging.warning(f"Missing required AltSource.App keys: {missing_keys}")
+            else:
+                logging.info(f"Brand new AltSource.App created. Please remember to update the following properties: {self._required_keys}")
+                self._src = {
+                    "name": "Example App",
+                    "appID": "com.example.app", 
+                    "bundleIdentifier": "com.example.app", 
+                    "developerName": "Example.com", 
+                    "versions": [AltSource.App.Version()],
+                    "localizedDescription": "An app that is an example.",
+                    "iconURL": "https://example.com/icon.png",
+                    "appPermissions": AltSource.App.Permissions({
+                        "entitlements": [],
+                        "privacy": []
+                    })
+                }
         
         def to_dict(self) -> dict[str]:
             ret = self._src.copy()
-            if "permissions" in self._src.keys():
-                ret["permissions"] = [perm.to_dict() for perm in self.permissions]
+            if "appPermissions" in self._src.keys():
+                ret["appPermissions"] = self.appPermissions.to_dict()
             if "versions" in self._src.keys():
                 ret["versions"] = [ver.to_dict() for ver in self.versions]
+            
             ret = {k:v for (k,v) in ret.items() if ret.get(k) is not None}
             return ret
         
         def missing_keys(self) -> list[str]:
             """Checks to see if the App has all the required values and returns the missing keys.
             
             Note that if the list is empty, it will evaluate as False.
 
             Returns:
                 list[str]: The list of required keys that are missing. If the App is valid, the list will be empty.
             """
             missing_keys = list()
-            for key in self._requiredKeys:
+            for key in self._required_keys:
                 if key not in self._src.keys():
                     missing_keys.append(key)
             return missing_keys
         
         def is_valid(self) -> bool:
             """Checks to see if the AltSource.App is valid and contains all the required information.
 
             Returns:
                 bool: True if the `App` is a valid AltSource.App.
             """
-            return not self.missing_keys()
+            valid_versions = self.versions is not None and len(self.versions) > 1 and all([version.is_valid() for version in self.versions])
+            
+            # Allow for old AltSource v1 API to be used
+            if not valid_versions:
+                valid_versions = self._src.get("version") is not None and self._src.get("downloadURL") is not None and self._src.get("versionDate") is not None
+            
+            valid_perms = self.appPermissions is None or self.appPermissions.is_valid()
+            return valid_versions and valid_perms and not self.missing_keys()
         
         def latest_version(self, use_dates: bool = False) -> Version:
             if use_dates:
                 return sorted(self.versions, key=lambda x: parse_github_datetime(x.date))[-1]
             return self.versions[0]
         
         def add_version(self, ver: Version):
-            versions_list = [ver.version for ver in self.versions]
-            if ver.version in versions_list:
-                logging.warning("Version already exists in AltSource. Automatically replaced with new one.")
-                self.versions[versions_list.index(ver.version)] = ver
+            versions_list = [(ver.version,ver.buildVersion) for ver in self.versions]
+            if (ver.version,ver.buildVersion) in versions_list:
+                logging.warning(f"Version already exists in {self.name}. Automatically replaced with new one.")
+                self.versions[versions_list.index((ver.version,ver.buildVersion))] = ver
             else:
                 self.versions.insert(0,ver)
             self._update_old_version_util(ver)
         
         def _update_old_version_util(self, ver: Version):
             """Takes an `AltSource.App.Version` and uses it to update all the original AltStore API 
                properties for managing updates. Utilize this method to maintain backwards compatibility.
@@ -310,23 +531,76 @@
         def subtitle(self) -> str:
             return self._src.get("subtitle")
         @subtitle.setter
         def subtitle(self, value: str):
             self._src["subtitle"] = value
             
         @property 
+        def localizedDescription(self) -> str:
+            return self._src.get("localizedDescription")
+        @localizedDescription.setter
+        def localizedDescription(self, value: str):
+            self._src["localizedDescription"] = value
+            
+        @property 
+        def iconURL(self) -> str:
+            return self._src.get("iconURL")
+        @iconURL.setter
+        def iconURL(self, value: str):
+            self._src["iconURL"] = value
+            
+        @property 
+        def tintColor(self) -> str:
+            return self._src.get("tintColor")
+        @tintColor.setter
+        def tintColor(self, value: str):
+            self._src["tintColor"] = value
+            
+        @property 
+        def screenshotURLs(self) -> list[str]:
+            return self._src.get("screenshotURLs")
+        @screenshotURLs.setter
+        def screenshotURLs(self, value: list[str]):
+            self._src["screenshotURLs"] = value
+        
+        @property 
         def versions(self) -> list[Version]:
-            return self._src.get("versions")
+            return self._src.get("versions",[])
         @versions.setter
         def versions(self, value: list[Version]):
             if self.versions is not None:
                 logging.warning(f"Entire `versions` section has been replaced for {self.name}.")
             self._src["versions"] = value
             
         @property 
+        def appPermissions(self) -> Permissions:
+            return self._src.get("appPermissions")
+        @appPermissions.setter
+        def appPermissions(self, value: Permissions):
+            self._src["appPermissions"] = value
+            
+        @property 
+        def beta(self) -> bool:
+            return self._src.get("beta")
+        @beta.setter
+        def beta(self, value: bool):
+            self._src["beta"] = value
+            
+        ### Deprecated properties ###
+        
+        @property 
+        def permissions(self) -> list[dict]:
+            logging.warning(f"Using deprecated v1 AltSource API.")
+            return self._src.get("permissions")
+        @permissions.setter
+        def permissions(self, value: list[dict]):
+            logging.warning(f"Using deprecated v1 AltSource API.")
+            self._src["permissions"] = value
+        
+        @property 
         def version(self) -> str:
             logging.warning(f"Using deprecated v1 AltSource API.")
             return self._src.get("version")
         @version.setter
         def version(self, value: str):
             logging.warning(f"Using deprecated v1 AltSource API.")
             self._src["version"] = value
@@ -355,64 +629,22 @@
             return self._src.get("downloadURL")
         @downloadURL.setter
         def downloadURL(self, value: str):
             logging.warning(f"Using deprecated v1 AltSource API.")
             self._src["downloadURL"] = value
             
         @property 
-        def localizedDescription(self) -> str:
-            return self._src.get("localizedDescription")
-        @localizedDescription.setter
-        def localizedDescription(self, value: str):
-            self._src["localizedDescription"] = value
-            
-        @property 
-        def iconURL(self) -> str:
-            return self._src.get("iconURL")
-        @iconURL.setter
-        def iconURL(self, value: str):
-            self._src["iconURL"] = value
-            
-        @property 
-        def tintColor(self) -> str:
-            return self._src.get("tintColor")
-        @tintColor.setter
-        def tintColor(self, value: str):
-            self._src["tintColor"] = value
-            
-        @property 
         def size(self) -> int:
+            logging.warning(f"Using deprecated v1 AltSource API.")
             return self._src.get("size")
         @size.setter
         def size(self, value: int):
+            logging.warning(f"Using deprecated v1 AltSource API.")
             self._src["size"] = value
             
-        @property 
-        def beta(self) -> bool:
-            return self._src.get("beta")
-        @beta.setter
-        def beta(self, value: bool):
-            self._src["beta"] = value
-            
-        @property 
-        def screenshotURLs(self) -> list[str]:
-            return self._src.get("screenshotURLs")
-        @screenshotURLs.setter
-        def screenshotURLs(self, value: list[str]):
-            self._src["screenshotURLs"] = value
-            
-        @property 
-        def permissions(self) -> list[Permission]:
-            return self._src.get("permissions")
-        @permissions.setter
-        def permissions(self, value: list[Permission]):
-            if self.permissions is not None:
-                logging.warning(f"Entire `permissions` section has been replaced for {self.name}.")
-            self._src["permissions"] = value
-            
         ### Additional properties that are not currently standard in AltSources ###
             
         @property 
         def appID(self) -> str:
             return self._src.get("appID")
         @appID.setter
         def appID(self, value: str):
@@ -420,20 +652,20 @@
                 raise ArgumentTypeError("AltSource.App.appID cannot be set to any type other than str.")
             if self._src.get("appID") is not None:
                 logging.warning(f"App `appID` changed from {self._src['appID']} to {value}.")
             self._src["appID"] = value
             
     # End class App
     
-    class Article:
-        _requiredKeys = ["title", "identifier", "caption", "date"]
+    class Article(Base):
+        _required_keys = ["title", "identifier", "caption", "date"]
         
         def __init__(self, src: dict | None = None):
             if src is None:
-                logging.info(f"Brand new AltSource.Article created. Please remember to set the following properties: {self._requiredKeys}")
+                logging.info(f"Brand new AltSource.Article created. Please remember to set the following properties: {self._required_keys}")
                 self._src = {"title": "Example Article Title", "identifier": "com.example.article", "caption": "Provoking example caption.", "date": fmt_github_datetime(utcnow())}
             else:
                 self._src = src
                 missing_keys = self.missing_keys()
                 if missing_keys:
                     logging.warning(f"Missing required AltSource.Article keys: {missing_keys}")
             
@@ -447,15 +679,15 @@
             
             Note that if the list is empty, it will evaluate as False.
 
             Returns:
                 list[str]: The list of required keys that are missing. If the `Article` is valid, the list will be empty.
             """
             missing_keys = list()
-            for key in self._requiredKeys:
+            for key in self._required_keys:
                 if key not in self._src.keys():
                     missing_keys.append(key)
             return missing_keys
         
         def is_valid(self) -> bool:
             """Checks to see if the AltSource.Article is valid and contains all the required information.
 
@@ -468,97 +700,95 @@
         def title(self) -> str:
             return self._src.get("title")
         @title.setter
         def title(self, value: str):
             self._src["title"] = value
             
         @property 
-        def name(self) -> str:
-            return self._src.get("name")
-        @name.setter
-        def name(self, value: str):
-            self._src["name"] = value
-            
-        @property 
-        def newsID(self) -> str:
+        def identifier(self) -> str:
             return self._src.get("identifier")
-        @newsID.setter
-        def newsID(self, value: str):
+        @identifier.setter
+        def identifier(self, value: str):
             logging.warning(f"Article `identifier` changed from {self._src['identifier']} to {value}.")
             self._src["identifier"] = value
             
         @property 
         def caption(self) -> str:
             return self._src.get("caption")
         @caption.setter
         def caption(self, value: str):
             self._src["caption"] = value
             
         @property 
+        def date(self) -> str:
+            return self._src.get("date")
+        @date.setter
+        def date(self, value: str):
+            self._src["date"] = value
+            
+        @property 
         def tintColor(self) -> str:
             return self._src.get("tintColor")
         @tintColor.setter
         def tintColor(self, value: str):
             self._src["tintColor"] = value
             
         @property 
         def imageURL(self) -> str:
             return self._src.get("imageURL")
         @imageURL.setter
         def imageURL(self, value: str):
             self._src["imageURL"] = value
             
         @property 
-        def appID(self) -> str:
-            return self._src.get("appID")
-        @appID.setter
-        def appID(self, value: str):
-            self._src["appID"] = value
-            
-        @property 
-        def date(self) -> str:
-            return self._src.get("date")
-        @date.setter
-        def date(self, value: str):
-            self._src["date"] = value
-            
-        @property 
         def notify(self) -> bool:
             return self._src.get("notify")
         @notify.setter
         def notify(self, value: bool):
             self._src["notify"] = value
             
         @property 
         def url(self) -> str:
             return self._src.get("url")
         @url.setter
         def url(self, value: str):
             self._src["url"] = value
+            
+        @property 
+        def appID(self) -> str:
+            return self._src.get("appID")
+        @appID.setter
+        def appID(self, value: str):
+            self._src["appID"] = value
     # End class Article
     
-    _requiredKeys = ["name", "identifier", "apps"]
+    _required_keys = ["name", "identifier", "apps"]
     
     def __init__(self, src: dict | None = None, path: str | Path | None = None):
         """Create new AltSource object. If a src is included, all properties will be retained regardless of use in a 
             standard AltSource. This will *not* load the data from path. Use the `altsource_from_file` method for that.
 
         Args:
             src (dict, optional): the direct serialization of an AltSource json file. Defaults to None.
             path (str | Path, optional): the filepath to which a physical version of the AltSource should be stored. Defaults to None.
         """
-        if src is None:
-            self._src = {"name": "ExampleSourceName", "identifier": "com.example.identifier", "apps": [], "version": 2}
-            logging.info(f"Brand new AltSource created. Please remember to set the following properties: {self._requiredKeys}")
-        else:
+        if src is not None:
             self._src = src
-            self._src["apps"] = [self.App(app) for app in src["apps"]]
+            self._src["apps"] = [self.App(app) for app in src.get("apps", [])]
             if "news" in self._src.keys():
                 self._src["news"] = [self.Article(art) for art in src["news"]]
-            self.version = 2 # set current API version
+            self.apiVersion = "v2" # set current API version
+            
+            missing_keys = self.missing_keys()
+            if missing_keys:
+                logging.warning(f"Missing required AltSource keys: {missing_keys}")
+        else:
+            self._src = {"name": "ExampleSourceName", "identifier": "com.example.identifier", "apps": [], "version": 2}
+            logging.info(f"Brand new AltSource created. Please remember to set the following properties: {self._required_keys}")
+            
         if path:
             if isinstance(path, str):
                 self.path = Path(path)
             self.path = path
         else:
             self.path = None
     
@@ -575,21 +805,28 @@
         
         Note that if the list is empty, it will evaluate as False.
 
         Returns:
             list[str]: The list of required keys that are missing. If the `AltSource` is valid, the list will be empty.
         """
         missing_keys = list()
-        for key in self._requiredKeys:
+        for key in self._required_keys:
             if key not in self._src.keys():
                 missing_keys.append(key)
         return missing_keys
     
     def is_valid(self):
-        return not self.missing_keys()
+        """Checks to see if the AltSource is valid and contains all the required information.
+
+            Returns:
+                bool: True if object is a valid AltSource.
+        """
+        valid_apps = all([app.is_valid() for app in self.apps])
+        valid_news = self.news is None or all([article.is_valid() for article in self.news])
+        return valid_apps and valid_news and not self.missing_keys()
     
     @property 
     def name(self) -> str:
         return self._src.get("name")
     @name.setter
     def name(self, value: str):
         self._src["name"] = value
@@ -598,20 +835,71 @@
     def identifier(self) -> str:
         return self._src.get("identifier")
     @identifier.setter
     def identifier(self, value: str):
         logging.warning(f"Source `identifier` changed from {self._src['identifier']} to {value}.")
         self._src["identifier"] = value
         
+    ### Unofficial AltSource property ###
     @property 
-    def sourceURL(self) -> str:
-        return self._src.get("sourceURL")
-    @sourceURL.setter
-    def sourceURL(self, value: str):
-        self._src["sourceURL"] = value
+    def apiVersion(self) -> str:
+        """Used to declare the AltSource API version."""
+        return self._src.get("apiVersion")
+    @apiVersion.setter
+    def apiVersion(self, value: str):
+        self._src["apiVersion"] = value
+    
+    @property 
+    def subtitle(self) -> str:
+        return self._src.get("subtitle")
+    @subtitle.setter
+    def subtitle(self, value: str):
+        self._src["subtitle"] = value
+        
+    @property 
+    def description(self) -> str:
+        return self._src.get("description")
+    @description.setter
+    def description(self, value: str):
+        self._src["description"] = value
+        
+    @property 
+    def iconURL(self) -> str:
+        return self._src.get("iconURL")
+    @iconURL.setter
+    def iconURL(self, value: str):
+        self._src["iconURL"] = value
+    
+    @property 
+    def headerURL(self) -> str:
+        return self._src.get("headerURL")
+    @headerURL.setter
+    def headerURL(self, value: str):
+        self._src["headerURL"] = value
+        
+    @property 
+    def website(self) -> str:
+        return self._src.get("website")
+    @website.setter
+    def website(self, value: str):
+        self._src["website"] = value
+        
+    @property 
+    def tintColor(self) -> str:
+        return self._src.get("tintColor")
+    @tintColor.setter
+    def tintColor(self, value: str):
+        self._src["tintColor"] = value
+        
+    @property 
+    def featuredApps(self) -> list[str]:
+        return self._src.get("featuredApps")
+    @featuredApps.setter
+    def featuredApps(self, value: list[str]):
+        self._src["featuredApps"] = value
     
     @property 
     def apps(self) -> list[App]:
         return self._src.get("apps")
     @apps.setter
     def apps(self, value: list[App]):
         logging.warning("Entire `apps` section has been replaced.")
@@ -622,31 +910,20 @@
         return self._src.get("news")
     @news.setter
     def news(self, value: list[Article]):
         if self.news is not None:
             logging.warning("Entire `news` section has been replaced.")
         self._src["news"] = value
         
-    # Start unofficial AltSource attributes.
-    
     @property 
-    def sourceIconURL(self) -> str:
-        return self._src.get("sourceIconURL")
-    @sourceIconURL.setter
-    def sourceIconURL(self, value: str):
-        self._src["sourceIconURL"] = value
-    
-    @property 
-    def version(self) -> str:
-        """Used to declare the AltSource API version.
-        """
-        return self._src.get("version")
-    @version.setter
-    def version(self, value: str):
-        self._src["version"] = value
+    def userinfo(self) -> dict:
+        return self._src.get("userinfo")
+    @userinfo.setter
+    def userinfo(self, value: dict):
+        self._src["userinfo"] = value
 # End class AltSource
 
 def altsource_from_file(filepath: Path | str) -> AltSource:
     """Loads an AltSource json into the Python object
 
     Args:
         filepath (Path | str): the filepath of an AltSource json. Will search for file in current working directory if only given a string
@@ -654,7 +931,15 @@
     if not isinstance(filepath, Path):
         try:
             filepath = next(Path.cwd().rglob(filepath))
         except StopIteration:
             raise FileNotFoundError(f"{filepath} not found in current working directory.")
     with open(filepath, "r", encoding="utf-8") as fp:
         return AltSource(json.load(fp), filepath)
+    
+def update_props_from_new_version(app: AltSource.App, new_ver: AltSource.App.Version):
+    if new_ver.sha256 is None or app.appPermissions is None:
+        ipa_path = download_tempfile(new_ver.downloadURL)
+        logging.debug(f"Updating {app.name} sha256 checksum.")
+        new_ver.calculate_sha256(ipa_path)
+        logging.debug(f"Collecting {app.name} entitlements and privacy permissions.")
+        app.appPermissions = AltSource.App.Permissions(extract_permissions(ipa_path=ipa_path))
```

### Comparing `altparse-0.2.1/src/altparse/parsers.py` & `altparse-0.3.0/src/altparse/parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                 path = Path(filepath)
                 with open(path, "r", encoding="utf-8") as fp:
                     self.src = AltSource(json.load(fp))
             except Exception as err:
                 raise ArgumentTypeError("Filepath must be a path-like object or a url.")
 
         if not self.src.is_valid():
-            raise AltSourceError("Invalid source formatting.")
+            logging.warning("Invalid source formatting.")
 
     def parse_apps(self, ids: list[str | dict[str, str]] | None = None) -> list[AltSource.App]:
         """Takes a provided list of ids that are `str` provided that `appID` is intended to be equal to `bundleIdentifier` or are type `dict` in the case that they are not the same value. The dict key will be the id being parsed from the other source, assumably the `bundleIdentifier` (but if an `appID` does exist, it will prioritize that) and the predetermined `appID` will be the value. It will then ensure every app has a unique `appID` before returning the list of Apps. This allows the user to change the appID of an app when they parse it.
 
         Args:
             ids (list[str | dict] | None, optional): _description_. Defaults to None.
 
@@ -79,15 +79,15 @@
         id_conv_tbl = gen_id_parse_table(ids)
         
         for app in self.src.apps:
             if app.is_valid():
                 id = app.appID or app.bundleIdentifier
                 if id in processed_keys: # appID / bundleID already exists in list of apps processed (meaning there's a duplicate)
                     index = processed_keys.index(id)
-                    if version.parse(processed_apps[index].versions[0].version) > version.parse(app.versions[0].version):
+                    if processed_apps[index].versions[0] > app.versions[0]:
                         continue
                     else:
                         processed_apps[index] = app
                 elif ids is None or id in fetch_ids:
                     processed_apps.append(app)
                 else:
                     continue # app is not going to be included
@@ -96,15 +96,15 @@
                     if ids is None or id in ids:
                         app.appID = app.bundleIdentifier
                     else:
                         app.appID = id_conv_tbl[app.bundleIdentifier]
                         
                 processed_keys.append(id)
             else:
-                logging.warning(f"Failed to parse invalid app: {app.name}")
+                logging.error(f"Failed to parse invalid app: {app.name}")
             
         # determine if any listed keys were not found in the source
         if len(processed_keys) < len(fetch_ids):
             missing_ids = set([pid for pid in fetch_ids if pid not in processed_keys])
             logging.warning(f"Requested ids not found in AltSource ({self.src.name}): {missing_ids}")
         return processed_apps
 
@@ -112,15 +112,15 @@
         processed_news = list()
         if self.src.news is None:
             return processed_news
         for article in self.src.news:
             if article.is_valid():
                 if ids is None:
                     processed_news.append(article)
-                elif article.newsID in ids:
+                elif article.identifier in ids:
                     processed_news.append(article)
         return processed_news
 
 class Unc0verParser:
     def __init__(self, url: str = "https://unc0ver.dev/releases.json", ver_parse: Callable = lambda x: x.lstrip("v"), prefer_date: bool = False, **kwargs):
         """Create a new Unc0verParser object that can be used to generate an AltSource.App using the Unc0ver team's personal json release data.
 
@@ -137,33 +137,35 @@
 
         if prefer_date:
             self.data = sorted(releases, key=lambda x: parse_github_datetime(x["published_at"]))[-1] # only grab the most recent release
         else:
             self.data = sorted(releases, key=lambda x: version.parse(x["tag_name"]))[-1] # only grab the release with the highest version
 
     @property
+    def downloadURL(self) -> str:
+        return "https://unc0ver.dev" + self.data["browser_download_url"]
+
+    @property
     def version(self) -> str:
         return self.data["tag_name"]
 
     @property
     def versionDate(self) -> str:
         return self.data["published_at"]
 
     @property
     def versionDescription(self) -> str:
         return "# " + self.data["name"] + "\n\n" + self.data["body"]
 
     def get_asset_metadata(self) -> dict[str]:
         """Returns a dictionary containing the downloadURL, size, bundleID, version
         """
-        download_url = "https://unc0ver.dev" + self.data["browser_download_url"]
-        ipa_path = download_tempfile(download_url)
+        ipa_path = download_tempfile(self.downloadURL)
         if ipa_path is not None:
             metadata = extract_altstore_metadata(ipa_path)
-        metadata["downloadURL"] = download_url
         return metadata
 
 class GithubParser:
     def __init__(self, url: str | None = None, repo_author: str | None = None, repo_name: str | None = None, ver_parse: Callable = lambda x: x.lstrip("v"), include_pre: bool = False, prefer_date: bool = False, asset_regex: str = r".*\.ipa", extract_twice: bool = False, upload_ipa_repo: Release | None = None, **kwargs):
         """Create a new GithubParser object that can be used to generate an AltSource.App.
         
         Supply either the api url explicitly or the repo_author and repo_name to automatically find the api url.
@@ -194,46 +196,66 @@
                 raise GitHubError("Github Repo not found.")
             elif releases.get("message").startswith("API rate limit exceeded"):
                 raise GitHubError("Github API rate limit has been exceeded for this hour.")
             else:
                 raise GitHubError("Github API issue: " + releases.get("message"))
 
         #### Helper methods ####
-        def match_asset(release):
+        def match_asset(release: dict):
+            """Uses asset_regex to find matching GitHub assets, then selects the most recent one and saves it to the key `asset`"""
             assets = list(filter(lambda x: re.fullmatch(self.asset_regex, x["name"]), release["assets"])) # filters assets to match asset_regex
+            if not assets: # there were no IPAs matching the regex
+                return
             asset = sorted(assets, key=lambda x: parse_github_datetime(x["updated_at"]))[-1] # gets most recently updated ipa
             release["asset"] = asset # set asset in the release to only be most recently IPA found
             
+        def filter_by_asset(releases: list[dict]) -> list[dict]:
+            """Uses asset_regex to remove any releases that don't contain a matching file"""
+            for x in releases: match_asset(x)
+            return list(filter(lambda x: x.get("asset") is not None, releases))
+            
+        def alter_tag_name(release: dict):
+            """Uses lambda function to convert the tag name to the Python packaging.version standard"""
+            release["tag_name"] = ver_parse(release["tag_name"])
+            
         def alter_tag_names(releases: list):
+            """Changes all release tag names to the Python packaging.version standard (otherwise it's removed)"""
             for index, release in enumerate(releases):
                 alter_tag_name(release)
                 ver = version.parse(release["tag_name"])
                 if isinstance(ver, version.LegacyVersion):
                     logging.warning(f"Invalid GitHub tag version not considered: {ver.base_version}")
                     releases.pop(index)
-
-        def alter_tag_name(release: dict):
-            release["tag_name"] = ver_parse(release["tag_name"])
         
         #### Parse the correct release ####
         if not include_pre:
             releases = list(filter(lambda x: x.get("prerelease") != True, releases)) # filter out prereleases
+            
+        # narrow down assets for all releases to make checking the asset timestamp easier
+        # by stripping out releases that don't match the asset_regex
+        releases = filter_by_asset(releases)
         if len(releases)==0:
             raise AltSourceError("No matching releases found.")
         if prefer_date:
             # narrow down assets for all releases to make checking the asset timestamp easier
-            for x in releases: match_asset(x)
+            # by stripping out releases that don't match the asset_regex
             self.data = sorted(releases, key=lambda x: parse_github_datetime(x["asset"]["updated_at"]))[-1] # only grab the most recent release
             alter_tag_name(self.data)
         else:
             # alter the github release tags to match AltStore version tags
             # strip out any invalid versions
             alter_tag_names(releases)
             self.data = sorted(releases, key=lambda x: version.parse(x["tag_name"]))[-1] # only grab the release with the highest version
-            match_asset(self.data)
+
+    @property
+    def downloadURL(self) -> str:
+        return self.data["asset"]["browser_download_url"]
+    @downloadURL.setter
+    def downloadURL(self, value: str):
+        self.data["asset"]["browser_download_url"] = value
 
     @property
     def version(self) -> str:
         return self.data["tag_name"]
 
     @property
     def versionDate(self) -> str:
@@ -245,28 +267,25 @@
 
     def get_asset_metadata(self) -> dict[str]:
         """Processes the most recently released ipa to get various internal metadata.
 
         Returns:
             dict: A dictionary containing the downloadURL, size, bundleID, version, and more.
         """
-        download_url = self.data["asset"]["browser_download_url"]
-
-        ipa_path = download_tempfile(download_url)
+        ipa_path = download_tempfile(self.downloadURL)
         if ipa_path is not None:
             payload_path = extract_ipa(ipa_path, self.extract_twice)
             if self.extract_twice:
                 ipa_path = payload_path.parent / "temp2.ipa"
             plist_path = list(payload_path.rglob("Info.plist"))[0] # locate the Info.plist path within the extracted data
             metadata = extract_altstore_metadata(ipa_path=ipa_path, plist_path=plist_path)
             
             # Uploads the ipa to a separate GitHub repository after its been processed
             if self.upload_ipa_repo is not None:
-                download_url = upload_ipa_github(ipa_path, self.upload_ipa_repo, name=metadata["bundleIdentifier"], ver=metadata["version"])
-        
-        metadata["downloadURL"] = download_url
+                self.downloadURL = upload_ipa_github(ipa_path, self.upload_ipa_repo, name=metadata["bundleIdentifier"], ver=metadata["version"])
+
         return metadata
 
 class Parser(Enum):
     ALTSOURCE = AltSourceParser
     GITHUB = GithubParser
     UNC0VER = Unc0verParser
```

### Comparing `altparse-0.2.1/src/altparse.egg-info/PKG-INFO` & `altparse-0.3.0/src/altparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altparse
-Version: 0.2.1
+Version: 0.3.0
 Summary: Designed to aid in creating and maintaining AltSources
 Author-email: Noah Keck <noahkeck@mindspring.com>
 License: MIT License
         
         Copyright (c) 2022 Noah Keck
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `altparse-0.2.1/src/altparse.egg-info/SOURCES.txt` & `altparse-0.3.0/src/altparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `altparse-0.2.1/tests/XPatcher_2.2.ipa` & `altparse-0.3.0/tests/XPatcher_2.2.ipa`

 * *Files identical despite different names*

### Comparing `altparse-0.2.1/tests/example_ipa_upload.py` & `altparse-0.3.0/tests/example_ipa_upload.py`

 * *Files identical despite different names*

### Comparing `altparse-0.2.1/tests/example_update.py` & `altparse-0.3.0/tests/example_update.py`

 * *Files identical despite different names*

### Comparing `altparse-0.2.1/tests/quantumsource.json` & `altparse-0.3.0/tests/quantumsource.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3816183740531554%*

 * *Differences: {"'apps'": "{4: {'versions': {0: {'sha256': "*

 * *           "'fe1eda29ab29ad408430934a35b9d46b08e10edd7eea50b072b2b54b16b1c182'}}, delete: "*

 * *           "['version', 'versionDate', 'versionDescription', 'downloadURL', 'size', 'permissions', "*

 * *           "'absoluteVersion']}, 5: {'versions': {0: {'sha256': "*

 * *           "'15868764789f1187ae3ed73cb7a3c9c599c9de18239a73f5cdd51fdfdcfda66d'}}, delete: "*

 * *           "['version', 'versionDate', 'versionDescription', 'downloadURL', 'size', "*

 * *           "'absoluteVersion' […]*

```diff
@@ -1,193 +1,298 @@
 {
     "apps": [
         {
-            "absoluteVersion": "1.0.1",
+            "bundleIdentifier": "com.worthdoingbadly.WDBRemoveThreeAppLimit",
+            "developerName": "Zhuowei",
+            "iconURL": "https://i.imgur.com/ODvSw7D.png",
+            "localizedDescription": "An app that removes the three app limit for free provisioning. Hit \"Go\" just before installing apps. Should work on iOS 16.1.2 and below / iOS 15.7.1 and below.\n\nThis is very limited:\n\n\u2022 Apps still expire after a week\n\u2022 They still do not get arbitrary entitlements\n\u2022 They still must be signed. It's probably not going to be that useful. It's meant more as a demo of what you can do with MacDirtyCow.",
+            "name": "WDBRemoveThreeAppLimit",
+            "screenshotURLs": [
+                "https://i.imgur.com/6pajtgW.png"
+            ],
+            "subtitle": "Removes three app limit from AltStore!",
+            "tintColor": "#404040",
+            "versions": [
+                {
+                    "date": "2023-02-16",
+                    "downloadURL": "https://github.com/zhuowei/WDBRemoveThreeAppLimit/releases/download/v1.0/WDBRemoveThreeAppLimit-v1.0.ipa",
+                    "localizedDescription": "\u2022 Updated WDBRemoveThreeAppLimit to v1.0",
+                    "sha256": "428982c14796e7caa66d2743964fa37157d0e9db574ada326aa09a65a11c147c",
+                    "size": 88800,
+                    "version": "1.0"
+                }
+            ]
+        },
+        {
+            "appID": "com.ginsudev.WDBFontOverwrite",
+            "bundleIdentifier": "com.ginsudev.WDBFontOverwrite",
+            "developerName": "Zhuowei + Ginsudev",
+            "iconURL": "https://i.imgur.com/SXK4rhS.png",
+            "localizedDescription": "An app that allows you to override the system used iOS font with one of the fonts from our built in selection. It's probably not going to be that useful. It's meant more as a demo of what you can do with MacDirtyCow.",
+            "name": "WDBFontOverwrite",
+            "screenshotURLs": [
+                "https://user-images.githubusercontent.com/704768/209511898-a1477b66-28e4-471a-87d9-36c1c2eb25ca.png",
+                "https://user-images.githubusercontent.com/704768/209606970-a382c273-bdcb-425c-bca1-1b6f9b31862f.png",
+                "https://user-images.githubusercontent.com/704768/209753262-b8204c92-b873-41a7-8127-38bf86096470.png"
+            ],
+            "subtitle": "Override the iOS system fonts!",
+            "tintColor": "#404040",
+            "versions": [
+                {
+                    "absoluteVersion": "1.10.8",
+                    "date": "2023-02-09T10:15:32Z",
+                    "downloadURL": "https://github.com/ginsudev/WDBFontOverwrite/releases/download/v1.10.8/WDBFontOverwrite.ipa",
+                    "localizedDescription": "# v1.10.8\n\n- Updated grant_full_disk_access.\r\n- Concurrency and code improvements/fixes.",
+                    "sha256": "c0247494c3852c200aeececaada8476b0967958154a28cfd260b21a9c20392ec",
+                    "size": 5348316,
+                    "version": "1.10.8"
+                }
+            ]
+        },
+        {
+            "appID": "com.rileytestut.Deltroid",
+            "bundleIdentifier": "com.rileytestut.Deltroid",
+            "developerName": "SideStore Team",
+            "iconURL": "https://i.imgur.com/Bimx1aO.png",
+            "localizedDescription": "Deltroid is an all-in-one emulator for iOS. Deltroid builds upon the strengths of its predecessor Delta while improving on it in a community supported fashion. \n\nGithub Repository (https://github.com/lonkelle/Deltroid) \n\nFEATURES\n\nSupported Game Systems\n\u2022 Nintendo Entertainment System\n\u2022 Super Nintendo Entertainment System\n\u2022 Nintendo 64\n\u2022 Game Boy (Color)\n\u2022 Game Boy Advance\n\u2022 Nintendo DS\n\u2022 Nintendo DSi\n\u2022 Sega Genesis\n\u2022 And plenty more to come!\n\nController Support\n\u2022 Supports PS4, PS5, Xbox One S, Xbox Series X, and MFi game controllers.\n\u2022 Supports bluetooth (and wired) keyboards, as well as the Apple Smart Keyboard.\n\u2022 Completely customize button mappings on a per-system, per-controller basis.\n\u2022 Map buttons to special \u201cQuick Save\u201d, \u201cQuick Load,\u201d and \u201cFast Forward\u201d actions.\n\nSave States\n\u2022 Save and load save states for any game from the pause menu.\n\u2022 Lock save states to prevent them from being accidentally overwritten.\n\u2022 Automatically makes backup save states to ensure you never lose your progress.\n\u2022 Support for \u201cQuick Saves,\u201d save states that can be quickly saved/loaded with a single button press (requires external controller).\n\nCheats\n\u2022 Supports various types of cheat codes for each supported system:\n\u2022 NES: Game Genie\n\u2022 SNES: Game Genie, Pro Action Replay\n\u2022 N64: GameShark\n\u2022 GBC: Game Genie, GameShark\n\u2022 GBA: Action Replay, Code Breaker, GameShark\n\u2022 DS: Action Replay\n\nDeltroid Sync\n\u2022 Sync your games, game saves, save states, cheats, controller skins, and controller mappings between devices.\n\u2022 View version histories of everything you sync and optionally restore them to earlier versions.\n\u2022 Supports both Google Drive and Dropbox.\n\nCustom Controller Skins\n\u2022 Beautiful built-in controller skins for all systems.\n\u2022 Import controller skins made by others, or even make your own to share with the world!\n\nHold Button\n\u2022 Choose buttons for Delta to hold down on your behalf, freeing up your thumbs to press other buttons instead.\n\u2022 Perfect for games that typically require one button be held down constantly (ex: run button in Mario games, or the A button in Mario Kart).\n\nFast Forward\n\u2022 Speed through slower parts of games by running the game much faster than normal.\n\u2022 Easily enable or disable from the pause menu, or optionally with a mapped button on an external controller.\n\n3D/Haptic Touch\n\u2022 Use 3D or Haptic Touch to \u201cpeek\u201d at games, save states, and cheat codes.\n\u2022 App icon shortcuts allow quick access to your most recently played games, or optionally customize the shortcuts to always include certain games.\n\nGame Artwork\n\u2022 Automatically displays appropriate box art for imported games.\n\u2022 Change a game\u2019s artwork to anything you want, or select from the built-in game artwork database.\n\nMisc.\n\u2022 Gyroscope support (WarioWare: Twisted! only)\n\u2022 Microphone support (DS only)\n\u2022 Support for delta:// URL scheme to jump directly into a specific game.\n\n**Deltroid and Sidestore are in no way affiliated with Nintendo. The name \"Nintendo\" and all associated game console names are registered trademarks of Nintendo Co., Ltd.**",
+            "name": "Deltroid",
+            "screenshotURLs": [
+                "https://user-images.githubusercontent.com/64176728/215964215-34cefad0-7178-4b38-930d-fc3df1c5592b.png",
+                "https://user-images.githubusercontent.com/64176728/215960133-70db5b84-d2e4-4638-9f96-179b9100aa9c.png",
+                "https://user-images.githubusercontent.com/64176728/215962679-1c01f62f-59ab-4e7f-9a2c-d1353fb409c6.png",
+                "https://user-images.githubusercontent.com/64176728/215960144-930836b3-543f-4729-8b6a-e06446aca4c4.png"
+            ],
+            "subtitle": "Multi-emulator for your classic games on the go!",
+            "tintColor": "8A28F7",
+            "versions": [
+                {
+                    "absoluteVersion": "0.9.1",
+                    "date": "2023-02-02T10:51:30Z",
+                    "downloadURL": "https://github.com/lonkelle/Deltroid/releases/download/v0.9.1/Deltroid.ipa",
+                    "localizedDescription": "# v0.9.1\n\n\u2022 Fixes default NES / DS skins\r\n\u2022 Fixes importing `.md` files from the in-app File Picker.",
+                    "sha256": "e7334a815833de25221675380d6774a3d2cb6df03fbd56caa80b0d6da553153b",
+                    "size": 48342198,
+                    "version": "1.5"
+                },
+                {
+                    "absoluteVersion": "0.1",
+                    "date": "2023-2-02T03:00:00-05:00",
+                    "downloadURL": "https://github.com/lonkelle/Deltroid/releases/download/v0.9.1/Deltroid.ipa",
+                    "localizedDescription": "Additions and Bugfixes. More info: https://github.com/lonkelle/Deltroid/releases",
+                    "size": 48300000,
+                    "version": "0.1"
+                }
+            ]
+        },
+        {
+            "appID": "com.vcmi.VCMI",
+            "bundleIdentifier": "eu.vcmi.vcmiclient",
+            "developerName": "VCMI Team",
+            "iconURL": "https://github.com/vcmi/vcmi/raw/develop/client/icons/vcmiclient.512x512.png",
+            "localizedDescription": "VCMI is a open source cross-platform HoMM3 engine written from scratch. \n\nYou need data copied from original game to play. \nFollow instructions from https://wiki.vcmi.eu/Installation_on_iOS",
+            "name": "VCMI",
+            "screenshotURLs": [
+                "https://raw.githubusercontent.com/vcmi/vcmi-updates/master/altstore/screenshots/screenshot1.png",
+                "https://raw.githubusercontent.com/vcmi/vcmi-updates/master/altstore/screenshots/screenshot2.png",
+                "https://raw.githubusercontent.com/vcmi/vcmi-updates/master/altstore/screenshots/screenshot3.png",
+                "https://raw.githubusercontent.com/vcmi/vcmi-updates/master/altstore/screenshots/screenshot4.png",
+                "https://raw.githubusercontent.com/vcmi/vcmi-updates/master/altstore/screenshots/screenshot5.png",
+                "https://raw.githubusercontent.com/vcmi/vcmi-updates/master/altstore/screenshots/screenshot6.png",
+                "https://raw.githubusercontent.com/vcmi/vcmi-updates/master/altstore/screenshots/screenshot7.png",
+                "https://raw.githubusercontent.com/vcmi/vcmi-updates/master/altstore/screenshots/screenshot8.png",
+                "https://raw.githubusercontent.com/vcmi/vcmi-updates/master/altstore/screenshots/screenshot9.png"
+            ],
+            "subtitle": "Heroes of Might & Magic III engine",
+            "tintColor": "CD8526",
+            "versions": [
+                {
+                    "absoluteVersion": "1.2.1",
+                    "date": "2023-04-28T18:40:12Z",
+                    "downloadURL": "https://github.com/vcmi/vcmi/releases/download/1.2.1/VCMI-1.2.1-iOS.ipa",
+                    "localizedDescription": "# VCMI 1.2.1\n\n### Player Changelog: [1.2.0 -> 1.2.1](https://github.com/vcmi/vcmi/blob/master/ChangeLog.md#120---121)\r\n\r\n### Full Changelog: https://github.com/vcmi/vcmi/compare/1.2.0...1.2.1\r\n\r\n<!-- ### Android release is available on [Google Play](https://play.google.com/store/apps/details?id=is.xyz.vcmi) -->\r\n### Ubuntu release is available on [VCMI PPA](https://launchpad.net/~vcmi/+archive/ubuntu/ppa)",
+                    "sha256": "7556bb42ca0afebad75be8ccf8a00a3121313178392f6ccb5a86059f060c3b00",
+                    "size": 26347869,
+                    "version": "1.2.1"
+                },
+                {
+                    "absoluteVersion": "1.2.0",
+                    "date": "2023-04-14T14:08:18Z",
+                    "downloadURL": "https://github.com/vcmi/vcmi/releases/download/1.2.0/VCMI-1.2.0-iOS.ipa",
+                    "localizedDescription": "# VCMI 1.2.0\n\n### Player Changelog: [1.1.1 -> 1.2](https://github.com/vcmi/vcmi/blob/master/ChangeLog.md#111---120)\r\n\r\n### Full Changelog: https://github.com/vcmi/vcmi/compare/1.1.1...1.2.0\r\n\r\n<!-- ### Android release is available on [Google Play](https://play.google.com/store/apps/details?id=is.xyz.vcmi) --->\r\n### Ubuntu release is available on [VCMI PPA](https://launchpad.net/~vcmi/+archive/ubuntu/ppa)\n\nNOTE: BundleIdentifier changed in this version and automatic updates have been disabled until manual install occurs.",
+                    "sha256": "8f1ea600a8156eae17de80f9f72a3cb38b4be9b087b276324192f797a3516511",
+                    "size": 26346303,
+                    "version": "1.2"
+                },
+                {
+                    "date": "2023-02-03T12:00:00+04:00",
+                    "downloadURL": "https://github.com/vcmi/vcmi/releases/download/1.1.1/VCMI-1.1.1-iOS.ipa",
+                    "localizedDescription": "Fixes for issues found in 1.1 release",
+                    "size": 25570455,
+                    "version": "1.1.1"
+                }
+            ]
+        },
+        {
             "bundleIdentifier": "com.ianclawson.DeltaPacEdition",
             "developerName": "Riley Testut & Ian Clawson",
-            "downloadURL": "https://github.com/ianclawson/Delta-iPac-Edition/releases/download/1.0.1/Delta-iPac.ipa",
             "iconURL": "https://i.imgur.com/OPkKmCO.png",
             "localizedDescription": "This version of Delta is essentially the base version of Delta, but with a large number of popular and highly anticipated Pull Requests merged in. Keep in mind there are some bugs and graphical glitches. Refer to https://github.com/ianclawson/Delta-iPac-Edition#readme for more details.",
             "name": "Delta iPac Edition",
-            "permissions": [
-                {
-                    "type": "photos",
-                    "usageDescription": "Allows Delta to use images from your Photo Library as game artwork."
-                }
-            ],
             "screenshotURLs": [
                 "https://user-images.githubusercontent.com/705880/65600448-f7d9be00-df54-11e9-9e3e-d4c31296da94.PNG",
                 "https://user-images.githubusercontent.com/705880/65813009-f2ae8600-e183-11e9-9eb7-704effc11173.png",
                 "https://user-images.githubusercontent.com/705880/65601117-58b5c600-df56-11e9-9c19-9a5ba5da54cf.PNG",
                 "https://user-images.githubusercontent.com/705880/65601125-5b182000-df56-11e9-9e7e-261480e893c0.PNG"
             ],
-            "size": 19765623,
             "subtitle": "A sneak peek preview of Delta!",
             "tintColor": "#8A28F7",
-            "version": "1",
-            "versionDate": "2021-11-19T19:13:13Z",
-            "versionDescription": "# iPac Edition Official Release\n\nOnly the IPA is included. The \"Source Code\" is merely the README.\r\n\r\nNew Features:\r\n* Optimized AirPlay Support\r\n* Local Mulitplayer (NES, SNES, N64, GEN)\r\n* Nintendo-Switch-Online-like Rewind\r\n* Additional MFi Inputs (L3, R3, Options, Home, and some PS/Xbox-specific inputs)\r\n* External Controller deadzones for analog inputs (allows analog sticks to work properly for d-pads)\r\n* External Controller connection now prevents game screen from rotating\r\n* SNES Audio no longer crackles\r\n* Bonus: Quick Saves now Sync",
             "versions": [
                 {
                     "absoluteVersion": "1.0.1",
                     "date": "2021-11-19T19:13:13Z",
                     "downloadURL": "https://github.com/ianclawson/Delta-iPac-Edition/releases/download/1.0.1/Delta-iPac.ipa",
                     "localizedDescription": "# iPac Edition Official Release\n\nOnly the IPA is included. The \"Source Code\" is merely the README.\r\n\r\nNew Features:\r\n* Optimized AirPlay Support\r\n* Local Mulitplayer (NES, SNES, N64, GEN)\r\n* Nintendo-Switch-Online-like Rewind\r\n* Additional MFi Inputs (L3, R3, Options, Home, and some PS/Xbox-specific inputs)\r\n* External Controller deadzones for analog inputs (allows analog sticks to work properly for d-pads)\r\n* External Controller connection now prevents game screen from rotating\r\n* SNES Audio no longer crackles\r\n* Bonus: Quick Saves now Sync",
+                    "sha256": "fe1eda29ab29ad408430934a35b9d46b08e10edd7eea50b072b2b54b16b1c182",
                     "size": 19765623,
                     "version": "1"
                 }
             ]
         },
         {
-            "absoluteVersion": "1.13.2",
             "appID": "org.ppsspp.ppsspp",
             "bundleIdentifier": "org.ppsspp.ppsspp",
             "developerName": "Henrik Rydg\u00e5rd",
-            "downloadURL": "https://github.com/QuarkSources/ppsspp-builder/releases/download/v1.13.2/PPSSPP_v1.13.2.ipa",
             "iconURL": "https://i.imgur.com/JP0Fncv.png",
             "localizedDescription": "PPSSPP can run your PSP games on your iPhone and iPad in full HD resolution. It can even upscale textures that would otherwise be too blurry as they were made for the small screen of the original PSP. Even on modern iPhones and iPads, you can often run at double the original resolution.",
             "name": "PPSSPP",
             "screenshotURLs": [
                 "https://i.imgur.com/CWl6GgH.png",
                 "https://i.imgur.com/SxmN1M0.png",
                 "https://i.imgur.com/sGWgR6z.png",
                 "https://i.imgur.com/AFKTdmZ.png"
             ],
-            "size": 14509458,
             "subtitle": "PlayStation Portable games on iOS.",
             "tintColor": "#21486b",
-            "version": "1.13.2",
-            "versionDate": "2022-09-18T23:59:49Z",
-            "versionDescription": "# v1.13.2\n\n",
             "versions": [
                 {
                     "absoluteVersion": "1.13.2",
                     "date": "2022-09-18T23:59:49Z",
                     "downloadURL": "https://github.com/QuarkSources/ppsspp-builder/releases/download/v1.13.2/PPSSPP_v1.13.2.ipa",
                     "localizedDescription": "# v1.13.2\n\n",
+                    "sha256": "15868764789f1187ae3ed73cb7a3c9c599c9de18239a73f5cdd51fdfdcfda66d",
                     "size": 14509458,
                     "version": "1.13.2"
                 }
             ]
         },
         {
-            "absoluteVersion": "1.5",
-            "bundleIdentifier": "com.firebird.firebird-emu",
+            "appID": "com.firebird.firebird-emu",
+            "bundleIdentifier": "com.adriweb.firebird-emu",
             "developerName": "nspire-emus",
-            "downloadURL": "https://github.com/nspire-emus/firebird/releases/download/v1.5/firebird-iOS.ipa",
             "iconURL": "https://i.imgur.com/U2HvZFZ.png",
             "localizedDescription": "Third-party multi-platform emulator of the ARM-based TI-Nspire calculators.",
             "name": "Firebird Emu",
             "screenshotURLs": [
                 "https://i.imgur.com/LT1u2bi.png"
             ],
-            "size": 9680896,
             "subtitle": "ARM-based TI-Nspire calculator.",
             "tintColor": "#010f00",
-            "version": "1.5",
-            "versionDate": "2020-03-28T14:25:34Z",
-            "versionDescription": "# A heap of improvements: Firebird 1.5\n\n**New features:**\r\n* UI language can be switched\r\n* The debugger has a command history, press Up and Down arrow keys\r\n* On Android, the system file picker is used now, which fixes \"Could not start the emulation\" in many cases\r\n* The color scheme follows the system now\r\n* Improved performance of CX flash access by ignoring certain cache flush requests\r\n\r\n**Improvements:**\r\n* LCD can be resized freely now\r\n* Performance improvements for the ARM and AArch64 JITs\r\n* Supports macOS 10.15 Catalina\r\n* The Android APK includes arm64-v8a now\r\n* The Windows ZIP includes software OpenGL now, so should work on more systems\r\n\r\n**Bugfixes:**\r\n* Fix the external LCD sometimes being invisible\r\n* Allows building with recent versions of the Android NDK with clang\r\n* Does not crash on exit due to use of incompatible compile flags with GCC\r\n* Android devices with a lower w/h ratio are marked as supported now\r\n* firebird-send supports different implementations of netcat now\r\n* GDB and remote debugger work after emulation autostart as well\r\n* Moving the cursor over keypad buttons no longer clicks\r\n* On Windows, the filename for snapshots can now include non-ASCII characters\r\n* Fix crash on emulation start on certain x86-64 systems\r\n* Fix freeze on exit on JIT builds for the iOS version\r\n\r\nNote: Firebird Emu requires Qt 5.9 now.\r\n\r\n_Repo for Arch, Debian, Fedora, Ubuntu and openSUSE: [via OBS](https://software.opensuse.org/download.html?project=home%3AVogtinator%3Afirebird-emu&package=firebird-emu&locale=en)._\r\n",
             "versions": [
                 {
+                    "absoluteVersion": "1.6",
+                    "date": "2023-01-07T16:36:46Z",
+                    "downloadURL": "https://github.com/nspire-emus/firebird/releases/download/v1.6/firebird-iOS.ipa",
+                    "localizedDescription": "# New year, new version: Firebird 1.6\n\n**New features:**\r\n* New dialog for creating Flash images, which is also available in the Mobile UI! (#262) \r\n* Running as 64bit application on Windows is supported now (#234)\r\n* Polish translation is available now (#207)\r\n* CX II (/-T/CAS) calculators can now be emulated (#165)! However, with the current dumping programs you will not get a complete bootrom and booting the OS will fail.\r\n\r\n**Improvements:**\r\n* Multiple files can be sent in the Mobile UI and by dropping them into the main window on desktop (#279)\r\n Reimplemented emulation speed control: Now it's more accurate, especially on Windows\r\n* GitHub actions now performs automated builds for Android (armeabi-v7a and arm64-v8a in one APK), macOS and Windows (32bit and 64bit) on releases and pull requests (#283, #284, #285)\r\n* The \"installer\" for OS 4.5.3.14 (and later?) works now. It requires [fastboot RAM](https://hackspire.org/index.php?title=Memory-mapped_I/O_ports_on_CX#90030000_-_Fastboot_RAM) to persist state across reboots, which is now implemented.\r\n* More accurate emulation of the On button: It's now possible to enter Press-To-Test mode (#271)\r\n* Faster saving and loading of snapshots (#231)\r\n* More reliable USB file transfers\r\n* The debugger console now includes entered commands in the log\r\n* Support for PIE (position-independent executables) on x86_64. Previously, care needed to be taken that PIE was disabled, otherwise it would crash on start. (#211)\r\n* Building the JIT is disabled automatically if the platform does not support it (#197)\r\n* Firebird builds on FreeBSD now (#228, #248)\r\n\r\n**Bugfixes:**\r\n* File access on Android got fixed (#202 and its various duplicates)\r\n* Fix placement of keypad buttons in the touchpad area (#41)\r\n* Various fixes for the Mobile UI layout (#201)\r\n* The kit configuration page in the Mobile UI no longer causes the keyboard to pop up by default (#257)\r\n* Connecting with GDB on windows works now (#259, #260)\r\n* Some shades of grey were not displayed properly when emulating pre-CX models (#270)\r\n* Fix crash on AArch64/arm64 when executing certain instructions\r\n* The keypad reacts to touch events in the desktop version as well now (#292, #293)\r\n* Some places were no longer translated correctly after the introduction of language switching in 1.5\r\n* Keys could get stuck on focus changes. Now they're all released when the keypad loses focus (#287)\r\n* The Ctrl key now changes color when pressed\r\n* Emulation speed no longer remains unlimited after a failed file transfer\r\n\r\n_Repo for Arch, Debian, Fedora, Ubuntu and openSUSE: [via OBS](https://software.opensuse.org/download.html?project=home%3AVogtinator%3Afirebird-emu&package=firebird-emu&locale=en)._\r\n\r\nThere is work in progress to implement and improve support for running in the browser on Qt for WebAssembly (#294). A preview is available on https://nspire-emus.github.io/firebird/wasm/\n\nNOTE: BundleIdentifier changed in this version and automatic updates have been disabled until manual install occurs.",
+                    "sha256": "54166448ccd9eee964b36997acff30beb1a1219cbacc1278bcc5fd1c97224e79",
+                    "size": 9953289,
+                    "version": "1.6"
+                },
+                {
                     "absoluteVersion": "1.5",
                     "date": "2020-03-28T14:25:34Z",
                     "downloadURL": "https://github.com/nspire-emus/firebird/releases/download/v1.5/firebird-iOS.ipa",
                     "localizedDescription": "# A heap of improvements: Firebird 1.5\n\n**New features:**\r\n* UI language can be switched\r\n* The debugger has a command history, press Up and Down arrow keys\r\n* On Android, the system file picker is used now, which fixes \"Could not start the emulation\" in many cases\r\n* The color scheme follows the system now\r\n* Improved performance of CX flash access by ignoring certain cache flush requests\r\n\r\n**Improvements:**\r\n* LCD can be resized freely now\r\n* Performance improvements for the ARM and AArch64 JITs\r\n* Supports macOS 10.15 Catalina\r\n* The Android APK includes arm64-v8a now\r\n* The Windows ZIP includes software OpenGL now, so should work on more systems\r\n\r\n**Bugfixes:**\r\n* Fix the external LCD sometimes being invisible\r\n* Allows building with recent versions of the Android NDK with clang\r\n* Does not crash on exit due to use of incompatible compile flags with GCC\r\n* Android devices with a lower w/h ratio are marked as supported now\r\n* firebird-send supports different implementations of netcat now\r\n* GDB and remote debugger work after emulation autostart as well\r\n* Moving the cursor over keypad buttons no longer clicks\r\n* On Windows, the filename for snapshots can now include non-ASCII characters\r\n* Fix crash on emulation start on certain x86-64 systems\r\n* Fix freeze on exit on JIT builds for the iOS version\r\n\r\nNote: Firebird Emu requires Qt 5.9 now.\r\n\r\n_Repo for Arch, Debian, Fedora, Ubuntu and openSUSE: [via OBS](https://software.opensuse.org/download.html?project=home%3AVogtinator%3Afirebird-emu&package=firebird-emu&locale=en)._\r\n",
                     "size": 9680896,
                     "version": "1.5"
                 }
             ]
         },
         {
-            "absoluteVersion": "2021.9",
             "bundleIdentifier": "com.yoshisuga.activeGS",
             "developerName": "yoshisuga & Olivier Goguel",
-            "downloadURL": "https://github.com/yoshisuga/activegs-ios/releases/download/2021.9/ActiveGS.ipa",
             "iconURL": "https://i.imgur.com/7LuLkoR.png",
             "localizedDescription": "An emulator for all things Apple.",
             "name": "ActiveGS iOS",
             "screenshotURLs": [
                 "https://i.imgur.com/8xekjhv.png",
                 "https://i.imgur.com/JFd6LiM.png",
                 "https://i.imgur.com/4ZE0DbB.png"
             ],
-            "size": 16593403,
             "subtitle": "An emulator for Apple II/2GS.",
             "tintColor": "#21486b",
-            "version": "2021.9",
-            "versionDate": "2021-09-23T09:28:59Z",
-            "versionDescription": "# 2021.9\n\nThis is a fork of Olivier Goguel's ActiveGS emulator for iOS.\r\n\r\nI've been tinkering it over the years and added some experimental features such as:\r\n\r\n- Support for iOS 15\r\n- Remap keyboard to supported wireless controller buttons (mFi/PS4/PS5/XBox One)\r\n- Custom split keyboard usable in landscape mode (written in Swift)\r\n\r\n![Simulator Screen Shot - iPhone 13 Pro Max - 2021-09-22 at 22 43 15](https://user-images.githubusercontent.com/564774/134484167-3c17c2a7-1d6a-467c-ac82-d7bfae7f281b.png)\r\n\r\n- A memory debugger/rudimentary memory-editing cheat engine (also written in Swift). Accessible via the \"D\" button in the right pane custom keyboard. Browse the memory map and change memory values. Not sure how the bank switching works and how it's mapped to memory but you get some representation of memory. \r\n![Simulator Screen Shot - iPhone 13 Pro Max - 2021-09-22 at 23 25 55](https://user-images.githubusercontent.com/564774/134484125-b984318a-b089-4484-b306-b976521963c3.png)\r\n\r\n\r\n",
             "versions": [
                 {
                     "absoluteVersion": "2021.9",
                     "date": "2021-09-23T09:28:59Z",
                     "downloadURL": "https://github.com/yoshisuga/activegs-ios/releases/download/2021.9/ActiveGS.ipa",
                     "localizedDescription": "# 2021.9\n\nThis is a fork of Olivier Goguel's ActiveGS emulator for iOS.\r\n\r\nI've been tinkering it over the years and added some experimental features such as:\r\n\r\n- Support for iOS 15\r\n- Remap keyboard to supported wireless controller buttons (mFi/PS4/PS5/XBox One)\r\n- Custom split keyboard usable in landscape mode (written in Swift)\r\n\r\n![Simulator Screen Shot - iPhone 13 Pro Max - 2021-09-22 at 22 43 15](https://user-images.githubusercontent.com/564774/134484167-3c17c2a7-1d6a-467c-ac82-d7bfae7f281b.png)\r\n\r\n- A memory debugger/rudimentary memory-editing cheat engine (also written in Swift). Accessible via the \"D\" button in the right pane custom keyboard. Browse the memory map and change memory values. Not sure how the bank switching works and how it's mapped to memory but you get some representation of memory. \r\n![Simulator Screen Shot - iPhone 13 Pro Max - 2021-09-22 at 23 25 55](https://user-images.githubusercontent.com/564774/134484125-b984318a-b089-4484-b306-b976521963c3.png)\r\n\r\n\r\n",
+                    "sha256": "4ce99019167c13e1fdce6005243002591586366852ddf793fa6a6521885a4910",
                     "size": 16593403,
                     "version": "2021.9"
                 }
             ]
         },
         {
-            "absoluteVersion": "1.6",
             "bundleIdentifier": "at.spiderlab.c64",
             "developerName": "T-Pau",
-            "downloadURL": "https://github.com/T-Pau/Ready/releases/download/release-1.6/Ready-1.6.ipa",
             "iconURL": "https://i.imgur.com/S9WS2C2.png",
             "localizedDescription": "Ready is an open source emulator for the following 8 bit home computers:\n* Commodore 64\n* Commodore VIC-20\n* Commodore 16, Plus/4\n* Sinclair ZX Spectrum (16k, 48k, Spectrum+, 128k, +2)\n\nWith preliminary support for these computers:\n* Atari 600XL, 800XL\n* Commodore 128\n* Commander X16\n\nIt is based on atari800, fuse, Vice, and x16-emulator, which provide accurate emulation of many hardware variants and peripherals. Ready requires at least iPadOS 13.5.\n\nReady aims to approximate the feeling of using actual hardware. Rather than configuring abstract settings, you select hardware components. The software keyboard is a facsimile of the original, reflecting the different existing styles. Even the noise of the disk drive is emulated. The Library section offers a way to organize a large collection of games, demos and programs. The emulated hardware can be customized for each entry.\n\nThe Inbox provides a place to quickly try new programs. You can easily move the ones you want to keep to the library.\n\nTools mode allows attaching a cartridge like Action Replay or Final Cartridge and a collection of disks with your favorite tools, to help you dig into the programs, like back in the day.",
             "name": "Ready",
             "screenshotURLs": [
                 "https://i.imgur.com/CN3fR34.png",
                 "https://i.imgur.com/q8ueM8W.png",
                 "https://i.imgur.com/2EHk0Wp.png",
                 "https://i.imgur.com/F3bXlmW.png"
             ],
-            "size": 63972294,
             "subtitle": "8-bit games for your iPad.",
             "tintColor": "#1c71c6",
-            "version": "1.6",
-            "versionDate": "2020-07-08T15:55:00Z",
-            "versionDescription": "# Release 1.6\n\n- Rename to Ready.\r\n\r\n- Add Commodore 16 and Plus/4 emulation.\r\n\r\n- Add ZX Spectrum emulation. Supported models are 16k, 48k, Specturm+, 128k, +2.\r\n\r\n- Add new app icons, one for each supported computer.\r\n",
             "versions": [
                 {
                     "absoluteVersion": "1.6",
                     "date": "2020-07-08T15:55:00Z",
                     "downloadURL": "https://github.com/T-Pau/Ready/releases/download/release-1.6/Ready-1.6.ipa",
                     "localizedDescription": "# Release 1.6\n\n- Rename to Ready.\r\n\r\n- Add Commodore 16 and Plus/4 emulation.\r\n\r\n- Add ZX Spectrum emulation. Supported models are 16k, 48k, Specturm+, 128k, +2.\r\n\r\n- Add new app icons, one for each supported computer.\r\n",
+                    "sha256": "379a0006350f996aa3e9b26be09bd1140553071d9301192e00f86666844e1a9b",
                     "size": 63972294,
                     "version": "1.6"
                 }
             ]
         },
         {
             "appID": "me.oatmealdome.dolphinios-njb",
             "beta": false,
             "bundleIdentifier": "me.oatmealdome.dolphinios-njb",
             "developerName": "OatmealDome",
-            "downloadURL": "https://github.com/OatmealDome/dolphin/releases/download/3.2.1/DolphiniOS-NJB-Universal-3.2.1-213.ipa",
             "iconURL": "https://cdn.oatmealdome.me/dolphinios/AppIcon.appiconset/ios_marketing1024x1024.png",
             "localizedDescription": "DolphiniOS is a port of the popular Dolphin emulator to iOS. Dolphin lets you play your favourite GameCube and Wii software with enhancements like higher resolutions, save states, and more. You can even play all of Nintendo's classics from past consoles through the Wii's Virtual Console library.\n\nPlease note that devices with A8 processors and older are not compatible.",
             "name": "DolphiniOS",
             "screenshotURLs": [
                 "https://cdn.oatmealdome.me/dolphinios/altstore/screenshots/screenshot_6s_1.PNG",
                 "https://cdn.oatmealdome.me/dolphinios/altstore/screenshots/screenshot_6s_2.PNG",
                 "https://cdn.oatmealdome.me/dolphinios/altstore/screenshots/screenshot_6s_3_reup.PNG",
                 "https://cdn.oatmealdome.me/dolphinios/altstore/screenshots/screenshot_6s_4_edit.png"
             ],
-            "size": 80253902,
             "subtitle": "GameCube and Wii games on the go.",
             "tintColor": "41cdff",
-            "version": "3.2.1",
-            "versionDate": "2022-09-11T18:00:00-04:00",
-            "versionDescription": "This update contains the following changes:\n\n- Fixed ubershaders.\n- Fixed fastmem crashing on iOS 16.\n\nFor more information, see https://oatmealdome.me/blog/dolphinios-ver-3-2-0/.",
             "versions": [
                 {
                     "date": "2022-09-11T18:00:00-04:00",
                     "downloadURL": "https://github.com/OatmealDome/dolphin/releases/download/3.2.1/DolphiniOS-NJB-Universal-3.2.1-213.ipa",
                     "localizedDescription": "This update contains the following changes:\n\n- Fixed ubershaders.\n- Fixed fastmem crashing on iOS 16.\n\nFor more information, see https://oatmealdome.me/blog/dolphinios-ver-3-2-0/.",
+                    "sha256": "dcae6e6053d6e4e3f3f44ab9e0d2f709f77f2405243e66184d7864796d80de5c",
                     "size": 80253902,
                     "version": "3.2.1"
                 },
                 {
                     "date": "2022-05-22T18:00:00-04:00",
                     "downloadURL": "https://github.com/OatmealDome/dolphin/releases/download/3.2.0/DolphiniOS-NJB-Universal-3.2.0-211.ipa",
                     "localizedDescription": "This update contains the following changes:\n\n- Fixes crashing when starting a game\n- Fixes graphical problems caused by an Apple silicon GPU driver bug\n- Integrates support for AltJIT and JitStreamer\n- Adds rumble when using the Touchscreen controller on iPhones\n\nFor more information, see https://oatmealdome.me/blog/dolphinios-ver-3-2-0/.",
@@ -197,290 +302,219 @@
             ]
         },
         {
             "appID": "me.oatmealdome.DolphiniOS-njb-patreon-beta",
             "beta": false,
             "bundleIdentifier": "me.oatmealdome.DolphiniOS-njb-patreon-beta",
             "developerName": "OatmealDome",
-            "downloadURL": "https://github.com/OatmealDome/dolphin/releases/download/3.2.1b1-213/DolphiniOS-NJB-Beta-Universal-3.2.1b1-213.ipa",
             "iconURL": "https://cdn.oatmealdome.me/dolphinios/AppIcon.appiconset/BetaAppStore.png",
             "localizedDescription": "DolphiniOS is a port of the popular Dolphin emulator to iOS. Dolphin lets you play your favourite GameCube and Wii software with enhancements like higher resolutions, save states, and more. You can even play all of Nintendo's classics from past consoles through the Wii's Virtual Console library.\n\nPlease note that devices with A8 processors and older are not compatible.",
             "name": "DolphiniOS (Public Beta)",
             "screenshotURLs": [
                 "https://cdn.oatmealdome.me/dolphinios/altstore/screenshots/screenshot_6s_1.PNG",
                 "https://cdn.oatmealdome.me/dolphinios/altstore/screenshots/screenshot_6s_2.PNG",
                 "https://cdn.oatmealdome.me/dolphinios/altstore/screenshots/screenshot_6s_3_reup.PNG",
                 "https://cdn.oatmealdome.me/dolphinios/altstore/screenshots/screenshot_6s_4_edit.png"
             ],
-            "size": 80291610,
             "subtitle": "Test the latest DolphiniOS.",
             "tintColor": "ffbb3d",
-            "version": "3.2.1b1",
-            "versionDate": "2022-07-05T18:00:00-04:00",
-            "versionDescription": "This update contains the following changes:\n\n- Fixed ubershaders.\n- Fixed fastmem crashing on iOS 16 betas.\n\nThe next beta build will be based off the rewritten DolphiniOS source code.\n\nFor more information, see https://oatmealdome.me/blog/dolphinios-ver-3-2-0/.",
             "versions": [
                 {
                     "date": "2022-07-05T18:00:00-04:00",
                     "downloadURL": "https://github.com/OatmealDome/dolphin/releases/download/3.2.1b1-213/DolphiniOS-NJB-Beta-Universal-3.2.1b1-213.ipa",
                     "localizedDescription": "This update contains the following changes:\n\n- Fixed ubershaders.\n- Fixed fastmem crashing on iOS 16 betas.\n\nThe next beta build will be based off the rewritten DolphiniOS source code.\n\nFor more information, see https://oatmealdome.me/blog/dolphinios-ver-3-2-0/.",
+                    "sha256": "302438ec452636ff0b033ac1561f35f95ec42c644263d318978ef6fb83fc09d8",
                     "size": 80291610,
                     "version": "3.2.1b1"
                 }
             ]
         },
         {
             "bundleIdentifier": "net.nerd.iNDS",
             "developerName": "iNDS Team",
-            "downloadURL": "https://github.com/iNDS-Team/iNDS/releases/download/v1.10.8/iNDS.ipa",
             "iconURL": "https://i.imgur.com/DbWJeF8.png",
             "localizedDescription": "iNDS is a derivation of the previous Nintendo DS emulator apps for iOS: nds4ios and Nitrogen. The iNDS Team release of iNDS is a fork of the original iNDS emulator by William Cobb. The iNDS Team aims to create a version that is driven by support from the community, adding trusted contributors to the team over time so that pull requests and issues do not sit untouched.\n\nCurrently, emulation is powered by the DeSmuME threaded ARM interpreter and runs at nearly full speed on the iPhone 5 and above. Due to the need to mmap the entire ROM into memory, older devices with only 256MB of RAM are not supported. These devices include the iPod Touch 4, iPad 1, iPhone 3GS, and anything below those devices.",
             "name": "iNDS",
-            "permissions": [
-                {
-                    "type": "photos",
-                    "usageDescription": "Allows iNDS to use images from your Photo Library as game artwork."
-                }
-            ],
             "screenshotURLs": [
                 "https://i.imgur.com/ap8Er1K.png",
                 "https://i.imgur.com/EgfrobI.png",
                 "https://i.imgur.com/9gLwHGD.png"
             ],
-            "size": 8553596,
             "subtitle": "Revival of the Nintendo DS emulator for iOS.",
             "tintColor": "#fc2125",
-            "version": "1.10.8",
-            "versionDate": "2021-03-01T22:39:20Z",
-            "versionDescription": "Version 1.10.8 fixes the cover art system, thus closing #190. ~~There also appears to be an issue with the previous Cydia release being corrupted, so hopefully, that is fixed in this version.~~\r\n\r\n**Full Changelog**\r\n- Fixed cover art system (#203). Thanks, @unlmtd.\r\n- Fixed compilation errors (#191). Thanks, @jdkula.",
             "versions": [
                 {
                     "date": "2021-03-01T22:39:20Z",
                     "downloadURL": "https://github.com/iNDS-Team/iNDS/releases/download/v1.10.8/iNDS.ipa",
                     "localizedDescription": "Version 1.10.8 fixes the cover art system, thus closing #190. ~~There also appears to be an issue with the previous Cydia release being corrupted, so hopefully, that is fixed in this version.~~\r\n\r\n**Full Changelog**\r\n- Fixed cover art system (#203). Thanks, @unlmtd.\r\n- Fixed compilation errors (#191). Thanks, @jdkula.",
+                    "sha256": "795253059e78f7acd96af1ce6e9430bc98611cf58342e51f8e7e6e8c459a59b0",
                     "size": 8553596,
                     "version": "1.10.8"
                 }
             ]
         },
         {
-            "absoluteVersion": "2022.3",
             "appID": "com.example.mame4ios",
             "bundleIdentifier": "com.example.mame4ios",
             "developerName": "yoshisuga",
-            "downloadURL": "https://github.com/yoshisuga/MAME4iOS/releases/download/2022.3/MAME4tvOS-2022.3-139.ipa",
             "iconURL": "https://i.imgur.com/gZCjhLl.png",
             "localizedDescription": "MAME stands for Multi Arcade Machine Emulator. This app lets you play arcade games from the past 30+ years on your iPhone, iPad, macOS, or AppleTV.\n\nMore than 2000 games are supported, and the currently supported romset version is MAME 0.139u1 (September 2010).\n\nOther nifty features include:\n* 64-bit binary to run on modern and future iOS devices\n* Supports modern device screen sizes, including iPhone X/XR/XS/XS Max and iPad Pro\n* A native iOS/iPadOS/tvOS frontend (by @ToddLa, new in 2020!)\n* A native Metal rendering engine (by @ToddLa, new in 2020!)\n* tvOS support (new in 2019!)\n* An in-app web server to transfer files from your computer (new in 2019!)\n* Transfer ROMs, Artwork, and ROMSETs via AirDrop or iOS File Sharing (new in 2020!)\n* Multiple MFI controllers (up to 4 with dual analog support - @DarrenBranford)\n* Supports using the touch screen as a lightgun\n* Turbo mode toggle for buttons\n* Touch analog for games like Arkanoid\n* Builds in Xcode 11.x/12.x and runs on latest iOS 13/14 versions",
             "name": "MAME4iOS",
-            "permissions": [
-                {
-                    "type": "bluetooth",
-                    "usageDescription": "We need bluetooth for peer play and steam controllers."
-                }
-            ],
             "screenshotURLs": [
                 "https://i.imgur.com/0JkUpEA.png",
                 "https://i.imgur.com/UJXiIUM.png"
             ],
-            "size": 46033990,
             "subtitle": "A MAME Arcade emulator for iOS.",
             "tintColor": "#51bacc",
-            "version": "2022.3",
-            "versionDate": "2022-09-17T02:33:58Z",
-            "versionDescription": "# 2022.3\n\n# Version 2022.3\r\n\r\n* iOS 16 support\r\n",
             "versions": [
                 {
+                    "absoluteVersion": "2022.5",
+                    "date": "2022-12-12T02:16:35Z",
+                    "downloadURL": "https://github.com/yoshisuga/MAME4iOS/releases/download/2022.5/MAME4iOS-2022.5-139.ipa",
+                    "localizedDescription": "# 2022.5\n\n* Updated to [MAME 250](https://www.mamedev.org/releases/whatsnew_0250.txt).\r\n* tvOS UX: use a Alert instead of a inline Segmented Control.\r\n* Show upload feedback in Web Server UX.\r\n* Added `Make First Favorite` to game context menu.\r\n",
+                    "sha256": "c3c715c4d4ffedb781141733c1e645c197a6548d30bc73e22246853d36ebc35b",
+                    "size": 52332306,
+                    "version": "2022.5"
+                },
+                {
                     "absoluteVersion": "2022.3",
                     "date": "2022-09-17T02:33:58Z",
                     "downloadURL": "https://github.com/yoshisuga/MAME4iOS/releases/download/2022.3/MAME4tvOS-2022.3-139.ipa",
                     "localizedDescription": "# 2022.3\n\n# Version 2022.3\r\n\r\n* iOS 16 support\r\n",
                     "size": 46033990,
                     "version": "2022.3"
                 }
             ]
         },
         {
-            "absoluteVersion": "1.0_18",
             "bundleIdentifier": "com.zurac.OldOS",
             "developerName": "zzanehip",
-            "downloadURL": "https://github.com/zzanehip/The-OldOS-Project/releases/download/1.0_18/OldOS.ipa",
             "iconURL": "https://raw.githubusercontent.com/zzanehip/The-OldOS-Project/master/OldOS/OldOS/Assets.xcassets/AppIcon.appiconset/1024.png",
             "localizedDescription": "OldOS is a testament to the days of yesteryear, showcasing what iOS once was ten years ago. The ethos of the app is to merge the technologies of today with a pixel-perfect recreation of the user experience of the past. The vast majority of apps in OldOS are fully functional \u2014 meaning they seamlessly integrate with the data on your phone to deliver a live, emulator-esque experience. What does this mean? Well, you can play your music in iPod, get directions in Maps, surf the web in Safari, view the current weather in Weather, and much more. By the same token, no shortcuts were taken in fully fleshing out the operating system. You can change your background, adjust settings, search apps, et cetera. There are a few apps still not ready for primetime but don't worry, they're coming soon.\n\nWith OldOS, you no longer need to worry about securing a legacy iPhone to experience nostalgia \u2014 it's available on your daily driver.\n\nPart of the goal with OldOS is to enable anyone to understand how iOS works and demonstrate just how powerful SwiftUI truly is. For that reason, the entire app is open-sourced \u2014 enabling developers to learn about, modify, and add to the app. I thought building this over my last six or so months in high school and sharing it with the world would be a fun and productive endeavor.\n\nSpecial Features:\n* \ud83e\uddd1\u200d\ud83d\udcbb Built almost entirely using SwiftUI.\n* \ud83c\udfa8 Designed to be as close to pixel-perfect as possible.\n* \ud83d\udcf1 Fully functional, perhaps even usable as a second OS.\n* \u2764\ufe0f A testament to the work of Apple employees of both the past and the present.\n* \ud83d\uddfa\ufe0f Fully open source for all to learn, modify, and build on.",
             "name": "OldOS",
-            "permissions": [
-                {
-                    "type": "camera",
-                    "usageDescription": "To take photos in OldOS, please enable access to your camera."
-                },
-                {
-                    "type": "photos",
-                    "usageDescription": "To view, manage, and add photos to your photo library in OldOS, please enable access. Then close and re-open the Photos app."
-                },
-                {
-                    "type": "music",
-                    "usageDescription": "To view, play, and experience your music in OldOS, please enable access to your music library."
-                },
-                {
-                    "type": "location",
-                    "usageDescription": "To enable maps to work properly, and see your current wifi network in Settings, please enable access to your location. Then close and re-open the Maps app."
-                },
-                {
-                    "type": "microphone",
-                    "usageDescription": "To record your audio while filming a video in OldOS, please in enable microphone access."
-                },
-                {
-                    "type": "contacts",
-                    "usageDescription": "To view and manage your contacts in OldOS, please enable access to your contacts list."
-                }
-            ],
             "screenshotURLs": [
                 "https://github.com/zzanehip/The-OldOS-Project/raw/master/Images/Market_1.jpg",
                 "https://github.com/zzanehip/The-OldOS-Project/raw/master/Images/Market_2.jpg",
                 "https://github.com/zzanehip/The-OldOS-Project/raw/master/Images/Market_3.jpg",
                 "https://github.com/zzanehip/The-OldOS-Project/raw/master/Images/Market_4.jpg",
                 "https://github.com/zzanehip/The-OldOS-Project/raw/master/Images/Market_5.jpg"
             ],
-            "size": 88173533,
             "subtitle": "OldOS is a testament to the days of iOS 4.",
             "tintColor": "#181818",
-            "version": "1.0",
-            "versionDate": "2021-11-23T19:01:37Z",
-            "versionDescription": "# IPA V1.0 Build 18\n\n1.0 (18):\r\n- Mail is here! This is a full-blown email client, no ifs, ands, or buts\r\n- View mailboxes, read emails, move emails, manage inbox, and send emails\r\n- Fixes to YouTube backend\r\n- Other bug fixes",
             "versions": [
                 {
                     "absoluteVersion": "1.0_18",
                     "date": "2021-11-23T19:01:37Z",
                     "downloadURL": "https://github.com/zzanehip/The-OldOS-Project/releases/download/1.0_18/OldOS.ipa",
                     "localizedDescription": "# IPA V1.0 Build 18\n\n1.0 (18):\r\n- Mail is here! This is a full-blown email client, no ifs, ands, or buts\r\n- View mailboxes, read emails, move emails, manage inbox, and send emails\r\n- Fixes to YouTube backend\r\n- Other bug fixes",
+                    "sha256": "60c65a79a5fda77cb6bb42280a379196ba0ed8be5d9c03dab1da8b76a97ddb18",
                     "size": 88173533,
                     "version": "1.0"
                 }
             ]
         },
         {
-            "absoluteVersion": "8.0.2",
             "bundleIdentifier": "science.xnu.undecimus",
             "developerName": "Pwn20wnd",
-            "downloadURL": "https://unc0ver.dev/downloads/8.0.2/9e44edfbfd1905cadf23c3b9ad1d5bed683ce061/unc0ver_Release_8.0.2.ipa",
             "iconURL": "https://i.imgur.com/5aehDxj.png",
             "localizedDescription": "unc0ver is an advanced jailbreaking tool for iOS devices. Jailbreaking with unc0ver unlocks the true power of your iDevice. Customize the appearance of your device, gain full control over how your device operates, obtain access to hidden features of iOS, and more.\n\nCompatibility:\n* unc0ver supports iOS 11.0 through to iOS 14.3 (Excluding 13.5.1 and 13.3.1)\n\nStability:\n* Utilizing the latest stable APT and Mobile Substrate, stability is guaranteed.\n\nSecurity:\n* Utilizing native system sandbox exceptions, security remains intact while enabling access to jailbreak files.",
             "name": "unc0ver",
             "screenshotURLs": [
                 "https://i.imgur.com/ItMaRRV.png",
                 "https://i.imgur.com/bjzyqpY.png",
                 "https://i.imgur.com/3TMGkaO.png",
                 "https://i.imgur.com/gTYfncm.png"
             ],
-            "size": 54489484,
             "subtitle": "The most advanced jailbreak tool.",
             "tintColor": "#101216",
-            "version": "8.0.2",
-            "versionDate": "2021-12-29T21:35:42Z",
-            "versionDescription": "# v8.0.2 Release\n\n- Add exploit guidance to improve reliability on A12-A13 iPhones running iOS 14.6-14.8\r\n- Fix exploit reliability on iPhone XS devices running iOS 14.6-14.8",
             "versions": [
                 {
                     "absoluteVersion": "8.0.2",
                     "date": "2021-12-29T21:35:42Z",
                     "downloadURL": "https://unc0ver.dev/downloads/8.0.2/9e44edfbfd1905cadf23c3b9ad1d5bed683ce061/unc0ver_Release_8.0.2.ipa",
                     "localizedDescription": "# v8.0.2 Release\n\n- Add exploit guidance to improve reliability on A12-A13 iPhones running iOS 14.6-14.8\r\n- Fix exploit reliability on iPhone XS devices running iOS 14.6-14.8",
+                    "sha256": "d385c2be158c3106266b0b7795647fe2f873905bca94874b57ef35cce6cf50f6",
                     "size": 54489484,
                     "version": "8.0.2"
                 }
             ]
         },
         {
             "bundleIdentifier": "ru.nonamedude.iTorrent",
             "developerName": "XITRIX",
-            "downloadURL": "https://github.com/XITRIX/iTorrent/releases/download/v1.8.3/iTorrent.ipa",
             "iconURL": "https://i.imgur.com/C3KwMP5.png",
             "localizedDescription": "iTorrent is an ordinary torrent client for iOS with Files app support.\n\nWhat can this app do:\n\n\u2022 Download in the background\n\u2022 Sequential download (use VLC to watch films while loading)\n\u2022 Add torrent files from Share menu (Safari and other apps)\n\u2022 Add magnet links directly from Safari\n\u2022 Store files in Files app (iOS 11+)\n\u2022 File sharing directly from app\n\u2022 Download torrent by link\n\u2022 Download torrent by magnet\n\u2022 Send notification on torrent downloaded\n\u2022 FTP Server (unstable)\n\u2022 Select files to download or not\n\u2022 Change UI to dark theme\n\nNow supporting these localizations:\n\u2022 English\n\u2022 Russian\n\u2022 Turkish",
             "name": "iTorrent",
-            "permissions": [
-                {
-                    "type": "photos",
-                    "usageDescription": "Allows iTorrent to save files to Photos app."
-                }
-            ],
             "screenshotURLs": [
                 "https://i.imgur.com/0o7qou3.png",
                 "https://i.imgur.com/sO510zC.png",
                 "https://i.imgur.com/MQPWxYz.png",
                 "https://i.imgur.com/xTAo5uE.png"
             ],
-            "size": 21218913,
             "subtitle": "Ordinary iOS torrent client app.",
             "tintColor": "#e32b3c",
-            "version": "1.8.3",
-            "versionDate": "2020-09-20",
-            "versionDescription": "What's new:\n\n\u2022 Text accessibility support added\n\u2022 Huge backend refactoring\n\u2022 Libtorrent updated to 1.2.9\n\u2022 Minor UI improvements\n\u2022 Many bugs fixed (possibly new ones added)",
             "versions": [
                 {
                     "date": "2020-09-20",
                     "downloadURL": "https://github.com/XITRIX/iTorrent/releases/download/v1.8.3/iTorrent.ipa",
                     "localizedDescription": "What's new:\n\n\u2022 Text accessibility support added\n\u2022 Huge backend refactoring\n\u2022 Libtorrent updated to 1.2.9\n\u2022 Minor UI improvements\n\u2022 Many bugs fixed (possibly new ones added)",
+                    "sha256": "f6854b9b402b522dca849469b15dd8c4c41f0fe2e3efcd2b3550f6074ece5564",
                     "size": 21218913,
                     "version": "1.8.3"
                 }
             ]
         },
         {
             "appID": "com.rileytestut.GBA4iOS",
             "bundleIdentifier": "com.rileytestut.GBA4iOS",
             "developerName": "Riley Testut",
-            "downloadURL": "https://f000.backblazeb2.com/file/altstore/sources/demo/GBA4iOS.ipa",
             "iconURL": "https://i.imgur.com/SBrqO9g.png",
             "localizedDescription": "Classic Gaming, Meet iOS.\n\nWhile iPhone and iOS have brought a new era of gaming upon us, there will always be room in our hearts for those classic games from decades ago. Unfortunately, there has been no easy way for people to play these games whenever they so desired...that is, until now. GBA4iOS was made for one purpose and one purpose only: to help everyone relive their favorite games from their past. Now, every where you take your iPhone, iPad, or iPod Touch, you can bring and play your classic games with you, giving you practically endless hours of entertainment!\n\nSo that's great and all, but what features does GBA4iOS actually have? Far too many to list in one App Store description, but here are some of the biggest:\n\n\u2022 Multiplayer (iPhone 5 or newer, iPad 4 or newer). GBA4iOS allows you to link with other players nearby and play with them, allowing you to unlock or experience certain events in games that are unavailable to just one player! Plus, nothing is cooler than playing games with your friends.\n\n\u2022 Save States. Ever get frustrated when a game requires you to save only at certain points? Well be frustrated no longer, GBA4iOS fully supports Save States, allowing you to save anywhere in the game and resume right from that point later. Even better, you can protect certain save states so you never accidentally overwrite them (and as everyone knows losing game data is one of the worst things in the world).\n\n\u2022 Cheat Codes. Sometimes games are just too hard, and you need a little boost to help defeat it. GBA4iOS allows you to input and use GameShark, Action Replay, Code Breaker, and Game Genie codes as you see fit. Don't worry, we won't judge!\n\n\u2022 Fast Forward (iPhone 4s or newer, iPad 2 or newer, iPod Touch 5th Gen). Don't you wish there was a way to speed up long cutscenes in games, or to reduce the time doing boring tasks in the game? Well, now there is! GBA4iOS allows you to \"Fast Forward\" through slow parts of the game, allowing you to get back to the fun even quicker.\n\n\u2022 Customizable Controller Skins. Want to change the look of the controller to something more personal? No worries, you can download a multitude of new controller skins from within the app, or download almost countless more from the web! You'll definitely be able to find a controller skin you like.\n\n\u2022 Dropbox Sync. Have multiple devices, or worried something will happen to your games? Dropbox Sync solves both these issues! When enabled, GBA4iOS will sync your game saves, save states, and cheat codes to Dropbox, keeping any and all your devices up to date with your latest changes. Plus, this means your game data is always backed up in the cloud, so if something happens to your device, your data is safe.\n\n\u2022 MFi Controller Support. Sometimes, touchscreen buttons just aren't good enough for the level of precision needed by some games. Luckily, GBA4iOS supports MFi Controllers, allowing you to connect and use physical controllers with your games! Now you can beat that final boss without a sweat.\n\nAll this and more ensures that GBA4iOS will give you the best portable gaming experience, hands down. So what are you waiting for, download GBA4iOS now and enjoy reliving your favorite classic games immediately!",
             "name": "GBA4iOS",
             "screenshotURLs": [
                 "https://i.imgur.com/L4H0yM3.png",
                 "https://i.imgur.com/UPGYLVr.png",
                 "https://i.imgur.com/sWpUAii.png",
                 "https://i.imgur.com/UwnDXRc.png"
             ],
-            "size": 7924507,
             "subtitle": "Game Boy games in your pocket.",
             "tintColor": "78209d",
-            "version": "2.1",
-            "versionDate": "2020-03-24T14:30:00-07:00",
-            "versionDescription": "Initial AltStore release!",
             "versions": [
                 {
                     "date": "2020-03-24T14:30:00-07:00",
                     "downloadURL": "https://f000.backblazeb2.com/file/altstore/sources/demo/GBA4iOS.ipa",
                     "localizedDescription": "Initial AltStore release!",
+                    "sha256": "523ede3000e89716dc6e16f04ddd1d6e66a950a9295784769dab3e65a5ecc351",
                     "size": 7924507,
                     "version": "2.1"
                 }
             ]
         },
         {
             "appID": "com.libretro.RetroArchiOS11",
             "bundleIdentifier": "com.libretro.RetroArchiOS11",
             "developerName": "libretro",
-            "downloadURL": "https://buildbot.libretro.com/stable/1.12.0/apple/ios-arm64/RetroArch.ipa",
             "iconURL": "https://i.imgur.com/pqgVB0v.png",
             "localizedDescription": "RetroArch is a frontend for a plethora of emulators. Almost every Retro console can be run using one of RetroArch's downloadable cores.\n\nThere are several ways to customize your experience by installing different themes, rearranging your touchscreen controls, and downloading game box art.\nRetroArch enables you to run classic games on a wide range of computers and consoles through its slick graphical interface. Settings are also unified so configuration is done once and for all.\n\nIn addition to this, you will soon be able to run original game discs (CDs) from RetroArch.\n\nRetroArch has advanced features like shaders, netplay, rewinding, next-frame response times, runahead, machine translation, blind accessibility features, and more!\n\nCheck out all of RetroArch's awesome features at our website: https://www.retroarch.com/",
             "name": "RetroArch",
             "screenshotURLs": [
                 "https://i.imgur.com/uv1x1c4.png",
                 "https://i.imgur.com/qJdyNl2.png",
                 "https://i.imgur.com/fijaR4n.png",
                 "https://i.imgur.com/B3J5zMB.png",
                 "https://i.imgur.com/4Mj77IY.png"
             ],
-            "size": 435770036,
             "subtitle": "Cross-platform, sophisticated frontend for emulation.",
             "tintColor": "#000000",
-            "version": "1.12.0",
-            "versionDate": "2022-10-17",
-            "versionDescription": "Many bug fixes and quality of life improvements. See full changelog for details: https://github.com/libretro/RetroArch/blob/master/CHANGES.md",
             "versions": [
                 {
                     "date": "2022-10-17",
                     "downloadURL": "https://buildbot.libretro.com/stable/1.12.0/apple/ios-arm64/RetroArch.ipa",
                     "localizedDescription": "Many bug fixes and quality of life improvements. See full changelog for details: https://github.com/libretro/RetroArch/blob/master/CHANGES.md",
+                    "sha256": "d790ce8ef9c2b8f9cd2c974f4e70690aa24c0a99cdb8c65ed235b790c1f0c47e",
                     "size": 435770036,
                     "version": "1.12.0"
                 },
                 {
                     "date": "2020-08-07",
                     "downloadURL": "https://github.com/QuarkSources/quarksources.github.io/releases/download/v1.0/RetroArch.ipa",
                     "localizedDescription": "Many bug fixes and quality of life improvements. See full changelog for details: https://github.com/libretro/RetroArch/blob/master/CHANGES.md",
@@ -489,197 +523,192 @@
                 }
             ]
         },
         {
             "appID": "com.louisanslow.record",
             "bundleIdentifier": "com.louisanslow.record",
             "developerName": "Louis Anslow",
-            "downloadURL": "https://github.com/QuarkSources/quarksources.github.io/releases/download/v1.0/Rewound.ipa",
             "iconURL": "https://i.imgur.com/LfIRxqb.png",
             "localizedDescription": "Rewound uses your Apple Music library and displays it in the nostalgic style of an old spin-wheel iPod.",
             "name": "Rewound",
-            "permissions": [
-                {
-                    "type": "music",
-                    "usageDescription": "Rewound needs access to your music library to control your music."
-                }
-            ],
             "screenshotURLs": [
                 "https://i.imgur.com/IfLobOR.png",
                 "https://i.imgur.com/IJcJ6WG.png",
                 "https://i.imgur.com/dVjieD9.png",
                 "https://i.imgur.com/kmC3NtZ.png"
             ],
-            "size": 5628716,
             "subtitle": "Turn your iPhone into an iPod. Classic.",
             "tintColor": "#9e968d",
-            "version": "2019.7",
-            "versionDate": "2019-12-09",
-            "versionDescription": "Small fixes.",
             "versions": [
                 {
                     "date": "2019-12-09",
                     "downloadURL": "https://github.com/QuarkSources/quarksources.github.io/releases/download/v1.0/Rewound.ipa",
                     "localizedDescription": "Small fixes.",
+                    "sha256": "6fe3f0e30e23e1a0a3f224245dfdb1f804de7bedf46496110b797eb271282721",
                     "size": 5628716,
                     "version": "2019.7"
                 }
             ]
         },
         {
             "appID": "org.scummvm.scummvm",
             "bundleIdentifier": "org.scummvm.scummvm",
             "developerName": "ScummVM Team",
-            "downloadURL": "https://downloads.scummvm.org/frs/scummvm/2.6.0/scummvm-2.6.0-ios.ipa",
             "iconURL": "https://i.imgur.com/sSQhbwJ.png",
             "localizedDescription": "ScummVM is a program which allows you to run certain classic graphical point-and-click adventure games and role-playing games, provided you already have their data files. The clever part about this: ScummVM just replaces the executables shipped with the games, allowing you to play them on systems for which they were never designed!\n\nScummVM supports a huge library of adventures with over 250 games in total. It supports many classics published by legendary studios like LucasArts, Sierra On-Line, Revolution Software, Cyan, Inc. and Westwood Studios. Next to ground-breaking titles like the Monkey Island series, Broken Sword, Myst, Blade Runner and countless other games you will find some really obscure adventures and truly hidden gems to explore.",
             "name": "ScummVM",
             "screenshotURLs": [
                 "https://i.imgur.com/7BHTMT0.png",
                 "https://i.imgur.com/Fp24Isf.png",
                 "https://i.imgur.com/vD3UJfE.png"
             ],
-            "size": 92033520,
             "subtitle": "Point and click adventures.",
             "tintColor": "#bf6a27",
-            "version": "2.6.0",
-            "versionDate": "2022-07-25",
-            "versionDescription": "Bug fixes.",
             "versions": [
                 {
                     "date": "2022-07-25",
                     "downloadURL": "https://downloads.scummvm.org/frs/scummvm/2.6.0/scummvm-2.6.0-ios.ipa",
                     "localizedDescription": "Bug fixes.",
+                    "sha256": "2d4a5cd37e20075af432af8fb072d1a204746da8edeb469714462ae603be329a",
                     "size": 92033520,
                     "version": "2.6.0"
                 },
                 {
                     "date": "2020-09-13",
                     "downloadURL": "https://github.com/QuarkSources/quarksources.github.io/releases/download/v1.0/ScummVM.ipa",
                     "localizedDescription": "Bug fixes.",
                     "size": 57222372,
                     "version": "2.2.0"
                 }
             ]
         },
         {
-            "absoluteVersion": "2.5",
             "bundleIdentifier": "net.namedfork.minivmac",
             "developerName": "Gryphel Project & zydeco",
-            "downloadURL": "https://github.com/zydeco/minivmac4ios/releases/download/v2.5/minivmac4ios-2.5.ipa",
             "iconURL": "https://i.imgur.com/MGxGvKR.png",
             "localizedDescription": "Features\n\n\u2022 Emulates Mac Plus, Mac II or Mac 128K\n\u2022 Full simulated keyboard (including all Mac keys)\n\u2022 Full sound output\n\u2022 Uses external keyboard if available\n\u2022 Regulable emulation speed\n\u2022 Easy(ish) to import/export disk images\n\nPlease check out the github README for usage instructions: https://github.com/zydeco/minivmac4ios",
             "name": "Mini vMac",
-            "permissions": [
-                {
-                    "type": "background-audio",
-                    "usageDescription": "This allows the application to continue running audio in the background."
-                }
+            "screenshotURLs": [
+                "https://i.imgur.com/Huqxo8z.png",
+                "https://i.imgur.com/Pq2vIrO.png",
+                "https://i.imgur.com/A7koKUp.png",
+                "https://i.imgur.com/IhtYS9E.png"
             ],
-            "screenshotURLs": [],
-            "size": 1194371,
             "subtitle": "A miniature early Macintosh emulator.",
             "tintColor": "#dd2b03",
-            "version": "2.5",
-            "versionDate": "2022-05-26T18:30:55Z",
-            "versionDescription": "# Mini vMac for iOS 2.5\n\n* Update to Mini vMac 37.03 beta\r\n* Fixed crash when deleting disk images on iPad\r\n* Adds recently used disks to quick actions menu\r\n* Removed custom presentation modes for disk and settings screens\r\n* Doesn't show \"The developer of this app needs to update it to work with this version of iOS\" error when installing IPA on iOS 15",
             "versions": [
                 {
                     "absoluteVersion": "2.5",
                     "date": "2022-05-26T18:30:55Z",
                     "downloadURL": "https://github.com/zydeco/minivmac4ios/releases/download/v2.5/minivmac4ios-2.5.ipa",
                     "localizedDescription": "# Mini vMac for iOS 2.5\n\n* Update to Mini vMac 37.03 beta\r\n* Fixed crash when deleting disk images on iPad\r\n* Adds recently used disks to quick actions menu\r\n* Removed custom presentation modes for disk and settings screens\r\n* Doesn't show \"The developer of this app needs to update it to work with this version of iOS\" error when installing IPA on iOS 15",
+                    "sha256": "2d3fd7a540944d46c1c968dbc88434deffea93a14a54f06191436fc804e9796b",
                     "size": 1194371,
                     "version": "2.5"
                 }
             ]
         },
         {
             "appID": "com.dry05.filzaescaped11-12",
             "bundleIdentifier": "com.dry05.filzaescaped11-12",
             "developerName": "Bas vT",
-            "downloadURL": "https://github.com/QuarkSources/quarksources.github.io/releases/download/v1.0/Filza-Escaped.ipa",
             "iconURL": "https://i.imgur.com/VsEGbQN.png",
             "localizedDescription": "It's just normal Filza but for jailed iPhones running iOS 12.1.3 - 13.4.1. This is possible using the Psychic Paper exploit to gain greater file access on stock iOS. Since the exploit used here was patched in iOS 13.5, do not expect many further updates to this application and it will likely never work the same on iOS 13.5 and up.",
             "name": "Filza Escaped",
-            "permissions": [
-                {
-                    "type": "photos",
-                    "usageDescription": "To save photos and videos to photo library."
-                },
-                {
-                    "type": "faceid",
-                    "usageDescription": "Filza uses Face ID to authenticate."
-                }
-            ],
             "screenshotURLs": [
                 "https://i.imgur.com/KBkDKkN.png"
             ],
-            "size": 10832361,
             "subtitle": "iOS 12-13 file manager for jailed iPhones.",
             "tintColor": "#d5ad0b",
-            "version": "3.7",
-            "versionDate": "2020-05-04",
-            "versionDescription": "iOS 13 support.",
             "versions": [
                 {
                     "date": "2020-05-04",
                     "downloadURL": "https://github.com/QuarkSources/quarksources.github.io/releases/download/v1.0/Filza-Escaped.ipa",
                     "localizedDescription": "iOS 13 support.",
+                    "sha256": "8c82cee4f15b4900395b8a1e34bce80cdd5caaa3646560524d412be5339947e7",
                     "size": 10832361,
                     "version": "3.7"
                 }
             ]
         },
         {
-            "absoluteVersion": "2.2",
             "bundleIdentifier": "com.wh0ba.xpatcher",
             "developerName": "Wh0ba",
-            "downloadURL": "https://github.com/Wh0ba/XPatcher/releases/download/v2.2/XPatcher_2.2.ipa",
             "iconURL": "https://i.imgur.com/cgrsWgC.png",
             "localizedDescription": "XPatcher is a GUI front-end for flips, libppf, xdelta, and libRUP patching libraries.\n\nThis app allows you to apply patches to files on your iOS devices, mostly used to apply rom hacks to video game roms with a simple to use interface to make it as user-friendly as possible.",
             "name": "XPatcher",
             "screenshotURLs": [
                 "https://i.imgur.com/nFunb9n.png",
                 "https://i.imgur.com/7UvBK4J.png"
             ],
-            "size": 357189,
             "subtitle": "A Rom-patcher utility for your iOS device.",
             "tintColor": "#ff767d",
-            "version": "2.2",
-            "versionDate": "2022-01-07T10:15:55Z",
-            "versionDescription": "# File hashes when selecting files\n\n### XPatcher 2.2\r\n### A small updated with a little feature \r\n\r\nNow when you select a file in the Documents tab, it will show SHA1, MD5, and CRC32 hashes of the selected file.\r\nclosing #5\r\nother changes might be adding .vcdiff to the recognized patch formats (XDelta) but so far it seems kinda broken as stated in #6 .\r\n\r\n**Full Changelog**: https://github.com/Wh0ba/XPatcher/compare/2.0...v2.2",
             "versions": [
                 {
                     "absoluteVersion": "2.2",
                     "date": "2022-01-07T10:15:55Z",
                     "downloadURL": "https://github.com/Wh0ba/XPatcher/releases/download/v2.2/XPatcher_2.2.ipa",
                     "localizedDescription": "# File hashes when selecting files\n\n### XPatcher 2.2\r\n### A small updated with a little feature \r\n\r\nNow when you select a file in the Documents tab, it will show SHA1, MD5, and CRC32 hashes of the selected file.\r\nclosing #5\r\nother changes might be adding .vcdiff to the recognized patch formats (XDelta) but so far it seems kinda broken as stated in #6 .\r\n\r\n**Full Changelog**: https://github.com/Wh0ba/XPatcher/compare/2.0...v2.2",
+                    "sha256": "0f2bf920c6760fdb410fb39fe5df7f678aaf12c55c4d4ca0e01c76bd860b8e24",
                     "size": 357189,
                     "version": "2.2"
                 }
             ]
         },
         {
+            "appID": "app.ish.iSH",
+            "bundleIdentifier": "app.ish.iSH",
+            "developerName": "Theodore Dubois and contributors",
+            "iconURL": "https://ish.app/assets/icon-full.png",
+            "localizedDescription": "iSH is a project to get a Linux shell environment running locally on your iOS device, using a usermode x86 emulator.",
+            "name": "iSH",
+            "screenshotURLs": [
+                "https://ish.app/assets/front-iphone-full.png"
+            ],
+            "subtitle": "Linux shell for iOS",
+            "tintColor": "#000000",
+            "versions": [
+                {
+                    "absoluteVersion": "builds/482",
+                    "date": "2023-04-23T04:46:13Z",
+                    "downloadURL": "https://github.com/ish-app/ish/releases/download/builds/482/iSH.ipa",
+                    "localizedDescription": "# iSH 1.3 (build 482)\n\nNew stuff:\r\n- iSH now supports custom themes\r\n- Preferences are now exposed via procfs\r\n- Some more app icon choices\r\n- Hyperlinks created by OSC 8 are underlined instead of invisible\r\n\r\nFixed bugs:\r\n- Forward SO_RCVTIMEO, SO_SNDTIMEO in setsockopts to support snac\r\n- Add about four dozen SIMD instructions to improve support for nodejs and Rust\r\n- Fix bottom keyboard inset for iPad, Stage Manager, and devices with no home button\r\n- Implement /proc/pid/task to fix recent versions of GDB\r\n- Fix VoiceOver focus stealing keyboard focus on iOS 15+\r\n- Resolve an issue with xadd causing git clones to hang\r\n- Trigger segfault on unaligned cmpxchg8b, which iSH does not support\r\n- Fix a race condition that causes some output to be lost\r\n- Fix toolbar button sizing",
+                    "sha256": "318c8aa2b36cf0879c07323e099a5b806a105a891af6dea15fdd4987e8fb43eb",
+                    "size": 4183791,
+                    "version": "1.3"
+                },
+                {
+                    "date": "2021-02-25T06:06:58+00:00",
+                    "downloadURL": "https://github.com/ish-app/ish/releases/download/builds/458/iSH.ipa",
+                    "localizedDescription": "Automated daily build",
+                    "size": 4183190,
+                    "version": "1.2.3"
+                }
+            ]
+        },
+        {
             "appID": "com.virtualapplications.play",
             "bundleIdentifier": "com.virtualapplications.play",
             "developerName": "Jean-Philip Desjardins",
-            "downloadURL": "https://purei.org/downloads/play/stable/0.56/Play.ipa",
             "iconURL": "https://i.imgur.com/NOi1cdl.png",
             "localizedDescription": "Play! is a portable PlayStation2 emulator. The focus of the project is on making PlayStation2 emulation easy and accessible. Just pop in your favorite game's disc and have fun!\n\n\u2022 No BIOS required. Play! is an high-level emulator.\n\u2022 Easy configuration. No custom settings to fix specific games.\n\u2022 Available on many platforms, making sure the experience is the same quality everywhere.",
             "name": "Play!",
             "screenshotURLs": [],
-            "size": 13371703,
             "subtitle": "PlayStation 2 Games on iOS.",
             "tintColor": "#5f5fff",
-            "version": "0.56",
-            "versionDate": "2022-09-13",
-            "versionDescription": "Bug fixes.",
             "versions": [
                 {
+                    "date": "2022-12-22",
+                    "downloadURL": "https://purei.org/downloads/play/stable/0.58/Play.ipa",
+                    "localizedDescription": "Bug fixes.",
+                    "sha256": "7ab7dc4cbc9202594188ef6d378753b9cc4ed4ecf595d7ed047d6f4419952597",
+                    "size": 13389347,
+                    "version": "0.58"
+                },
+                {
                     "date": "2022-09-13",
                     "downloadURL": "https://purei.org/downloads/play/stable/0.56/Play.ipa",
                     "localizedDescription": "Bug fixes.",
                     "size": 13371703,
                     "version": "0.56"
                 },
                 {
@@ -688,107 +717,143 @@
                     "localizedDescription": "Bug fixes.",
                     "size": 12346902,
                     "version": "0.50"
                 }
             ]
         },
         {
-            "absoluteVersion": "1.1.3",
             "appID": "it.ned.appdb-ios",
             "bundleIdentifier": "it.ned.appdb-ios",
             "developerName": "ned",
-            "downloadURL": "https://github.com/n3d1117/appdb/releases/download/v1.1.3/appdb_1.1.3_hotfix4.ipa",
             "iconURL": "https://i.imgur.com/vmryx82.png",
             "localizedDescription": "A fully-featured iOS client for appdb.to written in Swift 5 (iOS 10+).",
             "name": "appdb",
             "screenshotURLs": [
                 "https://i.imgur.com/r2id9BJ.png",
                 "https://i.imgur.com/DDl4zSF.png",
                 "https://i.imgur.com/TWDJ5ag.png",
                 "https://i.imgur.com/XytUEMV.png",
                 "https://i.imgur.com/bNBwJdt.png",
                 "https://i.imgur.com/tKaTJIY.png",
                 "https://i.imgur.com/PxjetRi.png"
             ],
-            "size": 25756822,
             "subtitle": "A fully-featured iOS client for appdb.to",
             "tintColor": "#007ed8",
-            "version": "1.1.3",
-            "versionDate": "2022-03-26T21:12:55Z",
-            "versionDescription": "# Release 1.1.3\n\n- Full support for new v1.5 APIs\r\n- Support new installation options (patch in-app, push notifications, app duplication, game trainer etc...). Make sure to enable \"Ask for installation options\" in Settings!\r\n- Added alternate icons! You can now change app icon from settings, check out the new shiny colors!\r\n- Various UI fixes and iOS 15 specific improvements",
             "versions": [
                 {
+                    "absoluteVersion": "1.1.5",
+                    "date": "2023-04-06T07:51:43Z",
+                    "downloadURL": "https://github.com/n3d1117/appdb/releases/download/v1.1.5/appdb-v1.1.5-stev3fvcks.ipa",
+                    "localizedDescription": "# Release 1.1.5\n\nSwitch between available Free Enterprise Signing certificates\r\nSupport for listing and deleting IPA Cache files\r\nShow download statistics on app detail page\r\nFix the bug on status page not showing some values\r\nAdd black icon\r\nAdd translations for icon chooser\r\nMake disabling ads easy and disabled by default\r\nCompletely remove old \"PRO\" stuff",
+                    "sha256": "2161101b4cd6464800c97fc1ae08390d87779684635c7c7bf223a2ab65246b1b",
+                    "size": 24408468,
+                    "version": "1.1.5"
+                },
+                {
+                    "absoluteVersion": "1.1.4",
+                    "date": "2023-04-03T23:20:04Z",
+                    "downloadURL": "https://github.com/n3d1117/appdb/releases/download/v1.1.4/appdb_1.1.4.ipa",
+                    "localizedDescription": "# Release 1.1.4\n\nSupport for Free Enterprise Signing\r\nSupport for appdb PLUS\r\nFull support for latest appdb features\r\nSupport for injecting dylibs, frameworks and debs into apps - Make sure to enable \"Ask for installation options\" in Settings!\r\nSupport for AltStore repos\r\nSupport for displaying link reports and link compatibility\r\nVarious UI and bug fixes",
+                    "size": 24356196,
+                    "version": "1.1.4"
+                },
+                {
                     "absoluteVersion": "1.1.3",
                     "date": "2022-03-26T21:12:55Z",
                     "downloadURL": "https://github.com/n3d1117/appdb/releases/download/v1.1.3/appdb_1.1.3_hotfix4.ipa",
                     "localizedDescription": "# Release 1.1.3\n\n- Full support for new v1.5 APIs\r\n- Support new installation options (patch in-app, push notifications, app duplication, game trainer etc...). Make sure to enable \"Ask for installation options\" in Settings!\r\n- Added alternate icons! You can now change app icon from settings, check out the new shiny colors!\r\n- Various UI fixes and iOS 15 specific improvements",
                     "size": 25756822,
                     "version": "1.1.3"
                 }
             ]
         },
         {
             "appID": "org.coolstar.odyssey",
             "beta": false,
             "bundleIdentifier": "org.coolstar.odyssey",
             "developerName": "Odyssey Team",
-            "downloadURL": "https://github.com/Odyssey-Team/Odyssey/releases/download/1.4.2/Odyssey-1.4.2.ipa",
             "iconURL": "https://theodyssey.dev/assets/images/icon.png",
             "localizedDescription": "Supporting iOS Versions: 13.0 - 13.7.\nOdyssey is the first jailbreak to be written almost entirely in Swift. Completely open source and welcomes community contributions and pull requests, as a tribute to the dearly departed s0uthwes and his continued optimism and faith in the project. Comes with the open source Procursus bootstrap, designed from the ground up with openness and compatiblity in mind. Along with a new tweak injection platform, libhooker.",
             "name": "Odyssey",
             "screenshotURLs": [
                 "https://theodyssey.dev/assets/images/ss-1.png",
                 "https://theodyssey.dev/assets/images/ss-2.png",
                 "https://theodyssey.dev/assets/images/ss-3.png"
             ],
-            "size": 27200000,
             "subtitle": "A new jailbreak for a new era.",
             "tintColor": "D287F4",
-            "version": "1.4.2",
-            "versionDate": "2022-02-18",
-            "versionDescription": "- Update Sileo to 2.3\n- Replace Packix with Havoc as default repo",
             "versions": [
                 {
+                    "date": "2023-04-03",
+                    "downloadURL": "https://github.com/Odyssey-Team/Odyssey/releases/download/1.4.3/Odyssey-1.4.3.ipa",
+                    "localizedDescription": "- Update Sileo to 2.3-1",
+                    "sha256": "0019dfc4b32d63c1392aa264aed2253c1e0c2fb09216f8e2cc269bbfb8bb49b5",
+                    "size": 27200000,
+                    "version": "1.4.3"
+                },
+                {
                     "date": "2022-02-18",
                     "downloadURL": "https://github.com/Odyssey-Team/Odyssey/releases/download/1.4.2/Odyssey-1.4.2.ipa",
                     "localizedDescription": "- Update Sileo to 2.3\n- Replace Packix with Havoc as default repo",
                     "size": 27200000,
                     "version": "1.4.2"
                 }
             ]
         },
         {
             "appID": "com.utmapp.UTM",
             "bundleIdentifier": "com.utmapp.UTM",
             "developerName": "osy",
-            "downloadURL": "https://github.com/utmapp/UTM/releases/download/v4.0.9/UTM.ipa",
-            "filename": "UTM.ipa",
-            "githubOwner": "utmapp",
-            "githubRepository": "UTM",
             "iconURL": "https://alt.getutm.app/icon.png",
             "localizedDescription": "UTM is a full featured virtual machine host for iOS. In short, it allows you to run Windows, Android, and more on your iPhone and iPad.\nThis version requires using AltJIT or iOS < 14.0 or iOS 14.2-14.4 (A14+ devices only). Install UTM SE for slower emulation without JIT.\n\n\nMore information at https://getutm.app/\n\nFeatures:\n\n\u2022 Emulate any Processor\n30+ processors supported by qemu including x86_64, ARM64, and RISC-V\n\u2022 Run any Operating System\nWindows, Linux, and more natively and securely on iOS within an App\n\u2022 Fast Emulation\nPara-virtualization with SPICE and JIT compilation with TCG\n\u2022 High Compatibility\niOS 11+ supported. Works on iPhone and iPad. No jailbreak needed\n\u2022 Free and Open Source\nUTM and its dependencies are all free and open source\n\u2022 Easy to Use\nConfigure and customize your VM in a native UI\n\n\nNote: Screenshots are from the updated interface only available on iOS 14.",
             "name": "UTM",
             "screenshotURLs": [
                 "https://alt.getutm.app/screen0.png",
                 "https://alt.getutm.app/screen1.png",
                 "https://alt.getutm.app/screen2.png",
                 "https://alt.getutm.app/screen3.png",
                 "https://alt.getutm.app/screen4.png",
                 "https://alt.getutm.app/screen5.png",
                 "https://alt.getutm.app/screen6.png"
             ],
-            "size": 138928961,
-            "skipPrerelease": true,
             "subtitle": "Virtual machines for iOS (with JIT support)",
             "tintColor": "1a2cc2",
-            "version": "4.0.9",
-            "versionDate": "2022-10-21T16:16:34Z",
-            "versionDescription": "## Highlights\r\n* **Multiple display and headless display is now supported for QEMU machines.** You can configure 0 or more displays as well as 0 or more builtin terminal consoles. On macOS, a new window will be created for each display and builtin terminal. On iOS, you can create multiple windows (iPad) as well as plug in an external display or AirPlay (iPad or iPhone) and assign outputs to each window.\r\n* **Ventura updates to Virtualization.** macOS Ventura introduces new features that is now integrated into UTM. You can now create GUI Linux VMs with EFI boot. Directory sharing now works with macOS Ventura guests. Rosetta x86_64 emulation is supported for Linux VMs on Apple Silicon. Check out https://docs.getutm.app/guides/debian/ for an installation guide. Note that base M1 chip users may experience issues that will be addressed in a future update.\r\n* **VirtFS sharing for QEMU.** This alternative directory sharing backend is supported by Linux and can have better performance. Note that macOS UID are numbered differently than Linux so you may have to run `chown` in the guest. Check out https://docs.getutm.app/guest-support/linux/ for more details.\r\n* **Easier Windows 10/11 installation and Windows guest tools downloader.** You can now download and mount the Windows drivers and guest tools ISO image with a single click (macOS: disk icon in VM window, iOS: 3D touch context menu on home screen). Additionally, the ISO now include an \"Autounattend.xml\" which is recognized by the Windows 10/11 installer. When mounted to a second CD drive, the installer will install the correct drivers, bypass secure boot/TPM requirements, and launch the SPICE tools installer on first login.\r\n* (macOS) **Resize QEMU disk images.** In the drives settings page, you can now expand the size of the QCOW2 disk image.\r\n* (iOS) **QEMU Virtualization for M1 iPad.** With the release of [TrollStore](https://github.com/opa334/TrollStore), you can now enable Hypervisor on iOS. Note that only M1 hardware and kernel have support for Hypervisor. iOS 14.4.2-14.5.1 is supported only on M1 iPad Pro jailbroken with fugu14/unc0ver. iOS 14.0-15.5b4 is supported on any M1 iPad running TrollStore.\r\n* **New documentation site.** https://docs.getutm.app/ is the home of the official UTM documentation.\r\n* **New localization.** Thanks to various community members, UTM is now translated to: Chinese (Simplified), Chinese (Traditional), Finnish, French, German, Japanese, Korean, and Spanish (Latin America)\r\n\r\n## Notes\r\n* **iOS 14 and macOS 11.3** are the new minimum supported systems. Please use UTM v3.x for support down to iOS 11 and macOS 11\r\n* The configuration backend has been massively rewritten. **Please backup all VMs prior to updating as you will not be able to re-open VMs saved by UTM v4 on older versions of UTM if you decide to downgrade.**\r\n* Since v4.0.6, the order of generated devices has changed to always create network devices first. This is to address an issue on some distributions (such as Ubuntu) where adding a device (drive, display, etc) would require re-configurating the network because the device name changed. Unfortunately, this change will cause the configuration issue to occur once more on any existing VM that is susceptible to the network issue. On Ubuntu, this will require you to modify `/etc/netplan/00-installer-config.yaml` and change the adapter name from `enp0s9` (or whatever it is currently) to `enp0s1` (which reflects the new device ordering). Other Linux distributions may require a similar change. However, after updating the guest network configuration, you should no longer have issues with networking when making device changes to the VM.\r\n\r\n## Changes (v4.0.9)\r\n\r\n* Fixed some broken links to documentation (#4529)\r\n* Fixed an issue where running ARM64 emulation on ARM64 gives an error \"The \u2018host\u2019 CPU type can only be used with KVM or HVF\" (#4528)\r\n* Fixed a regression where S390x and SPARC VMs cannot start due to missing USB bus\r\n* (iOS) Fixed UTM SE cannot launch any VMs (#4516)\r\n\r\n## Changes (v4.0.8)\r\n\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator and @alexis-martel)\r\n* Translation: Added German (thanks @conath)\r\n* (macOS) Disable resize button in GUI Apple VM window\r\n* (macOS) Reverted some SwiftUI issue workarounds that are no longer present in Ventura RC\r\n\r\n## Changes (v4.0.7)\r\n\r\n* Fixed renamed VM not appearing on next launch (#4469)\r\n* Fixed TCP server not working (#4479)\r\n* Fixed random network issues caused by invalid MAC address generation (you must re-generate MAC to apply the change if your VM created in UTM v4 does not have working network) (#4477)\r\n* Fixed a crash when trying to boot Kali Linux with terminal enabled\r\n* Fixed hypervisor on iOS 14.6-14.8\r\n* Added new setting for serial device in TCP server mode to listen on remote/local interfaces (#4483)\r\n* Fixed URL automation sending text to terminal\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* Wizard: Link to new documentation site (#4443, #4445)\r\n* (iOS) Fixed disponible run option not appearing\r\n* (macOS) Fixed settings getting stuck at information page (#4465)\r\n* (macOS) Updated display menu option to match title bar when multiple displays are used (#4484)\r\n* (macOS) Fixed no mouse/keyboard on Intel Apple Virtualization (#4409)\r\n* (macOS) Fixed no audio input device on Linux running on Apple Virtualization (#4409)\r\n* (macOS) Fixed auto-quit when all windows are closed happening when headless VM is still running\r\n\r\n## Changes (v4.0.6)\r\n\r\n* Fixed an issue in argument generation where PS/2 input was forced even when USB was enabled (#4424)\r\n* Validate settings on save before closing the settings dialog\r\n* Network devices are now created first before all other devices. Note this means that networking will be broken on some existing VMs and must be re-configured! (See notes above)\r\n* Fixed a deadlock issue when saving settings\r\n* Fixed an error when saving a VM with an external drive selected\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* Wizard: The Windows guest tools auto-installer currently only works on Windows 10 and above. A new option is added in the wizard to make this explicit. (#4440)\r\n* Wizard: Use VirtFS sharing by default when Linux is selected\r\n* (iOS) Default to emulated network instead of failing when importing a VM created on macOS\r\n* (macOS) Fixed an issue where opening a new display window from a serial window did not work\r\n* (macOS) Fixed logic on macOS 11 where serial window was not created\r\n* (macOS) Fixed a crash on macOS 11 when saving settings while the QEMU tab is selected\r\n* (macOS 13) Support clipboard sharing on Linux with Apple Virtualization when `spice-vdagent` is installed\r\n* (macOS) Fixed an issue changing the boot OS where the incorrect image type is prompted\r\n* (macOS) Perform settings validation when launching an Apple Virtualization VM to ensure selected features are available\r\n* (macOS 12+) Set a machine identifier when launching an Apple Virtualization VM\r\n* (macOS 13) Emulate trackpad on macOS guests with Apple Virtualization\r\n* (macOS) Fixed an issue when a newly created VM will not launch on macOS 11\r\n\r\n## Changes (v4.0.5)\r\n\r\n* Fixed moving an existing VM with Hypervisor enabled to a device on a different architecture. The VM will fallback to TCG and the option to disable hypervisor in settings is allowed. (#4407)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* (iOS) Fixed an issue that prevented external keyboards from working (#4399)\r\n* (iOS) Detect Hypervisor support on jailbroken devices so the option is not inadvertently enabled on non-supported devices\r\n* (iOS) Support Hypervisor on M1 iPad running jailbroken iOS 14.5\r\n\r\n## Changes (v4.0.4)\r\n\r\n* Fixed in issue generating configuration for IDE drives leading to PPC not booting and I/O errors on PC (#4372, #4376, others)\r\n* Moved the SPICE tools download directory to \"GuestSupportTools\" under \"Application Support\" (previously it was just under \"Application Support\")\r\n* Fixed creating a VM with illegal path characters in the name (#4385)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* Wizard: No longer tries to download the Windows guest tools when selecting a non-Windows OS\r\n* (iOS) Enable build with Hypervisor.framework (support limited to M1 iPad)\r\n* (iOS) Fixed a crash when switching display in a window\r\n* (iOS) On jailbroken devices, the memory limit will automatically be increased to the maximum, preventing the Jetsam system from terminating UTM for memory usage\r\n* (iOS) Fixed a regression which caused the home indicator to not be hidden (#4390)\r\n* (iOS) Fixed a regression which caused the cursor to not be captured (#4390)\r\n* (iOS) When switching display, notification handlers are properly cleaned up (example: cursor capture and console on screen keyboard events)\r\n* (iOS) Show the device cursor when VM is paused\r\n* (iOS) Fixed a regression where external keyboard events are not captured\r\n* (iOS) Fixed an error where extraneous stale VM entries show up after the container name changes (#4392)\r\n* (iOS) Fixed a crash on iOS 14 when opening a terminal view due to SwiftTerm handling the colour configuration\r\n* (macOS) Fixed a layout issue of the compress/resize buttons\r\n* (macOS) Forgot to actually enable compression for the drive setting button (#4377)\r\n* (macOS) Fixed some settings layout issue on < macOS 13 (#4374)\r\n\r\n## Changes (v4.0.3)\r\n\r\n* Fixed an issue where changing external drive/shared directory for a QEMU VM -> exit UTM -> reopen UTM and start the VM results in the drive/share not being restored\r\n* Disable changing a VirtFS share from the home window (this is not an supported operation)\r\n* Better detection of UUID collision which addresses an issue where VMs with the same UUID do not show up on the home screen and other VMs show up as duplicates and clicking on any of them results in a freeze\r\n* Fixed floppy drive argument not being correctly generated (#4362)\r\n* Fixed an issue where ejecting an external drive or shared directory does not persist\r\n* Fixed a memory issue when stopping or closing VMs causing UTM to crash\r\n* Fixed a regression where an access error occurs after moving a VM\r\n* Added the ability to download the Windows SPICE tools and drivers automatically (#4364)\r\n* Added support for more than 2 IDE drives in PC emulation\r\n* Restored the setting to turn off blinking cursor (#4296)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Wizard: Reworked some of the UI, text, and file selection\r\n* Wizard: Add option to auto download and mount the SPICE tools to a second CD drive\r\n* Wizard: Fixed an issue where the selected boot image and shared directory was not saved on the new VM\r\n* Wizard: Recommend UUP built ISO over the VHDX by default\r\n* Wizard: New \"confused user\" check will catch trying to mount an \"amd64\" ISO on an \"arm64\" guest or vice versa\r\n* (iOS 16) Use the new NavigationSplitView for a slightly polished look\r\n* (iOS 16) Fixed an issue where the bottom toolbar does not show up (#4325)\r\n* (iOS) Fixed an issue where the file importer was not opening (#4365)\r\n* (iOS 14) Fixed an issue in the settings screen where multiple drives were occupying a single cell\r\n* (iOS 14) Fixed an issue where UTM may crash when adding a drive or hardware\r\n* (macOS) Added the ability to re-open closed windows for a given VM (#4351)\r\n* (macOS) Fixed an issue where restarting a VM results in duplicate windows (#4367)\r\n* (macOS) Save the size of terminal windows (#4296)\r\n* (macOS) Add resize QCOW2 image feature (thanks @stewartsmith)\r\n\r\n## Changes (v4.0.2)\r\n\r\n* Removed \"view.plist\" for host-specific configuration settings (i.e. bookmarks to removable drives and window options) and replaced it with a new \"registry\" that is stored outside of the .utm bundle. Old \"view.plist\" settings and bookmarks will be migrated to the registry on first launch and the file will be deleted from the .utm bundle. For Apple VMs, the bookmarks will no longer be stored in config.plist and the settings will be migrated to the registry as well.\r\n* VirtFS no longer requires SPICE to be enabled (thanks @tie)\r\n* Fixed an issue with PPC VMs not showing 256 colours correctly (#4277)\r\n* Fixed incorrect parsing of CPU flags (#4282)\r\n* Do not save screenshots when running in disposable mode\r\n* Translation: Added Spanish (Latin America) (thanks @JezerM)\r\n* Translation: Added Finnish (thanks @marcusziade)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated Chinese (Simplified) (thanks @ty-yqs)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* (iOS) Per-display window settings (zoom, position, keyboard visibility, etc) will be stored in the new registry\r\n* (iOS) Prefer JitStreamer over AltJit when both are available (thanks @ktprograms)\r\n* (macOS) Fixed saving removable drives and shared directories for Apple VMs\r\n* (macOS) Fixed missing audio entitlements (#4342)\r\n* (macOS) Fixed QEMULauncher process not terminating when a VM is force quit\r\n* (macOS) Fixed issue selecting text in SwiftTerm (#4297)\r\n\r\n## Changes (v4.0.1)\r\n* Fixed an issue where an UEFI BIOS error was reported when the target does not use UEFI (#4265)\r\n* Added Elementary OS icon (thanks @Unbinilium)\r\n* Updated ja localization (thanks @MMP0)\r\n* Updated fr localization (thanks @FRtranslator)\r\n* Changed the icon for \"Serial\" so it appears on iOS 14 and macOS 11 as well\r\n* Fixed custom icon not showing up for \"legacy\" configurations\r\n* Fixed an error trying to migrate \"legacy\" configuration when \"Images\" does not exist (#4266)\r\n* Fixed USB redirection (#4263)\r\n* (iOS) Fixed a toolbar issue where USB button overflowed on screen.\r\n* (iOS) Fixed resume button not appearing on < iOS 16\r\n* (iOS) Attempt to close the download progress pop-up after download completes (#4261)\r\n* (iOS) \"Open\" popover refuses to show up again after swiping down (#4260)\r\n* (iOS) Hide \"Add\" text on iOS 14 settings\r\n* (iOS) Fixed crash on iOS 14 settings when attempting to use the picker (#4270)\r\n* (iOS) Fixed an issue on iOS 14 where picker selection was being reset\r\n* (iOS) Fixed an issue where the USB icon is stuck on busy after a device disconnects\r\n* (macOS) Fixed a crash trying to change shared directory for Apple VM (#4271)\r\n* (macOS) Wizard created invalid target configuration for virtualized targets (#4274)\r\n\r\n## Changes (v4.0.0)\r\n* USB redirection support in terminal mode\r\n* Configuration file format changed, newly saved VMs will not be compatible with older versions of UTM\r\n* Newly imported disk images will be converted to QCOW2 automatically\r\n* Settings: new layout with support for multiple {Display, Serial, Network, Sound} devices (#3585)\r\n* Support multiple displays (#220)\r\n* Added Japanese localization (thanks @MMP0)\r\n* Support adding PTTY (macOS only), TCP client, and TCP server serial connections for QEMU machines (address should show up in the home screen) (#3546)\r\n* Support headless display (remove all displays and built-in serial ports in the settings) (#2280)\r\n* Support redirecting QEMU monitor and GDB stub to a serial port\r\n* Support zstd compression for QCOW2 images and use zstd as default for image compression (#4211)\r\n* Update ANGLE (GL backend) to latest git commit\r\n* Added French localization (thanks @FRtranslator)\r\n* Fixed microphone recording silence (#219)\r\n* Fixed a crash when attempting to delete a QEMU additional argument\r\n* Option in VM settings to use virtfs/9pfs for file sharing (#2184)\r\n* Option in VM settings to change VGA RAM size (#4034)\r\n* Option in VM settings to enable virtio-balloon driver (#4136)\r\n* Invert mouse scrolling is now a global setting rather than a per-vm configuration option\r\n* (iOS) Replaced hterm.js with SwiftTerm for terminal mode (#3473)\r\n* (iOS) Attach to JitStreamer (set IP address in Settings app and UTM will try to connect automatically on launch) (thanks @ktprograms)\r\n* (iOS) Automatically resize the display to fit the screen when the resolution changes if the resize toolbar option is used\r\n* (iOS) Reimplemented the USB and Drives menu with a better UI\r\n* (iOS) On iPadOS 16, show the menu bar when holding Cmd on the keyboard. On previous versions, an on-screen help will show supported commands\r\n* (iOS) Improved audio handling including: output when on silence, mixing with other apps, working when both recording and outputting (including with another app) (#3996)\r\n* (iOS) Added a global setting to always prefer the built-in microphone to a bluetooth microphone\r\n* (macOS) Fixed running from shortcut in Apple VMs (no longer need to re-import after each launch)\r\n* (macOS) Improved IPSW selection interface and support drag and drop (thanks @pointum)\r\n* (macOS) Fixed running unsigned builds\r\n* (macOS) Removed some deprecated global settings\r\n* (macOS) Fixed an error when trying to download an IPSW and the Caches directory does not exist (thanks @LostInCompilation)\r\n* (macOS) Fixed an issue where a VM could be started twice if the home screen's toolbar is used leading to data corruption (#4166)\r\n* (macOS 13+) Boot into recoveryOS (to disable SIP, etc) by right clicking on the VM and selecting \"Run in recovery...\" (#3526)\r\n* (macOS 13+) Option in VM settings to enable Rosetta for x86_64 emulation (#4100)\r\n* (macOS 13+) Option in VM settings to enable clipboard sharing (SPICE support needed on the guest) (#4121)\r\n* (macOS 13+) GUI display for Linux VMs (#4120)\r\n* (macOS 13+) Add removable drives, will show up as USB mass storage\r\n\r\n## Issues\r\nPlease check the full list on [Github][2] and help report any bug you find that is not listed.\r\n\r\n## Installation\r\n\r\n* [iOS](https://docs.getutm.app/installation/ios/)\r\n* [macOS](https://docs.getutm.app/installation/macos/)\r\n\r\n| File | Description | Installation | JIT | Hypervisor | USB |\r\n|------|------------|--------------|-----|-----------|-----|\r\n| UTM.deb | Jailbroken iOS version | Open in Cydia, dpkg, or Sileo | Yes | Yes(1) | Yes |\r\n| UTM.dmg | macOS version | Mounting and copying UTM.app to /Applications | Yes | Yes | Yes |\r\n| UTM.ipa | Non-jailbroken iOS version (sideloading) | AltStore, etc (see guide) | Yes(2) | No | No |\r\n| UTM.HV.ipa | Non-jailbroken iOS version (TrollStore) | TrollStore | Yes(2) | Yes(1) | Yes |\r\n| UTM.SE.ipa | Non-jailbroken iOS version (sideloading) | AltStore, enterprise signing, etc | No | No | No |\r\n\r\n1. Hypervisor on iOS requires an M1 iPad.\r\n2. Enabling JIT may require a separate JIT enabler such as [Jitterbug][3] or Jitstreamer.\r\n\r\n[1]: https://getutm.app/install/\r\n[2]: https://github.com/utmapp/UTM/issues\r\n[3]: https://github.com/osy/Jitterbug",
             "versions": [
                 {
+                    "date": "2023-04-25T05:29:12Z",
+                    "downloadURL": "https://github.com/utmapp/UTM/releases/download/v4.2.5/UTM.ipa",
+                    "localizedDescription": "## Highlights\r\n* (iOS SE) **TCTI backend updates**. Vector instruction support can improve the performance of certain workloads.\r\n* (macOS) **Guest interface commands**. New commands accessible from the scripting interface as well as the command line interface (utmctl) can be used to read/write files, execute commands, and list IP addresses. These commands require QEMU guest agent to be installed.\r\n* (macOS) **Scripting interface additions**. The scripting interface now allows for creation of a new VM, configuration an existing VM, changing drive image, and more. See [this page](https://docs.getutm.app/scripting/reference/) for more details and [the cheat sheet](https://docs.getutm.app/scripting/cheat-sheet/) for example usage.\r\n* (macOS) **External read-write drive images**. In QEMU, if a supported drive interface is selected (USB, Floppy, etc) along with an image type of Disk, the drive can now be marked as either read-only or read-write. This can be used as an alternative way of transferring data to and from the VM when the guest does not support SPICE or VirtFS. In AVF, support for read-write images has be fixed as well (when \"read only\" is unchecked in the settings).\r\n\r\n## Changes (v4.2.5)\r\n* Reverted ANGLE to an older version which includes the fix detailed in v4.2.4 but also does not break the Metal backend (#5238)\r\n* Translation: updated Polish (thanks @matgaj, @mavethee)\r\n* (macOS) Fixed an issue where the pointer device stopped working on macOS Monterey guests (#5237)\r\n* (macOS) AVM: Added option to use emulated trackpad (requires macOS Ventura guest)\r\n\r\n## Changes (v4.2.4)\r\n* UTM will now display the release notes the first time a new version is launched\r\n* Updated ANGLE which should fix some GPU acceleration issues on Linux (please see known issues below for unresolved issues)\r\n* Fixed an issue where a removable drive or VirtIO shared directory was set up when QEMUHelper was already running and therefore was not able to create a bookmark and an \"access denied\" error shows up on startup\r\n* Introduced a new preference setting for using the Option key as Meta in the built in console. This was on by default in previous versions and is not off by default which should allow international text to be entered properly (#5202)\r\n* Wizard: Make virtio-gpu-pci default for Linux (again) which was reverted a few releases ago in order to address some GPU issues\r\n* Translation: updated Polish (thanks @matgaj)\r\n* (iOS) Fixed built in terminal overlapping in the safe area\r\n\r\n## Changes (v4.2.3)\r\n* Added support for read-write removable devices on supported interfaces (USB, Floppy, etc). To use this feature, set the image type to \"Disk\" and uncheck the \"Read Only?\" option in the drive settings. Note that you may have to eject and re-mount the drive image for effect to take place. (#5079)\r\n* Removable USB devices will no longer show up as a CD drive if the image type is set to \"Disk\" (#5171)\r\n* Reverted a change from v4.2.0 where virtio bus devices were removed (this broke some people's configurations) (#5137)\r\n* Fixed an issue where when QEMU fails to start, subsequent attempts to start the VM will automatically fail\r\n* Fixed an issue where due to a race, removable drives may not be mounted on start\r\n* (iOS) Fixed an issue when the pointer is hovering over a toolbar button when the VM starts and subsequent clicks will toggle the button (#4843)\r\n* (macOS) AVF: Fixed an issue where a removable drive that is not marked as read-only still gets marked as read-only after restarting UTM (when upgrading from a previous version, you must eject and re-mount the image for effect to take place) (#5170)\r\n* (macOS) Fixed an issue where incorrect subnet parameters are generated for vmnet advanced settings (#5128)\r\n* (macOS) CLI: Added a new `clone` command (#5004)\r\n\r\n## Changes (v4.2.2)\r\n* Fixed an issue where a VM that is moved manually (e.g. with Finder) cannot be started (#5121)\r\n* Fixed an issue where the cursor disappears after resuming a suspended VM (#4665)\r\n* (macOS) Scripting: Add support for `make`, `duplicate`, and `delete` verbs on virtual machines\r\n* (macOS) Scripting: Add support for modifying certain configuration options\r\n* (macOS) Scripting: Removed virtual machine properties: `notes`, `machine`, `architecture`, `memory`. You should now use similar properties in the `configuration` record\r\n* (macOS) Support changing the audio backend to CoreAudio and make CoreAudio the default (due to better latency and as a workaround to some crashes) (#5125)\r\n\r\n## Changes (v4.2.1)\r\n* QEMU: Support more than 8 cores for ARM64 targets (#4847)\r\n* Synchronize time on resume when QEMU guest agent is installed which should fix clock drift issues (#3218)\r\n* (iOS SE) Updated TCTI to latest branch from @ktemkin which has support for vector instructions (#4865)\r\n* (macOS) Switch to emulated trackpad when guest+host are macOS 13+ (second attempt for #4636 and #4645)\r\n* (macOS) Fixed the \"raw image\" checkbox when creating a new drive (#5100)\r\n* (macOS) Add PC speaker sound device as an option. You can now add a second sound device on supported targets (x86_64/i386 PC based targets) and set the hardware to PC Speaker to emulate older motherboard speakers.\r\n* (macOS) Scripting: new verbs \"open file\", \"execute\", and \"query ip\" which uses the QEMU guest agent to send commands to the guest. Use the Apple Script Editor's Open Dictionary tool for more information.\r\n* (macOS) CLI: new commands \"file push\", \"file pull\", \"exec\", and \"ip-address\". See `utmctl help` for more information.\r\n\r\n## Changes (v4.2.0)\r\n* Updated virglrenderer to latest (27/02/2023) commit\r\n* Automatically revert CPU to \"default\" if model is missing due to updated QEMU (#4910)\r\n* ~~Remove virtio-bus devices (they didn't work) (#4893)~~\r\n* Support drag and drop to import an .utm package (#3599)\r\n* Support copying sparse images across different volumes (thanks @ktprograms)\r\n* Fixed tearing/performance issue for non-GL accelerated displays when under graphics load (#5049)\r\n* Fixed error when importing a new drive with the same name as an existing drive (#5052)\r\n* ~~Fixed a crash on startup when multiple audio devices are plugged in (#4629)~~\r\n* Wizard: Generate a working configuration for isapc (#4961)\r\n* Settings: Use pretty labels for CPU flags (#4940)\r\n* Translation: updated French (thanks @FRtranslator)\r\n* Translation: added Czech readme (thanks @stinovlasmp)\r\n* Translation: updated German (thanks @LostInCompilation and @afh)\r\n* (macOS) Capture Mouse has been renamed to Capture Input and now will show the current capture status as a toggle button\r\n* (macOS) Apple VMs (macOS guests) now support Capture Input which will capture the system keys. This used to be always on as the default. It is now off by default and the toggle button will enable it. (#4667)\r\n* (macOS) Ignore missing links (drives, shared directory, etc) when saving an Apple VM\r\n* (macOS) Preference: added option to force Num Lock on (#4625)\r\n* (macOS) Preference: added option to prevent idle sleep while VM is running (#4963)\r\n* (macOS) Preference: added option to suppress exit confirmation (#4989)\r\n* (macOS) Fixed delete drive confirmation not showing up on latest macOS\r\n* (macOS) Fixed disposable mode stuck on when a VM is run once in disposable mode (#5025)\r\n* (macOS) Fixed an issue where a moved or deleted VM with a stopped window open will attempt to use the old path (#4985)\r\n* (macOS) Fixed cursor scrolling and double click issues (#4636, #4645)\r\n* (macOS) Support following a change in system default input or output audio device (#3488)\r\n* (macOS) Support retry of macOS installation when it fails (the IPSW will not automatically be unlinked)\r\n* (macOS) Support retaining of installer IPSW bookmark across VM moves and UTM restarts (#4938)\r\n\r\n## Issues\r\nPlease check the full list on [Github](https://github.com/utmapp/UTM/issues) and help report any bug you find that is not listed.\r\n\r\n* There is a known bug in newer versions of Mesa which prevents some Wayland applications (such as Firefox) from launching when GPU acceleration is enabled. One workaround is to switch to Xorg from the log-in screen (typically by clicking on the gear icon) and another is to patch Mesa to a newer version.\r\n* Debian 12 fails to load the GUI installer when GPU acceleration is enabled. Please use the text installer instead.\r\n\r\n## Installation\r\n\r\n* [iOS](https://docs.getutm.app/installation/ios/)\r\n* [macOS](https://docs.getutm.app/installation/macos/)\r\n\r\n| File | Description | Installation | JIT | Hypervisor | USB |\r\n|------|------------|--------------|-----|-----------|-----|\r\n| UTM.deb | Jailbroken iOS version | Open in Cydia, dpkg, or Sileo | Yes | Yes(1) | Yes |\r\n| UTM.dmg | macOS version | Mounting and copying UTM.app to /Applications | Yes | Yes | Yes |\r\n| UTM.ipa | Non-jailbroken iOS version (sideloading) | AltStore, etc (see guide) | Yes(2) | No | No |\r\n| UTM.HV.ipa | Non-jailbroken iOS version (TrollStore) | TrollStore | Yes | Yes(1) | Yes |\r\n| UTM.SE.ipa | Non-jailbroken iOS version (sideloading) | AltStore, enterprise signing, etc | No | No | No |\r\n\r\n1. Hypervisor on iOS requires an M1 iPad.\r\n2. Enabling JIT may require a separate JIT enabler such as [Jitterbug][2] or Jitstreamer.\r\n\r\n[1]: https://getutm.app/install/\r\n[2]: https://github.com/osy/Jitterbug",
+                    "sha256": "a4591cc068fde4d77805d10f5b8b779eb92a9bb36c20cd97e4d6af7ad3b55593",
+                    "size": 121911309,
+                    "version": "4.2.5"
+                },
+                {
+                    "date": "2023-04-23T22:15:49Z",
+                    "downloadURL": "https://github.com/utmapp/UTM/releases/download/v4.2.4/UTM.ipa",
+                    "localizedDescription": "## Highlights\r\n* (iOS SE) **TCTI backend updates**. Vector instruction support can improve the performance of certain workloads.\r\n* (macOS) **Guest interface commands**. New commands accessible from the scripting interface as well as the command line interface (utmctl) can be used to read/write files, execute commands, and list IP addresses. These commands require QEMU guest agent to be installed.\r\n* (macOS) **Scripting interface additions**. The scripting interface now allows for creation of a new VM, configuration an existing VM, changing drive image, and more. See [this page](https://docs.getutm.app/scripting/reference/) for more details and [the cheat sheet](https://docs.getutm.app/scripting/cheat-sheet/) for example usage.\r\n* (macOS) **External read-write drive images**. In QEMU, if a supported drive interface is selected (USB, Floppy, etc) along with an image type of Disk, the drive can now be marked as either read-only or read-write. This can be used as an alternative way of transferring data to and from the VM when the guest does not support SPICE or VirtFS. In AVF, support for read-write images has be fixed as well (when \"read only\" is unchecked in the settings).\r\n\r\n## Changes (v4.2.4)\r\n* UTM will now display the release notes the first time a new version is launched\r\n* Updated ANGLE which should fix some GPU acceleration issues on Linux (please see known issues below for unresolved issues)\r\n* Fixed an issue where a removable drive or VirtIO shared directory was set up when QEMUHelper was already running and therefore was not able to create a bookmark and an \"access denied\" error shows up on startup\r\n* Introduced a new preference setting for using the Option key as Meta in the built in console. This was on by default in previous versions and is not off by default which should allow international text to be entered properly (#5202)\r\n* Wizard: Make virtio-gpu-pci default for Linux (again) which was reverted a few releases ago in order to address some GPU issues\r\n* Translation: updated Polish (thanks @matgaj)\r\n* (iOS) Fixed built in terminal overlapping in the safe area\r\n\r\n## Changes (v4.2.3)\r\n* Added support for read-write removable devices on supported interfaces (USB, Floppy, etc). To use this feature, set the image type to \"Disk\" and uncheck the \"Read Only?\" option in the drive settings. Note that you may have to eject and re-mount the drive image for effect to take place. (#5079)\r\n* Removable USB devices will no longer show up as a CD drive if the image type is set to \"Disk\" (#5171)\r\n* Reverted a change from v4.2.0 where virtio bus devices were removed (this broke some people's configurations) (#5137)\r\n* Fixed an issue where when QEMU fails to start, subsequent attempts to start the VM will automatically fail\r\n* Fixed an issue where due to a race, removable drives may not be mounted on start\r\n* (iOS) Fixed an issue when the pointer is hovering over a toolbar button when the VM starts and subsequent clicks will toggle the button (#4843)\r\n* (macOS) AVF: Fixed an issue where a removable drive that is not marked as read-only still gets marked as read-only after restarting UTM (when upgrading from a previous version, you must eject and re-mount the image for effect to take place) (#5170)\r\n* (macOS) Fixed an issue where incorrect subnet parameters are generated for vmnet advanced settings (#5128)\r\n* (macOS) CLI: Added a new `clone` command (#5004)\r\n\r\n## Changes (v4.2.2)\r\n* Fixed an issue where a VM that is moved manually (e.g. with Finder) cannot be started (#5121)\r\n* Fixed an issue where the cursor disappears after resuming a suspended VM (#4665)\r\n* (macOS) Scripting: Add support for `make`, `duplicate`, and `delete` verbs on virtual machines\r\n* (macOS) Scripting: Add support for modifying certain configuration options\r\n* (macOS) Scripting: Removed virtual machine properties: `notes`, `machine`, `architecture`, `memory`. You should now use similar properties in the `configuration` record\r\n* (macOS) Support changing the audio backend to CoreAudio and make CoreAudio the default (due to better latency and as a workaround to some crashes) (#5125)\r\n\r\n## Changes (v4.2.1)\r\n* QEMU: Support more than 8 cores for ARM64 targets (#4847)\r\n* Synchronize time on resume when QEMU guest agent is installed which should fix clock drift issues (#3218)\r\n* (iOS SE) Updated TCTI to latest branch from @ktemkin which has support for vector instructions (#4865)\r\n* (macOS) Switch to emulated trackpad when guest+host are macOS 13+ (second attempt for #4636 and #4645)\r\n* (macOS) Fixed the \"raw image\" checkbox when creating a new drive (#5100)\r\n* (macOS) Add PC speaker sound device as an option. You can now add a second sound device on supported targets (x86_64/i386 PC based targets) and set the hardware to PC Speaker to emulate older motherboard speakers.\r\n* (macOS) Scripting: new verbs \"open file\", \"execute\", and \"query ip\" which uses the QEMU guest agent to send commands to the guest. Use the Apple Script Editor's Open Dictionary tool for more information.\r\n* (macOS) CLI: new commands \"file push\", \"file pull\", \"exec\", and \"ip-address\". See `utmctl help` for more information.\r\n\r\n## Changes (v4.2.0)\r\n* Updated virglrenderer to latest (27/02/2023) commit\r\n* Automatically revert CPU to \"default\" if model is missing due to updated QEMU (#4910)\r\n* ~~Remove virtio-bus devices (they didn't work) (#4893)~~\r\n* Support drag and drop to import an .utm package (#3599)\r\n* Support copying sparse images across different volumes (thanks @ktprograms)\r\n* Fixed tearing/performance issue for non-GL accelerated displays when under graphics load (#5049)\r\n* Fixed error when importing a new drive with the same name as an existing drive (#5052)\r\n* ~~Fixed a crash on startup when multiple audio devices are plugged in (#4629)~~\r\n* Wizard: Generate a working configuration for isapc (#4961)\r\n* Settings: Use pretty labels for CPU flags (#4940)\r\n* Translation: updated French (thanks @FRtranslator)\r\n* Translation: added Czech readme (thanks @stinovlasmp)\r\n* Translation: updated German (thanks @LostInCompilation and @afh)\r\n* (macOS) Capture Mouse has been renamed to Capture Input and now will show the current capture status as a toggle button\r\n* (macOS) Apple VMs (macOS guests) now support Capture Input which will capture the system keys. This used to be always on as the default. It is now off by default and the toggle button will enable it. (#4667)\r\n* (macOS) Ignore missing links (drives, shared directory, etc) when saving an Apple VM\r\n* (macOS) Preference: added option to force Num Lock on (#4625)\r\n* (macOS) Preference: added option to prevent idle sleep while VM is running (#4963)\r\n* (macOS) Preference: added option to suppress exit confirmation (#4989)\r\n* (macOS) Fixed delete drive confirmation not showing up on latest macOS\r\n* (macOS) Fixed disposable mode stuck on when a VM is run once in disposable mode (#5025)\r\n* (macOS) Fixed an issue where a moved or deleted VM with a stopped window open will attempt to use the old path (#4985)\r\n* (macOS) Fixed cursor scrolling and double click issues (#4636, #4645)\r\n* (macOS) Support following a change in system default input or output audio device (#3488)\r\n* (macOS) Support retry of macOS installation when it fails (the IPSW will not automatically be unlinked)\r\n* (macOS) Support retaining of installer IPSW bookmark across VM moves and UTM restarts (#4938)\r\n\r\n## Issues\r\nPlease check the full list on [Github](https://github.com/utmapp/UTM/issues) and help report any bug you find that is not listed.\r\n\r\n* There is a known bug in newer versions of Mesa which prevents some Wayland applications (such as Firefox) from launching when GPU acceleration is enabled. One workaround is to switch to Xorg from the log-in screen (typically by clicking on the gear icon) and another is to patch Mesa to a newer version.\r\n* Debian 12 fails to load the GUI installer when GPU acceleration is enabled. Please use the text installer instead.\r\n* The Metal renderer backend is broken on macOS, please change your renderer to OpenGL or \"Default\"\r\n\r\n## Installation\r\n\r\n* [iOS](https://docs.getutm.app/installation/ios/)\r\n* [macOS](https://docs.getutm.app/installation/macos/)\r\n\r\n| File | Description | Installation | JIT | Hypervisor | USB |\r\n|------|------------|--------------|-----|-----------|-----|\r\n| UTM.deb | Jailbroken iOS version | Open in Cydia, dpkg, or Sileo | Yes | Yes(1) | Yes |\r\n| UTM.dmg | macOS version | Mounting and copying UTM.app to /Applications | Yes | Yes | Yes |\r\n| UTM.ipa | Non-jailbroken iOS version (sideloading) | AltStore, etc (see guide) | Yes(2) | No | No |\r\n| UTM.HV.ipa | Non-jailbroken iOS version (TrollStore) | TrollStore | Yes | Yes(1) | Yes |\r\n| UTM.SE.ipa | Non-jailbroken iOS version (sideloading) | AltStore, enterprise signing, etc | No | No | No |\r\n\r\n1. Hypervisor on iOS requires an M1 iPad.\r\n2. Enabling JIT may require a separate JIT enabler such as [Jitterbug][2] or Jitstreamer.\r\n\r\n[1]: https://getutm.app/install/\r\n[2]: https://github.com/osy/Jitterbug",
+                    "sha256": "5d2af58d560086ee6714c861d3a81a918cc76bdb1251fb21a088c1bf2a044e47",
+                    "size": 121701488,
+                    "version": "4.2.4"
+                },
+                {
+                    "date": "2023-02-27T02:28:31Z",
+                    "downloadURL": "https://github.com/utmapp/UTM/releases/download/v4.1.6/UTM.ipa",
+                    "localizedDescription": "This is the same release as v4.1.5 but with the change to default enable GPU acceleration for Linux reverted. This is due to a number of guest-side driver issues in the latest version of Mesa (#4983). As a result of these issues, we decided to disable GPU acceleration in Linux by default for new VMs created by the wizard. If you have an existing VM with graphical issues, you can disable GPU acceleration by going into the VM settings, under Display, change the Emulated Display Card to `virtio-gpu-pci` or another card that does not have `-gl` in the name. You can verify that GPU acceleration is disabled when the checkbox below the card is unchecked.\r\n\r\n## Highlights\r\n* **QEMU backend updated to v7.2.0**. Also updated usbredir (0.13.0), virglrenderer (latest commit), ANGLE (latest commit)\r\n* **Improved renderer backend**. Lots of bug fixes and stability improvements to GPU accelerated Linux VMs (most common crashes when GPU acceleration is enabled should be gone now). New option to change the renderer backend to ANGLE Metal and limit FPS (in Preferences). Switching to Metal is highly recommended.\r\n* (iOS) **TrollStore build (UTM.HV.ipa) now supports JIT**. Additionally, there is now in-app settings.\r\n* (iOS) **TrollStore build now supports TSO (Total Store Ordering)**. TSO is used by Rosetta on the Mac to improve x86_64 emulation on ARM64. It can now be used on M1 iPads with QEMU to improve performance of FEX-Emu or a patched Rosetta. Note that it is recommended that TSO be disabled if you do not need to emulate x86_64 because it can reduce performance of other tasks.\r\n* (macOS) **AppleScript (OSA) support and CLI interface**. You can control parts of UTM through the OSA interface. Currently there is support for listing VMs as well as start/stop/suspend operations and the ability to print out the guest serial port connections. More functionality will be added in the future. A command line application is also provided in `UTM.app/Contents/MacOS/utmctl` (which you can symlink to `/usr/local/bin/utmctl` if desired) that can be used for automation tasks without needing to learn AppleScript.\r\n* (macOS 13+) **Menu bar extra**. You can enable the menu bar extra icon in Preferences (Cmd+,) as well as disable the dock icon. The menu bar extra provides a minimal interface to start/stop/suspend VMs and is useful when paired with headless VMs (a VM that does not have any display or terminal console installed).\r\n\r\n## Notes\r\n* **iOS 14 and macOS 11.3** are the minimum supported systems for UTM v4.x. Please use UTM v3.x for support down to iOS 11 and macOS 11\r\n* ~~Newly created Linux VMs will now use `virtio-gpu-gl-pci` by default. It is recommended that you change the display card of existing QEMU backend Linux VMs to this card in order to take advantage of the improved renderer backend. This should result in improved performance in GUI rendering. Note that some applications (particularly 3D applications) may lock up or crash UTM and if you are experiencing issues, you can go back to `virtio-ramfb` or `virtio-vga`.~~\r\n* Newly created Windows VMs will now use `virtio-ramfb-gl` (Apple Silicon) or `virtio-vga-gl` (Intel) by default. There is NO 3D acceleration drivers for Windows yet, so unlike Linux, this will not improve any compatibility with applications. However, the GL backend can still be beneficial to Windows users because it has smoother animations and less tearing and artifacts. The overall benefits will not be as pronounced as for Linux VMs so it is optional that you change existing VMs to a `-gl` display card.\r\n* (iOS) It is recommended that you switch to the Metal backend in Preferences for better performance. However, some applications such as `glxgears` will not work with the Metal backend.\r\n\r\n## Changes (v4.1.6)\r\n* Wizard: Re-introduced the checkbox for \"Hardware OpenGL Acceleration\" which is disabled by default due to guest-side issues in the latest Mesa driver\r\n\r\n## Changes (v4.1.5)\r\n* Improved rendering of non-GL graphics on the new renderer backend. This should reduce some of the tearing seen in earlier updates. For the best performance, it is recommended that a GL backend is selected.\r\n* Support read-only disk images in QEMU backend as well as selecting images that are read-only (#4838) Note: all external drive images (ISOs) are now loaded as read-only, this was not enforced in previous versions due to an error in the logic.\r\n* Newly created Windows VMs will now use `virtio-ramfb-gl` (Apple Silicon) or `virtio-vga-gl` (Intel) by default. See the Notes section for more information.\r\n* Fixed an issue where the incorrect tmp directory path was used by QEMU (#4882)\r\n* Scripting: Fixed an issue where the proper error message was not displayed in some cases.\r\n* CLI: Improved some help text.\r\n* Localization: updated Japanese (thanks @MMP0)\r\n\r\n## Changes (v4.1.4)\r\n* Fixed slow rendering of GRUB and EFI menus\r\n* Introduced new optimizations to renderer: bliting done on GPU instead of CPU now (for non-GL rendering), guest draw calls that are faster than the monitor refresh rate are now consolidated before drawing at vblank, rendering of multiple displays can happen concurrently now\r\n* Fixed rendering to multiple displays on the new renderer backend\r\n* Fixed an issue in QEMU where the vmnet backend uses 100% of CPU when the VM is suspended (#4803)\r\n* (iOS) TrollStore: Fixed JIT enable in the HV builds\r\n* (iOS) TrollStore: New option to enable TSO (Total Store Ordering) in QEMU settings (see Highlights for more details)\r\n* (iOS) Restored the default renderer backend to GL. This was changed in v4.1.3 because Metal is faster but the new backend can introduce regressions such as `glxgears` not working (#4856). As a result, the new backend is now opt-in but is still highly recommended.\r\n* (iOS) Fixed crash when changing VM settings on iOS 14 (#4864)\r\n* (iOS) Fixed crash when starting a VM with UTM SE (#4848)\r\n* (macOS) A tooltip will now reveal why suspend functionality is disabled\r\n\r\n## Changes (v4.1.3)\r\n* Updated QEMU to v7.2.0\r\n* Reworked CocoaSpice renderer to respond faster to GL updates from the guest, should improve frame pacing on GL supported Linux VMs\r\n* Added global setting to change renderer backend, introduce ANGLE Metal as an option (and also the new default for iOS)\r\n* Added global setting to limit FPS which can be used to improve frame pacing for a smoother rendering experience\r\n* Settings: clearly show if the current display hardware supports GPU acceleration\r\n* Wizard: GPU acceleration is now enabled by default when Linux is selected as the operating system\r\n* Fixed crash due to an error with `GL_DRAW_COOKIE_INVALID` (#4722)\r\n* Fixed deadlock on startup caused by gstosxaudio (#2364)\r\n* Fixed memory leak when GPU acceleration is enabled (#4449)\r\n* Fixed crash in `-[MTLResourceList releaseAllObjectsAndReset]` (#3519)\r\n* Fixed Mesa issue causing some GNOME desktop to freeze when GPU acceleration is enabled\r\n* Fixed incorrect logic when cloning a VM (#4815)\r\n* Fixed some thread scheduling warning (#4352)\r\n* Localization: updated French (thanks @FRtranslator)\r\n* (iOS) TrollStore build: use `com.apple.private.security.no-sandbox` instead of `com.apple.private.security.no-container` on recommendation of other devs and to align with how other apps perform JIT.\r\n* (iOS) Fixed blank screen when choosing \"Open\" in the wizard (#4842)\r\n* (iOS) Fixed toolbar not auto-hiding before first interaction (#4844)\r\n* (macOS) New design for global settings (Cmd+,) which better organizes the settings\r\n* (macOS) utmctl: Fixed crash when `utmctl help attach` runs (#4817)\r\n* (macOS) utmctl: Fixed `utmctl stop` with `--request` and `kill` (#4850)\r\n\r\n## Changes (v4.1.2)\r\n* Localization: updated Spanish (Latin America) (thanks @JezerM)\r\n* Localization: updated Japanese (thanks @MMP0 and @skyarrow87)\r\n* Localization: updated Chinese Simplified (thanks @changanmoon)\r\n* (iOS) Fix new VM wizard not appearing on < iOS 14.5 (#4776)\r\n* (macOS) Implement OSA interface for AppleScript\r\n* (macOS) Introduce a CLI application (`UTM.app/Contents/MacOS/utmctl`) that wraps around the OSA interface for automation\r\n* (macOS 13+) New settings option to enable a menu bar extra icon for controlling VMs\r\n* (macOS 13+) New settings option to disable the dock icon\r\n* (macOS) Fix various alignment issues in settings (#4596) (thanks @JezerM)\r\n* (macOS) Fix a crash when the pasteboard is updated (#4745)\r\n* (macOS) Support custom resolutions for Apple Virtualization VMs\r\n* (macOS) Fixed a UI freeze when canceling out of the settings for an Apple Virtualization VM\r\n\r\n## Changes (v4.1.1)\r\n* Fixed launching SPARC machines (#4575)\r\n* Fixed an error when attempting to save a VM where one of its removable drives is linked to a file that has been deleted\r\n* Fixed IPSW/.utm download failing when the device goes to sleep (the download should resume after wake up)\r\n* Restored scroll bars when system is set to always show scroll bars. Added a new SwiftUI crash workaround thanks to @evelyneee.\r\n* Display all sizes in binary (MiB/GiB) mode in order to be consistent (#4396)\r\n* Localization: added Polish (thanks @mavethee)\r\n* Localization: updated Japanese (thanks @MMP0)\r\n* Localization: updated Spanish (Latin America) (thanks @JezerM)\r\n* Localization: updated French (thanks @FRtranslator)\r\n* (macOS) Fixed the port forward UI on macOS 11 and introduce a new port forward UI for macOS 12+ (#4690)\r\n* (macOS) Fixed \"This virtual machine cannot be run on this machine.\" error on a newly created Apple VM (#4595)\r\n* (macOS) Added new 21:9 widescreen resolution for Apple VMs (thanks @Tandolf)\r\n* (macOS) Added a clarifying message about shared directory support on older macOS guests (#4594)\r\n* (macOS) Added new shutdown options (software request and force kill) which can be toggled by long pressing the power button in the VM window (#4001)\r\n* (macOS) Added a confirmation dialog when deleting a drive (#4687)\r\n\r\n## Changes (v4.1.0)\r\n* Updated QEMU to v7.1.0\r\n* Updated ANGLE and virglrenderer to latest commit\r\n* Fixed an issue where user override of machine property settings was not applied properly\r\n* Localization: updated Japanese (thanks @MMP0)\r\n* Localization: updated Spanish (Latin America) (thanks @JezerM)\r\n* (iOS) Added in-app settings popover which synchronizes with the Settings app (useful for TrollStore installs where the Settings app page is inaccessible) (#4446)\r\n* (iOS) TrollStore: support JIT without needing a separate JIT enabler (thanks @PojavLauncherTeam for the idea)\r\n\r\n## Issues\r\nPlease check the full list on [Github][2] and help report any bug you find that is not listed.\r\n\r\n## Installation\r\n\r\n* [iOS](https://docs.getutm.app/installation/ios/)\r\n* [macOS](https://docs.getutm.app/installation/macos/)\r\n\r\n| File | Description | Installation | JIT | Hypervisor | USB |\r\n|------|------------|--------------|-----|-----------|-----|\r\n| UTM.deb | Jailbroken iOS version | Open in Cydia, dpkg, or Sileo | Yes | Yes(1) | Yes |\r\n| UTM.dmg | macOS version | Mounting and copying UTM.app to /Applications | Yes | Yes | Yes |\r\n| UTM.ipa | Non-jailbroken iOS version (sideloading) | AltStore, etc (see guide) | Yes(2) | No | No |\r\n| UTM.HV.ipa | Non-jailbroken iOS version (TrollStore) | TrollStore | Yes | Yes(1) | Yes |\r\n| UTM.SE.ipa | Non-jailbroken iOS version (sideloading) | AltStore, enterprise signing, etc | No | No | No |\r\n\r\n1. Hypervisor on iOS requires an M1 iPad.\r\n2. Enabling JIT may require a separate JIT enabler such as [Jitterbug][3] or Jitstreamer.\r\n\r\n[1]: https://getutm.app/install/\r\n[2]: https://github.com/utmapp/UTM/issues\r\n[3]: https://github.com/osy/Jitterbug",
+                    "sha256": "85c12ff30c33a0a2911dcdbd8a19f3c3726a74500e4082edde9a667b8f83bcdb",
+                    "size": 121696501,
+                    "version": "4.1.6"
+                },
+                {
+                    "date": "2023-01-04T04:12:52Z",
+                    "downloadURL": "https://github.com/utmapp/UTM/releases/download/v4.1.5/UTM.ipa",
+                    "localizedDescription": "## Highlights\r\n* **QEMU backend updated to v7.2.0**. Also updated usbredir (0.13.0), virglrenderer (latest commit), ANGLE (latest commit)\r\n* **Improved renderer backend**. Lots of bug fixes and stability improvements to GPU accelerated Linux VMs (most common crashes when GPU acceleration is enabled should be gone now). New option to change the renderer backend to ANGLE Metal and limit FPS (in Preferences). Switching to Metal is highly recommended.\r\n* (iOS) **TrollStore build (UTM.HV.ipa) now supports JIT**. Additionally, there is now in-app settings.\r\n* (iOS) **TrollStore build now supports TSO (Total Store Ordering)**. TSO is used by Rosetta on the Mac to improve x86_64 emulation on ARM64. It can now be used on M1 iPads with QEMU to improve performance of FEX-Emu or a patched Rosetta. Note that it is recommended that TSO be disabled if you do not need to emulate x86_64 because it can reduce performance of other tasks.\r\n* (macOS) **AppleScript (OSA) support and CLI interface**. You can control parts of UTM through the OSA interface. Currently there is support for listing VMs as well as start/stop/suspend operations and the ability to print out the guest serial port connections. More functionality will be added in the future. A command line application is also provided in `UTM.app/Contents/MacOS/utmctl` (which you can symlink to `/usr/local/bin/utmctl` if desired) that can be used for automation tasks without needing to learn AppleScript.\r\n* (macOS 13+) **Menu bar extra**. You can enable the menu bar extra icon in Preferences (Cmd+,) as well as disable the dock icon. The menu bar extra provides a minimal interface to start/stop/suspend VMs and is useful when paired with headless VMs (a VM that does not have any display or terminal console installed).\r\n\r\n## Notes\r\n* **iOS 14 and macOS 11.3** are the minimum supported systems for UTM v4.x. Please use UTM v3.x for support down to iOS 11 and macOS 11\r\n* Newly created Linux VMs will now use `virtio-gpu-gl-pci` by default. It is recommended that you change the display card of existing QEMU backend Linux VMs to this card in order to take advantage of the improved renderer backend. This should result in improved performance in GUI rendering. Note that some applications (particularly 3D applications) may lock up or crash UTM and if you are experiencing issues, you can go back to `virtio-ramfb` or `virtio-vga`.\r\n* Newly created Windows VMs will now use `virtio-ramfb-gl` (Apple Silicon) or `virtio-vga-gl` (Intel) by default. There is NO 3D acceleration drivers for Windows yet, so unlike Linux, this will not improve any compatibility with applications. However, the GL backend can still be beneficial to Windows users because it has smoother animations and less tearing and artifacts. The overall benefits will not be as pronounced as for Linux VMs so it is optional that you change existing VMs to a `-gl` display card.\r\n* (iOS) It is recommended that you switch to the Metal backend in Preferences for better performance. However, some applications such as `glxgears` will not work with the Metal backend.\r\n\r\n## Changes (v4.1.5)\r\n* Improved rendering of non-GL graphics on the new renderer backend. This should reduce some of the tearing seen in earlier updates. For the best performance, it is recommended that a GL backend is selected.\r\n* Support read-only disk images in QEMU backend as well as selecting images that are read-only (#4838) Note: all external drive images (ISOs) are now loaded as read-only, this was not enforced in previous versions due to an error in the logic.\r\n* Newly created Windows VMs will now use `virtio-ramfb-gl` (Apple Silicon) or `virtio-vga-gl` (Intel) by default. See the Notes section for more information.\r\n* Fixed an issue where the incorrect tmp directory path was used by QEMU (#4882)\r\n* Scripting: Fixed an issue where the proper error message was not displayed in some cases.\r\n* CLI: Improved some help text.\r\n* Localization: updated Japanese (thanks @MMP0)\r\n\r\n## Changes (v4.1.4)\r\n* Fixed slow rendering of GRUB and EFI menus\r\n* Introduced new optimizations to renderer: bliting done on GPU instead of CPU now (for non-GL rendering), guest draw calls that are faster than the monitor refresh rate are now consolidated before drawing at vblank, rendering of multiple displays can happen concurrently now\r\n* Fixed rendering to multiple displays on the new renderer backend\r\n* Fixed an issue in QEMU where the vmnet backend uses 100% of CPU when the VM is suspended (#4803)\r\n* (iOS) TrollStore: Fixed JIT enable in the HV builds\r\n* (iOS) TrollStore: New option to enable TSO (Total Store Ordering) in QEMU settings (see Highlights for more details)\r\n* (iOS) Restored the default renderer backend to GL. This was changed in v4.1.3 because Metal is faster but the new backend can introduce regressions such as `glxgears` not working (#4856). As a result, the new backend is now opt-in but is still highly recommended.\r\n* (iOS) Fixed crash when changing VM settings on iOS 14 (#4864)\r\n* (iOS) Fixed crash when starting a VM with UTM SE (#4848)\r\n* (macOS) A tooltip will now reveal why suspend functionality is disabled\r\n\r\n## Changes (v4.1.3)\r\n* Updated QEMU to v7.2.0\r\n* Reworked CocoaSpice renderer to respond faster to GL updates from the guest, should improve frame pacing on GL supported Linux VMs\r\n* Added global setting to change renderer backend, introduce ANGLE Metal as an option (and also the new default for iOS)\r\n* Added global setting to limit FPS which can be used to improve frame pacing for a smoother rendering experience\r\n* Settings: clearly show if the current display hardware supports GPU acceleration\r\n* Wizard: GPU acceleration is now enabled by default when Linux is selected as the operating system\r\n* Fixed crash due to an error with `GL_DRAW_COOKIE_INVALID` (#4722)\r\n* Fixed deadlock on startup caused by gstosxaudio (#2364)\r\n* Fixed memory leak when GPU acceleration is enabled (#4449)\r\n* Fixed crash in `-[MTLResourceList releaseAllObjectsAndReset]` (#3519)\r\n* Fixed Mesa issue causing some GNOME desktop to freeze when GPU acceleration is enabled\r\n* Fixed incorrect logic when cloning a VM (#4815)\r\n* Fixed some thread scheduling warning (#4352)\r\n* Localization: updated French (thanks @FRtranslator)\r\n* (iOS) TrollStore build: use `com.apple.private.security.no-sandbox` instead of `com.apple.private.security.no-container` on recommendation of other devs and to align with how other apps perform JIT.\r\n* (iOS) Fixed blank screen when choosing \"Open\" in the wizard (#4842)\r\n* (iOS) Fixed toolbar not auto-hiding before first interaction (#4844)\r\n* (macOS) New design for global settings (Cmd+,) which better organizes the settings\r\n* (macOS) utmctl: Fixed crash when `utmctl help attach` runs (#4817)\r\n* (macOS) utmctl: Fixed `utmctl stop` with `--request` and `kill` (#4850)\r\n\r\n## Changes (v4.1.2)\r\n* Localization: updated Spanish (Latin America) (thanks @JezerM)\r\n* Localization: updated Japanese (thanks @MMP0 and @skyarrow87)\r\n* Localization: updated Chinese Simplified (thanks @changanmoon)\r\n* (iOS) Fix new VM wizard not appearing on < iOS 14.5 (#4776)\r\n* (macOS) Implement OSA interface for AppleScript\r\n* (macOS) Introduce a CLI application (`UTM.app/Contents/MacOS/utmctl`) that wraps around the OSA interface for automation\r\n* (macOS 13+) New settings option to enable a menu bar extra icon for controlling VMs\r\n* (macOS 13+) New settings option to disable the dock icon\r\n* (macOS) Fix various alignment issues in settings (#4596) (thanks @JezerM)\r\n* (macOS) Fix a crash when the pasteboard is updated (#4745)\r\n* (macOS) Support custom resolutions for Apple Virtualization VMs\r\n* (macOS) Fixed a UI freeze when canceling out of the settings for an Apple Virtualization VM\r\n\r\n## Changes (v4.1.1)\r\n* Fixed launching SPARC machines (#4575)\r\n* Fixed an error when attempting to save a VM where one of its removable drives is linked to a file that has been deleted\r\n* Fixed IPSW/.utm download failing when the device goes to sleep (the download should resume after wake up)\r\n* Restored scroll bars when system is set to always show scroll bars. Added a new SwiftUI crash workaround thanks to @evelyneee.\r\n* Display all sizes in binary (MiB/GiB) mode in order to be consistent (#4396)\r\n* Localization: added Polish (thanks @mavethee)\r\n* Localization: updated Japanese (thanks @MMP0)\r\n* Localization: updated Spanish (Latin America) (thanks @JezerM)\r\n* Localization: updated French (thanks @FRtranslator)\r\n* (macOS) Fixed the port forward UI on macOS 11 and introduce a new port forward UI for macOS 12+ (#4690)\r\n* (macOS) Fixed \"This virtual machine cannot be run on this machine.\" error on a newly created Apple VM (#4595)\r\n* (macOS) Added new 21:9 widescreen resolution for Apple VMs (thanks @Tandolf)\r\n* (macOS) Added a clarifying message about shared directory support on older macOS guests (#4594)\r\n* (macOS) Added new shutdown options (software request and force kill) which can be toggled by long pressing the power button in the VM window (#4001)\r\n* (macOS) Added a confirmation dialog when deleting a drive (#4687)\r\n\r\n## Changes (v4.1.0)\r\n* Updated QEMU to v7.1.0\r\n* Updated ANGLE and virglrenderer to latest commit\r\n* Fixed an issue where user override of machine property settings was not applied properly\r\n* Localization: updated Japanese (thanks @MMP0)\r\n* Localization: updated Spanish (Latin America) (thanks @JezerM)\r\n* (iOS) Added in-app settings popover which synchronizes with the Settings app (useful for TrollStore installs where the Settings app page is inaccessible) (#4446)\r\n* (iOS) TrollStore: support JIT without needing a separate JIT enabler (thanks @PojavLauncherTeam for the idea)\r\n\r\n## Issues\r\nPlease check the full list on [Github][2] and help report any bug you find that is not listed.\r\n\r\n## Installation\r\n\r\n* [iOS](https://docs.getutm.app/installation/ios/)\r\n* [macOS](https://docs.getutm.app/installation/macos/)\r\n\r\n| File | Description | Installation | JIT | Hypervisor | USB |\r\n|------|------------|--------------|-----|-----------|-----|\r\n| UTM.deb | Jailbroken iOS version | Open in Cydia, dpkg, or Sileo | Yes | Yes(1) | Yes |\r\n| UTM.dmg | macOS version | Mounting and copying UTM.app to /Applications | Yes | Yes | Yes |\r\n| UTM.ipa | Non-jailbroken iOS version (sideloading) | AltStore, etc (see guide) | Yes(2) | No | No |\r\n| UTM.HV.ipa | Non-jailbroken iOS version (TrollStore) | TrollStore | Yes | Yes(1) | Yes |\r\n| UTM.SE.ipa | Non-jailbroken iOS version (sideloading) | AltStore, enterprise signing, etc | No | No | No |\r\n\r\n1. Hypervisor on iOS requires an M1 iPad.\r\n2. Enabling JIT may require a separate JIT enabler such as [Jitterbug][3] or Jitstreamer.\r\n\r\n[1]: https://getutm.app/install/\r\n[2]: https://github.com/utmapp/UTM/issues\r\n[3]: https://github.com/osy/Jitterbug",
+                    "size": 121694840,
+                    "version": "4.1.5"
+                },
+                {
                     "date": "2022-10-21T16:16:34Z",
                     "downloadURL": "https://github.com/utmapp/UTM/releases/download/v4.0.9/UTM.ipa",
                     "localizedDescription": "## Highlights\r\n* **Multiple display and headless display is now supported for QEMU machines.** You can configure 0 or more displays as well as 0 or more builtin terminal consoles. On macOS, a new window will be created for each display and builtin terminal. On iOS, you can create multiple windows (iPad) as well as plug in an external display or AirPlay (iPad or iPhone) and assign outputs to each window.\r\n* **Ventura updates to Virtualization.** macOS Ventura introduces new features that is now integrated into UTM. You can now create GUI Linux VMs with EFI boot. Directory sharing now works with macOS Ventura guests. Rosetta x86_64 emulation is supported for Linux VMs on Apple Silicon. Check out https://docs.getutm.app/guides/debian/ for an installation guide. Note that base M1 chip users may experience issues that will be addressed in a future update.\r\n* **VirtFS sharing for QEMU.** This alternative directory sharing backend is supported by Linux and can have better performance. Note that macOS UID are numbered differently than Linux so you may have to run `chown` in the guest. Check out https://docs.getutm.app/guest-support/linux/ for more details.\r\n* **Easier Windows 10/11 installation and Windows guest tools downloader.** You can now download and mount the Windows drivers and guest tools ISO image with a single click (macOS: disk icon in VM window, iOS: 3D touch context menu on home screen). Additionally, the ISO now include an \"Autounattend.xml\" which is recognized by the Windows 10/11 installer. When mounted to a second CD drive, the installer will install the correct drivers, bypass secure boot/TPM requirements, and launch the SPICE tools installer on first login.\r\n* (macOS) **Resize QEMU disk images.** In the drives settings page, you can now expand the size of the QCOW2 disk image.\r\n* (iOS) **QEMU Virtualization for M1 iPad.** With the release of [TrollStore](https://github.com/opa334/TrollStore), you can now enable Hypervisor on iOS. Note that only M1 hardware and kernel have support for Hypervisor. iOS 14.4.2-14.5.1 is supported only on M1 iPad Pro jailbroken with fugu14/unc0ver. iOS 14.0-15.5b4 is supported on any M1 iPad running TrollStore.\r\n* **New documentation site.** https://docs.getutm.app/ is the home of the official UTM documentation.\r\n* **New localization.** Thanks to various community members, UTM is now translated to: Chinese (Simplified), Chinese (Traditional), Finnish, French, German, Japanese, Korean, and Spanish (Latin America)\r\n\r\n## Notes\r\n* **iOS 14 and macOS 11.3** are the new minimum supported systems. Please use UTM v3.x for support down to iOS 11 and macOS 11\r\n* The configuration backend has been massively rewritten. **Please backup all VMs prior to updating as you will not be able to re-open VMs saved by UTM v4 on older versions of UTM if you decide to downgrade.**\r\n* Since v4.0.6, the order of generated devices has changed to always create network devices first. This is to address an issue on some distributions (such as Ubuntu) where adding a device (drive, display, etc) would require re-configurating the network because the device name changed. Unfortunately, this change will cause the configuration issue to occur once more on any existing VM that is susceptible to the network issue. On Ubuntu, this will require you to modify `/etc/netplan/00-installer-config.yaml` and change the adapter name from `enp0s9` (or whatever it is currently) to `enp0s1` (which reflects the new device ordering). Other Linux distributions may require a similar change. However, after updating the guest network configuration, you should no longer have issues with networking when making device changes to the VM.\r\n\r\n## Changes (v4.0.9)\r\n\r\n* Fixed some broken links to documentation (#4529)\r\n* Fixed an issue where running ARM64 emulation on ARM64 gives an error \"The \u2018host\u2019 CPU type can only be used with KVM or HVF\" (#4528)\r\n* Fixed a regression where S390x and SPARC VMs cannot start due to missing USB bus\r\n* (iOS) Fixed UTM SE cannot launch any VMs (#4516)\r\n\r\n## Changes (v4.0.8)\r\n\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator and @alexis-martel)\r\n* Translation: Added German (thanks @conath)\r\n* (macOS) Disable resize button in GUI Apple VM window\r\n* (macOS) Reverted some SwiftUI issue workarounds that are no longer present in Ventura RC\r\n\r\n## Changes (v4.0.7)\r\n\r\n* Fixed renamed VM not appearing on next launch (#4469)\r\n* Fixed TCP server not working (#4479)\r\n* Fixed random network issues caused by invalid MAC address generation (you must re-generate MAC to apply the change if your VM created in UTM v4 does not have working network) (#4477)\r\n* Fixed a crash when trying to boot Kali Linux with terminal enabled\r\n* Fixed hypervisor on iOS 14.6-14.8\r\n* Added new setting for serial device in TCP server mode to listen on remote/local interfaces (#4483)\r\n* Fixed URL automation sending text to terminal\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* Wizard: Link to new documentation site (#4443, #4445)\r\n* (iOS) Fixed disponible run option not appearing\r\n* (macOS) Fixed settings getting stuck at information page (#4465)\r\n* (macOS) Updated display menu option to match title bar when multiple displays are used (#4484)\r\n* (macOS) Fixed no mouse/keyboard on Intel Apple Virtualization (#4409)\r\n* (macOS) Fixed no audio input device on Linux running on Apple Virtualization (#4409)\r\n* (macOS) Fixed auto-quit when all windows are closed happening when headless VM is still running\r\n\r\n## Changes (v4.0.6)\r\n\r\n* Fixed an issue in argument generation where PS/2 input was forced even when USB was enabled (#4424)\r\n* Validate settings on save before closing the settings dialog\r\n* Network devices are now created first before all other devices. Note this means that networking will be broken on some existing VMs and must be re-configured! (See notes above)\r\n* Fixed a deadlock issue when saving settings\r\n* Fixed an error when saving a VM with an external drive selected\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* Wizard: The Windows guest tools auto-installer currently only works on Windows 10 and above. A new option is added in the wizard to make this explicit. (#4440)\r\n* Wizard: Use VirtFS sharing by default when Linux is selected\r\n* (iOS) Default to emulated network instead of failing when importing a VM created on macOS\r\n* (macOS) Fixed an issue where opening a new display window from a serial window did not work\r\n* (macOS) Fixed logic on macOS 11 where serial window was not created\r\n* (macOS) Fixed a crash on macOS 11 when saving settings while the QEMU tab is selected\r\n* (macOS 13) Support clipboard sharing on Linux with Apple Virtualization when `spice-vdagent` is installed\r\n* (macOS) Fixed an issue changing the boot OS where the incorrect image type is prompted\r\n* (macOS) Perform settings validation when launching an Apple Virtualization VM to ensure selected features are available\r\n* (macOS 12+) Set a machine identifier when launching an Apple Virtualization VM\r\n* (macOS 13) Emulate trackpad on macOS guests with Apple Virtualization\r\n* (macOS) Fixed an issue when a newly created VM will not launch on macOS 11\r\n\r\n## Changes (v4.0.5)\r\n\r\n* Fixed moving an existing VM with Hypervisor enabled to a device on a different architecture. The VM will fallback to TCG and the option to disable hypervisor in settings is allowed. (#4407)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* (iOS) Fixed an issue that prevented external keyboards from working (#4399)\r\n* (iOS) Detect Hypervisor support on jailbroken devices so the option is not inadvertently enabled on non-supported devices\r\n* (iOS) Support Hypervisor on M1 iPad running jailbroken iOS 14.5\r\n\r\n## Changes (v4.0.4)\r\n\r\n* Fixed in issue generating configuration for IDE drives leading to PPC not booting and I/O errors on PC (#4372, #4376, others)\r\n* Moved the SPICE tools download directory to \"GuestSupportTools\" under \"Application Support\" (previously it was just under \"Application Support\")\r\n* Fixed creating a VM with illegal path characters in the name (#4385)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* Wizard: No longer tries to download the Windows guest tools when selecting a non-Windows OS\r\n* (iOS) Enable build with Hypervisor.framework (support limited to M1 iPad)\r\n* (iOS) Fixed a crash when switching display in a window\r\n* (iOS) On jailbroken devices, the memory limit will automatically be increased to the maximum, preventing the Jetsam system from terminating UTM for memory usage\r\n* (iOS) Fixed a regression which caused the home indicator to not be hidden (#4390)\r\n* (iOS) Fixed a regression which caused the cursor to not be captured (#4390)\r\n* (iOS) When switching display, notification handlers are properly cleaned up (example: cursor capture and console on screen keyboard events)\r\n* (iOS) Show the device cursor when VM is paused\r\n* (iOS) Fixed a regression where external keyboard events are not captured\r\n* (iOS) Fixed an error where extraneous stale VM entries show up after the container name changes (#4392)\r\n* (iOS) Fixed a crash on iOS 14 when opening a terminal view due to SwiftTerm handling the colour configuration\r\n* (macOS) Fixed a layout issue of the compress/resize buttons\r\n* (macOS) Forgot to actually enable compression for the drive setting button (#4377)\r\n* (macOS) Fixed some settings layout issue on < macOS 13 (#4374)\r\n\r\n## Changes (v4.0.3)\r\n\r\n* Fixed an issue where changing external drive/shared directory for a QEMU VM -> exit UTM -> reopen UTM and start the VM results in the drive/share not being restored\r\n* Disable changing a VirtFS share from the home window (this is not an supported operation)\r\n* Better detection of UUID collision which addresses an issue where VMs with the same UUID do not show up on the home screen and other VMs show up as duplicates and clicking on any of them results in a freeze\r\n* Fixed floppy drive argument not being correctly generated (#4362)\r\n* Fixed an issue where ejecting an external drive or shared directory does not persist\r\n* Fixed a memory issue when stopping or closing VMs causing UTM to crash\r\n* Fixed a regression where an access error occurs after moving a VM\r\n* Added the ability to download the Windows SPICE tools and drivers automatically (#4364)\r\n* Added support for more than 2 IDE drives in PC emulation\r\n* Restored the setting to turn off blinking cursor (#4296)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Wizard: Reworked some of the UI, text, and file selection\r\n* Wizard: Add option to auto download and mount the SPICE tools to a second CD drive\r\n* Wizard: Fixed an issue where the selected boot image and shared directory was not saved on the new VM\r\n* Wizard: Recommend UUP built ISO over the VHDX by default\r\n* Wizard: New \"confused user\" check will catch trying to mount an \"amd64\" ISO on an \"arm64\" guest or vice versa\r\n* (iOS 16) Use the new NavigationSplitView for a slightly polished look\r\n* (iOS 16) Fixed an issue where the bottom toolbar does not show up (#4325)\r\n* (iOS) Fixed an issue where the file importer was not opening (#4365)\r\n* (iOS 14) Fixed an issue in the settings screen where multiple drives were occupying a single cell\r\n* (iOS 14) Fixed an issue where UTM may crash when adding a drive or hardware\r\n* (macOS) Added the ability to re-open closed windows for a given VM (#4351)\r\n* (macOS) Fixed an issue where restarting a VM results in duplicate windows (#4367)\r\n* (macOS) Save the size of terminal windows (#4296)\r\n* (macOS) Add resize QCOW2 image feature (thanks @stewartsmith)\r\n\r\n## Changes (v4.0.2)\r\n\r\n* Removed \"view.plist\" for host-specific configuration settings (i.e. bookmarks to removable drives and window options) and replaced it with a new \"registry\" that is stored outside of the .utm bundle. Old \"view.plist\" settings and bookmarks will be migrated to the registry on first launch and the file will be deleted from the .utm bundle. For Apple VMs, the bookmarks will no longer be stored in config.plist and the settings will be migrated to the registry as well.\r\n* VirtFS no longer requires SPICE to be enabled (thanks @tie)\r\n* Fixed an issue with PPC VMs not showing 256 colours correctly (#4277)\r\n* Fixed incorrect parsing of CPU flags (#4282)\r\n* Do not save screenshots when running in disposable mode\r\n* Translation: Added Spanish (Latin America) (thanks @JezerM)\r\n* Translation: Added Finnish (thanks @marcusziade)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated Chinese (Simplified) (thanks @ty-yqs)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* (iOS) Per-display window settings (zoom, position, keyboard visibility, etc) will be stored in the new registry\r\n* (iOS) Prefer JitStreamer over AltJit when both are available (thanks @ktprograms)\r\n* (macOS) Fixed saving removable drives and shared directories for Apple VMs\r\n* (macOS) Fixed missing audio entitlements (#4342)\r\n* (macOS) Fixed QEMULauncher process not terminating when a VM is force quit\r\n* (macOS) Fixed issue selecting text in SwiftTerm (#4297)\r\n\r\n## Changes (v4.0.1)\r\n* Fixed an issue where an UEFI BIOS error was reported when the target does not use UEFI (#4265)\r\n* Added Elementary OS icon (thanks @Unbinilium)\r\n* Updated ja localization (thanks @MMP0)\r\n* Updated fr localization (thanks @FRtranslator)\r\n* Changed the icon for \"Serial\" so it appears on iOS 14 and macOS 11 as well\r\n* Fixed custom icon not showing up for \"legacy\" configurations\r\n* Fixed an error trying to migrate \"legacy\" configuration when \"Images\" does not exist (#4266)\r\n* Fixed USB redirection (#4263)\r\n* (iOS) Fixed a toolbar issue where USB button overflowed on screen.\r\n* (iOS) Fixed resume button not appearing on < iOS 16\r\n* (iOS) Attempt to close the download progress pop-up after download completes (#4261)\r\n* (iOS) \"Open\" popover refuses to show up again after swiping down (#4260)\r\n* (iOS) Hide \"Add\" text on iOS 14 settings\r\n* (iOS) Fixed crash on iOS 14 settings when attempting to use the picker (#4270)\r\n* (iOS) Fixed an issue on iOS 14 where picker selection was being reset\r\n* (iOS) Fixed an issue where the USB icon is stuck on busy after a device disconnects\r\n* (macOS) Fixed a crash trying to change shared directory for Apple VM (#4271)\r\n* (macOS) Wizard created invalid target configuration for virtualized targets (#4274)\r\n\r\n## Changes (v4.0.0)\r\n* USB redirection support in terminal mode\r\n* Configuration file format changed, newly saved VMs will not be compatible with older versions of UTM\r\n* Newly imported disk images will be converted to QCOW2 automatically\r\n* Settings: new layout with support for multiple {Display, Serial, Network, Sound} devices (#3585)\r\n* Support multiple displays (#220)\r\n* Added Japanese localization (thanks @MMP0)\r\n* Support adding PTTY (macOS only), TCP client, and TCP server serial connections for QEMU machines (address should show up in the home screen) (#3546)\r\n* Support headless display (remove all displays and built-in serial ports in the settings) (#2280)\r\n* Support redirecting QEMU monitor and GDB stub to a serial port\r\n* Support zstd compression for QCOW2 images and use zstd as default for image compression (#4211)\r\n* Update ANGLE (GL backend) to latest git commit\r\n* Added French localization (thanks @FRtranslator)\r\n* Fixed microphone recording silence (#219)\r\n* Fixed a crash when attempting to delete a QEMU additional argument\r\n* Option in VM settings to use virtfs/9pfs for file sharing (#2184)\r\n* Option in VM settings to change VGA RAM size (#4034)\r\n* Option in VM settings to enable virtio-balloon driver (#4136)\r\n* Invert mouse scrolling is now a global setting rather than a per-vm configuration option\r\n* (iOS) Replaced hterm.js with SwiftTerm for terminal mode (#3473)\r\n* (iOS) Attach to JitStreamer (set IP address in Settings app and UTM will try to connect automatically on launch) (thanks @ktprograms)\r\n* (iOS) Automatically resize the display to fit the screen when the resolution changes if the resize toolbar option is used\r\n* (iOS) Reimplemented the USB and Drives menu with a better UI\r\n* (iOS) On iPadOS 16, show the menu bar when holding Cmd on the keyboard. On previous versions, an on-screen help will show supported commands\r\n* (iOS) Improved audio handling including: output when on silence, mixing with other apps, working when both recording and outputting (including with another app) (#3996)\r\n* (iOS) Added a global setting to always prefer the built-in microphone to a bluetooth microphone\r\n* (macOS) Fixed running from shortcut in Apple VMs (no longer need to re-import after each launch)\r\n* (macOS) Improved IPSW selection interface and support drag and drop (thanks @pointum)\r\n* (macOS) Fixed running unsigned builds\r\n* (macOS) Removed some deprecated global settings\r\n* (macOS) Fixed an error when trying to download an IPSW and the Caches directory does not exist (thanks @LostInCompilation)\r\n* (macOS) Fixed an issue where a VM could be started twice if the home screen's toolbar is used leading to data corruption (#4166)\r\n* (macOS 13+) Boot into recoveryOS (to disable SIP, etc) by right clicking on the VM and selecting \"Run in recovery...\" (#3526)\r\n* (macOS 13+) Option in VM settings to enable Rosetta for x86_64 emulation (#4100)\r\n* (macOS 13+) Option in VM settings to enable clipboard sharing (SPICE support needed on the guest) (#4121)\r\n* (macOS 13+) GUI display for Linux VMs (#4120)\r\n* (macOS 13+) Add removable drives, will show up as USB mass storage\r\n\r\n## Issues\r\nPlease check the full list on [Github][2] and help report any bug you find that is not listed.\r\n\r\n## Installation\r\n\r\n* [iOS](https://docs.getutm.app/installation/ios/)\r\n* [macOS](https://docs.getutm.app/installation/macos/)\r\n\r\n| File | Description | Installation | JIT | Hypervisor | USB |\r\n|------|------------|--------------|-----|-----------|-----|\r\n| UTM.deb | Jailbroken iOS version | Open in Cydia, dpkg, or Sileo | Yes | Yes(1) | Yes |\r\n| UTM.dmg | macOS version | Mounting and copying UTM.app to /Applications | Yes | Yes | Yes |\r\n| UTM.ipa | Non-jailbroken iOS version (sideloading) | AltStore, etc (see guide) | Yes(2) | No | No |\r\n| UTM.HV.ipa | Non-jailbroken iOS version (TrollStore) | TrollStore | Yes(2) | Yes(1) | Yes |\r\n| UTM.SE.ipa | Non-jailbroken iOS version (sideloading) | AltStore, enterprise signing, etc | No | No | No |\r\n\r\n1. Hypervisor on iOS requires an M1 iPad.\r\n2. Enabling JIT may require a separate JIT enabler such as [Jitterbug][3] or Jitstreamer.\r\n\r\n[1]: https://getutm.app/install/\r\n[2]: https://github.com/utmapp/UTM/issues\r\n[3]: https://github.com/osy/Jitterbug",
                     "size": 138928961,
                     "version": "4.0.9"
                 },
                 {
@@ -806,99 +871,112 @@
                     "version": "3.2.4"
                 }
             ]
         },
         {
             "bundleIdentifier": "com.litchie.idosgames",
             "developerName": "litchie",
-            "downloadURL": "https://github.com/litchie/dospad/releases/download/2.1/iDOS.ipa",
             "iconURL": "https://i.imgur.com/Yah6zFk.png",
             "localizedDescription": "Play classic DOS games on your iPhone and iPad!\n\niDOS turns your device right into a powerful DOS gaming PC, with modern game control to make your old favorites as playable as possible.\n\nYou can also use iDOS for non-gaming purposes, such as word processing, casual programming. Apps in the DOS days are often simpler and surprisingly productive.\n\nKEYBOARD\n\niDOS provides a PC compatible on-screen keyboard with carefully designed layouts for different devices and orientations. The keyboard has a sliding control in landscape mode so that you can keep it from covering critical part of the screen.\n\nBluetooth keyboard is partially supported. We support ESC, function keys, and ordinary CTRL and ALT key bindings. Unfortunately the arrow keys can't be used for game control. You should use a bluetooth game controller instead.\n\nGAMEPAD\n\niDOS provides a virtual gamepad with key bindings that are fairly common in DOS games. You can customize the bindings. The DPAD works in 8-axis way. It can also be toggled into a joystick.\n\nExternal bluetooth game controllers are supported. Make sure your game controller is connected (System Settings->Bluetooth). To customize button bindings, go to iDOS in landscape mode, tap on bluetooth icon on the auto-hiding top bar.\n\nMOUSE\n\n* The screen area serves as a trackpad for moving mouse pointer.\n* Tap on the screen for left click. If direct touch is enabled, the mouse pointer will move to where you tap.\n* Hold one finger on the screen, and tap with another finger for right click.\n* On-screen mouse buttons are also provided for your convenience.\n* Bluetooth mice are only partially supported.\n\nSUPPORT\n\n- Visit https://litchie.com/dospad for more information.\n- Send email to idos@litchie.com\n- Follow the developer on Twitter: https://twitter.com/litchiedev\n- iDOS is open source, report issues on https://github.com/litchie/dospad",
             "name": "iDOS",
             "screenshotURLs": [
                 "https://i.imgur.com/hRMA2Zr.png",
                 "https://i.imgur.com/gvhvQpo.png",
                 "https://i.imgur.com/NHOE1ba.png",
                 "https://i.imgur.com/eBEqmnt.png"
             ],
-            "size": 5704322,
             "subtitle": "Play DOS games on iOS.",
             "tintColor": "#042eef",
-            "version": "2.1",
-            "versionDate": "2020-10-20",
-            "versionDescription": "- Support Mfi game controllers\n- Support external bluetooth keyboard (Text input only).\nYou can use Command-1, Command-2 .. for function keys.",
             "versions": [
                 {
                     "date": "2020-10-20",
                     "downloadURL": "https://github.com/litchie/dospad/releases/download/2.1/iDOS.ipa",
                     "localizedDescription": "- Support Mfi game controllers\n- Support external bluetooth keyboard (Text input only).\nYou can use Command-1, Command-2 .. for function keys.",
+                    "sha256": "1660903b0d3ec6cc4686bc99c028d3f46267018ecdac5ccf9c02778a96cb1a4d",
                     "size": 5704322,
                     "version": "2.1"
                 }
             ]
         },
         {
-            "absoluteVersion": "1.1.6",
             "bundleIdentifier": "org.coolstar.taurine",
             "developerName": "Odyssey Team",
-            "downloadURL": "https://github.com/Odyssey-Team/Taurine/releases/download/1.1.6/Taurine-1.1.6.ipa",
             "iconURL": "https://taurine.app/assets/images/icon.png",
             "localizedDescription": "Taurine is an iOS 14.0-14.3 jailbreak, utilizing Procursus and Libhooker.",
             "name": "Taurine",
             "screenshotURLs": [
                 "https://taurine.app/assets/images/ss-1.png",
                 "https://taurine.app/assets/images/ss-2.png",
                 "https://taurine.app/assets/images/ss-3.png"
             ],
-            "size": 31938370,
             "subtitle": "Time to get amped.",
             "tintColor": "#F65656",
-            "version": "1.1.6",
-            "versionDate": "2022-07-17T12:33:15Z",
-            "versionDescription": "# 1.1.6\n\n- Backports DER entitlement fixes from Taurine15\r\n- Backports codesignature fixes from Taurine15\r\n- Backports various other fixes from Taurine15\r\n",
             "versions": [
                 {
                     "absoluteVersion": "1.1.6",
                     "date": "2022-07-17T12:33:15Z",
                     "downloadURL": "https://github.com/Odyssey-Team/Taurine/releases/download/1.1.6/Taurine-1.1.6.ipa",
                     "localizedDescription": "# 1.1.6\n\n- Backports DER entitlement fixes from Taurine15\r\n- Backports codesignature fixes from Taurine15\r\n- Backports various other fixes from Taurine15\r\n",
+                    "sha256": "0e628c33eabeef030ac08478f79ac74d9be8582301df0ae7bec26d8d1af8dad6",
                     "size": 31938370,
                     "version": "1.1.6"
                 }
             ]
         },
         {
             "appID": "com.utmapp.UTM-SE",
             "bundleIdentifier": "com.utmapp.UTM-SE",
             "developerName": "osy",
-            "downloadURL": "https://github.com/utmapp/UTM/releases/download/v4.0.9/UTM.SE.ipa",
-            "filename": "UTM.SE.ipa",
-            "githubOwner": "utmapp",
-            "githubRepository": "UTM",
             "iconURL": "https://alt.getutm.app/icon.png",
             "localizedDescription": "UTM is a full featured virtual machine host for iOS. In short, it allows you to run Windows, Android, and more on your iPhone and iPad.\nThis version runs on all > iOS 11 devices but lacks JIT support and is slower than regular UTM.\n\n\nMore information at https://getutm.app/\n\nFeatures:\n\n\u2022 Emulate any Processor\n30+ processors supported by qemu including x86_64, ARM64, and RISC-V\n\u2022 Run any Operating System\nWindows, Linux, and more natively and securely on iOS within an App\n\u2022 Fast Emulation\nPara-virtualization with SPICE and JIT compilation with TCG\n\u2022 High Compatibility\niOS 11+ supported. Works on iPhone and iPad. No jailbreak needed\n\u2022 Free and Open Source\nUTM and its dependencies are all free and open source\n\u2022 Easy to Use\nConfigure and customize your VM in a native UI\n\n\nNote: Screenshots are from the updated interface only available on iOS 14.",
             "name": "UTM SE",
             "screenshotURLs": [
                 "https://alt.getutm.app/screen0.png",
                 "https://alt.getutm.app/screen1.png",
                 "https://alt.getutm.app/screen2.png",
                 "https://alt.getutm.app/screen3.png",
                 "https://alt.getutm.app/screen4.png",
                 "https://alt.getutm.app/screen5.png",
                 "https://alt.getutm.app/screen6.png"
             ],
-            "size": 153976253,
-            "skipPrerelease": true,
             "subtitle": "Virtual machines for iOS (without JIT support)",
             "tintColor": "1a2cc2",
-            "version": "4.0.9",
-            "versionDate": "2022-10-21T16:16:34Z",
-            "versionDescription": "## Highlights\r\n* **Multiple display and headless display is now supported for QEMU machines.** You can configure 0 or more displays as well as 0 or more builtin terminal consoles. On macOS, a new window will be created for each display and builtin terminal. On iOS, you can create multiple windows (iPad) as well as plug in an external display or AirPlay (iPad or iPhone) and assign outputs to each window.\r\n* **Ventura updates to Virtualization.** macOS Ventura introduces new features that is now integrated into UTM. You can now create GUI Linux VMs with EFI boot. Directory sharing now works with macOS Ventura guests. Rosetta x86_64 emulation is supported for Linux VMs on Apple Silicon. Check out https://docs.getutm.app/guides/debian/ for an installation guide. Note that base M1 chip users may experience issues that will be addressed in a future update.\r\n* **VirtFS sharing for QEMU.** This alternative directory sharing backend is supported by Linux and can have better performance. Note that macOS UID are numbered differently than Linux so you may have to run `chown` in the guest. Check out https://docs.getutm.app/guest-support/linux/ for more details.\r\n* **Easier Windows 10/11 installation and Windows guest tools downloader.** You can now download and mount the Windows drivers and guest tools ISO image with a single click (macOS: disk icon in VM window, iOS: 3D touch context menu on home screen). Additionally, the ISO now include an \"Autounattend.xml\" which is recognized by the Windows 10/11 installer. When mounted to a second CD drive, the installer will install the correct drivers, bypass secure boot/TPM requirements, and launch the SPICE tools installer on first login.\r\n* (macOS) **Resize QEMU disk images.** In the drives settings page, you can now expand the size of the QCOW2 disk image.\r\n* (iOS) **QEMU Virtualization for M1 iPad.** With the release of [TrollStore](https://github.com/opa334/TrollStore), you can now enable Hypervisor on iOS. Note that only M1 hardware and kernel have support for Hypervisor. iOS 14.4.2-14.5.1 is supported only on M1 iPad Pro jailbroken with fugu14/unc0ver. iOS 14.0-15.5b4 is supported on any M1 iPad running TrollStore.\r\n* **New documentation site.** https://docs.getutm.app/ is the home of the official UTM documentation.\r\n* **New localization.** Thanks to various community members, UTM is now translated to: Chinese (Simplified), Chinese (Traditional), Finnish, French, German, Japanese, Korean, and Spanish (Latin America)\r\n\r\n## Notes\r\n* **iOS 14 and macOS 11.3** are the new minimum supported systems. Please use UTM v3.x for support down to iOS 11 and macOS 11\r\n* The configuration backend has been massively rewritten. **Please backup all VMs prior to updating as you will not be able to re-open VMs saved by UTM v4 on older versions of UTM if you decide to downgrade.**\r\n* Since v4.0.6, the order of generated devices has changed to always create network devices first. This is to address an issue on some distributions (such as Ubuntu) where adding a device (drive, display, etc) would require re-configurating the network because the device name changed. Unfortunately, this change will cause the configuration issue to occur once more on any existing VM that is susceptible to the network issue. On Ubuntu, this will require you to modify `/etc/netplan/00-installer-config.yaml` and change the adapter name from `enp0s9` (or whatever it is currently) to `enp0s1` (which reflects the new device ordering). Other Linux distributions may require a similar change. However, after updating the guest network configuration, you should no longer have issues with networking when making device changes to the VM.\r\n\r\n## Changes (v4.0.9)\r\n\r\n* Fixed some broken links to documentation (#4529)\r\n* Fixed an issue where running ARM64 emulation on ARM64 gives an error \"The \u2018host\u2019 CPU type can only be used with KVM or HVF\" (#4528)\r\n* Fixed a regression where S390x and SPARC VMs cannot start due to missing USB bus\r\n* (iOS) Fixed UTM SE cannot launch any VMs (#4516)\r\n\r\n## Changes (v4.0.8)\r\n\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator and @alexis-martel)\r\n* Translation: Added German (thanks @conath)\r\n* (macOS) Disable resize button in GUI Apple VM window\r\n* (macOS) Reverted some SwiftUI issue workarounds that are no longer present in Ventura RC\r\n\r\n## Changes (v4.0.7)\r\n\r\n* Fixed renamed VM not appearing on next launch (#4469)\r\n* Fixed TCP server not working (#4479)\r\n* Fixed random network issues caused by invalid MAC address generation (you must re-generate MAC to apply the change if your VM created in UTM v4 does not have working network) (#4477)\r\n* Fixed a crash when trying to boot Kali Linux with terminal enabled\r\n* Fixed hypervisor on iOS 14.6-14.8\r\n* Added new setting for serial device in TCP server mode to listen on remote/local interfaces (#4483)\r\n* Fixed URL automation sending text to terminal\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* Wizard: Link to new documentation site (#4443, #4445)\r\n* (iOS) Fixed disponible run option not appearing\r\n* (macOS) Fixed settings getting stuck at information page (#4465)\r\n* (macOS) Updated display menu option to match title bar when multiple displays are used (#4484)\r\n* (macOS) Fixed no mouse/keyboard on Intel Apple Virtualization (#4409)\r\n* (macOS) Fixed no audio input device on Linux running on Apple Virtualization (#4409)\r\n* (macOS) Fixed auto-quit when all windows are closed happening when headless VM is still running\r\n\r\n## Changes (v4.0.6)\r\n\r\n* Fixed an issue in argument generation where PS/2 input was forced even when USB was enabled (#4424)\r\n* Validate settings on save before closing the settings dialog\r\n* Network devices are now created first before all other devices. Note this means that networking will be broken on some existing VMs and must be re-configured! (See notes above)\r\n* Fixed a deadlock issue when saving settings\r\n* Fixed an error when saving a VM with an external drive selected\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* Wizard: The Windows guest tools auto-installer currently only works on Windows 10 and above. A new option is added in the wizard to make this explicit. (#4440)\r\n* Wizard: Use VirtFS sharing by default when Linux is selected\r\n* (iOS) Default to emulated network instead of failing when importing a VM created on macOS\r\n* (macOS) Fixed an issue where opening a new display window from a serial window did not work\r\n* (macOS) Fixed logic on macOS 11 where serial window was not created\r\n* (macOS) Fixed a crash on macOS 11 when saving settings while the QEMU tab is selected\r\n* (macOS 13) Support clipboard sharing on Linux with Apple Virtualization when `spice-vdagent` is installed\r\n* (macOS) Fixed an issue changing the boot OS where the incorrect image type is prompted\r\n* (macOS) Perform settings validation when launching an Apple Virtualization VM to ensure selected features are available\r\n* (macOS 12+) Set a machine identifier when launching an Apple Virtualization VM\r\n* (macOS 13) Emulate trackpad on macOS guests with Apple Virtualization\r\n* (macOS) Fixed an issue when a newly created VM will not launch on macOS 11\r\n\r\n## Changes (v4.0.5)\r\n\r\n* Fixed moving an existing VM with Hypervisor enabled to a device on a different architecture. The VM will fallback to TCG and the option to disable hypervisor in settings is allowed. (#4407)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* (iOS) Fixed an issue that prevented external keyboards from working (#4399)\r\n* (iOS) Detect Hypervisor support on jailbroken devices so the option is not inadvertently enabled on non-supported devices\r\n* (iOS) Support Hypervisor on M1 iPad running jailbroken iOS 14.5\r\n\r\n## Changes (v4.0.4)\r\n\r\n* Fixed in issue generating configuration for IDE drives leading to PPC not booting and I/O errors on PC (#4372, #4376, others)\r\n* Moved the SPICE tools download directory to \"GuestSupportTools\" under \"Application Support\" (previously it was just under \"Application Support\")\r\n* Fixed creating a VM with illegal path characters in the name (#4385)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* Wizard: No longer tries to download the Windows guest tools when selecting a non-Windows OS\r\n* (iOS) Enable build with Hypervisor.framework (support limited to M1 iPad)\r\n* (iOS) Fixed a crash when switching display in a window\r\n* (iOS) On jailbroken devices, the memory limit will automatically be increased to the maximum, preventing the Jetsam system from terminating UTM for memory usage\r\n* (iOS) Fixed a regression which caused the home indicator to not be hidden (#4390)\r\n* (iOS) Fixed a regression which caused the cursor to not be captured (#4390)\r\n* (iOS) When switching display, notification handlers are properly cleaned up (example: cursor capture and console on screen keyboard events)\r\n* (iOS) Show the device cursor when VM is paused\r\n* (iOS) Fixed a regression where external keyboard events are not captured\r\n* (iOS) Fixed an error where extraneous stale VM entries show up after the container name changes (#4392)\r\n* (iOS) Fixed a crash on iOS 14 when opening a terminal view due to SwiftTerm handling the colour configuration\r\n* (macOS) Fixed a layout issue of the compress/resize buttons\r\n* (macOS) Forgot to actually enable compression for the drive setting button (#4377)\r\n* (macOS) Fixed some settings layout issue on < macOS 13 (#4374)\r\n\r\n## Changes (v4.0.3)\r\n\r\n* Fixed an issue where changing external drive/shared directory for a QEMU VM -> exit UTM -> reopen UTM and start the VM results in the drive/share not being restored\r\n* Disable changing a VirtFS share from the home window (this is not an supported operation)\r\n* Better detection of UUID collision which addresses an issue where VMs with the same UUID do not show up on the home screen and other VMs show up as duplicates and clicking on any of them results in a freeze\r\n* Fixed floppy drive argument not being correctly generated (#4362)\r\n* Fixed an issue where ejecting an external drive or shared directory does not persist\r\n* Fixed a memory issue when stopping or closing VMs causing UTM to crash\r\n* Fixed a regression where an access error occurs after moving a VM\r\n* Added the ability to download the Windows SPICE tools and drivers automatically (#4364)\r\n* Added support for more than 2 IDE drives in PC emulation\r\n* Restored the setting to turn off blinking cursor (#4296)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Wizard: Reworked some of the UI, text, and file selection\r\n* Wizard: Add option to auto download and mount the SPICE tools to a second CD drive\r\n* Wizard: Fixed an issue where the selected boot image and shared directory was not saved on the new VM\r\n* Wizard: Recommend UUP built ISO over the VHDX by default\r\n* Wizard: New \"confused user\" check will catch trying to mount an \"amd64\" ISO on an \"arm64\" guest or vice versa\r\n* (iOS 16) Use the new NavigationSplitView for a slightly polished look\r\n* (iOS 16) Fixed an issue where the bottom toolbar does not show up (#4325)\r\n* (iOS) Fixed an issue where the file importer was not opening (#4365)\r\n* (iOS 14) Fixed an issue in the settings screen where multiple drives were occupying a single cell\r\n* (iOS 14) Fixed an issue where UTM may crash when adding a drive or hardware\r\n* (macOS) Added the ability to re-open closed windows for a given VM (#4351)\r\n* (macOS) Fixed an issue where restarting a VM results in duplicate windows (#4367)\r\n* (macOS) Save the size of terminal windows (#4296)\r\n* (macOS) Add resize QCOW2 image feature (thanks @stewartsmith)\r\n\r\n## Changes (v4.0.2)\r\n\r\n* Removed \"view.plist\" for host-specific configuration settings (i.e. bookmarks to removable drives and window options) and replaced it with a new \"registry\" that is stored outside of the .utm bundle. Old \"view.plist\" settings and bookmarks will be migrated to the registry on first launch and the file will be deleted from the .utm bundle. For Apple VMs, the bookmarks will no longer be stored in config.plist and the settings will be migrated to the registry as well.\r\n* VirtFS no longer requires SPICE to be enabled (thanks @tie)\r\n* Fixed an issue with PPC VMs not showing 256 colours correctly (#4277)\r\n* Fixed incorrect parsing of CPU flags (#4282)\r\n* Do not save screenshots when running in disposable mode\r\n* Translation: Added Spanish (Latin America) (thanks @JezerM)\r\n* Translation: Added Finnish (thanks @marcusziade)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated Chinese (Simplified) (thanks @ty-yqs)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* (iOS) Per-display window settings (zoom, position, keyboard visibility, etc) will be stored in the new registry\r\n* (iOS) Prefer JitStreamer over AltJit when both are available (thanks @ktprograms)\r\n* (macOS) Fixed saving removable drives and shared directories for Apple VMs\r\n* (macOS) Fixed missing audio entitlements (#4342)\r\n* (macOS) Fixed QEMULauncher process not terminating when a VM is force quit\r\n* (macOS) Fixed issue selecting text in SwiftTerm (#4297)\r\n\r\n## Changes (v4.0.1)\r\n* Fixed an issue where an UEFI BIOS error was reported when the target does not use UEFI (#4265)\r\n* Added Elementary OS icon (thanks @Unbinilium)\r\n* Updated ja localization (thanks @MMP0)\r\n* Updated fr localization (thanks @FRtranslator)\r\n* Changed the icon for \"Serial\" so it appears on iOS 14 and macOS 11 as well\r\n* Fixed custom icon not showing up for \"legacy\" configurations\r\n* Fixed an error trying to migrate \"legacy\" configuration when \"Images\" does not exist (#4266)\r\n* Fixed USB redirection (#4263)\r\n* (iOS) Fixed a toolbar issue where USB button overflowed on screen.\r\n* (iOS) Fixed resume button not appearing on < iOS 16\r\n* (iOS) Attempt to close the download progress pop-up after download completes (#4261)\r\n* (iOS) \"Open\" popover refuses to show up again after swiping down (#4260)\r\n* (iOS) Hide \"Add\" text on iOS 14 settings\r\n* (iOS) Fixed crash on iOS 14 settings when attempting to use the picker (#4270)\r\n* (iOS) Fixed an issue on iOS 14 where picker selection was being reset\r\n* (iOS) Fixed an issue where the USB icon is stuck on busy after a device disconnects\r\n* (macOS) Fixed a crash trying to change shared directory for Apple VM (#4271)\r\n* (macOS) Wizard created invalid target configuration for virtualized targets (#4274)\r\n\r\n## Changes (v4.0.0)\r\n* USB redirection support in terminal mode\r\n* Configuration file format changed, newly saved VMs will not be compatible with older versions of UTM\r\n* Newly imported disk images will be converted to QCOW2 automatically\r\n* Settings: new layout with support for multiple {Display, Serial, Network, Sound} devices (#3585)\r\n* Support multiple displays (#220)\r\n* Added Japanese localization (thanks @MMP0)\r\n* Support adding PTTY (macOS only), TCP client, and TCP server serial connections for QEMU machines (address should show up in the home screen) (#3546)\r\n* Support headless display (remove all displays and built-in serial ports in the settings) (#2280)\r\n* Support redirecting QEMU monitor and GDB stub to a serial port\r\n* Support zstd compression for QCOW2 images and use zstd as default for image compression (#4211)\r\n* Update ANGLE (GL backend) to latest git commit\r\n* Added French localization (thanks @FRtranslator)\r\n* Fixed microphone recording silence (#219)\r\n* Fixed a crash when attempting to delete a QEMU additional argument\r\n* Option in VM settings to use virtfs/9pfs for file sharing (#2184)\r\n* Option in VM settings to change VGA RAM size (#4034)\r\n* Option in VM settings to enable virtio-balloon driver (#4136)\r\n* Invert mouse scrolling is now a global setting rather than a per-vm configuration option\r\n* (iOS) Replaced hterm.js with SwiftTerm for terminal mode (#3473)\r\n* (iOS) Attach to JitStreamer (set IP address in Settings app and UTM will try to connect automatically on launch) (thanks @ktprograms)\r\n* (iOS) Automatically resize the display to fit the screen when the resolution changes if the resize toolbar option is used\r\n* (iOS) Reimplemented the USB and Drives menu with a better UI\r\n* (iOS) On iPadOS 16, show the menu bar when holding Cmd on the keyboard. On previous versions, an on-screen help will show supported commands\r\n* (iOS) Improved audio handling including: output when on silence, mixing with other apps, working when both recording and outputting (including with another app) (#3996)\r\n* (iOS) Added a global setting to always prefer the built-in microphone to a bluetooth microphone\r\n* (macOS) Fixed running from shortcut in Apple VMs (no longer need to re-import after each launch)\r\n* (macOS) Improved IPSW selection interface and support drag and drop (thanks @pointum)\r\n* (macOS) Fixed running unsigned builds\r\n* (macOS) Removed some deprecated global settings\r\n* (macOS) Fixed an error when trying to download an IPSW and the Caches directory does not exist (thanks @LostInCompilation)\r\n* (macOS) Fixed an issue where a VM could be started twice if the home screen's toolbar is used leading to data corruption (#4166)\r\n* (macOS 13+) Boot into recoveryOS (to disable SIP, etc) by right clicking on the VM and selecting \"Run in recovery...\" (#3526)\r\n* (macOS 13+) Option in VM settings to enable Rosetta for x86_64 emulation (#4100)\r\n* (macOS 13+) Option in VM settings to enable clipboard sharing (SPICE support needed on the guest) (#4121)\r\n* (macOS 13+) GUI display for Linux VMs (#4120)\r\n* (macOS 13+) Add removable drives, will show up as USB mass storage\r\n\r\n## Issues\r\nPlease check the full list on [Github][2] and help report any bug you find that is not listed.\r\n\r\n## Installation\r\n\r\n* [iOS](https://docs.getutm.app/installation/ios/)\r\n* [macOS](https://docs.getutm.app/installation/macos/)\r\n\r\n| File | Description | Installation | JIT | Hypervisor | USB |\r\n|------|------------|--------------|-----|-----------|-----|\r\n| UTM.deb | Jailbroken iOS version | Open in Cydia, dpkg, or Sileo | Yes | Yes(1) | Yes |\r\n| UTM.dmg | macOS version | Mounting and copying UTM.app to /Applications | Yes | Yes | Yes |\r\n| UTM.ipa | Non-jailbroken iOS version (sideloading) | AltStore, etc (see guide) | Yes(2) | No | No |\r\n| UTM.HV.ipa | Non-jailbroken iOS version (TrollStore) | TrollStore | Yes(2) | Yes(1) | Yes |\r\n| UTM.SE.ipa | Non-jailbroken iOS version (sideloading) | AltStore, enterprise signing, etc | No | No | No |\r\n\r\n1. Hypervisor on iOS requires an M1 iPad.\r\n2. Enabling JIT may require a separate JIT enabler such as [Jitterbug][3] or Jitstreamer.\r\n\r\n[1]: https://getutm.app/install/\r\n[2]: https://github.com/utmapp/UTM/issues\r\n[3]: https://github.com/osy/Jitterbug",
             "versions": [
                 {
+                    "date": "2023-04-25T05:29:12Z",
+                    "downloadURL": "https://github.com/utmapp/UTM/releases/download/v4.2.5/UTM.SE.ipa",
+                    "localizedDescription": "## Highlights\r\n* (iOS SE) **TCTI backend updates**. Vector instruction support can improve the performance of certain workloads.\r\n* (macOS) **Guest interface commands**. New commands accessible from the scripting interface as well as the command line interface (utmctl) can be used to read/write files, execute commands, and list IP addresses. These commands require QEMU guest agent to be installed.\r\n* (macOS) **Scripting interface additions**. The scripting interface now allows for creation of a new VM, configuration an existing VM, changing drive image, and more. See [this page](https://docs.getutm.app/scripting/reference/) for more details and [the cheat sheet](https://docs.getutm.app/scripting/cheat-sheet/) for example usage.\r\n* (macOS) **External read-write drive images**. In QEMU, if a supported drive interface is selected (USB, Floppy, etc) along with an image type of Disk, the drive can now be marked as either read-only or read-write. This can be used as an alternative way of transferring data to and from the VM when the guest does not support SPICE or VirtFS. In AVF, support for read-write images has be fixed as well (when \"read only\" is unchecked in the settings).\r\n\r\n## Changes (v4.2.5)\r\n* Reverted ANGLE to an older version which includes the fix detailed in v4.2.4 but also does not break the Metal backend (#5238)\r\n* Translation: updated Polish (thanks @matgaj, @mavethee)\r\n* (macOS) Fixed an issue where the pointer device stopped working on macOS Monterey guests (#5237)\r\n* (macOS) AVM: Added option to use emulated trackpad (requires macOS Ventura guest)\r\n\r\n## Changes (v4.2.4)\r\n* UTM will now display the release notes the first time a new version is launched\r\n* Updated ANGLE which should fix some GPU acceleration issues on Linux (please see known issues below for unresolved issues)\r\n* Fixed an issue where a removable drive or VirtIO shared directory was set up when QEMUHelper was already running and therefore was not able to create a bookmark and an \"access denied\" error shows up on startup\r\n* Introduced a new preference setting for using the Option key as Meta in the built in console. This was on by default in previous versions and is not off by default which should allow international text to be entered properly (#5202)\r\n* Wizard: Make virtio-gpu-pci default for Linux (again) which was reverted a few releases ago in order to address some GPU issues\r\n* Translation: updated Polish (thanks @matgaj)\r\n* (iOS) Fixed built in terminal overlapping in the safe area\r\n\r\n## Changes (v4.2.3)\r\n* Added support for read-write removable devices on supported interfaces (USB, Floppy, etc). To use this feature, set the image type to \"Disk\" and uncheck the \"Read Only?\" option in the drive settings. Note that you may have to eject and re-mount the drive image for effect to take place. (#5079)\r\n* Removable USB devices will no longer show up as a CD drive if the image type is set to \"Disk\" (#5171)\r\n* Reverted a change from v4.2.0 where virtio bus devices were removed (this broke some people's configurations) (#5137)\r\n* Fixed an issue where when QEMU fails to start, subsequent attempts to start the VM will automatically fail\r\n* Fixed an issue where due to a race, removable drives may not be mounted on start\r\n* (iOS) Fixed an issue when the pointer is hovering over a toolbar button when the VM starts and subsequent clicks will toggle the button (#4843)\r\n* (macOS) AVF: Fixed an issue where a removable drive that is not marked as read-only still gets marked as read-only after restarting UTM (when upgrading from a previous version, you must eject and re-mount the image for effect to take place) (#5170)\r\n* (macOS) Fixed an issue where incorrect subnet parameters are generated for vmnet advanced settings (#5128)\r\n* (macOS) CLI: Added a new `clone` command (#5004)\r\n\r\n## Changes (v4.2.2)\r\n* Fixed an issue where a VM that is moved manually (e.g. with Finder) cannot be started (#5121)\r\n* Fixed an issue where the cursor disappears after resuming a suspended VM (#4665)\r\n* (macOS) Scripting: Add support for `make`, `duplicate`, and `delete` verbs on virtual machines\r\n* (macOS) Scripting: Add support for modifying certain configuration options\r\n* (macOS) Scripting: Removed virtual machine properties: `notes`, `machine`, `architecture`, `memory`. You should now use similar properties in the `configuration` record\r\n* (macOS) Support changing the audio backend to CoreAudio and make CoreAudio the default (due to better latency and as a workaround to some crashes) (#5125)\r\n\r\n## Changes (v4.2.1)\r\n* QEMU: Support more than 8 cores for ARM64 targets (#4847)\r\n* Synchronize time on resume when QEMU guest agent is installed which should fix clock drift issues (#3218)\r\n* (iOS SE) Updated TCTI to latest branch from @ktemkin which has support for vector instructions (#4865)\r\n* (macOS) Switch to emulated trackpad when guest+host are macOS 13+ (second attempt for #4636 and #4645)\r\n* (macOS) Fixed the \"raw image\" checkbox when creating a new drive (#5100)\r\n* (macOS) Add PC speaker sound device as an option. You can now add a second sound device on supported targets (x86_64/i386 PC based targets) and set the hardware to PC Speaker to emulate older motherboard speakers.\r\n* (macOS) Scripting: new verbs \"open file\", \"execute\", and \"query ip\" which uses the QEMU guest agent to send commands to the guest. Use the Apple Script Editor's Open Dictionary tool for more information.\r\n* (macOS) CLI: new commands \"file push\", \"file pull\", \"exec\", and \"ip-address\". See `utmctl help` for more information.\r\n\r\n## Changes (v4.2.0)\r\n* Updated virglrenderer to latest (27/02/2023) commit\r\n* Automatically revert CPU to \"default\" if model is missing due to updated QEMU (#4910)\r\n* ~~Remove virtio-bus devices (they didn't work) (#4893)~~\r\n* Support drag and drop to import an .utm package (#3599)\r\n* Support copying sparse images across different volumes (thanks @ktprograms)\r\n* Fixed tearing/performance issue for non-GL accelerated displays when under graphics load (#5049)\r\n* Fixed error when importing a new drive with the same name as an existing drive (#5052)\r\n* ~~Fixed a crash on startup when multiple audio devices are plugged in (#4629)~~\r\n* Wizard: Generate a working configuration for isapc (#4961)\r\n* Settings: Use pretty labels for CPU flags (#4940)\r\n* Translation: updated French (thanks @FRtranslator)\r\n* Translation: added Czech readme (thanks @stinovlasmp)\r\n* Translation: updated German (thanks @LostInCompilation and @afh)\r\n* (macOS) Capture Mouse has been renamed to Capture Input and now will show the current capture status as a toggle button\r\n* (macOS) Apple VMs (macOS guests) now support Capture Input which will capture the system keys. This used to be always on as the default. It is now off by default and the toggle button will enable it. (#4667)\r\n* (macOS) Ignore missing links (drives, shared directory, etc) when saving an Apple VM\r\n* (macOS) Preference: added option to force Num Lock on (#4625)\r\n* (macOS) Preference: added option to prevent idle sleep while VM is running (#4963)\r\n* (macOS) Preference: added option to suppress exit confirmation (#4989)\r\n* (macOS) Fixed delete drive confirmation not showing up on latest macOS\r\n* (macOS) Fixed disposable mode stuck on when a VM is run once in disposable mode (#5025)\r\n* (macOS) Fixed an issue where a moved or deleted VM with a stopped window open will attempt to use the old path (#4985)\r\n* (macOS) Fixed cursor scrolling and double click issues (#4636, #4645)\r\n* (macOS) Support following a change in system default input or output audio device (#3488)\r\n* (macOS) Support retry of macOS installation when it fails (the IPSW will not automatically be unlinked)\r\n* (macOS) Support retaining of installer IPSW bookmark across VM moves and UTM restarts (#4938)\r\n\r\n## Issues\r\nPlease check the full list on [Github](https://github.com/utmapp/UTM/issues) and help report any bug you find that is not listed.\r\n\r\n* There is a known bug in newer versions of Mesa which prevents some Wayland applications (such as Firefox) from launching when GPU acceleration is enabled. One workaround is to switch to Xorg from the log-in screen (typically by clicking on the gear icon) and another is to patch Mesa to a newer version.\r\n* Debian 12 fails to load the GUI installer when GPU acceleration is enabled. Please use the text installer instead.\r\n\r\n## Installation\r\n\r\n* [iOS](https://docs.getutm.app/installation/ios/)\r\n* [macOS](https://docs.getutm.app/installation/macos/)\r\n\r\n| File | Description | Installation | JIT | Hypervisor | USB |\r\n|------|------------|--------------|-----|-----------|-----|\r\n| UTM.deb | Jailbroken iOS version | Open in Cydia, dpkg, or Sileo | Yes | Yes(1) | Yes |\r\n| UTM.dmg | macOS version | Mounting and copying UTM.app to /Applications | Yes | Yes | Yes |\r\n| UTM.ipa | Non-jailbroken iOS version (sideloading) | AltStore, etc (see guide) | Yes(2) | No | No |\r\n| UTM.HV.ipa | Non-jailbroken iOS version (TrollStore) | TrollStore | Yes | Yes(1) | Yes |\r\n| UTM.SE.ipa | Non-jailbroken iOS version (sideloading) | AltStore, enterprise signing, etc | No | No | No |\r\n\r\n1. Hypervisor on iOS requires an M1 iPad.\r\n2. Enabling JIT may require a separate JIT enabler such as [Jitterbug][2] or Jitstreamer.\r\n\r\n[1]: https://getutm.app/install/\r\n[2]: https://github.com/osy/Jitterbug",
+                    "sha256": "ef26dd4944c8d4da657d543ee83c37ff33d2cb749cf2aeed1b81c90ea9735e38",
+                    "size": 216841321,
+                    "version": "4.2.5"
+                },
+                {
+                    "date": "2023-04-23T22:15:49Z",
+                    "downloadURL": "https://github.com/utmapp/UTM/releases/download/v4.2.4/UTM.SE.ipa",
+                    "localizedDescription": "## Highlights\r\n* (iOS SE) **TCTI backend updates**. Vector instruction support can improve the performance of certain workloads.\r\n* (macOS) **Guest interface commands**. New commands accessible from the scripting interface as well as the command line interface (utmctl) can be used to read/write files, execute commands, and list IP addresses. These commands require QEMU guest agent to be installed.\r\n* (macOS) **Scripting interface additions**. The scripting interface now allows for creation of a new VM, configuration an existing VM, changing drive image, and more. See [this page](https://docs.getutm.app/scripting/reference/) for more details and [the cheat sheet](https://docs.getutm.app/scripting/cheat-sheet/) for example usage.\r\n* (macOS) **External read-write drive images**. In QEMU, if a supported drive interface is selected (USB, Floppy, etc) along with an image type of Disk, the drive can now be marked as either read-only or read-write. This can be used as an alternative way of transferring data to and from the VM when the guest does not support SPICE or VirtFS. In AVF, support for read-write images has be fixed as well (when \"read only\" is unchecked in the settings).\r\n\r\n## Changes (v4.2.4)\r\n* UTM will now display the release notes the first time a new version is launched\r\n* Updated ANGLE which should fix some GPU acceleration issues on Linux (please see known issues below for unresolved issues)\r\n* Fixed an issue where a removable drive or VirtIO shared directory was set up when QEMUHelper was already running and therefore was not able to create a bookmark and an \"access denied\" error shows up on startup\r\n* Introduced a new preference setting for using the Option key as Meta in the built in console. This was on by default in previous versions and is not off by default which should allow international text to be entered properly (#5202)\r\n* Wizard: Make virtio-gpu-pci default for Linux (again) which was reverted a few releases ago in order to address some GPU issues\r\n* Translation: updated Polish (thanks @matgaj)\r\n* (iOS) Fixed built in terminal overlapping in the safe area\r\n\r\n## Changes (v4.2.3)\r\n* Added support for read-write removable devices on supported interfaces (USB, Floppy, etc). To use this feature, set the image type to \"Disk\" and uncheck the \"Read Only?\" option in the drive settings. Note that you may have to eject and re-mount the drive image for effect to take place. (#5079)\r\n* Removable USB devices will no longer show up as a CD drive if the image type is set to \"Disk\" (#5171)\r\n* Reverted a change from v4.2.0 where virtio bus devices were removed (this broke some people's configurations) (#5137)\r\n* Fixed an issue where when QEMU fails to start, subsequent attempts to start the VM will automatically fail\r\n* Fixed an issue where due to a race, removable drives may not be mounted on start\r\n* (iOS) Fixed an issue when the pointer is hovering over a toolbar button when the VM starts and subsequent clicks will toggle the button (#4843)\r\n* (macOS) AVF: Fixed an issue where a removable drive that is not marked as read-only still gets marked as read-only after restarting UTM (when upgrading from a previous version, you must eject and re-mount the image for effect to take place) (#5170)\r\n* (macOS) Fixed an issue where incorrect subnet parameters are generated for vmnet advanced settings (#5128)\r\n* (macOS) CLI: Added a new `clone` command (#5004)\r\n\r\n## Changes (v4.2.2)\r\n* Fixed an issue where a VM that is moved manually (e.g. with Finder) cannot be started (#5121)\r\n* Fixed an issue where the cursor disappears after resuming a suspended VM (#4665)\r\n* (macOS) Scripting: Add support for `make`, `duplicate`, and `delete` verbs on virtual machines\r\n* (macOS) Scripting: Add support for modifying certain configuration options\r\n* (macOS) Scripting: Removed virtual machine properties: `notes`, `machine`, `architecture`, `memory`. You should now use similar properties in the `configuration` record\r\n* (macOS) Support changing the audio backend to CoreAudio and make CoreAudio the default (due to better latency and as a workaround to some crashes) (#5125)\r\n\r\n## Changes (v4.2.1)\r\n* QEMU: Support more than 8 cores for ARM64 targets (#4847)\r\n* Synchronize time on resume when QEMU guest agent is installed which should fix clock drift issues (#3218)\r\n* (iOS SE) Updated TCTI to latest branch from @ktemkin which has support for vector instructions (#4865)\r\n* (macOS) Switch to emulated trackpad when guest+host are macOS 13+ (second attempt for #4636 and #4645)\r\n* (macOS) Fixed the \"raw image\" checkbox when creating a new drive (#5100)\r\n* (macOS) Add PC speaker sound device as an option. You can now add a second sound device on supported targets (x86_64/i386 PC based targets) and set the hardware to PC Speaker to emulate older motherboard speakers.\r\n* (macOS) Scripting: new verbs \"open file\", \"execute\", and \"query ip\" which uses the QEMU guest agent to send commands to the guest. Use the Apple Script Editor's Open Dictionary tool for more information.\r\n* (macOS) CLI: new commands \"file push\", \"file pull\", \"exec\", and \"ip-address\". See `utmctl help` for more information.\r\n\r\n## Changes (v4.2.0)\r\n* Updated virglrenderer to latest (27/02/2023) commit\r\n* Automatically revert CPU to \"default\" if model is missing due to updated QEMU (#4910)\r\n* ~~Remove virtio-bus devices (they didn't work) (#4893)~~\r\n* Support drag and drop to import an .utm package (#3599)\r\n* Support copying sparse images across different volumes (thanks @ktprograms)\r\n* Fixed tearing/performance issue for non-GL accelerated displays when under graphics load (#5049)\r\n* Fixed error when importing a new drive with the same name as an existing drive (#5052)\r\n* ~~Fixed a crash on startup when multiple audio devices are plugged in (#4629)~~\r\n* Wizard: Generate a working configuration for isapc (#4961)\r\n* Settings: Use pretty labels for CPU flags (#4940)\r\n* Translation: updated French (thanks @FRtranslator)\r\n* Translation: added Czech readme (thanks @stinovlasmp)\r\n* Translation: updated German (thanks @LostInCompilation and @afh)\r\n* (macOS) Capture Mouse has been renamed to Capture Input and now will show the current capture status as a toggle button\r\n* (macOS) Apple VMs (macOS guests) now support Capture Input which will capture the system keys. This used to be always on as the default. It is now off by default and the toggle button will enable it. (#4667)\r\n* (macOS) Ignore missing links (drives, shared directory, etc) when saving an Apple VM\r\n* (macOS) Preference: added option to force Num Lock on (#4625)\r\n* (macOS) Preference: added option to prevent idle sleep while VM is running (#4963)\r\n* (macOS) Preference: added option to suppress exit confirmation (#4989)\r\n* (macOS) Fixed delete drive confirmation not showing up on latest macOS\r\n* (macOS) Fixed disposable mode stuck on when a VM is run once in disposable mode (#5025)\r\n* (macOS) Fixed an issue where a moved or deleted VM with a stopped window open will attempt to use the old path (#4985)\r\n* (macOS) Fixed cursor scrolling and double click issues (#4636, #4645)\r\n* (macOS) Support following a change in system default input or output audio device (#3488)\r\n* (macOS) Support retry of macOS installation when it fails (the IPSW will not automatically be unlinked)\r\n* (macOS) Support retaining of installer IPSW bookmark across VM moves and UTM restarts (#4938)\r\n\r\n## Issues\r\nPlease check the full list on [Github](https://github.com/utmapp/UTM/issues) and help report any bug you find that is not listed.\r\n\r\n* There is a known bug in newer versions of Mesa which prevents some Wayland applications (such as Firefox) from launching when GPU acceleration is enabled. One workaround is to switch to Xorg from the log-in screen (typically by clicking on the gear icon) and another is to patch Mesa to a newer version.\r\n* Debian 12 fails to load the GUI installer when GPU acceleration is enabled. Please use the text installer instead.\r\n* The Metal renderer backend is broken on macOS, please change your renderer to OpenGL or \"Default\"\r\n\r\n## Installation\r\n\r\n* [iOS](https://docs.getutm.app/installation/ios/)\r\n* [macOS](https://docs.getutm.app/installation/macos/)\r\n\r\n| File | Description | Installation | JIT | Hypervisor | USB |\r\n|------|------------|--------------|-----|-----------|-----|\r\n| UTM.deb | Jailbroken iOS version | Open in Cydia, dpkg, or Sileo | Yes | Yes(1) | Yes |\r\n| UTM.dmg | macOS version | Mounting and copying UTM.app to /Applications | Yes | Yes | Yes |\r\n| UTM.ipa | Non-jailbroken iOS version (sideloading) | AltStore, etc (see guide) | Yes(2) | No | No |\r\n| UTM.HV.ipa | Non-jailbroken iOS version (TrollStore) | TrollStore | Yes | Yes(1) | Yes |\r\n| UTM.SE.ipa | Non-jailbroken iOS version (sideloading) | AltStore, enterprise signing, etc | No | No | No |\r\n\r\n1. Hypervisor on iOS requires an M1 iPad.\r\n2. Enabling JIT may require a separate JIT enabler such as [Jitterbug][2] or Jitstreamer.\r\n\r\n[1]: https://getutm.app/install/\r\n[2]: https://github.com/osy/Jitterbug",
+                    "sha256": "a8cc3869b731b7803d068c00019b19b9288e51d161adeef1723be845790d355f",
+                    "size": 216630098,
+                    "version": "4.2.4"
+                },
+                {
+                    "date": "2023-02-27T02:28:31Z",
+                    "downloadURL": "https://github.com/utmapp/UTM/releases/download/v4.1.6/UTM.SE.ipa",
+                    "localizedDescription": "This is the same release as v4.1.5 but with the change to default enable GPU acceleration for Linux reverted. This is due to a number of guest-side driver issues in the latest version of Mesa (#4983). As a result of these issues, we decided to disable GPU acceleration in Linux by default for new VMs created by the wizard. If you have an existing VM with graphical issues, you can disable GPU acceleration by going into the VM settings, under Display, change the Emulated Display Card to `virtio-gpu-pci` or another card that does not have `-gl` in the name. You can verify that GPU acceleration is disabled when the checkbox below the card is unchecked.\r\n\r\n## Highlights\r\n* **QEMU backend updated to v7.2.0**. Also updated usbredir (0.13.0), virglrenderer (latest commit), ANGLE (latest commit)\r\n* **Improved renderer backend**. Lots of bug fixes and stability improvements to GPU accelerated Linux VMs (most common crashes when GPU acceleration is enabled should be gone now). New option to change the renderer backend to ANGLE Metal and limit FPS (in Preferences). Switching to Metal is highly recommended.\r\n* (iOS) **TrollStore build (UTM.HV.ipa) now supports JIT**. Additionally, there is now in-app settings.\r\n* (iOS) **TrollStore build now supports TSO (Total Store Ordering)**. TSO is used by Rosetta on the Mac to improve x86_64 emulation on ARM64. It can now be used on M1 iPads with QEMU to improve performance of FEX-Emu or a patched Rosetta. Note that it is recommended that TSO be disabled if you do not need to emulate x86_64 because it can reduce performance of other tasks.\r\n* (macOS) **AppleScript (OSA) support and CLI interface**. You can control parts of UTM through the OSA interface. Currently there is support for listing VMs as well as start/stop/suspend operations and the ability to print out the guest serial port connections. More functionality will be added in the future. A command line application is also provided in `UTM.app/Contents/MacOS/utmctl` (which you can symlink to `/usr/local/bin/utmctl` if desired) that can be used for automation tasks without needing to learn AppleScript.\r\n* (macOS 13+) **Menu bar extra**. You can enable the menu bar extra icon in Preferences (Cmd+,) as well as disable the dock icon. The menu bar extra provides a minimal interface to start/stop/suspend VMs and is useful when paired with headless VMs (a VM that does not have any display or terminal console installed).\r\n\r\n## Notes\r\n* **iOS 14 and macOS 11.3** are the minimum supported systems for UTM v4.x. Please use UTM v3.x for support down to iOS 11 and macOS 11\r\n* ~~Newly created Linux VMs will now use `virtio-gpu-gl-pci` by default. It is recommended that you change the display card of existing QEMU backend Linux VMs to this card in order to take advantage of the improved renderer backend. This should result in improved performance in GUI rendering. Note that some applications (particularly 3D applications) may lock up or crash UTM and if you are experiencing issues, you can go back to `virtio-ramfb` or `virtio-vga`.~~\r\n* Newly created Windows VMs will now use `virtio-ramfb-gl` (Apple Silicon) or `virtio-vga-gl` (Intel) by default. There is NO 3D acceleration drivers for Windows yet, so unlike Linux, this will not improve any compatibility with applications. However, the GL backend can still be beneficial to Windows users because it has smoother animations and less tearing and artifacts. The overall benefits will not be as pronounced as for Linux VMs so it is optional that you change existing VMs to a `-gl` display card.\r\n* (iOS) It is recommended that you switch to the Metal backend in Preferences for better performance. However, some applications such as `glxgears` will not work with the Metal backend.\r\n\r\n## Changes (v4.1.6)\r\n* Wizard: Re-introduced the checkbox for \"Hardware OpenGL Acceleration\" which is disabled by default due to guest-side issues in the latest Mesa driver\r\n\r\n## Changes (v4.1.5)\r\n* Improved rendering of non-GL graphics on the new renderer backend. This should reduce some of the tearing seen in earlier updates. For the best performance, it is recommended that a GL backend is selected.\r\n* Support read-only disk images in QEMU backend as well as selecting images that are read-only (#4838) Note: all external drive images (ISOs) are now loaded as read-only, this was not enforced in previous versions due to an error in the logic.\r\n* Newly created Windows VMs will now use `virtio-ramfb-gl` (Apple Silicon) or `virtio-vga-gl` (Intel) by default. See the Notes section for more information.\r\n* Fixed an issue where the incorrect tmp directory path was used by QEMU (#4882)\r\n* Scripting: Fixed an issue where the proper error message was not displayed in some cases.\r\n* CLI: Improved some help text.\r\n* Localization: updated Japanese (thanks @MMP0)\r\n\r\n## Changes (v4.1.4)\r\n* Fixed slow rendering of GRUB and EFI menus\r\n* Introduced new optimizations to renderer: bliting done on GPU instead of CPU now (for non-GL rendering), guest draw calls that are faster than the monitor refresh rate are now consolidated before drawing at vblank, rendering of multiple displays can happen concurrently now\r\n* Fixed rendering to multiple displays on the new renderer backend\r\n* Fixed an issue in QEMU where the vmnet backend uses 100% of CPU when the VM is suspended (#4803)\r\n* (iOS) TrollStore: Fixed JIT enable in the HV builds\r\n* (iOS) TrollStore: New option to enable TSO (Total Store Ordering) in QEMU settings (see Highlights for more details)\r\n* (iOS) Restored the default renderer backend to GL. This was changed in v4.1.3 because Metal is faster but the new backend can introduce regressions such as `glxgears` not working (#4856). As a result, the new backend is now opt-in but is still highly recommended.\r\n* (iOS) Fixed crash when changing VM settings on iOS 14 (#4864)\r\n* (iOS) Fixed crash when starting a VM with UTM SE (#4848)\r\n* (macOS) A tooltip will now reveal why suspend functionality is disabled\r\n\r\n## Changes (v4.1.3)\r\n* Updated QEMU to v7.2.0\r\n* Reworked CocoaSpice renderer to respond faster to GL updates from the guest, should improve frame pacing on GL supported Linux VMs\r\n* Added global setting to change renderer backend, introduce ANGLE Metal as an option (and also the new default for iOS)\r\n* Added global setting to limit FPS which can be used to improve frame pacing for a smoother rendering experience\r\n* Settings: clearly show if the current display hardware supports GPU acceleration\r\n* Wizard: GPU acceleration is now enabled by default when Linux is selected as the operating system\r\n* Fixed crash due to an error with `GL_DRAW_COOKIE_INVALID` (#4722)\r\n* Fixed deadlock on startup caused by gstosxaudio (#2364)\r\n* Fixed memory leak when GPU acceleration is enabled (#4449)\r\n* Fixed crash in `-[MTLResourceList releaseAllObjectsAndReset]` (#3519)\r\n* Fixed Mesa issue causing some GNOME desktop to freeze when GPU acceleration is enabled\r\n* Fixed incorrect logic when cloning a VM (#4815)\r\n* Fixed some thread scheduling warning (#4352)\r\n* Localization: updated French (thanks @FRtranslator)\r\n* (iOS) TrollStore build: use `com.apple.private.security.no-sandbox` instead of `com.apple.private.security.no-container` on recommendation of other devs and to align with how other apps perform JIT.\r\n* (iOS) Fixed blank screen when choosing \"Open\" in the wizard (#4842)\r\n* (iOS) Fixed toolbar not auto-hiding before first interaction (#4844)\r\n* (macOS) New design for global settings (Cmd+,) which better organizes the settings\r\n* (macOS) utmctl: Fixed crash when `utmctl help attach` runs (#4817)\r\n* (macOS) utmctl: Fixed `utmctl stop` with `--request` and `kill` (#4850)\r\n\r\n## Changes (v4.1.2)\r\n* Localization: updated Spanish (Latin America) (thanks @JezerM)\r\n* Localization: updated Japanese (thanks @MMP0 and @skyarrow87)\r\n* Localization: updated Chinese Simplified (thanks @changanmoon)\r\n* (iOS) Fix new VM wizard not appearing on < iOS 14.5 (#4776)\r\n* (macOS) Implement OSA interface for AppleScript\r\n* (macOS) Introduce a CLI application (`UTM.app/Contents/MacOS/utmctl`) that wraps around the OSA interface for automation\r\n* (macOS 13+) New settings option to enable a menu bar extra icon for controlling VMs\r\n* (macOS 13+) New settings option to disable the dock icon\r\n* (macOS) Fix various alignment issues in settings (#4596) (thanks @JezerM)\r\n* (macOS) Fix a crash when the pasteboard is updated (#4745)\r\n* (macOS) Support custom resolutions for Apple Virtualization VMs\r\n* (macOS) Fixed a UI freeze when canceling out of the settings for an Apple Virtualization VM\r\n\r\n## Changes (v4.1.1)\r\n* Fixed launching SPARC machines (#4575)\r\n* Fixed an error when attempting to save a VM where one of its removable drives is linked to a file that has been deleted\r\n* Fixed IPSW/.utm download failing when the device goes to sleep (the download should resume after wake up)\r\n* Restored scroll bars when system is set to always show scroll bars. Added a new SwiftUI crash workaround thanks to @evelyneee.\r\n* Display all sizes in binary (MiB/GiB) mode in order to be consistent (#4396)\r\n* Localization: added Polish (thanks @mavethee)\r\n* Localization: updated Japanese (thanks @MMP0)\r\n* Localization: updated Spanish (Latin America) (thanks @JezerM)\r\n* Localization: updated French (thanks @FRtranslator)\r\n* (macOS) Fixed the port forward UI on macOS 11 and introduce a new port forward UI for macOS 12+ (#4690)\r\n* (macOS) Fixed \"This virtual machine cannot be run on this machine.\" error on a newly created Apple VM (#4595)\r\n* (macOS) Added new 21:9 widescreen resolution for Apple VMs (thanks @Tandolf)\r\n* (macOS) Added a clarifying message about shared directory support on older macOS guests (#4594)\r\n* (macOS) Added new shutdown options (software request and force kill) which can be toggled by long pressing the power button in the VM window (#4001)\r\n* (macOS) Added a confirmation dialog when deleting a drive (#4687)\r\n\r\n## Changes (v4.1.0)\r\n* Updated QEMU to v7.1.0\r\n* Updated ANGLE and virglrenderer to latest commit\r\n* Fixed an issue where user override of machine property settings was not applied properly\r\n* Localization: updated Japanese (thanks @MMP0)\r\n* Localization: updated Spanish (Latin America) (thanks @JezerM)\r\n* (iOS) Added in-app settings popover which synchronizes with the Settings app (useful for TrollStore installs where the Settings app page is inaccessible) (#4446)\r\n* (iOS) TrollStore: support JIT without needing a separate JIT enabler (thanks @PojavLauncherTeam for the idea)\r\n\r\n## Issues\r\nPlease check the full list on [Github][2] and help report any bug you find that is not listed.\r\n\r\n## Installation\r\n\r\n* [iOS](https://docs.getutm.app/installation/ios/)\r\n* [macOS](https://docs.getutm.app/installation/macos/)\r\n\r\n| File | Description | Installation | JIT | Hypervisor | USB |\r\n|------|------------|--------------|-----|-----------|-----|\r\n| UTM.deb | Jailbroken iOS version | Open in Cydia, dpkg, or Sileo | Yes | Yes(1) | Yes |\r\n| UTM.dmg | macOS version | Mounting and copying UTM.app to /Applications | Yes | Yes | Yes |\r\n| UTM.ipa | Non-jailbroken iOS version (sideloading) | AltStore, etc (see guide) | Yes(2) | No | No |\r\n| UTM.HV.ipa | Non-jailbroken iOS version (TrollStore) | TrollStore | Yes | Yes(1) | Yes |\r\n| UTM.SE.ipa | Non-jailbroken iOS version (sideloading) | AltStore, enterprise signing, etc | No | No | No |\r\n\r\n1. Hypervisor on iOS requires an M1 iPad.\r\n2. Enabling JIT may require a separate JIT enabler such as [Jitterbug][3] or Jitstreamer.\r\n\r\n[1]: https://getutm.app/install/\r\n[2]: https://github.com/utmapp/UTM/issues\r\n[3]: https://github.com/osy/Jitterbug",
+                    "sha256": "23e0634405388a01cadd1a864fecb81011b3c926b07ee818a311349a04668c92",
+                    "size": 149873322,
+                    "version": "4.1.6"
+                },
+                {
+                    "date": "2023-01-04T04:12:52Z",
+                    "downloadURL": "https://github.com/utmapp/UTM/releases/download/v4.1.5/UTM.SE.ipa",
+                    "localizedDescription": "## Highlights\r\n* **QEMU backend updated to v7.2.0**. Also updated usbredir (0.13.0), virglrenderer (latest commit), ANGLE (latest commit)\r\n* **Improved renderer backend**. Lots of bug fixes and stability improvements to GPU accelerated Linux VMs (most common crashes when GPU acceleration is enabled should be gone now). New option to change the renderer backend to ANGLE Metal and limit FPS (in Preferences). Switching to Metal is highly recommended.\r\n* (iOS) **TrollStore build (UTM.HV.ipa) now supports JIT**. Additionally, there is now in-app settings.\r\n* (iOS) **TrollStore build now supports TSO (Total Store Ordering)**. TSO is used by Rosetta on the Mac to improve x86_64 emulation on ARM64. It can now be used on M1 iPads with QEMU to improve performance of FEX-Emu or a patched Rosetta. Note that it is recommended that TSO be disabled if you do not need to emulate x86_64 because it can reduce performance of other tasks.\r\n* (macOS) **AppleScript (OSA) support and CLI interface**. You can control parts of UTM through the OSA interface. Currently there is support for listing VMs as well as start/stop/suspend operations and the ability to print out the guest serial port connections. More functionality will be added in the future. A command line application is also provided in `UTM.app/Contents/MacOS/utmctl` (which you can symlink to `/usr/local/bin/utmctl` if desired) that can be used for automation tasks without needing to learn AppleScript.\r\n* (macOS 13+) **Menu bar extra**. You can enable the menu bar extra icon in Preferences (Cmd+,) as well as disable the dock icon. The menu bar extra provides a minimal interface to start/stop/suspend VMs and is useful when paired with headless VMs (a VM that does not have any display or terminal console installed).\r\n\r\n## Notes\r\n* **iOS 14 and macOS 11.3** are the minimum supported systems for UTM v4.x. Please use UTM v3.x for support down to iOS 11 and macOS 11\r\n* Newly created Linux VMs will now use `virtio-gpu-gl-pci` by default. It is recommended that you change the display card of existing QEMU backend Linux VMs to this card in order to take advantage of the improved renderer backend. This should result in improved performance in GUI rendering. Note that some applications (particularly 3D applications) may lock up or crash UTM and if you are experiencing issues, you can go back to `virtio-ramfb` or `virtio-vga`.\r\n* Newly created Windows VMs will now use `virtio-ramfb-gl` (Apple Silicon) or `virtio-vga-gl` (Intel) by default. There is NO 3D acceleration drivers for Windows yet, so unlike Linux, this will not improve any compatibility with applications. However, the GL backend can still be beneficial to Windows users because it has smoother animations and less tearing and artifacts. The overall benefits will not be as pronounced as for Linux VMs so it is optional that you change existing VMs to a `-gl` display card.\r\n* (iOS) It is recommended that you switch to the Metal backend in Preferences for better performance. However, some applications such as `glxgears` will not work with the Metal backend.\r\n\r\n## Changes (v4.1.5)\r\n* Improved rendering of non-GL graphics on the new renderer backend. This should reduce some of the tearing seen in earlier updates. For the best performance, it is recommended that a GL backend is selected.\r\n* Support read-only disk images in QEMU backend as well as selecting images that are read-only (#4838) Note: all external drive images (ISOs) are now loaded as read-only, this was not enforced in previous versions due to an error in the logic.\r\n* Newly created Windows VMs will now use `virtio-ramfb-gl` (Apple Silicon) or `virtio-vga-gl` (Intel) by default. See the Notes section for more information.\r\n* Fixed an issue where the incorrect tmp directory path was used by QEMU (#4882)\r\n* Scripting: Fixed an issue where the proper error message was not displayed in some cases.\r\n* CLI: Improved some help text.\r\n* Localization: updated Japanese (thanks @MMP0)\r\n\r\n## Changes (v4.1.4)\r\n* Fixed slow rendering of GRUB and EFI menus\r\n* Introduced new optimizations to renderer: bliting done on GPU instead of CPU now (for non-GL rendering), guest draw calls that are faster than the monitor refresh rate are now consolidated before drawing at vblank, rendering of multiple displays can happen concurrently now\r\n* Fixed rendering to multiple displays on the new renderer backend\r\n* Fixed an issue in QEMU where the vmnet backend uses 100% of CPU when the VM is suspended (#4803)\r\n* (iOS) TrollStore: Fixed JIT enable in the HV builds\r\n* (iOS) TrollStore: New option to enable TSO (Total Store Ordering) in QEMU settings (see Highlights for more details)\r\n* (iOS) Restored the default renderer backend to GL. This was changed in v4.1.3 because Metal is faster but the new backend can introduce regressions such as `glxgears` not working (#4856). As a result, the new backend is now opt-in but is still highly recommended.\r\n* (iOS) Fixed crash when changing VM settings on iOS 14 (#4864)\r\n* (iOS) Fixed crash when starting a VM with UTM SE (#4848)\r\n* (macOS) A tooltip will now reveal why suspend functionality is disabled\r\n\r\n## Changes (v4.1.3)\r\n* Updated QEMU to v7.2.0\r\n* Reworked CocoaSpice renderer to respond faster to GL updates from the guest, should improve frame pacing on GL supported Linux VMs\r\n* Added global setting to change renderer backend, introduce ANGLE Metal as an option (and also the new default for iOS)\r\n* Added global setting to limit FPS which can be used to improve frame pacing for a smoother rendering experience\r\n* Settings: clearly show if the current display hardware supports GPU acceleration\r\n* Wizard: GPU acceleration is now enabled by default when Linux is selected as the operating system\r\n* Fixed crash due to an error with `GL_DRAW_COOKIE_INVALID` (#4722)\r\n* Fixed deadlock on startup caused by gstosxaudio (#2364)\r\n* Fixed memory leak when GPU acceleration is enabled (#4449)\r\n* Fixed crash in `-[MTLResourceList releaseAllObjectsAndReset]` (#3519)\r\n* Fixed Mesa issue causing some GNOME desktop to freeze when GPU acceleration is enabled\r\n* Fixed incorrect logic when cloning a VM (#4815)\r\n* Fixed some thread scheduling warning (#4352)\r\n* Localization: updated French (thanks @FRtranslator)\r\n* (iOS) TrollStore build: use `com.apple.private.security.no-sandbox` instead of `com.apple.private.security.no-container` on recommendation of other devs and to align with how other apps perform JIT.\r\n* (iOS) Fixed blank screen when choosing \"Open\" in the wizard (#4842)\r\n* (iOS) Fixed toolbar not auto-hiding before first interaction (#4844)\r\n* (macOS) New design for global settings (Cmd+,) which better organizes the settings\r\n* (macOS) utmctl: Fixed crash when `utmctl help attach` runs (#4817)\r\n* (macOS) utmctl: Fixed `utmctl stop` with `--request` and `kill` (#4850)\r\n\r\n## Changes (v4.1.2)\r\n* Localization: updated Spanish (Latin America) (thanks @JezerM)\r\n* Localization: updated Japanese (thanks @MMP0 and @skyarrow87)\r\n* Localization: updated Chinese Simplified (thanks @changanmoon)\r\n* (iOS) Fix new VM wizard not appearing on < iOS 14.5 (#4776)\r\n* (macOS) Implement OSA interface for AppleScript\r\n* (macOS) Introduce a CLI application (`UTM.app/Contents/MacOS/utmctl`) that wraps around the OSA interface for automation\r\n* (macOS 13+) New settings option to enable a menu bar extra icon for controlling VMs\r\n* (macOS 13+) New settings option to disable the dock icon\r\n* (macOS) Fix various alignment issues in settings (#4596) (thanks @JezerM)\r\n* (macOS) Fix a crash when the pasteboard is updated (#4745)\r\n* (macOS) Support custom resolutions for Apple Virtualization VMs\r\n* (macOS) Fixed a UI freeze when canceling out of the settings for an Apple Virtualization VM\r\n\r\n## Changes (v4.1.1)\r\n* Fixed launching SPARC machines (#4575)\r\n* Fixed an error when attempting to save a VM where one of its removable drives is linked to a file that has been deleted\r\n* Fixed IPSW/.utm download failing when the device goes to sleep (the download should resume after wake up)\r\n* Restored scroll bars when system is set to always show scroll bars. Added a new SwiftUI crash workaround thanks to @evelyneee.\r\n* Display all sizes in binary (MiB/GiB) mode in order to be consistent (#4396)\r\n* Localization: added Polish (thanks @mavethee)\r\n* Localization: updated Japanese (thanks @MMP0)\r\n* Localization: updated Spanish (Latin America) (thanks @JezerM)\r\n* Localization: updated French (thanks @FRtranslator)\r\n* (macOS) Fixed the port forward UI on macOS 11 and introduce a new port forward UI for macOS 12+ (#4690)\r\n* (macOS) Fixed \"This virtual machine cannot be run on this machine.\" error on a newly created Apple VM (#4595)\r\n* (macOS) Added new 21:9 widescreen resolution for Apple VMs (thanks @Tandolf)\r\n* (macOS) Added a clarifying message about shared directory support on older macOS guests (#4594)\r\n* (macOS) Added new shutdown options (software request and force kill) which can be toggled by long pressing the power button in the VM window (#4001)\r\n* (macOS) Added a confirmation dialog when deleting a drive (#4687)\r\n\r\n## Changes (v4.1.0)\r\n* Updated QEMU to v7.1.0\r\n* Updated ANGLE and virglrenderer to latest commit\r\n* Fixed an issue where user override of machine property settings was not applied properly\r\n* Localization: updated Japanese (thanks @MMP0)\r\n* Localization: updated Spanish (Latin America) (thanks @JezerM)\r\n* (iOS) Added in-app settings popover which synchronizes with the Settings app (useful for TrollStore installs where the Settings app page is inaccessible) (#4446)\r\n* (iOS) TrollStore: support JIT without needing a separate JIT enabler (thanks @PojavLauncherTeam for the idea)\r\n\r\n## Issues\r\nPlease check the full list on [Github][2] and help report any bug you find that is not listed.\r\n\r\n## Installation\r\n\r\n* [iOS](https://docs.getutm.app/installation/ios/)\r\n* [macOS](https://docs.getutm.app/installation/macos/)\r\n\r\n| File | Description | Installation | JIT | Hypervisor | USB |\r\n|------|------------|--------------|-----|-----------|-----|\r\n| UTM.deb | Jailbroken iOS version | Open in Cydia, dpkg, or Sileo | Yes | Yes(1) | Yes |\r\n| UTM.dmg | macOS version | Mounting and copying UTM.app to /Applications | Yes | Yes | Yes |\r\n| UTM.ipa | Non-jailbroken iOS version (sideloading) | AltStore, etc (see guide) | Yes(2) | No | No |\r\n| UTM.HV.ipa | Non-jailbroken iOS version (TrollStore) | TrollStore | Yes | Yes(1) | Yes |\r\n| UTM.SE.ipa | Non-jailbroken iOS version (sideloading) | AltStore, enterprise signing, etc | No | No | No |\r\n\r\n1. Hypervisor on iOS requires an M1 iPad.\r\n2. Enabling JIT may require a separate JIT enabler such as [Jitterbug][3] or Jitstreamer.\r\n\r\n[1]: https://getutm.app/install/\r\n[2]: https://github.com/utmapp/UTM/issues\r\n[3]: https://github.com/osy/Jitterbug",
+                    "size": 149850250,
+                    "version": "4.1.5"
+                },
+                {
                     "date": "2022-10-21T16:16:34Z",
                     "downloadURL": "https://github.com/utmapp/UTM/releases/download/v4.0.9/UTM.SE.ipa",
                     "localizedDescription": "## Highlights\r\n* **Multiple display and headless display is now supported for QEMU machines.** You can configure 0 or more displays as well as 0 or more builtin terminal consoles. On macOS, a new window will be created for each display and builtin terminal. On iOS, you can create multiple windows (iPad) as well as plug in an external display or AirPlay (iPad or iPhone) and assign outputs to each window.\r\n* **Ventura updates to Virtualization.** macOS Ventura introduces new features that is now integrated into UTM. You can now create GUI Linux VMs with EFI boot. Directory sharing now works with macOS Ventura guests. Rosetta x86_64 emulation is supported for Linux VMs on Apple Silicon. Check out https://docs.getutm.app/guides/debian/ for an installation guide. Note that base M1 chip users may experience issues that will be addressed in a future update.\r\n* **VirtFS sharing for QEMU.** This alternative directory sharing backend is supported by Linux and can have better performance. Note that macOS UID are numbered differently than Linux so you may have to run `chown` in the guest. Check out https://docs.getutm.app/guest-support/linux/ for more details.\r\n* **Easier Windows 10/11 installation and Windows guest tools downloader.** You can now download and mount the Windows drivers and guest tools ISO image with a single click (macOS: disk icon in VM window, iOS: 3D touch context menu on home screen). Additionally, the ISO now include an \"Autounattend.xml\" which is recognized by the Windows 10/11 installer. When mounted to a second CD drive, the installer will install the correct drivers, bypass secure boot/TPM requirements, and launch the SPICE tools installer on first login.\r\n* (macOS) **Resize QEMU disk images.** In the drives settings page, you can now expand the size of the QCOW2 disk image.\r\n* (iOS) **QEMU Virtualization for M1 iPad.** With the release of [TrollStore](https://github.com/opa334/TrollStore), you can now enable Hypervisor on iOS. Note that only M1 hardware and kernel have support for Hypervisor. iOS 14.4.2-14.5.1 is supported only on M1 iPad Pro jailbroken with fugu14/unc0ver. iOS 14.0-15.5b4 is supported on any M1 iPad running TrollStore.\r\n* **New documentation site.** https://docs.getutm.app/ is the home of the official UTM documentation.\r\n* **New localization.** Thanks to various community members, UTM is now translated to: Chinese (Simplified), Chinese (Traditional), Finnish, French, German, Japanese, Korean, and Spanish (Latin America)\r\n\r\n## Notes\r\n* **iOS 14 and macOS 11.3** are the new minimum supported systems. Please use UTM v3.x for support down to iOS 11 and macOS 11\r\n* The configuration backend has been massively rewritten. **Please backup all VMs prior to updating as you will not be able to re-open VMs saved by UTM v4 on older versions of UTM if you decide to downgrade.**\r\n* Since v4.0.6, the order of generated devices has changed to always create network devices first. This is to address an issue on some distributions (such as Ubuntu) where adding a device (drive, display, etc) would require re-configurating the network because the device name changed. Unfortunately, this change will cause the configuration issue to occur once more on any existing VM that is susceptible to the network issue. On Ubuntu, this will require you to modify `/etc/netplan/00-installer-config.yaml` and change the adapter name from `enp0s9` (or whatever it is currently) to `enp0s1` (which reflects the new device ordering). Other Linux distributions may require a similar change. However, after updating the guest network configuration, you should no longer have issues with networking when making device changes to the VM.\r\n\r\n## Changes (v4.0.9)\r\n\r\n* Fixed some broken links to documentation (#4529)\r\n* Fixed an issue where running ARM64 emulation on ARM64 gives an error \"The \u2018host\u2019 CPU type can only be used with KVM or HVF\" (#4528)\r\n* Fixed a regression where S390x and SPARC VMs cannot start due to missing USB bus\r\n* (iOS) Fixed UTM SE cannot launch any VMs (#4516)\r\n\r\n## Changes (v4.0.8)\r\n\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator and @alexis-martel)\r\n* Translation: Added German (thanks @conath)\r\n* (macOS) Disable resize button in GUI Apple VM window\r\n* (macOS) Reverted some SwiftUI issue workarounds that are no longer present in Ventura RC\r\n\r\n## Changes (v4.0.7)\r\n\r\n* Fixed renamed VM not appearing on next launch (#4469)\r\n* Fixed TCP server not working (#4479)\r\n* Fixed random network issues caused by invalid MAC address generation (you must re-generate MAC to apply the change if your VM created in UTM v4 does not have working network) (#4477)\r\n* Fixed a crash when trying to boot Kali Linux with terminal enabled\r\n* Fixed hypervisor on iOS 14.6-14.8\r\n* Added new setting for serial device in TCP server mode to listen on remote/local interfaces (#4483)\r\n* Fixed URL automation sending text to terminal\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* Wizard: Link to new documentation site (#4443, #4445)\r\n* (iOS) Fixed disponible run option not appearing\r\n* (macOS) Fixed settings getting stuck at information page (#4465)\r\n* (macOS) Updated display menu option to match title bar when multiple displays are used (#4484)\r\n* (macOS) Fixed no mouse/keyboard on Intel Apple Virtualization (#4409)\r\n* (macOS) Fixed no audio input device on Linux running on Apple Virtualization (#4409)\r\n* (macOS) Fixed auto-quit when all windows are closed happening when headless VM is still running\r\n\r\n## Changes (v4.0.6)\r\n\r\n* Fixed an issue in argument generation where PS/2 input was forced even when USB was enabled (#4424)\r\n* Validate settings on save before closing the settings dialog\r\n* Network devices are now created first before all other devices. Note this means that networking will be broken on some existing VMs and must be re-configured! (See notes above)\r\n* Fixed a deadlock issue when saving settings\r\n* Fixed an error when saving a VM with an external drive selected\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* Wizard: The Windows guest tools auto-installer currently only works on Windows 10 and above. A new option is added in the wizard to make this explicit. (#4440)\r\n* Wizard: Use VirtFS sharing by default when Linux is selected\r\n* (iOS) Default to emulated network instead of failing when importing a VM created on macOS\r\n* (macOS) Fixed an issue where opening a new display window from a serial window did not work\r\n* (macOS) Fixed logic on macOS 11 where serial window was not created\r\n* (macOS) Fixed a crash on macOS 11 when saving settings while the QEMU tab is selected\r\n* (macOS 13) Support clipboard sharing on Linux with Apple Virtualization when `spice-vdagent` is installed\r\n* (macOS) Fixed an issue changing the boot OS where the incorrect image type is prompted\r\n* (macOS) Perform settings validation when launching an Apple Virtualization VM to ensure selected features are available\r\n* (macOS 12+) Set a machine identifier when launching an Apple Virtualization VM\r\n* (macOS 13) Emulate trackpad on macOS guests with Apple Virtualization\r\n* (macOS) Fixed an issue when a newly created VM will not launch on macOS 11\r\n\r\n## Changes (v4.0.5)\r\n\r\n* Fixed moving an existing VM with Hypervisor enabled to a device on a different architecture. The VM will fallback to TCG and the option to disable hypervisor in settings is allowed. (#4407)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* (iOS) Fixed an issue that prevented external keyboards from working (#4399)\r\n* (iOS) Detect Hypervisor support on jailbroken devices so the option is not inadvertently enabled on non-supported devices\r\n* (iOS) Support Hypervisor on M1 iPad running jailbroken iOS 14.5\r\n\r\n## Changes (v4.0.4)\r\n\r\n* Fixed in issue generating configuration for IDE drives leading to PPC not booting and I/O errors on PC (#4372, #4376, others)\r\n* Moved the SPICE tools download directory to \"GuestSupportTools\" under \"Application Support\" (previously it was just under \"Application Support\")\r\n* Fixed creating a VM with illegal path characters in the name (#4385)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* Wizard: No longer tries to download the Windows guest tools when selecting a non-Windows OS\r\n* (iOS) Enable build with Hypervisor.framework (support limited to M1 iPad)\r\n* (iOS) Fixed a crash when switching display in a window\r\n* (iOS) On jailbroken devices, the memory limit will automatically be increased to the maximum, preventing the Jetsam system from terminating UTM for memory usage\r\n* (iOS) Fixed a regression which caused the home indicator to not be hidden (#4390)\r\n* (iOS) Fixed a regression which caused the cursor to not be captured (#4390)\r\n* (iOS) When switching display, notification handlers are properly cleaned up (example: cursor capture and console on screen keyboard events)\r\n* (iOS) Show the device cursor when VM is paused\r\n* (iOS) Fixed a regression where external keyboard events are not captured\r\n* (iOS) Fixed an error where extraneous stale VM entries show up after the container name changes (#4392)\r\n* (iOS) Fixed a crash on iOS 14 when opening a terminal view due to SwiftTerm handling the colour configuration\r\n* (macOS) Fixed a layout issue of the compress/resize buttons\r\n* (macOS) Forgot to actually enable compression for the drive setting button (#4377)\r\n* (macOS) Fixed some settings layout issue on < macOS 13 (#4374)\r\n\r\n## Changes (v4.0.3)\r\n\r\n* Fixed an issue where changing external drive/shared directory for a QEMU VM -> exit UTM -> reopen UTM and start the VM results in the drive/share not being restored\r\n* Disable changing a VirtFS share from the home window (this is not an supported operation)\r\n* Better detection of UUID collision which addresses an issue where VMs with the same UUID do not show up on the home screen and other VMs show up as duplicates and clicking on any of them results in a freeze\r\n* Fixed floppy drive argument not being correctly generated (#4362)\r\n* Fixed an issue where ejecting an external drive or shared directory does not persist\r\n* Fixed a memory issue when stopping or closing VMs causing UTM to crash\r\n* Fixed a regression where an access error occurs after moving a VM\r\n* Added the ability to download the Windows SPICE tools and drivers automatically (#4364)\r\n* Added support for more than 2 IDE drives in PC emulation\r\n* Restored the setting to turn off blinking cursor (#4296)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Wizard: Reworked some of the UI, text, and file selection\r\n* Wizard: Add option to auto download and mount the SPICE tools to a second CD drive\r\n* Wizard: Fixed an issue where the selected boot image and shared directory was not saved on the new VM\r\n* Wizard: Recommend UUP built ISO over the VHDX by default\r\n* Wizard: New \"confused user\" check will catch trying to mount an \"amd64\" ISO on an \"arm64\" guest or vice versa\r\n* (iOS 16) Use the new NavigationSplitView for a slightly polished look\r\n* (iOS 16) Fixed an issue where the bottom toolbar does not show up (#4325)\r\n* (iOS) Fixed an issue where the file importer was not opening (#4365)\r\n* (iOS 14) Fixed an issue in the settings screen where multiple drives were occupying a single cell\r\n* (iOS 14) Fixed an issue where UTM may crash when adding a drive or hardware\r\n* (macOS) Added the ability to re-open closed windows for a given VM (#4351)\r\n* (macOS) Fixed an issue where restarting a VM results in duplicate windows (#4367)\r\n* (macOS) Save the size of terminal windows (#4296)\r\n* (macOS) Add resize QCOW2 image feature (thanks @stewartsmith)\r\n\r\n## Changes (v4.0.2)\r\n\r\n* Removed \"view.plist\" for host-specific configuration settings (i.e. bookmarks to removable drives and window options) and replaced it with a new \"registry\" that is stored outside of the .utm bundle. Old \"view.plist\" settings and bookmarks will be migrated to the registry on first launch and the file will be deleted from the .utm bundle. For Apple VMs, the bookmarks will no longer be stored in config.plist and the settings will be migrated to the registry as well.\r\n* VirtFS no longer requires SPICE to be enabled (thanks @tie)\r\n* Fixed an issue with PPC VMs not showing 256 colours correctly (#4277)\r\n* Fixed incorrect parsing of CPU flags (#4282)\r\n* Do not save screenshots when running in disposable mode\r\n* Translation: Added Spanish (Latin America) (thanks @JezerM)\r\n* Translation: Added Finnish (thanks @marcusziade)\r\n* Translation: Updated Japanese (thanks @MMP0)\r\n* Translation: Updated Chinese (Simplified) (thanks @ty-yqs)\r\n* Translation: Updated French (thanks @FRtranslator)\r\n* (iOS) Per-display window settings (zoom, position, keyboard visibility, etc) will be stored in the new registry\r\n* (iOS) Prefer JitStreamer over AltJit when both are available (thanks @ktprograms)\r\n* (macOS) Fixed saving removable drives and shared directories for Apple VMs\r\n* (macOS) Fixed missing audio entitlements (#4342)\r\n* (macOS) Fixed QEMULauncher process not terminating when a VM is force quit\r\n* (macOS) Fixed issue selecting text in SwiftTerm (#4297)\r\n\r\n## Changes (v4.0.1)\r\n* Fixed an issue where an UEFI BIOS error was reported when the target does not use UEFI (#4265)\r\n* Added Elementary OS icon (thanks @Unbinilium)\r\n* Updated ja localization (thanks @MMP0)\r\n* Updated fr localization (thanks @FRtranslator)\r\n* Changed the icon for \"Serial\" so it appears on iOS 14 and macOS 11 as well\r\n* Fixed custom icon not showing up for \"legacy\" configurations\r\n* Fixed an error trying to migrate \"legacy\" configuration when \"Images\" does not exist (#4266)\r\n* Fixed USB redirection (#4263)\r\n* (iOS) Fixed a toolbar issue where USB button overflowed on screen.\r\n* (iOS) Fixed resume button not appearing on < iOS 16\r\n* (iOS) Attempt to close the download progress pop-up after download completes (#4261)\r\n* (iOS) \"Open\" popover refuses to show up again after swiping down (#4260)\r\n* (iOS) Hide \"Add\" text on iOS 14 settings\r\n* (iOS) Fixed crash on iOS 14 settings when attempting to use the picker (#4270)\r\n* (iOS) Fixed an issue on iOS 14 where picker selection was being reset\r\n* (iOS) Fixed an issue where the USB icon is stuck on busy after a device disconnects\r\n* (macOS) Fixed a crash trying to change shared directory for Apple VM (#4271)\r\n* (macOS) Wizard created invalid target configuration for virtualized targets (#4274)\r\n\r\n## Changes (v4.0.0)\r\n* USB redirection support in terminal mode\r\n* Configuration file format changed, newly saved VMs will not be compatible with older versions of UTM\r\n* Newly imported disk images will be converted to QCOW2 automatically\r\n* Settings: new layout with support for multiple {Display, Serial, Network, Sound} devices (#3585)\r\n* Support multiple displays (#220)\r\n* Added Japanese localization (thanks @MMP0)\r\n* Support adding PTTY (macOS only), TCP client, and TCP server serial connections for QEMU machines (address should show up in the home screen) (#3546)\r\n* Support headless display (remove all displays and built-in serial ports in the settings) (#2280)\r\n* Support redirecting QEMU monitor and GDB stub to a serial port\r\n* Support zstd compression for QCOW2 images and use zstd as default for image compression (#4211)\r\n* Update ANGLE (GL backend) to latest git commit\r\n* Added French localization (thanks @FRtranslator)\r\n* Fixed microphone recording silence (#219)\r\n* Fixed a crash when attempting to delete a QEMU additional argument\r\n* Option in VM settings to use virtfs/9pfs for file sharing (#2184)\r\n* Option in VM settings to change VGA RAM size (#4034)\r\n* Option in VM settings to enable virtio-balloon driver (#4136)\r\n* Invert mouse scrolling is now a global setting rather than a per-vm configuration option\r\n* (iOS) Replaced hterm.js with SwiftTerm for terminal mode (#3473)\r\n* (iOS) Attach to JitStreamer (set IP address in Settings app and UTM will try to connect automatically on launch) (thanks @ktprograms)\r\n* (iOS) Automatically resize the display to fit the screen when the resolution changes if the resize toolbar option is used\r\n* (iOS) Reimplemented the USB and Drives menu with a better UI\r\n* (iOS) On iPadOS 16, show the menu bar when holding Cmd on the keyboard. On previous versions, an on-screen help will show supported commands\r\n* (iOS) Improved audio handling including: output when on silence, mixing with other apps, working when both recording and outputting (including with another app) (#3996)\r\n* (iOS) Added a global setting to always prefer the built-in microphone to a bluetooth microphone\r\n* (macOS) Fixed running from shortcut in Apple VMs (no longer need to re-import after each launch)\r\n* (macOS) Improved IPSW selection interface and support drag and drop (thanks @pointum)\r\n* (macOS) Fixed running unsigned builds\r\n* (macOS) Removed some deprecated global settings\r\n* (macOS) Fixed an error when trying to download an IPSW and the Caches directory does not exist (thanks @LostInCompilation)\r\n* (macOS) Fixed an issue where a VM could be started twice if the home screen's toolbar is used leading to data corruption (#4166)\r\n* (macOS 13+) Boot into recoveryOS (to disable SIP, etc) by right clicking on the VM and selecting \"Run in recovery...\" (#3526)\r\n* (macOS 13+) Option in VM settings to enable Rosetta for x86_64 emulation (#4100)\r\n* (macOS 13+) Option in VM settings to enable clipboard sharing (SPICE support needed on the guest) (#4121)\r\n* (macOS 13+) GUI display for Linux VMs (#4120)\r\n* (macOS 13+) Add removable drives, will show up as USB mass storage\r\n\r\n## Issues\r\nPlease check the full list on [Github][2] and help report any bug you find that is not listed.\r\n\r\n## Installation\r\n\r\n* [iOS](https://docs.getutm.app/installation/ios/)\r\n* [macOS](https://docs.getutm.app/installation/macos/)\r\n\r\n| File | Description | Installation | JIT | Hypervisor | USB |\r\n|------|------------|--------------|-----|-----------|-----|\r\n| UTM.deb | Jailbroken iOS version | Open in Cydia, dpkg, or Sileo | Yes | Yes(1) | Yes |\r\n| UTM.dmg | macOS version | Mounting and copying UTM.app to /Applications | Yes | Yes | Yes |\r\n| UTM.ipa | Non-jailbroken iOS version (sideloading) | AltStore, etc (see guide) | Yes(2) | No | No |\r\n| UTM.HV.ipa | Non-jailbroken iOS version (TrollStore) | TrollStore | Yes(2) | Yes(1) | Yes |\r\n| UTM.SE.ipa | Non-jailbroken iOS version (sideloading) | AltStore, enterprise signing, etc | No | No | No |\r\n\r\n1. Hypervisor on iOS requires an M1 iPad.\r\n2. Enabling JIT may require a separate JIT enabler such as [Jitterbug][3] or Jitstreamer.\r\n\r\n[1]: https://getutm.app/install/\r\n[2]: https://github.com/utmapp/UTM/issues\r\n[3]: https://github.com/osy/Jitterbug",
                     "size": 153976253,
                     "version": "4.0.9"
                 },
                 {
@@ -917,120 +995,185 @@
                 }
             ]
         },
         {
             "appID": "org.provenance-emu.provenance",
             "bundleIdentifier": "org.provenance-emu.provenance",
             "developerName": "Joe Mattiello",
-            "downloadURL": "https://provenance-builds.s3-us-east-2.amazonaws.com/apps/2.1.1/Provenance-iOS.ipa",
             "iconURL": "https://provenance-emu.com/images/icons/icon.512x512.png",
             "localizedDescription": "Provenance is a multi-system emulator frontend for a plethora of retro gaming systems. You can keep all your games in one place, display them with cover art, and play to your heart's content.\n\nSystems Supported:\n\n\u2022 Atari\n  - 2600\n  - 5200\n  - 7800\n  - Lynx\n  - Jaguar\n\u2022 Bandai\n  - WonderSwan / WonderSwan Color\n\u2022 NEC\n  - PC Engine / TurboGrafx-16 (PCE/TG16)\n  - PC Engine Super CD-ROM\u00b2 System / TurboGrafx-CD\n  - PC Engine SuperGrafx\n  - PC-FX\n\u2022 Nintendo\n  - Nintendo Entertainment System / Famicom (NES/FC)\n  - Famicom Disk System\n  - Super Nintendo Entertainment System / Super Famicom (SNES/SFC)\n  - Game Boy / Game Boy Color (GB/GBC)\n  - Virtual Boy\n  - Game Boy Advance (GBA)\n  - Pok\u00e9mon mini\n\u2022 Sega\n  - SG-1000\n  - Master System\n  - Genesis / Mega Drive\n  - Game Gear\n  - CD / MegaCD\n  - 32X\n\u2022 SNK\n  - Neo Geo Pocket / Neo Geo Pocket Color\n\u2022 Sony\n  - PlayStation (PSX/PS1)",
             "name": "Provenance EMU",
-            "permissions": [
-                {
-                    "type": "camera",
-                    "usageDescription": "Used for album artwork."
-                },
-                {
-                    "type": "photos",
-                    "usageDescription": "Provenance can set custom artworks from your photos or save screenshots to your photos library."
-                },
-                {
-                    "type": "music",
-                    "usageDescription": "This will let you play your imported music on Spotify."
-                },
-                {
-                    "type": "bluetooth",
-                    "usageDescription": "Provenance uses Bluetooth to support game controllers."
-                },
-                {
-                    "type": "background-fetch",
-                    "usageDescription": "Provenance can continue running while in the background."
-                },
-                {
-                    "type": "background-audio",
-                    "usageDescription": "Provenance can continue playing game audio while in the background."
-                }
-            ],
             "screenshotURLs": [
-                "https://provenance-emu.com/blog/2022/02/15/release-2.1.0/images/ios-menu-icons.jpg",
-                "https://provenance-emu.com/blog/2022/02/15/release-2.1.0/images/tvos-settings.jpg",
-                "https://provenance-emu.com/blog/2022/02/15/release-2.1.0/images/ios-spotlight-mk.jpg",
-                "https://provenance-emu.com/blog/2022/02/15/release-2.1.0/images/n64-ios-newlayout.jpg",
-                "https://provenance-emu.com/blog/2022/02/15/release-2.1.0/images/ios-coreoptions-mednafen.jpg",
-                "https://provenance-emu.com/blog/2022/02/15/release-2.1.0/images/ios-coreoptions-genesis.jpg"
+                "https://provenance-emu.com/blog/2022/12/09/release-2.2.0/images/IMG_2306.jpg",
+                "https://provenance-emu.com/blog/2022/12/09/release-2.2.0/images/IMG_2307.jpg",
+                "https://provenance-emu.com/blog/2022/12/09/release-2.2.0/images/IMG_2308.jpg",
+                "https://provenance-emu.com/blog/2022/12/09/release-2.2.0/images/IMG_2309.jpg",
+                "https://provenance-emu.com/blog/2022/12/09/release-2.2.0/images/IMG_2310.jpg",
+                "https://provenance-emu.com/blog/2022/12/09/release-2.2.0/images/IMG_2311.jpg",
+                "https://provenance-emu.com/blog/2022/12/09/release-2.2.0/images/IMG_2312.jpg"
             ],
-            "size": 36120321,
             "subtitle": "Multi-emulator frontend for iOS & tvOS",
             "tintColor": "#1c7cf3",
-            "version": "2.1.1",
-            "versionDate": "2022-06-15T12:00:00-05:00",
-            "versionDescription": "PSX controller fixes, fceux update, SwiftUI updates.",
             "versions": [
                 {
+                    "date": "2022-12-30T00:01:00-05:00",
+                    "downloadURL": "https://provenance-builds.s3-us-east-2.amazonaws.com/apps/2.2.1.beta1/Provenance.ipa",
+                    "localizedDescription": "Pre-release of Play!, Dolphin and PPSSPP. JIT Required or cores will crash.",
+                    "sha256": "48b834e58724a07b16a8f951ff8983c6ca7088f85d5f480c3dfe04530c915f9c",
+                    "size": 77010038,
+                    "version": "2.2.1"
+                },
+                {
+                    "date": "2022-12-30T00:01:00-05:00",
+                    "downloadURL": "https://provenance-builds.s3-us-east-2.amazonaws.com/apps/2.2.1.beta1/Provenance.ipa",
+                    "localizedDescription": "Pre-release of Play!, Dolphin and PPSSPP. JIT Required or cores will crash.",
+                    "size": 33978209,
+                    "version": "2.2.1.beta.1"
+                },
+                {
+                    "date": "2022-12-09T00:01:00-05:00",
+                    "downloadURL": "https://provenance-builds.s3-us-east-2.amazonaws.com/apps/2.2.0/Provenance.ipa",
+                    "localizedDescription": "Many bug fixes, SwiftUI additions, new cores, new features and more. See GitHub changelog for more info.",
+                    "size": 33978209,
+                    "version": "2.2.0"
+                },
+                {
                     "date": "2022-06-15T12:00:00-05:00",
                     "downloadURL": "https://provenance-builds.s3-us-east-2.amazonaws.com/apps/2.1.1/Provenance-iOS.ipa",
                     "localizedDescription": "PSX controller fixes, fceux update, SwiftUI updates.",
                     "size": 36120321,
                     "version": "2.1.1"
                 }
             ]
         },
         {
             "appID": "com.flyinghead.Flycast",
             "beta": false,
             "bundleIdentifier": "com.flyinghead.Flycast",
             "developerName": "Flyinghead",
-            "downloadURL": "https://github.com/flyinghead/flycast/releases/download/v2.0/Flycast-2.0.ipa",
             "iconURL": "https://github.com/flyinghead/flycast/raw/master/shell/linux/flycast.png",
             "localizedDescription": "Flycast is a multi-platform Sega Dreamcast, Naomi and Atomiswave emulator derived from reicast.\nInformation about configuration and supported features can be found on TheArcadeStriker's [flycast wiki](https://github.com/TheArcadeStriker/flycast-wiki/wiki).",
             "name": "Flycast",
             "screenshotURLs": [
                 "https://i.imgur.com/47KjD5a.png",
                 "https://i.imgur.com/MfhD1h1.png",
                 "https://i.imgur.com/wO88IVP.png"
             ],
-            "size": 14716842,
             "subtitle": "Dreamcast, Naomi and Atomiswave emulator.",
             "tintColor": "9b54fd",
-            "version": "v2.0",
-            "versionDate": "2022-08-29T11:21:00+02:00",
-            "versionDescription": "This update brings Naomi 2 support",
             "versions": [
                 {
+                    "date": "2023-02-16T11:24:00+01:00",
+                    "downloadURL": "https://github.com/flyinghead/flycast/releases/download/V2.1/Flycast-2.1.ipa",
+                    "localizedDescription": "Full framebuffer emulation and texture upscaling on iOS.",
+                    "sha256": "ce84e20531ec2c4c283c860a6646bc6d113b476fff0e45da3912fd0d86f93644",
+                    "size": 14904310,
+                    "version": "v2.1"
+                },
+                {
                     "date": "2022-08-29T11:21:00+02:00",
                     "downloadURL": "https://github.com/flyinghead/flycast/releases/download/v2.0/Flycast-2.0.ipa",
                     "localizedDescription": "This update brings Naomi 2 support",
                     "size": 14716842,
                     "version": "v2.0"
                 }
             ]
         },
         {
             "appID": "eu.pokemmo.client",
             "beta": false,
             "bundleIdentifier": "eu.pokemmo.client",
             "developerName": "PokeMMO",
-            "downloadURL": "https://dl.pokemmo.com/download/PokeMMO-Client.ipa?hash=a333c880",
             "iconURL": "https://pokemmo.com/build/images/altstore.ba9b8a4e.png",
             "localizedDescription": "PokeMMO is a free to play mmorpg, come join a growing community as you level up and discover new monsters. Available now on PC, Android, iOS, Mac, and Linux.",
             "name": "PokeMMO",
             "screenshotURLs": [
                 "https://pokemmo.com/build/images/screenshot/c.f3968293.png",
                 "https://pokemmo.com/build/images/screenshot/b.3a233486.png",
                 "https://pokemmo.com/build/images/screenshot/d.4080dd9c.png",
                 "https://pokemmo.com/build/images/screenshot/e.ed0aa85b.png",
                 "https://pokemmo.com/build/images/screenshot/a.debf11f5.png"
             ],
-            "size": 77411824,
             "tintColor": "73ACE2",
-            "version": "21623",
-            "versionDate": "2022-11-02T16:37:28+00:00",
             "versions": [
                 {
+                    "date": "2023-05-18T11:53:56+00:00",
+                    "downloadURL": "https://dl.pokemmo.com/download/PokeMMO-Client.ipa?hash=46f423b6",
+                    "sha256": "46f423b6e51291c1caf3aed83e3548dc4cdee93060c3599d23996d4e6fc85c58",
+                    "size": 93158829,
+                    "version": "22920"
+                },
+                {
+                    "date": "2023-05-05T12:14:16+00:00",
+                    "downloadURL": "https://dl.pokemmo.com/download/PokeMMO-Client.ipa?hash=ade247a9",
+                    "sha256": "ade247a9c7da7e67d6dbdb13b99af9b053a07c0c6df74db0629af210beb6608f",
+                    "size": 93155840,
+                    "version": "22865"
+                },
+                {
+                    "date": "2023-05-05T08:19:49+00:00",
+                    "downloadURL": "https://dl.pokemmo.com/download/PokeMMO-Client.ipa?hash=547b93d7",
+                    "sha256": "547b93d704e562ebf57202406eae35eb60aa046e7e0cda882fb3d3464b0db9f8",
+                    "size": 93148485,
+                    "version": "22855"
+                },
+                {
+                    "date": "2023-04-29T06:11:12+00:00",
+                    "downloadURL": "https://dl.pokemmo.com/download/PokeMMO-Client.ipa?hash=dc6bb232",
+                    "sha256": "dc6bb232f97f2f17edcd94d289a2d97570694f195ec243a14ab343f7bc19c480",
+                    "size": 93878505,
+                    "version": "22760"
+                },
+                {
+                    "date": "2023-04-29T05:14:06+00:00",
+                    "downloadURL": "https://dl.pokemmo.com/download/PokeMMO-Client.ipa?hash=75230e15",
+                    "sha256": "75230e15e1b3fdc362a707be9dc74e2206f15ad2c5f2528617cf8337dbc09629",
+                    "size": 93879584,
+                    "version": "22758"
+                },
+                {
+                    "date": "2023-04-28T05:18:14+00:00",
+                    "downloadURL": "https://dl.pokemmo.com/download/PokeMMO-Client.ipa?hash=6a501c67",
+                    "sha256": "6a501c67e38fa63698119ad9dfbcd60dba5e9b13277bab024d8d635a452dfb33",
+                    "size": 93871750,
+                    "version": "22698"
+                },
+                {
+                    "date": "2023-04-28T04:16:15+00:00",
+                    "downloadURL": "https://dl.pokemmo.com/download/PokeMMO-Client.ipa?hash=e671771d",
+                    "sha256": "e671771d4cb455bb7c9879aac63ae7cb20008871030b8ad699ec731f69780291",
+                    "size": 93877962,
+                    "version": "22693"
+                },
+                {
+                    "date": "2023-03-27T16:43:48+00:00",
+                    "downloadURL": "https://dl.pokemmo.com/download/PokeMMO-Client.ipa?hash=73c73a82",
+                    "sha256": "73c73a82d759f6554315859b4cb35c59752e497ed124d1b1563e30eb3d25c370",
+                    "size": 143553661,
+                    "version": "22217"
+                },
+                {
+                    "date": "2023-01-24T02:06:46+00:00",
+                    "downloadURL": "https://dl.pokemmo.com/download/PokeMMO-Client.ipa?hash=6d42df75",
+                    "size": 143552701,
+                    "version": "22215"
+                },
+                {
+                    "date": "2022-12-29T08:16:55+00:00",
+                    "downloadURL": "https://dl.pokemmo.com/download/PokeMMO-Client.ipa?hash=00ebe475",
+                    "size": 142869724,
+                    "version": "21958"
+                },
+                {
+                    "date": "2022-12-27T01:40:11+00:00",
+                    "downloadURL": "https://dl.pokemmo.com/download/PokeMMO-Client.ipa?hash=d87b4536",
+                    "size": 142874491,
+                    "version": "21931"
+                },
+                {
                     "date": "2022-11-02T16:37:28+00:00",
                     "downloadURL": "https://dl.pokemmo.com/download/PokeMMO-Client.ipa?hash=a333c880",
                     "size": 77411824,
                     "version": "21623"
                 },
                 {
                     "date": "2022-11-01T21:41:25+00:00",
@@ -1095,20 +1238,334 @@
                 {
                     "date": "2022-07-01T01:51:22+00:00",
                     "downloadURL": "https://dl.pokemmo.com/download/PokeMMO-Client.ipa?hash=9c960d8a",
                     "size": 76575373,
                     "version": "20726"
                 }
             ]
+        },
+        {
+            "appID": "com.litritt.ignited",
+            "bundleIdentifier": "com.litritt.ignited",
+            "developerName": "Lit Development",
+            "iconURL": "https://github.com/Lit-Development/Assets/blob/main/apps/delta-ignited/icon-180.png?raw=true",
+            "localizedDescription": "Ignited is an overhaul of Delta, an all-in-one emulator for iOS.\n\nFEATURES\n\nSupported Game Systems\n\u2022 Nintendo Entertainment System\n\u2022 Super Nintendo Entertainment System\n\u2022 Sega Genesis\n\u2022 Nintendo 64\n\u2022 Game Boy (Color)\n\u2022 Game Boy Advance\n\u2022 Nintendo DS\n\nController Support\n\u2022 Supports PS4, PS5, Xbox One S, Xbox Series X, and MFi game controllers.\n\u2022 Supports bluetooth (and wired) keyboards, as well as the Apple Smart Keyboard.\n\u2022 Completely customize button mappings on a per-system, per-controller basis.\n\u2022 Map buttons to special \"Quick Save\", \"Quick Load,\" and \"Fast Forward\" actions.\n\nSave States\n\u2022 Save and load save states for any game from the pause menu.\n\u2022 Lock save states to prevent them from being accidentally overwritten.\n\u2022 Automatically makes backup save states to ensure you never lose your progress.\n\u2022 Support for \"Quick Saves,\" save states that can be quickly saved/loaded with a single button press (requires external controller or supported skin).\n\u2022 Save State Rewind - Rolling save states that can be rewound to for up to 2 minutes. Configurable interval. (Currently disabled)\n\nCheats\n\u2022 Supports various types of cheat codes for each supported system:\n\u2022 NES: Game Genie\n\u2022 SNES: Game Genie, Pro Action Replay\n\u2022 N64: GameShark\n\u2022 GBC: Game Genie, GameShark\n\u2022 GBA: Action Replay, Code Breaker, GameShark\n\u2022 DS: Action Replay\n\nDelta Sync\n\u2022 Sync your games, game saves, save states, cheats, controller skins, and controller mappings between devices.\n\u2022 View version histories of everything you sync and optionally restore them to earlier versions.\n\u2022 Supports both Google Drive and Dropbox.\n\nCustom Controller Skins\n\u2022 Beautiful built-in controller skins for all systems.\n\u2022 Import controller skins made by others, or even make your own to share with the world!\n\nHold Button\n\u2022 Choose buttons for Delta to hold down on your behalf, freeing up your thumbs to press other buttons instead.\n\u2022 Perfect for games that typically require one button be held down constantly (ex: run button in Mario games, or the A button in Mario Kart).\n\nFast Forward\n\u2022 Speed through slower parts of games by running the game much faster than normal.\n\u2022 Easily enable or disable from the pause menu, or optionally with a mapped button on an external controller.\n\n3D/Haptic Touch\n\u2022 Use 3D or Haptic Touch to \"peek\" at games, save states, and cheat codes.\n\u2022 App icon shortcuts allow quick access to your most recently played games, or optionally customize the shortcuts to always include certain games.\n\nGame Artwork\n\u2022 Automatically displays appropriate box art for imported games.\n\u2022 Change a game's artwork to anything you want, or select from the built-in game artwork database.\n\nMisc.\n\u2022 Gyroscope support (WarioWare: Twisted! only)\n\u2022 Microphone support (DS only)\n\u2022 Support for delta:// URL scheme to jump directly into a specific game.\n\n**Ignited and Lit Development are in no way affiliated with Nintendo. The name \"Nintendo\" and all associated game console names are registered trademarks of Nintendo Co., Ltd.**",
+            "name": "Ignited",
+            "screenshotURLs": [
+                "https://github.com/Lit-Development/Assets/blob/main/apps/delta-ignited/theme.jpg?raw=true",
+                "https://github.com/Lit-Development/Assets/blob/main/apps/delta-ignited/library.jpg?raw=true",
+                "https://github.com/Lit-Development/Assets/blob/main/apps/delta-ignited/game.jpg?raw=true",
+                "https://github.com/Lit-Development/Assets/blob/main/apps/delta-ignited/speed.jpg?raw=true",
+                "https://github.com/Lit-Development/Assets/blob/main/apps/delta-ignited/updates.jpg?raw=true",
+                "https://github.com/Lit-Development/Assets/blob/main/apps/delta-ignited/settings.jpg?raw=true"
+            ],
+            "subtitle": "Retro games meet modern design.",
+            "tintColor": "FF6A00",
+            "versions": [
+                {
+                    "date": "2023-06-04T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.4.3/Ignited.ipa",
+                    "localizedDescription": "Updates\n\u2022Adds an option for custom touch overlay color\n\u2022Creates a new feature section called Games Collection\n\u2022Moves settings previously found in Game Artwork Customization into separate sections within the Games Collection feature set\n\u2022Makes Favorites features respect whether the feature is actually enabled\n\nBugfixes\n\u2022Fixes lag when changing settings with animated artwork in the background\n\u2022Fixes animated artwork losing transparency when downsampling",
+                    "sha256": "87cd927aca7eceeafe72f9862b837c9ca0a86893fb9c958990d2d61aa2b05314",
+                    "size": 50355653,
+                    "version": "1.4.3"
+                },
+                {
+                    "date": "2023-06-03T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.4.2/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022Quick Settings\n  \u2022Quick access to game options and actions: screenshot, save, load, volume, game speed, palettes\n  \u2022Accessible from a controller/skin button as well as the pause menu\n\nUpdates\n\u2022New options for game title size and max lines, available in User Interface Features -> Game Artwork Customization\n\nBugfixes\n\u2022Fixes crash on iPad when resolving sync merge conflicts\n\u2022Fixes accidentally deleting Games directory during sync in rare circumstances",
+                    "sha256": "9f312809ecc7c048e2c6f050b08735af75e91d979876d8149ff942bfae85cc02",
+                    "size": 50355653,
+                    "version": "1.4.2"
+                },
+                {
+                    "date": "2023-05-14T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.4.1/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Adds an option to reset game artwork to the one provided by the games database\n\u2022 Adds a power user option to reset artwork for every game at once\n\nBugfixes\n\u2022 Fixes cancelling some pause menu popups causing the game to freeze\n\u2022 Fixes incorrect checkmarks next to selected palette for sprite 1 and 2\n\u2022 Fixes preview save state being overwritten by auto save state",
+                    "sha256": "203eff55dc5ef681e109ad5ee42ba51b9cd67340a1ea74e58d80dbe082732888",
+                    "size": 50355653,
+                    "version": "1.4.1"
+                },
+                {
+                    "date": "2023-05-13T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.4/Ignited.ipa",
+                    "localizedDescription": "Updates\n\u2022 Settings page has been completely revamped and reorganized\n  \u2022 Many existing features received improvements as they were moved\n\nNew Features\n\u2022 Game Boy color palettes\n  \u2022 Several built in palettes and 3 user customizable palettes\n  \u2022 Both the main and sprite palettes can be changed, allowing for unique palettes never before possible\n\u2022 Custom Theme Color\n  \u2022 Choose your own color to use for the app accent color\n\u2022 Favorite Games\n  \u2022 Games can be favorited, with options to highlight and sort them to the top of the games list\n\u2022 Game Sorting\n  \u2022 You can now sort games A-Z, Z-A, most recently played, and least recently played\n\u2022 Animated Game Artwork\n  \u2022 Support for short animated GIFs as your game artwork, with options for animation pause and speed\n\nBugfixes\n\u2022 Burnt a bunch of bugs",
+                    "sha256": "338f4434a122fa7492d363f079ba45c669528a52db637685acea52f200ea89c2",
+                    "size": 50355653,
+                    "version": "1.4"
+                },
+                {
+                    "date": "2023-04-28T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.3.0/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Skin Debug Device - Switch to another device type when debugging a skin, useful for testing skins on devices you don't own\n\nUpdates\n\u2022 Adds toasts notifications for more actions\n\nBugfixes\n\u2022 Now creates an auto save state when saving in-game, fixes old autosaves overwriting game data when loaded\n\u2022 Fixes the Resume button not working with auto-load save states disabled\n\u2022 Fixes the pause menu not fully showing in landscape with 2 rows of buttons",
+                    "sha256": "2cf7b2c705ea04baf8352679966644f18ce729e035648d83fdf08bae52e330df",
+                    "size": 50355653,
+                    "version": "1.3.0"
+                },
+                {
+                    "date": "2023-04-23T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.2.10/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 New Screenshot options - Save to Files, Save to Photos, Image Scale\n\nUpdates\n\u2022 Forced light status bar during gameplay\n\u2022 Updated licenses page formatting\n\u2022 Reordered pause menu buttons and adjusted spacing to 4 items per row\n\nBugfixes\n\u2022 Adjusted settings slider labels to fit with bold system text\n\u2022 Removed unimplemented swipable page control",
+                    "sha256": "c908d8b0c4fbf7b7f979723fc85222c702623c34c0501061bef675ceab4b40b4",
+                    "size": 50355653,
+                    "version": "1.2.10"
+                },
+                {
+                    "date": "2023-04-18T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.2.9/Ignited.ipa",
+                    "localizedDescription": "Updates\n\u2022 Added page for Lit Patrons shoutout\n\u2022 Changed rewind to be disabled by default\n\nBugfixes\n\u2022 Fixed a crash when toggling clicky haptics\n\u2022 Removed unsupported file extensions on GPGX",
+                    "sha256": "5cec577a5aec4529c76780a42741e89241366e4c062f8e54d9c0345203440b59",
+                    "size": 50355653,
+                    "version": "1.2.9"
+                },
+                {
+                    "date": "2023-04-16T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.2.8/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Added toggle to show or hide the status bar while in-game\n\u2022 Added\n\u2022 Resource Links section to settings\n\u2022 Added Rom Patcher JS and DS Save Converter links\n\nUpdates\n\u2022 Added remaining file extensions for all systems supported by the Genesis Plus GX core",
+                    "sha256": "122e3dcd212e39b4a7d5c2927ec027efb7b31cbc4e11b7a489bbc296d86ba5d1",
+                    "size": 50355653,
+                    "version": "1.2.8"
+                },
+                {
+                    "date": "2023-04-15T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.2.7/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Added options to toggle game artwork borders, shadows, and rounded corners\n\nUpdates\n\u2022 Added confirmation popup to advanced settings\n\u2022 Game screenshots are now scaled up by 5x before being saved",
+                    "sha256": "7bc39a5cb959649c715d77787ba395f63dc8a775a4ee8f0d0561b6253f1b8ac8",
+                    "size": 50355653,
+                    "version": "1.2.7"
+                },
+                {
+                    "date": "2023-04-14T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.2.5/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Game Screenshots - save a screenshot of the game screen to your photos with a pause menu item or controller skin button",
+                    "size": 50355653,
+                    "version": "1.2.6"
+                },
+                {
+                    "date": "2023-04-12T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.2.5/Ignited.ipa",
+                    "localizedDescription": "Bugfixes\n\u2022 Fixed importing game saves with auto-load save state enabled\n\nNew Features\n\u2022 Added advanced setting to clear auto save states from every game",
+                    "size": 50355653,
+                    "version": "1.2.5"
+                },
+                {
+                    "date": "2023-04-11T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.2.4/Ignited.ipa",
+                    "localizedDescription": "Bugfixes\n\u2022 Disabled auto-load save on DSi Home Screen\n\u2022 Removed cheats, save, load, and rewind pause menu items from DSi Home Screen\n\u2022 Removed cheats from DS Home Screen",
+                    "size": 50355653,
+                    "version": "1.2.4"
+                },
+                {
+                    "date": "2023-04-10T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.2.3/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Updates screen will now be shown once per update at launch\n\nUpdates\n\u2022 Updates screen now includes dates for all versions",
+                    "size": 50355653,
+                    "version": "1.2.3"
+                },
+                {
+                    "date": "2023-04-09T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.2.2/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Game Volume - Change the game volume relative to your device volume\n\u2022 Toggle for whether game audio should play when other audio is playing in the background\n\nUpdates\n\u2022 Updated OpenVGDB database",
+                    "size": 50355653,
+                    "version": "1.2.2"
+                },
+                {
+                    "date": "2023-04-09T00:00:08-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.2.1/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Audio Button Feedback - option to play a sound when a controller skin input is pressed\n\nUpdates\n\u2022 Raise minimum iOS to 14.0 - Removed all legacy code\n\nBugfixes\n\u2022 Fixed laggy sliders in settings that could crash the app when paused",
+                    "size": 50355653,
+                    "version": "1.2.1"
+                },
+                {
+                    "date": "2023-04-08T00:00:08-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.2.0/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Touch Overlays - Get visual feedback about what buttons are currently pressed\n\u2022 Options for size, opacity, and color of touch overlays\n\u2022 Resume Button added to game collection screen beside the page dots\n\nBugfixes\n\u2022 Fixed controller skins losing transparency on device rotation",
+                    "size": 50355653,
+                    "version": "1.2.0"
+                },
+                {
+                    "date": "2023-04-06T00:00:08-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.1.4/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Re-enabled Save State Rewind - Disabled on GBC to prevent crashes with gambette\n\nUpdates\n\u2022 Added new Advanced section to settings - Moved alt skin and debug toggles there\n\u2022 Custom fast forward speed is now default - Toggle removed\n\nBugfixes\n\u2022 Fixed the Show with Controller settings not working on DS",
+                    "size": 50355653,
+                    "version": "1.1.4"
+                },
+                {
+                    "date": "2023-04-02T00:00:08-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.1.3/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Added option for clicky haptic feedback - A more rigid haptic impulse will be sent on both button press and release\n\u2022 Added slider for haptic feedback strength",
+                    "size": 50355653,
+                    "version": "1.1.3"
+                },
+                {
+                    "date": "2023-04-02T00:00:08-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.1.2/Ignited.ipa",
+                    "localizedDescription": "WARNING\n\u2022 This update uses a new bundleID with my domain. It will never change again after this point. Installing will not overwrite your old app. You will need to use Sync or manually transfer data to the new app. I apologize for any inconvenience this causes.\n\nNew Features\n\u2022 Made auto save states syncable\n\nUpdates\n\u2022 Made the restart game button available to skins and controllers\n\u2022 Made the current game highlighting stand out more\n\nBugfixes\n\u2022 Fixed last unthemed elements buried in settings",
+                    "size": 50355653,
+                    "version": "1.1.2"
+                },
+                {
+                    "date": "2023-04-02T00:00:02-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.1.1/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Added a toggle to automatically load the last auto save when launching a game\n\u2022 Added toggle to enabled/disabled in-game toast notifications\n\nUpdates\n\u2022 Removed the Resume Game prompt from the game selection screen\n\u2022 Added a Restart Game pause menu button\n\u2022 Updated toast notification logic to prevent multiple toasts being shown at once",
+                    "size": 50355653,
+                    "version": "1.1.1"
+                },
+                {
+                    "date": "2023-04-02T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.1.0/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Added a toggle to automatically load the last auto save when launching a game\n\u2022 Added toggle to enabled/disabled in-game toast notifications\n\nUpdates\n\u2022 Removed the Resume Game prompt from the game selection screen\n\u2022 Added a Restart Game pause menu button",
+                    "size": 50355653,
+                    "version": "1.1.0"
+                },
+                {
+                    "date": "2023-04-01T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.0.2/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Added color highlighting to currently running game\n\nUpdates\n\u2022 Artwork spacing is now dynamic like the size\n\nBugfixes\n\u2022 Fixed some artwork bugs caused by resizing",
+                    "size": 50355653,
+                    "version": "1.0.2"
+                },
+                {
+                    "date": "2023-03-30T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Ignited/releases/download/v1.0.1/Ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 App Theming - Choose from a variety of colors to change the tint and app icon of Ignited. Emulate in your own style!\n\nUI Updates\n\u2022 Album artwork now has rounded corners, contrasting borders, and a drop shadow\n\u2022 Can now change the artwork size between small, medium, and large\n\u2022 Default box-art now features the cartridge of their respective system\n\nChanges\n\u2022 Custom fast-forward is enabled by default\n\u2022 Default speed changed to 4x\n\u2022 Removed 4x from unsafe speeds",
+                    "size": 50355653,
+                    "version": "1.0.1"
+                },
+                {
+                    "date": "2023-03-18T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Delta-Ignited/releases/download/v0.7.1/Ignited.ipa",
+                    "localizedDescription": "Changes\n\u2022 Alternate Skin pause menu item now only shows is the current skin supports it\n\u2022 Debug Mode pause menu item now only shows if the current skin's debug property is set to true, or debug mode is manually enabled in settings\n\u2022 Reordered save state menu sections. General at the top and Quick/Auto at the bottom\n\u2022 Rebrand to from Delta Ignited to just Ignited",
+                    "size": 50758248,
+                    "version": "0.7.1"
+                },
+                {
+                    "date": "2023-03-18T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Delta-Ignited/releases/download/v0.7.0/delta-ignited.ipa",
+                    "localizedDescription": "New Feature\n\u2022 AltSkin - Alternate appearances for skins\n\u2022 Options to show skins with a controller connected\n\u2022 Access to skin debug mode in-app\n\u2022 In-game toast notifications for various actions\n\nChanges\n\u2022 Updated settings section footers\n\u2022 Added Alternate Skin and Debug Mode options to pause menu",
+                    "size": 50760528,
+                    "version": "0.7.0"
+                },
+                {
+                    "date": "2023-03-11T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Delta-Ignited/releases/download/v0.6.3/delta-ignited.ipa",
+                    "localizedDescription": "New Feature\n\u2022 Access custom fast forward speeds from in-game menu\n\nChanges\n\u2022 Make users accept a warning prompt to access 4x and faster speeds\n\u2022 Add 150% speed setting\n\u2022 Game will auto-save on every fast forward activation\n\u2022 Number of auto-saves increased from 2 to 4",
+                    "size": 50627697,
+                    "version": "0.6.3"
+                },
+                {
+                    "date": "2023-03-05T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Delta-Ignited/releases/download/v0.6.2/delta-ignited.ipa",
+                    "localizedDescription": "New Feature\n\u2022 OTA Installation for patrons\n\u2022 In-App Update Changelog - View all updates from the settings\n\nChanges\n\u2022 Change formatting of updates screen\n\u2022 Move updates to its own section in settings\n\u2022 Fix controller skin previews not showing for standard size iPhones",
+                    "size": 50627697,
+                    "version": "0.6.2"
+                },
+                {
+                    "date": "2023-03-03T00:00:12-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Delta-Ignited/releases/download/v0.6.1/delta-ignited.ipa",
+                    "localizedDescription": "New Feature\n\u2022 In-App Update Changelog - View all updates from the settings\n\nChanges\n\u2022 Change formatting of updates screen\n\u2022 Move updates to its own section in settings",
+                    "size": 50743252,
+                    "version": "0.6.1"
+                },
+                {
+                    "date": "2023-03-03T00:00:10-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Delta-Ignited/releases/download/v0.6.0/delta-ignited.ipa",
+                    "localizedDescription": "New Feature\n\u2022 In-App Update Changelog - View all updates from the settings",
+                    "size": 50742803,
+                    "version": "0.6.0"
+                },
+                {
+                    "date": "2023-03-03T00:00:00-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Delta-Ignited/releases/download/v0.5.3/delta-ignited.ipa",
+                    "localizedDescription": "New Feature\n\u2022 Controller Skin Previews - Supports showing a preview image in settings instead of a bare skin image\n\nChanges\n\u2022 Update local multiplayer settings logic\n\u2022 Removed Rewind feature due to crashes\n\u2022 Updated GBC controller skin to new style\n\u2022 Updated GBA controller skin to use new previews\n\u2022 Removed branding from GBA skin for a cleaner look",
+                    "size": 50724007,
+                    "version": "0.5.3"
+                },
+                {
+                    "date": "2023-02-26T00:00:00-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Delta-Ignited/releases/download/v0.5.2/delta-ignited.ipa",
+                    "localizedDescription": "New Feature\n\u2022 Controller Skin Previews - Supports showing a preview image in settings instead of a bare skin image\n\nChanges\n\u2022 Updated GBC controller skin to new style\n\u2022 Updated GBA controller skin to use new previews\n\u2022 Removed branding from GBA skin for a cleaner look",
+                    "size": 52114631,
+                    "version": "0.5.2"
+                },
+                {
+                    "date": "2023-02-25T00:00:20-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Delta-Ignited/releases/download/v0.5.1/delta-ignited.ipa",
+                    "localizedDescription": "New Feature\n\u2022 Controller Skin Previews - Supports showing a preview image in settings instead of a bare skin image\n\nChanges\n\u2022 Updated GBA controller skin to use new previews\n\u2022 Removed branding from GBA skin for a cleaner look",
+                    "size": 52114631,
+                    "version": "0.5.1"
+                },
+                {
+                    "date": "2023-02-25T00:00:10-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Delta-Ignited/releases/download/v0.5.0/delta-ignited.ipa",
+                    "localizedDescription": "New Feature\n\u2022 Controller Skin Previews - Supports showing a preview image in settings instead of a bare skin image",
+                    "size": 52097008,
+                    "version": "0.5.0"
+                },
+                {
+                    "date": "2023-02-25T00:00:00-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Delta-Ignited/releases/download/v0.4.1/delta-ignited.ipa",
+                    "localizedDescription": "New Feature\n\u2022 Customizable Fast Forward Speed\n\nBug Fixes\n\u2022 Fixed some popups crashing on iPad\n\u2022 Fixed a crash in settings with local multiplayer\n  \u2022 Controller selection remains glitchy but functional",
+                    "size": 52094410,
+                    "version": "0.4.1"
+                },
+                {
+                    "date": "2023-02-24T00:00:00-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Delta-Ignited/releases/download/v0.4.0/delta-ignited.ipa",
+                    "localizedDescription": "New Feature\n\u2022 Customizable Fast Forward Speed",
+                    "size": 51978697,
+                    "version": "0.4.0"
+                },
+                {
+                    "date": "2023-02-23T00:00:00-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Delta-Ignited/releases/download/v0.3.0/delta-ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Download skins from settings\n\u2022 Rounded and inset settings tables",
+                    "size": 51973518,
+                    "version": "0.3.0"
+                },
+                {
+                    "date": "2023-02-21T00:00:00-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Delta-Ignited/releases/download/v0.2.1/delta-ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Add Genesis and remove all beta checks\n\u2022 Update and expand contributors list",
+                    "size": 51971781,
+                    "version": "0.2.1"
+                },
+                {
+                    "date": "2023-02-20T00:00:00-00:00",
+                    "downloadURL": "https://github.com/Lit-Development/Delta-Ignited/releases/download/v0.2.0/delta-ignited.ipa",
+                    "localizedDescription": "New Features\n\u2022 Local Multiplayer - Connect up to 4 controllers on supported consoles\n\u2022 Save State Rewind - Rolling save states that can be rewinded to at any time\n\u2022 Extended MFi Support - Add support for missing MFi inputs",
+                    "size": 51971282,
+                    "version": "0.2.0"
+                }
+            ]
         }
     ],
+    "description": "This source is an automatically kept up-to-date source, powered by GitHub Actions, the Python altparse library, and the support of independent developers. In here, you'll find anything from community maintained forks of Delta Emulator, to tiny Mac utilities that no one's ever heard of. If you have an app you'd like to see here, please use our website to reach out!",
+    "featuredApps": [
+        "com.litritt.ignited",
+        "com.example.mame4ios",
+        "com.wh0ba.xpatcher",
+        "net.namedfork.minivmac",
+        "com.zurac.OldOS"
+    ],
+    "headerURL": "https://quarksources.github.io/assets/quantumsource.png",
+    "iconURL": "https://quarksources.github.io/assets/ElementQ-Circled.png",
     "identifier": "com.quarksources.quantumsource",
     "name": "Quantum Source",
     "news": [
         {
+            "caption": "New features, fixes, and skins.\n\nTap for full changelog and more info.",
+            "date": "2023-02-25",
+            "identifier": "ignited-initial-release",
+            "notify": false,
+            "tintColor": "FF6A00",
+            "title": "Ignited Is Here!",
+            "url": "https://litritt.com/ignited"
+        },
+        {
             "appID": "me.oatmealdome.dolphinios-njb",
             "caption": "Play GameCube and Wii classics on your non-jailbroken iPhone or iPad.",
             "date": "2020-05-04",
             "identifier": "dolphinios-first-release",
             "imageURL": "https://cdn.oatmealdome.me/dolphinios/altstore/ios_marketing1024x1024_nobg.png",
             "notify": false,
             "tintColor": "363636",
@@ -1271,12 +1728,13 @@
             "identifier": "oldos-release",
             "imageURL": "https://github.com/zzanehip/The-OldOS-Project/raw/master/Images/Header.jpg",
             "notify": false,
             "tintColor": "251c21",
             "title": "OldOS now available!"
         }
     ],
-    "sourceIconURL": "https://quarksources.github.io/assets/ElementQ.png",
-    "sourceURL": "https://quarksources.github.io/quantumsource.json",
+    "subtitle": "Contains all of your favorite emulators, games, jailbreaks, utilities, and more.",
+    "tintColor": "#343a40",
     "userinfo": {},
-    "version": 2
+    "version": 2,
+    "website": "https://quarksources.github.io/"
 }
```

### Comparing `altparse-0.2.1/tests/test_create_altsource_obj.py` & `altparse-0.3.0/tests/test_create_altsource_obj.py`

 * *Files identical despite different names*

