# Comparing `tmp/hpolib_extractor-0.0.2-py3-none-any.whl.zip` & `tmp/hpolib_extractor-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6781 bytes, number of entries: 7
--rw-rw-r--  2.0 unx      329 b- defN 23-Jun-07 15:29 hpolib_extractor/__init__.py
--rw-rw-r--  2.0 unx     2746 b- defN 23-Jun-07 15:20 hpolib_extractor/extractor.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-07 15:30 hpolib_extractor-0.0.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx      311 b- defN 23-Jun-07 15:30 hpolib_extractor-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 15:30 hpolib_extractor-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       17 b- defN 23-Jun-07 15:30 hpolib_extractor-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      601 b- defN 23-Jun-07 15:30 hpolib_extractor-0.0.2.dist-info/RECORD
-7 files, 14856 bytes uncompressed, 5705 bytes compressed:  61.6%
+Zip file size: 6790 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx      330 b- defN 23-Jun-08 08:53 hpolib_extractor/__init__.py
+-rw-rw-r--  2.0 unx     2720 b- defN 23-Jun-08 08:42 hpolib_extractor/extractor.py
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-08 08:56 hpolib_extractor-1.0.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      312 b- defN 23-Jun-08 08:56 hpolib_extractor-1.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-08 08:56 hpolib_extractor-1.0.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       17 b- defN 23-Jun-08 08:56 hpolib_extractor-1.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      601 b- defN 23-Jun-08 08:56 hpolib_extractor-1.0.0.dist-info/RECORD
+7 files, 14832 bytes uncompressed, 5714 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: hpolib_extractor/__init__.py
 Comment: 
 
 Filename: hpolib_extractor/extractor.py
 Comment: 
 
-Filename: hpolib_extractor-0.0.2.dist-info/LICENSE
+Filename: hpolib_extractor-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: hpolib_extractor-0.0.2.dist-info/METADATA
+Filename: hpolib_extractor-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: hpolib_extractor-0.0.2.dist-info/WHEEL
+Filename: hpolib_extractor-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: hpolib_extractor-0.0.2.dist-info/top_level.txt
+Filename: hpolib_extractor-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: hpolib_extractor-0.0.2.dist-info/RECORD
+Filename: hpolib_extractor-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hpolib_extractor/__init__.py

```diff
@@ -1,12 +1,12 @@
 from hpolib_extractor.extractor import extract
 
 
-__version__ = "0.0.2"
+__version__ = "1.0.0"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
-__url__ = "https://github.com/nabenabe0928/hpolib-extractor"
+__url__ = "https://github.com/nabenabe0928/hpolib-extractor/"
 
 
 __all__ = ["extract"]
```

## hpolib_extractor/extractor.py

```diff
@@ -57,15 +57,15 @@
         for it in tqdm(itertools.product(*(list(v) for v in SEARCH_SPACE.values())), total=N_ENTRIES):
             config = {k: v for k, v in zip(SEARCH_SPACE.keys(), it)}
             key = json.dumps(config, sort_keys=True)
             target_data = self._db[key]
             self._collected_data[key] = {
                 loss_key: [{e: float(target_data[loss_key][s][e]) for e in self._epochs_id} for s in range(n_seeds)],
                 runtime_key: [float(target_data[runtime_key][s]) for s in range(n_seeds)],
-                n_params_key: [float(target_data[n_params_key][s]) for s in range(n_seeds)],
+                n_params_key: float(target_data[n_params_key][0]),
             }
 
 
 def extract(data_dir: str, epochs: List[int]):
     for i in range(4):
         extractor = HPOLibExtractor(dataset_id=i, epochs=epochs, data_dir=data_dir)
         print(f"Start extracting {extractor.dataset_name}")
```

## Comparing `hpolib_extractor-0.0.2.dist-info/LICENSE` & `hpolib_extractor-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hpolib_extractor-0.0.2.dist-info/RECORD` & `hpolib_extractor-1.0.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-hpolib_extractor/__init__.py,sha256=lwi1PclAtNfGwLx4Yh_5xSH7_fd8rY_yaQR7rhnnsOs,329
-hpolib_extractor/extractor.py,sha256=SBaBIL3vDHh82olPuHJJ3X1rxS7ej1AUfNze_7JXeVw,2746
-hpolib_extractor-0.0.2.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
-hpolib_extractor-0.0.2.dist-info/METADATA,sha256=g-5Y34iofov_O_OlWd5hgkiz5s5YsGxaw204f59h6II,311
-hpolib_extractor-0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-hpolib_extractor-0.0.2.dist-info/top_level.txt,sha256=XLMeFfnejGFDNOCBcSl7hSR9dJLiD6xEujjydHq6CyY,17
-hpolib_extractor-0.0.2.dist-info/RECORD,,
+hpolib_extractor/__init__.py,sha256=y4ZTrFwYRMzHhJj-rNUUcXHFvMuRMMia_y2mBNYxs40,330
+hpolib_extractor/extractor.py,sha256=bcAaSyC7Xu7l_YDd5BkF9Lnt9jHzn9b13J-ERSgSDbo,2720
+hpolib_extractor-1.0.0.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
+hpolib_extractor-1.0.0.dist-info/METADATA,sha256=782ZZKiFk_SaagZNjvsCkXxgSdkfdNQ9qLddHNMJMrA,312
+hpolib_extractor-1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+hpolib_extractor-1.0.0.dist-info/top_level.txt,sha256=XLMeFfnejGFDNOCBcSl7hSR9dJLiD6xEujjydHq6CyY,17
+hpolib_extractor-1.0.0.dist-info/RECORD,,
```

