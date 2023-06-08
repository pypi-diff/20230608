# Comparing `tmp/phc-ingestion-0.3.35.tar.gz` & `tmp/phc-ingestion-0.3.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.35.tar", last modified: Wed Jun  7 14:39:07 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.36.tar", last modified: Thu Jun  8 10:22:06 2023, max compression
```

## Comparing `phc-ingestion-0.3.35.tar` & `phc-ingestion-0.3.36.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       16 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/PYPI.md
--rw-r--r--   0        0        0        0 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1603 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4738 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1325 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      555 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4636 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21500 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4948 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     5010 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3127 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8876 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     3187 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0       46 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     2976 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2284 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     7368 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     3785 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     5664 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     1913 2023-06-07 14:38:43.223614 phc-ingestion-0.3.35/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2023-06-07 14:38:43.227614 phc-ingestion-0.3.35/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2023-06-07 14:38:43.227614 phc-ingestion-0.3.35/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2023-06-07 14:38:43.227614 phc-ingestion-0.3.35/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2023-06-07 14:38:43.227614 phc-ingestion-0.3.35/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2023-06-07 14:38:43.227614 phc-ingestion-0.3.35/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0     1029 2023-06-07 14:38:43.227614 phc-ingestion-0.3.35/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.35/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/PYPI.md
+-rw-r--r--   0        0        0        0 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1603 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4738 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1325 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      555 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4636 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21500 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4948 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     5010 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-06-08 10:21:40.889545 phc-ingestion-0.3.36/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3127 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8876 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     3187 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     2976 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2284 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     8461 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     3785 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     5664 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     1913 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0     1029 2023-06-08 10:21:40.893542 phc-ingestion-0.3.36/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.36/PKG-INFO
```

### Comparing `phc-ingestion-0.3.35/ingestion/caris/process.py` & `phc-ingestion-0.3.36/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.36/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.3.36/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.36/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.36/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/caris/util/json.py` & `phc-ingestion-0.3.36/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.36/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.36/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.36/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.36/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/foundation/process.py` & `phc-ingestion-0.3.36/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.36/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.36/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.36/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.36/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/nextgen/process.py` & `phc-ingestion-0.3.36/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.3.36/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.3.36/ingestion/nextgen/util/process_manifest.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,14 +29,42 @@
             break
         if in_range_trigger == True:
             patient_info_lines.append(line.strip())
 
     return patient_info_lines
 
 
+def extract_interpretation_text(xml_in_file: str):
+    with open(xml_in_file, "r") as f:
+        xml_lines = f.readlines()
+
+    in_range_trigger = False
+    interpretation_lines = []
+    for line in xml_lines:
+        if "INTERPRETATION" in line:
+            in_range_trigger = True
+        if "References" in line:
+            in_range_trigger = False
+            break
+        if in_range_trigger == True:
+            interpretation_lines.append(line.strip())
+
+    return interpretation_lines
+
+
+def get_cell_purity(interpretation_lines: list):
+    cell_purity_value = None
+    for line in interpretation_lines:
+        if "CD138+" in line:
+            cell_purity_value = float(re.search(r"\d\d\.\d\d\%", line).group(0)[:-2])
+            return cell_purity_value
+    if not cell_purity_value:
+        return float(00.00)
+
+
 def extract_patient_data(patient_info_lines: list):
     patient_data = {}
     patient_data["patientInfo"] = {}
 
     for line in patient_info_lines:
         if "patientLastName" not in patient_data and "Patient Name" in line:
             patientNameArray = line.split(" ")
@@ -74,18 +102,18 @@
             else:
                 gender = "other"
             patient_data["patientInfo"]["gender"] = gender
 
     return patient_data
 
 
-def extract_test_data(patient_info_lines: dict):
+def extract_test_data(patient_info_lines: list, interpretation_lines: list):
     # Initialize manifest and hard-code some values
     manifest = {}
-    manifest["testType"] = "NextGen"
+    manifest["testType"] = "Plasma Cell Myeloma Panel"
     manifest["name"] = "IU Diagnostic Genomics"
     manifest["reference"] = "GRCh38"
 
     manifest["ihcTests"] = []
     manifest["tumorTypePredictions"] = []
     manifest["orderingMDNPI"] = ""
 
@@ -134,27 +162,32 @@
         if "bodySite" not in manifest and "Specimen:" in line:
             bodySiteArray = line.split(" ")
             body_site_one = search_and_grab(bodySiteArray, "Specimen:", 1)
             body_site_two = search_and_grab(bodySiteArray, "Specimen:", 2)
             manifest["bodySite"] = f"{body_site_one} {body_site_two}"
             manifest["bodySiteDisplay"] = f"{body_site_one} {body_site_two}"
 
+    cell_purtiy = get_cell_purity(interpretation_lines)
+    if cell_purtiy != 00.00:
+        manifest["cellPurity"] = cell_purtiy
+
     return manifest
 
 
 def process_manifest(
     xml_in_file: str,
     source_file_id: str,
     prefix: str,
     structural_status: bool,
     log: Logger,
 ):
-    xml_text = extract_xml_text(xml_in_file)
-    manifest = extract_test_data(xml_text)
-    manifest.update(extract_patient_data(xml_text))
+    test_text = extract_xml_text(xml_in_file)
+    interpretation_text = extract_interpretation_text(xml_in_file)
+    manifest = extract_test_data(test_text, interpretation_text)
+    manifest.update(extract_patient_data(test_text))
 
     manifest["reportFile"] = f".lifeomic/nextgen/{prefix}/{prefix}.pdf"
     manifest["sourceFileId"] = source_file_id
     manifest["resources"] = [
         {"fileName": f".lifeomic/nextgen/{prefix}/{prefix}.pdf"},
     ]
```

### Comparing `phc-ingestion-0.3.35/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.3.36/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.3.36/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.3.36/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.3.36/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.3.36/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.3.36/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.3.36/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.35/pyproject.toml` & `phc-ingestion-0.3.36/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.35"
+version = "0.3.36"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

