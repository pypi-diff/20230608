# Comparing `tmp/cove_unified_logs-0.1.3.tar.gz` & `tmp/cove_unified_logs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cove_unified_logs-0.1.3.tar", last modified: Thu Jun  8 18:52:28 2023, max compression
+gzip compressed data, was "cove_unified_logs-0.1.4.tar", last modified: Thu Jun  8 19:55:34 2023, max compression
```

## Comparing `cove_unified_logs-0.1.3.tar` & `cove_unified_logs-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 18:52:28.215992 cove_unified_logs-0.1.3/
--rw-r--r--   0 sarvpriye   (502) staff       (20)      783 2023-06-08 18:20:43.000000 cove_unified_logs-0.1.3/LICENSE
--rw-r--r--   0 sarvpriye   (502) staff       (20)     5322 2023-06-08 18:52:28.215865 cove_unified_logs-0.1.3/PKG-INFO
--rw-r--r--   0 sarvpriye   (502) staff       (20)     4517 2023-06-08 18:22:32.000000 cove_unified_logs-0.1.3/README.md
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 18:52:28.214904 cove_unified_logs-0.1.3/cove_unified_logs/
--rw-r--r--   0 sarvpriye   (502) staff       (20)       72 2023-06-08 10:41:05.000000 cove_unified_logs-0.1.3/cove_unified_logs/__init__.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     5938 2023-06-08 17:20:34.000000 cove_unified_logs-0.1.3/cove_unified_logs/cloud_logger.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)      785 2023-06-08 16:58:09.000000 cove_unified_logs-0.1.3/cove_unified_logs/console_logger.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     2023 2023-06-08 18:52:03.000000 cove_unified_logs-0.1.3/cove_unified_logs/log_consumer.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1880 2023-06-08 18:44:58.000000 cove_unified_logs-0.1.3/cove_unified_logs/log_producer.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)      865 2023-06-08 17:53:38.000000 cove_unified_logs-0.1.3/cove_unified_logs/middleware.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1570 2023-06-08 17:10:22.000000 cove_unified_logs-0.1.3/cove_unified_logs/unified_logger.py
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 18:52:28.215682 cove_unified_logs-0.1.3/cove_unified_logs.egg-info/
--rw-r--r--   0 sarvpriye   (502) staff       (20)     5322 2023-06-08 18:52:28.000000 cove_unified_logs-0.1.3/cove_unified_logs.egg-info/PKG-INFO
--rw-r--r--   0 sarvpriye   (502) staff       (20)      466 2023-06-08 18:52:28.000000 cove_unified_logs-0.1.3/cove_unified_logs.egg-info/SOURCES.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)        1 2023-06-08 18:52:28.000000 cove_unified_logs-0.1.3/cove_unified_logs.egg-info/dependency_links.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       31 2023-06-08 18:52:28.000000 cove_unified_logs-0.1.3/cove_unified_logs.egg-info/requires.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       18 2023-06-08 18:52:28.000000 cove_unified_logs-0.1.3/cove_unified_logs.egg-info/top_level.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       38 2023-06-08 18:52:28.216030 cove_unified_logs-0.1.3/setup.cfg
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1174 2023-06-08 18:52:14.000000 cove_unified_logs-0.1.3/setup.py
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 19:55:34.039493 cove_unified_logs-0.1.4/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1076 2023-06-08 19:25:10.000000 cove_unified_logs-0.1.4/LICENSE
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-08 19:55:34.039378 cove_unified_logs-0.1.4/PKG-INFO
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     6452 2023-06-08 19:44:21.000000 cove_unified_logs-0.1.4/README.md
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 19:55:34.038494 cove_unified_logs-0.1.4/cove_unified_logs/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       72 2023-06-08 10:41:05.000000 cove_unified_logs-0.1.4/cove_unified_logs/__init__.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     5938 2023-06-08 17:20:34.000000 cove_unified_logs-0.1.4/cove_unified_logs/cloud_logger.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1397 2023-06-08 18:58:04.000000 cove_unified_logs-0.1.4/cove_unified_logs/console_logger.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     2219 2023-06-08 19:37:52.000000 cove_unified_logs-0.1.4/cove_unified_logs/log_consumer.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1880 2023-06-08 18:44:58.000000 cove_unified_logs-0.1.4/cove_unified_logs/log_producer.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      865 2023-06-08 17:53:38.000000 cove_unified_logs-0.1.4/cove_unified_logs/middleware.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1524 2023-06-08 19:03:18.000000 cove_unified_logs-0.1.4/cove_unified_logs/unified_logger.py
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 19:55:34.039206 cove_unified_logs-0.1.4/cove_unified_logs.egg-info/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-08 19:55:34.000000 cove_unified_logs-0.1.4/cove_unified_logs.egg-info/PKG-INFO
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      466 2023-06-08 19:55:34.000000 cove_unified_logs-0.1.4/cove_unified_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)        1 2023-06-08 19:55:34.000000 cove_unified_logs-0.1.4/cove_unified_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       31 2023-06-08 19:55:34.000000 cove_unified_logs-0.1.4/cove_unified_logs.egg-info/requires.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       18 2023-06-08 19:55:34.000000 cove_unified_logs-0.1.4/cove_unified_logs.egg-info/top_level.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       38 2023-06-08 19:55:34.039531 cove_unified_logs-0.1.4/setup.cfg
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1174 2023-06-08 19:14:41.000000 cove_unified_logs-0.1.4/setup.py
```

### Comparing `cove_unified_logs-0.1.3/PKG-INFO` & `cove_unified_logs-0.1.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,34 @@
-Metadata-Version: 2.1
-Name: cove_unified_logs
-Version: 0.1.3
-Summary: A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.
-Home-page: https://github.com/Cove-Identity/cove-unified-logs
-Author: Coveidentity Tech Private Limited
-Author-email: sarvpriye.soni@coveidentity.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # Cove Unified Logs
 
 Cove Unified Logs is a Python library for handling logs in various environments (Django, AWS Lambda, Google Cloud) and pushing them to AWS CloudWatch in an asynchronous way.
 
 ## Author
 
 **SARVPRIYE SONI**
 
 - Github: [@Cove-Identity](https://github.com/Cove-Identity/cove-unified-logs)
 - Email: sarvpriye.soni@coveidentity.com
+- Website: [Cove Identity](https://coveidentity.com)
 
 
-
+## Check out products from Cove Identity
+- Cove Identity: [Cove Identity](https://www.coveidentity.com/cove-identity-app)
+- Cove Drive: [Cove Drive](https://drive.coveidentity.com)
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Cove Unified Logs.
 
 ```bash
 pip install cove_unified_logs
 ```
 
 
-
 # AWS Credentials Configuration
 
 To interact with AWS services, Cove Unified Logs uses boto3, the AWS SDK for Python. You need to configure your AWS credentials for use with boto3. Here's how:
 
 1) **Environment Variables:** Set the `AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY` and `AWS_SESSION_TOKEN` (optional for when you are using AWS STS temporary credentials) environment variables.
 2) **Shared Credential File (~/.aws/credentials):** Use an AWS credentials file to specify your credentials. The default location is `~/.aws/credentials`.
 3) **AWS Config File (~/.aws/config):** Similar to the credentials file, you can also have a configuration file. The default location is ~/.aws/config. This file allows you to specify your region along with your credentials. 
@@ -105,28 +88,63 @@
 logger = UnifiedLogger(app_name, config='all')
 logger.set_level(settings.LOG_LEVEL)
 ```
 
 Remember to replace 'your-app-name' with the name of your application, and to adjust the apps.get_app_config(__package__.split('.')[0]).verbose_name line as necessary for your project structure.
 
 
-All logs from your Django application will then be sent to both the console and AWS CloudWatch.
+##Running the Log Consumer
+1. The `LogConsumer` class is responsible for consuming logs from a Redis queue and sending them to AWS CloudWatch. You can run it as a standalone service in your infrastructure.
+
+```python
+from cove_unified_logs.log_consumer import LogConsumer
+from cove_unified_logs.cloud_logger import CloudLogger
+cloud_logger = CloudLogger(group_name='log-group', stream_name='log-stream', region_name='eu-west-1', flush_interval=10, batch_size=100)
+consumer = LogConsumer(cloud_logger=cloud_logger)
+consumer.run()
+
+```
+
+2. **Environment Variables**: The script uses the following environment variables for Redis configuration:
+
+`REDIS_HOST`: The hostname of your Redis server.
+`REDIS_PORT`: The port number on which your Redis server is running.
+`REDIS_PASSWORD`: The password for your Redis server. (Optional)
+
+Make sure these environment variables are set correctly in your environment.
+
+3. Running the Script: To run the script, navigate to the root directory of this repository and use the following command:
+
+Remember, the consumer is designed to be long-running and should be managed with a process supervisor to ensure it stays running.
+
+
+
+Please make sure to adapt these instructions to your actual setup and include any additional steps or information that might be necessary.
+
 
 
 ##Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 # Confidentiality Notice
 
-This software, including all the code, scripts, features, and documentation associated with it, is a proprietary product of Coveidentity Tech Private Limited, and is confidential in nature. It is only intended for use within Coveidentity Tech Private Limited, by employees or authorized collaborators who have been granted access. 
+This software, including all the code, scripts, features, and documentation associated with it, is a proprietary product of Coveidentity Tech Private Limited and is confidential in nature. It is released under the MIT License and is free for use and modification in accordance with the terms of that license.
+
+Any use of this software, or any of its parts, outside of the terms laid out in the MIT License, without express permission of Coveidentity Tech Private Limited, is strictly prohibited.
+
 
 # License
 
-This project is licensed under the terms of the Proprietary License. Unauthorized copying, distribution, modification, public display, or public performance of this proprietary software, or any subset of the proprietary software, is strictly prohibited. 
+This software is licensed under the MIT License.
 
-# Disclaimer
+The MIT License is a permissive license that is short and to the point. It lets people do anything they want with your code as long as they provide attribution back to you and don’t hold you liable.
 
-The software is provided "AS IS", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability, whether in an action of
+For the detailed terms and conditions, please refer to the LICENSE file in this repository.
+
+Please note that this software is a proprietary product of Coveidentity Tech Private Limited and any use outside the terms laid out in the MIT License, without express permission of Coveidentity Tech Private Limited, is strictly prohibited.
 
 
+# Disclaimer
+
+The software is provided "AS IS", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability, whether in an action of
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cove_unified_logs-0.1.3/cove_unified_logs/cloud_logger.py` & `cove_unified_logs-0.1.4/cove_unified_logs/cloud_logger.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.3/cove_unified_logs/log_consumer.py` & `cove_unified_logs-0.1.4/cove_unified_logs/log_consumer.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,11 +43,15 @@
             # handle connection error, for example by retrying or by failing gracefully
         except Exception as e:
             logging.error(f"Failed to consume log event: {str(e)}")
             # exit failure, so that docker can restart the container
             exit(1)
             # handle unexpected errors
 
-
-cloud_logger = CloudLogger('cove-logger-v3', str(uuid.uuid4()))
+'''
+#usage
+from cove_unified_logs.log_consumer import LogConsumer
+from cove_unified_logs.cloud_logger import CloudLogger
+cloud_logger = CloudLogger(group_name='log-group', stream_name='log-stream', region_name='eu-west-1', flush_interval=10, batch_size=100)
 consumer = LogConsumer(cloud_logger=cloud_logger)
 consumer.run()
+'''
```

### Comparing `cove_unified_logs-0.1.3/cove_unified_logs/log_producer.py` & `cove_unified_logs-0.1.4/cove_unified_logs/log_producer.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.3/cove_unified_logs/middleware.py` & `cove_unified_logs-0.1.4/cove_unified_logs/middleware.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.3/cove_unified_logs/unified_logger.py` & `cove_unified_logs-0.1.4/cove_unified_logs/unified_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,18 @@
     def __init__(self, config='all', app_name='cove', log_level=None):
         if log_level is None:
             log_level = os.environ.get('LOG_LEVEL', 'info')
         self.log_level = log_level.lower()
         self.app_name = app_name
         self.loggers = []
         if config in ('all', 'console'):
-            self.loggers.append(ConsoleLogger())
+            self.loggers.append(ConsoleLogger(app_name))
         if config in ('all', 'cloud'):
             self.loggers.append(LogProducer())
 
-        print("====================================")
 
     def _log(self, level, message, **metadata):
         metadata['app_name'] = self.app_name
         for logger in self.loggers:
             getattr(logger, level)(message, **metadata)
 
     def debug(self, message, **metadata):
```

### Comparing `cove_unified_logs-0.1.3/cove_unified_logs.egg-info/PKG-INFO` & `cove_unified_logs-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cove-unified-logs
-Version: 0.1.3
+Name: cove_unified_logs
+Version: 0.1.4
 Summary: A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.
 Home-page: https://github.com/Cove-Identity/cove-unified-logs
 Author: Coveidentity Tech Private Limited
 Author-email: sarvpriye.soni@coveidentity.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -24,28 +24,30 @@
 
 ## Author
 
 **SARVPRIYE SONI**
 
 - Github: [@Cove-Identity](https://github.com/Cove-Identity/cove-unified-logs)
 - Email: sarvpriye.soni@coveidentity.com
+- Website: [Cove Identity](https://coveidentity.com)
 
 
-
+## Check out products from Cove Identity
+- Cove Identity: [Cove Identity](https://www.coveidentity.com/cove-identity-app)
+- Cove Drive: [Cove Drive](https://drive.coveidentity.com)
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Cove Unified Logs.
 
 ```bash
 pip install cove_unified_logs
 ```
 
 
-
 # AWS Credentials Configuration
 
 To interact with AWS services, Cove Unified Logs uses boto3, the AWS SDK for Python. You need to configure your AWS credentials for use with boto3. Here's how:
 
 1) **Environment Variables:** Set the `AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY` and `AWS_SESSION_TOKEN` (optional for when you are using AWS STS temporary credentials) environment variables.
 2) **Shared Credential File (~/.aws/credentials):** Use an AWS credentials file to specify your credentials. The default location is `~/.aws/credentials`.
 3) **AWS Config File (~/.aws/config):** Similar to the credentials file, you can also have a configuration file. The default location is ~/.aws/config. This file allows you to specify your region along with your credentials. 
@@ -105,28 +107,65 @@
 logger = UnifiedLogger(app_name, config='all')
 logger.set_level(settings.LOG_LEVEL)
 ```
 
 Remember to replace 'your-app-name' with the name of your application, and to adjust the apps.get_app_config(__package__.split('.')[0]).verbose_name line as necessary for your project structure.
 
 
-All logs from your Django application will then be sent to both the console and AWS CloudWatch.
+##Running the Log Consumer
+1. The `LogConsumer` class is responsible for consuming logs from a Redis queue and sending them to AWS CloudWatch. You can run it as a standalone service in your infrastructure.
+
+```python
+from cove_unified_logs.log_consumer import LogConsumer
+from cove_unified_logs.cloud_logger import CloudLogger
+cloud_logger = CloudLogger(group_name='log-group', stream_name='log-stream', region_name='eu-west-1', flush_interval=10, batch_size=100)
+consumer = LogConsumer(cloud_logger=cloud_logger)
+consumer.run()
+
+```
+
+2. **Environment Variables**: The script uses the following environment variables for Redis configuration:
+
+`REDIS_HOST`: The hostname of your Redis server.
+`REDIS_PORT`: The port number on which your Redis server is running.
+`REDIS_PASSWORD`: The password for your Redis server. (Optional)
+
+Make sure these environment variables are set correctly in your environment.
+
+3. Running the Script: To run the script, navigate to the root directory of this repository and use the following command:
+
+Remember, the consumer is designed to be long-running and should be managed with a process supervisor to ensure it stays running.
+
+
+
+Please make sure to adapt these instructions to your actual setup and include any additional steps or information that might be necessary.
+
 
 
 ##Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 # Confidentiality Notice
 
-This software, including all the code, scripts, features, and documentation associated with it, is a proprietary product of Coveidentity Tech Private Limited, and is confidential in nature. It is only intended for use within Coveidentity Tech Private Limited, by employees or authorized collaborators who have been granted access. 
+This software, including all the code, scripts, features, and documentation associated with it, is a proprietary product of Coveidentity Tech Private Limited and is confidential in nature. It is released under the MIT License and is free for use and modification in accordance with the terms of that license.
+
+Any use of this software, or any of its parts, outside of the terms laid out in the MIT License, without express permission of Coveidentity Tech Private Limited, is strictly prohibited.
+
 
 # License
 
-This project is licensed under the terms of the Proprietary License. Unauthorized copying, distribution, modification, public display, or public performance of this proprietary software, or any subset of the proprietary software, is strictly prohibited. 
+This software is licensed under the MIT License.
+
+The MIT License is a permissive license that is short and to the point. It lets people do anything they want with your code as long as they provide attribution back to you and don’t hold you liable.
+
+For the detailed terms and conditions, please refer to the LICENSE file in this repository.
+
+Please note that this software is a proprietary product of Coveidentity Tech Private Limited and any use outside the terms laid out in the MIT License, without express permission of Coveidentity Tech Private Limited, is strictly prohibited.
+
 
 # Disclaimer
 
 The software is provided "AS IS", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability, whether in an action of
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cove_unified_logs-0.1.3/setup.py` & `cove_unified_logs-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cove_unified_logs',
-    version='0.1.3',
+    version='0.1.4',
     description='A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Coveidentity Tech Private Limited',
     author_email='sarvpriye.soni@coveidentity.com',
     url='https://github.com/Cove-Identity/cove-unified-logs',
     packages=['cove_unified_logs'],
```

