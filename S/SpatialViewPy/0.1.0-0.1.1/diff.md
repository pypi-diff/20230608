# Comparing `tmp/SpatialViewPy-0.1.0.tar.gz` & `tmp/SpatialViewPy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpatialViewPy-0.1.0.tar", last modified: Thu Jun  8 07:06:33 2023, max compression
+gzip compressed data, was "SpatialViewPy-0.1.1.tar", last modified: Thu Jun  8 08:07:57 2023, max compression
```

## Comparing `SpatialViewPy-0.1.0.tar` & `SpatialViewPy-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-08 07:06:33.636264 SpatialViewPy-0.1.0/
--rw-r--r--   0 cmohanty2   (503) staff       (20)     1073 2023-06-07 20:55:25.000000 SpatialViewPy-0.1.0/LICENSE.txt
--rw-r--r--   0 cmohanty2   (503) staff       (20)       36 2023-06-08 03:39:33.000000 SpatialViewPy-0.1.0/MANIFEST.in
--rw-r--r--   0 cmohanty2   (503) staff       (20)     1014 2023-06-08 07:06:33.636130 SpatialViewPy-0.1.0/PKG-INFO
--rw-r--r--   0 cmohanty2   (503) staff       (20)      666 2023-06-08 06:56:19.000000 SpatialViewPy-0.1.0/README.md
-drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-08 07:06:33.634444 SpatialViewPy-0.1.0/notebooks/
--rw-r--r--   0 cmohanty2   (503) staff       (20)   420257 2023-06-08 07:05:51.000000 SpatialViewPy-0.1.0/notebooks/tutorial.ipynb
--rw-r--r--   0 cmohanty2   (503) staff       (20)       38 2023-06-08 07:06:33.636304 SpatialViewPy-0.1.0/setup.cfg
--rw-r--r--   0 cmohanty2   (503) staff       (20)      973 2023-06-08 06:37:21.000000 SpatialViewPy-0.1.0/setup.py
-drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-08 07:06:33.633712 SpatialViewPy-0.1.0/src/
-drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-08 07:06:33.635506 SpatialViewPy-0.1.0/src/SpatialViewPy.egg-info/
--rw-r--r--   0 cmohanty2   (503) staff       (20)     1014 2023-06-08 07:06:33.000000 SpatialViewPy-0.1.0/src/SpatialViewPy.egg-info/PKG-INFO
--rw-r--r--   0 cmohanty2   (503) staff       (20)      365 2023-06-08 07:06:33.000000 SpatialViewPy-0.1.0/src/SpatialViewPy.egg-info/SOURCES.txt
--rw-r--r--   0 cmohanty2   (503) staff       (20)        1 2023-06-08 07:06:33.000000 SpatialViewPy-0.1.0/src/SpatialViewPy.egg-info/dependency_links.txt
--rw-r--r--   0 cmohanty2   (503) staff       (20)      110 2023-06-08 07:06:33.000000 SpatialViewPy-0.1.0/src/SpatialViewPy.egg-info/requires.txt
--rw-r--r--   0 cmohanty2   (503) staff       (20)       14 2023-06-08 07:06:33.000000 SpatialViewPy-0.1.0/src/SpatialViewPy.egg-info/top_level.txt
-drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-08 07:06:33.635944 SpatialViewPy-0.1.0/src/spatialviewpy/
--rw-r--r--   0 cmohanty2   (503) staff       (20)       82 2023-06-08 06:37:49.000000 SpatialViewPy-0.1.0/src/spatialviewpy/__init__.py
--rw-r--r--   0 cmohanty2   (503) staff       (20)       21 2023-06-08 06:36:09.000000 SpatialViewPy-0.1.0/src/spatialviewpy/__version.py
--rw-r--r--   0 cmohanty2   (503) staff       (20)    13474 2023-06-08 01:58:27.000000 SpatialViewPy-0.1.0/src/spatialviewpy/prepare_viz.py
+drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-08 08:07:57.700486 SpatialViewPy-0.1.1/
+-rw-r--r--   0 cmohanty2   (503) staff       (20)     1073 2023-06-07 20:55:25.000000 SpatialViewPy-0.1.1/LICENSE.txt
+-rw-r--r--   0 cmohanty2   (503) staff       (20)       36 2023-06-08 03:39:33.000000 SpatialViewPy-0.1.1/MANIFEST.in
+-rw-r--r--   0 cmohanty2   (503) staff       (20)     1014 2023-06-08 08:07:57.700291 SpatialViewPy-0.1.1/PKG-INFO
+-rw-r--r--   0 cmohanty2   (503) staff       (20)      666 2023-06-08 06:56:19.000000 SpatialViewPy-0.1.1/README.md
+drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-08 08:07:57.698095 SpatialViewPy-0.1.1/notebooks/
+-rw-r--r--   0 cmohanty2   (503) staff       (20)   420498 2023-06-08 08:03:00.000000 SpatialViewPy-0.1.1/notebooks/tutorial.ipynb
+-rw-r--r--   0 cmohanty2   (503) staff       (20)       38 2023-06-08 08:07:57.700533 SpatialViewPy-0.1.1/setup.cfg
+-rw-r--r--   0 cmohanty2   (503) staff       (20)     1005 2023-06-08 08:07:31.000000 SpatialViewPy-0.1.1/setup.py
+drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-08 08:07:57.696876 SpatialViewPy-0.1.1/src/
+drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-08 08:07:57.699242 SpatialViewPy-0.1.1/src/SpatialViewPy.egg-info/
+-rw-r--r--   0 cmohanty2   (503) staff       (20)     1014 2023-06-08 08:07:57.000000 SpatialViewPy-0.1.1/src/SpatialViewPy.egg-info/PKG-INFO
+-rw-r--r--   0 cmohanty2   (503) staff       (20)      365 2023-06-08 08:07:57.000000 SpatialViewPy-0.1.1/src/SpatialViewPy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmohanty2   (503) staff       (20)        1 2023-06-08 08:07:57.000000 SpatialViewPy-0.1.1/src/SpatialViewPy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmohanty2   (503) staff       (20)      126 2023-06-08 08:07:57.000000 SpatialViewPy-0.1.1/src/SpatialViewPy.egg-info/requires.txt
+-rw-r--r--   0 cmohanty2   (503) staff       (20)       14 2023-06-08 08:07:57.000000 SpatialViewPy-0.1.1/src/SpatialViewPy.egg-info/top_level.txt
+drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-08 08:07:57.699915 SpatialViewPy-0.1.1/src/spatialviewpy/
+-rw-r--r--   0 cmohanty2   (503) staff       (20)       82 2023-06-08 06:37:49.000000 SpatialViewPy-0.1.1/src/spatialviewpy/__init__.py
+-rw-r--r--   0 cmohanty2   (503) staff       (20)       21 2023-06-08 06:36:09.000000 SpatialViewPy-0.1.1/src/spatialviewpy/__version.py
+-rw-r--r--   0 cmohanty2   (503) staff       (20)    16484 2023-06-08 08:04:35.000000 SpatialViewPy-0.1.1/src/spatialviewpy/prepare_viz.py
```

### Comparing `SpatialViewPy-0.1.0/LICENSE.txt` & `SpatialViewPy-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SpatialViewPy-0.1.0/PKG-INFO` & `SpatialViewPy-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpatialViewPy
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/kendziorski-lab/SpatialViewPy
 Author: Chitrasen Mohanty
 Author-email: mohantychitraen@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `SpatialViewPy-0.1.0/README.md` & `SpatialViewPy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `SpatialViewPy-0.1.0/notebooks/tutorial.ipynb` & `SpatialViewPy-0.1.1/notebooks/tutorial.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940957633053221%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(3, '# !pip install scanorama\\n'), (4, '# !pip install "*

 * *            "requests')], delete: [3]}}, 3: {'source': {insert: [(9, 'from spatialviewpy import "*

 * *            "prepare10x_from_scanpy\\n')], delete: [9]}}, 21: {'source': {insert: [(2, "*

 * *            "'                       n_genes = 30)\\n')], delete: [2]}}, 22: {'source': {delete: "*

 * *            "[0]}}, 23: {'source': {insert: [(7, '                       launch_app = True,\\n'), "*

 * *            "(8, '             […]*

```diff
@@ -7,24 +7,34 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "!pip install spatialviewpy"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "c22cce7c",
+            "metadata": {},
+            "source": [
+                "May need to install following additional packages."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": 2,
             "id": "e0c48e49",
             "metadata": {},
             "outputs": [],
             "source": [
                 "## If running in conda environment\n",
                 "# !conda install -c conda-forge python-annoy -y\n",
                 "\n",
-                "# !pip install scanorama"
+                "# !pip install scanorama\n",
+                "# !pip install requests"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "7596d305",
             "metadata": {},
@@ -35,15 +45,15 @@
                 "import pandas as pd\n",
                 "import numpy as np\n",
                 "import matplotlib as mpl\n",
                 "import matplotlib.pyplot as plt\n",
                 "import seaborn as sns\n",
                 "import scanorama\n",
                 "\n",
-                "from SpatialViewPy import prepare10x_from_scanpy\n",
+                "from spatialviewpy import prepare10x_from_scanpy\n",
                 "\n",
                 "from os import listdir, path\n",
                 "from collections import OrderedDict\n",
                 "\n",
                 "import warnings\n",
                 "warnings.filterwarnings('ignore')"
             ]
@@ -460,27 +470,26 @@
             "execution_count": 15,
             "id": "b7620358",
             "metadata": {},
             "outputs": [],
             "source": [
                 "sc.tl.rank_genes_groups(adata_spatial, 'clusters', layer = 'normalized_counts',\n",
                 "                        method='wilcoxon', key_added = \"de_genes\",\n",
-                "                       n_genes = 20)\n",
+                "                       n_genes = 30)\n",
                 "\n",
                 "ranked_genes = adata_spatial.uns['de_genes']['names']\n",
                 "de_genes = [','.join(ranked_genes[c]) for c in ranked_genes.dtype.names]"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "26e8eb69",
             "metadata": {},
             "source": [
-                "-----\n",
                 "\n",
                 "## Visualize using SpatialView"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -491,15 +500,16 @@
                 "sample_paths = [path.join(data_path, sample_name) for sample_name in sample_names]\n",
                 "\n",
                 "prepare10x_from_scanpy(adata_spatial, data_paths = sample_paths,\n",
                 "                       export_path = \"TME\",\n",
                 "                       cluster_genes = de_genes,\n",
                 "                       layer = 'normalized_counts',\n",
                 "                       download_repo = True,\n",
-                "                       launch_app = True)"
+                "                       launch_app = True,\n",
+                "                       verbose= True)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `SpatialViewPy-0.1.0/setup.py` & `SpatialViewPy-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='SpatialViewPy',
-      version='0.1.0',
+      version='0.1.1',
       descriptiopn = 'Visualizing multi-sample spatial transcriptimic data using SpatialView',
       py_module='spatialviewpy/prepare_viz',
       package_dir = {'':'src'},
       classifiers=[
           "Programming Language :: Python :: 3.6",
           "Operating System :: OS Independent",
       ],
       long_description = long_description,
       long_description_content_type = "text/markdown",
       install_requires = [
+           "requests >= 2.0.0",
             "numpy >= 1.23.0",
             "pandas >= 2.0.0",
             "scipy >= 1.10",
             "scanpy >= 1.9",
             "anndata >= 0.8",
             "pandas >= 1.5",
             "zipfile2 >= 0.0.12",
```

### Comparing `SpatialViewPy-0.1.0/src/SpatialViewPy.egg-info/PKG-INFO` & `SpatialViewPy-0.1.1/src/SpatialViewPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpatialViewPy
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/kendziorski-lab/SpatialViewPy
 Author: Chitrasen Mohanty
 Author-email: mohantychitraen@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `SpatialViewPy-0.1.0/src/spatialviewpy/prepare_viz.py` & `SpatialViewPy-0.1.1/src/spatialviewpy/prepare_viz.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 def prepare10x_from_scanpy(adataObj,
                                    data_paths,
                                    export_path,
                                    samples_id_col = "sample_id",
                                    project_name = "spatial",
-                                   clusterCol = "clusters",
+                                   cluster_col = "clusters",
                                    cluster_names = None,
                                    cluster_genes = None,
                                    clust_colors = None,
                                    layer = None,
                                    multisample_pattern = "_",
                                    expr_round = 3,
                                    spatial_sub_dir = "spatial",
@@ -21,14 +21,48 @@
                                    export_sparse = True,
                                    data_file_name_expressions = "expression_matrix.csv",
                                    data_file_name_expressions_sparse = "expression_matrix_sparse.txt",
                                    data_file_name_genes = "genes.csv",
                                    data_file_name_barcodes = "barcodes.csv",
                                    verbose = False,
                                    config_list = None):
+    """
+    Prepares data from Scanpy object and runs SpatialView.
+
+    Args:
+        adataObj (Scanpy): Scanpy object
+        data_paths (str): directory path to raw data location
+        export_path (str): directory path where the prepared data will be exported or SpatialView will be run
+        samples_id_col (str, optional): Column name in adataObj containing sample names. Defaults to "sample_id".
+        project_name (str, optional): Name of the project. Defaults to "spatial".
+        cluster_col (str, optional): Column name in adataObj containing cluster annotations. Defaults to "clusters".
+        cluster_names (str list, optional): Name of the clustes. If provided must match to the number of clusters. Defaults to None.
+        cluster_genes (str list, optional): list of gene names with ',' separated. Defaults to None.
+        clust_colors (str list, optional): list of hex colors corresponding to clusters. Defaults to None.
+        layer (str, optional): Which later of Scanpy to be used. Defaults to None.
+        multisample_pattern (str, optional): Character suffixed to the barcodes to make unique in case of multiple samples. Defaults to "_".
+        expr_round (int, optional): The expression values are rounded upto. Defaults to 3.
+        spatial_sub_dir (str, optional): subdirectory name where files related to spatial information are stored. Defaults to "spatial".
+        sample_info (dataframe, optional): Metadata information about the samples. Rows corresponding to samples. Defaults to None.
+        download_repo (bool, optional): If True, SpatialView will be downloaded from Github repository. Defaults to True.
+        spatialview_repo (str, optional): SpatialView repo location. Defaults to "https://github.com/kendziorski-lab/spatialview/archive/refs/tags/".
+        spatialview_version (str, optional): Which version to use. Defaults to "spatialview-latest".
+        port (int, optional): Port number to be used by SpatialView. Defaults to 8878.
+        launch_app (bool, optional): If True, then the SpatialView is launched. Defaults to True.
+        export_sparse (bool, optional): Data compression for SpatialView. Defaults to True.
+        data_file_name_expressions (str, optional): (For SpatialView) Name of the expression matrix. Defaults to "expression_matrix.csv".
+        data_file_name_expressions_sparse (str, optional): (For SpatialView) Name of the expression matrix in sparse format. Defaults to "expression_matrix_sparse.txt".
+        data_file_name_genes (str, optional): (For SpatialView) Name of the file containing genes name. Defaults to "genes.csv".
+        data_file_name_barcodes (str, optional): (For SpatialView) Name of the file containing barcodes. Defaults to "barcodes.csv".
+        verbose (bool, optional): Defaults to False.
+        config_list (dictionary, optional): (For SpatialView) Additional configuration values to be passed to SpatialView. Defaults to None.
+
+    Raises:
+        FileNotFoundError: _description_
+    """
     
     import numpy as np
     import pandas as pd
     from scipy.io import mmwrite
     from zipfile2 import ZipFile
     import seaborn as sns
     import requests
@@ -89,15 +123,15 @@
                     if k in spatalview_config:
                         spatalview_config[k] = v
                     
         spatalview_config['data_file_name_expressions'] = data_file_name_expressions
         spatalview_config['data_file_name_expressions_sparse'] = data_file_name_expressions_sparse
         spatalview_config['data_file_name_genes'] = data_file_name_genes
         spatalview_config['data_file_name_barcodes'] = data_file_name_barcodes
-        spatalview_config['data_cluster_column'] = clusterCol
+        spatalview_config['data_cluster_column'] = cluster_col
         
         with open(config_path, 'w') as json_file:
             json.dump(spatalview_config, json_file)
             
         #updating html data info tab
         dataInfo = pd.DataFrame({'Sample' : samples_ids})
         if sample_info is not None:
@@ -200,16 +234,16 @@
 
         # Step 4
         #---------
         # creating metadata
         metadata = adataObj_temp.obs.copy()
         metadata['barcode'] = ["-".join(bc.split(multisample_pattern)[:-1]) for bc in metadata.index]
         
-        if clusterCol in metadata.columns:
-            metadata['cluster'] = metadata[clusterCol]
+        if cluster_col in metadata.columns:
+            metadata['cluster'] = metadata[cluster_col]
         else:
             metadata['cluster'] = 1
             
         spot_info = pd.read_csv(path.join(data_path, spatial_sub_dir,
                                           "tissue_positions_list.csv"),
                                 header = None)        
         spot_info.columns = ["barcode", "in_tissue", "array_row", 
@@ -249,16 +283,16 @@
             normalized_counts['barcode'] = adataObj_temp.obs.index
             normalized_counts.to_csv(path.join(export_path_sample, data_file_name_expressions), index = False)
             
         # Step 6
         #----------
         # creating cluster info
         unique_clusters = 1
-        if clusterCol in adataObj.obs.columns:
-            unique_clusters = adataObj.obs[clusterCol].unique().sort_values()
+        if cluster_col in adataObj.obs.columns:
+            unique_clusters = adataObj.obs[cluster_col].unique().sort_values()
         
         if not clust_colors:
             clust_colors = sns.color_palette("colorblind", len(unique_clusters))
             clust_colors = clust_colors.as_hex()
         
         if not cluster_names:
             cluster_names = unique_clusters
```

