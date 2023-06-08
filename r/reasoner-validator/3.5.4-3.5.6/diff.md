# Comparing `tmp/reasoner_validator-3.5.4.tar.gz` & `tmp/reasoner_validator-3.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.5.4.tar", max compression
+gzip compressed data, was "reasoner_validator-3.5.6.tar", max compression
```

## Comparing `reasoner_validator-3.5.4.tar` & `reasoner_validator-3.5.6.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1153 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/LICENSE
--rw-r--r--   0        0        0    12164 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/README.md
--rw-r--r--   0        0        0      131 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/Makefile
--rw-r--r--   0        0        0     2288 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/conf.py
--rw-r--r--   0        0        0    18216 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/index.rst
--rw-r--r--   0        0        0      795 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/make.bat
--rw-r--r--   0        0        0      136 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    36025 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2093 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/pyproject.toml
--rw-r--r--   0        0        0    20298 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    59895 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    39243 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0    26512 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4350 2023-06-01 17:48:46.742933 reasoner_validator-3.5.4/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0     7977 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    13781 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0     9922 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/reasoner_validator/versioning.py
--rw-r--r--   0        0        0        0 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/__init__.py
--rw-r--r--   0        0        0   104709 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    42178 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_data/sample_trapi_schema.yaml
--rw-r--r--   0        0        0    31906 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_response_validator.py
--rw-r--r--   0        0        0     4546 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_semver.py
--rw-r--r--   0        0        0     1746 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    26567 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_validate.py
--rw-r--r--   0        0        0    19013 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_validation_report.py
--rw-r--r--   0        0        0     2068 2023-06-01 17:48:46.746933 reasoner_validator-3.5.4/tests/test_workflows.py
--rw-r--r--   0        0        0    14203 1970-01-01 00:00:00.000000 reasoner_validator-3.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/LICENSE
+-rw-r--r--   0        0        0    12431 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/README.md
+-rw-r--r--   0        0        0      131 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/Makefile
+-rw-r--r--   0        0        0     2288 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/conf.py
+-rw-r--r--   0        0        0    18216 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    36025 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2093 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/pyproject.toml
+-rw-r--r--   0        0        0    20545 2023-06-08 21:17:05.755437 reasoner_validator-3.5.6/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    61249 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    39243 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0    26862 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4350 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0     9718 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    13781 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0     9922 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0        0 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/conftest.py
+-rw-r--r--   0        0        0   111722 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    42178 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_data/sample_trapi_schema.yaml
+-rw-r--r--   0        0        0    31899 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_response_validator.py
+-rw-r--r--   0        0        0     4533 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_semver.py
+-rw-r--r--   0        0        0     1746 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    26543 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_validate.py
+-rw-r--r--   0        0        0    19013 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2061 2023-06-08 21:17:05.759437 reasoner_validator-3.5.6/tests/test_workflows.py
+-rw-r--r--   0        0        0    14470 1970-01-01 00:00:00.000000 reasoner_validator-3.5.6/PKG-INFO
```

### Comparing `reasoner_validator-3.5.4/LICENSE` & `reasoner_validator-3.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.4/README.md` & `reasoner_validator-3.5.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,26 +45,31 @@
 
 To develop this package, install with all extras dependencies using:
 
 ```bash
 poetry install --all-extras
 ```
 
-## Running Validation against an ARS UUID Result(*)
+## Running Validation against an ARS UUID Result(*) or using a Local TRAPI Request Query
 
-A local script **`ars_uuid_result_test_runner.py`** is available to run TRAPI Response validation against a 
-UUID indexed query result of the Biomedical Knowledge Translator "Autonomous Relay System" (ARS).
+A local script **`trapi_validator.py`** is available to run TRAPI Response validation against either a PK (UUID)
+indexed query result of the Biomedical Knowledge Translator "Autonomous Relay System" (ARS), a local JSON Response
+text file or a locally triggered _ad hoc_ query Request against an directly specified TRAPI endpoint.
 
-For usage, type:
+Note that it is best run within a **`poetry shell`** created by **`poetry install`**.
+
+For script usage, type:
 
 ```bash
-./ars_uuid_result_test_runner.py --help
+./trapi_validator.py --help
 ```
 
-(*) Thank you Eric Deutsch for the prototype of this script
+The script allows
+
+(*) Thank you Eric Deutsch for the prototype code for this script
 
 ## Running tests
 
 To run the test locally install with the `dev` dependencies group if not already done:
 
 ```bash
 poetry install --extras dev
```

### Comparing `reasoner_validator-3.5.4/docs/Makefile` & `reasoner_validator-3.5.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.4/docs/conf.py` & `reasoner_validator-3.5.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.4/docs/index.rst` & `reasoner_validator-3.5.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.4/docs/make.bat` & `reasoner_validator-3.5.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.4/docs/validation_codes_dictionary.md` & `reasoner_validator-3.5.6/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.4/pyproject.toml` & `reasoner_validator-3.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.5.4"
+version = "3.5.6"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.5.4/reasoner_validator/__init__.py` & `reasoner_validator-3.5.6/reasoner_validator/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,26 +229,28 @@
                     instance=query_graph,
                     component="QueryGraph",
                     trapi_version=self.trapi_version
                 )
                 if trapi_validator.has_messages():
                     self.merge(trapi_validator)
 
-                # Validate the Biolink Model compliance of the Query Graph
-                biolink_validator = check_biolink_model_compliance_of_query_graph(
-                    graph=query_graph,
-                    biolink_version=self.biolink_version,
-                    # the ValidationReporter calling this function *might*
-                    # have an explicit strict_validation override (if not None)
-                    strict_validation=self.strict_validation
-                )
-                if biolink_validator.has_messages():
-                    self.merge(biolink_validator)
-                    # 'info' and 'warning' messages do
-                    # not fully invalidate the query_graph
+                if self.validate_biolink():
+                    # Conduct validation of Biolink Model compliance
+                    # of the Query Graph, if not suppressed...
+                    biolink_validator = check_biolink_model_compliance_of_query_graph(
+                        graph=query_graph,
+                        biolink_version=self.biolink_version,
+                        # the ValidationReporter calling this function *might*
+                        # have an explicit strict_validation override (if not None)
+                        strict_validation=self.strict_validation
+                    )
+                    if biolink_validator.has_messages():
+                        self.merge(biolink_validator)
+                        # 'info' and 'warning' messages do
+                        # not fully invalidate the query_graph
 
         # Only 'error' but not 'info' nor 'warning' messages invalidate the overall Message
         return False if self.has_errors() else True
 
     def has_valid_knowledge_graph(self, message: Dict, edges_limit: int = 100) -> bool:
         """
         Validate a TRAPI Knowledge Graph.
@@ -295,28 +297,29 @@
                     instance=kg_sample,
                     component="KnowledgeGraph",
                     trapi_version=self.trapi_version
                 )
                 if trapi_validator.has_messages():
                     self.merge(trapi_validator)
 
-                # Verify that the sample of the knowledge graph is
-                # compliant to the currently applicable Biolink Model release
-                biolink_validator: BiolinkValidator = \
-                    check_biolink_model_compliance_of_knowledge_graph(
-                        graph=kg_sample,
-                        trapi_version=self.trapi_version,
-                        biolink_version=self.biolink_version,
-                        sources=self.sources,
-                        # the ValidationReporter calling this function *might*
-                        # have an explicit strict_validation override (if not None)
-                        strict_validation=self.strict_validation
-                    )
-                if biolink_validator.has_messages():
-                    self.merge(biolink_validator)
+                if self.validate_biolink():
+                    # Conduct validation of Biolink Model compliance of the
+                    # Knowledge Graph, if Biolink validation not suppressed...
+                    biolink_validator: BiolinkValidator = \
+                        check_biolink_model_compliance_of_knowledge_graph(
+                            graph=kg_sample,
+                            trapi_version=self.trapi_version,
+                            biolink_version=self.biolink_version,
+                            sources=self.sources,
+                            # the ValidationReporter calling this function *might*
+                            # have an explicit strict_validation override (if not None)
+                            strict_validation=self.strict_validation
+                        )
+                    if biolink_validator.has_messages():
+                        self.merge(biolink_validator)
 
         # Only 'error' but not 'info' nor 'warning' messages invalidate the overall Message
         return False if self.has_errors() else True
 
     def has_valid_results(self, message: Dict) -> bool:
         """
         Validate a TRAPI Results.
```

### Comparing `reasoner_validator-3.5.4/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.5.6/reasoner_validator/biolink/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from enum import Enum
 from functools import lru_cache
 from urllib.error import HTTPError
 from pprint import PrettyPrinter
 
 
 from bmt import Toolkit
-from bmt.utils import parse_name
 from linkml_runtime.linkml_model import ClassDefinition, Element
 
 from reasoner_validator.sri.util import is_curie
 from reasoner_validator.report import ValidationReporter
 from reasoner_validator.versioning import SemVer, SemVerError
 
 import logging
@@ -35,15 +34,14 @@
         except SemVerError:
             raise TypeError(
                 "The 'biolink_version' argument '"
                 + biolink_version
                 + "' is not a properly formatted semantic version?"
             )
 
-
         if svm >= SemVer.from_string("2.2.14"):
             biolink_version = "v" + str(svm)
         else:
             biolink_version = str(svm)
         schema = f"https://raw.githubusercontent.com/biolink/biolink-model/{biolink_version}/biolink-model.yaml"
         return schema
     else:
@@ -105,16 +103,21 @@
         :param trapi_version: caller specified Biolink Model version (default: None, which takes the TRAPI 'latest')
         :type trapi_version: Optional[str] or None
         :param biolink_version: caller specified Biolink Model version (default: None, which takes the BMT 'latest')
         :type biolink_version: Optional[str] or None
         :param sources: Dictionary of validation context identifying the ARA and KP for provenance attribute validation
         :type sources: Optional[Dict[str,str]]
         """
-        self.bmt: Toolkit = get_biolink_model_toolkit(biolink_version=biolink_version)
-        resolved_biolink_version = self.bmt.get_model_version()
+        self.bmt: Optional[Toolkit] = None
+        if biolink_version != "suppress":
+            # Here, the Biolink Model version is validated, and the relevant Toolkit pulled.
+            self.bmt = get_biolink_model_toolkit(biolink_version=biolink_version)
+            resolved_biolink_version = self.bmt.get_model_version()
+        else:
+            resolved_biolink_version = "suppress"
         ValidationReporter.__init__(
             self,
             prefix=f"Biolink Validation of {graph_type.value}",
             trapi_version=trapi_version,
             biolink_version=resolved_biolink_version,
             sources=sources,
             strict_validation=strict_validation
@@ -159,48 +162,50 @@
             # TODO: this will fail for an earlier TRAPI data schema version
             #       which didn't use the tag 'categories' for nodes...
             #       probably no longer relevant to the community?
             if 'categories' in slots:
                 if not isinstance(slots["categories"], List):
                     self.report(code="error.knowledge_graph.node.categories.not_array", identifier=node_id)
                 else:
-                    categories = slots["categories"]
-                    node_prefix_mapped: bool = False
-                    concrete_category_found: bool = False
-                    for category in categories:
-                        category: Optional[ClassDefinition] = \
-                            self.validate_category(
-                                context="knowledge_graph",
-                                node_id=node_id,
-                                category=category
-                            )
-                        # Only 'concrete' (non-abstract, non-mixin, preferably,
-                        # non-deprecated) categories are of interest here,
-                        # since only they will have associated namespaces
-                        if category:
-                            concrete_category_found: bool = True
-                            possible_subject_categories = self.bmt.get_element_by_prefix(node_id)
-                            if possible_subject_categories and category.name in possible_subject_categories:
-                                node_prefix_mapped = True
-                                # don't need to search any more categories
-                                break
+                    if self.validate_biolink():
+                        # Biolink Validation of node, if not suppressed
+                        categories = slots["categories"]
+                        node_prefix_mapped: bool = False
+                        concrete_category_found: bool = False
+                        for category in categories:
+                            category: Optional[ClassDefinition] = \
+                                self.validate_category(
+                                    context="knowledge_graph",
+                                    node_id=node_id,
+                                    category=category
+                                )
+                            # Only 'concrete' (non-abstract, non-mixin, preferably,
+                            # non-deprecated) categories are of interest here,
+                            # since only they will have associated namespaces
+                            if category:
+                                concrete_category_found: bool = True
+                                possible_subject_categories = self.bmt.get_element_by_prefix(node_id)
+                                if possible_subject_categories and category.name in possible_subject_categories:
+                                    node_prefix_mapped = True
+                                    # don't need to search any more categories
+                                    break
 
-                    if not concrete_category_found:
-                        self.report(
-                            code="error.knowledge_graph.node.categories.not_concrete",
-                            identifier=node_id,
-                            categories=str(categories)
-                        )
+                        if not concrete_category_found:
+                            self.report(
+                                code="error.knowledge_graph.node.categories.not_concrete",
+                                identifier=node_id,
+                                categories=str(categories)
+                            )
 
-                    if not node_prefix_mapped:
-                        self.report(
-                            code="warning.knowledge_graph.node.id.unmapped_prefix",
-                            identifier=node_id,
-                            categories=str(categories)
-                        )
+                        if not node_prefix_mapped:
+                            self.report(
+                                code="warning.knowledge_graph.node.id.unmapped_prefix",
+                                identifier=node_id,
+                                categories=str(categories)
+                            )
             else:
                 self.report(
                     code="error.knowledge_graph.node.category.missing",
                     context=self.graph_type.value, identifier=node_id
                 )
 
             # TODO: Do we need to (or can we) validate here, any other
@@ -227,43 +232,45 @@
 
             if "categories" in slots:
                 categories = slots["categories"]
                 if categories:
                     if not isinstance(categories, List):
                         self.report(code="error.query_graph.node.categories.not_array", identifier=node_id)
                     else:
-                        id_prefix_mapped: Dict = {identifier: False for identifier in node_ids}
-                        for category in categories:
-                            category: Optional[ClassDefinition] = \
-                                self.validate_category(
-                                    context="query_graph",
-                                    node_id=node_id,
-                                    category=category
+                        if self.validate_biolink():
+                            # Biolink Validation of node, if not suppressed
+                            id_prefix_mapped: Dict = {identifier: False for identifier in node_ids}
+                            for category in categories:
+                                category: Optional[ClassDefinition] = \
+                                    self.validate_category(
+                                        context="query_graph",
+                                        node_id=node_id,
+                                        category=category
+                                    )
+                                # Only 'concrete' (non-abstract, non-mixin, preferably, non-deprecated)
+                                # categories will be tested here for identifier namespaces.  Also, we
+                                # actually don't care if Query Graphs don't have at least one concrete category...
+                                if category:
+                                    for identifier in node_ids:  # may be empty list if not provided...
+                                        possible_subject_categories = self.bmt.get_element_by_prefix(identifier)
+                                        if category.name in possible_subject_categories:
+                                            id_prefix_mapped[identifier] = True
+                                            node_ids.remove(identifier)
+                                            # found a suitable mapping for the given identifier
+                                            break
+
+                            # At this point, if any 'node_ids' are NOT
+                            # removed (above), then they are unmapped
+                            if has_node_ids and node_ids:
+                                self.report(
+                                    code="warning.query_graph.node.ids.unmapped_prefix",
+                                    identifier=node_id,
+                                    unmapped_ids=str(node_ids),
+                                    categories=str(categories)
                                 )
-                            # Only 'concrete' (non-abstract, non-mixin, preferably, non-deprecated)
-                            # categories will be tested here for identifier namespaces.  Also, we
-                            # actually don't care if Query Graphs don't have at least one concrete category...
-                            if category:
-                                for identifier in node_ids:  # may be empty list if not provided...
-                                    possible_subject_categories = self.bmt.get_element_by_prefix(identifier)
-                                    if category.name in possible_subject_categories:
-                                        id_prefix_mapped[identifier] = True
-                                        node_ids.remove(identifier)
-                                        # found a suitable mapping for the given identifier
-                                        break
-
-                        # At this point, if any 'node_ids' are NOT
-                        # removed (above), then they are unmapped
-                        if has_node_ids and node_ids:
-                            self.report(
-                                code="warning.query_graph.node.ids.unmapped_prefix",
-                                identifier=node_id,
-                                unmapped_ids=str(node_ids),
-                                categories=str(categories)
-                            )
 
                 # else:  # null "categories" value is permitted in QNodes by nullable: true
             # else:  # missing "categories" key is permitted in QNodes by nullable: true
 
             if 'is_set' in slots:
                 is_set = slots["is_set"]
                 if is_set and not isinstance(is_set, bool):
@@ -392,20 +399,24 @@
         Validate Knowledge Edge Attributes.
 
         :param edge_id: str, string identifier for the edge (for reporting purposes)
         :param edge: Dict, the edge object associated with some attributes are expected to be found
         :return: None (validation messages captured in the 'self' BiolinkValidator context)
         """
         # we only report errors about missing or empty edge attributes if TRAPI 1.3.0 or earlier,
+        # and Biolink Validation is not suppressed, since we can't fully validate provenance)
         # since earlier TRAPI releases are minimally expected to record provenance attributes
+        # we only report this for TRAPI < 1.4 when Biolink Validation is done given that
+        # without Biolink validation, provenance cannot be reliably assessed
+
         if 'attributes' not in edge:
-            if not self.minimum_required_trapi_version("1.4.0-beta"):
+            if self.validate_biolink() and not self.minimum_required_trapi_version("1.4.0-beta"):
                 self.report(code="error.knowledge_graph.edge.attribute.missing", identifier=edge_id)
         elif not edge['attributes']:
-            if not self.minimum_required_trapi_version("1.4.0-beta"):
+            if self.validate_biolink() and not self.minimum_required_trapi_version("1.4.0-beta"):
                 self.report(code="error.knowledge_graph.edge.attribute.empty", identifier=edge_id)
         elif not isinstance(edge['attributes'], List):
             self.report(code="error.knowledge_graph.edge.attribute.not_array", identifier=edge_id)
         else:
             attributes = edge['attributes']
 
             ara_source: Optional[str]
@@ -435,15 +446,15 @@
                     )
                 elif 'value' not in attribute:
                     self.report(
                         code="error.knowledge_graph.edge.attribute.value.missing",
                         identifier=edge_id
                     )
                 elif not attribute['value'] or \
-                        str(attribute['value']).upper() in ["N/A","NONE","NULL"]:
+                        str(attribute['value']).upper() in ["N/A", "NONE", "NULL"]:
                     self.report(
                         code="error.knowledge_graph.edge.attribute.value.empty",
                         identifier=edge_id
                     )
                 else:
                     attribute_type_id: str = attribute['attribute_type_id']
                     value = attribute['value']
@@ -457,15 +468,15 @@
 
                     if not is_curie(attribute_type_id):
                         self.report(
                             code="error.knowledge_graph.edge.attribute.type_id.not_curie",
                             identifier=attribute_type_id,
                             edge_id=edge_id
                         )
-                    else:
+                    elif self.validate_biolink():
                         # 'attribute_type_id' is a CURIE, but how well does it map?
                         prefix = attribute_type_id.split(":", 1)[0]
                         if prefix == 'biolink':
                             biolink_class = self.validate_element_status(
                                 context="knowledge_graph.edge.attribute.type_id",
                                 identifier=attribute_type_id,
                                 edge_id=edge_id
@@ -539,18 +550,19 @@
                             self.report(
                                 code="info.knowledge_graph.edge.attribute.type_id.non_biolink_prefix",
                                 identifier=attribute_type_id,
                                 edge_id=edge_id
                             )
 
             # Edge provenance tags only recorded in Edge attributes prior to TRAPI 1.4.0-beta
-            if not self.minimum_required_trapi_version("1.4.0-beta"):
-
-                # TODO: After all the attributes have been scanned,
-                #       check for provenance. Treat as warnings for now.
+            if not self.minimum_required_trapi_version("1.4.0-beta") and self.validate_biolink():
+                # After all the attributes have been scanned,
+                # check for provenance. Treat as warnings for now.
+                # Note that provenance checking is only done when Biolink validation is done
+                # (since the various flags are not properly set above, for the test)
                 self.validate_provenance(
                     edge_id,
                     ara_source, found_ara_knowledge_source,
                     kp_source, found_kp_knowledge_source, kp_source_type,
                     found_primary_knowledge_source
                 )
 
@@ -638,15 +650,15 @@
         # but with missing 'qualifiers', no validation is attempted
         if 'qualifiers' not in edge or edge['qualifiers'] is None:
             return  # nullable: true... missing key or None value is ok?
         elif not isinstance(edge['qualifiers'], List):
             self.report(code="error.knowledge_graph.edge.qualifiers.not_array", identifier=edge_id)
         elif not edge['qualifiers']:
             return  # nullable: true... an empty 'qualifiers' array is ok?
-        else:
+        elif self.validate_biolink():
             qualifiers: List = edge['qualifiers']
             self.validate_qualifier_entry(
                 context="knowledge_graph.edge.qualifiers",
                 edge_id=edge_id,
                 qualifiers=qualifiers
             )
 
@@ -672,15 +684,15 @@
                 # and a dictionary, if qualifier_constraints is not empty
                 # Mandatory tag in every 'qualifier_constraint' entry
                 if not qualifier_set_entry['qualifier_set']:
                     self.report(
                         code="error.query_graph.edge.qualifier_constraints.qualifier_set.empty",
                         identifier=edge_id
                     )
-                else:
+                elif self.validate_biolink():
                     # We have a putative non-empty 'qualifier_set'
                     qualifier_set: List = qualifier_set_entry['qualifier_set']
                     self.validate_qualifier_entry(
                         context="query_graph.edge.qualifier_constraints.qualifier_set",
                         edge_id=edge_id,
                         qualifiers=qualifier_set
                     )
@@ -898,26 +910,28 @@
         if self.graph_type is TRAPIGraphType.Knowledge_Graph:
             if not predicate:
                 self.report(
                     code="error.knowledge_graph.edge.predicate.missing",
                     context=self.graph_type.value,
                     identifier=edge_id
                 )
-            else:
+            elif self.validate_biolink():
                 self.validate_predicate(edge_id=edge_id, predicate=predicate)
+
         else:  # is a Query Graph...
             if predicates is None:
                 # Query Graphs can have a missing or null predicates slot
                 pass
             elif not isinstance(predicates, List):
                 self.report(code="error.query_graph.edge.predicate.not_array", identifier=edge_id)
             elif len(predicates) == 0:
                 self.report(code="error.query_graph.edge.predicate.empty_array", identifier=edge_id)
-            else:
-                # Should now be a non-empty list of CURIES which are valid Biolink Predicates
+            elif self.validate_biolink():
+                # Should now be a non-empty list of CURIES
+                # which should validate as Biolink Predicates
                 for predicate in predicates:
                     if not predicate:
                         continue  # sanity check
                     self.validate_predicate(edge_id=edge_id, predicate=predicate)
 
         # Validate Object Node
         if not object_id:
@@ -1189,15 +1203,15 @@
         biolink_version=biolink_version,
         strict_validation=strict_validation
     )
     validator.check_biolink_model_compliance(graph)
     return validator
 
 
-def  check_biolink_model_compliance_of_knowledge_graph(
+def check_biolink_model_compliance_of_knowledge_graph(
     graph: Dict,
     trapi_version: Optional[str] = None,
     biolink_version: Optional[str] = None,
     sources: Optional[Dict] = None,
     strict_validation: Optional[bool] = None
 ) -> BiolinkValidator:
     """
```

### Comparing `reasoner_validator-3.5.4/reasoner_validator/codes.yaml` & `reasoner_validator-3.5.6/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.4/reasoner_validator/report.py` & `reasoner_validator-3.5.6/reasoner_validator/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,24 @@
     def get_biolink_version(self) -> str:
         """
         :return: Biolink Model version currently targeted by the ValidationReporter.
         :rtype biolink_version: str
         """
         return self.biolink_version
 
+    def validate_biolink(self) -> bool:
+        """
+        Predicate to check if the Biolink (version) is
+        tagged to 'suppress" compliance validation.
+
+        :return: returns 'True' if Biolink Validation is expected.
+        :rtype bool
+        """
+        return self.biolink_version is None or self.biolink_version.lower() != "suppress"
+
     def is_strict_validation(self) -> bool:
         """
         :return: bool, value of validation strictness set in the ValidationReporter.
         """
         return self.strict_validation
 
     def has_messages(self) -> bool:
```

### Comparing `reasoner_validator-3.5.4/reasoner_validator/sri/util.py` & `reasoner_validator-3.5.6/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.4/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.5.6/reasoner_validator/trapi/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """TRAPI Validation Functions."""
+from json import dumps
 from typing import Optional, Dict
 from os.path import isfile
 import copy
 from functools import lru_cache
 
 import jsonschema
 import requests
@@ -12,31 +13,34 @@
 from reasoner_validator.report import ValidationReporter
 from reasoner_validator.trapi.mapping import check_node_edge_mappings
 from reasoner_validator.versioning import (
     SemVer,
     SemVerError,
     get_latest_version,
     GIT_ORG,
-    GIT_REPO,
-    branches
+    GIT_REPO
 )
 
 import logging
 logger = logging.getLogger(__name__)
 
 
+# For testing, set TRAPI API query POST timeouts to 10 minutes == 600 seconds
+DEFAULT_TRAPI_POST_TIMEOUT = 600.0
+
+
 class TRAPIAccessError(RuntimeError):
     pass
 
 
 @lru_cache()
 def _load_schema(schema_version: str) -> Dict:
     """
     Load schema from GitHub version or directly from a local schema file.
-    :param schema_version: either a Github 'v' prefixed SemVer version of a
+    :param schema_version: either a GitHub 'v' prefixed SemVer version of a
            TRAPI schema or a file name (path) from which the TRAPI schema may be read in.
     :return: Dict, schema components
     """
     spec: Dict
     if schema_version.lower().endswith(".yaml"):
         # treat as a candidate TRAPI schema file path or name (the latter, assumed local)
         if not isfile(schema_version):
@@ -79,14 +83,59 @@
         err_msg: str = f"No TRAPI version {target}"
         logger.error(err_msg)
         raise ValueError(err_msg)
 
     return _load_schema(schema_version)
 
 
+def _output(json, flat=False):
+    return dumps(json, sort_keys=False, indent=None if flat else 4)
+
+
+async def call_trapi(url: str, trapi_message):
+    """
+    Given an url and a TRAPI message, post the message
+    to the url and return the status and json response.
+
+    :param url:
+    :param trapi_message:
+    :return:
+    """
+    query_url = f'{url}/query'
+
+    # print(f"\ncall_trapi({query_url}):\n\t{dumps(trapi_message, sort_keys=False, indent=4)}", file=stderr, flush=True)
+
+    try:
+        response = requests.post(query_url, json=trapi_message, timeout=DEFAULT_TRAPI_POST_TIMEOUT)
+    except requests.Timeout:
+        # fake response object
+        logger.error(
+            f"call_trapi(\n\turl: '{url}',\n\ttrapi_message: '{_output(trapi_message)}') - Request POST TimeOut?"
+        )
+        response = requests.Response()
+        response.status_code = 408
+    except requests.RequestException as re:
+        # perhaps another unexpected Request failure?
+        logger.error(
+            f"call_trapi(\n\turl: '{url}',\n\ttrapi_message: '{_output(trapi_message)}') - "
+            f"Request POST exception: {str(re)}"
+        )
+        response = requests.Response()
+        response.status_code = 408
+
+    response_json = None
+    if response.status_code == 200:
+        try:
+            response_json = response.json()
+        except Exception as exc:
+            logger.error(f"call_trapi({query_url}) JSON access error: {str(exc)}")
+
+    return {'status_code': response.status_code, 'response_json': response_json}
+
+
 def fix_nullable(schema) -> None:
     """Fix nullable schema."""
     if "oneOf" in schema:
         schema["oneOf"].append({"type": "null"})
         return
     if "anyOf" in schema:
         schema["anyOf"].append({"type": "null"})
@@ -208,15 +257,20 @@
                 component=component
             )
         except jsonschema.ValidationError as e:
             if len(e.message) <= 160:
                 reason = e.message
             else:
                 reason = e.message[0:49] + " "*5 + "... " + " "*5 + e.message[-100:-1]
-            self.report(code="error.trapi.validation", identifier=self.trapi_version, component=component, reason=reason)
+            self.report(
+                code="error.trapi.validation",
+                identifier=self.trapi_version,
+                component=component,
+                reason=reason
+            )
 
 
 def check_trapi_validity(instance, trapi_version: str, component: str = "Query") -> TRAPISchemaValidator:
     """
     Checks schema compliance of a Query component against a given TRAPI version.
 
     Parameters
```

### Comparing `reasoner_validator-3.5.4/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.5.6/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.4/reasoner_validator/validation_codes.py` & `reasoner_validator-3.5.6/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.4/reasoner_validator/versioning.py` & `reasoner_validator-3.5.6/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.4/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.5.6/tests/test_biolink_compliance_validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 
 # January 25, 2023 - as of reasoner-validator 3.1.0,
 # we don't pretend to totally support Biolink Models any earlier than 3.1.1.
 # If earlier biolink model compliance testing is desired,
 # then perhaps reasoner-validator version 3.0.5 or earlier can be used.
 LATEST_BIOLINK_MODEL_VERSION = "3.2.0"
 
+# special case of signalling suppression of validation
+SUPPRESS_BIOLINK_MODEL_VALIDATION = "suppress"
+
 
 def test_set_default_biolink_versioned_global_environment():
     validator = BiolinkValidator(graph_type=TRAPIGraphType.Knowledge_Graph)
     model_version = validator.get_biolink_version()
     print(
         f"\ntest_set_default_global_environment(): Biolink Model version is: '{str(model_version)}'",
         file=stderr, flush=True
@@ -845,14 +848,59 @@
                         "predicates": ["biolink:increases_amount_or_activity_of"],
                         "object": "IRS1"
                     }
                 }
             },
             # f"{QUERY_GRAPH_PREFIX}: INFO - Predicate element 'biolink:increases_amount_or_activity_of' is a mixin."
             "info.query_graph.edge.predicate.mixin"
+        ),
+        (
+            SUPPRESS_BIOLINK_MODEL_VALIDATION,
+            # Query 24: ... but if present, predicates must be valid
+            #           for the specified Biolink Model version, but...
+            {
+                "nodes": {
+                    "type-2 diabetes": {"ids": ["MONDO:0005148"]},
+                    "drug": {
+                        "categories": ["biolink:Drug"]
+                    }
+                },
+                "edges": {
+                    "treats": {
+                        "subject": "drug",
+                        "predicates": ["biolink:has_unit"],
+                        "object": "type-2 diabetes"
+                    }
+                }
+            },
+            # ...since Biolink Model validation is tagged as 'suppress',
+            # we  don't expect any validation output here?
+            ""
+        ),
+        (
+            SUPPRESS_BIOLINK_MODEL_VALIDATION,
+            # Query 25: Query edge predicate is a mixin...but...
+            {
+                "nodes": {
+                    "IRS1": {"ids": ["HGNC:6125"], "categories": ["biolink:Gene"]},
+                    "drug": {
+                        "categories": ["biolink:Drug"]
+                    }
+                },
+                "edges": {
+                    "treats": {
+                        "subject": "drug",
+                        "predicates": ["biolink:increases_amount_or_activity_of"],
+                        "object": "IRS1"
+                    }
+                }
+            },
+            # ...since Biolink Model validation is tagged as 'suppress',
+            # we  don't expect any validation output here?
+            ""
         )
     ]
 )
 def test_check_biolink_model_compliance_of_query_graph(query: Tuple):
     validator: BiolinkValidator = \
         check_biolink_model_compliance_of_query_graph(graph=query[1], biolink_version=query[0])
     check_messages(validator, query[2])
@@ -1227,15 +1275,16 @@
     check_messages(validator, query[2])
 
 
 def qualifier_validator(
         tested_method,
         edge_model: str,
         query: Tuple[Dict, str],
-        trapi_version: Optional[str] = None
+        trapi_version: Optional[str] = None,
+        biolink_version: Optional[str] = LATEST_BIOLINK_MODEL_VERSION
 ):
     # TODO: to review: which of the validation tests that may be overridden by earlier TRAPI validation
     # Sanity check: does TRAPI validation catch this first?
     trapi_validator = TRAPISchemaValidator(trapi_version=trapi_version)
     # Wrap Qualifiers inside a small mock QEdge
     mock_edge: Dict = deepcopy(query[0])
     mock_edge["subject"] = "mock_subject"
@@ -1257,15 +1306,15 @@
     if trapi_validator.has_errors():
         validator = trapi_validator
     else:
         # if you get this far,then attempt additional Biolink Validation
         validator = BiolinkValidator(
             graph_type=TRAPIGraphType.Query_Graph,
             trapi_version=trapi_version,
-            biolink_version=LATEST_BIOLINK_MODEL_VERSION
+            biolink_version=biolink_version
         )
         tested_method(
             validator,
             edge_id=f"{tested_method.__name__} unit test",
             edge=query[0]
         )
     check_messages(validator, query[1])
@@ -1508,14 +1557,64 @@
     qualifier_validator(
         tested_method=BiolinkValidator.validate_qualifier_constraints,
         edge_model="QEdge",
         query=query
     )
 
 
+@pytest.mark.parametrize(
+    "query",
+    [
+        (   # Query 0 - 'qualifier_type_id' is the special qualifier case 'biolink:qualified_predicate'
+            #            an incorrect value, which is not a Biolink predicate,  but...
+            {
+                'qualifier_constraints': [
+                    {
+                        "qualifier_set": [
+                            {
+                                'qualifier_type_id': "biolink:qualified_predicate",
+                                'qualifier_value': "biolink:Association"
+                            }
+                        ]
+                    }
+                ]
+            },
+            # ...since Biolink Model validation is tagged as 'suppress',
+            #    then we don't expect any validation output here?
+            ""
+        ),
+        (  # Query 14 - 'qualifier_type_id' property value is not a Biolink qualifier term, but...
+            {
+                'qualifier_constraints': [
+                    {
+                        "qualifier_set": [
+                            {
+                                'qualifier_type_id': "biolink:related_to",
+                                'qualifier_value': "fake-qualifier-value"
+                            }
+                        ]
+                    }
+                ]
+            },
+            # ...since Biolink Model validation is tagged as 'suppress',
+            #    then we don't expect any validation output here?
+            ""
+        )
+    ]
+)
+def test_biolink_validation_suppressed_validate_qualifier_constraints(query: Tuple[Dict, str]):
+    qualifier_validator(
+        tested_method=BiolinkValidator.validate_qualifier_constraints,
+        edge_model="QEdge",
+        query=query,
+        biolink_version="suppress"
+    )
+
+
+
 QC_QS_NOT_A_CURIE = {
     'qualifier_constraints': [
         {
             "qualifier_set": [
                 {
                     'qualifier_type_id': "not-a-curie",
                     'qualifier_value': "fake-qualifier-value"
@@ -2603,14 +2702,86 @@
                        "subject": "NCBIGene:29974",
                        "predicate": "biolink:physically_interacts_with",
                        "object": "PUBCHEM.COMPOUND:597",
                     }
                 }
             },
             "error.knowledge_graph.node.category.unknown"
+        ),
+        (   # Query 27:  #'attribute_type_id' has a CURIE prefix namespace unknown to Biolink but...
+            SUPPRESS_BIOLINK_MODEL_VALIDATION,
+            {
+                "nodes": {
+                    "NCBIGene:29974": {
+                       "categories": [
+                           "biolink:Gene"
+                       ]
+                    },
+                    "PUBCHEM.COMPOUND:597": {
+                        "name": "cytosine",
+                        "categories": [
+                            "biolink:SmallMolecule"
+                        ],
+                    }
+                },
+                "edges": {
+                    "edge_1": {
+                        "subject": "NCBIGene:29974",
+                        "predicate": "biolink:physically_interacts_with",
+                        "object": "PUBCHEM.COMPOUND:597",
+                        "attributes": [{"attribute_type_id": "foo:bar", "value": "some value"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
+                    }
+                }
+            },
+            # ...since Biolink Model validation is tagged as 'suppress',
+            # we  don't expect any validation output here?
+            ""
+        ),
+        (
+            SUPPRESS_BIOLINK_MODEL_VALIDATION,
+            # Query 28: 'attribute_type_id' is not a 'biolink:association_slot'
+            #           (biolink:synonym is a node property) but...
+            {
+                "nodes": {
+                    "NCBIGene:29974": {
+                       "categories": [
+                           "biolink:Gene"
+                       ]
+                    },
+                    "PUBCHEM.COMPOUND:597": {
+                        "name": "cytosine",
+                        "categories": [
+                            "biolink:SmallMolecule"
+                        ],
+                    }
+                },
+                "edges": {
+                    "edge_1": {
+                        "subject": "NCBIGene:29974",
+                        "predicate": "biolink:physically_interacts_with",
+                        "object": "PUBCHEM.COMPOUND:597",
+                        "attributes": [{"attribute_type_id": "biolink:synonym", "value": "some synonym"}],
+                        "sources": [
+                            {
+                                "resource_id": "infores:molepro",
+                                "resource_role": "primary_knowledge_source"
+                            }
+                        ]
+                    }
+                }
+            },
+            # ...since Biolink Model validation is tagged as 'suppress',
+            # we  don't expect any validation output here?
+            ""
         )
     ]
 )
 def test_check_biolink_model_compliance_of_knowledge_graph(query: Tuple):
     validator: BiolinkValidator = check_biolink_model_compliance_of_knowledge_graph(
         graph=query[1], biolink_version=query[0]
     )
@@ -2649,14 +2820,25 @@
         graph=edge_without_attributes,
         trapi_version="1.3.0",
         biolink_version=LATEST_BIOLINK_MODEL_VERSION
     )
     check_messages(validator, "error.knowledge_graph.edge.attribute.missing")
 
 
+def test_suppress_biolink_validation_pre_trapi_1_4_0_validate_attributes():
+    # message edges must have at least some 'provenance' attributes
+    edge_without_attributes = deepcopy(MESSAGE_EDGE_WITHOUT_ATTRIBUTES)
+    validator: BiolinkValidator = check_biolink_model_compliance_of_knowledge_graph(
+        graph=edge_without_attributes,
+        trapi_version="1.3.0",
+        biolink_version=SUPPRESS_BIOLINK_MODEL_VALIDATION
+    )
+    check_messages(validator, "")
+
+
 SAMPLE_RETRIEVAL_SOURCE = {
     # required, infores CURIE to an Information Resource
     "resource_id": "infores:molepro",
 
     # required, string drawn from the TRAPI ResourceRoleEnum
     # values that were formerly recorded as TRAPI attributes
     # are now presented as first class edge annotation
```

### Comparing `reasoner_validator-3.5.4/tests/test_data/sample_trapi_schema.yaml` & `reasoner_validator-3.5.6/tests/test_data/sample_trapi_schema.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.4/tests/test_response_validator.py` & `reasoner_validator-3.5.6/tests/test_response_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Unit tests for the generic (shared) components of the SRI Testing Framework
 """
-from typing import Tuple,  Dict, Union
+from typing import Tuple,  Dict
 import logging
 import pytest
 
 from reasoner_validator import TRAPIResponseValidator
 from tests.test_validation_report import check_messages
 
 logger = logging.getLogger(__name__)
```

### Comparing `reasoner_validator-3.5.4/tests/test_semver.py` & `reasoner_validator-3.5.6/tests/test_semver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Test semantic version handling."""
 import pytest
 
-from reasoner_validator.versioning import semver_pattern, SemVer, SemVerError, SemVerUnderspecified
+from reasoner_validator.versioning import semver_pattern, SemVer, SemVerUnderspecified
 
 
 def test_regex_pattern():
     # test the semver pattern directly
     assert semver_pattern.fullmatch("1.2.3")
     assert semver_pattern.fullmatch("1.2")
     assert semver_pattern.fullmatch("1")
```

### Comparing `reasoner_validator-3.5.4/tests/test_trapi_versioning.py` & `reasoner_validator-3.5.6/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.4/tests/test_validate.py` & `reasoner_validator-3.5.6/tests/test_validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from copy import deepcopy
 
 import pytest
 
 from jsonschema.exceptions import ValidationError
 
 from reasoner_validator.trapi import TRAPISchemaValidator, openapi_to_jsonschema, load_schema
-from pprint import pprint
+
 PRE_1_4_0_TEST_VERSIONS = "1.2", "1.2.0", "1.3", "1.3.0"
 LATEST_TEST_VERSIONS = "1", "1.4", "1.4.0", "1.4.0-beta4"
 ALL_TEST_VERSIONS = PRE_1_4_0_TEST_VERSIONS + LATEST_TEST_VERSIONS
 
 
 @pytest.mark.parametrize(
     "query",
@@ -513,15 +513,15 @@
 
 @pytest.mark.parametrize("trapi_version", ALL_TEST_VERSIONS)
 def test_message_node_binding_component_validation(trapi_version):
     """Test NodeBinding component in TRAPIValidator(trapi_version=query).validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     sample_node_binding = {
         "id": "SGD:S000000065",
-        # 'qnode_id' is not formally specified in spec but it is an
+        # 'qnode_id' is not formally specified in spec, but it is an
         # example of an additionalProperties: true permitted field
         "qnode_id": "SGD:S000000065",
         "query_id": None
     }
 
     validator.validate(sample_node_binding, "NodeBinding")
     with pytest.raises(ValidationError):
```

### Comparing `reasoner_validator-3.5.4/tests/test_validation_report.py` & `reasoner_validator-3.5.6/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.4/tests/test_workflows.py` & `reasoner_validator-3.5.6/tests/test_workflows.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This test file overlaps a bit with test_validate.py but intentionally isolates
 basic TRAPI Query 'workflow' testing to help troubleshoot the validation.
 """
 import pytest
-from typing import Tuple, Dict
+from typing import Dict
 from itertools import product
 from json import dumps
 
 from reasoner_validator.trapi import TRAPISchemaValidator
 
 LATEST_TEST_VERSIONS = "1", "1.4", "1.4.0", "1.4.0-beta4"
```

### Comparing `reasoner_validator-3.5.4/PKG-INFO` & `reasoner_validator-3.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.5.4
+Version: 3.5.6
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -88,26 +88,31 @@
 
 To develop this package, install with all extras dependencies using:
 
 ```bash
 poetry install --all-extras
 ```
 
-## Running Validation against an ARS UUID Result(*)
+## Running Validation against an ARS UUID Result(*) or using a Local TRAPI Request Query
 
-A local script **`ars_uuid_result_test_runner.py`** is available to run TRAPI Response validation against a 
-UUID indexed query result of the Biomedical Knowledge Translator "Autonomous Relay System" (ARS).
+A local script **`trapi_validator.py`** is available to run TRAPI Response validation against either a PK (UUID)
+indexed query result of the Biomedical Knowledge Translator "Autonomous Relay System" (ARS), a local JSON Response
+text file or a locally triggered _ad hoc_ query Request against an directly specified TRAPI endpoint.
 
-For usage, type:
+Note that it is best run within a **`poetry shell`** created by **`poetry install`**.
+
+For script usage, type:
 
 ```bash
-./ars_uuid_result_test_runner.py --help
+./trapi_validator.py --help
 ```
 
-(*) Thank you Eric Deutsch for the prototype of this script
+The script allows
+
+(*) Thank you Eric Deutsch for the prototype code for this script
 
 ## Running tests
 
 To run the test locally install with the `dev` dependencies group if not already done:
 
 ```bash
 poetry install --extras dev
```

