# Comparing `tmp/PrimeBotFramework-1.0.31.tar.gz` & `tmp/PrimeBotFramework-1.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-lolul7dg/PrimeBotFramework-1.0.31.tar", last modified: Thu Jun  1 14:12:20 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-xdhe40q0/PrimeBotFramework-1.0.34.tar", last modified: Thu Jun  8 11:54:56 2023, max compression
```

## Comparing `PrimeBotFramework-1.0.31.tar` & `PrimeBotFramework-1.0.34.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.321182 PrimeBotFramework-1.0.31/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-01 14:12:20.329182 PrimeBotFramework-1.0.31/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.321182 PrimeBotFramework-1.0.31/PrimeBot/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.321182 PrimeBotFramework-1.0.31/PrimeBot/B2E/
--rw-rw-rw-   0 root         (0) root         (0)     4028 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/B2E/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.321182 PrimeBotFramework-1.0.31/PrimeBot/Cnab750/
--rw-rw-rw-   0 root         (0) root         (0)    10211 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/Cnab750/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/CpfCnpj/
--rw-rw-rw-   0 root         (0) root         (0)     1963 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/CpfCnpj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/CpfCnpj/api_codes.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/CpfCnpj/model.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/D4Sign/
--rw-rw-rw-   0 root         (0) root         (0)     2600 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/D4Sign/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/DeathByCaptcha/
--rw-rw-rw-   0 root         (0) root         (0)     2822 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/DeathByCaptcha/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/Documents/
--rw-rw-rw-   0 root         (0) root         (0)     1098 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/Documents/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/Elastic/
--rw-rw-rw-   0 root         (0) root         (0)     1239 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/Elastic/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/ExchangeGraph/
--rw-rw-rw-   0 root         (0) root         (0)     8987 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/ExchangeGraph/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/IntegracaoSendGrid/
--rw-rw-rw-   0 root         (0) root         (0)     4251 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/IntegracaoSendGrid/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/ListenerECS/
--rw-rw-rw-   0 root         (0) root         (0)     4096 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/ListenerECS/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/Mongo/
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/Mongo/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/OracleDB/
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/OracleDB/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/Vault/
--rw-rw-rw-   0 root         (0) root         (0)     2740 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/Vault/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.329182 PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-01 14:12:20.000000 PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      707 2023-06-01 14:12:20.000000 PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-01 14:12:20.000000 PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-01 14:12:20.000000 PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-06-01 14:12:20.000000 PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-01 14:12:20.329182 PrimeBotFramework-1.0.31/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.195003 PrimeBotFramework-1.0.34/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.195003 PrimeBotFramework-1.0.34/PrimeBot/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.195003 PrimeBotFramework-1.0.34/PrimeBot/B2E/
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/B2E/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.195003 PrimeBotFramework-1.0.34/PrimeBot/Cnab750/
+-rw-rw-rw-   0 root         (0) root         (0)    10211 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/Cnab750/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.195003 PrimeBotFramework-1.0.34/PrimeBot/CpfCnpj/
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/CpfCnpj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/CpfCnpj/api_codes.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/CpfCnpj/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.195003 PrimeBotFramework-1.0.34/PrimeBot/D4Sign/
+-rw-rw-rw-   0 root         (0) root         (0)     2600 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/D4Sign/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.195003 PrimeBotFramework-1.0.34/PrimeBot/DeathByCaptcha/
+-rw-rw-rw-   0 root         (0) root         (0)     2822 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/DeathByCaptcha/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/Documents/
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/Documents/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/Elastic/
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/Elastic/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/ExchangeGraph/
+-rw-rw-rw-   0 root         (0) root         (0)     8987 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/ExchangeGraph/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/FeriadosBancarios/
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/FeriadosBancarios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/FeriadosBancarios/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/IntegracaoSendGrid/
+-rw-rw-rw-   0 root         (0) root         (0)     4251 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/IntegracaoSendGrid/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/ListenerECS/
+-rw-rw-rw-   0 root         (0) root         (0)     4096 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/ListenerECS/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/Mongo/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/Mongo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/OracleDB/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/OracleDB/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/Vault/
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/Vault/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-08 11:54:56.000000 PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-06-08 11:54:56.000000 PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-08 11:54:56.000000 PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-08 11:54:56.000000 PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-06-08 11:54:56.000000 PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/setup.py
```

### Comparing `PrimeBotFramework-1.0.31/PKG-INFO` & `PrimeBotFramework-1.0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.31
+Version: 1.0.34
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.31/PrimeBot/B2E/__init__.py` & `PrimeBotFramework-1.0.34/PrimeBot/B2E/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.31/PrimeBot/Cnab750/__init__.py` & `PrimeBotFramework-1.0.34/PrimeBot/Cnab750/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.31/PrimeBot/CpfCnpj/__init__.py` & `PrimeBotFramework-1.0.34/PrimeBot/CpfCnpj/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.31/PrimeBot/CpfCnpj/api_codes.py` & `PrimeBotFramework-1.0.34/PrimeBot/CpfCnpj/api_codes.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.31/PrimeBot/D4Sign/__init__.py` & `PrimeBotFramework-1.0.34/PrimeBot/D4Sign/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.31/PrimeBot/DeathByCaptcha/__init__.py` & `PrimeBotFramework-1.0.34/PrimeBot/DeathByCaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.31/PrimeBot/Documents/__init__.py` & `PrimeBotFramework-1.0.34/PrimeBot/Documents/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.31/PrimeBot/Elastic/__init__.py` & `PrimeBotFramework-1.0.34/PrimeBot/Elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.31/PrimeBot/ExchangeGraph/__init__.py` & `PrimeBotFramework-1.0.34/PrimeBot/ExchangeGraph/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.31/PrimeBot/IntegracaoSendGrid/__init__.py` & `PrimeBotFramework-1.0.34/PrimeBot/IntegracaoSendGrid/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.31/PrimeBot/ListenerECS/__init__.py` & `PrimeBotFramework-1.0.34/PrimeBot/ListenerECS/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.31/PrimeBot/OracleDB/__init__.py` & `PrimeBotFramework-1.0.34/PrimeBot/OracleDB/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.31/PrimeBot/Vault/__init__.py` & `PrimeBotFramework-1.0.34/PrimeBot/Vault/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/PKG-INFO` & `PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.31
+Version: 1.0.34
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/SOURCES.txt` & `PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 PrimeBot/CpfCnpj/api_codes.py
 PrimeBot/CpfCnpj/model.py
 PrimeBot/D4Sign/__init__.py
 PrimeBot/DeathByCaptcha/__init__.py
 PrimeBot/Documents/__init__.py
 PrimeBot/Elastic/__init__.py
 PrimeBot/ExchangeGraph/__init__.py
+PrimeBot/FeriadosBancarios/__init__.py
+PrimeBot/FeriadosBancarios/model.py
 PrimeBot/IntegracaoSendGrid/__init__.py
 PrimeBot/ListenerECS/__init__.py
 PrimeBot/Mongo/__init__.py
 PrimeBot/OracleDB/__init__.py
 PrimeBot/Vault/__init__.py
 PrimeBotFramework.egg-info/PKG-INFO
 PrimeBotFramework.egg-info/SOURCES.txt
```

### Comparing `PrimeBotFramework-1.0.31/setup.py` & `PrimeBotFramework-1.0.34/setup.py`

 * *Files identical despite different names*

