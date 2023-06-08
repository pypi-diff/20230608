# Comparing `tmp/posuto-2023.6.0.tar.gz` & `tmp/posuto-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posuto-2023.6.0.tar", last modified: Fri Jun  2 01:28:54 2023, max compression
+gzip compressed data, was "posuto-2023.6.1.tar", last modified: Thu Jun  8 11:22:44 2023, max compression
```

## Comparing `posuto-2023.6.0.tar` & `posuto-2023.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-02 01:28:54.258375 posuto-2023.6.0/
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-02 01:28:54.158424 posuto-2023.6.0/.github/
--rw-r--r--   0 23        (1000) u23       (1000)       13 2020-12-07 10:56:39.000000 posuto-2023.6.0/.github/FUNDING.yml
--rw-r--r--   0 23        (1000) u23       (1000)     1872 2020-12-07 10:56:39.000000 posuto-2023.6.0/.gitignore
--rw-r--r--   0 23        (1000) u23       (1000)     1076 2020-12-07 10:56:39.000000 posuto-2023.6.0/LICENSE
--rw-r--r--   0 23        (1000) u23       (1000)      142 2020-12-07 10:56:39.000000 posuto-2023.6.0/MANIFEST.in
--rw-r--r--   0 23        (1000) u23       (1000)      692 2021-02-26 11:37:41.000000 posuto-2023.6.0/Makefile
--rw-r--r--   0 23        (1000) u23       (1000)     6455 2023-06-02 01:28:54.258375 posuto-2023.6.0/PKG-INFO
--rw-r--r--   0 23        (1000) u23       (1000)     5639 2023-01-31 11:52:04.000000 posuto-2023.6.0/README.md
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-02 01:28:54.158424 posuto-2023.6.0/examples/
--rw-r--r--   0 23        (1000) u23       (1000)      272 2020-12-07 10:56:39.000000 posuto-2023.6.0/examples/sample.py
--rw-r--r--   0 23        (1000) u23       (1000)   295014 2020-12-07 10:56:39.000000 posuto-2023.6.0/postcharacter.png
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-02 01:28:54.258375 posuto-2023.6.0/posuto/
--rw-r--r--   0 23        (1000) u23       (1000)       40 2022-12-01 14:35:27.000000 posuto-2023.6.0/posuto/__init__.py
--rw-r--r--   0 23        (1000) u23       (1000) 13065151 2023-06-02 01:27:03.000000 posuto-2023.6.0/posuto/officedata.json
--rw-r--r--   0 23        (1000) u23       (1000) 81154048 2023-06-02 01:27:04.000000 posuto-2023.6.0/posuto/postaldata.db
--rw-r--r--   0 23        (1000) u23       (1000)     2770 2022-12-01 14:35:27.000000 posuto-2023.6.0/posuto/posuto.py
--rw-r--r--   0 23        (1000) u23       (1000)    11156 2023-03-15 04:34:33.000000 posuto-2023.6.0/posuto/prep.py
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-02 01:28:54.258375 posuto-2023.6.0/posuto/tests/
--rw-r--r--   0 23        (1000) u23       (1000)     1756 2023-03-15 04:34:33.000000 posuto-2023.6.0/posuto/tests/test_basic.py
-drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-02 01:28:54.258375 posuto-2023.6.0/posuto.egg-info/
--rw-r--r--   0 23        (1000) u23       (1000)     6455 2023-06-02 01:28:53.000000 posuto-2023.6.0/posuto.egg-info/PKG-INFO
--rw-r--r--   0 23        (1000) u23       (1000)      367 2023-06-02 01:28:53.000000 posuto-2023.6.0/posuto.egg-info/SOURCES.txt
--rw-r--r--   0 23        (1000) u23       (1000)        1 2023-06-02 01:28:53.000000 posuto-2023.6.0/posuto.egg-info/dependency_links.txt
--rw-r--r--   0 23        (1000) u23       (1000)        7 2023-06-02 01:28:53.000000 posuto-2023.6.0/posuto.egg-info/top_level.txt
--rw-r--r--   0 23        (1000) u23       (1000)      706 2023-06-02 01:28:54.261707 posuto-2023.6.0/setup.cfg
--rw-r--r--   0 23        (1000) u23       (1000)      471 2020-12-07 10:56:40.000000 posuto-2023.6.0/setup.py
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-08 11:22:44.395402 posuto-2023.6.1/
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-08 11:22:44.328735 posuto-2023.6.1/.github/
+-rw-r--r--   0 23        (1000) u23       (1000)       13 2020-12-07 10:56:39.000000 posuto-2023.6.1/.github/FUNDING.yml
+-rw-r--r--   0 23        (1000) u23       (1000)     1872 2020-12-07 10:56:39.000000 posuto-2023.6.1/.gitignore
+-rw-r--r--   0 23        (1000) u23       (1000)     1076 2020-12-07 10:56:39.000000 posuto-2023.6.1/LICENSE
+-rw-r--r--   0 23        (1000) u23       (1000)      142 2020-12-07 10:56:39.000000 posuto-2023.6.1/MANIFEST.in
+-rw-r--r--   0 23        (1000) u23       (1000)      692 2021-02-26 11:37:41.000000 posuto-2023.6.1/Makefile
+-rw-r--r--   0 23        (1000) u23       (1000)     6455 2023-06-08 11:22:44.395402 posuto-2023.6.1/PKG-INFO
+-rw-r--r--   0 23        (1000) u23       (1000)     5639 2023-01-31 11:52:04.000000 posuto-2023.6.1/README.md
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-08 11:22:44.328735 posuto-2023.6.1/examples/
+-rw-r--r--   0 23        (1000) u23       (1000)      272 2020-12-07 10:56:39.000000 posuto-2023.6.1/examples/sample.py
+-rw-r--r--   0 23        (1000) u23       (1000)   295014 2020-12-07 10:56:39.000000 posuto-2023.6.1/postcharacter.png
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-08 11:22:44.395402 posuto-2023.6.1/posuto/
+-rw-r--r--   0 23        (1000) u23       (1000)       40 2022-12-01 14:35:27.000000 posuto-2023.6.1/posuto/__init__.py
+-rw-r--r--   0 23        (1000) u23       (1000) 13065151 2023-06-08 11:14:45.000000 posuto-2023.6.1/posuto/officedata.json
+-rw-r--r--   0 23        (1000) u23       (1000) 83783680 2023-06-08 11:14:46.000000 posuto-2023.6.1/posuto/postaldata.db
+-rw-r--r--   0 23        (1000) u23       (1000)     2770 2022-12-01 14:35:27.000000 posuto-2023.6.1/posuto/posuto.py
+-rw-r--r--   0 23        (1000) u23       (1000)    11314 2023-06-08 11:14:31.000000 posuto-2023.6.1/posuto/prep.py
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-08 11:22:44.395402 posuto-2023.6.1/posuto/tests/
+-rw-r--r--   0 23        (1000) u23       (1000)     1756 2023-03-15 04:34:33.000000 posuto-2023.6.1/posuto/tests/test_basic.py
+drwxr-xr-x   0 23        (1000) u23       (1000)        0 2023-06-08 11:22:44.395402 posuto-2023.6.1/posuto.egg-info/
+-rw-r--r--   0 23        (1000) u23       (1000)     6455 2023-06-08 11:22:44.000000 posuto-2023.6.1/posuto.egg-info/PKG-INFO
+-rw-r--r--   0 23        (1000) u23       (1000)      367 2023-06-08 11:22:44.000000 posuto-2023.6.1/posuto.egg-info/SOURCES.txt
+-rw-r--r--   0 23        (1000) u23       (1000)        1 2023-06-08 11:22:44.000000 posuto-2023.6.1/posuto.egg-info/dependency_links.txt
+-rw-r--r--   0 23        (1000) u23       (1000)        7 2023-06-08 11:22:44.000000 posuto-2023.6.1/posuto.egg-info/top_level.txt
+-rw-r--r--   0 23        (1000) u23       (1000)      706 2023-06-08 11:22:44.395402 posuto-2023.6.1/setup.cfg
+-rw-r--r--   0 23        (1000) u23       (1000)      471 2020-12-07 10:56:40.000000 posuto-2023.6.1/setup.py
```

### Comparing `posuto-2023.6.0/.gitignore` & `posuto-2023.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `posuto-2023.6.0/LICENSE` & `posuto-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `posuto-2023.6.0/Makefile` & `posuto-2023.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `posuto-2023.6.0/PKG-INFO` & `posuto-2023.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posuto
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: Japanese Postal Code Data
 Home-page: https://github.com/polm/posuto.git
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `posuto-2023.6.0/README.md` & `posuto-2023.6.1/README.md`

 * *Files identical despite different names*

### Comparing `posuto-2023.6.0/postcharacter.png` & `posuto-2023.6.1/postcharacter.png`

 * *Files identical despite different names*

### Comparing `posuto-2023.6.0/posuto/officedata.json` & `posuto-2023.6.1/posuto/officedata.json`

 * *Files identical despite different names*

### Comparing `posuto-2023.6.0/posuto/postaldata.db` & `posuto-2023.6.1/posuto/postaldata.db`

 * *Files 1% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -142651,8 +142651,11 @@
 INSERT INTO office_data VALUES('9010494','{"jis": "47362", "kana": "ナンブスイドウキギヨウダン", "name": "南部水道企業団", "prefecture": "沖縄県", "city": "島尻郡八重瀬町", "neighborhood": "東風平", "banchi": "1473番地2", "postal_code": "9010494", "old_code": "90104", "post_office": "南風原中", "type": "office", "multiple": false, "new": false, "prefecture_kana": "オキナワケン", "city_kana": "シマジリグンヤエセチョウ", "neighborhood_kana": "コチンダ", "alternates": []}');
 INSERT INTO office_data VALUES('9010492','{"jis": "47362", "kana": "ヤエセチヨウヤクバ", "name": "八重瀬町役場", "prefecture": "沖縄県", "city": "島尻郡八重瀬町", "neighborhood": "字東風平", "banchi": "1188番地", "postal_code": "9010492", "old_code": "90104", "post_office": "東風平", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9010496','{"jis": "47362", "kana": "リクジヨウジエイタイ ヨザブントンチ", "name": "陸上自衛隊　与座分屯地", "prefecture": "沖縄県", "city": "島尻郡八重瀬町", "neighborhood": "字富盛", "banchi": "2608", "postal_code": "9010496", "old_code": "90104", "post_office": "東風平", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9010592','{"jis": "47362", "kana": "ヤエセチヨウヤクバ グシカミシユツチヨウシヨ", "name": "八重瀬町役場　具志頭出張所", "prefecture": "沖縄県", "city": "島尻郡八重瀬町", "neighborhood": "字具志頭", "banchi": "1番地", "postal_code": "9010592", "old_code": "90105", "post_office": "東風平", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9060692','{"jis": "47375", "kana": "タラマソンヤクバ", "name": "多良間村役場", "prefecture": "沖縄県", "city": "宮古郡多良間村", "neighborhood": "字仲筋", "banchi": "99-2", "postal_code": "9060692", "old_code": "90606", "post_office": "宮古", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9071292','{"jis": "47381", "kana": "カブシキガイシヤ ハイムルブシ", "name": "株式会社　はいむるぶし", "prefecture": "沖縄県", "city": "八重山郡竹富町", "neighborhood": "字小浜", "banchi": "2930", "postal_code": "9071292", "old_code": "90712", "post_office": "八重山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
 INSERT INTO office_data VALUES('9071892','{"jis": "47382", "kana": "ヨナグニチヨウヤクバ", "name": "与那国町役場", "prefecture": "沖縄県", "city": "八重山郡与那国町", "neighborhood": "字与那国", "banchi": "129", "postal_code": "9071892", "old_code": "90718", "post_office": "八重山", "type": "office", "multiple": false, "new": false, "prefecture_kana": "", "city_kana": "", "neighborhood_kana": "", "alternates": []}');
+CREATE INDEX postal_code_index on postal_data(code);
+CREATE INDEX office_code_index on office_data(code)
+      ;
 COMMIT;
```

### Comparing `posuto-2023.6.0/posuto/posuto.py` & `posuto-2023.6.1/posuto/posuto.py`

 * *Files identical despite different names*

### Comparing `posuto-2023.6.0/posuto/prep.py` & `posuto-2023.6.1/posuto/prep.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,17 @@
     with open('posuto/officedata.json', 'w') as outfile:
         outfile.write(json.dumps(data, ensure_ascii=False, indent=2))
     # write sqlite db
     db.execute("drop table if exists office_data")
     db.execute("""
       create table office_data (
         code text, data text)""")
+    db.execute("""
+      create index office_code_index on office_data(code)
+      """)
     for key, val in data.items():
         entry = json.dumps(val, ensure_ascii=False)
         db.execute("insert into office_data(code, data) values (?, ?)",
                 (key, entry))
     conn.commit()
     conn.close()
 
@@ -263,14 +266,15 @@
     # write sqlite db
     conn = sqlite3.connect('posuto/postaldata.db')
     db = conn.cursor()
     db.execute("drop table if exists postal_data")
     db.execute("""
       create table postal_data (
         code text, data text, prefecture text, city text, neighborhood text)""")
+    db.execute("create index postal_code_index on postal_data(code)")
     for key, val in data.items():
         entry = json.dumps(val, ensure_ascii=False)
         # add additional columns for querying in order to fix office data
         prefecture = val['prefecture']
         city = val['city']
         neighborhood = val['neighborhood']
         db.execute("insert into postal_data(code, data, prefecture, city, neighborhood) values (?, ?, ?, ?, ?)",
```

### Comparing `posuto-2023.6.0/posuto/tests/test_basic.py` & `posuto-2023.6.1/posuto/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `posuto-2023.6.0/posuto.egg-info/PKG-INFO` & `posuto-2023.6.1/posuto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posuto
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: Japanese Postal Code Data
 Home-page: https://github.com/polm/posuto.git
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `posuto-2023.6.0/setup.cfg` & `posuto-2023.6.1/setup.cfg`

 * *Files identical despite different names*

