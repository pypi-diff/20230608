# Comparing `tmp/nextflow-23.4.1.tar.gz` & `tmp/nextflow-23.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextflow-23.4.1.tar", last modified: Mon Apr 17 09:33:59 2023, max compression
+gzip compressed data, was "nextflow-23.4.2.tar", last modified: Thu Jun  8 12:44:17 2023, max compression
```

## Comparing `nextflow-23.4.1.tar` & `nextflow-23.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-17 09:33:59.603348 nextflow-23.4.1/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1417 2023-04-17 09:33:59.603348 nextflow-23.4.1/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      877 2023-01-24 06:27:33.000000 nextflow-23.4.1/README.md
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-17 09:33:59.603348 nextflow-23.4.1/launcher/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    14760 2023-04-17 09:33:59.000000 nextflow-23.4.1/launcher/nextflow
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-17 09:33:59.603348 nextflow-23.4.1/nextflow.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1417 2023-04-17 09:33:59.000000 nextflow-23.4.1/nextflow.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      164 2023-04-17 09:33:59.000000 nextflow-23.4.1/nextflow.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-17 09:33:59.000000 nextflow-23.4.1/nextflow.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-17 09:33:59.000000 nextflow-23.4.1/nextflow.egg-info/top_level.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-04-17 09:33:59.603348 nextflow-23.4.1/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      786 2023-04-17 09:30:32.000000 nextflow-23.4.1/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-08 12:44:17.576790 nextflow-23.4.2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1417 2023-06-08 12:44:17.576790 nextflow-23.4.2/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      877 2023-01-24 06:27:33.000000 nextflow-23.4.2/README.md
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-08 12:44:17.576790 nextflow-23.4.2/launcher/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    14760 2023-06-08 12:44:17.000000 nextflow-23.4.2/launcher/nextflow
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-08 12:44:17.576790 nextflow-23.4.2/nextflow.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1417 2023-06-08 12:44:17.000000 nextflow-23.4.2/nextflow.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      164 2023-06-08 12:44:17.000000 nextflow-23.4.2/nextflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-06-08 12:44:17.000000 nextflow-23.4.2/nextflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-06-08 12:44:17.000000 nextflow-23.4.2/nextflow.egg-info/top_level.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-06-08 12:44:17.576790 nextflow-23.4.2/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      786 2023-06-08 12:42:12.000000 nextflow-23.4.2/setup.py
```

### Comparing `nextflow-23.4.1/PKG-INFO` & `nextflow-23.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextflow
-Version: 23.4.1
+Version: 23.4.2
 Summary: A Python wrapper that installs the Nextflow launcher
 Home-page: UNKNOWN
 Author: Jordi Deu-Pons
 License: Apache License 2.0
 Keywords: pipeline,workflow,nextflow
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `nextflow-23.4.1/README.md` & `nextflow-23.4.2/README.md`

 * *Files identical despite different names*

### Comparing `nextflow-23.4.1/launcher/nextflow` & `nextflow-23.4.2/launcher/nextflow`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 [[ "$NXF_DEBUG" == 'x' ]] && set -x
-NXF_VER=${NXF_VER:-'23.04.1'}
+NXF_VER=${NXF_VER:-'23.04.2'}
 NXF_ORG=${NXF_ORG:-'nextflow-io'}
 NXF_HOME=${NXF_HOME:-$HOME/.nextflow}
 NXF_PROT=${NXF_PROT:-'https'}
 NXF_BASE=${NXF_BASE:-$NXF_PROT://www.nextflow.io/releases}
 NXF_TEMP=${NXF_TEMP:-$TMPDIR}
 NXF_DIST=${NXF_DIST:-$NXF_HOME/framework}
 NXF_CLI="$0 $@"
```

### Comparing `nextflow-23.4.1/nextflow.egg-info/PKG-INFO` & `nextflow-23.4.2/nextflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextflow
-Version: 23.4.1
+Version: 23.4.2
 Summary: A Python wrapper that installs the Nextflow launcher
 Home-page: UNKNOWN
 Author: Jordi Deu-Pons
 License: Apache License 2.0
 Keywords: pipeline,workflow,nextflow
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `nextflow-23.4.1/setup.py` & `nextflow-23.4.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = '23.04.1'
+__version__ = '23.04.2'
 
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
```

