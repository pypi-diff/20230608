# Comparing `tmp/galaxy-config-22.1.1.tar.gz` & `tmp/galaxy-config-23.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-config-22.1.1.tar", last modified: Mon Aug 22 19:45:41 2022, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/config/dist/.tmp-1tn8a__p/galaxy-config-23.0.1.tar", last modified: Thu Jun  8 17:38:11 2023, max compression
```

## Comparing `galaxy-config-22.1.1.tar` & `galaxy-config-23.0.1.tar`

### file list

```diff
@@ -1,279 +1,65 @@
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.807995 galaxy-config-22.1.1/
--rw-r--r--   0 mvandenb   (501) staff       (20)      119 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)    11109 2021-09-10 08:52:38.000000 galaxy-config-22.1.1/LICENSE
--rw-r--r--   0 mvandenb   (501) staff       (20)      103 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) staff       (20)     2954 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/Makefile
--rw-r--r--   0 mvandenb   (501) staff       (20)     1428 2022-08-22 19:45:41.808109 galaxy-config-22.1.1/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      294 2022-08-18 15:49:03.000000 galaxy-config-22.1.1/README.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)       89 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.744881 galaxy-config-22.1.1/galaxy/
--rw-r--r--   0 mvandenb   (501) staff       (20)       91 2022-08-18 15:49:03.000000 galaxy-config-22.1.1/galaxy/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.746051 galaxy-config-22.1.1/galaxy/config/
--rw-r--r--   0 mvandenb   (501) staff       (20)    58936 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    31462 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/config_manage.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.755773 galaxy-config-22.1.1/galaxy/config/sample/
--rw-r--r--   0 mvandenb   (501) staff       (20)     6301 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/sample/auth_conf.xml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     1080 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/build_sites.yml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     3367 2022-08-18 15:49:02.000000 galaxy-config-22.1.1/galaxy/config/sample/container_resolvers_conf.xml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)    13084 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/sample/containers_conf.yml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)       55 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/data_manager_conf.xml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)   108626 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/sample/datatypes_conf.xml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)      412 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/disposable_email_blocklist.conf.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     2555 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/environment_modules_mapping.yml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     4121 2022-08-18 15:49:02.000000 galaxy-config-22.1.1/galaxy/config/sample/error_report.yml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     4796 2022-08-18 15:49:02.000000 galaxy-config-22.1.1/galaxy/config/sample/file_sources_conf.yml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)   113165 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/sample/galaxy.yml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)      739 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/sample/galaxy_vscode.ini
--rw-r--r--   0 mvandenb   (501) staff       (20)    75288 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/sample/job_conf.xml.sample_advanced
--rw-r--r--   0 mvandenb   (501) staff       (20)      408 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/job_conf.xml.sample_basic
--rw-r--r--   0 mvandenb   (501) staff       (20)     7398 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/job_metrics_conf.xml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)      698 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/job_resource_params_conf.xml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     1950 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/lmod_modules_mapping.yml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)      262 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/local_conda_mapping.yml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     8831 2022-08-18 15:49:02.000000 galaxy-config-22.1.1/galaxy/config/sample/object_store_conf.xml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     9944 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/sample/oidc_backends_config.xml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     1199 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/oidc_config.xml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     5060 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/sample/reports.yml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     6571 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/sample/tool_conf.xml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     8084 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/sample/tool_data_table_conf.xml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     9732 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/tool_destinations.yml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     1790 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/tool_recommendations_overwrite.yml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)    18068 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/sample/tool_shed.yml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)      288 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/tool_sheds_conf.xml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)      784 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/trs_servers_conf.yml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     3210 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/user_preferences_extra_conf.yml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)      334 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/workflow_resource_mapper_conf.yml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     1136 2022-03-24 19:47:10.000000 galaxy-config-22.1.1/galaxy/config/sample/workflow_resource_params_conf.xml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     1878 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/sample/workflow_schedulers_conf.xml.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     3970 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/schema.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.757309 galaxy-config-22.1.1/galaxy/config/schemas/
--rw-r--r--   0 mvandenb   (501) staff       (20)   138257 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/schemas/config_schema.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)     2765 2022-08-18 15:49:02.000000 galaxy-config-22.1.1/galaxy/config/schemas/job_config_schema.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)     2529 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/schemas/reports_config_schema.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)    20993 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/schemas/tool_shed_config_schema.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)   113171 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/schemas/uwsgi_schema.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)     7153 2022-08-22 19:45:27.000000 galaxy-config-22.1.1/galaxy/config/script.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      409 2022-08-22 19:45:29.000000 galaxy-config-22.1.1/galaxy/project_galaxy_config.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.759294 galaxy-config-22.1.1/galaxy_config.egg-info/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1428 2022-08-22 19:45:41.000000 galaxy-config-22.1.1/galaxy_config.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)     7632 2022-08-22 19:45:41.000000 galaxy-config-22.1.1/galaxy_config.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:41.000000 galaxy-config-22.1.1/galaxy_config.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       75 2022-08-22 19:45:41.000000 galaxy-config-22.1.1/galaxy_config.egg-info/entry_points.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:41.000000 galaxy-config-22.1.1/galaxy_config.egg-info/not-zip-safe
--rw-r--r--   0 mvandenb   (501) staff       (20)       52 2022-08-22 19:45:41.000000 galaxy-config-22.1.1/galaxy_config.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-08-22 19:45:41.000000 galaxy-config-22.1.1/galaxy_config.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       52 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.760071 galaxy-config-22.1.1/scripts/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1442 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/scripts/commit_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2166 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/scripts/new_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      804 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/scripts/print_version_for_release.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    33060 2022-08-22 19:45:41.813799 galaxy-config-22.1.1/setup.cfg
--rw-r--r--   0 mvandenb   (501) staff       (20)     2868 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/setup.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.798441 galaxy-config-22.1.1/test-data/
--rw-r--r--   0 mvandenb   (501) staff       (20)       59 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/1.RData
--rw-r--r--   0 mvandenb   (501) staff       (20)    29710 2020-02-19 09:47:53.000000 galaxy-config-22.1.1/test-data/1.axt
--rw-r--r--   0 mvandenb   (501) staff       (20)     3592 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/1.bam
--rw-r--r--   0 mvandenb   (501) staff       (20)     4202 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/1.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)     4202 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/1.bed.spaces
--rw-r--r--   0 mvandenb   (501) staff       (20)      566 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/1.bedgraph
--rw-r--r--   0 mvandenb   (501) staff       (20)   154328 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/1.bigbed
--rw-r--r--   0 mvandenb   (501) staff       (20)    21218 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/1.bigwig
--rw-r--r--   0 mvandenb   (501) staff       (20)     9641 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/1.csv
--rw-r--r--   0 mvandenb   (501) staff       (20)      265 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/1.customtrack
--rw-r--r--   0 mvandenb   (501) staff       (20)    21625 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/1.fasta
--rw-r--r--   0 mvandenb   (501) staff       (20)     7012 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/1.fasta.gz
--rw-r--r--   0 mvandenb   (501) staff       (20)      418 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/1.fastq
--rw-r--r--   0 mvandenb   (501) staff       (20)      178 2022-03-24 19:46:45.000000 galaxy-config-22.1.1/test-data/1.fastqsanger
--rw-r--r--   0 mvandenb   (501) staff       (20)      155 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/1.fastqsanger.bz2
--rw-r--r--   0 mvandenb   (501) staff       (20)      161 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/1.fastqsanger.gz
--rw-r--r--   0 mvandenb   (501) staff       (20)      419 2022-03-24 19:46:45.000000 galaxy-config-22.1.1/test-data/1.fastqsolexa
--rw-r--r--   0 mvandenb   (501) staff       (20)      234 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/1.interval
--rw-r--r--   0 mvandenb   (501) staff       (20)     2757 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/1.lav
--rw-r--r--   0 mvandenb   (501) staff       (20)    21086 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/1.pileup
--rw-r--r--   0 mvandenb   (501) staff       (20)     3444 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/1.sam
--rw-r--r--   0 mvandenb   (501) staff       (20)     1249 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/1.sam.gz
--rwxr-xr-x   0 mvandenb   (501) staff       (20)   139484 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/1.scf
--rw-r--r--   0 mvandenb   (501) staff       (20)      100 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/1.sff
--rw-r--r--   0 mvandenb   (501) staff       (20)       99 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/1.tabular
--rw-r--r--   0 mvandenb   (501) staff       (20)    19378 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/1.tiff
--rw-r--r--   0 mvandenb   (501) staff       (20)      208 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/1.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)      273 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/1.wig
--rw-r--r--   0 mvandenb   (501) staff       (20)     1441 2022-08-18 15:49:03.000000 galaxy-config-22.1.1/test-data/1.yaml
--rw-r--r--   0 mvandenb   (501) staff       (20)       24 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/11.tabular
--rw-r--r--   0 mvandenb   (501) staff       (20)     4272 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/2.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)    54312 2022-08-18 15:49:03.000000 galaxy-config-22.1.1/test-data/2.cram
--rw-r--r--   0 mvandenb   (501) staff       (20)      671 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/2.fasta
--rw-r--r--   0 mvandenb   (501) staff       (20)       93 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/2.tabular
--rw-r--r--   0 mvandenb   (501) staff       (20)      181 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/2gen.fastq
--rw-r--r--   0 mvandenb   (501) staff       (20)     1655 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/3.bam
--rw-r--r--   0 mvandenb   (501) staff       (20)     4696 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/3.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)    10929 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/3.maf
--rw-r--r--   0 mvandenb   (501) staff       (20)     1666 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/3unsorted.bam
--rw-r--r--   0 mvandenb   (501) staff       (20)       61 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/4.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)       92 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/4.bed.bz2
--rw-r--r--   0 mvandenb   (501) staff       (20)       80 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/4.bed.gz
--rw-r--r--   0 mvandenb   (501) staff       (20)      198 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/4.bed.zip
--rw-r--r--   0 mvandenb   (501) staff       (20)    10123 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/454Score.pdf
--rw-r--r--   0 mvandenb   (501) staff       (20)     4392 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/454Score.png
--rw-r--r--   0 mvandenb   (501) staff       (20)     8754 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/5.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)     1841 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/5.gff
--rw-r--r--   0 mvandenb   (501) staff       (20)     8530 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/5.gff3
--rw-r--r--   0 mvandenb   (501) staff       (20)       63 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/5_Ig-like.gff
--rw-r--r--   0 mvandenb   (501) staff       (20)      650 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/6.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)     5489 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/7.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)      162 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/8.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)      135 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/9.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)   276538 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/GRCm38mm10_chr5_34761740-34912521.fa
--rw-r--r--   0 mvandenb   (501) staff       (20)     4873 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/MTBLS6.zip
--rw-r--r--   0 mvandenb   (501) staff       (20)      818 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/a.tab
--rw-r--r--   0 mvandenb   (501) staff       (20)     1335 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/a.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       80 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/asian_chars_1.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       78 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/bad.html.gz
--rw-r--r--   0 mvandenb   (501) staff       (20)      502 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/bam_from_sam.bam
--rw-r--r--   0 mvandenb   (501) staff       (20)      484 2022-03-24 19:46:45.000000 galaxy-config-22.1.1/test-data/bam_native_from_sam.bam
--rw-r--r--   0 mvandenb   (501) staff       (20)    12492 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/bcf_index_metadata_test.bcf
--rw-r--r--   0 mvandenb   (501) staff       (20)       47 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/bcf_index_metadata_test.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)      706 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/biom1_metadata_test.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)     8474 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/cat_wrapper_out1.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)     1300 2022-08-18 15:49:03.000000 galaxy-config-22.1.1/test-data/chebi_57262.v3k.mol
--rw-r--r--   0 mvandenb   (501) staff       (20)      185 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/composite_output_expected_log
--rw-r--r--   0 mvandenb   (501) staff       (20)    19144 2022-08-18 15:49:03.000000 galaxy-config-22.1.1/test-data/drugbank_drugs.cml
--rw-r--r--   0 mvandenb   (501) staff       (20)      973 2022-08-18 15:49:03.000000 galaxy-config-22.1.1/test-data/drugbank_drugs.inchi
--rw-r--r--   0 mvandenb   (501) staff       (20)     8562 2022-08-18 15:49:03.000000 galaxy-config-22.1.1/test-data/drugbank_drugs.mol
--rw-r--r--   0 mvandenb   (501) staff       (20)    17032 2022-08-18 15:49:03.000000 galaxy-config-22.1.1/test-data/drugbank_drugs.mol2
--rw-r--r--   0 mvandenb   (501) staff       (20)    18997 2022-08-18 15:49:03.000000 galaxy-config-22.1.1/test-data/drugbank_drugs.sdf
--rw-r--r--   0 mvandenb   (501) staff       (20)      401 2022-08-18 15:49:03.000000 galaxy-config-22.1.1/test-data/drugbank_drugs.smi
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/empty.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)     2966 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/example-bag.zip
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.798787 galaxy-config-22.1.1/test-data/exports/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1482 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/exports/1901_two_datasets.tgz
--rw-r--r--   0 mvandenb   (501) staff       (20)    13573 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/filter1_in3.sam
--rw-r--r--   0 mvandenb   (501) staff       (20)      576 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/filter1_in5.tab
--rw-r--r--   0 mvandenb   (501) staff       (20)      287 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/filter1_in6.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)      310 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/filter1_inbad.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)      260 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/filter1_test1.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)      317 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/filter1_test2.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)      815 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/filter1_test3.sam
--rw-r--r--   0 mvandenb   (501) staff       (20)      286 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/filter1_test4.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)      494 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/filter1_test5.tab
--rw-r--r--   0 mvandenb   (501) staff       (20)       27 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/filter1_test6.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)        3 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/filter_labels_1.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)     3611 2020-09-12 06:37:53.000000 galaxy-config-22.1.1/test-data/html_file.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)     1838 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/input_taxonomy.biom1
--rw-r--r--   0 mvandenb   (501) staff       (20)       71 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/joiner_header_in1.tab
--rw-r--r--   0 mvandenb   (501) staff       (20)       76 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/joiner_header_in2.tab
--rw-r--r--   0 mvandenb   (501) staff       (20)     6257 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/joiner_out1.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)     7287 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/joiner_out2.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)     7479 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/joiner_out3.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)     7495 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/joiner_out4.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)      105 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/joiner_out5.tab
--rw-r--r--   0 mvandenb   (501) staff       (20)      126 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/joiner_out6.tab
--rw-r--r--   0 mvandenb   (501) staff       (20)       68 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/joiner_out7.tab
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.799439 galaxy-config-22.1.1/test-data/library/
--rw-r--r--   0 mvandenb   (501) staff       (20)     4696 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/library/3.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)       61 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/library/4.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)     8754 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/library/5.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)   408850 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/matrix.cool
--rw-r--r--   0 mvandenb   (501) staff       (20)      284 2022-03-24 19:46:45.000000 galaxy-config-22.1.1/test-data/neostore.zip
--rw-r--r--   0 mvandenb   (501) staff       (20)       20 2022-03-24 19:46:45.000000 galaxy-config-22.1.1/test-data/new_element_sort_order.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        6 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/new_labels_1.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       10 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/new_labels_2.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       13 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/new_labels_bad_1.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       11 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/new_labels_bad_2.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)      136 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/new_tags_1.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)     5473 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/phiX.fasta
--rw-r--r--   0 mvandenb   (501) staff       (20)      506 2022-03-24 19:46:45.000000 galaxy-config-22.1.1/test-data/qname_sorted.bam
--rw-r--r--   0 mvandenb   (501) staff       (20)     5691 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/qualscores.qual454
--rw-r--r--   0 mvandenb   (501) staff       (20)     2565 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/qualscores.qualsolid
--rw-r--r--   0 mvandenb   (501) staff       (20)     1024 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/random-file
--rw-r--r--   0 mvandenb   (501) staff       (20)      253 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/rgenetics.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)      700 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/rgenetics.bim
--rw-r--r--   0 mvandenb   (501) staff       (20)      603 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/rgenetics.fam
--rw-r--r--   0 mvandenb   (501) staff       (20)      600 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/rgenetics.map
--rw-r--r--   0 mvandenb   (501) staff       (20)     4603 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/rgenetics.ped
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.802657 galaxy-config-22.1.1/test-data/rules/
--rw-r--r--   0 mvandenb   (501) staff       (20)      700 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/rules/PRJDA60709.tsv
--rw-r--r--   0 mvandenb   (501) staff       (20)     1233 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/rules/PRJDB3920.tsv
--rw-r--r--   0 mvandenb   (501) staff       (20)    17005 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/rules/PRJNA355367.tsv
--rw-r--r--   0 mvandenb   (501) staff       (20)     5738 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/rules/treated1fb.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)     5694 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/rules/treated2fb.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)     5706 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/rules/treated3fb.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)      784 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/rules/uniprot.json
--rw-r--r--   0 mvandenb   (501) staff       (20)      744 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/rules/uniprot.tsv
--rw-r--r--   0 mvandenb   (501) staff       (20)     5707 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/rules/untreated1fb.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)     5735 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/rules/untreated2fb.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)     5685 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/rules/untreated3fb.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)     5692 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/rules/untreated4fb.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)    10240 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/safe_relative_symlink.tar
--rw-r--r--   0 mvandenb   (501) staff       (20)     3072 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/safetar_with_symlink.tar
--rw-r--r--   0 mvandenb   (501) staff       (20)      786 2022-03-24 19:46:45.000000 galaxy-config-22.1.1/test-data/sam_with_header.sam
--rw-r--r--   0 mvandenb   (501) staff       (20)     2914 2022-03-24 19:46:45.000000 galaxy-config-22.1.1/test-data/selenium-test-notebook.ipynb
--rw-r--r--   0 mvandenb   (501) staff       (20)   166534 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/shrimp_cs_test1.csfasta
--rw-r--r--   0 mvandenb   (501) staff       (20)       93 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/simple.xml
--rw-r--r--   0 mvandenb   (501) staff       (20)       24 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/simple_line.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       34 2022-03-24 19:46:45.000000 galaxy-config-22.1.1/test-data/simple_line_alternative.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       23 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/simple_line_no_newline.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       48 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/simple_line_x2.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       48 2022-08-18 15:49:03.000000 galaxy-config-22.1.1/test-data/simple_line_x2_windows.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       72 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/simple_line_x3.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)      120 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/simple_line_x5.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       57 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/simple_lines_both.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)      116 2022-03-24 19:46:45.000000 galaxy-config-22.1.1/test-data/simple_lines_interleaved.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)     4202 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/sort_out1.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)     4202 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/sort_out2.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)      818 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/sort_out3.tab
--rw-r--r--   0 mvandenb   (501) staff       (20)      786 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/sort_out4.sam
--rw-r--r--   0 mvandenb   (501) staff       (20)     1242 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/test.vcf
--rw-r--r--   0 mvandenb   (501) staff       (20)      422 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/test.vcf.gz
--rw-r--r--   0 mvandenb   (501) staff       (20)     3584 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/testdir.tar
--rw-r--r--   0 mvandenb   (501) staff       (20)    10240 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/testdir1.tar
--rw-r--r--   0 mvandenb   (501) staff       (20)      425 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/testdir1.tar.gz
--rw-r--r--   0 mvandenb   (501) staff       (20)      825 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/testdir1.zip
--rw-r--r--   0 mvandenb   (501) staff       (20)      253 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/tinywga.bed
--rw-r--r--   0 mvandenb   (501) staff       (20)      700 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/tinywga.bim
--rw-r--r--   0 mvandenb   (501) staff       (20)      603 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/tinywga.fam
--rw-r--r--   0 mvandenb   (501) staff       (20)      600 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/tinywga.map
--rw-r--r--   0 mvandenb   (501) staff       (20)     4603 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/tinywga.ped
--rw-r--r--   0 mvandenb   (501) staff       (20)     4603 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/tinywga.ped.space_to_tab
--rw-r--r--   0 mvandenb   (501) staff       (20)     2048 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/unsafe.tar
--rw-r--r--   0 mvandenb   (501) staff       (20)      309 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/unsafe.zip
--rw-r--r--   0 mvandenb   (501) staff       (20)     3072 2022-03-24 19:47:11.000000 galaxy-config-22.1.1/test-data/unsafe_relative_symlink.tar
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.740266 galaxy-config-22.1.1/test-data/users/
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.802881 galaxy-config-22.1.1/test-data/users/test1@bx.psu.edu/
--rw-r--r--   0 mvandenb   (501) staff       (20)    21625 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/users/test1@bx.psu.edu/1.fasta
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.740351 galaxy-config-22.1.1/test-data/users/test3@bx.psu.edu/
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.803138 galaxy-config-22.1.1/test-data/users/test3@bx.psu.edu/run1/
--rw-r--r--   0 mvandenb   (501) staff       (20)      672 2021-09-10 08:52:40.000000 galaxy-config-22.1.1/test-data/users/test3@bx.psu.edu/run1/2.fasta
--rw-r--r--   0 mvandenb   (501) staff       (20)       19 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/test-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.803353 galaxy-config-22.1.1/tests/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-08-18 15:49:03.000000 galaxy-config-22.1.1/tests/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.805189 galaxy-config-22.1.1/tests/config/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-08-18 15:49:03.000000 galaxy-config-22.1.1/tests/config/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.805564 galaxy-config-22.1.1/tests/config/config_manage/
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.740953 galaxy-config-22.1.1/tests/config/config_manage/1607_root_filters/
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.806266 galaxy-config-22.1.1/tests/config/config_manage/1607_root_filters/config/
--rw-r--r--   0 mvandenb   (501) staff       (20)    56349 2022-03-24 19:47:13.000000 galaxy-config-22.1.1/tests/config/config_manage/1607_root_filters/config/galaxy.ini
--rw-r--r--   0 mvandenb   (501) staff       (20)     6656 2022-03-24 19:47:13.000000 galaxy-config-22.1.1/tests/config/config_manage/1607_root_filters/config/tool_shed.ini
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.741176 galaxy-config-22.1.1/tests/config/config_manage/1607_root_samples/
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.807003 galaxy-config-22.1.1/tests/config/config_manage/1607_root_samples/config/
--rw-r--r--   0 mvandenb   (501) staff       (20)    56349 2022-03-24 19:47:13.000000 galaxy-config-22.1.1/tests/config/config_manage/1607_root_samples/config/galaxy.ini
--rw-r--r--   0 mvandenb   (501) staff       (20)     3001 2022-03-24 19:47:13.000000 galaxy-config-22.1.1/tests/config/config_manage/1607_root_samples/config/reports.ini
--rw-r--r--   0 mvandenb   (501) staff       (20)     6527 2022-03-24 19:47:13.000000 galaxy-config-22.1.1/tests/config/config_manage/1607_root_samples/config/tool_shed.ini
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.741397 galaxy-config-22.1.1/tests/config/config_manage/1705_allow_path_paste/
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.807375 galaxy-config-22.1.1/tests/config/config_manage/1705_allow_path_paste/config/
--rw-r--r--   0 mvandenb   (501) staff       (20)      100 2022-03-24 19:47:13.000000 galaxy-config-22.1.1/tests/config/config_manage/1705_allow_path_paste/config/galaxy.ini
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:13.000000 galaxy-config-22.1.1/tests/config/config_manage/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.741610 galaxy-config-22.1.1/tests/config/config_manage/embedded/
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.807592 galaxy-config-22.1.1/tests/config/config_manage/embedded/config/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1128 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/tests/config/config_manage/embedded/config/galaxy.yml
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.741826 galaxy-config-22.1.1/tests/config/config_manage/simple/
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:41.807809 galaxy-config-22.1.1/tests/config/config_manage/simple/config/
--rw-r--r--   0 mvandenb   (501) staff       (20)      584 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/tests/config/config_manage/simple/config/galaxy.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)     5014 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/tests/config/config_manage/test_config_manage.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1571 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/tests/config/test_config_dataset_storage.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    12810 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/tests/config/test_config_values.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     6861 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/tests/config/test_load_config.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5265 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/tests/config/test_path_graph.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    10891 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/tests/config/test_path_resolves_to.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3862 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/tests/config/test_reload_config.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2135 2022-08-22 19:45:28.000000 galaxy-config-22.1.1/tests/config/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:11.000000 galaxy-config-23.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-08 17:37:03.000000 galaxy-config-23.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-08 17:38:11.000000 galaxy-config-23.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:11.000000 galaxy-config-23.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:11.000000 galaxy-config-23.0.1/galaxy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    62353 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20123 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/config_manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:11.000000 galaxy-config-23.0.1/galaxy/config/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/auth_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/build_sites.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/container_resolvers_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/data_manager_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)   113255 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/datatypes_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/disposable_email_blocklist.conf.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/environment_modules_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/error_report.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/file_sources_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)   124190 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/galaxy.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)    53359 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/job_conf.sample.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    79082 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/job_conf.xml.sample_advanced
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/job_conf.xml.sample_basic
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/job_metrics_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/job_resource_params_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/lmod_modules_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/local_conda_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/object_store_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/oidc_backends_config.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/oidc_config.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/reports.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/themes_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/tool_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/tool_data_table_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/tool_destinations.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/tool_recommendations_overwrite.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)    14874 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/tool_shed.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/tool_sheds_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/trs_servers_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/user_preferences_extra_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/workflow_resource_mapper_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/workflow_resource_params_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/sample/workflow_schedulers_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:11.000000 galaxy-config-23.0.1/galaxy/config/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)   146525 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/schemas/config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/schemas/job_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/schemas/reports_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21370 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/schemas/tool_shed_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/config/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:11.000000 galaxy-config-23.0.1/galaxy_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-08 17:38:11.000000 galaxy-config-23.0.1/galaxy_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-08 17:38:11.000000 galaxy-config-23.0.1/galaxy_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:38:11.000000 galaxy-config-23.0.1/galaxy_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 17:38:11.000000 galaxy-config-23.0.1/galaxy_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 17:38:11.000000 galaxy-config-23.0.1/galaxy_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:38:11.000000 galaxy-config-23.0.1/galaxy_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-08 17:38:11.000000 galaxy-config-23.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 17:37:04.000000 galaxy-config-23.0.1/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `galaxy-config-22.1.1/LICENSE` & `galaxy-config-23.0.1/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,61 @@
-Copyright (c) 2005-2016 Galaxy Contributors (see CONTRIBUTORS.md)
+Copyright (c) 2005-2022 Galaxy Contributors (see CONTRIBUTORS.md)
+
+Work contributed from 2021-04-07 onwards is licensed under the MIT License.
+Work contributed before this date is licensed under the Academic Free License
+version 3.0.
+See https://github.com/galaxyproject/galaxy/ for the contribution history.
+See below for the full text of both licenses.
+
+
+Some icons found in Galaxy are from the Silk Icons set, available under
+the Creative Commons Attribution 2.5 License, from:
+
+http://www.famfamfam.com/lab/icons/silk/
+
+
+Other images and documentation are licensed under the Creative Commons
+Attribution 3.0 (CC BY 3.0) License. See:
+
+http://creativecommons.org/licenses/by/3.0/
+
+
+--------------------------------------------------------------------------------
+
+
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+--------------------------------------------------------------------------------
+
+
+Academic Free License ("AFL") v. 3.0
+
+This Academic Free License (the "License") applies to any original work of
+authorship (the "Original Work") whose owner (the "Licensor") has placed the
+following licensing notice adjacent to the copyright notice for the Original
+Work:
 
 Licensed under the Academic Free License version 3.0
 
  1) Grant of Copyright License. Licensor grants You a worldwide, royalty-free, 
     non-exclusive, sublicensable license, for the duration of the copyright, to 
     do the following:
 
@@ -169,18 +222,7 @@
     replace the notice specified in the first paragraph above with the 
     notice "Licensed under <insert your license name here>" or with a notice 
     of your own that is not confusingly similar to the notice in this 
     License; and (iii) You may not claim that your original works are open 
     source software unless your Modified License has been approved by Open 
     Source Initiative (OSI) and You comply with its license review and 
     certification process.
-
-
-Some icons found in Galaxy are from the Silk Icons set, available under
-the Creative Commons Attribution 2.5 License, from:
-
-http://www.famfamfam.com/lab/icons/silk/
-
-
-Other images and documentation are licensed under the Creative Commons Attribution 3.0 (CC BY 3.0) License.   See 
-
-http://creativecommons.org/licenses/by/3.0/
```

### Comparing `galaxy-config-22.1.1/PKG-INFO` & `galaxy-config-23.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,69 @@
 Metadata-Version: 2.1
 Name: galaxy-config
-Version: 22.1.1
-Summary: Galaxy Configuration
+Version: 23.0.1
+Summary: Galaxy configuration
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
-Keywords: galaxy
-Platform: UNKNOWN
+Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Testing
 Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: https://badge.fury.io/py/galaxy-config.svg
    :target: https://pypi.org/project/galaxy-config/
 
 
 Overview
 --------
 
 The Galaxy_ config module.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
-
-
-
 History
 -------
 
 .. to_doc
 
----------------------
-22.1.0.dev0
----------------------
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
-* Initial release
 
+=========
+Bug fixes
+=========
+
+* Change default watchdog inotify_buffer log level to info by `@mvdbeek <https://github.com/mvdbeek>`_ in `#15967 <https://github.com/galaxyproject/galaxy/pull/15967>`_
 
+============
+Enhancements
+============
+
+* Add ``ca_certs`` option for sentry client by `@mvdbeek <https://github.com/mvdbeek>`_ in `#15943 <https://github.com/galaxyproject/galaxy/pull/15943>`_
+
+-------------------
+22.1.1 (2022-08-22)
+-------------------
+
+* Initial release
```

### Comparing `galaxy-config-22.1.1/galaxy/config/__init__.py` & `galaxy-config-23.0.1/galaxy/config/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Universe configuration builder.
 """
 # absolute_import needed for tool_shed package.
 
 import configparser
 import ipaddress
+import json
 import locale
 import logging
 import logging.config
 import os
 import re
 import socket
 import string
@@ -21,110 +22,129 @@
     Callable,
     cast,
     Dict,
     List,
     Optional,
     Set,
     SupportsInt,
+    TYPE_CHECKING,
     TypeVar,
     Union,
 )
 
 import yaml
 
 from galaxy.config.schema import AppSchema
-from galaxy.containers import parse_containers_config
 from galaxy.exceptions import ConfigurationError
 from galaxy.util import (
     listify,
+    size_to_bytes,
     string_as_bool,
     unicodify,
 )
 from galaxy.util.custom_logging import LOGLV_TRACE
 from galaxy.util.dynamic import HasDynamicProperties
 from galaxy.util.facts import get_facts
 from galaxy.util.properties import (
-    find_config_file,
     read_properties_from_file,
     running_from_source,
 )
-from ..version import VERSION_MAJOR, VERSION_MINOR
+from galaxy.util.themes import flatten_theme
+from ..version import (
+    VERSION_MAJOR,
+    VERSION_MINOR,
+)
+
+if TYPE_CHECKING:
+    from galaxy.model import User
 
 try:
     from importlib.resources import files  # type: ignore[attr-defined]
 except ImportError:
     # Python < 3.9
     from importlib_resources import files  # type: ignore[no-redef]
 
 log = logging.getLogger(__name__)
 
-DEFAULT_LOCALE_FORMAT = '%a %b %e %H:%M:%S %Y'
+DEFAULT_LOCALE_FORMAT = "%a %b %e %H:%M:%S %Y"
 ISO_DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 GALAXY_APP_NAME = "galaxy"
 GALAXY_SCHEMAS_PATH = files("galaxy.config") / "schemas"
 GALAXY_CONFIG_SCHEMA_PATH = GALAXY_SCHEMAS_PATH / "config_schema.yml"
 REPORTS_CONFIG_SCHEMA_PATH = GALAXY_SCHEMAS_PATH / "reports_config_schema.yml"
 TOOL_SHED_CONFIG_SCHEMA_PATH = GALAXY_SCHEMAS_PATH / "tool_shed_config_schema.yml"
-UWSGI_SCHEMA_PATH = GALAXY_SCHEMAS_PATH / "uwsgi_schema.yml"
 LOGGING_CONFIG_DEFAULT: Dict[str, Any] = {
-    'disable_existing_loggers': False,
-    'version': 1,
-    'root': {
-        'handlers': ['console'],
-        'level': 'DEBUG',
+    "disable_existing_loggers": False,
+    "version": 1,
+    "root": {
+        "handlers": ["console"],
+        "level": "DEBUG",
     },
-    'loggers': {
-        'paste.httpserver.ThreadPool': {
-            'level': 'WARN',
-            'qualname': 'paste.httpserver.ThreadPool',
+    "loggers": {
+        "paste.httpserver.ThreadPool": {
+            "level": "WARN",
+            "qualname": "paste.httpserver.ThreadPool",
+        },
+        "sqlalchemy_json.track": {
+            "level": "WARN",
+            "qualname": "sqlalchemy_json.track",
         },
-        'sqlalchemy_json.track': {
-            'level': 'WARN',
-            'qualname': 'sqlalchemy_json.track',
+        "urllib3.connectionpool": {
+            "level": "WARN",
+            "qualname": "urllib3.connectionpool",
         },
-        'urllib3.connectionpool': {
-            'level': 'WARN',
-            'qualname': 'urllib3.connectionpool',
+        "routes.middleware": {
+            "level": "WARN",
+            "qualname": "routes.middleware",
         },
-        'routes.middleware': {
-            'level': 'WARN',
-            'qualname': 'routes.middleware',
+        "amqp": {
+            "level": "INFO",
+            "qualname": "amqp",
         },
-        'amqp': {
-            'level': 'INFO',
-            'qualname': 'amqp',
+        "botocore": {
+            "level": "INFO",
+            "qualname": "botocore",
         },
-        'botocore': {
-            'level': 'INFO',
-            'qualname': 'botocore',
+        "gunicorn.access": {
+            "level": "INFO",
+            "qualname": "gunicorn.access",
+            "propagate": False,
+            "handlers": ["console"],
+        },
+        "watchdog.observers.inotify_buffer": {
+            "level": "INFO",
+            "qualname": "watchdog.observers.inotify_buffer",
         },
     },
-    'filters': {
-        'stack': {
-            '()': 'galaxy.web_stack.application_stack_log_filter',
+    "filters": {
+        "stack": {
+            "()": "galaxy.web_stack.application_stack_log_filter",
         },
     },
-    'handlers': {
-        'console': {
-            'class': 'logging.StreamHandler',
-            'formatter': 'stack',
-            'level': 'DEBUG',
-            'stream': 'ext://sys.stderr',
-            'filters': ['stack'],
+    "handlers": {
+        "console": {
+            "class": "logging.StreamHandler",
+            "formatter": "stack",
+            "level": "DEBUG",
+            "stream": "ext://sys.stderr",
+            "filters": ["stack"],
         },
     },
-    'formatters': {
-        'stack': {
-            '()': 'galaxy.web_stack.application_stack_log_formatter',
+    "formatters": {
+        "stack": {
+            "()": "galaxy.web_stack.application_stack_log_formatter",
         },
     },
 }
 """Default value for logging configuration, passed to :func:`logging.config.dictConfig`"""
 
+VERSION_JSON_FILE = "version.json"
+DISABLED_FLAG = "disabled"  # Used to mark a config option as disabled
+
 
 def configure_logging(config, facts=None):
     """Allow some basic logging configuration to be read from ini file.
 
     This should be able to consume either a galaxy.config.Configuration object
     or a simple dictionary of configuration variables.
     """
@@ -135,32 +155,38 @@
     # 'loggers' section was found in the config file, otherwise we do
     # some simple setup using the 'log_*' values from the config.
     parser = getattr(config, "global_conf_parser", None)
     if parser:
         paste_configures_logging = config.global_conf_parser.has_section("loggers")
     else:
         paste_configures_logging = False
-    auto_configure_logging = not paste_configures_logging and string_as_bool(config.get("auto_configure_logging", "True"))
+    auto_configure_logging = not paste_configures_logging and string_as_bool(
+        config.get("auto_configure_logging", "True")
+    )
     if auto_configure_logging:
-        logging_conf = config.get('logging', None)
+        logging_conf = config.get("logging", None)
         if logging_conf is None:
             # if using the default logging config, honor the log_level setting
             logging_conf = LOGGING_CONFIG_DEFAULT
-            if config.get('log_level', 'DEBUG') != 'DEBUG':
-                logging_conf['handlers']['console']['level'] = config.get('log_level', 'DEBUG')
+            if config.get("log_level", "DEBUG") != "DEBUG":
+                logging_conf["handlers"]["console"]["level"] = config.get("log_level", "DEBUG")
         # configure logging with logging dict in config, template *FileHandler handler filenames with the `filename_template` option
-        for name, conf in logging_conf.get('handlers', {}).items():
-            if conf['class'].startswith('logging.') and conf['class'].endswith('FileHandler') and 'filename_template' in conf:
-                conf['filename'] = conf.pop('filename_template').format(**facts)
-                logging_conf['handlers'][name] = conf
+        for name, conf in logging_conf.get("handlers", {}).items():
+            if (
+                conf["class"].startswith("logging.")
+                and conf["class"].endswith("FileHandler")
+                and "filename_template" in conf
+            ):
+                conf["filename"] = conf.pop("filename_template").format(**facts)
+                logging_conf["handlers"][name] = conf
         logging.config.dictConfig(logging_conf)
 
 
 def find_root(kwargs):
-    return os.path.abspath(kwargs.get('root_dir', '.'))
+    return os.path.abspath(kwargs.get("root_dir", "."))
 
 
 def expand_pretty_datetime_format(value):
     """
 
     >>> expand_pretty_datetime_format("%H:%M:%S %Z")
     '%H:%M:%S %Z'
@@ -190,15 +216,17 @@
 
 
 class BaseAppConfiguration(HasDynamicProperties):
     # Override in subclasses (optional): {KEY: config option, VALUE: deprecated directory name}
     # If VALUE == first directory in a user-supplied path that resolves to KEY, it will be stripped from that path
     renamed_options: Optional[Dict[str, str]] = None
     deprecated_dirs: Dict[str, str] = {}
-    paths_to_check_against_root: Set[str] = set()  # backward compatibility: if resolved path doesn't exist, try resolving w.r.t root
+    paths_to_check_against_root: Set[
+        str
+    ] = set()  # backward compatibility: if resolved path doesn't exist, try resolving w.r.t root
     add_sample_file_to_defaults: Set[str] = set()  # for these options, add sample config files to their defaults
     listify_options: Set[str] = set()  # values for these options are processed as lists of values
     object_store_store_by: str
 
     def __init__(self, **kwargs):
         self._preprocess_kwargs(kwargs)
         self._kwargs = kwargs  # Save these as a record of explicitly set options
@@ -228,147 +256,155 @@
                     kwargs[new] = kwargs[old]
 
     def _fix_postgresql_dburl(self, kwargs):
         """
         Fix deprecated database URLs (postgres... >> postgresql...)
         https://docs.sqlalchemy.org/en/14/changelog/changelog_14.html#change-3687655465c25a39b968b4f5f6e9170b
         """
-        old_dialect, new_dialect = 'postgres', 'postgresql'
-        old_prefixes = (f'{old_dialect}:', f'{old_dialect}+')  # check for postgres://foo and postgres+driver//foo
+        old_dialect, new_dialect = "postgres", "postgresql"
+        old_prefixes = (f"{old_dialect}:", f"{old_dialect}+")  # check for postgres://foo and postgres+driver//foo
         offset = len(old_dialect)
-        keys = ('database_connection', 'install_database_connection')
+        keys = ("database_connection", "install_database_connection")
         for key in keys:
             if key in kwargs:
                 value = kwargs[key]
                 for prefix in old_prefixes:
                     if value.startswith(prefix):
-                        value = f'{new_dialect}{value[offset:]}'
+                        value = f"{new_dialect}{value[offset:]}"
                         kwargs[key] = value
-                        log.warning('PostgreSQL database URLs of the form "postgres://" have been '
-                            'deprecated. Please use "postgresql://".')
+                        log.warning(
+                            'PostgreSQL database URLs of the form "postgres://" have been '
+                            'deprecated. Please use "postgresql://".'
+                        )
 
     def is_set(self, key):
         """Check if a configuration option has been explicitly set."""
         # NOTE: This will check all supplied keyword arguments, including those not in the schema.
         # To check only schema options, change the line below to `if property not in self._raw_config:`
         if key not in self._raw_config:
             log.warning(f"Configuration option does not exist: '{key}'")
         return key in self._kwargs
 
     def resolve_path(self, path):
         """Resolve a path relative to Galaxy's root."""
         return self._in_root_dir(path)
 
     def _set_config_base(self, config_kwargs):
-
         def _set_global_conf():
-            self.config_file = find_config_file('galaxy')
-            self.global_conf = config_kwargs.get('global_conf')
+            self.config_file = config_kwargs.get("__file__", None)
+            self.global_conf = config_kwargs.get("global_conf")
             self.global_conf_parser = configparser.ConfigParser()
             if not self.config_file and self.global_conf and "__file__" in self.global_conf:
-                self.config_file = os.path.join(self.root, self.global_conf['__file__'])
+                self.config_file = os.path.join(self.root, self.global_conf["__file__"])
 
             if self.config_file is None:
                 log.warning("No Galaxy config file found, running from current working directory: %s", os.getcwd())
             else:
                 try:
                     self.global_conf_parser.read(self.config_file)
                 except OSError:
                     raise
                 except Exception:
                     pass  # Not an INI file
 
         def _set_config_directories():
             # Set config_dir to value from kwargs OR dirname of config_file OR None
             _config_dir = os.path.dirname(self.config_file) if self.config_file else None
-            self.config_dir = config_kwargs.get('config_dir', _config_dir)
+            self.config_dir = config_kwargs.get("config_dir", _config_dir)
             # Make path absolute before using it as base for other paths
             if self.config_dir:
                 self.config_dir = os.path.abspath(self.config_dir)
 
-            self.data_dir = config_kwargs.get('data_dir')
+            self.data_dir = config_kwargs.get("data_dir")
             if self.data_dir:
                 self.data_dir = os.path.abspath(self.data_dir)
 
-            self.sample_config_dir = os.path.join(os.path.dirname(__file__), 'sample')
+            self.sample_config_dir = os.path.join(os.path.dirname(__file__), "sample")
             if self.sample_config_dir:
                 self.sample_config_dir = os.path.abspath(self.sample_config_dir)
 
-            self.managed_config_dir = config_kwargs.get('managed_config_dir')
+            self.managed_config_dir = config_kwargs.get("managed_config_dir")
             if self.managed_config_dir:
                 self.managed_config_dir = os.path.abspath(self.managed_config_dir)
 
             if running_from_source:
                 if not self.config_dir:
-                    self.config_dir = os.path.join(self.root, 'config')
+                    self.config_dir = os.path.join(self.root, "config")
                 if not self.data_dir:
-                    self.data_dir = os.path.join(self.root, 'database')
+                    self.data_dir = os.path.join(self.root, "database")
                 if not self.managed_config_dir:
                     self.managed_config_dir = self.config_dir
             else:
                 if not self.config_dir:
                     self.config_dir = os.getcwd()
                 if not self.data_dir:
-                    self.data_dir = self._in_config_dir('data')
+                    self.data_dir = self._in_config_dir("data")
                 if not self.managed_config_dir:
-                    self.managed_config_dir = self._in_data_dir('config')
+                    self.managed_config_dir = self._in_data_dir("config")
 
             # TODO: do we still need to support ../shed_tools when running_from_source?
-            self.shed_tools_dir = self._in_data_dir('shed_tools')
+            self.shed_tools_dir = self._in_data_dir("shed_tools")
 
             log.debug("Configuration directory is %s", self.config_dir)
             log.debug("Data directory is %s", self.data_dir)
             log.debug("Managed config directory is %s", self.managed_config_dir)
 
         _set_global_conf()
         _set_config_directories()
 
     def _load_schema(self):
         # Override in subclasses
-        raise Exception('Not implemented')
+        raise Exception("Not implemented")
 
     def _preprocess_paths_to_resolve(self):
         # For these options, if option is not set, listify its defaults and add a sample config file.
         if self.add_sample_file_to_defaults:
             for key in self.add_sample_file_to_defaults:
                 if not self.is_set(key):
                     defaults = listify(getattr(self, key), do_strip=True)
-                    sample = f'{defaults[-1]}.sample'  # if there are multiple defaults, use last as template
+                    sample = f"{defaults[-1]}.sample"  # if there are multiple defaults, use last as template
                     sample = self._in_sample_dir(sample)  # resolve w.r.t sample_dir
                     defaults.append(sample)
                     setattr(self, key, defaults)
 
     def _postprocess_paths_to_resolve(self):
-
         def select_one_path_from_list():
             # To consider: options with a sample file added to defaults except options that can have multiple values.
             # If value is not set, check each path in list; set to first path that exists; if none exist, set to last path in list.
-            keys = self.add_sample_file_to_defaults - self.listify_options if self.listify_options else self.add_sample_file_to_defaults
+            keys = (
+                self.add_sample_file_to_defaults - self.listify_options
+                if self.listify_options
+                else self.add_sample_file_to_defaults
+            )
             for key in keys:
                 if not self.is_set(key):
                     paths = getattr(self, key)
                     for path in paths:
                         if self._path_exists(path):
                             setattr(self, key, path)
                             break
                     else:
-                        setattr(self, key, paths[-1])  # TODO: we assume it exists; but we've already checked in the loop! Raise error instead?
+                        setattr(
+                            self, key, paths[-1]
+                        )  # TODO: we assume it exists; but we've already checked in the loop! Raise error instead?
 
         def select_one_or_all_paths_from_list():
             # Values for these options are lists of paths. If value is not set, use defaults if all paths in list exist;
             # otherwise, set to last path in list.
             for key in self.listify_options:
                 if not self.is_set(key):
                     paths = getattr(self, key)
                     for path in paths:
                         if not self._path_exists(path):
                             setattr(self, key, [paths[-1]])  # value is a list
                             break
 
-        if self.add_sample_file_to_defaults:  # Currently, this is the ONLY case when we need to pick one file from a list
+        if (
+            self.add_sample_file_to_defaults
+        ):  # Currently, this is the ONLY case when we need to pick one file from a list
             select_one_path_from_list()
         if self.listify_options:
             select_one_or_all_paths_from_list()
 
     def _path_exists(self, path):  # factored out so we can mock it in tests
         return os.path.exists(path)
 
@@ -377,24 +413,23 @@
         if not self.is_set(option):
             for path in alt_paths:
                 if self._path_exists(path):
                     setattr(self, option, path)
                     return path
 
     def _update_raw_config_from_kwargs(self, kwargs):
-
         type_converters: Dict[str, Callable[[Any], Union[bool, int, float, str]]] = {
             "bool": string_as_bool,
             "int": int,
             "float": float,
             "str": str,
         }
 
         def convert_datatype(key, value):
-            datatype = self.schema.app_schema[key].get('type')
+            datatype = self.schema.app_schema[key].get("type")
             # check for `not None` explicitly (value can be falsy)
             if value is not None and datatype in type_converters:
                 # convert value or each item in value to type `datatype`
                 f = type_converters[datatype]
                 if isinstance(value, list):
                     return [f(item) for item in value]
                 else:
@@ -407,43 +442,51 @@
                 paths = listify(value, do_strip=True)
                 for i, path in enumerate(paths):
                     first_dir = path.split(os.sep)[0]  # get first directory component
                     if first_dir == self.deprecated_dirs.get(resolves_to):  # first_dir is deprecated for this option
                         ignore = first_dir + os.sep
                         log.warning(
                             "Paths for the '%s' option are now relative to '%s', remove the leading '%s' "
-                            "to suppress this warning: %s", key, resolves_to, ignore, path
+                            "to suppress this warning: %s",
+                            key,
+                            resolves_to,
+                            ignore,
+                            path,
                         )
-                        paths[i] = path[len(ignore):]
+                        paths[i] = path[len(ignore) :]
 
                 # return list or string, depending on type of `value`
                 if isinstance(value, list):
                     return paths
-                return ','.join(paths)
+                return ",".join(paths)
             return value
 
         for key, value in kwargs.items():
+            if key in self.schema._deprecated_aliases:
+                new_key = self.schema._deprecated_aliases[key]
+                log.warning(f"Option {key} has been deprecated in favor of {new_key}")
+                key = new_key
+
             if key in self.schema.app_schema:
                 value = convert_datatype(key, value)
                 if value and self.deprecated_dirs:
                     value = strip_deprecated_dir(key, value)
                 self._raw_config[key] = value
 
     def _create_attributes_from_raw_config(self):
         # `base_configs` are a special case: these attributes have been created and will be ignored
         # by the code below. Trying to overwrite any other existing attributes will raise an error.
-        base_configs = {'config_dir', 'data_dir', 'managed_config_dir'}
+        base_configs = {"config_dir", "data_dir", "managed_config_dir"}
         for key, value in self._raw_config.items():
             if not hasattr(self, key):
                 setattr(self, key, value)
             elif key not in base_configs:
                 raise ConfigurationError(f"Attempting to override existing attribute '{key}'")
 
     def _resolve_paths(self):
-
         def resolve(key):
             if key in _cache:  # resolve each path only once
                 return _cache[key]
 
             path = getattr(self, key)  # path prior to being resolved
             parent = self.schema.paths_to_resolve.get(key)
             if not parent:  # base case: nothing else needs resolving
@@ -460,28 +503,27 @@
 
         _cache = {}
         for key in self.schema.paths_to_resolve:
             value = getattr(self, key)
             # Check if value is a list or should be listified; if so, listify and resolve each item separately.
             if type(value) is list or (self.listify_options and key in self.listify_options):
                 saved_values = listify(getattr(self, key), do_strip=True)  # listify and save original value
-                setattr(self, key, '_')  # replace value with temporary placeholder
+                setattr(self, key, "_")  # replace value with temporary placeholder
                 resolve(key)  # resolve temporary value (`_` becomes `parent-path/_`)
                 resolved_base = getattr(self, key)[:-1]  # get rid of placeholder in resolved path
                 # apply resolved base to saved values
                 resolved_paths = [os.path.join(resolved_base, value) for value in saved_values]
                 setattr(self, key, resolved_paths)  # set config.key to a list of resolved paths
             else:
                 resolve(key)
             # Check options that have been set and may need to be resolved w.r.t. root
             if self.is_set(key) and self.paths_to_check_against_root and key in self.paths_to_check_against_root:
                 self._check_against_root(key)
 
     def _check_against_root(self, key):
-
         def get_path(current_path, initial_path):
             # if path does not exist and was set as relative:
             if not self._path_exists(current_path) and not os.path.isabs(initial_path):
                 new_path = self._in_root_dir(initial_path)
                 if self._path_exists(new_path):  # That's a bingo!
                     resolves_to = self.schema.paths_to_resolve.get(key)
                     log.warning(
@@ -538,17 +580,17 @@
         return self._admin_users
 
     @admin_users.setter
     def admin_users(self, value):
         self._admin_users = value
         self.admin_users_list = listify(value)
 
-    def is_admin_user(self, user):
+    def is_admin_user(self, user: Optional["User"]) -> bool:
         """Determine if the provided user is listed in `admin_users`."""
-        return user and (user.email in self.admin_users_list or user.bootstrap_admin_user)
+        return user is not None and (user.email in self.admin_users_list or user.bootstrap_admin_user)
 
     @property
     def sentry_dsn_public(self):
         """
         Sentry URL with private key removed for use in client side scripts,
         sentry server will need to be configured to accept events
         """
@@ -571,76 +613,89 @@
             try:
                 os.makedirs(path)
             except Exception as e:
                 raise ConfigurationError(f"Unable to create missing directory: {path}\n{unicodify(e)}")
 
 
 class GalaxyAppConfiguration(BaseAppConfiguration, CommonConfigurationMixin):
-    deprecated_options = ('database_file', 'track_jobs_in_database', 'blacklist_file', 'whitelist_file',
-                          'sanitize_whitelist_file', 'user_library_import_symlink_whitelist', 'fetch_url_whitelist',
-                          'containers_resolvers_config_file')
+    deprecated_options = (
+        "database_file",
+        "track_jobs_in_database",
+        "blacklist_file",
+        "whitelist_file",
+        "sanitize_whitelist_file",
+        "user_library_import_symlink_whitelist",
+        "fetch_url_whitelist",
+        "containers_resolvers_config_file",
+    )
     renamed_options = {
-        'blacklist_file': 'email_domain_blocklist_file',
-        'whitelist_file': 'email_domain_allowlist_file',
-        'sanitize_whitelist_file': 'sanitize_allowlist_file',
-        'user_library_import_symlink_whitelist': 'user_library_import_symlink_allowlist',
-        'fetch_url_whitelist': 'fetch_url_allowlist',
-        'containers_resolvers_config_file': 'container_resolvers_config_file',
+        "blacklist_file": "email_domain_blocklist_file",
+        "whitelist_file": "email_domain_allowlist_file",
+        "sanitize_whitelist_file": "sanitize_allowlist_file",
+        "user_library_import_symlink_whitelist": "user_library_import_symlink_allowlist",
+        "fetch_url_whitelist": "fetch_url_allowlist",
+        "containers_resolvers_config_file": "container_resolvers_config_file",
     }
-    default_config_file_name = 'galaxy.yml'
-    deprecated_dirs = {'config_dir': 'config', 'data_dir': 'database'}
+    default_config_file_name = "galaxy.yml"
+    deprecated_dirs = {"config_dir": "config", "data_dir": "database"}
 
     paths_to_check_against_root = {
-        'auth_config_file',
-        'build_sites_config_file',
-        'containers_config_file',
-        'data_manager_config_file',
-        'datatypes_config_file',
-        'dependency_resolvers_config_file',
-        'error_report_file',
-        'job_config_file',
-        'job_metrics_config_file',
-        'job_resource_params_file',
-        'local_conda_mapping_file',
-        'migrated_tools_config',
-        'modules_mapping_files',
-        'object_store_config_file',
-        'oidc_backends_config_file',
-        'oidc_config_file',
-        'shed_data_manager_config_file',
-        'shed_tool_config_file',
-        'shed_tool_data_table_config',
-        'tool_destinations_config_file',
-        'tool_sheds_config_file',
-        'user_preferences_extra_conf_path',
-        'workflow_resource_params_file',
-        'workflow_schedulers_config_file',
-        'markdown_export_css',
-        'markdown_export_css_pages',
-        'markdown_export_css_invocation_reports',
-        'file_path',
-        'tool_data_table_config_path',
-        'tool_config_file',
+        "auth_config_file",
+        "build_sites_config_file",
+        "data_manager_config_file",
+        "datatypes_config_file",
+        "dependency_resolvers_config_file",
+        "error_report_file",
+        "job_config_file",
+        "job_metrics_config_file",
+        "job_resource_params_file",
+        "local_conda_mapping_file",
+        "migrated_tools_config",
+        "modules_mapping_files",
+        "object_store_config_file",
+        "oidc_backends_config_file",
+        "oidc_config_file",
+        "shed_data_manager_config_file",
+        "shed_tool_config_file",
+        "shed_tool_data_table_config",
+        "tool_destinations_config_file",
+        "tool_sheds_config_file",
+        "user_preferences_extra_conf_path",
+        "workflow_resource_params_file",
+        "workflow_schedulers_config_file",
+        "markdown_export_css",
+        "markdown_export_css_pages",
+        "markdown_export_css_invocation_reports",
+        "file_path",
+        "tool_data_table_config_path",
+        "tool_config_file",
+        "themes_config_file",
     }
 
     add_sample_file_to_defaults = {
-        'build_sites_config_file',
-        'datatypes_config_file',
-        'job_metrics_config_file',
-        'tool_data_table_config_path',
-        'tool_config_file',
+        "build_sites_config_file",
+        "datatypes_config_file",
+        "job_metrics_config_file",
+        "tool_data_table_config_path",
+        "tool_config_file",
     }
 
     listify_options = {
-        'tool_data_table_config_path',
-        'tool_config_file',
+        "tool_data_table_config_path",
+        "tool_config_file",
     }
     database_connection: str
     tool_path: str
     tool_data_path: str
+    new_file_path: str
+    drmaa_external_runjob_script: str
+    track_jobs_in_database: bool
+    monitor_thread_join_timeout: int
+    manage_dependency_relationships: bool
+    enable_tool_shed_check: bool
     builds_file_path: str
     len_file_path: str
     integrated_tool_panel_config: str
     toolbox_filter_base_modules: List[str]
     tool_filters: List[str]
     tool_label_filters: List[str]
     tool_section_filters: List[str]
@@ -648,17 +703,16 @@
     user_tool_section_filters: List[str]
     user_tool_label_filters: List[str]
     password_expiration_period: timedelta
     shed_tool_data_path: str
     hours_between_check: int
     galaxy_data_manager_data_path: str
     use_remote_user: bool
-    cluster_files_directory: str
     preserve_python_environment: str
-    email_from: str
+    email_from: Optional[str]
     workflow_resource_params_mapper: str
     sanitize_allowlist_file: str
     allowed_origin_hostnames: List[str]
     trust_jupyter_notebook_conversion: bool
     user_library_import_symlink_allowlist: List[str]
     user_library_import_dir_auto_creation: bool
     container_resolvers_config_file: str
@@ -666,37 +720,42 @@
     involucro_path: str
     mulled_channels: List[str]
     nginx_upload_store: str
     tus_upload_store: str
     pretty_datetime_format: str
     visualization_plugins_directory: str
     galaxy_infrastructure_url: str
+    themes: Dict[str, Dict[str, str]]
+    themes_by_host: Dict[str, Dict[str, Dict[str, str]]]
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._override_tempdir(kwargs)
         self._configure_sqlalchemy20_warnings(kwargs)
         self._process_config(kwargs)
 
     def _configure_sqlalchemy20_warnings(self, kwargs):
         """
         This method should be deleted after migration to SQLAlchemy 2.0 is complete.
         To enable warnings, set `GALAXY_CONFIG_SQLALCHEMY_WARN_20=1`,
         """
-        warn = string_as_bool(kwargs.get('sqlalchemy_warn_20', False))
+        warn = string_as_bool(kwargs.get("sqlalchemy_warn_20", False))
         if warn:
             import sqlalchemy
+
             sqlalchemy.util.deprecations.SQLALCHEMY_WARN_20 = True
             self._setup_sqlalchemy20_warnings_filters()
 
     def _setup_sqlalchemy20_warnings_filters(self):
         import warnings
+
         from sqlalchemy.exc import RemovedIn20Warning
+
         # Always display RemovedIn20Warning warnings.
-        warnings.filterwarnings('always', category=RemovedIn20Warning)
+        warnings.filterwarnings("always", category=RemovedIn20Warning)
         # Optionally, enable filters for specific warnings (raise error, or log, etc.)
         # messages = [
         #     r"replace with warning text to match",
         # ]
         # for msg in messages:
         #     warnings.filterwarnings('error', message=msg, category=RemovedIn20Warning)
         #
@@ -711,84 +770,100 @@
         if string_as_bool(kwargs.get("override_tempdir", "True")):
             tempfile.tempdir = self.new_file_path
 
     def config_value_for_host(self, config_option, host):
         val = getattr(self, config_option)
         if config_option in self.schema.per_host_options:
             per_host_option = f"{config_option}_by_host"
+            per_host: Dict[str, Any] = {}
             if per_host_option in self.config_dict:
                 per_host = self.config_dict[per_host_option] or {}
-                for host_key, host_val in per_host.items():
-                    if host_key in host:
-                        val = host_val
-                        break
+            else:
+                per_host = getattr(self, per_host_option, {})
+            for host_key, host_val in per_host.items():
+                if host_key in host:
+                    val = host_val
+                    break
 
         return val
 
-    def _process_config(self, kwargs):
+    def _process_config(self, kwargs: Dict[str, Any]) -> None:
         # Backwards compatibility for names used in too many places to fix
         self.datatypes_config = self.datatypes_config_file
         self.tool_configs = self.tool_config_file
 
         # Collect the umask and primary gid from the environment
         self.umask = os.umask(0o77)  # get the current umask
         os.umask(self.umask)  # can't get w/o set, so set it back
         self.gid = os.getgid()  # if running under newgrp(1) we'll need to fix the group of data created on the cluster
 
         self.version_major = VERSION_MAJOR
         self.version_minor = VERSION_MINOR
+        # Try loading extra version info
+        self.version_extra = None
+        json_file = os.environ.get(
+            "GALAXY_VERSION_JSON_FILE", self._in_root_dir(VERSION_JSON_FILE)
+        )  # TODO: add this to schema
+        try:
+            with open(json_file) as f:
+                extra_info = json.load(f)
+        except FileNotFoundError:
+            log.debug("No extra version JSON file detected at %s", json_file)
+        except ValueError:
+            log.error("Error loading Galaxy extra version JSON file %s - details not loaded.", json_file)
+        else:
+            self.version_extra = extra_info
 
         # Database related configuration
-        self.check_migrate_databases = kwargs.get('check_migrate_databases', True)
+        self.check_migrate_databases = string_as_bool(kwargs.get("check_migrate_databases", True))
         if not self.database_connection:  # Provide default if not supplied by user
-            db_path = self._in_data_dir('universe.sqlite')
-            self.database_connection = f'sqlite:///{db_path}?isolation_level=IMMEDIATE'
+            db_path = self._in_data_dir("universe.sqlite")
+            self.database_connection = f"sqlite:///{db_path}?isolation_level=IMMEDIATE"
         self.database_engine_options = get_database_engine_options(kwargs)
-        self.database_create_tables = string_as_bool(kwargs.get('database_create_tables', 'True'))
-        self.database_encoding = kwargs.get('database_encoding')  # Create new databases with this encoding
+        self.database_encoding = kwargs.get("database_encoding")  # Create new databases with this encoding
         self.thread_local_log = None
         if self.enable_per_request_sql_debugging:
             self.thread_local_log = threading.local()
         # Install database related configuration (if different)
         self.install_database_engine_options = get_database_engine_options(kwargs, model_prefix="install_")
         self.shared_home_dir = kwargs.get("shared_home_dir")
         self.cookie_path = kwargs.get("cookie_path")
         self.tool_path = self._in_root_dir(self.tool_path)
         self.tool_data_path = self._in_root_dir(self.tool_data_path)
         if not running_from_source and kwargs.get("tool_data_path") is None:
-            self.tool_data_path = self._in_data_dir(self.schema.defaults['tool_data_path'])
+            self.tool_data_path = self._in_data_dir(self.schema.defaults["tool_data_path"])
         self.builds_file_path = os.path.join(self.tool_data_path, self.builds_file_path)
         self.len_file_path = os.path.join(self.tool_data_path, self.len_file_path)
-        self.oidc = {}
+        self.oidc: Dict[str, Dict] = {}
         self.integrated_tool_panel_config = self._in_managed_config_dir(self.integrated_tool_panel_config)
-        integrated_tool_panel_tracking_directory = kwargs.get('integrated_tool_panel_tracking_directory')
+        integrated_tool_panel_tracking_directory = kwargs.get("integrated_tool_panel_tracking_directory")
         if integrated_tool_panel_tracking_directory:
             self.integrated_tool_panel_tracking_directory = self._in_root_dir(integrated_tool_panel_tracking_directory)
         else:
             self.integrated_tool_panel_tracking_directory = None
         self.toolbox_filter_base_modules = listify(self.toolbox_filter_base_modules)
         self.tool_filters = listify(self.tool_filters, do_strip=True)
         self.tool_label_filters = listify(self.tool_label_filters, do_strip=True)
         self.tool_section_filters = listify(self.tool_section_filters, do_strip=True)
 
         self.user_tool_filters = listify(self.user_tool_filters, do_strip=True)
         self.user_tool_label_filters = listify(self.user_tool_label_filters, do_strip=True)
         self.user_tool_section_filters = listify(self.user_tool_section_filters, do_strip=True)
-        self.has_user_tool_filters = bool(self.user_tool_filters or self.user_tool_label_filters or self.user_tool_section_filters)
-
-        self.password_expiration_period = timedelta(
-            days=int(cast(SupportsInt, self.password_expiration_period))
+        self.has_user_tool_filters = bool(
+            self.user_tool_filters or self.user_tool_label_filters or self.user_tool_section_filters
         )
 
+        self.password_expiration_period = timedelta(days=int(cast(SupportsInt, self.password_expiration_period)))
+
         if self.shed_tool_data_path:
             self.shed_tool_data_path = self._in_root_dir(self.shed_tool_data_path)
         else:
             self.shed_tool_data_path = self.tool_data_path
 
-        self.running_functional_tests = string_as_bool(kwargs.get('running_functional_tests', False))
+        self.running_functional_tests = string_as_bool(kwargs.get("running_functional_tests", False))
         if isinstance(self.hours_between_check, str):
             self.hours_between_check = float(self.hours_between_check)
         try:
             if isinstance(self.hours_between_check, int):
                 if self.hours_between_check < 1 or self.hours_between_check > 24:
                     self.hours_between_check = 12
             elif isinstance(self.hours_between_check, float):
@@ -806,217 +881,233 @@
         self.update_integrated_tool_panel = kwargs.get("update_integrated_tool_panel", True)
         self.galaxy_data_manager_data_path = self.galaxy_data_manager_data_path or self.tool_data_path
         self.tool_secret = kwargs.get("tool_secret", "")
         self.metadata_strategy = kwargs.get("metadata_strategy", "directory")
         self.use_remote_user = self.use_remote_user or self.single_user
         self.fetch_url_allowlist_ips = [
             ipaddress.ip_network(unicodify(ip.strip()))  # If it has a slash, assume 127.0.0.1/24 notation
-            if '/' in ip else
-            ipaddress.ip_address(unicodify(ip.strip()))  # Otherwise interpret it as an ip address.
-            for ip in kwargs.get("fetch_url_allowlist", "").split(',')
+            if "/" in ip
+            else ipaddress.ip_address(unicodify(ip.strip()))  # Otherwise interpret it as an ip address.
+            for ip in kwargs.get("fetch_url_allowlist", "").split(",")
             if len(ip.strip()) > 0
         ]
         self.job_queue_cleanup_interval = int(kwargs.get("job_queue_cleanup_interval", "5"))
-        self.cluster_files_directory = self._in_root_dir(self.cluster_files_directory)
 
         # Fall back to legacy job_working_directory config variable if set.
         self.jobs_directory = self._in_data_dir(kwargs.get("jobs_directory", self.job_working_directory))
         if self.preserve_python_environment not in ["legacy_only", "legacy_and_local", "always"]:
             log.warning("preserve_python_environment set to unknown value [%s], defaulting to legacy_only")
             self.preserve_python_environment = "legacy_only"
         self.nodejs_path = kwargs.get("nodejs_path")
         self.container_image_cache_path = self._in_data_dir(kwargs.get("container_image_cache_path", "container_cache"))
-        self.output_size_limit = int(kwargs.get('output_size_limit', 0))
+        self.output_size_limit = int(kwargs.get("output_size_limit", 0))
         # activation_email was used until release_15.03
-        activation_email = kwargs.get('activation_email')
-        self.email_from = self.email_from or activation_email
+        self.email_from = self.email_from or kwargs.get("activation_email")
 
-        self.email_domain_blocklist_content = self._load_list_from_file(self._in_config_dir(self.email_domain_blocklist_file)) if self.email_domain_blocklist_file else None
-        self.email_domain_allowlist_content = self._load_list_from_file(self._in_config_dir(self.email_domain_allowlist_file)) if self.email_domain_allowlist_file else None
+        self.email_domain_blocklist_content = (
+            self._load_list_from_file(self._in_config_dir(self.email_domain_blocklist_file))
+            if self.email_domain_blocklist_file
+            else None
+        )
+        self.email_domain_allowlist_content = (
+            self._load_list_from_file(self._in_config_dir(self.email_domain_allowlist_file))
+            if self.email_domain_allowlist_file
+            else None
+        )
 
         # These are not even beta - just experiments - don't use them unless
         # you want yours tools to be broken in the future.
-        self.enable_beta_tool_formats = string_as_bool(kwargs.get('enable_beta_tool_formats', 'False'))
+        self.enable_beta_tool_formats = string_as_bool(kwargs.get("enable_beta_tool_formats", "False"))
 
-        if self.workflow_resource_params_mapper and ':' not in self.workflow_resource_params_mapper:
+        if self.workflow_resource_params_mapper and ":" not in self.workflow_resource_params_mapper:
             # Assume it is not a Python function, so a file; else: a Python function
             self.workflow_resource_params_mapper = self._in_root_dir(self.workflow_resource_params_mapper)
 
-        self.pbs_application_server = kwargs.get('pbs_application_server', "")
-        self.pbs_dataset_server = kwargs.get('pbs_dataset_server', "")
-        self.pbs_dataset_path = kwargs.get('pbs_dataset_path', "")
-        self.pbs_stage_path = kwargs.get('pbs_stage_path', "")
+        self.pbs_application_server = kwargs.get("pbs_application_server", "")
+        self.pbs_dataset_server = kwargs.get("pbs_dataset_server", "")
+        self.pbs_dataset_path = kwargs.get("pbs_dataset_path", "")
+        self.pbs_stage_path = kwargs.get("pbs_stage_path", "")
 
         _sanitize_allowlist_path = self._in_managed_config_dir(self.sanitize_allowlist_file)
         if not os.path.isfile(_sanitize_allowlist_path):  # then check old default location
             for deprecated in (
-                    self._in_managed_config_dir('sanitize_whitelist.txt'),
-                    self._in_root_dir('config/sanitize_whitelist.txt')):
+                self._in_managed_config_dir("sanitize_whitelist.txt"),
+                self._in_root_dir("config/sanitize_whitelist.txt"),
+            ):
                 if os.path.isfile(deprecated):
-                    log.warning("The path '%s' for the 'sanitize_allowlist_file' config option is "
+                    log.warning(
+                        "The path '%s' for the 'sanitize_allowlist_file' config option is "
                         "deprecated and will be no longer checked in a future release. Please consult "
-                        "the latest version of the sample configuration file." % deprecated)
+                        "the latest version of the sample configuration file." % deprecated
+                    )
                     _sanitize_allowlist_path = deprecated
                     break
         self.sanitize_allowlist_file = _sanitize_allowlist_path
 
         self.allowed_origin_hostnames = self._parse_allowed_origin_hostnames(self.allowed_origin_hostnames)
         if "trust_jupyter_notebook_conversion" not in kwargs:
             # if option not set, check IPython-named alternative, falling back to schema default if not set either
             _default = self.trust_jupyter_notebook_conversion
-            self.trust_jupyter_notebook_conversion = string_as_bool(kwargs.get('trust_ipython_notebook_conversion', _default))
+            self.trust_jupyter_notebook_conversion = string_as_bool(
+                kwargs.get("trust_ipython_notebook_conversion", _default)
+            )
         # Configuration for the message box directly below the masthead.
-        self.blog_url = kwargs.get('blog_url')
+        self.blog_url = kwargs.get("blog_url")
         self.user_library_import_symlink_allowlist = listify(self.user_library_import_symlink_allowlist, do_strip=True)
-        self.user_library_import_dir_auto_creation = self.user_library_import_dir_auto_creation if self.user_library_import_dir else False
+        self.user_library_import_dir_auto_creation = (
+            self.user_library_import_dir_auto_creation if self.user_library_import_dir else False
+        )
         # Searching data libraries
-        self.ftp_upload_dir_template = kwargs.get('ftp_upload_dir_template', '${ftp_upload_dir}%s${ftp_upload_dir_identifier}' % os.path.sep)
+        self.ftp_upload_dir_template = kwargs.get(
+            "ftp_upload_dir_template", "${ftp_upload_dir}%s${ftp_upload_dir_identifier}" % os.path.sep
+        )
         # Support older library-specific path paste option but just default to the new
         # allow_path_paste value.
-        self.allow_library_path_paste = string_as_bool(kwargs.get('allow_library_path_paste', self.allow_path_paste))
-        self.disable_library_comptypes = kwargs.get('disable_library_comptypes', '').lower().split(',')
-        self.check_upload_content = string_as_bool(kwargs.get('check_upload_content', True))
+        self.allow_library_path_paste = string_as_bool(kwargs.get("allow_library_path_paste", self.allow_path_paste))
+        self.disable_library_comptypes = kwargs.get("disable_library_comptypes", "").lower().split(",")
+        self.check_upload_content = string_as_bool(kwargs.get("check_upload_content", True))
         # On can mildly speed up Galaxy startup time by disabling index of help,
         # not needed on production systems but useful if running many functional tests.
         self.index_tool_help = string_as_bool(kwargs.get("index_tool_help", True))
         self.tool_labels_boost = kwargs.get("tool_labels_boost", 1)
         default_tool_test_data_directories = os.environ.get("GALAXY_TEST_FILE_DIR", self._in_root_dir("test-data"))
         self.tool_test_data_directories = kwargs.get("tool_test_data_directories", default_tool_test_data_directories)
         # Deployers may either specify a complete list of mapping files or get the default for free and just
         # specify a local mapping file to adapt and extend the default one.
         if "conda_mapping_files" not in kwargs:
-            _default_mapping = self._in_root_dir(os.path.join("lib", "galaxy", "tool_util", "deps", "resolvers", "default_conda_mapping.yml"))
+            _default_mapping = self._in_root_dir(
+                os.path.join("lib", "galaxy", "tool_util", "deps", "resolvers", "default_conda_mapping.yml")
+            )
             # dependency resolution options are consumed via config_dict - so don't populate
             # self, populate config_dict
             self.config_dict["conda_mapping_files"] = [self.local_conda_mapping_file, _default_mapping]
 
         if self.container_resolvers_config_file:
             self.container_resolvers_config_file = self._in_config_dir(self.container_resolvers_config_file)
 
         # tool_dependency_dir can be "none" (in old configs). If so, set it to None
-        if self.tool_dependency_dir and self.tool_dependency_dir.lower() == 'none':
+        if self.tool_dependency_dir and self.tool_dependency_dir.lower() == "none":
             self.tool_dependency_dir = None
-        if self.involucro_path is None:
-            target_dir = self.tool_dependency_dir or self.schema.defaults['tool_dependency_dir']
-            self.involucro_path = self._in_data_dir(os.path.join(target_dir, "involucro"))
-        self.involucro_path = self._in_root_dir(self.involucro_path)
         if self.mulled_channels:
             self.mulled_channels = [c.strip() for c in self.mulled_channels.split(",")]  # type: ignore[attr-defined]
 
-        default_job_resubmission_condition = kwargs.get('default_job_resubmission_condition', '')
+        default_job_resubmission_condition = kwargs.get("default_job_resubmission_condition", "")
         if not default_job_resubmission_condition.strip():
             default_job_resubmission_condition = None
         self.default_job_resubmission_condition = default_job_resubmission_condition
 
         # Configuration options for taking advantage of nginx features
         if self.nginx_upload_store:
             self.nginx_upload_store = os.path.abspath(self.nginx_upload_store)
 
         if self.tus_upload_store:
             self.tus_upload_store = os.path.abspath(self.tus_upload_store)
 
-        self.object_store = kwargs.get('object_store', 'disk')
-        self.object_store_check_old_style = string_as_bool(kwargs.get('object_store_check_old_style', False))
-        self.object_store_cache_path = self._in_root_dir(kwargs.get("object_store_cache_path", self._in_data_dir("object_store_cache")))
+        self.object_store = kwargs.get("object_store", "disk")
+        self.object_store_check_old_style = string_as_bool(kwargs.get("object_store_check_old_style", False))
+        self.object_store_cache_path = self._in_root_dir(
+            kwargs.get("object_store_cache_path", self._in_data_dir("object_store_cache"))
+        )
         self._configure_dataset_storage()
 
         # Handle AWS-specific config options for backward compatibility
-        if kwargs.get('aws_access_key') is not None:
-            self.os_access_key = kwargs.get('aws_access_key')
-            self.os_secret_key = kwargs.get('aws_secret_key')
-            self.os_bucket_name = kwargs.get('s3_bucket')
-            self.os_use_reduced_redundancy = kwargs.get('use_reduced_redundancy', False)
+        if kwargs.get("aws_access_key") is not None:
+            self.os_access_key = kwargs.get("aws_access_key")
+            self.os_secret_key = kwargs.get("aws_secret_key")
+            self.os_bucket_name = kwargs.get("s3_bucket")
+            self.os_use_reduced_redundancy = kwargs.get("use_reduced_redundancy", False)
         else:
-            self.os_access_key = kwargs.get('os_access_key')
-            self.os_secret_key = kwargs.get('os_secret_key')
-            self.os_bucket_name = kwargs.get('os_bucket_name')
-            self.os_use_reduced_redundancy = kwargs.get('os_use_reduced_redundancy', False)
-        self.os_host = kwargs.get('os_host')
-        self.os_port = kwargs.get('os_port')
-        self.os_is_secure = string_as_bool(kwargs.get('os_is_secure', True))
-        self.os_conn_path = kwargs.get('os_conn_path', '/')
-        self.object_store_cache_size = float(kwargs.get('object_store_cache_size', -1))
-        self.distributed_object_store_config_file = kwargs.get('distributed_object_store_config_file')
+            self.os_access_key = kwargs.get("os_access_key")
+            self.os_secret_key = kwargs.get("os_secret_key")
+            self.os_bucket_name = kwargs.get("os_bucket_name")
+            self.os_use_reduced_redundancy = kwargs.get("os_use_reduced_redundancy", False)
+        self.os_host = kwargs.get("os_host")
+        self.os_port = kwargs.get("os_port")
+        self.os_is_secure = string_as_bool(kwargs.get("os_is_secure", True))
+        self.os_conn_path = kwargs.get("os_conn_path", "/")
+        self.object_store_cache_size = float(kwargs.get("object_store_cache_size", -1))
+        self.distributed_object_store_config_file = kwargs.get("distributed_object_store_config_file")
         if self.distributed_object_store_config_file is not None:
             self.distributed_object_store_config_file = self._in_root_dir(self.distributed_object_store_config_file)
-        self.irods_root_collection_path = kwargs.get('irods_root_collection_path')
-        self.irods_default_resource = kwargs.get('irods_default_resource')
+        self.irods_root_collection_path = kwargs.get("irods_root_collection_path")
+        self.irods_default_resource = kwargs.get("irods_default_resource")
         # Heartbeat log file name override
-        if self.global_conf is not None and 'heartbeat_log' in self.global_conf:
-            self.heartbeat_log = self.global_conf['heartbeat_log']
+        if self.global_conf is not None and "heartbeat_log" in self.global_conf:
+            self.heartbeat_log = self.global_conf["heartbeat_log"]
         # Determine which 'server:' this is
-        self.server_name = 'main'
+        self.server_name = "main"
         for arg in sys.argv:
             # Crummy, but PasteScript does not give you a way to determine this
-            if arg.lower().startswith('--server-name='):
-                self.server_name = arg.split('=', 1)[-1]
+            if arg.lower().startswith("--server-name="):
+                self.server_name = arg.split("=", 1)[-1]
         # Allow explicit override of server name in config params
         if "server_name" in kwargs:
-            self.server_name = kwargs.get("server_name")
+            self.server_name = kwargs["server_name"]
         # The application stack code may manipulate the server name. It also needs to be accessible via the get() method
         # for galaxy.util.facts()
-        self.config_dict['base_server_name'] = self.base_server_name = self.server_name
+        self.config_dict["base_server_name"] = self.base_server_name = self.server_name
         # Store all configured server names for the message queue routing
         self.server_names = []
         for section in self.global_conf_parser.sections():
-            if section.startswith('server:'):
-                self.server_names.append(section.replace('server:', '', 1))
+            if section.startswith("server:"):
+                self.server_names.append(section.replace("server:", "", 1))
 
         self._set_galaxy_infrastructure_url(kwargs)
 
         # Asynchronous execution process pools - limited functionality for now, attach_to_pools is designed to allow
         # webless Galaxy server processes to attach to arbitrary message queues (e.g. as job handlers) so they do not
         # have to be explicitly defined as such in the job configuration.
-        self.attach_to_pools = kwargs.get('attach_to_pools', []) or []
+        self.attach_to_pools = kwargs.get("attach_to_pools", []) or []
 
         # Store advanced job management config
-        self.job_handlers = [x.strip() for x in kwargs.get('job_handlers', self.server_name).split(',')]
-        self.default_job_handlers = [x.strip() for x in kwargs.get('default_job_handlers', ','.join(self.job_handlers)).split(',')]
+        self.job_handlers = [x.strip() for x in kwargs.get("job_handlers", self.server_name).split(",")]
+        self.default_job_handlers = [
+            x.strip() for x in kwargs.get("default_job_handlers", ",".join(self.job_handlers)).split(",")
+        ]
         # Galaxy internal control queue configuration.
         # If specified in universe, use it, otherwise we use whatever 'real'
         # database is specified.  Lastly, we create and use new sqlite database
         # (to minimize locking) as a final option.
-        if 'amqp_internal_connection' in kwargs:
-            self.amqp_internal_connection = kwargs.get('amqp_internal_connection')
+        if "amqp_internal_connection" in kwargs:
+            self.amqp_internal_connection = kwargs.get("amqp_internal_connection")
             # TODO Get extra amqp args as necessary for ssl
-        elif 'database_connection' in kwargs:
+        elif "database_connection" in kwargs:
             self.amqp_internal_connection = f"sqlalchemy+{self.database_connection}"
         else:
-            self.amqp_internal_connection = f"sqlalchemy+sqlite:///{self._in_data_dir('control.sqlite')}?isolation_level=IMMEDIATE"
+            self.amqp_internal_connection = (
+                f"sqlalchemy+sqlite:///{self._in_data_dir('control.sqlite')}?isolation_level=IMMEDIATE"
+            )
         self.pretty_datetime_format = expand_pretty_datetime_format(self.pretty_datetime_format)
         try:
             with open(self.user_preferences_extra_conf_path) as stream:
                 self.user_preferences_extra = yaml.safe_load(stream)
         except Exception:
-            if self.is_set('user_preferences_extra_conf_path'):
-                log.warning(f'Config file ({self.user_preferences_extra_conf_path}) could not be found or is malformed.')
-            self.user_preferences_extra = {'preferences': {}}
+            if self.is_set("user_preferences_extra_conf_path"):
+                log.warning(
+                    f"Config file ({self.user_preferences_extra_conf_path}) could not be found or is malformed."
+                )
+            self.user_preferences_extra = {"preferences": {}}
 
         # Experimental: This will not be enabled by default and will hide
         # nonproduction code.
         # The api_folders refers to whether the API exposes the /folders section.
-        self.api_folders = string_as_bool(kwargs.get('api_folders', False))
+        self.api_folders = string_as_bool(kwargs.get("api_folders", False))
         # This is for testing new library browsing capabilities.
-        self.new_lib_browse = string_as_bool(kwargs.get('new_lib_browse', False))
+        self.new_lib_browse = string_as_bool(kwargs.get("new_lib_browse", False))
         # Logging configuration with logging.config.configDict:
         # Statistics and profiling with statsd
-        self.statsd_host = kwargs.get('statsd_host', '')
-
-        ie_dirs = self.interactive_environment_plugins_directory
-        self.gie_dirs = [d.strip() for d in (ie_dirs.split(",") if ie_dirs else [])]
-        if ie_dirs:
-            self.visualization_plugins_directory += f",{ie_dirs}"
+        self.statsd_host = kwargs.get("statsd_host", "")
 
         self.proxy_session_map = self.dynamic_proxy_session_map
         self.manage_dynamic_proxy = self.dynamic_proxy_manage  # Set to false if being launched externally
 
         # InteractiveTools propagator mapping file
-        self.interactivetools_map = self._in_root_dir(kwargs.get("interactivetools_map", self._in_data_dir("interactivetools_map.sqlite")))
-
-        self.containers_conf = parse_containers_config(self.containers_config_file)
+        self.interactivetools_map = self._in_root_dir(
+            kwargs.get("interactivetools_map", self._in_data_dir("interactivetools_map.sqlite"))
+        )
 
         # Compliance/Policy variables
         self.redact_username_during_deletion = False
         self.redact_email_during_deletion = False
         self.redact_ip_address = False
         self.redact_username_in_logs = False
         self.redact_email_in_job_name = False
@@ -1033,107 +1124,131 @@
             self.redact_ip_address = True
             self.redact_username_in_logs = True
             self.redact_email_in_job_name = True
             self.redact_user_details_in_bugreport = True
             self.redact_user_address_during_deletion = True
             self.allow_user_deletion = True
 
-            LOGGING_CONFIG_DEFAULT['formatters']['brief'] = {
-                'format': '%(asctime)s %(levelname)-8s %(name)-15s %(message)s'
+            LOGGING_CONFIG_DEFAULT["formatters"]["brief"] = {
+                "format": "%(asctime)s %(levelname)-8s %(name)-15s %(message)s"
             }
-            LOGGING_CONFIG_DEFAULT['handlers']['compliance_log'] = {
-                'class': 'logging.handlers.RotatingFileHandler',
-                'formatter': 'brief',
-                'filename': 'compliance.log',
-                'backupCount': 0,
+            LOGGING_CONFIG_DEFAULT["handlers"]["compliance_log"] = {
+                "class": "logging.handlers.RotatingFileHandler",
+                "formatter": "brief",
+                "filename": "compliance.log",
+                "backupCount": 0,
             }
-            LOGGING_CONFIG_DEFAULT['loggers']['COMPLIANCE'] = {
-                'handlers': ['compliance_log'],
-                'level': 'DEBUG',
-                'qualname': 'COMPLIANCE'
+            LOGGING_CONFIG_DEFAULT["loggers"]["COMPLIANCE"] = {
+                "handlers": ["compliance_log"],
+                "level": "DEBUG",
+                "qualname": "COMPLIANCE",
             }
 
         log_destination = kwargs.get("log_destination")
-        galaxy_daemon_log_destination = os.environ.get('GALAXY_DAEMON_LOG')
+        log_rotate_size = size_to_bytes(unicodify(kwargs.get("log_rotate_size", 0)))
+        log_rotate_count = int(kwargs.get("log_rotate_count", 0))
+        galaxy_daemon_log_destination = os.environ.get("GALAXY_DAEMON_LOG")
         if log_destination == "stdout":
-            LOGGING_CONFIG_DEFAULT['handlers']['console'] = {
-                'class': 'logging.StreamHandler',
-                'formatter': 'stack',
-                'level': 'DEBUG',
-                'stream': 'ext://sys.stdout',
-                'filters': ['stack']
+            LOGGING_CONFIG_DEFAULT["handlers"]["console"] = {
+                "class": "logging.StreamHandler",
+                "formatter": "stack",
+                "level": "DEBUG",
+                "stream": "ext://sys.stdout",
+                "filters": ["stack"],
             }
         elif log_destination:
-            LOGGING_CONFIG_DEFAULT['handlers']['console'] = {
-                'class': 'logging.FileHandler',
-                'formatter': 'stack',
-                'level': 'DEBUG',
-                'filename': log_destination,
-                'filters': ['stack']
+            LOGGING_CONFIG_DEFAULT["handlers"]["console"] = {
+                "class": "logging.handlers.RotatingFileHandler",
+                "formatter": "stack",
+                "level": "DEBUG",
+                "filename": log_destination,
+                "filters": ["stack"],
+                "maxBytes": log_rotate_size,
+                "backupCount": log_rotate_count,
             }
         if galaxy_daemon_log_destination:
-            LOGGING_CONFIG_DEFAULT['handlers']['files'] = {
-                'class': 'logging.FileHandler',
-                'formatter': 'stack',
-                'level': 'DEBUG',
-                'filename': galaxy_daemon_log_destination,
-                'filters': ['stack']
+            LOGGING_CONFIG_DEFAULT["handlers"]["files"] = {
+                "class": "logging.handlers.RotatingFileHandler",
+                "formatter": "stack",
+                "level": "DEBUG",
+                "filename": galaxy_daemon_log_destination,
+                "filters": ["stack"],
+                "maxBytes": log_rotate_size,
+                "backupCount": log_rotate_count,
             }
-            LOGGING_CONFIG_DEFAULT['root']['handlers'].append('files')
+            LOGGING_CONFIG_DEFAULT["root"]["handlers"].append("files")
+
+        # Load and flatten themes into css variables
+        def _load_theme(path: str, theme_dict: dict):
+            if self._path_exists(path):
+                with open(path) as f:
+                    themes = yaml.safe_load(f)
+                    for key, val in themes.items():
+                        theme_dict[key] = flatten_theme(val)
+
+        self.themes = {}
+
+        if "themes_config_file_by_host" in self.config_dict:
+            self.themes_by_host = {}
+            resolve_to_dir = self.schema.paths_to_resolve["themes_config_file"]
+            resolve_dir_path = getattr(self, resolve_to_dir)
+            for host, file_name in self.config_dict["themes_config_file_by_host"].items():
+                self.themes_by_host[host] = {}
+                file_path = self._in_dir(resolve_dir_path, file_name)
+                _load_theme(file_path, self.themes_by_host[host])
+        else:
+            _load_theme(self.themes_config_file, self.themes)
 
     def _configure_dataset_storage(self):
         # The default for `file_path` has changed in 20.05; we may need to fall back to the old default
-        self._set_alt_paths('file_path', self._in_data_dir('files'))  # this is called BEFORE guessing id/uuid
-        ID, UUID = 'id', 'uuid'
-        if self.is_set('object_store_store_by'):
+        self._set_alt_paths("file_path", self._in_data_dir("files"))  # this is called BEFORE guessing id/uuid
+        ID, UUID = "id", "uuid"
+        if self.is_set("object_store_store_by"):
             if self.object_store_store_by not in [ID, UUID]:
-                raise Exception(
-                    f"Invalid value for object_store_store_by [{self.object_store_store_by}]"
-                )
+                raise Exception(f"Invalid value for object_store_store_by [{self.object_store_store_by}]")
         elif os.path.basename(self.file_path) == "objects":
             self.object_store_store_by = UUID
         else:
             self.object_store_store_by = ID
 
     def _load_list_from_file(self, filepath):
         with open(filepath) as f:
             return [line.strip() for line in f]
 
     def _set_galaxy_infrastructure_url(self, kwargs):
         # indicate if this was not set explicitly, so dependending on the context a better default
         # can be used (request url in a web thread, Docker parent in IE stuff, etc.)
-        self.galaxy_infrastructure_url_set = kwargs.get('galaxy_infrastructure_url') is not None
+        self.galaxy_infrastructure_url_set = kwargs.get("galaxy_infrastructure_url") is not None
         if "HOST_IP" in self.galaxy_infrastructure_url:
-            self.galaxy_infrastructure_url = string.Template(self.galaxy_infrastructure_url).safe_substitute({
-                'HOST_IP': socket.gethostbyname(socket.gethostname())
-            })
+            self.galaxy_infrastructure_url = string.Template(self.galaxy_infrastructure_url).safe_substitute(
+                {"HOST_IP": socket.gethostbyname(socket.gethostname())}
+            )
         if "GALAXY_WEB_PORT" in self.galaxy_infrastructure_url:
-            port = os.environ.get('GALAXY_WEB_PORT')
+            port = os.environ.get("GALAXY_WEB_PORT")
             if not port:
-                raise Exception('$GALAXY_WEB_PORT set in galaxy_infrastructure_url, but environment variable not set')
-            self.galaxy_infrastructure_url = string.Template(self.galaxy_infrastructure_url).safe_substitute({
-                'GALAXY_WEB_PORT': port
-            })
+                raise Exception("$GALAXY_WEB_PORT set in galaxy_infrastructure_url, but environment variable not set")
+            self.galaxy_infrastructure_url = string.Template(self.galaxy_infrastructure_url).safe_substitute(
+                {"GALAXY_WEB_PORT": port}
+            )
         if "UWSGI_PORT" in self.galaxy_infrastructure_url:
-            import uwsgi
-            http = unicodify(uwsgi.opt['http'])
-            host, port = http.split(":", 1)
-            assert port, "galaxy_infrastructure_url depends on dynamic PORT determination but port unknown"
-            self.galaxy_infrastructure_url = string.Template(self.galaxy_infrastructure_url).safe_substitute({
-                'UWSGI_PORT': port
-            })
+            raise Exception("UWSGI_PORT is not supported anymore")
 
     def reload_sanitize_allowlist(self, explicit=True):
         self.sanitize_allowlist = []
         if not os.path.exists(self.sanitize_allowlist_file):
             if explicit:
-                log.warning("Sanitize log file explicitly specified as '%s' but does not exist, continuing with no tools allowlisted.", self.sanitize_allowlist_file)
+                log.warning(
+                    "Sanitize log file explicitly specified as '%s' but does not exist, continuing with no tools allowlisted.",
+                    self.sanitize_allowlist_file,
+                )
         else:
             with open(self.sanitize_allowlist_file) as f:
-                self.sanitize_allowlist = sorted(line.strip() for line in f.readlines() if line.strip() and not line.startswith('#'))
+                self.sanitize_allowlist = sorted(
+                    line.strip() for line in f.readlines() if line.strip() and not line.startswith("#")
+                )
 
     def ensure_tempdir(self):
         self._ensure_directory(self.new_file_path)
 
     def check(self):
         # Check that required directories exist; attempt to create otherwise
         paths_to_check = [
@@ -1158,29 +1273,42 @@
                 raise ConfigurationError(f"Tool config file not found: {path}")
         for datatypes_config in listify(self.datatypes_config):
             if not os.path.isfile(datatypes_config):
                 raise ConfigurationError(f"Datatypes config file not found: {datatypes_config}")
         # Check for deprecated options.
         for key in self.config_dict.keys():
             if key in self.deprecated_options:
-                log.warning(f"Config option '{key}' is deprecated and will be removed in a future release.  Please consult the latest version of the sample configuration file.")
+                log.warning(
+                    f"Config option '{key}' is deprecated and will be removed in a future release.  Please consult the latest version of the sample configuration file."
+                )
+
+    def is_fetch_with_celery_enabled(self):
+        """
+        True iff celery is enabled and celery_conf["task_routes"]["galaxy.fetch_data"] != DISABLED_FLAG.
+        """
+        celery_enabled = self.enable_celery_tasks
+        try:
+            fetch_disabled = self.celery_conf["task_routes"]["galaxy.fetch_data"] == DISABLED_FLAG
+        except (TypeError, KeyError):  # celery_conf is None or sub-dictionary is none or either key is not present
+            fetch_disabled = False
+        return celery_enabled and not fetch_disabled
 
     @staticmethod
     def _parse_allowed_origin_hostnames(allowed_origin_hostnames):
         """
         Parse a CSV list of strings/regexp of hostnames that should be allowed
         to use CORS and will be sent the Access-Control-Allow-Origin header.
         """
         allowed_origin_hostnames_list = listify(allowed_origin_hostnames)
         if not allowed_origin_hostnames_list:
             return None
 
         def parse(string):
             # a string enclosed in fwd slashes will be parsed as a regexp: e.g. /<some val>/
-            if string[0] == '/' and string[-1] == '/':
+            if string[0] == "/" and string[-1] == "/":
                 string = string[1:-1]
                 return re.compile(string, flags=(re.UNICODE))
             return string
 
         return [parse(v) for v in allowed_origin_hostnames_list if v]
 
 
@@ -1193,32 +1321,32 @@
     modified_config = read_properties_from_file(current_config.config_file)
     for option in current_config.schema.reloadable_options:
         if option in modified_config:
             # compare to raw value, as that one is set only on load and reload
             if current_config._raw_config[option] != modified_config[option]:
                 current_config._raw_config[option] = modified_config[option]
                 setattr(current_config, option, modified_config[option])
-                log.info(f'Reloaded {option}')
+                log.info(f"Reloaded {option}")
 
 
-def get_database_engine_options(kwargs, model_prefix=''):
+def get_database_engine_options(kwargs, model_prefix=""):
     """
     Allow options for the SQLAlchemy database engine to be passed by using
     the prefix "database_engine_option".
     """
     conversions: Dict[str, Callable[[Any], Union[bool, int]]] = {
-        'convert_unicode': string_as_bool,
-        'pool_timeout': int,
-        'echo': string_as_bool,
-        'echo_pool': string_as_bool,
-        'pool_recycle': int,
-        'pool_size': int,
-        'max_overflow': int,
-        'pool_threadlocal': string_as_bool,
-        'server_side_cursors': string_as_bool
+        "convert_unicode": string_as_bool,
+        "pool_timeout": int,
+        "echo": string_as_bool,
+        "echo_pool": string_as_bool,
+        "pool_recycle": int,
+        "pool_size": int,
+        "max_overflow": int,
+        "pool_threadlocal": string_as_bool,
+        "server_side_cursors": string_as_bool,
     }
     prefix = f"{model_prefix}database_engine_option_"
     prefix_len = len(prefix)
     rval = {}
     for key, value in kwargs.items():
         if key.startswith(prefix):
             key = key[prefix_len:]
```

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/auth_conf.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/auth_conf.xml.sample`

 * *Files 4% similar despite different names*

#### Comparing `galaxy-config-22.1.1/galaxy/config/sample/auth_conf.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/auth_conf.xml.sample`

```diff
@@ -18,14 +18,19 @@
                  successful authentication). Default is True. -->
   <!--        <allow-register>False</allow-register>
 -->
   <!-- Whether Galaxy should automatically register users when they
                  first login. Default is False. -->
   <!--        <auto-register>True</auto-register>
 -->
+  <!-- How often Galaxy should retry to validate a user-name: 
+                 If a username is invalid (already taken, too short, too long, non-alphanumeric + '_-')
+                 Galaxy tries again with username+"-i" for i<= max-retries. -->
+  <!--        <max-retries>10</max-retries>
+-->
   <!-- Whether users are allowed to change their password. Default is
                  False. -->
   <!--        <allow-password-change>False</allow-password-change>
 -->
   <!-- Whether roles should be automatically created if
                  the attribute specified under auto-register-roles can be found.
                  Default is False. -->
@@ -46,15 +51,17 @@
   <!--        <server>ldap://dc1.example.com</server>
 -->
   <!-- Additional options for the LDAP connection. The syntax is:
                  option1=value1,option2=value2,...
                  Options and values should match those from the python-ldap
                  documentation.
                  The following example allows connecting to ldaps:// (SSL/TLS)
-                 when self-signed certificates are used -->
+                 when self-signed certificates are used 
+                 These options are valid only if ldap provider is used. 
+                 For ldap3 none of these options are used-->
   <!--        <ldap-options>OPT_X_TLS_REQUIRE_CERT=OPT_X_TLS_ALLOW</ldap-options>
 -->
   <!-- Whether unregistered users should use their LDAP username
                  instead of the email at their first login when auto-register is
                  True. Default is False. -->
   <!--        <login-use-username>False</login-use-username>
 -->
```

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/build_sites.yml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/build_sites.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/container_resolvers_conf.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/container_resolvers_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/datatypes_conf.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/datatypes_conf.xml.sample`

 * *Files 1% similar despite different names*

#### Comparing `galaxy-config-22.1.1/galaxy/config/sample/datatypes_conf.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/datatypes_conf.xml.sample`

```diff
@@ -24,16 +24,16 @@
     <datatype extension="anvio_profile_db" type="galaxy.datatypes.anvio:AnvioProfileDB" display_in_upload="false"/>
     <datatype extension="anvio_samples_db" type="galaxy.datatypes.anvio:AnvioSamplesDB" display_in_upload="false"/>
     <datatype extension="anvio_state" type="galaxy.datatypes.text:Json" mimetype="application/json" subclass="true" display_in_upload="false"/>
     <datatype extension="anvio_structure_db" type="galaxy.datatypes.anvio:AnvioStructureDB" display_in_upload="false"/>
     <datatype extension="anvio_variability" type="galaxy.datatypes.tabular:TSV" display_in_upload="false" subclass="true"/>
     <datatype extension="arff" type="galaxy.datatypes.text:Arff" mimetype="text/plain" display_in_upload="true"/>
     <datatype extension="paf" auto_compressed_types="gz" type="galaxy.datatypes.text:Paf" mimetype="text/plain" display_in_upload="true"/>
-    <datatype extension="gfa1" type="galaxy.datatypes.text:Gfa1" mimetype="text/plain" display_in_upload="true"/>
-    <datatype extension="gfa2" type="galaxy.datatypes.text:Gfa2" mimetype="text/plain" display_in_upload="true"/>
+    <datatype extension="gfa1" auto_compressed_types="gz" type="galaxy.datatypes.text:Gfa1" mimetype="text/plain" display_in_upload="true"/>
+    <datatype extension="gfa2" auto_compressed_types="gz" type="galaxy.datatypes.text:Gfa2" mimetype="text/plain" display_in_upload="true"/>
     <datatype extension="asn1" type="galaxy.datatypes.data:GenericAsn1" mimetype="text/plain" display_in_upload="true"/>
     <datatype extension="asn1-binary" type="galaxy.datatypes.binary:GenericAsn1Binary" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="axt" type="galaxy.datatypes.sequence:Axt" display_in_upload="true" description="blastz pairwise alignment format.  Each alignment block in an axt file contains three lines: a summary line and 2 sequence lines.  Blocks are separated from one another by blank lines.  The summary line contains chromosomal position and size information about the alignment. It consists of 9 required fields." description_url="https://wiki.galaxyproject.org/Learn/Datatypes#Axt"/>
     <datatype extension="fli" type="galaxy.datatypes.tabular:FeatureLocationIndex" display_in_upload="false"/>
     <datatype extension="bam" type="galaxy.datatypes.binary:Bam" mimetype="application/octet-stream" display_in_upload="true" description="A binary file compressed in the BGZF format with a '.bam' file extension." description_url="https://wiki.galaxyproject.org/Learn/Datatypes#BAM">
       <converter file="bam_to_bai.xml" target_datatype="bai"/>
       <converter file="bam_to_bigwig_converter.xml" target_datatype="bigwig"/>
@@ -84,14 +84,15 @@
     </datatype>
     <datatype extension="idat" type="galaxy.datatypes.binary:Idat" display_in_upload="true"/>
     <datatype extension="bigbed" type="galaxy.datatypes.binary:BigBed" mimetype="application/octet-stream" display_in_upload="true">
       <display file="ucsc/bigbed.xml"/>
       <display file="igb/bb.xml"/>
     </datatype>
     <datatype extension="bigwig" type="galaxy.datatypes.binary:BigWig" mimetype="application/octet-stream" display_in_upload="true">
+      <converter file="bigwig_to_wig_converter.xml" target_datatype="wig"/>
       <display file="ucsc/bigwig.xml"/>
       <display file="igb/bigwig.xml"/>
       <display file="igv/bigwig.xml"/>
     </datatype>
     <datatype extension="cxb" type="galaxy.datatypes.binary:Binary" mimetype="application/octet-stream" subclass="true" display_in_upload="true" description="Cuffquant output format"/>
     <datatype extension="chrint" type="galaxy.datatypes.interval:ChromatinInteractions" display_in_upload="true">
       <converter file="interval_to_bgzip_converter.xml" target_datatype="bgzip"/>
@@ -117,27 +118,30 @@
     <datatype extension="d3_hierarchy" type="galaxy.datatypes.text:Json" mimetype="application/json" subclass="true" display_in_upload="true"/>
     <datatype extension="imgt.json" type="galaxy.datatypes.text:ImgtJson" mimetype="application/json" display_in_upload="True"/>
     <datatype extension="geojson" type="galaxy.datatypes.text:GeoJson" mimetype="application/json" display_in_upload="True"/>
     <datatype extension="data_manager_json" type="galaxy.datatypes.text:Json" mimetype="application/json" subclass="true" display_in_upload="false"/>
     <datatype extension="dbn" type="galaxy.datatypes.sequence:DotBracket" display_in_upload="true" description="Dot-Bracket format is a text-based format for storing both an RNA sequence and its corresponding 2D structure." description_url="https://wiki.galaxyproject.org/Learn/Datatypes#Dbn"/>
     <datatype extension="fai" type="galaxy.datatypes.tabular:Tabular" display_in_upload="true" subclass="true" description="A Fasta Index File is a text file consisting of lines each with five TAB-delimited columns : Name, Length, offset, linebases, Linewidth" description_url="http://www.htslib.org/doc/faidx.html"/>
     <datatype extension="fasta" auto_compressed_types="gz" type="galaxy.datatypes.sequence:Fasta" display_in_upload="true" description="A sequence in FASTA format consists of a single-line description, followed by lines of sequence data. The first character of the description line is a greater-than ('&gt;') symbol in the first column. All lines should be shorter than 80 characters." description_url="https://wiki.galaxyproject.org/Learn/Datatypes#Fasta">
+      <infer_from suffix="fa"/>
       <converter file="fasta_to_tabular_converter.xml" target_datatype="tabular"/>
       <converter file="fasta_to_bowtie_base_index_converter.xml" target_datatype="bowtie_base_index"/>
       <converter file="fasta_to_bowtie_color_index_converter.xml" target_datatype="bowtie_color_index"/>
       <converter file="fasta_to_2bit.xml" target_datatype="twobit"/>
       <converter file="fasta_to_len.xml" target_datatype="len"/>
       <converter file="fasta_to_fai.xml" target_datatype="fai"/>
       <display file="igv/genome_fasta.xml" inherit="true"/>
     </datatype>
     <datatype extension="fastg" type="galaxy.datatypes.sequence:Fastg" display_in_upload="true" description="fastg format faithfully represents genome assemblies in the face of allelic polymorphism and assembly uncertainty" description_url="http://fastg.sourceforge.net/FASTG_Spec_v1.00.pdf"/>
     <datatype extension="fastq" auto_compressed_types="gz,bz2" type="galaxy.datatypes.sequence:Fastq" display_in_upload="true" description="FASTQ format is a text-based format for storing both a biological sequence (usually nucleotide sequence) and its corresponding quality scores." description_url="https://wiki.galaxyproject.org/Learn/Datatypes#Fastq">
       <converter file="fastq_to_fqtoc.xml" target_datatype="fqtoc"/>
     </datatype>
     <datatype extension="fastqsanger" auto_compressed_types="gz,bz2" type="galaxy.datatypes.sequence:FastqSanger" display_in_upload="true" description="Sanger variant of the FASTQ format: phred+33">
+      <infer_from suffix="fq"/>
+      <infer_from suffix="fastq"/>
       <converter file="fastq_to_fqtoc.xml" target_datatype="fqtoc"/>
     </datatype>
     <datatype extension="fastqsolexa" auto_compressed_types="gz,bz2" type="galaxy.datatypes.sequence:FastqSolexa" display_in_upload="true" description="Solexa variant of the FASTQ format: solexa+64" description_url="https://wiki.galaxyproject.org/Learn/Datatypes#FastqSolexa">
       <converter file="fastq_to_fqtoc.xml" target_datatype="fqtoc"/>
     </datatype>
     <datatype extension="fastqcssanger" auto_compressed_types="gz,bz2" type="galaxy.datatypes.sequence:FastqCSSanger" display_in_upload="true" description="sequence in in color space phred scored quality values 0:93 represented by ASCII 33:126">
       <converter file="fastq_to_fqtoc.xml" target_datatype="fqtoc"/>
@@ -169,25 +173,27 @@
     <datatype extension="gtf" type="galaxy.datatypes.interval:Gtf" display_in_upload="true">
       <converter file="gff_to_interval_index_converter.xml" target_datatype="interval_index"/>
       <converter file="bed_gff_or_vcf_to_bigwig_converter.xml" target_datatype="bigwig"/>
       <display file="igb/gtf.xml"/>
     </datatype>
     <datatype extension="toolshed.gz" type="galaxy.datatypes.binary:Binary" mimetype="multipart/x-gzip" subclass="true"/>
     <datatype extension="h5" type="galaxy.datatypes.binary:H5" mimetype="application/octet-stream" display_in_upload="true"/>
+    <datatype extension="scool" type="galaxy.datatypes.binary:H5" mimetype="application/octet-stream" display_in_upload="true" subclass="true"/>
     <datatype extension="grib" type="galaxy.datatypes.binary:Grib" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="loom" type="galaxy.datatypes.binary:Loom" description="An HDF5-based Loom File" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="h5ad" type="galaxy.datatypes.binary:Anndata" description="An HDF5-based anndata File" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="mz5" type="galaxy.datatypes.binary:H5" subclass="true" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="hyphy_results.json" type="galaxy.datatypes.text:Json" mimetype="application/json" subclass="true" display_in_upload="false"/>
     <datatype extension="hivtrace" type="galaxy.datatypes.text:Json" mimetype="application/json" subclass="true" display_in_upload="false"/>
     <datatype extension="cool" type="galaxy.datatypes.binary:Cool" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="mcool" type="galaxy.datatypes.binary:MCool" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="h5mlm" type="galaxy.datatypes.binary:H5MLM" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="ludwig_model" type="galaxy.datatypes.binary:LudwigModel" display_in_upload="true"/>
     <datatype extension="html" type="galaxy.datatypes.text:Html" mimetype="text/html"/>
+    <datatype extension="ludwig_report.html" type="galaxy.datatypes.text:Html" mimetype="text/html" display_in_upload="false" subclass="true"/>
     <datatype extension="interval" type="galaxy.datatypes.interval:Interval" display_in_upload="true" description="File must start with definition line in the following format (columns may be in any order).">
       <converter file="interval_to_bed_converter.xml" target_datatype="bed"/>
       <converter file="interval_to_bedstrict_converter.xml" target_datatype="bedstrict"/>
       <converter file="interval_to_bed6_converter.xml" target_datatype="bed6"/>
       <converter file="interval_to_bed12_converter.xml" target_datatype="bed12"/>
       <converter file="interval_to_bgzip_converter.xml" target_datatype="bgzip"/>
       <converter file="interval_to_tabix_converter.xml" target_datatype="tabix" depends_on="bgzip"/>
@@ -238,14 +244,21 @@
     <datatype extension="xpm" type="galaxy.datatypes.images:Xpm" mimetype="image/xpm"/>
     <datatype extension="rgb" type="galaxy.datatypes.images:Rgb" mimetype="image/rgb"/>
     <datatype extension="pbm" type="galaxy.datatypes.images:Pbm" mimetype="image/pbm"/>
     <datatype extension="pgm" type="galaxy.datatypes.images:Pgm" mimetype="image/pgm"/>
     <datatype extension="nrrd" type="galaxy.datatypes.images:Nrrd" mimetype="image/nrrd"/>
     <datatype extension="nhdr" type="galaxy.datatypes.images:Nrrd" subclass="true"/>
     <datatype extension="rna_eps" type="galaxy.datatypes.sequence:RNADotPlotMatrix" mimetype="image/eps" display_in_upload="true"/>
+    <datatype extension="qza" type="galaxy.datatypes.qiime2:QIIME2Artifact" mimetype="application/octet-stream" display_in_upload="true">
+      <display file="qiime/qiime2/q2view.xml"/>
+    </datatype>
+    <datatype extension="qzv" type="galaxy.datatypes.qiime2:QIIME2Visualization" mimetype="application/octet-stream" display_in_upload="true">
+      <display file="qiime/qiime2/q2view.xml"/>
+    </datatype>
+    <datatype extension="qiime2.tabular" type="galaxy.datatypes.qiime2:QIIME2Metadata" display_in_upload="true"/>
     <datatype extension="zip" type="galaxy.datatypes.binary:CompressedZipArchive" display_in_upload="true"/>
     <datatype extension="ncbi_genome_dataset.zip" type="galaxy.datatypes.binary:CompressedZipArchive" subclass="true" display_in_upload="true"/>
     <datatype extension="tar" type="galaxy.datatypes.binary:CompressedArchive" subclass="true" display_in_upload="true">
       <converter file="tar_to_directory.xml" target_datatype="directory"/>
     </datatype>
     <datatype extension="directory" type="galaxy.datatypes.data:Directory"/>
     <datatype extension="yaml" type="galaxy.datatypes.text:Yaml" display_in_upload="true"/>
@@ -273,23 +286,25 @@
     <datatype extension="thermo.raw" type="galaxy.datatypes.proteomics:ThermoRAW" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="brukerbaf.d.tar" type="galaxy.datatypes.binary:BafTar" display_in_upload="true"/>
     <datatype extension="agilentbrukeryep.d.tar" type="galaxy.datatypes.binary:YepTar" display_in_upload="true"/>
     <datatype extension="brukertdf.d.tar" type="galaxy.datatypes.binary:TdfTar" display_in_upload="true"/>
     <datatype extension="agilentmasshunter.d.tar" type="galaxy.datatypes.binary:MassHunterTar" display_in_upload="true"/>
     <datatype extension="watersmasslynx.raw.tar" type="galaxy.datatypes.binary:MassLynxTar" display_in_upload="true"/>
     <datatype extension="wiff.tar" type="galaxy.datatypes.binary:WiffTar" display_in_upload="true"/>
+    <datatype extension="wiff2.tar" type="galaxy.datatypes.binary:Wiff2Tar" display_in_upload="true"/>
     <datatype extension="mascotxml" type="galaxy.datatypes.proteomics:MascotXML" mimetype="application/xml" display_in_upload="true"/>
     <datatype extension="mztab" type="galaxy.datatypes.proteomics:MzTab" display_in_upload="true"/>
     <datatype extension="mztab2" type="galaxy.datatypes.proteomics:MzTab2" display_in_upload="true"/>
     <datatype extension="mzml" type="galaxy.datatypes.proteomics:MzML" mimetype="application/xml" display_in_upload="true"/>
     <datatype extension="nmrml" type="galaxy.datatypes.proteomics:NmrML" mimetype="application/xml" display_in_upload="true" description="nmrML is an open mark-up language for NMR data." description_url="http://nmrml.org/schema/"/>
     <datatype extension="meryldb" type="galaxy.datatypes.binary:Meryldb" subclass="true" display_in_upload="true" description="MerylDB is a tar.gz archive containing 64 binaries + 64 indexes."/>
     <datatype extension="bref3" type="galaxy.datatypes.binary:Bref3" display_in_upload="true" description="Bref3 format is a binary format for storing phased, non-missing genotypes for a list of samples. More information in https://faculty.washington.edu/browning/beagle/bref3.14May18.pdf"/>
     <datatype extension="mgf" type="galaxy.datatypes.proteomics:Mgf" display_in_upload="true"/>
     <datatype extension="wiff" type="galaxy.datatypes.proteomics:Wiff" display_in_upload="true"/>
+    <datatype extension="wiff2" type="galaxy.datatypes.proteomics:Wiff2" display_in_upload="true"/>
     <datatype extension="mzxml" type="galaxy.datatypes.proteomics:MzXML" mimetype="application/xml" display_in_upload="true"/>
     <datatype extension="mzdata" type="galaxy.datatypes.proteomics:MzData" mimetype="application/xml" display_in_upload="true"/>
     <datatype extension="ms2" type="galaxy.datatypes.proteomics:Ms2" display_in_upload="true"/>
     <datatype extension="mzq" type="galaxy.datatypes.proteomics:MzQuantML" mimetype="application/xml" display_in_upload="true"/>
     <datatype extension="sqlite" type="galaxy.datatypes.binary:SQlite" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="mz.sqlite" type="galaxy.datatypes.binary:MzSQlite" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="osw" type="galaxy.datatypes.binary:OSW" mimetype="application/octet-stream" display_in_upload="true"/>
@@ -375,14 +390,15 @@
       <converter file="bed_gff_or_vcf_to_bigwig_converter.xml" target_datatype="bigwig"/>
     </datatype>
     <datatype extension="pdf" type="galaxy.datatypes.images:Pdf" mimetype="application/pdf" display_in_upload="true"/>
     <datatype extension="pileup" type="galaxy.datatypes.tabular:Pileup" display_in_upload="true">
       <converter file="interval_to_bgzip_converter.xml" target_datatype="bgzip"/>
       <converter file="interval_to_tabix_converter.xml" target_datatype="tabix" depends_on="bgzip"/>
     </datatype>
+    <datatype extension="psl" type="galaxy.datatypes.tabular:Psl" display_in_upload="true"/>
     <datatype extension="obo" type="galaxy.datatypes.text:Obo" mimetype="text/html" display_in_upload="true"/>
     <datatype extension="owl" type="galaxy.datatypes.xml:Owl" mimetype="text/html" display_in_upload="true"/>
     <datatype extension="png" type="galaxy.datatypes.images:Png" mimetype="image/png" display_in_upload="true"/>
     <datatype extension="qual" type="galaxy.datatypes.qualityscore:QualityScore"/>
     <datatype extension="qualsolexa" type="galaxy.datatypes.qualityscore:QualityScoreSolexa" display_in_upload="true"/>
     <datatype extension="qualillumina" type="galaxy.datatypes.qualityscore:QualityScoreIllumina" display_in_upload="true"/>
     <datatype extension="qualsolid" type="galaxy.datatypes.qualityscore:QualityScoreSOLiD" display_in_upload="true"/>
@@ -392,15 +408,14 @@
       <converter file="sam_to_unsorted_bam.xml" target_datatype="unsorted.bam"/>
       <converter file="to_coordinate_sorted_bam.xml" target_datatype="bam"/>
       <converter file="to_qname_sorted_bam.xml" target_datatype="qname_sorted.bam"/>
       <converter file="sam_to_bigwig_converter.xml" target_datatype="bigwig"/>
     </datatype>
     <datatype extension="scf" type="galaxy.datatypes.binary:Scf" mimetype="application/octet-stream" display_in_upload="true" description="A binary sequence file in 'scf' format with a '.scf' file extension.  You must manually select this 'File Format' when uploading the file." description_url="https://wiki.galaxyproject.org/Learn/Datatypes#Scf"/>
     <datatype extension="sequences" type="galaxy.datatypes.assembly:Sequences" display_in_upload="false"/>
-    <datatype extension="shp" type="galaxy.datatypes.gis:Shapefile" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="snpeffdb" type="galaxy.datatypes.text:SnpEffDb" display_in_upload="true"/>
     <datatype extension="snpsiftdbnsfp" type="galaxy.datatypes.text:SnpSiftDbNSFP" display_in_upload="true"/>
     <datatype extension="dbnsfp.tabular" type="galaxy.datatypes.tabular:Tabular" subclass="true" display_in_upload="true">
       <converter file="tabular_to_dbnsfp.xml" target_datatype="snpsiftdbnsfp"/>
     </datatype>
     <datatype extension="sff" type="galaxy.datatypes.binary:Sff" mimetype="application/octet-stream" display_in_upload="true" description="A binary file in 'Standard Flowgram Format' with a '.sff' file extension." description_url="https://wiki.galaxyproject.org/Learn/Datatypes#Sff"/>
     <datatype extension="sra" type="galaxy.datatypes.binary:Sra" mimetype="application/octet-stream" display_in_upload="true" description="A binary file archive format from the NCBI Sequence Read Archive with a '.sra' file extension." description_url="http://www.ncbi.nlm.nih.gov/books/n/helpsra/SRA_Overview_BK/#SRA_Overview_BK.4_SRA_Data_Structure"/>
@@ -419,14 +434,15 @@
     <datatype extension="ncbitaxonomy.sqlite" type="galaxy.datatypes.binary:NcbiTaxonomySQlite" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="txt" type="galaxy.datatypes.data:Text" display_in_upload="true" description="Any text file." description_url="https://wiki.galaxyproject.org/Learn/Datatypes#Plain_text"/>
     <datatype extension="linecount" type="galaxy.datatypes.data:LineCount" display_in_upload="false"/>
     <datatype extension="memepsp" type="galaxy.datatypes.sequence:MemePsp" display_in_upload="true" description="The MEME Position Specific Priors (PSP) format includes the name of the sequence for which a prior distribution corresponds." description_url="http://meme-suite.org/doc/psp-format.html"/>
     <datatype extension="memexml" type="galaxy.datatypes.xml:MEMEXml" mimetype="application/xml" display_in_upload="true"/>
     <datatype extension="cisml" type="galaxy.datatypes.xml:CisML" mimetype="application/xml" display_in_upload="true"/>
     <datatype extension="xml" type="galaxy.datatypes.xml:GenericXml" mimetype="application/xml" display_in_upload="true"/>
+    <datatype extension="xsd" type="galaxy.datatypes.xml:GenericXml" mimetype="application/xml" display_in_upload="true"/>
     <datatype extension="dzi" type="galaxy.datatypes.xml:Dzi" mimetype="application/xml" display_in_upload="true"/>
     <datatype extension="vcf" type="galaxy.datatypes.tabular:Vcf" display_in_upload="true">
       <converter file="interval_to_bgzip_converter.xml" target_datatype="bgzip"/>
       <converter file="vcf_to_vcf_bgzip_converter.xml" target_datatype="vcf_bgzip"/>
       <converter file="interval_to_tabix_converter.xml" target_datatype="tabix" depends_on="bgzip"/>
       <converter file="bed_gff_or_vcf_to_bigwig_converter.xml" target_datatype="bigwig"/>
       <converter file="uncompressed_to_gz.xml" target_datatype="vcf_bgzip"/>
@@ -454,14 +470,18 @@
     <datatype extension="odgi" type="galaxy.datatypes.binary:Binary" subclass="true" description="Genomic variation graphs self index used by odgi." display_in_upload="true"/>
     <datatype extension="vg" type="galaxy.datatypes.binary:CompressedArchive" subclass="true" description="Genomic variation graphs." display_in_upload="true"/>
     <datatype extension="xg" type="galaxy.datatypes.binary:Binary" subclass="true" description="Genomic variation graphs with vg index." display_in_upload="true"/>
     <datatype extension="protobuf2" type="galaxy.datatypes.binary:Binary" subclass="true" description="Protocol Buffers (Protobuf) is data format for serializing structured data." display_in_upload="true"/>
     <datatype extension="protobuf3" type="galaxy.datatypes.binary:Binary" subclass="true" description="Protocol Buffers (Protobuf) is data format for serializing structured data." display_in_upload="true"/>
     <datatype extension="onnx" type="galaxy.datatypes.binary:Binary" subclass="true" description="ONNX (Open neural network exchange) is data format for storing and sharing machine learning and deep learning models." display_in_upload="true"/>
     <datatype extension="tabix" type="galaxy.datatypes.binary:Binary" subclass="true"/>
+    <datatype extension="interval_tabix.gz" type="galaxy.datatypes.interval:IntervalTabix" mimetype="application/octet-stream"/>
+    <datatype extension="juicer_medium_tabix.gz" type="galaxy.datatypes.interval:JuicerMediumTabix" mimetype="application/octet-stream" display_in_upload="true"/>
+    <datatype extension="bed_tabix.gz" type="galaxy.datatypes.interval:BedTabix" mimetype="application/octet-stream" display_in_upload="true"/>
+    <datatype extension="gff_tabix.gz" type="galaxy.datatypes.interval:GffTabix" mimetype="application/octet-stream" display_in_upload="true"/>
     <datatype extension="bgzip" type="galaxy.datatypes.binary:Binary" subclass="true" display_in_upload="true"/>
     <datatype extension="vcf_bgzip" type="galaxy.datatypes.tabular:VcfGz" display_in_upload="true">
       <display file="igv/vcf.xml"/>
       <converter file="vcf_bgzip_to_tabix_converter.xml" target_datatype="tabix"/>
       <converter file="gz_to_uncompressed.xml" target_datatype="vcf"/>
     </datatype>
     <datatype extension="bus" type="galaxy.datatypes.binary:Binary" subclass="true" display_in_upload="true"/>
@@ -902,14 +922,31 @@
     <datatype extension="neper.mscell" type="galaxy.datatypes.constructive_solid_geometry:NeperMultiScaleCell" display_in_upload="true"/>
     <datatype extension="gmsh.msh" type="galaxy.datatypes.constructive_solid_geometry:GmshMsh" display_in_upload="true"/>
     <datatype extension="gmsh.geo" type="galaxy.datatypes.constructive_solid_geometry:GmshGeo" display_in_upload="true"/>
     <datatype extension="zset.geof" type="galaxy.datatypes.constructive_solid_geometry:ZsetGeof" display_in_upload="true"/>
     <!-- Povray script -->
     <datatype extension="pov" type="galaxy.datatypes.text:Text" subclass="true" display_in_upload="true"/>
     <!-- End Structural Materials datatypes -->
+    <!-- Sybila types -->
+    <datatype extension="pithya.result" type="galaxy.datatypes.text:PithyaResult" mimetype="application/json" display_in_upload="true"/>
+    <datatype extension="pithya.property" type="galaxy.datatypes.text:PithyaProperty" display_in_upload="true"/>
+    <datatype extension="pithya.model" type="galaxy.datatypes.text:PithyaModel" display_in_upload="true"/>
+    <datatype extension="bcsl.ts" type="galaxy.datatypes.text:BCSLts" mimetype="application/json" display_in_upload="true"/>
+    <datatype extension="bcsl.model" type="galaxy.datatypes.text:BCSLmodel" display_in_upload="true"/>
+    <datatype extension="storm.sample" type="galaxy.datatypes.text:StormSample" display_in_upload="true"/>
+    <datatype extension="storm.check" type="galaxy.datatypes.text:StormCheck" display_in_upload="true"/>
+    <datatype extension="ctl.result" type="galaxy.datatypes.text:CTLresult" display_in_upload="true"/>
+    <!-- CASTEP types -->
+    <datatype extension="castep" type="galaxy.datatypes.text:Castep" display_in_upload="true"/>
+    <datatype extension="param" type="galaxy.datatypes.text:Param" display_in_upload="true"/>
+    <datatype extension="den_fmt" type="galaxy.datatypes.text:FormattedDensity" display_in_upload="true"/>
+    <!-- ECOLOGY types -->
+    <datatype extension="bil" type="galaxy.datatypes.binary:Binary" mimetype="application/octet-stream" display_in_upload="true" subclass="true" description="ENVI file with band interleave by line (BIL) format"/>
+    <datatype extension="hdr" type="galaxy.datatypes.data:Text" mimetype="text/plain" display_in_upload="true" subclass="true" description="ENVI metadata header file"/>
+    <datatype extension="shp" type="galaxy.datatypes.gis:Shapefile" mimetype="application/octet-stream" display_in_upload="true" description="geospatial vector data format for geographic information system"/>
   </registration>
   <sniffers>
     <!--
     The order in which Galaxy attempts to determine data types is
     important because some formats are much more loosely defined
     than others.  The following list should be the most rigidly
     defined format first, followed by next-most rigidly defined,
@@ -996,14 +1033,17 @@
     <sniffer type="galaxy.datatypes.binary:Trr"/>
     <sniffer type="galaxy.datatypes.binary:Dcd"/>
     <sniffer type="galaxy.datatypes.binary:Xtc"/>
     <sniffer type="galaxy.datatypes.binary:Cpt"/>
     <sniffer type="galaxy.datatypes.binary:Edr"/>
     <sniffer type="galaxy.datatypes.binary:Vel"/>
     <sniffer type="galaxy.datatypes.binary:Xlsx"/>
+    <sniffer type="galaxy.datatypes.qiime2:QIIME2Metadata"/>
+    <sniffer type="galaxy.datatypes.qiime2:QIIME2Artifact"/>
+    <sniffer type="galaxy.datatypes.qiime2:QIIME2Visualization"/>
     <sniffer type="galaxy.datatypes.binary:CompressedZipArchive"/>
     <sniffer type="galaxy.datatypes.binary:Pretext"/>
     <sniffer type="galaxy.datatypes.annotation:Augustus"/>
     <sniffer type="galaxy.datatypes.xml:Owl"/>
     <sniffer type="galaxy.datatypes.triples:Rdf"/>
     <sniffer type="galaxy.datatypes.blast:BlastXml"/>
     <sniffer type="galaxy.datatypes.images:Gifti"/>
@@ -1081,26 +1121,29 @@
     <sniffer type="galaxy.datatypes.sequence:Genbank"/>
     <sniffer type="galaxy.datatypes.interval:Bed"/>
     <sniffer type="galaxy.datatypes.interval:CustomTrack"/>
     <sniffer type="galaxy.datatypes.interval:Gtf"/>
     <sniffer type="galaxy.datatypes.interval:Gff"/>
     <sniffer type="galaxy.datatypes.interval:Gff3"/>
     <sniffer type="galaxy.datatypes.tabular:Pileup"/>
+    <sniffer type="galaxy.datatypes.tabular:Psl"/>
     <sniffer type="galaxy.datatypes.text:Paf"/>
     <sniffer type="galaxy.datatypes.interval:Interval"/>
     <sniffer type="galaxy.datatypes.tabular:Sam"/>
     <sniffer type="galaxy.datatypes.data:Newick"/>
     <sniffer type="galaxy.datatypes.data:Nexus"/>
     <sniffer type="galaxy.datatypes.text:IQTree"/>
     <sniffer type="galaxy.datatypes.text:Obo"/>
     <sniffer type="galaxy.datatypes.text:Arff"/>
     <sniffer type="galaxy.datatypes.text:Ipynb"/>
     <sniffer type="galaxy.datatypes.text:Biom1"/>
     <sniffer type="galaxy.datatypes.text:ImgtJson"/>
     <sniffer type="galaxy.datatypes.text:GeoJson"/>
+    <sniffer type="galaxy.datatypes.text:PithyaResult"/>
+    <sniffer type="galaxy.datatypes.text:BCSLts"/>
     <sniffer type="galaxy.datatypes.text:Json"/>
     <sniffer type="galaxy.datatypes.genetics:GenotypeMatrix"/>
     <sniffer type="galaxy.datatypes.genetics:DataIn"/>
     <sniffer type="galaxy.datatypes.genetics:MarkerMap"/>
     <sniffer type="galaxy.datatypes.genetics:AllegroLOD"/>
     <sniffer type="galaxy.datatypes.sequence:RNADotPlotMatrix"/>
     <sniffer type="galaxy.datatypes.sequence:DotBracket"/>
@@ -1150,22 +1193,31 @@
     <sniffer type="galaxy.datatypes.media:Mkv"/>
     <sniffer type="galaxy.datatypes.media:Mp3"/>
     <sniffer type="galaxy.datatypes.media:Mp4"/>
     <sniffer type="galaxy.datatypes.media:Flv"/>
     <sniffer type="galaxy.datatypes.media:Mpg"/>
     <sniffer type="galaxy.datatypes.speech:TextGrid"/>
     <sniffer type="galaxy.datatypes.speech:BPF"/>
+    <sniffer type="galaxy.datatypes.text:Castep"/>
+    <sniffer type="galaxy.datatypes.text:CTLresult"/>
+    <sniffer type="galaxy.datatypes.text:FormattedDensity"/>
+    <sniffer type="galaxy.datatypes.text:Param"/>
     <sniffer type="galaxy.datatypes.text:Yaml"/>
     <!--
     Keep this commented until the sniff method in the assembly.py
     module is fixed to not read the entire file.
     <sniffer type="galaxy.datatypes.assembly:Amos"/>
     -->
     <sniffer type="galaxy.datatypes.binary:OxliCountGraph"/>
     <sniffer type="galaxy.datatypes.binary:OxliNodeGraph"/>
     <sniffer type="galaxy.datatypes.binary:OxliTagSet"/>
     <sniffer type="galaxy.datatypes.binary:OxliStopTags"/>
     <sniffer type="galaxy.datatypes.binary:OxliSubset"/>
     <sniffer type="galaxy.datatypes.binary:OxliGraphLabels"/>
     <sniffer type="galaxy.datatypes.neo4j:Neo4jDBzip"/>
+    <sniffer type="galaxy.datatypes.text:PithyaProperty"/>
+    <sniffer type="galaxy.datatypes.text:PithyaModel"/>
+    <sniffer type="galaxy.datatypes.text:BCSLmodel"/>
+    <sniffer type="galaxy.datatypes.text:StormSample"/>
+    <sniffer type="galaxy.datatypes.text:StormCheck"/>
   </sniffers>
 </datatypes>
```

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/environment_modules_mapping.yml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/environment_modules_mapping.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/error_report.yml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/error_report.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/file_sources_conf.yml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/file_sources_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/galaxy.yml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/galaxy.yml.sample`

 * *Files 3% similar despite different names*

```diff
@@ -16,40 +16,82 @@
 # 
 # Config hackers are encouraged to check there before asking for help.
 # 
 # Configuration for Gravity process manager.
 # ``uwsgi:`` section will be ignored if Galaxy is started via Gravity commands (e.g ``./run.sh``, ``galaxy`` or ``galaxyctl``).
 gravity:
 
+  # Process manager to use.
+  # ``supervisor`` is the default process manager when Gravity is invoked as a non-root user.
+  # ``systemd`` is the default when Gravity is invoked as root.
+  # Valid options are: supervisor, systemd
+  # process_manager:
+
+  # What command to write to the process manager configs
+  # `gravity` (`galaxyctl exec <service-name>`) is the default
+  # `direct` (each service's actual command) is also supported.
+  # Valid options are: gravity, direct
+  # service_command_style: gravity
+
+  # Use the process manager's *service instance* functionality for services that can run multiple instances.
+  # Presently this includes services like gunicorn and Galaxy dynamic job handlers. Service instances are only supported if
+  # ``service_command_style`` is ``gravity``, and so this option is automatically set to ``false`` if
+  # ``service_command_style`` is set to ``direct``.
+  # use_service_instances: true
+
+  # umask under which services should be executed. Setting ``umask`` on an individual service overrides this value.
+  # umask: '022'
+
+  # Memory limit (in GB), processes exceeding the limit will be killed. Default is no limit. If set, this is default value
+  # for all services. Setting ``memory_limit`` on an individual service overrides this value. Ignored if ``process_manager``
+  # is ``supervisor``.
+  # memory_limit:
+
+  # Specify Galaxy config file (galaxy.yml), if the Gravity config is separate from the Galaxy config. Assumed to be the
+  # same file as the Gravity config if a ``galaxy`` key exists at the root level, otherwise, this option is required.
+  # galaxy_config_file:
+
   # Specify Galaxy's root directory.
   # Gravity will attempt to find the root directory, but you can set the directory explicitly with this option.
   # galaxy_root:
 
+  # User to run Galaxy as, required when using the systemd process manager as root.
+  # Ignored if ``process_manager`` is ``supervisor`` or user-mode (non-root) ``systemd``.
+  # galaxy_user:
+
+  # Group to run Galaxy as, optional when using the systemd process manager as root.
+  # Ignored if ``process_manager`` is ``supervisor`` or user-mode (non-root) ``systemd``.
+  # galaxy_group:
+
   # Set to a directory that should contain log files for the processes controlled by Gravity.
-  # If not specified defaults to ``<state_dir>/log``.
+  # If not specified defaults to ``<galaxy_data_dir>/gravity/log``.
   # log_dir:
 
   # Set to Galaxy's virtualenv directory.
-  # If not specified, Gravity assumes all processes are on PATH.
+  # If not specified, Gravity assumes all processes are on PATH. This option is required in most circumstances when using
+  # the ``systemd`` process manager.
   # virtualenv:
 
   # Select the application server.
   # ``gunicorn`` is the default application server.
   # ``unicornherder`` is a production-oriented manager for (G)unicorn servers that automates zero-downtime Galaxy server restarts,
   # similar to uWSGI Zerg Mode used in the past.
   # Valid options are: gunicorn, unicornherder
   # app_server: gunicorn
 
   # Override the default instance name.
   # this is hidden from you when running a single instance.
   # instance_name: _default_
 
-  # Configuration for Gunicorn.
+  # Configuration for Gunicorn. Can be a list to run multiple gunicorns for rolling restarts.
   gunicorn:
 
+    # Enable Galaxy gunicorn server.
+    # enable: true
+
     # The socket to bind. A string of the form: ``HOST``, ``HOST:PORT``, ``unix:PATH``, ``fd://FD``. An IP is a valid HOST.
     # bind: localhost:8080
 
     # Controls the number of Galaxy application processes Gunicorn will spawn.
     # Increased web performance can be attained by increasing this value.
     # If Gunicorn is the only application on the server, a good starting value is the number of CPUs * 2 + 1.
     # 4-12 workers should be able to handle hundreds if not thousands of requests per second.
@@ -60,20 +102,47 @@
     # If you disable the ``preload`` option workers need to have finished booting within the timeout.
     # timeout: 300
 
     # Extra arguments to pass to Gunicorn command line.
     # extra_args:
 
     # Use Gunicorn's --preload option to fork workers after loading the Galaxy Application.
-    # Consumes less memory when multiple processes are configured.
-    # preload: true
+    # Consumes less memory when multiple processes are configured. Default is ``false`` if using unicornherder, else ``true``.
+    # preload:
+
+    # umask under which service should be executed
+    # umask:
+
+    # Value of supervisor startsecs, systemd TimeoutStartSec
+    # start_timeout: 15
+
+    # Value of supervisor stopwaitsecs, systemd TimeoutStopSec
+    # stop_timeout: 65
+
+    # Amount of time to wait for a server to become alive when performing rolling restarts.
+    # restart_timeout: 300
+
+    # Memory limit (in GB). If the service exceeds the limit, it will be killed. Default is no limit or the value of the
+    # ``memory_limit`` setting at the top level of the Gravity configuration, if set. Ignored if ``process_manager`` is
+    # ``supervisor``.
+    # memory_limit:
+
+    # Extra environment variables and their values to set when running the service. A dictionary where keys are the variable
+    # names.
+    # environment: {}
 
   # Configuration for Celery Processes.
   celery:
 
+    # Enable Celery distributed task queue.
+    # enable: true
+
+    # Enable Celery Beat periodic task runner.
+    # enable_beat: true
+
     # Number of Celery Workers to start.
     # concurrency: 2
 
     # Log Level to use for Celery Worker.
     # Valid options are: DEBUG, INFO, WARNING, ERROR
     # loglevel: DEBUG
 
@@ -83,28 +152,50 @@
     # Pool implementation
     # Valid options are: prefork, eventlet, gevent, solo, processes, threads
     # pool: threads
 
     # Extra arguments to pass to Celery command line.
     # extra_args:
 
+    # umask under which service should be executed
+    # umask:
+
+    # Value of supervisor startsecs, systemd TimeoutStartSec
+    # start_timeout: 10
+
+    # Value of supervisor stopwaitsecs, systemd TimeoutStopSec
+    # stop_timeout: 10
+
+    # Memory limit (in GB). If the service exceeds the limit, it will be killed. Default is no limit or the value of the
+    # ``memory_limit`` setting at the top level of the Gravity configuration, if set. Ignored if ``process_manager`` is
+    # ``supervisor``.
+    # memory_limit:
+
+    # Extra environment variables and their values to set when running the service. A dictionary where keys are the variable
+    # names.
+    # environment: {}
+
   # Configuration for gx-it-proxy.
   gx_it_proxy:
 
     # Set to true to start gx-it-proxy
     # enable: false
 
+    # gx-it-proxy version
+    # version: '>=0.0.5'
+
     # Public-facing IP of the proxy
     # ip: localhost
 
     # Public-facing port of the proxy
     # port: 4002
 
     # Routes file to monitor.
-    # Should be set to the same path as ``interactivetools_map`` in the ``galaxy:`` section.
+    # Should be set to the same path as ``interactivetools_map`` in the ``galaxy:`` section. This is ignored if
+    # ``interactivetools_map is set``.
     # sessions: database/interactivetools_map.sqlite
 
     # Include verbose messages in gx-it-proxy
     # verbose: true
 
     # Forward all requests to IP.
     # This is an advanced option that is only needed when proxying to remote interactive tool container that cannot be reached through the local network.
@@ -114,130 +205,141 @@
     # This is an advanced option that is only needed when proxying to remote interactive tool container that cannot be reached through the local network.
     # forward_port:
 
     # Rewrite location blocks with proxy port.
     # This is an advanced option that is only needed when proxying to remote interactive tool container that cannot be reached through the local network.
     # reverse_proxy: false
 
+    # umask under which service should be executed
+    # umask:
+
+    # Value of supervisor startsecs, systemd TimeoutStartSec
+    # start_timeout: 10
+
+    # Value of supervisor stopwaitsecs, systemd TimeoutStopSec
+    # stop_timeout: 10
+
+    # Memory limit (in GB). If the service exceeds the limit, it will be killed. Default is no limit or the value of the
+    # ``memory_limit`` setting at the top level of the Gravity configuration, if set. Ignored if ``process_manager`` is
+    # ``supervisor``.
+    # memory_limit:
+
+    # Extra environment variables and their values to set when running the service. A dictionary where keys are the variable
+    # names.
+    # environment: {}
+
   # Configuration for tusd server (https://github.com/tus/tusd).
   # The ``tusd`` binary must be installed manually and made available on PATH (e.g in galaxy's .venv/bin directory).
   tusd:
 
     # Enable tusd server.
     # If enabled, you also need to set up your proxy as outlined in https://docs.galaxyproject.org/en/latest/admin/nginx.html#receiving-files-via-the-tus-protocol.
     # enable: false
 
+    # Path to tusd binary
+    # tusd_path: tusd
+
     # Host to bind the tusd server to
     # host: localhost
 
     # Port to bind the tusd server to
     # port: 1080
 
     # Directory to store uploads in.
     # Must match ``tus_upload_store`` setting in ``galaxy:`` section.
     # upload_dir:
 
+    # Comma-separated string of enabled tusd hooks.
+    #
+    # Leave at the default value to require authorization at upload creation time.
+    # This means Galaxy's web process does not need to be running after creating the initial
+    # upload request.
+    #
+    # Set to empty string to disable all authorization. This means data can be uploaded (but not processed)
+    # without the Galaxy web process being available.
+    #
+    # You can find a list of available hooks at https://github.com/tus/tusd/blob/master/docs/hooks.md#list-of-available-hooks.
+    # hooks_enabled_events: pre-create
+
     # Extra arguments to pass to tusd command line.
     # extra_args:
 
+    # umask under which service should be executed
+    # umask:
+
+    # Value of supervisor startsecs, systemd TimeoutStartSec
+    # start_timeout: 10
+
+    # Value of supervisor stopwaitsecs, systemd TimeoutStopSec
+    # stop_timeout: 10
+
+    # Memory limit (in GB). If the service exceeds the limit, it will be killed. Default is no limit or the value of the
+    # ``memory_limit`` setting at the top level of the Gravity configuration, if set. Ignored if ``process_manager`` is
+    # ``supervisor``.
+    # memory_limit:
+
+    # Extra environment variables and their values to set when running the service. A dictionary where keys are the variable
+    # names.
+    # environment: {}
+
+  # Configuration for Galaxy Reports.
+  reports:
+
+    # Enable Galaxy Reports server.
+    # enable: false
+
+    # Path to reports.yml, relative to galaxy.yml if not absolute
+    # config_file: reports.yml
+
+    # The socket to bind. A string of the form: ``HOST``, ``HOST:PORT``, ``unix:PATH``, ``fd://FD``. An IP is a valid HOST.
+    # bind: localhost:9001
+
+    # Controls the number of Galaxy Reports application processes Gunicorn will spawn.
+    # It is not generally necessary to increase this for the low-traffic Reports server.
+    # workers: 1
+
+    # Gunicorn workers silent for more than this many seconds are killed and restarted.
+    # Value is a positive number or 0. Setting it to 0 has the effect of infinite timeouts by disabling timeouts for all workers entirely.
+    # timeout: 300
+
+    # URL prefix to serve from.
+    # The corresponding nginx configuration is (replace <url_prefix> and <bind> with the values from these options):
+    #
+    # location /<url_prefix>/ {
+    #     proxy_pass http://<bind>/;
+    # }
+    #
+    # If <bind> is a unix socket, you will need a ``:`` after the socket path but before the trailing slash like so:
+    #     proxy_pass http://unix:/run/reports.sock:/;
+    # url_prefix:
+
+    # Extra arguments to pass to Gunicorn command line.
+    # extra_args:
+
+    # umask under which service should be executed
+    # umask:
+
+    # Value of supervisor startsecs, systemd TimeoutStartSec
+    # start_timeout: 10
+
+    # Value of supervisor stopwaitsecs, systemd TimeoutStopSec
+    # stop_timeout: 10
+
+    # Memory limit (in GB). If the service exceeds the limit, it will be killed. Default is no limit or the value of the
+    # ``memory_limit`` setting at the top level of the Gravity configuration, if set. Ignored if ``process_manager`` is
+    # ``supervisor``.
+    # memory_limit:
+
+    # Extra environment variables and their values to set when running the service. A dictionary where keys are the variable
+    # names.
+    # environment: {}
+
   # Configure dynamic handlers in this section.
   # See https://docs.galaxyproject.org/en/latest/admin/scaling.html#dynamically-defined-handlers for details.
   # handlers: {}
-uwsgi:
-
-  # The address and port on which to listen.  By default, only listen to
-  # localhost (galaxy will not be accessible over the network).  Use
-  # ':8080' to listen on all available network interfaces.
-  http: 127.0.0.1:8080
-
-  # By default uWSGI allocates a very small buffer (4096 bytes) for the
-  # headers of each request. If you start receiving "invalid request
-  # block size" in your logs, it could mean you need a bigger buffer. We
-  # recommend at least 16384.
-  buffer-size: 16384
-
-  # Number of web server (worker) processes to fork after the
-  # application has loaded. If this is set to greater than 1,
-  # thunder-lock likely should be enabled below.
-  processes: 1
-
-  # Number of threads for each web server process.
-  threads: 4
-
-  # Number of threads for serving static content and handling internal
-  # routing requests.
-  offload-threads: 2
-
-  # Mapping to serve static content.
-  static-map: /static=static
-
-  # Mapping to serve the favicon.
-  static-map: /favicon.ico=static/favicon.ico
-
-  # Allow serving certain assets out of `client`.  Most modern Galaxy
-  # interfaces bundle all of this, but some older pages still serve
-  # these via symlink, requiring this rule.
-  static-safe: client/src/assets
-
-  # Enable the master process manager. Disabled by default for maximum
-  # compatibility with CTRL+C, but should be enabled for use with
-  # --daemon and/or production deployments.
-  master: false
-
-  # Path to the application's Python virtual environment. If using Conda
-  # for Galaxy's framework dependencies (not tools!), do not set this.
-  virtualenv: .venv
-
-  # Path to the application's Python library.
-  pythonpath: lib
-
-  # The entry point which returns the web application (e.g. Galaxy,
-  # Reports, etc.) that you are loading.
-  module: galaxy.webapps.galaxy.buildapp:uwsgi_app()
-
-  # Mount the web application (e.g. Galaxy, Reports, etc.) at the given
-  # URL prefix. Cannot be used together with 'module:' above.
-  #mount: /galaxy=galaxy.webapps.galaxy.buildapp:uwsgi_app()
-
-  # Make uWSGI rewrite PATH_INFO and SCRIPT_NAME according to
-  # mount-points. Set this to true if a URL prefix is used.
-  manage-script-name: false
-
-  # It is usually a good idea to set this to ``true`` if processes is
-  # greater than 1.
-  thunder-lock: false
-
-  # Cause uWSGI to respect the traditional behavior of dying on SIGTERM
-  # (its default is to brutally reload workers)
-  die-on-term: true
-
-  # Cause uWSGI to gracefully reload workers and mules upon receipt of
-  # SIGINT (its default is to brutally kill workers)
-  hook-master-start: unix_signal:2 gracefully_kill_them_all
-
-  # Cause uWSGI to gracefully reload workers and mules upon receipt of
-  # SIGTERM (its default is to brutally kill workers)
-  hook-master-start: unix_signal:15 gracefully_kill_them_all
-
-  # Feature necessary for proper mule signal handling on Python versions
-  # below 3.7.2. The default is set to false to prevent a runtime error
-  # under Python 3.7.2 and newer (see
-  # https://github.com/unbit/uwsgi/issues/1978).
-  py-call-osafterfork: false
-
-  # Ensure application threads will run if `threads` is unset.
-  enable-threads: true
-
-  # uWSGI default umask. On some systems uWSGI has a default umask of
-  # 000, for Galaxy a somewhat safer default is chosen. If Galaxy
-  # submits jobs as real user then all users needs to be able to read
-  # the files, i.e. the umask needs to be '022' or the Galaxy users need
-  # to be in the same group as the Galaxy system user
-  umask: 027
-
 galaxy:
 
   # The directory that will be prepended to relative paths in options
   # specifying other Galaxy config files (e.g. datatypes_config_file).
   # Defaults to the directory in which galaxy.yml is located.
   #config_dir: null
 
@@ -250,26 +352,43 @@
 
   # The directory that will be prepended to relative paths in options
   # specifying Galaxy data/cache directories and files (such as the
   # default SQLite database, file_path, etc.). Defaults to `database/`
   # if running Galaxy from source or `<config_dir>/data` otherwise.
   #data_dir: null
 
+  # The directory containing custom templates for Galaxy, such as
+  # HTML/text email templates. Defaults to 'templates'. Default
+  # templates can be found in the Galaxy root under config/templates.
+  # These can be copied to <templates_dir> if you wish to customize
+  # them.
+  # The value of this option will be resolved with respect to
+  # <config_dir>.
+  #templates_dir: templates
+
   # Top level cache directory. Any other cache directories
   # (tool_cache_data_dir, template_cache_path, etc.) should be
   # subdirectories.
   # The value of this option will be resolved with respect to
   # <data_dir>.
   #cache_dir: cache
 
   # By default, Galaxy uses a SQLite database at
-  # '<data_dir>/universe.sqlite'.  You may use a SQLAlchemy connection
+  # '<data_dir>/universe.sqlite'. You may use a SQLAlchemy connection
   # string to specify an external database instead.
   # Sample default
   # 'sqlite:///<data_dir>/universe.sqlite?isolation_level=IMMEDIATE'
+  # You may specify additional options that will be passed to the
+  # SQLAlchemy database engine by using the prefix
+  # "database_engine_option_". For some of these options, default values
+  # are provided (e.g. see database_engine_option_pool_size, etc.).
+  # The same applies to `install_database_connection`, for which you
+  # should use the "install_database_engine_option_" prefix.
+  # For more options, please check SQLAlchemy's documentation at
+  # https://docs.sqlalchemy.org/en/14/core/engines.html?highlight=create_engine#sqlalchemy.create_engine
   #database_connection: null
 
   # If the server logs errors about not having enough database pool
   # connections, you will want to increase these values, or consider
   # running more Galaxy processes.
   #database_engine_option_pool_size: 5
 
@@ -514,23 +633,14 @@
   # File containing the Galaxy Tool Sheds that should be made available
   # to install from in the admin interface (.sample used if default does
   # not exist).
   # The value of this option will be resolved with respect to
   # <config_dir>.
   #tool_sheds_config_file: tool_sheds_conf.xml
 
-  # This option controls whether legacy datatypes are loaded from
-  # installed tool shed repositories. We're are in the process of
-  # disabling Tool Shed datatypes. This option with a default of true
-  # will be added in 22.01, we will disable the datatypes on the big
-  # public servers during that release. This option will be switched to
-  # False by default in 22.05 and this broken functionality will be
-  # removed all together during some future release.
-  #load_tool_shed_datatypes: true
-
   # Monitor the tools and tool directories listed in any tool config
   # file specified in tool_config_file option.  If changes are found,
   # tools are automatically reloaded. Watchdog (
   # https://pypi.org/project/watchdog/ ) must be installed and available
   # to Galaxy to use this option. Other options include 'auto' which
   # will attempt to watch tools if the watchdog library is available but
   # won't fail to load Galaxy if it is not and 'polling' which will use
@@ -551,19 +661,47 @@
 
   # Monitor the interactive tours directory specified in the
   # 'tour_config_dir' option. If changes are found, modified tours are
   # automatically reloaded. Takes the same values as the 'watch_tools'
   # option.
   #watch_tours: 'false'
 
+  # Location of files available for a short time as downloads (short
+  # term storage). This directory is exclusively used for serving
+  # dynamically generated downloadable content. Galaxy may uses the
+  # new_file_path parameter as a general temporary directory and that
+  # directory should be monitored by a tool such as tmpwatch in
+  # production environments. short_term_storage_dir on the other hand is
+  # monitored by Galaxy's task framework and should not require such
+  # external tooling.
+  # The value of this option will be resolved with respect to
+  # <cache_dir>.
+  #short_term_storage_dir: short_term_web_storage
+
+  # Default duration before short term web storage files will be cleaned
+  # up by Galaxy tasks (in seconds). The default duration is 1 day.
+  #short_term_storage_default_duration: 86400
+
+  # The maximum duration short term storage files can hosted before they
+  # will be marked for clean up.  The default setting of 0 indicates no
+  # limit here.
+  #short_term_storage_maximum_duration: 0
+
+  # How many seconds between instances of short term storage being
+  # cleaned up in default Celery task configuration.
+  #short_term_storage_cleanup_interval: 3600
+
   # Configured FileSource plugins.
   # The value of this option will be resolved with respect to
   # <config_dir>.
   #file_sources_config_file: file_sources_conf.yml
 
+  # FileSource plugins described embedded into Galaxy's config.
+  #file_sources: null
+
   # Enable Galaxy to fetch containers registered with quay.io generated
   # from tool requirements resolved through Conda. These containers
   # (when available) have been generated using mulled -
   # https://github.com/mulled. Container availability will vary by tool,
   # this option will only be used for job destinations with Docker or
   # Singularity enabled.
   #enable_mulled_containers: true
@@ -696,23 +834,14 @@
 
   # Visualizations config directory: where to look for individual
   # visualization plugins.  The path is relative to the Galaxy root dir.
   # To use an absolute path begin the path with '/'.  This is a
   # comma-separated list.
   #visualization_plugins_directory: config/plugins/visualizations
 
-  # Interactive environment plugins root directory: where to look for
-  # interactive environment plugins.  By default none will be loaded.
-  # Set to config/plugins/interactive_environments to load Galaxy's
-  # stock plugins. These will require Docker to be configured and have
-  # security considerations, so proceed with caution. The path is
-  # relative to the Galaxy root dir.  To use an absolute path begin the
-  # path with '/'.  This is a comma-separated list.
-  #interactive_environment_plugins_directory: null
-
   # Interactive tour directory: where to store interactive tour
   # definition files. Galaxy ships with several basic interface tours
   # enabled, though a different directory with custom tours can be
   # specified here. The path is relative to the Galaxy root dir.  To use
   # an absolute path begin the path with '/'.  This is a comma-separated
   # list.
   #tour_config_dir: config/plugins/tours
@@ -728,20 +857,14 @@
   # Each job is given a unique empty directory as its current working
   # directory. This option defines in what parent directory those
   # directories will be created.
   # The value of this option will be resolved with respect to
   # <data_dir>.
   #job_working_directory: jobs_directory
 
-  # If using a cluster, Galaxy will write job scripts and stdout/stderr
-  # to this directory.
-  # The value of this option will be resolved with respect to
-  # <data_dir>.
-  #cluster_files_directory: pbs
-
   # Mako templates are compiled as needed and cached for reuse, this
   # directory is used for the cache
   # The value of this option will be resolved with respect to
   # <cache_dir>.
   #template_cache_path: compiled_templates
 
   # Set to false to disable various checks Galaxy will do to ensure it
@@ -1098,15 +1221,16 @@
   # Class of the message box under the masthead. Possible values are:
   # 'info' (the default), 'warning', 'error', 'done'.
   #message_box_class: info
 
   # Append "{brand}" text to the masthead.
   #brand: null
 
-  # Display the "Galaxy" text in the masthead.
+  # This option has been deprecated, use the `logo_src` instead to
+  # change the default logo including the galaxy brand title.
   #display_galaxy_brand: true
 
   # Format string used when showing date and time information. The
   # string may contain: - the directives used by Python time.strftime()
   # function (see
   # https://docs.python.org/library/time.html#time.strftime), - $locale
   # (complete format string for the server locale), - $iso8601 (complete
@@ -1119,14 +1243,19 @@
   # 'doc' may be be specified as well for each entry.
   # If this is null (the default), a simple configuration containing
   # just Dockstore will be used.
   # The value of this option will be resolved with respect to
   # <config_dir>.
   #trs_servers_config_file: trs_servers_conf.yml
 
+  # Server-wide default selection to use the legacy history during the
+  # transition period, after which this option will disappear.  Users
+  # will remain able to swap back and forth per their preference.
+  #use_legacy_history: false
+
   # Location of the configuration file containing extra user
   # preferences.
   # The value of this option will be resolved with respect to
   # <config_dir>.
   #user_preferences_extra_conf_path: user_preferences_extra_conf.yml
 
   # Default localization for Galaxy UI. Allowed values are listed at the
@@ -1142,16 +1271,15 @@
   #galaxy_url_prefix: /
 
   # URL (with schema http/https) of the Galaxy instance as accessible
   # within your local network. This URL is used as a default by pulsar
   # file staging and Interactive Tool containers for communicating back
   # with Galaxy via the API.
   # If you plan to run Interactive Tools make sure the docker container
-  # can reach this URL. For more details see
-  # `job_conf.xml.interactivetools`.
+  # can reach this URL.
   #galaxy_infrastructure_url: http://localhost:8080
 
   # If the above URL cannot be determined ahead of time in dynamic
   # environments but the port which should be used to access Galaxy can
   # be - this should be set to prevent Galaxy from having to guess.  For
   # example if Galaxy is sitting behind a proxy with REMOTE_USER enabled
   # - infrastructure shouldn't talk to Python processes directly and
@@ -1163,56 +1291,45 @@
   # This can be an absolute or relative URL.
   #welcome_url: /static/welcome.html
 
   # The URL linked by the "Galaxy/brand" text.
   #logo_url: /
 
   # The brand image source.
-  #logo_src: /static/favicon.png
+  #logo_src: /static/favicon.svg
 
   # The custom brand image source.
   #logo_src_secondary: null
 
   # The URL linked by the "Galaxy Help" link in the "Help" menu.
-  #helpsite_url: null
+  #helpsite_url: https://help.galaxyproject.org/
 
-  # The URL linked by the "Wiki" link in the "Help" menu.
+  # The URL linked by the "Community Hub" link in the "Help" menu.
   #wiki_url: https://galaxyproject.org/
 
   # The URL linked for quota information in the UI.
   #quota_url: https://galaxyproject.org/support/account-quotas/
 
   # The URL linked by the "Support" link in the "Help" menu.
   #support_url: https://galaxyproject.org/support/
 
   # The URL linked by the "How to Cite Galaxy" link in the "Help" menu.
   #citation_url: https://galaxyproject.org/citing-galaxy
 
   # The URL linked by the "Galaxy Version" link in the "Help" menu.
   #release_doc_base_url: https://docs.galaxyproject.org/en/release_
 
-  # The URL linked by the "Search" link in the "Help" menu.
-  #search_url: https://galaxyproject.org/search/
-
-  # The URL linked by the "Mailing Lists" link in the "Help" menu.
-  #mailing_lists_url: https://galaxyproject.org/mailing-lists/
-
   # The URL linked by the "Videos" link in the "Help" menu.
-  #screencasts_url: https://vimeo.com/galaxyproject
+  #screencasts_url: https://www.youtube.com/c/galaxyproject
 
   # The URL linked by the "Terms and Conditions" link in the "Help"
   # menu, as well as on the user registration and login forms and in the
   # activation emails.
   #terms_url: null
 
-  # The URL linked by the "Galaxy Q&A" link in the "Help" menu The
-  # Galaxy Q&A site is under development; when the site is done, this
-  # URL will be set and uncommented.
-  #qa_url: null
-
   # Serve static content, which must be enabled if you're not serving it
   # via a proxy server.  These options should be self explanatory and so
   # are not documented individually.  You can use these paths (or ones
   # in the proxy server) to point to your own styles.
   #static_enabled: true
 
   # Serve static content, which must be enabled if you're not serving it
@@ -1398,22 +1515,43 @@
   # if you are managing the proxy manually.
   #dynamic_proxy_golang_api_key: null
 
   # If true, Galaxy will attempt to configure a simple root logger if a
   # "loggers" section does not appear in this configuration file.
   #auto_configure_logging: true
 
-  # Verbosity of console log messages.  Acceptable values can be found
+  # Log destination, defaults to special value "stdout" that logs to
+  # standard output. If set to anything else, then it will be
+  # interpreted as a path that will be used as the log file, and logging
+  # to stdout will be disabled.
+  #log_destination: stdout
+
+  # Size of log file at which size it will be rotated as per the
+  # documentation in
+  # https://docs.python.org/library/logging.handlers.html#logging.handlers.RotatingFileHandler
+  # If log_rotate_count is not also set, no log rotation will be
+  # performed. A value of 0 (the default) means no rotation. Size can be
+  # a number of bytes or a human-friendly representation like "100 MB"
+  # or "1G".
+  #log_rotate_size: '0'
+
+  # Number of log file backups to keep, per the documentation in
+  # https://docs.python.org/library/logging.handlers.html#logging.handlers.RotatingFileHandler
+  # Any additional rotated log files will automatically be pruned. If
+  # log_rotate_size is not also set, no log rotation will be performed.
+  # A value of 0 (the default) means no rotation.
+  #log_rotate_count: 0
+
+  # Verbosity of console log messages. Acceptable values can be found
   # here: https://docs.python.org/library/logging.html#logging-levels A
   # custom debug level of "TRACE" is available for even more verbosity.
   #log_level: DEBUG
 
-  # Controls where and how the server logs messages. If unset, the
-  # default is to log all messages to standard output at the level
-  # defined by the `log_level` configuration option. Configuration is
+  # Controls where and how the server logs messages. If set, overrides
+  # all settings in the log_* configuration options. Configuration is
   # described in the documentation at:
   # https://docs.galaxyproject.org/en/master/admin/config_logging.html
   #logging: null
 
   # Print database operations to the server log (warning, quite
   # verbose!).
   #database_engine_option_echo: false
@@ -1452,15 +1590,15 @@
   #sanitize_all_html: true
 
   # Datasets created by tools listed in this file are trusted and will
   # not have their HTML sanitized on display.  This can be manually
   # edited or manipulated through the Admin control panel -- see "Manage
   # Allowlist"
   # The value of this option will be resolved with respect to
-  # <mutable_config_dir>.
+  # <managed_config_dir>.
   #sanitize_allowlist_file: sanitize_allowlist.txt
 
   # By default Galaxy will serve non-HTML tool output that may
   # potentially contain browser executable JavaScript content as plain
   # text.  This will for instance cause SVG datasets to not render
   # properly and so may be disabled by setting this option to true.
   #serve_xss_vulnerable_mimetypes: false
@@ -1482,19 +1620,14 @@
   #trust_jupyter_notebook_conversion: false
 
   # Debug enables access to various config options useful for
   # development and debugging: use_lint, use_profile, and
   # use_printdebug.  It also causes the files used by PBS/SGE
   # (submission script, output, and error) to remain on disk after the
   # job is complete.
-  # In addition, this will set uWSGI's `honour-stdin` option to `true`;
-  # thus, preventing uWSGI from remapping stdin to `/dev/null` and
-  # enabling debugging with tools like pdb. To keep uWSGI's default
-  # setting, set `honor-stdin` to `false` in the `uwsgi` section of this
-  # configuration file.
   #debug: false
 
   # Check for WSGI compliance.
   #use_lint: false
 
   # Run the Python profiler on each request.
   #use_profile: false
@@ -1505,28 +1638,25 @@
   # When stopping Galaxy cleanly, how much time to give various
   # monitoring/polling threads to finish before giving up on joining
   # them. Set to 0 to disable this and terminate without waiting. Among
   # others, these threads include the job handler workers, which are
   # responsible for preparing/submitting and collecting/finishing jobs,
   # and which can cause job errors if not shut down cleanly. If using
   # supervisord, consider also increasing the value of `stopwaitsecs`.
-  # If using job handler mules, consider also setting the
-  # `mule-reload-mercy` uWSGI option. See the Galaxy Admin Documentation
-  # for more.
+  # See the Galaxy Admin Documentation for more.
   #monitor_thread_join_timeout: 30
 
   # Write thread status periodically to 'heartbeat.log',  (careful, uses
   # disk space rapidly!).  Useful to determine why your processes may be
   # consuming a lot of CPU.
   #use_heartbeat: false
 
   # Control the period (in seconds) between dumps. Use -1 to disable.
   # Regardless of this setting, if use_heartbeat is enabled, you can
-  # send a Galaxy process (unless running with uWSGI) SIGUSR1 (`kill
-  # -USR1`) to force a dump.
+  # send a Galaxy process SIGUSR1 (`kill -USR1`) to force a dump.
   #heartbeat_interval: 20
 
   # Heartbeat log filename. Can accept the template variables
   # {server_name} and {pid}
   #heartbeat_log: heartbeat_{server_name}.log
 
   # Log to Sentry Sentry is an open source logging and error aggregation
@@ -1536,14 +1666,24 @@
   # <project_name> -> Settings -> API Keys.
   #sentry_dsn: null
 
   # Determines the minimum log level that will be sent as an event to
   # Sentry. Possible values are DEBUG, INFO, WARNING, ERROR or CRITICAL.
   #sentry_event_level: ERROR
 
+  # Set to a number between 0 and 1. With this option set, every
+  # transaction created will have that percentage chance of being sent
+  # to Sentry. A value higher than 0 is required to analyze performance.
+  #sentry_traces_sample_rate: 0.0
+
+  # Use this option to provide the path to location of the CA
+  # (Certificate Authority) certificate file if the sentry server uses a
+  # self-signed certificate.
+  #sentry_ca_certs: null
+
   # Log to statsd Statsd is an external statistics aggregator
   # (https://github.com/etsy/statsd) Enabling the following options will
   # cause galaxy to log request timing and other statistics to the
   # configured statsd instance.  The statsd_prefix is useful if you are
   # running multiple Galaxy instances and want to segment statistics
   # between them within the same aggregator.
   #statsd_host: null
@@ -1620,71 +1760,77 @@
   # archive.  By default, Galaxy allows users to select from a few
   # different archive formats if testing shows that Galaxy is able to
   # create files using these formats. Specific formats can be disabled
   # with this option, separate more than one format with commas.
   # Available formats are currently 'zip', 'gz', and 'bz2'.
   #disable_library_comptypes: null
 
-  # Boosts are used to customize this instance's toolbox search. The
-  # higher the boost, the more importance the scoring algorithm gives to
-  # the given field.  Section refers to the tool group in the tool
-  # panel.  Rest of the fields are tool's attributes.
-  #tool_name_boost: 9.0
-
-  # Boosts are used to customize this instance's toolbox search. The
-  # higher the boost, the more importance the scoring algorithm gives to
-  # the given field.  Section refers to the tool group in the tool
-  # panel.  Rest of the fields are tool's attributes.
-  #tool_id_boost: 9.0
-
-  # Boosts are used to customize this instance's toolbox search. The
-  # higher the boost, the more importance the scoring algorithm gives to
-  # the given field.  Section refers to the tool group in the tool
-  # panel.  Rest of the fields are tool's attributes.
+  # In tool search, a query match against a tool's name text will
+  # receive this score multiplier.
+  #tool_name_boost: 20.0
+
+  # If a search query matches a tool name exactly, the score will be
+  # multiplied by this factor.
+  #tool_name_exact_multiplier: 10.0
+
+  # In tool search, a query match against a tool's ID text will receive
+  # this score multiplier. The query must be an exact match against ID
+  # in order to be counted as a match.
+  #tool_id_boost: 20.0
+
+  # In tool search, a query match against a tool's section text will
+  # receive this score multiplier.
   #tool_section_boost: 3.0
 
-  # Boosts are used to customize this instance's toolbox search. The
-  # higher the boost, the more importance the scoring algorithm gives to
-  # the given field.  Section refers to the tool group in the tool
-  # panel.  Rest of the fields are tool's attributes.
-  #tool_description_boost: 2.0
-
-  # Boosts are used to customize this instance's toolbox search. The
-  # higher the boost, the more importance the scoring algorithm gives to
-  # the given field.  Section refers to the tool group in the tool
-  # panel.  Rest of the fields are tool's attributes.
+  # In tool search, a query match against a tool's description text will
+  # receive this score multiplier.
+  #tool_description_boost: 8.0
+
+  # In tool search, a query match against a tool's label text will
+  # receive this score multiplier.
   #tool_label_boost: 1.0
 
-  # Boosts are used to customize this instance's toolbox search. The
-  # higher the boost, the more importance the scoring algorithm gives to
-  # the given field.  Section refers to the tool group in the tool
-  # panel.  Rest of the fields are tool's attributes.
-  #tool_stub_boost: 5.0
-
-  # Boosts are used to customize this instance's toolbox search. The
-  # higher the boost, the more importance the scoring algorithm gives to
-  # the given field.  Section refers to the tool group in the tool
-  # panel.  Rest of the fields are tool's attributes.
-  #tool_help_boost: 0.5
+  # A stub is parsed from the GUID as "owner/repo/tool_id". In tool
+  # search, a query match against a tool's stub text will receive this
+  # score multiplier.
+  #tool_stub_boost: 2.0
+
+  # In tool search, a query match against a tool's help text will
+  # receive this score multiplier.
+  #tool_help_boost: 1.0
+
+  # The lower this parameter, the greater the diminishing reward for
+  # term frequency in the help text. A higher K1 increases the level of
+  # reward for additional occurences of a term. The default value will
+  # provide a slight increase in score for the first, second and third
+  # occurrence and little reward thereafter.
+  #tool_help_bm25f_k1: 0.5
 
-  # Limits the number of results in toolbox search.  Can be used to
-  # tweak how many results will appear.
+  # Limits the number of results in toolbox search. Use to set the
+  # maximum number of tool search results to display.
   #tool_search_limit: 20
 
-  # Enable/ disable Ngram-search for tools. It makes tool search results
-  # tolerant for spelling mistakes in the query by dividing the query
-  # into multiple ngrams and search for each ngram
+  # Disabling this will prevent partial matches on tool names.
+  # Enable/disable Ngram-search for tools. It makes tool search results
+  # tolerant for spelling mistakes in the query, and will also match
+  # query substrings e.g. "genome" will match "genomics" or
+  # "metagenome".
   #tool_enable_ngram_search: true
 
-  # Set minimum size of ngrams
+  # Set minimum character length of ngrams
   #tool_ngram_minsize: 3
 
-  # Set maximum size of ngrams
+  # Set maximum character length of ngrams
   #tool_ngram_maxsize: 4
 
+  # Ngram matched scores will be multiplied by this factor. Should
+  # always be below 1, because an ngram match is a partial match of a
+  # search term.
+  #tool_ngram_factor: 0.2
+
   # Set tool test data directory. The test framework sets this value to
   # 'test-data,https://github.com/galaxyproject/galaxy-test-data.git'
   # which will cause Galaxy to clone down extra test data on the fly for
   # certain tools distributed with Galaxy but this is likely not
   # appropriate for production systems. Instead one can simply clone
   # that repository directly and specify a path here instead of a Git
   # HTTP repository.
@@ -1728,14 +1874,18 @@
   # header 'GX_SECRET' that is identical to the one below.
   #remote_user_secret: USING THE DEFAULT IS NOT SECURE!
 
   # If use_remote_user is enabled, you can set this to a URL that will
   # log your users out.
   #remote_user_logout_href: null
 
+  # This is the default url to which users are redirected after they log
+  # out.
+  #post_user_logout_href: /root/login?is_logout_redirect=true
+
   # If your proxy and/or authentication source does not normalize e-mail
   # addresses or user names being passed to Galaxy - set this option to
   # true to force these to lower case.
   #normalize_remote_user_email: false
 
   # If an e-mail address is specified here, it will hijack remote user
   # mechanics (``use_remote_user``) and have the webapp inject a single
@@ -1754,14 +1904,18 @@
   # Force everyone to log in (disable anonymous access).
   #require_login: false
 
   # Show the site's welcome page (see welcome_url) alongside the login
   # page (even if require_login is true).
   #show_welcome_with_login: false
 
+  # Controls the order of the login page to prefer Custos-based login
+  # and registration.
+  #prefer_custos_login: false
+
   # Allow unregistered users to create new accounts (otherwise, they
   # will have to be created by an admin).
   #allow_user_creation: true
 
   # Allow administrators to delete accounts.
   #allow_user_deletion: false
 
@@ -1834,17 +1988,14 @@
   # You are responsible for removing personal data from backups.
   # This forces expose_user_email and expose_user_name to be false, and
   # forces user_deletion to be true to support the right to erasure.
   # Please read the GDPR section under the special topics area of the
   # admin documentation.
   #enable_beta_gdpr: false
 
-  # Enable the new container interface for Interactive Environments
-  #enable_beta_containers_interface: false
-
   # Enable beta workflow modules that should not yet be considered part
   # of Galaxy's stable API. (The module state definitions may change and
   # workflows built using these modules may not function in the future.)
   #enable_beta_workflow_modules: false
 
   # Comma-separated list of the EDAM panel views to load - choose from
   # merged, operations, topics. Set to empty string to disable EDAM all
@@ -1944,15 +2095,53 @@
   #api_allow_run_as: null
 
   # API key that allows performing some admin actions without actually
   # having a real admin user in the database and config. Only set this
   # if you need to bootstrap Galaxy, in particular to create a real
   # admin user account via API. You should probably not set this on a
   # production server.
-  #master_api_key: null
+  #bootstrap_admin_api_key: null
+
+  # Service ID for GA4GH services (exposed via the service-info endpoint
+  # for the Galaxy DRS API). If unset, one will be generated using the
+  # URL the target API requests are made against.
+  # For more information on GA4GH service definitions - check out
+  # https://github.com/ga4gh-discovery/ga4gh-service-registry and
+  # https://editor.swagger.io/?url=https://raw.githubusercontent.com/ga4gh-discovery/ga4gh-service-registry/develop/service-registry.yaml
+  # This value should likely reflect your service's URL. For instance
+  # for usegalaxy.org this value should be org.usegalaxy. Particular
+  # Galaxy implementations will treat this value as a prefix and append
+  # the service type to this ID. For instance for the DRS service "id"
+  # (available via the DRS API) for the above configuration value would
+  # be org.usegalaxy.drs.
+  #ga4gh_service_id: null
+
+  # Service name for host organization (exposed via the service-info
+  # endpoint for the Galaxy DRS API). If unset, one will be generated
+  # using ga4gh_service_id.
+  # For more information on GA4GH service definitions - check out
+  # https://github.com/ga4gh-discovery/ga4gh-service-registry and
+  # https://editor.swagger.io/?url=https://raw.githubusercontent.com/ga4gh-discovery/ga4gh-service-registry/develop/service-registry.yaml
+  #ga4gh_service_organization_name: null
+
+  # Organization URL for host organization (exposed via the service-info
+  # endpoint for the Galaxy DRS API). If unset, one will be generated
+  # using the URL the target API requests are made against.
+  # For more information on GA4GH service definitions - check out
+  # https://github.com/ga4gh-discovery/ga4gh-service-registry and
+  # https://editor.swagger.io/?url=https://raw.githubusercontent.com/ga4gh-discovery/ga4gh-service-registry/develop/service-registry.yaml
+  #ga4gh_service_organization_url: null
+
+  # Service environment (exposed via the service-info endpoint for the
+  # Galaxy DRS API) for implemented GA4GH services.
+  # Suggested values are prod, test, dev, staging.
+  # For more information on GA4GH service definitions - check out
+  # https://github.com/ga4gh-discovery/ga4gh-service-registry and
+  # https://editor.swagger.io/?url=https://raw.githubusercontent.com/ga4gh-discovery/ga4gh-service-registry/develop/service-registry.yaml
+  #ga4gh_service_environment: null
 
   # Enable tool tags (associating tools with tags).  This has its own
   # option since its implementation has a few performance implications
   # on startup for large servers.
   #enable_tool_tags: false
 
   # Enable a feature when running workflows.  When enabled, default
@@ -1972,16 +2161,21 @@
   # replacement parameters within tool steps). In the future 'force' may
   # be added an option for Galaskio-style servers that should only
   # render simplified workflows.
   #simplified_workflow_run_ui: prefer
 
   # When the simplified workflow run form is rendered, should the
   # invocation outputs be sent to the 'current' history or a 'new'
-  # history.
-  #simplified_workflow_run_ui_target_history: current
+  # history. If the user should be presented and option between these -
+  # set this to 'prefer_current' or 'prefer_new' to display a runtime
+  # setting with the corresponding default. The default is to provide
+  # the user this option and default it to the current history (the
+  # traditional behavior of Galaxy for years) - this corresponds to the
+  # setting 'prefer_current'.
+  #simplified_workflow_run_ui_target_history: prefer_current
 
   # When the simplified workflow run form is rendered, should the
   # invocation use job caching. This isn't a boolean so an option for
   # 'show-selection' can be added later.
   #simplified_workflow_run_ui_job_cache: 'off'
 
   # The URL to the myExperiment instance being used (omit scheme but
@@ -2070,18 +2264,18 @@
   # one way to do this, and they are explained in detail in the
   # documentation:
   # https://docs.galaxyproject.org/en/master/admin/scaling.html
   # By default, Galaxy manages and executes jobs from within a single
   # process and notifies itself of new jobs via in-memory queues.  Jobs
   # are run locally on the system on which Galaxy is started.  Advanced
   # job running capabilities can be configured through the job
-  # configuration file.
+  # configuration file or the <job_config> option.
   # The value of this option will be resolved with respect to
   # <config_dir>.
-  #job_config_file: job_conf.xml
+  #job_config_file: job_conf.yml
 
   # Description of job running configuration, can be embedded into
   # Galaxy configuration or loaded from an additional file with the
   # job_config_file option.
   #job_config: null
 
   # Rather than specifying a dependency_resolvers_config_file, the
@@ -2098,19 +2292,19 @@
   # object - so this is ideal for automating the configuration of
   # dependency resolution from one application that uses a
   # DependencyManager to another.
   #dependency_resolution: null
 
   # When jobs fail due to job runner problems, Galaxy can be configured
   # to retry these or reroute the jobs to new destinations. Very fine
-  # control of this is available with resubmit declarations in
-  # job_conf.xml. For simple deployments of Galaxy though, the following
+  # control of this is available with resubmit declarations in the job
+  # config. For simple deployments of Galaxy though, the following
   # attribute can define resubmission conditions for all job
   # destinations. If any job destination defines even one resubmission
-  # condition explicitly in job_conf.xml - the condition described by
+  # condition explicitly in the job config - the condition described by
   # this option will not apply to that destination. For instance, the
   # condition: 'attempt < 3 and unknown_error and (time_running < 300 or
   # time_since_queued < 300)' would retry up to two times jobs that
   # didn't fail due to detected memory or walltime limits but did fail
   # quickly (either while queueing or running). The commented out
   # default below results in no default job resubmission condition,
   # failing jobs are just failed outright.
@@ -2143,21 +2337,31 @@
   # jobs.  This thread operates in a loop and sleeps for the given
   # number of seconds at the end of each iteration. This can be
   # decreased if extremely high job throughput is necessary, but doing
   # so can increase CPU usage of handler processes. Float values are
   # allowed.
   #job_runner_monitor_sleep: 1.0
 
-  # Determines how metadata will be set. Valid values are `directory`
-  # and `extended`. In extended mode jobs will decide if a tool run
-  # failed, the object stores configuration is serialized and made
-  # available to the job and is used for writing output datasets to the
-  # object store as part of the job and dynamic output discovery (e.g.
-  # discovered datasets <discover_datasets>, unpopulated collections,
-  # etc) happens as part of the job.
+  # Each Galaxy workflow handler process runs one thread responsible for
+  # checking the state of active workflow invocations.  This thread
+  # operates in a loop and sleeps for the given number of seconds at the
+  # end of each iteration. This can be decreased if extremely high job
+  # throughput is necessary, but doing so can increase CPU usage of
+  # handler processes. Float values are allowed.
+  #workflow_monitor_sleep: 1.0
+
+  # Determines how metadata will be set. Valid values are `directory`,
+  # `extended`, `directory_celery` and `extended_celery`. In extended
+  # mode jobs will decide if a tool run failed, the object stores
+  # configuration is serialized and made available to the job and is
+  # used for writing output datasets to the object store as part of the
+  # job and dynamic output discovery (e.g. discovered datasets
+  # <discover_datasets>, unpopulated collections, etc) happens as part
+  # of the job. In `directory_celery` and `extended_celery` metadata
+  # will be set within a celery task.
   #metadata_strategy: directory
 
   # Although it is fairly reliable, setting metadata can occasionally
   # fail.  In these instances, you can choose to retry setting it
   # internally or leave it in a failed state (since retrying internally
   # may cause the Galaxy process to be unresponsive).  If this option is
   # set to false, the user will be given the option to retry externally,
@@ -2356,14 +2560,21 @@
   # run, but if cache_user_job_count is set to true, it will only happen
   # once per iteration of the handler queue. Although better for
   # performance due to reduced queries, the trade-off is a greater
   # possibility that jobs will be dispatched past the configured limits
   # if running many handlers.
   #cache_user_job_count: false
 
+  # If true, the toolbox will be sorted by tool id when the toolbox is
+  # loaded. This is useful for ensuring that tools are always displayed
+  # in the same order in the UI.  If false, the order of tools in the
+  # toolbox will be preserved as they are loaded from the tool config
+  # files.
+  #toolbox_auto_sort: true
+
   # Define toolbox filters
   # (https://galaxyproject.org/user-defined-toolbox-filters/) that
   # admins may use to restrict the tools to display.
   #tool_filters: null
 
   # Define toolbox filters
   # (https://galaxyproject.org/user-defined-toolbox-filters/) that
@@ -2395,22 +2606,39 @@
   # functions.
   #toolbox_filter_base_modules: galaxy.tools.filters,galaxy.tools.toolbox.filters,galaxy.tool_util.toolbox.filters
 
   # Galaxy uses AMQP internally for communicating between processes.
   # For example, when reloading the toolbox or locking job execution,
   # the process that handled that particular request will tell all
   # others to also reload, lock jobs, etc. For connection examples, see
-  # http://docs.celeryproject.org/projects/kombu/en/latest/userguide/connections.html
+  # https://docs.celeryq.dev/projects/kombu/en/stable/userguide/connections.html
   # Without specifying anything here, galaxy will first attempt to use
   # your specified database_connection above.  If that's not specified
   # either, Galaxy will automatically create and use a separate sqlite
   # database located in your <galaxy>/database folder (indicated in the
   # commented out line below).
   #amqp_internal_connection: sqlalchemy+sqlite:///./database/control.sqlite?isolation_level=IMMEDIATE
 
+  # Configuration options passed to Celery.
+  # To refer to a task by name, use the template `galaxy.foo` where
+  # `foo` is the function name of the task defined in the
+  # galaxy.celery.tasks module.
+  # The `broker_url` option, if unset, defaults to the value of
+  # `amqp_internal_connection`. The `result_backend` option must be set
+  # if the `enable_celery_tasks` option is set.
+  # The galaxy.fetch_data task can be disabled by setting its route to
+  # "disabled": `galaxy.fetch_data: disabled`. (Other tasks cannot be
+  # disabled on a per-task basis at this time.)
+  # For details, see Celery documentation at
+  # https://docs.celeryq.dev/en/stable/userguide/configuration.html.
+  #celery_conf:
+  #  task_routes:
+  #    galaxy.fetch_data: galaxy.external
+  #    galaxy.set_job_metadata: galaxy.external
+
   # Offload long-running tasks to a Celery task queue. Activate this
   # only if you have setup a Celery worker for Galaxy. For details, see
   # https://docs.galaxyproject.org/en/master/admin/production.html
   #enable_celery_tasks: false
 
   # Allow disabling pbkdf2 hashing of passwords for legacy situations.
   # This should normally be left enabled unless there is a specific
@@ -2435,19 +2663,19 @@
   # Allow the display of tool recommendations in workflow editor and
   # after tool execution. If it is enabled and set to true, please
   # enable 'tool_recommendation_model_path' as well
   #enable_tool_recommendations: false
 
   # Set remote path of the trained model (HDF5 file) for tool
   # recommendation.
-  #tool_recommendation_model_path: https://github.com/galaxyproject/galaxy-test-data/raw/master/tool_recommendation_model.hdf5
+  #tool_recommendation_model_path: https://github.com/galaxyproject/galaxy-test-data/raw/master/tool_recommendation_model_v_0.2.hdf5
 
   # Set the number of predictions/recommendations to be made by the
   # model
-  #topk_recommendations: 10
+  #topk_recommendations: 20
 
   # Set path to the additional tool preferences from Galaxy admins. It
   # has two blocks. One for listing deprecated tools which will be
   # removed from the recommendations and another is for adding
   # additional tools to be recommended along side those from the deep
   # learning model.
   # The value of this option will be resolved with respect to
@@ -2463,21 +2691,14 @@
   #overwrite_model_recommendations: false
 
   # Path to error reports configuration file.
   # The value of this option will be resolved with respect to
   # <config_dir>.
   #error_report_file: error_report.yml
 
-  # Path to container interface configuration file. The containers
-  # interface is only used if `enable_beta_containers_interface` config
-  # option is set.
-  # The value of this option will be resolved with respect to
-  # <config_dir>.
-  #containers_config_file: containers_conf.yml
-
   # Path to dynamic tool destinations configuration file.
   # The value of this option will be resolved with respect to
   # <config_dir>.
   #tool_destinations_config_file: tool_destinations.yml
 
   # Location of New User Welcome data, a single directory containing the
   # images and JSON of Topics/Subtopics/Slides as export. This location
@@ -2485,7 +2706,21 @@
   #welcome_directory: plugins/welcome_page/new_user/static/topics/
 
   # Vault config file.
   # The value of this option will be resolved with respect to
   # <config_dir>.
   #vault_config_file: vault_conf.yml
 
+  # Display built-in converters in the tool panel.
+  #display_builtin_converters: true
+
+  # Optional file containing one or more themes for galaxy. If several
+  # themes are defined, users can choose their preferred theme in the
+  # client.
+  # The value of this option will be resolved with respect to
+  # <config_dir>.
+  #themes_config_file: themes_conf.yml
+
+  # Enables user preferences and api endpoint for the beacon
+  # integration.
+  #enable_beacon_integration: false
+
```

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/job_conf.xml.sample_advanced` & `galaxy-config-23.0.1/galaxy/config/sample/job_conf.xml.sample_advanced`

 * *Files 2% similar despite different names*

#### Comparing `galaxy-config-22.1.1/galaxy/config/sample/job_conf.xml.sample_advanced` & `galaxy-config-23.0.1/galaxy/config/sample/job_conf.xml.sample_advanced`

```diff
@@ -108,25 +108,25 @@
                This maybe be useful for instance when Pulsar
                staging is important but a Pulsar server is
                unneeded (for instance if compute servers cannot
                mount Galaxy's files but Galaxy can mount a
                scratch directory available on compute). -->
       <!-- Specify a complete description of the Pulsar app
                to create. If this configuration defines more than
-               one manager - you can specify the manager name 
+               one manager - you can specify the manager name
                using the "manager" destination parameter. For more
                information on configuring a Pulsar app see:
 
                https://github.com/galaxyproject/pulsar/blob/master/app.yml.sample
                https://pulsar.readthedocs.io/en/latest/configure.html
           -->
       <!-- <param id="pulsar_config">path/to/pulsar/app.yml</param> -->
     </plugin>
     <plugin id="k8s" type="runner" load="galaxy.jobs.runners.kubernetes:KubernetesJobRunner">
-      <!-- The Kubernetes (k8s) plugin allows to send jobs to a k8s cluster which shares filesystem with Galaxy.
+      <!-- The Kubernetes (k8s) plugin allows Galaxy to send jobs to a k8s cluster which it shares a filesystem with.
 
                  The shared file system needs to be exposed to k8s through a Persistent Volume (rw) and a Persistent
                  Volume Claim. An example of a Persistent Volume could be, in yaml (access modes, reclaim policy and
                  path are relevant) (persistent_volume.yaml):
 
                     kind: PersistentVolume
                     apiVersion: v1
@@ -143,15 +143,15 @@
                       nfs:
                         path: /scratch1/galaxy_data
                         server: 192.168.64.1
 
                  The path (nfs:path: in the example) set needs to be a parent directory of the directories used for
                  variables “file_path” and “new_file_path” on the galaxy.yml files. Clearly, for this particular example
                  to work, there needs to be a NFS server serving that directory on that ip. Please make sure that you
-                 use reasonable storage size for your set up (possibly larger that the 10Gi written).
+                 use a reasonable storage size for your setup (possibly larger that the 10Gi written).
                  An example of the volume claim should be (this needs to be followed more closely) (pv_claim.yaml):
 
                     kind: PersistentVolumeClaim
                     apiVersion: v1
                     metadata:
                       name: galaxy-pvc
                     spec:
@@ -159,15 +159,15 @@
                         - ReadWriteMany
                       volumeName: pv-galaxy-nfs
                       resources:
                         requests:
                           storage: 2Gi
 
                  The volume claim needs to reference the name of the volume in spec:volumeName. The name of the claim
-                 (metadat:name) is referenced in the plugin definition (see below), through param
+                 (metadata:name) is referenced in the plugin definition (see below), through param
                  "k8s_persistent_volume_claim_name". These two k8s object need to be created before galaxy can use them:
 
                  kubectl create -f <path/to/persistent_volume.yaml>
                  kubectl create -f <path/to/pv_claim.yaml>
 
                  pointing to the Kubernetes cluster that you intend to use.
             -->
@@ -175,15 +175,15 @@
       <!-- This is the path to the kube config file, which is normally on ~/.kube/config, but that will depend on
                  your installation. This is the file that tells the plugin where the k8s cluster is, access credentials,
                  etc. This parameter is not necessary and ignored if k8s_use_service_account is set to True -->
       <!-- <param id="k8s_pull_policy">Default</param> -->
       <!-- Sets the pull policy to be used for all containers invoked for jobs by the Kubernetes cluster. Can take
                  any value among the possible Kubernetes container image pull policies: Always, IfNotPresent or Never
                  (respecting capitalization). Any other value, such as "Default", will not change the setting on k8s and
-                 leave for the containers to run with the default pull policy specified at the cluster (this is normally
+                 leave for the containers to run with the default pull policy of the cluster (this is normally
                  IfNotPresent). Container images using latest are by default always pulled, so you need to use defined
                  versions for offline cases to work (and images need to be previously pulled). -->
       <!-- <param id="k8s_use_service_account">false</param> -->
       <!-- For use when Kubernetes should be accessed from inside a Pod running Galaxy (that is,
                  galaxy is running inside Kubernetes). If this variable is True, then the previous k8s_config_path is
                  not required and actually ignored. It is not necessary to set this value if not setting it to true -->
       <!-- <param id="k8s_job_api_version">batch/v1</param> -->
@@ -197,15 +197,15 @@
       <param id="k8s_working_volume_claim">galaxy_pvc:/mount_point</param>
       <!-- Persistent Volume Claim (PVC) to container mount point mappings, in the format 'PVC:mount_path'
                  If specified, the job's working directory will be mounted from this PVC. -->
       <param id="k8s_persistent_volume_claims">galaxy_pvc1:/mount_point1,galaxy_pvc2:/mount_point2</param>
       <!-- Comma separated list of Persistent Volume Claim (PVC) to container mount point mappings, in the format
                  PVC:mount point
 
-                 Typical mount paths are extra mounts that are expected to be mounted for all jobs, such as 
+                 Typical mount paths are extra mounts that are expected to be mounted for all jobs, such as
                  tool scripts, the CVMFS, and all library paths set in galaxy.yml (or equivalent general galaxy config file). -->
       <!-- <param id="k8s_namespace">default</param> -->
       <!-- The namespace to be used on the Kubernetes cluster, if different from default, this needs to be set
                  accordingly in the PV and PVC detailed above -->
       <!-- <param id="k8s_pod_priority_class">medium-priority-class</param> -->
       <!-- An optional priority class to be assigned to the job, which can control whether or not jobs can
                  preempt existing pods to make room for new ones.
@@ -345,14 +345,25 @@
       <param id="username">username</param>
       <!-- Username to access Mesos cluster. -->
       <param id="password">password</param>
       <!-- Password to access Mesos cluster. -->
       <param id="insecure">false</param>
       <!-- False to communicate with Chronos over HTTPS; true otherwise-->
     </plugin>
+    <plugin id="aws_batch" type="runner" load="galaxy.jobs.runners.aws:AWSBatchJobRunner">
+      <!-- Run `aws configure` with aws cli or set params below -->
+      <!-- <param id="aws_access_key_id">xxxxxxxxx</param>
+            <param id="aws_secret_access_key">xxxxxxxxxxxxxxxxxxx</param>
+            <param id="region">us-west-1</param> -->
+      <!--
+               This runner requires that an AWS EFS is mounted as a local drive  and all Galaxy
+               job-related paths, such as objects, job_directory, tool_directory and so on, are placed
+               in the EFS drive.
+            -->
+    </plugin>
     <!-- Additionally any plugin or destination (below) may define an "enabled" parameter that should
              evaluate to True or False. When setup using
                 <param id="enabled" from_environ="<VAR>">True|False</param>
              plugins and destinations can be conditionally loaded using environment variables.
              Setting the param body above to True or False is required and specifies the default
              used by Galaxy is no environment variable of the specified name is found.
         -->
@@ -366,21 +377,20 @@
 
              The <handlers> container tag takes four optional attributes:
 
                <handlers assign_with="method" max_grab="count" ready_window_size="100" default="id_or_tag"/>
 
                - `assign_with` - How jobs should be assigned to handlers. The value can be a single method or a
                  comma-separated list that will be tried in order. The default depends on whether any handlers and a job
-                 handler "pool" (such as uWSGI mules in a `job-handlers` farm) are configured. Valid methods are
+                 handler "pool" are configured. Valid methods are
                  explained in detail in the documentation referenced above and have the values:
 
                    - `mem-self` - In-memory Self Assignment
                    - `db-self`- Database Self Assignment
                    - `db-preassign` - Database Preassignment
-                   - `uwsgi-mule-message` - uWSGI Mule Messaging
                    - `db-transaction-isolation` - Database Transaction Isolation
                    - `db-skip-locked` - Database SKIP LOCKED
 
                - `max_grab` - Limit the number of jobs that a handler will self-assign per jobs-ready-to-run check loop
                  iteration. This only applies for methods that cause handlers to self-assign multiple jobs at once
                  (db-skip-locked, db-transaction-isolation) and the value is an integer > 0. Default is to grab as many
                  jobs ready to run as possible.
@@ -527,15 +537,15 @@
                adding the '\-\-rm' flag to the command line, the container
                will be removed automatically after the program is complete.
                Galaxy does this by default to clean up the containers it runs,
                but this can be disabled for debugging and such using the following
                command.
           -->
       <!-- <param id="docker_auto_rm">true</param> -->
-      <!-- Override which user to launch Docker container as - defaults to 
+      <!-- Override which user to launch Docker container as - defaults to
                Galaxy's user id. For remote job execution (e.g. Pulsar) set to
                remote job user. Leave empty to not use the -u argument with
                Docker. -->
       <!-- <param id="docker_set_user">$UID</param> -->
       <!-- Pass extra arguments to the docker run command not covered by the
                above options. -->
       <!-- <param id="docker_run_extra_arguments"></param> -->
@@ -581,14 +591,19 @@
       <!-- You can configure singularity to run using sudo - this probably should not
                be set and may be removed in the future.
           -->
       <!-- <param id="singularity_sudo">false</param> -->
       <!-- Following option can be used to tweak sudo command used by
                default. -->
       <!-- <param id="singularity_sudo_cmd">/usr/bin/sudo -extra_param</param> -->
+      <!-- Singularity by default passes most host environment variables into the container.
+               This may be a security or configuration issue, hence galaxy passes the `cleanenv`
+               argument by default. You can turn this off by setting singularity_cleanenv to `false`.
+          -->
+      <!-- <param id="singularity_cleanenv">true</param> -->
       <!-- Pass extra arguments to the singularity exec command not covered by the
                above options. -->
       <!-- <param id="singularity_run_extra_arguments"></param> -->
       <!-- Following command can be used to tweak singularity command. -->
       <!-- <param id="singularity_cmd">/usr/local/custom_docker/docker</param> -->
       <!-- If deployer wants to use singularity for isolation, but does not
                trust tool's specified container - a destination wide override
@@ -773,14 +788,23 @@
       <!-- id of the PulsarRESTJobRunner plugin. Defaults to "pulsar" -->
       <param id="pulsar_runner_id">pulsar</param>
       <!-- Destination to fallback to if no nodes are available -->
       <param id="fallback_destination">local</param>
       <!-- Pick next available server and resubmit if an unknown error occurs -->
       <resubmit condition="unknown_error and attempt &lt;= 3" destination="galaxycloudrunner"/>
     </destination>
+    <destination id="tpv_dispatcher" runner="dynamic">
+      <!-- Demonstrates how to use total-perspective-vortex, which enables dynamic destination
+            selection for entities (Tools, Users, Groups) based on a configurable yaml file.
+            See: https://total-perspective-vortex.readthedocs.io/ for documentation. -->
+      <param id="type">python</param>
+      <param id="function">map_tool_to_destination</param>
+      <param id="rules_module">tpv.rules</param>
+      <param id="tpv_config_files">https://raw.githubusercontent.com/galaxyproject/total-perspective-vortex/main/tests/fixtures/mapping-sample.yml</param>
+    </destination>
     <destination id="docker_dispatch" runner="dynamic">
       <!-- Follow dynamic destination type will send all tool's that
             support docker to static destination defined by
             docker_destination_id (docker_cluster in this example) and all
             other tools to default_destination_id (normal_cluster in this
             example).
             -->
@@ -874,16 +898,16 @@
     <!-- Example CLI LSF Runner: 8 cores and 16 GB ram -->
     <destination id="local_lsf_8cpu_16GbRam" runner="cli">
       <param id="shell_plugin">LocalShell</param>
       <param id="job_plugin">LSF</param>
       <param id="job_memory">16000</param>
       <param id="job_cores">8</param>
       <param id="job_project">BigMem</param>
-      <!-- Exclude hosts in the LSF cluster from receiving the job. 
-                 Useful for avoiding nodes with temporal issues. 
+      <!-- Exclude hosts in the LSF cluster from receiving the job.
+                 Useful for avoiding nodes with temporal issues.
             -->
       <param id="job_excluded_hosts">/path/to/file/with/hosts/to/be/excluded/one_per_line.txt</param>
     </destination>
     <destination id="condor" runner="condor">
       <!-- With no params, jobs are submitted to the 'vanilla' universe with:
                     notification = NEVER
                     getenv = true
@@ -897,16 +921,16 @@
       <!-- <param id="universe">docker</param> -->
       <!-- If the tool has a container specified this one is used.
 
                 <requirements>
                     <container type="docker">bgruening/galaxy-stable</container>
                 </requirements>
 
-            Unless the job destination specifies an override 
-            with docker_container_id_override. If neither of 
+            Unless the job destination specifies an override
+            with docker_container_id_override. If neither of
             these is set a default container can be specified
             with docker_default_container_id. The resolved
             container ID will be passed along to condor as
             the docker_image submission parameter.
             -->
       <!-- <param id="docker_default_container_id">busybox:ubuntu-14.04</param> -->
     </destination>
@@ -928,18 +952,18 @@
                - "memory_limit_reached" (True if and only if the job runner indicates a memory limit was hit)
                - "unknown_error" (True for job or job runner problems that aren't otherwise classified)
                - "attempt" (the re-submission attempt number this is)
                - "seconds_since_queued" (the number of seconds since the last time the job was in a queued state within Galaxy)
                - "seconds_running" (the number of seconds the job was in a running state within Galaxy)
 
              The ``handler`` attribute is optional, if not present, the job's original
-             handler will be reused for the resubmitted job. The ``destination`` attriubte
+             handler will be reused for the resubmitted job. The ``destination`` attribute
              is optional, if not present the job's original destination will be reused for the
              re-submission. The ``delay`` attribute is optional, if present it will cause the job to
-             delay for that number of seconds before being re-submitted. 
+             delay for that number of seconds before being re-submitted.
         -->
     <destination id="short_fast" runner="slurm">
       <param id="nativeSpecification">--time=00:05:00 --nodes=1</param>
       <resubmit condition="walltime_reached" destination="long_slow" handler="sge_handler"/>
     </destination>
     <destination id="long_slow" runner="sge">
       <!-- The destination that you resubmit jobs to can be any runner type -->
@@ -1018,17 +1042,18 @@
 
                  Overrides the runner config. (Not implemented yet)
             -->
       <!-- REQUIRED: To play nicely with the existing galaxy setup for containers. This could be set though
                  internally by the runner. -->
       <param id="docker_enabled">true</param>
       <param id="container_monitor">true</param>
-      <!-- Flag for appending the container monitor command to jobs. This should be set to false
-                 when running Interactive Tools with the kubernetes runner, but is needed for running with the
-                 local docker runner.
+      <!-- Flag for appending the container monitor command to jobs. The monitor is responsible for determining
+                 the IP and port of the container and reporting it to Galaxy. This should be set to false when running
+                 Interactive Tools with the kubernetes runner, but is needed for running with local, DRM, and
+                 non-Kubernetes Pulsar docker runners.
             -->
     </destination>
     <destination id="kubernetes" runner="k8s">
       <!-- <param id="requests_cpu">500m</param> -->
       <!-- <param id="requests_memory">500Mi</param> -->
       <!-- <param id="limits_cpu">2</param> -->
       <!-- <param id="limits_memory">2Gi</param> -->
@@ -1057,20 +1082,20 @@
       <!-- The following are configurations for the container -->
       <param id="docker_enabled">true</param>
       <param id="docker_cpu">1</param>
       <param id="docker_memory">2</param>
       <param id="docker_default_container_id">centos:latest</param>
       <!-- Specify the image on which the jobs have to be executed -->
       <param id="godocker_volumes"/>
-      <!-- Mount the godocker volumes 
+      <!-- Mount the godocker volumes
                  volumes must be separated by commas.
                  eg: <param id="godocker_volumes">home,galaxy</param>
             -->
       <param id="virtualenv">false</param>
-      <!-- If a tool execution in container requires galaxy virtualenv, 
+      <!-- If a tool execution in container requires galaxy virtualenv,
                  then enable it by setting the value to true.
                  Disable venv by setting the value to false.
             -->
     </destination>
     <destination id="chronos_dest" runner="chronos">
       <param id="docker_enabled">true</param>
       <param id="docker_memory">512</param>
@@ -1079,14 +1104,50 @@
       <!-- Directory which is mounted to the container and is parent of
                  the  `job_working_directory`, `file_path`, `new_file_path`
                  directories. Other directories of the data used by tools can
                  be mounted as well, separated by commas.-->
       <param id="max_retries">0</param>
       <!-- Number of retries to attempt if a command returns a non-zero status -->
     </destination>
+    <destination id="aws_batch_auto" runner="aws_batch">
+      <param id="docker_enabled">true</param>
+      <!-- `docker_enabled = true` is always required -->
+      <param id="job_queue">arn_for_Fargate_job_queue, arn_for_EC2_job_queue</param>
+      <!-- Fargate and non-GPU EC2 -->
+      <param id="job_role_arn">arn:aws:iam::xxxxxxxxxxxxxxxxxx</param>
+      <param id="vcpu">1</param>
+      <param id="memory">2048</param>
+      <param id="efs_filesystem_id">fs-xxxxxxxxxxxxxx</param>
+      <param id="efs_mount_point">/mnt/efs/fs1</param>
+      <!-- This is the location where the EFS is mounted -->
+      <param id="fargate_version">1.4.0</param>
+      <!-- `fargate_version` is required to use Fargate compute resources -->
+      <param id="auto_platform">true</param>
+      <!-- To let AWS Batch retry on failed jobs, set the number of attempts to 2-10 and `on_exit` conditions -->
+      <!-- 
+            <param id="retry_attempts">2</param>
+            <param id="retry_on_exit_statusReason">...</param>
+            <param id="retry_on_exit_reason">...</param>
+            <param id="retry_on_exit_exitCode">...</param>
+            <param id="retry_on_exit_action">exit</param>
+            -->
+    </destination>
+    <destination id="aws_batch_gpu" runner="aws_batch">
+      <param id="docker_enabled">true</param>
+      <!-- `docker_enabled = true` is always required -->
+      <param id="job_queue">arn_for_gpu_job_queue</param>
+      <!-- Job queue must be built on GPU-specific compute environment -->
+      <param id="job_role_arn">arn:aws:iam::xxxxxxxxxxxxxxxxxx</param>
+      <param id="vcpu">4</param>
+      <param id="memory">20000</param>
+      <param id="gpu">1</param>
+      <param id="efs_filesystem_id">fs-xxxxxxxxxxxxxx</param>
+      <param id="efs_mount_point">/mnt/efs/fs1</param>
+      <!-- This is the location where the EFS is mounted -->
+    </destination>
     <!-- Templatized destinations - macros can be used to create templated
         destinations with reduced XML duplication. Here we are creating 4 destinations in 4 lines instead of 28 using the macros defined below.
         -->
     <expand macro="foohost_destination" id="foo_small" ncpus="1" walltime="1:00:00"/>
     <expand macro="foohost_destination" id="foo_medium" ncpus="2" walltime="4:00:00"/>
     <expand macro="foohost_destination" id="foo_large" ncpus="8" walltime="24:00:00"/>
     <expand macro="foohost_destination" id="foo_longrunning" ncpus="1" walltime="48:00:00"/>
```

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/job_metrics_conf.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/job_metrics_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/job_resource_params_conf.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/job_resource_params_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/lmod_modules_mapping.yml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/lmod_modules_mapping.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/object_store_conf.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/object_store_conf.xml.sample`

 * *Files 1% similar despite different names*

#### Comparing `galaxy-config-22.1.1/galaxy/config/sample/object_store_conf.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/object_store_conf.xml.sample`

```diff
@@ -139,15 +139,15 @@
     Sample iRODS Object Store
 -->
 <!--
 <object_store type="irods">
     <auth username="rods" password="rods" />
     <resource name="demoResc" />
     <zone name="tempZone" />
-    <connection host="localhost" port="1247" timeout="30" refresh_time="300"/>
+    <connection host="localhost" port="1247" timeout="30" refresh_time="300" connection_pool_monitor_interval="3600"/>
     <cache path="database/object_store_cache_irods" size="1000" />
     <extra_dir type="job_work" path="database/job_working_directory_irods"/>
     <extra_dir type="temp" path="database/tmp_irods"/>
 </object_store>
 -->
 <!--
     Sample Swift Object Store
```

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/oidc_backends_config.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/oidc_backends_config.xml.sample`

 * *Files 2% similar despite different names*

#### Comparing `galaxy-config-22.1.1/galaxy/config/sample/oidc_backends_config.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/oidc_backends_config.xml.sample`

```diff
@@ -81,15 +81,15 @@
   <provider name="Globus">
     <client_id>...</client_id>
     <client_secret>...</client_secret>
     <redirect_uri>http://localhost:8080/authnz/globus/callback</redirect_uri>
     <prompt>consent</prompt>
   </provider>
   <provider name="Custos">
-    <url>https://custos.scigap.org/apiserver/identity-management/v1.0.0/</url>
+    <url>https://dev.custos.usecustos.org/apiserver/identity-management/v1.0.0/</url>
     <client_id>...</client_id>
     <client_secret>...</client_secret>
     <redirect_uri>http://localhost:8080/authnz/custos/callback</redirect_uri>
     <!-- (Optional) Trusted CA certificate file or directory to use when verify Custos authorization server.
              See http://docs.python-requests.org/en/master/user/advanced/#ssl-cert-verification for more information. -->
     <!-- <ca_bundle>/path/to/ca_bundle</ca_bundle> -->
     <!-- (Optional) Override the default Custos well-known URL to point to a different instance -->
@@ -130,14 +130,16 @@
     <!-- (Optional) Override the default Custos well-known URL to point to a different instance -->
     <!-- <well_known_oidc_config_uri>https://.../.well-known/openid-configuration</well_known_oidc_config_uri> -->
     <!-- (Optional) Override the default idp hint -->
     <!-- <idphint>cilogon</idphint> -->
     <!-- (Optional) Enable logging out of the IDP when user logs out of Galaxy -->
     <!-- <enable_idp_logout>false</enable_idp_logout> -->
     <!-- <icon>https://path/to/icon</icon>  -->
+    <!-- (Optional) Enable PKCE for this IDP -->
+    <!-- <pkce_support>false</pkce_support> -->
   </provider>
   <!-- Documentation: https://galaxyproject.org/authnz/config/oidc/idps/elixir-aai  -->
   <provider name="Elixir">
     <client_id>...</client_id>
     <client_secret>...</client_secret>
     <redirect_uri>http://localhost:8080/authnz/elixir/callback</redirect_uri>
     <prompt>consent</prompt>
```

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/oidc_config.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/oidc_config.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/tool_conf.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/tool_conf.xml.sample`

 * *Files 2% similar despite different names*

#### Comparing `galaxy-config-22.1.1/galaxy/config/sample/tool_conf.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/tool_conf.xml.sample`

```diff
@@ -38,14 +38,15 @@
     <tool file="${model_tools_path}/filter_from_file.xml"/>
     <tool file="${model_tools_path}/sort_collection_list.xml"/>
     <tool file="${model_tools_path}/tag_collection_from_file.xml"/>
     <tool file="${model_tools_path}/apply_rules.xml"/>
     <tool file="${model_tools_path}/build_list.xml"/>
     <tool file="${model_tools_path}/build_list_1.2.0.xml"/>
     <tool file="${model_tools_path}/extract_dataset.xml"/>
+    <tool file="${model_tools_path}/duplicate_file_to_collection.xml"/>
   </section>
   <section id="expression_tools" name="Expression Tools">
     <tool file="expression_tools/parse_values_from_file.xml"/>
   </section>
   <section id="liftOver" name="Lift-Over">
     <tool file="extract/liftOver_wrapper.xml"/>
   </section>
@@ -91,15 +92,14 @@
   <section id="group" name="Join, Subtract and Group">
     <tool file="filters/joiner.xml"/>
     <tool file="filters/compare.xml"/>
     <tool file="stats/grouping.xml"/>
   </section>
   <section id="fetchAlignSeq" name="Fetch Alignments/Sequences">
     <tool file="maf/interval2maf_pairwise.xml"/>
-    <tool file="maf/interval2maf.xml"/>
     <tool file="maf/maf_split_by_species.xml"/>
     <tool file="maf/interval_maf_to_merged_fasta.xml"/>
     <tool file="maf/genebed_maf_to_fasta.xml"/>
     <tool file="maf/maf_stats.xml"/>
     <tool file="maf/maf_thread_for_species.xml"/>
     <tool file="maf/maf_limit_to_species.xml"/>
     <tool file="maf/maf_limit_size.xml"/>
@@ -124,19 +124,22 @@
     <tool file="evolution/add_scores.xml"/>
     <tool file="phenotype_association/sift.xml"/>
     <tool file="phenotype_association/linkToGProfile.xml"/>
     <tool file="phenotype_association/linkToDavid.xml"/>
     <tool file="phenotype_association/ldtools.xml"/>
     <tool file="phenotype_association/master2pg.xml"/>
   </section>
-  <!--section id="interactivetools" name="Interactive tools">
+  <!--
+  <section id="interactivetools" name="Interactive tools">
     <tool file="interactive/codingSnps.xml" />
     <tool file="interactive/interactivetool_askomics.xml" />
     <tool file="interactive/interactivetool_bam_iobio.xml" />
     <tool file="interactive/interactivetool_cellxgene.xml" />
     <tool file="interactive/interactivetool_ethercalc.xml" />
     <tool file="interactive/interactivetool_hicbrowser.xml" />
+    <tool file="interactive/interactivetool_jupyter_notebook_1.0.0.xml" />
     <tool file="interactive/interactivetool_jupyter_notebook.xml" />
     <tool file="interactive/interactivetool_neo4j.xml" />
     <tool file="interactive/interactivetool_phinch.xml" />
-  </section-->
+  </section>
+  -->
 </toolbox>
```

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/tool_data_table_conf.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/tool_data_table_conf.xml.sample`

 * *Files 3% similar despite different names*

```diff
@@ -153,8 +153,13 @@
     <table name="hisat2_indexes" type="refgenie" asset="hisat2_index" >
         <file from_config="refgenie_config_file" />
         <field name="value" template="true">${__REFGENIE_UUID__}</field>
         <field name="dbkey" template="true">${__REFGENIE_GENOME__}</field>
         <field name="name" template="true">${__REFGENIE_DISPLAY_NAME__}</field>
         <field name="path" template="true">${__REFGENIE_ASSET__}</field>
     </table>
+    <!-- q2view servers -->
+    <table name="q2view_display" comment_char="#" allow_duplicate_entries="False">
+        <columns>value, name, url</columns>
+        <file path="tool-data/q2view_display.loc" />
+    </table>
 </tables>
```

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/tool_destinations.yml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/tool_destinations.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/tool_recommendations_overwrite.yml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/tool_recommendations_overwrite.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/tool_shed.yml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/tool_shed.yml.sample`

 * *Files 11% similar despite different names*

```diff
@@ -1,103 +1,7 @@
-uwsgi:
-
-  # The address and port on which to listen.  By default, only listen to
-  # localhost (tool_shed will not be accessible over the network).  Use
-  # ':9009' to listen on all available network interfaces.
-  http: 127.0.0.1:9009
-
-  # By default uWSGI allocates a very small buffer (4096 bytes) for the
-  # headers of each request. If you start receiving "invalid request
-  # block size" in your logs, it could mean you need a bigger buffer. We
-  # recommend at least 16384.
-  buffer-size: 16384
-
-  # Number of web server (worker) processes to fork after the
-  # application has loaded. If this is set to greater than 1,
-  # thunder-lock likely should be enabled below.
-  processes: 1
-
-  # Number of threads for each web server process.
-  threads: 4
-
-  # Number of threads for serving static content and handling internal
-  # routing requests.
-  offload-threads: 2
-
-  # Mapping to serve static content.
-  static-map: /static=static
-
-  # Mapping to serve the favicon.
-  static-map: /favicon.ico=static/favicon.ico
-
-  # Allow serving certain assets out of `client`.  Most modern Galaxy
-  # interfaces bundle all of this, but some older pages still serve
-  # these via symlink, requiring this rule.
-  static-safe: client/src/assets
-
-  # Enable the master process manager. Disabled by default for maximum
-  # compatibility with CTRL+C, but should be enabled for use with
-  # --daemon and/or production deployments.
-  master: false
-
-  # Path to the application's Python virtual environment. If using Conda
-  # for Galaxy's framework dependencies (not tools!), do not set this.
-  virtualenv: .venv
-
-  # Path to the application's Python library.
-  pythonpath: lib
-
-  # The entry point which returns the web application (e.g. Galaxy,
-  # Reports, etc.) that you are loading.
-  module: tool_shed.webapp.buildapp:uwsgi_app()
-
-  # Mount the web application (e.g. Galaxy, Reports, etc.) at the given
-  # URL prefix. Cannot be used together with 'module:' above.
-  #mount: /galaxy=tool_shed.webapp.buildapp:uwsgi_app()
-
-  # Make uWSGI rewrite PATH_INFO and SCRIPT_NAME according to
-  # mount-points. Set this to true if a URL prefix is used.
-  manage-script-name: false
-
-  # It is usually a good idea to set this to ``true`` if processes is
-  # greater than 1.
-  thunder-lock: false
-
-  # Cause uWSGI to respect the traditional behavior of dying on SIGTERM
-  # (its default is to brutally reload workers)
-  die-on-term: true
-
-  # Cause uWSGI to gracefully reload workers and mules upon receipt of
-  # SIGINT (its default is to brutally kill workers)
-  hook-master-start: unix_signal:2 gracefully_kill_them_all
-
-  # Cause uWSGI to gracefully reload workers and mules upon receipt of
-  # SIGTERM (its default is to brutally kill workers)
-  hook-master-start: unix_signal:15 gracefully_kill_them_all
-
-  # Feature necessary for proper mule signal handling on Python versions
-  # below 3.7.2. The default is set to false to prevent a runtime error
-  # under Python 3.7.2 and newer (see
-  # https://github.com/unbit/uwsgi/issues/1978).
-  py-call-osafterfork: false
-
-  # Ensure application threads will run if `threads` is unset.
-  enable-threads: true
-
-  # uWSGI default umask. On some systems uWSGI has a default umask of
-  # 000, for Galaxy a somewhat safer default is chosen. If Galaxy
-  # submits jobs as real user then all users needs to be able to read
-  # the files, i.e. the umask needs to be '022' or the Galaxy users need
-  # to be in the same group as the Galaxy system user
-  umask: 027
-
-  # Task for rebuilding Toolshed search indexes using the uWSGI
-  # cron-like interface.
-  cron: 0 -1 -1 -1 -1 python scripts/tool_shed/build_ts_whoosh_index.py -c config/tool_shed.yml --config-section tool_shed
-
 tool_shed:
 
   # Verbosity of console log messages.  Acceptable values can be found
   # here: https://docs.python.org/library/logging.html#logging-levels
   #log_level: DEBUG
 
   # By default, the Tool Shed uses a SQLite database at
@@ -236,23 +140,14 @@
   # the beginning of the header name.
   #remote_user_header: HTTP_REMOTE_USER
 
   # If use_remote_user is enabled, you can set this to a URL that will
   # log your users out.
   #remote_user_logout_href: null
 
-  # Configuration for debugging middleware
-  #debug: false
-
-  # Check for WSGI compliance.
-  #use_lint: false
-
-  # Intercept print statements and show them on the returned page.
-  #use_printdebug: true
-
   # Administrative users - set this to a comma-separated list of valid
   # Tool Shed users (email addresses).  These users will have access to
   # the Admin section of the server, and will have access to create
   # users, groups, roles, libraries, and more.
   #admin_users: null
 
   # Force everyone to log in (disable anonymous access)
@@ -293,17 +188,14 @@
   # Address to join mailing list
   #mailing_join_addr: galaxy-announce-join@bx.psu.edu
 
   # Write thread status periodically to 'heartbeat.log' (careful, uses
   # disk  space rapidly!)
   #use_heartbeat: true
 
-  # Profiling middleware (cProfile based)
-  #use_profile: true
-
   # Enable creation of Galaxy flavor Docker Image
   #enable_galaxy_flavor_docker_image: false
 
   # Show a message box under the masthead.
   #message_box_visible: false
 
   # Show a message box under the masthead.
@@ -415,14 +307,24 @@
   # <project_name> -> Settings -> API Keys.
   #sentry_dsn: null
 
   # Determines the minimum log level that will be sent as an event to
   # Sentry. Possible values are DEBUG, INFO, WARNING, ERROR or CRITICAL.
   #sentry_event_level: ERROR
 
+  # Set to a number between 0 and 1. With this option set, every
+  # transaction created will have that percentage chance of being sent
+  # to Sentry. A value higher than 0 is required to analyze performance.
+  #sentry_traces_sample_rate: 0.0
+
+  # Use this option to provide the path to location of the CA
+  # (Certificate Authority) certificate file if the sentry server uses a
+  # self-signed certificate.
+  #sentry_ca_certs: null
+
   # Galaxy Session Timeout This provides a timeout (in minutes) after
   # which a user will have to log back in. A duration of 0 disables this
   # feature.
   #session_duration: 0
 
   # The URL linked by the "Terms and Conditions" link in the "Help"
   # menu, as well as on the user registration and login forms and in the
@@ -432,14 +334,21 @@
   # XML config file that allows the use of different authentication
   # providers (e.g. LDAP) instead or in addition to local authentication
   # (.sample is used if default does not exist).
   # The value of this option will be resolved with respect to
   # <config_dir>.
   #auth_config_file: auth_conf.xml
 
+  # API key that allows performing some admin actions without actually
+  # having a real admin user in the database and config. Only set this
+  # if you need to bootstrap Galaxy, in particular to create a real
+  # admin user account via API. You should probably not set this on a
+  # production server.
+  #bootstrap_admin_api_key: null
+
   # XML config file that contains additional data table entries for the
   # ToolDataTableManager.  This file is automatically generated based on
   # the current installed tool shed repositories that contain valid
   # tool_data_table_conf.xml.sample files.  At the time of installation,
   # these entries are automatically added to the following file, which
   # is parsed and applied to the ToolDataTableManager at server start
   # up.
```

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/trs_servers_conf.yml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/trs_servers_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/user_preferences_extra_conf.yml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/user_preferences_extra_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/workflow_resource_params_conf.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/workflow_resource_params_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-22.1.1/galaxy/config/sample/workflow_schedulers_conf.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/workflow_schedulers_conf.xml.sample`

 * *Files 26% similar despite different names*

#### Comparing `galaxy-config-22.1.1/galaxy/config/sample/workflow_schedulers_conf.xml.sample` & `galaxy-config-23.0.1/galaxy/config/sample/workflow_schedulers_conf.xml.sample`

```diff
@@ -12,27 +12,15 @@
   <!-- Handlers (Galaxy server processes that perform the scheduling work) can
        be defined here in the same format as in job_conf.xml. By default, the
        handlers defined in job_conf.xml will be used (or the web process that
        receives the workflow scheduling request if handlers are not configured
        in job_conf.xml).
 
        The options here are the same as is documented for <handlers> in
-       job_conf.xml.sample_advanced with two exceptions:
-
-       - If a uWSGI farm named `workflow-schedulers` is present, it will be
-         preferred, followed by `job-handlers`. If any untagged handlers are
-         defined in this configuration they are eligible to schedule workflows
-         in addition to any matching mules.
-       - If uWSGI farms are present, the default assignment method is
-         `db-preassign` rather than `uwsgi-mule-message`, because `db-preassign`
-         is deterministic. All workflows scheduled in a single history will be
-         assigned to the same handler, ensuring they are scheduled serially
-         (preventing their outputs from being interleaved in the history). You
-         can override this by explicitly setting
-         `assign_with="uwsgi-mule-message"`.
+       job_conf.xml.sample_advanced
   -->
   <!--
   <handlers>
     <handler id="handler0"/>
     <handler id="handler1"/>
   </handlers>
   -->
```

### Comparing `galaxy-config-22.1.1/galaxy/config/schema.py` & `galaxy-config-23.0.1/galaxy/config/schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,60 +12,65 @@
     "desc": None,
 }
 
 UNKNOWN_OPTION = {
     "type": "str",
     "required": False,
     "unknown_option": True,
-    "desc": "Unknown option, may want to remove or report to Galaxy team."
+    "desc": "Unknown option, may want to remove or report to Galaxy team.",
 }
 
 
 class Schema:
-
     def __init__(self, mapping):
         self.app_schema = mapping
 
     def get_app_option(self, name):
         try:
             raw_option = self.app_schema[name]
         except KeyError:
             raw_option = UNKNOWN_OPTION
         option = OPTION_DEFAULTS.copy()
         option.update(raw_option)
         return option
 
 
 class AppSchema(Schema):
-
     def __init__(self, schema_path, app_name):
         self.raw_schema = self._read_schema(schema_path)
         self.description = self.raw_schema.get("desc", None)
-        app_schema = self.raw_schema['mapping'][app_name]['mapping']
+        app_schema = self.raw_schema["mapping"][app_name]["mapping"]
         self._preprocess(app_schema)
         super().__init__(app_schema)
 
     def _read_schema(self, path):
         with open(path) as f:
             return ordered_load(f)
 
     def _preprocess(self, app_schema):
         """Populate schema collections used for app configuration."""
         self._defaults = {}  # {config option: default value or null}
         self._reloadable_options = set()  # config options we can reload at runtime
         self._paths_to_resolve = {}  # {config option: referenced config option}
         self._per_host_options = set()  # config options that can be set using a per_host config parameter
+        self._deprecated_aliases = {}
         for key, data in app_schema.items():
-            self._defaults[key] = data.get('default')
-            if data.get('reloadable'):
+            self._defaults[key] = data.get("default")
+            if data.get("deprecated_alias"):
+                self._deprecated_aliases[data.get("deprecated_alias")] = key
+            if data.get("reloadable"):
                 self._reloadable_options.add(key)
-            if data.get('per_host'):
-                self._per_host_options.add(key)
-            if data.get('path_resolves_to'):
-                self._paths_to_resolve[key] = data.get('path_resolves_to')
+            if data.get("per_host"):
+                resolves_to = data.get("resolves_to")
+                if resolves_to:
+                    self._per_host_options.add(resolves_to)
+                else:
+                    self._per_host_options.add(key)
+            if data.get("path_resolves_to"):
+                self._paths_to_resolve[key] = data.get("path_resolves_to")
 
     @property
     def defaults(self):
         return self._defaults
 
     @property
     def paths_to_resolve(self):
@@ -77,36 +82,39 @@
 
     @property
     def per_host_options(self):
         return self._per_host_options
 
     def validate_path_resolution_graph(self):
         """This method is for tests only: we SHOULD validate the schema's path resolution graph
-           as part of automated testing; but we should NOT validate it at runtime.
+        as part of automated testing; but we should NOT validate it at runtime.
         """
+
         def check_exists(option, key):
             if not option:
-                message = "Invalid schema: property '{}' listed as path resolution target " \
+                message = (
+                    "Invalid schema: property '{}' listed as path resolution target "
                     "for '{}' does not exist".format(resolves_to, key)
+                )
                 raise_error(message)
 
         def check_type_is_str_or_any(option, key):
-            if option.get('type') not in ('str', 'any'):
+            if option.get("type") not in ("str", "any"):
                 message = f"Invalid schema: property '{key}' should have type 'str'"
                 raise_error(message)
 
         def check_is_dag():
             visited = set()
             for key in self.paths_to_resolve:
                 visited.clear()
                 while key:
                     visited.add(key)
-                    key = self.app_schema[key].get('path_resolves_to')
+                    key = self.app_schema[key].get("path_resolves_to")
                     if key and key in visited:
-                        raise_error('Invalid schema: cycle detected')
+                        raise_error("Invalid schema: cycle detected")
 
         def raise_error(message):
             log.error(message)
             raise ConfigurationError(message)
 
         for key, resolves_to in self.paths_to_resolve.items():
             print(key)
```

### Comparing `galaxy-config-22.1.1/galaxy/config/schemas/config_schema.yml` & `galaxy-config-23.0.1/galaxy/config/schemas/config_schema.yml`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
   Examples of many of these options are explained in more detail in the Galaxy
   Community Hub.
 
     https://galaxyproject.org/admin/config
 
   Config hackers are encouraged to check there before asking for help.
 mapping:
-  uwsgi: !include uwsgi_schema.yml
   galaxy:
     type: map
     required: true
     mapping:
 
       config_dir:
         type: str
@@ -48,33 +47,51 @@
         required: false
         desc: |
           The directory that will be prepended to relative paths in options specifying
           Galaxy data/cache directories and files (such as the default SQLite database,
           file_path, etc.). Defaults to `database/` if running Galaxy from source or
           `<config_dir>/data` otherwise.
 
+      templates_dir:
+        type: str
+        path_resolves_to: config_dir
+        required: false
+        default: templates
+        desc: |
+          The directory containing custom templates for Galaxy, such as HTML/text email templates. Defaults to 'templates'. Default templates can be found in the Galaxy root under config/templates. These can be copied to <templates_dir> if you wish to customize them.
+
       cache_dir:
         type: str
         default: cache
         path_resolves_to: data_dir
         required: false
         desc: |
           Top level cache directory. Any other cache directories (tool_cache_data_dir,
           template_cache_path, etc.) should be subdirectories.
 
       database_connection:
         type: str
         required: false
         desc: |
-          By default, Galaxy uses a SQLite database at '<data_dir>/universe.sqlite'.  You
-          may use a SQLAlchemy connection string to specify an external database
-          instead.
+          By default, Galaxy uses a SQLite database at '<data_dir>/universe.sqlite'. You
+          may use a SQLAlchemy connection string to specify an external database instead.
 
           Sample default 'sqlite:///<data_dir>/universe.sqlite?isolation_level=IMMEDIATE'
 
+          You may specify additional options that will be passed to the SQLAlchemy
+          database engine by using the prefix "database_engine_option_". For some of these
+          options, default values are provided (e.g. see database_engine_option_pool_size,
+          etc.).
+
+          The same applies to `install_database_connection`, for which you should use the
+          "install_database_engine_option_" prefix.
+
+          For more options, please check SQLAlchemy's documentation at
+          https://docs.sqlalchemy.org/en/14/core/engines.html?highlight=create_engine#sqlalchemy.create_engine
+
       database_engine_option_pool_size:
         type: int
         default: 5
         required: false
         desc: |
           If the server logs errors about not having enough database pool connections,
           you will want to increase these values, or consider running more Galaxy
@@ -292,26 +309,25 @@
           Default path to the directory containing the tools defined in tool_conf.xml.
           Other tool config files must include the tool_path as an attribute in the
           <toolbox> tag.
 
       tool_dependency_dir:
         type: str
         default: dependencies
+        path_resolves_to: data_dir
         required: false
         desc: |
           Various dependency resolver configuration parameters will have defaults set relative
           to this path, such as the default conda prefix, default Galaxy packages path, legacy
           tool shed dependencies path, and the dependency cache directory.
 
           Set the string to null to explicitly disable tool dependency handling.
           If this option is set to none or an invalid path, installing tools with dependencies
           from the Tool Shed or in Conda will fail.
 
-          The value of this option will be resolved with respect to <data_dir>.
-
       dependency_resolvers_config_file:
         type: str
         default: dependency_resolvers_conf.xml
         path_resolves_to: config_dir
         required: false
         desc: |
           Specifies the path to the standalone dependency resolvers configuration file. This
@@ -440,25 +456,14 @@
         default: tool_sheds_conf.xml
         path_resolves_to: config_dir
         required: false
         desc: |
           File containing the Galaxy Tool Sheds that should be made available to
           install from in the admin interface (.sample used if default does not exist).
 
-      load_tool_shed_datatypes:
-        type: bool
-        default: true
-        required: false
-        desc: |
-          This option controls whether legacy datatypes are loaded from installed tool shed repositories.
-          We're are in the process of disabling Tool Shed datatypes. This option with a default of true
-          will be added in 22.01, we will disable the datatypes on the big public servers during that
-          release. This option will be switched to False by default in 22.05 and this broken functionality
-          will be removed all together during some future release.
-
       watch_tools:
         type: str
         default: 'false'
         required: false
         desc: |
           Monitor the tools and tool directories listed in any tool config file specified in
           tool_config_file option.  If changes are found, tools are automatically reloaded.
@@ -490,22 +495,66 @@
         default: 'false'
         required: false
         desc: |
           Monitor the interactive tours directory specified in the 'tour_config_dir' option. If
           changes are found, modified tours are automatically reloaded. Takes the same values as the
           'watch_tools' option.
 
+      short_term_storage_dir:
+        type: str
+        default: short_term_web_storage
+        path_resolves_to: cache_dir
+        required: false
+        desc: |
+          Location of files available for a short time as downloads (short term storage).
+          This directory is exclusively used for serving dynamically generated downloadable
+          content. Galaxy may uses the new_file_path parameter as a general temporary directory
+          and that directory should be monitored by a tool such as tmpwatch in production
+          environments. short_term_storage_dir on the other hand is monitored by Galaxy's task
+          framework and should not require such external tooling.
+
+      short_term_storage_default_duration:
+        type: int
+        required: false
+        default: 86400
+        desc: |
+          Default duration before short term web storage files will be cleaned up by Galaxy
+          tasks (in seconds). The default duration is 1 day.
+
+      short_term_storage_maximum_duration:
+        type: int
+        required: false
+        default: 0
+        desc: |
+          The maximum duration short term storage files can hosted before they will be marked for
+          clean up.  The default setting of 0 indicates no limit here.
+
+      short_term_storage_cleanup_interval:
+        type: int
+        required: false
+        default: 3600
+        desc: |
+          How many seconds between instances of short term storage being cleaned up in default
+          Celery task configuration.
+
       file_sources_config_file:
         type: str
         default: file_sources_conf.yml
         path_resolves_to: config_dir
         required: false
         desc: |
           Configured FileSource plugins.
 
+      file_sources:
+        type: seq
+        sequence:
+          - type: any
+        desc: |
+          FileSource plugins described embedded into Galaxy's config.
+
       enable_mulled_containers:
         type: bool
         default: true
         required: false
         desc: |
           Enable Galaxy to fetch containers registered with quay.io generated
           from tool requirements resolved through Conda. These containers (when
@@ -532,24 +581,23 @@
           resolvers to enable can be embedded into Galaxy's config with this option.
           This has no effect if a container_resolvers_config_file is used.
           Takes the same options that can be set in container_resolvers_config_file.
 
       involucro_path:
         type: str
         default: involucro
+        path_resolves_to: tool_dependency_dir
         required: false
         desc: |
           involucro is a tool used to build Docker or Singularity containers for tools from Conda
           dependencies referenced in tools as `requirement` s. The following path is
           the location of involucro on the Galaxy host. This is ignored if the relevant
           container resolver isn't enabled, and will install on demand unless
           involucro_auto_init is set to false.
 
-          The value of this option will be resolved with respect to <tool_dependency_dir>.
-
       involucro_auto_init:
         type: bool
         default: true
         required: false
         desc: |
           Install involucro as needed to build Docker or Singularity containers for tools. Ignored if
           relevant container resolver is not used.
@@ -699,25 +747,14 @@
         default: config/plugins/visualizations
         required: false
         desc: |
           Visualizations config directory: where to look for individual visualization
           plugins.  The path is relative to the Galaxy root dir.  To use an absolute
           path begin the path with '/'.  This is a comma-separated list.
 
-      interactive_environment_plugins_directory:
-        type: str
-        required: false
-        desc: |
-          Interactive environment plugins root directory: where to look for interactive
-          environment plugins.  By default none will be loaded.  Set to
-          config/plugins/interactive_environments to load Galaxy's stock plugins.
-          These will require Docker to be configured and have security considerations,
-          so proceed with caution. The path is relative to the Galaxy root dir.  To use
-          an absolute path begin the path with '/'.  This is a comma-separated list.
-
       tour_config_dir:
         type: str
         default: config/plugins/tours
         required: false
         desc: |
           Interactive tour directory: where to store interactive tour definition files.
           Galaxy ships with several basic interface tours enabled, though a different
@@ -743,23 +780,14 @@
         desc: |
           Each job is given a unique empty directory as its current working directory.
           This option defines in what parent directory those directories will be
           created.
 
           The value of this option will be resolved with respect to <data_dir>.
 
-      cluster_files_directory:
-        type: str
-        default: pbs
-        path_resolves_to: data_dir
-        required: false
-        desc: |
-          If using a cluster, Galaxy will write job scripts and stdout/stderr to this
-          directory.
-
       template_cache_path:
         type: str
         default: compiled_templates
         path_resolves_to: cache_dir
         required: false
         desc: |
           Mako templates are compiled as needed and cached for reuse, this directory is
@@ -1334,15 +1362,16 @@
 
       display_galaxy_brand:
         type: bool
         default: true
         required: false
         per_host: true
         desc: |
-          Display the "Galaxy" text in the masthead.
+          This option has been deprecated, use the `logo_src` instead to change the
+          default logo including the galaxy brand title.
 
       pretty_datetime_format:
         type: str
         default: $locale (UTC)
         required: false
         desc: |
           Format string used when showing date and time information.
@@ -1363,14 +1392,23 @@
           the specified YAML or JSON file. The file should be a list with
           'id', 'label', and 'api_url' for each entry. Optionally,
           'link_url' and 'doc' may be be specified as well for each entry.
 
           If this is null (the default), a simple configuration containing
           just Dockstore will be used.
 
+      use_legacy_history:
+        type: bool
+        default: false
+        required: false
+        desc: |
+          Server-wide default selection to use the legacy history during the
+          transition period, after which this option will disappear.  Users will
+          remain able to swap back and forth per their preference.
+
       user_preferences_extra_conf_path:
         type: str
         default: 'user_preferences_extra_conf.yml'
         path_resolves_to: config_dir
         required: false
         desc: |
           Location of the configuration file containing extra user preferences.
@@ -1402,15 +1440,15 @@
         desc: |
           URL (with schema http/https) of the Galaxy instance as accessible
           within your local network. This URL is used as a default by pulsar
           file staging and Interactive Tool containers for communicating back with
           Galaxy via the API.
 
           If you plan to run Interactive Tools make sure the docker container
-          can reach this URL. For more details see `job_conf.xml.interactivetools`.
+          can reach this URL.
 
       galaxy_infrastructure_web_port:
         type: int
         default: 8080
         required: false
         desc: |
           If the above URL cannot be determined ahead of time in dynamic environments
@@ -1437,41 +1475,42 @@
         required: false
         per_host: true
         desc: |
           The URL linked by the "Galaxy/brand" text.
 
       logo_src:
         type: str
-        default: /static/favicon.png
+        default: /static/favicon.svg
         required: false
         per_host: true
         desc: |
           The brand image source.
 
       logo_src_secondary:
         type: str
         required: false
         per_host: true
         desc: |
           The custom brand image source.
 
       helpsite_url:
         type: str
-        required: false
+        required: true
+        default: https://help.galaxyproject.org/
         per_host: true
         desc: |
           The URL linked by the "Galaxy Help" link in the "Help" menu.
 
       wiki_url:
         type: str
         default: https://galaxyproject.org/
         required: false
         per_host: true
         desc: |
-          The URL linked by the "Wiki" link in the "Help" menu.
+          The URL linked by the "Community Hub" link in the "Help" menu.
 
       quota_url:
         type: str
         default: https://galaxyproject.org/support/account-quotas/
         required: false
         desc: |
           The URL linked for quota information in the UI.
@@ -1495,54 +1534,30 @@
       release_doc_base_url:
         type: str
         default: https://docs.galaxyproject.org/en/release_
         required: false
         desc: |
           The URL linked by the "Galaxy Version" link in the "Help" menu.
 
-      search_url:
-        type: str
-        default: https://galaxyproject.org/search/
-        required: false
-        per_host: true
-        desc: |
-          The URL linked by the "Search" link in the "Help" menu.
-
-      mailing_lists_url:
-        type: str
-        default: https://galaxyproject.org/mailing-lists/
-        required: false
-        per_host: true
-        desc: |
-          The URL linked by the "Mailing Lists" link in the "Help" menu.
-
       screencasts_url:
         type: str
-        default: https://vimeo.com/galaxyproject
+        default: https://www.youtube.com/c/galaxyproject
         required: false
         per_host: true
         desc: |
           The URL linked by the "Videos" link in the "Help" menu.
 
       terms_url:
         type: str
         required: false
-        per_host: true        
+        per_host: true
         desc: |
           The URL linked by the "Terms and Conditions" link in the "Help" menu, as well
           as on the user registration and login forms and in the activation emails.
 
-      qa_url:
-        type: str
-        required: false
-        desc: |
-          The URL linked by the "Galaxy Q&A" link in the "Help" menu
-          The Galaxy Q&A site is under development; when the site is done, this URL
-          will be set and uncommented.
-
       static_enabled:
         type: bool
         default: true
         required: false
         desc: |
           Serve static content, which must be enabled if you're not serving it via a
           proxy server.  These options should be self explanatory and so are not
@@ -1849,30 +1864,58 @@
         type: bool
         default: true
         required: false
         desc: |
           If true, Galaxy will attempt to configure a simple root logger if a
           "loggers" section does not appear in this configuration file.
 
+      log_destination:
+        type: str
+        default: stdout
+        required: false
+        desc: |
+          Log destination, defaults to special value "stdout" that logs to standard output. If set to anything else,
+          then it will be interpreted as a path that will be used as the log file, and logging to stdout will be
+          disabled.
+
+      log_rotate_size:
+        type: str
+        default: "0"
+        required: false
+        desc: |
+          Size of log file at which size it will be rotated as per the documentation in
+          https://docs.python.org/library/logging.handlers.html#logging.handlers.RotatingFileHandler
+          If log_rotate_count is not also set, no log rotation will be performed. A value of 0 (the default) means no
+          rotation. Size can be a number of bytes or a human-friendly representation like "100 MB" or "1G".
+
+      log_rotate_count:
+        type: int
+        default: 0
+        required: false
+        desc: |
+          Number of log file backups to keep, per the documentation in
+          https://docs.python.org/library/logging.handlers.html#logging.handlers.RotatingFileHandler
+          Any additional rotated log files will automatically be pruned. If log_rotate_size is not also set, no log
+          rotation will be performed. A value of 0 (the default) means no rotation.
+
       log_level:
         type: str
         default: DEBUG
         required: false
         desc: |
-          Verbosity of console log messages.  Acceptable values can be found here:
+          Verbosity of console log messages. Acceptable values can be found here:
           https://docs.python.org/library/logging.html#logging-levels
           A custom debug level of "TRACE" is available for even more verbosity.
 
       logging:
         type: map
         allowempty: true
         desc: |
-          Controls where and how the server logs messages. If unset, the default is to log all messages to standard
-          output at the level defined by the `log_level` configuration option. Configuration is described in the
-          documentation at:
+          Controls where and how the server logs messages. If set, overrides all settings in the log_* configuration
+          options. Configuration is described in the documentation at:
           https://docs.galaxyproject.org/en/master/admin/config_logging.html
 
       database_engine_option_echo:
         type: bool
         default: false
         required: false
         desc: |
@@ -1940,15 +1983,15 @@
         default: sanitize_allowlist.txt
         required: false
         desc: |
           Datasets created by tools listed in this file are trusted and will not have
           their HTML sanitized on display.  This can be manually edited or manipulated
           through the Admin control panel -- see "Manage Allowlist"
 
-          The value of this option will be resolved with respect to <mutable_config_dir>.
+          The value of this option will be resolved with respect to <managed_config_dir>.
 
       serve_xss_vulnerable_mimetypes:
         type: bool
         default: false
         required: false
         desc: |
           By default Galaxy will serve non-HTML tool output that may potentially
@@ -1984,20 +2027,14 @@
         required: false
         desc: |
           Debug enables access to various config options useful for development
           and debugging: use_lint, use_profile, and use_printdebug.  It also
           causes the files used by PBS/SGE (submission script, output, and error)
           to remain on disk after the job is complete.
 
-          In addition, this will set uWSGI's `honour-stdin` option to `true`;
-          thus, preventing uWSGI from remapping stdin to `/dev/null` and
-          enabling debugging with tools like pdb. To keep uWSGI's default
-          setting, set `honor-stdin` to `false` in the `uwsgi` section of this
-          configuration file.
-
       use_lint:
         type: bool
         default: false
         required: false
         desc: |
           Check for WSGI compliance.
 
@@ -2021,17 +2058,16 @@
         required: false
         desc: |
           When stopping Galaxy cleanly, how much time to give various monitoring/polling
           threads to finish before giving up on joining them. Set to 0 to disable this and
           terminate without waiting. Among others, these threads include the job handler
           workers, which are responsible for preparing/submitting and collecting/finishing
           jobs, and which can cause job errors if not shut down cleanly. If using
-          supervisord, consider also increasing the value of `stopwaitsecs`. If using job
-          handler mules, consider also setting the `mule-reload-mercy` uWSGI option. See
-          the Galaxy Admin Documentation for more.
+          supervisord, consider also increasing the value of `stopwaitsecs`. See the
+          Galaxy Admin Documentation for more.
 
       use_heartbeat:
         type: bool
         default: false
         required: false
         desc: |
           Write thread status periodically to 'heartbeat.log',  (careful, uses disk
@@ -2041,15 +2077,15 @@
       heartbeat_interval:
         type: int
         default: 20
         required: false
         desc: |
           Control the period (in seconds) between dumps. Use -1 to disable. Regardless
           of this setting, if use_heartbeat is enabled, you can send a Galaxy process
-          (unless running with uWSGI) SIGUSR1 (`kill -USR1`) to force a dump.
+          SIGUSR1 (`kill -USR1`) to force a dump.
 
       heartbeat_log:
         type: str
         default: heartbeat_{server_name}.log
         required: false
         desc: |
           Heartbeat log filename. Can accept the template variables {server_name} and {pid}
@@ -2068,14 +2104,30 @@
         type: str
         default: ERROR
         required: false
         desc: |
           Determines the minimum log level that will be sent as an event to Sentry.
           Possible values are DEBUG, INFO, WARNING, ERROR or CRITICAL.
 
+      sentry_traces_sample_rate:
+        type: float
+        default: 0.0
+        required: false
+        desc: |
+          Set to a number between 0 and 1. With this option set, every transaction created
+          will have that percentage chance of being sent to Sentry. A value higher than 0
+          is required to analyze performance.
+
+      sentry_ca_certs:
+        type: str
+        required: False
+        desc: |
+          Use this option to provide the path to location of the CA (Certificate Authority)
+          certificate file if the sentry server uses a self-signed certificate.
+
       statsd_host:
         type: str
         required: false
         desc: |
           Log to statsd
           Statsd is an external statistics aggregator (https://github.com/etsy/statsd)
           Enabling the following options will cause galaxy to log request timing and
@@ -2191,124 +2243,143 @@
           default, Galaxy allows users to select from a few different archive formats
           if testing shows that Galaxy is able to create files using these formats.
           Specific formats can be disabled with this option, separate more than one
           format with commas.  Available formats are currently 'zip', 'gz', and 'bz2'.
 
       tool_name_boost:
         type: float
-        default: 9.0
+        default: 20.0
         required: false
         reloadable: true
         desc: |
-          Boosts are used to customize this instance's toolbox search.
-          The higher the boost, the more importance the scoring algorithm gives to the
-          given field.  Section refers to the tool group in the tool panel.  Rest of
-          the fields are tool's attributes.
+          In tool search, a query match against a tool's name text will receive
+          this score multiplier.
+
+      tool_name_exact_multiplier:
+        type: float
+        default: 10.0
+        required: false
+        reloadable: true
+        desc: |
+          If a search query matches a tool name exactly, the score will be
+          multiplied by this factor.
 
       tool_id_boost:
         type: float
-        default: 9.0
+        default: 20.0
         required: false
         reloadable: true
         desc: |
-          Boosts are used to customize this instance's toolbox search.
-          The higher the boost, the more importance the scoring algorithm gives to the
-          given field.  Section refers to the tool group in the tool panel.  Rest of
-          the fields are tool's attributes.
+          In tool search, a query match against a tool's ID text will receive
+          this score multiplier. The query must be an exact match against ID
+          in order to be counted as a match.
 
       tool_section_boost:
         type: float
         default: 3.0
         required: false
         reloadable: true
         desc: |
-          Boosts are used to customize this instance's toolbox search.
-          The higher the boost, the more importance the scoring algorithm gives to the
-          given field.  Section refers to the tool group in the tool panel.  Rest of
-          the fields are tool's attributes.
+          In tool search, a query match against a tool's section text will
+          receive this score multiplier.
 
       tool_description_boost:
         type: float
-        default: 2.0
+        default: 8.0
         required: false
         reloadable: true
         desc: |
-          Boosts are used to customize this instance's toolbox search.
-          The higher the boost, the more importance the scoring algorithm gives to the
-          given field.  Section refers to the tool group in the tool panel.  Rest of
-          the fields are tool's attributes.
+          In tool search, a query match against a tool's description text will
+          receive this score multiplier.
 
       tool_label_boost:
         type: float
         default: 1.0
         required: false
         reloadable: true
         desc: |
-          Boosts are used to customize this instance's toolbox search.
-          The higher the boost, the more importance the scoring algorithm gives to the
-          given field.  Section refers to the tool group in the tool panel.  Rest of
-          the fields are tool's attributes.
+          In tool search, a query match against a tool's label text will
+          receive this score multiplier.
 
       tool_stub_boost:
         type: float
-        default: 5.0
+        default: 2.0
         required: false
         reloadable: true
         desc: |
-          Boosts are used to customize this instance's toolbox search.
-          The higher the boost, the more importance the scoring algorithm gives to the
-          given field.  Section refers to the tool group in the tool panel.  Rest of
-          the fields are tool's attributes.
+          A stub is parsed from the GUID as "owner/repo/tool_id".
+          In tool search, a query match against a tool's stub text will receive
+          this score multiplier.
 
       tool_help_boost:
         type: float
+        default: 1.0
+        required: false
+        reloadable: true
+        desc: |
+          In tool search, a query match against a tool's help text will receive
+          this score multiplier.
+
+      tool_help_bm25f_k1:
+        type: float
         default: 0.5
         required: false
         reloadable: true
         desc: |
-          Boosts are used to customize this instance's toolbox search.
-          The higher the boost, the more importance the scoring algorithm gives to the
-          given field.  Section refers to the tool group in the tool panel.  Rest of
-          the fields are tool's attributes.
+          The lower this parameter, the greater the diminishing reward for
+          term frequency in the help text. A higher K1 increases the level
+          of reward for additional occurences of a term. The default value will
+          provide a slight increase in score for the first, second and third
+          occurrence and little reward thereafter.
 
       tool_search_limit:
         type: int
         default: 20
         required: false
         reloadable: true
         desc: |
-          Limits the number of results in toolbox search.  Can be used to tweak how many
-          results will appear.
+          Limits the number of results in toolbox search. Use to set the
+          maximum number of tool search results to display.
 
       tool_enable_ngram_search:
         type: bool
         default: true
         required: false
         reloadable: true
         desc: |
-          Enable/ disable Ngram-search for tools. It makes tool
-          search results tolerant for spelling mistakes in the query
-          by dividing the query into multiple ngrams and search for
-          each ngram
+          Disabling this will prevent partial matches on tool names.
+          Enable/disable Ngram-search for tools. It makes tool
+          search results tolerant for spelling mistakes in the query, and will
+          also match query substrings e.g. "genome" will match "genomics" or
+          "metagenome".
 
       tool_ngram_minsize:
         type: int
         default: 3
         required: false
         reloadable: true
         desc: |
-          Set minimum size of ngrams
+          Set minimum character length of ngrams
 
       tool_ngram_maxsize:
         type: int
         default: 4
         required: false
         reloadable: true
         desc: |
-          Set maximum size of ngrams
+          Set maximum character length of ngrams
+
+      tool_ngram_factor:
+        type: float
+        default: 0.2
+        required: false
+        reloadable: true
+        desc: |
+          Ngram matched scores will be multiplied by this factor. Should always
+          be below 1, because an ngram match is a partial match of a search term.
 
       tool_test_data_directories:
         type: str
         default: 'test-data'
         required: false
         desc: |
           Set tool test data directory. The test framework sets this value to
@@ -2374,14 +2445,21 @@
       remote_user_logout_href:
         type: str
         required: false
         desc: |
           If use_remote_user is enabled, you can set this to a URL that will log your
           users out.
 
+      post_user_logout_href:
+        type: str
+        default: /root/login?is_logout_redirect=true
+        required: false
+        desc: |
+          This is the default url to which users are redirected after they log out.
+
       normalize_remote_user_email:
         type: bool
         default: false
         required: false
         desc: |
           If your proxy and/or authentication source does not normalize e-mail
           addresses or user names being passed to Galaxy - set this option
@@ -2419,14 +2497,21 @@
         type: bool
         default: false
         required: false
         desc: |
           Show the site's welcome page (see welcome_url) alongside the login page
           (even if require_login is true).
 
+      prefer_custos_login:
+        type: bool
+        default: false
+        required: False
+        desc: |
+          Controls the order of the login page to prefer Custos-based login and registration.
+
       allow_user_creation:
         type: bool
         default: true
         required: false
         desc: |
           Allow unregistered users to create new accounts (otherwise, they will have to
           be created by an admin).
@@ -2542,21 +2627,14 @@
 
           This forces expose_user_email and expose_user_name to be false, and
           forces user_deletion to be true to support the right to erasure.
 
           Please read the GDPR section under the special topics area of the
           admin documentation.
 
-      enable_beta_containers_interface:
-        type: bool
-        default: false
-        required: false
-        desc: |
-          Enable the new container interface for Interactive Environments
-
       enable_beta_workflow_modules:
         type: bool
         default: false
         required: false
         desc: |
           Enable beta workflow modules that should not yet be considered part of Galaxy's
           stable API. (The module state definitions may change and workflows built using
@@ -2708,24 +2786,77 @@
       api_allow_run_as:
         type: str
         required: false
         desc: |
           Optional list of email addresses of API users who can make calls on behalf of
           other users.
 
-      master_api_key:
+      bootstrap_admin_api_key:
         type: str
         required: false
+        deprecated_alias: master_api_key
         desc: |
           API key that allows performing some admin actions without actually
           having a real admin user in the database and config.
           Only set this if you need to bootstrap Galaxy, in particular to create
           a real admin user account via API.
           You should probably not set this on a production server.
 
+      ga4gh_service_id:
+        type: str
+        required: false
+        desc: |
+          Service ID for GA4GH services (exposed via the service-info endpoint for the Galaxy DRS API).
+          If unset, one will be generated using the URL the target API requests are made against.
+
+          For more information on GA4GH service definitions - check out
+          https://github.com/ga4gh-discovery/ga4gh-service-registry
+          and https://editor.swagger.io/?url=https://raw.githubusercontent.com/ga4gh-discovery/ga4gh-service-registry/develop/service-registry.yaml
+
+          This value should likely reflect your service's URL. For instance for usegalaxy.org
+          this value should be org.usegalaxy. Particular Galaxy implementations will treat this
+          value as a prefix and append the service type to this ID. For instance for the DRS
+          service "id" (available via the DRS API) for the above configuration value would be
+          org.usegalaxy.drs.
+
+      ga4gh_service_organization_name:
+        type: str
+        required: false
+        desc: |
+          Service name for host organization (exposed via the service-info endpoint for the Galaxy DRS API).
+          If unset, one will be generated using ga4gh_service_id.
+
+          For more information on GA4GH service definitions - check out
+          https://github.com/ga4gh-discovery/ga4gh-service-registry
+          and https://editor.swagger.io/?url=https://raw.githubusercontent.com/ga4gh-discovery/ga4gh-service-registry/develop/service-registry.yaml
+
+      ga4gh_service_organization_url:
+        type: str
+        required: False
+        desc: |
+          Organization URL for host organization (exposed via the service-info endpoint for the Galaxy DRS API).
+          If unset, one will be generated using the URL the target API requests are made against.
+
+          For more information on GA4GH service definitions - check out
+          https://github.com/ga4gh-discovery/ga4gh-service-registry
+          and https://editor.swagger.io/?url=https://raw.githubusercontent.com/ga4gh-discovery/ga4gh-service-registry/develop/service-registry.yaml
+
+      ga4gh_service_environment:
+        type: str
+        required: False
+        desc: |
+          Service environment (exposed via the service-info endpoint for the Galaxy DRS API) for
+          implemented GA4GH services.
+
+          Suggested values are prod, test, dev, staging.
+
+          For more information on GA4GH service definitions - check out
+          https://github.com/ga4gh-discovery/ga4gh-service-registry
+          and https://editor.swagger.io/?url=https://raw.githubusercontent.com/ga4gh-discovery/ga4gh-service-registry/develop/service-registry.yaml
+
       enable_tool_tags:
         type: bool
         default: false
         required: false
         desc: |
           Enable tool tags (associating tools with tags).  This has its own option
           since its implementation has a few performance implications on startup for
@@ -2756,21 +2887,25 @@
           only renders the inputs if possible (the workflow must have no disconnected
           runtime inputs and not replacement parameters within tool steps). In the
           future 'force' may be added an option for Galaskio-style servers that should
           only render simplified workflows.
 
       simplified_workflow_run_ui_target_history:
         type: str
-        default: 'current'
-        enum: ['current', 'new']
+        default: 'prefer_current'
+        enum: ['current', 'new', 'prefer_current', 'prefer_new']
         required: false
         per_host: true
         desc: |
           When the simplified workflow run form is rendered, should the invocation outputs
-          be sent to the 'current' history or a 'new' history.
+          be sent to the 'current' history or a 'new' history. If the user should be presented
+          and option between these - set this to 'prefer_current' or 'prefer_new' to display
+          a runtime setting with the corresponding default. The default is to provide the
+          user this option and default it to the current history (the traditional behavior
+          of Galaxy for years) - this corresponds to the setting 'prefer_current'.
 
       simplified_workflow_run_ui_job_cache:
         type: str
         default: 'off'
         enum: ['on', 'off']
         required: false
         per_host: true
@@ -2910,28 +3045,28 @@
         required: false
         desc: |
           Directory to store Data Manager based tool-data. Defaults to the value of the
           <tool_data_path> option.
 
       job_config_file:
         type: str
-        default: job_conf.xml
+        default: job_conf.yml
         path_resolves_to: config_dir
         required: false
         desc: |
           To increase performance of job execution and the web interface, you can
           separate Galaxy into multiple processes.  There are more than one way to do
           this, and they are explained in detail in the documentation:
 
           https://docs.galaxyproject.org/en/master/admin/scaling.html
 
           By default, Galaxy manages and executes jobs from within a single process and
           notifies itself of new jobs via in-memory queues.  Jobs are run locally on
           the system on which Galaxy is started.  Advanced job running capabilities can
-          be configured through the job configuration file.
+          be configured through the job configuration file or the <job_config> option.
 
       job_config:
         !include job_config_schema.yml
 
       dependency_resolvers:
         type: seq
         sequence:
@@ -2975,18 +3110,18 @@
 
       default_job_resubmission_condition:
         type: str
         required: false
         desc: |
           When jobs fail due to job runner problems, Galaxy can be configured to retry
           these or reroute the jobs to new destinations. Very fine control of this is
-          available with resubmit declarations in job_conf.xml. For simple deployments
+          available with resubmit declarations in the job config. For simple deployments
           of Galaxy though, the following attribute can define resubmission conditions
           for all job destinations. If any job destination defines even one
-          resubmission condition explicitly in job_conf.xml - the condition described
+          resubmission condition explicitly in the job config - the condition described
           by this option will not apply to that destination. For instance, the condition:
           'attempt < 3 and unknown_error and (time_running < 300 or time_since_queued < 300)'
           would retry up to two times jobs that didn't fail due to detected memory or
           walltime limits but did fail quickly (either while queueing or running). The
           commented out default below results in no default job resubmission condition,
           failing jobs are just failed outright.
 
@@ -3034,25 +3169,38 @@
         desc: |
           Each Galaxy job handler process runs one thread per job runner plugin responsible for
           checking the state of queued and running jobs.  This thread operates in a loop and
           sleeps for the given number of seconds at the end of each iteration. This can be
           decreased if extremely high job throughput is necessary, but doing so can increase CPU
           usage of handler processes. Float values are allowed.
 
+      workflow_monitor_sleep:
+        type: float
+        default: 1.0
+        required: false
+        desc: |
+          Each Galaxy workflow handler process runs one thread responsible for
+          checking the state of active workflow invocations.  This thread operates in a loop and
+          sleeps for the given number of seconds at the end of each iteration. This can be
+          decreased if extremely high job throughput is necessary, but doing so can increase CPU
+          usage of handler processes. Float values are allowed.
+
       metadata_strategy:
         type: str
         required: false
         default: directory
         desc: |
-          Determines how metadata will be set. Valid values are `directory` and `extended`.
+          Determines how metadata will be set. Valid values are `directory`, `extended`,
+          `directory_celery` and `extended_celery`.
           In extended mode jobs will decide if a tool run failed, the object stores
           configuration is serialized and made available to the job and is used for
           writing output datasets to the object store as part of the job and dynamic
           output discovery (e.g. discovered datasets <discover_datasets>, unpopulated collections,
-          etc) happens as part of the job.
+          etc) happens as part of the job. In `directory_celery` and `extended_celery` metadata
+          will be set within a celery task.
 
       retry_metadata_internally:
         type: bool
         default: true
         required: false
         desc: |
           Although it is fairly reliable, setting metadata can occasionally fail.  In
@@ -3330,14 +3478,25 @@
           user has dispatched to a given destination.  By default, these queries will
           happen for every job that is waiting to run, but if cache_user_job_count is
           set to true, it will only happen once per iteration of the handler queue.
           Although better for performance due to reduced queries, the trade-off is a
           greater possibility that jobs will be dispatched past the configured limits
           if running many handlers.
 
+      toolbox_auto_sort:
+        type: bool
+        default: true
+        required: false
+        reloadable: true
+        desc: |
+          If true, the toolbox will be sorted by tool id when the toolbox is loaded.
+          This is useful for ensuring that tools are always displayed in the same
+          order in the UI.  If false, the order of tools in the toolbox will be
+          preserved as they are loaded from the tool config files.
+
       tool_filters:
         type: str
         required: false
         desc: |
           Define toolbox filters (https://galaxyproject.org/user-defined-toolbox-filters/)
           that admins may use to restrict the tools to display.
 
@@ -3392,21 +3551,42 @@
         default: sqlalchemy+sqlite:///./database/control.sqlite?isolation_level=IMMEDIATE
         required: false
         desc: |
           Galaxy uses AMQP internally for communicating between processes.  For
           example, when reloading the toolbox or locking job execution, the process
           that handled that particular request will tell all others to also reload,
           lock jobs, etc.
-          For connection examples, see http://docs.celeryproject.org/projects/kombu/en/latest/userguide/connections.html
+          For connection examples, see https://docs.celeryq.dev/projects/kombu/en/stable/userguide/connections.html
 
           Without specifying anything here, galaxy will first attempt to use your
           specified database_connection above.  If that's not specified either, Galaxy
           will automatically create and use a separate sqlite database located in your
           <galaxy>/database folder (indicated in the commented out line below).
 
+      celery_conf:
+        type: any
+        required: false
+        default:
+          task_routes:
+            'galaxy.fetch_data': 'galaxy.external'
+            'galaxy.set_job_metadata': 'galaxy.external'
+        desc: |
+          Configuration options passed to Celery.
+
+          To refer to a task by name, use the template `galaxy.foo` where `foo` is the function name
+          of the task defined in the galaxy.celery.tasks module.
+
+          The `broker_url` option, if unset, defaults to the value of `amqp_internal_connection`.
+          The `result_backend` option must be set if the `enable_celery_tasks` option is set.
+
+          The galaxy.fetch_data task can be disabled by setting its route to "disabled": `galaxy.fetch_data: disabled`.
+          (Other tasks cannot be disabled on a per-task basis at this time.)
+
+          For details, see Celery documentation at https://docs.celeryq.dev/en/stable/userguide/configuration.html.
+
       enable_celery_tasks:
         type: bool
         default: false
         required: false
         desc: |
           Offload long-running tasks to a Celery task queue.
           Activate this only if you have setup a Celery worker for Galaxy.
@@ -3449,22 +3629,22 @@
         required: false
         desc: |
           Allow the display of tool recommendations in workflow editor and after tool execution.
           If it is enabled and set to true, please enable 'tool_recommendation_model_path' as well
 
       tool_recommendation_model_path:
         type: str
-        default: 'https://github.com/galaxyproject/galaxy-test-data/raw/master/tool_recommendation_model.hdf5'
+        default: 'https://github.com/galaxyproject/galaxy-test-data/raw/master/tool_recommendation_model_v_0.2.hdf5'
         required: false
         desc: |
           Set remote path of the trained model (HDF5 file) for tool recommendation.
 
       topk_recommendations:
         type: int
-        default: 10
+        default: 20
         required: false
         desc: |
           Set the number of predictions/recommendations to be made by the model
 
       admin_tool_recommendations_path:
         type: str
         required: false
@@ -3488,23 +3668,14 @@
         type: str
         default: 'error_report.yml'
         path_resolves_to: config_dir
         required: false
         desc: |
           Path to error reports configuration file.
 
-      containers_config_file:
-        type: str
-        default: 'containers_conf.yml'
-        path_resolves_to: config_dir
-        required: false
-        desc: |
-          Path to container interface configuration file. The containers interface is only used if
-          `enable_beta_containers_interface` config option is set.
-
       tool_destinations_config_file:
         type: str
         default: 'tool_destinations.yml'
         path_resolves_to: config_dir
         required: false
         desc: |
           Path to dynamic tool destinations configuration file.
@@ -3521,7 +3692,32 @@
       vault_config_file:
         type: str
         default: vault_conf.yml
         path_resolves_to: config_dir
         required: false
         desc: |
           Vault config file.
+
+      display_builtin_converters:
+        type: bool
+        default: true
+        required: false
+        desc: Display built-in converters in the tool panel.
+
+      themes_config_file:
+        type: str
+        default: themes_conf.yml
+        path_resolves_to: config_dir
+        resolves_to: themes
+        per_host: true
+        required: false
+        desc: |
+          Optional file containing one or more themes for galaxy. If several themes
+          are defined, users can choose their preferred theme in the client.
+
+      enable_beacon_integration:
+        type: bool
+        default: false
+        required: false
+        desc: |
+          Enables user preferences and api endpoint for the beacon integration.
+
```

### Comparing `galaxy-config-22.1.1/galaxy/config/schemas/job_config_schema.yml` & `galaxy-config-23.0.1/galaxy/config/schemas/job_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-22.1.1/galaxy/config/schemas/reports_config_schema.yml` & `galaxy-config-23.0.1/galaxy/config/schemas/reports_config_schema.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 type: map
 mapping:
-  uwsgi: !include uwsgi_schema.yml
   reports:
     type: map
     required: true
     desc: |
       Galaxy Reports configuration options.
     mapping:
 
@@ -39,38 +38,20 @@
       template_cache_path:
         type: str
         default: database/compiled_templates/reports
         desc: |
           Mako templates are compiled as needed and cached for reuse, this directory is
           used for the cache
 
-      debug:
-        type: bool
-        default: false
-        desc: |
-          Configuration for debugging middleware
-
-      use_lint:
-        type: bool
-        default: false
-        desc: |
-          Check for WSGI compliance.
-
       use_heartbeat:
         type: bool
         default: true
         desc: |
           Write thread status periodically to 'heartbeat.log' (careful, uses disk space rapidly!)
 
-      use_profile:
-        type: bool
-        default: true
-        desc: |
-          Profiling middleware (cProfile based)
-
       smtp_server:
         type: str
         default: yourserver@yourfacility.edu
         desc: |
           Mail
 
       error_email_to:
```

### Comparing `galaxy-config-22.1.1/galaxy/config/schemas/tool_shed_config_schema.yml` & `galaxy-config-23.0.1/galaxy/config/schemas/tool_shed_config_schema.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 type: map
 mapping:
-  uwsgi: !include uwsgi_schema.yml
   tool_shed:
     type: map
     required: true
     desc: |
       Tool Shed configuration options.
     mapping:
       log_level:
@@ -256,35 +255,14 @@
       remote_user_logout_href:
         type: str
         required: false
         desc: |
           If use_remote_user is enabled, you can set this to a URL that will log your
           users out.
 
-      debug:
-        type: bool
-        default: false
-        required: false
-        desc: |
-          Configuration for debugging middleware
-
-      use_lint:
-        type: bool
-        default: false
-        required: false
-        desc: |
-          Check for WSGI compliance.
-
-      use_printdebug:
-        type: bool
-        default: true
-        required: false
-        desc: |
-          Intercept print statements and show them on the returned page.
-
       admin_users:
         type: str
         required: false
         desc: |
           Administrative users - set this to a comma-separated list of valid Tool Shed
           users (email addresses).  These users will have access to the Admin section
           of the server, and will have access to create users, groups, roles,
@@ -368,21 +346,14 @@
         type: bool
         default: true
         required: false
         desc: |
           Write thread status periodically to 'heartbeat.log' (careful, uses disk
            space rapidly!)
 
-      use_profile:
-        type: bool
-        default: true
-        required: false
-        desc: |
-          Profiling middleware (cProfile based)
-
       enable_galaxy_flavor_docker_image:
         type: bool
         default: false
         required: false
         desc: |
           Enable creation of Galaxy flavor Docker Image
 
@@ -582,14 +553,30 @@
         type: str
         default: ERROR
         required: false
         desc: |
           Determines the minimum log level that will be sent as an event to Sentry.
           Possible values are DEBUG, INFO, WARNING, ERROR or CRITICAL.
 
+      sentry_traces_sample_rate:
+        type: float
+        default: 0.0
+        required: false
+        desc: |
+          Set to a number between 0 and 1. With this option set, every transaction created
+          will have that percentage chance of being sent to Sentry. A value higher than 0
+          is required to analyze performance.
+
+      sentry_ca_certs:
+        type: str
+        required: False
+        desc: |
+          Use this option to provide the path to location of the CA (Certificate Authority)
+          certificate file if the sentry server uses a self-signed certificate.
+
       session_duration:
         type: int
         default: 0
         required: false
         desc: |
           Galaxy Session Timeout
           This provides a timeout (in minutes) after which a user will have to log back in.
@@ -608,14 +595,24 @@
         path_resolves_to: config_dir
         required: false
         desc: |
           XML config file that allows the use of different authentication providers
           (e.g. LDAP) instead or in addition to local authentication (.sample is used
           if default does not exist).
 
+      bootstrap_admin_api_key:
+        type: str
+        required: false
+        desc: |
+          API key that allows performing some admin actions without actually
+          having a real admin user in the database and config.
+          Only set this if you need to bootstrap Galaxy, in particular to create
+          a real admin user account via API.
+          You should probably not set this on a production server.
+
       shed_tool_data_table_config:
         type: str
         default: shed_tool_data_table_conf.xml
         path_resolves_to: managed_config_dir
         required: false
         desc: |
           XML config file that contains additional data table entries for the
```

### Comparing `galaxy-config-22.1.1/galaxy/config/script.py` & `galaxy-config-23.0.1/galaxy/config/script.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,67 +13,54 @@
 
 CONFIGURE_URL = "https://docs.galaxyproject.org/en/master/admin/"
 
 DESCRIPTION = "Initialize a directory with a minimal Galaxy config."
 HELP_CONFIG_DIR = "Directory containing the configuration files for Galaxy."
 HELP_DATA_DIR = "Directory containing Galaxy-created data."
 HELP_FORCE = "Overwrite existing files if they already exist."
-HELP_WSGI_SERVER = ("Web server stack used to host Galaxy web application, and if uWSGI, which protocol to use.")
-HELP_LIBDRMAA = (
-    "Configure Galaxy to submit jobs to a cluster via DRMAA by supplying the path to a libdrmaa.so file using this "
-    "argument."
-)
-HELP_INSTALL = ("Install optional dependencies required by specified configuration (e.g. drmaa, etc...).")
+HELP_INSTALL = "Install optional dependencies required by specified configuration (e.g. drmaa, etc...)."
 HELP_HOST = (
     'Host to bind Galaxy to - defaults to localhost. Specify an IP address or "all" to listen on all interfaces.'
 )
-HELP_PORT = ("Port to bind Galaxy to.")
-HELP_DB_CONN = ("Galaxy database connection URI.")
+HELP_PORT = "Port to bind Galaxy to."
+HELP_DB_CONN = "Galaxy database connection URI."
 
 DEFAULT_HOST = "localhost"
 DEFAULT_YML = "galaxy.yml"
-DEFAULT_DB_CONN = 'sqlite:///./database/universe.sqlite?isolation_level=IMMEDIATE'
+DEFAULT_DB_CONN = "sqlite:///./database/universe.sqlite?isolation_level=IMMEDIATE"
 
-SAMPLES_PATH = os.path.abspath(os.path.join(os.path.dirname(__file__), 'sample'))
-GALAXY_CONFIG_TEMPLATE_FILE = os.path.join(SAMPLES_PATH, 'galaxy.yml.sample')
-STATIC_PATH = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir, 'web', 'framework', 'static'))
-CLIENT_PATH = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir, os.pardir, os.pardir, 'client'))
+SAMPLES_PATH = os.path.abspath(os.path.join(os.path.dirname(__file__), "sample"))
+GALAXY_CONFIG_TEMPLATE_FILE = os.path.join(SAMPLES_PATH, "galaxy.yml.sample")
+STATIC_PATH = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir, "web", "framework", "static"))
+CLIENT_PATH = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir, os.pardir, os.pardir, "client"))
 
 MSG_CONFIG_SUMMARY = """
 For help on configuring Galaxy, consult the documentation at: \n {}
 
 Additional sample configuration files for various Galaxy components (jobs,
 datatypes, etc.) can be found in:\n {}
 
 Start Galaxy by running the command from directory [{}]:
 """
 
 # The sample is used as the default config file for Galaxy started without a config, and we don't want to duplicate the
 # whole thing into galaxy.config for templating, so for now just substitute some lines. In the future we will build
 # configs differently.
 GALAXY_CONFIG_SUBSTITUTIONS = {
-    '  http: 127.0.0.1:8080': '  ${uwsgi_transport}: ${host}:${port}',
-    '  static-map: /static=static': '  static-map: /static=${static_path}',
-    '  static-map: /favicon.ico=static/favicon.ico': '  static-map: /static=${static_path}/favicon.ico',
-    '  static-safe: client/src/assets': '  ${client_path}/src/assets',
-    '  virtualenv: .venv': '  #venv: .venv   # not used when running installed',
-    '  pythonpath: lib': '  #pythonpath: lib  # not used  when running installed',
-    '  #config_dir: false': '  config_dir: ${config_dir}',
-    '  #data_dir: false': '  data_dir: ${data_dir}',
-    '  #database_connection: sqlite:///./database/universe.sqlite?isolation_level=IMMEDIATE': '  database_connection: ${database_connection}',
+    "  #config_dir: false": "  config_dir: ${config_dir}",
+    "  #data_dir: false": "  data_dir: ${data_dir}",
+    "  #database_connection: sqlite:///./database/universe.sqlite?isolation_level=IMMEDIATE": "  database_connection: ${database_connection}",
 }
 
 
 def main(argv=None):
     dependencies = []
     arg_parser = ArgumentParser(description=DESCRIPTION)
     arg_parser.add_argument("--config-dir", default=".", help=HELP_CONFIG_DIR)
     arg_parser.add_argument("--data-dir", default="./data", help=HELP_DATA_DIR)
-    arg_parser.add_argument("--wsgi-server", choices=["uwsgi-http", "uwsgi-native"], default="uwsgi-http",
-                            help=HELP_WSGI_SERVER)
     arg_parser.add_argument("--host", default=DEFAULT_HOST, help=HELP_HOST)
     arg_parser.add_argument("--port", default="8080", help=HELP_PORT)
     arg_parser.add_argument("--db-conn", default=DEFAULT_DB_CONN, help=HELP_DB_CONN)
     arg_parser.add_argument("--install", action="store_true", help=HELP_INSTALL)
     arg_parser.add_argument("--force", action="store_true", default=False, help=HELP_FORCE)
     args = arg_parser.parse_args(argv)
     config_dir = args.config_dir
@@ -95,80 +82,64 @@
     _handle_install(args, dependencies)
     _print_config_summary(args, mode, relative_config_dir)
 
 
 def _print_config_summary(args, mode, relative_config_dir):
     _print_galaxy_yml_info(args, mode)
     print(MSG_CONFIG_SUMMARY.format(CONFIGURE_URL, SAMPLES_PATH, relative_config_dir))
-    _print_galaxy_run(mode)
 
 
 def _print_galaxy_yml_info(args, mode):
     print(" - galaxy.yml created, update to configure Galaxy.")
     print(f"   * Target web server {mode}")
     if args.host == DEFAULT_HOST:
         print("   * Binding to host localhost, remote clients will not be able to connect.")
     elif _determine_host(args) == "0.0.0.0":
         print("   * Binding to all network interfaces.")
     else:
         print("   * Binding to host [%s].", args.host)
 
 
-def _print_galaxy_run(mode):
-    if mode.startswith("uwsgi"):
-        print("    uwsgi --yaml galaxy.yml")
-    else:
-        raise Exception(f"Unknown mode: {mode}")
-
-
 def _determine_mode(args):
-    if args.wsgi_server:
-        mode = args.wsgi_server
-    else:
-        mode = "paster"
-    return mode
+    return "gunicorn"
 
 
 def _determine_host(args):
-    return '0.0.0.0' if args.host == 'all' else args.host
+    return "0.0.0.0" if args.host == "all" else args.host
 
 
 def _determine_yml_file(config_dir):
     return os.path.join(config_dir, DEFAULT_YML)
 
 
 def _handle_galaxy_yml(args, config_dir, data_dir):
     force = args.force
     yml_file = _determine_yml_file(config_dir)
     _check_file(yml_file, force)
-    uwsgi_transport = 'socket' if args.wsgi_server == 'uwsgi-native' else 'http'
     config_dict = dict(
         port=args.port,
         host=_determine_host(args),
-        uwsgi_transport=uwsgi_transport,
         config_dir=config_dir,
         data_dir=data_dir,
         client_dir=CLIENT_PATH,
         static_path=STATIC_PATH,
         database_connection=args.db_conn,
     )
 
     galaxy_config_template = []
     with open(GALAXY_CONFIG_TEMPLATE_FILE) as fh:
         for line in fh:
-            line = line.rstrip('\n')
+            line = line.rstrip("\n")
             for k, v in GALAXY_CONFIG_SUBSTITUTIONS.items():
                 if line == k:
                     line = v
             galaxy_config_template.append(line)
-    galaxy_config_template = string.Template('\n'.join(galaxy_config_template))
+    galaxy_config_template = string.Template("\n".join(galaxy_config_template))
 
-    galaxy_config = galaxy_config_template.safe_substitute(
-        **config_dict
-    )
+    galaxy_config = galaxy_config_template.safe_substitute(**config_dict)
     open(yml_file, "w").write(galaxy_config)
 
 
 def _handle_install(args, dependencies):
     if args.install and dependencies:
         if pip is None:
             raise ImportError("Bootstrapping Galaxy dependencies requires pip.")
@@ -178,9 +149,9 @@
 
 def _check_file(path, force):
     if os.path.exists(path) and not force:
         print(f"File {path} exists, exiting. Run with --force to replace configuration.", file=sys.stderr)
         sys.exit(1)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `galaxy-config-22.1.1/galaxy_config.egg-info/PKG-INFO` & `galaxy-config-23.0.1/galaxy_config.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,69 @@
 Metadata-Version: 2.1
 Name: galaxy-config
-Version: 22.1.1
-Summary: Galaxy Configuration
+Version: 23.0.1
+Summary: Galaxy configuration
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
-Keywords: galaxy
-Platform: UNKNOWN
+Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Testing
 Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: https://badge.fury.io/py/galaxy-config.svg
    :target: https://pypi.org/project/galaxy-config/
 
 
 Overview
 --------
 
 The Galaxy_ config module.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
-
-
-
 History
 -------
 
 .. to_doc
 
----------------------
-22.1.0.dev0
----------------------
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
-* Initial release
 
+=========
+Bug fixes
+=========
+
+* Change default watchdog inotify_buffer log level to info by `@mvdbeek <https://github.com/mvdbeek>`_ in `#15967 <https://github.com/galaxyproject/galaxy/pull/15967>`_
 
+============
+Enhancements
+============
+
+* Add ``ca_certs`` option for sentry client by `@mvdbeek <https://github.com/mvdbeek>`_ in `#15943 <https://github.com/galaxyproject/galaxy/pull/15943>`_
+
+-------------------
+22.1.1 (2022-08-22)
+-------------------
+
+* Initial release
```

