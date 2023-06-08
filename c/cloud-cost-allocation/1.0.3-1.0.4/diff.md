# Comparing `tmp/cloud-cost-allocation-1.0.3.tar.gz` & `tmp/cloud-cost-allocation-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-cost-allocation-1.0.3.tar", last modified: Tue Apr 11 07:31:03 2023, max compression
+gzip compressed data, was "cloud-cost-allocation-1.0.4.tar", last modified: Thu Jun  8 12:21:20 2023, max compression
```

## Comparing `cloud-cost-allocation-1.0.3.tar` & `cloud-cost-allocation-1.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/cloud_cost_allocation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23784 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/cloud_cost_allocator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    40095 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/cost_items.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/base_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/csv_allocated_cost_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/cloud_cost_allocation/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/cloud_cost_allocation/writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/writer/base_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/writer/csv_allocated_cost_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/cloud_cost_allocation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-04-11 07:31:02.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-11 07:31:03.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:31:02.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 07:31:02.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/puml/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/puml/cost-allocation-model.puml
--rw-r--r--   0 runner    (1001) docker     (123)    23813 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/puml/cost-allocation-model.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/puml/hierarchical-service-consumption-example.puml
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/puml/hierarchical-service-consumption-example.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/puml/hierarchical-service-cost-allocation-example.puml
--rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/puml/hierarchical-service-cost-allocation-example.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-11 07:31:03.013227 cloud-cost-allocation-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.985045 cloud-cost-allocation-1.0.4/cloud_cost_allocation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23784 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/cloud_cost_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41310 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/cost_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/base_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/csv_allocated_cost_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/cloud_cost_allocation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/cloud_cost_allocation/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/writer/base_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation/writer/csv_allocated_cost_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/cloud_cost_allocation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-08 12:21:20.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-08 12:21:20.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:21:20.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 12:21:20.000000 cloud-cost-allocation-1.0.4/cloud_cost_allocation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/puml/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/puml/cost-allocation-model.puml
+-rw-r--r--   0 runner    (1001) docker     (123)    23813 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/puml/cost-allocation-model.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/puml/hierarchical-service-consumption-example.puml
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/puml/hierarchical-service-consumption-example.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/puml/hierarchical-service-cost-allocation-example.puml
+-rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/puml/hierarchical-service-cost-allocation-example.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:21:20.989045 cloud-cost-allocation-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-08 12:21:09.000000 cloud-cost-allocation-1.0.4/tests/test.py
```

### Comparing `cloud-cost-allocation-1.0.3/LICENSE` & `cloud-cost-allocation-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/PKG-INFO` & `cloud-cost-allocation-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-cost-allocation
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python library for shared, hierarchical cost allocation based on user-defined usage metrics.
 Home-page: https://github.com/AmadeusITGroup/cloud-cost-allocation
 Author: Marc Perreaut
 Author-email: marc.perreaut@amadeus.com
 Maintainer: Amadeus IT Group
 Maintainer-email: opensource@amadeus.com
 License: MIT license
```

### Comparing `cloud-cost-allocation-1.0.3/README.md` & `cloud-cost-allocation-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/cloud_cost_allocation/cloud_cost_allocator.py` & `cloud-cost-allocation-1.0.4/cloud_cost_allocation/cloud_cost_allocator.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/cloud_cost_allocation/config.py` & `cloud-cost-allocation-1.0.4/cloud_cost_allocation/config.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/cloud_cost_allocation/cost_items.py` & `cloud-cost-allocation-1.0.4/cloud_cost_allocation/cost_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -560,14 +560,20 @@
                 amounts_by_product_info.nb_keys[index] += 1
                 index += 1
 
         # Reset the number of matching provider tag selectors of every item
         for item in self.cost_items:
             item.nb_matching_provider_tag_selectors = 0
 
+        # Build evaluation error dict, used to avoid error streaming in case of incorrect provider tag
+        # selector expression
+        # Key = date, provider service, provider instance, provider tag selector, expression
+        # Value = count of errors
+        evaluation_error_dict = {}
+
         # Compute raw costs of non-default provider tag selectors, by checking matching items
         total_provider_tag_selector_raw_amounts = [0.0] * nb_amounts
         total_provider_tag_selector_raw_product_amounts = [0.0] * nb_amounts
         for provider_tag_selector_amount in self.provider_tag_selector_amounts.values():
             if not provider_tag_selector_amount.is_default():
                 for cost_item in self.cost_items:
                     if not cost_item.is_self_consumption():
@@ -580,30 +586,46 @@
                         try:
                             # Eval is dangerous. Considerations:
                             # - Audit cost allocation keys, which are provided by DevOps
                             # - Possibly forbid provider tag selectors
                             eval_true = eval(provider_tag_selector_amount.selector, eval_globals_dict, {})
                         except:
                             exception = sys.exc_info()[0]
-                            error("Caught exception '" + str(exception) +
-                                  "' while evaluating provider tag selector '" +
-                                  provider_tag_selector_amount.selector +
-                                  "' for provider service '" +
-                                  self.service +
-                                  "'")
+                            error_key =\
+                                cost_item.date_str + chr(10) + self.service + chr(10) + self.instance + chr(10) +\
+                                provider_tag_selector_amount.selector + chr(10) + str(exception)
+                            if error_key in evaluation_error_dict:
+                                error_count = evaluation_error_dict[error_key]
+                            else:
+                                error_count = 0
+                            evaluation_error_dict[error_key] = error_count + 1
 
                         # If item matches provider tag selector, update raw amounts of the provider tag selector
                         if eval_true:
                             cost_item.nb_matching_provider_tag_selectors += 1
                             provider_tag_selector_amount\
                                 .update_raw_amounts(cost_item,
                                                     total_provider_tag_selector_raw_amounts,
                                                     total_provider_tag_selector_raw_product_amounts,
                                                     amount_to_allocation_key_indexes)
 
+        # Log evaluation errors
+        for error_key, error_count in evaluation_error_dict.items():
+            error_fields = error_key.split(chr(10))
+            date_str = error_fields[0]
+            provider_service = error_fields[1]
+            provider_instance = error_fields[2]
+            provider_tag_selector = error_fields[3]
+            exception = error_fields[4]
+            error("Caught exception '" + exception + "' " + str(error_count) + " times " +
+                  "when evaluating ProviderTagSelector '" + provider_tag_selector +
+                  "' of ProviderService '" + provider_service +
+                  "' and of ProviderInstance '" + provider_instance + "'" +
+                  ", for date " + date_str)
+
         # Compute the raw amounts of the default provider tag selector
         if '' in self.provider_tag_selector_amounts:
             default_provider_tag_selector = self.provider_tag_selector_amounts['']
             for cost_item in self.cost_items:
                 if cost_item.nb_matching_provider_tag_selectors == 0 and not cost_item.is_self_consumption():
                     cost_item.nb_matching_provider_tag_selectors = 1
                     default_provider_tag_selector.update_raw_amounts(cost_item,
```

### Comparing `cloud-cost-allocation-1.0.3/cloud_cost_allocation/main.py` & `cloud-cost-allocation-1.0.4/cloud_cost_allocation/main.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py` & `cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/base_reader.py` & `cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/base_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/csv_allocated_cost_reader.py` & `cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/csv_allocated_cost_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py` & `cloud-cost-allocation-1.0.4/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/cloud_cost_allocation/utils/utils.py` & `cloud-cost-allocation-1.0.4/cloud_cost_allocation/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/cloud_cost_allocation/writer/base_writer.py` & `cloud-cost-allocation-1.0.4/cloud_cost_allocation/writer/base_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 class GenericWriter(ABC):
     '''
     classdocs
     '''
 
     __slots__ = (
         'config',               # type: Config
-        'service_instances',    # type: ServiceInstance
+        'service_instances',    # type: dict[ServiceInstance]
         'exporters',            # type: dict[type -> method]
     )
 
-    def __init__(self, service_instances: list[ServiceInstance], config: Config):
+    def __init__(self, service_instances: dict[ServiceInstance], config: Config):
         '''
         Constructor
         '''
         self.service_instances = service_instances
         self.config = config
         self.exporters = {}
         self.exporters[CostItem] = self.export_item_base
```

### Comparing `cloud-cost-allocation-1.0.3/cloud_cost_allocation/writer/csv_allocated_cost_writer.py` & `cloud-cost-allocation-1.0.4/cloud_cost_allocation/writer/csv_allocated_cost_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class CSV_AllocatedCostWriter(GenericWriter):
     '''
     classdocs
     '''
 
-    def __init__(self, service_instances: list[ServiceInstance], config: Config):
+    def __init__(self, service_instances: dict[ServiceInstance], config: Config):
         super().__init__(service_instances, config)
 
     def get_headers(self) -> list[str]:
 
         # Column order is historical
 
         # Initialize
```

### Comparing `cloud-cost-allocation-1.0.3/cloud_cost_allocation.egg-info/PKG-INFO` & `cloud-cost-allocation-1.0.4/cloud_cost_allocation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-cost-allocation
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python library for shared, hierarchical cost allocation based on user-defined usage metrics.
 Home-page: https://github.com/AmadeusITGroup/cloud-cost-allocation
 Author: Marc Perreaut
 Author-email: marc.perreaut@amadeus.com
 Maintainer: Amadeus IT Group
 Maintainer-email: opensource@amadeus.com
 License: MIT license
```

### Comparing `cloud-cost-allocation-1.0.3/cloud_cost_allocation.egg-info/SOURCES.txt` & `cloud-cost-allocation-1.0.4/cloud_cost_allocation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/puml/cost-allocation-model.puml` & `cloud-cost-allocation-1.0.4/puml/cost-allocation-model.puml`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/puml/cost-allocation-model.svg` & `cloud-cost-allocation-1.0.4/puml/cost-allocation-model.svg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/puml/hierarchical-service-consumption-example.puml` & `cloud-cost-allocation-1.0.4/puml/hierarchical-service-consumption-example.puml`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/puml/hierarchical-service-consumption-example.svg` & `cloud-cost-allocation-1.0.4/puml/hierarchical-service-consumption-example.svg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/puml/hierarchical-service-cost-allocation-example.puml` & `cloud-cost-allocation-1.0.4/puml/hierarchical-service-cost-allocation-example.puml`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/puml/hierarchical-service-cost-allocation-example.svg` & `cloud-cost-allocation-1.0.4/puml/hierarchical-service-cost-allocation-example.svg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/setup.cfg` & `cloud-cost-allocation-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.3/setup.py` & `cloud-cost-allocation-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Import readme
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme_file:
     readme = readme_file.read()
 
 # Setup
 setup(
     name='cloud-cost-allocation',
-    version='1.0.3',
+    version='1.0.4',
     description='Python library for shared, hierarchical cost allocation based on user-defined usage metrics.',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=['cloud_cost_allocation',
               'cloud_cost_allocation.reader',
               'cloud_cost_allocation.utils',
               'cloud_cost_allocation.writer'],
```

### Comparing `cloud-cost-allocation-1.0.3/tests/test.py` & `cloud-cost-allocation-1.0.4/tests/test.py`

 * *Files identical despite different names*

