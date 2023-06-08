# Comparing `tmp/dumbo_esse3-0.4.2.tar.gz` & `tmp/dumbo_esse3-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumbo_esse3-0.4.2.tar", max compression
+gzip compressed data, was "dumbo_esse3-0.4.4.tar", max compression
```

## Comparing `dumbo_esse3-0.4.2.tar` & `dumbo_esse3-0.4.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2022-09-11 08:55:51.265066 dumbo_esse3-0.4.2/LICENSE
--rw-r--r--   0        0        0        0 2022-09-11 07:49:43.077054 dumbo_esse3-0.4.2/dumbo_esse3/__init__.py
--rw-r--r--   0        0        0      101 2023-01-18 08:46:22.755370 dumbo_esse3-0.4.2/dumbo_esse3/__main__.py
--rwxr-xr-x   0        0        0    22705 2023-04-20 16:13:03.551751 dumbo_esse3-0.4.2/dumbo_esse3/cli.py
--rw-r--r--   0        0        0    23044 2023-04-20 16:08:42.523435 dumbo_esse3-0.4.2/dumbo_esse3/esse3_wrapper.py
--rw-r--r--   0        0        0    10306 2023-02-03 22:04:42.668983 dumbo_esse3-0.4.2/dumbo_esse3/primitives.py
--rw-r--r--   0        0        0      515 2023-04-20 16:14:38.783867 dumbo_esse3-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 dumbo_esse3-0.4.2/setup.py
--rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 dumbo_esse3-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-09-11 08:55:51.265066 dumbo_esse3-0.4.4/LICENSE
+-rw-r--r--   0        0        0        0 2022-09-11 07:49:43.077054 dumbo_esse3-0.4.4/dumbo_esse3/__init__.py
+-rw-r--r--   0        0        0      101 2023-01-18 08:46:22.755370 dumbo_esse3-0.4.4/dumbo_esse3/__main__.py
+-rwxr-xr-x   0        0        0    22705 2023-04-20 16:13:03.551751 dumbo_esse3-0.4.4/dumbo_esse3/cli.py
+-rw-r--r--   0        0        0    23184 2023-04-20 16:30:50.996190 dumbo_esse3-0.4.4/dumbo_esse3/esse3_wrapper.py
+-rw-r--r--   0        0        0    10307 2023-06-08 19:43:33.890292 dumbo_esse3-0.4.4/dumbo_esse3/primitives.py
+-rw-r--r--   0        0        0      515 2023-06-08 19:42:57.956728 dumbo_esse3-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 dumbo_esse3-0.4.4/setup.py
+-rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 dumbo_esse3-0.4.4/PKG-INFO
```

### Comparing `dumbo_esse3-0.4.2/LICENSE` & `dumbo_esse3-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dumbo_esse3-0.4.2/dumbo_esse3/cli.py` & `dumbo_esse3-0.4.4/dumbo_esse3/cli.py`

 * *Files identical despite different names*

### Comparing `dumbo_esse3-0.4.2/dumbo_esse3/esse3_wrapper.py` & `dumbo_esse3-0.4.4/dumbo_esse3/esse3_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dumbo_utils.primitives import PrivateKey
 from lxml import html
 
 import typeguard
 from selenium import webdriver
 from selenium.common import WebDriverException, NoSuchElementException, ElementNotSelectableException, \
-    ElementNotVisibleException
+    ElementNotVisibleException, TimeoutException
 from selenium.webdriver import Keys
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions
 from selenium.webdriver.support.wait import WebDriverWait
 
 from dumbo_esse3.primitives import Course, Username, Password, Exam, Student, StudentThesisState, CdL, \
     ExamDescription, ExamNotes, ExamType, DateTime, Register, NumberOfHours, Semester, RegisterActivity, \
@@ -425,30 +425,33 @@
             f"//table[@id = 'tableElencoCommissioni']/tbody/tr[td[1] = '{committee.name}']/td[3]/a"
         ).send_keys(Keys.RETURN)
         self.driver.find_element(
             By.XPATH,
             f"//table[@id = 'tableElencoConcTurni']/tbody/tr[td[2] = '{committee.part}']/td[4]/a"
         ).send_keys(Keys.RETURN)
 
-        ignore_list = [ElementNotVisibleException, ElementNotSelectableException]
-        wait = WebDriverWait(self.driver, timeout=10, poll_frequency=1, ignored_exceptions=ignore_list)
-        wait.until(expected_conditions.presence_of_element_located(
-            (By.XPATH, "//table[@id='tableElencoIscritti']/tfoot/tr"))
-        )
+        try:
+            ignore_list = [ElementNotVisibleException, ElementNotSelectableException]
+            wait = WebDriverWait(self.driver, timeout=3, poll_frequency=1, ignored_exceptions=ignore_list)
+            wait.until(expected_conditions.presence_of_element_located(
+                (By.XPATH, "//table[@id='tableElencoIscritti']/tfoot/tr"))
+            )
 
-        self.driver.execute_script("""
-            Object.keys(localStorage).forEach(key => {
-                if (key.endsWith(":paging")) {
-                    localStorage.setItem(key, '{"current": 1,"size": 999999}');
-                }
-            });
-            console.log(Object.keys(localStorage));
-            console.log(Object.values(localStorage));
-        """)
-        self.driver.refresh()
+            self.driver.execute_script("""
+                Object.keys(localStorage).forEach(key => {
+                    if (key.endsWith(":paging")) {
+                        localStorage.setItem(key, '{"current": 1,"size": 999999}');
+                    }
+                });
+                console.log(Object.keys(localStorage));
+                console.log(Object.values(localStorage));
+            """)
+            self.driver.refresh()
+        except TimeoutException:
+            pass
 
         fiscal_code_to_valuation = {valuation.fiscal_code: valuation for valuation in valuations}
 
         html_document = html.fromstring(self.driver.page_source)
         fiscal_code_to_url = {
             FiscalCode(row.xpath("td[3]")[0].text): ESSE3_SERVER + '/' + row.xpath("td[5]/a/@href")[0]
             for row in html_document.xpath('//table[@id="tableElencoIscritti"]/tbody/tr')
```

### Comparing `dumbo_esse3-0.4.2/dumbo_esse3/primitives.py` & `dumbo_esse3-0.4.4/dumbo_esse3/primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 
 @bounded_string(min_length=3, max_length=8, pattern=r'[0-9]*')
 class StudentId:
     pass
 
 
-@bounded_string(min_length=3, max_length=80, pattern=r"[A-ZÀÈÉÌÒÙÍ' ]*")
+@bounded_string(min_length=3, max_length=80, pattern=r"[A-ZÀÈÉÌÒÙÍ' -]*")
 class StudentName:
     pass
 
 
 @bounded_string(min_length=1, max_length=80, pattern=r"[A-Za-z0-9ÀÈÉÌÒÙàèéìòù '\":;.,()\[\]_-]*")
 class ExamDescription:
     pass
```

### Comparing `dumbo_esse3-0.4.2/pyproject.toml` & `dumbo_esse3-0.4.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dumbo-esse3"
-version = "0.4.2"
+version = "0.4.4"
 description = "Esse3 command line utility, to save my future time!"
 authors = ["Mario Alviano <mario.alviano@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dateutils = "^0.6.12"
 dumbo-utils = "^0.1.4"
```

### Comparing `dumbo_esse3-0.4.2/setup.py` & `dumbo_esse3-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['dateutils>=0.6.12,<0.7.0',
  'dumbo-utils>=0.1.4,<0.2.0',
  'lxml>=4.9.2,<5.0.0',
  'selenium>=4.4.3,<5.0.0']
 
 setup_kwargs = {
     'name': 'dumbo-esse3',
-    'version': '0.4.2',
+    'version': '0.4.4',
     'description': 'Esse3 command line utility, to save my future time!',
     'long_description': 'None',
     'author': 'Mario Alviano',
     'author_email': 'mario.alviano@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dumbo_esse3-0.4.2/PKG-INFO` & `dumbo_esse3-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumbo-esse3
-Version: 0.4.2
+Version: 0.4.4
 Summary: Esse3 command line utility, to save my future time!
 Author: Mario Alviano
 Author-email: mario.alviano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

