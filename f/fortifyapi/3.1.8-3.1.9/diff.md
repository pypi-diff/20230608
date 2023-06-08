# Comparing `tmp/fortifyapi-3.1.8.tar.gz` & `tmp/fortifyapi-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortifyapi-3.1.8.tar", last modified: Thu Jun  8 02:34:03 2023, max compression
+gzip compressed data, was "fortifyapi-3.1.9.tar", last modified: Thu Jun  8 21:44:56 2023, max compression
```

## Comparing `fortifyapi-3.1.8.tar` & `fortifyapi-3.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 02:34:03.899080 fortifyapi-3.1.8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1046 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       29 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3347 2023-06-08 02:34:03.899080 fortifyapi-3.1.8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2228 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 02:34:03.895080 fortifyapi-3.1.8/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7460 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/docs/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/docs/couscous.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 02:34:03.895080 fortifyapi-3.1.8/fortifyapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/fortifyapi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6749 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/fortifyapi/api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27850 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/fortifyapi/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/fortifyapi/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    40384 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/fortifyapi/fortify.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/fortifyapi/query.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7013 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/fortifyapi/template.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 02:34:03.895080 fortifyapi-3.1.8/fortifyapi.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3347 2023-06-08 02:34:03.000000 fortifyapi-3.1.8/fortifyapi.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2023-06-08 02:34:03.000000 fortifyapi-3.1.8/fortifyapi.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-08 02:34:03.000000 fortifyapi-3.1.8/fortifyapi.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-06-08 02:34:03.000000 fortifyapi-3.1.8/fortifyapi.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-06-08 02:34:03.000000 fortifyapi-3.1.8/fortifyapi.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-08 02:34:03.000000 fortifyapi-3.1.8/fortifyapi.egg-info/zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-06-08 02:34:03.899080 fortifyapi-3.1.8/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 02:34:03.899080 fortifyapi-3.1.8/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1963 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      986 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_artifacts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      884 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_bugtracker.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1544 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2143 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_issues.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_jobs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_pool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3918 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_projects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      442 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_reports.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1024 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_rulepack.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2994 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_versions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:44:56.510756 fortifyapi-3.1.9/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1046 2023-06-08 21:44:49.000000 fortifyapi-3.1.9/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       29 2023-06-08 21:44:49.000000 fortifyapi-3.1.9/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3347 2023-06-08 21:44:56.510756 fortifyapi-3.1.9/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2228 2023-06-08 21:44:49.000000 fortifyapi-3.1.9/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:44:56.506756 fortifyapi-3.1.9/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7460 2023-06-08 21:44:49.000000 fortifyapi-3.1.9/docs/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-06-08 21:44:49.000000 fortifyapi-3.1.9/docs/couscous.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:44:56.506756 fortifyapi-3.1.9/fortifyapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2023-06-08 21:44:49.000000 fortifyapi-3.1.9/fortifyapi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6749 2023-06-08 21:44:49.000000 fortifyapi-3.1.9/fortifyapi/api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27850 2023-06-08 21:44:49.000000 fortifyapi-3.1.9/fortifyapi/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-06-08 21:44:49.000000 fortifyapi-3.1.9/fortifyapi/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41232 2023-06-08 21:44:49.000000 fortifyapi-3.1.9/fortifyapi/fortify.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-06-08 21:44:49.000000 fortifyapi-3.1.9/fortifyapi/query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7013 2023-06-08 21:44:49.000000 fortifyapi-3.1.9/fortifyapi/template.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:44:56.506756 fortifyapi-3.1.9/fortifyapi.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3347 2023-06-08 21:44:56.000000 fortifyapi-3.1.9/fortifyapi.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2023-06-08 21:44:56.000000 fortifyapi-3.1.9/fortifyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-08 21:44:56.000000 fortifyapi-3.1.9/fortifyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-06-08 21:44:56.000000 fortifyapi-3.1.9/fortifyapi.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-06-08 21:44:56.000000 fortifyapi-3.1.9/fortifyapi.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-08 21:44:56.000000 fortifyapi-3.1.9/fortifyapi.egg-info/zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-06-08 21:44:56.514756 fortifyapi-3.1.9/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2023-06-08 21:44:49.000000 fortifyapi-3.1.9/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 21:44:56.510756 fortifyapi-3.1.9/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1963 2023-06-08 21:44:50.000000 fortifyapi-3.1.9/tests/test_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      986 2023-06-08 21:44:50.000000 fortifyapi-3.1.9/tests/test_artifacts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      884 2023-06-08 21:44:50.000000 fortifyapi-3.1.9/tests/test_bugtracker.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1544 2023-06-08 21:44:50.000000 fortifyapi-3.1.9/tests/test_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2143 2023-06-08 21:44:50.000000 fortifyapi-3.1.9/tests/test_issues.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-06-08 21:44:50.000000 fortifyapi-3.1.9/tests/test_jobs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2023-06-08 21:44:50.000000 fortifyapi-3.1.9/tests/test_pool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3918 2023-06-08 21:44:50.000000 fortifyapi-3.1.9/tests/test_projects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      442 2023-06-08 21:44:50.000000 fortifyapi-3.1.9/tests/test_reports.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1024 2023-06-08 21:44:50.000000 fortifyapi-3.1.9/tests/test_rulepack.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2994 2023-06-08 21:44:50.000000 fortifyapi-3.1.9/tests/test_versions.py
```

### Comparing `fortifyapi-3.1.8/LICENSE.txt` & `fortifyapi-3.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/PKG-INFO` & `fortifyapi-3.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fortifyapi
-Version: 3.1.8
+Version: 3.1.9
 Summary: Python library for Fortify Software Security Center (SSC) RESTFul API
 Home-page: https://github.com/fortifyadmin/fortifyapi
-Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.8
+Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.9
 Author: Brandon Spruth, Matthew Gill
 Author-email: brandon@spruth.co, mgill@c0ffee.me
 License: MIT
 Keywords: fortify,api,security,software,microfocus,ssc,sast
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `fortifyapi-3.1.8/README.rst` & `fortifyapi-3.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/docs/README.md` & `fortifyapi-3.1.9/docs/README.md`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/fortifyapi/api.py` & `fortifyapi-3.1.9/fortifyapi/api.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/fortifyapi/client.py` & `fortifyapi-3.1.9/fortifyapi/client.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/fortifyapi/fortify.py` & `fortifyapi-3.1.9/fortifyapi/fortify.py`

 * *Files 1% similar despite different names*

```diff
@@ -642,14 +642,19 @@
             "terminalDate": expire_date
         }
 
         url = "/api/v1/tokens"
         return self._request('POST', url, json=data)
 
     def set_assign_user(self, version_id, issue_id, user, revision=0):
+        """
+        :version_id: Project Version ID integer typically found within a SSC Deeplink
+        :issue_id: Issue integer that identifies the issue, this is NOT the UUID or SSC Instance ID
+        :user: Registered Fortify SSC User name
+        """
         data = {
                 "type": "AUDIT_ISSUE",
                 "values": {
                     "issues": [
                         {
                             "id": issue_id,
                             "revision": revision
@@ -657,14 +662,25 @@
                     ],
                     "user": user
                 }
         }
         url = f'/api/v1/projectVersions/{version_id}/issues/action'
         return self._request('POST', url, json=data)
 
+    def get_project_version_issue(self, version_id, issue_id):
+        """
+        Manage issues in the application version. Usage for this may be to garner the revision ID to increment for
+        set_assign_user.  Other calls may be to query for audit info on a given issue.
+
+        :version_id: Project Version ID integer typically found within a SSC Deeplink
+        :issue_id: Issue integer that identifies the issue, this is NOT the UUID or SSC Instance ID
+        """
+        url = f"/api/v1/projectVersions/{version_id}/issues/{issue_id}"
+        return self._request('GET', url)
+
     def get_all_rulepacks(self):
         """
         List all rules on an SSC instance
         :return:
         """
         url = "/api/v1/coreRulepacks"
         return self._request('GET', url)
```

### Comparing `fortifyapi-3.1.8/fortifyapi/query.py` & `fortifyapi-3.1.9/fortifyapi/query.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/fortifyapi/template.py` & `fortifyapi-3.1.9/fortifyapi/template.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/fortifyapi.egg-info/PKG-INFO` & `fortifyapi-3.1.9/fortifyapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fortifyapi
-Version: 3.1.8
+Version: 3.1.9
 Summary: Python library for Fortify Software Security Center (SSC) RESTFul API
 Home-page: https://github.com/fortifyadmin/fortifyapi
-Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.8
+Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.9
 Author: Brandon Spruth, Matthew Gill
 Author-email: brandon@spruth.co, mgill@c0ffee.me
 License: MIT
 Keywords: fortify,api,security,software,microfocus,ssc,sast
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `fortifyapi-3.1.8/fortifyapi.egg-info/SOURCES.txt` & `fortifyapi-3.1.9/fortifyapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/setup.py` & `fortifyapi-3.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/tests/test_api.py` & `fortifyapi-3.1.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/tests/test_artifacts.py` & `fortifyapi-3.1.9/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/tests/test_bugtracker.py` & `fortifyapi-3.1.9/tests/test_bugtracker.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/tests/test_client.py` & `fortifyapi-3.1.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/tests/test_issues.py` & `fortifyapi-3.1.9/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/tests/test_jobs.py` & `fortifyapi-3.1.9/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/tests/test_pool.py` & `fortifyapi-3.1.9/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/tests/test_projects.py` & `fortifyapi-3.1.9/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/tests/test_rulepack.py` & `fortifyapi-3.1.9/tests/test_rulepack.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.8/tests/test_versions.py` & `fortifyapi-3.1.9/tests/test_versions.py`

 * *Files identical despite different names*

