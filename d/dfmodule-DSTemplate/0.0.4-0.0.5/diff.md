# Comparing `tmp/dfmodule_DSTemplate-0.0.4.tar.gz` & `tmp/dfmodule_DSTemplate-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfmodule_DSTemplate-0.0.4.tar", last modified: Wed Jun  7 03:33:07 2023, max compression
+gzip compressed data, was "dfmodule_DSTemplate-0.0.5.tar", last modified: Thu Jun  8 07:47:12 2023, max compression
```

## Comparing `dfmodule_DSTemplate-0.0.4.tar` & `dfmodule_DSTemplate-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 03:33:07.861474 dfmodule_DSTemplate-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-06-07 03:33:07.850474 dfmodule_DSTemplate-0.0.4/DS/
--rw-rw-rw-   0        0        0     2420 2023-06-07 03:07:03.000000 dfmodule_DSTemplate-0.0.4/DS/Get_by_dates.py
--rw-rw-rw-   0        0        0     1885 2023-06-07 03:32:56.000000 dfmodule_DSTemplate-0.0.4/DS/Loads.py
--rw-rw-rw-   0        0        0       55 2023-06-07 02:50:58.000000 dfmodule_DSTemplate-0.0.4/DS/__init__.py
--rw-rw-rw-   0        0        0      563 2023-06-07 03:33:07.860475 dfmodule_DSTemplate-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-07 02:36:22.000000 dfmodule_DSTemplate-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 03:33:07.860475 dfmodule_DSTemplate-0.0.4/dfmodule_DSTemplate.egg-info/
--rw-rw-rw-   0        0        0      563 2023-06-07 03:33:07.000000 dfmodule_DSTemplate-0.0.4/dfmodule_DSTemplate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-06-07 03:33:07.000000 dfmodule_DSTemplate-0.0.4/dfmodule_DSTemplate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 03:33:07.000000 dfmodule_DSTemplate-0.0.4/dfmodule_DSTemplate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-07 02:43:58.000000 dfmodule_DSTemplate-0.0.4/dfmodule_DSTemplate.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       45 2023-06-07 03:33:07.000000 dfmodule_DSTemplate-0.0.4/dfmodule_DSTemplate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2023-06-07 03:33:07.000000 dfmodule_DSTemplate-0.0.4/dfmodule_DSTemplate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 03:33:07.861474 dfmodule_DSTemplate-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-06-07 03:32:47.000000 dfmodule_DSTemplate-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:47:12.657719 dfmodule_DSTemplate-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-06-08 07:47:12.653732 dfmodule_DSTemplate-0.0.5/DS/
+-rw-rw-rw-   0        0        0     2571 2023-06-08 07:42:22.000000 dfmodule_DSTemplate-0.0.5/DS/Get_by_dates.py
+-rw-rw-rw-   0        0        0     1855 2023-06-08 07:24:27.000000 dfmodule_DSTemplate-0.0.5/DS/Loads.py
+-rw-rw-rw-   0        0        0       55 2023-06-08 07:00:37.000000 dfmodule_DSTemplate-0.0.5/DS/__init__.py
+-rw-rw-rw-   0        0        0      563 2023-06-08 07:47:12.657719 dfmodule_DSTemplate-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-06-08 07:46:17.000000 dfmodule_DSTemplate-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 07:47:12.657719 dfmodule_DSTemplate-0.0.5/dfmodule_DSTemplate.egg-info/
+-rw-rw-rw-   0        0        0      563 2023-06-08 07:47:12.000000 dfmodule_DSTemplate-0.0.5/dfmodule_DSTemplate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-06-08 07:47:12.000000 dfmodule_DSTemplate-0.0.5/dfmodule_DSTemplate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 07:47:12.000000 dfmodule_DSTemplate-0.0.5/dfmodule_DSTemplate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-08 07:47:12.000000 dfmodule_DSTemplate-0.0.5/dfmodule_DSTemplate.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       45 2023-06-08 07:47:12.000000 dfmodule_DSTemplate-0.0.5/dfmodule_DSTemplate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2023-06-08 07:47:12.000000 dfmodule_DSTemplate-0.0.5/dfmodule_DSTemplate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 07:47:12.657719 dfmodule_DSTemplate-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-06-08 07:40:24.000000 dfmodule_DSTemplate-0.0.5/setup.py
```

### Comparing `dfmodule_DSTemplate-0.0.4/DS/Get_by_dates.py` & `dfmodule_DSTemplate-0.0.5/DS/Get_by_dates.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,84 @@
 
 def get_obj(aws_access_key_id, 
             aws_secret_access_key, 
             aws_s3_bucket_name, 
-            date1, date2=None):
+            date1, date2=None,
+            item=None, grade=None):
     '''
     aws S3 에서 파일을 불러온 뒤\n
     gzip 압축을 풀고 json 데이터를 반환하는 함수
     '''
     from datetime import datetime, timedelta
     import boto3
-    import os
     import gzip
     import json
     import pandas as pd
 
-    # TODO sg : 금요일 회의때 선우님께 .env 파일 전달
-
     s3 = boto3.client(
                 service_name="s3",
                 region_name="ap-northeast-2",
                 aws_access_key_id=aws_access_key_id,
                 aws_secret_access_key=aws_secret_access_key,
             )
 
     if date2 == None:
-        year = date1[0:4]
-        month = date1[4:6]
+        try:
+            year = date1[0:4]
+            month = date1[4:6]
 
-        obj = s3.get_object(
-            Bucket = aws_s3_bucket_name,
-            Key = f'items/{year}/{month}/{date1}.json.gz'
-        )
+            obj = s3.get_object(
+                Bucket = aws_s3_bucket_name,
+                Key = f'items/{year}/{month}/{item}_{grade}/{date1}.json.gz'
+            )
 
-        with gzip.GzipFile(fileobj=obj.get('Body'), mode='r') as gz:
-            content = gz.read()
+            with gzip.GzipFile(fileobj=obj.get('Body'), mode='r') as gz:
+                content = gz.read()
 
-        json_data = json.loads(content)
-        df = pd.DataFrame(json_data)
-        return df
+            json_data = json.loads(content)
+            df = pd.DataFrame(json_data)
+            return df
+        except:
+            print('해당 날짜에 데이터가 없습니다.')
     
     else:
         start = date1
         end = date2
 
         start_date = datetime.strptime(start, '%Y%m%d')
         end_date = datetime.strptime(end, '%Y%m%d')
         dates = [(start_date + timedelta(days=i)).strftime("%Y%m%d") for i in range((end_date-start_date).days+1)]
         
         data = []
         for date in dates:
-            year = date[0:4]
-            month = date[4:6]
-
-            obj = s3.get_object(
-                Bucket = aws_s3_bucket_name,
-                Key = f'items/{year}/{month}/{date}.json.gz' # TODO sg : cp2_goguma_etl : 146 / 품목_등급 형식으로 ETL 코드로 AWS 폴더 동기화
-            )
-
-            with gzip.GzipFile(fileobj=obj.get('Body'), mode='r') as gz:
-                content = gz.read()
-
-            json_data = json.loads(content)
-            data += json_data
+            try:
+                year = date[0:4]
+                month = date[4:6]
+
+                obj = s3.get_object(
+                    Bucket = aws_s3_bucket_name,
+                    Key = f'items/{year}/{month}/{item}_{grade}/{date}.json.gz'
+                )
+
+                with gzip.GzipFile(fileobj=obj.get('Body'), mode='r') as gz:
+                    content = gz.read()
+
+                json_data = json.loads(content)
+                data += json_data
+            except:
+                pass
         df = pd.DataFrame(data)
         return df
 
 def save_local(data, file_path):
     '''
     불러온 json 데이터를 로컬에 저장하는 함수
     '''
     import json
     
     path = f'{file_path}.json'
     with open(path, 'w', encoding='utf-8') as f:
         json.dump(data, f, ensure_ascii=False, indent=4)
 
 if __name__ == "__main__":
-    data = get_obj('20230403', '20230407')
+    data = get_obj('20230403', '20230407', '고구마', '특(1등)')
     print(data)
```

### Comparing `dfmodule_DSTemplate-0.0.4/DS/Loads.py` & `dfmodule_DSTemplate-0.0.5/DS/Loads.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     '''
     aws S3에 연결하는 함수
 
     Returns
     -------
     s3 : boto3.client
     '''
-    import os
     import boto3
 
     try:
         s3 = boto3.client(
             service_name="s3",
             region_name="ap-northeast-2",
             aws_access_key_id=aws_access_key_id,
@@ -51,15 +50,14 @@
     Returns
     -------
     None.
     """
 
     import json
     import gzip
-    import os
 
     if aiModel is None:
         raise ValueError("aiModel is None")
 
     directory = f'items/AIModel/{filename}.gz'    
     compressed_data = gzip.compress(json.dumps(aiModel, ensure_ascii=False, indent=4).encode('utf-8'))
```

### Comparing `dfmodule_DSTemplate-0.0.4/PKG-INFO` & `dfmodule_DSTemplate-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfmodule_DSTemplate
-Version: 0.0.4
+Version: 0.0.5
 Summary: dfmodule for DE -> DS code transition
 Home-page: https://github.com/Data-Flower/dfmodule_DSTemplate
 Author: SG, JH
 Author-email: rimmoyee@example.com
 Keywords: dfmodule_DS, dfmodule, dfmodule_DSTemplate
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dfmodule_DSTemplate-0.0.4/dfmodule_DSTemplate.egg-info/PKG-INFO` & `dfmodule_DSTemplate-0.0.5/dfmodule_DSTemplate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfmodule-DSTemplate
-Version: 0.0.4
+Version: 0.0.5
 Summary: dfmodule for DE -> DS code transition
 Home-page: https://github.com/Data-Flower/dfmodule_DSTemplate
 Author: SG, JH
 Author-email: rimmoyee@example.com
 Keywords: dfmodule_DS, dfmodule, dfmodule_DSTemplate
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dfmodule_DSTemplate-0.0.4/setup.py` & `dfmodule_DSTemplate-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dfmodule_DSTemplate",
-    version="0.0.4",
+    version="0.0.5",
     description="dfmodule for DE -> DS code transition",
     author="SG, JH",
     author_email="rimmoyee@example.com",
     url="https://github.com/Data-Flower/dfmodule_DSTemplate",
     install_requires=['boto3', 'pandas', 'python-dotenv', 'requests', 'dfmodule'],
     packages=find_packages(exclude=['tests*']),
     keywords=['dfmodule_DS, dfmodule, dfmodule_DSTemplate'],
```

