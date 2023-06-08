# Comparing `tmp/cads_sdk-0.0.25-py3-none-any.whl.zip` & `tmp/cads_sdk-0.0.26-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 56553 bytes, number of entries: 18
--rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-05 09:30 cads_sdk/__init__.py
+Zip file size: 56540 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-08 03:23 cads_sdk/__init__.py
 -rw-rw-r--  2.0 unx     1264 b- defN 23-Apr-01 02:59 cads_sdk/nosql/__init__.py
 -rw-rw-r--  2.0 unx    11231 b- defN 23-Apr-17 08:04 cads_sdk/nosql/codec.py
 -rw-rw-r--  2.0 unx    86938 b- defN 23-May-18 09:04 cads_sdk/nosql/converter.py
--rw-rw-r--  2.0 unx    20911 b- defN 23-Jun-05 09:30 cads_sdk/nosql/display.py
+-rw-rw-r--  2.0 unx    20961 b- defN 23-Jun-08 03:25 cads_sdk/nosql/display.py
 -rw-rw-r--  2.0 unx     1187 b- defN 23-Apr-10 10:46 cads_sdk/nosql/etl.py
 -rw-rw-r--  2.0 unx     1291 b- defN 23-May-19 02:11 cads_sdk/nosql/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 14:03 cads_sdk/petastorm/__init__.py
 -rw-rw-r--  2.0 unx    19967 b- defN 23-Apr-10 04:34 cads_sdk/petastorm/dataset_metadata.py
 -rw-rw-r--  2.0 unx    10508 b- defN 23-Apr-10 07:19 cads_sdk/petastorm/fs_utils.py
 -rw-rw-r--  2.0 unx     5427 b- defN 23-Apr-10 04:42 cads_sdk/petastorm/utils.py
 -rw-rw-r--  2.0 unx    22554 b- defN 23-Apr-18 15:18 cads_sdk/pytorch/__init__.py
 -rw-rw-r--  2.0 unx    10653 b- defN 23-Apr-17 08:05 cads_sdk/pytorch/codec.py
 -rw-rw-r--  2.0 unx    78369 b- defN 23-Apr-20 08:23 cads_sdk/pytorch/converter.py
--rw-rw-r--  2.0 unx     7111 b- defN 23-Jun-05 09:30 cads_sdk-0.0.25.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-05 09:30 cads_sdk-0.0.25.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-05 09:30 cads_sdk-0.0.25.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1480 b- defN 23-Jun-05 09:30 cads_sdk-0.0.25.dist-info/RECORD
-18 files, 280257 bytes uncompressed, 54147 bytes compressed:  80.7%
+-rw-rw-r--  2.0 unx     7123 b- defN 23-Jun-08 03:27 cads_sdk-0.0.26.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-08 03:27 cads_sdk-0.0.26.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-08 03:27 cads_sdk-0.0.26.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1480 b- defN 23-Jun-08 03:27 cads_sdk-0.0.26.dist-info/RECORD
+18 files, 280319 bytes uncompressed, 54134 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: cads_sdk/pytorch/codec.py
 Comment: 
 
 Filename: cads_sdk/pytorch/converter.py
 Comment: 
 
-Filename: cads_sdk-0.0.25.dist-info/METADATA
+Filename: cads_sdk-0.0.26.dist-info/METADATA
 Comment: 
 
-Filename: cads_sdk-0.0.25.dist-info/WHEEL
+Filename: cads_sdk-0.0.26.dist-info/WHEEL
 Comment: 
 
-Filename: cads_sdk-0.0.25.dist-info/top_level.txt
+Filename: cads_sdk-0.0.26.dist-info/top_level.txt
 Comment: 
 
-Filename: cads_sdk-0.0.25.dist-info/RECORD
+Filename: cads_sdk-0.0.26.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cads_sdk/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.25'
+__version__ = '0.0.26'
 
 __doc__ = """
 cads-sdk: Functions to help Data Scientist work more effectively with unstructured data and datalake
 =====================================================================
 **cads-sdk**
 Function to convert 
 -------------
```

## cads_sdk/nosql/display.py

```diff
@@ -495,14 +495,15 @@
             df = spark.sql(f"""select {columns} from delta.`{self.input_path}` """)
         else:
             df = spark.sql(f"""select {columns} from parquet.`{self.input_path}`""")
         return df
     
     
     def write_to_folder(self, row):
+        self.output.append_display_data(row.path)
         if '.pcm' in row.path:
             data = np.frombuffer(row.audio, dtype = 'float64')
             from IPython.display import Audio, display
             self.output.append_display_data(Audio(data, rate=int(row.samplerate)))
             
         elif '.wav' in row.path:
             from scipy.io import wavfile
```

## Comparing `cads_sdk-0.0.25.dist-info/METADATA` & `cads_sdk-0.0.26.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cads-sdk
-Version: 0.0.25
+Version: 0.0.26
 Summary: Function to help Data Scientist work more effectively with DWH
 Home-page: http://git.bigdata.local/data-engineers/sdk/utilities
 Author: duyvnc
 Author-email: duyvnc@fpt.com.vn
 License: duyvnc
-Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Requires-Dist: spark-sdk (>=0.4.20)
 Requires-Dist: opencv-python
 Requires-Dist: Pillow
 Requires-Dist: scipy
 Requires-Dist: pydub
@@ -83,18 +82,18 @@
 ```python
 from cads_sdk.nosql.converter import ConvertFromFolderImage
 
 converter = ConvertFromFolderImage(
               input_path="/path/to/folder/**/*.jpg",
               input_type = 'jpg' # 'jpg' | ('jpg', 'png')
               input_recursive = True,
-
+              
               #setting output
               output_path = f"file:/output/path/image_storage",
-
+              
               # setting converter
               image_type = 'jpg',
               image_color = 3,
               resize_mode=None, # |padding|resize
               size = [(212,212),
                      (597, 597)],
              )
@@ -104,15 +103,15 @@
 # convert directly from .zip file to parquet
 from cads_sdk.nosql.converter import ConvertFromZipImage
 
 converter = ConvertFromZipImage(
               input_path="/path/to/image_storage/ETHZ.zip",
               input_recursive = True, # will loop through folder to get all pattern
               input_type = 'jpg' # 'jpg' | ('jpg', 'png')
-
+    
               #setting output
               output_path = f"file:/output/path/img_ethz.parquet",
               table_name = 'img_ethz',
               database = 'default',
               file_format = 'parquet', # delta|parquet
               compression = 'zstd', # zstd|snappy
               # setting converter
@@ -207,9 +206,7 @@
 converter.execute()
 ```
 ### For more information use class instance
 ```python
 ConvertFromFolderImage.__doc__
 ```
 
-
-
```

## Comparing `cads_sdk-0.0.25.dist-info/RECORD` & `cads_sdk-0.0.26.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-cads_sdk/__init__.py,sha256=eyC0S1MrgjKdxxp0dvuaG_BNw7s7IE4mOzhIsa6FOVw,1265
+cads_sdk/__init__.py,sha256=NvUb-g5CIN1tFa1dnXVjSzIBIrIYax3v3fewap5c6Fs,1265
 cads_sdk/nosql/__init__.py,sha256=Yu2Zt5cpSXSLqIRAvIxaXOtoyj3yBisGTbnFlH4UD2A,1264
 cads_sdk/nosql/codec.py,sha256=Z0RdndLtSHAnqHOpDGE-Wb_jD9eIWvKiuX4Yj1KudX4,11231
 cads_sdk/nosql/converter.py,sha256=TUVOQIEqE60zpoxZbyc9fcgaFOVkYy37ZmwtBVG8LoI,86938
-cads_sdk/nosql/display.py,sha256=5GlofvnWxw4nzz9hOeee3v_UpAYpRmdI59WNmkLIbgA,20911
+cads_sdk/nosql/display.py,sha256=pUA_qTcNP3Vra3oZtUd4RAR3aXmyMqCZIZ3wrF8p_QE,20961
 cads_sdk/nosql/etl.py,sha256=PWhXNWZyIFFEEvTIoUNuKK5cDqTy8A4FPn07BGMr0Vk,1187
 cads_sdk/nosql/utils.py,sha256=nQVGBLBx7mhIgLulY1_bUefBEOqHhZbht4jI9E9azuY,1291
 cads_sdk/petastorm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cads_sdk/petastorm/dataset_metadata.py,sha256=3sXVulFmpZEJC7mM0cwEXBVmB-0TD-U746ltLcsqIno,19967
 cads_sdk/petastorm/fs_utils.py,sha256=qFAzfi_VM4Rr2mBW8JsgxPUojLFFQGZI93MpI4sL_Xo,10508
 cads_sdk/petastorm/utils.py,sha256=CyeRPL_ih9wC1BdElvf1VknF1lBdNvJxgldSiU1OkFs,5427
 cads_sdk/pytorch/__init__.py,sha256=qyLEDZ_2BXLQBqievSj4wg2h4EQf9AdbIi_1SKFyIsM,22554
 cads_sdk/pytorch/codec.py,sha256=5XZulM21El-lsL3jZMexnJAHc2cIeRZj721PMuPhsJU,10653
 cads_sdk/pytorch/converter.py,sha256=lT2c3ix8Q35TEOUdFzlQVIzf7GfRklomwrdfRaXcY7k,78369
-cads_sdk-0.0.25.dist-info/METADATA,sha256=oOe24RoJjXMbuR2dg3QyND59ZY1qoPXVNts9Y8vagT4,7111
-cads_sdk-0.0.25.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-cads_sdk-0.0.25.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
-cads_sdk-0.0.25.dist-info/RECORD,,
+cads_sdk-0.0.26.dist-info/METADATA,sha256=t10vIrxsXhYZt0FD3P8CcVK64838n_HewHWAz1Wga8g,7123
+cads_sdk-0.0.26.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+cads_sdk-0.0.26.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
+cads_sdk-0.0.26.dist-info/RECORD,,
```

