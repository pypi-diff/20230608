# Comparing `tmp/apf_base-2.4.2.tar.gz` & `tmp/apf_base-2.4.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/APF/APF/dist/.tmp-afpig74w/apf_base-2.4.2.tar", last modified: Wed Jun  7 16:33:36 2023, max compression
+gzip compressed data, was "/home/runner/work/APF/APF/dist/.tmp-ctlkk1p6/apf_base-2.4.3b0.tar", last modified: Thu Jun  8 16:52:46 2023, max compression
```

## Comparing `apf_base-2.4.2.tar` & `apf_base-2.4.3b0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:36.000000 apf_base-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-07 16:33:10.000000 apf_base-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-07 16:33:36.000000 apf_base-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-07 16:33:10.000000 apf_base-2.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf/consumers/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/consumers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/consumers/avro_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/consumers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/consumers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/consumers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/consumers/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf/core/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/core/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/core/management/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/core/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf/core/templates/step/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/core/templates/step/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf/core/templates/step/package/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/core/templates/step/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/core/templates/step/package/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/core/templates/step/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf/core/templates/step/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/core/templates/step/scripts/run_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/core/templates/step/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/core/templates/step/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/core/topic_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/metrics/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/metrics/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf/metrics/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/metrics/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/metrics/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf/producers/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/producers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/producers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/producers/json_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-06-07 16:33:10.000000 apf_base-2.4.2/apf/producers/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-07 16:33:36.000000 apf_base-2.4.2/apf_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:33:36.000000 apf_base-2.4.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-07 16:33:10.000000 apf_base-2.4.2/scripts/apf
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 16:33:36.000000 apf_base-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-07 16:33:10.000000 apf_base-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/consumers/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/consumers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/consumers/avro_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/consumers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/consumers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/consumers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/consumers/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/management/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/core/templates/step/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/templates/step/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/core/templates/step/package/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/templates/step/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/templates/step/package/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/templates/step/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/core/templates/step/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/templates/step/scripts/run_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/templates/step/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/templates/step/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/core/topic_management.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/metrics/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/metrics/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/metrics/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/metrics/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/metrics/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf/producers/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/producers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/producers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/producers/json_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/apf/producers/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/apf_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/scripts/apf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 16:52:46.000000 apf_base-2.4.3b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-08 16:52:18.000000 apf_base-2.4.3b0/setup.py
```

### Comparing `apf_base-2.4.2/LICENSE` & `apf_base-2.4.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/PKG-INFO` & `apf_base-2.4.3b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apf_base
-Version: 2.4.2
+Version: 2.4.3b0
 Summary: ALeRCE Alert Processing Framework.
 Author: ALeRCE Team
 Author-email: contact@alerce.online
 Project-URL: Github, https://github.com/alercebroker/APF
 Project-URL: Documentation, https://apf.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apf_base-2.4.2/README.md` & `apf_base-2.4.3b0/README.md`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/consumers/avro_file.py` & `apf_base-2.4.3b0/apf/consumers/avro_file.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/consumers/csv.py` & `apf_base-2.4.3b0/apf/consumers/csv.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/consumers/generic.py` & `apf_base-2.4.3b0/apf/consumers/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/consumers/json.py` & `apf_base-2.4.3b0/apf/consumers/json.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/consumers/kafka.py` & `apf_base-2.4.3b0/apf/consumers/kafka.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
                     if message.error().name() == "_PARTITION_EOF":
                         self.logger.info("PARTITION_EOF: No more messages")
                         return
                     self.logger.exception(f"Error in kafka stream: {message.error()}")
                     continue
                 else:
                     ds_message = self._deserialize_message(message)
-                    ds_message["timestamp"] = message.timestamp()
+                    ds_message["timestamp"] = message.timestamp()[1]
                     deserialized.append(ds_message)
 
             self.messages = messages
             messages = []
             if len(deserialized) > 0:
                 if num_messages == 1:
                     yield deserialized[0]
```

### Comparing `apf_base-2.4.2/apf/core/__init__.py` & `apf_base-2.4.3b0/apf/core/__init__.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/core/management/helpers.py` & `apf_base-2.4.3b0/apf/core/management/helpers.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/core/secret_manager.py` & `apf_base-2.4.3b0/apf/core/secret_manager.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/core/step.py` & `apf_base-2.4.3b0/apf/core/step.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/core/templates/step/package/step.py` & `apf_base-2.4.3b0/apf/core/templates/step/package/step.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/core/templates/step/scripts/run_step.py` & `apf_base-2.4.3b0/apf/core/templates/step/scripts/run_step.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/core/topic_management.py` & `apf_base-2.4.3b0/apf/core/topic_management.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/metrics/generic.py` & `apf_base-2.4.3b0/apf/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/metrics/kafka.py` & `apf_base-2.4.3b0/apf/metrics/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/metrics/log.py` & `apf_base-2.4.3b0/apf/metrics/log.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/metrics/prometheus/prometheus.py` & `apf_base-2.4.3b0/apf/metrics/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/producers/csv.py` & `apf_base-2.4.3b0/apf/producers/csv.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/producers/generic.py` & `apf_base-2.4.3b0/apf/producers/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/producers/json_prod.py` & `apf_base-2.4.3b0/apf/producers/json_prod.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/apf/producers/kafka.py` & `apf_base-2.4.3b0/apf/producers/kafka.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,9 +165,9 @@
         self.logger.info("Waiting to produce last messages")
         self.producer.flush()
 
 class KafkaSchemalessProducer(KafkaProducer):
 
     def _serialize_message(self, message):
         out = io.BytesIO()
-        fastavro.schemaless_writer(out, self.schema, message) #strict=True
+        fastavro.schemaless_writer(out, self.schema, message, strict=True)
         return out.getvalue()
```

### Comparing `apf_base-2.4.2/apf_base.egg-info/PKG-INFO` & `apf_base-2.4.3b0/apf_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apf-base
-Version: 2.4.2
+Version: 2.4.3b0
 Summary: ALeRCE Alert Processing Framework.
 Author: ALeRCE Team
 Author-email: contact@alerce.online
 Project-URL: Github, https://github.com/alercebroker/APF
 Project-URL: Documentation, https://apf.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apf_base-2.4.2/apf_base.egg-info/SOURCES.txt` & `apf_base-2.4.3b0/apf_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apf_base-2.4.2/setup.py` & `apf_base-2.4.3b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="apf_base",
-    version="2.4.2",
+    version="2.4.3b",
     description="ALeRCE Alert Processing Framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ALeRCE Team",
     author_email="contact@alerce.online",
     packages=find_namespace_packages(include=["apf.*"]),
     scripts=["scripts/apf"],
```

