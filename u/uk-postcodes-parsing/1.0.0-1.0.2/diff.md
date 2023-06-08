# Comparing `tmp/uk_postcodes_parsing-1.0.0.tar.gz` & `tmp/uk_postcodes_parsing-1.0.2.tar.gz`

## Comparing `uk_postcodes_parsing-1.0.0.tar` & `uk_postcodes_parsing-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/__init__.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/fix.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/postcode_utils.py
--rw-r--r--   0        0        0 20547700 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/postcodes_nov_2022.py
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/ukpostcode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/tests/test_all.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/tests/data/postcode_parse_test.csv
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/LICENSE
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/README.md
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     9591 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/__init__.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/fix.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/postcode_utils.py
+-rw-r--r--   0        0        0 20547700 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/postcodes_nov_2022.py
+-rw-r--r--   0        0        0     7715 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/ukpostcode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/tests/test_all.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/tests/data/postcode_parse_test.csv
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/LICENSE
+-rw-r--r--   0        0        0     9788 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/README.md
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.2/PKG-INFO
```

### Comparing `uk_postcodes_parsing-1.0.0/.pre-commit-config.yaml` & `uk_postcodes_parsing-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-1.0.0/.github/workflows/python-publish.yml` & `uk_postcodes_parsing-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-1.0.0/.github/workflows/test.yml` & `uk_postcodes_parsing-1.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/fix.py` & `uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/fix.py`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/postcode_utils.py` & `uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/postcode_utils.py`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/postcodes_nov_2022.py` & `uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/postcodes_nov_2022.py`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/ukpostcode.py` & `uk_postcodes_parsing-1.0.2/src/uk_postcodes_parsing/ukpostcode.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         postcodes = re.findall(POSTCODE_CORPUS_REGEX, text)
         postcodes = [parse(postcode, attempt_fix=False) for postcode in postcodes]
         postcodes = [postcode for postcode in postcodes if postcode is not None]
         return postcodes
 
 
 def is_in_ons_postcode_directory(postcode: str) -> bool:
-    """Check if the postcode is valid with postcodes.io
+    """Check if the postcode is valid with ons directory
 
     Args:
         postcode (str): The postcode to check
 
     Returns:
         bool: True if the postcode is valid, False otherwise
     """
```

### Comparing `uk_postcodes_parsing-1.0.0/tests/test_all.py` & `uk_postcodes_parsing-1.0.2/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-1.0.0/.gitignore` & `uk_postcodes_parsing-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-1.0.0/LICENSE` & `uk_postcodes_parsing-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-1.0.0/README.md` & `uk_postcodes_parsing-1.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -52,14 +52,27 @@
 >>> from uk_postcodes_parsing import ukpostcode
 >>> corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e3 4ss. But also eh16 50y and ei412"
 >>> postcodes = ukpostcode.parse_from_corpus(corpus, attempt_fix=True)
 INFO:uk-postcodes-parsing:Found 3 postcodes in corpus
 INFO:uk-postcodes-parsing:Postcode Fixed: 'eh16 50y' => 'EH16 5OY'
 ```
 
+You can also do an undertermisitic postcode auto-correct where if there is more than one possible answer, all answers are returned.
+
+```python
+>>> postcodes = ukpostcode.parse_from_corpus("OOO 4SS",
+                             attempt_fix=True,
+                             try_all_fix_options=True
+                             )
+>> postcodes # "O00 4SS", "OO0 4SS", and "O0O 4SS"
+[Postcode(is_in_ons_postcode_directory=False, fix_distance=-2, original='OOO 4SS', postcode='O00 4SS', incode='4SS', outcode='O00', area='O', district='O00', sub_district=None, sector='O00 4', unit='SS'),
+ Postcode(is_in_ons_postcode_directory=False, fix_distance=-1, original='OOO 4SS', postcode='OO0 4SS', incode='4SS', outcode='OO0', area='OO', district='OO0', sub_district=None, sector='OO0 4', unit='SS'),
+ Postcode(is_in_ons_postcode_directory=False, fix_distance=-1, original='OOO 4SS', postcode='O0O 4SS', incode='4SS', outcode='O0O', area='O', district='O0', sub_district='O0O', sector='O0O 4', unit='SS')]
+```
+
 - Parsing
 
 ```python
 >>> from uk_postcodes_parsing import ukpostcode
 >>> ukpostcode.parse("EC1r 1ub")
 Postcode(is_in_ons_postcode_directory=True, fix_distance=0, original='EC1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB')
 ```
```

### Comparing `uk_postcodes_parsing-1.0.0/pyproject.toml` & `uk_postcodes_parsing-1.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "uk_postcodes_parsing"
-version = "1.0.0"
+version = "1.0.2"
 authors = [
   { name="Anirudh Gangwal", email="angangwa@amazon.com" },
 ]
 description = "A Python package to parse UK postcodes from text. Useful in applications such as OCR and IDP."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `uk_postcodes_parsing-1.0.0/PKG-INFO` & `uk_postcodes_parsing-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk_postcodes_parsing
-Version: 1.0.0
+Version: 1.0.2
 Summary: A Python package to parse UK postcodes from text. Useful in applications such as OCR and IDP.
 Project-URL: Homepage, https://github.com/anirudhgangwal/ukpostcodes
 Project-URL: Bug Tracker, https://github.com/anirudhgangwal/ukpostcodes/issues
 Author-email: Anirudh Gangwal <angangwa@amazon.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -72,14 +72,27 @@
 >>> from uk_postcodes_parsing import ukpostcode
 >>> corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e3 4ss. But also eh16 50y and ei412"
 >>> postcodes = ukpostcode.parse_from_corpus(corpus, attempt_fix=True)
 INFO:uk-postcodes-parsing:Found 3 postcodes in corpus
 INFO:uk-postcodes-parsing:Postcode Fixed: 'eh16 50y' => 'EH16 5OY'
 ```
 
+You can also do an undertermisitic postcode auto-correct where if there is more than one possible answer, all answers are returned.
+
+```python
+>>> postcodes = ukpostcode.parse_from_corpus("OOO 4SS",
+                             attempt_fix=True,
+                             try_all_fix_options=True
+                             )
+>> postcodes # "O00 4SS", "OO0 4SS", and "O0O 4SS"
+[Postcode(is_in_ons_postcode_directory=False, fix_distance=-2, original='OOO 4SS', postcode='O00 4SS', incode='4SS', outcode='O00', area='O', district='O00', sub_district=None, sector='O00 4', unit='SS'),
+ Postcode(is_in_ons_postcode_directory=False, fix_distance=-1, original='OOO 4SS', postcode='OO0 4SS', incode='4SS', outcode='OO0', area='OO', district='OO0', sub_district=None, sector='OO0 4', unit='SS'),
+ Postcode(is_in_ons_postcode_directory=False, fix_distance=-1, original='OOO 4SS', postcode='O0O 4SS', incode='4SS', outcode='O0O', area='O', district='O0', sub_district='O0O', sector='O0O 4', unit='SS')]
+```
+
 - Parsing
 
 ```python
 >>> from uk_postcodes_parsing import ukpostcode
 >>> ukpostcode.parse("EC1r 1ub")
 Postcode(is_in_ons_postcode_directory=True, fix_distance=0, original='EC1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB')
 ```
```

