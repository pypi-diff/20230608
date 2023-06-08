# Comparing `tmp/teamsgraphapi-0.0.2.tar.gz` & `tmp/teamsgraphapi-0.0.3.tar.gz`

## Comparing `teamsgraphapi-0.0.2.tar` & `teamsgraphapi-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/graphapi/__init__.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/graphapi/auth.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/graphapi/graph.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/LICENCE
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/README.md
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/graphapi/__init__.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/graphapi/auth.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/graphapi/graph.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/LICENCE
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/README.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.3/PKG-INFO
```

### Comparing `teamsgraphapi-0.0.2/graphapi/graph.py` & `teamsgraphapi-0.0.3/graphapi/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     def api(self, url):
         endpoint = f'{self.base_url}{url}'
         try:
             headers = self.headers
             response = requests.get(endpoint, headers=headers)
         except Exception as e:
             return {"error": e}
-        pprint(response.json())
         return response.json()
 
     def get_teams(self):
         """
         get the all teams of authenticated user
         """
         url = '/me/joinedTeams'
```

### Comparing `teamsgraphapi-0.0.2/LICENCE` & `teamsgraphapi-0.0.3/LICENCE`

 * *Files identical despite different names*

