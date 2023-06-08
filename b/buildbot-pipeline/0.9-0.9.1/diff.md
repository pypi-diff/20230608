# Comparing `tmp/buildbot_pipeline-0.9.tar.gz` & `tmp/buildbot_pipeline-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildbot_pipeline-0.9.tar", last modified: Sun Mar 27 13:36:54 2022, max compression
+gzip compressed data, was "buildbot_pipeline-0.9.1.tar", last modified: Mon Mar 28 09:32:56 2022, max compression
```

## Comparing `buildbot_pipeline-0.9.tar` & `buildbot_pipeline-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bobrov    (1000) bobrov    (1000)        0 2022-03-27 13:36:54.348181 buildbot_pipeline-0.9/
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)     1069 2022-03-15 19:07:31.000000 buildbot_pipeline-0.9/LICENSE
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)     2126 2022-03-27 13:36:54.348181 buildbot_pipeline-0.9/PKG-INFO
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)     1463 2022-03-27 13:26:42.000000 buildbot_pipeline-0.9/README.rst
-drwxr-xr-x   0 bobrov    (1000) bobrov    (1000)        0 2022-03-27 13:36:54.348181 buildbot_pipeline-0.9/buildbot_pipeline/
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)     2887 2022-03-24 19:02:14.000000 buildbot_pipeline-0.9/buildbot_pipeline/__init__.py
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)     2059 2022-03-24 18:21:29.000000 buildbot_pipeline-0.9/buildbot_pipeline/build.py
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)      735 2022-03-24 18:54:32.000000 buildbot_pipeline-0.9/buildbot_pipeline/builder.py
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)      784 2022-03-22 16:46:33.000000 buildbot_pipeline-0.9/buildbot_pipeline/changes.py
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)      853 2022-03-15 19:08:03.000000 buildbot_pipeline-0.9/buildbot_pipeline/file_store.py
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)     2386 2022-03-25 07:18:57.000000 buildbot_pipeline-0.9/buildbot_pipeline/filters.py
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)     4486 2022-03-24 05:06:07.000000 buildbot_pipeline-0.9/buildbot_pipeline/junit.py
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)     2197 2022-03-21 18:35:30.000000 buildbot_pipeline-0.9/buildbot_pipeline/reporters.py
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)    11394 2022-03-27 12:20:42.000000 buildbot_pipeline-0.9/buildbot_pipeline/steps.py
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)     2809 2022-03-24 19:03:45.000000 buildbot_pipeline-0.9/buildbot_pipeline/utils.py
-drwxr-xr-x   0 bobrov    (1000) bobrov    (1000)        0 2022-03-27 13:36:54.348181 buildbot_pipeline-0.9/buildbot_pipeline.egg-info/
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)     2126 2022-03-27 13:36:54.000000 buildbot_pipeline-0.9/buildbot_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)      559 2022-03-27 13:36:54.000000 buildbot_pipeline-0.9/buildbot_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)        1 2022-03-27 13:36:54.000000 buildbot_pipeline-0.9/buildbot_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)        1 2022-03-27 13:31:11.000000 buildbot_pipeline-0.9/buildbot_pipeline.egg-info/not-zip-safe
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)        8 2022-03-27 13:36:54.000000 buildbot_pipeline-0.9/buildbot_pipeline.egg-info/requires.txt
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)       18 2022-03-27 13:36:54.000000 buildbot_pipeline-0.9/buildbot_pipeline.egg-info/top_level.txt
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)       38 2022-03-27 13:36:54.348181 buildbot_pipeline-0.9/setup.cfg
--rw-r--r--   0 bobrov    (1000) bobrov    (1000)      926 2022-03-27 13:36:49.000000 buildbot_pipeline-0.9/setup.py
+drwxr-xr-x   0 bobrov    (1000) bobrov    (1000)        0 2022-03-28 09:32:56.737092 buildbot_pipeline-0.9.1/
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)     1069 2022-03-15 19:07:31.000000 buildbot_pipeline-0.9.1/LICENSE
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)     2128 2022-03-28 09:32:56.737092 buildbot_pipeline-0.9.1/PKG-INFO
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)     1463 2022-03-27 13:26:42.000000 buildbot_pipeline-0.9.1/README.rst
+drwxr-xr-x   0 bobrov    (1000) bobrov    (1000)        0 2022-03-28 09:32:56.737092 buildbot_pipeline-0.9.1/buildbot_pipeline/
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)     2887 2022-03-24 19:02:14.000000 buildbot_pipeline-0.9.1/buildbot_pipeline/__init__.py
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)     2059 2022-03-24 18:21:29.000000 buildbot_pipeline-0.9.1/buildbot_pipeline/build.py
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)      735 2022-03-24 18:54:32.000000 buildbot_pipeline-0.9.1/buildbot_pipeline/builder.py
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)      784 2022-03-22 16:46:33.000000 buildbot_pipeline-0.9.1/buildbot_pipeline/changes.py
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)      853 2022-03-15 19:08:03.000000 buildbot_pipeline-0.9.1/buildbot_pipeline/file_store.py
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)     2394 2022-03-28 09:10:56.000000 buildbot_pipeline-0.9.1/buildbot_pipeline/filters.py
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)     4486 2022-03-24 05:06:07.000000 buildbot_pipeline-0.9.1/buildbot_pipeline/junit.py
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)     2197 2022-03-21 18:35:30.000000 buildbot_pipeline-0.9.1/buildbot_pipeline/reporters.py
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)    11631 2022-03-28 09:26:22.000000 buildbot_pipeline-0.9.1/buildbot_pipeline/steps.py
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)     2809 2022-03-24 19:03:45.000000 buildbot_pipeline-0.9.1/buildbot_pipeline/utils.py
+drwxr-xr-x   0 bobrov    (1000) bobrov    (1000)        0 2022-03-28 09:32:56.737092 buildbot_pipeline-0.9.1/buildbot_pipeline.egg-info/
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)     2128 2022-03-28 09:32:56.000000 buildbot_pipeline-0.9.1/buildbot_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)      559 2022-03-28 09:32:56.000000 buildbot_pipeline-0.9.1/buildbot_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)        1 2022-03-28 09:32:56.000000 buildbot_pipeline-0.9.1/buildbot_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)        1 2022-03-27 13:31:11.000000 buildbot_pipeline-0.9.1/buildbot_pipeline.egg-info/not-zip-safe
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)        8 2022-03-28 09:32:56.000000 buildbot_pipeline-0.9.1/buildbot_pipeline.egg-info/requires.txt
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)       18 2022-03-28 09:32:56.000000 buildbot_pipeline-0.9.1/buildbot_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)       38 2022-03-28 09:32:56.737092 buildbot_pipeline-0.9.1/setup.cfg
+-rw-r--r--   0 bobrov    (1000) bobrov    (1000)      928 2022-03-28 09:32:37.000000 buildbot_pipeline-0.9.1/setup.py
```

### Comparing `buildbot_pipeline-0.9/LICENSE` & `buildbot_pipeline-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `buildbot_pipeline-0.9/PKG-INFO` & `buildbot_pipeline-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildbot_pipeline
-Version: 0.9
+Version: 0.9.1
 Summary: Pipeline syntax for buildbot
 Home-page: https://github.com/baverman/buildbot_pipeline/
 Author: Anton Bobrov
 Author-email: baverman@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `buildbot_pipeline-0.9/README.rst` & `buildbot_pipeline-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `buildbot_pipeline-0.9/buildbot_pipeline/__init__.py` & `buildbot_pipeline-0.9.1/buildbot_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot_pipeline-0.9/buildbot_pipeline/build.py` & `buildbot_pipeline-0.9.1/buildbot_pipeline/build.py`

 * *Files identical despite different names*

### Comparing `buildbot_pipeline-0.9/buildbot_pipeline/builder.py` & `buildbot_pipeline-0.9.1/buildbot_pipeline/builder.py`

 * *Files identical despite different names*

### Comparing `buildbot_pipeline-0.9/buildbot_pipeline/changes.py` & `buildbot_pipeline-0.9.1/buildbot_pipeline/changes.py`

 * *Files identical despite different names*

### Comparing `buildbot_pipeline-0.9/buildbot_pipeline/file_store.py` & `buildbot_pipeline-0.9.1/buildbot_pipeline/file_store.py`

 * *Files identical despite different names*

### Comparing `buildbot_pipeline-0.9/buildbot_pipeline/filters.py` & `buildbot_pipeline-0.9.1/buildbot_pipeline/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 def make_filters(filters, is_or=False):
     if hasattr(filters, 'keys'):
         filters = [filters]
 
     result = []
     for desc in filters:
-        for name, values in desc:
+        for name, values in desc.items():
             if name in FILTERS:
                 fn, getter = FILTERS[name]
                 result.append(make_filter(values, fn, getter))
             elif name == 'not':
                 result.append(filter_op_not(make_filters(values)))
             elif name == 'or':
                 result.append(make_filters(values, True))
```

### Comparing `buildbot_pipeline-0.9/buildbot_pipeline/junit.py` & `buildbot_pipeline-0.9.1/buildbot_pipeline/junit.py`

 * *Files identical despite different names*

### Comparing `buildbot_pipeline-0.9/buildbot_pipeline/reporters.py` & `buildbot_pipeline-0.9.1/buildbot_pipeline/reporters.py`

 * *Files identical despite different names*

### Comparing `buildbot_pipeline-0.9/buildbot_pipeline/steps.py` & `buildbot_pipeline-0.9.1/buildbot_pipeline/steps.py`

 * *Files 6% similar despite different names*

```diff
@@ -173,35 +173,40 @@
                 step['name'] = name
                 if 'steps' in step:
                     step['steps'].insert(0, {'git': True, 'repourl': repo})
 
                 changes = list(self.build.allChanges())
                 if changes:
                     start_build = None
+                    skip_reason = 'unknown'
                     if step.get('disabled'):
                         start_build = False
+                        skip_reason = 'disabled'
 
                     if start_build is None and it_repo_path in changes[0].files:
                         start_build = True
 
-                    if start_build is None and 'filters' in step:
+                    if start_build is None and 'filter' in step:
                         try:
-                            flt = filters.make_filters(step['filters'])
+                            flt = filters.make_filters(step['filter'])
                         except Exception as e:
                             result = results.WARNINGS
+                            skip_reason = str(e)
                             yield self.addCompleteLog(name, str(e))
                         else:
                             changes[0].props = self.getProperties()
                             if flt and flt(changes[0]):
                                 start_build = True
+                            else:
+                                skip_reason = 'filter'
 
                     if start_build:
                         step_info.append(step)
                     else:
-                        yield self.addCompleteLog(name, 'skipped by filters')
+                        yield self.addCompleteLog(name, f'skipped by: {skip_reason}')
 
         if step_info:
             self.build.addStepsAfterCurrentStep([Parallel(step_info, inner=False, waitForFinish=False)])
             return result
 
         self.descriptionDone = ['There are no suitable jobs']
         self.build.results = results.SKIPPED
```

### Comparing `buildbot_pipeline-0.9/buildbot_pipeline/utils.py` & `buildbot_pipeline-0.9.1/buildbot_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `buildbot_pipeline-0.9/buildbot_pipeline.egg-info/PKG-INFO` & `buildbot_pipeline-0.9.1/buildbot_pipeline.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildbot-pipeline
-Version: 0.9
+Version: 0.9.1
 Summary: Pipeline syntax for buildbot
 Home-page: https://github.com/baverman/buildbot_pipeline/
 Author: Anton Bobrov
 Author-email: baverman@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `buildbot_pipeline-0.9/buildbot_pipeline.egg-info/SOURCES.txt` & `buildbot_pipeline-0.9.1/buildbot_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildbot_pipeline-0.9/setup.py` & `buildbot_pipeline-0.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='buildbot_pipeline',
-    version='0.9',
+    version='0.9.1',
     url='https://github.com/baverman/buildbot_pipeline/',
     license='MIT',
     author='Anton Bobrov',
     author_email='baverman@gmail.com',
     description='Pipeline syntax for buildbot',
     long_description=open('README.rst', 'rb').read().decode('utf-8'),
     long_description_content_type='text/x-rst',
```

