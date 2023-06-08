# Comparing `tmp/JsonPreprocessor-0.2.3.tar.gz` & `tmp/JsonPreprocessor-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JsonPreprocessor-0.2.3.tar", last modified: Thu May  4 14:30:17 2023, max compression
+gzip compressed data, was "JsonPreprocessor-0.2.4.tar", last modified: Thu Jun  8 14:01:42 2023, max compression
```

## Comparing `JsonPreprocessor-0.2.3.tar` & `JsonPreprocessor-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:30:17.401166 JsonPreprocessor-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:30:17.401166 JsonPreprocessor-0.2.3/JsonPreprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)    28745 2023-05-04 14:27:47.000000 JsonPreprocessor-0.2.3/JsonPreprocessor/CJsonPreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)   274550 2023-05-04 14:30:17.000000 JsonPreprocessor-0.2.3/JsonPreprocessor/JsonPreprocessor.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-04 14:27:47.000000 JsonPreprocessor-0.2.3/JsonPreprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-04 14:27:47.000000 JsonPreprocessor-0.2.3/JsonPreprocessor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:30:17.401166 JsonPreprocessor-0.2.3/JsonPreprocessor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-04 14:30:17.000000 JsonPreprocessor-0.2.3/JsonPreprocessor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-04 14:30:17.000000 JsonPreprocessor-0.2.3/JsonPreprocessor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:30:17.000000 JsonPreprocessor-0.2.3/JsonPreprocessor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 14:30:17.000000 JsonPreprocessor-0.2.3/JsonPreprocessor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-04 14:27:47.000000 JsonPreprocessor-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-04 14:30:17.401166 JsonPreprocessor-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-04 14:27:47.000000 JsonPreprocessor-0.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:30:17.405166 JsonPreprocessor-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-05-04 14:27:47.000000 JsonPreprocessor-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:01:42.327988 JsonPreprocessor-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:01:42.323988 JsonPreprocessor-0.2.4/JsonPreprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)    28767 2023-06-08 13:59:35.000000 JsonPreprocessor-0.2.4/JsonPreprocessor/CJsonPreprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   220463 2023-06-08 14:01:42.000000 JsonPreprocessor-0.2.4/JsonPreprocessor/JsonPreprocessor.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-08 13:59:35.000000 JsonPreprocessor-0.2.4/JsonPreprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-08 13:59:35.000000 JsonPreprocessor-0.2.4/JsonPreprocessor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:01:42.323988 JsonPreprocessor-0.2.4/JsonPreprocessor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-08 14:01:42.000000 JsonPreprocessor-0.2.4/JsonPreprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-08 14:01:42.000000 JsonPreprocessor-0.2.4/JsonPreprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:01:42.000000 JsonPreprocessor-0.2.4/JsonPreprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 14:01:42.000000 JsonPreprocessor-0.2.4/JsonPreprocessor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-08 13:59:35.000000 JsonPreprocessor-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-08 14:01:42.327988 JsonPreprocessor-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-08 13:59:35.000000 JsonPreprocessor-0.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:01:42.327988 JsonPreprocessor-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-06-08 13:59:35.000000 JsonPreprocessor-0.2.4/setup.py
```

### Comparing `JsonPreprocessor-0.2.3/JsonPreprocessor/CJsonPreprocessor.py` & `JsonPreprocessor-0.2.4/JsonPreprocessor/CJsonPreprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -387,29 +387,30 @@
                 pattern = re.sub('\]', '\\]', pattern)
                 sInputStr = re.sub('\\' + pattern, '\'' + tmpValue + '\'', sInputStr) if isinstance(tmpValue, str) else \
                             re.sub('\\' + pattern, '\'' + str(tmpValue) + '\'', sInputStr)
             sStrHandled = sUpdateVar + sInputStr
             return sStrHandled
                     
         else:
+            if "." in referVars[0]:
+                dotdictVariable = re.sub('\${\s*(.*?)\s*}', '\\1', referVars[0])
+                lDotdictVariable = dotdictVariable.split(".")
+                lParams = self.__handleDotdictFormat(lDotdictVariable, [])
+                sParam = '${' + lParams[0] + '}'
+                lParams.pop(0)
+                for item in lParams:
+                    sParam = sParam + "['" + item + "']"
+                sInputStr = re.sub('\${\s*([^\}]*)\s*}', sParam, sInputStr)
+
+                referVars = re.findall('(\${\s*.*?\s*})', sInputStr)
+
             pattern = '(\\' + referVars[0] + '\s*\[\s*.*?\s*\])'
             variable = re.findall(pattern, sInputStr)
             if variable == []:
-                if "." in referVars[0]:
-                    dotdictVariable = re.sub('\${\s*(.*?)\s*}', '\\1', referVars[0])
-                    lDotdictVariable = dotdictVariable.split(".")
-                    lParams = self.__handleDotdictFormat(lDotdictVariable, [])
-                    sStrHandled = '${' + lParams[0] + '}'
-                    lParams.pop(0)
-                    for item in lParams:
-                        sStrHandled = sStrHandled + "['" + item + "']"
-                else:
-                    sStrHandled = referVars[0]
-
-                return sStrHandled
+                return referVars[0]
             else:
                 fullVariable = variable[0]
                 while variable != []:
                     pattern = pattern[:-1] + '\[\s*.*?\s*\])'
                     variable = re.findall(pattern, sInputStr)
                     if variable != []:
                         fullVariable = variable[0]
@@ -533,15 +534,15 @@
                             ldict = {}
                             exec(sExec, globals(), ldict)
                             if bStringValue:
                                 item = str(ldict['value'])
                             else:
                                 item = ldict['value']
                         except:
-                            raise Exception(f"The variable '{tmpItemAfterProcessed}' is not available!")
+                            raise Exception(f"The variable '{itemAfterProcessed}' is not available!")
 
                     tmpValue.append(item)
                 v = tmpValue
             
             elif isinstance(v, str):
                 if re.match('^.*\s*\${\s*', v.lower()):
                     bStringValue = False
@@ -557,15 +558,15 @@
                         ldict = {}
                         exec(sExec, globals(), ldict)
                         if bStringValue:
                             v = str(ldict['value'])
                         else:
                             v = ldict['value']
                     except:
-                        raise Exception(f"The variable '{tmpValueAfterProcessed}' is not available!")
+                        raise Exception(f"The variable '{valueAfterProcessed}' is not available!")
                         
                     if isinstance(v, str) and re.match('^\s*none|true|false\s*$', v.lower()):
                         v = '\"' + v + '\"'
                         
             __jsonUpdated(k, v, oJson, bNested, keyNested)
             if keyNested != '':
                 self.lUpdatedParams.update({k:v})
@@ -755,10 +756,10 @@
                 tmpParseNestedParam = re.sub('\\${\s*(.*?)\s*}', '\\1', parseNestedParam)
                 sExec = "value = " + tmpParseNestedParam if isinstance(tmpParseNestedParam, str) else \
                         "value = " + str(tmpParseNestedParam)
                 try:
                     ldict = {}
                     exec(sExec, globals(), ldict)
                 except:
-                    raise Exception(f"The variable '{tmpParseNestedParam}' is not available!")  
+                    raise Exception(f"The variable '{parseNestedParam}' is not available!")  
             
         return oJson
```

### Comparing `JsonPreprocessor-0.2.3/JsonPreprocessor/JsonPreprocessor.pdf` & `JsonPreprocessor-0.2.4/JsonPreprocessor/JsonPreprocessor.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 26% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 JsonPreprocessor
-v. 0.2.3
+v. 0.2.4
 Mai Dinh Nam Son
-04.05.2023
+08.06.2023
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -602,19 +602,19 @@
 
 Name
 
 JsonPreprocessor
 
 Version
 
-0.2.3
+0.2.4
 
 Date
 
-04.05.2023
+08.06.2023
 
 Description
 
 Preprocessor for json files
 
 Package URL
 
@@ -669,15 +669,25 @@
 
 Initial version
 0.1.4
 
 09/2022
 
 Updated documentation
+0.2.3
+
+05/2023
+
+Added dotdict format
+0.2.4
+
+06/2023
+
+Improved dotdict format and update log output
 
 JsonPreprocessor.pdf
-Created at 04.05.2023 - 14:30:13
-by GenPackageDoc v. 0.39.2
+Created at 08.06.2023 - 14:01:39
+by GenPackageDoc v. 0.40.3
 
 11
```

### Comparing `JsonPreprocessor-0.2.3/JsonPreprocessor/__init__.py` & `JsonPreprocessor-0.2.4/JsonPreprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.2.3/JsonPreprocessor/version.py` & `JsonPreprocessor-0.2.4/JsonPreprocessor/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of JsonPreprocessor
 #
-VERSION      = "0.2.3"
-VERSION_DATE = "04.05.2023"
+VERSION      = "0.2.4"
+VERSION_DATE = "08.06.2023"
```

### Comparing `JsonPreprocessor-0.2.3/LICENSE` & `JsonPreprocessor-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `JsonPreprocessor-0.2.3/README.rst` & `JsonPreprocessor-0.2.4/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -14,52 +14,81 @@
 
 Json Preprocessor's Package Description
 =======================================
 
 Getting Started
 ---------------
 
-The JsonPreprocessor is a Python3 package which allows programmers to handle  
-additional features in json files such as
+The **JsonPreprocessor** is a Python3 package which allows programmers to handle  
+additional features in JSON files such as
 
 * add comments
 * import other json files
 * overwrite already existing parameters with new values
 
-These json files will be handled by the JsonPreprocessor which returns as result
+These JSON files will be handled by the **JsonPreprocessor** which returns as result
 a dictionary object of the deserialized data.
 
 How to install
 --------------
 
-**JsonPreprocessor** can be installed in two different ways.
+The **JsonPreprocessor** can be installed in two different ways.
 
 1. Installation via PyPi (recommended for users)
 
    .. code::
 
       pip install JsonPreprocessor
 
    `JsonPreprocessor in PyPi <https://pypi.org/project/JsonPreprocessor/>`_
 
 2. Installation via GitHub (recommended for developers)
 
-   Clone the **JsonPreprocessor** repository to your machine.
+   * Clone the **JsonPreprocessor** repository to your machine.
 
-   .. code::
+     .. code::
 
-      git clone https://github.com/test-fullautomation/python-jsonpreprocessor.git
+        git clone https://github.com/test-fullautomation/python-jsonpreprocessor.git
 
-   `JsonPreprocessor in GitHub <https://github.com/test-fullautomation/python-jsonpreprocessor>`_
+     `JsonPreprocessor in GitHub <https://github.com/test-fullautomation/python-jsonpreprocessor>`_
 
-   Use the following command to install **JsonPreprocessor**:
+   * Install dependencies
 
-   .. code::
+     **JsonPreprocessor** requires some additional Python libraries. Before you install the cloned repository sources
+     you have to install the dependencies manually. The names of all related packages you can find in the file ``requirements.txt``
+     in the repository root folder. Use pip to install them:
+
+     .. code::
+
+        pip install -r ./requirements.txt
+
+     Additionally install **LaTeX** (recommended: TeX Live). This is used to render the documentation.
+
+   * Configure dependencies
+
+     The installation of **JsonPreprocessor** includes to generate the documentation in PDF format. This is done by
+     an application called **GenPackageDoc**, that is part of the installation dependencies (see ``requirements.txt``).
+
+     **GenPackageDoc** uses **LaTeX** to generate the documentation in PDF format. Therefore **GenPackageDoc** needs to know where to find
+     **LaTeX**. This is defined in the **GenPackageDoc** configuration file
+
+     .. code::
+
+        packagedoc\packagedoc_config.json
+
+     Before you start the installation you have to introduce the following environment variable, that is used in ``packagedoc_config.json``:
+
+     - ``GENDOC_LATEXPATH`` : path to ``pdflatex`` executable
+
+   * Use the following command to install **JsonPreprocessor**:
+
+     .. code::
+
+        setup.py install
 
-      setup.py install
 
 Package Documentation
 ---------------------
 
 A detailed documentation of the Json Preprocessor's package can be found here: `JsonPreprocessor.pdf <https://github.com/test-fullautomation/python-jsonpreprocessor/blob/develop/JsonPreprocessor/JsonPreprocessor.pdf>`_
 
 Feedback
```

### Comparing `JsonPreprocessor-0.2.3/setup.py` & `JsonPreprocessor-0.2.4/setup.py`

 * *Files identical despite different names*

