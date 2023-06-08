# Comparing `tmp/kedro-0.18.8.tar.gz` & `tmp/kedro-0.18.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/circleci/project/dist/.tmp-eup6eyn_/kedro-0.18.8.tar", last modified: Tue May  2 12:17:02 2023, max compression
+gzip compressed data, was "/home/circleci/project/dist/.tmp-j64jwc6c/kedro-0.18.9.tar", last modified: Wed May 31 16:59:14 2023, max compression
```

## Comparing `kedro-0.18.8.tar` & `kedro-0.18.9.tar`

### file list

```diff
@@ -1,250 +1,251 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-05-02 12:12:54.000000 kedro-0.18.8/LICENSE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2023-05-02 12:12:54.000000 kedro-0.18.8/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13118 2023-05-02 12:17:02.000000 kedro-0.18.8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10671 2023-05-02 12:12:54.000000 kedro-0.18.8/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/dependency/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2023-05-02 12:12:54.000000 kedro-0.18.8/dependency/requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      290 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      274 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/__main__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/config/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1079 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/config/abstract_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8959 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/config/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5332 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/config/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13573 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/config/omegaconf_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10683 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/config/templated_config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5233 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/api/api_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/biosequence/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/biosequence/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5543 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/biosequence/biosequence_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/dask/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/dask/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8298 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/dask/parquet_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/email/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/email/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8066 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/email/message_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/geopandas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      237 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/geopandas/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6467 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/geopandas/geojson_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/holoviews/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      226 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/holoviews/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5210 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/holoviews/holoviews_writer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/json/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/json/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6157 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/json/json_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/matplotlib/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/matplotlib/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8926 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/matplotlib/matplotlib_writer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/networkx/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/networkx/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5896 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/networkx/gml_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5929 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/networkx/graphml_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5967 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/networkx/json_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/pandas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1128 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7270 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/csv_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10403 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/excel_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7287 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/feather_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11787 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/gbq_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/generic_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7953 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/hdf_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7139 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/json_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8950 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/parquet_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18006 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/sql_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6622 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pandas/xml_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/pickle/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      219 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pickle/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10690 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pickle/pickle_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/pillow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pillow/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5635 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/pillow/image_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/plotly/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/plotly/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6713 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/plotly/json_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6101 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/plotly/plotly_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/redis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      215 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/redis/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8008 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/redis/redis_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/spark/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/spark/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3945 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/spark/deltatable_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15687 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/spark/spark_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9174 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/spark/spark_hive_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7063 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/spark/spark_jdbc_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/svmlight/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      246 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/svmlight/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5885 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/svmlight/svmlight_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/tensorflow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      207 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/tensorflow/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7536 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/tensorflow/tensorflow_model_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/text/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/text/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5314 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/text/text_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/tracking/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      359 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/tracking/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1696 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/tracking/json_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2593 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/tracking/metrics_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/video/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12182 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/video/video_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/datasets/yaml/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/yaml/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6062 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/datasets/yaml/yaml_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/extensions/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/extensions/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      806 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/extensions/ipython.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/extras/logging/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      328 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/logging/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2508 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/extras/logging/color_logger.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/framework/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/framework/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5713 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/catalog.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7309 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/cli.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/framework/cli/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/hooks/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1617 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/hooks/manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      391 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/hooks/markers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1652 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/hooks/specs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10525 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/jupyter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30232 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/micropkg.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11144 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/pipeline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15085 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1630 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20841 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/starters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16744 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/cli/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/framework/context/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      196 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/context/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12666 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/context/context.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/framework/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/hooks/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3706 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/hooks/manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      344 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/hooks/markers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11098 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/hooks/specs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/framework/project/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15378 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/project/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/project/default_logging.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/framework/session/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/session/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16362 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/session/session.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1371 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/session/shelvestore.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1181 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/session/store.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6546 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/framework/startup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/io/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/io/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4151 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/io/cached_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27408 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/io/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21689 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/io/data_catalog.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3690 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/io/lambda_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4140 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/io/memory_dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23205 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/io/partitioned_dataset.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/ipython/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5615 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/ipython/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1735 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/ipython/logo-32x32.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3527 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/ipython/logo-64x64.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1331 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/ipython/logo-svg.svg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/pipeline/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11661 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/pipeline/modular_pipeline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23303 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/pipeline/node.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33957 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/pipeline/pipeline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/py.typed
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/runner/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      387 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/runner/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14068 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/runner/parallel_runner.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16528 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/runner/runner.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2977 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/runner/sequential_runner.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5950 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/runner/thread_runner.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/cookiecutter.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/parameters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/parameters/{{ cookiecutter.pipeline_name }}.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/nodes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      251 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/pipeline.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/test_pipeline.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/cookiecutter.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      331 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/prompts.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1901 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3965 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1067 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      651 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/logging.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)      300 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/credentials.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6849 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      459 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/index.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
--rw-r--r--   0 circleci  (1001) circleci  (1002)      446 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      332 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1198 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/pipelines/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/pipelines/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1179 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/test_run.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1535 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      423 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1404 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      925 2023-05-02 12:12:54.000000 kedro-0.18.8/kedro/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13118 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8006 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-02 12:16:50.000000 kedro-0.18.8/kedro.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4738 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-02 12:17:02.000000 kedro-0.18.8/kedro.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4050 2023-05-02 12:12:54.000000 kedro-0.18.8/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-02 12:17:02.000000 kedro-0.18.8/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5772 2023-05-02 12:12:54.000000 kedro-0.18.8/setup.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1978 2023-05-02 12:12:54.000000 kedro-0.18.8/test_requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-02 12:17:02.000000 kedro-0.18.8/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      908 2023-05-02 12:12:54.000000 kedro-0.18.8/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-05-31 16:55:25.000000 kedro-0.18.9/LICENSE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2023-05-31 16:55:25.000000 kedro-0.18.9/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13118 2023-05-31 16:59:14.000000 kedro-0.18.9/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10671 2023-05-31 16:55:25.000000 kedro-0.18.9/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/dependency/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2023-05-31 16:55:25.000000 kedro-0.18.9/dependency/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      210 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      274 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/__main__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/config/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1116 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/config/abstract_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8977 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/config/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5356 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/config/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14135 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/config/omegaconf_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10691 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/config/templated_config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5233 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/api/api_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/biosequence/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/biosequence/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5543 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/biosequence/biosequence_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/dask/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/dask/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8298 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/dask/parquet_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/email/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/email/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8066 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/email/message_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/geopandas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      237 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/geopandas/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6467 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/geopandas/geojson_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/holoviews/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      226 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/holoviews/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5210 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/holoviews/holoviews_writer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/json/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/json/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6157 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/json/json_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/matplotlib/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/matplotlib/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8926 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/matplotlib/matplotlib_writer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/networkx/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/networkx/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5896 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/networkx/gml_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5929 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/networkx/graphml_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5967 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/networkx/json_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/pandas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1128 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/pandas/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7270 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/pandas/csv_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10403 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/pandas/excel_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7287 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/pandas/feather_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11787 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/pandas/gbq_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/pandas/generic_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7953 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/pandas/hdf_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7139 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/pandas/json_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8950 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/pandas/parquet_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18006 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/pandas/sql_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6622 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/pandas/xml_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/pickle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      219 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/pickle/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10690 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/pickle/pickle_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/pillow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/pillow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5635 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/pillow/image_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/plotly/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/plotly/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6713 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/plotly/json_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6101 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/plotly/plotly_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/redis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      215 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/redis/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8008 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/redis/redis_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/spark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/spark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3945 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/spark/deltatable_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15687 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/spark/spark_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9174 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/spark/spark_hive_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7063 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/spark/spark_jdbc_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/svmlight/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      246 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/svmlight/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5885 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/svmlight/svmlight_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/tensorflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      207 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/tensorflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7536 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/tensorflow/tensorflow_model_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/text/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/text/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5314 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/text/text_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/tracking/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      359 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/tracking/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1696 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/tracking/json_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2593 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/tracking/metrics_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/video/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12182 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/video/video_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/datasets/yaml/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/yaml/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6062 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/datasets/yaml/yaml_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/extensions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/extensions/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      806 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/extensions/ipython.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/extras/logging/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      328 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/logging/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2508 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/extras/logging/color_logger.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/framework/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/framework/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5713 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/cli/catalog.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7309 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/cli/cli.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/framework/cli/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/cli/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1730 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/cli/hooks/manager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      391 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/cli/hooks/markers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1663 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/cli/hooks/specs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10555 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/cli/jupyter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30232 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/cli/micropkg.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11167 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/cli/pipeline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14809 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/cli/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1630 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/cli/registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20839 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/cli/starters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16742 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/cli/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/framework/context/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      196 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/context/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12563 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/context/context.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/framework/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3944 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/hooks/manager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      344 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/hooks/markers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11371 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/hooks/specs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/framework/project/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14621 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/project/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      363 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/project/default_logging.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/framework/session/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/session/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16197 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/session/session.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1401 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/session/shelvestore.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/session/store.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6546 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/framework/startup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/io/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/io/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4380 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/io/cached_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27392 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/io/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21667 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/io/data_catalog.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3957 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/io/lambda_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4387 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/io/memory_dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23620 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/io/partitioned_dataset.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/ipython/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5626 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/ipython/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1735 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/ipython/logo-32x32.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3527 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/ipython/logo-64x64.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1331 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/ipython/logo-svg.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2401 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/logging.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/pipeline/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11664 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/pipeline/modular_pipeline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23274 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/pipeline/node.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33915 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/pipeline/pipeline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/py.typed
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/runner/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      387 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/runner/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14093 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/runner/parallel_runner.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16546 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/runner/runner.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2977 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/runner/sequential_runner.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5963 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/runner/thread_runner.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/pipeline/cookiecutter.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/parameters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/config/parameters/{{ cookiecutter.pipeline_name }}.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/nodes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      251 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/pipeline.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/pipeline/{{ cookiecutter.pipeline_name }}/tests/test_pipeline.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/cookiecutter.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      331 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/prompts.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1901 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3965 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1067 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      854 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/logging.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      300 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/local/credentials.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6849 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      459 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/index.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      446 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      332 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1198 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/pipelines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/pipelines/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1179 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/test_run.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1535 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      434 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1543 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      925 2023-05-31 16:55:26.000000 kedro-0.18.9/kedro/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13118 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8023 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-31 16:59:03.000000 kedro-0.18.9/kedro.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4130 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-31 16:59:14.000000 kedro-0.18.9/kedro.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4050 2023-05-31 16:55:26.000000 kedro-0.18.9/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-31 16:59:14.000000 kedro-0.18.9/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5328 2023-05-31 16:55:26.000000 kedro-0.18.9/setup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1978 2023-05-31 16:55:26.000000 kedro-0.18.9/test_requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 16:59:14.000000 kedro-0.18.9/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      908 2023-05-31 16:55:26.000000 kedro-0.18.9/tests/test_utils.py
```

### Comparing `kedro-0.18.8/LICENSE.md` & `kedro-0.18.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/PKG-INFO` & `kedro-0.18.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro
-Version: 0.18.8
+Version: 0.18.9
 Summary: Kedro helps you build production-ready data and analytics pipelines
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://kedro.org
 Project-URL: Source, https://github.com/kedro-org/kedro
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro/issues
```

### Comparing `kedro-0.18.8/README.md` & `kedro-0.18.9/README.md`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/dependency/requirements.txt` & `kedro-0.18.9/dependency/requirements.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 anyconfig~=0.10.0
 attrs>=21.3
+build
 cachetools~=5.3
 click<9.0
 cookiecutter>=2.1.1, <3.0
 dynaconf>=3.1.2, <4.0
 fsspec>=2021.4, <2024.1  # Upper bound set arbitrarily, to be reassessed in early 2024
 gitpython~=3.0
 importlib-metadata>=3.6; python_version >= '3.8'
```

### Comparing `kedro-0.18.8/kedro/config/__init__.py` & `kedro-0.18.9/kedro/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/config/abstract_config.py` & `kedro-0.18.9/kedro/config/abstract_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """This module provides ``kedro.abstract_config`` with the baseline
 class model for a `ConfigLoader` implementation.
 """
+from __future__ import annotations
+
 from collections import UserDict
-from typing import Any, Dict
+from typing import Any
 
 
 class AbstractConfigLoader(UserDict):
     """``AbstractConfigLoader`` is the abstract base class
         for all `ConfigLoader` implementations.
     All user-defined `ConfigLoader` implementations should inherit
         from `AbstractConfigLoader` and implement all relevant abstract methods.
     """
 
     def __init__(
         self,
         conf_source: str,
         env: str = None,
-        runtime_params: Dict[str, Any] = None,
-        **kwargs
+        runtime_params: dict[str, Any] = None,
+        **kwargs,
     ):
         super().__init__()
         self.conf_source = conf_source
         self.env = env
-        self.runtime_params = runtime_params
+        self.runtime_params = runtime_params or {}
 
 
 class BadConfigException(Exception):
     """Raised when a configuration file cannot be loaded, for instance
     due to wrong syntax or poor formatting.
     """
```

### Comparing `kedro-0.18.8/kedro/config/common.py` & `kedro-0.18.9/kedro/config/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """This module contains methods and facade interfaces for various ConfigLoader
 implementations.
 """
+from __future__ import annotations
 
 import logging
 from glob import iglob
 from pathlib import Path
-from typing import AbstractSet, Any, Dict, Iterable, List, Set
+from typing import AbstractSet, Any, Iterable
 from warnings import warn
 
 from yaml.parser import ParserError
 
 from kedro.config.abstract_config import BadConfigException, MissingConfigException
 
 SUPPORTED_EXTENSIONS = [
@@ -24,16 +25,16 @@
 _config_logger = logging.getLogger(__name__)
 
 
 def _get_config_from_patterns(
     conf_paths: Iterable[str],
     patterns: Iterable[str] = None,
     ac_template: bool = False,
-    ac_context: Dict[str, Any] = None,
-) -> Dict[str, Any]:
+    ac_context: dict[str, Any] = None,
+) -> dict[str, Any]:
     """Recursively scan for configuration files, load and merge them, and
     return them in the form of a config dictionary.
 
     Args:
         conf_paths: List of configuration paths to directories
         patterns: Glob patterns to match. Files, which names match
             any of the specified patterns, will be processed.
@@ -60,16 +61,16 @@
 
     if not patterns:
         raise ValueError(
             "'patterns' must contain at least one glob "
             "pattern to match config filenames against."
         )
 
-    config: Dict[str, Any] = {}
-    processed_files: Set[Path] = set()
+    config: dict[str, Any] = {}
+    processed_files: set[Path] = set()
 
     for conf_path in conf_paths:
         if not Path(conf_path).is_dir():
             raise ValueError(
                 f"Given configuration path either does not exist "
                 f"or is not a valid directory: {conf_path}"
             )
@@ -100,16 +101,16 @@
             f"No files found in {conf_paths} matching the glob "
             f"pattern(s): {patterns}"
         )
     return config
 
 
 def _load_config_file(
-    config_file: Path, ac_template: bool = False, ac_context: Dict[str, Any] = None
-) -> Dict[str, Any]:
+    config_file: Path, ac_template: bool = False, ac_context: dict[str, Any] = None
+) -> dict[str, Any]:
     """Load an individual config file using `anyconfig` as a backend.
 
     Args:
         config_file: Path to a config file to process.
         ac_template: Boolean flag to indicate whether to use the `ac_template`
             argument of the ``anyconfig.load`` method.
         ac_context: anyconfig context to pass to ``anyconfig.load`` method.
@@ -145,16 +146,16 @@
         cursor = exc.problem_mark.column
         raise ParserError(
             f"Invalid YAML file {config_file}, unable to read line {line}, position {cursor}."
         ) from exc
 
 
 def _load_configs(
-    config_filepaths: List[Path], ac_template: bool, ac_context: Dict[str, Any] = None
-) -> Dict[str, Any]:
+    config_filepaths: list[Path], ac_template: bool, ac_context: dict[str, Any] = None
+) -> dict[str, Any]:
     """Recursively load all configuration files, which satisfy
     a given list of glob patterns from a specific path.
 
     Args:
         config_filepaths: Configuration files sorted in the order of precedence.
         ac_template: Boolean flag to indicate whether to use the `ac_template`
             argument of the ``anyconfig.load`` method. Used in the context of
@@ -169,15 +170,15 @@
 
     Returns:
         Resulting configuration dictionary.
 
     """
 
     aggregate_config = {}
-    seen_file_to_keys: Dict[Path, AbstractSet[str]] = {}
+    seen_file_to_keys: dict[Path, AbstractSet[str]] = {}
 
     for config_filepath in config_filepaths:
         single_config = _load_config_file(
             config_filepath, ac_template=ac_template, ac_context=ac_context
         )
         _check_duplicate_keys(seen_file_to_keys, config_filepath, single_config)
         seen_file_to_keys[config_filepath] = single_config.keys()
@@ -185,17 +186,17 @@
 
     return aggregate_config
 
 
 def _lookup_config_filepaths(
     conf_path: Path,
     patterns: Iterable[str],
-    processed_files: Set[Path],
+    processed_files: set[Path],
     logger: Any,
-) -> List[Path]:
+) -> list[Path]:
     config_files = _path_lookup(conf_path, patterns)
 
     seen_files = config_files & processed_files
     if seen_files:
         logger.warning(
             "Config file(s): %s already processed, skipping loading...",
             ", ".join(str(seen) for seen in sorted(seen_files)),
@@ -203,28 +204,28 @@
         config_files -= seen_files
 
     return sorted(config_files)
 
 
 def _remove_duplicates(items: Iterable[str]):
     """Remove duplicates while preserving the order."""
-    unique_items: List[str] = []
+    unique_items: list[str] = []
     for item in items:
         if item not in unique_items:
             unique_items.append(item)
         else:
             warn(
                 f"Duplicate environment detected! "
                 f"Skipping re-loading from configuration path: {item}"
             )
     return unique_items
 
 
 def _check_duplicate_keys(
-    processed_files: Dict[Path, AbstractSet[str]], filepath: Path, conf: Dict[str, Any]
+    processed_files: dict[Path, AbstractSet[str]], filepath: Path, conf: dict[str, Any]
 ) -> None:
     duplicates = []
 
     for processed_file, keys in processed_files.items():
         overlapping_keys = conf.keys() & keys
 
         if overlapping_keys:
@@ -234,15 +235,15 @@
             duplicates.append(f"{processed_file}: {sorted_keys}")
 
     if duplicates:
         dup_str = "\n- ".join(duplicates)
         raise ValueError(f"Duplicate keys found in {filepath} and:\n- {dup_str}")
 
 
-def _path_lookup(conf_path: Path, patterns: Iterable[str]) -> Set[Path]:
+def _path_lookup(conf_path: Path, patterns: Iterable[str]) -> set[Path]:
     """Return a set of all configuration files from ``conf_path`` or
     its subdirectories, which satisfy a given list of glob patterns.
 
     Args:
         conf_path: Path to configuration directory.
         patterns: List of glob patterns to match the filenames against.
```

### Comparing `kedro-0.18.8/kedro/config/config.py` & `kedro-0.18.9/kedro/config/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """This module provides ``kedro.config`` with the functionality to load one
 or more configuration files from specified paths.
 """
+from __future__ import annotations
+
 from pathlib import Path
-from typing import Any, Dict, Iterable, List
+from typing import Any, Iterable
 
 from kedro.config.abstract_config import AbstractConfigLoader
 from kedro.config.common import _get_config_from_patterns, _remove_duplicates
 
 
 class ConfigLoader(AbstractConfigLoader):
     """Recursively scan directories (config paths) contained in ``conf_source`` for
@@ -64,16 +66,16 @@
 
     """
 
     def __init__(
         self,
         conf_source: str,
         env: str = None,
-        runtime_params: Dict[str, Any] = None,
-        config_patterns: Dict[str, List[str]] = None,
+        runtime_params: dict[str, Any] = None,
+        config_patterns: dict[str, list[str]] = None,
         *,
         base_env: str = "base",
         default_run_env: str = "local",
     ):
         """Instantiates a ``ConfigLoader``.
 
         Args:
@@ -121,15 +123,15 @@
         )
 
     @property
     def conf_paths(self):
         """Property method to return deduplicated configuration paths."""
         return _remove_duplicates(self._build_conf_paths())
 
-    def get(self, *patterns: str) -> Dict[str, Any]:  # type: ignore
+    def get(self, *patterns: str) -> dict[str, Any]:  # type: ignore
         return _get_config_from_patterns(
             conf_paths=self.conf_paths, patterns=list(patterns)
         )
 
     def _build_conf_paths(self) -> Iterable[str]:
         run_env = self.env or self.default_run_env
         return [
```

### Comparing `kedro-0.18.8/kedro/config/omegaconf_config.py` & `kedro-0.18.9/kedro/config/omegaconf_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """This module provides ``kedro.config`` with the functionality to load one
 or more configuration files of yaml or json type from specified paths through OmegaConf.
 """
+from __future__ import annotations
+
 import io
 import logging
 import mimetypes
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Optional, Set  # noqa
+from typing import Any, Iterable
 
 import fsspec
 from omegaconf import OmegaConf
 from omegaconf.resolvers import oc
 from yaml.parser import ParserError
 from yaml.scanner import ScannerError
 
@@ -71,17 +73,17 @@
 
     """
 
     def __init__(
         self,
         conf_source: str,
         env: str = None,
-        runtime_params: Dict[str, Any] = None,
+        runtime_params: dict[str, Any] = None,
         *,
-        config_patterns: Dict[str, List[str]] = None,
+        config_patterns: dict[str, list[str]] = None,
         base_env: str = "base",
         default_run_env: str = "local",
     ):
         """Instantiates a ``OmegaConfigLoader``.
 
         Args:
             conf_source: Path to use as root directory for loading configuration.
@@ -126,15 +128,15 @@
 
         super().__init__(
             conf_source=conf_source,
             env=env,
             runtime_params=runtime_params,
         )
 
-    def __getitem__(self, key) -> Dict[str, Any]:
+    def __getitem__(self, key) -> dict[str, Any]:
         """Get configuration files by key, load and merge them, and
         return them in the form of a config dictionary.
 
         Args:
             key: Key of the configuration type to fetch.
 
         Raises:
@@ -156,71 +158,75 @@
             raise KeyError(
                 f"No config patterns were found for '{key}' in your config loader"
             )
         patterns = [*self.config_patterns[key]]
 
         read_environment_variables = key == "credentials"
 
+        processed_files: set[Path] = set()
         # Load base env config
         if self._protocol == "file":
             base_path = str(Path(self.conf_source) / self.base_env)
         else:
             base_path = str(Path(self._fs.ls("", detail=False)[-1]) / self.base_env)
         base_config = self.load_and_merge_dir_config(
-            base_path, patterns, read_environment_variables
+            base_path, patterns, key, processed_files, read_environment_variables
         )
         config = base_config
 
         # Load chosen env config
         run_env = self.env or self.default_run_env
         if self._protocol == "file":
             env_path = str(Path(self.conf_source) / run_env)
         else:
             env_path = str(Path(self._fs.ls("", detail=False)[-1]) / run_env)
         env_config = self.load_and_merge_dir_config(
-            env_path, patterns, read_environment_variables
+            env_path, patterns, key, processed_files, read_environment_variables
         )
-
         # Destructively merge the two env dirs. The chosen env will override base.
         common_keys = config.keys() & env_config.keys()
         if common_keys:
             sorted_keys = ", ".join(sorted(common_keys))
             msg = (
                 "Config from path '%s' will override the following "
                 "existing top-level config keys: %s"
             )
             _config_logger.debug(msg, env_path, sorted_keys)
 
         config.update(env_config)
 
-        if not config:
+        if not processed_files:
             raise MissingConfigException(
                 f"No files of YAML or JSON format found in {base_path} or {env_path} matching"
                 f" the glob pattern(s): {[*self.config_patterns[key]]}"
             )
         return config
 
     def __repr__(self):  # pragma: no cover
         return (
             f"OmegaConfigLoader(conf_source={self.conf_source}, env={self.env}, "
             f"config_patterns={self.config_patterns})"
         )
 
-    def load_and_merge_dir_config(
+    def load_and_merge_dir_config(  # pylint: disable=too-many-arguments
         self,
         conf_path: str,
         patterns: Iterable[str],
-        read_environment_variables: Optional[bool] = False,
-    ) -> Dict[str, Any]:
+        key: str,
+        processed_files: set,
+        read_environment_variables: bool | None = False,
+    ) -> dict[str, Any]:
         """Recursively load and merge all configuration files in a directory using OmegaConf,
         which satisfy a given list of glob patterns from a specific path.
 
         Args:
             conf_path: Path to configuration directory.
             patterns: List of glob patterns to match the filenames against.
+            key: Key of the configuration type to fetch.
+            processed_files: Set of files read for a given configuration type.
             read_environment_variables: Whether to resolve environment variables.
 
         Raises:
             MissingConfigException: If configuration path doesn't exist or isn't valid.
             ValueError: If two or more configuration files contain the same key(s).
             ParserError: If config file contains invalid YAML or JSON syntax.
 
@@ -250,14 +256,15 @@
         for config_filepath in config_files_filtered:
             try:
                 with self._fs.open(str(config_filepath.as_posix())) as open_config:
                     # As fsspec doesn't allow the file to be read as StringIO,
                     # this is a workaround to read it as a binary file and decode it back to utf8.
                     tmp_fo = io.StringIO(open_config.read().decode("utf8"))
                     config = OmegaConf.load(tmp_fo)
+                    processed_files.add(config_filepath)
                 if read_environment_variables:
                     self._resolve_environment_variables(config)
                 config_per_file[config_filepath] = config
             except (ParserError, ScannerError) as exc:
                 line = exc.problem_mark.line  # type: ignore
                 cursor = exc.problem_mark.column  # type: ignore
                 raise ParserError(
@@ -269,29 +276,33 @@
             file: set(config.keys()) for file, config in config_per_file.items()
         }
         aggregate_config = config_per_file.values()
         self._check_duplicates(seen_file_to_keys)
 
         if not aggregate_config:
             return {}
-        if len(aggregate_config) == 1:
-            return list(aggregate_config)[0]
-        return dict(OmegaConf.merge(*aggregate_config))
+
+        if key == "parameters":
+            # Merge with runtime parameters only for "parameters"
+            return OmegaConf.to_container(
+                OmegaConf.merge(*aggregate_config, self.runtime_params), resolve=True
+            )
+        return OmegaConf.to_container(OmegaConf.merge(*aggregate_config), resolve=True)
 
     def _is_valid_config_path(self, path):
         """Check if given path is a file path and file type is yaml or json."""
         posix_path = path.as_posix()
         return self._fs.isfile(str(posix_path)) and path.suffix in [
             ".yml",
             ".yaml",
             ".json",
         ]
 
     @staticmethod
-    def _check_duplicates(seen_files_to_keys: Dict[Path, Set[Any]]):
+    def _check_duplicates(seen_files_to_keys: dict[Path, set[Any]]):
         duplicates = []
 
         filepaths = list(seen_files_to_keys.keys())
         for i, filepath1 in enumerate(filepaths, 1):
             config1 = seen_files_to_keys[filepath1]
             for filepath2 in filepaths[i:]:
                 config2 = seen_files_to_keys[filepath2]
@@ -307,15 +318,15 @@
                     )
 
         if duplicates:
             dup_str = "\n".join(duplicates)
             raise ValueError(f"{dup_str}")
 
     @staticmethod
-    def _resolve_environment_variables(config: Dict[str, Any]) -> None:
+    def _resolve_environment_variables(config: dict[str, Any]) -> None:
         """Use the ``oc.env`` resolver to read environment variables and replace
         them in-place, clearing the resolver after the operation is complete if
         it was not registered beforehand.
 
         Arguments:
             config {Dict[str, Any]} -- The configuration dictionary to resolve.
         """
```

### Comparing `kedro-0.18.8/kedro/config/templated_config.py` & `kedro-0.18.9/kedro/config/templated_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """This module provides ``kedro.config`` with the functionality to load one
 or more configuration files from specified paths, and format template strings
 with the values from the passed dictionary.
 """
+from __future__ import annotations
+
 import re
 from copy import deepcopy
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Optional
+from typing import Any, Iterable
 
 import jmespath
 
 from kedro.config.abstract_config import AbstractConfigLoader
 from kedro.config.common import _get_config_from_patterns, _remove_duplicates
 
 IDENTIFIER_PATTERN = re.compile(
@@ -87,21 +89,21 @@
     https://github.com/jmespath/jmespath.py and https://jmespath.org/.
     """
 
     def __init__(
         self,
         conf_source: str,
         env: str = None,
-        runtime_params: Dict[str, Any] = None,
-        config_patterns: Dict[str, List[str]] = None,
+        runtime_params: dict[str, Any] = None,
+        config_patterns: dict[str, list[str]] = None,
         *,
         base_env: str = "base",
         default_run_env: str = "local",
-        globals_pattern: Optional[str] = None,
-        globals_dict: Optional[Dict[str, Any]] = None,
+        globals_pattern: str | None = None,
+        globals_dict: dict[str, Any] | None = None,
     ):
         """Instantiates a ``TemplatedConfigLoader``.
 
         Args:
             conf_source: Path to use as root directory for loading configuration.
             env: Environment that will take precedence over base.
             runtime_params: Extra parameters passed to a Kedro run.
@@ -158,15 +160,15 @@
         )
 
     @property
     def conf_paths(self):
         """Property method to return deduplicated configuration paths."""
         return _remove_duplicates(self._build_conf_paths())
 
-    def get(self, *patterns: str) -> Dict[str, Any]:  # type: ignore
+    def get(self, *patterns: str) -> dict[str, Any]:  # type: ignore
         """Tries to resolve the template variables in the config dictionary
         provided by the ``ConfigLoader`` (super class) ``get`` method using the
         dictionary of replacement values obtained in the ``__init__`` method.
 
         Args:
             *patterns: Glob patterns to match. Files, which names match
                 any of the specified patterns, will be processed.
@@ -190,15 +192,15 @@
         run_env = self.env or self.default_run_env
         return [
             str(Path(self.conf_source) / self.base_env),
             str(Path(self.conf_source) / run_env),
         ]
 
 
-def _format_object(val: Any, format_dict: Dict[str, Any]) -> Any:
+def _format_object(val: Any, format_dict: dict[str, Any]) -> Any:
     """Recursive function that loops through the values of a map. In case another
     map or a list is encountered, it calls itself. When a string is encountered,
     it will use the `format_dict` to replace strings that look like `${expr}`,
     where `expr` is a JMESPath expression evaluated against `format_dict`.
 
     Some notes on behavior:
         * If val is not a dict, list or string, the same value gets passed back.
```

### Comparing `kedro-0.18.8/kedro/extras/datasets/__init__.py` & `kedro-0.18.9/kedro/extras/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/api/api_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/api/api_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/biosequence/biosequence_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/biosequence/biosequence_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/dask/parquet_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/dask/parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/email/message_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/email/message_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/geopandas/geojson_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/geopandas/geojson_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/holoviews/holoviews_writer.py` & `kedro-0.18.9/kedro/extras/datasets/holoviews/holoviews_writer.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/json/json_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/json/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/matplotlib/matplotlib_writer.py` & `kedro-0.18.9/kedro/extras/datasets/matplotlib/matplotlib_writer.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/networkx/gml_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/networkx/gml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/networkx/graphml_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/networkx/graphml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/networkx/json_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/networkx/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/pandas/__init__.py` & `kedro-0.18.9/kedro/extras/datasets/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/pandas/csv_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/pandas/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/pandas/excel_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/pandas/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/pandas/feather_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/pandas/feather_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/pandas/gbq_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/pandas/gbq_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/pandas/generic_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/pandas/generic_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/pandas/hdf_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/pandas/hdf_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/pandas/json_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/pandas/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/pandas/parquet_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/pandas/parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/pandas/sql_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/pandas/sql_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/pandas/xml_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/pandas/xml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/pickle/pickle_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/pickle/pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/pillow/image_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/pillow/image_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/plotly/json_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/plotly/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/plotly/plotly_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/plotly/plotly_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/redis/redis_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/redis/redis_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/spark/deltatable_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/spark/deltatable_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/spark/spark_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/spark/spark_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/spark/spark_hive_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/spark/spark_hive_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/spark/spark_jdbc_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/spark/spark_jdbc_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/svmlight/svmlight_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/svmlight/svmlight_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/tensorflow/tensorflow_model_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/tensorflow/tensorflow_model_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/text/text_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/text/text_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/tracking/json_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/tracking/json_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/tracking/metrics_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/tracking/metrics_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/video/video_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/video/video_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/datasets/yaml/yaml_dataset.py` & `kedro-0.18.9/kedro/extras/datasets/yaml/yaml_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/extensions/ipython.py` & `kedro-0.18.9/kedro/extras/extensions/ipython.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/extras/logging/color_logger.py` & `kedro-0.18.9/kedro/extras/logging/color_logger.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/framework/cli/catalog.py` & `kedro-0.18.9/kedro/framework/cli/catalog.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/framework/cli/cli.py` & `kedro-0.18.9/kedro/framework/cli/cli.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/framework/cli/hooks/manager.py` & `kedro-0.18.9/kedro/framework/cli/hooks/manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 import logging
 
 from pluggy import PluginManager
 
 from .markers import CLI_HOOK_NAMESPACE
 from .specs import CLICommandSpecs
 
+logger = logging.getLogger(__name__)
+
 _cli_hook_manager = None
 
 _CLI_PLUGIN_HOOKS = "kedro.cli_hooks"
 
 
 def get_cli_hook_manager():
     """Create or return the global _hook_manager singleton instance."""
     global _cli_hook_manager
     if _cli_hook_manager is None:
         _cli_hook_manager = CLIHooksManager()
+    _cli_hook_manager.trace.root.setwriter(logger.debug)
+    _cli_hook_manager.enable_tracing()
     return _cli_hook_manager
 
 
 class CLIHooksManager(PluginManager):
     """Hooks manager to manage CLI hooks"""
 
     def __init__(self) -> None:
@@ -38,12 +42,12 @@
         plugin_names = {
             f"{dist.project_name}-{dist.version}"
             for plugin, dist in plugininfo
             if plugin not in already_registered
         }
 
         if plugin_names:
-            logging.getLogger(__name__).debug(
+            logger.debug(
                 "Registered CLI hooks from %d installed plugin(s): %s",
                 len(plugin_names),
                 ", ".join(sorted(plugin_names)),
             )
```

### Comparing `kedro-0.18.8/kedro/framework/cli/hooks/specs.py` & `kedro-0.18.9/kedro/framework/cli/hooks/specs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """A module containing specifications for all callable hooks in the Kedro CLI's execution timeline.
 For more information about these specifications, please visit
 [Pluggy's documentation](https://pluggy.readthedocs.io/en/stable/#specs)
 """
-from typing import List
+from __future__ import annotations
 
 from kedro.framework.startup import ProjectMetadata
 
 from .markers import cli_hook_spec
 
 
 class CLICommandSpecs:
     """Namespace that defines all specifications for Kedro CLI's lifecycle hooks."""
 
     @cli_hook_spec
     def before_command_run(
         self,
         project_metadata: ProjectMetadata,
-        command_args: List[str],
+        command_args: list[str],
     ):
         """Hooks to be invoked before a CLI command runs.
         It receives the ``project_metadata`` as well as
         all command line arguments that were used, including the command
         and subcommand themselves.
 
         Args:
             project_metadata: The Kedro project's metadata.
             command_args: The command line arguments that were used.
         """
         pass
 
     @cli_hook_spec
     def after_command_run(
-        self, project_metadata: ProjectMetadata, command_args: List[str], exit_code: int
+        self, project_metadata: ProjectMetadata, command_args: list[str], exit_code: int
     ):
         """Hooks to be invoked after a CLI command runs.
         It receives the ``project_metadata`` as well as
         all command line arguments that were used, including the command
         and subcommand themselves and if the operation was successful or not.
 
         Args:
```

### Comparing `kedro-0.18.8/kedro/framework/cli/jupyter.py` & `kedro-0.18.9/kedro/framework/cli/jupyter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """A collection of helper functions to integrate with Jupyter/IPython
 and CLI commands for working with Kedro catalog.
 """
+from __future__ import annotations
+
 import json
 import os
 import shutil
 import sys
 from collections import Counter
 from glob import iglob
 from pathlib import Path
-from typing import Any, Dict
+from typing import Any
 from warnings import warn
 
 import click
 from click import secho
 
 from kedro.framework.cli.utils import (
     KedroCliError,
@@ -296,11 +298,11 @@
         output_path.write_text("")
         for cell in cells:
             _append_source_code(cell, output_path)
     else:
         warn(f"Skipping notebook '{filepath}' - no nodes to export.")
 
 
-def _append_source_code(cell: Dict[str, Any], path: Path) -> None:
+def _append_source_code(cell: dict[str, Any], path: Path) -> None:
     source_code = "".join(cell["source"]).strip() + "\n"
     with path.open(mode="a") as file_:
         file_.write(source_code)
```

### Comparing `kedro-0.18.8/kedro/framework/cli/micropkg.py` & `kedro-0.18.9/kedro/framework/cli/micropkg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """A collection of CLI commands for working with Kedro micro-packages."""
+from __future__ import annotations
 
 import re
 import shutil
 import sys
 import tarfile
 import tempfile
 from importlib import import_module
 from pathlib import Path
-from typing import Iterable, List, Optional, Set, Tuple, Union
+from typing import Iterable, List, Tuple, Union
 
 import click
 import pkg_resources
 from rope.base.project import Project
 from rope.contrib import generate
 from rope.refactor.move import MoveModule
 from rope.refactor.rename import Rename
@@ -275,15 +276,15 @@
     message = (
         f"'{metadata.package_name}.{module_path}' packaged{as_alias}! "
         f"Location: {result_path}"
     )
     click.secho(message, fg="green")
 
 
-def _get_fsspec_filesystem(location: str, fs_args: Optional[str]):
+def _get_fsspec_filesystem(location: str, fs_args: str | None):
     # pylint: disable=import-outside-toplevel
     import anyconfig
     import fsspec
 
     from kedro.io.core import get_protocol_and_path
 
     protocol, _ = get_protocol_and_path(location)
@@ -310,15 +311,15 @@
         member_path = path / member.name
         if not _is_within_directory(path, member_path):
             # pylint: disable=broad-exception-raised
             raise Exception("Failed to safely extract tar file.")
     tar.extractall(path)  # nosec B202
 
 
-def _unpack_sdist(location: str, destination: Path, fs_args: Optional[str]) -> None:
+def _unpack_sdist(location: str, destination: Path, fs_args: str | None) -> None:
     filesystem = _get_fsspec_filesystem(location, fs_args)
 
     if location.endswith(".tar.gz") and filesystem and filesystem.exists(location):
         with filesystem.open(location) as fs_file:
             with tarfile.open(fileobj=fs_file, mode="r:gz") as tar_file:
                 safe_extract(tar_file, destination)
     else:
@@ -349,18 +350,18 @@
         config_file.rename(config_file.parent / new_config_name)
 
 
 def _refactor_code_for_unpacking(
     project: Project,
     package_path: Path,
     tests_path: Path,
-    alias: Optional[str],
-    destination: Optional[str],
+    alias: str | None,
+    destination: str | None,
     project_metadata: ProjectMetadata,
-) -> Tuple[Path, Path]:
+) -> tuple[Path, Path]:
     """This is the reverse operation of `_refactor_code_for_package`, i.e
     we go from:
     <temp_dir>  # also the root of the Rope project
     |__ <micro_package>  # or <alias>
         |__ __init__.py
     |__ tests  # only tests for <micro_package>
         |__ __init__.py
@@ -474,17 +475,17 @@
     # Sync everything under package directory, except `config`
     # since it has already been copied.
     if refactored_package_source.is_dir():
         _sync_dirs(refactored_package_source, package_dest)
 
 
 def _find_config_files(
-    source_config_dir: Path, glob_patterns: List[str]
-) -> List[Tuple[Path, str]]:
-    config_files: List[Tuple[Path, str]] = []
+    source_config_dir: Path, glob_patterns: list[str]
+) -> list[tuple[Path, str]]:
+    config_files: list[tuple[Path, str]] = []
 
     if source_config_dir.is_dir():
         config_files = [
             (path, path.parent.relative_to(source_config_dir).as_posix())
             for glob_pattern in glob_patterns
             for path in source_config_dir.glob(glob_pattern)
             if path.is_file()
@@ -557,21 +558,21 @@
         raise KedroCliError(f"'{path}' is an empty directory.")
 
 
 def _get_sdist_name(name, version):
     return f"{name}-{version}.tar.gz"
 
 
-def _sync_path_list(source: List[Tuple[Path, str]], target: Path) -> None:
+def _sync_path_list(source: list[tuple[Path, str]], target: Path) -> None:
     for source_path, suffix in source:
         target_with_suffix = (target / suffix).resolve()
         _sync_dirs(source_path, target_with_suffix)
 
 
-def _make_install_requires(requirements_txt: Path) -> List[str]:
+def _make_install_requires(requirements_txt: Path) -> list[str]:
     """Parses each line of requirements.txt into a version specifier valid to put in
     install_requires."""
     if not requirements_txt.exists():
         return []
     requirements = pkg_resources.parse_requirements(requirements_txt.read_text())
     return [str(requirement) for requirement in requirements]
 
@@ -624,15 +625,15 @@
     project.do(change)
 
 
 def _refactor_code_for_package(
     project: Project,
     package_path: Path,
     tests_path: Path,
-    alias: Optional[str],
+    alias: str | None,
     project_metadata: ProjectMetadata,
 ) -> None:
     """In order to refactor the imports properly, we need to recreate
     the same nested structure as in the project. Therefore, we create:
     <temp_dir>  # also the root of the Rope project
     |__ <package_name>
         |__ __init__.py
@@ -710,15 +711,15 @@
 _SourcePathType = Union[Path, List[Tuple[Path, str]]]
 
 
 # pylint: disable=too-many-arguments,too-many-locals
 def _generate_sdist_file(
     micropkg_name: str,
     destination: Path,
-    source_paths: Tuple[_SourcePathType, ...],
+    source_paths: tuple[_SourcePathType, ...],
     version: str,
     metadata: ProjectMetadata,
     alias: str = None,
 ) -> None:
     package_name = alias or micropkg_name
     package_source, tests_source, conf_source = source_paths
 
@@ -783,15 +784,15 @@
         global-include config/parameters*/**
         global-include config/parameters*/**/*
         """
     )
 
 
 def _generate_setup_file(
-    package_name: str, version: str, install_requires: List[str], output_dir: Path
+    package_name: str, version: str, install_requires: list[str], output_dir: Path
 ) -> Path:
     setup_file = output_dir / "setup.py"
 
     setup_file_context = {
         "name": package_name,
         "version": version,
         "install_requires": install_requires,
@@ -799,29 +800,29 @@
 
     setup_file.write_text(_SETUP_PY_TEMPLATE.format(**setup_file_context))
     return setup_file
 
 
 def _get_package_artifacts(
     source_path: Path, package_name: str
-) -> Tuple[Path, Path, Path]:
+) -> tuple[Path, Path, Path]:
     """From existing package, returns in order:
     source_path, tests_path, config_path
     """
     artifacts = (
         source_path / package_name,
         source_path / "tests",
         # package_data (non-python files) needs to live inside one of the packages
         source_path / package_name / "config",
     )
     return artifacts
 
 
 def _append_package_reqs(
-    requirements_txt: Path, package_reqs: List[str], package_name: str
+    requirements_txt: Path, package_reqs: list[str], package_name: str
 ) -> None:
     """Appends micro-package requirements to project level requirements.txt"""
     incoming_reqs = _safe_parse_requirements(package_reqs)
     if requirements_txt.is_file():
         existing_reqs = _safe_parse_requirements(requirements_txt.read_text())
         reqs_to_add = set(incoming_reqs) - set(existing_reqs)
         if not reqs_to_add:
@@ -850,16 +851,16 @@
     click.secho(
         "Use 'kedro build-reqs' to compile and 'pip install -r src/requirements.lock' to install "
         "the updated list of requirements."
     )
 
 
 def _safe_parse_requirements(
-    requirements: Union[str, Iterable[str]]
-) -> Set[pkg_resources.Requirement]:
+    requirements: str | Iterable[str],
+) -> set[pkg_resources.Requirement]:
     """Safely parse a requirement or set of requirements. This effectively replaces
     pkg_resources.parse_requirements, which blows up with a ValueError as soon as it
     encounters a requirement it cannot parse (e.g. `-r requirements.txt`). This way
     we can still extract all the parseable requirements out of a set containing some
     unparseable requirements.
     """
     parseable_requirements = set()
```

### Comparing `kedro-0.18.8/kedro/framework/cli/pipeline.py` & `kedro-0.18.9/kedro/framework/cli/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """A collection of CLI commands for working with Kedro pipelines."""
+from __future__ import annotations
+
 import re
 import shutil
 from pathlib import Path
 from textwrap import indent
-from typing import List, NamedTuple, Tuple
+from typing import NamedTuple
 
 import click
 
 import kedro
 from kedro.framework.cli.utils import (
     KedroCliError,
     _clean_pycache,
@@ -169,15 +171,15 @@
     click.secho(
         f"\nIf you added the pipeline '{name}' to 'register_pipelines()' in"
         f""" '{package_dir / "pipeline_registry.py"}', you will need to remove it.""",
         fg="yellow",
     )
 
 
-def _echo_deletion_warning(message: str, **paths: List[Path]):
+def _echo_deletion_warning(message: str, **paths: list[Path]):
     paths = {key: values for key, values in paths.items() if values}
 
     if paths:
         click.secho(message, bold=True)
 
     for key, values in paths.items():
         click.echo(f"\n{key.capitalize()}:")
@@ -277,15 +279,15 @@
         project_metadata, f"pipelines.{pipeline_name}", env
     )
     return PipelineArtifacts(*artifacts)
 
 
 def _get_artifacts_to_package(
     project_metadata: ProjectMetadata, module_path: str, env: str
-) -> Tuple[Path, Path, Path]:
+) -> tuple[Path, Path, Path]:
     """From existing project, returns in order: source_path, tests_path, config_paths"""
     package_dir = project_metadata.source_dir / project_metadata.package_name
     project_conf_path = project_metadata.project_path / settings.CONF_SOURCE
     artifacts = (
         Path(package_dir, *module_path.split(".")),
         Path(package_dir.parent, "tests", *module_path.split(".")),
         project_conf_path / env,
```

### Comparing `kedro-0.18.8/kedro/framework/cli/project.py` & `kedro-0.18.9/kedro/framework/cli/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,36 +144,23 @@
         os.environ["KEDRO_ENV"] = env
     call(["ipython", "--ext", "kedro.ipython"] + list(args))
 
 
 @project_group.command()
 @click.pass_obj  # this will pass the metadata as first argument
 def package(metadata: ProjectMetadata):
-    """Package the project as a Python egg and wheel."""
+    """Package the project as a Python wheel."""
     source_path = metadata.source_dir
     call(
         [
             sys.executable,
-            "setup.py",
-            "clean",
-            "--all",
-            "bdist_egg",
-            "--dist-dir",
-            "../dist",
-        ],
-        cwd=str(source_path),
-    )
-    call(
-        [
-            sys.executable,
-            "setup.py",
-            "clean",
-            "--all",
-            "bdist_wheel",
-            "--dist-dir",
+            "-m",
+            "build",
+            "--wheel",
+            "--outdir",
             "../dist",
         ],
         cwd=str(source_path),
     )
 
     directory = (
         str(Path(settings.CONF_SOURCE).parent)
```

### Comparing `kedro-0.18.8/kedro/framework/cli/registry.py` & `kedro-0.18.9/kedro/framework/cli/registry.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/framework/cli/starters.py` & `kedro-0.18.9/kedro/framework/cli/starters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """kedro is a CLI for managing Kedro projects.
 
 This module implements commands available from the kedro CLI for creating
 projects.
 """
+from __future__ import annotations
+
 import os
 import re
 import shutil
 import stat
 import tempfile
 from collections import OrderedDict
 from itertools import groupby
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Tuple
+from typing import Any, Callable
 
 import click
 import yaml
 from attrs import define, field
 
 import kedro
 from kedro import __version__ as version
@@ -45,16 +47,16 @@
         directory: optional directory inside the repository where the starter resides.
         origin: reserved field used by kedro internally to determine where the starter
         comes from, users do not need to provide this field.
     """
 
     alias: str
     template_path: str
-    directory: Optional[str] = None
-    origin: Optional[str] = field(init=False)
+    directory: str | None = None
+    origin: str | None = field(init=False)
 
 
 _OFFICIAL_STARTER_SPECS = [
     KedroStarterSpec("astro-airflow-iris", _STARTERS_REPO, "astro-airflow-iris"),
     # The `astro-iris` was renamed to `astro-airflow-iris`, but old (external)
     # documentation and tutorials still refer to `astro-iris`. We create an alias to
     # check if a user has entered old `astro-iris` as the starter name and changes it
@@ -86,23 +88,23 @@
 )
 DIRECTORY_ARG_HELP = (
     "An optional directory inside the repository where the starter resides."
 )
 
 
 # pylint: disable=unused-argument
-def _remove_readonly(func: Callable, path: Path, excinfo: Tuple):  # pragma: no cover
+def _remove_readonly(func: Callable, path: Path, excinfo: tuple):  # pragma: no cover
     """Remove readonly files on Windows
     See: https://docs.python.org/3/library/shutil.html?highlight=shutil#rmtree-example
     """
     os.chmod(path, stat.S_IWRITE)
     func(path)
 
 
-def _get_starters_dict() -> Dict[str, KedroStarterSpec]:
+def _get_starters_dict() -> dict[str, KedroStarterSpec]:
     """This function lists all the starter aliases declared in
     the core repo and in plugins entry points.
 
     For example, the output for official kedro starters looks like:
     {"astro-airflow-iris":
         KedroStarterSpec(
             name="astro-airflow-iris",
@@ -141,18 +143,18 @@
             else:
                 spec.origin = origin
                 starter_specs[spec.alias] = spec
     return starter_specs
 
 
 def _starter_spec_to_dict(
-    starter_specs: Dict[str, KedroStarterSpec]
-) -> Dict[str, Dict[str, str]]:
+    starter_specs: dict[str, KedroStarterSpec]
+) -> dict[str, dict[str, str]]:
     """Convert a dictionary of starters spec to a nicely formatted dictionary"""
-    format_dict: Dict[str, Dict[str, str]] = {}
+    format_dict: dict[str, dict[str, str]] = {}
     for alias, spec in starter_specs.items():
         format_dict[alias] = {}  # Each dictionary represent 1 starter
         format_dict[alias]["template_path"] = spec.template_path
         if spec.directory:
             format_dict[alias]["directory"] = spec.directory
     return format_dict
 
@@ -240,15 +242,15 @@
 
 @starter.command("list")
 def list_starters():
     """List all official project starters available."""
     starters_dict = _get_starters_dict()
 
     # Group all specs by origin as nested dict and sort it.
-    sorted_starters_dict: Dict[str, Dict[str, KedroStarterSpec]] = {
+    sorted_starters_dict: dict[str, dict[str, KedroStarterSpec]] = {
         origin: dict(sorted(starters_dict_by_origin))
         for origin, starters_dict_by_origin in groupby(
             starters_dict.items(), lambda item: item[1].origin
         )
     }
 
     # ensure kedro starters are listed first
@@ -259,15 +261,15 @@
     for origin, starters_spec in sorted_starters_dict.items():
         click.secho(f"\nStarters from {origin}\n", fg="yellow")
         click.echo(
             yaml.safe_dump(_starter_spec_to_dict(starters_spec), sort_keys=False)
         )
 
 
-def _fetch_config_from_file(config_path: str) -> Dict[str, str]:
+def _fetch_config_from_file(config_path: str) -> dict[str, str]:
     """Obtains configuration for a new kedro project non-interactively from a file.
 
     Args:
         config_path: The path of the config.yml which should contain the data required
             by ``prompts.yml``.
 
     Returns:
@@ -290,18 +292,18 @@
             f"Failed to generate project: could not load config at {config_path}."
         ) from exc
 
     return config
 
 
 def _make_cookiecutter_args(
-    config: Dict[str, str],
+    config: dict[str, str],
     checkout: str,
     directory: str,
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     """Creates a dictionary of arguments to pass to cookiecutter.
 
     Args:
         config: Configuration for starting a new project. This is passed as
             ``extra_context`` to cookiecutter and will overwrite the cookiecutter.json
             defaults.
         checkout: The tag, branch or commit in the starter repository to checkout.
@@ -326,15 +328,15 @@
         cookiecutter_args["checkout"] = checkout
     if directory:
         cookiecutter_args["directory"] = directory
 
     return cookiecutter_args
 
 
-def _create_project(template_path: str, cookiecutter_args: Dict[str, Any]):
+def _create_project(template_path: str, cookiecutter_args: dict[str, Any]):
     """Creates a new kedro project using cookiecutter.
 
     Args:
         template_path: The path to the cookiecutter template to create the project.
             It could either be a local directory or a remote VCS repository
             supported by cookiecutter. For more details, please see:
             https://cookiecutter.readthedocs.io/en/latest/usage.html#generate-your-project
@@ -412,15 +414,15 @@
             f"{error_message}. The aliases for the official Kedro starters are: \n"
             f"{yaml.safe_dump(official_starters, sort_keys=False)}"
         ) from exc
 
     return Path(cookiecutter_dir)
 
 
-def _get_prompts_required(cookiecutter_dir: Path) -> Optional[Dict[str, Any]]:
+def _get_prompts_required(cookiecutter_dir: Path) -> dict[str, Any] | None:
     """Finds the information a user must supply according to prompts.yml."""
     prompts_yml = cookiecutter_dir / "prompts.yml"
     if not prompts_yml.is_file():
         return None
 
     try:
         with prompts_yml.open("r") as prompts_file:
@@ -428,31 +430,31 @@
     except Exception as exc:
         raise KedroCliError(
             "Failed to generate project: could not load prompts.yml."
         ) from exc
 
 
 def _fetch_config_from_user_prompts(
-    prompts: Dict[str, Any], cookiecutter_context: OrderedDict
-) -> Dict[str, str]:
+    prompts: dict[str, Any], cookiecutter_context: OrderedDict
+) -> dict[str, str]:
     """Interactively obtains information from user prompts.
 
     Args:
         prompts: Prompts from prompts.yml.
         cookiecutter_context: Cookiecutter context generated from cookiecutter.json.
 
     Returns:
         Configuration for starting a new project. This is passed as ``extra_context``
             to cookiecutter and will overwrite the cookiecutter.json defaults.
     """
     # pylint: disable=import-outside-toplevel
     from cookiecutter.environment import StrictEnvironment
     from cookiecutter.prompt import read_user_variable, render_variable
 
-    config: Dict[str, str] = {}
+    config: dict[str, str] = {}
 
     for variable_name, prompt_dict in prompts.items():
         prompt = _Prompt(**prompt_dict)
 
         # render the variable on the command line
         cookiecutter_variable = render_variable(
             env=StrictEnvironment(context=cookiecutter_context),
@@ -503,15 +505,15 @@
         if self.regexp and not re.match(self.regexp, user_input):
             message = f"'{user_input}' is an invalid value for {self.title}."
             click.secho(message, fg="red", err=True)
             click.secho(self.error_message, fg="red", err=True)
             raise ValueError(message, self.error_message)
 
 
-def _get_available_tags(template_path: str) -> List:
+def _get_available_tags(template_path: str) -> list:
     # Not at top level so that kedro CLI works without a working git executable.
     # pylint: disable=import-outside-toplevel
     import git
 
     try:
         tags = git.cmd.Git().ls_remote("--tags", template_path.replace("git+", ""))
 
@@ -523,15 +525,15 @@
         # unique_tags: {'version'}
 
     except git.GitCommandError:
         return []
     return sorted(unique_tags)
 
 
-def _validate_config_file(config: Dict[str, str], prompts: Dict[str, Any]):
+def _validate_config_file(config: dict[str, str], prompts: dict[str, Any]):
     """Checks that the configuration file contains all needed variables.
 
     Args:
         config: The config as a dictionary.
         prompts: Prompts from prompts.yml.
 
     Raises:
```

### Comparing `kedro-0.18.8/kedro/framework/cli/utils.py` & `kedro-0.18.9/kedro/framework/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Utilities for use with click."""
+from __future__ import annotations
+
 import difflib
 import logging
 import re
 import shlex
 import shutil
 import subprocess
 import sys
@@ -10,15 +12,15 @@
 import traceback
 import warnings
 from collections import defaultdict
 from contextlib import contextmanager
 from importlib import import_module
 from itertools import chain
 from pathlib import Path
-from typing import Dict, Iterable, List, Mapping, Sequence, Set, Tuple, Union
+from typing import Iterable, Sequence
 
 import click
 import importlib_metadata
 from omegaconf import OmegaConf
 
 CONTEXT_SETTINGS = {"help_option_names": ["-h", "--help"]}
 MAX_SUGGESTIONS = 3
@@ -35,15 +37,15 @@
     "cli_hooks": "kedro.cli_hooks",
     "starters": "kedro.starters",
 }
 
 logger = logging.getLogger(__name__)
 
 
-def call(cmd: List[str], **kwargs):  # pragma: no cover
+def call(cmd: list[str], **kwargs):  # pragma: no cover
     """Run a subprocess command and raise if it fails.
 
     Args:
         cmd: List of command parts.
         **kwargs: Optional keyword arguments passed to `subprocess.run`.
 
     Raises:
@@ -106,15 +108,15 @@
     suggestion += textwrap.indent("\n".join(matches), " " * 4)  # type: ignore
     return suggestion
 
 
 class CommandCollection(click.CommandCollection):
     """Modified from the Click one to still run the source groups function."""
 
-    def __init__(self, *groups: Tuple[str, Sequence[click.MultiCommand]]):
+    def __init__(self, *groups: tuple[str, Sequence[click.MultiCommand]]):
         self.groups = [
             (title, self._merge_same_name_collections(cli_list))
             for title, cli_list in groups
         ]
         sources = list(chain.from_iterable(cli_list for _, cli_list in self.groups))
 
         help_texts = [
@@ -133,15 +135,15 @@
         self.callback = sources[0].callback
 
     @staticmethod
     def _dedupe_commands(cli_collections: Sequence[click.CommandCollection]):
         """Deduplicate commands by keeping the ones from the last source
         in the list.
         """
-        seen_names: Set[str] = set()
+        seen_names: set[str] = set()
         for cli_collection in reversed(cli_collections):
             for cmd_group in reversed(cli_collection.sources):
                 cmd_group.commands = {  # type: ignore
                     cmd_name: cmd
                     for cmd_name, cmd in cmd_group.commands.items()  # type: ignore
                     if cmd_name not in seen_names
                 }
@@ -153,16 +155,16 @@
                 cmd_group
                 for cmd_group in cli_collection.sources
                 if cmd_group.commands  # type: ignore
             ]
 
     @staticmethod
     def _merge_same_name_collections(groups: Sequence[click.MultiCommand]):
-        named_groups: Mapping[str, List[click.MultiCommand]] = defaultdict(list)
-        helps: Mapping[str, list] = defaultdict(list)
+        named_groups: defaultdict[str, list[click.MultiCommand]] = defaultdict(list)
+        helps: defaultdict[str, list] = defaultdict(list)
         for group in groups:
             named_groups[group.name].append(group)
             if group.help:
                 helps[group.name].append(group.help)
 
         return [
             click.CommandCollection(
@@ -172,15 +174,15 @@
                 callback=cli_list[0].callback,
                 params=cli_list[0].params,
             )
             for group_name, cli_list in named_groups.items()
             if cli_list
         ]
 
-    def resolve_command(self, ctx: click.core.Context, args: List):
+    def resolve_command(self, ctx: click.core.Context, args: list):
         try:
             return super().resolve_command(ctx, args)
         except click.exceptions.UsageError as exc:
             original_command_name = click.utils.make_str(args[0])
             existing_command_names = self.list_commands(ctx)
             exc.message += _suggest_cli_command(
                 original_command_name, existing_command_names
@@ -195,15 +197,15 @@
                 if group.sources:
                     formatter.write(
                         click.style(f"\n{title} from {group.name}", fg="green")
                     )
                     group.format_commands(ctx, formatter)
 
 
-def get_pkg_version(reqs_path: (Union[str, Path]), package_name: str) -> str:
+def get_pkg_version(reqs_path: (str | Path), package_name: str) -> str:
     """Get package version from requirements.txt.
 
     Args:
         reqs_path: Path to requirements.txt file.
         package_name: Package to search for.
 
     Returns:
@@ -291,15 +293,15 @@
 
 def split_string(ctx, param, value):  # pylint: disable=unused-argument
     """Split string by comma."""
     return [item.strip() for item in value.split(",") if item.strip()]
 
 
 # pylint: disable=unused-argument,missing-param-doc,missing-type-doc
-def split_node_names(ctx, param, to_split: str) -> List[str]:
+def split_node_names(ctx, param, to_split: str) -> list[str]:
     """Split string by comma, ignoring commas enclosed by square parentheses.
     This avoids splitting the string of nodes names on commas included in
     default node names, which have the pattern
     <function_name>([<input_name>,...]) -> [<output_name>,...])
 
     Note:
         - `to_split` will have such commas if and only if it includes a
@@ -413,15 +415,15 @@
     if value:
         config = anyconfig.load(value)[section]
         ctx.default_map.update(config)
 
     return value
 
 
-def _reformat_load_versions(ctx, param, value) -> Dict[str, str]:
+def _reformat_load_versions(ctx, param, value) -> dict[str, str]:
     """Reformat data structure from tuple to dictionary for `load-version`, e.g.:
     ('dataset1:time1', 'dataset2:time2') -> {"dataset1": "time1", "dataset2": "time2"}.
     """
     if param.name == "load_version":
         _deprecate_options(ctx, param, value)
 
     load_versions_dict = {}
@@ -471,15 +473,15 @@
 
 
 def _split_load_versions(ctx, param, value):
     lv_tuple = _get_values_as_tuple([value])
     return _reformat_load_versions(ctx, param, lv_tuple) if value else {}
 
 
-def _get_values_as_tuple(values: Iterable[str]) -> Tuple[str, ...]:
+def _get_values_as_tuple(values: Iterable[str]) -> tuple[str, ...]:
     return tuple(chain.from_iterable(value.split(",") for value in values))
 
 
 def _deprecate_options(ctx, param, value):
     deprecated_flag = {
         "node_names": "--node",
         "tag": "--tag",
```

### Comparing `kedro-0.18.8/kedro/framework/context/context.py` & `kedro-0.18.9/kedro/framework/context/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """This module provides context for Kedro project."""
+from __future__ import annotations
 
 import logging
 from copy import deepcopy
 from pathlib import Path, PurePosixPath, PureWindowsPath
-from typing import Any, Dict, Optional, Union
+from typing import Any
 from urllib.parse import urlparse
 from warnings import warn
 
-from omegaconf import DictConfig
 from pluggy import PluginManager
 
 from kedro.config import ConfigLoader, MissingConfigException
 from kedro.framework.project import settings
 from kedro.io import DataCatalog
 from kedro.pipeline.pipeline import _transcode_split
 
@@ -48,16 +48,16 @@
     if is_absolute_path:
         return False
 
     return True
 
 
 def _convert_paths_to_absolute_posix(
-    project_path: Path, conf_dictionary: Dict[str, Any]
-) -> Dict[str, Any]:
+    project_path: Path, conf_dictionary: dict[str, Any]
+) -> dict[str, Any]:
     """Turn all relative paths inside ``conf_dictionary`` into absolute paths by appending them
     to ``project_path`` and convert absolute Windows paths to POSIX format. This is a hack to
     make sure that we don't have to change user's working directory for logging and datasets to
     work. It is important for non-standard workflows such as IPython notebook where users don't go
     through `kedro run` or `__main__.py` entrypoints.
 
     Example:
@@ -88,15 +88,14 @@
             f"project_path must be an absolute path. Received: {project_path}"
         )
 
     # only check a few conf keys that are known to specify a path string as value
     conf_keys_with_filepath = ("filename", "filepath", "path")
 
     for conf_key, conf_value in conf_dictionary.items():
-
         # if the conf_value is another dictionary, absolutify its paths first.
         if isinstance(conf_value, dict):
             conf_dictionary[conf_key] = _convert_paths_to_absolute_posix(
                 project_path, conf_value
             )
             continue
 
@@ -139,47 +138,45 @@
     if conflicting_datasets:
         error_str = ", ".join(conflicting_datasets)
         raise ValueError(
             f"Transcoded datasets should have the same layer. Mismatch found for: {error_str}"
         )
 
 
-def _update_nested_dict(old_dict: Dict[Any, Any], new_dict: Dict[Any, Any]) -> None:
+def _update_nested_dict(old_dict: dict[Any, Any], new_dict: dict[Any, Any]) -> None:
     """Update a nested dict with values of new_dict.
 
     Args:
         old_dict: dict to be updated
         new_dict: dict to use for updating old_dict
 
     """
     for key, value in new_dict.items():
         if key not in old_dict:
             old_dict[key] = value
         else:
-            if isinstance(old_dict[key], (dict, DictConfig)) and isinstance(
-                value, (dict, DictConfig)
-            ):
+            if isinstance(old_dict[key], dict) and isinstance(value, dict):
                 _update_nested_dict(old_dict[key], value)
             else:
                 old_dict[key] = value
 
 
 class KedroContext:
     """``KedroContext`` is the base class which holds the configuration and
     Kedro's main functionality.
     """
 
     def __init__(
         self,
         package_name: str,
-        project_path: Union[Path, str],
+        project_path: Path | str,
         config_loader: ConfigLoader,
         hook_manager: PluginManager,
         env: str = None,
-        extra_params: Dict[str, Any] = None,
+        extra_params: dict[str, Any] = None,
     ):  # pylint: disable=too-many-arguments
         """Create a context object by providing the root of a Kedro project and
         the environment configuration subfolders
         (see ``kedro.config.ConfigLoader``)
 
         Raises:
             KedroContextError: If there is a mismatch
@@ -200,15 +197,15 @@
         self._package_name = package_name
         self._config_loader = config_loader
         self._env = env
         self._extra_params = deepcopy(extra_params)
         self._hook_manager = hook_manager
 
     @property  # type: ignore
-    def env(self) -> Optional[str]:
+    def env(self) -> str | None:
         """Property for the current Kedro environment.
 
         Returns:
             Name of the current Kedro environment.
 
         """
         return self._env
@@ -232,15 +229,15 @@
         Raises:
             KedroContextError: Incorrect ``DataCatalog`` registered for the project.
 
         """
         return self._get_catalog()
 
     @property
-    def params(self) -> Dict[str, Any]:
+    def params(self) -> dict[str, Any]:
         """Read-only property referring to Kedro's parameters for this context.
 
         Returns:
             Parameters defined in `parameters.yml` with the addition of any
                 extra parameters passed at initialization.
         """
         try:
@@ -261,15 +258,15 @@
             KedroContextError: Incorrect ``ConfigLoader`` registered for the project.
         """
         return self._config_loader
 
     def _get_catalog(
         self,
         save_version: str = None,
-        load_versions: Dict[str, str] = None,
+        load_versions: dict[str, str] = None,
     ) -> DataCatalog:
         """A hook for changing the creation of a DataCatalog instance.
 
         Returns:
             DataCatalog defined in `catalog.yml`.
         Raises:
             KedroContextError: Incorrect ``DataCatalog`` registered for the project.
@@ -301,15 +298,15 @@
             conf_creds=conf_creds,
             feed_dict=feed_dict,
             save_version=save_version,
             load_versions=load_versions,
         )
         return catalog
 
-    def _get_feed_dict(self) -> Dict[str, Any]:
+    def _get_feed_dict(self) -> dict[str, Any]:
         """Get parameters and return the feed dictionary."""
         params = self.params
         feed_dict = {"parameters": params}
 
         def _add_param_to_feed_dict(param_name, param_value):
             """This recursively adds parameter paths to the `feed_dict`,
             whenever `param_value` is a dictionary itself, so that users can
@@ -321,24 +318,24 @@
                 >>> param_value = {"b": 1}
                 >>> _add_param_to_feed_dict(param_name, param_value)
                 >>> assert feed_dict["params:a"] == {"b": 1}
                 >>> assert feed_dict["params:a.b"] == 1
             """
             key = f"params:{param_name}"
             feed_dict[key] = param_value
-            if isinstance(param_value, (dict, DictConfig)):
+            if isinstance(param_value, dict):
                 for key, val in param_value.items():
                     _add_param_to_feed_dict(f"{param_name}.{key}", val)
 
         for param_name, param_value in params.items():
             _add_param_to_feed_dict(param_name, param_value)
 
         return feed_dict
 
-    def _get_config_credentials(self) -> Dict[str, Any]:
+    def _get_config_credentials(self) -> dict[str, Any]:
         """Getter for credentials specified in credentials directory."""
         try:
             conf_creds = self.config_loader["credentials"]
         except MissingConfigException as exc:
             logging.getLogger(__name__).debug(
                 "Credentials not found in your Kedro project config.\n %s", str(exc)
             )
```

### Comparing `kedro-0.18.8/kedro/framework/hooks/manager.py` & `kedro-0.18.9/kedro/framework/hooks/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 logger = logging.getLogger(__name__)
 
 
 def _create_hook_manager() -> PluginManager:
     """Create a new PluginManager instance and register Kedro's hook specs."""
     manager = PluginManager(HOOK_NAMESPACE)
+    manager.trace.root.setwriter(logger.debug)
+    manager.enable_tracing()
     manager.add_hookspecs(NodeSpecs)
     manager.add_hookspecs(PipelineSpecs)
     manager.add_hookspecs(DataCatalogSpecs)
     manager.add_hookspecs(DatasetSpecs)
     manager.add_hookspecs(KedroContextSpecs)
     return manager
 
@@ -56,18 +58,21 @@
         hook_manager: Hook manager instance to register the hooks with.
         disabled_plugins: An iterable returning the names of plugins
             which hooks must not be registered; any already registered
             hooks will be unregistered.
 
     """
     already_registered = hook_manager.get_plugins()
+    # Method name is misleading:
+    # entry points are standard and don't require setuptools,
+    # see https://packaging.python.org/en/latest/specifications/entry-points/
     hook_manager.load_setuptools_entrypoints(_PLUGIN_HOOKS)
     disabled_plugins = set(disabled_plugins)
 
-    # Get list of plugin/distinfo tuples for all setuptools registered plugins.
+    # Get list of plugin/distinfo tuples for all registered plugins.
     plugininfo = hook_manager.list_plugin_distinfo()
     plugin_names = set()
     disabled_plugin_names = set()
     for plugin, dist in plugininfo:
         if dist.project_name in disabled_plugins:
             # `unregister()` is used instead of `set_blocked()` because
             # we want to disable hooks for specific plugin based on project
```

### Comparing `kedro-0.18.8/kedro/framework/hooks/specs.py` & `kedro-0.18.9/kedro/framework/hooks/specs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """A module containing specifications for all callable hooks in the Kedro's execution timeline.
 For more information about these specifications, please visit
 [Pluggy's documentation](https://pluggy.readthedocs.io/en/stable/#specs)
 """
-from typing import Any, Dict, Optional
+from __future__ import annotations
+
+from typing import Any
 
 from kedro.framework.context import KedroContext
 from kedro.io import DataCatalog
 from kedro.pipeline import Pipeline
 from kedro.pipeline.node import Node
 
 from .markers import hook_spec
@@ -15,19 +17,19 @@
 class DataCatalogSpecs:
     """Namespace that defines all specifications for a data catalog's lifecycle hooks."""
 
     @hook_spec
     def after_catalog_created(  # pylint: disable=too-many-arguments
         self,
         catalog: DataCatalog,
-        conf_catalog: Dict[str, Any],
-        conf_creds: Dict[str, Any],
-        feed_dict: Dict[str, Any],
+        conf_catalog: dict[str, Any],
+        conf_creds: dict[str, Any],
+        feed_dict: dict[str, Any],
         save_version: str,
-        load_versions: Dict[str, str],
+        load_versions: dict[str, str],
     ) -> None:
         """Hooks to be invoked after a data catalog is created.
         It receives the ``catalog`` as well as
         all the arguments for ``KedroContext._create_catalog``.
 
         Args:
             catalog: The catalog that was created.
@@ -46,18 +48,18 @@
     """Namespace that defines all specifications for a node's lifecycle hooks."""
 
     @hook_spec
     def before_node_run(  # pylint: disable=too-many-arguments
         self,
         node: Node,
         catalog: DataCatalog,
-        inputs: Dict[str, Any],
+        inputs: dict[str, Any],
         is_async: bool,
         session_id: str,
-    ) -> Optional[Dict[str, Any]]:
+    ) -> dict[str, Any] | None:
         """Hook to be invoked before a node runs.
         The arguments received are the same as those used by ``kedro.runner.run_node``
 
         Args:
             node: The ``Node`` to run.
             catalog: A ``DataCatalog`` containing the node's inputs and outputs.
             inputs: The dictionary of inputs dataset.
@@ -74,16 +76,16 @@
         pass
 
     @hook_spec
     def after_node_run(  # pylint: disable=too-many-arguments
         self,
         node: Node,
         catalog: DataCatalog,
-        inputs: Dict[str, Any],
-        outputs: Dict[str, Any],
+        inputs: dict[str, Any],
+        outputs: dict[str, Any],
         is_async: bool,
         session_id: str,
     ) -> None:
         """Hook to be invoked after a node runs.
         The arguments received are the same as those used by ``kedro.runner.run_node``
         as well as the ``outputs`` of the node run.
 
@@ -103,15 +105,15 @@
 
     @hook_spec
     def on_node_error(  # pylint: disable=too-many-arguments
         self,
         error: Exception,
         node: Node,
         catalog: DataCatalog,
-        inputs: Dict[str, Any],
+        inputs: dict[str, Any],
         is_async: bool,
         session_id: str,
     ):
         """Hook to be invoked if a node run throws an uncaught error.
         The signature of this error hook should match the signature of ``before_node_run``
         along with the error that was raised.
 
@@ -129,15 +131,15 @@
 
 
 class PipelineSpecs:
     """Namespace that defines all specifications for a pipeline's lifecycle hooks."""
 
     @hook_spec
     def before_pipeline_run(
-        self, run_params: Dict[str, Any], pipeline: Pipeline, catalog: DataCatalog
+        self, run_params: dict[str, Any], pipeline: Pipeline, catalog: DataCatalog
     ) -> None:
         """Hook to be invoked before a pipeline runs.
 
         Args:
             run_params: The params used to run the pipeline.
                 Should have the following schema::
 
@@ -149,28 +151,30 @@
                      "tags": Optional[List[str]],
                      "from_nodes": Optional[List[str]],
                      "to_nodes": Optional[List[str]],
                      "node_names": Optional[List[str]],
                      "from_inputs": Optional[List[str]],
                      "to_outputs": Optional[List[str]],
                      "load_versions": Optional[List[str]],
-                     "pipeline_name": str,
                      "extra_params": Optional[Dict[str, Any]]
+                     "pipeline_name": str,
+                     "namespace": Optional[str],
+                     "runner": str,
                    }
 
             pipeline: The ``Pipeline`` that will be run.
             catalog: The ``DataCatalog`` to be used during the run.
         """
         pass
 
     @hook_spec
     def after_pipeline_run(
         self,
-        run_params: Dict[str, Any],
-        run_result: Dict[str, Any],
+        run_params: dict[str, Any],
+        run_result: dict[str, Any],
         pipeline: Pipeline,
         catalog: DataCatalog,
     ) -> None:
         """Hook to be invoked after a pipeline runs.
 
         Args:
             run_params: The params used to run the pipeline.
@@ -184,29 +188,31 @@
                      "tags": Optional[List[str]],
                      "from_nodes": Optional[List[str]],
                      "to_nodes": Optional[List[str]],
                      "node_names": Optional[List[str]],
                      "from_inputs": Optional[List[str]],
                      "to_outputs": Optional[List[str]],
                      "load_versions": Optional[List[str]],
-                     "pipeline_name": str,
                      "extra_params": Optional[Dict[str, Any]]
+                     "pipeline_name": str,
+                     "namespace": Optional[str],
+                     "runner": str,
                    }
 
             run_result: The output of ``Pipeline`` run.
             pipeline: The ``Pipeline`` that was run.
             catalog: The ``DataCatalog`` used during the run.
         """
         pass
 
     @hook_spec
     def on_pipeline_error(
         self,
         error: Exception,
-        run_params: Dict[str, Any],
+        run_params: dict[str, Any],
         pipeline: Pipeline,
         catalog: DataCatalog,
     ):
         """Hook to be invoked if a pipeline run throws an uncaught Exception.
         The signature of this error hook should match the signature of ``before_pipeline_run``
         along with the error that was raised.
 
@@ -223,17 +229,20 @@
                      "tags": Optional[List[str]],
                      "from_nodes": Optional[List[str]],
                      "to_nodes": Optional[List[str]],
                      "node_names": Optional[List[str]],
                      "from_inputs": Optional[List[str]],
                      "to_outputs": Optional[List[str]],
                      "load_versions": Optional[List[str]],
-                     "pipeline_name": str,
                      "extra_params": Optional[Dict[str, Any]]
+                     "pipeline_name": str,
+                     "namespace": Optional[str],
+                     "runner": str,
                    }
+
             pipeline: The ``Pipeline`` that will was run.
             catalog: The ``DataCatalog`` used during the run.
         """
         pass
 
 
 class DatasetSpecs:
```

### Comparing `kedro-0.18.8/kedro/framework/project/__init__.py` & `kedro-0.18.9/kedro/framework/project/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """``kedro.framework.project`` module provides utitlity to
 configure a Kedro project and access its settings."""
 # pylint: disable=redefined-outer-name,unused-argument,global-statement
+from __future__ import annotations
+
 import importlib
 import logging.config
 import operator
 import os
-import sys
 import traceback
 import types
 import warnings
 from collections import UserDict
 from collections.abc import MutableMapping
 from pathlib import Path
-from typing import Any, Dict, Optional
+from typing import Any
 
-import click
 import importlib_resources
-import rich.pretty
-import rich.traceback
 import yaml
 from dynaconf import LazySettings
 from dynaconf.validator import ValidationError, Validator
 
 from kedro.pipeline import Pipeline, pipeline
 
 IMPORT_ERROR_MESSAGE = (
@@ -155,17 +153,17 @@
        modules need to be imported.
     3. To ensure Kedro CLI remains functional when pipelines are broken. During development, broken
        pipelines are common, but they shouldn't prevent other parts of Kedro CLI from functioning
        properly (e.g. `kedro -h`).
     """
 
     def __init__(self) -> None:
-        self._pipelines_module: Optional[str] = None
+        self._pipelines_module: str | None = None
         self._is_data_loaded = False
-        self._content: Dict[str, Pipeline] = {}
+        self._content: dict[str, Pipeline] = {}
 
     @staticmethod
     def _get_pipelines_registry_callable(pipelines_module: str):
         module_obj = importlib.import_module(pipelines_module)
         register_pipelines = getattr(module_obj, "register_pipelines")
         return register_pipelines
 
@@ -181,15 +179,15 @@
             self._pipelines_module
         )
         project_pipelines = register_pipelines()
 
         self._content = project_pipelines
         self._is_data_loaded = True
 
-    def configure(self, pipelines_module: Optional[str] = None) -> None:
+    def configure(self, pipelines_module: str | None = None) -> None:
         """Configure the pipelines_module to load the pipelines dictionary.
         Reset the data loading state so that after every ``configure`` call,
         data are reloaded.
         """
         self._pipelines_module = pipelines_module
         self._is_data_loaded = False
         self._content = {}
@@ -215,28 +213,16 @@
         """Initialise project logging. The path to logging configuration is given in
         environment variable KEDRO_LOGGING_CONFIG (defaults to default_logging.yml)."""
         path = os.environ.get(
             "KEDRO_LOGGING_CONFIG", Path(__file__).parent / "default_logging.yml"
         )
         logging_config = Path(path).read_text(encoding="utf-8")
         self.configure(yaml.safe_load(logging_config))
-        logging.captureWarnings(True)
-
-        # We suppress click here to hide tracebacks related to it conversely,
-        # kedro is not suppressed to show its tracebacks for easier debugging.
-        # sys.executable is used to get the kedro executable path to hide the
-        # top level traceback.
-        # Rich traceback handling does not work on databricks. Hopefully this will be
-        # fixed on their side at some point, but until then we disable it.
-        # See https://github.com/Textualize/rich/issues/2455
-        if "DATABRICKS_RUNTIME_VERSION" not in os.environ:
-            rich.traceback.install(suppress=[click, str(Path(sys.executable).parent)])
-        rich.pretty.install()
 
-    def configure(self, logging_config: Dict[str, Any]) -> None:
+    def configure(self, logging_config: dict[str, Any]) -> None:
         """Configure project logging using ``logging_config`` (e.g. from project
         logging.yml). We store this in the UserDict data so that it can be reconfigured
         in _bootstrap_subprocess.
         """
         logging.config.dictConfig(logging_config)
         self.data = logging_config
 
@@ -263,15 +249,15 @@
     # global variable to make it easily accessible. This is used by validate_settings()
     # below, and also by ParallelRunner on Windows, as package_name is required every
     # time a new subprocess is spawned.
     global PACKAGE_NAME
     PACKAGE_NAME = package_name
 
 
-def configure_logging(logging_config: Dict[str, Any]) -> None:
+def configure_logging(logging_config: dict[str, Any]) -> None:
     """Configure logging according to ``logging_config`` dictionary."""
     LOGGING.configure(logging_config)
 
 
 def validate_settings():
     """Eagerly validate that the settings module is importable. This is desirable to
     surface any syntax or import errors early. In particular, without eagerly importing
@@ -286,15 +272,15 @@
             "'bootstrap_project'. This should happen automatically if you are using "
             "Kedro command line interface."
         )
 
     importlib.import_module(f"{PACKAGE_NAME}.settings")
 
 
-def _create_pipeline(pipeline_module: types.ModuleType) -> Optional[Pipeline]:
+def _create_pipeline(pipeline_module: types.ModuleType) -> Pipeline | None:
     if not hasattr(pipeline_module, "create_pipeline"):
         warnings.warn(
             f"The '{pipeline_module.__name__}' module does not "
             f"expose a 'create_pipeline' function, so no pipelines "
             f"defined therein will be returned by 'find_pipelines'."
         )
         return None
@@ -309,15 +295,15 @@
             f"'find_pipelines'."
         )
         return None
 
     return obj
 
 
-def find_pipelines() -> Dict[str, Pipeline]:
+def find_pipelines() -> dict[str, Pipeline]:
     """Automatically find modular pipelines having a ``create_pipeline``
     function. By default, projects created using Kedro 0.18.3 and higher
     call this function to autoregister pipelines upon creation/addition.
 
     Projects that require more fine-grained control can still define the
     pipeline registry without calling this function. Alternatively, they
     can modify the mapping generated by the ``find_pipelines`` function.
```

### Comparing `kedro-0.18.8/kedro/framework/session/session.py` & `kedro-0.18.9/kedro/framework/session/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """This module implements Kedro session responsible for project lifecycle."""
+from __future__ import annotations
+
 import getpass
 import logging
 import logging.config
 import os
 import subprocess
 import sys
 import traceback
 from copy import deepcopy
 from pathlib import Path
-from typing import Any, Dict, Iterable, Optional, Union
+from typing import Any, Iterable
 
 import click
-from omegaconf import OmegaConf, omegaconf
 
 from kedro import __version__ as kedro_version
 from kedro.config import ConfigLoader, MissingConfigException
 from kedro.framework.context import KedroContext
 from kedro.framework.context.context import _convert_paths_to_absolute_posix
 from kedro.framework.hooks import _create_hook_manager
 from kedro.framework.hooks.manager import _register_hooks, _register_hooks_setuptools
@@ -26,23 +27,23 @@
     validate_settings,
 )
 from kedro.framework.session.store import BaseSessionStore
 from kedro.io.core import generate_timestamp
 from kedro.runner import AbstractRunner, SequentialRunner
 
 
-def _describe_git(project_path: Path) -> Dict[str, Dict[str, Any]]:
+def _describe_git(project_path: Path) -> dict[str, dict[str, Any]]:
     project_path = str(project_path)
     try:
         res = subprocess.check_output(
             ["git", "rev-parse", "--short", "HEAD"],
             cwd=project_path,
             stderr=subprocess.STDOUT,
         )
-        git_data: Dict[str, Any] = {"commit_sha": res.decode().strip()}
+        git_data: dict[str, Any] = {"commit_sha": res.decode().strip()}
         git_status_res = subprocess.check_output(
             ["git", "status", "--short"],
             cwd=project_path,
             stderr=subprocess.STDOUT,
         )
         git_data["dirty"] = bool(git_status_res.decode().strip())
 
@@ -52,15 +53,15 @@
         logger.debug("Unable to git describe %s", project_path)
         logger.debug(traceback.format_exc())
         return {}
 
     return {"git": git_data}
 
 
-def _jsonify_cli_context(ctx: click.core.Context) -> Dict[str, Any]:
+def _jsonify_cli_context(ctx: click.core.Context) -> dict[str, Any]:
     return {
         "args": ctx.args,
         "params": ctx.params,
         "command_name": ctx.command.name,
         "command_path": " ".join(["kedro"] + sys.argv[1:]),
     }
 
@@ -99,17 +100,17 @@
     """
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         session_id: str,
         package_name: str = None,
-        project_path: Union[Path, str] = None,
+        project_path: Path | str | None = None,
         save_on_close: bool = False,
-        conf_source: Optional[str] = None,
+        conf_source: str | None = None,
     ):
         self._project_path = Path(project_path or Path.cwd()).resolve()
         self.session_id = session_id
         self.save_on_close = save_on_close
         self._package_name = package_name
         self._store = self._init_store()
         self._run_called = False
@@ -123,20 +124,20 @@
             self._project_path / settings.CONF_SOURCE
         )
 
     @classmethod
     def create(  # pylint: disable=too-many-arguments
         cls,
         package_name: str = None,
-        project_path: Union[Path, str] = None,
+        project_path: Path | str | None = None,
         save_on_close: bool = True,
         env: str = None,
-        extra_params: Dict[str, Any] = None,
-        conf_source: Optional[str] = None,
-    ) -> "KedroSession":
+        extra_params: dict[str, Any] = None,
+        conf_source: str | None = None,
+    ) -> KedroSession:
         """Create a new instance of ``KedroSession`` with the session data.
 
         Args:
             package_name: Package name for the Kedro project the session is
                 created for. The package_name argument will be removed in Kedro `0.19.0`.
             project_path: Path to the project root directory. Default is
                 current working directory Path.cwd().
@@ -159,15 +160,15 @@
             session_id=generate_timestamp(),
             save_on_close=save_on_close,
             conf_source=conf_source,
         )
 
         # have to explicitly type session_data otherwise mypy will complain
         # possibly related to this: https://github.com/python/mypy/issues/1430
-        session_data: Dict[str, Any] = {
+        session_data: dict[str, Any] = {
             "package_name": session._package_name,
             "project_path": session._project_path,
             "session_id": session.session_id,
         }
 
         ctx = click.get_current_context(silent=True)
         if ctx:
@@ -192,18 +193,16 @@
         # We need ConfigLoader and env to setup logging correctly
         session._setup_logging()
         session_data.update(**_describe_git(session._project_path))
         session._store.update(session_data)
 
         return session
 
-    def _get_logging_config(self) -> Dict[str, Any]:
+    def _get_logging_config(self) -> dict[str, Any]:
         logging_config = self._get_config_loader()["logging"]
-        if isinstance(logging_config, omegaconf.DictConfig):
-            logging_config = OmegaConf.to_container(logging_config)
         # turn relative paths in logging config into absolute path
         # before initialising loggers
         logging_config = _convert_paths_to_absolute_posix(
             project_path=self._project_path, conf_dictionary=logging_config
         )
         return logging_config
 
@@ -250,15 +249,15 @@
         self._store["exception"] = exc_data
 
     @property
     def _logger(self) -> logging.Logger:
         return logging.getLogger(__name__)
 
     @property
-    def store(self) -> Dict[str, Any]:
+    def store(self) -> dict[str, Any]:
         """Return a copy of internal store."""
         return dict(self._store)
 
     def load_context(self) -> KedroContext:
         """An instance of the project context."""
         env = self.store.get("env")
         extra_params = self.store.get("extra_params")
@@ -313,17 +312,17 @@
         tags: Iterable[str] = None,
         runner: AbstractRunner = None,
         node_names: Iterable[str] = None,
         from_nodes: Iterable[str] = None,
         to_nodes: Iterable[str] = None,
         from_inputs: Iterable[str] = None,
         to_outputs: Iterable[str] = None,
-        load_versions: Dict[str, str] = None,
+        load_versions: dict[str, str] = None,
         namespace: str = None,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """Runs the pipeline with a specified runner.
 
         Args:
             pipeline_name: Name of the pipeline that is being run.
             tags: An optional list of node tags which should be used to
                 filter the nodes of the ``Pipeline``. If specified, only the nodes
                 containing *any* of these tags will be run.
```

### Comparing `kedro-0.18.8/kedro/framework/session/shelvestore.py` & `kedro-0.18.9/kedro/framework/session/shelvestore.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """This module implements a dict-like store object used to persist Kedro sessions.
 This module is separated from store.py to ensure it's only imported when exported explicitly.
 """
+from __future__ import annotations
+
 import dbm
 import shelve
 from multiprocessing import Lock
 from pathlib import Path
-from typing import Any, Dict
+from typing import Any
 
 from .store import BaseSessionStore
 
 
 class ShelveStore(BaseSessionStore):
     """Stores the session data on disk using `shelve` package.
     This is an example of how to persist data on disk."""
 
     _lock = Lock()
 
     @property
     def _location(self) -> Path:
         return Path(self._path).expanduser().resolve() / self._session_id / "store"
 
-    def read(self) -> Dict[str, Any]:
+    def read(self) -> dict[str, Any]:
         """Read the data from disk using `shelve` package."""
-        data: Dict[str, Any] = {}
+        data: dict[str, Any] = {}
         try:
             with shelve.open(str(self._location), flag="r") as _sh:  # nosec
                 data = dict(_sh)
         except dbm.error:
             pass
         return data
```

### Comparing `kedro-0.18.8/kedro/framework/session/store.py` & `kedro-0.18.9/kedro/framework/session/store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """This module implements a dict-like store object used to persist Kedro sessions."""
+from __future__ import annotations
+
 import logging
 from collections import UserDict
-from typing import Any, Dict
+from typing import Any
 
 
 class BaseSessionStore(UserDict):
     """``BaseSessionStore`` is the base class for all session stores.
     ``BaseSessionStore`` is an ephemeral store implementation that doesn't
     persist the session data.
     """
@@ -15,15 +17,15 @@
         self._session_id = session_id
         super().__init__(self.read())
 
     @property
     def _logger(self) -> logging.Logger:
         return logging.getLogger(__name__)
 
-    def read(self) -> Dict[str, Any]:
+    def read(self) -> dict[str, Any]:
         """Read the data from the session store.
 
         Returns:
             A mapping containing the session store data.
         """
         self._logger.debug(
             "'read()' not implemented for '%s'. Assuming empty store.",
```

### Comparing `kedro-0.18.8/kedro/framework/startup.py` & `kedro-0.18.9/kedro/framework/startup.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/io/__init__.py` & `kedro-0.18.9/kedro/io/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/io/cached_dataset.py` & `kedro-0.18.9/kedro/io/cached_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 This module contains ``CachedDataSet``, a dataset wrapper which caches in memory the data saved,
 so that the user avoids io operations with slow storage media
 """
+from __future__ import annotations
+
 import logging
-from typing import Any, Dict, Union
+from typing import Any
 
 from kedro.io.core import VERSIONED_FLAG_KEY, AbstractDataSet, Version
 from kedro.io.memory_dataset import MemoryDataSet
 
 
 class CachedDataSet(AbstractDataSet):
     """``CachedDataSet`` is a dataset wrapper which caches in memory the data saved,
@@ -30,30 +32,33 @@
     # this dataset cannot be used with ``ParallelRunner``,
     # therefore it has the attribute ``_SINGLE_PROCESS = True``
     # for parallelism please consider ``ThreadRunner`` instead
     _SINGLE_PROCESS = True
 
     def __init__(
         self,
-        dataset: Union[AbstractDataSet, Dict],
+        dataset: AbstractDataSet | dict,
         version: Version = None,
         copy_mode: str = None,
+        metadata: dict[str, Any] = None,
     ):
         """Creates a new instance of ``CachedDataSet`` pointing to the
         provided Python object.
 
         Args:
             dataset: A Kedro DataSet object or a dictionary to cache.
             version: If specified, should be an instance of
                 ``kedro.io.core.Version``. If its ``load`` attribute is
                 None, the latest version will be loaded. If its ``save``
                 attribute is None, save version will be autogenerated.
             copy_mode: The copy mode used to copy the data. Possible
                 values are: "deepcopy", "copy" and "assign". If not
                 provided, it is inferred based on the data type.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Raises:
             ValueError: If the provided dataset is not a valid dict/YAML
                 representation of a dataset or an actual dataset.
         """
         if isinstance(dataset, dict):
             self._dataset = self._from_config(dataset, version)
@@ -61,14 +66,15 @@
             self._dataset = dataset
         else:
             raise ValueError(
                 "The argument type of 'dataset' should be either a dict/YAML "
                 "representation of the dataset, or the actual dataset object."
             )
         self._cache = MemoryDataSet(copy_mode=copy_mode)
+        self.metadata = metadata
 
     def _release(self) -> None:
         self._cache.release()
         self._dataset.release()
 
     @staticmethod
     def _from_config(config, version):
@@ -80,15 +86,15 @@
         if version:
             config[VERSIONED_FLAG_KEY] = True
             return AbstractDataSet.from_config(
                 "_cached", config, version.load, version.save
             )
         return AbstractDataSet.from_config("_cached", config)
 
-    def _describe(self) -> Dict[str, Any]:
+    def _describe(self) -> dict[str, Any]:
         return {
             "dataset": self._dataset._describe(),  # pylint: disable=protected-access
             "cache": self._cache._describe(),  # pylint: disable=protected-access
         }
 
     def _load(self):
         data = self._cache.load() if self._cache.exists() else self._dataset.load()
```

### Comparing `kedro-0.18.8/kedro/io/core.py` & `kedro-0.18.9/kedro/io/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """This module provides a set of classes which underpin the data loading and
 saving functionality provided by ``kedro.io``.
 """
+from __future__ import annotations
 
 import abc
 import copy
 import logging
 import re
 import warnings
 from collections import namedtuple
 from datetime import datetime, timezone
 from functools import partial
 from glob import iglob
 from operator import attrgetter
 from pathlib import Path, PurePath, PurePosixPath
-from typing import Any, Callable, Dict, Generic, List, Optional, Tuple, Type, TypeVar
+from typing import Any, Callable, Generic, TypeVar
 from urllib.parse import urlsplit
 
 from cachetools import Cache, cachedmethod
 from cachetools.keys import hashkey
 
 from kedro.utils import load_obj
 
@@ -111,20 +112,20 @@
             filepath: data/01_raw/my_data.csv
             param1: <param1-value> # param1 is a required argument
             # param2 will be True by default
     """
 
     @classmethod
     def from_config(
-        cls: Type,
+        cls: type,
         name: str,
-        config: Dict[str, Any],
+        config: dict[str, Any],
         load_version: str = None,
         save_version: str = None,
-    ) -> "AbstractDataSet":
+    ) -> AbstractDataSet:
         """Create a data set instance using the configuration provided.
 
         Args:
             name: Data set name.
             config: Data set config dictionary.
             load_version: Version string to be used for ``load`` operation if
                 the data set is versioned. Has no effect on the data set
@@ -258,15 +259,15 @@
     def _save(self, data: _DI) -> None:
         raise NotImplementedError(
             f"'{self.__class__.__name__}' is a subclass of AbstractDataSet and "
             f"it must implement the '_save' method"
         )
 
     @abc.abstractmethod
-    def _describe(self) -> Dict[str, Any]:
+    def _describe(self) -> dict[str, Any]:
         raise NotImplementedError(
             f"'{self.__class__.__name__}' is a subclass of AbstractDataSet and "
             f"it must implement the '_describe' method"
         )
 
     def exists(self) -> bool:
         """Checks whether a data set's output already exists by calling
@@ -308,15 +309,15 @@
         except Exception as exc:
             message = f"Failed during release for data set {str(self)}.\n{str(exc)}"
             raise DataSetError(message) from exc
 
     def _release(self) -> None:
         pass
 
-    def _copy(self, **overwrite_params) -> "AbstractDataSet":
+    def _copy(self, **overwrite_params) -> AbstractDataSet:
         dataset_copy = copy.deepcopy(self)
         for name, value in overwrite_params.items():
             setattr(dataset_copy, name, value)
         return dataset_copy
 
 
 def generate_timestamp() -> str:
@@ -350,16 +351,16 @@
 # `kedro_datasets` is probed before `kedro.extras.datasets`,
 # hence the DeprecationWarning will not be shown
 # if the dataset is available in the former
 _DEFAULT_PACKAGES = ["kedro.io.", "kedro_datasets.", "kedro.extras.datasets.", ""]
 
 
 def parse_dataset_definition(
-    config: Dict[str, Any], load_version: str = None, save_version: str = None
-) -> Tuple[Type[AbstractDataSet], Dict[str, Any]]:
+    config: dict[str, Any], load_version: str = None, save_version: str = None
+) -> tuple[type[AbstractDataSet], dict[str, Any]]:
     """Parse and instantiate a dataset class using the configuration provided.
 
     Args:
         config: Data set config dictionary. It *must* contain the `type` key
             with fully qualified class name.
         load_version: Version string to be used for ``load`` operation if
                 the data set is versioned. Has no effect on the data set
@@ -420,15 +421,15 @@
         class_obj, VERSIONED_FLAG_KEY, False
     ):
         config[VERSION_KEY] = Version(load_version, save_version)
 
     return class_obj, config
 
 
-def _load_obj(class_path: str) -> Optional[object]:
+def _load_obj(class_path: str) -> object | None:
     mod_path, _, class_name = class_path.rpartition(".")
     try:
         available_classes = load_obj(f"{mod_path}.__all__")
     # ModuleNotFoundError: When `load_obj` can't find `mod_path` (e.g `kedro.io.pandas`)
     #                      this is because we try a combination of all prefixes.
     # AttributeError: When `load_obj` manages to load `mod_path` but it doesn't have an
     #                 `__all__` attribute -- either because it's a custom or a kedro.io dataset
@@ -502,17 +503,17 @@
             param1: <param1-value> # param1 is a required argument
             # param2 will be True by default
     """
 
     def __init__(
         self,
         filepath: PurePosixPath,
-        version: Optional[Version],
+        version: Version | None,
         exists_function: Callable[[str], bool] = None,
-        glob_function: Callable[[str], List[str]] = None,
+        glob_function: Callable[[str], list[str]] = None,
     ):
         """Creates a new instance of ``AbstractVersionedDataSet``.
 
         Args:
             filepath: Filepath in POSIX format to a file.
             version: If specified, should be an instance of
                 ``kedro.io.core.Version``. If its ``load`` attribute is
@@ -556,15 +557,15 @@
     # 'key' is set to prevent cache key overlapping for load and save:
     # https://cachetools.readthedocs.io/en/stable/#cachetools.cachedmethod
     @cachedmethod(cache=attrgetter("_version_cache"), key=partial(hashkey, "save"))
     def _fetch_latest_save_version(self) -> str:  # pylint: disable=no-self-use
         """Generate and cache the current save version"""
         return generate_timestamp()
 
-    def resolve_load_version(self) -> Optional[str]:
+    def resolve_load_version(self) -> str | None:
         """Compute the version the dataset should be loaded with."""
         if not self._version:
             return None
         if self._version.load:
             return self._version.load
         return self._fetch_latest_load_version()
 
@@ -572,15 +573,15 @@
         if not self._version:
             # When versioning is disabled, load from original filepath
             return self._filepath
 
         load_version = self.resolve_load_version()
         return self._get_versioned_path(load_version)  # type: ignore
 
-    def resolve_save_version(self) -> Optional[str]:
+    def resolve_save_version(self) -> str | None:
         """Compute the version the dataset should be saved with."""
         if not self._version:
             return None
         if self._version.save:
             return self._version.save
         return self._fetch_latest_save_version()
 
@@ -655,15 +656,15 @@
             raise DataSetError(message) from exc
 
     def _release(self) -> None:
         super()._release()
         self._version_cache.clear()
 
 
-def _parse_filepath(filepath: str) -> Dict[str, str]:
+def _parse_filepath(filepath: str) -> dict[str, str]:
     """Split filepath on protocol and path. Based on `fsspec.utils.infer_storage_options`.
 
     Args:
         filepath: Either local absolute file path or URL (s3://bucket/file.csv)
 
     Returns:
         Parsed filepath.
@@ -696,15 +697,15 @@
         # 'username' field of a URL (@ syntax), so we need to add it to the path
         if protocol == "abfss" and parsed_path.username:
             options["path"] = parsed_path.username + "@" + options["path"]
 
     return options
 
 
-def get_protocol_and_path(filepath: str, version: Version = None) -> Tuple[str, str]:
+def get_protocol_and_path(filepath: str, version: Version = None) -> tuple[str, str]:
     """Parses filepath on protocol and path.
 
     Args:
         filepath: raw filepath e.g.: `gcs://bucket/test.json`.
         version: instance of ``kedro.io.core.Version`` or None.
 
     Returns:
```

### Comparing `kedro-0.18.8/kedro/io/data_catalog.py` & `kedro-0.18.9/kedro/io/data_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """``DataCatalog`` stores instances of ``AbstractDataSet`` implementations to
 provide ``load`` and ``save`` capabilities from anywhere in the program. To
 use a ``DataCatalog``, you need to instantiate it with a dictionary of data
 sets. Then it will act as a single point of reference for your calls,
 relaying load and save functions to the underlying data sets.
 """
+from __future__ import annotations
+
 import copy
 import difflib
 import logging
 import re
 from collections import defaultdict
-from typing import Any, Dict, List, Optional, Set, Type, Union
+from typing import Any
 
 from kedro.io.core import (
     AbstractDataSet,
     AbstractVersionedDataSet,
     DataSetAlreadyExistsError,
     DataSetError,
     DataSetNotFoundError,
@@ -24,16 +26,16 @@
 
 CATALOG_KEY = "catalog"
 CREDENTIALS_KEY = "credentials"
 WORDS_REGEX_PATTERN = re.compile(r"\W+")
 
 
 def _get_credentials(
-    credentials_name: str, credentials: Dict[str, Any]
-) -> Dict[str, Any]:
+    credentials_name: str, credentials: dict[str, Any]
+) -> dict[str, Any]:
     """Return a set of credentials from the provided credentials dict.
 
     Args:
         credentials_name: Credentials name.
         credentials: A dictionary with all credentials.
 
     Returns:
@@ -52,16 +54,16 @@
             "catalog and credentials configuration. See "
             "https://kedro.readthedocs.io/en/stable/kedro.io.DataCatalog.html "
             "for an example."
         ) from exc
 
 
 def _resolve_credentials(
-    config: Dict[str, Any], credentials: Dict[str, Any]
-) -> Dict[str, Any]:
+    config: dict[str, Any], credentials: dict[str, Any]
+) -> dict[str, Any]:
     """Return the dataset configuration where credentials are resolved using
     credentials dictionary provided.
 
     Args:
         config: Original dataset config, which may contain unresolved credentials.
         credentials: A dictionary with all credentials.
 
@@ -93,15 +95,15 @@
 
 
 class _FrozenDatasets:
     """Helper class to access underlying loaded datasets"""
 
     def __init__(
         self,
-        *datasets_collections: Union["_FrozenDatasets", Dict[str, AbstractDataSet]],
+        *datasets_collections: _FrozenDatasets | dict[str, AbstractDataSet],
     ):
         """Return a _FrozenDatasets instance from some datasets collections.
         Each collection could either be another _FrozenDatasets or a dictionary.
         """
         for collection in datasets_collections:
             if isinstance(collection, _FrozenDatasets):
                 self.__dict__.update(collection.__dict__)
@@ -132,17 +134,17 @@
     a dictionary of data sets. Then it will act as a single point of reference
     for your calls, relaying load and save functions
     to the underlying data sets.
     """
 
     def __init__(
         self,
-        data_sets: Dict[str, AbstractDataSet] = None,
-        feed_dict: Dict[str, Any] = None,
-        layers: Dict[str, Set[str]] = None,
+        data_sets: dict[str, AbstractDataSet] = None,
+        feed_dict: dict[str, Any] = None,
+        layers: dict[str, set[str]] = None,
     ) -> None:
         """``DataCatalog`` stores instances of ``AbstractDataSet``
         implementations to provide ``load`` and ``save`` capabilities from
         anywhere in the program. To use a ``DataCatalog``, you need to
         instantiate it with a dictionary of data sets. Then it will act as a
         single point of reference for your calls, relaying load and save
         functions to the underlying data sets.
@@ -175,20 +177,20 @@
 
     @property
     def _logger(self):
         return logging.getLogger(__name__)
 
     @classmethod
     def from_config(
-        cls: Type,
-        catalog: Optional[Dict[str, Dict[str, Any]]],
-        credentials: Dict[str, Dict[str, Any]] = None,
-        load_versions: Dict[str, str] = None,
+        cls: type,
+        catalog: dict[str, dict[str, Any]] | None,
+        credentials: dict[str, dict[str, Any]] = None,
+        load_versions: dict[str, str] = None,
         save_version: str = None,
-    ) -> "DataCatalog":
+    ) -> DataCatalog:
         """Create a ``DataCatalog`` instance from configuration. This is a
         factory method used to provide developers with a way to instantiate
         ``DataCatalog`` with configuration parsed from configuration files.
 
         Args:
             catalog: A dictionary whose keys are the data set names and
                 the values are dictionaries with the constructor arguments
@@ -263,15 +265,15 @@
         missing_keys = load_versions.keys() - catalog.keys()
         if missing_keys:
             raise DataSetNotFoundError(
                 f"'load_versions' keys [{', '.join(sorted(missing_keys))}] "
                 f"are not found in the catalog."
             )
 
-        layers: Dict[str, Set[str]] = defaultdict(set)
+        layers: dict[str, set[str]] = defaultdict(set)
         for ds_name, ds_config in catalog.items():
             ds_layer = ds_config.pop("layer", None)
             if ds_layer is not None:
                 layers[ds_layer].add(ds_name)
 
             ds_config = _resolve_credentials(ds_config, credentials)
             data_sets[ds_name] = AbstractDataSet.from_config(
@@ -449,15 +451,15 @@
                 raise DataSetAlreadyExistsError(
                     f"DataSet '{data_set_name}' has already been registered"
                 )
         self._data_sets[data_set_name] = data_set
         self.datasets = _FrozenDatasets(self.datasets, {data_set_name: data_set})
 
     def add_all(
-        self, data_sets: Dict[str, AbstractDataSet], replace: bool = False
+        self, data_sets: dict[str, AbstractDataSet], replace: bool = False
     ) -> None:
         """Adds a group of new data sets to the ``DataCatalog``.
 
         Args:
             data_sets: A dictionary of ``DataSet`` names and data set
                 instances.
             replace: Specifies whether to replace an existing ``DataSet``
@@ -483,15 +485,15 @@
             >>> io.add_all(additional)
             >>>
             >>> assert io.list() == ["cars", "planes", "boats"]
         """
         for name, data_set in data_sets.items():
             self.add(name, data_set, replace)
 
-    def add_feed_dict(self, feed_dict: Dict[str, Any], replace: bool = False) -> None:
+    def add_feed_dict(self, feed_dict: dict[str, Any], replace: bool = False) -> None:
         """Adds instances of ``MemoryDataSet``, containing the data provided
         through feed_dict.
 
         Args:
             feed_dict: A feed dict with data to be added in memory.
             replace: Specifies whether to replace an existing ``DataSet``
                 with the same name is allowed.
@@ -516,15 +518,15 @@
             if isinstance(feed_dict[data_set_name], AbstractDataSet):
                 data_set = feed_dict[data_set_name]
             else:
                 data_set = MemoryDataSet(data=feed_dict[data_set_name])
 
             self.add(data_set_name, data_set, replace)
 
-    def list(self, regex_search: Optional[str] = None) -> List[str]:
+    def list(self, regex_search: str | None = None) -> list[str]:
         """
         List of all ``DataSet`` names registered in the catalog.
         This can be filtered by providing an optional regular expression
         which will only return matching keys.
 
         Args:
             regex_search: An optional regular expression which can be provided
@@ -561,15 +563,15 @@
 
         except re.error as exc:
             raise SyntaxError(
                 f"Invalid regular expression provided: '{regex_search}'"
             ) from exc
         return [dset_name for dset_name in self._data_sets if pattern.search(dset_name)]
 
-    def shallow_copy(self) -> "DataCatalog":
+    def shallow_copy(self) -> DataCatalog:
         """Returns a shallow copy of the current object.
 
         Returns:
             Copy of the current object.
         """
         return DataCatalog(data_sets=self._data_sets, layers=self.layers)
```

### Comparing `kedro-0.18.8/kedro/io/lambda_dataset.py` & `kedro-0.18.9/kedro/io/lambda_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """``LambdaDataSet`` is an implementation of ``AbstractDataSet`` which allows for
 providing custom load, save, and exists methods without extending
 ``AbstractDataSet``.
 """
-from typing import Any, Callable, Dict, Optional
+from __future__ import annotations
+
+from typing import Any, Callable
 
 from kedro.io.core import AbstractDataSet, DataSetError
 
 
 class LambdaDataSet(AbstractDataSet):
     """``LambdaDataSet`` loads and saves data to a data set.
     It relies on delegating to specific implementation such as csv, sql, etc.
@@ -25,15 +27,15 @@
         >>> file_name = "test.csv"
         >>> def load() -> pd.DataFrame:
         >>>     raise FileNotFoundError("'{}' csv file not found."
         >>>                             .format(file_name))
         >>> data_set = LambdaDataSet(load, None)
     """
 
-    def _describe(self) -> Dict[str, Any]:
+    def _describe(self) -> dict[str, Any]:
         def _to_str(func):
             if not func:
                 return None
             try:
                 return f"<{func.__module__}.{func.__name__}>"
             except AttributeError:  # pragma: no cover
                 return str(func)
@@ -70,29 +72,33 @@
 
     def _release(self) -> None:
         if not self.__release:
             super()._release()
         else:
             self.__release()
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
-        load: Optional[Callable[[], Any]],
-        save: Optional[Callable[[Any], None]],
+        load: Callable[[], Any] | None,
+        save: Callable[[Any], None] | None,
         exists: Callable[[], bool] = None,
         release: Callable[[], None] = None,
+        metadata: dict[str, Any] = None,
     ):
         """Creates a new instance of ``LambdaDataSet`` with references to the
         required input/output data set methods.
 
         Args:
             load: Method to load data from a data set.
             save: Method to save data to a data set.
             exists: Method to check whether output data already exists.
             release: Method to release any cached information.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Raises:
             DataSetError: If a method is specified, but is not a Callable.
 
         """
 
         for name, value in [
@@ -107,7 +113,8 @@
                     f"Object of type '{value.__class__.__name__}' provided instead."
                 )
 
         self.__load = load
         self.__save = save
         self.__exists = exists
         self.__release = release
+        self.metadata = metadata
```

### Comparing `kedro-0.18.8/kedro/io/memory_dataset.py` & `kedro-0.18.9/kedro/io/memory_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """``MemoryDataSet`` is a data set implementation which handles in-memory data.
 """
+from __future__ import annotations
 
 import copy
-from typing import Any, Dict
+from typing import Any
 
 from kedro.io.core import AbstractDataSet, DataSetError
 
 _EMPTY = object()
 
 
 class MemoryDataSet(AbstractDataSet):
@@ -29,26 +30,31 @@
         >>> new_data = pd.DataFrame({'col1': [1, 2], 'col2': [4, 5]})
         >>> data_set.save(new_data)
         >>> reloaded_data = data_set.load()
         >>> assert reloaded_data.equals(new_data)
 
     """
 
-    def __init__(self, data: Any = _EMPTY, copy_mode: str = None):
+    def __init__(
+        self, data: Any = _EMPTY, copy_mode: str = None, metadata: dict[str, Any] = None
+    ):
         """Creates a new instance of ``MemoryDataSet`` pointing to the
         provided Python object.
 
         Args:
             data: Python object containing the data.
             copy_mode: The copy mode used to copy the data. Possible
                 values are: "deepcopy", "copy" and "assign". If not
                 provided, it is inferred based on the data type.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         self._data = _EMPTY
         self._copy_mode = copy_mode
+        self.metadata = metadata
         if data is not _EMPTY:
             self._save(data)
 
     def _load(self) -> Any:
         if self._data is _EMPTY:
             raise DataSetError("Data for MemoryDataSet has not been saved yet.")
 
@@ -62,15 +68,15 @@
 
     def _exists(self) -> bool:
         return self._data is not _EMPTY
 
     def _release(self) -> None:
         self._data = _EMPTY
 
-    def _describe(self) -> Dict[str, Any]:
+    def _describe(self) -> dict[str, Any]:
         if self._data is not _EMPTY:
             return {"data": f"<{type(self._data).__name__}>"}
         # the string representation of datasets leaves out __init__
         # arguments that are empty/None, equivalent here is _EMPTY
         return {"data": None}  # pragma: no cover
```

### Comparing `kedro-0.18.8/kedro/io/partitioned_dataset.py` & `kedro-0.18.9/kedro/io/partitioned_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """``PartitionedDataSet`` loads and saves partitioned file-like data using the
 underlying dataset definition. It also uses `fsspec` for filesystem level operations.
 """
+from __future__ import annotations
+
 import operator
 from copy import deepcopy
-from typing import Any, Callable, Dict, List, Type, Union
+from typing import Any, Callable
 from urllib.parse import urlparse
 from warnings import warn
 
 from cachetools import Cache, cachedmethod
 
 from kedro.io.core import (
     VERSION_KEY,
@@ -128,21 +130,22 @@
         >>> data_set.save({"new/partition.csv": new_data})
 
     """
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
         path: str,
-        dataset: Union[str, Type[AbstractDataSet], Dict[str, Any]],
+        dataset: str | type[AbstractDataSet] | dict[str, Any],
         filepath_arg: str = "filepath",
         filename_suffix: str = "",
-        credentials: Dict[str, Any] = None,
-        load_args: Dict[str, Any] = None,
-        fs_args: Dict[str, Any] = None,
+        credentials: dict[str, Any] = None,
+        load_args: dict[str, Any] = None,
+        fs_args: dict[str, Any] = None,
         overwrite: bool = False,
+        metadata: dict[str, Any] = None,
     ):
         """Creates a new instance of ``PartitionedDataSet``.
 
         Args:
             path: Path to the folder containing partitioned data.
                 If path starts with the protocol (e.g., ``s3://``) then the
                 corresponding ``fsspec`` concrete filesystem implementation will
@@ -173,28 +176,31 @@
                 All possible credentials management scenarios are documented here:
                 https://kedro.readthedocs.io/en/stable/data/kedro_io.html#partitioned-dataset-credentials
             load_args: Keyword arguments to be passed into ``find()`` method of
                 the filesystem implementation.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``)
             overwrite: If True, any existing partitions will be removed.
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Raises:
             DataSetError: If versioning is enabled for the underlying dataset.
         """
         # pylint: disable=import-outside-toplevel
         from fsspec.utils import infer_storage_options  # for performance reasons
 
         super().__init__()
 
         self._path = path
         self._filename_suffix = filename_suffix
         self._overwrite = overwrite
         self._protocol = infer_storage_options(self._path)["protocol"]
         self._partition_cache: Cache = Cache(maxsize=1)
+        self.metadata = metadata
 
         dataset = dataset if isinstance(dataset, dict) else {"type": dataset}
         self._dataset_type, self._dataset_config = parse_dataset_definition(dataset)
         if VERSION_KEY in self._dataset_config:
             raise DataSetError(
                 f"'{self.__class__.__name__}' does not support versioning of the "
                 f"underlying dataset. Please remove '{VERSIONED_FLAG_KEY}' flag from "
@@ -245,15 +251,15 @@
     @property
     def _normalized_path(self) -> str:
         if self._protocol in S3_PROTOCOLS:
             return urlparse(self._path)._replace(scheme="s3").geturl()
         return self._path
 
     @cachedmethod(cache=operator.attrgetter("_partition_cache"))
-    def _list_partitions(self) -> List[str]:
+    def _list_partitions(self) -> list[str]:
         return [
             path
             for path in self._filesystem.find(self._normalized_path, **self._load_args)
             if path.endswith(self._filename_suffix)
         ]
 
     def _join_protocol(self, path: str) -> str:
@@ -272,15 +278,15 @@
     def _path_to_partition(self, path: str) -> str:
         dir_path = self._filesystem._strip_protocol(self._normalized_path)
         path = path.split(dir_path, 1).pop().lstrip(self._sep)
         if self._filename_suffix and path.endswith(self._filename_suffix):
             path = path[: -len(self._filename_suffix)]
         return path
 
-    def _load(self) -> Dict[str, Callable[[], Any]]:
+    def _load(self) -> dict[str, Callable[[], Any]]:
         partitions = {}
 
         for partition in self._list_partitions():
             kwargs = deepcopy(self._dataset_config)
             # join the protocol back since PySpark may rely on it
             kwargs[self._filepath_arg] = self._join_protocol(partition)
             dataset = self._dataset_type(**kwargs)  # type: ignore
@@ -288,30 +294,30 @@
             partitions[partition_id] = dataset.load
 
         if not partitions:
             raise DataSetError(f"No partitions found in '{self._path}'")
 
         return partitions
 
-    def _save(self, data: Dict[str, Any]) -> None:
+    def _save(self, data: dict[str, Any]) -> None:
         if self._overwrite and self._filesystem.exists(self._normalized_path):
             self._filesystem.rm(self._normalized_path, recursive=True)
 
         for partition_id, partition_data in sorted(data.items()):
             kwargs = deepcopy(self._dataset_config)
             partition = self._partition_to_path(partition_id)
             # join the protocol back since tools like PySpark may rely on it
             kwargs[self._filepath_arg] = self._join_protocol(partition)
             dataset = self._dataset_type(**kwargs)  # type: ignore
             if callable(partition_data):
                 partition_data = partition_data()
             dataset.save(partition_data)
         self._invalidate_caches()
 
-    def _describe(self) -> Dict[str, Any]:
+    def _describe(self) -> dict[str, Any]:
         clean_dataset_config = (
             {k: v for k, v in self._dataset_config.items() if k != CREDENTIALS_KEY}
             if isinstance(self._dataset_config, dict)
             else self._dataset_config
         )
         return {
             "path": self._path,
@@ -370,21 +376,22 @@
     DEFAULT_CHECKPOINT_TYPE = "kedro.extras.datasets.text.TextDataSet"
     DEFAULT_CHECKPOINT_FILENAME = "CHECKPOINT"
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         path: str,
-        dataset: Union[str, Type[AbstractDataSet], Dict[str, Any]],
-        checkpoint: Union[str, Dict[str, Any]] = None,
+        dataset: str | type[AbstractDataSet] | dict[str, Any],
+        checkpoint: str | dict[str, Any] | None = None,
         filepath_arg: str = "filepath",
         filename_suffix: str = "",
-        credentials: Dict[str, Any] = None,
-        load_args: Dict[str, Any] = None,
-        fs_args: Dict[str, Any] = None,
+        credentials: dict[str, Any] = None,
+        load_args: dict[str, Any] = None,
+        fs_args: dict[str, Any] = None,
+        metadata: dict[str, Any] = None,
     ):
 
         """Creates a new instance of ``IncrementalDataSet``.
 
         Args:
             path: Path to the folder containing partitioned data.
                 If path starts with the protocol (e.g., ``s3://``) then the
@@ -423,14 +430,16 @@
                 credentials spec, then such spec will take precedence.
                 All possible credentials management scenarios are documented here:
                 https://kedro.readthedocs.io/en/stable/data/kedro_io.html#partitioned-dataset-credentials
             load_args: Keyword arguments to be passed into ``find()`` method of
                 the filesystem implementation.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``).
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Raises:
             DataSetError: If versioning is enabled for the underlying dataset.
         """
 
         super().__init__(
             path=path,
@@ -440,23 +449,24 @@
             credentials=credentials,
             load_args=load_args,
             fs_args=fs_args,
         )
 
         self._checkpoint_config = self._parse_checkpoint_config(checkpoint)
         self._force_checkpoint = self._checkpoint_config.pop("force_checkpoint", None)
+        self.metadata = metadata
 
         comparison_func = self._checkpoint_config.pop("comparison_func", operator.gt)
         if isinstance(comparison_func, str):
             comparison_func = load_obj(comparison_func)
         self._comparison_func = comparison_func
 
     def _parse_checkpoint_config(
-        self, checkpoint_config: Union[str, Dict[str, Any], None]
-    ) -> Dict[str, Any]:
+        self, checkpoint_config: str | dict[str, Any] | None
+    ) -> dict[str, Any]:
         checkpoint_config = deepcopy(checkpoint_config)
         if isinstance(checkpoint_config, str):
             checkpoint_config = {"force_checkpoint": checkpoint_config}
         checkpoint_config = checkpoint_config or {}
 
         for key in {VERSION_KEY, VERSIONED_FLAG_KEY} & checkpoint_config.keys():
             raise DataSetError(
@@ -479,15 +489,15 @@
                 KEY_PROPAGATION_WARNING,
                 {"keys": CREDENTIALS_KEY, "target": "checkpoint"},
             )
 
         return {**default_config, **checkpoint_config}
 
     @cachedmethod(cache=operator.attrgetter("_partition_cache"))
-    def _list_partitions(self) -> List[str]:
+    def _list_partitions(self) -> list[str]:
         checkpoint = self._read_checkpoint()
         checkpoint_path = (
             self._filesystem._strip_protocol(  # pylint: disable=protected-access
                 self._checkpoint_config[self._filepath_arg]
             )
         )
 
@@ -509,23 +519,23 @@
         )
 
     @property
     def _checkpoint(self) -> AbstractDataSet:
         type_, kwargs = parse_dataset_definition(self._checkpoint_config)
         return type_(**kwargs)  # type: ignore
 
-    def _read_checkpoint(self) -> Union[str, None]:
+    def _read_checkpoint(self) -> str | None:
         if self._force_checkpoint is not None:
             return self._force_checkpoint
         try:
             return self._checkpoint.load()
         except DataSetError:
             return None
 
-    def _load(self) -> Dict[str, Callable[[], Any]]:
+    def _load(self) -> dict[str, Callable[[], Any]]:
         partitions = {}
 
         for partition in self._list_partitions():
             partition_id = self._path_to_partition(partition)
             kwargs = deepcopy(self._dataset_config)
             # join the protocol back since PySpark may rely on it
             kwargs[self._filepath_arg] = self._join_protocol(partition)
```

### Comparing `kedro-0.18.8/kedro/ipython/__init__.py` & `kedro-0.18.9/kedro/ipython/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 This script creates an IPython extension to load Kedro-related variables in
 local scope.
 """
+from __future__ import annotations
+
 import logging
 import sys
 from pathlib import Path
-from typing import Any, Dict, Optional
+from typing import Any
 
 from IPython import get_ipython
 from IPython.core.magic import needs_local_scope, register_line_magic
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
 
 from kedro.framework.cli import load_entry_points
 from kedro.framework.cli.project import PARAMS_ARG_HELP
@@ -56,29 +58,29 @@
 @argument("-e", "--env", type=str, default=None, help=ENV_HELP)
 @argument(
     "--params",
     type=lambda value: _split_params(None, None, value),
     default=None,
     help=PARAMS_ARG_HELP,
 )
-def magic_reload_kedro(line: str, local_ns: Dict[str, Any] = None):
+def magic_reload_kedro(line: str, local_ns: dict[str, Any] = None):
     """
     The `%reload_kedro` IPython line magic.
     See https://kedro.readthedocs.io/en/stable/notebooks_and_ipython/kedro_and_notebooks.html#reload-kedro-line-magic # pylint: disable=line-too-long
     for more.
     """
     args = parse_argstring(magic_reload_kedro, line)
     reload_kedro(args.path, args.env, args.params, local_ns)
 
 
 def reload_kedro(
     path: str = None,
     env: str = None,
-    extra_params: Dict[str, Any] = None,
-    local_namespace: Optional[Dict[str, Any]] = None,
+    extra_params: dict[str, Any] = None,
+    local_namespace: dict[str, Any] | None = None,
 ) -> None:  # pragma: no cover
     """Function that underlies the %reload_kedro Line magic. This should not be imported
     or run directly but instead invoked through %reload_kedro."""
 
     project_path = _resolve_project_path(path, local_namespace)
 
     metadata = bootstrap_project(project_path)
@@ -107,15 +109,15 @@
 
     for line_magic in load_entry_points("line_magic"):
         register_line_magic(needs_local_scope(line_magic))
         logger.info("Registered line magic '%s'", line_magic.__name__)  # type: ignore
 
 
 def _resolve_project_path(
-    path: Optional[str] = None, local_namespace: Optional[Dict[str, Any]] = None
+    path: str | None = None, local_namespace: dict[str, Any] | None = None
 ) -> Path:
     """
     Resolve the project path to use with reload_kedro, updating or adding it
     (in-place) to the local ipython Namespace (``local_namespace``) if necessary.
 
     Arguments:
         path: the path to use as a string object
```

### Comparing `kedro-0.18.8/kedro/ipython/logo-32x32.png` & `kedro-0.18.9/kedro/ipython/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/ipython/logo-64x64.png` & `kedro-0.18.9/kedro/ipython/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/ipython/logo-svg.svg` & `kedro-0.18.9/kedro/ipython/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/pipeline/modular_pipeline.py` & `kedro-0.18.9/kedro/pipeline/modular_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Helper to integrate modular pipelines into a master pipeline."""
+from __future__ import annotations
+
 import copy
-from typing import AbstractSet, Dict, Iterable, List, Set, Union
+from typing import AbstractSet, Iterable
 
 from kedro.pipeline.node import Node
 from kedro.pipeline.pipeline import (
     TRANSCODING_SEPARATOR,
     Pipeline,
     _strip_transcoding,
     _transcode_split,
@@ -71,34 +73,34 @@
         raise ModularPipelineError(
             f"Failed to map datasets and/or parameters: "
             f"{', '.join(sorted(non_existent))}"
         )
 
 
 def _get_dataset_names_mapping(
-    names: Union[str, Set[str], Dict[str, str]] = None
-) -> Dict[str, str]:
+    names: str | set[str] | dict[str, str] | None = None
+) -> dict[str, str]:
     """Take a name or a collection of dataset names
     and turn it into a mapping from the old dataset names to the provided ones if necessary.
 
     Args:
         names: A dataset name or collection of dataset names.
-            When str or Set[str] is provided, the listed names will stay
+            When str or set[str] is provided, the listed names will stay
             the same as they are named in the provided pipeline.
-            When Dict[str, str] is provided, current names will be
+            When dict[str, str] is provided, current names will be
             mapped to new names in the resultant pipeline.
     Returns:
         A dictionary that maps the old dataset names to the provided ones.
     Examples:
         >>> _get_dataset_names_mapping("dataset_name")
         {"dataset_name": "dataset_name"}  # a str name will stay the same
         >>> _get_dataset_names_mapping(set(["ds_1", "ds_2"]))
-        {"ds_1": "ds_1", "ds_2": "ds_2"}  # a Set[str] of names will stay the same
+        {"ds_1": "ds_1", "ds_2": "ds_2"}  # a set[str] of names will stay the same
         >>> _get_dataset_names_mapping({"ds_1": "new_ds_1_name"})
-        {"ds_1": "new_ds_1_name"}  # a Dict[str, str] of names will map key to value
+        {"ds_1": "new_ds_1_name"}  # a dict[str, str] of names will map key to value
     """
     if names is None:
         return {}
     if isinstance(names, str):
         return {names: names}
     if isinstance(names, dict):
         return copy.deepcopy(names)
@@ -108,87 +110,87 @@
 
 def _normalize_param_name(name: str) -> str:
     """Make sure that a param name has a `params:` prefix before passing to the node"""
     return name if name.startswith("params:") else f"params:{name}"
 
 
 def _get_param_names_mapping(
-    names: Union[str, Set[str], Dict[str, str]] = None
-) -> Dict[str, str]:
+    names: str | set[str] | dict[str, str] | None = None
+) -> dict[str, str]:
     """Take a parameter or a collection of parameter names
     and turn it into a mapping from existing parameter names to new ones if necessary.
     It follows the same rule as `_get_dataset_names_mapping` and
     prefixes the keys on the resultant dictionary with `params:` to comply with node's syntax.
 
     Args:
         names: A parameter name or collection of parameter names.
-            When str or Set[str] is provided, the listed names will stay
+            When str or set[str] is provided, the listed names will stay
             the same as they are named in the provided pipeline.
-            When Dict[str, str] is provided, current names will be
+            When dict[str, str] is provided, current names will be
             mapped to new names in the resultant pipeline.
     Returns:
         A dictionary that maps the old parameter names to the provided ones.
     Examples:
         >>> _get_param_names_mapping("param_name")
         {"params:param_name": "params:param_name"}  # a str name will stay the same
         >>> _get_param_names_mapping(set(["param_1", "param_2"]))
-        # a Set[str] of names will stay the same
+        # a set[str] of names will stay the same
         {"params:param_1": "params:param_1", "params:param_2": "params:param_2"}
         >>> _get_param_names_mapping({"param_1": "new_name_for_param_1"})
-        # a Dict[str, str] of names will map key to valu
+        # a dict[str, str] of names will map key to valu
         {"params:param_1": "params:new_name_for_param_1"}
     """
     params = {}
     for name, new_name in _get_dataset_names_mapping(names).items():
         if _is_all_parameters(name):
             params[name] = name  # don't map parameters into params:parameters
         else:
             param_name = _normalize_param_name(name)
             param_new_name = _normalize_param_name(new_name)
             params[param_name] = param_new_name
     return params
 
 
 def pipeline(
-    pipe: Union[Iterable[Union[Node, Pipeline]], Pipeline],
+    pipe: Iterable[Node | Pipeline] | Pipeline,
     *,
-    inputs: Union[str, Set[str], Dict[str, str]] = None,
-    outputs: Union[str, Set[str], Dict[str, str]] = None,
-    parameters: Union[str, Set[str], Dict[str, str]] = None,
-    tags: Union[str, Iterable[str]] = None,
+    inputs: str | set[str] | dict[str, str] | None = None,
+    outputs: str | set[str] | dict[str, str] | None = None,
+    parameters: str | set[str] | dict[str, str] | None = None,
+    tags: str | Iterable[str] | None = None,
     namespace: str = None,
 ) -> Pipeline:
     r"""Create a ``Pipeline`` from a collection of nodes and/or ``Pipeline``\s.
 
     Args:
         pipe: The nodes the ``Pipeline`` will be made of. If you
             provide pipelines among the list of nodes, those pipelines will
             be expanded and all their nodes will become part of this
             new pipeline.
         inputs: A name or collection of input names to be exposed as connection points
             to other pipelines upstream. This is optional; if not provided, the
             pipeline inputs are automatically inferred from the pipeline structure.
-            When str or Set[str] is provided, the listed input names will stay
+            When str or set[str] is provided, the listed input names will stay
             the same as they are named in the provided pipeline.
-            When Dict[str, str] is provided, current input names will be
+            When dict[str, str] is provided, current input names will be
             mapped to new names.
             Must only refer to the pipeline's free inputs.
         outputs: A name or collection of names to be exposed as connection points
             to other pipelines downstream. This is optional; if not provided, the
             pipeline inputs are automatically inferred from the pipeline structure.
-            When str or Set[str] is provided, the listed output names will stay
+            When str or set[str] is provided, the listed output names will stay
             the same as they are named in the provided pipeline.
-            When Dict[str, str] is provided, current output names will be
+            When dict[str, str] is provided, current output names will be
             mapped to new names.
             Can refer to both the pipeline's free outputs, as well as
             intermediate results that need to be exposed.
         parameters: A name or collection of parameters to namespace.
-            When str or Set[str] are provided, the listed parameter names will stay
+            When str or set[str] are provided, the listed parameter names will stay
             the same as they are named in the provided pipeline.
-            When Dict[str, str] is provided, current parameter names will be
+            When dict[str, str] is provided, current parameter names will be
             mapped to new names.
             The parameters can be specified without the `params:` prefix.
         tags: Optional set of tags to be applied to all the pipeline nodes.
         namespace: A prefix to give to all dataset names,
             except those explicitly named with the `inputs`/`outputs`
             arguments, and parameter references (`params:` and `parameters`).
 
@@ -253,16 +255,16 @@
             if predicate(name):
                 return processor(name)
 
         # leave name as is
         return name
 
     def _process_dataset_names(
-        datasets: Union[None, str, List[str], Dict[str, str]]
-    ) -> Union[None, str, List[str], Dict[str, str]]:
+        datasets: None | str | list[str] | dict[str, str]
+    ) -> None | str | list[str] | dict[str, str]:
         if datasets is None:
             return None
         if isinstance(datasets, str):
             return _rename(datasets)
         if isinstance(datasets, list):
             return [_rename(name) for name in datasets]
         if isinstance(datasets, dict):
```

### Comparing `kedro-0.18.8/kedro/pipeline/node.py` & `kedro-0.18.9/kedro/pipeline/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 """This module provides user-friendly functions for creating nodes as parts
 of Kedro pipelines.
 """
+from __future__ import annotations
+
 import copy
 import inspect
 import logging
 import re
 from collections import Counter
-from typing import Any, Callable, Dict, Iterable, List, Optional, Set, Union
+from typing import Any, Callable, Iterable
 from warnings import warn
 
 from more_itertools import spy, unzip
 
 
 class Node:
     """``Node`` is an auxiliary class facilitating the operations required to
     run user-provided functions as part of Kedro pipelines.
     """
 
     def __init__(
         self,
         func: Callable,
-        inputs: Union[None, str, List[str], Dict[str, str]],
-        outputs: Union[None, str, List[str], Dict[str, str]],
+        inputs: None | str | list[str] | dict[str, str],
+        outputs: None | str | list[str] | dict[str, str],
         *,
         name: str = None,
-        tags: Union[str, Iterable[str]] = None,
-        confirms: Union[str, List[str]] = None,
+        tags: str | Iterable[str] | None = None,
+        confirms: str | list[str] | None = None,
         namespace: str = None,
     ):
         """Create a node in the pipeline by providing a function to be called
         along with variable names for inputs and/or outputs.
 
         Args:
             func: A function that corresponds to the node logic.
                 The function should have at least one input or output.
             inputs: The name or the list of the names of variables used as
                 inputs to the function. The number of names should match
                 the number of arguments in the definition of the provided
-                function. When Dict[str, str] is provided, variable names
+                function. When dict[str, str] is provided, variable names
                 will be mapped to function argument names.
             outputs: The name or the list of the names of variables used
                 as outputs to the function. The number of names should match
                 the number of outputs returned by the provided function.
-                When Dict[str, str] is provided, variable names will be mapped
+                When dict[str, str] is provided, variable names will be mapped
                 to the named outputs the function returns.
             name: Optional node name to be used when displaying the node in
                 logs or any other visualisations.
             tags: Optional set of tags to be applied to the node.
             confirms: Optional name or the list of the names of the datasets
                 that should be confirmed. This will result in calling
                 ``confirm()`` method of the corresponding data set instance.
@@ -171,15 +173,15 @@
 
     def __repr__(self):  # pragma: no cover
         return (
             f"Node({self._func_name}, {repr(self._inputs)}, {repr(self._outputs)}, "
             f"{repr(self._name)})"
         )
 
-    def __call__(self, **kwargs) -> Dict[str, Any]:
+    def __call__(self, **kwargs) -> dict[str, Any]:
         return self.run(inputs=kwargs)
 
     @property
     def _func_name(self) -> str:
         name = _get_readable_func_name(self._func)
         if name == "<partial>":
             warn(
@@ -205,24 +207,24 @@
 
         Args:
             func: The new function for node's execution.
         """
         self._func = func
 
     @property
-    def tags(self) -> Set[str]:
+    def tags(self) -> set[str]:
         """Return the tags assigned to the node.
 
         Returns:
             Return the set of all assigned tags to the node.
 
         """
         return set(self._tags)
 
-    def tag(self, tags: Union[str, Iterable[str]]) -> "Node":
+    def tag(self, tags: str | Iterable[str]) -> Node:
         """Create a new ``Node`` which is an exact copy of the current one,
             but with more tags added to it.
 
         Args:
             tags: The tags to be added to the new node.
 
         Returns:
@@ -253,56 +255,56 @@
         """
         if self._name:
             return self._name
 
         return self._func_name.replace("_", " ").title()
 
     @property
-    def namespace(self) -> Optional[str]:
+    def namespace(self) -> str | None:
         """Node's namespace.
 
         Returns:
             String representing node's namespace, typically from outer to inner scopes.
         """
         return self._namespace
 
     @property
-    def inputs(self) -> List[str]:
+    def inputs(self) -> list[str]:
         """Return node inputs as a list, in the order required to bind them properly to
         the node's function.
 
         Returns:
             Node input names as a list.
 
         """
         if isinstance(self._inputs, dict):
             return _dict_inputs_to_list(self._func, self._inputs)
         return _to_list(self._inputs)
 
     @property
-    def outputs(self) -> List[str]:
+    def outputs(self) -> list[str]:
         """Return node outputs as a list preserving the original order
             if possible.
 
         Returns:
             Node output names as a list.
 
         """
         return _to_list(self._outputs)
 
     @property
-    def confirms(self) -> List[str]:
+    def confirms(self) -> list[str]:
         """Return dataset names to confirm as a list.
 
         Returns:
             Dataset names to confirm as a list.
         """
         return _to_list(self._confirms)
 
-    def run(self, inputs: Dict[str, Any] = None) -> Dict[str, Any]:
+    def run(self, inputs: dict[str, Any] = None) -> dict[str, Any]:
         """Run this node using the provided inputs and return its results
         in a dictionary.
 
         Args:
             inputs: Dictionary of inputs as specified at the creation of
                 the node.
 
@@ -350,46 +352,46 @@
             return self._outputs_to_dictionary(outputs)
 
         # purposely catch all exceptions
         except Exception as exc:
             self._logger.error("Node '%s' failed with error: \n%s", str(self), str(exc))
             raise exc
 
-    def _run_with_no_inputs(self, inputs: Dict[str, Any]):
+    def _run_with_no_inputs(self, inputs: dict[str, Any]):
         if inputs:
             raise ValueError(
                 f"Node {str(self)} expected no inputs, "
                 f"but got the following {len(inputs)} input(s) instead: "
                 f"{sorted(inputs.keys())}."
             )
 
         return self._func()
 
-    def _run_with_one_input(self, inputs: Dict[str, Any], node_input: str):
+    def _run_with_one_input(self, inputs: dict[str, Any], node_input: str):
         if len(inputs) != 1 or node_input not in inputs:
             raise ValueError(
                 f"Node {str(self)} expected one input named '{node_input}', "
                 f"but got the following {len(inputs)} input(s) instead: "
                 f"{sorted(inputs.keys())}."
             )
 
         return self._func(inputs[node_input])
 
-    def _run_with_list(self, inputs: Dict[str, Any], node_inputs: List[str]):
+    def _run_with_list(self, inputs: dict[str, Any], node_inputs: list[str]):
         # Node inputs and provided run inputs should completely overlap
         if set(node_inputs) != set(inputs.keys()):
             raise ValueError(
                 f"Node {str(self)} expected {len(node_inputs)} input(s) {node_inputs}, "
                 f"but got the following {len(inputs)} input(s) instead: "
                 f"{sorted(inputs.keys())}."
             )
         # Ensure the function gets the inputs in the correct order
         return self._func(*(inputs[item] for item in node_inputs))
 
-    def _run_with_dict(self, inputs: Dict[str, Any], node_inputs: Dict[str, str]):
+    def _run_with_dict(self, inputs: dict[str, Any], node_inputs: dict[str, str]):
         # Node inputs and provided run inputs should completely overlap
         if set(node_inputs.values()) != set(inputs.keys()):
             raise ValueError(
                 f"Node {str(self)} expected {len(set(node_inputs.values()))} input(s) "
                 f"{sorted(set(node_inputs.values()))}, "
                 f"but got the following {len(inputs)} input(s) instead: "
                 f"{sorted(inputs.keys())}."
@@ -491,19 +493,19 @@
             raise ValueError(
                 f"Failed to create node {self}.\n"
                 f"A node cannot have the same inputs and outputs: "
                 f"{common_in_out}"
             )
 
     @staticmethod
-    def _process_inputs_for_bind(inputs: Union[None, str, List[str], Dict[str, str]]):
+    def _process_inputs_for_bind(inputs: None | str | list[str] | dict[str, str]):
         # Safeguard that we do not mutate list inputs
         inputs = copy.copy(inputs)
-        args: List[str] = []
-        kwargs: Dict[str, str] = {}
+        args: list[str] = []
+        kwargs: dict[str, str] = {}
         if isinstance(inputs, str):
             args = [inputs]
         elif isinstance(inputs, list):
             args = inputs
         elif isinstance(inputs, dict):
             kwargs = inputs
         return args, kwargs
@@ -514,36 +516,36 @@
         f"Invalid Node definition: {msg}\n"
         f"Format should be: node(function, inputs, outputs)"
     )
 
 
 def node(
     func: Callable,
-    inputs: Union[None, str, List[str], Dict[str, str]],
-    outputs: Union[None, str, List[str], Dict[str, str]],
+    inputs: None | str | list[str] | dict[str, str],
+    outputs: None | str | list[str] | dict[str, str],
     *,
     name: str = None,
-    tags: Union[str, Iterable[str]] = None,
-    confirms: Union[str, List[str]] = None,
+    tags: str | Iterable[str] | None = None,
+    confirms: str | list[str] | None = None,
     namespace: str = None,
 ) -> Node:
     """Create a node in the pipeline by providing a function to be called
     along with variable names for inputs and/or outputs.
 
     Args:
         func: A function that corresponds to the node logic. The function
             should have at least one input or output.
         inputs: The name or the list of the names of variables used as inputs
             to the function. The number of names should match the number of
             arguments in the definition of the provided function. When
-            Dict[str, str] is provided, variable names will be mapped to
+            dict[str, str] is provided, variable names will be mapped to
             function argument names.
         outputs: The name or the list of the names of variables used as outputs
             to the function. The number of names should match the number of
-            outputs returned by the provided function. When Dict[str, str]
+            outputs returned by the provided function. When dict[str, str]
             is provided, variable names will be mapped to the named outputs the
             function returns.
         name: Optional node name to be used when displaying the node in logs or
             any other visualisations.
         tags: Optional set of tags to be applied to the node.
         confirms: Optional name or the list of the names of the datasets
             that should be confirmed. This will result in calling ``confirm()``
@@ -558,15 +560,15 @@
     Example:
     ::
 
         >>> import pandas as pd
         >>> import numpy as np
         >>>
         >>> def clean_data(cars: pd.DataFrame,
-        >>>                boats: pd.DataFrame) -> Dict[str, pd.DataFrame]:
+        >>>                boats: pd.DataFrame) -> dict[str, pd.DataFrame]:
         >>>     return dict(cars_df=cars.dropna(), boats_df=boats.dropna())
         >>>
         >>> def halve_dataframe(data: pd.DataFrame) -> List[pd.DataFrame]:
         >>>     return np.array_split(data, 2)
         >>>
         >>> nodes = [
         >>>     node(clean_data,
@@ -588,27 +590,27 @@
         name=name,
         tags=tags,
         confirms=confirms,
         namespace=namespace,
     )
 
 
-def _dict_inputs_to_list(func: Callable[[Any], Any], inputs: Dict[str, str]):
+def _dict_inputs_to_list(func: Callable[[Any], Any], inputs: dict[str, str]):
     """Convert a dict representation of the node inputs to a list, ensuring
     the appropriate order for binding them to the node's function.
     """
     sig = inspect.signature(func, follow_wrapped=False).bind(**inputs)
     return [*sig.args, *sig.kwargs.values()]
 
 
-def _to_list(element: Union[None, str, Iterable[str], Dict[str, str]]) -> List[str]:
+def _to_list(element: None | str | Iterable[str] | dict[str, str]) -> list[str]:
     """Make a list out of node inputs/outputs.
 
     Returns:
-        List[str]: Node input/output names as a list to standardise.
+        list[str]: Node input/output names as a list to standardise.
     """
 
     if element is None:
         return []
     if isinstance(element, str):
         return [element]
     if isinstance(element, dict):
```

### Comparing `kedro-0.18.8/kedro/pipeline/pipeline.py` & `kedro-0.18.9/kedro/pipeline/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """A ``Pipeline`` is a collection of ``Node`` objects which can be executed as
 a Directed Acyclic Graph, sequentially or in parallel. The ``Pipeline`` class
 offers quick access to input dependencies,
 produced outputs and execution order.
 """
+from __future__ import annotations
+
 import copy
 import json
 from collections import Counter, defaultdict
 from itertools import chain
-from typing import Dict, Iterable, List, Set, Tuple, Union
+from typing import Iterable
 
 from toposort import CircularDependencyError as ToposortCircleError
 from toposort import toposort
 
 import kedro
 from kedro.pipeline.node import Node, _to_list
 
 TRANSCODING_SEPARATOR = "@"
 
 
-def _transcode_split(element: str) -> Tuple[str, str]:
+def _transcode_split(element: str) -> tuple[str, str]:
     """Split the name by the transcoding separator.
     If the transcoding part is missing, empty string will be put in.
 
     Returns:
         Node input/output name before the transcoding separator, if present.
     Raises:
         ValueError: Raised if more than one transcoding separator
@@ -73,17 +75,17 @@
     """A ``Pipeline`` defined as a collection of ``Node`` objects. This class
     treats nodes as part of a graph representation and provides inputs,
     outputs and execution order.
     """
 
     def __init__(
         self,
-        nodes: Iterable[Union[Node, "Pipeline"]],
+        nodes: Iterable[Node | Pipeline],
         *,
-        tags: Union[str, Iterable[str]] = None,
+        tags: str | Iterable[str] | None = None,
     ):
         """Initialise ``Pipeline`` with a list of ``Node`` instances.
 
         Args:
             nodes: The iterable of nodes the ``Pipeline`` will be made of. If you
                 provide pipelines among the list of nodes, those pipelines will
                 be expanded and all their nodes will become part of this
@@ -146,21 +148,21 @@
         nodes = [n.tag(_tags) for n in nodes]
 
         self._nodes_by_name = {node.name: node for node in nodes}
         _validate_unique_outputs(nodes)
         _validate_unique_confirms(nodes)
 
         # input -> nodes with input
-        self._nodes_by_input: Dict[str, Set[Node]] = defaultdict(set)
+        self._nodes_by_input: dict[str, set[Node]] = defaultdict(set)
         for node in nodes:
             for input_ in node.inputs:
                 self._nodes_by_input[_strip_transcoding(input_)].add(node)
 
         # output -> node with output
-        self._nodes_by_output: Dict[str, Node] = {}
+        self._nodes_by_output: dict[str, Node] = {}
         for node in nodes:
             for output in node.outputs:
                 self._nodes_by_output[_strip_transcoding(output)] = node
 
         self._nodes = nodes
         self._topo_sorted_nodes = _topologically_sorted(self.node_dependencies)
 
@@ -197,62 +199,62 @@
         return Pipeline(set(self.nodes) & set(other.nodes))
 
     def __or__(self, other):
         if not isinstance(other, Pipeline):
             return NotImplemented
         return Pipeline(set(self.nodes + other.nodes))
 
-    def all_inputs(self) -> Set[str]:
+    def all_inputs(self) -> set[str]:
         """All inputs for all nodes in the pipeline.
 
         Returns:
             All node input names as a Set.
 
         """
         return set.union(set(), *(node.inputs for node in self.nodes))
 
-    def all_outputs(self) -> Set[str]:
+    def all_outputs(self) -> set[str]:
         """All outputs of all nodes in the pipeline.
 
         Returns:
             All node outputs.
 
         """
         return set.union(set(), *(node.outputs for node in self.nodes))
 
-    def _remove_intermediates(self, datasets: Set[str]) -> Set[str]:
+    def _remove_intermediates(self, datasets: set[str]) -> set[str]:
         intermediate = {_strip_transcoding(i) for i in self.all_inputs()} & {
             _strip_transcoding(o) for o in self.all_outputs()
         }
         return {d for d in datasets if _strip_transcoding(d) not in intermediate}
 
-    def inputs(self) -> Set[str]:
+    def inputs(self) -> set[str]:
         """The names of free inputs that must be provided at runtime so that
         the pipeline is runnable. Does not include intermediate inputs which
         are produced and consumed by the inner pipeline nodes. Resolves
         transcoded names where necessary.
 
         Returns:
             The set of free input names needed by the pipeline.
 
         """
         return self._remove_intermediates(self.all_inputs())
 
-    def outputs(self) -> Set[str]:
+    def outputs(self) -> set[str]:
         """The names of outputs produced when the whole pipeline is run.
         Does not include intermediate outputs that are consumed by
         other pipeline nodes. Resolves transcoded names where necessary.
 
         Returns:
             The set of final pipeline outputs.
 
         """
         return self._remove_intermediates(self.all_outputs())
 
-    def data_sets(self) -> Set[str]:
+    def data_sets(self) -> set[str]:
         """The names of all data sets used by the ``Pipeline``,
         including inputs and outputs.
 
         Returns:
             The set of all pipeline data sets.
 
         """
@@ -317,55 +319,55 @@
         )
 
         return str_representation.format(
             set_to_string(self.inputs()), nodes_as_string, set_to_string(self.outputs())
         )
 
     @property
-    def node_dependencies(self) -> Dict[Node, Set[Node]]:
+    def node_dependencies(self) -> dict[Node, set[Node]]:
         """All dependencies of nodes where the first Node has a direct dependency on
         the second Node.
 
         Returns:
             Dictionary where keys are nodes and values are sets made up of
             their parent nodes. Independent nodes have this as empty sets.
         """
-        dependencies: Dict[Node, Set[Node]] = {node: set() for node in self._nodes}
+        dependencies: dict[Node, set[Node]] = {node: set() for node in self._nodes}
         for parent in self._nodes:
             for output in parent.outputs:
                 for child in self._nodes_by_input[_strip_transcoding(output)]:
                     dependencies[child].add(parent)
 
         return dependencies
 
     @property
-    def nodes(self) -> List[Node]:
+    def nodes(self) -> list[Node]:
         """Return a list of the pipeline nodes in topological order, i.e. if
         node A needs to be run before node B, it will appear earlier in the
         list.
 
         Returns:
             The list of all pipeline nodes in topological order.
 
         """
         return list(chain.from_iterable(self._topo_sorted_nodes))
 
     @property
-    def grouped_nodes(self) -> List[List[Node]]:
+    def grouped_nodes(self) -> list[list[Node]]:
         """Return a list of the pipeline nodes in topologically ordered groups,
         i.e. if node A needs to be run before node B, it will appear in an
         earlier group.
 
         Returns:
             The pipeline nodes in topologically ordered groups.
 
         """
         return copy.copy(self._topo_sorted_nodes)
 
-    def only_nodes(self, *node_names: str) -> "Pipeline":
+    def only_nodes(self, *node_names: str) -> Pipeline:
         """Create a new ``Pipeline`` which will contain only the specified
         nodes by name.
 
         Args:
             *node_names: One or more node names. The returned ``Pipeline``
                 will only contain these nodes.
 
@@ -396,15 +398,15 @@
             raise ValueError(
                 f"Pipeline does not contain nodes named {list(unregistered_nodes)}."
             )
 
         nodes = [self._nodes_by_name[name] for name in node_names]
         return Pipeline(nodes)
 
-    def only_nodes_with_namespace(self, node_namespace: str) -> "Pipeline":
+    def only_nodes_with_namespace(self, node_namespace: str) -> Pipeline:
         """Creates a new ``Pipeline`` containing only nodes with the specified
         namespace.
 
         Args:
             node_namespace: One node namespace.
 
         Raises:
@@ -421,16 +423,16 @@
         if not nodes:
             raise ValueError(
                 f"Pipeline does not contain nodes with namespace '{node_namespace}'"
             )
         return Pipeline(nodes)
 
     def _get_nodes_with_inputs_transcode_compatible(
-        self, datasets: Set[str]
-    ) -> Set[Node]:
+        self, datasets: set[str]
+    ) -> set[Node]:
         """Retrieves nodes that use the given `datasets` as inputs.
         If provided a name, but no format, for a transcoded dataset, it
         includes all nodes that use inputs with that name, otherwise it
         matches to the fully-qualified name only (i.e. name@format).
 
         Raises:
             ValueError: if any of the given datasets do not exist in the
@@ -452,16 +454,16 @@
             else:
                 for node_ in self._nodes_by_input[_strip_transcoding(input_)]:
                     if input_ in node_.inputs:
                         relevant_nodes.add(node_)
         return relevant_nodes
 
     def _get_nodes_with_outputs_transcode_compatible(
-        self, datasets: Set[str]
-    ) -> Set[Node]:
+        self, datasets: set[str]
+    ) -> set[Node]:
         """Retrieves nodes that output to the given `datasets`.
         If provided a name, but no format, for a transcoded dataset, it
         includes the node that outputs to that name, otherwise it matches
         to the fully-qualified name only (i.e. name@format).
 
         Raises:
             ValueError: if any of the given datasets do not exist in the
@@ -484,15 +486,15 @@
                     _strip_transcoding(output) == output
                     or output in node_with_output.outputs
                 ):
                     relevant_nodes.add(node_with_output)
 
         return relevant_nodes
 
-    def only_nodes_with_inputs(self, *inputs: str) -> "Pipeline":
+    def only_nodes_with_inputs(self, *inputs: str) -> Pipeline:
         """Create a new ``Pipeline`` object with the nodes which depend
         directly on the provided inputs.
         If provided a name, but no format, for a transcoded input, it
         includes all the nodes that use inputs with that name, otherwise it
         matches to the fully-qualified name only (i.e. name@format).
 
         Args:
@@ -510,15 +512,15 @@
 
         """
         starting = set(inputs)
         nodes = self._get_nodes_with_inputs_transcode_compatible(starting)
 
         return Pipeline(nodes)
 
-    def from_inputs(self, *inputs: str) -> "Pipeline":
+    def from_inputs(self, *inputs: str) -> Pipeline:
         """Create a new ``Pipeline`` object with the nodes which depend
         directly or transitively on the provided inputs.
         If provided a name, but no format, for a transcoded input, it
         includes all the nodes that use inputs with that name, otherwise it
         matches to the fully-qualified name only (i.e. name@format).
 
         Args:
@@ -533,15 +535,15 @@
             A new ``Pipeline`` object, containing a subset of the
                 nodes of the current one such that only nodes depending
                 directly or transitively on the provided inputs are being
                 copied.
 
         """
         starting = set(inputs)
-        result: Set[Node] = set()
+        result: set[Node] = set()
         next_nodes = self._get_nodes_with_inputs_transcode_compatible(starting)
 
         while next_nodes:
             result |= next_nodes
             outputs = set(chain.from_iterable(node.outputs for node in next_nodes))
             starting = outputs
 
@@ -550,15 +552,15 @@
                     self._nodes_by_input[_strip_transcoding(input_)]
                     for input_ in starting
                 )
             )
 
         return Pipeline(result)
 
-    def only_nodes_with_outputs(self, *outputs: str) -> "Pipeline":
+    def only_nodes_with_outputs(self, *outputs: str) -> Pipeline:
         """Create a new ``Pipeline`` object with the nodes which are directly
         required to produce the provided outputs.
         If provided a name, but no format, for a transcoded dataset, it
         includes all the nodes that output to that name, otherwise it matches
         to the fully-qualified name only (i.e. name@format).
 
         Args:
@@ -575,15 +577,15 @@
             produce the provided outputs are being copied.
         """
         starting = set(outputs)
         nodes = self._get_nodes_with_outputs_transcode_compatible(starting)
 
         return Pipeline(nodes)
 
-    def to_outputs(self, *outputs: str) -> "Pipeline":
+    def to_outputs(self, *outputs: str) -> Pipeline:
         """Create a new ``Pipeline`` object with the nodes which are directly
         or transitively required to produce the provided outputs.
         If provided a name, but no format, for a transcoded dataset, it
         includes all the nodes that output to that name, otherwise it matches
         to the fully-qualified name only (i.e. name@format).
 
         Args:
@@ -598,15 +600,15 @@
         Returns:
             A new ``Pipeline`` object, containing a subset of the nodes of the
             current one such that only nodes which are directly or transitively
             required to produce the provided outputs are being copied.
 
         """
         starting = set(outputs)
-        result: Set[Node] = set()
+        result: set[Node] = set()
         next_nodes = self._get_nodes_with_outputs_transcode_compatible(starting)
 
         while next_nodes:
             result |= next_nodes
             inputs = set(chain.from_iterable(node.inputs for node in next_nodes))
             starting = inputs
 
@@ -614,15 +616,15 @@
                 self._nodes_by_output[_strip_transcoding(output)]
                 for output in starting
                 if _strip_transcoding(output) in self._nodes_by_output
             }
 
         return Pipeline(result)
 
-    def from_nodes(self, *node_names: str) -> "Pipeline":
+    def from_nodes(self, *node_names: str) -> Pipeline:
         """Create a new ``Pipeline`` object with the nodes which depend
         directly or transitively on the provided nodes.
 
         Args:
             *node_names: A list of node_names which should be used as a
                 starting point of the new ``Pipeline``.
         Raises:
@@ -635,15 +637,15 @@
 
         """
 
         res = self.only_nodes(*node_names)
         res += self.from_inputs(*map(_strip_transcoding, res.all_outputs()))
         return res
 
-    def to_nodes(self, *node_names: str) -> "Pipeline":
+    def to_nodes(self, *node_names: str) -> Pipeline:
         """Create a new ``Pipeline`` object with the nodes required directly
         or transitively by the provided nodes.
 
         Args:
             *node_names: A list of node_names which should be used as an
                 end point of the new ``Pipeline``.
         Raises:
@@ -656,15 +658,15 @@
 
         """
 
         res = self.only_nodes(*node_names)
         res += self.to_outputs(*map(_strip_transcoding, res.all_inputs()))
         return res
 
-    def only_nodes_with_tags(self, *tags: str) -> "Pipeline":
+    def only_nodes_with_tags(self, *tags: str) -> Pipeline:
         """Creates a new ``Pipeline`` object with the nodes which contain *any*
         of the provided tags. The resulting ``Pipeline`` is empty if no tags
         are provided.
 
         Args:
             *tags: A list of node tags which should be used to lookup
                 the nodes of the new ``Pipeline``.
@@ -683,15 +685,15 @@
         tags: Iterable[str] = None,
         from_nodes: Iterable[str] = None,
         to_nodes: Iterable[str] = None,
         node_names: Iterable[str] = None,
         from_inputs: Iterable[str] = None,
         to_outputs: Iterable[str] = None,
         node_namespace: str = None,
-    ) -> "Pipeline":
+    ) -> Pipeline:
         """Creates a new ``Pipeline`` object with the nodes that meet all of the
         specified filtering conditions.
 
         The new pipeline object is the intersection of pipelines that meet each
         filtering condition. This is distinct from chaining multiple filters together.
 
         Args:
@@ -765,15 +767,15 @@
 
         if not filtered_pipeline.nodes:
             raise ValueError(
                 "Pipeline contains no nodes after applying all provided filters"
             )
         return filtered_pipeline
 
-    def tag(self, tags: Union[str, Iterable[str]]) -> "Pipeline":
+    def tag(self, tags: str | Iterable[str]) -> Pipeline:
         """Tags all the nodes in the pipeline.
 
         Args:
             tags: The tags to be added to the nodes.
 
         Returns:
             New ``Pipeline`` object with nodes tagged.
@@ -796,17 +798,17 @@
             "kedro_version": kedro.__version__,
             "pipeline": transformed,
         }
 
         return json.dumps(pipeline_versioned)
 
 
-def _validate_duplicate_nodes(nodes_or_pipes: Iterable[Union[Node, Pipeline]]):
-    seen_nodes: Set[str] = set()
-    duplicates: Dict[Union[Pipeline, None], Set[str]] = defaultdict(set)
+def _validate_duplicate_nodes(nodes_or_pipes: Iterable[Node | Pipeline]):
+    seen_nodes: set[str] = set()
+    duplicates: dict[Pipeline | None, set[str]] = defaultdict(set)
 
     def _check_node(node_: Node, pipeline_: Pipeline = None):
         name = node_.name
         if name in seen_nodes:
             duplicates[pipeline_].add(name)
         else:
             seen_nodes.add(name)
@@ -831,37 +833,37 @@
         raise ValueError(
             f"Pipeline nodes must have unique names. The following node names "
             f"appear more than once:\n\n{duplicates_info}\nYou can name your "
             f"nodes using the last argument of 'node()'."
         )
 
 
-def _validate_unique_outputs(nodes: List[Node]) -> None:
+def _validate_unique_outputs(nodes: list[Node]) -> None:
     outputs = chain.from_iterable(node.outputs for node in nodes)
     outputs = map(_strip_transcoding, outputs)
     duplicates = [key for key, value in Counter(outputs).items() if value > 1]
     if duplicates:
         raise OutputNotUniqueError(
             f"Output(s) {sorted(duplicates)} are returned by more than one nodes. Node "
             f"outputs must be unique."
         )
 
 
-def _validate_unique_confirms(nodes: List[Node]) -> None:
+def _validate_unique_confirms(nodes: list[Node]) -> None:
     confirms = chain.from_iterable(node.confirms for node in nodes)
     confirms = map(_strip_transcoding, confirms)
     duplicates = [key for key, value in Counter(confirms).items() if value > 1]
     if duplicates:
         raise ConfirmNotUniqueError(
             f"{sorted(duplicates)} datasets are confirmed by more than one node. Node "
             f"confirms must be unique."
         )
 
 
-def _validate_transcoded_inputs_outputs(nodes: List[Node]) -> None:
+def _validate_transcoded_inputs_outputs(nodes: list[Node]) -> None:
     """Users should not be allowed to refer to a transcoded dataset both
     with and without the separator.
     """
     all_inputs_outputs = set(
         chain(
             chain.from_iterable(node.inputs for node in nodes),
             chain.from_iterable(node.outputs for node in nodes),
@@ -879,29 +881,29 @@
             f"The following datasets are used with transcoding, but "
             f"were referenced without the separator: {', '.join(invalid)}.\n"
             f"Please specify a transcoding option or "
             f"rename the datasets."
         )
 
 
-def _topologically_sorted(node_dependencies) -> List[List[Node]]:
+def _topologically_sorted(node_dependencies) -> list[list[Node]]:
     """Topologically group and sort (order) nodes such that no node depends on
     a node that appears in the same or a later group.
 
     Raises:
         CircularDependencyError: When it is not possible to topologically order
             provided nodes.
 
     Returns:
         The list of node sets in order of execution. First set is nodes that should
         be executed first (no dependencies), second set are nodes that should be
         executed on the second step, etc.
     """
 
-    def _circle_error_message(error_data: Dict[str, str]) -> str:
+    def _circle_error_message(error_data: dict[str, str]) -> str:
         """Error messages provided by the toposort library will
         refer to indices that are used as an intermediate step.
         This method can be used to replace that message with
         one that refers to the nodes' string representations.
         """
         circular = [str(node) for node in error_data.keys()]
         return f"Circular dependencies exist among these items: {circular}"
```

### Comparing `kedro-0.18.8/kedro/runner/parallel_runner.py` & `kedro-0.18.9/kedro/runner/parallel_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """``ParallelRunner`` is an ``AbstractRunner`` implementation. It can
 be used to run the ``Pipeline`` in parallel groups formed by toposort.
 """
+from __future__ import annotations
+
 import multiprocessing
 import os
 import pickle
 import sys
 from collections import Counter
 from concurrent.futures import FIRST_COMPLETED, ProcessPoolExecutor, wait
 from itertools import chain
 from multiprocessing.managers import BaseProxy, SyncManager  # type: ignore
 from multiprocessing.reduction import ForkingPickler
 from pickle import PicklingError
-from typing import Any, Dict, Iterable, Set
+from typing import Any, Iterable
 
 from pluggy import PluginManager
 
 from kedro.framework.hooks.manager import (
     _create_hook_manager,
     _register_hooks,
     _register_hooks_setuptools,
@@ -74,29 +76,29 @@
 
 
 ParallelRunnerManager.register(  # pylint: disable=no-member
     "MemoryDataSet", MemoryDataSet
 )
 
 
-def _bootstrap_subprocess(package_name: str, logging_config: Dict[str, Any]):
+def _bootstrap_subprocess(package_name: str, logging_config: dict[str, Any]):
     # pylint: disable=import-outside-toplevel,cyclic-import
     from kedro.framework.project import configure_logging, configure_project
 
     configure_project(package_name)
     configure_logging(logging_config)
 
 
 def _run_node_synchronization(  # pylint: disable=too-many-arguments
     node: Node,
     catalog: DataCatalog,
     is_async: bool = False,
     session_id: str = None,
     package_name: str = None,
-    logging_config: Dict[str, Any] = None,
+    logging_config: dict[str, Any] = None,
 ) -> Node:
     """Run a single `Node` with inputs from and outputs to the `catalog`.
 
     A ``PluginManager`` instance is created in each subprocess because the
     ``PluginManager`` can't be serialised.
 
     Args:
@@ -286,15 +288,15 @@
         nodes = pipeline.nodes
         self._validate_catalog(catalog, pipeline)
         self._validate_nodes(nodes)
 
         load_counts = Counter(chain.from_iterable(n.inputs for n in nodes))
         node_dependencies = pipeline.node_dependencies
         todo_nodes = set(node_dependencies.keys())
-        done_nodes: Set[Node] = set()
+        done_nodes: set[Node] = set()
         futures = set()
         done = None
         max_workers = self._get_required_workers_count(pipeline)
 
         from kedro.framework.project import LOGGING, PACKAGE_NAME
 
         with ProcessPoolExecutor(max_workers=max_workers) as pool:
```

### Comparing `kedro-0.18.8/kedro/runner/runner.py` & `kedro-0.18.9/kedro/runner/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """``AbstractRunner`` is the base class for all ``Pipeline`` runner
 implementations.
 """
+from __future__ import annotations
 
 import inspect
 import itertools as it
 import logging
 from abc import ABC, abstractmethod
 from collections import deque
 from concurrent.futures import (
     ALL_COMPLETED,
     Future,
     ThreadPoolExecutor,
     as_completed,
     wait,
 )
-from typing import Any, Dict, Iterable, Iterator, List, Set
+from typing import Any, Iterable, Iterator
 
 from more_itertools import interleave
 from pluggy import PluginManager
 
 from kedro.framework.hooks.manager import _NullPluginManager
 from kedro.io import AbstractDataSet, DataCatalog, MemoryDataSet
 from kedro.pipeline import Pipeline
@@ -46,15 +47,15 @@
 
     def run(
         self,
         pipeline: Pipeline,
         catalog: DataCatalog,
         hook_manager: PluginManager = None,
         session_id: str = None,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """Run the ``Pipeline`` using the datasets provided by ``catalog``
         and save results back to the same objects.
 
         Args:
             pipeline: The ``Pipeline`` to run.
             catalog: The ``DataCatalog`` from which to fetch data.
             hook_manager: The ``PluginManager`` to activate hooks.
@@ -92,15 +93,15 @@
 
         self._logger.info("Pipeline execution completed successfully.")
 
         return {ds_name: catalog.load(ds_name) for ds_name in free_outputs}
 
     def run_only_missing(
         self, pipeline: Pipeline, catalog: DataCatalog, hook_manager: PluginManager
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """Run only the missing outputs from the ``Pipeline`` using the
         datasets provided by ``catalog``, and save results back to the
         same objects.
 
         Args:
             pipeline: The ``Pipeline`` to run.
             catalog: The ``DataCatalog`` from which to fetch data.
@@ -210,15 +211,15 @@
                 len(remaining_nodes),
                 postfix,
             )
 
 
 def _find_persistent_ancestors(
     pipeline: Pipeline, children: Iterable[Node], catalog: DataCatalog
-) -> Set[Node]:
+) -> set[Node]:
     """Breadth-first search approach to finding the complete set of
     persistent ancestors of an iterable of ``Node``s. Persistent
     ancestors exclusively have persisted ``Dataset``s as inputs.
 
     Args:
         pipeline: the ``Pipeline`` to find ancestors in.
         children: the iterable containing ``Node``s to find ancestors of.
@@ -240,15 +241,15 @@
             if parent in visited:
                 continue
             visited.add(parent)
             queue.append(parent)
     return ancestor_nodes_to_run
 
 
-def _enumerate_parents(pipeline: Pipeline, child: Node) -> List[Node]:
+def _enumerate_parents(pipeline: Pipeline, child: Node) -> list[Node]:
     """For a given ``Node``, returns a list containing the direct parents
     of that ``Node`` in the given ``Pipeline``.
 
     Args:
         pipeline: the ``Pipeline`` to search for direct parents in.
         child: the ``Node`` to find parents of.
 
@@ -322,19 +323,19 @@
         catalog.confirm(name)
     return node
 
 
 def _collect_inputs_from_hook(
     node: Node,
     catalog: DataCatalog,
-    inputs: Dict[str, Any],
+    inputs: dict[str, Any],
     is_async: bool,
     hook_manager: PluginManager,
     session_id: str = None,
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     # pylint: disable=too-many-arguments
     inputs = inputs.copy()  # shallow copy to prevent in-place modification by the hook
     hook_response = hook_manager.hook.before_node_run(
         node=node,
         catalog=catalog,
         inputs=inputs,
         is_async=is_async,
@@ -357,19 +358,19 @@
 
     return additional_inputs
 
 
 def _call_node_run(
     node: Node,
     catalog: DataCatalog,
-    inputs: Dict[str, Any],
+    inputs: dict[str, Any],
     is_async: bool,
     hook_manager: PluginManager,
     session_id: str = None,
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     # pylint: disable=too-many-arguments
     try:
         outputs = node.run(inputs)
     except Exception as exc:
         hook_manager.hook.on_node_error(
             error=exc,
             node=node,
@@ -450,15 +451,15 @@
         return_ds = catalog.load(dataset_name)
         hook_manager.hook.after_dataset_loaded(
             dataset_name=dataset_name, data=return_ds, node=node
         )
         return return_ds
 
     with ThreadPoolExecutor() as pool:
-        inputs: Dict[str, Future] = {}
+        inputs: dict[str, Future] = {}
 
         for name in node.inputs:
             inputs[name] = pool.submit(_synchronous_dataset_load, name)
 
         wait(inputs.values(), return_when=ALL_COMPLETED)
         inputs = {key: value.result() for key, value in inputs.items()}
         is_async = True
```

### Comparing `kedro-0.18.8/kedro/runner/sequential_runner.py` & `kedro-0.18.9/kedro/runner/sequential_runner.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/runner/thread_runner.py` & `kedro-0.18.9/kedro/runner/thread_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """``ThreadRunner`` is an ``AbstractRunner`` implementation. It can
 be used to run the ``Pipeline`` in parallel groups formed by toposort
 using threads.
 """
+from __future__ import annotations
+
 import warnings
 from collections import Counter
 from concurrent.futures import FIRST_COMPLETED, ThreadPoolExecutor, wait
 from itertools import chain
-from typing import Set
 
 from pluggy import PluginManager
 
 from kedro.io import DataCatalog, MemoryDataSet
 from kedro.pipeline import Pipeline
 from kedro.pipeline.node import Node
 from kedro.runner.runner import AbstractRunner, run_node
@@ -99,15 +100,15 @@
             Exception: in case of any downstream node failure.
 
         """
         nodes = pipeline.nodes
         load_counts = Counter(chain.from_iterable(n.inputs for n in nodes))
         node_dependencies = pipeline.node_dependencies
         todo_nodes = set(node_dependencies.keys())
-        done_nodes: Set[Node] = set()
+        done_nodes: set[Node] = set()
         futures = set()
         done = None
         max_workers = self._get_required_workers_count(pipeline)
 
         with ThreadPoolExecutor(max_workers=max_workers) as pool:
             while True:
                 ready = {n for n in todo_nodes if node_dependencies[n] <= done_nodes}
```

### Comparing `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore` & `kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md` & `kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/README.md`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md` & `kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/conf/README.md`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py` & `kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/setup.py` & `kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/setup.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/test_run.py` & `kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py` & `kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py` & `kedro-0.18.9/kedro/templates/project/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 """Project settings. There is no need to edit this file unless you want to change values
 from the Kedro defaults. For further information, including these default values, see
 https://kedro.readthedocs.io/en/stable/kedro_project_setup/settings.html."""
 
 # Instantiated project hooks.
+# For example, after creating a hooks.py and defining a ProjectHooks class there, do
 # from {{cookiecutter.python_package}}.hooks import ProjectHooks
 # HOOKS = (ProjectHooks(),)
 
 # Installed plugins for which to disable hook auto-registration.
 # DISABLE_HOOKS_FOR_PLUGINS = ("kedro-viz",)
 
 # Class that manages storing KedroSession data.
-# from kedro.framework.session.shelvestore import ShelveStore
-# SESSION_STORE_CLASS = ShelveStore
+# from kedro.framework.session.store import BaseSessionStore
+# SESSION_STORE_CLASS = BaseSessionStore
 # Keyword arguments to pass to the `SESSION_STORE_CLASS` constructor.
 # SESSION_STORE_ARGS = {
 #     "path": "./sessions"
 # }
 
-# Class that manages Kedro's library components.
-# from kedro.framework.context import KedroContext
-# CONTEXT_CLASS = KedroContext
-
 # Directory that holds configuration.
 # CONF_SOURCE = "conf"
 
 # Class that manages how configuration is loaded.
-# CONFIG_LOADER_CLASS = ConfigLoader
+# from kedro.config import OmegaConfigLoader
+# CONFIG_LOADER_CLASS = OmegaConfigLoader
 # Keyword arguments to pass to the `CONFIG_LOADER_CLASS` constructor.
 # CONFIG_LOADER_ARGS = {
 #       "config_patterns": {
 #           "spark" : ["spark*/"],
 #           "parameters": ["parameters*", "parameters*/**", "**/parameters*"],
 #       }
 # }
 
+# Class that manages Kedro's library components.
+# from kedro.framework.context import KedroContext
+# CONTEXT_CLASS = KedroContext
+
 # Class that manages the Data Catalog.
 # from kedro.io import DataCatalog
 # DATA_CATALOG_CLASS = DataCatalog
```

### Comparing `kedro-0.18.8/kedro/utils.py` & `kedro-0.18.9/kedro/utils.py`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/kedro.egg-info/PKG-INFO` & `kedro-0.18.9/kedro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro
-Version: 0.18.8
+Version: 0.18.9
 Summary: Kedro helps you build production-ready data and analytics pipelines
 Author: Kedro
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://kedro.org
 Project-URL: Source, https://github.com/kedro-org/kedro
 Project-URL: Documentation, https://docs.kedro.org
 Project-URL: Tracker, https://github.com/kedro-org/kedro/issues
```

### Comparing `kedro-0.18.8/kedro.egg-info/SOURCES.txt` & `kedro-0.18.9/kedro.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.py
 test_requirements.txt
 dependency/requirements.txt
 kedro/__init__.py
 kedro/__main__.py
+kedro/logging.py
 kedro/py.typed
 kedro/utils.py
 kedro.egg-info/PKG-INFO
 kedro.egg-info/SOURCES.txt
 kedro.egg-info/dependency_links.txt
 kedro.egg-info/entry_points.txt
 kedro.egg-info/not-zip-safe
```

### Comparing `kedro-0.18.8/pyproject.toml` & `kedro-0.18.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kedro-0.18.8/setup.py` & `kedro-0.18.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -100,19 +100,15 @@
         "sphinx-autodoc-typehints==1.20.2",
         "sphinx_copybutton==0.3.1",
         "sphinx-notfound-page",
         "ipykernel>=5.3, <7.0",
         "sphinxcontrib-mermaid~=0.7.1",
         "myst-parser~=1.0.0",
         "Jinja2<3.1.0",
-        # https://github.com/kedro-org/kedro-plugins/issues/141
-        # https://github.com/kedro-org/kedro-plugins/issues/143
-        "kedro-datasets[api,biosequence,dask,geopandas,matplotlib,holoviews,networkx,pandas,pillow,polars,video,plotly,redis,spark,svmlight,yaml]==1.1.1",
-        "kedro-datasets[tensorflow]==1.1.1; platform_system != 'Darwin' or platform_machine != 'arm64'",
-        "tensorflow-macos~=2.0; platform_system == 'Darwin' and platform_machine == 'arm64'",
+        "kedro-datasets[all]~=1.4.0",
     ],
     "geopandas": _collect_requirements(geopandas_require),
     "matplotlib": _collect_requirements(matplotlib_require),
     "holoviews": _collect_requirements(holoviews_require),
     "networkx": _collect_requirements(networkx_require),
     "pandas": _collect_requirements(pandas_require),
     "pickle": _collect_requirements(pickle_require),
```

### Comparing `kedro-0.18.8/test_requirements.txt` & `kedro-0.18.9/test_requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 dill~=0.3.1
 filelock>=3.4.0, <4.0
 gcsfs>=2021.4, <=2023.1; python_version == '3.7'
 gcsfs>=2023.1, <2023.3; python_version >= '3.8'
 geopandas>=0.6.0, <1.0
 hdfs>=2.5.8, <3.0
 holoviews~=1.13.0
-import-linter[toml]==1.2.6
+import-linter[toml]==1.8.0
 ipython>=7.31.1, <8.0; python_version < '3.8'
 ipython~=8.10; python_version >= '3.8'
 isort~=5.0
 Jinja2<3.1.0
 joblib>=0.14
 jupyterlab_server>=2.11.1, <2.16.0 # 2.16.0 requires importlib_metedata >= 4.8.3 which conflicts with flake8 requirement
 jupyterlab~=3.0, <3.6.0 # 3.6.0 requires jupyterlab_server~=2.19
```

### Comparing `kedro-0.18.8/tests/test_utils.py` & `kedro-0.18.9/tests/test_utils.py`

 * *Files identical despite different names*

