# Comparing `tmp/uk_postcodes_parsing-0.3.0.tar.gz` & `tmp/uk_postcodes_parsing-1.0.0.tar.gz`

## Comparing `uk_postcodes_parsing-0.3.0.tar` & `uk_postcodes_parsing-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/__init__.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/fix.py
--rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/postcode_utils.py
--rw-r--r--   0        0        0 20547700 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/postcodes_nov_2022.py
--rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/ukpostcode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/tests/test_all.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/tests/data/postcode_parse_test.csv
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/LICENSE
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/README.md
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     9591 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/__init__.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/fix.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/postcode_utils.py
+-rw-r--r--   0        0        0 20547700 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/postcodes_nov_2022.py
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/ukpostcode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/tests/test_all.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/tests/data/postcode_parse_test.csv
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/LICENSE
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/README.md
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9591 2020-02-02 00:00:00.000000 uk_postcodes_parsing-1.0.0/PKG-INFO
```

### Comparing `uk_postcodes_parsing-0.3.0/.pre-commit-config.yaml` & `uk_postcodes_parsing-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.3.0/.github/workflows/python-publish.yml` & `uk_postcodes_parsing-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.3.0/.github/workflows/test.yml` & `uk_postcodes_parsing-1.0.0/.github/workflows/test.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 name: Test
 
-on: 
+on:
   push:
     paths:
       - 'tests/**'
       - 'src/uk_postcodes_parsing/**'
   workflow_dispatch:
 
 jobs:
   Quality-checks:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
```

### Comparing `uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/postcode_utils.py` & `uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/postcode_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """
 postcode_utils.py: Utilities for working with postcodes.
 """
 import re
 from typing import Union
 
+from uk_postcodes_parsing.postcodes_nov_2022 import POSTCODE_NOV_2022
+
+
 # Tests for district
 DISTRICT_SPLIT_REGEX = re.compile(r"^([a-z]{1,2}\d)([a-z])$", re.I)
 
 # Tests for the unit section of a postcode
 UNIT_REGEX = re.compile(r"[a-z]{2}$", re.I)
 
 # Tests for the inward code section of a postcode
```

### Comparing `uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/postcodes_nov_2022.py` & `uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/postcodes_nov_2022.py`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/ukpostcode.py` & `uk_postcodes_parsing-1.0.0/src/uk_postcodes_parsing/ukpostcode.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,24 +13,24 @@
     to_incode,
     to_area,
     to_sector,
     to_unit,
     to_district,
     to_sub_district,
 )
-from uk_postcodes_parsing.fix import fix
+from uk_postcodes_parsing.fix import fix, fix_with_options
 from uk_postcodes_parsing.postcodes_nov_2022 import POSTCODE_NOV_2022
 
 logging.basicConfig(level=logging.INFO)
-logger = logging.getLogger("uk-postcodes-parsing")
+logger = logging.getLogger("uk-postcodes-parsing.ukpostcode")
 
 # Test for a valid postcode embedded in text
 POSTCODE_CORPUS_REGEX = re.compile(r"[a-z]{1,2}\d[a-z\d]?\s*\d[a-z]{2}", re.I)
 FIXABLE_POSTCODE_CORPUS_REGEX = re.compile(
-    r"[a-z01]{1,2}[0-9oi][a-z\d]?\s*[0-9oi][a-z01]{2}"
+    r"[a-z01]{1,2}[0-9oi][a-z\d]?\s*[0-9oi][a-z01]{2}", re.I
 )
 
 SPECIAL_CASE_POSTCODES = ("GIR", "NPT", "BX", "BF")
 
 logger.debug("Imported POSTCODE_NOV_2022 with length: %s", len(POSTCODE_NOV_2022))
 
 
@@ -119,15 +119,36 @@
         "district": to_district(postcode),
         "sub_district": to_sub_district(postcode),
         "sector": to_sector(postcode),
         "unit": to_unit(postcode),
     }
 
 
-def parse(postcode, attempt_fix=True) -> Optional[Postcode]:
+def parse_all_options(postcode) -> List[Postcode]:
+    """Parse possible postcodes
+
+    Args:
+        postcode (str): Postcode to parse. E.g. "EC1R 1UB".
+        attempt_fix (bool): Attempt to fix postcodes. Defaults to True.
+    Returns:
+        Postcode: Parsed postcode.
+    """
+    if postcode.strip().upper().startswith(SPECIAL_CASE_POSTCODES):  # Edge case logging
+        logger.info("Found special case postcode: %s", postcode)
+    if is_valid(postcode):
+        return [Postcode(**_parse(postcode), original=postcode)]
+    else:
+        fixed_list = fix_with_options(postcode)
+        return [
+            Postcode(**_parse(fixed_postcode), original=postcode)
+            for fixed_postcode in fixed_list
+        ]
+
+
+def parse(postcode: str, attempt_fix: bool = True) -> Optional[Postcode]:
     """Parse a postcode
 
     Args:
         postcode (str): Postcode to parse. E.g. "EC1R 1UB".
         attempt_fix (bool): Attempt to fix postcodes. Defaults to True.
     Returns:
         Postcode: Parsed postcode.
@@ -142,30 +163,46 @@
             logger.info("Postcode Fixed: '%s' => '%s'", postcode, fixed)
             return Postcode(**_parse(fixed), original=postcode)
         logger.error("Unable to fix postcode")
     logger.error("Failed to parse postcode: %s", postcode)
     return None
 
 
-def parse_from_corpus(text: str, attempt_fix=False) -> List[str]:
+def parse_from_corpus(
+    text: str, attempt_fix=False, try_all_fix_options=False
+) -> List[Postcode]:
     """Parse postcodes from a text corpus
 
     Args:
         text (str): Text corpus. E.g. "The postcode could be EC1R 1UB or EC1R IUB"
         attempt_fix (bool): Attempt to fix postcodes. Defaults to False.
+        try_all_fix_options (bool): If postcode is invalid and attempt_fix=True, this option
+            tries all possibilites to correct mistakes. Note this can create postcodes out of
+            invaid text in edge cases.
     Returns:
         List[Postcode]: List of parsed postcodes.
 
     """
+    if try_all_fix_options and not attempt_fix:
+        raise ValueError("attempt_fix must be true if try_all_fix_options is True")
+
     if attempt_fix:
-        postcodes = re.findall(FIXABLE_POSTCODE_CORPUS_REGEX, text.lower())
+        postcodes = re.findall(FIXABLE_POSTCODE_CORPUS_REGEX, text)
+        if try_all_fix_options:
+            postcodes = [parse_all_options(postcode) for postcode in postcodes]
+            postcodes = [item for sublist in postcodes for item in sublist]  # Flatten
+        else:
+            postcodes = [parse(postcode, attempt_fix=True) for postcode in postcodes]
+            postcodes = [postcode for postcode in postcodes if postcode is not None]
+        return postcodes
     else:
-        postcodes = re.findall(POSTCODE_CORPUS_REGEX, text.lower())
-    logger.info("Found %d postcodes in corpus", len(postcodes))
-    return list(map(parse, postcodes))
+        postcodes = re.findall(POSTCODE_CORPUS_REGEX, text)
+        postcodes = [parse(postcode, attempt_fix=False) for postcode in postcodes]
+        postcodes = [postcode for postcode in postcodes if postcode is not None]
+        return postcodes
 
 
 def is_in_ons_postcode_directory(postcode: str) -> bool:
     """Check if the postcode is valid with postcodes.io
 
     Args:
         postcode (str): The postcode to check
```

### Comparing `uk_postcodes_parsing-0.3.0/tests/test_all.py` & `uk_postcodes_parsing-1.0.0/tests/test_all.py`

 * *Files 18% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
 
 def test_sort_by_fix_distance():
     corpus = "this EC1r 1ub followed by to one, ecir iub e0 i00"
     lst = parse_from_corpus(corpus, attempt_fix=True)
     assert sorted(lst, reverse=True) == [
         Postcode(
-            original="ec1r 1ub",
+            original="EC1r 1ub",
             postcode="EC1R 1UB",
             incode="1UB",
             outcode="EC1R",
             area="EC",
             district="EC1",
             sub_district="EC1R",
             sector="EC1R 1",
@@ -191,7 +191,46 @@
             area="E",
             district="E0",
             sub_district=None,
             sector="E0 1",
             unit="OO",
         ),
     ]
+
+
+def test_parse_from_corpus():
+    corpus = "sso 7hg HA0 1AQ"
+    lst = parse_from_corpus(corpus)
+    assert lst[0].is_in_ons_postcode_directory
+    assert lst[0].fix_distance == 0
+    assert lst[0].postcode == "HA0 1AQ"
+
+    corpus = "sso 7hg HA0 1AQ"
+    lst = parse_from_corpus(corpus, attempt_fix=True)
+    assert lst[0].is_in_ons_postcode_directory
+    assert lst[0].fix_distance == 0
+    assert lst[0].postcode == "HA0 1AQ"
+
+    corpus = "sso 7hg HAO 1AQ"
+    lst = parse_from_corpus(corpus, attempt_fix=True)
+    assert lst == []
+
+    corpus = "sso 7hg HA0 1AQ"
+    lst = parse_from_corpus(corpus, attempt_fix=True, try_all_fix_options=True)
+    assert lst[0].is_in_ons_postcode_directory
+    assert lst[0].fix_distance == -1
+    assert lst[0].postcode == "SS0 7HG"
+
+    assert lst[1].is_in_ons_postcode_directory
+    assert lst[1].fix_distance == 0
+    assert lst[1].postcode == "HA0 1AQ"
+
+    corpus = "OOO 4SS"
+    lst = [
+        postcode.postcode
+        for postcode in parse_from_corpus(
+            corpus, attempt_fix=True, try_all_fix_options=True
+        )
+    ]
+    assert "O00 4SS" in lst  # LNN
+    assert "OO0 4SS" in lst  # LLN
+    assert "O0O 4SS" in lst  # LNL
```

### Comparing `uk_postcodes_parsing-0.3.0/.gitignore` & `uk_postcodes_parsing-1.0.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# vs code
+.DS_Store
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `uk_postcodes_parsing-0.3.0/LICENSE` & `uk_postcodes_parsing-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.3.0/README.md` & `uk_postcodes_parsing-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.3.0/PKG-INFO` & `uk_postcodes_parsing-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: uk_postcodes_parsing
-Version: 0.3.0
+Version: 1.0.0
 Summary: A Python package to parse UK postcodes from text. Useful in applications such as OCR and IDP.
 Project-URL: Homepage, https://github.com/anirudhgangwal/ukpostcodes
 Project-URL: Bug Tracker, https://github.com/anirudhgangwal/ukpostcodes/issues
 Author-email: Anirudh Gangwal <angangwa@amazon.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: lint
 Requires-Dist: black; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: bandit[toml]; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
```

