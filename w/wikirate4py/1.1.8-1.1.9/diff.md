# Comparing `tmp/wikirate4py-1.1.8.tar.gz` & `tmp/wikirate4py-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikirate4py-1.1.8.tar", last modified: Fri May 12 11:54:36 2023, max compression
+gzip compressed data, was "wikirate4py-1.1.9.tar", last modified: Thu Jun  8 09:59:33 2023, max compression
```

## Comparing `wikirate4py-1.1.8.tar` & `wikirate4py-1.1.9.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 11:54:36.413273 wikirate4py-1.1.8/
--rw-rw-rw-   0        0        0    35823 2023-02-02 11:17:13.000000 wikirate4py-1.1.8/LICENSE
--rw-rw-rw-   0        0        0     3721 2023-05-12 11:54:36.413273 wikirate4py-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2485 2023-02-02 11:17:13.000000 wikirate4py-1.1.8/README.rst
--rw-rw-rw-   0        0        0       87 2023-05-12 11:54:36.414285 wikirate4py-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     2190 2023-05-12 11:52:41.000000 wikirate4py-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:54:36.390906 wikirate4py-1.1.8/wikirate4py/
--rw-rw-rw-   0        0        0     1124 2023-05-12 11:52:41.000000 wikirate4py-1.1.8/wikirate4py/__init__.py
--rw-rw-rw-   0        0        0    62893 2023-05-12 11:41:45.000000 wikirate4py-1.1.8/wikirate4py/api.py
--rw-rw-rw-   0        0        0      586 2023-05-12 11:40:36.000000 wikirate4py-1.1.8/wikirate4py/cursor.py
--rw-rw-rw-   0        0        0     1675 2023-02-02 11:17:13.000000 wikirate4py-1.1.8/wikirate4py/exceptions.py
--rw-rw-rw-   0        0        0     5953 2023-05-12 09:53:30.000000 wikirate4py-1.1.8/wikirate4py/main.py
--rw-rw-rw-   0        0        0      541 2023-02-02 11:17:13.000000 wikirate4py-1.1.8/wikirate4py/mixins.py
--rw-rw-rw-   0        0        0    18417 2023-04-05 10:25:18.000000 wikirate4py-1.1.8/wikirate4py/models.py
--rw-rw-rw-   0        0        0     2210 2023-05-12 11:39:59.000000 wikirate4py-1.1.8/wikirate4py/msa_download_script.py
--rw-rw-rw-   0        0        0     2154 2023-04-04 16:58:48.000000 wikirate4py-1.1.8/wikirate4py/new_metrics.py
--rw-rw-rw-   0        0        0     5377 2023-05-10 06:47:11.000000 wikirate4py-1.1.8/wikirate4py/uk_assessed_statements.py
--rw-rw-rw-   0        0        0      859 2023-02-02 11:17:13.000000 wikirate4py-1.1.8/wikirate4py/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:54:36.411764 wikirate4py-1.1.8/wikirate4py.egg-info/
--rw-rw-rw-   0        0        0     3721 2023-05-12 11:54:36.000000 wikirate4py-1.1.8/wikirate4py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-05-12 11:54:36.000000 wikirate4py-1.1.8/wikirate4py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 11:54:36.000000 wikirate4py-1.1.8/wikirate4py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-05-12 11:54:36.000000 wikirate4py-1.1.8/wikirate4py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-12 11:54:36.000000 wikirate4py-1.1.8/wikirate4py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-03 19:11:20.000000 wikirate4py-1.1.8/wikirate4py.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-08 09:59:33.574389 wikirate4py-1.1.9/
+-rw-rw-rw-   0        0        0    35823 2023-02-02 11:17:13.000000 wikirate4py-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0     3721 2023-06-08 09:59:33.574389 wikirate4py-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2485 2023-02-02 11:17:13.000000 wikirate4py-1.1.9/README.rst
+-rw-rw-rw-   0        0        0       87 2023-06-08 09:59:33.575390 wikirate4py-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2190 2023-06-08 09:53:35.000000 wikirate4py-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:59:33.549387 wikirate4py-1.1.9/wikirate4py/
+-rw-rw-rw-   0        0        0     1124 2023-06-08 09:53:35.000000 wikirate4py-1.1.9/wikirate4py/__init__.py
+-rw-rw-rw-   0        0        0    63710 2023-06-08 09:51:59.000000 wikirate4py-1.1.9/wikirate4py/api.py
+-rw-rw-rw-   0        0        0     3875 2023-06-07 09:29:38.000000 wikirate4py-1.1.9/wikirate4py/copy_answers.py
+-rw-rw-rw-   0        0        0      586 2023-05-12 11:40:36.000000 wikirate4py-1.1.9/wikirate4py/cursor.py
+-rw-rw-rw-   0        0        0     1675 2023-02-02 11:17:13.000000 wikirate4py-1.1.9/wikirate4py/exceptions.py
+-rw-rw-rw-   0        0        0     1295 2023-06-06 08:21:26.000000 wikirate4py-1.1.9/wikirate4py/find_verified.py
+-rw-rw-rw-   0        0        0     5953 2023-05-19 16:54:07.000000 wikirate4py-1.1.9/wikirate4py/main.py
+-rw-rw-rw-   0        0        0      541 2023-02-02 11:17:13.000000 wikirate4py-1.1.9/wikirate4py/mixins.py
+-rw-rw-rw-   0        0        0    18701 2023-05-15 13:51:43.000000 wikirate4py-1.1.9/wikirate4py/models.py
+-rw-rw-rw-   0        0        0     2210 2023-05-12 11:39:59.000000 wikirate4py-1.1.9/wikirate4py/msa_download_script.py
+-rw-rw-rw-   0        0        0     2154 2023-04-04 16:58:48.000000 wikirate4py-1.1.9/wikirate4py/new_metrics.py
+-rw-rw-rw-   0        0        0      989 2023-05-15 14:42:10.000000 wikirate4py-1.1.9/wikirate4py/subsidiaries.py
+-rw-rw-rw-   0        0        0     2047 2023-06-02 09:46:04.000000 wikirate4py-1.1.9/wikirate4py/test_publish.py
+-rw-rw-rw-   0        0        0      382 2023-05-31 20:45:16.000000 wikirate4py-1.1.9/wikirate4py/test_unpublished.py
+-rw-rw-rw-   0        0        0     5377 2023-05-10 06:47:11.000000 wikirate4py-1.1.9/wikirate4py/uk_assessed_statements.py
+-rw-rw-rw-   0        0        0      859 2023-02-02 11:17:13.000000 wikirate4py-1.1.9/wikirate4py/utils.py
+-rw-rw-rw-   0        0        0     1490 2023-06-06 08:20:11.000000 wikirate4py-1.1.9/wikirate4py/verify_answers.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:59:33.573388 wikirate4py-1.1.9/wikirate4py.egg-info/
+-rw-rw-rw-   0        0        0     3721 2023-06-08 09:59:33.000000 wikirate4py-1.1.9/wikirate4py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2023-06-08 09:59:33.000000 wikirate4py-1.1.9/wikirate4py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 09:59:33.000000 wikirate4py-1.1.9/wikirate4py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-08 09:59:33.000000 wikirate4py-1.1.9/wikirate4py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-08 09:59:33.000000 wikirate4py-1.1.9/wikirate4py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-03 19:11:20.000000 wikirate4py-1.1.9/wikirate4py.egg-info/zip-safe
```

### Comparing `wikirate4py-1.1.8/LICENSE` & `wikirate4py-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.8/PKG-INFO` & `wikirate4py-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wikirate4py
-Version: 1.1.8
+Version: 1.1.9
 Summary: WikiRate for Python!
 Home-page: https://github.com/wikirate/wikirate4py
 Author: Vasiliki Gkatziaki
 Author-email: vasso@wikirate.org
 License: GPL-3.0
-Download-URL: https://github.com/wikirate/wikirate4py/archive/refs/tags/v1.1.8.tar.gz
+Download-URL: https://github.com/wikirate/wikirate4py/archive/refs/tags/v1.1.9.tar.gz
 Project-URL: Documentation, https://wikirate4py.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/wikirate4py/wikirate4py/issues
 Project-URL: Source Code, https://github.com/wikirate4py/wikirate4py
 Keywords: wikirate library
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `wikirate4py-1.1.8/README.rst` & `wikirate4py-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.8/setup.py` & `wikirate4py-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       version=version,
       description='WikiRate for Python!',
       long_description=readme,
       url='https://github.com/wikirate/wikirate4py',
       author='Vasiliki Gkatziaki',
       author_email='vasso@wikirate.org',
       license='GPL-3.0',
-      download_url='https://github.com/wikirate/wikirate4py/archive/refs/tags/v1.1.8.tar.gz',
+      download_url='https://github.com/wikirate/wikirate4py/archive/refs/tags/v1.1.9.tar.gz',
       packages=find_packages(exclude=["tests", "examples"]),
       install_requires=[
           "requests",
           "html2text",
           "pandas"
       ],
       project_urls={
```

### Comparing `wikirate4py-1.1.8/wikirate4py/__init__.py` & `wikirate4py-1.1.9/wikirate4py/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # wikirate4py
 # Copyright 2021 Vasiliki Gkatziaki for WikiRate
 # See LICENSE for details.
 
 """
 wikirate4py WikiRate API library
 """
-__version__ = '1.1.8'
+__version__ = '1.1.9'
 __author__ = 'Vasiliki Gkatziaki'
 __license__ = 'GPL-3.0'
 
 from wikirate4py.api import API
 from wikirate4py.cursor import Cursor
 from wikirate4py.exceptions import (IllegalHttpMethod, WikiRate4PyException, HTTPException, BadRequestException,
                                     UnauthorizedException, ForbiddenException, NotFoundException,
```

### Comparing `wikirate4py-1.1.8/wikirate4py/api.py` & `wikirate4py-1.1.9/wikirate4py/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,16 +428,17 @@
         id
             numeric identifier of the metric answer
 
         Returns
         -------
             :py:class:`~wikirate4py.models.Company`
         """
-        company = ('~' + company.__str__()) if isinstance(company, int) else company.__str__().replace(',', ' ').replace('.',
-                                                                                                        ' ').replace(
+        company = ('~' + company.__str__()) if isinstance(company, int) else company.__str__().replace(',',
+                                                                                                       ' ').replace('.',
+                                                                                                                    ' ').replace(
             '/', ' ').replace('-', ' ').strip().replace(" ", "_")
         return self.get("/{0}+{1}+{2}+{3}.json".format(metric_designer, metric_name, company, str(year)))
 
     @objectify(Answer)
     def get_answer(self, id):
         """get_answer(id)
 
@@ -811,15 +812,15 @@
             -------
                 :py:class:`List`\[:class:`~wikirate4py.models.RelationshipAnswerItem`]
 
             """
 
         return self.get("/~{0}+{1}+Relationship_Answer.json".format(metric_designer.replace(" ", "_"),
                                                                     metric_name.replace(" ", "_")),
-                        endpoint_params=('limit', 'offset'), filters=(
+                        endpoint_params=('limit', 'offset', 'view'), filters=(
                 'year', 'status', 'company_group', 'country', 'value', 'value_from', 'value_to', 'updated',
                 'updater', 'outliers', 'source', 'verification', 'project', 'bookmark', 'published'), **kwargs)
 
     @objectify(Project)
     def get_project(self, identifier):
         """get_project(identifier)
         Returns a WikiRate Project based on the given identifier (name or number)
@@ -1138,14 +1139,15 @@
 
         Returns
         -------
             :py:class:`~wikirate4py.models.Answer`
 
         """
         required_params = ('metric_designer', 'metric_name', 'company', 'year', 'value', 'source')
+        optional_params = ('comment', 'unpublished')
 
         for k in required_params:
             if k not in kwargs:
                 raise WikiRate4PyException("""Invalid set of params! You need to define all the following params to import 
                     a new research answer: """ + required_params.__str__())
 
         company_identifier = '~' + str(kwargs['company']) if isinstance(kwargs['company'], int) else kwargs[
@@ -1155,16 +1157,19 @@
             "card[name]": kwargs['metric_designer'] + '+' + kwargs['metric_name'] + '+' + company_identifier + '+' +
                           str(kwargs['year']),
             "card[subcards][+:value]": kwargs['value'],
             "card[subcards][+:source]": kwargs['source'],
             "format": "json",
             "success[format]": "json"
         }
-        if kwargs.get('comment') is not None:
-            params['card[subcards][+:discussion]'] = str(kwargs['comment'])
+        for k in kwargs.keys():
+            if k == 'comment':
+                params['card[subcards][+:discussion]'] = str(kwargs[k])
+            elif k != required_params and k in optional_params:
+                params['card[subcards][+:' + k + ']'] = kwargs[k]
         log.debug("PARAMS: %r", params)
 
         return self.post("/card/create", params)
 
     @objectify(Answer)
     def update_research_metric_answer(self, **kwargs):
         """update_research_metric_answer(metric_designer, metric_name, company, year, *, value, source, comment)
@@ -1260,15 +1265,15 @@
 
         Returns
         -------
             :py:class:`~wikirate4py.models.Answer`
 
         """
         required_param = 'id'
-        optional_params = ('company', 'year', 'value', 'source', 'comment')
+        optional_params = ('company', 'year', 'value', 'source', 'comment', 'unpublished')
 
         if required_param not in kwargs:
             raise WikiRate4PyException(
                 """Invalid set of params! You need to define all the following params to update the research answer: """ + required_param.__str__())
 
         if kwargs.get('company') is not None:
             company_identifier = '~' + str(kwargs['company']) if isinstance(kwargs['company'], int) else kwargs[
@@ -1636,7 +1641,21 @@
             "card[name]": '~' + group_id + '+' + 'Company',
             "card[content]": ids,
             "format": "json",
             "success[format]": "json"
         }
 
         return self.post("/card/update", params)
+
+    def verify_answer(self, identifier):
+        params = {
+            "card[type]": "List",
+            "card[name]": '~{0}+checked_by'.format(identifier),
+            "card[trigger]": 'add_check',
+            "format": "json",
+            "success[format]": "json"
+        }
+
+        return self.post("/card/update", params)
+
+    def get_comments(self, identifier):
+        return self.get("/~{0}+discussion.json".format(identifier)).json().get('content', '')
```

### Comparing `wikirate4py-1.1.8/wikirate4py/cursor.py` & `wikirate4py-1.1.9/wikirate4py/cursor.py`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.8/wikirate4py/exceptions.py` & `wikirate4py-1.1.9/wikirate4py/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.8/wikirate4py/main.py` & `wikirate4py-1.1.9/wikirate4py/main.py`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.8/wikirate4py/mixins.py` & `wikirate4py-1.1.9/wikirate4py/mixins.py`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.8/wikirate4py/models.py` & `wikirate4py-1.1.9/wikirate4py/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -418,31 +418,33 @@
     __slots__ = (
         "id", "metric", "metric_id", "value", "year", "comments", "sources",
         "subject_company_name", "object_company_name", "subject_company_id", "object_company_id",
         "url", "raw")
 
     def __init__(self, data):
         self.raw = data
-        if data["type"] != 'Relationship Answer':
+        if data.get("type", {}).get("name") != 'Relationship Answer' and data["type"] != 'Relationship Answer':
             raise WikiRate4PyException('Invalid type of entity')
 
         self.id = data.get("id")
         fields = data.get("name").split("+")
         self.metric = fields[0] + "+" + fields[1]
         self.metric_id = data.get("metric_id")
         self.value = data.get("value")
         self.year = data.get("year")
         self.subject_company_id = data.get("subject_company_id")
         self.object_company_id = data.get("object_company_id")
         self.comments = data.get("comments")
         self.sources = []
         for s in data.get("sources", []):
             self.sources.append(s.get("name"))
-        self.subject_company_name = data.get("subject_company")
-        self.object_company_name = data.get("object_company")
+        self.subject_company_name = data.get("subject_company") \
+            if isinstance(data.get("subject_company"), str) else data.get("subject_company", {}).get("name")
+        self.object_company_name = data.get("object_company") \
+            if isinstance(data.get("object_company"), str) else data.get("object_company", {}).get("name")
         self.url = data.get("url").replace(".json", "")
 
 
 class RegionItem(WikiRateEntity):
     __slots__ = (
         "id", "name", "url", "raw")
```

### Comparing `wikirate4py-1.1.8/wikirate4py/msa_download_script.py` & `wikirate4py-1.1.9/wikirate4py/msa_download_script.py`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.8/wikirate4py/new_metrics.py` & `wikirate4py-1.1.9/wikirate4py/new_metrics.py`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.8/wikirate4py/uk_assessed_statements.py` & `wikirate4py-1.1.9/wikirate4py/uk_assessed_statements.py`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.8/wikirate4py/utils.py` & `wikirate4py-1.1.9/wikirate4py/utils.py`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.8/wikirate4py.egg-info/PKG-INFO` & `wikirate4py-1.1.9/wikirate4py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wikirate4py
-Version: 1.1.8
+Version: 1.1.9
 Summary: WikiRate for Python!
 Home-page: https://github.com/wikirate/wikirate4py
 Author: Vasiliki Gkatziaki
 Author-email: vasso@wikirate.org
 License: GPL-3.0
-Download-URL: https://github.com/wikirate/wikirate4py/archive/refs/tags/v1.1.8.tar.gz
+Download-URL: https://github.com/wikirate/wikirate4py/archive/refs/tags/v1.1.9.tar.gz
 Project-URL: Documentation, https://wikirate4py.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/wikirate4py/wikirate4py/issues
 Project-URL: Source Code, https://github.com/wikirate4py/wikirate4py
 Keywords: wikirate library
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `wikirate4py-1.1.8/wikirate4py.egg-info/SOURCES.txt` & `wikirate4py-1.1.9/wikirate4py.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 LICENSE
 README.rst
 setup.cfg
 setup.py
 wikirate4py/__init__.py
 wikirate4py/api.py
+wikirate4py/copy_answers.py
 wikirate4py/cursor.py
 wikirate4py/exceptions.py
+wikirate4py/find_verified.py
 wikirate4py/main.py
 wikirate4py/mixins.py
 wikirate4py/models.py
 wikirate4py/msa_download_script.py
 wikirate4py/new_metrics.py
+wikirate4py/subsidiaries.py
+wikirate4py/test_publish.py
+wikirate4py/test_unpublished.py
 wikirate4py/uk_assessed_statements.py
 wikirate4py/utils.py
+wikirate4py/verify_answers.py
 wikirate4py.egg-info/PKG-INFO
 wikirate4py.egg-info/SOURCES.txt
 wikirate4py.egg-info/dependency_links.txt
 wikirate4py.egg-info/requires.txt
 wikirate4py.egg-info/top_level.txt
 wikirate4py.egg-info/zip-safe
```

