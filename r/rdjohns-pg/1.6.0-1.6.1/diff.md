# Comparing `tmp/rdjohns_pg-1.6.0.tar.gz` & `tmp/rdjohns_pg-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdjohns_pg-1.6.0.tar", last modified: Wed Apr 19 09:16:14 2023, max compression
+gzip compressed data, was "rdjohns_pg-1.6.1.tar", last modified: Thu Jun  8 10:41:03 2023, max compression
```

## Comparing `rdjohns_pg-1.6.0.tar` & `rdjohns_pg-1.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 09:16:14.093283 rdjohns_pg-1.6.0/
--rw-rw-rw-   0        0        0     1088 2022-09-06 08:48:21.000000 rdjohns_pg-1.6.0/LICENSE
--rw-rw-rw-   0        0        0      904 2023-04-19 09:16:14.090349 rdjohns_pg-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      442 2022-09-06 09:59:58.000000 rdjohns_pg-1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 09:16:14.071798 rdjohns_pg-1.6.0/rdjohns_pg/
--rw-rw-rw-   0        0        0     3386 2022-12-06 10:24:32.000000 rdjohns_pg-1.6.0/rdjohns_pg/Datatable_Data.py
--rw-rw-rw-   0        0        0     7827 2022-11-17 16:53:02.000000 rdjohns_pg-1.6.0/rdjohns_pg/Datatable_JS.py
--rw-rw-rw-   0        0        0     6847 2023-04-19 09:01:00.000000 rdjohns_pg-1.6.0/rdjohns_pg/InsertComand.py
--rw-rw-rw-   0        0        0      873 2023-01-24 12:35:37.000000 rdjohns_pg-1.6.0/rdjohns_pg/Str_verification.py
--rw-rw-rw-   0        0        0     1704 2022-09-12 08:15:37.000000 rdjohns_pg-1.6.0/rdjohns_pg/Write_log.py
--rw-rw-rw-   0        0        0      195 2022-12-07 09:14:14.000000 rdjohns_pg-1.6.0/rdjohns_pg/__init__.py
--rw-rw-rw-   0        0        0      355 2022-09-09 13:28:53.000000 rdjohns_pg-1.6.0/rdjohns_pg/date.py
--rw-rw-rw-   0        0        0     4589 2023-03-24 12:53:47.000000 rdjohns_pg-1.6.0/rdjohns_pg/rdjohns_pg.py
-drwxrwxrwx   0        0        0        0 2023-04-19 09:16:14.089372 rdjohns_pg-1.6.0/rdjohns_pg.egg-info/
--rw-rw-rw-   0        0        0      904 2023-04-19 09:16:13.000000 rdjohns_pg-1.6.0/rdjohns_pg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-04-19 09:16:13.000000 rdjohns_pg-1.6.0/rdjohns_pg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 09:16:13.000000 rdjohns_pg-1.6.0/rdjohns_pg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-19 09:16:13.000000 rdjohns_pg-1.6.0/rdjohns_pg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 09:16:14.094254 rdjohns_pg-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1090 2023-04-19 09:01:10.000000 rdjohns_pg-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:41:03.421189 rdjohns_pg-1.6.1/
+-rw-rw-rw-   0        0        0     1088 2022-09-06 08:48:21.000000 rdjohns_pg-1.6.1/LICENSE
+-rw-rw-rw-   0        0        0      904 2023-06-08 10:41:03.413378 rdjohns_pg-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2022-09-06 09:59:58.000000 rdjohns_pg-1.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 10:41:03.188783 rdjohns_pg-1.6.1/rdjohns_pg/
+-rw-rw-rw-   0        0        0     3386 2022-12-06 10:24:32.000000 rdjohns_pg-1.6.1/rdjohns_pg/Datatable_Data.py
+-rw-rw-rw-   0        0        0     7823 2023-06-08 10:38:02.000000 rdjohns_pg-1.6.1/rdjohns_pg/Datatable_JS.py
+-rw-rw-rw-   0        0        0     6847 2023-04-19 09:01:00.000000 rdjohns_pg-1.6.1/rdjohns_pg/InsertComand.py
+-rw-rw-rw-   0        0        0      873 2023-01-24 12:35:37.000000 rdjohns_pg-1.6.1/rdjohns_pg/Str_verification.py
+-rw-rw-rw-   0        0        0     1704 2022-09-12 08:15:37.000000 rdjohns_pg-1.6.1/rdjohns_pg/Write_log.py
+-rw-rw-rw-   0        0        0      195 2022-12-07 09:14:14.000000 rdjohns_pg-1.6.1/rdjohns_pg/__init__.py
+-rw-rw-rw-   0        0        0      355 2022-09-09 13:28:53.000000 rdjohns_pg-1.6.1/rdjohns_pg/date.py
+-rw-rw-rw-   0        0        0     4589 2023-03-24 12:53:47.000000 rdjohns_pg-1.6.1/rdjohns_pg/rdjohns_pg.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:41:03.277645 rdjohns_pg-1.6.1/rdjohns_pg.egg-info/
+-rw-rw-rw-   0        0        0      904 2023-06-08 10:41:01.000000 rdjohns_pg-1.6.1/rdjohns_pg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-06-08 10:41:02.000000 rdjohns_pg-1.6.1/rdjohns_pg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 10:41:01.000000 rdjohns_pg-1.6.1/rdjohns_pg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-08 10:41:01.000000 rdjohns_pg-1.6.1/rdjohns_pg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 10:41:03.422167 rdjohns_pg-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2023-06-08 10:38:59.000000 rdjohns_pg-1.6.1/setup.py
```

### Comparing `rdjohns_pg-1.6.0/LICENSE` & `rdjohns_pg-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rdjohns_pg-1.6.0/PKG-INFO` & `rdjohns_pg-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdjohns_pg
-Version: 1.6.0
+Version: 1.6.1
 Summary: Use for the multiple delete, update or insert and select!
 Home-page: https://github.com/RDJohns/rdjohns_pg
 Author: David Johns
 Author-email: rakotonindrianajohns@email.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rdjohns_pg-1.6.0/rdjohns_pg/Datatable_Data.py` & `rdjohns_pg-1.6.1/rdjohns_pg/Datatable_Data.py`

 * *Files identical despite different names*

### Comparing `rdjohns_pg-1.6.0/rdjohns_pg/Datatable_JS.py` & `rdjohns_pg-1.6.1/rdjohns_pg/Datatable_JS.py`

 * *Files 4% similar despite different names*

```diff
@@ -395,96 +395,95 @@
 000018a0: 2020 2020 2020 2020 2020 2020 2020 6275                bu
 000018b0: 7474 6f6e 733a 205b 0d0a 2020 2020 2020  ttons: [..      
 000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000018d0: 2020 2020 2020 2020 2020 2020 2020 2222                ""
 000018e0: 222b 7365 6c66 2e62 6f75 746f 6e2b 2222  "+self.bouton+""
 000018f0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
 00001900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001910: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
+00001910: 2020 2020 2020 202f 2a7b 0d0a 2020 2020         /*{..    
 00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001940: 2020 6578 7465 6e64 3a20 2265 7863 656c    extend: "excel
-00001950: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00001940: 2020 2020 6578 7465 6e64 3a20 2265 7863      extend: "exc
+00001950: 656c 222c 0d0a 2020 2020 2020 2020 2020  el",..          
 00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001970: 2020 2020 2020 2020 2020 2020 7469 746c              titl
-00001980: 653a 2027 2222 222b 7365 6c66 2e74 6974  e: '"""+self.tit
-00001990: 7265 2b22 2222 272c 0d0a 2020 2020 2020  re+"""',..      
+00001970: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+00001980: 746c 653a 2027 2222 222b 7365 6c66 2e74  tle: '"""+self.t
+00001990: 6974 7265 2b22 2222 272c 0d0a 2020 2020  itre+"""',..    
 000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019c0: 2020 7465 7874 3a20 273c 7370 616e 2063    text: '<span c
-000019d0: 6c61 7373 3d22 6661 2066 612d 6669 6c65  lass="fa fa-file
-000019e0: 2d65 7863 656c 2d6f 223e 3c2f 7370 616e  -excel-o"></span
-000019f0: 3e20 4578 6365 6c27 2c0d 0a20 2020 2020  > Excel',..     
+000019c0: 2020 2020 7465 7874 3a20 273c 7370 616e      text: '<span
+000019d0: 2063 6c61 7373 3d22 6661 2066 612d 6669   class="fa fa-fi
+000019e0: 6c65 2d65 7863 656c 2d6f 223e 3c2f 7370  le-excel-o"></sp
+000019f0: 616e 3e20 4578 6365 6c27 2c0d 0a20 2020  an> Excel',..   
 00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a20: 2020 2065 7870 6f72 744f 7074 696f 6e73     exportOptions
-00001a30: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
+00001a20: 2020 2020 2065 7870 6f72 744f 7074 696f       exportOptio
+00001a30: 6e73 3a20 7b0d 0a20 2020 2020 2020 2020  ns: {..         
 00001a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a60: 202f 2a63 6f6c 756d 6e73 3a20 223a 7669   /*columns: ":vi
-00001a70: 7369 626c 6522 2c2a 2f0d 0a20 2020 2020  sible",*/..     
+00001a60: 2020 2063 6f6c 756d 6e73 3a20 223a 7669     columns: ":vi
+00001a70: 7369 626c 6522 2c0d 0a20 2020 2020 2020  sible",..       
 00001a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001aa0: 2020 2020 2020 2063 6f6c 756d 6e73 3a20         columns: 
-00001ab0: 2274 6865 6164 2074 683a 6e6f 7428 2e6e  "thead th:not(.n
-00001ac0: 6f45 7870 6f72 7429 220d 0a20 2020 2020  oExport)"..     
+00001aa0: 2020 2020 2063 6f6c 756d 6e73 3a20 2274       columns: "t
+00001ab0: 6865 6164 2074 683a 6e6f 7428 2e6e 6f45  head th:not(.noE
+00001ac0: 7870 6f72 7429 220d 0a20 2020 2020 2020  xport)"..       
 00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001af0: 2020 207d 0d0a 0909 0909 0909 0909 097d     }...........}
-00001b00: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001af0: 207d 0d0a 0909 0909 0909 0909 097d 2c0d   }...........},.
+00001b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b20: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
+00001b20: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
 00001b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b50: 2020 6578 7465 6e64 3a20 2263 6f70 7922    extend: "copy"
-00001b60: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001b50: 6578 7465 6e64 3a20 2263 6f70 7922 2c0d  extend: "copy",.
+00001b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b80: 2020 2020 2020 2020 2020 2074 6974 6c65             title
-00001b90: 3a20 2722 2222 2b73 656c 662e 7469 7472  : '"""+self.titr
-00001ba0: 652b 2222 2227 2c0d 0a20 2020 2020 2020  e+"""',..       
+00001b80: 2020 2020 2020 2020 2074 6974 6c65 3a20           title: 
+00001b90: 2722 2222 2b73 656c 662e 7469 7472 652b  '"""+self.titre+
+00001ba0: 2222 2227 2c0d 0a20 2020 2020 2020 2020  """',..         
 00001bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bd0: 2074 6578 743a 2027 3c73 7061 6e20 636c   text: '<span cl
-00001be0: 6173 733d 2266 6120 6661 2d66 696c 6573  ass="fa fa-files
-00001bf0: 2d6f 223e 3c2f 7370 616e 3e20 436f 7079  -o"></span> Copy
-00001c00: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00001bc0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00001bd0: 6578 743a 2027 3c73 7061 6e20 636c 6173  ext: '<span clas
+00001be0: 733d 2266 6120 6661 2d66 696c 6573 2d6f  s="fa fa-files-o
+00001bf0: 223e 3c2f 7370 616e 3e20 436f 7079 272c  "></span> Copy',
+00001c00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00001c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c20: 2020 2020 2020 2020 2020 2020 6578 706f              expo
-00001c30: 7274 4f70 7469 6f6e 733a 207b 0d0a 2020  rtOptions: {..  
+00001c20: 2020 2020 2020 2020 2020 6578 706f 7274            export
+00001c30: 4f70 7469 6f6e 733a 207b 0d0a 2020 2020  Options: {..    
 00001c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c60: 2020 2020 2020 2020 2020 2f2a 636f 6c75            /*colu
-00001c70: 6d6e 733a 2022 3a76 6973 6962 6c65 222a  mns: ":visible"*
-00001c80: 2f0d 0a20 2020 2020 2020 2020 2020 2020  /..             
+00001c60: 2020 2020 2020 2020 636f 6c75 6d6e 733a          columns:
+00001c70: 2022 3a76 6973 6962 6c65 220d 0a20 2020   ":visible"..   
+00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ca0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001cb0: 6f6c 756d 6e73 3a20 2274 6865 6164 2074  olumns: "thead t
-00001cc0: 683a 6e6f 7428 2e6e 6f45 7870 6f72 7429  h:not(.noExport)
-00001cd0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00001ca0: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
+00001cb0: 3a20 2274 6865 6164 2074 683a 6e6f 7428  : "thead th:not(
+00001cc0: 2e6e 6f45 7870 6f72 7429 220d 0a20 2020  .noExport)"..   
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cf0: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+00001cf0: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
 00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d20: 2020 7d2c 0d0a 0909 0909 0909 0909 0922    },..........."
-00001d30: 2222 2b73 656c 662e 6274 6e5f 7064 665f  ""+self.btn_pdf_
-00001d40: 636f 7079 2b22 2222 0d0a 2020 2020 2020  copy+"""..      
+00001d10: 2020 2020 2020 2020 2020 2020 7d2c 2a2f              },*/
+00001d20: 0d0a 0909 0909 0909 0909 0922 2222 2b73  ..........."""+s
+00001d30: 656c 662e 6274 6e5f 7064 665f 636f 7079  elf.btn_pdf_copy
+00001d40: 2b22 2222 0d0a 2020 2020 2020 2020 2020  +"""..          
 00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d60: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
+00001d60: 2020 2020 2020 5d0d 0a20 2020 2020 2020        ]..       
 00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d80: 2020 2020 2020 2020 207d 292e 636f 6c75           }).colu
-00001d90: 6d6e 732e 6164 6a75 7374 2829 2e64 7261  mns.adjust().dra
-00001da0: 7728 293b 0d0a 2020 2020 2020 2020 2020  w();..          
-00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001dc0: 2020 2428 222e 6474 2d62 7574 746f 6e73    $(".dt-buttons
-00001dd0: 2229 2e63 7373 2822 666c 6f61 7422 2c22  ").css("float","
-00001de0: 7269 6768 7422 293b 0d0a 2020 2020 2020  right");..      
+00001d80: 2020 2020 207d 292e 636f 6c75 6d6e 732e       }).columns.
+00001d90: 6164 6a75 7374 2829 2e64 7261 7728 293b  adjust().draw();
+00001da0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2428                $(
+00001dc0: 222e 6474 2d62 7574 746f 6e73 2229 2e63  ".dt-buttons").c
+00001dd0: 7373 2822 666c 6f61 7422 2c22 7269 6768  ss("float","righ
+00001de0: 7422 293b 0d0a 2020 2020 2020 2020 2020  t");..          
 00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e00: 2020 2020 2020 2428 2264 6976 2e74 6f6f        $("div.too
-00001e10: 6c62 6172 2229 2e63 7373 2822 666c 6f61  lbar").css("floa
-00001e20: 7422 2c22 7269 6768 7422 293b 0d0a 2020  t","right");..  
+00001e00: 2020 2428 2264 6976 2e74 6f6f 6c62 6172    $("div.toolbar
+00001e10: 2229 2e63 7373 2822 666c 6f61 7422 2c22  ").css("float","
+00001e20: 7269 6768 7422 293b 0d0a 2020 2020 2020  right");..      
 00001e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e40: 2020 2020 2020 2020 2020 2222 222b 7365            """+se
-00001e50: 6c66 2e73 6372 6970 742b 2222 220d 0a20  lf.script+""".. 
+00001e40: 2020 2020 2020 2222 222b 7365 6c66 2e73        """+self.s
+00001e50: 6372 6970 742b 2222 220d 0a20 2020 2020  cript+"""..     
 00001e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e70: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00001e80: 2020 2020 7265 7475 726e 206f 7574 7075      return outpu
-00001e90: 740d 0a                                  t..
+00001e70: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00001e80: 7265 7475 726e 206f 7574 7075 740d 0a    return output..
```

### Comparing `rdjohns_pg-1.6.0/rdjohns_pg/InsertComand.py` & `rdjohns_pg-1.6.1/rdjohns_pg/InsertComand.py`

 * *Files identical despite different names*

### Comparing `rdjohns_pg-1.6.0/rdjohns_pg/Str_verification.py` & `rdjohns_pg-1.6.1/rdjohns_pg/Str_verification.py`

 * *Files identical despite different names*

### Comparing `rdjohns_pg-1.6.0/rdjohns_pg/Write_log.py` & `rdjohns_pg-1.6.1/rdjohns_pg/Write_log.py`

 * *Files identical despite different names*

### Comparing `rdjohns_pg-1.6.0/rdjohns_pg/rdjohns_pg.py` & `rdjohns_pg-1.6.1/rdjohns_pg/rdjohns_pg.py`

 * *Files identical despite different names*

### Comparing `rdjohns_pg-1.6.0/rdjohns_pg.egg-info/PKG-INFO` & `rdjohns_pg-1.6.1/rdjohns_pg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdjohns-pg
-Version: 1.6.0
+Version: 1.6.1
 Summary: Use for the multiple delete, update or insert and select!
 Home-page: https://github.com/RDJohns/rdjohns_pg
 Author: David Johns
 Author-email: rakotonindrianajohns@email.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rdjohns_pg-1.6.0/setup.py` & `rdjohns_pg-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rdjohns_pg",
-    version="1.6.0",
+    version="1.6.1",
     author="David Johns",
     author_email="rakotonindrianajohns@email.com",
     description="Use for the multiple delete, update or insert and select!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/RDJohns/rdjohns_pg",
     packages=setuptools.find_packages(),
```

