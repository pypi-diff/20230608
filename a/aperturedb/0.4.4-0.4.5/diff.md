# Comparing `tmp/aperturedb-0.4.4.tar.gz` & `tmp/aperturedb-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aperturedb-0.4.4.tar", last modified: Fri May 19 23:51:56 2023, max compression
+gzip compressed data, was "aperturedb-0.4.5.tar", last modified: Thu Jun  8 17:17:12 2023, max compression
```

## Comparing `aperturedb-0.4.4.tar` & `aperturedb-0.4.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:51:56.817841 aperturedb-0.4.4/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-15 16:49:00.000000 aperturedb-0.4.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1957 2023-05-19 23:51:56.817841 aperturedb-0.4.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1442 2023-05-15 16:49:00.000000 aperturedb-0.4.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:51:56.817841 aperturedb-0.4.4/aperturedb/
--rw-r--r--   0 root         (0) root         (0)     4497 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/BBoxDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     2817 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/BlobDataCSV.py
--rw-r--r--   0 root         (0) root         (0)      126 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Blobs.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/BoundingBoxes.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/CSVParser.py
--rw-r--r--   0 root         (0) root         (0)     4764 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/ConnectionDataCSV.py
--rw-r--r--   0 root         (0) root         (0)    13798 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Connector.py
--rw-r--r--   0 root         (0) root         (0)     5664 2023-05-19 19:28:21.000000 aperturedb-0.4.4/aperturedb/ConnectorRest.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Constraints.py
--rw-r--r--   0 root         (0) root         (0)     3366 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/DaskManager.py
--rw-r--r--   0 root         (0) root         (0)     5329 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/DescriptorDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     3316 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/DescriptorSetDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     9263 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Entities.py
--rw-r--r--   0 root         (0) root         (0)     2155 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/EntityDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     7713 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/ImageDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     4834 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/ImageDownloader.py
--rw-r--r--   0 root         (0) root         (0)    21476 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Images.py
--rw-r--r--   0 root         (0) root         (0)     6498 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/KaggleData.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/NotebookHelpers.py
--rw-r--r--   0 root         (0) root         (0)      546 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Operations.py
--rw-r--r--   0 root         (0) root         (0)     4665 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/ParallelLoader.py
--rw-r--r--   0 root         (0) root         (0)    12172 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/ParallelQuery.py
--rw-r--r--   0 root         (0) root         (0)     2261 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Parallelizer.py
--rw-r--r--   0 root         (0) root         (0)     4020 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/PolygonDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     1995 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Polygons.py
--rw-r--r--   0 root         (0) root         (0)     3138 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/ProgressBar.py
--rw-r--r--   0 root         (0) root         (0)     4961 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/PyTorchDataset.py
--rw-r--r--   0 root         (0) root         (0)      917 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/PytorchData.py
--rw-r--r--   0 root         (0) root         (0)     9952 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Query.py
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/QueryGenerator.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/QueryTypes.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Sort.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Stats.py
--rw-r--r--   0 root         (0) root         (0)     1565 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Subscriptable.py
--rw-r--r--   0 root         (0) root         (0)    18835 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Utils.py
--rw-r--r--   0 root         (0) root         (0)     2792 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/VideoDataCSV.py
--rw-r--r--   0 root         (0) root         (0)     3899 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/VideoDownloader.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/Videos.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-05-19 22:38:25.000000 aperturedb-0.4.4/aperturedb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-05-15 16:49:00.000000 aperturedb-0.4.4/aperturedb/queryMessage_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:51:56.817841 aperturedb-0.4.4/aperturedb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1957 2023-05-19 23:51:56.000000 aperturedb-0.4.4/aperturedb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-19 23:51:56.000000 aperturedb-0.4.4/aperturedb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 23:51:56.000000 aperturedb-0.4.4/aperturedb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      201 2023-05-19 23:51:56.000000 aperturedb-0.4.4/aperturedb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-19 23:51:56.000000 aperturedb-0.4.4/aperturedb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 23:51:56.817841 aperturedb-0.4.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1535 2023-05-19 22:38:25.000000 aperturedb-0.4.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:51:56.817841 aperturedb-0.4.4/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5358 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/conftest.py
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/dbinfo.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/download_images.py
--rw-r--r--   0 root         (0) root         (0)    10159 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/generateInput.py
--rw-r--r--   0 root         (0) root         (0)     4897 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_Data.py
--rw-r--r--   0 root         (0) root         (0)     6363 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_Datawizard.py
--rw-r--r--   0 root         (0) root         (0)     5358 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_ResponseHandler.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_Session.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_Stats.py
--rw-r--r--   0 root         (0) root         (0)     1963 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_Success.py
--rw-r--r--   0 root         (0) root         (0)      264 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_Utils.py
--rw-r--r--   0 root         (0) root         (0)     4607 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4292 2023-05-15 16:49:00.000000 aperturedb-0.4.4/test/test_torch_connector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:17:12.930357 aperturedb-0.4.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-15 16:49:00.000000 aperturedb-0.4.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-08 17:17:12.930357 aperturedb-0.4.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-05-15 16:49:00.000000 aperturedb-0.4.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:17:12.930357 aperturedb-0.4.5/aperturedb/
+-rw-r--r--   0 root         (0) root         (0)     4497 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/BBoxDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     2817 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/BlobDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)      126 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/Blobs.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/BoundingBoxes.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/CSVParser.py
+-rw-r--r--   0 root         (0) root         (0)     4764 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/ConnectionDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)    13798 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/Connector.py
+-rw-r--r--   0 root         (0) root         (0)     5664 2023-05-19 19:28:21.000000 aperturedb-0.4.5/aperturedb/ConnectorRest.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/Constraints.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/DaskManager.py
+-rw-r--r--   0 root         (0) root         (0)     5329 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/DescriptorDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     3316 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/DescriptorSetDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     9263 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/Entities.py
+-rw-r--r--   0 root         (0) root         (0)     2155 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/EntityDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     7826 2023-06-07 21:15:39.000000 aperturedb-0.4.5/aperturedb/ImageDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     4834 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/ImageDownloader.py
+-rw-r--r--   0 root         (0) root         (0)    21476 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/Images.py
+-rw-r--r--   0 root         (0) root         (0)     6498 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/KaggleData.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/NotebookHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      546 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/Operations.py
+-rw-r--r--   0 root         (0) root         (0)     4665 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/ParallelLoader.py
+-rw-r--r--   0 root         (0) root         (0)    12172 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/ParallelQuery.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/Parallelizer.py
+-rw-r--r--   0 root         (0) root         (0)     4020 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/PolygonDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/Polygons.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/ProgressBar.py
+-rw-r--r--   0 root         (0) root         (0)     4961 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/PyTorchDataset.py
+-rw-r--r--   0 root         (0) root         (0)      917 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/PytorchData.py
+-rw-r--r--   0 root         (0) root         (0)     9952 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/Query.py
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/QueryGenerator.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/QueryTypes.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/Sort.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/Stats.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/Subscriptable.py
+-rw-r--r--   0 root         (0) root         (0)    18835 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/Utils.py
+-rw-r--r--   0 root         (0) root         (0)     2792 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/VideoDataCSV.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/VideoDownloader.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/Videos.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-06-08 16:51:19.000000 aperturedb-0.4.5/aperturedb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-05-15 16:49:00.000000 aperturedb-0.4.5/aperturedb/queryMessage_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:17:12.930357 aperturedb-0.4.5/aperturedb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-08 17:17:12.000000 aperturedb-0.4.5/aperturedb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-08 17:17:12.000000 aperturedb-0.4.5/aperturedb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 17:17:12.000000 aperturedb-0.4.5/aperturedb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      201 2023-06-08 17:17:12.000000 aperturedb-0.4.5/aperturedb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 17:17:12.000000 aperturedb-0.4.5/aperturedb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 17:17:12.930357 aperturedb-0.4.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-06-08 16:51:19.000000 aperturedb-0.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:17:12.930357 aperturedb-0.4.5/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 16:49:00.000000 aperturedb-0.4.5/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5358 2023-05-15 16:49:00.000000 aperturedb-0.4.5/test/conftest.py
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-15 16:49:00.000000 aperturedb-0.4.5/test/dbinfo.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-15 16:49:00.000000 aperturedb-0.4.5/test/download_images.py
+-rw-r--r--   0 root         (0) root         (0)    10159 2023-05-15 16:49:00.000000 aperturedb-0.4.5/test/generateInput.py
+-rw-r--r--   0 root         (0) root         (0)     4897 2023-05-15 16:49:00.000000 aperturedb-0.4.5/test/test_Data.py
+-rw-r--r--   0 root         (0) root         (0)     6363 2023-05-15 16:49:00.000000 aperturedb-0.4.5/test/test_Datawizard.py
+-rw-r--r--   0 root         (0) root         (0)     5358 2023-05-15 16:49:00.000000 aperturedb-0.4.5/test/test_ResponseHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-05-15 16:49:00.000000 aperturedb-0.4.5/test/test_Session.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-05-15 16:49:00.000000 aperturedb-0.4.5/test/test_Stats.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-05-15 16:49:00.000000 aperturedb-0.4.5/test/test_Success.py
+-rw-r--r--   0 root         (0) root         (0)      264 2023-05-15 16:49:00.000000 aperturedb-0.4.5/test/test_Utils.py
+-rw-r--r--   0 root         (0) root         (0)     4607 2023-05-15 16:49:00.000000 aperturedb-0.4.5/test/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4292 2023-05-15 16:49:00.000000 aperturedb-0.4.5/test/test_torch_connector.py
```

### Comparing `aperturedb-0.4.4/LICENSE` & `aperturedb-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/PKG-INFO` & `aperturedb-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aperturedb
-Version: 0.4.4
+Version: 0.4.5
 Summary: ApertureDB Client Module
 Home-page: https://github.com/aperture-data/aperturedb-python
 Author: Luis Remis
 Author-email: luis@aperturedata.io
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aperturedb-0.4.4/README.md` & `aperturedb-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/BBoxDataCSV.py` & `aperturedb-0.4.5/aperturedb/BBoxDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/BlobDataCSV.py` & `aperturedb-0.4.5/aperturedb/BlobDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/CSVParser.py` & `aperturedb-0.4.5/aperturedb/CSVParser.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/ConnectionDataCSV.py` & `aperturedb-0.4.5/aperturedb/ConnectionDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/Connector.py` & `aperturedb-0.4.5/aperturedb/Connector.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/ConnectorRest.py` & `aperturedb-0.4.5/aperturedb/ConnectorRest.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/Constraints.py` & `aperturedb-0.4.5/aperturedb/Constraints.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/DaskManager.py` & `aperturedb-0.4.5/aperturedb/DaskManager.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/DescriptorDataCSV.py` & `aperturedb-0.4.5/aperturedb/DescriptorDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/DescriptorSetDataCSV.py` & `aperturedb-0.4.5/aperturedb/DescriptorSetDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/Entities.py` & `aperturedb-0.4.5/aperturedb/Entities.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/EntityDataCSV.py` & `aperturedb-0.4.5/aperturedb/EntityDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/ImageDataCSV.py` & `aperturedb-0.4.5/aperturedb/ImageDataCSV.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,20 @@
         self.source_loader    = {
             st: sl for st, sl in zip(self.source_types, self.loaders)
         }
 
         self.n_download_retries = n_download_retries
         self.command = "AddImage"
 
+        self.s3 = None
+        if use_dask == False and self.source_type == HEADER_S3_URL:
+            # The connections by boto3 cause ResourceWarning. Known
+            # issue: https://github.com/boto/boto3/issues/454
+            self.s3 = boto3.client('s3')
+
     def get_indices(self):
         return {
             "entity": {
                 "_Image": self.get_indexed_properties()
             }
         }
 
@@ -175,23 +181,19 @@
                 time.sleep(2)
 
         return False, None
 
     def load_s3_url(self, s3_url):
         retries = 0
 
-        # The connections by boto3 cause ResourceWarning. Known
-        # issue: https://github.com/boto/boto3/issues/454
-        s3 = boto3.client('s3')
-
         while True:
             try:
                 bucket_name = s3_url.split("/")[2]
                 object_name = s3_url.split("s3://" + bucket_name + "/")[-1]
-                s3_response_object = s3.get_object(
+                s3_response_object = self.s3.get_object(
                     Bucket=bucket_name, Key=object_name)
                 img = s3_response_object['Body'].read()
                 imgbuffer = np.frombuffer(img, dtype='uint8')
                 if self.check_image and not self.check_image_buffer(imgbuffer):
                     logger.error("IMAGE ERROR: ", s3_url)
                     return False, None
```

### Comparing `aperturedb-0.4.4/aperturedb/ImageDownloader.py` & `aperturedb-0.4.5/aperturedb/ImageDownloader.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/Images.py` & `aperturedb-0.4.5/aperturedb/Images.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/KaggleData.py` & `aperturedb-0.4.5/aperturedb/KaggleData.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/NotebookHelpers.py` & `aperturedb-0.4.5/aperturedb/NotebookHelpers.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/Operations.py` & `aperturedb-0.4.5/aperturedb/Operations.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/ParallelLoader.py` & `aperturedb-0.4.5/aperturedb/ParallelLoader.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/ParallelQuery.py` & `aperturedb-0.4.5/aperturedb/ParallelQuery.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/Parallelizer.py` & `aperturedb-0.4.5/aperturedb/Parallelizer.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/PolygonDataCSV.py` & `aperturedb-0.4.5/aperturedb/PolygonDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/Polygons.py` & `aperturedb-0.4.5/aperturedb/Polygons.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/ProgressBar.py` & `aperturedb-0.4.5/aperturedb/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/PyTorchDataset.py` & `aperturedb-0.4.5/aperturedb/PyTorchDataset.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/PytorchData.py` & `aperturedb-0.4.5/aperturedb/PytorchData.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/Query.py` & `aperturedb-0.4.5/aperturedb/Query.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/QueryTypes.py` & `aperturedb-0.4.5/aperturedb/QueryTypes.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/Subscriptable.py` & `aperturedb-0.4.5/aperturedb/Subscriptable.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/Utils.py` & `aperturedb-0.4.5/aperturedb/Utils.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/VideoDataCSV.py` & `aperturedb-0.4.5/aperturedb/VideoDataCSV.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/VideoDownloader.py` & `aperturedb-0.4.5/aperturedb/VideoDownloader.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/Videos.py` & `aperturedb-0.4.5/aperturedb/Videos.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb/__init__.py` & `aperturedb-0.4.5/aperturedb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime
 import os
 import json
 import requests
 
 logger = logging.getLogger(__name__)
 
-__version__ = "0.4.4"
+__version__ = "0.4.5"
 
 # set log level
 logger.setLevel(logging.DEBUG)
 formatter    = logging.Formatter(
     "%(asctime)s : %(levelname)s : %(name)s : %(thread)d : %(lineno)d : %(message)s")
 
 log_file_level = logging.getLevelName(os.getenv("LOG_FILE_LEVEL", "WARN"))
```

### Comparing `aperturedb-0.4.4/aperturedb/queryMessage_pb2.py` & `aperturedb-0.4.5/aperturedb/queryMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/aperturedb.egg-info/PKG-INFO` & `aperturedb-0.4.5/aperturedb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aperturedb
-Version: 0.4.4
+Version: 0.4.5
 Summary: ApertureDB Client Module
 Home-page: https://github.com/aperture-data/aperturedb-python
 Author: Luis Remis
 Author-email: luis@aperturedata.io
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aperturedb-0.4.4/aperturedb.egg-info/SOURCES.txt` & `aperturedb-0.4.5/aperturedb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/setup.py` & `aperturedb-0.4.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                     'ipywidgets==8.0.4'
                     ]
 if OPENCV_VERSION is None:
     install_requires.append('opencv-python')
 
 setuptools.setup(
     name="aperturedb",
-    version="0.4.4",
+    version="0.4.5",
     description="ApertureDB Client Module",
     install_requires=install_requires,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aperture-data/aperturedb-python",
     license="Apache",
     packages=setuptools.find_packages(),
```

### Comparing `aperturedb-0.4.4/test/conftest.py` & `aperturedb-0.4.5/test/conftest.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/test/download_images.py` & `aperturedb-0.4.5/test/download_images.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/test/generateInput.py` & `aperturedb-0.4.5/test/generateInput.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/test/test_Data.py` & `aperturedb-0.4.5/test/test_Data.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/test/test_Datawizard.py` & `aperturedb-0.4.5/test/test_Datawizard.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/test/test_ResponseHandler.py` & `aperturedb-0.4.5/test/test_ResponseHandler.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/test/test_Session.py` & `aperturedb-0.4.5/test/test_Session.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/test/test_Stats.py` & `aperturedb-0.4.5/test/test_Stats.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/test/test_Success.py` & `aperturedb-0.4.5/test/test_Success.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/test/test_kaggle.py` & `aperturedb-0.4.5/test/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `aperturedb-0.4.4/test/test_torch_connector.py` & `aperturedb-0.4.5/test/test_torch_connector.py`

 * *Files identical despite different names*

