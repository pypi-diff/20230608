# Comparing `tmp/cryoet_data_portal-0.0.2.tar.gz` & `tmp/cryoet_data_portal-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryoet_data_portal-0.0.2.tar", last modified: Wed Jun  7 19:38:09 2023, max compression
+gzip compressed data, was "cryoet_data_portal-1.0.0.tar", last modified: Thu Jun  8 06:41:40 2023, max compression
```

## Comparing `cryoet_data_portal-0.0.2.tar` & `cryoet_data_portal-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:38:09.616719 cryoet_data_portal-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-07 19:38:09.616719 cryoet_data_portal-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:38:09.612719 cryoet_data_portal-0.0.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:38:09.616719 cryoet_data_portal-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:38:09.612719 cryoet_data_portal-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:38:09.612719 cryoet_data_portal-0.0.2/src/cryoet_data_portal/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal/_file_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal/_gql_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26971 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal/_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:38:09.612719 cryoet_data_portal-0.0.2/src/cryoet_data_portal/data/
--rw-r--r--   0 runner    (1001) docker     (123)   174865 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal/data/schema.graphql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:38:09.612719 cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-07 19:38:09.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-07 19:38:09.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:38:09.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-07 19:38:09.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 19:38:09.000000 cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:38:09.616719 cryoet_data_portal-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-07 19:37:57.000000 cryoet_data_portal-0.0.2/tests/test_get_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:40.410415 cryoet_data_portal-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-08 06:41:40.410415 cryoet_data_portal-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:40.406415 cryoet_data_portal-1.0.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 06:41:40.410415 cryoet_data_portal-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:40.406415 cryoet_data_portal-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:40.406415 cryoet_data_portal-1.0.0/src/cryoet_data_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal/_file_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal/_gql_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28822 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal/_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:40.410415 cryoet_data_portal-1.0.0/src/cryoet_data_portal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   171477 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal/data/schema.graphql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:40.410415 cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-08 06:41:40.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-08 06:41:40.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 06:41:40.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 06:41:40.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 06:41:40.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:40.410415 cryoet_data_portal-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/tests/test_get_client.py
```

### Comparing `cryoet_data_portal-0.0.2/LICENSE` & `cryoet_data_portal-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-0.0.2/PKG-INFO` & `cryoet_data_portal-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryoet_data_portal
-Version: 0.0.2
+Version: 1.0.0
 Summary: API Client to facilitate the use of the CryoET Portal. For more information about the API and the project visit https://github.com/chanzuckerberg/cryoet-data-portal/
 Author-email: Chan Zuckerberg Initiative <cryoetdataportal@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cryoet-data-portal
 Project-URL: repository, https://github.com/chanzuckerberg/cryoet-data-portal
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cryoet_data_portal-0.0.2/README.md` & `cryoet_data_portal-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-0.0.2/pyproject.toml` & `cryoet_data_portal-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-0.0.2/src/cryoet_data_portal/__init__.py` & `cryoet_data_portal-1.0.0/src/cryoet_data_portal/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 try:
     from importlib import metadata
 except ImportError:
     # for python <=3.7
     import importlib_metadata as metadata  # type: ignore[no-redef]
 
 from ._client import Client
-from ._models import Annotation, AnnotationAuthor, Dataset, DatasetAuthor, DatasetFunding, Run, TiltSeries, Tomogram
+from ._models import Annotation, AnnotationAuthor, Dataset, DatasetAuthor, DatasetFunding, Run, TiltSeries, Tomogram, TomogramVoxelSpacing
 
 try:
     __version__ = metadata.version("cryoet_data_portal")
 except metadata.PackageNotFoundError:
     # package is not installed
     __version__ = "0.0.0-unknown"
 
@@ -25,8 +25,9 @@
     "AnnotationAuthor",
     "Dataset",
     "DatasetAuthor",
     "DatasetFunding",
     "Run",
     "TiltSeries",
     "Tomogram",
+    "TomogramVoxelSpacing",
 ]
```

### Comparing `cryoet_data_portal-0.0.2/src/cryoet_data_portal/_client.py` & `cryoet_data_portal-1.0.0/src/cryoet_data_portal/_client.py`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-0.0.2/src/cryoet_data_portal/_file_tools.py` & `cryoet_data_portal-1.0.0/src/cryoet_data_portal/_file_tools.py`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-0.0.2/src/cryoet_data_portal/_gql_base.py` & `cryoet_data_portal-1.0.0/src/cryoet_data_portal/_gql_base.py`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-0.0.2/src/cryoet_data_portal/_models.py` & `cryoet_data_portal-1.0.0/src/cryoet_data_portal/_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,25 @@
 import os
 from datetime import date
 from typing import Iterable, Optional
 
 from ._file_tools import download_directory, download_https
-from ._gql_base import (
-    BooleanField,
-    DateField,
-    FloatField,
-    IntField,
-    ItemRelationship,
-    ListRelationship,
-    Model,
-    StringField,
-)
+from ._gql_base import (BooleanField, DateField, FloatField, IntField,
+                        ItemRelationship, ListRelationship, Model, StringField)
 
 
 class Dataset(Model):
     """Metadata for a dataset in the CryoET Data Portal
 
     Attributes:
         id (int): An identifier for a CryoET dataset, assigned by the Data Portal. Used to identify the dataset as the directory name in data tree
         authors (List[DatasetAuthor]): An array relationship with DatasetAuthor
-        cell_line_name (str): Cell line or strain for the sample.
-        cell_line_source (str): Name of the company from which the sample is sourced from.
         cell_name (str): Name of the cell from which a biological sample used in a CryoET study is derived from.
+        cell_strain_id (str): Link to more information about the cell strain
+        cell_strain_name (str): Cell line or strain for the sample.
         cell_type_id (str): Cell Ontology identifier for the cell type
         dataset_citations (str): DOIs for publications that cite the dataset. Use a comma to separate multiple DOIs.
         dataset_publications (str): DOIs for publications that describe the dataset. Use a comma to separate multiple DOIs.
         deposition_date: date! Date when a dataset is initially received by the Data Portal.
         description (str): A short description of a CryoET dataset, similar to an abstract for a journal article or dataset.
         funding_sources: List[FundingSource] An array relationship with FundingSource
         grid_preparation (str): Describe Cryo-ET grid preparation.
@@ -42,15 +34,14 @@
         runs: List[Run] An array relationship with Run
         s3_prefix (str): The S3 public bucket path where this dataset is contained
         sample_preparation (str): Describe how the sample was prepared.
         sample_type (str): Type of samples used in a CryoET study. (cell, tissue, organism, intact organelle, in-vitro mixture, in-silico synthetic data, other)
         tissue_id (str): UBERON identifier for the tissue
         tissue_name (str): Name of the tissue from which a biological sample used in a CryoET study is derived from.
         title (str): Title of a CryoET dataset
-        tomograms (list[Tomogram]): An array relationship with Tomogram
     """
 
     _gql_type = "datasets"
 
     id: int = IntField()
     title: str = StringField()
     description: str = StringField()
@@ -64,23 +55,22 @@
     sample_type: str = StringField()
     organism_name: str = StringField()
     organism_taxid: str = StringField()
     tissue_name: str = StringField()
     tissue_id: str = StringField()
     cell_name: str = StringField()
     cell_type_id: str = StringField()
-    cell_line_name: str = StringField()
-    cell_line_source: str = StringField()
+    cell_strain_name: str = StringField()
+    cell_strain_id: str = StringField()
     sample_preparation: str = StringField()
     grid_preparation: str = StringField()
     other_setup: str = StringField()
     s3_prefix: str = StringField()
     https_prefix: str = StringField()
 
-    tomograms: Iterable["Tomogram"] = ListRelationship("Tomogram", "id", "dataset_id")
     runs: Iterable["Run"] = ListRelationship("Run", "id", "dataset_id")
     authors: Iterable["DatasetAuthor"] = ListRelationship("DatasetAuthor", "id", "dataset_id")
     funding_sources: Iterable["DatasetFunding"] = ListRelationship("DatasetFunding", "id", "dataset_id")
 
     def download_everything(self, dest_path: Optional[str] = None):
         """Download all of the data for this dataset.
 
@@ -95,14 +85,15 @@
     """Metadata for authors of a dataset
 
     Attributes:
         id (int): A numeric identifier for this author
         affiliation_address (str): Address of the institution an author is affiliated with.
         affiliation_identifier (str):  A unique identifier assigned to the affiliated institution by The Research Organization Registry (ROR).
         affiliation_name (str): Name of the institutions an author is affiliated with. Comma separated
+        primary_author_status (bool): Indicating whether an annotator is the main person executing the annotation, especially on manual annotation
         corresponding_author_status (bool):Indicating whether an author is the corresponding author
         dataset (Dataset): An object relationship with the dataset this author correspods to
         dataset_id (int): Numeric identifier for the dataset this author corresponds to
         email (str): Email address for each autho
         name (str): Full name of a dataset author (e.g. Jane Doe).
         orcid (str): A unique, persistent identifier for researchers, provided by ORCID.
     """
@@ -112,14 +103,15 @@
     dataset: Dataset = ItemRelationship(Dataset, "dataset_id", "id")
 
     id: int = IntField()
     dataset_id: int = IntField()
     orcid: str = StringField()
     name: str = StringField()
     corresponding_author_status: int = BooleanField()
+    primary_author_status: int = BooleanField()
     email: str = StringField()
     affiliation_name: str = StringField()
     affiliation_address: str = StringField()
     affiliation_identifier: str = StringField()
 
 
 class DatasetFunding(Model):
@@ -144,92 +136,84 @@
 
 
 class Run(Model):
     """Metadata for an experiment run
 
     Attributes:
         id (int): Numeric identifier (May change!)
-        acceleration_voltage (int): Electron Microscope Accelerator voltage in volts
-        annotations (list[Annotation]): An array relationship with the annotations associated with this run
-        binning_from_frames (float): Describes the binning factor from frames to tilt series file
-        camera_manufacturer: (str): Name of the camera manufacturer
-        camera_model (str): Camera model name
-        data_acquisition_software: (str): Software used to collect data
         dataset (Dataset): An object relationship with the dataset this run is a part of
         dataset_id (int): Reference to the dataset this run is a part of
+        name (str): Short name for the experiment run
         https_prefix (str): The HTTPS directory path where this dataset is contained
-        microscope_additional_info (str):  Other microscope optical setup information, in addition to energy filter, phase plate and image corrector
-        microscope_energy_filter: (str): Energy filter setup used
-        microscope_image_corrector (str): Image corrector setup
-        microscope_manufacturer (str): Name of the microscope manufacturer
-        microscope_model (str): Microscope model name
-        microscope_phase_plate (str): Phase plate configuration
-        name (str): Short name for the tilt series
-        related_empiar_entry (str):  If a tilt series is deposited into EMPIAR, enter the EMPIAR dataset identifier
         s3_prefix (str): The S3 public bucket path where this dataset is contained
-        spherical_aberration_constant (float): Spherical Aberration Constant of the objective lens in millimeters
-        tilt_axis (float): Rotation angle in degrees
-        tilt_max (float): Maximal tilt angle in degrees
-        tilt_min (float): Minimal tilt angle in degrees
-        tilt_range (float): Total tilt range in degrees
-        tilt_series_quality (int): Author assessment of tilt series quality within the dataset (1-5, 5 is best)
-        tilt_step (float): Tilt step in degrees
-        tilting_scheme (str): The order of stage tilting during acquisition of the data
         tiltseries (list[TiltSeries]): An array relationship with TiltSeries that correspond to this run
-        tomograms (list[Tomogram]): An array relationship with Tomograms that correspond to this run
-        total_flux (float): Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
+        tomogram_voxel_spacings (list[TomogramVoxelSpacing]): An array relationship with the Tomogram Voxel Spacings created from this run
     """
 
     _gql_type = "runs"
 
     dataset: Dataset = ItemRelationship(Dataset, "dataset_id", "id")
 
     id: int = IntField()
     dataset_id: int = IntField()
     name: str = StringField()
-    acceleration_voltage: int = IntField()
-    spherical_aberration_constant: float = FloatField()
-    microscope_manufacturer: str = StringField()
-    microscope_model: str = StringField()
-    microscope_energy_filter: str = StringField()
-    microscope_phase_plate: str = StringField()
-    microscope_image_corrector: str = StringField()
-    microscope_additional_info: str = StringField()
-    camera_manufacturer: str = StringField()
-    camera_model: str = StringField()
-    tilt_min: float = FloatField()
-    tilt_max: float = FloatField()
-    tilt_range: float = FloatField()
-    tilt_step: float = FloatField()
-    tilting_scheme: str = StringField()
-    tilt_axis: float = FloatField()
-    total_flux: float = FloatField()
-    data_acquisition_software: float = FloatField()
-    related_empiar_entry: str = StringField()
-    binning_from_frames: float = FloatField()
-    tilt_series_quality: int = IntField()
     s3_prefix: str = StringField()
     https_prefix: str = StringField()
 
-    tomograms: Iterable["Tomogram"] = ListRelationship("Tomogram", "id", "run_id")
-    annotations: Iterable["Annotation"] = ListRelationship("Annotation", "id", "run_id")
+    tomogram_voxel_spacings: Iterable["TomogramVoxelSpacing"] = ListRelationship("TomogramVoxelSpacing", "id", "run_id")
     tiltseries: Iterable["TiltSeries"] = ListRelationship("TiltSeries", "id", "run_id")
 
     def download_everything(self, dest_path: Optional[str] = None):
         """Download all of the data for this run.
 
         Args:
             dest_path (Optional[str], optional): Choose a destination directory. Defaults to $CWD.
         """
         download_directory(self.s3_prefix, self.dataset.s3_prefix, dest_path)
 
     def download_frames(self, dest_path: Optional[str] = None):
         download_directory(os.path.join(self.s3_prefix, "Frames"), self.dataset.s3_prefix)
 
 
+class TomogramVoxelSpacing(Model):
+    """Metadata for a set of tomograms and annotations of a given voxel spacing
+
+    Attributes:
+        id (int): Numeric identifier (May change!)
+        annotations (list[Annotation]): An array relationship with the annotations associated with this voxel spacing
+        https_prefix (str): The HTTPS directory path where this dataset is contained
+        run (Run): An object relationship with the run this voxel spacing is a part of
+        run_id (int): Reference to the dataset this run is a part of
+        s3_prefix (str): The S3 public bucket path where this dataset is contained
+        tomograms (list[Tomogram]): An array relationship with Tomograms of this voxel spacing
+        voxel_spacing (float): The voxel spacing for the tomograms in this set
+    """
+
+    _gql_type = "tomogram_voxel_spacings"
+
+    run: Run = ItemRelationship(Run, "run_id", "id")
+
+    id: int = IntField()
+    run_id: int = IntField()
+    voxel_spacing: float = FloatField()
+    s3_prefix: str = StringField()
+    https_prefix: str = StringField()
+
+    tomograms: Iterable["Tomogram"] = ListRelationship("Tomogram", "id", "tomogram_voxel_spacing_id")
+    annotations: Iterable["Annotation"] = ListRelationship("Annotation", "id", "tomogram_voxel_spacing_id")
+
+    def download_everything(self, dest_path: Optional[str] = None):
+        """Download all of the data for this run.
+
+        Args:
+            dest_path (Optional[str], optional): Choose a destination directory. Defaults to $CWD.
+        """
+        download_directory(self.s3_prefix, self.run.s3_prefix, dest_path)
+
+
 class Tomogram(Model):
     """Metadata for a tomogram
 
     Attributes:
         id (int): Numeric identifier for this tomogram (this may change!)
         ctf_corrected (bool): Whether this tomogram is CTF corrected
         dataset (Dataset): An object relationship with the dataset this tomogram is a part of
@@ -241,43 +225,41 @@
         https_omezarr_dir (str): HTTPS path to the this multiscale omezarr tomogram
         is_canonical (bool): Is this tomogram considered the canonical tomogram for the run experiment? True=Yes
         name (str): Short name for this tomogram
         processing (str): Describe additional processing used to derive the tomogram
         processing_software (str): Processing software used to derive the tomogram
         reconstruction_method (str):Describe reconstruction method (Weighted backprojection, SART, SIRT)
         reconstruction_software (str):Name of software used for reconstruction
-        run (Run): An object relationship with the run this tomogram is a part of
-        run_id (int): Reference to the run this tomogram is a part of
         s3_mrc_scale1 (str):S3 path to this tomogram in MRC format (downscaled to 50%)
         s3_mrc_scale2 (str):S3 path to this tomogram in MRC format (downscaled to 25%)
         s3_mrc_scale0 (str):S3 path to this tomogram in MRC format (no scaling)
         s3_omezarr_dir (str):S3 path to the this multiscale omezarr tomogram
         scale0_dimensions (str):comma separated x,y,z dimensions of the unscaled tomogram
         scale1_dimensions (str):comma separated x,y,z dimensions of the scale1 tomogram
         scale2_dimensions (str):comma separated x,y,z dimensions of the scale2 tomogram
         size_x (int): Number of pixels in the 3D data fast axis
         size_y (int): Number of pixels in the 3D data medium axis
         size_z (int):  Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
         tomogram_version (str): Version of tomogram using the same software and post-processing. Version of tomogram using the same software and post-processing. This will be presented as the latest version
+        tomogram_voxel_spacing (TomogramVoxelSpacing): An object relationship with a specific voxel spacing for this experiment run
         voxel_spacing (float): Voxel spacing equal in all three axes in angstroms
     """
 
     _gql_type = "tomograms"
 
-    dataset: Dataset = ItemRelationship(Dataset, "dataset_id", "id")
-    run: Run = ItemRelationship(Run, "run_id", "id")
+    tomogram_voxel_spacing: TomogramVoxelSpacing = ItemRelationship(
+        TomogramVoxelSpacing, "tomogram_voxel_spacing_id", "id"
+    )
 
     id: int = IntField()
-    dataset_id: int = IntField()
-    run_id: int = IntField()
+    tomogram_voxel_spacing_id: int = IntField()
     name: str = StringField()
     size_x: int = IntField()
     size_y: int = IntField()
     size_z: int = IntField()
-    voxel_spacing: float = FloatField()
     fiducial_alignment_status: str = StringField()
     reconstruction_method: str = StringField()
     reconstruction_software: str = StringField()
     processing: str = StringField()
     processing_software: str = StringField()
     tomogram_version: str = StringField()
     is_canonical: int = BooleanField()
@@ -289,14 +271,15 @@
     https_mrc_scale0: str = StringField()
     https_mrc_scale1: str = StringField()
     https_mrc_scale2: str = StringField()
     scale0_dimensions: str = StringField()
     scale1_dimensions: str = StringField()
     scale2_dimensions: str = StringField()
     ctf_corrected: int = BooleanField()
+    voxel_spacing: float = FloatField()
 
     def download_omezarr(self, dest_path: Optional[str] = None):
         """Download the omezarr version of this tomogram
 
         Args:
             dest_path (Optional[str], optional): Choose a destination directory. Defaults to $CWD.
         """
@@ -321,14 +304,15 @@
 class Annotation(Model):
     """Metadata for an annotation
 
     Attributes:
         id (int): Numeric identifier (May change!)
         annotation_method (str): Describe how the annotation is made (e.g. Manual, crYoLO, Positive Unlabeled Learning, template matching)
         annotation_publication (str): DOIs for publications that describe the dataset. Use a comma to separate multiple DOIs.
+        annotation_software (str): Software used for generating this annotation
         authors (list[Author]): An array relationship with the authors of this annotation
         confidence_precision (float): Describe the confidence level of the annotation. Precision is defined as the % of annotation objects being true positive
         confidence_recall (float): Describe the confidence level of the annotation. Recall is defined as the % of true positives being annotated correctly
         deposition_date (date): Date when an annotation set is initially received by the Data Portal.
         ground_truth_status (bool): Whether an annotation is considered ground truth, as determined by the annotator.
         ground_truth_used (str): Annotation filename used as ground truth for precision and recall
         https_annotations_path (str): HTTPS path for the annotations file for these annotations
@@ -339,36 +323,39 @@
         object_diameter (float): Diameter of the annotation object in Angstrom; applicable if the object shape is point or vector
         object_id (str): Gene Ontology Cellular Component identifier for the annotation object
         object_name (str): Name of the object being annotated (e.g. ribosome, nuclear pore complex, actin filament, membrane)
         object_state (str): Molecule state annotated (e.g. open, closed)
         object_weight (float): Molecular weight of the annotation object, in Dalton
         object_width (float): Average width of the annotation object in Angstroms; applicable if the object shape is line
         release_date (date): Date when annotation data is made public by the Data Portal.
-        run (Run): An object relationship with the run this annotation is a part of
-        run_id (int): Reference to the run these annotations are a part of
+        tomogram_voxel_spacing (TomogramVoxelSpacing): An object relationship with a specific voxel spacing for this annotation
+        tomogram_voxel_spacing_id (int): Reference to the tomogram voxel spacing group this annotation applies to
         s3_annotations_path (str): S3 path for the annotations file for these annotations
         s3_metadata_path (str): S3 path for the metadata json file for this annotation
         shape_type (str): The format are the individual annotations are stored in
     """
 
     _gql_type = "annotations"
 
-    run: Run = ItemRelationship(Run, "run_id", "id")
+    tomogram_voxel_spacing: TomogramVoxelSpacing = ItemRelationship(
+        TomogramVoxelSpacing, "tomogram_voxel_spacing_id", "id"
+    )
 
     id: int = IntField()
-    run_id: int = IntField()
+    tomogram_voxel_spacing_id: int = IntField()
     s3_metadata_path: str = StringField()
     https_metadata_path: str = StringField()
     s3_annotations_path: str = StringField()
     https_annotations_path: str = StringField()
     deposition_date: date = DateField()
     release_date: date = DateField()
     last_modified_date: date = DateField()
     annotation_publication: str = StringField()
     annotation_method: str = StringField()
+    annotation_software: str = StringField()
     ground_truth_status: int = BooleanField()
     object_name: str = StringField()
     object_id: str = StringField()
     object_description: str = StringField()
     object_state: str = StringField()
     shape_type: str = StringField()
     object_weight: float = FloatField()
@@ -416,34 +403,55 @@
     email: str = StringField()
     affiliation_name: str = StringField()
     affiliation_address: str = StringField()
     affiliation_identifier: str = StringField()
 
 
 class TiltSeries(Model):
-    """File locations for key files in a run's TiltSeries
+    """Metadata about how a tilt series was generated, and locations of output files
 
     Attributes:
         id (int): Numeric identifier for this tilt series (this may change!)
+        run (Run): An object relationship with the run this tiltseries is a part of
+        run_id (int): Reference to the run this tiltseries is a part of
+        acceleration_voltage (int): Electron Microscope Accelerator voltage in volts
+        binning_from_frames (float): Describes the binning factor from frames to tilt series file
+        camera_manufacturer: (str): Name of the camera manufacturer
+        camera_model (str): Camera model name
+        data_acquisition_software: (str): Software used to collect data
         https_alignment_file (str): HTTPS path to the alignment file for this tiltseries
         https_angle_list (str): HTTPS path to the angle list file for this tiltseries
         https_collection_metadata (str): HTTPS path to the collection metadata file for this tiltseries
         https_mrc_bin1 (str): HTTPS path to this tiltseries in MRC format (no scaling)
         https_mrc_bin2 (str): HTTPS path to this tiltseries in MRC format (downscaled to 50%)
         https_mrc_bin4 (str): HTTPS path to this tiltseries in MRC format (downscaled to 25%)
         https_omezarr_dir (str): HTTPS path to the this multiscale omezarr tiltseries
-        run (Run): An object relationship with the run this tiltseries is a part of
-        run_id (int): Reference to the run this tiltseries is a part of
+        microscope_additional_info (str):  Other microscope optical setup information, in addition to energy filter, phase plate and image corrector
+        microscope_energy_filter: (str): Energy filter setup used
+        microscope_image_corrector (str): Image corrector setup
+        microscope_manufacturer (str): Name of the microscope manufacturer
+        microscope_model (str): Microscope model name
+        microscope_phase_plate (str): Phase plate configuration
+        related_empiar_entry (str):  If a tilt series is deposited into EMPIAR, enter the EMPIAR dataset identifier
         s3_alignment_file (str): S3 path to the alignment file for this tiltseries
         s3_angle_list (str): S3 path to the angle list file for this tiltseries
         s3_collection_metadata (str): S3 path to the collection metadata file for this tiltseries
         s3_mrc_bin1 (str): S3 path to this tiltseries in MRC format (no scaling)
         s3_mrc_bin2 (str): S3 path to this tiltseries in MRC format (downscaled to 50%)
         s3_mrc_bin4 (str): S3 path to this tiltseries in MRC format (downscaled to 25%)
         s3_omezarr_dir (str): S3 path to the this multiscale omezarr tiltseries
+        spherical_aberration_constant (float): Spherical Aberration Constant of the objective lens in millimeters
+        tilt_axis (float): Rotation angle in degrees
+        tilt_max (float): Maximal tilt angle in degrees
+        tilt_min (float): Minimal tilt angle in degrees
+        tilt_range (float): Total tilt range in degrees
+        tilt_series_quality (int): Author assessment of tilt series quality within the dataset (1-5, 5 is best)
+        tilt_step (float): Tilt step in degrees
+        tilting_scheme (str): The order of stage tilting during acquisition of the data
+        total_flux (float): Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
     """
 
     _gql_type = "tiltseries"
 
     run: Run = ItemRelationship(Run, "run_id", "id")
 
     id: int = IntField()
@@ -458,14 +466,35 @@
     https_omezarr_dir: str = StringField()
     s3_collection_metadata: str = StringField()
     https_collection_metadata: str = StringField()
     s3_angle_list: str = StringField()
     https_angle_list: str = StringField()
     s3_alignment_file: str = StringField()
     https_alignment_file: str = StringField()
+    acceleration_voltage: int = IntField()
+    spherical_aberration_constant: float = FloatField()
+    microscope_manufacturer: str = StringField()
+    microscope_model: str = StringField()
+    microscope_energy_filter: str = StringField()
+    microscope_phase_plate: str = StringField()
+    microscope_image_corrector: str = StringField()
+    microscope_additional_info: str = StringField()
+    camera_manufacturer: str = StringField()
+    camera_model: str = StringField()
+    tilt_min: float = FloatField()
+    tilt_max: float = FloatField()
+    tilt_range: float = FloatField()
+    tilt_step: float = FloatField()
+    tilting_scheme: str = StringField()
+    tilt_axis: float = FloatField()
+    total_flux: float = FloatField()
+    data_acquisition_software: float = FloatField()
+    related_empiar_entry: str = StringField()
+    binning_from_frames: float = FloatField()
+    tilt_series_quality: int = IntField()
 
     def download_collection_metadata(self, dest_path: Optional[str] = None):
         """Download the collection metadata for this tiltseries
 
         Args:
             dest_path (Optional[str], optional): Choose a destination directory. Defaults to $CWD.
         """
@@ -516,7 +545,8 @@
 DatasetAuthor.setup()
 DatasetFunding.setup()
 Run.setup()
 Tomogram.setup()
 Annotation.setup()
 AnnotationAuthor.setup()
 TiltSeries.setup()
+TomogramVoxelSpacing.setup()
```

### Comparing `cryoet_data_portal-0.0.2/src/cryoet_data_portal/data/schema.graphql` & `cryoet_data_portal-1.0.0/src/cryoet_data_portal/data/schema.graphql`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 schema {
   query: query_root
-  subscription: subscription_root
 }
 
 """whether this query should be cached (Hasura Cloud only)"""
 directive @cached(
   """measured in seconds"""
   ttl: Int! = 60
 
@@ -595,14 +594,15 @@
   """
   annotation_method: String!
 
   """
   DOIs for publications that describe the dataset. Use a comma to separate multiple DOIs.
   """
   annotation_publication: String
+  annotation_software: String
 
   """An array relationship"""
   authors(
     """distinct select on columns"""
     distinct_on: [annotation_authors_select_column!]
 
     """limit the number of rows returned"""
@@ -700,28 +700,26 @@
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: numeric
 
   """Date when annotation data is made public by the Data Portal."""
   release_date: date!
 
-  """An object relationship"""
-  run: runs!
-
-  """Reference to the run these annotations are a part of"""
-  run_id: Int!
-
   """s3 path for the annotations file for these annotations"""
   s3_annotations_path: String
 
   """s3 path for the metadata json file for this annotation"""
   s3_metadata_path: String!
 
   """The format are the individual annotations are stored in"""
   shape_type: String!
+
+  """An object relationship"""
+  tomogram_voxel_spacing: tomogram_voxel_spacings
+  tomogram_voxel_spacing_id: Int
 }
 
 """
 aggregated selection of "annotations"
 """
 type annotations_aggregate {
   aggregate: annotations_aggregate_fields
@@ -815,17 +813,15 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: Float
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: Float
-
-  """Reference to the run these annotations are a part of"""
-  run_id: Float
+  tomogram_voxel_spacing_id: Float
 }
 
 """
 order by avg() on columns of table "annotations"
 """
 input annotations_avg_order_by {
   """
@@ -852,28 +848,27 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: order_by
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: order_by
-
-  """Reference to the run these annotations are a part of"""
-  run_id: order_by
+  tomogram_voxel_spacing_id: order_by
 }
 
 """
 Boolean expression to filter rows from the table "annotations". All fields are combined with a logical 'AND'.
 """
 input annotations_bool_exp {
   _and: [annotations_bool_exp!]
   _not: annotations_bool_exp
   _or: [annotations_bool_exp!]
   annotation_method: String_comparison_exp
   annotation_publication: String_comparison_exp
+  annotation_software: String_comparison_exp
   authors: annotation_authors_bool_exp
   authors_aggregate: annotation_authors_aggregate_bool_exp
   confidence_precision: numeric_comparison_exp
   confidence_recall: numeric_comparison_exp
   deposition_date: date_comparison_exp
   ground_truth_status: Boolean_comparison_exp
   ground_truth_used: String_comparison_exp
@@ -886,32 +881,33 @@
   object_diameter: numeric_comparison_exp
   object_id: String_comparison_exp
   object_name: String_comparison_exp
   object_state: String_comparison_exp
   object_weight: numeric_comparison_exp
   object_width: numeric_comparison_exp
   release_date: date_comparison_exp
-  run: runs_bool_exp
-  run_id: Int_comparison_exp
   s3_annotations_path: String_comparison_exp
   s3_metadata_path: String_comparison_exp
   shape_type: String_comparison_exp
+  tomogram_voxel_spacing: tomogram_voxel_spacings_bool_exp
+  tomogram_voxel_spacing_id: Int_comparison_exp
 }
 
 """aggregate max on columns"""
 type annotations_max_fields {
   """
   Describe how the annotation is made (e.g. Manual, crYoLO, Positive Unlabeled Learning, template matching)
   """
   annotation_method: String
 
   """
   DOIs for publications that describe the dataset. Use a comma to separate multiple DOIs.
   """
   annotation_publication: String
+  annotation_software: String
 
   """
   Describe the confidence level of the annotation. Precision is defined as the % of annotation objects being true positive
   """
   confidence_precision: numeric
 
   """
@@ -968,25 +964,23 @@
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: numeric
 
   """Date when annotation data is made public by the Data Portal."""
   release_date: date
 
-  """Reference to the run these annotations are a part of"""
-  run_id: Int
-
   """s3 path for the annotations file for these annotations"""
   s3_annotations_path: String
 
   """s3 path for the metadata json file for this annotation"""
   s3_metadata_path: String
 
   """The format are the individual annotations are stored in"""
   shape_type: String
+  tomogram_voxel_spacing_id: Int
 }
 
 """
 order by max() on columns of table "annotations"
 """
 input annotations_max_order_by {
   """
@@ -994,14 +988,15 @@
   """
   annotation_method: order_by
 
   """
   DOIs for publications that describe the dataset. Use a comma to separate multiple DOIs.
   """
   annotation_publication: order_by
+  annotation_software: order_by
 
   """
   Describe the confidence level of the annotation. Precision is defined as the % of annotation objects being true positive
   """
   confidence_precision: order_by
 
   """
@@ -1058,38 +1053,37 @@
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: order_by
 
   """Date when annotation data is made public by the Data Portal."""
   release_date: order_by
 
-  """Reference to the run these annotations are a part of"""
-  run_id: order_by
-
   """s3 path for the annotations file for these annotations"""
   s3_annotations_path: order_by
 
   """s3 path for the metadata json file for this annotation"""
   s3_metadata_path: order_by
 
   """The format are the individual annotations are stored in"""
   shape_type: order_by
+  tomogram_voxel_spacing_id: order_by
 }
 
 """aggregate min on columns"""
 type annotations_min_fields {
   """
   Describe how the annotation is made (e.g. Manual, crYoLO, Positive Unlabeled Learning, template matching)
   """
   annotation_method: String
 
   """
   DOIs for publications that describe the dataset. Use a comma to separate multiple DOIs.
   """
   annotation_publication: String
+  annotation_software: String
 
   """
   Describe the confidence level of the annotation. Precision is defined as the % of annotation objects being true positive
   """
   confidence_precision: numeric
 
   """
@@ -1146,25 +1140,23 @@
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: numeric
 
   """Date when annotation data is made public by the Data Portal."""
   release_date: date
 
-  """Reference to the run these annotations are a part of"""
-  run_id: Int
-
   """s3 path for the annotations file for these annotations"""
   s3_annotations_path: String
 
   """s3 path for the metadata json file for this annotation"""
   s3_metadata_path: String
 
   """The format are the individual annotations are stored in"""
   shape_type: String
+  tomogram_voxel_spacing_id: Int
 }
 
 """
 order by min() on columns of table "annotations"
 """
 input annotations_min_order_by {
   """
@@ -1172,14 +1164,15 @@
   """
   annotation_method: order_by
 
   """
   DOIs for publications that describe the dataset. Use a comma to separate multiple DOIs.
   """
   annotation_publication: order_by
+  annotation_software: order_by
 
   """
   Describe the confidence level of the annotation. Precision is defined as the % of annotation objects being true positive
   """
   confidence_precision: order_by
 
   """
@@ -1236,31 +1229,30 @@
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: order_by
 
   """Date when annotation data is made public by the Data Portal."""
   release_date: order_by
 
-  """Reference to the run these annotations are a part of"""
-  run_id: order_by
-
   """s3 path for the annotations file for these annotations"""
   s3_annotations_path: order_by
 
   """s3 path for the metadata json file for this annotation"""
   s3_metadata_path: order_by
 
   """The format are the individual annotations are stored in"""
   shape_type: order_by
+  tomogram_voxel_spacing_id: order_by
 }
 
 """Ordering options when selecting data from "annotations"."""
 input annotations_order_by {
   annotation_method: order_by
   annotation_publication: order_by
+  annotation_software: order_by
   authors_aggregate: annotation_authors_aggregate_order_by
   confidence_precision: order_by
   confidence_recall: order_by
   deposition_date: order_by
   ground_truth_status: order_by
   ground_truth_used: order_by
   https_annotations_path: order_by
@@ -1272,32 +1264,35 @@
   object_diameter: order_by
   object_id: order_by
   object_name: order_by
   object_state: order_by
   object_weight: order_by
   object_width: order_by
   release_date: order_by
-  run: runs_order_by
-  run_id: order_by
   s3_annotations_path: order_by
   s3_metadata_path: order_by
   shape_type: order_by
+  tomogram_voxel_spacing: tomogram_voxel_spacings_order_by
+  tomogram_voxel_spacing_id: order_by
 }
 
 """
 select columns of table "annotations"
 """
 enum annotations_select_column {
   """column name"""
   annotation_method
 
   """column name"""
   annotation_publication
 
   """column name"""
+  annotation_software
+
+  """column name"""
   confidence_precision
 
   """column name"""
   confidence_recall
 
   """column name"""
   deposition_date
@@ -1344,24 +1339,24 @@
   """column name"""
   object_width
 
   """column name"""
   release_date
 
   """column name"""
-  run_id
-
-  """column name"""
   s3_annotations_path
 
   """column name"""
   s3_metadata_path
 
   """column name"""
   shape_type
+
+  """column name"""
+  tomogram_voxel_spacing_id
 }
 
 """
 select "annotations_aggregate_bool_exp_bool_and_arguments_columns" columns of table "annotations"
 """
 enum annotations_select_column_annotations_aggregate_bool_exp_bool_and_arguments_columns {
   """column name"""
@@ -1402,17 +1397,15 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: Float
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: Float
-
-  """Reference to the run these annotations are a part of"""
-  run_id: Float
+  tomogram_voxel_spacing_id: Float
 }
 
 """
 order by stddev() on columns of table "annotations"
 """
 input annotations_stddev_order_by {
   """
@@ -1439,17 +1432,15 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: order_by
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: order_by
-
-  """Reference to the run these annotations are a part of"""
-  run_id: order_by
+  tomogram_voxel_spacing_id: order_by
 }
 
 """aggregate stddev_pop on columns"""
 type annotations_stddev_pop_fields {
   """
   Describe the confidence level of the annotation. Precision is defined as the % of annotation objects being true positive
   """
@@ -1474,17 +1465,15 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: Float
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: Float
-
-  """Reference to the run these annotations are a part of"""
-  run_id: Float
+  tomogram_voxel_spacing_id: Float
 }
 
 """
 order by stddev_pop() on columns of table "annotations"
 """
 input annotations_stddev_pop_order_by {
   """
@@ -1511,17 +1500,15 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: order_by
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: order_by
-
-  """Reference to the run these annotations are a part of"""
-  run_id: order_by
+  tomogram_voxel_spacing_id: order_by
 }
 
 """aggregate stddev_samp on columns"""
 type annotations_stddev_samp_fields {
   """
   Describe the confidence level of the annotation. Precision is defined as the % of annotation objects being true positive
   """
@@ -1546,17 +1533,15 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: Float
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: Float
-
-  """Reference to the run these annotations are a part of"""
-  run_id: Float
+  tomogram_voxel_spacing_id: Float
 }
 
 """
 order by stddev_samp() on columns of table "annotations"
 """
 input annotations_stddev_samp_order_by {
   """
@@ -1583,17 +1568,15 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: order_by
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: order_by
-
-  """Reference to the run these annotations are a part of"""
-  run_id: order_by
+  tomogram_voxel_spacing_id: order_by
 }
 
 """aggregate sum on columns"""
 type annotations_sum_fields {
   """
   Describe the confidence level of the annotation. Precision is defined as the % of annotation objects being true positive
   """
@@ -1618,17 +1601,15 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: numeric
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: numeric
-
-  """Reference to the run these annotations are a part of"""
-  run_id: Int
+  tomogram_voxel_spacing_id: Int
 }
 
 """
 order by sum() on columns of table "annotations"
 """
 input annotations_sum_order_by {
   """
@@ -1655,17 +1636,15 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: order_by
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: order_by
-
-  """Reference to the run these annotations are a part of"""
-  run_id: order_by
+  tomogram_voxel_spacing_id: order_by
 }
 
 """aggregate var_pop on columns"""
 type annotations_var_pop_fields {
   """
   Describe the confidence level of the annotation. Precision is defined as the % of annotation objects being true positive
   """
@@ -1690,17 +1669,15 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: Float
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: Float
-
-  """Reference to the run these annotations are a part of"""
-  run_id: Float
+  tomogram_voxel_spacing_id: Float
 }
 
 """
 order by var_pop() on columns of table "annotations"
 """
 input annotations_var_pop_order_by {
   """
@@ -1727,17 +1704,15 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: order_by
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: order_by
-
-  """Reference to the run these annotations are a part of"""
-  run_id: order_by
+  tomogram_voxel_spacing_id: order_by
 }
 
 """aggregate var_samp on columns"""
 type annotations_var_samp_fields {
   """
   Describe the confidence level of the annotation. Precision is defined as the % of annotation objects being true positive
   """
@@ -1762,17 +1737,15 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: Float
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: Float
-
-  """Reference to the run these annotations are a part of"""
-  run_id: Float
+  tomogram_voxel_spacing_id: Float
 }
 
 """
 order by var_samp() on columns of table "annotations"
 """
 input annotations_var_samp_order_by {
   """
@@ -1799,17 +1772,15 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: order_by
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: order_by
-
-  """Reference to the run these annotations are a part of"""
-  run_id: order_by
+  tomogram_voxel_spacing_id: order_by
 }
 
 """aggregate variance on columns"""
 type annotations_variance_fields {
   """
   Describe the confidence level of the annotation. Precision is defined as the % of annotation objects being true positive
   """
@@ -1834,17 +1805,15 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: Float
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: Float
-
-  """Reference to the run these annotations are a part of"""
-  run_id: Float
+  tomogram_voxel_spacing_id: Float
 }
 
 """
 order by variance() on columns of table "annotations"
 """
 input annotations_variance_order_by {
   """
@@ -1871,17 +1840,15 @@
   """Molecular weight of the annotation object, in Dalton"""
   object_weight: order_by
 
   """
   Average width of the annotation object in Angstroms; applicable if the object shape is line
   """
   object_width: order_by
-
-  """Reference to the run these annotations are a part of"""
-  run_id: order_by
+  tomogram_voxel_spacing_id: order_by
 }
 
 """Authors of a dataset"""
 type dataset_authors {
   """Address of the institution an author is affiliated with."""
   affiliation_address: String
 
@@ -1905,14 +1872,15 @@
   id: Int!
 
   """Full name of a dataset author (e.g. Jane Doe)."""
   name: String!
 
   """A unique, persistent identifier for researchers, provided by ORCID."""
   orcid: String
+  primary_author_status: Boolean
 }
 
 """
 aggregated selection of "dataset_authors"
 """
 type dataset_authors_aggregate {
   aggregate: dataset_authors_aggregate_fields
@@ -2007,14 +1975,15 @@
   corresponding_author_status: Boolean_comparison_exp
   dataset: datasets_bool_exp
   dataset_id: Int_comparison_exp
   email: String_comparison_exp
   id: Int_comparison_exp
   name: String_comparison_exp
   orcid: String_comparison_exp
+  primary_author_status: Boolean_comparison_exp
 }
 
 """aggregate max on columns"""
 type dataset_authors_max_fields {
   """Address of the institution an author is affiliated with."""
   affiliation_address: String
 
@@ -2125,14 +2094,15 @@
   corresponding_author_status: order_by
   dataset: datasets_order_by
   dataset_id: order_by
   email: order_by
   id: order_by
   name: order_by
   orcid: order_by
+  primary_author_status: order_by
 }
 
 """
 select columns of table "dataset_authors"
 """
 enum dataset_authors_select_column {
   """column name"""
@@ -2157,30 +2127,39 @@
   id
 
   """column name"""
   name
 
   """column name"""
   orcid
+
+  """column name"""
+  primary_author_status
 }
 
 """
 select "dataset_authors_aggregate_bool_exp_bool_and_arguments_columns" columns of table "dataset_authors"
 """
 enum dataset_authors_select_column_dataset_authors_aggregate_bool_exp_bool_and_arguments_columns {
   """column name"""
   corresponding_author_status
+
+  """column name"""
+  primary_author_status
 }
 
 """
 select "dataset_authors_aggregate_bool_exp_bool_or_arguments_columns" columns of table "dataset_authors"
 """
 enum dataset_authors_select_column_dataset_authors_aggregate_bool_exp_bool_or_arguments_columns {
   """column name"""
   corresponding_author_status
+
+  """column name"""
+  primary_author_status
 }
 
 """aggregate stddev on columns"""
 type dataset_authors_stddev_fields {
   dataset_id: Float
   id: Float
 }
@@ -2582,25 +2561,25 @@
     """sort the rows by one or more columns"""
     order_by: [dataset_authors_order_by!]
 
     """filter the rows returned"""
     where: dataset_authors_bool_exp
   ): dataset_authors_aggregate!
 
-  """Cell line or strain for the sample."""
-  cell_line_name: String
-
-  """Name of the company from which the sample is sourced from."""
-  cell_line_source: String
-
   """
   Name of the cell from which a biological sample used in a CryoET study is derived from.
   """
   cell_name: String
 
+  """NCBI Identifier for the cell line or strain"""
+  cell_strain_id: String
+
+  """Cell line or strain for the sample."""
+  cell_strain_name: String
+
   """Cell Ontology identifier for the cell type"""
   cell_type_id: String
 
   """
   DOIs for publications that cite the dataset. Use a comma to separate multiple DOIs.
   """
   dataset_citations: String
@@ -2747,50 +2726,14 @@
   """
   Name of the tissue from which a biological sample used in a CryoET study is derived from.
   """
   tissue_name: String
 
   """Title of a CryoET dataset"""
   title: String!
-
-  """An array relationship"""
-  tomograms(
-    """distinct select on columns"""
-    distinct_on: [tomograms_select_column!]
-
-    """limit the number of rows returned"""
-    limit: Int
-
-    """skip the first n rows. Use only with order_by"""
-    offset: Int
-
-    """sort the rows by one or more columns"""
-    order_by: [tomograms_order_by!]
-
-    """filter the rows returned"""
-    where: tomograms_bool_exp
-  ): [tomograms!]!
-
-  """An aggregate relationship"""
-  tomograms_aggregate(
-    """distinct select on columns"""
-    distinct_on: [tomograms_select_column!]
-
-    """limit the number of rows returned"""
-    limit: Int
-
-    """skip the first n rows. Use only with order_by"""
-    offset: Int
-
-    """sort the rows by one or more columns"""
-    order_by: [tomograms_order_by!]
-
-    """filter the rows returned"""
-    where: tomograms_bool_exp
-  ): tomograms_aggregate!
 }
 
 """
 aggregated selection of "datasets"
 """
 type datasets_aggregate {
   aggregate: datasets_aggregate_fields
@@ -2827,17 +2770,17 @@
 """
 input datasets_bool_exp {
   _and: [datasets_bool_exp!]
   _not: datasets_bool_exp
   _or: [datasets_bool_exp!]
   authors: dataset_authors_bool_exp
   authors_aggregate: dataset_authors_aggregate_bool_exp
-  cell_line_name: String_comparison_exp
-  cell_line_source: String_comparison_exp
   cell_name: String_comparison_exp
+  cell_strain_id: String_comparison_exp
+  cell_strain_name: String_comparison_exp
   cell_type_id: String_comparison_exp
   dataset_citations: String_comparison_exp
   dataset_publications: String_comparison_exp
   deposition_date: date_comparison_exp
   description: String_comparison_exp
   funding_sources: dataset_funding_bool_exp
   funding_sources_aggregate: dataset_funding_aggregate_bool_exp
@@ -2855,31 +2798,29 @@
   runs_aggregate: runs_aggregate_bool_exp
   s3_prefix: String_comparison_exp
   sample_preparation: String_comparison_exp
   sample_type: String_comparison_exp
   tissue_id: String_comparison_exp
   tissue_name: String_comparison_exp
   title: String_comparison_exp
-  tomograms: tomograms_bool_exp
-  tomograms_aggregate: tomograms_aggregate_bool_exp
 }
 
 """aggregate max on columns"""
 type datasets_max_fields {
-  """Cell line or strain for the sample."""
-  cell_line_name: String
-
-  """Name of the company from which the sample is sourced from."""
-  cell_line_source: String
-
   """
   Name of the cell from which a biological sample used in a CryoET study is derived from.
   """
   cell_name: String
 
+  """NCBI Identifier for the cell line or strain"""
+  cell_strain_id: String
+
+  """Cell line or strain for the sample."""
+  cell_strain_name: String
+
   """Cell Ontology identifier for the cell type"""
   cell_type_id: String
 
   """
   DOIs for publications that cite the dataset. Use a comma to separate multiple DOIs.
   """
   dataset_citations: String
@@ -2958,25 +2899,25 @@
 
   """Title of a CryoET dataset"""
   title: String
 }
 
 """aggregate min on columns"""
 type datasets_min_fields {
-  """Cell line or strain for the sample."""
-  cell_line_name: String
-
-  """Name of the company from which the sample is sourced from."""
-  cell_line_source: String
-
   """
   Name of the cell from which a biological sample used in a CryoET study is derived from.
   """
   cell_name: String
 
+  """NCBI Identifier for the cell line or strain"""
+  cell_strain_id: String
+
+  """Cell line or strain for the sample."""
+  cell_strain_name: String
+
   """Cell Ontology identifier for the cell type"""
   cell_type_id: String
 
   """
   DOIs for publications that cite the dataset. Use a comma to separate multiple DOIs.
   """
   dataset_citations: String
@@ -3056,17 +2997,17 @@
   """Title of a CryoET dataset"""
   title: String
 }
 
 """Ordering options when selecting data from "datasets"."""
 input datasets_order_by {
   authors_aggregate: dataset_authors_aggregate_order_by
-  cell_line_name: order_by
-  cell_line_source: order_by
   cell_name: order_by
+  cell_strain_id: order_by
+  cell_strain_name: order_by
   cell_type_id: order_by
   dataset_citations: order_by
   dataset_publications: order_by
   deposition_date: order_by
   description: order_by
   funding_sources_aggregate: dataset_funding_aggregate_order_by
   grid_preparation: order_by
@@ -3082,29 +3023,28 @@
   runs_aggregate: runs_aggregate_order_by
   s3_prefix: order_by
   sample_preparation: order_by
   sample_type: order_by
   tissue_id: order_by
   tissue_name: order_by
   title: order_by
-  tomograms_aggregate: tomograms_aggregate_order_by
 }
 
 """
 select columns of table "datasets"
 """
 enum datasets_select_column {
   """column name"""
-  cell_line_name
+  cell_name
 
   """column name"""
-  cell_line_source
+  cell_strain_id
 
   """column name"""
-  cell_name
+  cell_strain_name
 
   """column name"""
   cell_type_id
 
   """column name"""
   dataset_citations
 
@@ -3580,176 +3520,117 @@
     where: tiltseries_bool_exp
   ): tiltseries_aggregate!
 
   """fetch data from the table: "tiltseries" using primary key columns"""
   tiltseries_by_pk(id: Int!): tiltseries
 
   """An array relationship"""
-  tomograms(
+  tomogram_voxel_spacings(
     """distinct select on columns"""
-    distinct_on: [tomograms_select_column!]
+    distinct_on: [tomogram_voxel_spacings_select_column!]
 
     """limit the number of rows returned"""
     limit: Int
 
     """skip the first n rows. Use only with order_by"""
     offset: Int
 
     """sort the rows by one or more columns"""
-    order_by: [tomograms_order_by!]
+    order_by: [tomogram_voxel_spacings_order_by!]
 
     """filter the rows returned"""
-    where: tomograms_bool_exp
-  ): [tomograms!]!
+    where: tomogram_voxel_spacings_bool_exp
+  ): [tomogram_voxel_spacings!]!
 
   """An aggregate relationship"""
-  tomograms_aggregate(
+  tomogram_voxel_spacings_aggregate(
     """distinct select on columns"""
-    distinct_on: [tomograms_select_column!]
+    distinct_on: [tomogram_voxel_spacings_select_column!]
 
     """limit the number of rows returned"""
     limit: Int
 
     """skip the first n rows. Use only with order_by"""
     offset: Int
 
     """sort the rows by one or more columns"""
-    order_by: [tomograms_order_by!]
+    order_by: [tomogram_voxel_spacings_order_by!]
 
     """filter the rows returned"""
-    where: tomograms_bool_exp
-  ): tomograms_aggregate!
+    where: tomogram_voxel_spacings_bool_exp
+  ): tomogram_voxel_spacings_aggregate!
 
-  """fetch data from the table: "tomograms" using primary key columns"""
-  tomograms_by_pk(
-    """Numeric identifier for this tomogram (this may change!)"""
-    id: Int!
-  ): tomograms
-}
-
-"""Data related to an experiment run"""
-type runs {
-  """Electron Microscope Accelerator voltage in volts"""
-  acceleration_voltage: Int!
+  """
+  fetch data from the table: "tomogram_voxel_spacings" using primary key columns
+  """
+  tomogram_voxel_spacings_by_pk(id: Int!): tomogram_voxel_spacings
 
   """An array relationship"""
-  annotations(
+  tomograms(
     """distinct select on columns"""
-    distinct_on: [annotations_select_column!]
+    distinct_on: [tomograms_select_column!]
 
     """limit the number of rows returned"""
     limit: Int
 
     """skip the first n rows. Use only with order_by"""
     offset: Int
 
     """sort the rows by one or more columns"""
-    order_by: [annotations_order_by!]
+    order_by: [tomograms_order_by!]
 
     """filter the rows returned"""
-    where: annotations_bool_exp
-  ): [annotations!]!
+    where: tomograms_bool_exp
+  ): [tomograms!]!
 
   """An aggregate relationship"""
-  annotations_aggregate(
+  tomograms_aggregate(
     """distinct select on columns"""
-    distinct_on: [annotations_select_column!]
+    distinct_on: [tomograms_select_column!]
 
     """limit the number of rows returned"""
     limit: Int
 
     """skip the first n rows. Use only with order_by"""
     offset: Int
 
     """sort the rows by one or more columns"""
-    order_by: [annotations_order_by!]
+    order_by: [tomograms_order_by!]
 
     """filter the rows returned"""
-    where: annotations_bool_exp
-  ): annotations_aggregate!
-
-  """Describes the binning factor from frames to tilt series file"""
-  binning_from_frames: numeric!
-
-  """Name of the camera manufacturer"""
-  camera_manufacturer: String!
-
-  """Camera model name"""
-  camera_model: String!
+    where: tomograms_bool_exp
+  ): tomograms_aggregate!
 
-  """Software used to collect data"""
-  data_acquisition_software: String!
+  """fetch data from the table: "tomograms" using primary key columns"""
+  tomograms_by_pk(
+    """Numeric identifier for this tomogram (this may change!)"""
+    id: Int!
+  ): tomograms
+}
 
+"""Data related to an experiment run"""
+type runs {
   """An object relationship"""
   dataset: datasets!
 
   """Reference to the dataset this run is a part of"""
   dataset_id: Int!
 
   """The https directory path where this dataset is contained"""
   https_prefix: String!
 
   """Numeric identifier (May change!)"""
   id: Int!
 
-  """
-  Other microscope optical setup information, in addition to energy filter, phase plate and image corrector
-  """
-  microscope_additional_info: String
-
-  """Energy filter setup used"""
-  microscope_energy_filter: String!
-
-  """Image corrector setup"""
-  microscope_image_corrector: String!
-
-  """Name of the microscope manufacturer"""
-  microscope_manufacturer: String!
-
-  """Microscope model name"""
-  microscope_model: String!
-
-  """Phase plate configuration"""
-  microscope_phase_plate: String!
-
   """Short name for the tilt series"""
   name: String!
 
-  """
-  If a tilt series is deposited into EMPIAR, enter the EMPIAR dataset identifier
-  """
-  related_empiar_entry: String
-
   """The S3 public bucket path where this dataset is contained"""
   s3_prefix: String!
 
-  """Spherical Aberration Constant of the objective lens in millimeters"""
-  spherical_aberration_constant: numeric!
-
-  """Rotation angle in degrees"""
-  tilt_axis: numeric
-
-  """Maximal tilt angle in degrees"""
-  tilt_max: numeric!
-
-  """Minimal tilt angle in degrees"""
-  tilt_min: numeric!
-  tilt_range: numeric!
-
-  """
-  Author assessment of tilt series quality within the dataset (1-5, 5 is best)
-  """
-  tilt_series_quality: Int!
-
-  """Tilt step in degrees"""
-  tilt_step: numeric!
-
-  """The order of stage tilting during acquisition of the data"""
-  tilting_scheme: String!
-
   """An array relationship"""
   tiltseries(
     """distinct select on columns"""
     distinct_on: [tiltseries_select_column!]
 
     """limit the number of rows returned"""
     limit: Int
@@ -3779,53 +3660,48 @@
     order_by: [tiltseries_order_by!]
 
     """filter the rows returned"""
     where: tiltseries_bool_exp
   ): tiltseries_aggregate!
 
   """An array relationship"""
-  tomograms(
+  tomogram_voxel_spacings(
     """distinct select on columns"""
-    distinct_on: [tomograms_select_column!]
+    distinct_on: [tomogram_voxel_spacings_select_column!]
 
     """limit the number of rows returned"""
     limit: Int
 
     """skip the first n rows. Use only with order_by"""
     offset: Int
 
     """sort the rows by one or more columns"""
-    order_by: [tomograms_order_by!]
+    order_by: [tomogram_voxel_spacings_order_by!]
 
     """filter the rows returned"""
-    where: tomograms_bool_exp
-  ): [tomograms!]!
+    where: tomogram_voxel_spacings_bool_exp
+  ): [tomogram_voxel_spacings!]!
 
   """An aggregate relationship"""
-  tomograms_aggregate(
+  tomogram_voxel_spacings_aggregate(
     """distinct select on columns"""
-    distinct_on: [tomograms_select_column!]
+    distinct_on: [tomogram_voxel_spacings_select_column!]
 
     """limit the number of rows returned"""
     limit: Int
 
     """skip the first n rows. Use only with order_by"""
     offset: Int
 
     """sort the rows by one or more columns"""
-    order_by: [tomograms_order_by!]
+    order_by: [tomogram_voxel_spacings_order_by!]
 
     """filter the rows returned"""
-    where: tomograms_bool_exp
-  ): tomograms_aggregate!
-
-  """
-  Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
-  """
-  total_flux: numeric!
+    where: tomogram_voxel_spacings_bool_exp
+  ): tomogram_voxel_spacings_aggregate!
 }
 
 """
 aggregated selection of "runs"
 """
 type runs_aggregate {
   aggregate: runs_aggregate_fields
@@ -3875,162 +3751,589 @@
   var_pop: runs_var_pop_order_by
   var_samp: runs_var_samp_order_by
   variance: runs_variance_order_by
 }
 
 """aggregate avg on columns"""
 type runs_avg_fields {
-  """Electron Microscope Accelerator voltage in volts"""
-  acceleration_voltage: Float
+  """Reference to the dataset this run is a part of"""
+  dataset_id: Float
 
-  """Describes the binning factor from frames to tilt series file"""
-  binning_from_frames: Float
+  """Numeric identifier (May change!)"""
+  id: Float
+}
 
+"""
+order by avg() on columns of table "runs"
+"""
+input runs_avg_order_by {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: order_by
+
+  """Numeric identifier (May change!)"""
+  id: order_by
+}
+
+"""
+Boolean expression to filter rows from the table "runs". All fields are combined with a logical 'AND'.
+"""
+input runs_bool_exp {
+  _and: [runs_bool_exp!]
+  _not: runs_bool_exp
+  _or: [runs_bool_exp!]
+  dataset: datasets_bool_exp
+  dataset_id: Int_comparison_exp
+  https_prefix: String_comparison_exp
+  id: Int_comparison_exp
+  name: String_comparison_exp
+  s3_prefix: String_comparison_exp
+  tiltseries: tiltseries_bool_exp
+  tiltseries_aggregate: tiltseries_aggregate_bool_exp
+  tomogram_voxel_spacings: tomogram_voxel_spacings_bool_exp
+  tomogram_voxel_spacings_aggregate: tomogram_voxel_spacings_aggregate_bool_exp
+}
+
+"""aggregate max on columns"""
+type runs_max_fields {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: Int
+
+  """The https directory path where this dataset is contained"""
+  https_prefix: String
+
+  """Numeric identifier (May change!)"""
+  id: Int
+
+  """Short name for the tilt series"""
+  name: String
+
+  """The S3 public bucket path where this dataset is contained"""
+  s3_prefix: String
+}
+
+"""
+order by max() on columns of table "runs"
+"""
+input runs_max_order_by {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: order_by
+
+  """The https directory path where this dataset is contained"""
+  https_prefix: order_by
+
+  """Numeric identifier (May change!)"""
+  id: order_by
+
+  """Short name for the tilt series"""
+  name: order_by
+
+  """The S3 public bucket path where this dataset is contained"""
+  s3_prefix: order_by
+}
+
+"""aggregate min on columns"""
+type runs_min_fields {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: Int
+
+  """The https directory path where this dataset is contained"""
+  https_prefix: String
+
+  """Numeric identifier (May change!)"""
+  id: Int
+
+  """Short name for the tilt series"""
+  name: String
+
+  """The S3 public bucket path where this dataset is contained"""
+  s3_prefix: String
+}
+
+"""
+order by min() on columns of table "runs"
+"""
+input runs_min_order_by {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: order_by
+
+  """The https directory path where this dataset is contained"""
+  https_prefix: order_by
+
+  """Numeric identifier (May change!)"""
+  id: order_by
+
+  """Short name for the tilt series"""
+  name: order_by
+
+  """The S3 public bucket path where this dataset is contained"""
+  s3_prefix: order_by
+}
+
+"""Ordering options when selecting data from "runs"."""
+input runs_order_by {
+  dataset: datasets_order_by
+  dataset_id: order_by
+  https_prefix: order_by
+  id: order_by
+  name: order_by
+  s3_prefix: order_by
+  tiltseries_aggregate: tiltseries_aggregate_order_by
+  tomogram_voxel_spacings_aggregate: tomogram_voxel_spacings_aggregate_order_by
+}
+
+"""
+select columns of table "runs"
+"""
+enum runs_select_column {
+  """column name"""
+  dataset_id
+
+  """column name"""
+  https_prefix
+
+  """column name"""
+  id
+
+  """column name"""
+  name
+
+  """column name"""
+  s3_prefix
+}
+
+"""aggregate stddev on columns"""
+type runs_stddev_fields {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: Float
+
+  """Numeric identifier (May change!)"""
+  id: Float
+}
+
+"""
+order by stddev() on columns of table "runs"
+"""
+input runs_stddev_order_by {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: order_by
+
+  """Numeric identifier (May change!)"""
+  id: order_by
+}
+
+"""aggregate stddev_pop on columns"""
+type runs_stddev_pop_fields {
   """Reference to the dataset this run is a part of"""
   dataset_id: Float
 
   """Numeric identifier (May change!)"""
   id: Float
+}
+
+"""
+order by stddev_pop() on columns of table "runs"
+"""
+input runs_stddev_pop_order_by {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: order_by
+
+  """Numeric identifier (May change!)"""
+  id: order_by
+}
+
+"""aggregate stddev_samp on columns"""
+type runs_stddev_samp_fields {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: Float
+
+  """Numeric identifier (May change!)"""
+  id: Float
+}
+
+"""
+order by stddev_samp() on columns of table "runs"
+"""
+input runs_stddev_samp_order_by {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: order_by
+
+  """Numeric identifier (May change!)"""
+  id: order_by
+}
+
+"""aggregate sum on columns"""
+type runs_sum_fields {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: Int
+
+  """Numeric identifier (May change!)"""
+  id: Int
+}
+
+"""
+order by sum() on columns of table "runs"
+"""
+input runs_sum_order_by {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: order_by
+
+  """Numeric identifier (May change!)"""
+  id: order_by
+}
+
+"""aggregate var_pop on columns"""
+type runs_var_pop_fields {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: Float
+
+  """Numeric identifier (May change!)"""
+  id: Float
+}
+
+"""
+order by var_pop() on columns of table "runs"
+"""
+input runs_var_pop_order_by {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: order_by
+
+  """Numeric identifier (May change!)"""
+  id: order_by
+}
+
+"""aggregate var_samp on columns"""
+type runs_var_samp_fields {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: Float
+
+  """Numeric identifier (May change!)"""
+  id: Float
+}
+
+"""
+order by var_samp() on columns of table "runs"
+"""
+input runs_var_samp_order_by {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: order_by
+
+  """Numeric identifier (May change!)"""
+  id: order_by
+}
+
+"""aggregate variance on columns"""
+type runs_variance_fields {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: Float
+
+  """Numeric identifier (May change!)"""
+  id: Float
+}
+
+"""
+order by variance() on columns of table "runs"
+"""
+input runs_variance_order_by {
+  """Reference to the dataset this run is a part of"""
+  dataset_id: order_by
+
+  """Numeric identifier (May change!)"""
+  id: order_by
+}
+
+"""Tilt Series Metadata"""
+type tiltseries {
+  """Electron Microscope Accelerator voltage in volts"""
+  acceleration_voltage: Int!
+
+  """Describes the binning factor from frames to tilt series file"""
+  binning_from_frames: numeric!
+
+  """Name of the camera manufacturer"""
+  camera_manufacturer: String!
+
+  """Camera model name"""
+  camera_model: String!
+
+  """Software used to collect data"""
+  data_acquisition_software: String!
+  https_alignment_file: String!
+  https_angle_list: String!
+  https_collection_metadata: String
+  https_mrc_bin1: String!
+  https_mrc_bin2: String!
+  https_mrc_bin4: String!
+  https_omezarr_dir: String!
+  id: Int!
+
+  """
+  Other microscope optical setup information, in addition to energy filter, phase plate and image corrector
+  """
+  microscope_additional_info: String
+
+  """Energy filter setup used"""
+  microscope_energy_filter: String!
+
+  """Image corrector setup"""
+  microscope_image_corrector: String
+
+  """Name of the microscope manufacturer"""
+  microscope_manufacturer: String!
+
+  """Microscope model name"""
+  microscope_model: String!
+
+  """Phase plate configuration"""
+  microscope_phase_plate: String
+
+  """
+  If a tilt series is deposited into EMPIAR, enter the EMPIAR dataset identifier
+  """
+  related_empiar_entry: String
+
+  """An object relationship"""
+  run: runs!
+  run_id: Int!
+  s3_alignment_file: String!
+  s3_angle_list: String!
+  s3_collection_metadata: String
+  s3_mrc_bin1: String!
+  s3_mrc_bin2: String!
+  s3_mrc_bin4: String!
+  s3_omezarr_dir: String!
+
+  """Spherical Aberration Constant of the objective lens in millimeters"""
+  spherical_aberration_constant: numeric!
+
+  """Rotation angle in degrees"""
+  tilt_axis: numeric!
+
+  """Maximal tilt angle in degrees"""
+  tilt_max: numeric!
+
+  """Minimal tilt angle in degrees"""
+  tilt_min: numeric!
+
+  """The difference between tilt_min and tilt_max"""
+  tilt_range: numeric!
+
+  """
+  Author assessment of tilt series quality within the dataset (1-5, 5 is best)
+  """
+  tilt_series_quality: Int!
+  tilt_step: numeric!
+
+  """The order of stage tilting during acquisition of the data"""
+  tilting_scheme: String!
+
+  """
+  Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
+  """
+  total_flux: numeric!
+}
+
+"""
+aggregated selection of "tiltseries"
+"""
+type tiltseries_aggregate {
+  aggregate: tiltseries_aggregate_fields
+  nodes: [tiltseries!]!
+}
+
+input tiltseries_aggregate_bool_exp {
+  count: tiltseries_aggregate_bool_exp_count
+}
+
+input tiltseries_aggregate_bool_exp_count {
+  arguments: [tiltseries_select_column!]
+  distinct: Boolean
+  filter: tiltseries_bool_exp
+  predicate: Int_comparison_exp!
+}
+
+"""
+aggregate fields of "tiltseries"
+"""
+type tiltseries_aggregate_fields {
+  avg: tiltseries_avg_fields
+  count(columns: [tiltseries_select_column!], distinct: Boolean): Int!
+  max: tiltseries_max_fields
+  min: tiltseries_min_fields
+  stddev: tiltseries_stddev_fields
+  stddev_pop: tiltseries_stddev_pop_fields
+  stddev_samp: tiltseries_stddev_samp_fields
+  sum: tiltseries_sum_fields
+  var_pop: tiltseries_var_pop_fields
+  var_samp: tiltseries_var_samp_fields
+  variance: tiltseries_variance_fields
+}
+
+"""
+order by aggregate values of table "tiltseries"
+"""
+input tiltseries_aggregate_order_by {
+  avg: tiltseries_avg_order_by
+  count: order_by
+  max: tiltseries_max_order_by
+  min: tiltseries_min_order_by
+  stddev: tiltseries_stddev_order_by
+  stddev_pop: tiltseries_stddev_pop_order_by
+  stddev_samp: tiltseries_stddev_samp_order_by
+  sum: tiltseries_sum_order_by
+  var_pop: tiltseries_var_pop_order_by
+  var_samp: tiltseries_var_samp_order_by
+  variance: tiltseries_variance_order_by
+}
+
+"""aggregate avg on columns"""
+type tiltseries_avg_fields {
+  """Electron Microscope Accelerator voltage in volts"""
+  acceleration_voltage: Float
+
+  """Describes the binning factor from frames to tilt series file"""
+  binning_from_frames: Float
+  id: Float
+  run_id: Float
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: Float
 
   """Rotation angle in degrees"""
   tilt_axis: Float
 
   """Maximal tilt angle in degrees"""
   tilt_max: Float
 
   """Minimal tilt angle in degrees"""
   tilt_min: Float
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: Float
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: Float
-
-  """Tilt step in degrees"""
   tilt_step: Float
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: Float
 }
 
 """
-order by avg() on columns of table "runs"
+order by avg() on columns of table "tiltseries"
 """
-input runs_avg_order_by {
+input tiltseries_avg_order_by {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: order_by
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: order_by
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: order_by
-
-  """Numeric identifier (May change!)"""
   id: order_by
+  run_id: order_by
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: order_by
 
   """Rotation angle in degrees"""
   tilt_axis: order_by
 
   """Maximal tilt angle in degrees"""
   tilt_max: order_by
 
   """Minimal tilt angle in degrees"""
   tilt_min: order_by
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: order_by
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: order_by
-
-  """Tilt step in degrees"""
   tilt_step: order_by
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: order_by
 }
 
 """
-Boolean expression to filter rows from the table "runs". All fields are combined with a logical 'AND'.
+Boolean expression to filter rows from the table "tiltseries". All fields are combined with a logical 'AND'.
 """
-input runs_bool_exp {
-  _and: [runs_bool_exp!]
-  _not: runs_bool_exp
-  _or: [runs_bool_exp!]
+input tiltseries_bool_exp {
+  _and: [tiltseries_bool_exp!]
+  _not: tiltseries_bool_exp
+  _or: [tiltseries_bool_exp!]
   acceleration_voltage: Int_comparison_exp
-  annotations: annotations_bool_exp
-  annotations_aggregate: annotations_aggregate_bool_exp
   binning_from_frames: numeric_comparison_exp
   camera_manufacturer: String_comparison_exp
   camera_model: String_comparison_exp
   data_acquisition_software: String_comparison_exp
-  dataset: datasets_bool_exp
-  dataset_id: Int_comparison_exp
-  https_prefix: String_comparison_exp
+  https_alignment_file: String_comparison_exp
+  https_angle_list: String_comparison_exp
+  https_collection_metadata: String_comparison_exp
+  https_mrc_bin1: String_comparison_exp
+  https_mrc_bin2: String_comparison_exp
+  https_mrc_bin4: String_comparison_exp
+  https_omezarr_dir: String_comparison_exp
   id: Int_comparison_exp
   microscope_additional_info: String_comparison_exp
   microscope_energy_filter: String_comparison_exp
   microscope_image_corrector: String_comparison_exp
   microscope_manufacturer: String_comparison_exp
   microscope_model: String_comparison_exp
   microscope_phase_plate: String_comparison_exp
-  name: String_comparison_exp
   related_empiar_entry: String_comparison_exp
-  s3_prefix: String_comparison_exp
+  run: runs_bool_exp
+  run_id: Int_comparison_exp
+  s3_alignment_file: String_comparison_exp
+  s3_angle_list: String_comparison_exp
+  s3_collection_metadata: String_comparison_exp
+  s3_mrc_bin1: String_comparison_exp
+  s3_mrc_bin2: String_comparison_exp
+  s3_mrc_bin4: String_comparison_exp
+  s3_omezarr_dir: String_comparison_exp
   spherical_aberration_constant: numeric_comparison_exp
   tilt_axis: numeric_comparison_exp
   tilt_max: numeric_comparison_exp
   tilt_min: numeric_comparison_exp
   tilt_range: numeric_comparison_exp
   tilt_series_quality: Int_comparison_exp
   tilt_step: numeric_comparison_exp
   tilting_scheme: String_comparison_exp
-  tiltseries: tiltseries_bool_exp
-  tiltseries_aggregate: tiltseries_aggregate_bool_exp
-  tomograms: tomograms_bool_exp
-  tomograms_aggregate: tomograms_aggregate_bool_exp
   total_flux: numeric_comparison_exp
 }
 
 """aggregate max on columns"""
-type runs_max_fields {
+type tiltseries_max_fields {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: Int
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: numeric
 
   """Name of the camera manufacturer"""
   camera_manufacturer: String
 
   """Camera model name"""
   camera_model: String
 
   """Software used to collect data"""
   data_acquisition_software: String
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: Int
-
-  """The https directory path where this dataset is contained"""
-  https_prefix: String
-
-  """Numeric identifier (May change!)"""
+  https_alignment_file: String
+  https_angle_list: String
+  https_collection_metadata: String
+  https_mrc_bin1: String
+  https_mrc_bin2: String
+  https_mrc_bin4: String
+  https_omezarr_dir: String
   id: Int
 
   """
   Other microscope optical setup information, in addition to energy filter, phase plate and image corrector
   """
   microscope_additional_info: String
 
@@ -4045,81 +4348,82 @@
 
   """Microscope model name"""
   microscope_model: String
 
   """Phase plate configuration"""
   microscope_phase_plate: String
 
-  """Short name for the tilt series"""
-  name: String
-
   """
   If a tilt series is deposited into EMPIAR, enter the EMPIAR dataset identifier
   """
   related_empiar_entry: String
-
-  """The S3 public bucket path where this dataset is contained"""
-  s3_prefix: String
+  run_id: Int
+  s3_alignment_file: String
+  s3_angle_list: String
+  s3_collection_metadata: String
+  s3_mrc_bin1: String
+  s3_mrc_bin2: String
+  s3_mrc_bin4: String
+  s3_omezarr_dir: String
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: numeric
 
   """Rotation angle in degrees"""
   tilt_axis: numeric
 
   """Maximal tilt angle in degrees"""
   tilt_max: numeric
 
   """Minimal tilt angle in degrees"""
   tilt_min: numeric
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: numeric
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: Int
-
-  """Tilt step in degrees"""
   tilt_step: numeric
 
   """The order of stage tilting during acquisition of the data"""
   tilting_scheme: String
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: numeric
 }
 
 """
-order by max() on columns of table "runs"
+order by max() on columns of table "tiltseries"
 """
-input runs_max_order_by {
+input tiltseries_max_order_by {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: order_by
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: order_by
 
   """Name of the camera manufacturer"""
   camera_manufacturer: order_by
 
   """Camera model name"""
   camera_model: order_by
 
   """Software used to collect data"""
   data_acquisition_software: order_by
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: order_by
-
-  """The https directory path where this dataset is contained"""
-  https_prefix: order_by
-
-  """Numeric identifier (May change!)"""
+  https_alignment_file: order_by
+  https_angle_list: order_by
+  https_collection_metadata: order_by
+  https_mrc_bin1: order_by
+  https_mrc_bin2: order_by
+  https_mrc_bin4: order_by
+  https_omezarr_dir: order_by
   id: order_by
 
   """
   Other microscope optical setup information, in addition to energy filter, phase plate and image corrector
   """
   microscope_additional_info: order_by
 
@@ -4134,79 +4438,80 @@
 
   """Microscope model name"""
   microscope_model: order_by
 
   """Phase plate configuration"""
   microscope_phase_plate: order_by
 
-  """Short name for the tilt series"""
-  name: order_by
-
   """
   If a tilt series is deposited into EMPIAR, enter the EMPIAR dataset identifier
   """
   related_empiar_entry: order_by
-
-  """The S3 public bucket path where this dataset is contained"""
-  s3_prefix: order_by
+  run_id: order_by
+  s3_alignment_file: order_by
+  s3_angle_list: order_by
+  s3_collection_metadata: order_by
+  s3_mrc_bin1: order_by
+  s3_mrc_bin2: order_by
+  s3_mrc_bin4: order_by
+  s3_omezarr_dir: order_by
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: order_by
 
   """Rotation angle in degrees"""
   tilt_axis: order_by
 
   """Maximal tilt angle in degrees"""
   tilt_max: order_by
 
   """Minimal tilt angle in degrees"""
   tilt_min: order_by
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: order_by
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: order_by
-
-  """Tilt step in degrees"""
   tilt_step: order_by
 
   """The order of stage tilting during acquisition of the data"""
   tilting_scheme: order_by
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: order_by
 }
 
 """aggregate min on columns"""
-type runs_min_fields {
+type tiltseries_min_fields {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: Int
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: numeric
 
   """Name of the camera manufacturer"""
   camera_manufacturer: String
 
   """Camera model name"""
   camera_model: String
 
   """Software used to collect data"""
   data_acquisition_software: String
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: Int
-
-  """The https directory path where this dataset is contained"""
-  https_prefix: String
-
-  """Numeric identifier (May change!)"""
+  https_alignment_file: String
+  https_angle_list: String
+  https_collection_metadata: String
+  https_mrc_bin1: String
+  https_mrc_bin2: String
+  https_mrc_bin4: String
+  https_omezarr_dir: String
   id: Int
 
   """
   Other microscope optical setup information, in addition to energy filter, phase plate and image corrector
   """
   microscope_additional_info: String
 
@@ -4221,81 +4526,82 @@
 
   """Microscope model name"""
   microscope_model: String
 
   """Phase plate configuration"""
   microscope_phase_plate: String
 
-  """Short name for the tilt series"""
-  name: String
-
   """
   If a tilt series is deposited into EMPIAR, enter the EMPIAR dataset identifier
   """
   related_empiar_entry: String
-
-  """The S3 public bucket path where this dataset is contained"""
-  s3_prefix: String
+  run_id: Int
+  s3_alignment_file: String
+  s3_angle_list: String
+  s3_collection_metadata: String
+  s3_mrc_bin1: String
+  s3_mrc_bin2: String
+  s3_mrc_bin4: String
+  s3_omezarr_dir: String
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: numeric
 
   """Rotation angle in degrees"""
   tilt_axis: numeric
 
   """Maximal tilt angle in degrees"""
   tilt_max: numeric
 
   """Minimal tilt angle in degrees"""
   tilt_min: numeric
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: numeric
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: Int
-
-  """Tilt step in degrees"""
   tilt_step: numeric
 
   """The order of stage tilting during acquisition of the data"""
   tilting_scheme: String
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: numeric
 }
 
 """
-order by min() on columns of table "runs"
+order by min() on columns of table "tiltseries"
 """
-input runs_min_order_by {
+input tiltseries_min_order_by {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: order_by
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: order_by
 
   """Name of the camera manufacturer"""
   camera_manufacturer: order_by
 
   """Camera model name"""
   camera_model: order_by
 
   """Software used to collect data"""
   data_acquisition_software: order_by
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: order_by
-
-  """The https directory path where this dataset is contained"""
-  https_prefix: order_by
-
-  """Numeric identifier (May change!)"""
+  https_alignment_file: order_by
+  https_angle_list: order_by
+  https_collection_metadata: order_by
+  https_mrc_bin1: order_by
+  https_mrc_bin2: order_by
+  https_mrc_bin4: order_by
+  https_omezarr_dir: order_by
   id: order_by
 
   """
   Other microscope optical setup information, in addition to energy filter, phase plate and image corrector
   """
   microscope_additional_info: order_by
 
@@ -4310,93 +4616,103 @@
 
   """Microscope model name"""
   microscope_model: order_by
 
   """Phase plate configuration"""
   microscope_phase_plate: order_by
 
-  """Short name for the tilt series"""
-  name: order_by
-
   """
   If a tilt series is deposited into EMPIAR, enter the EMPIAR dataset identifier
   """
   related_empiar_entry: order_by
-
-  """The S3 public bucket path where this dataset is contained"""
-  s3_prefix: order_by
+  run_id: order_by
+  s3_alignment_file: order_by
+  s3_angle_list: order_by
+  s3_collection_metadata: order_by
+  s3_mrc_bin1: order_by
+  s3_mrc_bin2: order_by
+  s3_mrc_bin4: order_by
+  s3_omezarr_dir: order_by
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: order_by
 
   """Rotation angle in degrees"""
   tilt_axis: order_by
 
   """Maximal tilt angle in degrees"""
   tilt_max: order_by
 
   """Minimal tilt angle in degrees"""
   tilt_min: order_by
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: order_by
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: order_by
-
-  """Tilt step in degrees"""
   tilt_step: order_by
 
   """The order of stage tilting during acquisition of the data"""
   tilting_scheme: order_by
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: order_by
 }
 
-"""Ordering options when selecting data from "runs"."""
-input runs_order_by {
+"""Ordering options when selecting data from "tiltseries"."""
+input tiltseries_order_by {
   acceleration_voltage: order_by
-  annotations_aggregate: annotations_aggregate_order_by
   binning_from_frames: order_by
   camera_manufacturer: order_by
   camera_model: order_by
   data_acquisition_software: order_by
-  dataset: datasets_order_by
-  dataset_id: order_by
-  https_prefix: order_by
+  https_alignment_file: order_by
+  https_angle_list: order_by
+  https_collection_metadata: order_by
+  https_mrc_bin1: order_by
+  https_mrc_bin2: order_by
+  https_mrc_bin4: order_by
+  https_omezarr_dir: order_by
   id: order_by
   microscope_additional_info: order_by
   microscope_energy_filter: order_by
   microscope_image_corrector: order_by
   microscope_manufacturer: order_by
   microscope_model: order_by
   microscope_phase_plate: order_by
-  name: order_by
   related_empiar_entry: order_by
-  s3_prefix: order_by
+  run: runs_order_by
+  run_id: order_by
+  s3_alignment_file: order_by
+  s3_angle_list: order_by
+  s3_collection_metadata: order_by
+  s3_mrc_bin1: order_by
+  s3_mrc_bin2: order_by
+  s3_mrc_bin4: order_by
+  s3_omezarr_dir: order_by
   spherical_aberration_constant: order_by
   tilt_axis: order_by
   tilt_max: order_by
   tilt_min: order_by
   tilt_range: order_by
   tilt_series_quality: order_by
   tilt_step: order_by
   tilting_scheme: order_by
-  tiltseries_aggregate: tiltseries_aggregate_order_by
-  tomograms_aggregate: tomograms_aggregate_order_by
   total_flux: order_by
 }
 
 """
-select columns of table "runs"
+select columns of table "tiltseries"
 """
-enum runs_select_column {
+enum tiltseries_select_column {
   """column name"""
   acceleration_voltage
 
   """column name"""
   binning_from_frames
 
   """column name"""
@@ -4405,18 +4721,33 @@
   """column name"""
   camera_model
 
   """column name"""
   data_acquisition_software
 
   """column name"""
-  dataset_id
+  https_alignment_file
 
   """column name"""
-  https_prefix
+  https_angle_list
+
+  """column name"""
+  https_collection_metadata
+
+  """column name"""
+  https_mrc_bin1
+
+  """column name"""
+  https_mrc_bin2
+
+  """column name"""
+  https_mrc_bin4
+
+  """column name"""
+  https_omezarr_dir
 
   """column name"""
   id
 
   """column name"""
   microscope_additional_info
 
@@ -4432,21 +4763,39 @@
   """column name"""
   microscope_model
 
   """column name"""
   microscope_phase_plate
 
   """column name"""
-  name
+  related_empiar_entry
 
   """column name"""
-  related_empiar_entry
+  run_id
 
   """column name"""
-  s3_prefix
+  s3_alignment_file
+
+  """column name"""
+  s3_angle_list
+
+  """column name"""
+  s3_collection_metadata
+
+  """column name"""
+  s3_mrc_bin1
+
+  """column name"""
+  s3_mrc_bin2
+
+  """column name"""
+  s3_mrc_bin4
+
+  """column name"""
+  s3_omezarr_dir
 
   """column name"""
   spherical_aberration_constant
 
   """column name"""
   tilt_axis
 
@@ -4469,650 +4818,547 @@
   tilting_scheme
 
   """column name"""
   total_flux
 }
 
 """aggregate stddev on columns"""
-type runs_stddev_fields {
+type tiltseries_stddev_fields {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: Float
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: Float
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: Float
-
-  """Numeric identifier (May change!)"""
   id: Float
+  run_id: Float
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: Float
 
   """Rotation angle in degrees"""
   tilt_axis: Float
 
   """Maximal tilt angle in degrees"""
   tilt_max: Float
 
   """Minimal tilt angle in degrees"""
   tilt_min: Float
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: Float
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: Float
-
-  """Tilt step in degrees"""
   tilt_step: Float
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: Float
 }
 
 """
-order by stddev() on columns of table "runs"
+order by stddev() on columns of table "tiltseries"
 """
-input runs_stddev_order_by {
+input tiltseries_stddev_order_by {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: order_by
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: order_by
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: order_by
-
-  """Numeric identifier (May change!)"""
   id: order_by
+  run_id: order_by
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: order_by
 
   """Rotation angle in degrees"""
   tilt_axis: order_by
 
   """Maximal tilt angle in degrees"""
   tilt_max: order_by
 
   """Minimal tilt angle in degrees"""
   tilt_min: order_by
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: order_by
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: order_by
-
-  """Tilt step in degrees"""
   tilt_step: order_by
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: order_by
 }
 
 """aggregate stddev_pop on columns"""
-type runs_stddev_pop_fields {
+type tiltseries_stddev_pop_fields {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: Float
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: Float
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: Float
-
-  """Numeric identifier (May change!)"""
   id: Float
+  run_id: Float
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: Float
 
   """Rotation angle in degrees"""
   tilt_axis: Float
 
   """Maximal tilt angle in degrees"""
   tilt_max: Float
 
   """Minimal tilt angle in degrees"""
   tilt_min: Float
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: Float
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: Float
-
-  """Tilt step in degrees"""
   tilt_step: Float
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: Float
 }
 
 """
-order by stddev_pop() on columns of table "runs"
+order by stddev_pop() on columns of table "tiltseries"
 """
-input runs_stddev_pop_order_by {
+input tiltseries_stddev_pop_order_by {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: order_by
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: order_by
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: order_by
-
-  """Numeric identifier (May change!)"""
   id: order_by
+  run_id: order_by
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: order_by
 
   """Rotation angle in degrees"""
   tilt_axis: order_by
 
   """Maximal tilt angle in degrees"""
   tilt_max: order_by
 
   """Minimal tilt angle in degrees"""
   tilt_min: order_by
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: order_by
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: order_by
-
-  """Tilt step in degrees"""
   tilt_step: order_by
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: order_by
 }
 
 """aggregate stddev_samp on columns"""
-type runs_stddev_samp_fields {
+type tiltseries_stddev_samp_fields {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: Float
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: Float
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: Float
-
-  """Numeric identifier (May change!)"""
   id: Float
+  run_id: Float
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: Float
 
   """Rotation angle in degrees"""
   tilt_axis: Float
 
   """Maximal tilt angle in degrees"""
   tilt_max: Float
 
   """Minimal tilt angle in degrees"""
   tilt_min: Float
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: Float
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: Float
-
-  """Tilt step in degrees"""
   tilt_step: Float
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: Float
 }
 
 """
-order by stddev_samp() on columns of table "runs"
+order by stddev_samp() on columns of table "tiltseries"
 """
-input runs_stddev_samp_order_by {
+input tiltseries_stddev_samp_order_by {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: order_by
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: order_by
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: order_by
-
-  """Numeric identifier (May change!)"""
   id: order_by
+  run_id: order_by
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: order_by
 
   """Rotation angle in degrees"""
   tilt_axis: order_by
 
   """Maximal tilt angle in degrees"""
   tilt_max: order_by
 
   """Minimal tilt angle in degrees"""
   tilt_min: order_by
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: order_by
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: order_by
-
-  """Tilt step in degrees"""
   tilt_step: order_by
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: order_by
 }
 
 """aggregate sum on columns"""
-type runs_sum_fields {
+type tiltseries_sum_fields {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: Int
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: numeric
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: Int
-
-  """Numeric identifier (May change!)"""
   id: Int
+  run_id: Int
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: numeric
 
   """Rotation angle in degrees"""
   tilt_axis: numeric
 
   """Maximal tilt angle in degrees"""
   tilt_max: numeric
 
   """Minimal tilt angle in degrees"""
   tilt_min: numeric
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: numeric
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: Int
-
-  """Tilt step in degrees"""
   tilt_step: numeric
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: numeric
 }
 
 """
-order by sum() on columns of table "runs"
+order by sum() on columns of table "tiltseries"
 """
-input runs_sum_order_by {
+input tiltseries_sum_order_by {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: order_by
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: order_by
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: order_by
-
-  """Numeric identifier (May change!)"""
   id: order_by
+  run_id: order_by
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: order_by
 
   """Rotation angle in degrees"""
   tilt_axis: order_by
 
   """Maximal tilt angle in degrees"""
   tilt_max: order_by
 
   """Minimal tilt angle in degrees"""
   tilt_min: order_by
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: order_by
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: order_by
-
-  """Tilt step in degrees"""
   tilt_step: order_by
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: order_by
 }
 
 """aggregate var_pop on columns"""
-type runs_var_pop_fields {
+type tiltseries_var_pop_fields {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: Float
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: Float
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: Float
-
-  """Numeric identifier (May change!)"""
   id: Float
+  run_id: Float
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: Float
 
   """Rotation angle in degrees"""
   tilt_axis: Float
 
   """Maximal tilt angle in degrees"""
   tilt_max: Float
 
   """Minimal tilt angle in degrees"""
   tilt_min: Float
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: Float
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: Float
-
-  """Tilt step in degrees"""
   tilt_step: Float
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: Float
 }
 
 """
-order by var_pop() on columns of table "runs"
+order by var_pop() on columns of table "tiltseries"
 """
-input runs_var_pop_order_by {
+input tiltseries_var_pop_order_by {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: order_by
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: order_by
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: order_by
-
-  """Numeric identifier (May change!)"""
   id: order_by
+  run_id: order_by
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: order_by
 
   """Rotation angle in degrees"""
   tilt_axis: order_by
 
   """Maximal tilt angle in degrees"""
   tilt_max: order_by
 
   """Minimal tilt angle in degrees"""
   tilt_min: order_by
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: order_by
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: order_by
-
-  """Tilt step in degrees"""
   tilt_step: order_by
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: order_by
 }
 
 """aggregate var_samp on columns"""
-type runs_var_samp_fields {
+type tiltseries_var_samp_fields {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: Float
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: Float
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: Float
-
-  """Numeric identifier (May change!)"""
   id: Float
+  run_id: Float
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: Float
 
   """Rotation angle in degrees"""
   tilt_axis: Float
 
   """Maximal tilt angle in degrees"""
   tilt_max: Float
 
   """Minimal tilt angle in degrees"""
   tilt_min: Float
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: Float
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: Float
-
-  """Tilt step in degrees"""
   tilt_step: Float
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: Float
 }
 
 """
-order by var_samp() on columns of table "runs"
+order by var_samp() on columns of table "tiltseries"
 """
-input runs_var_samp_order_by {
+input tiltseries_var_samp_order_by {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: order_by
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: order_by
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: order_by
-
-  """Numeric identifier (May change!)"""
   id: order_by
+  run_id: order_by
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: order_by
 
   """Rotation angle in degrees"""
   tilt_axis: order_by
 
   """Maximal tilt angle in degrees"""
   tilt_max: order_by
 
   """Minimal tilt angle in degrees"""
   tilt_min: order_by
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: order_by
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: order_by
-
-  """Tilt step in degrees"""
   tilt_step: order_by
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: order_by
 }
 
 """aggregate variance on columns"""
-type runs_variance_fields {
+type tiltseries_variance_fields {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: Float
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: Float
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: Float
-
-  """Numeric identifier (May change!)"""
   id: Float
+  run_id: Float
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: Float
 
   """Rotation angle in degrees"""
   tilt_axis: Float
 
   """Maximal tilt angle in degrees"""
   tilt_max: Float
 
   """Minimal tilt angle in degrees"""
   tilt_min: Float
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: Float
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: Float
-
-  """Tilt step in degrees"""
   tilt_step: Float
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: Float
 }
 
 """
-order by variance() on columns of table "runs"
+order by variance() on columns of table "tiltseries"
 """
-input runs_variance_order_by {
+input tiltseries_variance_order_by {
   """Electron Microscope Accelerator voltage in volts"""
   acceleration_voltage: order_by
 
   """Describes the binning factor from frames to tilt series file"""
   binning_from_frames: order_by
-
-  """Reference to the dataset this run is a part of"""
-  dataset_id: order_by
-
-  """Numeric identifier (May change!)"""
   id: order_by
+  run_id: order_by
 
   """Spherical Aberration Constant of the objective lens in millimeters"""
   spherical_aberration_constant: order_by
 
   """Rotation angle in degrees"""
   tilt_axis: order_by
 
   """Maximal tilt angle in degrees"""
   tilt_max: order_by
 
   """Minimal tilt angle in degrees"""
   tilt_min: order_by
+
+  """The difference between tilt_min and tilt_max"""
   tilt_range: order_by
 
   """
   Author assessment of tilt series quality within the dataset (1-5, 5 is best)
   """
   tilt_series_quality: order_by
-
-  """Tilt step in degrees"""
   tilt_step: order_by
 
   """
   Number of Electrons reaching the specimen in a square Angstrom area for the entire tilt series
   """
   total_flux: order_by
 }
 
-type subscription_root {
-  """
-  fetch data from the table: "annotation_authors"
-  """
-  annotation_authors(
-    """distinct select on columns"""
-    distinct_on: [annotation_authors_select_column!]
-
-    """limit the number of rows returned"""
-    limit: Int
-
-    """skip the first n rows. Use only with order_by"""
-    offset: Int
-
-    """sort the rows by one or more columns"""
-    order_by: [annotation_authors_order_by!]
-
-    """filter the rows returned"""
-    where: annotation_authors_bool_exp
-  ): [annotation_authors!]!
-
-  """
-  fetch aggregated fields from the table: "annotation_authors"
-  """
-  annotation_authors_aggregate(
-    """distinct select on columns"""
-    distinct_on: [annotation_authors_select_column!]
-
-    """limit the number of rows returned"""
-    limit: Int
-
-    """skip the first n rows. Use only with order_by"""
-    offset: Int
-
-    """sort the rows by one or more columns"""
-    order_by: [annotation_authors_order_by!]
-
-    """filter the rows returned"""
-    where: annotation_authors_bool_exp
-  ): annotation_authors_aggregate!
-
-  """
-  fetch data from the table: "annotation_authors" using primary key columns
-  """
-  annotation_authors_by_pk(
-    """Numeric identifier for this annotation author (this may change!)"""
-    id: Int!
-  ): annotation_authors
-
+"""The tomograms for each run are grouped by their voxel spacing"""
+type tomogram_voxel_spacings {
   """An array relationship"""
   annotations(
     """distinct select on columns"""
     distinct_on: [annotations_select_column!]
 
     """limit the number of rows returned"""
     limit: Int
@@ -5140,235 +5386,21 @@
 
     """sort the rows by one or more columns"""
     order_by: [annotations_order_by!]
 
     """filter the rows returned"""
     where: annotations_bool_exp
   ): annotations_aggregate!
+  https_prefix: String
+  id: Int!
 
-  """fetch data from the table: "annotations" using primary key columns"""
-  annotations_by_pk(
-    """Numeric identifier (May change!)"""
-    id: Int!
-  ): annotations
-
-  """
-  fetch data from the table: "dataset_authors"
-  """
-  dataset_authors(
-    """distinct select on columns"""
-    distinct_on: [dataset_authors_select_column!]
-
-    """limit the number of rows returned"""
-    limit: Int
-
-    """skip the first n rows. Use only with order_by"""
-    offset: Int
-
-    """sort the rows by one or more columns"""
-    order_by: [dataset_authors_order_by!]
-
-    """filter the rows returned"""
-    where: dataset_authors_bool_exp
-  ): [dataset_authors!]!
-
-  """
-  fetch aggregated fields from the table: "dataset_authors"
-  """
-  dataset_authors_aggregate(
-    """distinct select on columns"""
-    distinct_on: [dataset_authors_select_column!]
-
-    """limit the number of rows returned"""
-    limit: Int
-
-    """skip the first n rows. Use only with order_by"""
-    offset: Int
-
-    """sort the rows by one or more columns"""
-    order_by: [dataset_authors_order_by!]
-
-    """filter the rows returned"""
-    where: dataset_authors_bool_exp
-  ): dataset_authors_aggregate!
-
-  """fetch data from the table: "dataset_authors" using primary key columns"""
-  dataset_authors_by_pk(id: Int!): dataset_authors
-
-  """
-  fetch data from the table: "dataset_funding"
-  """
-  dataset_funding(
-    """distinct select on columns"""
-    distinct_on: [dataset_funding_select_column!]
-
-    """limit the number of rows returned"""
-    limit: Int
-
-    """skip the first n rows. Use only with order_by"""
-    offset: Int
-
-    """sort the rows by one or more columns"""
-    order_by: [dataset_funding_order_by!]
-
-    """filter the rows returned"""
-    where: dataset_funding_bool_exp
-  ): [dataset_funding!]!
-
-  """
-  fetch aggregated fields from the table: "dataset_funding"
-  """
-  dataset_funding_aggregate(
-    """distinct select on columns"""
-    distinct_on: [dataset_funding_select_column!]
-
-    """limit the number of rows returned"""
-    limit: Int
-
-    """skip the first n rows. Use only with order_by"""
-    offset: Int
-
-    """sort the rows by one or more columns"""
-    order_by: [dataset_funding_order_by!]
-
-    """filter the rows returned"""
-    where: dataset_funding_bool_exp
-  ): dataset_funding_aggregate!
-
-  """fetch data from the table: "dataset_funding" using primary key columns"""
-  dataset_funding_by_pk(id: Int!): dataset_funding
-
-  """
-  fetch data from the table: "datasets"
-  """
-  datasets(
-    """distinct select on columns"""
-    distinct_on: [datasets_select_column!]
-
-    """limit the number of rows returned"""
-    limit: Int
-
-    """skip the first n rows. Use only with order_by"""
-    offset: Int
-
-    """sort the rows by one or more columns"""
-    order_by: [datasets_order_by!]
-
-    """filter the rows returned"""
-    where: datasets_bool_exp
-  ): [datasets!]!
-
-  """
-  fetch aggregated fields from the table: "datasets"
-  """
-  datasets_aggregate(
-    """distinct select on columns"""
-    distinct_on: [datasets_select_column!]
-
-    """limit the number of rows returned"""
-    limit: Int
-
-    """skip the first n rows. Use only with order_by"""
-    offset: Int
-
-    """sort the rows by one or more columns"""
-    order_by: [datasets_order_by!]
-
-    """filter the rows returned"""
-    where: datasets_bool_exp
-  ): datasets_aggregate!
-
-  """fetch data from the table: "datasets" using primary key columns"""
-  datasets_by_pk(
-    """
-    An identifier for a CryoET dataset, assigned by the Data Portal. Used to identify the dataset as the directory name in data tree
-    """
-    id: Int!
-  ): datasets
-
-  """An array relationship"""
-  runs(
-    """distinct select on columns"""
-    distinct_on: [runs_select_column!]
-
-    """limit the number of rows returned"""
-    limit: Int
-
-    """skip the first n rows. Use only with order_by"""
-    offset: Int
-
-    """sort the rows by one or more columns"""
-    order_by: [runs_order_by!]
-
-    """filter the rows returned"""
-    where: runs_bool_exp
-  ): [runs!]!
-
-  """An aggregate relationship"""
-  runs_aggregate(
-    """distinct select on columns"""
-    distinct_on: [runs_select_column!]
-
-    """limit the number of rows returned"""
-    limit: Int
-
-    """skip the first n rows. Use only with order_by"""
-    offset: Int
-
-    """sort the rows by one or more columns"""
-    order_by: [runs_order_by!]
-
-    """filter the rows returned"""
-    where: runs_bool_exp
-  ): runs_aggregate!
-
-  """fetch data from the table: "runs" using primary key columns"""
-  runs_by_pk(
-    """Numeric identifier (May change!)"""
-    id: Int!
-  ): runs
-
-  """An array relationship"""
-  tiltseries(
-    """distinct select on columns"""
-    distinct_on: [tiltseries_select_column!]
-
-    """limit the number of rows returned"""
-    limit: Int
-
-    """skip the first n rows. Use only with order_by"""
-    offset: Int
-
-    """sort the rows by one or more columns"""
-    order_by: [tiltseries_order_by!]
-
-    """filter the rows returned"""
-    where: tiltseries_bool_exp
-  ): [tiltseries!]!
-
-  """An aggregate relationship"""
-  tiltseries_aggregate(
-    """distinct select on columns"""
-    distinct_on: [tiltseries_select_column!]
-
-    """limit the number of rows returned"""
-    limit: Int
-
-    """skip the first n rows. Use only with order_by"""
-    offset: Int
-
-    """sort the rows by one or more columns"""
-    order_by: [tiltseries_order_by!]
-
-    """filter the rows returned"""
-    where: tiltseries_bool_exp
-  ): tiltseries_aggregate!
-
-  """fetch data from the table: "tiltseries" using primary key columns"""
-  tiltseries_by_pk(id: Int!): tiltseries
+  """An object relationship"""
+  run: runs!
+  run_id: Int!
+  s3_prefix: String
 
   """An array relationship"""
   tomograms(
     """distinct select on columns"""
     distinct_on: [tomograms_select_column!]
 
     """limit the number of rows returned"""
@@ -5397,404 +5429,293 @@
 
     """sort the rows by one or more columns"""
     order_by: [tomograms_order_by!]
 
     """filter the rows returned"""
     where: tomograms_bool_exp
   ): tomograms_aggregate!
-
-  """fetch data from the table: "tomograms" using primary key columns"""
-  tomograms_by_pk(
-    """Numeric identifier for this tomogram (this may change!)"""
-    id: Int!
-  ): tomograms
-}
-
-"""Tilt Series Metadata"""
-type tiltseries {
-  https_alignment_file: String!
-  https_angle_list: String!
-  https_collection_metadata: String
-  https_mrc_bin1: String!
-  https_mrc_bin2: String!
-  https_mrc_bin4: String!
-  https_omezarr_dir: String!
-  id: Int!
-
-  """An object relationship"""
-  run: runs!
-  run_id: Int!
-  s3_alignment_file: String!
-  s3_angle_list: String!
-  s3_collection_metadata: String
-  s3_mrc_bin1: String!
-  s3_mrc_bin2: String!
-  s3_mrc_bin4: String!
-  s3_omezarr_dir: String!
+  voxel_spacing: numeric!
 }
 
 """
-aggregated selection of "tiltseries"
+aggregated selection of "tomogram_voxel_spacings"
 """
-type tiltseries_aggregate {
-  aggregate: tiltseries_aggregate_fields
-  nodes: [tiltseries!]!
+type tomogram_voxel_spacings_aggregate {
+  aggregate: tomogram_voxel_spacings_aggregate_fields
+  nodes: [tomogram_voxel_spacings!]!
 }
 
-input tiltseries_aggregate_bool_exp {
-  count: tiltseries_aggregate_bool_exp_count
+input tomogram_voxel_spacings_aggregate_bool_exp {
+  count: tomogram_voxel_spacings_aggregate_bool_exp_count
 }
 
-input tiltseries_aggregate_bool_exp_count {
-  arguments: [tiltseries_select_column!]
+input tomogram_voxel_spacings_aggregate_bool_exp_count {
+  arguments: [tomogram_voxel_spacings_select_column!]
   distinct: Boolean
-  filter: tiltseries_bool_exp
+  filter: tomogram_voxel_spacings_bool_exp
   predicate: Int_comparison_exp!
 }
 
 """
-aggregate fields of "tiltseries"
+aggregate fields of "tomogram_voxel_spacings"
 """
-type tiltseries_aggregate_fields {
-  avg: tiltseries_avg_fields
-  count(columns: [tiltseries_select_column!], distinct: Boolean): Int!
-  max: tiltseries_max_fields
-  min: tiltseries_min_fields
-  stddev: tiltseries_stddev_fields
-  stddev_pop: tiltseries_stddev_pop_fields
-  stddev_samp: tiltseries_stddev_samp_fields
-  sum: tiltseries_sum_fields
-  var_pop: tiltseries_var_pop_fields
-  var_samp: tiltseries_var_samp_fields
-  variance: tiltseries_variance_fields
+type tomogram_voxel_spacings_aggregate_fields {
+  avg: tomogram_voxel_spacings_avg_fields
+  count(columns: [tomogram_voxel_spacings_select_column!], distinct: Boolean): Int!
+  max: tomogram_voxel_spacings_max_fields
+  min: tomogram_voxel_spacings_min_fields
+  stddev: tomogram_voxel_spacings_stddev_fields
+  stddev_pop: tomogram_voxel_spacings_stddev_pop_fields
+  stddev_samp: tomogram_voxel_spacings_stddev_samp_fields
+  sum: tomogram_voxel_spacings_sum_fields
+  var_pop: tomogram_voxel_spacings_var_pop_fields
+  var_samp: tomogram_voxel_spacings_var_samp_fields
+  variance: tomogram_voxel_spacings_variance_fields
 }
 
 """
-order by aggregate values of table "tiltseries"
+order by aggregate values of table "tomogram_voxel_spacings"
 """
-input tiltseries_aggregate_order_by {
-  avg: tiltseries_avg_order_by
+input tomogram_voxel_spacings_aggregate_order_by {
+  avg: tomogram_voxel_spacings_avg_order_by
   count: order_by
-  max: tiltseries_max_order_by
-  min: tiltseries_min_order_by
-  stddev: tiltseries_stddev_order_by
-  stddev_pop: tiltseries_stddev_pop_order_by
-  stddev_samp: tiltseries_stddev_samp_order_by
-  sum: tiltseries_sum_order_by
-  var_pop: tiltseries_var_pop_order_by
-  var_samp: tiltseries_var_samp_order_by
-  variance: tiltseries_variance_order_by
+  max: tomogram_voxel_spacings_max_order_by
+  min: tomogram_voxel_spacings_min_order_by
+  stddev: tomogram_voxel_spacings_stddev_order_by
+  stddev_pop: tomogram_voxel_spacings_stddev_pop_order_by
+  stddev_samp: tomogram_voxel_spacings_stddev_samp_order_by
+  sum: tomogram_voxel_spacings_sum_order_by
+  var_pop: tomogram_voxel_spacings_var_pop_order_by
+  var_samp: tomogram_voxel_spacings_var_samp_order_by
+  variance: tomogram_voxel_spacings_variance_order_by
 }
 
 """aggregate avg on columns"""
-type tiltseries_avg_fields {
+type tomogram_voxel_spacings_avg_fields {
   id: Float
   run_id: Float
+  voxel_spacing: Float
 }
 
 """
-order by avg() on columns of table "tiltseries"
+order by avg() on columns of table "tomogram_voxel_spacings"
 """
-input tiltseries_avg_order_by {
+input tomogram_voxel_spacings_avg_order_by {
   id: order_by
   run_id: order_by
+  voxel_spacing: order_by
 }
 
 """
-Boolean expression to filter rows from the table "tiltseries". All fields are combined with a logical 'AND'.
+Boolean expression to filter rows from the table "tomogram_voxel_spacings". All fields are combined with a logical 'AND'.
 """
-input tiltseries_bool_exp {
-  _and: [tiltseries_bool_exp!]
-  _not: tiltseries_bool_exp
-  _or: [tiltseries_bool_exp!]
-  https_alignment_file: String_comparison_exp
-  https_angle_list: String_comparison_exp
-  https_collection_metadata: String_comparison_exp
-  https_mrc_bin1: String_comparison_exp
-  https_mrc_bin2: String_comparison_exp
-  https_mrc_bin4: String_comparison_exp
-  https_omezarr_dir: String_comparison_exp
+input tomogram_voxel_spacings_bool_exp {
+  _and: [tomogram_voxel_spacings_bool_exp!]
+  _not: tomogram_voxel_spacings_bool_exp
+  _or: [tomogram_voxel_spacings_bool_exp!]
+  annotations: annotations_bool_exp
+  annotations_aggregate: annotations_aggregate_bool_exp
+  https_prefix: String_comparison_exp
   id: Int_comparison_exp
   run: runs_bool_exp
   run_id: Int_comparison_exp
-  s3_alignment_file: String_comparison_exp
-  s3_angle_list: String_comparison_exp
-  s3_collection_metadata: String_comparison_exp
-  s3_mrc_bin1: String_comparison_exp
-  s3_mrc_bin2: String_comparison_exp
-  s3_mrc_bin4: String_comparison_exp
-  s3_omezarr_dir: String_comparison_exp
+  s3_prefix: String_comparison_exp
+  tomograms: tomograms_bool_exp
+  tomograms_aggregate: tomograms_aggregate_bool_exp
+  voxel_spacing: numeric_comparison_exp
 }
 
 """aggregate max on columns"""
-type tiltseries_max_fields {
-  https_alignment_file: String
-  https_angle_list: String
-  https_collection_metadata: String
-  https_mrc_bin1: String
-  https_mrc_bin2: String
-  https_mrc_bin4: String
-  https_omezarr_dir: String
+type tomogram_voxel_spacings_max_fields {
+  https_prefix: String
   id: Int
   run_id: Int
-  s3_alignment_file: String
-  s3_angle_list: String
-  s3_collection_metadata: String
-  s3_mrc_bin1: String
-  s3_mrc_bin2: String
-  s3_mrc_bin4: String
-  s3_omezarr_dir: String
+  s3_prefix: String
+  voxel_spacing: numeric
 }
 
 """
-order by max() on columns of table "tiltseries"
+order by max() on columns of table "tomogram_voxel_spacings"
 """
-input tiltseries_max_order_by {
-  https_alignment_file: order_by
-  https_angle_list: order_by
-  https_collection_metadata: order_by
-  https_mrc_bin1: order_by
-  https_mrc_bin2: order_by
-  https_mrc_bin4: order_by
-  https_omezarr_dir: order_by
+input tomogram_voxel_spacings_max_order_by {
+  https_prefix: order_by
   id: order_by
   run_id: order_by
-  s3_alignment_file: order_by
-  s3_angle_list: order_by
-  s3_collection_metadata: order_by
-  s3_mrc_bin1: order_by
-  s3_mrc_bin2: order_by
-  s3_mrc_bin4: order_by
-  s3_omezarr_dir: order_by
+  s3_prefix: order_by
+  voxel_spacing: order_by
 }
 
 """aggregate min on columns"""
-type tiltseries_min_fields {
-  https_alignment_file: String
-  https_angle_list: String
-  https_collection_metadata: String
-  https_mrc_bin1: String
-  https_mrc_bin2: String
-  https_mrc_bin4: String
-  https_omezarr_dir: String
+type tomogram_voxel_spacings_min_fields {
+  https_prefix: String
   id: Int
   run_id: Int
-  s3_alignment_file: String
-  s3_angle_list: String
-  s3_collection_metadata: String
-  s3_mrc_bin1: String
-  s3_mrc_bin2: String
-  s3_mrc_bin4: String
-  s3_omezarr_dir: String
+  s3_prefix: String
+  voxel_spacing: numeric
 }
 
 """
-order by min() on columns of table "tiltseries"
+order by min() on columns of table "tomogram_voxel_spacings"
 """
-input tiltseries_min_order_by {
-  https_alignment_file: order_by
-  https_angle_list: order_by
-  https_collection_metadata: order_by
-  https_mrc_bin1: order_by
-  https_mrc_bin2: order_by
-  https_mrc_bin4: order_by
-  https_omezarr_dir: order_by
+input tomogram_voxel_spacings_min_order_by {
+  https_prefix: order_by
   id: order_by
   run_id: order_by
-  s3_alignment_file: order_by
-  s3_angle_list: order_by
-  s3_collection_metadata: order_by
-  s3_mrc_bin1: order_by
-  s3_mrc_bin2: order_by
-  s3_mrc_bin4: order_by
-  s3_omezarr_dir: order_by
+  s3_prefix: order_by
+  voxel_spacing: order_by
 }
 
-"""Ordering options when selecting data from "tiltseries"."""
-input tiltseries_order_by {
-  https_alignment_file: order_by
-  https_angle_list: order_by
-  https_collection_metadata: order_by
-  https_mrc_bin1: order_by
-  https_mrc_bin2: order_by
-  https_mrc_bin4: order_by
-  https_omezarr_dir: order_by
+"""Ordering options when selecting data from "tomogram_voxel_spacings"."""
+input tomogram_voxel_spacings_order_by {
+  annotations_aggregate: annotations_aggregate_order_by
+  https_prefix: order_by
   id: order_by
   run: runs_order_by
   run_id: order_by
-  s3_alignment_file: order_by
-  s3_angle_list: order_by
-  s3_collection_metadata: order_by
-  s3_mrc_bin1: order_by
-  s3_mrc_bin2: order_by
-  s3_mrc_bin4: order_by
-  s3_omezarr_dir: order_by
+  s3_prefix: order_by
+  tomograms_aggregate: tomograms_aggregate_order_by
+  voxel_spacing: order_by
 }
 
 """
-select columns of table "tiltseries"
+select columns of table "tomogram_voxel_spacings"
 """
-enum tiltseries_select_column {
-  """column name"""
-  https_alignment_file
-
-  """column name"""
-  https_angle_list
-
-  """column name"""
-  https_collection_metadata
-
+enum tomogram_voxel_spacings_select_column {
   """column name"""
-  https_mrc_bin1
-
-  """column name"""
-  https_mrc_bin2
-
-  """column name"""
-  https_mrc_bin4
-
-  """column name"""
-  https_omezarr_dir
+  https_prefix
 
   """column name"""
   id
 
   """column name"""
   run_id
 
   """column name"""
-  s3_alignment_file
-
-  """column name"""
-  s3_angle_list
-
-  """column name"""
-  s3_collection_metadata
-
-  """column name"""
-  s3_mrc_bin1
-
-  """column name"""
-  s3_mrc_bin2
-
-  """column name"""
-  s3_mrc_bin4
+  s3_prefix
 
   """column name"""
-  s3_omezarr_dir
+  voxel_spacing
 }
 
 """aggregate stddev on columns"""
-type tiltseries_stddev_fields {
+type tomogram_voxel_spacings_stddev_fields {
   id: Float
   run_id: Float
+  voxel_spacing: Float
 }
 
 """
-order by stddev() on columns of table "tiltseries"
+order by stddev() on columns of table "tomogram_voxel_spacings"
 """
-input tiltseries_stddev_order_by {
+input tomogram_voxel_spacings_stddev_order_by {
   id: order_by
   run_id: order_by
+  voxel_spacing: order_by
 }
 
 """aggregate stddev_pop on columns"""
-type tiltseries_stddev_pop_fields {
+type tomogram_voxel_spacings_stddev_pop_fields {
   id: Float
   run_id: Float
+  voxel_spacing: Float
 }
 
 """
-order by stddev_pop() on columns of table "tiltseries"
+order by stddev_pop() on columns of table "tomogram_voxel_spacings"
 """
-input tiltseries_stddev_pop_order_by {
+input tomogram_voxel_spacings_stddev_pop_order_by {
   id: order_by
   run_id: order_by
+  voxel_spacing: order_by
 }
 
 """aggregate stddev_samp on columns"""
-type tiltseries_stddev_samp_fields {
+type tomogram_voxel_spacings_stddev_samp_fields {
   id: Float
   run_id: Float
+  voxel_spacing: Float
 }
 
 """
-order by stddev_samp() on columns of table "tiltseries"
+order by stddev_samp() on columns of table "tomogram_voxel_spacings"
 """
-input tiltseries_stddev_samp_order_by {
+input tomogram_voxel_spacings_stddev_samp_order_by {
   id: order_by
   run_id: order_by
+  voxel_spacing: order_by
 }
 
 """aggregate sum on columns"""
-type tiltseries_sum_fields {
+type tomogram_voxel_spacings_sum_fields {
   id: Int
   run_id: Int
+  voxel_spacing: numeric
 }
 
 """
-order by sum() on columns of table "tiltseries"
+order by sum() on columns of table "tomogram_voxel_spacings"
 """
-input tiltseries_sum_order_by {
+input tomogram_voxel_spacings_sum_order_by {
   id: order_by
   run_id: order_by
+  voxel_spacing: order_by
 }
 
 """aggregate var_pop on columns"""
-type tiltseries_var_pop_fields {
+type tomogram_voxel_spacings_var_pop_fields {
   id: Float
   run_id: Float
+  voxel_spacing: Float
 }
 
 """
-order by var_pop() on columns of table "tiltseries"
+order by var_pop() on columns of table "tomogram_voxel_spacings"
 """
-input tiltseries_var_pop_order_by {
+input tomogram_voxel_spacings_var_pop_order_by {
   id: order_by
   run_id: order_by
+  voxel_spacing: order_by
 }
 
 """aggregate var_samp on columns"""
-type tiltseries_var_samp_fields {
+type tomogram_voxel_spacings_var_samp_fields {
   id: Float
   run_id: Float
+  voxel_spacing: Float
 }
 
 """
-order by var_samp() on columns of table "tiltseries"
+order by var_samp() on columns of table "tomogram_voxel_spacings"
 """
-input tiltseries_var_samp_order_by {
+input tomogram_voxel_spacings_var_samp_order_by {
   id: order_by
   run_id: order_by
+  voxel_spacing: order_by
 }
 
 """aggregate variance on columns"""
-type tiltseries_variance_fields {
+type tomogram_voxel_spacings_variance_fields {
   id: Float
   run_id: Float
+  voxel_spacing: Float
 }
 
 """
-order by variance() on columns of table "tiltseries"
+order by variance() on columns of table "tomogram_voxel_spacings"
 """
-input tiltseries_variance_order_by {
+input tomogram_voxel_spacings_variance_order_by {
   id: order_by
   run_id: order_by
+  voxel_spacing: order_by
 }
 
 """information about the tomograms in the CryoET Data Portal"""
 type tomograms {
   ctf_corrected: Boolean
 
-  """An object relationship"""
-  dataset: datasets!
-
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: Int!
-
   """
   Fiducial Alignment status: True = aligned with fiducial False = aligned without fiducial
   """
   fiducial_alignment_status: String!
 
   """https path to this tomogram in MRC format (no scaling)"""
   https_mrc_scale0: String!
@@ -5827,29 +5748,23 @@
 
   """Describe reconstruction method (Weighted backprojection, SART, SIRT)"""
   reconstruction_method: String!
 
   """Name of software used for reconstruction"""
   reconstruction_software: String!
 
-  """An object relationship"""
-  run: runs!
-
-  """Reference to the run this tomogram is a part of"""
-  run_id: Int!
+  """S3 path to this tomogram in MRC format (no scaling)"""
+  s3_mrc_scale0: String!
 
   """S3 path to this tomogram in MRC format (downscaled to 50%)"""
   s3_mrc_scale1: String!
 
   """S3 path to this tomogram in MRC format (downscaled to 25%)"""
   s3_mrc_scale2: String!
 
-  """S3 path to this tomogram in MRC format (no scaling)"""
-  s3_mrc_scale0: String!
-
   """S3 path to the this multiscale omezarr tomogram"""
   s3_omezarr_dir: String!
 
   """comma separated x,y,z dimensions of the unscaled tomogram"""
   scale0_dimensions: String!
 
   """comma separated x,y,z dimensions of the scale1 tomogram"""
@@ -5870,14 +5785,18 @@
   size_z: Int!
 
   """
   Version of tomogram using the same software and post-processing. Version of tomogram using the same software and post-processing. This will be presented as the latest version
   """
   tomogram_version: String!
 
+  """An object relationship"""
+  tomogram_voxel_spacing: tomogram_voxel_spacings
+  tomogram_voxel_spacing_id: Int
+
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: numeric!
 }
 
 """
 aggregated selection of "tomograms"
 """
@@ -5945,109 +5864,94 @@
   var_pop: tomograms_var_pop_order_by
   var_samp: tomograms_var_samp_order_by
   variance: tomograms_variance_order_by
 }
 
 """aggregate avg on columns"""
 type tomograms_avg_fields {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: Float
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: Float
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: Float
-
   """Number of pixels in the 3D data fast axis"""
   size_x: Float
 
   """Number of pixels in the 3D data medium axis"""
   size_y: Float
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: Float
+  tomogram_voxel_spacing_id: Float
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: Float
 }
 
 """
 order by avg() on columns of table "tomograms"
 """
 input tomograms_avg_order_by {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: order_by
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: order_by
-
   """Number of pixels in the 3D data fast axis"""
   size_x: order_by
 
   """Number of pixels in the 3D data medium axis"""
   size_y: order_by
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: order_by
+  tomogram_voxel_spacing_id: order_by
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """
 Boolean expression to filter rows from the table "tomograms". All fields are combined with a logical 'AND'.
 """
 input tomograms_bool_exp {
   _and: [tomograms_bool_exp!]
   _not: tomograms_bool_exp
   _or: [tomograms_bool_exp!]
   ctf_corrected: Boolean_comparison_exp
-  dataset: datasets_bool_exp
-  dataset_id: Int_comparison_exp
   fiducial_alignment_status: String_comparison_exp
   https_mrc_scale0: String_comparison_exp
   https_mrc_scale1: String_comparison_exp
   https_mrc_scale2: String_comparison_exp
   https_omezarr_dir: String_comparison_exp
   id: Int_comparison_exp
   is_canonical: Boolean_comparison_exp
   name: String_comparison_exp
   processing: String_comparison_exp
   processing_software: String_comparison_exp
   reconstruction_method: String_comparison_exp
   reconstruction_software: String_comparison_exp
-  run: runs_bool_exp
-  run_id: Int_comparison_exp
+  s3_mrc_scale0: String_comparison_exp
   s3_mrc_scale1: String_comparison_exp
   s3_mrc_scale2: String_comparison_exp
-  s3_mrc_scale0: String_comparison_exp
   s3_omezarr_dir: String_comparison_exp
   scale0_dimensions: String_comparison_exp
   scale1_dimensions: String_comparison_exp
   scale2_dimensions: String_comparison_exp
   size_x: Int_comparison_exp
   size_y: Int_comparison_exp
   size_z: Int_comparison_exp
   tomogram_version: String_comparison_exp
+  tomogram_voxel_spacing: tomogram_voxel_spacings_bool_exp
+  tomogram_voxel_spacing_id: Int_comparison_exp
   voxel_spacing: numeric_comparison_exp
 }
 
 """aggregate max on columns"""
 type tomograms_max_fields {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: Int
-
   """
   Fiducial Alignment status: True = aligned with fiducial False = aligned without fiducial
   """
   fiducial_alignment_status: String
 
   """https path to this tomogram in MRC format (no scaling)"""
   https_mrc_scale0: String
@@ -6075,26 +5979,23 @@
 
   """Describe reconstruction method (Weighted backprojection, SART, SIRT)"""
   reconstruction_method: String
 
   """Name of software used for reconstruction"""
   reconstruction_software: String
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: Int
+  """S3 path to this tomogram in MRC format (no scaling)"""
+  s3_mrc_scale0: String
 
   """S3 path to this tomogram in MRC format (downscaled to 50%)"""
   s3_mrc_scale1: String
 
   """S3 path to this tomogram in MRC format (downscaled to 25%)"""
   s3_mrc_scale2: String
 
-  """S3 path to this tomogram in MRC format (no scaling)"""
-  s3_mrc_scale0: String
-
   """S3 path to the this multiscale omezarr tomogram"""
   s3_omezarr_dir: String
 
   """comma separated x,y,z dimensions of the unscaled tomogram"""
   scale0_dimensions: String
 
   """comma separated x,y,z dimensions of the scale1 tomogram"""
@@ -6114,26 +6015,24 @@
   """
   size_z: Int
 
   """
   Version of tomogram using the same software and post-processing. Version of tomogram using the same software and post-processing. This will be presented as the latest version
   """
   tomogram_version: String
+  tomogram_voxel_spacing_id: Int
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: numeric
 }
 
 """
 order by max() on columns of table "tomograms"
 """
 input tomograms_max_order_by {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: order_by
-
   """
   Fiducial Alignment status: True = aligned with fiducial False = aligned without fiducial
   """
   fiducial_alignment_status: order_by
 
   """https path to this tomogram in MRC format (no scaling)"""
   https_mrc_scale0: order_by
@@ -6161,26 +6060,23 @@
 
   """Describe reconstruction method (Weighted backprojection, SART, SIRT)"""
   reconstruction_method: order_by
 
   """Name of software used for reconstruction"""
   reconstruction_software: order_by
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: order_by
+  """S3 path to this tomogram in MRC format (no scaling)"""
+  s3_mrc_scale0: order_by
 
   """S3 path to this tomogram in MRC format (downscaled to 50%)"""
   s3_mrc_scale1: order_by
 
   """S3 path to this tomogram in MRC format (downscaled to 25%)"""
   s3_mrc_scale2: order_by
 
-  """S3 path to this tomogram in MRC format (no scaling)"""
-  s3_mrc_scale0: order_by
-
   """S3 path to the this multiscale omezarr tomogram"""
   s3_omezarr_dir: order_by
 
   """comma separated x,y,z dimensions of the unscaled tomogram"""
   scale0_dimensions: order_by
 
   """comma separated x,y,z dimensions of the scale1 tomogram"""
@@ -6200,24 +6096,22 @@
   """
   size_z: order_by
 
   """
   Version of tomogram using the same software and post-processing. Version of tomogram using the same software and post-processing. This will be presented as the latest version
   """
   tomogram_version: order_by
+  tomogram_voxel_spacing_id: order_by
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """aggregate min on columns"""
 type tomograms_min_fields {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: Int
-
   """
   Fiducial Alignment status: True = aligned with fiducial False = aligned without fiducial
   """
   fiducial_alignment_status: String
 
   """https path to this tomogram in MRC format (no scaling)"""
   https_mrc_scale0: String
@@ -6245,26 +6139,23 @@
 
   """Describe reconstruction method (Weighted backprojection, SART, SIRT)"""
   reconstruction_method: String
 
   """Name of software used for reconstruction"""
   reconstruction_software: String
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: Int
+  """S3 path to this tomogram in MRC format (no scaling)"""
+  s3_mrc_scale0: String
 
   """S3 path to this tomogram in MRC format (downscaled to 50%)"""
   s3_mrc_scale1: String
 
   """S3 path to this tomogram in MRC format (downscaled to 25%)"""
   s3_mrc_scale2: String
 
-  """S3 path to this tomogram in MRC format (no scaling)"""
-  s3_mrc_scale0: String
-
   """S3 path to the this multiscale omezarr tomogram"""
   s3_omezarr_dir: String
 
   """comma separated x,y,z dimensions of the unscaled tomogram"""
   scale0_dimensions: String
 
   """comma separated x,y,z dimensions of the scale1 tomogram"""
@@ -6284,26 +6175,24 @@
   """
   size_z: Int
 
   """
   Version of tomogram using the same software and post-processing. Version of tomogram using the same software and post-processing. This will be presented as the latest version
   """
   tomogram_version: String
+  tomogram_voxel_spacing_id: Int
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: numeric
 }
 
 """
 order by min() on columns of table "tomograms"
 """
 input tomograms_min_order_by {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: order_by
-
   """
   Fiducial Alignment status: True = aligned with fiducial False = aligned without fiducial
   """
   fiducial_alignment_status: order_by
 
   """https path to this tomogram in MRC format (no scaling)"""
   https_mrc_scale0: order_by
@@ -6331,26 +6220,23 @@
 
   """Describe reconstruction method (Weighted backprojection, SART, SIRT)"""
   reconstruction_method: order_by
 
   """Name of software used for reconstruction"""
   reconstruction_software: order_by
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: order_by
+  """S3 path to this tomogram in MRC format (no scaling)"""
+  s3_mrc_scale0: order_by
 
   """S3 path to this tomogram in MRC format (downscaled to 50%)"""
   s3_mrc_scale1: order_by
 
   """S3 path to this tomogram in MRC format (downscaled to 25%)"""
   s3_mrc_scale2: order_by
 
-  """S3 path to this tomogram in MRC format (no scaling)"""
-  s3_mrc_scale0: order_by
-
   """S3 path to the this multiscale omezarr tomogram"""
   s3_omezarr_dir: order_by
 
   """comma separated x,y,z dimensions of the unscaled tomogram"""
   scale0_dimensions: order_by
 
   """comma separated x,y,z dimensions of the scale1 tomogram"""
@@ -6370,63 +6256,59 @@
   """
   size_z: order_by
 
   """
   Version of tomogram using the same software and post-processing. Version of tomogram using the same software and post-processing. This will be presented as the latest version
   """
   tomogram_version: order_by
+  tomogram_voxel_spacing_id: order_by
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """Ordering options when selecting data from "tomograms"."""
 input tomograms_order_by {
   ctf_corrected: order_by
-  dataset: datasets_order_by
-  dataset_id: order_by
   fiducial_alignment_status: order_by
   https_mrc_scale0: order_by
   https_mrc_scale1: order_by
   https_mrc_scale2: order_by
   https_omezarr_dir: order_by
   id: order_by
   is_canonical: order_by
   name: order_by
   processing: order_by
   processing_software: order_by
   reconstruction_method: order_by
   reconstruction_software: order_by
-  run: runs_order_by
-  run_id: order_by
+  s3_mrc_scale0: order_by
   s3_mrc_scale1: order_by
   s3_mrc_scale2: order_by
-  s3_mrc_scale0: order_by
   s3_omezarr_dir: order_by
   scale0_dimensions: order_by
   scale1_dimensions: order_by
   scale2_dimensions: order_by
   size_x: order_by
   size_y: order_by
   size_z: order_by
   tomogram_version: order_by
+  tomogram_voxel_spacing: tomogram_voxel_spacings_order_by
+  tomogram_voxel_spacing_id: order_by
   voxel_spacing: order_by
 }
 
 """
 select columns of table "tomograms"
 """
 enum tomograms_select_column {
   """column name"""
   ctf_corrected
 
   """column name"""
-  dataset_id
-
-  """column name"""
   fiducial_alignment_status
 
   """column name"""
   https_mrc_scale0
 
   """column name"""
   https_mrc_scale1
@@ -6455,26 +6337,23 @@
   """column name"""
   reconstruction_method
 
   """column name"""
   reconstruction_software
 
   """column name"""
-  run_id
+  s3_mrc_scale0
 
   """column name"""
   s3_mrc_scale1
 
   """column name"""
   s3_mrc_scale2
 
   """column name"""
-  s3_mrc_scale0
-
-  """column name"""
   s3_omezarr_dir
 
   """column name"""
   scale0_dimensions
 
   """column name"""
   scale1_dimensions
@@ -6491,14 +6370,17 @@
   """column name"""
   size_z
 
   """column name"""
   tomogram_version
 
   """column name"""
+  tomogram_voxel_spacing_id
+
+  """column name"""
   voxel_spacing
 }
 
 """
 select "tomograms_aggregate_bool_exp_bool_and_arguments_columns" columns of table "tomograms"
 """
 enum tomograms_select_column_tomograms_aggregate_bool_exp_bool_and_arguments_columns {
@@ -6518,383 +6400,313 @@
 
   """column name"""
   is_canonical
 }
 
 """aggregate stddev on columns"""
 type tomograms_stddev_fields {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: Float
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: Float
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: Float
-
   """Number of pixels in the 3D data fast axis"""
   size_x: Float
 
   """Number of pixels in the 3D data medium axis"""
   size_y: Float
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: Float
+  tomogram_voxel_spacing_id: Float
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: Float
 }
 
 """
 order by stddev() on columns of table "tomograms"
 """
 input tomograms_stddev_order_by {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: order_by
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: order_by
-
   """Number of pixels in the 3D data fast axis"""
   size_x: order_by
 
   """Number of pixels in the 3D data medium axis"""
   size_y: order_by
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: order_by
+  tomogram_voxel_spacing_id: order_by
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """aggregate stddev_pop on columns"""
 type tomograms_stddev_pop_fields {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: Float
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: Float
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: Float
-
   """Number of pixels in the 3D data fast axis"""
   size_x: Float
 
   """Number of pixels in the 3D data medium axis"""
   size_y: Float
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: Float
+  tomogram_voxel_spacing_id: Float
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: Float
 }
 
 """
 order by stddev_pop() on columns of table "tomograms"
 """
 input tomograms_stddev_pop_order_by {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: order_by
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: order_by
-
   """Number of pixels in the 3D data fast axis"""
   size_x: order_by
 
   """Number of pixels in the 3D data medium axis"""
   size_y: order_by
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: order_by
+  tomogram_voxel_spacing_id: order_by
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """aggregate stddev_samp on columns"""
 type tomograms_stddev_samp_fields {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: Float
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: Float
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: Float
-
   """Number of pixels in the 3D data fast axis"""
   size_x: Float
 
   """Number of pixels in the 3D data medium axis"""
   size_y: Float
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: Float
+  tomogram_voxel_spacing_id: Float
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: Float
 }
 
 """
 order by stddev_samp() on columns of table "tomograms"
 """
 input tomograms_stddev_samp_order_by {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: order_by
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: order_by
-
   """Number of pixels in the 3D data fast axis"""
   size_x: order_by
 
   """Number of pixels in the 3D data medium axis"""
   size_y: order_by
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: order_by
+  tomogram_voxel_spacing_id: order_by
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """aggregate sum on columns"""
 type tomograms_sum_fields {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: Int
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: Int
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: Int
-
   """Number of pixels in the 3D data fast axis"""
   size_x: Int
 
   """Number of pixels in the 3D data medium axis"""
   size_y: Int
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: Int
+  tomogram_voxel_spacing_id: Int
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: numeric
 }
 
 """
 order by sum() on columns of table "tomograms"
 """
 input tomograms_sum_order_by {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: order_by
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: order_by
-
   """Number of pixels in the 3D data fast axis"""
   size_x: order_by
 
   """Number of pixels in the 3D data medium axis"""
   size_y: order_by
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: order_by
+  tomogram_voxel_spacing_id: order_by
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """aggregate var_pop on columns"""
 type tomograms_var_pop_fields {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: Float
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: Float
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: Float
-
   """Number of pixels in the 3D data fast axis"""
   size_x: Float
 
   """Number of pixels in the 3D data medium axis"""
   size_y: Float
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: Float
+  tomogram_voxel_spacing_id: Float
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: Float
 }
 
 """
 order by var_pop() on columns of table "tomograms"
 """
 input tomograms_var_pop_order_by {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: order_by
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: order_by
-
   """Number of pixels in the 3D data fast axis"""
   size_x: order_by
 
   """Number of pixels in the 3D data medium axis"""
   size_y: order_by
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: order_by
+  tomogram_voxel_spacing_id: order_by
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """aggregate var_samp on columns"""
 type tomograms_var_samp_fields {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: Float
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: Float
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: Float
-
   """Number of pixels in the 3D data fast axis"""
   size_x: Float
 
   """Number of pixels in the 3D data medium axis"""
   size_y: Float
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: Float
+  tomogram_voxel_spacing_id: Float
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: Float
 }
 
 """
 order by var_samp() on columns of table "tomograms"
 """
 input tomograms_var_samp_order_by {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: order_by
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: order_by
-
   """Number of pixels in the 3D data fast axis"""
   size_x: order_by
 
   """Number of pixels in the 3D data medium axis"""
   size_y: order_by
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: order_by
+  tomogram_voxel_spacing_id: order_by
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
 
 """aggregate variance on columns"""
 type tomograms_variance_fields {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: Float
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: Float
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: Float
-
   """Number of pixels in the 3D data fast axis"""
   size_x: Float
 
   """Number of pixels in the 3D data medium axis"""
   size_y: Float
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: Float
+  tomogram_voxel_spacing_id: Float
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: Float
 }
 
 """
 order by variance() on columns of table "tomograms"
 """
 input tomograms_variance_order_by {
-  """Reference to the dataset this tomogram is a part of"""
-  dataset_id: order_by
-
   """Numeric identifier for this tomogram (this may change!)"""
   id: order_by
 
-  """Reference to the run this tomogram is a part of"""
-  run_id: order_by
-
   """Number of pixels in the 3D data fast axis"""
   size_x: order_by
 
   """Number of pixels in the 3D data medium axis"""
   size_y: order_by
 
   """
   Number of pixels in the 3D data slow axis.  This is the image projection direction at zero stage tilt
   """
   size_z: order_by
+  tomogram_voxel_spacing_id: order_by
 
   """Voxel spacing equal in all three axes in angstroms"""
   voxel_spacing: order_by
 }
```

### Comparing `cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/PKG-INFO` & `cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryoet-data-portal
-Version: 0.0.2
+Version: 1.0.0
 Summary: API Client to facilitate the use of the CryoET Portal. For more information about the API and the project visit https://github.com/chanzuckerberg/cryoet-data-portal/
 Author-email: Chan Zuckerberg Initiative <cryoetdataportal@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cryoet-data-portal
 Project-URL: repository, https://github.com/chanzuckerberg/cryoet-data-portal
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cryoet_data_portal-0.0.2/src/cryoet_data_portal.egg-info/SOURCES.txt` & `cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-0.0.2/tests/README.md` & `cryoet_data_portal-1.0.0/tests/README.md`

 * *Files identical despite different names*

