# Comparing `tmp/data_product_definition_tooling-0.0.8.tar.gz` & `tmp/data_product_definition_tooling-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_product_definition_tooling-0.0.8.tar", max compression
+gzip compressed data, was "data_product_definition_tooling-0.0.9.tar", max compression
```

## Comparing `data_product_definition_tooling-0.0.8.tar` & `data_product_definition_tooling-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1519 2023-01-02 10:29:18.359686 data_product_definition_tooling-0.0.8/LICENSE
--rw-r--r--   0        0        0      597 2023-01-02 10:29:18.359686 data_product_definition_tooling-0.0.8/README.md
--rw-r--r--   0        0        0      145 2023-01-02 10:29:18.359686 data_product_definition_tooling-0.0.8/converter/__init__.py
--rw-r--r--   0        0        0      620 2023-01-02 10:29:18.359686 data_product_definition_tooling-0.0.8/converter/cli.py
--rw-r--r--   0        0        0     6000 2023-01-02 10:29:18.359686 data_product_definition_tooling-0.0.8/converter/converter.py
--rw-r--r--   0        0        0     5498 2023-01-02 10:29:18.359686 data_product_definition_tooling-0.0.8/converter/tests/__snapshots__/test_converter/test_air_quality.json
--rw-r--r--   0        0        0     5706 2023-01-02 10:29:18.359686 data_product_definition_tooling-0.0.8/converter/tests/__snapshots__/test_converter/test_current_weather_required_headers.json
--rw-r--r--   0        0        0      175 2023-01-02 10:29:18.359686 data_product_definition_tooling-0.0.8/converter/tests/conftest.py
--rw-r--r--   0        0        0     1642 2023-01-02 10:29:18.359686 data_product_definition_tooling-0.0.8/converter/tests/data/AirQuality/Current.py
--rw-r--r--   0        0        0     1625 2023-01-02 10:29:18.359686 data_product_definition_tooling-0.0.8/converter/tests/data/Weather/Current/Metric.py
--rw-r--r--   0        0        0     2417 2023-01-02 10:29:18.359686 data_product_definition_tooling-0.0.8/converter/tests/test_converter.py
--rw-r--r--   0        0        0      957 2023-01-02 10:29:18.359686 data_product_definition_tooling-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1782 1970-01-01 00:00:00.000000 data_product_definition_tooling-0.0.8/setup.py
--rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 data_product_definition_tooling-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1519 2023-01-27 14:49:28.878645 data_product_definition_tooling-0.0.9/LICENSE
+-rw-r--r--   0        0        0      597 2023-01-27 14:49:28.878645 data_product_definition_tooling-0.0.9/README.md
+-rw-r--r--   0        0        0      145 2023-01-27 14:49:28.878645 data_product_definition_tooling-0.0.9/converter/__init__.py
+-rw-r--r--   0        0        0      620 2023-01-27 14:49:28.878645 data_product_definition_tooling-0.0.9/converter/cli.py
+-rw-r--r--   0        0        0     6089 2023-01-27 14:49:28.878645 data_product_definition_tooling-0.0.9/converter/converter.py
+-rw-r--r--   0        0        0     5497 2023-01-27 14:49:28.878645 data_product_definition_tooling-0.0.9/converter/tests/__snapshots__/test_converter/test_air_quality.json
+-rw-r--r--   0        0        0     5708 2023-01-27 14:49:28.882645 data_product_definition_tooling-0.0.9/converter/tests/__snapshots__/test_converter/test_current_weather_required_headers.json
+-rw-r--r--   0        0        0      175 2023-01-27 14:49:28.882645 data_product_definition_tooling-0.0.9/converter/tests/conftest.py
+-rw-r--r--   0        0        0     1642 2023-01-27 14:49:28.882645 data_product_definition_tooling-0.0.9/converter/tests/data/AirQuality/Current.py
+-rw-r--r--   0        0        0     1625 2023-01-27 14:49:28.882645 data_product_definition_tooling-0.0.9/converter/tests/data/Weather/Current/Metric.py
+-rw-r--r--   0        0        0     2417 2023-01-27 14:49:28.882645 data_product_definition_tooling-0.0.9/converter/tests/test_converter.py
+-rw-r--r--   0        0        0      957 2023-01-27 14:49:28.882645 data_product_definition_tooling-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1782 1970-01-01 00:00:00.000000 data_product_definition_tooling-0.0.9/setup.py
+-rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 data_product_definition_tooling-0.0.9/PKG-INFO
```

### Comparing `data_product_definition_tooling-0.0.8/LICENSE` & `data_product_definition_tooling-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `data_product_definition_tooling-0.0.8/README.md` & `data_product_definition_tooling-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `data_product_definition_tooling-0.0.8/converter/cli.py` & `data_product_definition_tooling-0.0.9/converter/cli.py`

 * *Files identical despite different names*

### Comparing `data_product_definition_tooling-0.0.8/converter/converter.py` & `data_product_definition_tooling-0.0.9/converter/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         super().__init__(**kwargs)
 
         if self.summary:
             if not self.route_description:
                 self.route_description = self.summary
             if not self.description:
                 self.description = self.summary
+            if not self.route_summary:
+                self.route_summary = self.summary
 
 
 def export_openapi_spec(definition: DataProductDefinition) -> dict:
     """
     Given a data product definition, create a FastAPI application and a corresponding
     POST route. Then export its OpenAPI spec
     :param definition: Data product definition
```

### Comparing `data_product_definition_tooling-0.0.8/converter/tests/__snapshots__/test_converter/test_air_quality.json` & `data_product_definition_tooling-0.0.9/converter/tests/__snapshots__/test_converter/test_air_quality.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333333%*

 * *Differences: {"'paths'": "{'/AirQuality/Current': {'post': {'summary': 'Air Quality Index'}}}"}*

```diff
@@ -184,12 +184,12 @@
                                     "$ref": "#/components/schemas/HTTPValidationError"
                                 }
                             }
                         },
                         "description": "Validation Error"
                     }
                 },
-                "summary": "AirQuality/Current"
+                "summary": "Air Quality Index"
             }
         }
     }
 }
```

### Comparing `data_product_definition_tooling-0.0.8/converter/tests/__snapshots__/test_converter/test_current_weather_required_headers.json` & `data_product_definition_tooling-0.0.9/converter/tests/__snapshots__/test_converter/test_current_weather_required_headers.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333333%*

 * *Differences: {"'paths'": "{'/Weather/Current/Metric': {'post': {'summary': 'Current Weather (Metric)'}}}"}*

```diff
@@ -197,12 +197,12 @@
                                     "$ref": "#/components/schemas/HTTPValidationError"
                                 }
                             }
                         },
                         "description": "Validation Error"
                     }
                 },
-                "summary": "Weather/Current/Metric"
+                "summary": "Current Weather (Metric)"
             }
         }
     }
 }
```

### Comparing `data_product_definition_tooling-0.0.8/converter/tests/data/AirQuality/Current.py` & `data_product_definition_tooling-0.0.9/converter/tests/data/AirQuality/Current.py`

 * *Files identical despite different names*

### Comparing `data_product_definition_tooling-0.0.8/converter/tests/data/Weather/Current/Metric.py` & `data_product_definition_tooling-0.0.9/converter/tests/data/Weather/Current/Metric.py`

 * *Files identical despite different names*

### Comparing `data_product_definition_tooling-0.0.8/converter/tests/test_converter.py` & `data_product_definition_tooling-0.0.9/converter/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `data_product_definition_tooling-0.0.8/setup.py` & `data_product_definition_tooling-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 
 package_data = \
 {'': ['*'], 'converter.tests': ['__snapshots__/test_converter/*']}
 
 install_requires = \
 ['deepdiff>=6.2.2,<7.0.0',
  'fastapi>=0.88.0,<0.89.0',
- 'pydantic[email]>=1.10.2,<2.0.0',
+ 'pydantic[email]>=1.10.4,<2.0.0',
  'stringcase>=1.2.0,<2.0.0',
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['converter = converter.cli:cli']}
 
 setup_kwargs = {
     'name': 'data-product-definition-tooling',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Data Product Definition Tooling',
     'long_description': '# Data Product Definitions tooling\n\nTools for managing Data Product definitions\n\n# Installation\n\n```shell\npoetry install\n```\n\n# Usage\n\n```shell\npoetry run converter --help\n\n# run tests\npoetry run invoke test\n\n# release a new version (after bumping it in pyproject.toml)\npoetry run invoke release\n```\n\n## Pre-commit hooks\n\n```yaml\nrepos:\n  - repo: https://github.com/ioxio-dataspace/data-product-definition-tooling\n    rev: main # You probably want to lock this to a specific tag\n    hooks:\n      - id: data-product-definition-converter\n        files: "src/.*py$"\n        args: ["src", "dest"]\n```\n',
     'author': 'Digital Living International Ltd',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ioxio-dataspace/data-product-definition-tooling',
```

### Comparing `data_product_definition_tooling-0.0.8/PKG-INFO` & `data_product_definition_tooling-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: data-product-definition-tooling
-Version: 0.0.8
+Version: 0.0.9
 Summary: Data Product Definition Tooling
 Home-page: https://github.com/ioxio-dataspace/data-product-definition-tooling
 License: BSD-3-Clause
 Author: Digital Living International Ltd
 Requires-Python: >=3.9.0,<4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: deepdiff (>=6.2.2,<7.0.0)
 Requires-Dist: fastapi (>=0.88.0,<0.89.0)
-Requires-Dist: pydantic[email] (>=1.10.2,<2.0.0)
+Requires-Dist: pydantic[email] (>=1.10.4,<2.0.0)
 Requires-Dist: stringcase (>=1.2.0,<2.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/ioxio-dataspace/data-product-definition-tooling
 Description-Content-Type: text/markdown
 
 # Data Product Definitions tooling
```

