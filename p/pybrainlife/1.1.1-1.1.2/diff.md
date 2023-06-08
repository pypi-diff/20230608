# Comparing `tmp/pybrainlife-1.1.1.tar.gz` & `tmp/pybrainlife-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybrainlife-1.1.1.tar", max compression
+gzip compressed data, was "pybrainlife-1.1.2.tar", max compression
```

## Comparing `pybrainlife-1.1.1.tar` & `pybrainlife-1.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2370 2023-02-13 20:00:45.821811 pybrainlife-1.1.1/README.md
--rw-r--r--   0        0        0       22 2023-02-13 15:57:42.245812 pybrainlife-1.1.1/pybrainlife/__init__.py
--rwxr-xr-x   0        0        0    19170 2023-05-20 02:51:12.704559 pybrainlife-1.1.1/pybrainlife/data/collect.py
--rwxr-xr-x   0        0        0    19287 2023-04-12 21:52:50.584436 pybrainlife-1.1.1/pybrainlife/data/manipulate.py
--rw-r--r--   0        0        0     4011 2023-02-13 15:57:42.245812 pybrainlife-1.1.1/pybrainlife/vis/__pycache__/data.cpython-38.pyc
--rw-r--r--   0        0        0     7091 2023-02-13 15:57:42.245812 pybrainlife-1.1.1/pybrainlife/vis/__pycache__/plots.cpython-38.pyc
--rwxr-xr-x   0        0        0    19483 2023-02-13 19:55:42.426571 pybrainlife-1.1.1/pybrainlife/vis/plots.py
--rw-r--r--   0        0        0      747 2023-05-20 02:51:25.376524 pybrainlife-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3488 1970-01-01 00:00:00.000000 pybrainlife-1.1.1/setup.py
--rw-r--r--   0        0        0     3426 1970-01-01 00:00:00.000000 pybrainlife-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-02-13 20:00:45.821811 pybrainlife-1.1.2/README.md
+-rw-r--r--   0        0        0       22 2023-02-13 15:57:42.245812 pybrainlife-1.1.2/pybrainlife/__init__.py
+-rwxr-xr-x   0        0        0    19744 2023-06-08 19:08:27.612900 pybrainlife-1.1.2/pybrainlife/data/collect.py
+-rwxr-xr-x   0        0        0    19287 2023-04-12 21:52:50.584436 pybrainlife-1.1.2/pybrainlife/data/manipulate.py
+-rw-r--r--   0        0        0     4011 2023-02-13 15:57:42.245812 pybrainlife-1.1.2/pybrainlife/vis/__pycache__/data.cpython-38.pyc
+-rw-r--r--   0        0        0     7091 2023-02-13 15:57:42.245812 pybrainlife-1.1.2/pybrainlife/vis/__pycache__/plots.cpython-38.pyc
+-rwxr-xr-x   0        0        0    19483 2023-02-13 19:55:42.426571 pybrainlife-1.1.2/pybrainlife/vis/plots.py
+-rw-r--r--   0        0        0      747 2023-06-08 19:08:41.676869 pybrainlife-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3488 1970-01-01 00:00:00.000000 pybrainlife-1.1.2/setup.py
+-rw-r--r--   0        0        0     3426 1970-01-01 00:00:00.000000 pybrainlife-1.1.2/PKG-INFO
```

### Comparing `pybrainlife-1.1.1/README.md` & `pybrainlife-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.1.1/pybrainlife/data/collect.py` & `pybrainlife-1.1.2/pybrainlife/data/collect.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,106 +196,111 @@
     
     return ctr
 
 ## this function is the wrapper function that calls all the prevouis functions to generate a dataframe for the entire project of the appropriate datatype
 # def collect_data(datatype,datatype_tags,tags,filename,outPath,net_adj): # net_adj no longer necessary
 def collect_data(datatype,datatype_tags,tags,filename,outPath,duplicates=False):
 
-    # grab path and data objects
-    objects = requests.get('https://brainlife.io/api/warehouse/secondary/list/%s'%os.environ['PROJECT_ID']).json()
+    if datatype in ['cortex_example','tractmeasures_example']:
+        data = pd.read_csv('./sample-data/'+datatype.replace('_example','')+'.csv')
+        obj_tags = ['example_data']
+        obj_datatype_tags = ['example_data']
+    else:
+        # grab path and data objects
+        objects = requests.get('https://brainlife.io/api/warehouse/secondary/list/%s'%os.environ['PROJECT_ID']).json()
 
-    # subjects and paths
-    subjects = []
-    sessions = []
-    paths = []
-    finish_dates = []
-    obj_datatype_tags = []
-    obj_tags = []
-
-    # set up output
-    data = pd.DataFrame()
-
-    # loop through objects and find appropriate objects based on datatype, datatype_tags, and tags. can include drop tags ('!'). this logic could probably be simplified
-    for obj in objects:
-        if obj['datatype']['name'] == datatype:
-            # if datatype_tags is set, identify data using this info. if not, just use tag data. if no tags either, just append if meets datatype criteria. will check for filter with a not tag (!)
-            if datatype_tags:
-                # if the input datatype_tags are included in the object's datatype_tags, look for appropriate tags. if no tags, just append
-                if 'datatype_tags' in list(obj['output'].keys()) and len(obj['output']['datatype_tags']) != 0:
-                    ctr=0
-                    if '!' in str(datatype_tags):
-                        datatype_tags_to_drop = [ f for f in datatype_tags if '!' in str(f) ]
-                        datatype_tag_keep = [ f for f in datatype_tags if f not in datatype_tags_to_drop ]
-
-                        ctr = check_tags_dtags(datatype_tag_keep,obj,'datatype_tags')
-                        if ctr > 0:
-                            datatype_tag_checks = check_for_filter_tags(datatype_tags_to_drop,obj,'datatype_tags')
-                            if datatype_tag_checks == len(datatype_tags_to_drop):
-                                datatype_tag_filter = True
+        # subjects and paths
+        subjects = []
+        sessions = []
+        paths = []
+        finish_dates = []
+        obj_datatype_tags = []
+        obj_tags = []
+
+        # set up output
+        data = pd.DataFrame()
+
+        # loop through objects and find appropriate objects based on datatype, datatype_tags, and tags. can include drop tags ('!'). this logic could probably be simplified
+        for obj in objects:
+            if obj['datatype']['name'] == datatype:
+                # if datatype_tags is set, identify data using this info. if not, just use tag data. if no tags either, just append if meets datatype criteria. will check for filter with a not tag (!)
+                if datatype_tags:
+                    # if the input datatype_tags are included in the object's datatype_tags, look for appropriate tags. if no tags, just append
+                    if 'datatype_tags' in list(obj['output'].keys()) and len(obj['output']['datatype_tags']) != 0:
+                        ctr=0
+                        if '!' in str(datatype_tags):
+                            datatype_tags_to_drop = [ f for f in datatype_tags if '!' in str(f) ]
+                            datatype_tag_keep = [ f for f in datatype_tags if f not in datatype_tags_to_drop ]
+
+                            ctr = check_tags_dtags(datatype_tag_keep,obj,'datatype_tags')
+                            if ctr > 0:
+                                datatype_tag_checks = check_for_filter_tags(datatype_tags_to_drop,obj,'datatype_tags')
+                                if datatype_tag_checks == len(datatype_tags_to_drop):
+                                    datatype_tag_filter = True
+                                else:
+                                    datatype_tag_filter = False
                             else:
                                 datatype_tag_filter = False
                         else:
-                            datatype_tag_filter = False
+                            ctr = check_tags_dtags(datatype_tags,obj,'datatype_tags')
+                            if ctr > 0:
+                                datatype_tag_filter = True
+                            else:
+                                datatype_tag_filter = False
                     else:
-                        ctr = check_tags_dtags(datatype_tags,obj,'datatype_tags')
-                        if ctr > 0:
-                            datatype_tag_filter = True
-                        else:
-                            datatype_tag_filter = False
+                        datatype_tag_filter = False
                 else:
-                    datatype_tag_filter = False
-            else:
-                datatype_tag_filter = True
-
-            if tags:
-                if 'tags' in list(obj['output'].keys()) and len(obj['output']['tags']) != 0:
-                    ctr = 0
-                    if '!' in str(tags):
-                        tags_drop = [ f for f in tags if '!' in str(f) ]
-                        tags_keep = [ f for f in tags if f not in tags_drop ]
-                        ctr = check_tags_dtags(tags_keep,obj,'tags')
-                        if ctr > 0:
-                            tag_checks = check_for_filter_tags(tags_drop,obj,'tags')
-                            if tag_checks == len(tags_drop):
-                                tag_filter = True
+                    datatype_tag_filter = True
+
+                if tags:
+                    if 'tags' in list(obj['output'].keys()) and len(obj['output']['tags']) != 0:
+                        ctr = 0
+                        if '!' in str(tags):
+                            tags_drop = [ f for f in tags if '!' in str(f) ]
+                            tags_keep = [ f for f in tags if f not in tags_drop ]
+                            ctr = check_tags_dtags(tags_keep,obj,'tags')
+                            if ctr > 0:
+                                tag_checks = check_for_filter_tags(tags_drop,obj,'tags')
+                                if tag_checks == len(tags_drop):
+                                    tag_filter = True
+                                else:
+                                    tag_filter = False
                             else:
                                 tag_filter = False
                         else:
-                            tag_filter = False
+                            ctr = check_tags_dtags(tags,obj,'tags')
+                            if ctr > 0:
+                                tag_filter = True
+                            else:
+                                tag_filter = False
                     else:
-                        ctr = check_tags_dtags(tags,obj,'tags')
-                        if ctr > 0:
-                            tag_filter = True
-                        else:
-                            tag_filter = False
+                        tag_filter = False
                 else:
-                    tag_filter = False
-            else:
-                tag_filter = True
-
-            if datatype_tag_filter == True & tag_filter == True:
-                finish_dates, subjects, sessions, paths, obj_tags, obj_datatype_tags = append_data(subjects,sessions,paths,finish_dates,obj,filename,obj_tags,obj_datatype_tags,duplicates)
-    # check if tab separated or comma separated by looking at input filename
-    if '.tsv' in filename:
-        sep = '\t'
-    else:
-        sep = ','
+                    tag_filter = True
 
-    # compile data
-    # if net_adj:
-    #     data = {}
-    #     data = compile_network_adjacency_matrices(paths,subjects,sessions,data)
-    #     if outPath:
-    #         np.save(outPath,data)
-    # else:
-    data = compile_data(paths,subjects,sessions,data,obj_datatype_tags,obj_tags,finish_dates)
-
-    # output data structure for records and any further analyses
-    if outPath:
-        data.to_csv(outPath,sep=sep,index=False)
+                if datatype_tag_filter == True & tag_filter == True:
+                    finish_dates, subjects, sessions, paths, obj_tags, obj_datatype_tags = append_data(subjects,sessions,paths,finish_dates,obj,filename,obj_tags,obj_datatype_tags,duplicates)
+        # check if tab separated or comma separated by looking at input filename
+        if '.tsv' in filename:
+            sep = '\t'
+        else:
+            sep = ','
+
+        # compile data
+        # if net_adj:
+        #     data = {}
+        #     data = compile_network_adjacency_matrices(paths,subjects,sessions,data)
+        #     if outPath:
+        #         np.save(outPath,data)
+        # else:
+        data = compile_data(paths,subjects,sessions,data,obj_datatype_tags,obj_tags,finish_dates)
+
+        # output data structure for records and any further analyses
+        if outPath:
+            data.to_csv(outPath,sep=sep,index=False)
 
     return data, obj_tags, obj_datatype_tags
 
 # ## this function is the wrapper function that calls all the prevouis functions to generate a dataframe for the entire project of the appropriate datatype
 # def collect_data(datatype,datatype_tags=[],tags=[],filename='',outPath='',net_adj=False):
 
 #     if datatype in ['cortex_example','tractmeasures_example']:
```

### Comparing `pybrainlife-1.1.1/pybrainlife/data/manipulate.py` & `pybrainlife-1.1.2/pybrainlife/data/manipulate.py`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.1.1/pybrainlife/vis/__pycache__/data.cpython-38.pyc` & `pybrainlife-1.1.2/pybrainlife/vis/__pycache__/data.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.1.1/pybrainlife/vis/__pycache__/plots.cpython-38.pyc` & `pybrainlife-1.1.2/pybrainlife/vis/__pycache__/plots.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.1.1/pybrainlife/vis/plots.py` & `pybrainlife-1.1.2/pybrainlife/vis/plots.py`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.1.1/pyproject.toml` & `pybrainlife-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybrainlife"
-version = "1.1.1"
+version = "1.1.2"
 description = "This project is a collection of functions that are useful for analyzing MRI data derivatives generated on brainlife.io"
 authors = ["Brad Caron <bacaron245@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/brainlife/pybrainlife"
 repository = "https://github.com/brainlife/pybrainlife"
 keywords = ["brainlife"]
```

### Comparing `pybrainlife-1.1.1/setup.py` & `pybrainlife-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'requests>=2.28.1,<3.0.0',
  'scikit-learn>=1.0.2,<2.0.0',
  'scipy>=1.8.0,<2.0.0',
  'seaborn>=0.12.2,<0.13.0']
 
 setup_kwargs = {
     'name': 'pybrainlife',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'This project is a collection of functions that are useful for analyzing MRI data derivatives generated on brainlife.io',
     'long_description': '[![Abcdspec-compliant](https://img.shields.io/badge/ABCD_Spec-v1.1-green.svg)](https://github.com/soichih/abcd-spec)\n\n# pybrainlife\nThis repository contains the python package for collecting, collating, manipulating, analyzing, and visualizing MRI data generated on brainlife.io. Designed to used within the brainlife.io Analysis tab Jupyter notebooks, can be installed as a pypi package to your local machine.\n\n### Authors\n- Brad Caron (bacaron@iu.edu)\n\n### Contributors\n- Soichi Hayashi (hayashi@iu.edu)\n- Franco Pestilli (franpest@indiana.edu)\n\n### Funding\n[![NSF-BCS-1734853](https://img.shields.io/badge/NSF_BCS-1734853-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1734853)\n[![NSF-BCS-1636893](https://img.shields.io/badge/NSF_BCS-1636893-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1636893)\n\n### Citations\n\nPlease cite the following articles when publishing papers that used data, code or other resources created by the brainlife.io community.\n\n1. Avesani, P., McPherson, B., Hayashi, S. et al. The open diffusion data derivatives, brain data upcycling via integrated publishing of derivatives and reproducible open cloud services. Sci Data 6, 69 (2019). https://doi.org/10.1038/s41597-019-0073-y\n\n### Directory structure\n```\npybrainlife\n├── dist\n│\xa0\xa0 ├── pybrainlife-1.0.0-py3-none-any.whl\n│\xa0\xa0 └── pybrainlife-1.0.0.tar.gz\n├── poetry.lock\n├── pybrainlife\n│\xa0\xa0 ├── data\n│\xa0\xa0 │\xa0\xa0 ├── collect.py\n│\xa0\xa0 │\xa0\xa0 └── manipulate.py\n│\xa0\xa0 ├── __init__.py\n│\xa0\xa0 └── vis\n│\xa0\xa0     ├── plots.py\n│\xa0\xa0     └── __pycache__\n│\xa0\xa0         ├── data.cpython-38.pyc\n│\xa0\xa0         └── plots.cpython-38.pyc\n├── pyproject.toml\n├── README.md\n└── tests\n    ├── __init__.py\n    └── test_pybrainlife.py\n```\n\n### Installing locally\nThis package can be installed locally via PyPi using the following command:\n\n```\npip install pybrainlife\n```\n\n### Dependencies\n\nThis package requires the following libraries.\n  - python = "3.8"\n  - numpy = "^1.9.3"\n  - bctpy = "^0.5.2"\n  - seaborn = "^0.11.2"\n  - jgf = "^0.2.2"\n  - scikit-learn = "^1.0.2"\n  - pandas = "^1.4.2"\n  - scipy = "^1.8.0"\n  - requests = "^2.27.1"\n\nLibrary of Modules for Loading Data and Analyzing Data from brainlife.io\n\n2022 The University of Texas at Austin\n',
     'author': 'Brad Caron',
     'author_email': 'bacaron245@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/brainlife/pybrainlife',
```

### Comparing `pybrainlife-1.1.1/PKG-INFO` & `pybrainlife-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybrainlife
-Version: 1.1.1
+Version: 1.1.2
 Summary: This project is a collection of functions that are useful for analyzing MRI data derivatives generated on brainlife.io
 Home-page: https://github.com/brainlife/pybrainlife
 Keywords: brainlife
 Author: Brad Caron
 Author-email: bacaron245@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

