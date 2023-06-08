# Comparing `tmp/TorchSisso-1.0.6.tar.gz` & `tmp/TorchSisso-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchSisso-1.0.6.tar", last modified: Wed Jun  7 17:38:14 2023, max compression
+gzip compressed data, was "TorchSisso-1.0.7.tar", last modified: Wed Jun  7 17:42:27 2023, max compression
```

## Comparing `TorchSisso-1.0.6.tar` & `TorchSisso-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-07 17:38:14.860953 TorchSisso-1.0.6/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-07 17:38:14.859959 TorchSisso-1.0.6/PKG-INFO
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-07 17:38:14.841952 TorchSisso-1.0.6/TorchSisso/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    22981 2023-06-04 21:51:26.000000 TorchSisso-1.0.6/TorchSisso/FC_copy.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23771 2023-06-03 02:04:32.000000 TorchSisso-1.0.6/TorchSisso/FC_copy_working.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23766 2023-06-07 16:53:54.000000 TorchSisso-1.0.6/TorchSisso/FeatureSpaceConstruction.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    20266 2023-06-03 02:11:41.000000 TorchSisso-1.0.6/TorchSisso/Feature_space_construction_1.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10954 2023-06-05 21:48:28.000000 TorchSisso-1.0.6/TorchSisso/SISSORegressor.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10758 2023-06-04 15:54:54.000000 TorchSisso-1.0.6/TorchSisso/SISSORegressor_L1L0.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     8257 2023-06-07 17:31:12.000000 TorchSisso-1.0.6/TorchSisso/SISSO_REGRESSOR_TORCH.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     8313 2023-06-07 17:35:30.000000 TorchSisso-1.0.6/TorchSisso/SISSO_Torch_1.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      273 2023-06-07 16:24:26.000000 TorchSisso-1.0.6/TorchSisso/__init__.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     6179 2023-06-07 17:35:36.000000 TorchSisso-1.0.6/TorchSisso/testRegressor.py
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-07 17:38:14.856952 TorchSisso-1.0.6/TorchSisso.egg-info/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-07 17:38:14.000000 TorchSisso-1.0.6/TorchSisso.egg-info/PKG-INFO
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      489 2023-06-07 17:38:14.000000 TorchSisso-1.0.6/TorchSisso.egg-info/SOURCES.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-06-07 17:38:14.000000 TorchSisso-1.0.6/TorchSisso.egg-info/dependency_links.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-06-07 17:38:14.000000 TorchSisso-1.0.6/TorchSisso.egg-info/requires.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-06-07 17:38:14.000000 TorchSisso-1.0.6/TorchSisso.egg-info/top_level.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-06-07 17:38:14.861953 TorchSisso-1.0.6/setup.cfg
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-06-07 17:38:06.000000 TorchSisso-1.0.6/setup.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-07 17:42:27.503913 TorchSisso-1.0.7/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-07 17:42:27.501915 TorchSisso-1.0.7/PKG-INFO
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-07 17:42:27.484744 TorchSisso-1.0.7/TorchSisso/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    22981 2023-06-04 21:51:26.000000 TorchSisso-1.0.7/TorchSisso/FC_copy.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23771 2023-06-03 02:04:32.000000 TorchSisso-1.0.7/TorchSisso/FC_copy_working.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    23766 2023-06-07 16:53:54.000000 TorchSisso-1.0.7/TorchSisso/FeatureSpaceConstruction.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    20266 2023-06-03 02:11:41.000000 TorchSisso-1.0.7/TorchSisso/Feature_space_construction_1.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10954 2023-06-05 21:48:28.000000 TorchSisso-1.0.7/TorchSisso/SISSORegressor.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    10758 2023-06-04 15:54:54.000000 TorchSisso-1.0.7/TorchSisso/SISSORegressor_L1L0.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     8313 2023-06-07 17:42:10.000000 TorchSisso-1.0.7/TorchSisso/SISSO_REGRESSOR_TORCH.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     8313 2023-06-07 17:35:30.000000 TorchSisso-1.0.7/TorchSisso/SISSO_Torch_1.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      273 2023-06-07 16:24:26.000000 TorchSisso-1.0.7/TorchSisso/__init__.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     6179 2023-06-07 17:35:36.000000 TorchSisso-1.0.7/TorchSisso/testRegressor.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-07 17:42:27.499753 TorchSisso-1.0.7/TorchSisso.egg-info/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-07 17:42:27.000000 TorchSisso-1.0.7/TorchSisso.egg-info/PKG-INFO
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      489 2023-06-07 17:42:27.000000 TorchSisso-1.0.7/TorchSisso.egg-info/SOURCES.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-06-07 17:42:27.000000 TorchSisso-1.0.7/TorchSisso.egg-info/dependency_links.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-06-07 17:42:27.000000 TorchSisso-1.0.7/TorchSisso.egg-info/requires.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-06-07 17:42:27.000000 TorchSisso-1.0.7/TorchSisso.egg-info/top_level.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-06-07 17:42:27.503920 TorchSisso-1.0.7/setup.cfg
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-06-07 17:42:18.000000 TorchSisso-1.0.7/setup.py
```

### Comparing `TorchSisso-1.0.6/TorchSisso/FC_copy.py` & `TorchSisso-1.0.7/TorchSisso/FC_copy.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.6/TorchSisso/FC_copy_working.py` & `TorchSisso-1.0.7/TorchSisso/FC_copy_working.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.6/TorchSisso/FeatureSpaceConstruction.py` & `TorchSisso-1.0.7/TorchSisso/FeatureSpaceConstruction.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.6/TorchSisso/Feature_space_construction_1.py` & `TorchSisso-1.0.7/TorchSisso/Feature_space_construction_1.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.6/TorchSisso/SISSORegressor.py` & `TorchSisso-1.0.7/TorchSisso/SISSORegressor.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.6/TorchSisso/SISSORegressor_L1L0.py` & `TorchSisso-1.0.7/TorchSisso/SISSORegressor_L1L0.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.6/TorchSisso/SISSO_REGRESSOR_TORCH.py` & `TorchSisso-1.0.7/TorchSisso/SISSO_REGRESSOR_TORCH.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,24 +141,26 @@
                     equation = str(float(coefficient)) + '*' + str(self.names[int(selected_index)])  + str(float(intercept))
                     print('Equation: ', equation)
                     print('RMSE: ', rmse)
                 print('Time taken to generate one dimensional equation: ', time.time()-start_1D,'seconds')
             else:
                 start = time.time()
                 rmse,terms,intercept,coefs = self.higher_dimension(i)
+                equation =''
                 for k in range(len(terms)):
                     print(f'{k+1} term in the equation is {terms[k]}')
                     if coefs.flatten()[k] > 0:
                         equation = equation + ' + ' + (str(terms[k])) 
                     else:
                         equation = equation + (str(terms[k])) + '  '
-                print(f'{i} term equation:',equation[:len(equation)-1])
+                print('Equation: ',equation[:len(equation)-1])
                 print('Intercept:', float(intercept))
                 print('RMSE:',float(rmse))
                 print(f'Time taken for {i} dimension is: ', time.time()-start)
+        return float(rmse),equation
```

### Comparing `TorchSisso-1.0.6/TorchSisso/SISSO_Torch_1.py` & `TorchSisso-1.0.7/TorchSisso/SISSO_Torch_1.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.6/TorchSisso/testRegressor.py` & `TorchSisso-1.0.7/TorchSisso/testRegressor.py`

 * *Files identical despite different names*

### Comparing `TorchSisso-1.0.6/setup.py` & `TorchSisso-1.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import setuptools
 
 
 setuptools.setup(
     name="TorchSisso",
-    version="1.0.6",
+    version="1.0.7",
     author="Madhav Muthyala",
     author_email="madhavreddymuthyala@gmail.com",
     description="GPU Supported Sure Independence Screening and Sparsifying Operator Package",
     url="https://github.com/MR1319/TorchSisso",
     packages=setuptools.find_packages(),
     install_requires=[
         "torch",
```

