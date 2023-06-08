# Comparing `tmp/splicekit-0.4.2.tar.gz` & `tmp/splicekit-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splicekit-0.4.2.tar", last modified: Tue May 30 11:38:25 2023, max compression
+gzip compressed data, was "splicekit-0.4.3.tar", last modified: Thu Jun  8 07:40:46 2023, max compression
```

## Comparing `splicekit-0.4.2.tar` & `splicekit-0.4.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-30 11:38:25.387109 splicekit-0.4.2/
--rw-rw-r--   0 rotg     (2023757) games       (20)    22857 2023-05-30 11:38:25.386836 splicekit-0.4.2/PKG-INFO
--rwxrwxr-x   0 rotg     (2023757) games       (20)    22459 2023-05-30 11:36:14.000000 splicekit-0.4.2/README.md
--rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-05-30 11:38:25.387203 splicekit-0.4.2/setup.cfg
--rw-rw-r--   0 rotg     (2023757) games       (20)     1133 2023-05-25 08:08:20.000000 splicekit-0.4.2/setup.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-30 11:38:25.371393 splicekit-0.4.2/splicekit/
--rw-rw-r--   0 rotg     (2023757) games       (20)    13778 2023-05-30 11:37:41.000000 splicekit-0.4.2/splicekit/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-30 11:38:25.375309 splicekit-0.4.2/splicekit/clusterlogfc/
--rw-rw-r--   0 rotg     (2023757) games       (20)     5584 2023-05-05 11:49:03.000000 splicekit-0.4.2/splicekit/clusterlogfc/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-30 11:38:25.376013 splicekit-0.4.2/splicekit/config/
--rw-rw-r--   0 rotg     (2023757) games       (20)      850 2023-05-25 11:18:03.000000 splicekit-0.4.2/splicekit/config/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-30 11:38:25.385656 splicekit-0.4.2/splicekit/core/
--rw-rw-r--   0 rotg     (2023757) games       (20)      396 2023-01-31 12:27:24.000000 splicekit-0.4.2/splicekit/core/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     6667 2023-05-05 06:13:11.000000 splicekit-0.4.2/splicekit/core/anchors.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    16752 2023-05-24 07:18:50.000000 splicekit-0.4.2/splicekit/core/annotation.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     3988 2023-01-31 12:27:24.000000 splicekit-0.4.2/splicekit/core/delta_dar.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     5407 2023-05-05 08:10:13.000000 splicekit-0.4.2/splicekit/core/exons.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)    29902 2023-05-03 08:24:07.000000 splicekit-0.4.2/splicekit/core/features.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     5662 2023-05-05 06:13:26.000000 splicekit-0.4.2/splicekit/core/genes.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1061 2023-05-25 11:01:47.000000 splicekit-0.4.2/splicekit/core/jbrowse2.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     8872 2023-05-30 11:34:53.000000 splicekit-0.4.2/splicekit/core/jbrowse2_create.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2948 2023-04-26 12:12:45.000000 splicekit-0.4.2/splicekit/core/juan.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    18195 2023-05-02 17:27:43.000000 splicekit-0.4.2/splicekit/core/junctions.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    37713 2023-05-04 06:56:59.000000 splicekit-0.4.2/splicekit/core/motifs.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1663 2023-05-02 18:35:35.000000 splicekit-0.4.2/splicekit/core/patterns.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2420 2023-05-03 10:54:22.000000 splicekit-0.4.2/splicekit/core/promisc.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     9045 2023-05-03 09:57:04.000000 splicekit-0.4.2/splicekit/core/report.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-30 11:38:25.386260 splicekit-0.4.2/splicekit/judge/
--rw-rw-r--   0 rotg     (2023757) games       (20)    26830 2023-05-02 18:05:54.000000 splicekit-0.4.2/splicekit/judge/__init__.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)     5402 2023-05-05 10:18:19.000000 splicekit-0.4.2/splicekit/splicecompare
--rwxrwxr-x   0 rotg     (2023757) games       (20)     4750 2023-05-30 11:35:14.000000 splicekit-0.4.2/splicekit/splicekit
--rw-rw-r--   0 rotg     (2023757) games       (20)     1670 2023-05-24 07:25:57.000000 splicekit-0.4.2/splicekit/splicekit.config.template
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-05-30 11:38:19.000000 splicekit-0.4.2/splicekit/version
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-30 11:38:25.374887 splicekit-0.4.2/splicekit.egg-info/
--rw-rw-r--   0 rotg     (2023757) games       (20)    22857 2023-05-30 11:38:25.372121 splicekit-0.4.2/splicekit.egg-info/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)      826 2023-05-30 11:38:25.373141 splicekit-0.4.2/splicekit.egg-info/SOURCES.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-30 11:38:25.373461 splicekit-0.4.2/splicekit.egg-info/dependency_links.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-09 07:35:55.000000 splicekit-0.4.2/splicekit.egg-info/not-zip-safe
--rw-rw-r--   0 rotg     (2023757) games       (20)       62 2023-05-30 11:38:25.374645 splicekit-0.4.2/splicekit.egg-info/requires.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)       10 2023-05-30 11:38:25.374963 splicekit-0.4.2/splicekit.egg-info/top_level.txt
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-08 07:40:46.110929 splicekit-0.4.3/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    23142 2023-06-08 07:40:46.110340 splicekit-0.4.3/PKG-INFO
+-rwxrwxr-x   0 rotg     (2023757) games       (20)    22744 2023-06-06 14:20:03.000000 splicekit-0.4.3/README.md
+-rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-06-08 07:40:46.111031 splicekit-0.4.3/setup.cfg
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1133 2023-05-25 08:08:20.000000 splicekit-0.4.3/setup.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-08 07:40:46.087030 splicekit-0.4.3/splicekit/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    13857 2023-06-08 07:08:02.000000 splicekit-0.4.3/splicekit/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-08 07:40:46.090636 splicekit-0.4.3/splicekit/clusterlogfc/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5584 2023-05-05 11:49:03.000000 splicekit-0.4.3/splicekit/clusterlogfc/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-08 07:40:46.092167 splicekit-0.4.3/splicekit/config/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      951 2023-06-07 13:26:10.000000 splicekit-0.4.3/splicekit/config/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-08 07:40:46.107484 splicekit-0.4.3/splicekit/core/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      396 2023-01-31 12:27:24.000000 splicekit-0.4.3/splicekit/core/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     6667 2023-05-05 06:13:11.000000 splicekit-0.4.3/splicekit/core/anchors.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    16752 2023-05-24 07:18:50.000000 splicekit-0.4.3/splicekit/core/annotation.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     3988 2023-01-31 12:27:24.000000 splicekit-0.4.3/splicekit/core/delta_dar.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5407 2023-05-05 08:10:13.000000 splicekit-0.4.3/splicekit/core/exons.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)    29902 2023-05-03 08:24:07.000000 splicekit-0.4.3/splicekit/core/features.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5662 2023-05-05 06:13:26.000000 splicekit-0.4.3/splicekit/core/genes.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1059 2023-06-07 14:32:33.000000 splicekit-0.4.3/splicekit/core/jbrowse2.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     8978 2023-06-07 14:07:47.000000 splicekit-0.4.3/splicekit/core/jbrowse2_create.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2948 2023-04-26 12:12:45.000000 splicekit-0.4.3/splicekit/core/juan.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    18195 2023-05-02 17:27:43.000000 splicekit-0.4.3/splicekit/core/junctions.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    37713 2023-05-04 06:56:59.000000 splicekit-0.4.3/splicekit/core/motifs.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1663 2023-05-02 18:35:35.000000 splicekit-0.4.3/splicekit/core/patterns.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2420 2023-05-03 10:54:22.000000 splicekit-0.4.3/splicekit/core/promisc.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9045 2023-05-03 09:57:04.000000 splicekit-0.4.3/splicekit/core/report.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-08 07:40:46.109005 splicekit-0.4.3/splicekit/judge/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    26830 2023-05-02 18:05:54.000000 splicekit-0.4.3/splicekit/judge/__init__.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     5402 2023-05-05 10:18:19.000000 splicekit-0.4.3/splicekit/splicecompare
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     5165 2023-06-08 07:07:45.000000 splicekit-0.4.3/splicekit/splicekit
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1638 2023-06-06 07:56:19.000000 splicekit-0.4.3/splicekit/splicekit.config.template
+-rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-06-08 07:40:35.000000 splicekit-0.4.3/splicekit/version
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-06-08 07:40:46.089992 splicekit-0.4.3/splicekit.egg-info/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    23142 2023-06-08 07:40:45.000000 splicekit-0.4.3/splicekit.egg-info/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)      826 2023-06-08 07:40:45.000000 splicekit-0.4.3/splicekit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-06-08 07:40:45.000000 splicekit-0.4.3/splicekit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-09 07:35:55.000000 splicekit-0.4.3/splicekit.egg-info/not-zip-safe
+-rw-rw-r--   0 rotg     (2023757) games       (20)       62 2023-06-08 07:40:45.000000 splicekit-0.4.3/splicekit.egg-info/requires.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)       10 2023-06-08 07:40:45.000000 splicekit-0.4.3/splicekit.egg-info/top_level.txt
```

### Comparing `splicekit-0.4.2/PKG-INFO` & `splicekit-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,92 +1,53 @@
 Metadata-Version: 2.1
 Name: splicekit
-Version: 0.4.2
+Version: 0.4.3
 Summary: splicekit: comprehensive toolkit for splicing analysis from short-read RNA-seq
 Home-page: https://github.com/bedapub/splicekit
 Author: Roche, PMDA Spliceosome team
 Author-email: gregor.rot@gmail.com
 Keywords: splicekit,splicing,transcriptomics,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 
-A comprehensive platform for splicing analysis of RNA-seq short-read sequencing data. <b>splicekit</b> input are read alignments in .bam format (look at [datasets](datasets) for details on how to run examples).
+A comprehensive platform for splicing analysis of RNA-seq short-read sequencing data. <b>splicekit</b> input are read alignments in BAM format (look at [datasets](datasets) for details on how to run examples).
 
-[What does splicekit do?](#what_do)<br>
-[Changelog](#changelog)<br>
-[Quick start and installation](#initial_setup)<br>
-[Running Splicekit](#running_splicekit)<br>
+[What is splicekit?](#what_do)<br>
+[Installation and quick start](#initial_setup)<br>
+[Running splicekit](#running_splicekit)<br>
 &nbsp;&nbsp;[Annotation and comparisons](#annot_comp)<br>
 &nbsp;&nbsp;[Preparing feature (genes, exon, junction, anchor) data tables](#make_tables)<br>
 &nbsp;&nbsp;[Running edgeR gene context analysis on junction features](#id_features)<br>
 [Motif analysis](#motif)<br>
 [Scanning for RNA-protein binding with scanRBP](#scanRBP)<br>
 [juDGE plots](#judgeplot)<br>
-[Jbrowse2 visualizations](#jbrowse)<br>
+[JBrowse2 visualizations](#jbrowse)<br>
 [Documentation and specifications](#filedescriptors)<br>
+[Changelog](#changelog)<br>
 
 <b>splicekit</b> is a modular platform for splicing analysis of RNA-seq datasets. The platform also integrates an JBrowse2 instance together with [pybio](https://github.com/grexor/pybio) for genomic operations and [scanRBP](https://github.com/grexor/scanRBP) for RNA-protein binding studies. The whole analysis is self-contained (one single folder) and the platform is written in Python, in a modular way.
 
-## What does splicekit do?<a name="what_do"></a>
-From an initial setup (`splicekit.config`) and sample annotation (`samples.tab`), splicekit generates comparisons (which samples to compare to which controls). Next, feature count tables are generated (exons, anchors, junctions, genes) based on defined comparisons. Analyses incude edgeR altsplice (differentially used features), motif analysis with DonJuan (junction-anchor) and DREME, RNA-protein binding enrichment analysis with scanRBP and clustering analysis on expression of features. To facilitate result and data interpretation, splicekit also provides an instance of JBrowse2.
-
-## Changelog<a name="changelog"></a>
-
-**v0.4**: released in May 2023
-* added singularity container with all dependencies
-* added local integrated JBrowse2
-* cluster or desktop runs
-* scanRBP and bootstrap analysis of RNA-protein binding
-* further development and integration with pybio
-* extended documentation of concepts, analysis and results
-
-<details>
-<summary><b>v0.3</b>: released in January 2023 (click to show details)</summary>
-
-* re-coded junction analysis
-  * independent junctions parsing from provided bam files
-  * master table of all junctions in the samples of the analyzed project, including novel junctions (refseq/ensembl non-annotated)
-* clustering by logFC of pairwise-comparisons with dendrogram: junction, exon and gene levels (clusterlogfc module)
-* added *first_exon* annotation for junctions touching annotated first exons of transcripts
-* extended documentation of concepts, analysis and results
-</details>
-
-<details>
-<summary><b>v0.2</b>: released in October 2022 (click to show details)</summary>
-
-* software architecture restructure with python modules
-* filtering of lowly expressed features by edgeR
-* DonJuan analysis (junction-anchor analysis)
-* more advanced motif analysis with DREME
-* filtering regulated junctions with regulated donors
-</details>
-
-<details>
-<summary><b>v0.1</b>: released in July 2022 (click to show details)</summary>
+## What is splicekit?<a name="what_do"></a>
+From an initial config file (`splicekit.config`), sample annotation (`samples.tab`) and aligned reads in BAM format, splicekit first defines comparisons (which test samples to compare to which controls). Next, feature count tables are generated (exons, anchors, junctions, genes) based on defined comparisons. Analysis incude edgeR alt-splice (differentially used features), motif analysis with DonJuAn (junction-anchor) and DREME, RNA-protein binding enrichment analysis with scanRBP and clustering analysis on expression of features. To facilitate result and data interpretation, splicekit also provides an instance of JBrowse2.
 
-* initial version of splicekit
-* parsing of junction and exon counts
-* computing edgeR analysis from count tables and producing a results file with direct links to JBrowse2
-* basic motif analysis
-</details>
-
-## Quick start and installation<a name="initial_setup"></a>
+## Installation and quick start<a name="initial_setup"></a>
 
 The easiest way to install splicekit is to simply run:
 
 `$ pip install splicekit`
 
+Note that on some systems, pip is installing the executable scripts under `~/.local/bin`. However this folder is not in the PATH which will result in `command not found` if you try to run `$ splicekit` on the command line. To fix this, please execute `export PATH="$PATH:~/.local/bin"` (and add this to your `.profile`). Another suggestion is to install inside a virtual environment (using `virtualenv`).
+
 If you would like to install splicekit directly from this repository, clone the repository into a folder, for example `~/software/splicekit`. Add the `~/software/splicekit` folder to $PYTHONPATH (`export PYTHONPATH=$PYTHONPATH:~/software/splicekit`).
 
 ### Software dependencies
 
 splicekit uses several third-party open-source software. If you don't have the software installed on your system, we prepared a [singularity definition file](singularity), where you can also directly see all dependencies. Using the singularity image, you don't need to install the dependencies yourself, you just need to install singularity.
 
-
 ### Example runs and datasets
 
 Example runs can be found in the [datasets](datasets) folder.
 
 ### Configuration file documentation
 
 <details>
@@ -129,20 +90,14 @@
 Processing parameters:
 
 | Parameter | Description | Default / Example |
 |-|-|-|
 | platform | "desktop" or "cluster" (HPC with SLURM) | "desktop"
 | container | leave empty or for singularity use: "singularity"; this will download and run "singularity/splicekit_version.sif" | "desktop"
 
-JBrowse2 parameters:
-
-| Parameter | Description | Default / Example |
-|-|-|-|
-| jbrowse2_url | URL of the local JBrowse2 instance | "localhost/jbrowse2"
-
 Visualization, labelling and other parameters:
 
 | Parameter | Description | Default / Example |
 |-|-|-|
 | short_names | List of triples for shortening names in results, if last string is "complete", only entire strings will be considered (no partial replacement) | [], example: [("cell_line_A", "A", "complete")], this would only replace cell_line_A with A if cell_line_A is the whole string, while if "partial" is provided, also strings like ...cell_line_A... would be replaced with ...A... | ("original name", "short name", "complete")
 
 </details>
@@ -388,7 +343,47 @@
 **Exon** specific (additional) columns:
 
 | column | description |
 |-|-|
 | delta_PSI | test_PSI-control_PSI, percentage spliced-in |
 
 </details>
+
+## Changelog<a name="changelog"></a>
+
+**v0.4**: released in May 2023
+* added singularity container with all dependencies
+* added local integrated JBrowse2
+* cluster or desktop runs
+* scanRBP and bootstrap analysis of RNA-protein binding
+* further development and integration with pybio
+* extended documentation of concepts, analysis and results
+
+<details>
+<summary><b>v0.3</b>: released in January 2023 (click to show details)</summary>
+
+* re-coded junction analysis
+  * independent junctions parsing from provided bam files
+  * master table of all junctions in the samples of the analyzed project, including novel junctions (refseq/ensembl non-annotated)
+* clustering by logFC of pairwise-comparisons with dendrogram: junction, exon and gene levels (clusterlogfc module)
+* added *first_exon* annotation for junctions touching annotated first exons of transcripts
+* extended documentation of concepts, analysis and results
+</details>
+
+<details>
+<summary><b>v0.2</b>: released in October 2022 (click to show details)</summary>
+
+* software architecture restructure with python modules
+* filtering of lowly expressed features by edgeR
+* DonJuan analysis (junction-anchor analysis)
+* more advanced motif analysis with DREME
+* filtering regulated junctions with regulated donors
+</details>
+
+<details>
+<summary><b>v0.1</b>: released in July 2022 (click to show details)</summary>
+
+* initial version of splicekit
+* parsing of junction and exon counts
+* computing edgeR analysis from count tables and producing a results file with direct links to JBrowse2
+* basic motif analysis
+</details>
```

### Comparing `splicekit-0.4.2/README.md` & `splicekit-0.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,82 +1,43 @@
 # splicekit
 
-A comprehensive platform for splicing analysis of RNA-seq short-read sequencing data. <b>splicekit</b> input are read alignments in .bam format (look at [datasets](datasets) for details on how to run examples).
+A comprehensive platform for splicing analysis of RNA-seq short-read sequencing data. <b>splicekit</b> input are read alignments in BAM format (look at [datasets](datasets) for details on how to run examples).
 
-[What does splicekit do?](#what_do)<br>
-[Changelog](#changelog)<br>
-[Quick start and installation](#initial_setup)<br>
-[Running Splicekit](#running_splicekit)<br>
+[What is splicekit?](#what_do)<br>
+[Installation and quick start](#initial_setup)<br>
+[Running splicekit](#running_splicekit)<br>
 &nbsp;&nbsp;[Annotation and comparisons](#annot_comp)<br>
 &nbsp;&nbsp;[Preparing feature (genes, exon, junction, anchor) data tables](#make_tables)<br>
 &nbsp;&nbsp;[Running edgeR gene context analysis on junction features](#id_features)<br>
 [Motif analysis](#motif)<br>
 [Scanning for RNA-protein binding with scanRBP](#scanRBP)<br>
 [juDGE plots](#judgeplot)<br>
-[Jbrowse2 visualizations](#jbrowse)<br>
+[JBrowse2 visualizations](#jbrowse)<br>
 [Documentation and specifications](#filedescriptors)<br>
+[Changelog](#changelog)<br>
 
 <b>splicekit</b> is a modular platform for splicing analysis of RNA-seq datasets. The platform also integrates an JBrowse2 instance together with [pybio](https://github.com/grexor/pybio) for genomic operations and [scanRBP](https://github.com/grexor/scanRBP) for RNA-protein binding studies. The whole analysis is self-contained (one single folder) and the platform is written in Python, in a modular way.
 
-## What does splicekit do?<a name="what_do"></a>
-From an initial setup (`splicekit.config`) and sample annotation (`samples.tab`), splicekit generates comparisons (which samples to compare to which controls). Next, feature count tables are generated (exons, anchors, junctions, genes) based on defined comparisons. Analyses incude edgeR altsplice (differentially used features), motif analysis with DonJuan (junction-anchor) and DREME, RNA-protein binding enrichment analysis with scanRBP and clustering analysis on expression of features. To facilitate result and data interpretation, splicekit also provides an instance of JBrowse2.
-
-## Changelog<a name="changelog"></a>
-
-**v0.4**: released in May 2023
-* added singularity container with all dependencies
-* added local integrated JBrowse2
-* cluster or desktop runs
-* scanRBP and bootstrap analysis of RNA-protein binding
-* further development and integration with pybio
-* extended documentation of concepts, analysis and results
-
-<details>
-<summary><b>v0.3</b>: released in January 2023 (click to show details)</summary>
-
-* re-coded junction analysis
-  * independent junctions parsing from provided bam files
-  * master table of all junctions in the samples of the analyzed project, including novel junctions (refseq/ensembl non-annotated)
-* clustering by logFC of pairwise-comparisons with dendrogram: junction, exon and gene levels (clusterlogfc module)
-* added *first_exon* annotation for junctions touching annotated first exons of transcripts
-* extended documentation of concepts, analysis and results
-</details>
-
-<details>
-<summary><b>v0.2</b>: released in October 2022 (click to show details)</summary>
-
-* software architecture restructure with python modules
-* filtering of lowly expressed features by edgeR
-* DonJuan analysis (junction-anchor analysis)
-* more advanced motif analysis with DREME
-* filtering regulated junctions with regulated donors
-</details>
-
-<details>
-<summary><b>v0.1</b>: released in July 2022 (click to show details)</summary>
+## What is splicekit?<a name="what_do"></a>
+From an initial config file (`splicekit.config`), sample annotation (`samples.tab`) and aligned reads in BAM format, splicekit first defines comparisons (which test samples to compare to which controls). Next, feature count tables are generated (exons, anchors, junctions, genes) based on defined comparisons. Analysis incude edgeR alt-splice (differentially used features), motif analysis with DonJuAn (junction-anchor) and DREME, RNA-protein binding enrichment analysis with scanRBP and clustering analysis on expression of features. To facilitate result and data interpretation, splicekit also provides an instance of JBrowse2.
 
-* initial version of splicekit
-* parsing of junction and exon counts
-* computing edgeR analysis from count tables and producing a results file with direct links to JBrowse2
-* basic motif analysis
-</details>
-
-## Quick start and installation<a name="initial_setup"></a>
+## Installation and quick start<a name="initial_setup"></a>
 
 The easiest way to install splicekit is to simply run:
 
 `$ pip install splicekit`
 
+Note that on some systems, pip is installing the executable scripts under `~/.local/bin`. However this folder is not in the PATH which will result in `command not found` if you try to run `$ splicekit` on the command line. To fix this, please execute `export PATH="$PATH:~/.local/bin"` (and add this to your `.profile`). Another suggestion is to install inside a virtual environment (using `virtualenv`).
+
 If you would like to install splicekit directly from this repository, clone the repository into a folder, for example `~/software/splicekit`. Add the `~/software/splicekit` folder to $PYTHONPATH (`export PYTHONPATH=$PYTHONPATH:~/software/splicekit`).
 
 ### Software dependencies
 
 splicekit uses several third-party open-source software. If you don't have the software installed on your system, we prepared a [singularity definition file](singularity), where you can also directly see all dependencies. Using the singularity image, you don't need to install the dependencies yourself, you just need to install singularity.
 
-
 ### Example runs and datasets
 
 Example runs can be found in the [datasets](datasets) folder.
 
 ### Configuration file documentation
 
 <details>
@@ -119,20 +80,14 @@
 Processing parameters:
 
 | Parameter | Description | Default / Example |
 |-|-|-|
 | platform | "desktop" or "cluster" (HPC with SLURM) | "desktop"
 | container | leave empty or for singularity use: "singularity"; this will download and run "singularity/splicekit_version.sif" | "desktop"
 
-JBrowse2 parameters:
-
-| Parameter | Description | Default / Example |
-|-|-|-|
-| jbrowse2_url | URL of the local JBrowse2 instance | "localhost/jbrowse2"
-
 Visualization, labelling and other parameters:
 
 | Parameter | Description | Default / Example |
 |-|-|-|
 | short_names | List of triples for shortening names in results, if last string is "complete", only entire strings will be considered (no partial replacement) | [], example: [("cell_line_A", "A", "complete")], this would only replace cell_line_A with A if cell_line_A is the whole string, while if "partial" is provided, also strings like ...cell_line_A... would be replaced with ...A... | ("original name", "short name", "complete")
 
 </details>
@@ -378,7 +333,47 @@
 **Exon** specific (additional) columns:
 
 | column | description |
 |-|-|
 | delta_PSI | test_PSI-control_PSI, percentage spliced-in |
 
 </details>
+
+## Changelog<a name="changelog"></a>
+
+**v0.4**: released in May 2023
+* added singularity container with all dependencies
+* added local integrated JBrowse2
+* cluster or desktop runs
+* scanRBP and bootstrap analysis of RNA-protein binding
+* further development and integration with pybio
+* extended documentation of concepts, analysis and results
+
+<details>
+<summary><b>v0.3</b>: released in January 2023 (click to show details)</summary>
+
+* re-coded junction analysis
+  * independent junctions parsing from provided bam files
+  * master table of all junctions in the samples of the analyzed project, including novel junctions (refseq/ensembl non-annotated)
+* clustering by logFC of pairwise-comparisons with dendrogram: junction, exon and gene levels (clusterlogfc module)
+* added *first_exon* annotation for junctions touching annotated first exons of transcripts
+* extended documentation of concepts, analysis and results
+</details>
+
+<details>
+<summary><b>v0.2</b>: released in October 2022 (click to show details)</summary>
+
+* software architecture restructure with python modules
+* filtering of lowly expressed features by edgeR
+* DonJuan analysis (junction-anchor analysis)
+* more advanced motif analysis with DREME
+* filtering regulated junctions with regulated donors
+</details>
+
+<details>
+<summary><b>v0.1</b>: released in July 2022 (click to show details)</summary>
+
+* initial version of splicekit
+* parsing of junction and exon counts
+* computing edgeR analysis from count tables and producing a results file with direct links to JBrowse2
+* basic motif analysis
+</details>
```

### Comparing `splicekit-0.4.2/setup.py` & `splicekit-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/__init__.py` & `splicekit-0.4.3/splicekit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,20 +223,21 @@
 
 def judge_process():
     splicekit.judge.process()
 
 def clusterlogfc_process():
     splicekit.clusterlogfc.process()
 
-def jbrowse2_create(force_samples=False, force_annotation=False):
-    splicekit.core.jbrowse2_create.process(force_samples,force_annotation)
+def jbrowse2_process(force_samples=False, force_annotation=False):
+    splicekit.core.jbrowse2_create.process(force_samples, force_annotation)
 
-def process():
+def process(force=False):
     setup()
     annotation()
     features()
     edgeR()
     juan()
     motifs()
     promisc()
     judge_process()
     clusterlogfc_process()
+    jbrowse2_process(force_samples=force, force_annotation=force)
```

### Comparing `splicekit-0.4.2/splicekit/clusterlogfc/__init__.py` & `splicekit-0.4.3/splicekit/clusterlogfc/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/config/__init__.py` & `splicekit-0.4.3/splicekit/config/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 import socket
 
 if os.path.exists("splicekit.config"):
     config_lines = open("splicekit.config").readlines()
     for cline in config_lines:
         exec(cline.replace("\r", "").replace("\n", ""))
 
-# JBrowse2 URL
+jbrowse2_url = ""
 
-if jbrowse2_url == "":
+def jbrowse2_config(hostname):
+    global jbrowse2_url
+    # JBrowse2 URL
     port = jbrowse2.port
-    hostname=socket.gethostname()
+    if hostname==None: # get hostname?
+        hostname=socket.gethostname()
     ip_addr=socket.gethostbyname(hostname)
     jbrowse2_url = f"http://{ip_addr}:{port}/jbrowse2/?config=splicekit_data/config.json"
 
-cwd = os.getcwd()
+jbrowse2_config(None)
 
 # read in location of gtf and fasta files
 temp = os.popen(f"pybio path {species}").read()
 temp = temp.split("\n")
 for line in temp:
     if line.endswith(".fasta"):
         fasta_path = line
```

### Comparing `splicekit-0.4.2/splicekit/core/anchors.py` & `splicekit-0.4.3/splicekit/core/anchors.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/core/annotation.py` & `splicekit-0.4.3/splicekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/core/delta_dar.py` & `splicekit-0.4.3/splicekit/core/delta_dar.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/core/exons.py` & `splicekit-0.4.3/splicekit/core/exons.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/core/features.py` & `splicekit-0.4.3/splicekit/core/features.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/core/genes.py` & `splicekit-0.4.3/splicekit/core/genes.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/core/jbrowse2.py` & `splicekit-0.4.3/splicekit/core/jbrowse2.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import http.server
 import socket
 import socketserver
 import RangeHTTPServer
 
 port = 8007
 
-def process():
+def start():
     setup()
     server()
 
 def server():
     hostname=socket.gethostname()
     ip_addr=socket.gethostbyname(hostname)
     Handler = RangeHTTPServer.RangeRequestHandler
```

### Comparing `splicekit-0.4.2/splicekit/core/jbrowse2_create.py` & `splicekit-0.4.3/splicekit/core/jbrowse2_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,16 +90,17 @@
         os.system('mkdir jbrowse2/splicekit_data') # first create folder to put everything inside
 
     # initialize config.json with adding fasta file --------------------------------------------------------------------------------------------------------------------------------------
     if (not os.path.exists('jbrowse2/splicekit_data/config.json')) or (force_annotation==True):
         
         # clean up previous jobs
         os.system(f'rm -r jbrowse2/splicekit_data/*')
-        os.system(f'rm logs/logs_jbrowse/{sample}.out')
-        os.system(f'rm logs/logs_jbrowse/{sample}.err')
+        for sample in bam_files:
+            os.system(f'rm logs/logs_jbrowse/{sample}.out')
+            os.system(f'rm logs/logs_jbrowse/{sample}.err')
 
         print('[jbrowse] creating config.json in jbrowse2/splicekit_data')
 
         if os.path.isabs(genome_fa): # check if genome_fa path is absolute or relative
             os.system(f'cd jbrowse2/splicekit_data; {container} jbrowse add-assembly {genome_fa} --name GenomeSequence --load symlink') # initialize config.json with genome sequence
         else:
             os.system(f'cd jbrowse2/splicekit_data; {container} jbrowse add-assembly ../../{genome_fa} --name GenomeSequence --load symlink') # initialize config.json with genome sequence
@@ -138,15 +139,15 @@
 def process(force_samples=False, force_annotation=False):
     #os.system(f'rm -r jbrowse2/splicekit_data/*') # clean up before starting
     check_genome()
     # clean up previous jobs
     os.system(f'rm -r jobs/jobs_jbrowse/*')
     write_sample_jobs(force_samples) # if force_samples is True, then jobs are created
     # run  sample jobs if available
-    if force_samples:
+    if (not os.path.exists('jbrowse2/splicekit_data/config.json')) or (force_samples):
         if splicekit.config.platform=="cluster":
             os.system('export BSUB_QUIET=Y; jobs=( $(ls jobs/jobs_jbrowse/*.job) ); g=10; for((i=0; i < ${#jobs[@]}; i+=g)); do part=( "${jobs[@]:i:g}" ); for job_fname in ${part[*]}; do echo "[jbrowse] submitted $job_fname"; bsub -K < ${job_fname} & done; wait; echo "[jbrowse] processing next 10"; done; echo "[jbrowse] processing complete"')
         if splicekit.config.platform=="desktop":
             os.system("source jobs/jobs_jbrowse/process.sh")
     create_jbrowse_config(force_annotation)
```

### Comparing `splicekit-0.4.2/splicekit/core/juan.py` & `splicekit-0.4.3/splicekit/core/juan.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/core/junctions.py` & `splicekit-0.4.3/splicekit/core/junctions.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/core/motifs.py` & `splicekit-0.4.3/splicekit/core/motifs.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/core/patterns.py` & `splicekit-0.4.3/splicekit/core/patterns.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/core/promisc.py` & `splicekit-0.4.3/splicekit/core/promisc.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/core/report.py` & `splicekit-0.4.3/splicekit/core/report.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/judge/__init__.py` & `splicekit-0.4.3/splicekit/judge/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/splicecompare` & `splicekit-0.4.3/splicekit/splicecompare`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.2/splicekit/splicekit` & `splicekit-0.4.3/splicekit/splicekit`

 * *Files 7% similar despite different names*

```diff
@@ -22,16 +22,21 @@
      promisc           promiscuity analysis: genes and their junctions changes across conditions
      clusterlogfc      log fold-change clusters of significant changes (FDR<0.05) on junction, exon, gene level
 
   -- scanRBP, motif and sequence analyses
      motifs            run motif and scanRBP analysis
 
   -- JBrowse2 genomic browser
-     jbrowse2          creates all required JBrowse2 files and starts JBrowse2 web server
-     
+     jbrowse2 [process | start] processes (creates) all required JBrowse2 files and/or starts JBrowse2 web server
+
+Options
+
+  -- hostname
+     If you are submitting 'splicekit process' to the cluster, you can provide a custom hostname. This will be used to create JBrowse2 URLs.
+
 """
 
 help_edgeR = """
 Usage: splicekit edgeR [sub-command]
 
 Sub-commands:
      junctions      run edgeR on junctions table data
@@ -42,15 +47,16 @@
 If no sub-command is given, all analyses will be run (junctions, exons, anchors, genes).
 """
 
 parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter, add_help=False)
 parser.add_argument('command', help="command(s) to run", nargs='*')
 parser.add_argument("-help", "-h", "--help", action="store_true")
 parser.add_argument("-version", "--version", help="Print version", action="store_true")
-parser.add_argument("-force", "--force", help="Force recreation / overwrite of results", action="store_true")
+parser.add_argument("-force", "--force", help="Force recreation / overwrite of results", action="store_true", default=False)
+parser.add_argument("-hostname", "--hostname", help="If you are submitting 'splicekit process' to the cluster, you can provide a custom hostname. This will be used to create JBrowse2 URLs.", default=None)
 args = parser.parse_args()
 
 # lookup version without loading splicekit
 import importlib
 splicekit_init = importlib.util.find_spec("splicekit")
 splicekit_path = splicekit_init.origin
 splicekit_folder = os.path.dirname(splicekit_path)
@@ -70,14 +76,16 @@
     print()
     print("[splicekit] Please specify an action to perform or specify --help to get help on available actions. Running 'splicekit process' will perform all available analyses.")
     sys.exit(0)
 
 # loading splicekit modules takes time, only load if the user is not asking to display help
 if not args.help:
     import splicekit
+    if args.hostname!=None:
+        splicekit.config.jbrowse2_config(args.hostname)
 
 if args.command[0]=="basic":
     splicekit.setup()
     splicekit.annotation()
     splicekit.features()
     splicekit.edgeR()
 elif args.command[0]=="setup":
@@ -115,24 +123,23 @@
 elif args.command[0]=="cassettes":
     splicekit.cassettes()
 elif args.command[0]=="patterns":
     splicekit.patterns()
 elif args.command[0]=="clusterlogfc":
     splicekit.clusterlogfc_process()
 elif args.command[0]=="process":
-    splicekit.process()
+    splicekit.process(force=args.force)
 elif args.command[0]=="judge":
     splicekit.judge_process()
 elif args.command[0]=="juan":
     splicekit.juan()
-elif args.command [0] == "jbrowse2":
-    force_samples=False; force_annotation = False
-    if len(args.command)>1 and args.command[1] == 'samples':
-        force_samples=args.force
-    if len(args.command)>1 and args.command[1] == 'annotation':
-        force_annotation=args.force
-    if len(args.command)==1:
-        force_annotation = args.force; force_samples = args.force
-    splicekit.jbrowse2_create(force_samples=force_samples,force_annotation=force_annotation)
-    splicekit.core.jbrowse2.process()
+elif args.command[0] == "jbrowse2":
+    if len(args.command)>1:
+        if args.command[1]=="process":
+            splicekit.jbrowse2_process(force_samples=args.force, force_annotation=args.force)
+        if args.command[1]=="start":
+            splicekit.core.jbrowse2.start()
+    else:
+        splicekit.jbrowse2_process(force_samples=args.force, force_annotation=args.force)
+        splicekit.core.jbrowse2.start()
 else:
     print(help_0)
```

### Comparing `splicekit-0.4.2/splicekit/splicekit.config.template` & `splicekit-0.4.3/splicekit/splicekit.config.template`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 library_type = "paired-end" # ["paired-end", "single-end"]
 library_strand = "NONE" # ["SECOND_READ_TRANSCRIPTION_STRAND", "FIRST_READ_TRANSCRIPTION_STRAND", "SINGLE_STRAND", "SINGLE_REVERSE", "NONE"] "{{ cookiecutter.rna_library_strand }}" 
 
 # edgeR results filtering
 edgeR_FDR_thr = 0.05
 
 # sample annotation (read from samples.tab)
-sample_column = "readout_id" # where are sample ids stored; we expect bam names: sample_id1.bam, sample_id2.bam, ...
-treatment_column = "compound_name"
+sample_column = "sample_id" # where are sample ids stored; we expect bam names: sample_id1.bam, sample_id2.bam, ...
+treatment_column = "treatment_id"
 control_name = "DMSO" # name of controls in the treatment_column, other samples are compared to these marked controls
 separate_column = "" # separate comparisons by grouping samples on separate_column? if "", do not separate
 group_column = "" # only include DMSOs in the same range as compounds (compound replicates on plate1,plate2,plate3? only include DMSO from plate1,plate2,plate3)
 
 # genome
 species = "homo_sapiens"
 genome_version = None # pybio genome version, leave None to take latest Ensembl version
@@ -26,10 +26,7 @@
 scanRBP = False # run scanRBP? (False / True)
 protein = "K562.TARDBP.0"
 protein_label = "tdp43" # used in file names and titles
 
 # platform and container
 platform = "desktop" # "desktop" or "cluster" (HPC with SLURM)
 container = "" # leave empty or for singularity use: "singularity run /my_path/splicekit.sif"
-
-# JBrowse2
-jbrowse2_url = ""
```

### Comparing `splicekit-0.4.2/splicekit.egg-info/PKG-INFO` & `splicekit-0.4.3/splicekit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,92 +1,53 @@
 Metadata-Version: 2.1
 Name: splicekit
-Version: 0.4.2
+Version: 0.4.3
 Summary: splicekit: comprehensive toolkit for splicing analysis from short-read RNA-seq
 Home-page: https://github.com/bedapub/splicekit
 Author: Roche, PMDA Spliceosome team
 Author-email: gregor.rot@gmail.com
 Keywords: splicekit,splicing,transcriptomics,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 
-A comprehensive platform for splicing analysis of RNA-seq short-read sequencing data. <b>splicekit</b> input are read alignments in .bam format (look at [datasets](datasets) for details on how to run examples).
+A comprehensive platform for splicing analysis of RNA-seq short-read sequencing data. <b>splicekit</b> input are read alignments in BAM format (look at [datasets](datasets) for details on how to run examples).
 
-[What does splicekit do?](#what_do)<br>
-[Changelog](#changelog)<br>
-[Quick start and installation](#initial_setup)<br>
-[Running Splicekit](#running_splicekit)<br>
+[What is splicekit?](#what_do)<br>
+[Installation and quick start](#initial_setup)<br>
+[Running splicekit](#running_splicekit)<br>
 &nbsp;&nbsp;[Annotation and comparisons](#annot_comp)<br>
 &nbsp;&nbsp;[Preparing feature (genes, exon, junction, anchor) data tables](#make_tables)<br>
 &nbsp;&nbsp;[Running edgeR gene context analysis on junction features](#id_features)<br>
 [Motif analysis](#motif)<br>
 [Scanning for RNA-protein binding with scanRBP](#scanRBP)<br>
 [juDGE plots](#judgeplot)<br>
-[Jbrowse2 visualizations](#jbrowse)<br>
+[JBrowse2 visualizations](#jbrowse)<br>
 [Documentation and specifications](#filedescriptors)<br>
+[Changelog](#changelog)<br>
 
 <b>splicekit</b> is a modular platform for splicing analysis of RNA-seq datasets. The platform also integrates an JBrowse2 instance together with [pybio](https://github.com/grexor/pybio) for genomic operations and [scanRBP](https://github.com/grexor/scanRBP) for RNA-protein binding studies. The whole analysis is self-contained (one single folder) and the platform is written in Python, in a modular way.
 
-## What does splicekit do?<a name="what_do"></a>
-From an initial setup (`splicekit.config`) and sample annotation (`samples.tab`), splicekit generates comparisons (which samples to compare to which controls). Next, feature count tables are generated (exons, anchors, junctions, genes) based on defined comparisons. Analyses incude edgeR altsplice (differentially used features), motif analysis with DonJuan (junction-anchor) and DREME, RNA-protein binding enrichment analysis with scanRBP and clustering analysis on expression of features. To facilitate result and data interpretation, splicekit also provides an instance of JBrowse2.
-
-## Changelog<a name="changelog"></a>
-
-**v0.4**: released in May 2023
-* added singularity container with all dependencies
-* added local integrated JBrowse2
-* cluster or desktop runs
-* scanRBP and bootstrap analysis of RNA-protein binding
-* further development and integration with pybio
-* extended documentation of concepts, analysis and results
-
-<details>
-<summary><b>v0.3</b>: released in January 2023 (click to show details)</summary>
-
-* re-coded junction analysis
-  * independent junctions parsing from provided bam files
-  * master table of all junctions in the samples of the analyzed project, including novel junctions (refseq/ensembl non-annotated)
-* clustering by logFC of pairwise-comparisons with dendrogram: junction, exon and gene levels (clusterlogfc module)
-* added *first_exon* annotation for junctions touching annotated first exons of transcripts
-* extended documentation of concepts, analysis and results
-</details>
-
-<details>
-<summary><b>v0.2</b>: released in October 2022 (click to show details)</summary>
-
-* software architecture restructure with python modules
-* filtering of lowly expressed features by edgeR
-* DonJuan analysis (junction-anchor analysis)
-* more advanced motif analysis with DREME
-* filtering regulated junctions with regulated donors
-</details>
-
-<details>
-<summary><b>v0.1</b>: released in July 2022 (click to show details)</summary>
+## What is splicekit?<a name="what_do"></a>
+From an initial config file (`splicekit.config`), sample annotation (`samples.tab`) and aligned reads in BAM format, splicekit first defines comparisons (which test samples to compare to which controls). Next, feature count tables are generated (exons, anchors, junctions, genes) based on defined comparisons. Analysis incude edgeR alt-splice (differentially used features), motif analysis with DonJuAn (junction-anchor) and DREME, RNA-protein binding enrichment analysis with scanRBP and clustering analysis on expression of features. To facilitate result and data interpretation, splicekit also provides an instance of JBrowse2.
 
-* initial version of splicekit
-* parsing of junction and exon counts
-* computing edgeR analysis from count tables and producing a results file with direct links to JBrowse2
-* basic motif analysis
-</details>
-
-## Quick start and installation<a name="initial_setup"></a>
+## Installation and quick start<a name="initial_setup"></a>
 
 The easiest way to install splicekit is to simply run:
 
 `$ pip install splicekit`
 
+Note that on some systems, pip is installing the executable scripts under `~/.local/bin`. However this folder is not in the PATH which will result in `command not found` if you try to run `$ splicekit` on the command line. To fix this, please execute `export PATH="$PATH:~/.local/bin"` (and add this to your `.profile`). Another suggestion is to install inside a virtual environment (using `virtualenv`).
+
 If you would like to install splicekit directly from this repository, clone the repository into a folder, for example `~/software/splicekit`. Add the `~/software/splicekit` folder to $PYTHONPATH (`export PYTHONPATH=$PYTHONPATH:~/software/splicekit`).
 
 ### Software dependencies
 
 splicekit uses several third-party open-source software. If you don't have the software installed on your system, we prepared a [singularity definition file](singularity), where you can also directly see all dependencies. Using the singularity image, you don't need to install the dependencies yourself, you just need to install singularity.
 
-
 ### Example runs and datasets
 
 Example runs can be found in the [datasets](datasets) folder.
 
 ### Configuration file documentation
 
 <details>
@@ -129,20 +90,14 @@
 Processing parameters:
 
 | Parameter | Description | Default / Example |
 |-|-|-|
 | platform | "desktop" or "cluster" (HPC with SLURM) | "desktop"
 | container | leave empty or for singularity use: "singularity"; this will download and run "singularity/splicekit_version.sif" | "desktop"
 
-JBrowse2 parameters:
-
-| Parameter | Description | Default / Example |
-|-|-|-|
-| jbrowse2_url | URL of the local JBrowse2 instance | "localhost/jbrowse2"
-
 Visualization, labelling and other parameters:
 
 | Parameter | Description | Default / Example |
 |-|-|-|
 | short_names | List of triples for shortening names in results, if last string is "complete", only entire strings will be considered (no partial replacement) | [], example: [("cell_line_A", "A", "complete")], this would only replace cell_line_A with A if cell_line_A is the whole string, while if "partial" is provided, also strings like ...cell_line_A... would be replaced with ...A... | ("original name", "short name", "complete")
 
 </details>
@@ -388,7 +343,47 @@
 **Exon** specific (additional) columns:
 
 | column | description |
 |-|-|
 | delta_PSI | test_PSI-control_PSI, percentage spliced-in |
 
 </details>
+
+## Changelog<a name="changelog"></a>
+
+**v0.4**: released in May 2023
+* added singularity container with all dependencies
+* added local integrated JBrowse2
+* cluster or desktop runs
+* scanRBP and bootstrap analysis of RNA-protein binding
+* further development and integration with pybio
+* extended documentation of concepts, analysis and results
+
+<details>
+<summary><b>v0.3</b>: released in January 2023 (click to show details)</summary>
+
+* re-coded junction analysis
+  * independent junctions parsing from provided bam files
+  * master table of all junctions in the samples of the analyzed project, including novel junctions (refseq/ensembl non-annotated)
+* clustering by logFC of pairwise-comparisons with dendrogram: junction, exon and gene levels (clusterlogfc module)
+* added *first_exon* annotation for junctions touching annotated first exons of transcripts
+* extended documentation of concepts, analysis and results
+</details>
+
+<details>
+<summary><b>v0.2</b>: released in October 2022 (click to show details)</summary>
+
+* software architecture restructure with python modules
+* filtering of lowly expressed features by edgeR
+* DonJuan analysis (junction-anchor analysis)
+* more advanced motif analysis with DREME
+* filtering regulated junctions with regulated donors
+</details>
+
+<details>
+<summary><b>v0.1</b>: released in July 2022 (click to show details)</summary>
+
+* initial version of splicekit
+* parsing of junction and exon counts
+* computing edgeR analysis from count tables and producing a results file with direct links to JBrowse2
+* basic motif analysis
+</details>
```

### Comparing `splicekit-0.4.2/splicekit.egg-info/SOURCES.txt` & `splicekit-0.4.3/splicekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

