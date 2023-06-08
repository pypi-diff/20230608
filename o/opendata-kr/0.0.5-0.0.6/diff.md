# Comparing `tmp/opendata_kr-0.0.5-py3-none-any.whl.zip` & `tmp/opendata_kr-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 14769 bytes, number of entries: 7
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-02 16:59 opendata/__init__.py
--rw-r--r--  2.0 unx     3744 b- defN 23-Jun-02 16:42 opendata/dataset.py
--rw-r--r--  2.0 unx    34523 b- defN 23-Jun-02 17:00 opendata_kr-0.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      478 b- defN 23-Jun-02 17:00 opendata_kr-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 17:00 opendata_kr-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-02 17:00 opendata_kr-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      556 b- defN 23-Jun-02 17:00 opendata_kr-0.0.5.dist-info/RECORD
-7 files, 39423 bytes uncompressed, 13779 bytes compressed:  65.0%
+Zip file size: 14804 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-08 15:03 opendata/__init__.py
+-rw-r--r--  2.0 unx     3859 b- defN 23-Jun-08 15:05 opendata/dataset.py
+-rw-r--r--  2.0 unx    34523 b- defN 23-Jun-08 15:13 opendata_kr-0.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      478 b- defN 23-Jun-08 15:13 opendata_kr-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 15:13 opendata_kr-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-08 15:13 opendata_kr-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      556 b- defN 23-Jun-08 15:13 opendata_kr-0.0.6.dist-info/RECORD
+7 files, 39538 bytes uncompressed, 13814 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: opendata/__init__.py
 Comment: 
 
 Filename: opendata/dataset.py
 Comment: 
 
-Filename: opendata_kr-0.0.5.dist-info/LICENSE
+Filename: opendata_kr-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: opendata_kr-0.0.5.dist-info/METADATA
+Filename: opendata_kr-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: opendata_kr-0.0.5.dist-info/WHEEL
+Filename: opendata_kr-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: opendata_kr-0.0.5.dist-info/top_level.txt
+Filename: opendata_kr-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: opendata_kr-0.0.5.dist-info/RECORD
+Filename: opendata_kr-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opendata/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.0.5'
+__version__ = '0.0.6'
```

## opendata/dataset.py

```diff
@@ -31,17 +31,21 @@
         if self.alt_url:
             metadata_url = 'http://data.jaen.kr/download?download_path=%2Fdata%2Ffiles%2FmySUNI%2Fdatasets%2F000-metadata%2Fmetadata.csv'
             cols = ['filename', 'alt_url']
             
         metadata = pd.read_csv(metadata_url)
         self.meta = {i: v for i, v in metadata.loc[metadata['id'] == self.id, cols].values}
 
-    def download(self):
+    def download(self, path=None):
         print('======= 다운로드 시작 =======\n')
-        dir_name = os.path.join(self.data_dir, self.name)
+        if path is None:
+            dir_name = os.path.join(self.data_dir, self.name)
+        else:
+            dir_name = path
+            
         if not os.path.isdir(dir_name):
             os.mkdir(dir_name)
             
         for idx, (filename, url) in enumerate(self.meta.items()):
             r = requests.get(url, stream=True)
             filepath = os.path.join(dir_name, filename)
 
@@ -81,20 +85,20 @@
         print('[서버] Dropbox')
     print(download_url)
     ret = pd.read_csv(download_url).iloc[:, :-1]
     ret.columns = ['데이터셋', '설명']
     return ret
 
 
-def download(name, data_dir='data', alt_url=True):
+def download(name, data_dir='data', alt_url=True, path=None):
     download_url = 'https://www.dropbox.com/s/95wzfrmoc4qrfvw/dataset.csv?dl=1'
     if alt_url:
         download_url = 'http://data.jaen.kr/download?download_path=%2Fdata%2Ffiles%2FmySUNI%2Fdatasets%2F000-metadata%2Fdataset.csv'
         print('[서버] Jaen')
     else:
         print('[서버] Dropbox')
     
     ds = pd.read_csv(download_url)
     row = ds.loc[ds['data'] == name]
     if len(row) > 0:
         dataset = Dataset(row['data'].values[0], row['data_desc'], row['id'].iloc[0], data_dir=data_dir)
-        dataset.download()
+        dataset.download(path=path)
```

## Comparing `opendata_kr-0.0.5.dist-info/LICENSE` & `opendata_kr-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

