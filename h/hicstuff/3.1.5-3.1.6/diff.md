# Comparing `tmp/hicstuff-3.1.5.tar.gz` & `tmp/hicstuff-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hicstuff-3.1.5.tar", last modified: Thu Oct  6 09:47:08 2022, max compression
+gzip compressed data, was "hicstuff-3.1.6.tar", last modified: Thu Jun  8 06:34:54 2023, max compression
```

## Comparing `hicstuff-3.1.5.tar` & `hicstuff-3.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:47:08.964179 hicstuff-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-10-06 09:46:55.000000 hicstuff-3.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-06 09:46:55.000000 hicstuff-3.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    22491 2022-10-06 09:47:08.968180 hicstuff-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18294 2022-10-06 09:46:55.000000 hicstuff-3.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:47:08.964179 hicstuff-3.1.5/hicstuff/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-10-06 09:46:56.000000 hicstuff-3.1.5/hicstuff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    76486 2022-10-06 09:46:56.000000 hicstuff-3.1.5/hicstuff/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)    12787 2022-10-06 09:46:56.000000 hicstuff-3.1.5/hicstuff/cutsite.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17126 2022-10-06 09:46:56.000000 hicstuff-3.1.5/hicstuff/digest.py
--rw-r--r--   0 runner    (1001) docker     (121)    32461 2022-10-06 09:46:56.000000 hicstuff-3.1.5/hicstuff/distance_law.py
--rw-r--r--   0 runner    (1001) docker     (121)    18713 2022-10-06 09:46:56.000000 hicstuff-3.1.5/hicstuff/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    67774 2022-10-06 09:46:56.000000 hicstuff-3.1.5/hicstuff/hicstuff.py
--rw-r--r--   0 runner    (1001) docker     (121)    45144 2022-10-06 09:46:56.000000 hicstuff-3.1.5/hicstuff/io.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10962 2022-10-06 09:46:56.000000 hicstuff-3.1.5/hicstuff/iteralign.py
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-10-06 09:46:56.000000 hicstuff-3.1.5/hicstuff/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-10-06 09:46:56.000000 hicstuff-3.1.5/hicstuff/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    36555 2022-10-06 09:46:56.000000 hicstuff-3.1.5/hicstuff/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-06 09:47:08.000000 hicstuff-3.1.5/hicstuff/version.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5542 2022-10-06 09:46:56.000000 hicstuff-3.1.5/hicstuff/view.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:47:08.964179 hicstuff-3.1.5/hicstuff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22491 2022-10-06 09:47:08.000000 hicstuff-3.1.5/hicstuff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-10-06 09:47:08.000000 hicstuff-3.1.5/hicstuff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-06 09:47:08.000000 hicstuff-3.1.5/hicstuff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-06 09:47:08.000000 hicstuff-3.1.5/hicstuff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-10-06 09:47:08.000000 hicstuff-3.1.5/hicstuff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-06 09:47:08.000000 hicstuff-3.1.5/hicstuff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-06 09:46:56.000000 hicstuff-3.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-10-06 09:47:08.968180 hicstuff-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1981 2022-10-06 09:46:56.000000 hicstuff-3.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:34:54.491829 hicstuff-3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-08 06:34:42.000000 hicstuff-3.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-08 06:34:42.000000 hicstuff-3.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-06-08 06:34:54.491829 hicstuff-3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-06-08 06:34:42.000000 hicstuff-3.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:34:54.491829 hicstuff-3.1.6/hicstuff/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-08 06:34:42.000000 hicstuff-3.1.6/hicstuff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76487 2023-06-08 06:34:42.000000 hicstuff-3.1.6/hicstuff/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-06-08 06:34:42.000000 hicstuff-3.1.6/hicstuff/cutsite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17126 2023-06-08 06:34:42.000000 hicstuff-3.1.6/hicstuff/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32461 2023-06-08 06:34:42.000000 hicstuff-3.1.6/hicstuff/distance_law.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-06-08 06:34:42.000000 hicstuff-3.1.6/hicstuff/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    67774 2023-06-08 06:34:42.000000 hicstuff-3.1.6/hicstuff/hicstuff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45144 2023-06-08 06:34:42.000000 hicstuff-3.1.6/hicstuff/io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11000 2023-06-08 06:34:42.000000 hicstuff-3.1.6/hicstuff/iteralign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-08 06:34:42.000000 hicstuff-3.1.6/hicstuff/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-08 06:34:42.000000 hicstuff-3.1.6/hicstuff/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36555 2023-06-08 06:34:42.000000 hicstuff-3.1.6/hicstuff/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 06:34:54.000000 hicstuff-3.1.6/hicstuff/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5542 2023-06-08 06:34:42.000000 hicstuff-3.1.6/hicstuff/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:34:54.491829 hicstuff-3.1.6/hicstuff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-06-08 06:34:54.000000 hicstuff-3.1.6/hicstuff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-08 06:34:54.000000 hicstuff-3.1.6/hicstuff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 06:34:54.000000 hicstuff-3.1.6/hicstuff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 06:34:54.000000 hicstuff-3.1.6/hicstuff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-08 06:34:54.000000 hicstuff-3.1.6/hicstuff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 06:34:54.000000 hicstuff-3.1.6/hicstuff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 06:34:42.000000 hicstuff-3.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 06:34:54.491829 hicstuff-3.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-08 06:34:42.000000 hicstuff-3.1.6/setup.py
```

### Comparing `hicstuff-3.1.5/LICENSE` & `hicstuff-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hicstuff-3.1.5/PKG-INFO` & `hicstuff-3.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,72 +1,84 @@
 Metadata-Version: 2.1
 Name: hicstuff
-Version: 3.1.5
+Version: 3.1.6
 Summary: General purpose stuff to generate and handle Hi-C data in its simplest form.
 Home-page: https://github.com/koszullab/hicstuff
 Author: cyril.matthey-doret@pasteur.fr
 License: BSD-3-Clause
 Description: # hicstuff
         
         [![PyPI version](https://badge.fury.io/py/hicstuff.svg)](https://badge.fury.io/py/hicstuff)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hicstuff.svg)
+        [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/hicstuff/README.html)
         [![Build Status](https://github.com/koszullab/hicstuff/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/koszullab/hicstuff/actions/workflows/build.yml)
-        [![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/koszullab/hicstuff)](https://hub.docker.com/r/koszullab/hicstuff)
         [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2620608.svg)](https://doi.org/10.5281/zenodo.2620608)
         [![codecov](https://codecov.io/gh/koszullab/hicstuff/branch/master/graph/badge.svg)](https://codecov.io/gh/koszullab/hicstuff)
         [![Read the docs](https://readthedocs.org/projects/hicstuff/badge)](https://hicstuff.readthedocs.io)
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/koszullab/hicstuff/master?filepath=doc%2Fnotebooks%2Fdemo_api.ipynb)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
         
         A lightweight library that generates and handles Hi-C contact maps in either cooler-compatible 2Dbedgraph or [instaGRAAL](https://github.com/koszullab/instaGRAAL) format. It is essentially a merge of the [yahcp](https://github.com/baudrly/yahcp) pipeline, the [hicstuff](https://github.com/baudrly/hicstuff) library and extra features illustrated in the [3C tutorial](https://github.com/axelcournac/3C_tutorial) and the [DADE pipeline](https://github.com/scovit/dade), all packaged together for extra convenience.
         
         The goal is to make generation and manipulation of Hi-C matrices as simple as possible and work for any organism.
         
         ## Table of contents
         
-        * [Installation](#Installation)
-        * [Usage](#Usage)
-          * [Full pipeline](#Full-pipeline)
-          * [Individual components](#Individual-components)
-        * [Library](#Library)
-        * [Connecting the modules](#Connecting-the-modules)
-        * [File formats](#File-formats)
-        * [Contributing](#Contributing)
+        * [Installation](#installation)
+          * [pip](#pip)
+          * [conda](#conda)
+          * [docker](#docker)
+        * [Usage](#usage)
+          * [Full pipeline](#full-pipeline)
+          * [Individual components](#individual-components)
+        * [Library](#library)
+        * [Connecting the modules](#connecting-the-modules)
+        * [File formats](#file-formats)
+        * [Contributing](#contributing)
         
         ## Installation
         
+        ### pip
+        
         To install a stable version:
         ```sh
         pip3 install -U hicstuff
         ```
         
         or, for the latest development version:
         
         ```sh
             pip3 install -e git+https://github.com/koszullab/hicstuff.git@master#egg=hicstuff
         ```
         
-        ### External dependencies
-        
-        Bowtie2 and/or minimap2 as well as samtools are required for the `pipeline` utility.
+        `bowtie2`, `bwa` and/or `minimap2` as well as `samtools` are required by the `pipeline` command.
         
         You can install them via the conda package manager:
         ```bash
-        conda install -c bioconda minimap2 bowtie2 samtools
+        conda install -c bioconda bowtie2 bwa minimap2 samtools
         ```
         Alternatively, on ubuntu you can also install them along with additional dependencies through APT:
         ```bash
-        apt-get install samtools bowtie2 minimap2 libbz2-dev liblzma-dev
+        apt-get install bowtie2 bwa minimap2 samtools libbz2-dev liblzma-dev
         ```
         
-        ### Docker installation
+        ### Conda
+        
+        hicstuff is available as a bioconda package. It can be installed, along with all dependencies using:
         
-        A pre-built docker image is available on dockerhub and can be ran using:
         ```bash
-        docker run koszullab/hicstuff
+        conda install -c bioconda hicstuff
+        ```
+        
+        ### Docker
+        
+        A pre-built docker image is made available on quay.io via [biocontainers](https://biocontainers.pro/) and can be ran using:
+        
+        ```bash
+        docker pull quay.io/biocontainers/hicstuff:<tag>
         ```
         
         ## Usage
         
         The hicstuff command line interface is composed of multiple subcommands. You can always get a summary of all available commands by running:
         
         ```bash
@@ -78,34 +90,37 @@
             hicstuff [-hv] <command> [<args>...]
         
         options:
             -h, --help                  shows the help
             -v, --version               shows the version
         
         The subcommands are:
+            convert         Convert Hi-C data between different formats.
             digest          Digest genome into a list of fragments.
+            cutsite         Preprocess fastq files by digesting reads at religation site.
             distancelaw     Analyse and plot distance law.
             filter          Filters Hi-C pairs to exclude spurious events.
             iteralign       Iteratively aligns reads to a reference genome.
+            missview        Preview missing Hi-C bins in based on the genome and read length.
             pipeline        Hi-C pipeline to generate contact matrix from fastq files.
             rebin           Bin the matrix and regenerate files accordingly.
             subsample       Bootstrap subsampling of contacts from a Hi-C map.
-            view            Visualize a Hi-C matrix.  
+            view            Visualize a Hi-C matrix.
         ```
         
         ### Full pipeline
         
         All components of the pipeline can be run at once using the `hicstuff pipeline` command. This allows to generate a contact matrix from reads in a single command. By default, the output is in GRAAL compatible COO sparse matrix format, but it can be a 2D bedgraph or cool file instead using the `--matfmt` option. More detailed documentation can be found on the readthedocs website: https://hicstuff.readthedocs.io/en/latest/index.html
         
             usage:
-                pipeline [--quality-min=INT] [--size=INT] [--no-cleanup] [--start-stage=STAGE]
-                         [--threads=INT] [--aligner=bowtie2] [--matfmt=FMT] [--prefix=PREFIX]
-                         [--tmpdir=DIR] [--iterative] [--outdir=DIR] [--filter] [--enzyme=ENZ]
-                         [--plot] [--circular] [--distance-law] [--duplicates] [--read-len=INT]
-                         [--centromeres=FILE] [--remove-centromeres=INT] --genome=FILE <input1> [<input2>]
+                pipeline [--aligner=bowtie2] [--centromeres=FILE] [--circular] [--distance-law]
+                         [--duplicates] [--enzyme=5000] [--filter] [--force] [--mapping=normal]
+                         [--matfmt=graal] [--no-cleanup] [--outdir=DIR] [--plot] [--prefix=PREFIX]
+                         [--quality-min=30] [--read-len=INT] [--remove-centromeres=0] [--size=0]
+                         [--start-stage=fastq] [--threads=1] [--tmpdir=DIR] --genome=FILE <input1> [<input2>]
         
             arguments:
                 input1:             Forward fastq file, if start_stage is "fastq", sam
                                     file for aligned forward reads if start_stage is
                                     "bam", or a .pairs file if start_stage is "pairs".
                 input2:             Reverse fastq file, if start_stage is "fastq", sam
                                     file for aligned reverse reads if start_stage is
@@ -124,76 +139,86 @@
         # Note the bam files have to be name-sorted, this can be done using samtools
         samtools sort -n aligned_for.bam -o namesorted_for.bam
         samtools sort -n aligned_rev.bam -o namesorted_rev.bam
         hicstuff pipeline -S bam -e 5000 -M cool -o out/ -g genome.fa namesorted_for.bam namesorted_rev.bam
         ```
         
         
-        The pipeline can also be run from python, using the `hicstuff.pipeline` submodule. For example, this would run the pipeline with bowtie2 (default) using iterative alignment and keep all intermediate files. For more examples using the API, see the [API demo](https://hicstuff.readthedocs.io/en/latest/notebooks/demo_api.html)
+        The pipeline can also be run from python, using the `hicstuff.pipeline` submodule. For example, this would run the pipeline with bowtie2 (default) using cutsiste alignment and keep all intermediate files. For more examples using the API, see the [API demo](https://hicstuff.readthedocs.io/en/latest/notebooks/demo_api.html)
         
         ```python
         from hicstuff import pipeline as hpi
         
         hpi.full_pipeline(
             'genome.fa', 
             'end1.fq', 
             'end2.fq', 
             no_cleanup=True
-            iterative=True
+            mapping='cutsite',
             out_dir='out', 
             enzyme="DpnII")
         ```
         
         The general steps of the pipeline are as follows:
         
         ![Pipeline flowchart](doc/images/pipeline.svg)
         
         ### Individual components
         
         For more advanced usage, different scripts can be used independently on the command line to perform individual parts of the pipeline. This readme contains quick descriptions and example usages. To obtain detailed instructions on any subcommand, one can use `hicstuff <subcommand> --help`.
         
+        ### Digestion of the reads
+         
+        Generates new gzipped fastq files from original fastq. The function will cut the reads at their religation sites and creates new pairs of reads with the different fragments obtained after cutting at the digestion sites.
+        
+            usage:
+                cutsite --forward=FILE --reverse=FILE  --prefix=STR --enzyme=STR
+                [--mode=for_vs_rev] [--seed-size=20] [--threads=1]
+        
         #### Iterative alignment
         
         Truncate reads from a fastq file to 20 basepairs and iteratively extend and re-align the unmapped reads to optimize the proportion of uniquely aligned reads in a 3C library.
         
             usage:
-                iteralign [--aligner=bowtie2] [--threads=1] [--min_len=20]
-                          [--tempdir DIR] --out_sam=FILE --genome=FILE <reads.fq>
+                iteralign [--aligner=bowtie2] [--threads=1] [--min-len=20] [--read-len=INT]
+                          [--tempdir=DIR] --out-bam=FILE --genome=FILE <reads.fq>
         
         #### Digestion of the genome
         
         Digests a fasta file into fragments based on a restriction enzyme or a
         fixed chunk size. Generates two output files into the target directory
         named "info_contigs.txt" and "fragments_list.txt"
         
             usage:
-                digest [--plot] [--figdir=FILE] [--circular] [--size=INT]
+                digest [--plot] [--figdir=FILE] [--force] [--circular] [--size=0]
                        [--outdir=DIR] --enzyme=ENZ <fasta>
         
          
          For example, to digest the yeast genome with MaeII and HinfI and show histogram of fragment lengths:
         
         `hicstuff digest --plot --outdir output_dir --enzyme MaeII,HinfI Sc_ref.fa`
         
         #### Filtering of 3C events
         
         Filters spurious 3C events such as loops and uncuts from the library based on a minimum distance threshold automatically estimated from the library by default. Can also plot 3C library statistics. This module takes a pairs file with 9 columns as input (readID, chr1, pos1, chr2, pos2, strand1, strand2, frag1, frag2) and filters it. 
         
             usage:
                 filter [--interactive | --thresholds INT-INT] [--plot]
-                       [--figdir FILE] <input.pairs> <output.pairs>
+                       [--figdir FILE] [--prefix STR] <input> <output>
         
         #### Viewing the contact map
         
-        Visualize a Hi-C matrix file as a heatmap of contact frequencies. Allows to tune visualisation by binning and normalizing the matrix, and to save the output image to disk. If no output is specified, the output is displayed interactively. If two contact maps are provided, the log ratio of the first divided by the second will be shown.
+        Visualize a Hi-C matrix file as a heatmap of contact frequencies. Allows to
+        tune visualisation by binning and normalizing the matrix, and to save the
+        output image to disk. If no output is specified, the output is displayed.
         
             usage:
-                view [--binning=1] [--despeckle] [--frags FILE] [--trim INT] [--n-mad FLOAT]
-                     [--normalize] [--max=99] [--output=IMG] [--cmap=CMAP] [--dpi=INT]
-                     [--transform=FUN] [--circular] [--region=STR] <contact_map> [<contact_map2>]
+                view [--binning=1] [--despeckle] [--frags FILE] [--trim INT] [--n-mad 3.0] [--lines]
+                     [--normalize] [--min=0] [--max=99%] [--output=IMG] [--cmap=Reds] [--dpi=300]
+                     [--transform=STR] [--circular] [--region=STR] <contact_map> [<contact_map2>]
         
             arguments:
                 contact_map             Sparse contact matrix in bg2, cool or graal format
                 contact_map2            Sparse contact matrix in bg2, cool or graal format,
                                         if given, the log ratio of contact_map/contact_map2
                                         will be shown.
         
@@ -203,14 +228,15 @@
             hicstuff view --normalize --binning 10kb --region chr1:10,000,000-11,000,000 --frags fragments_list.txt contact_map.tsv
         ```
         ### Library
         
         All components of the hicstuff program can be used as python modules. See the documentation on [reathedocs](https://hicstuff.readthedocs.io). The expected contact map format for the library is a simple CSV file, and the objects handled by the library are simple ```numpy``` arrays. The various submodules of hicstuff contain various utilities.
         
         ```python
+        import hicstuff.cutsite # Functions to digest fastq librairies
         import hicstuff.digest # Functions to work with restriction fragments
         import hicstuff.iteralign # Functions related to iterative alignment
         import hicstuff.hicstuff # Contains utilities to modify and operate on contact maps as numpy arrays
         import hicstuff.filter # Functions for filtering 3C events by type (uncut, loop)
         import hicstuff.view # Utilities to visualise contact maps
         import hicstuff.io # Reading and writing hicstuff files
         import hicstuff.pipeline # Generation and processing of files to generate matrices.
@@ -218,41 +244,40 @@
         
         ### Connecting the modules
         
         All the steps described here are handled automatically when running the `hicstuff pipeline`. But if you want to connect the different modules manually, the intermediate input and output files can be processed using some python scripting.
         
         #### Aligning the reads
         
-        You can generate SAM files independently using your favorite read mapping software, use the command line utility `hicstuff iteralign`, or use the helper function `align_reads` in the submodule `hicstuff.pipeline`. For example, to perform iterative alignment using minimap2 (instead of bowtie2 by default):
+        You can generate SAM files independently using your favorite read mapping software, use the command line utility `hicstuff iteralign`, or use the helper function `align_reads` in the submodule `hicstuff.pipeline`. For example, to perform iterative alignment using bwa (instead of bowtie2 by default):
         
         **Using the python function:**
         
         ```python
         from hicstuff import pipeline as hpi
         
-        hpi.align_reads("end1.fastq", "genome.fasta", "end1.bam", iterative=True, minimap2=True)
+        hpi.align_reads("end1.fastq", "genome.fasta", "end1.bam", iterative=True, aligner='bwa')
         ```
         
         **Using the command line tool:**
         
         ```bash
-        hicstuff iteralign --minimap2 --iterative -f genome.fasta -o end1.sam end1.fastq
+        hicstuff iteralign --aligner bwa --genome genome.fasta --out-bam end1.bam end1.fastq
         ```
         
-        
         #### Extracting contacts from the alignment
         
-        The output from `hicstuff iteralign` is a SAM file. In order to retrieve Hi-C pairs, you need to run iteralign separately on the two fastq files and process the resulting alignment files into a name-sorted BAM file as follows using the `pipeline` submodules of hicstuff.
+        The output from `hicstuff iteralign` is a BAM file. In order to retrieve Hi-C pairs, you need to run iteralign separately on the two fastq files and process the resulting alignment files into a name-sorted BAM file as follows using the `pipeline` submodules of hicstuff.
         
         ```python
         from hicstuff import pipeline as hpi
         import pysam as ps
         # Sort alignments by read names and get into BAM format
-        ps.sort("-n", "-O", "BAM", "-o", "end1.bam.sorted", "end1.sam")
-        ps.sort("-n", "-O", "BAM", "-o", "end2.bam.sorted", "end2.sam")
+        ps.sort("-n", "-O", "BAM", "-o", "end1.bam.sorted", "end1.bam")
+        ps.sort("-n", "-O", "BAM", "-o", "end2.bam.sorted", "end2.bam")
         # Combine BAM files
         hpi.bam2pairs("end1.sorted.bam", "end2.sorted.bam", "output.pairs", "info_contigs.txt", min_qual=30)
         
         ```
         This will generate a "pairs" file containing all read pairs where both reads have been aligned with a mapping quality of at least 30.
         
         #### Attributing each read to a restriction fragment
```

### Comparing `hicstuff-3.1.5/README.md` & `hicstuff-3.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,65 +1,77 @@
 # hicstuff
 
 [![PyPI version](https://badge.fury.io/py/hicstuff.svg)](https://badge.fury.io/py/hicstuff)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hicstuff.svg)
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/hicstuff/README.html)
 [![Build Status](https://github.com/koszullab/hicstuff/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/koszullab/hicstuff/actions/workflows/build.yml)
-[![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/koszullab/hicstuff)](https://hub.docker.com/r/koszullab/hicstuff)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2620608.svg)](https://doi.org/10.5281/zenodo.2620608)
 [![codecov](https://codecov.io/gh/koszullab/hicstuff/branch/master/graph/badge.svg)](https://codecov.io/gh/koszullab/hicstuff)
 [![Read the docs](https://readthedocs.org/projects/hicstuff/badge)](https://hicstuff.readthedocs.io)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/koszullab/hicstuff/master?filepath=doc%2Fnotebooks%2Fdemo_api.ipynb)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 A lightweight library that generates and handles Hi-C contact maps in either cooler-compatible 2Dbedgraph or [instaGRAAL](https://github.com/koszullab/instaGRAAL) format. It is essentially a merge of the [yahcp](https://github.com/baudrly/yahcp) pipeline, the [hicstuff](https://github.com/baudrly/hicstuff) library and extra features illustrated in the [3C tutorial](https://github.com/axelcournac/3C_tutorial) and the [DADE pipeline](https://github.com/scovit/dade), all packaged together for extra convenience.
 
 The goal is to make generation and manipulation of Hi-C matrices as simple as possible and work for any organism.
 
 ## Table of contents
 
-* [Installation](#Installation)
-* [Usage](#Usage)
-  * [Full pipeline](#Full-pipeline)
-  * [Individual components](#Individual-components)
-* [Library](#Library)
-* [Connecting the modules](#Connecting-the-modules)
-* [File formats](#File-formats)
-* [Contributing](#Contributing)
+* [Installation](#installation)
+  * [pip](#pip)
+  * [conda](#conda)
+  * [docker](#docker)
+* [Usage](#usage)
+  * [Full pipeline](#full-pipeline)
+  * [Individual components](#individual-components)
+* [Library](#library)
+* [Connecting the modules](#connecting-the-modules)
+* [File formats](#file-formats)
+* [Contributing](#contributing)
 
 ## Installation
 
+### pip
+
 To install a stable version:
 ```sh
 pip3 install -U hicstuff
 ```
 
 or, for the latest development version:
 
 ```sh
     pip3 install -e git+https://github.com/koszullab/hicstuff.git@master#egg=hicstuff
 ```
 
-### External dependencies
-
-Bowtie2 and/or minimap2 as well as samtools are required for the `pipeline` utility.
+`bowtie2`, `bwa` and/or `minimap2` as well as `samtools` are required by the `pipeline` command.
 
 You can install them via the conda package manager:
 ```bash
-conda install -c bioconda minimap2 bowtie2 samtools
+conda install -c bioconda bowtie2 bwa minimap2 samtools
 ```
 Alternatively, on ubuntu you can also install them along with additional dependencies through APT:
 ```bash
-apt-get install samtools bowtie2 minimap2 libbz2-dev liblzma-dev
+apt-get install bowtie2 bwa minimap2 samtools libbz2-dev liblzma-dev
 ```
 
-### Docker installation
+### Conda
+
+hicstuff is available as a bioconda package. It can be installed, along with all dependencies using:
 
-A pre-built docker image is available on dockerhub and can be ran using:
 ```bash
-docker run koszullab/hicstuff
+conda install -c bioconda hicstuff
+```
+
+### Docker
+
+A pre-built docker image is made available on quay.io via [biocontainers](https://biocontainers.pro/) and can be ran using:
+
+```bash
+docker pull quay.io/biocontainers/hicstuff:<tag>
 ```
 
 ## Usage
 
 The hicstuff command line interface is composed of multiple subcommands. You can always get a summary of all available commands by running:
 
 ```bash
@@ -71,34 +83,37 @@
     hicstuff [-hv] <command> [<args>...]
 
 options:
     -h, --help                  shows the help
     -v, --version               shows the version
 
 The subcommands are:
+    convert         Convert Hi-C data between different formats.
     digest          Digest genome into a list of fragments.
+    cutsite         Preprocess fastq files by digesting reads at religation site.
     distancelaw     Analyse and plot distance law.
     filter          Filters Hi-C pairs to exclude spurious events.
     iteralign       Iteratively aligns reads to a reference genome.
+    missview        Preview missing Hi-C bins in based on the genome and read length.
     pipeline        Hi-C pipeline to generate contact matrix from fastq files.
     rebin           Bin the matrix and regenerate files accordingly.
     subsample       Bootstrap subsampling of contacts from a Hi-C map.
-    view            Visualize a Hi-C matrix.  
+    view            Visualize a Hi-C matrix.
 ```
 
 ### Full pipeline
 
 All components of the pipeline can be run at once using the `hicstuff pipeline` command. This allows to generate a contact matrix from reads in a single command. By default, the output is in GRAAL compatible COO sparse matrix format, but it can be a 2D bedgraph or cool file instead using the `--matfmt` option. More detailed documentation can be found on the readthedocs website: https://hicstuff.readthedocs.io/en/latest/index.html
 
     usage:
-        pipeline [--quality-min=INT] [--size=INT] [--no-cleanup] [--start-stage=STAGE]
-                 [--threads=INT] [--aligner=bowtie2] [--matfmt=FMT] [--prefix=PREFIX]
-                 [--tmpdir=DIR] [--iterative] [--outdir=DIR] [--filter] [--enzyme=ENZ]
-                 [--plot] [--circular] [--distance-law] [--duplicates] [--read-len=INT]
-                 [--centromeres=FILE] [--remove-centromeres=INT] --genome=FILE <input1> [<input2>]
+        pipeline [--aligner=bowtie2] [--centromeres=FILE] [--circular] [--distance-law]
+                 [--duplicates] [--enzyme=5000] [--filter] [--force] [--mapping=normal]
+                 [--matfmt=graal] [--no-cleanup] [--outdir=DIR] [--plot] [--prefix=PREFIX]
+                 [--quality-min=30] [--read-len=INT] [--remove-centromeres=0] [--size=0]
+                 [--start-stage=fastq] [--threads=1] [--tmpdir=DIR] --genome=FILE <input1> [<input2>]
 
     arguments:
         input1:             Forward fastq file, if start_stage is "fastq", sam
                             file for aligned forward reads if start_stage is
                             "bam", or a .pairs file if start_stage is "pairs".
         input2:             Reverse fastq file, if start_stage is "fastq", sam
                             file for aligned reverse reads if start_stage is
@@ -117,76 +132,86 @@
 # Note the bam files have to be name-sorted, this can be done using samtools
 samtools sort -n aligned_for.bam -o namesorted_for.bam
 samtools sort -n aligned_rev.bam -o namesorted_rev.bam
 hicstuff pipeline -S bam -e 5000 -M cool -o out/ -g genome.fa namesorted_for.bam namesorted_rev.bam
 ```
 
 
-The pipeline can also be run from python, using the `hicstuff.pipeline` submodule. For example, this would run the pipeline with bowtie2 (default) using iterative alignment and keep all intermediate files. For more examples using the API, see the [API demo](https://hicstuff.readthedocs.io/en/latest/notebooks/demo_api.html)
+The pipeline can also be run from python, using the `hicstuff.pipeline` submodule. For example, this would run the pipeline with bowtie2 (default) using cutsiste alignment and keep all intermediate files. For more examples using the API, see the [API demo](https://hicstuff.readthedocs.io/en/latest/notebooks/demo_api.html)
 
 ```python
 from hicstuff import pipeline as hpi
 
 hpi.full_pipeline(
     'genome.fa', 
     'end1.fq', 
     'end2.fq', 
     no_cleanup=True
-    iterative=True
+    mapping='cutsite',
     out_dir='out', 
     enzyme="DpnII")
 ```
 
 The general steps of the pipeline are as follows:
 
 ![Pipeline flowchart](doc/images/pipeline.svg)
 
 ### Individual components
 
 For more advanced usage, different scripts can be used independently on the command line to perform individual parts of the pipeline. This readme contains quick descriptions and example usages. To obtain detailed instructions on any subcommand, one can use `hicstuff <subcommand> --help`.
 
+### Digestion of the reads
+ 
+Generates new gzipped fastq files from original fastq. The function will cut the reads at their religation sites and creates new pairs of reads with the different fragments obtained after cutting at the digestion sites.
+
+    usage:
+        cutsite --forward=FILE --reverse=FILE  --prefix=STR --enzyme=STR
+        [--mode=for_vs_rev] [--seed-size=20] [--threads=1]
+
 #### Iterative alignment
 
 Truncate reads from a fastq file to 20 basepairs and iteratively extend and re-align the unmapped reads to optimize the proportion of uniquely aligned reads in a 3C library.
 
     usage:
-        iteralign [--aligner=bowtie2] [--threads=1] [--min_len=20]
-                  [--tempdir DIR] --out_sam=FILE --genome=FILE <reads.fq>
+        iteralign [--aligner=bowtie2] [--threads=1] [--min-len=20] [--read-len=INT]
+                  [--tempdir=DIR] --out-bam=FILE --genome=FILE <reads.fq>
 
 #### Digestion of the genome
 
 Digests a fasta file into fragments based on a restriction enzyme or a
 fixed chunk size. Generates two output files into the target directory
 named "info_contigs.txt" and "fragments_list.txt"
 
     usage:
-        digest [--plot] [--figdir=FILE] [--circular] [--size=INT]
+        digest [--plot] [--figdir=FILE] [--force] [--circular] [--size=0]
                [--outdir=DIR] --enzyme=ENZ <fasta>
 
  
  For example, to digest the yeast genome with MaeII and HinfI and show histogram of fragment lengths:
 
 `hicstuff digest --plot --outdir output_dir --enzyme MaeII,HinfI Sc_ref.fa`
 
 #### Filtering of 3C events
 
 Filters spurious 3C events such as loops and uncuts from the library based on a minimum distance threshold automatically estimated from the library by default. Can also plot 3C library statistics. This module takes a pairs file with 9 columns as input (readID, chr1, pos1, chr2, pos2, strand1, strand2, frag1, frag2) and filters it. 
 
     usage:
         filter [--interactive | --thresholds INT-INT] [--plot]
-               [--figdir FILE] <input.pairs> <output.pairs>
+               [--figdir FILE] [--prefix STR] <input> <output>
 
 #### Viewing the contact map
 
-Visualize a Hi-C matrix file as a heatmap of contact frequencies. Allows to tune visualisation by binning and normalizing the matrix, and to save the output image to disk. If no output is specified, the output is displayed interactively. If two contact maps are provided, the log ratio of the first divided by the second will be shown.
+Visualize a Hi-C matrix file as a heatmap of contact frequencies. Allows to
+tune visualisation by binning and normalizing the matrix, and to save the
+output image to disk. If no output is specified, the output is displayed.
 
     usage:
-        view [--binning=1] [--despeckle] [--frags FILE] [--trim INT] [--n-mad FLOAT]
-             [--normalize] [--max=99] [--output=IMG] [--cmap=CMAP] [--dpi=INT]
-             [--transform=FUN] [--circular] [--region=STR] <contact_map> [<contact_map2>]
+        view [--binning=1] [--despeckle] [--frags FILE] [--trim INT] [--n-mad 3.0] [--lines]
+             [--normalize] [--min=0] [--max=99%] [--output=IMG] [--cmap=Reds] [--dpi=300]
+             [--transform=STR] [--circular] [--region=STR] <contact_map> [<contact_map2>]
 
     arguments:
         contact_map             Sparse contact matrix in bg2, cool or graal format
         contact_map2            Sparse contact matrix in bg2, cool or graal format,
                                 if given, the log ratio of contact_map/contact_map2
                                 will be shown.
 
@@ -196,14 +221,15 @@
     hicstuff view --normalize --binning 10kb --region chr1:10,000,000-11,000,000 --frags fragments_list.txt contact_map.tsv
 ```
 ### Library
 
 All components of the hicstuff program can be used as python modules. See the documentation on [reathedocs](https://hicstuff.readthedocs.io). The expected contact map format for the library is a simple CSV file, and the objects handled by the library are simple ```numpy``` arrays. The various submodules of hicstuff contain various utilities.
 
 ```python
+import hicstuff.cutsite # Functions to digest fastq librairies
 import hicstuff.digest # Functions to work with restriction fragments
 import hicstuff.iteralign # Functions related to iterative alignment
 import hicstuff.hicstuff # Contains utilities to modify and operate on contact maps as numpy arrays
 import hicstuff.filter # Functions for filtering 3C events by type (uncut, loop)
 import hicstuff.view # Utilities to visualise contact maps
 import hicstuff.io # Reading and writing hicstuff files
 import hicstuff.pipeline # Generation and processing of files to generate matrices.
@@ -211,41 +237,40 @@
 
 ### Connecting the modules
 
 All the steps described here are handled automatically when running the `hicstuff pipeline`. But if you want to connect the different modules manually, the intermediate input and output files can be processed using some python scripting.
 
 #### Aligning the reads
 
-You can generate SAM files independently using your favorite read mapping software, use the command line utility `hicstuff iteralign`, or use the helper function `align_reads` in the submodule `hicstuff.pipeline`. For example, to perform iterative alignment using minimap2 (instead of bowtie2 by default):
+You can generate SAM files independently using your favorite read mapping software, use the command line utility `hicstuff iteralign`, or use the helper function `align_reads` in the submodule `hicstuff.pipeline`. For example, to perform iterative alignment using bwa (instead of bowtie2 by default):
 
 **Using the python function:**
 
 ```python
 from hicstuff import pipeline as hpi
 
-hpi.align_reads("end1.fastq", "genome.fasta", "end1.bam", iterative=True, minimap2=True)
+hpi.align_reads("end1.fastq", "genome.fasta", "end1.bam", iterative=True, aligner='bwa')
 ```
 
 **Using the command line tool:**
 
 ```bash
-hicstuff iteralign --minimap2 --iterative -f genome.fasta -o end1.sam end1.fastq
+hicstuff iteralign --aligner bwa --genome genome.fasta --out-bam end1.bam end1.fastq
 ```
 
-
 #### Extracting contacts from the alignment
 
-The output from `hicstuff iteralign` is a SAM file. In order to retrieve Hi-C pairs, you need to run iteralign separately on the two fastq files and process the resulting alignment files into a name-sorted BAM file as follows using the `pipeline` submodules of hicstuff.
+The output from `hicstuff iteralign` is a BAM file. In order to retrieve Hi-C pairs, you need to run iteralign separately on the two fastq files and process the resulting alignment files into a name-sorted BAM file as follows using the `pipeline` submodules of hicstuff.
 
 ```python
 from hicstuff import pipeline as hpi
 import pysam as ps
 # Sort alignments by read names and get into BAM format
-ps.sort("-n", "-O", "BAM", "-o", "end1.bam.sorted", "end1.sam")
-ps.sort("-n", "-O", "BAM", "-o", "end2.bam.sorted", "end2.sam")
+ps.sort("-n", "-O", "BAM", "-o", "end1.bam.sorted", "end1.bam")
+ps.sort("-n", "-O", "BAM", "-o", "end2.bam.sorted", "end2.bam")
 # Combine BAM files
 hpi.bam2pairs("end1.sorted.bam", "end2.sorted.bam", "output.pairs", "info_contigs.txt", min_qual=30)
 
 ```
 This will generate a "pairs" file containing all read pairs where both reads have been aligned with a mapping quality of at least 30.
 
 #### Attributing each read to a restriction fragment
```

### Comparing `hicstuff-3.1.5/hicstuff/__init__.py` & `hicstuff-3.1.6/hicstuff/__init__.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.1.5/hicstuff/commands.py` & `hicstuff-3.1.6/hicstuff/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
     options:
         -1, --forward=FILE      Fastq file containing the forward reads to
                                 digest.
         -2, --reverse=FILE      Fastq file containing the reverse reads to
                                 digest.
         -p, --prefix=STR        Prefix of the path where to write the digested
                                 gzipped fastq files. Filenames will be added the
-                                suffix "_{1,2}.fq.gz".
+                                suffix "_R{1,2}.fq.gz".
         -e, --enzyme=STR        The list of restriction enzyme used to digest
                                 the genome separated by a comma. Example:
                                 HpaII,MluCI.
         -m, --mode=STR          Digestion mode. There are three possibilities:
                                 "for_vs_rev", "all" and "pile". The first one
                                 "for_vs_rev" makes all possible contact between
                                 fragments from forward read versus the fragments
```

### Comparing `hicstuff-3.1.5/hicstuff/cutsite.py` & `hicstuff-3.1.6/hicstuff/cutsite.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     enzyme : str
         The list of restriction enzyme used to digest the genome separated by a
         comma. Example: HpaII,MluCI.
     mode : str
         Mode to use to make the digestion. Three values possible: "all",
         "for_vs_rev", "pile".
     seed_size : int
-        Minimum size of a fragment (i.e. seed size used in mapping as reads 
+        Minimum size of a fragment (i.e. seed size used in mapping as reads
         smaller won't be mapped.)
     n_cpu : int
         Number of CPUs.
     """
     # Process the ligation sites given
     ligation_sites = hcd.gen_enzyme_religation_regex(enzyme)
 
@@ -113,18 +113,24 @@
                     for_name, rev_name
                 )
             )
             sys.exit(1)
 
         # Cut the forward and reverse reads at the ligation sites.
         for_seq_list, for_qual_list = cutsite_read(
-            ligation_sites, for_seq, for_qual, seed_size,
+            ligation_sites,
+            for_seq,
+            for_qual,
+            seed_size,
         )
         rev_seq_list, rev_qual_list = cutsite_read(
-            ligation_sites, rev_seq, rev_qual, seed_size,
+            ligation_sites,
+            rev_seq,
+            rev_qual,
+            seed_size,
         )
 
         # Write the new combinations of fragments.
         new_reads_for, new_reads_rev, final_number_of_pairs = write_pair(
             new_reads_for,
             new_reads_rev,
             for_name,
@@ -152,20 +158,16 @@
     pairs = (new_reads_for.encode(), new_reads_rev.encode())
     queue.put(pairs)
     queue.put(stop_token)
     writer_process.join()
 
     # Return information on the different pairs created
     logger.info(f"Library used: {fq_for} - {fq_rev}")
-    logger.info(
-        f"Number of pairs before digestion: {original_number_of_pairs}"
-    )
-    logger.info(
-        f"Number of pairs after digestion: {final_number_of_pairs}"
-    )
+    logger.info(f"Number of pairs before digestion: {original_number_of_pairs}")
+    logger.info(f"Number of pairs after digestion: {final_number_of_pairs}")
 
 
 def cutsite_read(ligation_sites, seq, qual, seed_size=0):
     """Find ligation sites in a given sequence and return list of the fragmented
     sequence and quality.
 
     Parameters:
@@ -173,15 +175,15 @@
     ligation_sites : re.Pattern
         Regex of all possible ligations according to the given enzymes.
     seq : str
         Sequence where to search for ligation_sites.
     qual : str
         Quality values of the sequence given.
     seed_size : int
-        Minimum size of a fragment (i.e. seed size used in mapping as reads 
+        Minimum size of a fragment (i.e. seed size used in mapping as reads
         smaller won't be mapped.)
 
     Returns:
     --------
     list of str
         List of string of the sequences. The split is made at the start of the
         ligation sites.
@@ -203,18 +205,18 @@
     ligation_sites_list.append(len(seq))
 
     # Split the sequences on the ligation sites.
     seq_list = []
     qual_list = []
     left_site = 0
     for right_site in ligation_sites_list:
-        if right_site - left_site > seed_size:
-            seq_list.append(seq[left_site:right_site])
-            qual_list.append(qual[left_site:right_site])
-            left_site = right_site
+        if right_site + 4 - left_site > seed_size:
+            seq_list.append(seq[left_site : right_site + 4])
+            qual_list.append(qual[left_site : right_site + 4])
+            left_site = right_site + 4
 
     return seq_list, qual_list
 
 
 def write_pair(
     new_reads_for,
     new_reads_rev,
```

### Comparing `hicstuff-3.1.5/hicstuff/digest.py` & `hicstuff-3.1.6/hicstuff/digest.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.1.5/hicstuff/distance_law.py` & `hicstuff-3.1.6/hicstuff/distance_law.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.1.5/hicstuff/filter.py` & `hicstuff-3.1.6/hicstuff/filter.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.1.5/hicstuff/hicstuff.py` & `hicstuff-3.1.6/hicstuff/hicstuff.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.1.5/hicstuff/io.py` & `hicstuff-3.1.6/hicstuff/io.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.1.5/hicstuff/iteralign.py` & `hicstuff-3.1.6/hicstuff/iteralign.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 import shutil as st
 import hicstuff.io as hio
 import contextlib
 from hicstuff.log import logger
 from os.path import join
 
 
-
-
 def iterative_align(
     fq_in,
     tmp_dir,
     ref,
     n_cpu,
     bam_out,
     aligner="bowtie2",
@@ -48,30 +46,30 @@
 
     fq_in : str
         Path to input fastq file to align iteratively.
     tmp_dir : str
         Path where temporary files should be written.
     ref : str
         Path to the reference genome if Minimap2 is used for alignment.
-        Path to the index genome if Bowtie2/bwa is used for alignment. 
+        Path to the index genome if Bowtie2/bwa is used for alignment.
     n_cpu : int
         The number of CPUs to use for the iterative alignment.
     bam_out : str
         Path where the final alignment should be written in BAM format.
     aligner : str
         Choose between minimap2, bwa or bowtie2 for the alignment.
     min_len : int
         The initial length of the fragments to align.
     min_qual : int
         Minimum mapping quality required to keep Hi-C pairs.
     read_len : int
         Read length in the fasta file. If set to None, the length of the first read
         is used. Set this value to the longest read length in the file if you have
         different read lengths.
-        
+
     Examples
     --------
 
     iterative_align(fq_in='example_for.fastq', ref='example_bt2_index', bam_out='example_for.bam', aligner="bowtie2")
     iterative_align(fq_in='example_for.fastq', ref='example_genome.fa', bam_out='example_for.bam', aligner="minimap2")
     """
     # set with the name of the unaligned reads :
@@ -98,15 +96,15 @@
     else:
         uncomp_path = fq_in
 
     # throw error if index does not exist
     index = hio.check_fasta_index(ref, mode=aligner)
     if index is None:
         logger.error(
-            f"Reference index is missing, please build the {aligner} index first." 
+            f"Reference index is missing, please build the {aligner} index first."
         )
         sys.exit(1)
     # Counting reads
     with hio.read_compressed(uncomp_path) as inf:
         for _ in inf:
             total_reads += 1
     total_reads /= 4
@@ -156,18 +154,20 @@
         }
         if re.match(r"^(minimap[2]?|mm[2]?)$", aligner, flags=re.IGNORECASE):
             cmd = "minimap2 -x sr -a -t {cpus} {fa} {fq}".format(**map_args)
         elif re.match(r"^(bwa)$", aligner, flags=re.IGNORECASE):
             cmd = "bwa mem -t {cpus} -v 1 {idx} {fq}".format(**map_args)
         elif re.match(r"^(bowtie[2]?|bt[2]?)$", aligner, flags=re.IGNORECASE):
             cmd = (
-                "bowtie2 -x {idx} -p {cpus}" " --quiet --very-sensitive {fq}"
+                "bowtie2 -x {idx} -p {cpus} --quiet --very-sensitive-local -U {fq}"
             ).format(**map_args)
         else:
-            raise ValueError("Unknown aligner. Select bowtie2, minimap2 or bwa.")
+            raise ValueError(
+                "Unknown aligner. Select bowtie2, minimap2 or bwa."
+            )
 
         map_process = sp.Popen(cmd, shell=True, stdout=sp.PIPE)
         sort_process = sp.Popen(
             "samtools sort -n -@ {cpus} -O BAM -o {bam}".format(**map_args),
             shell=True,
             stdin=map_process.stdout,
         )
@@ -179,15 +179,17 @@
         remaining_reads = filter_bamfile(temp_alignment, iter_out[-1], min_qual)
 
         n += 20
         first_round = False
 
     # one last round without trimming
     logger.info(
-        "Trying to map unaligned reads at full length ({0}bp).".format(int(read_len))
+        "Trying to map unaligned reads at full length ({0}bp).".format(
+            int(read_len)
+        )
     )
 
     truncated_reads = truncate_reads(
         tmp_dir,
         infile=uncomp_path,
         unaligned_set=remaining_reads,
         trunc_len=n,
@@ -198,17 +200,17 @@
             fa=ref, cpus=n_cpu, fq=truncated_reads
         )
     elif aligner == "bwa" or aligner == "Bwa" or aligner == "BWA":
         cmd = "bwa mem -v 1 -t {cpus} {idx} {fq}".format(
             idx=index, cpus=n_cpu, fq=truncated_reads
         )
     else:
-        cmd = ("bowtie2 -x {idx} -p {cpus} --quiet " "--very-sensitive {fq}").format(
-            idx=index, cpus=n_cpu, fq=truncated_reads
-        )
+        cmd = (
+            "bowtie2 -x {idx} -p {cpus} --quiet " "--very-sensitive {fq}"
+        ).format(idx=index, cpus=n_cpu, fq=truncated_reads)
     map_process = sp.Popen(cmd, shell=True, stdout=sp.PIPE)
     # Keep reads sorted by name
     sort_process = sp.Popen(
         "samtools sort -n -@ {cpus} -O BAM -o {bam}".format(
             cpus=n_cpu, bam=temp_alignment
         ),
         shell=True,
@@ -256,15 +258,15 @@
     unaligned_set : set
         Contains the names of all reads that did not map unambiguously in
         previous rounds.
     trunc_len : int
         The number of basepairs to keep in each truncated sequence.
     first_round : bool
         If this is the first round, truncate all reads without checking mapping.
-    
+
     Returns
     -------
 
     str :
         Path to the output fastq file containing truncated reads.
     """
 
@@ -291,15 +293,15 @@
     ----------
     temp_alignment : str
         Path to the input temporary alignment.
     outfile : str
         Path to the output filtered temporary alignment.
     min_qual : int
         Minimum mapping quality required to keep a Hi-C pair.
-    
+
     Returns
     -------
     set:
         Contains the names reads that did not align.
     """
     # Check the quality and status of each aligned fragment.
     # Write the ones with good quality in the final output file.
```

### Comparing `hicstuff-3.1.5/hicstuff/log.py` & `hicstuff-3.1.6/hicstuff/log.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.1.5/hicstuff/main.py` & `hicstuff-3.1.6/hicstuff/main.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.1.5/hicstuff/pipeline.py` & `hicstuff-3.1.6/hicstuff/pipeline.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.1.5/hicstuff/view.py` & `hicstuff-3.1.6/hicstuff/view.py`

 * *Files identical despite different names*

### Comparing `hicstuff-3.1.5/hicstuff.egg-info/PKG-INFO` & `hicstuff-3.1.6/hicstuff.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,72 +1,84 @@
 Metadata-Version: 2.1
 Name: hicstuff
-Version: 3.1.5
+Version: 3.1.6
 Summary: General purpose stuff to generate and handle Hi-C data in its simplest form.
 Home-page: https://github.com/koszullab/hicstuff
 Author: cyril.matthey-doret@pasteur.fr
 License: BSD-3-Clause
 Description: # hicstuff
         
         [![PyPI version](https://badge.fury.io/py/hicstuff.svg)](https://badge.fury.io/py/hicstuff)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hicstuff.svg)
+        [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/hicstuff/README.html)
         [![Build Status](https://github.com/koszullab/hicstuff/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/koszullab/hicstuff/actions/workflows/build.yml)
-        [![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/koszullab/hicstuff)](https://hub.docker.com/r/koszullab/hicstuff)
         [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2620608.svg)](https://doi.org/10.5281/zenodo.2620608)
         [![codecov](https://codecov.io/gh/koszullab/hicstuff/branch/master/graph/badge.svg)](https://codecov.io/gh/koszullab/hicstuff)
         [![Read the docs](https://readthedocs.org/projects/hicstuff/badge)](https://hicstuff.readthedocs.io)
         [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/koszullab/hicstuff/master?filepath=doc%2Fnotebooks%2Fdemo_api.ipynb)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
         
         A lightweight library that generates and handles Hi-C contact maps in either cooler-compatible 2Dbedgraph or [instaGRAAL](https://github.com/koszullab/instaGRAAL) format. It is essentially a merge of the [yahcp](https://github.com/baudrly/yahcp) pipeline, the [hicstuff](https://github.com/baudrly/hicstuff) library and extra features illustrated in the [3C tutorial](https://github.com/axelcournac/3C_tutorial) and the [DADE pipeline](https://github.com/scovit/dade), all packaged together for extra convenience.
         
         The goal is to make generation and manipulation of Hi-C matrices as simple as possible and work for any organism.
         
         ## Table of contents
         
-        * [Installation](#Installation)
-        * [Usage](#Usage)
-          * [Full pipeline](#Full-pipeline)
-          * [Individual components](#Individual-components)
-        * [Library](#Library)
-        * [Connecting the modules](#Connecting-the-modules)
-        * [File formats](#File-formats)
-        * [Contributing](#Contributing)
+        * [Installation](#installation)
+          * [pip](#pip)
+          * [conda](#conda)
+          * [docker](#docker)
+        * [Usage](#usage)
+          * [Full pipeline](#full-pipeline)
+          * [Individual components](#individual-components)
+        * [Library](#library)
+        * [Connecting the modules](#connecting-the-modules)
+        * [File formats](#file-formats)
+        * [Contributing](#contributing)
         
         ## Installation
         
+        ### pip
+        
         To install a stable version:
         ```sh
         pip3 install -U hicstuff
         ```
         
         or, for the latest development version:
         
         ```sh
             pip3 install -e git+https://github.com/koszullab/hicstuff.git@master#egg=hicstuff
         ```
         
-        ### External dependencies
-        
-        Bowtie2 and/or minimap2 as well as samtools are required for the `pipeline` utility.
+        `bowtie2`, `bwa` and/or `minimap2` as well as `samtools` are required by the `pipeline` command.
         
         You can install them via the conda package manager:
         ```bash
-        conda install -c bioconda minimap2 bowtie2 samtools
+        conda install -c bioconda bowtie2 bwa minimap2 samtools
         ```
         Alternatively, on ubuntu you can also install them along with additional dependencies through APT:
         ```bash
-        apt-get install samtools bowtie2 minimap2 libbz2-dev liblzma-dev
+        apt-get install bowtie2 bwa minimap2 samtools libbz2-dev liblzma-dev
         ```
         
-        ### Docker installation
+        ### Conda
+        
+        hicstuff is available as a bioconda package. It can be installed, along with all dependencies using:
         
-        A pre-built docker image is available on dockerhub and can be ran using:
         ```bash
-        docker run koszullab/hicstuff
+        conda install -c bioconda hicstuff
+        ```
+        
+        ### Docker
+        
+        A pre-built docker image is made available on quay.io via [biocontainers](https://biocontainers.pro/) and can be ran using:
+        
+        ```bash
+        docker pull quay.io/biocontainers/hicstuff:<tag>
         ```
         
         ## Usage
         
         The hicstuff command line interface is composed of multiple subcommands. You can always get a summary of all available commands by running:
         
         ```bash
@@ -78,34 +90,37 @@
             hicstuff [-hv] <command> [<args>...]
         
         options:
             -h, --help                  shows the help
             -v, --version               shows the version
         
         The subcommands are:
+            convert         Convert Hi-C data between different formats.
             digest          Digest genome into a list of fragments.
+            cutsite         Preprocess fastq files by digesting reads at religation site.
             distancelaw     Analyse and plot distance law.
             filter          Filters Hi-C pairs to exclude spurious events.
             iteralign       Iteratively aligns reads to a reference genome.
+            missview        Preview missing Hi-C bins in based on the genome and read length.
             pipeline        Hi-C pipeline to generate contact matrix from fastq files.
             rebin           Bin the matrix and regenerate files accordingly.
             subsample       Bootstrap subsampling of contacts from a Hi-C map.
-            view            Visualize a Hi-C matrix.  
+            view            Visualize a Hi-C matrix.
         ```
         
         ### Full pipeline
         
         All components of the pipeline can be run at once using the `hicstuff pipeline` command. This allows to generate a contact matrix from reads in a single command. By default, the output is in GRAAL compatible COO sparse matrix format, but it can be a 2D bedgraph or cool file instead using the `--matfmt` option. More detailed documentation can be found on the readthedocs website: https://hicstuff.readthedocs.io/en/latest/index.html
         
             usage:
-                pipeline [--quality-min=INT] [--size=INT] [--no-cleanup] [--start-stage=STAGE]
-                         [--threads=INT] [--aligner=bowtie2] [--matfmt=FMT] [--prefix=PREFIX]
-                         [--tmpdir=DIR] [--iterative] [--outdir=DIR] [--filter] [--enzyme=ENZ]
-                         [--plot] [--circular] [--distance-law] [--duplicates] [--read-len=INT]
-                         [--centromeres=FILE] [--remove-centromeres=INT] --genome=FILE <input1> [<input2>]
+                pipeline [--aligner=bowtie2] [--centromeres=FILE] [--circular] [--distance-law]
+                         [--duplicates] [--enzyme=5000] [--filter] [--force] [--mapping=normal]
+                         [--matfmt=graal] [--no-cleanup] [--outdir=DIR] [--plot] [--prefix=PREFIX]
+                         [--quality-min=30] [--read-len=INT] [--remove-centromeres=0] [--size=0]
+                         [--start-stage=fastq] [--threads=1] [--tmpdir=DIR] --genome=FILE <input1> [<input2>]
         
             arguments:
                 input1:             Forward fastq file, if start_stage is "fastq", sam
                                     file for aligned forward reads if start_stage is
                                     "bam", or a .pairs file if start_stage is "pairs".
                 input2:             Reverse fastq file, if start_stage is "fastq", sam
                                     file for aligned reverse reads if start_stage is
@@ -124,76 +139,86 @@
         # Note the bam files have to be name-sorted, this can be done using samtools
         samtools sort -n aligned_for.bam -o namesorted_for.bam
         samtools sort -n aligned_rev.bam -o namesorted_rev.bam
         hicstuff pipeline -S bam -e 5000 -M cool -o out/ -g genome.fa namesorted_for.bam namesorted_rev.bam
         ```
         
         
-        The pipeline can also be run from python, using the `hicstuff.pipeline` submodule. For example, this would run the pipeline with bowtie2 (default) using iterative alignment and keep all intermediate files. For more examples using the API, see the [API demo](https://hicstuff.readthedocs.io/en/latest/notebooks/demo_api.html)
+        The pipeline can also be run from python, using the `hicstuff.pipeline` submodule. For example, this would run the pipeline with bowtie2 (default) using cutsiste alignment and keep all intermediate files. For more examples using the API, see the [API demo](https://hicstuff.readthedocs.io/en/latest/notebooks/demo_api.html)
         
         ```python
         from hicstuff import pipeline as hpi
         
         hpi.full_pipeline(
             'genome.fa', 
             'end1.fq', 
             'end2.fq', 
             no_cleanup=True
-            iterative=True
+            mapping='cutsite',
             out_dir='out', 
             enzyme="DpnII")
         ```
         
         The general steps of the pipeline are as follows:
         
         ![Pipeline flowchart](doc/images/pipeline.svg)
         
         ### Individual components
         
         For more advanced usage, different scripts can be used independently on the command line to perform individual parts of the pipeline. This readme contains quick descriptions and example usages. To obtain detailed instructions on any subcommand, one can use `hicstuff <subcommand> --help`.
         
+        ### Digestion of the reads
+         
+        Generates new gzipped fastq files from original fastq. The function will cut the reads at their religation sites and creates new pairs of reads with the different fragments obtained after cutting at the digestion sites.
+        
+            usage:
+                cutsite --forward=FILE --reverse=FILE  --prefix=STR --enzyme=STR
+                [--mode=for_vs_rev] [--seed-size=20] [--threads=1]
+        
         #### Iterative alignment
         
         Truncate reads from a fastq file to 20 basepairs and iteratively extend and re-align the unmapped reads to optimize the proportion of uniquely aligned reads in a 3C library.
         
             usage:
-                iteralign [--aligner=bowtie2] [--threads=1] [--min_len=20]
-                          [--tempdir DIR] --out_sam=FILE --genome=FILE <reads.fq>
+                iteralign [--aligner=bowtie2] [--threads=1] [--min-len=20] [--read-len=INT]
+                          [--tempdir=DIR] --out-bam=FILE --genome=FILE <reads.fq>
         
         #### Digestion of the genome
         
         Digests a fasta file into fragments based on a restriction enzyme or a
         fixed chunk size. Generates two output files into the target directory
         named "info_contigs.txt" and "fragments_list.txt"
         
             usage:
-                digest [--plot] [--figdir=FILE] [--circular] [--size=INT]
+                digest [--plot] [--figdir=FILE] [--force] [--circular] [--size=0]
                        [--outdir=DIR] --enzyme=ENZ <fasta>
         
          
          For example, to digest the yeast genome with MaeII and HinfI and show histogram of fragment lengths:
         
         `hicstuff digest --plot --outdir output_dir --enzyme MaeII,HinfI Sc_ref.fa`
         
         #### Filtering of 3C events
         
         Filters spurious 3C events such as loops and uncuts from the library based on a minimum distance threshold automatically estimated from the library by default. Can also plot 3C library statistics. This module takes a pairs file with 9 columns as input (readID, chr1, pos1, chr2, pos2, strand1, strand2, frag1, frag2) and filters it. 
         
             usage:
                 filter [--interactive | --thresholds INT-INT] [--plot]
-                       [--figdir FILE] <input.pairs> <output.pairs>
+                       [--figdir FILE] [--prefix STR] <input> <output>
         
         #### Viewing the contact map
         
-        Visualize a Hi-C matrix file as a heatmap of contact frequencies. Allows to tune visualisation by binning and normalizing the matrix, and to save the output image to disk. If no output is specified, the output is displayed interactively. If two contact maps are provided, the log ratio of the first divided by the second will be shown.
+        Visualize a Hi-C matrix file as a heatmap of contact frequencies. Allows to
+        tune visualisation by binning and normalizing the matrix, and to save the
+        output image to disk. If no output is specified, the output is displayed.
         
             usage:
-                view [--binning=1] [--despeckle] [--frags FILE] [--trim INT] [--n-mad FLOAT]
-                     [--normalize] [--max=99] [--output=IMG] [--cmap=CMAP] [--dpi=INT]
-                     [--transform=FUN] [--circular] [--region=STR] <contact_map> [<contact_map2>]
+                view [--binning=1] [--despeckle] [--frags FILE] [--trim INT] [--n-mad 3.0] [--lines]
+                     [--normalize] [--min=0] [--max=99%] [--output=IMG] [--cmap=Reds] [--dpi=300]
+                     [--transform=STR] [--circular] [--region=STR] <contact_map> [<contact_map2>]
         
             arguments:
                 contact_map             Sparse contact matrix in bg2, cool or graal format
                 contact_map2            Sparse contact matrix in bg2, cool or graal format,
                                         if given, the log ratio of contact_map/contact_map2
                                         will be shown.
         
@@ -203,14 +228,15 @@
             hicstuff view --normalize --binning 10kb --region chr1:10,000,000-11,000,000 --frags fragments_list.txt contact_map.tsv
         ```
         ### Library
         
         All components of the hicstuff program can be used as python modules. See the documentation on [reathedocs](https://hicstuff.readthedocs.io). The expected contact map format for the library is a simple CSV file, and the objects handled by the library are simple ```numpy``` arrays. The various submodules of hicstuff contain various utilities.
         
         ```python
+        import hicstuff.cutsite # Functions to digest fastq librairies
         import hicstuff.digest # Functions to work with restriction fragments
         import hicstuff.iteralign # Functions related to iterative alignment
         import hicstuff.hicstuff # Contains utilities to modify and operate on contact maps as numpy arrays
         import hicstuff.filter # Functions for filtering 3C events by type (uncut, loop)
         import hicstuff.view # Utilities to visualise contact maps
         import hicstuff.io # Reading and writing hicstuff files
         import hicstuff.pipeline # Generation and processing of files to generate matrices.
@@ -218,41 +244,40 @@
         
         ### Connecting the modules
         
         All the steps described here are handled automatically when running the `hicstuff pipeline`. But if you want to connect the different modules manually, the intermediate input and output files can be processed using some python scripting.
         
         #### Aligning the reads
         
-        You can generate SAM files independently using your favorite read mapping software, use the command line utility `hicstuff iteralign`, or use the helper function `align_reads` in the submodule `hicstuff.pipeline`. For example, to perform iterative alignment using minimap2 (instead of bowtie2 by default):
+        You can generate SAM files independently using your favorite read mapping software, use the command line utility `hicstuff iteralign`, or use the helper function `align_reads` in the submodule `hicstuff.pipeline`. For example, to perform iterative alignment using bwa (instead of bowtie2 by default):
         
         **Using the python function:**
         
         ```python
         from hicstuff import pipeline as hpi
         
-        hpi.align_reads("end1.fastq", "genome.fasta", "end1.bam", iterative=True, minimap2=True)
+        hpi.align_reads("end1.fastq", "genome.fasta", "end1.bam", iterative=True, aligner='bwa')
         ```
         
         **Using the command line tool:**
         
         ```bash
-        hicstuff iteralign --minimap2 --iterative -f genome.fasta -o end1.sam end1.fastq
+        hicstuff iteralign --aligner bwa --genome genome.fasta --out-bam end1.bam end1.fastq
         ```
         
-        
         #### Extracting contacts from the alignment
         
-        The output from `hicstuff iteralign` is a SAM file. In order to retrieve Hi-C pairs, you need to run iteralign separately on the two fastq files and process the resulting alignment files into a name-sorted BAM file as follows using the `pipeline` submodules of hicstuff.
+        The output from `hicstuff iteralign` is a BAM file. In order to retrieve Hi-C pairs, you need to run iteralign separately on the two fastq files and process the resulting alignment files into a name-sorted BAM file as follows using the `pipeline` submodules of hicstuff.
         
         ```python
         from hicstuff import pipeline as hpi
         import pysam as ps
         # Sort alignments by read names and get into BAM format
-        ps.sort("-n", "-O", "BAM", "-o", "end1.bam.sorted", "end1.sam")
-        ps.sort("-n", "-O", "BAM", "-o", "end2.bam.sorted", "end2.sam")
+        ps.sort("-n", "-O", "BAM", "-o", "end1.bam.sorted", "end1.bam")
+        ps.sort("-n", "-O", "BAM", "-o", "end2.bam.sorted", "end2.bam")
         # Combine BAM files
         hpi.bam2pairs("end1.sorted.bam", "end2.sorted.bam", "output.pairs", "info_contigs.txt", min_qual=30)
         
         ```
         This will generate a "pairs" file containing all read pairs where both reads have been aligned with a mapping quality of at least 30.
         
         #### Attributing each read to a restriction fragment
```

### Comparing `hicstuff-3.1.5/hicstuff.egg-info/SOURCES.txt` & `hicstuff-3.1.6/hicstuff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hicstuff-3.1.5/setup.py` & `hicstuff-3.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Operating System :: MacOS",
 ]
 
 name = "hicstuff"
 
 MAJOR = 3
 MINOR = 1
-MAINTENANCE = 5
+MAINTENANCE = 6
 VERSION = "{}.{}.{}".format(MAJOR, MINOR, MAINTENANCE)
 
 LICENSE = "BSD-3-Clause"
 URL = "https://github.com/koszullab/hicstuff"
 
 DESCRIPTION = __doc__.strip("\n")
```

