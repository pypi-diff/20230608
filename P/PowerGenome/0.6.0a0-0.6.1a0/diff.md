# Comparing `tmp/powergenome-0.6.0a0.tar.gz` & `tmp/PowerGenome-0.6.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powergenome-0.6.0a0.tar", last modified: Tue May 30 23:03:23 2023, max compression
+gzip compressed data, was "PowerGenome-0.6.1a0.tar", last modified: Thu Jun  8 05:26:42 2023, max compression
```

## Comparing `powergenome-0.6.0a0.tar` & `PowerGenome-0.6.1a0.tar`

### file list

```diff
@@ -1,36 +1,51 @@
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-30 23:03:23.920318 powergenome-0.6.0a0/
--rw-r--r--   0 greg       (501) staff       (20)     1070 2020-09-04 02:25:43.000000 powergenome-0.6.0a0/LICENSE.md
--rw-r--r--   0 greg       (501) staff       (20)      851 2023-05-30 23:03:23.919887 powergenome-0.6.0a0/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)    16121 2023-05-04 20:39:41.000000 powergenome-0.6.0a0/README.md
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-30 23:03:23.915054 powergenome-0.6.0a0/powergenome/
--rw-r--r--   0 greg       (501) staff       (20)    44810 2023-05-24 17:58:28.000000 powergenome-0.6.0a0/powergenome/GenX.py
--rw-r--r--   0 greg       (501) staff       (20)        0 2020-09-04 02:25:43.000000 powergenome-0.6.0a0/powergenome/__init__.py
--rw-r--r--   0 greg       (501) staff       (20)     6669 2023-05-04 20:39:41.000000 powergenome-0.6.0a0/powergenome/cluster_method.py
--rw-r--r--   0 greg       (501) staff       (20)     7980 2023-05-24 17:58:28.000000 powergenome-0.6.0a0/powergenome/co2_pipeline_cost.py
--rw-r--r--   0 greg       (501) staff       (20)      451 2023-05-23 19:09:03.000000 powergenome-0.6.0a0/powergenome/debug.py
--rw-r--r--   0 greg       (501) staff       (20)     9060 2023-05-05 15:59:43.000000 powergenome-0.6.0a0/powergenome/distributed_gen.py
--rw-r--r--   0 greg       (501) staff       (20)    19382 2023-05-24 20:47:20.000000 powergenome-0.6.0a0/powergenome/eia_opendata.py
--rw-r--r--   0 greg       (501) staff       (20)    21118 2023-05-24 17:58:28.000000 powergenome-0.6.0a0/powergenome/external_data.py
--rw-r--r--   0 greg       (501) staff       (20)     7655 2023-05-04 20:39:41.000000 powergenome-0.6.0a0/powergenome/extract_pudl_data.py
--rw-r--r--   0 greg       (501) staff       (20)     4855 2023-05-04 20:39:41.000000 powergenome-0.6.0a0/powergenome/fuels.py
--rw-r--r--   0 greg       (501) staff       (20)   135654 2023-05-30 18:39:37.000000 powergenome-0.6.0a0/powergenome/generators.py
--rw-r--r--   0 greg       (501) staff       (20)      118 2023-05-30 15:59:53.000000 powergenome-0.6.0a0/powergenome/heat_rate.py
--rw-r--r--   0 greg       (501) staff       (20)    11163 2023-05-05 15:59:43.000000 powergenome-0.6.0a0/powergenome/load_construction.py
--rw-r--r--   0 greg       (501) staff       (20)    33579 2023-05-05 15:59:43.000000 powergenome-0.6.0a0/powergenome/load_profiles.py
--rw-r--r--   0 greg       (501) staff       (20)    63849 2023-05-24 17:58:28.000000 powergenome-0.6.0a0/powergenome/nrelatb.py
--rw-r--r--   0 greg       (501) staff       (20)     2271 2023-05-26 18:18:21.000000 powergenome-0.6.0a0/powergenome/params.py
--rw-r--r--   0 greg       (501) staff       (20)     7515 2023-05-04 20:39:41.000000 powergenome-0.6.0a0/powergenome/price_adjustment.py
--rw-r--r--   0 greg       (501) staff       (20)    45015 2023-05-26 18:18:21.000000 powergenome-0.6.0a0/powergenome/resource_clusters.py
--rw-r--r--   0 greg       (501) staff       (20)    17783 2023-05-24 17:58:28.000000 powergenome-0.6.0a0/powergenome/run_powergenome_multiple_outputs_cli.py
--rw-r--r--   0 greg       (501) staff       (20)    14980 2023-05-24 17:58:28.000000 powergenome-0.6.0a0/powergenome/time_reduction.py
--rw-r--r--   0 greg       (501) staff       (20)    11110 2023-05-04 20:39:41.000000 powergenome-0.6.0a0/powergenome/transmission.py
--rw-r--r--   0 greg       (501) staff       (20)    35491 2023-05-25 18:34:26.000000 powergenome-0.6.0a0/powergenome/util.py
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-05-30 23:03:23.919277 powergenome-0.6.0a0/powergenome.egg-info/
--rw-r--r--   0 greg       (501) staff       (20)      851 2023-05-30 23:03:23.000000 powergenome-0.6.0a0/powergenome.egg-info/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)      864 2023-05-30 23:03:23.000000 powergenome-0.6.0a0/powergenome.egg-info/SOURCES.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2023-05-30 23:03:23.000000 powergenome-0.6.0a0/powergenome.egg-info/dependency_links.txt
--rw-r--r--   0 greg       (501) staff       (20)       99 2023-05-30 23:03:23.000000 powergenome-0.6.0a0/powergenome.egg-info/entry_points.txt
--rw-r--r--   0 greg       (501) staff       (20)      453 2023-05-30 23:03:23.000000 powergenome-0.6.0a0/powergenome.egg-info/requires.txt
--rw-r--r--   0 greg       (501) staff       (20)       12 2023-05-30 23:03:23.000000 powergenome-0.6.0a0/powergenome.egg-info/top_level.txt
--rw-r--r--   0 greg       (501) staff       (20)       38 2023-05-30 23:03:23.920446 powergenome-0.6.0a0/setup.cfg
--rw-r--r--   0 greg       (501) staff       (20)     2525 2023-05-30 23:03:14.000000 powergenome-0.6.0a0/setup.py
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.260635 PowerGenome-0.6.1a0/
+-rw-r--r--   0 gs5183     (501) staff       (20)     1070 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/LICENSE.md
+-rw-r--r--   0 gs5183     (501) staff       (20)    16941 2023-06-08 05:26:42.260376 PowerGenome-0.6.1a0/PKG-INFO
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.249740 PowerGenome-0.6.1a0/PowerGenome.egg-info/
+-rw-r--r--   0 gs5183     (501) staff       (20)    16941 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/PKG-INFO
+-rw-r--r--   0 gs5183     (501) staff       (20)     1308 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/SOURCES.txt
+-rw-r--r--   0 gs5183     (501) staff       (20)        1 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/dependency_links.txt
+-rw-r--r--   0 gs5183     (501) staff       (20)       99 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/entry_points.txt
+-rw-r--r--   0 gs5183     (501) staff       (20)      232 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/requires.txt
+-rw-r--r--   0 gs5183     (501) staff       (20)       17 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/top_level.txt
+-rw-r--r--   0 gs5183     (501) staff       (20)    16060 2023-06-08 05:16:33.000000 PowerGenome-0.6.1a0/README.md
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.249896 PowerGenome-0.6.1a0/data/
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.255083 PowerGenome-0.6.1a0/data/additional_technologies/
+-rw-r--r--   0 gs5183     (501) staff       (20)     1083 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/additional_technologies/AZ_additional_tech.csv
+-rw-r--r--   0 gs5183     (501) staff       (20)      823 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/additional_technologies/AZ_additional_tech_2030.csv
+-rw-r--r--   0 gs5183     (501) staff       (20)      822 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/additional_technologies/AZ_additional_tech_2045.csv
+-rw-r--r--   0 gs5183     (501) staff       (20)      625 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/additional_technologies/sample_additional_tech.csv
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.255232 PowerGenome-0.6.1a0/data/coal_fgd/
+-rw-r--r--   0 gs5183     (501) staff       (20)    15123 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/coal_fgd/fgd_output.csv
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.255548 PowerGenome-0.6.1a0/data/cost_multipliers/
+-rw-r--r--   0 gs5183     (501) staff       (20)     6226 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/cost_multipliers/AEO_2020_regional_cost_corrections.csv
+-rw-r--r--   0 gs5183     (501) staff       (20)     1844 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/cost_multipliers/EIA regional cost multipliers.csv
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.255706 PowerGenome-0.6.1a0/data/cpi_data/
+-rw-r--r--   0 gs5183     (501) staff       (20)      694 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/data/cpi_data/cpi_data.csv
+-rw-r--r--   0 gs5183     (501) staff       (20)  7754322 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/ipm_regions_simple.geojson
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.259538 PowerGenome-0.6.1a0/powergenome/
+-rw-r--r--   0 gs5183     (501) staff       (20)    44811 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/GenX.py
+-rw-r--r--   0 gs5183     (501) staff       (20)       23 2023-06-08 02:26:41.000000 PowerGenome-0.6.1a0/powergenome/__init__.py
+drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.259894 PowerGenome-0.6.1a0/powergenome/cluster/
+-rw-r--r--   0 gs5183     (501) staff       (20)    20651 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/cluster/renewables.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     6669 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/cluster_method.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     7980 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/co2_pipeline_cost.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     9047 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/distributed_gen.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    19178 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/eia_opendata.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    21119 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/external_data.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     7656 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/extract_pudl_data.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     4856 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/fuels.py
+-rw-r--r--   0 gs5183     (501) staff       (20)   135331 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/generators.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    11145 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/load_construction.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    33579 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/load_profiles.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    63909 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/nrelatb.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     2381 2023-06-08 03:45:29.000000 PowerGenome-0.6.1a0/powergenome/params.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     7516 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/price_adjustment.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    45619 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/resource_clusters.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    17869 2023-06-08 03:49:06.000000 PowerGenome-0.6.1a0/powergenome/run_powergenome_multiple_outputs_cli.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    14981 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/time_reduction.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    11110 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/transmission.py
+-rw-r--r--   0 gs5183     (501) staff       (20)    36496 2023-06-08 03:59:24.000000 PowerGenome-0.6.1a0/powergenome/util.py
+-rw-r--r--   0 gs5183     (501) staff       (20)       23 2023-06-08 01:52:09.000000 PowerGenome-0.6.1a0/powergenome/version.py
+-rw-r--r--   0 gs5183     (501) staff       (20)     1730 2023-06-08 03:23:37.000000 PowerGenome-0.6.1a0/pyproject.toml
+-rw-r--r--   0 gs5183     (501) staff       (20)       38 2023-06-08 05:26:42.260707 PowerGenome-0.6.1a0/setup.cfg
```

### Comparing `powergenome-0.6.0a0/LICENSE.md` & `PowerGenome-0.6.1a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.0a0/README.md` & `PowerGenome-0.6.1a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: PowerGenome
+Version: 0.6.1a0
+Summary: Create power system inputs for capacity expansion models
+Author-email: Greg Schivley <greg.schivley@princeton.edu>
+Maintainer-email: Greg Schivley <greg.schivley@princeton.edu>
+License: MIT
+Project-URL: Source, https://github.com/PowerGenome/PowerGenome
+Keywords: power system data,capacity expansion,two
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.md
+
 # PowerGenome
 
 [![The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![code style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4426097.svg)](https://doi.org/10.5281/zenodo.4426096)
 [![pytest](https://github.com/PowerGenome/PowerGenome/actions/workflows/pytest.yml/badge.svg)](https://github.com/PowerGenome/PowerGenome/actions/workflows/pytest.yml)
 [![codecov](https://codecov.io/gh/PowerGenome/PowerGenome/branch/master/graph/badge.svg?token=7KJYLE3jOW)](https://codecov.io/gh/PowerGenome/PowerGenome)
@@ -34,43 +57,23 @@
 - A simplified geojson version of EPA's shapefile for IPM regions (`data/ipm_regions_simple.geojson`).
 - Information on user-defined technologies, which can be included in outputs. This can be used to define a custom cost case (e.g. $500/kW PV) or a new technology such as natural gas with 100% carbon capture. The CSV files are stored in the `extra_inputs` subfolders of each example system. A documentation file in that folder describes what to include in the file.
 
 ## PUDL Dependency
 
 This project pulls data from [PUDL](https://github.com/catalyst-cooperative/pudl). As such, it requires installation of PUDL to access a normalized sqlite database and some of the convienience PUDL functions.
 
-`catalystcoop.pudl` is included in the `environment.yml` file and will be installed automatically in the conda environment (see instructions below). Catalyst Cooperative will be creating versioned data releases of PUDL, which can be [accessed on Zenodo](https://doi.org/10.5281/zenodo.3653158). Download the zip file from Zenodo, unzip it, and find the sqlite database under `pudl_data/sqlite/pudl.sqlite`. Note that the version of `catalystcoop.pudl` software may change based on the database version you use. Look on the right-hand side of the zenodo archive to see what software version was used to compile the data. If the version in your conda environment does not match the version used to compile the data, you can change it in the `environment.yml` file or install a [different version](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-packages) using `conda install catalystcoop.pudl=<your_version>`.
+`catalystcoop.pudl` is included in the `environment.yml` file and will be installed automatically in the conda environment (see instructions below). Catalyst Cooperative will be creating versioned data releases of PUDL, which can be [accessed on Zenodo](https://doi.org/10.5281/zenodo.3653158). Download the zip file from Zenodo, unzip it, and find the sqlite database under `pudl_data/sqlite/pudl.sqlite`. Note that the version of `catalystcoop.pudl` software may change based on the database version you use. Look on the right-hand side of the zenodo archive to see what software version was used to compile the data. If the version in your conda environment does not match the version used to compile the data, you can change it in the `environment.yml` file or install a [different version](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-packages) using `mamba install catalystcoop.pudl=<your_version>`.
 
 ![PUDL software version for database](/docs/_static/pudl_version.png)
 
-**IMPORTANT UPDATE:** As of December 2021, our pinned `catalystcoop.pudl` dependency has bumped from 0.3.* to 0.5.* This version bump is associated with some changes in the PUDL database structure and an increase in the Pandas dependency from 0.25.* to 1.* If you are running an older version of PowerGenome it may be easiest to [remove the existing `powergenome` conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#removing-an-environment) and reinstall it.
-
-```sh
-conda remove --name powergenome --all
-```
-
-Alternatively, you can [update your existing environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#updating-an-environment).
-
-```sh
-conda env update --file environment.yml  --prune
-```
-
-Either way, you will need to download the new database files in steps 5/6 below and update your `.env` file.
-
-## Installation
+## Installation from GitHub
 
 1. Clone this repository to your local machine and navigate to the top level (PowerGenome) folder.
 
-2. Create a conda environment named `powergenome` using the provided `environment.yml` file. If you don't already use conda, [download and install miniconda](https://docs.conda.io/en/latest/miniconda.html). Note that resolving all the dependencies can be slow with conda, so I highly recommend that you [install mamba](https://mamba.readthedocs.io/en/latest/installation.html#existing-conda-install) and use it instead (just sub `mamba` for `conda` below). Mamba installation is easy and will probably take less time than sitting around while conda resolves dependencies.
-
-```sh
-conda env create -f environment.yml
-```
-
-or if you installed mamba:
+2. Create a conda environment named `powergenome` using the provided `environment.yml` file. If you don't already use conda it is easiest to download and install [Mambaforge](https://github.com/conda-forge/miniforge#mambaforge), which will install conda with mamba in the `base` environment. See [this description](https://bioconda.github.io/faqs.html#what-s-the-difference-between-miniconda-miniforge-mambaforge-micromamba) for more information on the difference between different ways to install conda and mamba. Conda usually fail to resolve dependencies in under a day so I highly recommend that you either start with Mambaforge or [install mamba in your `base` environment](https://mamba.readthedocs.io/en/latest/installation.html#existing-conda-install) and use it instead.
 
 ```sh
 mamba env create -f environment.yml
 ```
 
 3. Activate the `powergenome` environment.
 
@@ -80,32 +83,41 @@
 
 4. pip-install an editable version of this project
 
 ```sh
 pip install -e .
 ```
 
-5. Download [the PUDL database](https://doi.org/10.5281/zenodo.3653158), unzip it, and copy the `/pudl_data/sqlite/pudl.sqlite` to wherever you would like to store PowerGenome data on your computer. The zip file contains other data sets that aren't needed for PowerGenome and can be deleted.  Note that as of December 2021 the most recent version of this database (Data Release v3.0.0) is compatible with `catalystcoop.pudl` version 0.5.* and will not work if an earlier version is included in your conda environment.
+5. Download [the PUDL database](https://doi.org/10.5281/zenodo.3653158), unzip it, and copy the `/pudl_data/sqlite/pudl.sqlite` to wherever you would like to store PowerGenome data on your computer. The zip file contains other data sets that aren't needed for PowerGenome and can be deleted.  Note that as of May 2023 the most recent version of this database (v2022.11.30) is compatible with `catalystcoop.pudl` version v2022.11.30 and may not work if an earlier software version is included in your conda environment.
 
 6. Download [additional PowerGenome data](https://drive.google.com/file/d/1LCB0uwnx6VHrmHQDPH2huLHU6fKXb7kG/view?usp=sharing) that includes NREL ATB cost data, transmission constraints between IPM regions, and hourly demand for each IPM region. Hourly demand is based on a 2012 weather year and was constructed either directly from FERC 714 data (`load_curves_ferc`) or from NREL EFS data (`load_curves_nrel_efs`) that also sources back to FERC 714. The NREL load curves, which separate hourly demand by sector and subsector, are now the default source for load curves in PowerGenome. See [the wiki](https://github.com/PowerGenome/PowerGenome/wiki/Settings-files#demand) for more information. These files will eventually be provided through a data repository with citation information.
 
-7. Download the [renewable resource data](https://drive.google.com/file/d/1g0Q6TdNp4C12HQJy6pAURzp_oVg0Q7ly/view?usp=sharing) containing generation profiles and capacity for existing and new-build renewable resources. Save and unzip this file. The suggested location for all of the unzipped files is `PowerGenome/data/resource_groups/`. These files will eventually be provided through a data repository with citation information.
+7. Download the appropriate [renewable resource data files](https://drive.google.com/drive/folders/1G9IHtY1RMZHUEXAmYQEb-mvzzhqun-Kb?usp=sharing). Read through the README for more background. This folder contains:
 
-8. Download and unzip [data files derived from NREL's EFS](https://drive.google.com/file/d/1bS-5LycImdp1AYoS_0uK7tXRHo8TWKCD/view?usp=sharing)
+- `generation_profiles` can be saved in a single place and used across multiple studies.
+- Each of the folders under `resource_groups` has CSV files that tell PowerGenome the metro that each potential wind/solar site will deliver power to based on a set of regional aggregations. Use the corresponding regional aggregations in your settings file. You can request new resource group files for different regional aggregations on the [repository discussion page](https://github.com/PowerGenome/PowerGenome/discussions)
 
-9. Get an [API key for EIA's OpenData portal](https://www.eia.gov/opendata/register.php). This key is needed to download projected fuel prices and regonal demand growth from EIA's Annual Energy Outlook.
+8. Download and unzip [data files derived from NREL's EFS](https://drive.google.com/file/d/1bS-5LycImdp1AYoS_0uK7tXRHo8TWKCD/view?usp=sharing) that provide hourly demand profiles for growing electrification technologies like electric vehicles and heat pumps.
 
-10. Create the file `PowerGenome/powergenome/.env`. In this file, add:
+9. Download and unzip [distributed generation profiles](https://drive.google.com/file/d/1kqBQle2CLET_BMZd0Y91o6AjfgunQKf4/view?usp=share_link) compiled from NREL Cambium 2022 scenarios.
+
+9. Create the file `PowerGenome/powergenome/.env`. In this file, add:
 
 - `PUDL_DB=YOUR_PATH_HERE` (your path to the PUDL database downloaded in step 5)
 - `PG_DB=YOUR_PATH_HERE` (your path to the additional PowerGenome data downloaded in step 6)
-- `EIA_API_KEY=YOUR_KEY_HERE` (your EIA API key)
-- `RESOURCE_GROUPS=YOUR_PATH_HERE` (your path to where the resource groups data from Step 6 are saved)
+- `RESOURCE_GROUP_PROFILES=YOUR_PATH_HERE` (your path to the folder with hourly wind/solar generation parquet files)
 - `EFS_DATA=YOUR_PATH_HERE` (your path to the folder with EFS derived data files)
-Quotation marks are only needed if your values contain spaces. The `.env` file is included in `.gitignore` and will not be synced with the repository. See the [SQLAlchemy documentation](https://docs.sqlalchemy.org/en/13/dialects/sqlite.html#connect-strings) for examples of how to format the `PUDL_DB` and `PG_DB` paths (e.g. `sqlite:////<entire path to the folder containing pudl file>/pudl.sqlite`, or `sqlite:///C:/path/to/folder/pudl.sqlite` on Windows). If you get any errors when trying to initite the PUDL database, go back and check your path formatting against the SQLAlchemy documentation examples.
+- `DISTRIBUTED_GEN_DATA=YOUR_PATH_HERE` (your path to the folder with distributed generation profiles)
+- OPTIONAL: `RESOURCE_GROUPS=YOUR_PATH_HERE` (your path to the resource groups data for a project -- **this can be included in your settings file instead of the .env file**)
+
+Quotation marks are only needed if your values contain spaces. The `.env` file is included in `.gitignore` and will not be synced with the repository.
+
+## Installation a packaged version (pip/conda-forge)
+
+If you are installing a packaged version of PowerGenome you won't be able to easily use a .env file. Instead, add the environment parameters (`PUDL_DB`, `PG_DB`, etc) to a YAML file in the same folder as the rest of your settings. It doesn't really matter which file these parameters are included in but creating a new file such as `env.yml` will help keep them separate from other settings parameters that might be shared with other PowerGenome users.
 
 ## Running code
 
 ### Suggested folder structure
 
 It is best practice to set up project folders outside of the cloned repository so that git doesn't track any new/changed files within the upper-level `PowerGenome` folder. Try copying one of the example systems (settings file and extra inputs) and modifying it. Copy the `notebooks` folder into your project folder, change the path to the settings file as needed, and run code in the notebooks. This can also be a good way to learn how data are created in PowerGenome and debug problem.
```

### Comparing `powergenome-0.6.0a0/powergenome/GenX.py` & `PowerGenome-0.6.1a0/powergenome/GenX.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 "Functions specific to GenX outputs"
 
-from itertools import product
 import logging
+from itertools import product
 from pathlib import Path
 from typing import Dict, List
+
 import pandas as pd
 
 from powergenome.external_data import (
-    load_policy_scenarios,
     load_demand_segments,
+    load_policy_scenarios,
     load_user_genx_settings,
     make_generator_variability,
 )
 from powergenome.load_profiles import make_distributed_gen_profiles
+from powergenome.nrelatb import investment_cost_calculator
 from powergenome.time_reduction import kmeans_time_clustering
 from powergenome.util import find_region_col, load_settings, snake_case_col
-from powergenome.nrelatb import investment_cost_calculator
 
 logger = logging.getLogger(__name__)
 
 INT_COLS = [
     "Inv_Cost_per_MWyr",
     "Fixed_OM_Cost_per_MWyr",
     "Inv_Cost_per_MWhyr",
```

### Comparing `powergenome-0.6.0a0/powergenome/cluster_method.py` & `PowerGenome-0.6.1a0/powergenome/cluster_method.py`

 * *Files identical despite different names*

### Comparing `powergenome-0.6.0a0/powergenome/co2_pipeline_cost.py` & `PowerGenome-0.6.1a0/powergenome/co2_pipeline_cost.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 "Load data from file for pipeline/transport/injection costs"
 
+import logging
 from pathlib import Path
 from typing import Dict, List
 
 import pandas as pd
-import logging
-from powergenome.price_adjustment import inflation_price_adjustment
 
-from powergenome.util import snake_case_col, snake_case_str
 from powergenome.params import DATA_PATHS
+from powergenome.price_adjustment import inflation_price_adjustment
+from powergenome.util import snake_case_col, snake_case_str
 
 logger = logging.getLogger(__name__)
 
 
 def merge_co2_pipeline_costs(
     df: pd.DataFrame,
     co2_data_path: Path,
```

### Comparing `powergenome-0.6.0a0/powergenome/distributed_gen.py` & `PowerGenome-0.6.1a0/powergenome/distributed_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-from pathlib import Path
-from typing import Dict, List
-import os
 import logging
+import os
 from functools import lru_cache
+from pathlib import Path
+from typing import Dict, List
 
 import pandas as pd
 import pyarrow.parquet as pq
 
-from powergenome.util import (
-    deep_freeze_args,
-    snake_case_col,
-)
-from powergenome.params import SETTINGS
 from powergenome.load_construction import us_state_abbrev
+from powergenome.params import SETTINGS
+from powergenome.util import deep_freeze_args, snake_case_col
 
 logger = logging.getLogger(__name__)
 
 
 def load_region_pop_frac(
     path_in: Path,
     fn: str = "ipm_state_pop_weight_20220329.csv",
```

### Comparing `powergenome-0.6.0a0/powergenome/eia_opendata.py` & `PowerGenome-0.6.1a0/powergenome/eia_opendata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
-Load data from EIA's Open Data API. Requires an api key, which should be included in a
-.env file (/powergenome/.env) with the format EIA_API_KEY=YOUR_API_KEY
+Load data from EIA's bulk data
 """
 
-from itertools import product
 import logging
 import operator
+import zipfile
+from itertools import product
 from typing import Union
 
 import pandas as pd
 import requests
-import zipfile
 
-from powergenome.params import SETTINGS, DATA_PATHS
+from powergenome.params import DATA_PATHS, SETTINGS
 from powergenome.price_adjustment import inflation_price_adjustment
 from powergenome.util import download_save, reverse_dict_of_lists
 
 logger = logging.getLogger(__name__)
 
 numeric = Union[int, float]
 
@@ -174,15 +173,14 @@
 
     >>> fuel_price = fetch_fuel_prices(settings)
     ************
     Unable to inflate fuel prices. Check your settings file to ensure the keys
     "target_usd_year" and "aeo_fuel_usd_year" exist and are valid integers.
     ************
     """
-    API_KEY = SETTINGS["EIA_API_KEY"]
 
     if settings.get("fuel_eia_aeo_year"):
         aeo_year = settings.get("fuel_eia_aeo_year")
     else:
         aeo_year = settings.get("eia_aeo_year")
 
     if not aeo_year:
@@ -507,16 +505,14 @@
        year      demand
     0  2050  489.009247
     1  2049  483.176544
     2  2048  477.624481
     3  2047  472.314972
     4  2046  466.875671
     """
-    API_KEY = SETTINGS["EIA_API_KEY"]
-
     SERIES_ID = (
         f"AEO.{aeo_year}.{scenario_series}.CNSM_NA_{sector}_NA_ELC_NA_{region}_BLNKWH.A"
     )
 
     df = load_aeo_series(SERIES_ID)
     df["year"] = df["year"].astype(int)
```

### Comparing `powergenome-0.6.0a0/powergenome/external_data.py` & `PowerGenome-0.6.1a0/powergenome/external_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Read in and add external inputs (user-supplied files) to PowerGenome outputs
 
 import logging
-import numpy as np
-import pandas as pd
 from pathlib import Path
 from typing import Any, List
 
-from powergenome.util import snake_case_col, remove_feb_29
+import numpy as np
+import pandas as pd
+
 from powergenome.price_adjustment import inflation_price_adjustment
+from powergenome.util import remove_feb_29, snake_case_col
 
 logger = logging.getLogger(__name__)
 
 
 def make_demand_response_profiles(
     path: Path, resource_name: str, year: int, scenario: str
 ) -> pd.DataFrame:
```

### Comparing `powergenome-0.6.0a0/powergenome/extract_pudl_data.py` & `PowerGenome-0.6.1a0/powergenome/extract_pudl_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import logging
 import shutil
 import sys
 from datetime import datetime as dt
 
 import pandas as pd
+
 import powergenome
 from powergenome.fuels import fuel_cost_table
 from powergenome.generators import GeneratorClusters, load_ipm_shapefile
 from powergenome.load_profiles import make_final_load_curves
 from powergenome.params import DATA_PATHS
 from powergenome.transmission import (
     agg_transmission_constraints,
```

### Comparing `powergenome-0.6.0a0/powergenome/fuels.py` & `PowerGenome-0.6.1a0/powergenome/fuels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Load fuel prices needed for the model
 """
 
 from asyncio.log import logger
+
 import pandas as pd
 
 from powergenome.eia_opendata import add_user_fuel_prices
 
 
 def fuel_cost_table(fuel_costs, generators, settings):
     all_fuel_costs = add_user_fuel_prices(settings, fuel_costs)
```

### Comparing `powergenome-0.6.0a0/powergenome/generators.py` & `PowerGenome-0.6.1a0/powergenome/generators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,67 +1,63 @@
 import collections
 import logging
+import re
 from numbers import Number
+from pathlib import Path
 from typing import Dict, List, Union
-import re
 from zipfile import BadZipFile
 
-import requests
-
 import geopandas as gpd
 import numpy as np
 import pandas as pd
-from pathlib import Path
 import pudl
+import requests
+import sqlalchemy
 from bs4 import BeautifulSoup
 from flatten_dict import flatten
-import sqlalchemy
+from scipy.stats import iqr
+from sklearn import cluster, preprocessing
+from xlrd import XLRDError
+
 from powergenome.cluster_method import (
     cluster_by_owner,
     cluster_kmeans,
     weighted_ownership_by_unit,
 )
 from powergenome.co2_pipeline_cost import merge_co2_pipeline_costs
 from powergenome.eia_opendata import fetch_fuel_prices, modify_fuel_prices
 from powergenome.external_data import (
-    make_demand_response_profiles,
-    demand_response_resource_capacity,
     add_resource_max_cap_spur,
+    demand_response_resource_capacity,
+    make_demand_response_profiles,
 )
+from powergenome.GenX import rename_gen_cols
 from powergenome.load_profiles import make_distributed_gen_profiles
 from powergenome.nrelatb import (
     atb_fixed_var_om_existing,
     atb_new_generators,
     fetch_atb_costs,
     fetch_atb_heat_rates,
     fetch_atb_offshore_spur_costs,
     investment_cost_calculator,
 )
-from powergenome.params import (
-    DATA_PATHS,
-    IPM_GEOJSON_PATH,
-    build_resource_clusters,
-)
+from powergenome.params import DATA_PATHS, IPM_GEOJSON_PATH, build_resource_clusters
 from powergenome.price_adjustment import inflation_price_adjustment
 from powergenome.resource_clusters import map_eia_technology
 from powergenome.util import (
     download_save,
     find_region_col,
+    load_ipm_shapefile,
     map_agg_region_names,
+    regions_to_keep,
+    remove_leading_zero,
     reverse_dict_of_lists,
     snake_case_col,
-    regions_to_keep,
     snake_case_str,
-    load_ipm_shapefile,
-    remove_leading_zero,
 )
-from powergenome.GenX import rename_gen_cols
-from scipy.stats import iqr
-from sklearn import cluster, preprocessing
-from xlrd import XLRDError
 
 logger = logging.getLogger(__name__)
 
 
 planned_col_map = {
     "Entity ID": "utility_id_eia",
     "Entity Name": "utility_name",
@@ -1967,22 +1963,17 @@
         The dictionary of settings with a dictionary of region aggregations
 
     Returns
     -------
     DataFrame
         A dataframe with the capacity factor of every selected technology
     """
-    data_years = [str(y) for y in settings["data_years"]]
+    data_years = [str(y) for y in settings["eia_data_years"]]
     data_years.extend(settings.get("capacity_factor_default_year_filter", []))
-    if type(settings.get("alt_year_filters")) is dict:
-        for tech, value in settings["alt_year_filters"].items():
-            if isinstance(value, list):
-                data_years.extend(value)
-            else:
-                data_years.append(value)
+
     cap_col = settings["capacity_col"]
 
     # Include standby (SB) generators since they are in our capacity totals
     sql = f"""
         SELECT
             G.report_date,
             G.plant_id_eia,
@@ -2064,40 +2055,18 @@
         capacity_factor = group_technologies(
             capacity_factor,
             settings["group_technologies"],
             settings.get("tech_groups", {}) or {},
             settings.get("regional_no_grouping", {}) or {},
         )
 
-    if years_filter is None:
-        years_filter = {
-            tech: settings["capacity_factor_default_year_filter"]
-            for tech in plant_gen_tech_cap["technology_description"].unique()
-        }
-        if type(settings.get("alt_year_filters")) is dict:
-            for tech, value in settings["alt_year_filters"].items():
-                years_filter[tech] = value
-
-        data_years = plant_gen_tech_cap["report_date"].dt.year.unique()
-
-        # Use all years where the value is None
-
-        for tech, value in years_filter.items():
-            if value is None:
-                years_filter[tech] = data_years
-
-    df_list = []
-    for tech, years in years_filter.items():
-        _df = capacity_factor.loc[
-            (capacity_factor["technology_description"] == tech)
-            & (capacity_factor["report_date"].dt.year.isin(years)),
-            :,
-        ]
-        df_list.append(_df)
-    capacity_factor = pd.concat(df_list, sort=False)
+    cf_years = settings.get("capacity_factor_default_year_filter", data_years)
+    capacity_factor = capacity_factor.loc[
+        capacity_factor["report_date"].dt.year.isin(cf_years)
+    ]
 
     # get a unique set of dates to generate the number of hours
     dates = capacity_factor["report_date"].drop_duplicates()
     dates_to_hours = pd.DataFrame(
         data={
             "report_date": dates,
             "hours": dates.apply(
@@ -2111,14 +2080,26 @@
     )
 
     # merge in the hours for the calculation
     capacity_factor = capacity_factor.merge(dates_to_hours, on=["report_date"])
     capacity_factor["potential_generation_mwh"] = (
         capacity_factor[cap_col] * capacity_factor["hours"]
     )
+    plant_tech_capacity_factor = capacity_factor.groupby(
+        ["plant_id_eia", "technology_description"], as_index=False
+    )[["potential_generation_mwh", "net_generation_mwh"]].sum()
+
+    plant_tech_capacity_factor["capacity_factor"] = (
+        plant_tech_capacity_factor["net_generation_mwh"]
+        / plant_tech_capacity_factor["potential_generation_mwh"]
+    )
+    plant_tech_capacity_factor.rename(
+        columns={"technology_description": "technology"},
+        inplace=True,
+    )
 
     capacity_factor_tech_region = capacity_factor.groupby(
         ["model_region", "technology_description"], as_index=False
     )[["potential_generation_mwh", "net_generation_mwh"]].sum()
 
     # actually calculate capacity factor wooo!
     capacity_factor_tech_region["capacity_factor"] = (
@@ -2129,15 +2110,15 @@
     capacity_factor_tech_region.rename(
         columns={"model_region": "region", "technology_description": "technology"},
         inplace=True,
     )
 
     logger.debug(capacity_factor_tech_region)
 
-    return capacity_factor_tech_region
+    return plant_tech_capacity_factor, capacity_factor_tech_region
 
 
 def add_fuel_labels(df, fuel_prices, settings):
     """Add a Fuel column with the approproriate regional fuel for each generator type
 
     Parameters
     ----------
@@ -2804,15 +2785,15 @@
         self.weighted_unit_hr = None
         self.supplement_with_860m = supplement_with_860m
         self.cluster_builder = build_resource_clusters(
             self.settings.get("RESOURCE_GROUPS")
         )
 
         if self.current_gens:
-            self.data_years = self.settings["data_years"]
+            self.data_years = self.settings.get("eia_data_years") or []
 
             self.gens_860 = load_generator_860_data(self.pudl_engine, self.data_years)
             self.gens_entity = pd.read_sql_table(
                 "generators_entity_eia", self.pudl_engine
             )
 
             bga = self.pudl_out.bga_eia860()
@@ -3395,27 +3376,14 @@
             on=["plant_id_eia", "unit_id_pg"],
             how="inner",
         ).merge(
             self.plants_860[["plant_id_eia", "utility_id_eia"]],
             on=["plant_id_eia"],
             how="left",
         )
-        if self.settings.get("extra_outputs"):
-            self.all_units = self.all_units.rename(columns={"model_region": "region"})
-            self.all_units["Resource"] = (
-                self.all_units["region"]
-                + "_"
-                + snake_case_col(self.all_units["technology"])
-                + "_"
-                + self.all_units["cluster"].astype(str)
-            )
-            self.all_units.to_csv(
-                Path(self.settings["extra_outputs"]) / "existing_gen_units.csv",
-                index=False,
-            )
 
         logger.info("Finalizing generation clusters")
         self.results = pd.concat(self.cluster_list)
         logger.info(
             f"Results technologies are {self.results.technology.unique().tolist()}"
         )
 
@@ -3434,45 +3402,68 @@
                 self.settings["capacity_col"]: "Cap_Size",
                 "heat_rate_mmbtu_mwh": "Heat_Rate_MMBTU_per_MWh",
             },
             inplace=True,
         )
 
         # Calculate average capacity factors
-        if type(self.settings.get("capacity_factor_techs")) is list:
-            self.capacity_factors = gentype_region_capacity_factor(
+        if self.settings.get("derate_techs"):
+            (
+                plant_tech_cf,
+                self.region_tech_capacity_factors,
+            ) = gentype_region_capacity_factor(
                 self.pudl_engine,
                 self.units_model[["plant_id_eia", "model_region"]],
                 self.settings,
             )
+            self.all_units = pd.merge(
+                self.all_units,
+                plant_tech_cf,
+                how="left",
+                on=["plant_id_eia", "technology"],
+            )
 
             self.results = pd.merge(
                 self.results.reset_index(),
-                self.capacity_factors[["region", "technology", "capacity_factor"]],
+                self.region_tech_capacity_factors[
+                    ["region", "technology", "capacity_factor"]
+                ],
                 on=["region", "technology"],
                 how="left",
             )
 
-            if self.settings.get("derate_capacity"):
-                derate_techs = self.settings["derate_techs"]
-                self.results.loc[:, "unmodified_cap_size"] = self.results.loc[
-                    :, "Cap_Size"
-                ].copy()
+            derate_techs = self.settings["derate_techs"]
+            self.results.loc[:, "unmodified_cap_size"] = self.results.loc[
+                :, "Cap_Size"
+            ].copy()
+            self.results.loc[
+                self.results["technology"].isin(derate_techs), "Cap_Size"
+            ] = (
                 self.results.loc[
-                    self.results["technology"].isin(derate_techs), "Cap_Size"
-                ] = (
-                    self.results.loc[
-                        self.results["technology"].isin(derate_techs),
-                        "unmodified_cap_size",
-                    ]
-                    * self.results.loc[
-                        self.results["technology"].isin(derate_techs), "capacity_factor"
-                    ]
-                )
+                    self.results["technology"].isin(derate_techs),
+                    "unmodified_cap_size",
+                ]
+                * self.results.loc[
+                    self.results["technology"].isin(derate_techs), "capacity_factor"
+                ]
+            )
 
+        if self.settings.get("extra_outputs"):
+            self.all_units = self.all_units.rename(columns={"model_region": "region"})
+            self.all_units["Resource"] = (
+                self.all_units["region"]
+                + "_"
+                + snake_case_col(self.all_units["technology"])
+                + "_"
+                + self.all_units["cluster"].astype(str)
+            )
+            self.all_units.to_csv(
+                Path(self.settings["extra_outputs"]) / "existing_gen_units.csv",
+                index=False,
+            )
         # Round Cap_size to prevent GenX error.
         self.results = self.results.round(3)
         self.results["Cap_Size"] = self.results["Cap_Size"]
         self.results["Existing_Cap_MW"] = self.results.Cap_Size * self.results.num_units
         if self.settings.get("derate_capacity"):
             self.results["unmodified_existing_cap_mw"] = (
                 self.results["unmodified_cap_size"] * self.results["num_units"]
```

### Comparing `powergenome-0.6.0a0/powergenome/load_construction.py` & `PowerGenome-0.6.1a0/powergenome/load_construction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-from typing import Dict, List, Union
-import numpy as np
-import pandas as pd
-import os
 import logging
+import os
 from functools import lru_cache
-
 from pathlib import Path
+from typing import Dict, List, Union
 
+import numpy as np
+import pandas as pd
 
-from powergenome.util import (
-    deep_freeze_args,
-    find_region_col,
-    snake_case_col,
-)
 from powergenome.params import DATA_PATHS, SETTINGS
+from powergenome.util import deep_freeze_args, find_region_col, snake_case_col
 
 logger = logging.getLogger(__name__)
 
 
 us_state_abbrev = {
     "Alabama": "AL",
     "Alaska": "AK",
```

### Comparing `powergenome-0.6.0a0/powergenome/load_profiles.py` & `PowerGenome-0.6.1a0/powergenome/load_profiles.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from inspect import signature
 from pathlib import Path
 from typing import Dict, List, Tuple
 
 import numpy as np
 import pandas as pd
 import sqlalchemy as sa
-from powergenome.distributed_gen import distributed_gen_profiles
 
-from powergenome.load_construction import electrification_profiles
+from powergenome.distributed_gen import distributed_gen_profiles
 from powergenome.eia_opendata import get_aeo_load
 from powergenome.external_data import make_demand_response_profiles
+from powergenome.load_construction import electrification_profiles
 from powergenome.util import (
     find_region_col,
     map_agg_region_names,
     regions_to_keep,
-    reverse_dict_of_lists,
     remove_feb_29,
+    reverse_dict_of_lists,
 )
 
 logger = logging.getLogger(__name__)
 
 
 def filter_load_by_region(load_source):  # "decorator factory"
     """If regional load options are given, return the columns listed in
```

### Comparing `powergenome-0.6.0a0/powergenome/nrelatb.py` & `PowerGenome-0.6.1a0/powergenome/nrelatb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
 Functions to fetch and modify NREL ATB data from PUDL
 """
 
-import copy
 import collections
+import copy
 import logging
 import operator
 from pathlib import Path
 from typing import Dict, List, Tuple, Union
-from joblib import Parallel, delayed
 
 import numpy as np
 import pandas as pd
 import sqlalchemy
-from powergenome.cluster.renewables import assign_site_cluster, calc_cluster_values
+from joblib import Parallel, delayed
 
+from powergenome.cluster.renewables import assign_site_cluster, calc_cluster_values
 from powergenome.params import DATA_PATHS, SETTINGS, build_resource_clusters
 from powergenome.price_adjustment import inflation_price_adjustment
 from powergenome.resource_clusters import (
     ClusterBuilder,
     ResourceGroup,
     Table,
     map_nrel_atb_technology,
 )
 from powergenome.util import (
     apply_all_tag_to_regions,
-    reverse_dict_of_lists,
     remove_leading_zero,
+    reverse_dict_of_lists,
     snake_case_col,
     snake_case_str,
 )
 
 idx = pd.IndexSlice
 logger = logging.getLogger(__name__)
 
@@ -1538,14 +1538,16 @@
                     renew_data=renew_data,
                     profile_path=resource_groups[0].group.get("profiles"),
                     regions=regions,
                     site_map=site_map,
                     utc_offset=settings.get("utc_offset", 0),
                     **_scenario,
                 )
+                if data.empty:
+                    continue
                 clusters = (
                     data.groupby("cluster", as_index=False)
                     .apply(calc_cluster_values)
                     .rename(columns={"mw": "Max_Cap_MW"})
                     .assign(technology=technology, region=region)
                 )
```

### Comparing `powergenome-0.6.0a0/powergenome/params.py` & `PowerGenome-0.6.1a0/powergenome/params.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 Parameters and settings
 """
-from typing import Union
 import os
 from pathlib import Path
+from typing import Union
 
 from dotenv import find_dotenv, load_dotenv
 
 from powergenome import __file__
 from powergenome.resource_clusters import ClusterBuilder
+from powergenome.util import sqlalchemy_prefix
 
 # Not convinced this is the best way to set folder paths but it works!
 powergenome_path = Path(__file__).parent
 project_path = powergenome_path.parent
 
 load_dotenv(dotenv_path=powergenome_path / ".env")
 
+
 DATA_PATHS = {}
 DATA_PATHS["results"] = project_path / "results"
 DATA_PATHS["powergenome"] = project_path / "powergenome"
 DATA_PATHS["data"] = project_path / "data"
 DATA_PATHS["atb_storage_costs"] = DATA_PATHS["data"] / "NREL_ATB_battery_costs.csv"
 DATA_PATHS["ipm_shapefiles"] = DATA_PATHS["data"] / "IPM Regions v617 04-05-17"
 DATA_PATHS["tests"] = project_path / "tests"
@@ -34,20 +36,20 @@
 DATA_PATHS["coal_fgd"] = DATA_PATHS["data"] / "coal_fgd" / "fgd_output.csv"
 DATA_PATHS["cpi_data"] = DATA_PATHS["data"] / "cpi_data" / "cpi_data.csv"
 
 IPM_SHAPEFILE_PATH = DATA_PATHS["ipm_shapefiles"] / "IPM_Regions_201770405.shp"
 IPM_GEOJSON_PATH = DATA_PATHS["data"] / "ipm_regions_simple.geojson"
 
 SETTINGS = {}
-SETTINGS["PUDL_DB"] = os.environ.get("PUDL_DB")
-SETTINGS["PG_DB"] = os.environ.get("PG_DB")
-SETTINGS["EIA_API_KEY"] = os.environ.get("EIA_API_KEY")
+SETTINGS["PUDL_DB"] = sqlalchemy_prefix(os.environ.get("PUDL_DB"))
+SETTINGS["PG_DB"] = sqlalchemy_prefix(os.environ.get("PG_DB"))
 SETTINGS["EFS_DATA"] = os.environ.get("EFS_DATA")
 SETTINGS["RESOURCE_GROUPS"] = os.environ.get("RESOURCE_GROUPS")
 SETTINGS["DISTRIBUTED_GEN_DATA"] = os.environ.get("DISTRIBUTED_GEN_DATA")
+SETTINGS["RESOURCE_GROUP_PROFILES"] = os.environ.get("RESOURCE_GROUP_PROFILES")
 
 
 def build_resource_clusters(group_path: Union[str, Path] = None):
     if not group_path:
         group_path = SETTINGS.get("RESOURCE_GROUPS")
     if not group_path:
         cluster_builder = ClusterBuilder([])
```

### Comparing `powergenome-0.6.0a0/powergenome/price_adjustment.py` & `PowerGenome-0.6.1a0/powergenome/price_adjustment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 Adjust price/cost from one year to another
 """
 
-from functools import lru_cache
-import logging
-
-import requests
 import json
-from typing import NamedTuple, Union
+import logging
 from datetime import date
-import pandas as pd
-import numpy as np
+from functools import lru_cache
 from pathlib import Path
+from typing import NamedTuple, Union
+
+import numpy as np
+import pandas as pd
+import requests
+
 from powergenome.params import DATA_PATHS
 
 
 class MonthlyCPI(NamedTuple):
     year: int
     period: int
     value: float
```

### Comparing `powergenome-0.6.0a0/powergenome/resource_clusters.py` & `PowerGenome-0.6.1a0/powergenome/resource_clusters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 import glob
 import json
 import os
 import re
-from typing import Any, Callable, Dict, Iterable, List, Mapping, Optional, Union
 from pathlib import Path
+from typing import Any, Callable, Dict, Iterable, List, Mapping, Optional, Union
 
 import numpy as np
 import pandas as pd
 import pyarrow
 import pyarrow.parquet as pq
 import scipy.cluster.hierarchy
 
@@ -435,19 +435,34 @@
     def __init__(
         self,
         group: Dict[str, Any],
         metadata: pd.DataFrame = None,
         profiles: pd.DataFrame = None,
         path: str = ".",
     ) -> None:
+        from powergenome.params import SETTINGS
+
         self.group = {"existing": False, "tree": None, **group.copy()}
-        for key in ["metadata", "profiles"]:
-            if self.group.get(key):
-                # Convert relative paths (relative to group file) to absolute paths
-                self.group[key] = Path(path) / self.group[key]
+
+        # Convert relative paths (relative to group file) to absolute paths
+        # Profiles may be stored in a single location and reused across resource groups
+        if self.group.get("metadata"):
+            self.group["metadata"] = Path(path) / self.group["metadata"]
+        if self.group.get("profiles"):
+            if (
+                SETTINGS.get("RESOURCE_GROUP_PROFILES")
+                and (
+                    Path(SETTINGS["RESOURCE_GROUP_PROFILES"]) / self.group["profiles"]
+                ).exists()
+            ):
+                self.group["profiles"] = (
+                    Path(SETTINGS["RESOURCE_GROUP_PROFILES"]) / self.group["profiles"]
+                )
+            else:
+                self.group["profiles"] = Path(path) / self.group["profiles"]
         required = ["technology"]
         if metadata is None:
             required.append("metadata")
         missing = [key for key in required if not self.group.get(key)]
         if missing:
             raise ValueError(
                 f"Group metadata missing required keys {missing}: {self.group}"
```

### Comparing `powergenome-0.6.0a0/powergenome/run_powergenome_multiple_outputs_cli.py` & `PowerGenome-0.6.1a0/powergenome/run_powergenome_multiple_outputs_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,62 +5,62 @@
 import sys
 from datetime import datetime as dt
 from pathlib import Path
 
 import pandas as pd
 
 import powergenome
+from powergenome.external_data import (
+    insert_user_tx_costs,
+    load_user_tx_costs,
+    make_generator_variability,
+)
 from powergenome.fuels import fuel_cost_table
 from powergenome.generators import (
     GeneratorClusters,
     add_fuel_labels,
     add_genx_model_tags,
 )
 from powergenome.GenX import (
     add_cap_res_network,
     add_co2_costs_to_o_m,
+    add_misc_gen_values,
+    calculate_partial_CES_values,
     check_resource_tags,
     create_policy_req,
     create_regional_cap_res,
     fix_min_power_values,
     hydro_energy_to_power,
-    min_cap_req,
     max_cap_req,
-    reduce_time_domain,
-    add_misc_gen_values,
+    min_cap_req,
     network_line_loss,
     network_max_reinforcement,
     network_reinforcement_cost,
+    reduce_time_domain,
     round_col_values,
     set_int_cols,
-    calculate_partial_CES_values,
     set_must_run_generation,
 )
 from powergenome.load_profiles import make_final_load_curves
+from powergenome.nrelatb import atb_fixed_var_om_existing
 from powergenome.transmission import (
     agg_transmission_constraints,
     transmission_line_distance,
 )
-from powergenome.nrelatb import atb_fixed_var_om_existing
-from powergenome.external_data import (
-    insert_user_tx_costs,
-    load_user_tx_costs,
-    make_generator_variability,
-)
 from powergenome.util import (
     build_scenario_settings,
     check_settings,
     init_pudl_connection,
+    load_ipm_shapefile,
     load_settings,
-    remove_fuel_scenario_name,
     remove_fuel_gen_scenario_name,
+    remove_fuel_scenario_name,
     update_dictionary,
     write_case_settings_file,
     write_results_file,
-    load_ipm_shapefile,
 )
 
 if not sys.warnoptions:
     import warnings
 
     warnings.simplefilter("ignore")
 
@@ -172,16 +172,18 @@
             args.settings_file, out_folder / "pg_settings", dirs_exist_ok=True
         )
 
     logger.info("Initiating PUDL connections")
 
     pudl_engine, pudl_out, pg_engine = init_pudl_connection(
         freq="AS",
-        start_year=min(settings.get("data_years")),
-        end_year=max(settings.get("data_years")),
+        start_year=min(settings.get("eia_data_years")),
+        end_year=max(settings.get("eia_data_years")),
+        pudl_db=settings.get("PUDL_DB"),
+        pg_db=settings.get("PG_DB"),
     )
 
     check_settings(settings, pg_engine)
 
     # Make sure everything in model_regions is either an aggregate region
     # or an IPM region. Will need to change this once we start using non-IPM
     # regions.
```

### Comparing `powergenome-0.6.0a0/powergenome/time_reduction.py` & `PowerGenome-0.6.1a0/powergenome/time_reduction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 "Functions to cluster or otherwise reduce the number of hours in generation and load profiles"
 
-from sklearn.cluster import KMeans
-from sklearn.preprocessing import minmax_scale
-import numpy as np
 import datetime
+
+import numpy as np
 import pandas as pd
+from sklearn.cluster import KMeans
+from sklearn.preprocessing import minmax_scale
 
 
 def kmeans_time_clustering(
     resource_profiles,
     load_profiles,
     days_in_group,
     num_clusters,
```

### Comparing `powergenome-0.6.0a0/powergenome/transmission.py` & `PowerGenome-0.6.1a0/powergenome/transmission.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 from math import asin, cos, radians, sin, sqrt
 from pathlib import Path
 
 import pandas as pd
 import sqlalchemy as sa
 
-from powergenome.util import map_agg_region_names, reverse_dict_of_lists, find_centroid
+from powergenome.util import find_centroid, map_agg_region_names, reverse_dict_of_lists
 
 logger = logging.getLogger(__name__)
 
 
 def agg_transmission_constraints(
     pg_engine: sa.engine.base.Engine,
     settings: dict,
```

### Comparing `powergenome-0.6.0a0/powergenome/util.py` & `PowerGenome-0.6.1a0/powergenome/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 import collections
-from copy import deepcopy
-import functools
 import itertools
 import logging
+import os
 import re
 import subprocess
-from typing import Dict, List, Tuple, Union
 from collections.abc import Iterable
+from copy import deepcopy
+from pathlib import Path
+from typing import Dict, List, Tuple, Union
 
-import pandas as pd
 import geopandas as gpd
+import pandas as pd
 import pudl
 import requests
 import sqlalchemy as sa
-
-from flatten_dict import flatten
 import yaml
+from flatten_dict import flatten
 from ruamel.yaml import YAML
-from pathlib import Path
-from frozendict import frozendict
-
-from powergenome.params import IPM_GEOJSON_PATH, SETTINGS
 
 logger = logging.getLogger(__name__)
 
 
 def load_settings(path: Union[str, Path]) -> dict:
     """Load a YAML file or a dictionary of YAML files with settings parameters
 
@@ -58,17 +54,49 @@
         )
 
     if settings.get("input_folder"):
         settings["input_folder"] = path.parent / settings["input_folder"]
 
     settings = apply_all_tag_to_regions(settings)
 
+    for key in ["PUDL_DB", "PG_DB"]:
+        # Add correct connection string prefix if it isn't there
+        if settings.get(key):
+            settings[key] = sqlalchemy_prefix(settings[key])
+
     return fix_param_names(settings)
 
 
+def sqlalchemy_prefix(db_path: str) -> str:
+    """Check the database path and add sqlite prefix if needed
+
+    Parameters
+    ----------
+    db_path : str
+        Path to the sqlite database. May or may not include sqlite://// (OS specific)
+
+    Returns
+    -------
+    str
+        SqlAlchemy connection string
+    """
+    if os.name == "nt":
+        # if user is using a windows system
+        sql_prefix = "sqlite:///"
+    else:
+        sql_prefix = "sqlite:////"
+
+    if not db_path:
+        return None
+    if sql_prefix in db_path:
+        return db_path
+    else:
+        return sql_prefix + str(Path(db_path))
+
+
 def apply_all_tag_to_regions(settings: dict) -> dict:
     """Make copies of renewables_clusters dicts with region "all"
 
     If a renewables clustering object doesn't already existing for a region/technology
     then make a copy for use. This is helpful with large numbers of regions when
     the clustering parameters can be applied everywhere.
 
@@ -159,14 +187,15 @@
     return settings
 
 
 def fix_param_names(settings: dict) -> dict:
     fix_params = {
         "historical_load_region_maps": "historical_load_region_map",
         "demand_response_resources": "flexible_demand_resources",
+        "data_years": "eia_data_years",
     }
     for k, v in fix_params.items():
         if k in settings:
             settings[v] = settings[k]
             s = f"""
             The settings parameter named {k} has been changed to {v}. Please correct it in
             your settings file.
@@ -420,14 +449,16 @@
     Returns
     -------
     sa.Engine, pudl.pudltabl
         A sqlalchemy engine for connecting to the PUDL database, and a pudl PudlTabl
         object for quickly accessing parts of the database. `pudl_out` is used
         to access unit heat rates.
     """
+    from powergenome.params import SETTINGS
+
     if not pudl_db:
         pudl_db = SETTINGS["PUDL_DB"]
     if not pg_db:
         if SETTINGS.get("PG_DB"):
             pg_db = SETTINGS["PG_DB"]
         else:
             logger.warning(
@@ -914,15 +945,15 @@
     df = df.loc[~((df.datetime.dt.month == 2) & (df.datetime.dt.day == 29)), :]
     df.index = range(idx_start, idx_start + 8760)
     df.index.name = idx_name
 
     return df.drop(columns=["datetime"])
 
 
-def load_ipm_shapefile(settings: dict, path: Union[str, Path] = IPM_GEOJSON_PATH):
+def load_ipm_shapefile(settings: dict, path: Union[str, Path] = None):
     """
     Load the shapefile of IPM regions
 
     Parameters
     ----------
     settings : dict
         User-defined parameters from a settings YAML file. This is where any region
@@ -932,19 +963,25 @@
         a simplified geojson stored in the PowerGenome data folder.
 
     Returns
     -------
     geodataframe
         Regions to use in the study with the matching geometry for each.
     """
+    if not path:
+        from powergenome.params import IPM_GEOJSON_PATH
+
+        path = IPM_GEOJSON_PATH
     keep_regions, region_agg_map = regions_to_keep(
         settings["model_regions"], settings.get("region_aggregations", {}) or {}
     )
-
-    ipm_regions = gpd.read_file(path)
+    try:
+        ipm_regions = gpd.read_file(path, engine="pyogrio")
+    except ImportError:
+        ipm_regions = gpd.read_file(path, engine="fiona")
     ipm_regions = ipm_regions.rename(columns={"IPM_Region": "region"})
 
     if settings.get("user_region_geodata_fn"):
         logger.info("Appending user regions to IPM Regions")
         user_regions = gpd.read_file(
             Path(settings["input_folder"]) / settings["user_region_geodata_fn"]
         )
@@ -965,15 +1002,16 @@
     return model_regions_gdf
 
 
 def deep_freeze(thing):
     """
     https://stackoverflow.com/a/66729248/3393071
     """
-    from collections.abc import Collection, Mapping, Hashable
+    from collections.abc import Collection, Hashable, Mapping
+
     from frozendict import frozendict
 
     if thing is None or isinstance(thing, str):
         return thing
     elif isinstance(thing, Mapping):
         return frozendict({k: deep_freeze(v) for k, v in thing.items()})
     elif isinstance(thing, Collection):
```

