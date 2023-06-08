# Comparing `tmp/log_mgr-0.0.2.tar.gz` & `tmp/log_mgr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log_mgr-0.0.2.tar", last modified: Fri May  5 18:56:27 2023, max compression
+gzip compressed data, was "log_mgr-0.1.1.tar", last modified: Thu Jun  8 18:14:05 2023, max compression
```

## Comparing `log_mgr-0.0.2.tar` & `log_mgr-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:56:27.872301 log_mgr-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-05 18:56:27.872301 log_mgr-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-05 18:56:17.000000 log_mgr-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:56:27.872301 log_mgr-0.0.2/log_mgr/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 18:56:17.000000 log_mgr-0.0.2/log_mgr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-05 18:56:17.000000 log_mgr-0.0.2/log_mgr/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:56:27.872301 log_mgr-0.0.2/log_mgr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-05 18:56:27.000000 log_mgr-0.0.2/log_mgr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-05 18:56:27.000000 log_mgr-0.0.2/log_mgr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:56:27.000000 log_mgr-0.0.2/log_mgr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 18:56:27.000000 log_mgr-0.0.2/log_mgr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 18:56:27.872301 log_mgr-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-05 18:56:17.000000 log_mgr-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:56:27.872301 log_mgr-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:56:17.000000 log_mgr-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-05 18:56:17.000000 log_mgr-0.0.2/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:14:05.294531 log_mgr-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-08 18:14:05.294531 log_mgr-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-08 18:13:52.000000 log_mgr-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:14:05.294531 log_mgr-0.1.1/log_mgr/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-08 18:13:52.000000 log_mgr-0.1.1/log_mgr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-08 18:13:52.000000 log_mgr-0.1.1/log_mgr/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:14:05.294531 log_mgr-0.1.1/log_mgr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-08 18:14:05.000000 log_mgr-0.1.1/log_mgr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-08 18:14:05.000000 log_mgr-0.1.1/log_mgr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:14:05.000000 log_mgr-0.1.1/log_mgr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 18:14:05.000000 log_mgr-0.1.1/log_mgr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:14:05.294531 log_mgr-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-08 18:13:52.000000 log_mgr-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:14:05.294531 log_mgr-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:13:52.000000 log_mgr-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-08 18:13:52.000000 log_mgr-0.1.1/tests/test_config.py
```

### Comparing `log_mgr-0.0.2/PKG-INFO` & `log_mgr-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log_mgr
-Version: 0.0.2
+Version: 0.1.1
 Summary: Utility class for logging with handlers included
 Home-page: https://github.com/Phornee/log_mgr
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `log_mgr-0.0.2/log_mgr/logger.py` & `log_mgr-0.1.1/log_mgr/logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,17 +19,22 @@
 
 class UTCFormatter(logging.Formatter):
     """ Class for formatter """
     converter = time.gmtime
 
 
 class Logger():
-    """ Logger class with builtin handler configuration"""
+    """ Logger class with builtin handler configuration. 
+        Must be used only from the root application to define the handlers and other parameters
+        In the inner libraries logging.getLogger() should be used.
+        Also can be used by inner libraries, if they want for some reason a different log configuration or handlers.
+        """
     def __init__(self, package_name: str,
                  log_file_name: str,
+                 log_name: str = None,
                  mode: LoggerMode = LoggerMode.FILE,
                  level=logging.INFO,
                  utc: bool = False,
                  dry_run: bool = False):
         """ Init of the class
         Args:
             package_name (str): Root package name, to put the logs into the right /var/log/ subfolder
@@ -51,36 +56,45 @@
             self.dry_run = True
             self.homevar = os.path.join(self.homevar, 'dryrun_log')
             if not os.path.exists(self.homevar):
                 os.makedirs(self.homevar)
         else:
             self.dry_run = False
 
-        self.setup_logger(mode, level, utc)
+        self.setup_logger(log_name, mode, level, utc)
 
     def __del__(self):
         logging.shutdown() # Shutdown logger, otherwise we cannot rmtree because files are still opened
         if self.dry_run and os.path.exists(self.homevar):
             shutil.rmtree(self.homevar)
 
+    def __getattr__(self, name):
+        """ Inherits and delegates all the functions from logging.logger (i.e. info, debug, warning, error methods)
+        Args:
+            name (str): Name of the property to be delegated
+        Returns:
+            _type_: The delegated result
+        """
+        return getattr(self.logger, name)
+
     def get_log_path(self) -> str:
         """ Returns the log path based on the homevar folder and the log file name specified"""
         return os.path.join(self.homevar, f"{self.log_file_name}.log")
 
-    def setup_logger(self, mode: LoggerMode, level, utc: bool):
+    def setup_logger(self, log_name: str, mode: LoggerMode, level, utc: bool):
         """ Setup the selected mode, that means which builtin handlers will be added to the logger """
-        self.logger = logging.getLogger(f'{self.package_name}_{self.log_file_name}_log')
+        self.logger = logging.getLogger(log_name)
 
         if not os.path.exists(self.homevar):
             os.mkdir(self.homevar)
 
         if utc:
-            formatter = UTCFormatter('%(asctime)s-%(message)s', '%Y-%m-%d %H:%M:%S')
+            formatter = UTCFormatter('%(asctime)s-%(filename)s-%(message)s', '%Y-%m-%d %H:%M:%S')
         else:
-            formatter = logging.Formatter('%(asctime)s-%(message)s', '%Y-%m-%d %H:%M:%S')
+            formatter = logging.Formatter('%(asctime)s-%(filename)s-%(message)s', '%Y-%m-%d %H:%M:%S')
 
         # Create rotating file handler
         if mode in [LoggerMode.FILE, LoggerMode.BOTH]:
             file_handler = RotatingFileHandler(self.get_log_path(), maxBytes=10000, backupCount=10)
             file_handler.setFormatter(formatter)
             self.logger.addHandler(file_handler)
 
@@ -103,23 +117,7 @@
         with open(self.get_log_path(), 'r', encoding='UTF-8') as file:
             return file.read()
 
     def get_log_lines(self) -> str:
         """ Get log file content split in lines"""
         with open(self.get_log_path(), 'r', encoding='UTF-8') as file:
             return file.readlines()
-
-    def info(self, message: str):
-        """ Outputs a info log """
-        self.logger.info(message)
-
-    def debug(self, message: str):
-        """ Outputs a debug log """
-        self.logger.debug(message)
-
-    def warning(self, message: str):
-        """ Outputs a warning log """
-        self.logger.warning(message)
-
-    def error(self, message: str):
-        """ Outputs an error log """
-        self.logger.error(message)
```

### Comparing `log_mgr-0.0.2/log_mgr.egg-info/PKG-INFO` & `log_mgr-0.1.1/log_mgr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log-mgr
-Version: 0.0.2
+Version: 0.1.1
 Summary: Utility class for logging with handlers included
 Home-page: https://github.com/Phornee/log_mgr
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `log_mgr-0.0.2/setup.py` & `log_mgr-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="log_mgr",
-    version="0.0.2",
+    version="0.1.1",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Utility class for logging with handlers included",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/log_mgr",
     packages=setuptools.find_packages(),
```

### Comparing `log_mgr-0.0.2/tests/test_config.py` & `log_mgr-0.1.1/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,12 +24,12 @@
         logger.debug('debug message')
         logger.info('info message')
 
         content = logger.get_log_lines()
 
         self.assertEqual(len(content), 1)
 
-        skip_date = content[0][20:].rstrip()
+        skip_date = content[0].rstrip()[-12:]
         self.assertEqual(skip_date, 'info message')
 
 if __name__ == "__main__":
     unittest.main()
```

