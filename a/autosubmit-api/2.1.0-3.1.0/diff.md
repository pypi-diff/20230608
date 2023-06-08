# Comparing `tmp/autosubmit_api-2.1.0.tar.gz` & `tmp/autosubmit_api-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autosubmit_api-2.1.0.tar", last modified: Tue Jan 24 11:56:40 2023, max compression
+gzip compressed data, was "dist/autosubmit_api-3.1.0.tar", last modified: Thu Jun  8 14:31:16 2023, max compression
```

## Comparing `autosubmit_api-2.1.0.tar` & `autosubmit_api-3.1.0.tar`

### file list

```diff
@@ -1,197 +1,200 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      588 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2261 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/
--rw-r--r--   0 root         (0) root         (0)       99 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18635 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/__init__.py
--rw-r--r--   0 root         (0) root         (0)   164377 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/autosubmit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47503 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job.py
--rw-r--r--   0 root         (0) root         (0)     6512 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_common.py
--rw-r--r--   0 root         (0) root         (0)    15976 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_dict.py
--rw-rw-rw-   0 root         (0) root         (0)      989 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_exceptions.py
--rw-r--r--   0 root         (0) root         (0)    24369 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_grouping.py
--rw-r--r--   0 root         (0) root         (0)   159742 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_list.py
--rw-r--r--   0 root         (0) root         (0)     5147 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_list_persistence.py
--rw-r--r--   0 root         (0) root         (0)     3366 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_package_persistence.py
--rw-r--r--   0 root         (0) root         (0)    21782 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_packager.py
--rw-r--r--   0 root         (0) root         (0)    21025 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_packages.py
--rw-r--r--   0 root         (0) root         (0)    16035 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33229 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/ecmwf_adaptor.py
--rw-r--r--   0 root         (0) root         (0)     7914 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/ecplatform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5436 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_cca_header.py
--rw-rw-rw-   0 root         (0) root         (0)     4014 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_header.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/local_header.py
--rw-rw-rw-   0 root         (0) root         (0)     7289 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/lsf_header.py
--rw-rw-rw-   0 root         (0) root         (0)     2950 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs10_header.py
--rw-rw-rw-   0 root         (0) root         (0)     3377 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs11_header.py
--rw-rw-rw-   0 root         (0) root         (0)     2941 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs12_header.py
--rw-rw-rw-   0 root         (0) root         (0)     2192 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ps_header.py
--rw-rw-rw-   0 root         (0) root         (0)     3517 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/sge_header.py
--rw-rw-rw-   0 root         (0) root         (0)     6049 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/slurm_header.py
--rw-r--r--   0 root         (0) root         (0)     5778 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/locplatform.py
--rw-r--r--   0 root         (0) root         (0)     4060 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/lsfplatform.py
--rw-r--r--   0 root         (0) root         (0)    37704 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/mn_adaptor.py
--rw-r--r--   0 root         (0) root         (0)    24711 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_platform.py
--rw-r--r--   0 root         (0) root         (0)     7855 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_submitter.py
--rw-r--r--   0 root         (0) root         (0)     3739 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/pbsplatform.py
--rw-r--r--   0 root         (0) root         (0)    10116 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/platform.py
--rw-r--r--   0 root         (0) root         (0)     2626 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/psplatform.py
--rw-r--r--   0 root         (0) root         (0)    13130 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/saga_platform.py
--rw-r--r--   0 root         (0) root         (0)     9152 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/saga_submitter.py
--rw-r--r--   0 root         (0) root         (0)     3184 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/sgeplatform.py
--rw-r--r--   0 root         (0) root         (0)     6945 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/slurmplatform.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/submitter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15542 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_builder.py
--rw-r--r--   0 root         (0) root         (0)     4971 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/builders/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/builders/__init__.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/builders/basic_builder.py
--rw-r--r--   0 root         (0) root         (0)     2627 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/builders/configuration_facade_builder.py
--rw-r--r--   0 root         (0) root         (0)     3133 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/builders/experiment_history_builder.py
--rw-r--r--   0 root         (0) root         (0)     2620 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/builders/joblist_helper_builder.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/builders/joblist_loader_builder.py
--rw-r--r--   0 root         (0) root         (0)     2188 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/builders/pkl_organizer_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7487 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/common/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/common/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/components/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/components/experiment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/components/experiment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9130 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/components/experiment/configuration_facade.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/components/experiment/pkl_organizer.py
--rw-r--r--   0 root         (0) root         (0)     4012 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/components/experiment/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/components/jobs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/components/jobs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12506 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/components/jobs/job_factory.py
--rw-r--r--   0 root         (0) root         (0)     3121 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/components/jobs/job_support.py
--rw-r--r--   0 root         (0) root         (0)     3441 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/components/jobs/joblist_helper.py
--rw-r--r--   0 root         (0) root         (0)     8744 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/components/jobs/joblist_loader.py
--rw-r--r--   0 root         (0) root         (0)      637 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/components/jobs/test.py
--rw-r--r--   0 root         (0) root         (0)     5243 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/components/jobs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/components/representations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/components/representations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/components/representations/graph/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/components/representations/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1321 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/components/representations/graph/edge.py
--rw-r--r--   0 root         (0) root         (0)    17156 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/components/representations/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)     6891 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/components/representations/graph/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/components/representations/tree/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/components/representations/tree/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2669 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/components/representations/tree/test.py
--rw-r--r--   0 root         (0) root         (0)    13632 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/components/representations/tree/tree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8192 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/config/basicConfig.py
--rw-r--r--   0 root         (0) root         (0)    49904 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/config/config_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/database/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/database/__init__.py
--rw-r--r--   0 root         (0) root         (0)   164539 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/database/autosubmit.py
--rw-r--r--   0 root         (0) root         (0)    24962 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/database/db_common.py
--rw-r--r--   0 root         (0) root         (0)    93216 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/database/db_jobdata.py
--rw-r--r--   0 root         (0) root         (0)     8229 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/database/db_manager.py
--rw-r--r--   0 root         (0) root         (0)     5331 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/database/db_structure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/experiment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/experiment/__init__.py
--rw-r--r--   0 root         (0) root         (0)      590 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/experiment/as_times_db_manager.py
--rw-r--r--   0 root         (0) root         (0)    37090 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/experiment/common_db_requests.py
--rw-r--r--   0 root         (0) root         (0)    69550 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/experiment/common_requests.py
--rw-r--r--   0 root         (0) root         (0)     5784 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/experiment/experiment_common.py
--rw-r--r--   0 root         (0) root         (0)     1904 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/experiment/experiment_db_manager.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/experiment/test.py
--rw-r--r--   0 root         (0) root         (0)      647 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/experiment/utils.py
--rw-r--r--   0 root         (0) root         (0)  2569500 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/get-pip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/git/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/git/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8606 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/git/autosubmit_git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/history/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/history/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/history/data_classes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/history/data_classes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5902 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/data_classes/experiment_run.py
--rw-r--r--   0 root         (0) root         (0)    11544 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/data_classes/job_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/history/database_managers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/history/database_managers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5781 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/database_managers/database_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     5197 2022-04-13 10:23:20.000000 autosubmit_api-2.1.0/autosubmit_api/history/database_managers/database_models.py
--rw-r--r--   0 root         (0) root         (0)    23160 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/database_managers/experiment_history_db_manager.py
--rw-r--r--   0 root         (0) root         (0)     6721 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/database_managers/experiment_status_db_manager.py
--rw-r--r--   0 root         (0) root         (0)    13582 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/database_managers/test.py
--rw-r--r--   0 root         (0) root         (0)    22104 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/experiment_history.py
--rw-r--r--   0 root         (0) root         (0)     3545 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/experiment_status.py
--rw-r--r--   0 root         (0) root         (0)     3973 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/experiment_status_manager.py
--rw-r--r--   0 root         (0) root         (0)     2035 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/internal_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/history/platform_monitor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/history/platform_monitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/platform_monitor/platform_monitor.py
--rw-rw-rw-   0 root         (0) root         (0)     2315 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/history/platform_monitor/platform_utils.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/platform_monitor/slurm_monitor.py
--rw-r--r--   0 root         (0) root         (0)     3429 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/platform_monitor/slurm_monitor_item.py
--rw-r--r--   0 root         (0) root         (0)     4427 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/platform_monitor/test.py
--rw-r--r--   0 root         (0) root         (0)    10701 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/strategies.py
--rw-r--r--   0 root         (0) root         (0)    24841 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/test.py
--rw-r--r--   0 root         (0) root         (0)     3470 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/test_job_history.py
--rw-r--r--   0 root         (0) root         (0)     6630 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/test_strategies.py
--rw-r--r--   0 root         (0) root         (0)     1116 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/history/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3090 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/history/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/monitor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/monitor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6293 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/monitor/diagram.py
--rw-r--r--   0 root         (0) root         (0)    20102 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/monitor/monitor.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/monitor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/notifications/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2435 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/notifications/mail_notifier.py
--rw-rw-rw-   0 root         (0) root         (0)     1001 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/notifications/notifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/performance/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/performance/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7642 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/performance/performance_metrics.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/performance/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/statistics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/statistics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/statistics/job_stat.py
--rw-r--r--   0 root         (0) root         (0)     6950 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/statistics/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)     2565 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/statistics/stats_summary.py
--rw-r--r--   0 root         (0) root         (0)     3390 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/statistics/test.py
--rw-r--r--   0 root         (0) root         (0)     1318 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/statistics/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/workers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/workers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/workers/business/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/workers/business/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14039 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/workers/business/populate_times.py
--rw-r--r--   0 root         (0) root         (0)     2271 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/workers/business/process_graph_drawings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/workers/deprecated/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/workers/deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6359 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/workers/deprecated/fix_historic.py
--rw-r--r--   0 root         (0) root         (0)     6782 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/workers/deprecated/fix_historic_energy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api/workers/populate_details/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-2.1.0/autosubmit_api/workers/populate_details/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4077 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/workers/populate_details/populate.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/workers/populate_details/test.py
--rw-r--r--   0 root         (0) root         (0)      212 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/workers/populate_details_db.py
--rw-r--r--   0 root         (0) root         (0)      249 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/workers/populate_graph.py
--rw-r--r--   0 root         (0) root         (0)      220 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/workers/populate_queue_run_times.py
--rw-r--r--   0 root         (0) root         (0)      307 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/workers/populate_running_experiments.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/workers/test.py
--rw-r--r--   0 root         (0) root         (0)      158 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/workers/test_esarchive.py
--rw-r--r--   0 root         (0) root         (0)      184 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/autosubmit_api/workers/verify_complete.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      588 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7802 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      182 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/autosubmit_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-24 11:56:40.000000 autosubmit_api-2.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1335 2023-01-24 10:12:43.000000 autosubmit_api-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:16.000000 autosubmit_api-3.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-08 14:31:16.000000 autosubmit_api-3.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2261 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18635 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   164377 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/autosubmit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47503 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job.py
+-rw-r--r--   0 root         (0) root         (0)     6512 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_common.py
+-rw-r--r--   0 root         (0) root         (0)    16066 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_dict.py
+-rw-rw-rw-   0 root         (0) root         (0)      989 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    24369 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_grouping.py
+-rw-r--r--   0 root         (0) root         (0)   159761 2023-06-08 14:08:18.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_list.py
+-rw-r--r--   0 root         (0) root         (0)     5147 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_list_persistence.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_package_persistence.py
+-rw-r--r--   0 root         (0) root         (0)    21782 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_packager.py
+-rw-r--r--   0 root         (0) root         (0)    21025 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_packages.py
+-rw-r--r--   0 root         (0) root         (0)    16035 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33229 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/ecmwf_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)     7914 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/ecplatform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5436 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_cca_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     4014 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/local_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     7289 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/lsf_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     2950 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs10_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     3377 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs11_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     2941 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs12_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ps_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     3517 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/sge_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     6049 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/slurm_header.py
+-rw-r--r--   0 root         (0) root         (0)     5778 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/locplatform.py
+-rw-r--r--   0 root         (0) root         (0)     4060 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/lsfplatform.py
+-rw-r--r--   0 root         (0) root         (0)    37704 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/mn_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)    24711 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_platform.py
+-rw-r--r--   0 root         (0) root         (0)     7855 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     3739 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/pbsplatform.py
+-rw-r--r--   0 root         (0) root         (0)    10116 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/platform.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/psplatform.py
+-rw-r--r--   0 root         (0) root         (0)    13130 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/saga_platform.py
+-rw-r--r--   0 root         (0) root         (0)     9152 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/saga_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     3184 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/sgeplatform.py
+-rw-r--r--   0 root         (0) root         (0)     6945 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/slurmplatform.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/submitter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15542 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_builder.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/builders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/builders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/builders/basic_builder.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/builders/configuration_facade_builder.py
+-rw-r--r--   0 root         (0) root         (0)     3133 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/builders/experiment_history_builder.py
+-rw-r--r--   0 root         (0) root         (0)     2620 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/builders/joblist_helper_builder.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/builders/joblist_loader_builder.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/builders/pkl_organizer_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7517 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/common/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/components/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/components/experiment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/components/experiment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/components/experiment/configuration_facade.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/experiment/pkl_organizer.py
+-rw-r--r--   0 root         (0) root         (0)     4012 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/experiment/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12506 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/job_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/job_support.py
+-rw-r--r--   0 root         (0) root         (0)     3441 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/joblist_helper.py
+-rw-r--r--   0 root         (0) root         (0)     8889 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/joblist_loader.py
+-rw-r--r--   0 root         (0) root         (0)      637 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/test.py
+-rw-r--r--   0 root         (0) root         (0)     5243 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1321 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/edge.py
+-rw-r--r--   0 root         (0) root         (0)    17156 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)     6891 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/tree/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/tree/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2669 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/tree/test.py
+-rw-r--r--   0 root         (0) root         (0)    13728 2023-06-08 14:08:18.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/tree/tree.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/config/
+-rw-r--r--   0 root         (0) root         (0)    19435 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/config/IConfigStrategy.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8268 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/config/basicConfig.py
+-rw-r--r--   0 root         (0) root         (0)    49155 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/config/confConfigStrategy.py
+-rw-r--r--   0 root         (0) root         (0)    24603 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/config/config_common.py
+-rw-r--r--   0 root         (0) root         (0)    13398 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/config/ymlConfigStrategy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/database/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/database/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   164539 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/database/autosubmit.py
+-rw-r--r--   0 root         (0) root         (0)    24836 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/database/db_common.py
+-rw-r--r--   0 root         (0) root         (0)    93216 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/database/db_jobdata.py
+-rw-r--r--   0 root         (0) root         (0)     8229 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/database/db_manager.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/database/db_structure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      590 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/as_times_db_manager.py
+-rw-r--r--   0 root         (0) root         (0)    37090 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/common_db_requests.py
+-rw-r--r--   0 root         (0) root         (0)    69844 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/common_requests.py
+-rw-r--r--   0 root         (0) root         (0)     5784 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/experiment_common.py
+-rw-r--r--   0 root         (0) root         (0)     1904 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/experiment_db_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/test.py
+-rw-r--r--   0 root         (0) root         (0)      647 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/utils.py
+-rw-r--r--   0 root         (0) root         (0)  2569500 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/get-pip.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/git/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/git/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8606 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/git/autosubmit_git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/history/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/history/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/history/data_classes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/history/data_classes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7514 2023-06-08 14:08:18.000000 autosubmit_api-3.1.0/autosubmit_api/history/data_classes/experiment_run.py
+-rw-r--r--   0 root         (0) root         (0)    11544 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/data_classes/job_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/history/database_managers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/history/database_managers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5781 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/database_managers/database_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5197 2022-04-13 10:23:20.000000 autosubmit_api-3.1.0/autosubmit_api/history/database_managers/database_models.py
+-rw-r--r--   0 root         (0) root         (0)    23160 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/database_managers/experiment_history_db_manager.py
+-rw-r--r--   0 root         (0) root         (0)     6721 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/database_managers/experiment_status_db_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13582 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/database_managers/test.py
+-rw-r--r--   0 root         (0) root         (0)    22104 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/experiment_history.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/experiment_status.py
+-rw-r--r--   0 root         (0) root         (0)     3973 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/experiment_status_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/internal_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/platform_monitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2315 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/platform_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/slurm_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/slurm_monitor_item.py
+-rw-r--r--   0 root         (0) root         (0)     4427 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/test.py
+-rw-r--r--   0 root         (0) root         (0)    10701 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/strategies.py
+-rw-r--r--   0 root         (0) root         (0)    24841 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/test.py
+-rw-r--r--   0 root         (0) root         (0)     3470 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/test_job_history.py
+-rw-r--r--   0 root         (0) root         (0)     6630 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/test_strategies.py
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3090 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/history/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/monitor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/monitor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6293 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/monitor/diagram.py
+-rw-r--r--   0 root         (0) root         (0)    20102 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/monitor/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/monitor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/notifications/mail_notifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/notifications/notifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/performance/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/performance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7642 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/performance/performance_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/performance/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/statistics/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/statistics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/statistics/job_stat.py
+-rw-r--r--   0 root         (0) root         (0)     6950 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/statistics/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2565 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/statistics/stats_summary.py
+-rw-r--r--   0 root         (0) root         (0)     3390 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/statistics/test.py
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/statistics/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:16.000000 autosubmit_api-3.1.0/autosubmit_api/workers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/workers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:16.000000 autosubmit_api-3.1.0/autosubmit_api/workers/business/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/workers/business/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14039 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/business/populate_times.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/business/process_graph_drawings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:16.000000 autosubmit_api-3.1.0/autosubmit_api/workers/deprecated/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/workers/deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/deprecated/fix_historic.py
+-rw-r--r--   0 root         (0) root         (0)     6782 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/deprecated/fix_historic_energy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:16.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_details/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_details/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4077 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_details/populate.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_details/test.py
+-rw-r--r--   0 root         (0) root         (0)      212 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_details_db.py
+-rw-r--r--   0 root         (0) root         (0)      249 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_graph.py
+-rw-r--r--   0 root         (0) root         (0)      220 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_queue_run_times.py
+-rw-r--r--   0 root         (0) root         (0)      307 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_running_experiments.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/test.py
+-rw-r--r--   0 root         (0) root         (0)      158 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/test_esarchive.py
+-rw-r--r--   0 root         (0) root         (0)      184 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/verify_complete.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7930 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 14:31:16.000000 autosubmit_api-3.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/setup.py
```

### Comparing `autosubmit_api-2.1.0/LICENSE` & `autosubmit_api-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/PKG-INFO` & `autosubmit_api-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit_api
-Version: 2.1.0
+Version: 3.1.0
 Summary: An extension to the Autosubmit package that serves its information as an API
 Home-page: https://earth.bsc.es/gitlab/wuruchi/autosubmit_api
 Author: Wilmer Uruchi
 Author-email: wilmer.uruchi@bsc.es
 License: GNU GPL
 Keywords: autosubmit,API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `autosubmit_api-2.1.0/README.md` & `autosubmit_api-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/app.py` & `autosubmit_api-3.1.0/autosubmit_api/app.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/autosubmit.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/autosubmit.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_common.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_dict.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,11 +367,14 @@
         :param section: section name
         :type section: str
         :param option: option to return
         :type option: str
         :param default: value to return if not defined in configuration file
         :type default: object
         """
+        #todo: here should be implemented some of the changes for supporting yaml files
+
+
         if self._parser.has_option(section, option):
             return self._parser.get(section, option)
         else:
             return default
```

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_exceptions.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_exceptions.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_grouping.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_grouping.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_list.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -885,15 +885,15 @@
     def sort_by_id(self):
         """
         Returns a list of jobs sorted by id
 
         :return: jobs sorted by ID
         :rtype: list
         """
-        return sorted(self._job_list, key=lambda k: k.id)
+        return sorted(self._job_list, key=lambda k: int(k.id))
 
     def sort_by_type(self):
         """
         Returns a list of jobs sorted by type
 
         :return: job sorted by type
         :rtype: list
@@ -2486,15 +2486,15 @@
                 mainCoordinates = ExperimentGraphDrawing(
                     self.expid).calculate_drawing(allJobs, independent=True, num_chunks=len(chunk_list))
                 if not mainCoordinates:
                     mainCoordinates = dict()
                     graph = monitor.create_tree_list(
                         self.expid, allJobs, None, dict(), False)
                     result = graph.create('dot', format="plain")
-                    for u in result.split("\n"):
+                    for u in result.decode().split("\n"):
                         splitList = u.split(" ")
                         if len(splitList) > 1 and splitList[0] == "node":
                             mainCoordinates[splitList[1]] = (
                                 float(splitList[2]) * 90, float(splitList[3]) * -90)
 
             # print("Seconds spent in GraphViz: " + str(time() - start_time))
         elif (layout == 'standard' or layout == 'hierarchical'):
@@ -2642,15 +2642,15 @@
                           'children_list': [job_search.name for job_search in job._children],
                           'parents': len(job._parents),
                           'parent_list': [job_search.name for job_search in job._parents],
                           'custom_directives': job.custom_directives,
                           'status_color': Monitor.color_status(job.status),
                           'err': err,
                           'out': out,
-                          'rm_id': job.id if job.id and job.id > 0 else None,
+                          'rm_id': job.id if job.id and int(job.id) > 0 else None,
                           'minutes_queue': job_info.queue_time if job_info else 0,
                           'minutes': job_info.run_time if job_info else 0,
                           'submit': timestamp_to_datetime_format(job_info.submit) if job_info else None,
                           'start': timestamp_to_datetime_format(job_info.start) if job_info else None,
                           'finish': timestamp_to_datetime_format(job_info.finish) if job_info else None,
                           'x': x,
                           'y': y})
```

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_list_persistence.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_list_persistence.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_package_persistence.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_package_persistence.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_packager.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_packager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_packages.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_packages.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/job/job_utils.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/ecmwf_adaptor.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/ecmwf_adaptor.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/ecplatform.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/ecplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_cca_header.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_cca_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_header.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/local_header.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/local_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/lsf_header.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/lsf_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs10_header.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs10_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs11_header.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs11_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs12_header.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs12_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ps_header.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ps_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/sge_header.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/sge_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/slurm_header.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/slurm_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/locplatform.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/locplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/lsfplatform.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/lsfplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/mn_adaptor.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/mn_adaptor.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_platform.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_submitter.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_submitter.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/pbsplatform.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/pbsplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/platform.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/psplatform.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/psplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/saga_platform.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/saga_platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/saga_submitter.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/saga_submitter.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/sgeplatform.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/sgeplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/slurmplatform.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/slurmplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/submitter.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/submitter.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_builder.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_factory.py` & `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/builders/basic_builder.py` & `autosubmit_api-3.1.0/autosubmit_api/builders/basic_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/builders/configuration_facade_builder.py` & `autosubmit_api-3.1.0/autosubmit_api/builders/configuration_facade_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/builders/experiment_history_builder.py` & `autosubmit_api-3.1.0/autosubmit_api/builders/experiment_history_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/builders/joblist_helper_builder.py` & `autosubmit_api-3.1.0/autosubmit_api/builders/joblist_helper_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/builders/joblist_loader_builder.py` & `autosubmit_api-3.1.0/autosubmit_api/builders/joblist_loader_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/builders/pkl_organizer_builder.py` & `autosubmit_api-3.1.0/autosubmit_api/builders/pkl_organizer_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/common/utils.py` & `autosubmit_api-3.1.0/autosubmit_api/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,21 +197,22 @@
     SUBMITTED = 2
     QUEUING = 3
     RUNNING = 4
     COMPLETED = 5
     HELD = 6
     PREPARED = 7
     SKIPPED = 8
+    DELAYED = 9
     FAILED = -1
     UNKNOWN = -2
     SUSPENDED = -3
     #######
     # Note: any change on constants must be applied on the dict below!!!
     VALUE_TO_KEY = {-3: 'SUSPENDED', -2: 'UNKNOWN', -1: 'FAILED', 0: 'WAITING', 1: 'READY',
-                    2: 'SUBMITTED', 3: 'QUEUING', 4: 'RUNNING', 5: 'COMPLETED', 6: 'HELD', 7: 'PREPARED', 8: 'SKIPPED'}
+                    2: 'SUBMITTED', 3: 'QUEUING', 4: 'RUNNING', 5: 'COMPLETED', 6: 'HELD', 7: 'PREPARED', 8: 'SKIPPED', 9: 'DELAYED'}
     STRING_TO_CODE = {v: k for k, v in list(VALUE_TO_KEY.items())}
 
     def retval(self, value):
         return getattr(self, value)
 
 
 class bcolors:
```

### Comparing `autosubmit_api-2.1.0/autosubmit_api/common/utils_for_testing.py` & `autosubmit_api-3.1.0/autosubmit_api/common/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/components/experiment/configuration_facade.py` & `autosubmit_api-3.1.0/autosubmit_api/components/experiment/configuration_facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
   def get_wrapper_qos(self):
     # type: () -> str
     return str(self.autosubmit_conf.get_wrapper_queue())
 
   def get_wrapper_type(self):
     # type: () -> str | None
-    if self.autosubmit_conf.get_wrapper_type().upper() != "NONE":
+    if self.autosubmit_conf.get_wrapper_type() and self.autosubmit_conf.get_wrapper_type().upper() != "NONE":
       return self.autosubmit_conf.get_wrapper_type().upper()
     return None
 
   def get_section_wallclock(self, section_name):
     return str(self.autosubmit_conf.get_wallclock(section_name))
 
   def get_platform_max_wallclock(self, platform_name):
```

### Comparing `autosubmit_api-2.1.0/autosubmit_api/components/experiment/pkl_organizer.py` & `autosubmit_api-3.1.0/autosubmit_api/components/experiment/pkl_organizer.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/components/experiment/test.py` & `autosubmit_api-3.1.0/autosubmit_api/components/experiment/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/components/jobs/job_factory.py` & `autosubmit_api-3.1.0/autosubmit_api/components/jobs/job_factory.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/components/jobs/job_support.py` & `autosubmit_api-3.1.0/autosubmit_api/components/jobs/job_support.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/components/jobs/joblist_helper.py` & `autosubmit_api-3.1.0/autosubmit_api/components/jobs/joblist_helper.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/components/jobs/joblist_loader.py` & `autosubmit_api-3.1.0/autosubmit_api/components/jobs/joblist_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 from ...autosubmit_legacy.job.job_common import Status
 from bscearth.utils.date import date2str, parse_date
 from typing import Dict, List, Set, Tuple
 # Builder Imports
 from ...config.config_common import AutosubmitConfig
 from ...config.basicConfig import BasicConfig
 import json
+import logging
+
+
+logger = logging.getLogger('gunicorn.error')
 
 class JobListLoader(object):
   """ Class that manages loading the list of jobs from the pkl. Adds other resources. """
   def __init__(self, expid, joblist_helper):
     # type: (str, JobListHelper) -> None
     self.expid = expid
     self.joblist_helper = joblist_helper
@@ -183,22 +187,24 @@
     # type: (Job) -> None
     job_qos = ""
     if job.package is not None:
       job_qos = self.configuration_facade.get_wrapper_qos()
     else:
       job_qos = self.configuration_facade.get_section_qos(job.section)
     if len(job_qos.strip()) == 0:
-      job_qos = self.configuration_facade.get_platform_qos(job.platform, job.ncpus)
+        if job.platform != "None":
+             job_qos = self.configuration_facade.get_platform_qos(job.platform, job.ncpus)
     return job_qos
 
   def _determine_wallclock(self, job):
     # type: (Job) -> None
     wallclock = self.configuration_facade.get_section_wallclock(job.section)
     if len(wallclock.strip()) == 0:
-      wallclock = self.configuration_facade.get_platform_max_wallclock(job.platform)
+        if job.platform != "None":
+            wallclock = self.configuration_facade.get_platform_max_wallclock(job.platform)
     return wallclock
 
   def assign_packages_to_jobs(self):
     # type: () -> None
     if self.joblist_helper.job_to_package:
       for job in self._jobs:
         job.package = self.joblist_helper.job_to_package.get(job.name, None)
```

### Comparing `autosubmit_api-2.1.0/autosubmit_api/components/jobs/test.py` & `autosubmit_api-3.1.0/autosubmit_api/components/jobs/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/components/jobs/utils.py` & `autosubmit_api-3.1.0/autosubmit_api/components/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/components/representations/graph/edge.py` & `autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/edge.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/components/representations/graph/graph.py` & `autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/graph.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/components/representations/graph/test.py` & `autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/components/representations/tree/test.py` & `autosubmit_api-3.1.0/autosubmit_api/components/representations/tree/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/components/representations/tree/tree.py` & `autosubmit_api-3.1.0/autosubmit_api/components/representations/tree/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from ...jobs import utils as JUtils
 from ....performance import utils as PUtils
 from ...jobs.joblist_loader import JobListLoader
 from ...jobs.job_factory import Job
 from ....common.utils import Status, get_average_total_time, get_current_timestamp
 from collections import deque, OrderedDict
 from typing import List, Dict, Tuple, Set, Any
+from operator import is_not
+from functools import partial
 
 DEFAULT_MEMBER = "DEFAULT"
 
 class TreeRepresentation(object):
   def __init__(self, expid, job_list_loader):
     # type: (str, JobListLoader) -> None
     self.expid = expid # type: str
@@ -190,15 +192,15 @@
 
   def _generate_package_tree_folders(self):
     """ Package folders (wrappers) as roots in the tree. """
     # sort the list before iterating
     result_exp_wrappers = []
     sorted_wrappers = sorted(self.joblist_loader.package_names)
     for package_name in sorted_wrappers:
-      jobs_in_package = sorted(self.joblist_loader.get_all_jobs_in_package(package_name), key=lambda x: x.chunk if x.chunk is not None else 0)
+      jobs_in_package = sorted( list(filter(partial(is_not, None), self.joblist_loader.get_all_jobs_in_package(package_name))), key=lambda x: x.chunk if x.chunk is not None else 0)
       simple_title = "Wrapper: {0}".format(package_name)
       total_count = len(jobs_in_package)
       status_counters = {
           Status.COMPLETED: 0,
           Status.RUNNING: 0,
           Status.QUEUING: 0,
           Status.FAILED: 0,
```

### Comparing `autosubmit_api-2.1.0/autosubmit_api/config/basicConfig.py` & `autosubmit_api-3.1.0/autosubmit_api/config/basicConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
 try:
     # noinspection PyCompatibility
     from configparser import SafeConfigParser
+    from autosubmitconfigparser.config.configcommon import AutosubmitConfig
 except ImportError:
     # noinspection PyCompatibility
     from configparser import SafeConfigParser
 import os
 import re
 # from log.log import Log, AutosubmitError, AutosubmitCritical
```

### Comparing `autosubmit_api-2.1.0/autosubmit_api/config/config_common.py` & `autosubmit_api-3.1.0/autosubmit_api/config/confConfigStrategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-#!/usr/bin/env python
+
+# !/usr/bin/env python
 
 # Copyright 2015 Earth Sciences Department, BSC-CNS
 
 # This file is part of Autosubmit.
 
 # Autosubmit is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -15,88 +16,85 @@
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
 try:
     # noinspection PyCompatibility
     from configparser import SafeConfigParser
+    from autosubmitconfigparser.config.configcommon import AutosubmitConfig as Autosubmit4Config
 except ImportError:
     # noinspection PyCompatibility
     from configparser import SafeConfigParser
+
+
 import os
 import re
 import subprocess
 import json
+import logging
 
 from pyparsing import nestedExpr
 from bscearth.utils.config_parser import ConfigParserFactory, ConfigParser
 from bscearth.utils.date import parse_date
 from bscearth.utils.log import Log
 from ..config.basicConfig import BasicConfig
+from ..config.IConfigStrategy import IConfigStrategy
 
+logger = logging.getLogger('gunicorn.error')
 
-class AutosubmitConfig(object):
+class confConfigStrategy(IConfigStrategy):
     """
     Class to handle experiment configuration coming from file or database
 
     :param expid: experiment identifier
     :type expid: str
     """
 
-    def __init__(self, expid, basic_config, parser_factory, extension=".yml"):
+    def __init__(self, expid, basic_config, parser_factory, extension=".conf"):
         # type: (str, BasicConfig, ConfigParserFactory, Extension) -> None
-        self.expid = expid
 
+        self.expid = expid
         self.basic_config = basic_config
-
         self.parser_factory = parser_factory
 
         # By default check for .yml files first as it is the new standard for AS 4.0
-
-        self._conf_parser = None # type: ConfigParser
-        self._conf_parser_file = os.path.join(self.basic_config.LOCAL_ROOT_DIR, expid, "conf", "autosubmit_" + expid + extension)
+        self._conf_parser = None  # type: ConfigParser
+        self._conf_parser_file = os.path.join(self.basic_config.LOCAL_ROOT_DIR, expid, "conf",
+                                              "autosubmit_" + expid + extension)
         if os.path.exists(self._conf_parser_file) == False:
-            if extension == ".yml":
-                self.__init__(expid, basic_config, parser_factory, ".conf")
-            elif extension == ".conf":
-                return None
+           return None
 
-        self._exp_parser = None # type: ConfigParser
-        self._exp_parser_file = os.path.join(self.basic_config.LOCAL_ROOT_DIR, expid, "conf", "expdef_" + expid + extension)
+        self._exp_parser = None  # type: ConfigParser
+        self._exp_parser_file = os.path.join(self.basic_config.LOCAL_ROOT_DIR, expid, "conf",
+                                             "expdef_" + expid + extension)
         if os.path.exists(self._exp_parser_file) == False:
-            if extension == ".yml":
-                self.__init__(expid, basic_config, parser_factory, ".conf")
-            elif extension == ".conf":
-                return None
+           return None
 
-        self._platforms_parser = None # type: ConfigParser
-        self._platforms_parser_file = os.path.join(self.basic_config.LOCAL_ROOT_DIR, expid, "conf", "platforms_" + expid + extension)
+        self._platforms_parser = None  # type: ConfigParser
+        self._platforms_parser_file = os.path.join(self.basic_config.LOCAL_ROOT_DIR, expid, "conf",
+                                                   "platforms_" + expid + extension)
         if os.path.exists(self._platforms_parser_file) == False:
-            if extension == ".yml":
-                self.__init__(expid, basic_config, parser_factory, ".conf")
-            elif extension == ".conf":
-                return None
+           return None
 
-        self._jobs_parser = None # type: ConfigParser
-        self._jobs_parser_file = os.path.join(self.basic_config.LOCAL_ROOT_DIR, expid, "conf", "jobs_" + expid + extension)
+        self._jobs_parser = None  # type: ConfigParser
+        self._jobs_parser_file = os.path.join(self.basic_config.LOCAL_ROOT_DIR, expid, "conf",
+                                              "jobs_" + expid + extension)
         if os.path.exists(self._jobs_parser_file) == False:
-            if extension == ".yml":
-                self.__init__(expid, basic_config, parser_factory, ".conf")
-            elif extension == ".conf":
-                return None
+           return None
 
-        self._proj_parser = None # type: ConfigParser
-        self._proj_parser_file = os.path.join(self.basic_config.LOCAL_ROOT_DIR, expid, "conf", "proj_" + expid + extension)
+        self._proj_parser = None  # type: ConfigParser
+        self._proj_parser_file = os.path.join(self.basic_config.LOCAL_ROOT_DIR, expid, "conf",
+                                              "proj_" + expid + extension)
         if os.path.exists(self._proj_parser_file) == False:
-            if extension == ".yml":
-                self.__init__(expid, basic_config, parser_factory, ".conf")
-            elif extension == ".conf":
-                return None
+           return None
 
-        self.check_proj_file()
+
+    @property
+    def jobs_parser(self):
+        return self._jobs_parser
 
     @property
     def jobs_parser(self):
         return self._jobs_parser
 
     @property
     def experiment_file(self):
@@ -128,28 +126,14 @@
     @property
     def project_file(self):
         """
         Returns project's config file name
         """
         return self._proj_parser_file
 
-    def check_proj_file(self):
-        """
-        Add a section header to the project's configuration file (if not exists)
-        """
-        # if os.path.exists(self._proj_parser_file):
-        #     with open(self._proj_parser_file, 'w') as f:
-        #         first_line = f.readline()
-        #         if not re.match('[[a-zA-Z0-9]*]', first_line):
-        #             content = f.read()
-        #             f.seek(0, 0)
-        #             f.write('[DEFAULT]'.rstrip('\r\n') +
-        #                     '\n' + first_line + content)
-        pass
-
     @property
     def jobs_file(self):
         """
         Returns project's jobs file name
         """
         return self._jobs_parser_file
 
@@ -163,14 +147,15 @@
         def get_data(parser):
             """
             dictionary comprehension to get data from parser
             """
             res = {sec: {option: parser.get(sec, option) for option in parser.options(sec)} for sec in [
                 section for section in parser.sections()]}
             return res
+
         # print(self._conf_parser)
         result["conf"] = get_data(
             self._conf_parser) if self._conf_parser else None
         result["exp"] = get_data(
             self._exp_parser) if self._exp_parser else None
         result["platforms"] = get_data(
             self._platforms_parser) if self._platforms_parser else None
@@ -686,26 +671,30 @@
                 self.get_platform(), 'MAX_WALLCLOCK')
         return result
 
     def reload(self):
         """
         Creates parser objects for configuration files
         """
-        if not os.path.exists(self._conf_parser_file): raise IOError("Required file not found {0}".format(self._conf_parser_file))
-        if not os.path.exists(self._platforms_parser_file): raise IOError("Required file not found {0}".format(self._platforms_parser_file))
-        if not os.path.exists(self._jobs_parser_file): raise IOError("Required file not found {0}".format(self._jobs_parser_file))
-        if not os.path.exists(self._exp_parser_file): raise IOError("Required file not found {0}".format(self._exp_parser_file))
-        self._conf_parser = AutosubmitConfig.get_parser(self.parser_factory, self._conf_parser_file)
-        self._platforms_parser = AutosubmitConfig.get_parser(self.parser_factory, self._platforms_parser_file)
-        self._jobs_parser = AutosubmitConfig.get_parser(self.parser_factory, self._jobs_parser_file)
-        self._exp_parser = AutosubmitConfig.get_parser(self.parser_factory, self._exp_parser_file)
+        if not os.path.exists(self._conf_parser_file): raise IOError(
+            "Required file not found {0}".format(self._conf_parser_file))
+        if not os.path.exists(self._platforms_parser_file): raise IOError(
+            "Required file not found {0}".format(self._platforms_parser_file))
+        if not os.path.exists(self._jobs_parser_file): raise IOError(
+            "Required file not found {0}".format(self._jobs_parser_file))
+        if not os.path.exists(self._exp_parser_file): raise IOError(
+            "Required file not found {0}".format(self._exp_parser_file))
+        self._conf_parser = confConfigStrategy.get_parser(self.parser_factory, self._conf_parser_file)
+        self._platforms_parser = confConfigStrategy.get_parser(self.parser_factory, self._platforms_parser_file)
+        self._jobs_parser = confConfigStrategy.get_parser(self.parser_factory, self._jobs_parser_file)
+        self._exp_parser = confConfigStrategy.get_parser(self.parser_factory, self._exp_parser_file)
         if self._proj_parser_file == '':
             self._proj_parser = None
         else:
-            self._proj_parser = AutosubmitConfig.get_parser(self.parser_factory, self._proj_parser_file)
+            self._proj_parser = confConfigStrategy.get_parser(self.parser_factory, self._proj_parser_file)
 
     def load_parameters(self):
         """
         Load parameters from experiment and autosubmit config files. If experiment's type is not none,
         also load parameters from model's config file
 
         :return: a dictionary containing tuples [parameter_name, parameter_value]
@@ -853,16 +842,17 @@
         """
         Function to register in the configuration the commit SHA of the git project version.
         :param as_conf: Configuration class for exteriment
         :type as_conf: AutosubmitConfig
         """
         full_project_path = as_conf.get_project_dir()
         try:
-            output = subprocess.check_output("cd {0}; git rev-parse --abbrev-ref HEAD".format(full_project_path),
-                                             shell=True)
+            output = subprocess.check_output(
+                "cd {0}; git rev-parse --abbrev-ref HEAD".format(full_project_path),
+                shell=True)
         except subprocess.CalledProcessError:
             Log.critical("Failed to retrieve project branch...")
             return False
 
         project_branch = output
         Log.debug("Project branch is: " + project_branch)
         try:
@@ -1008,15 +998,16 @@
         """
         Returns members list from experiment's config file
 
         :return: experiment's members
         :rtype: list
         """
         member_list = list()
-        string = self._exp_parser.get('experiment', 'MEMBERS') if run_only == False else self._exp_parser.get_option(
+        string = self._exp_parser.get('experiment',
+                                      'MEMBERS') if run_only == False else self._exp_parser.get_option(
             'experiment', 'RUN_ONLY_MEMBERS', '')
         if not string.startswith("["):
             string = '[{0}]'.format(string)
         split_string = nestedExpr('[', ']').parseString(string).asList()
         string_member = None
         for split in split_string[0]:
             if type(split) is list:
```

### Comparing `autosubmit_api-2.1.0/autosubmit_api/database/autosubmit.py` & `autosubmit_api-3.1.0/autosubmit_api/database/autosubmit.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/database/db_common.py` & `autosubmit_api-3.1.0/autosubmit_api/database/db_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,16 +361,14 @@
         last_modified_pkl_datetime = None
         try:
             autosubmit_config_facade = ConfigurationFacadeDirector(AutosubmitConfigurationFacadeBuilder(expid)).build_autosubmit_configuration_facade()
             version = autosubmit_config_facade.get_autosubmit_version()
             wrapper = autosubmit_config_facade.get_wrapper_type()
             last_modified_pkl_datetime = autosubmit_config_facade.get_pkl_last_modified_time_as_datetime()
         except Exception as exp:
-            version = "Unknown"
-            wrapper = None
             last_modified_pkl_datetime = None
             pass
         status = experiment_status.get(expid, "NOT RUNNING")
         total, completed, last_modified_timestamp = experiment_times.get(
             expid, ("NA", "NA", None))
 
         # Getting run data from historical database
@@ -450,16 +448,14 @@
         if status == "RUNNING":
             try:
                 autosubmit_config_facade = ConfigurationFacadeDirector(AutosubmitConfigurationFacadeBuilder(expid)).build_autosubmit_configuration_facade()
                 version = autosubmit_config_facade.get_autosubmit_version()
                 wrapper = autosubmit_config_facade.get_wrapper_type()
                 last_modified_pkl_datetime = autosubmit_config_facade.get_pkl_last_modified_time_as_datetime()
             except Exception as exp:
-                version = "Unknown"
-                wrapper = None
                 last_modified_pkl_datetime = None
                 pass
             if (expid in experiment_times):
                 if len(user) == 0:
                     # Retrieve user from path
                     path = BasicConfig.LOCAL_ROOT_DIR + '/' + expid
                     if (os.path.exists(path)):
```

### Comparing `autosubmit_api-2.1.0/autosubmit_api/database/db_jobdata.py` & `autosubmit_api-3.1.0/autosubmit_api/database/db_jobdata.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/database/db_manager.py` & `autosubmit_api-3.1.0/autosubmit_api/database/db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/database/db_structure.py` & `autosubmit_api-3.1.0/autosubmit_api/database/db_structure.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/experiment/as_times_db_manager.py` & `autosubmit_api-3.1.0/autosubmit_api/experiment/as_times_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/experiment/common_db_requests.py` & `autosubmit_api-3.1.0/autosubmit_api/experiment/common_db_requests.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/experiment/common_requests.py` & `autosubmit_api-3.1.0/autosubmit_api/experiment/common_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 import time
 import pickle
 import traceback
 import datetime
 import json
 import multiprocessing
 import subprocess
+import logging
+
 from collections import deque
 from ..autosubmit_legacy.autosubmit import Autosubmit
 from ..database import db_common as db_common
 from . import common_db_requests as DbRequests
 from ..database import db_jobdata as JobData
 from ..autosubmit_legacy.job import job_utils as LegacyJobUtils
 from ..common import utils as common_utils
@@ -61,14 +63,16 @@
 from autosubmitconfigparser.config.configcommon import AutosubmitConfig as Autosubmit4Config
 
 BasicConfig.read()
 
 SAFE_TIME_LIMIT = 300
 SAFE_TIME_LIMIT_STATUS = 180
 
+# global object for logging
+logger = logging.getLogger('gunicorn.error')
 
 def get_experiment_stats(expid, filter_period, filter_type):
     # type: (str, int, str) -> Dict[str, Any]
     """
     Lite version of the stats generator from Autosubmit autosubmit.py
     """
     error = False
@@ -1115,14 +1119,15 @@
         if not as_conf.check_conf_files():
             #print('Can not create with invalid configuration')
             return (wrapper_type, max_wrapped)
         wrapper_type = as_conf.get_wrapper_type()
         max_wrapped = as_conf.get_max_wrapped_jobs()
         return (wrapper_type, max_wrapped)
     except Exception as ex:
+        logger.info(traceback.format_exc())
         print(("Couldn't retrieve conf data (wrapper info) from {0}. Exception {1}.".format(expid, str(ex))))
         return ("None", 0)
 
 
 def verify_last_completed(seconds=300):
     """
     Verifying last 300 seconds by default
@@ -1376,14 +1381,15 @@
             currentFileSystemConfig["contains_nones"] = True if not currentFileSystemConfigContent or None in list(currentFileSystemConfigContent.values(
             )) else False
 
         except Exception as exp:
             warning = True
             warning_message = "The filesystem system configuration can't be retrieved because '{}'".format(
                 exp)
+            logger.info(traceback.format_exc())
             currentFileSystemConfig["contains_nones"] = True
             log.info(warning_message)
             pass
 
         removeParameterDuplication(currentRunConfig, "EXPID", ["experiment"])
         removeParameterDuplication(currentFileSystemConfig, "EXPID", ["experiment"])
 
@@ -1466,18 +1472,21 @@
                                 "SYPD": experiment_run.getSYPD(valid_SIM_in_run),
                                 "ASYPD": experiment_run.getASYPD(valid_SIM_in_run, valid_POST_in_run, run_id_wrapper_code_to_job_dcs)})
             result.sort(key=lambda x: x["run_id"], reverse=True)
         else:
             error = True
             error_message = "No data"
     except Exception as exp:
-        print((traceback.format_exc()))
         error = True
         error_message = str(exp)
+        logger.info( traceback.format_exc() )
+        logger.info("Error: " + error_message)
         pass
+        # for full debug, uncomment this
+        #raise exp
     return {"error": error, "error_message": error_message, "runs": result}
 
 
 def read_esarchive(result):
     # t0 = time.time()
     # Using as_times.db as reference
     current_latency = 10000
```

### Comparing `autosubmit_api-2.1.0/autosubmit_api/experiment/experiment_common.py` & `autosubmit_api-3.1.0/autosubmit_api/experiment/experiment_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/experiment/experiment_db_manager.py` & `autosubmit_api-3.1.0/autosubmit_api/experiment/experiment_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/experiment/test.py` & `autosubmit_api-3.1.0/autosubmit_api/experiment/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/experiment/utils.py` & `autosubmit_api-3.1.0/autosubmit_api/experiment/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/get-pip.py` & `autosubmit_api-3.1.0/autosubmit_api/get-pip.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/git/autosubmit_git.py` & `autosubmit_api-3.1.0/autosubmit_api/git/autosubmit_git.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/data_classes/experiment_run.py` & `autosubmit_api-3.1.0/autosubmit_api/history/data_classes/experiment_run.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,108 +19,146 @@
 import json
 from ...common import utils as common_utils
 from ...performance import utils as PUtils
 from ..utils import get_current_datetime_if_none
 from .job_data import JobData
 from ...components.jobs.job_factory import SimJob
 from typing import List, Dict, Tuple
+
+
+class DatabaseCorruptedException(Exception):
+    """Exception raised when the database is corrupted or present issues in its schema.
+
+    Attributes:
+        databaseName -- nameID
+        tableName -- TableID
+        message -- error description
+        sourceException -- original exception
+    """
+
+    def __init__(self, db, table, exp,
+                 msg = "Database file seems corrupted or with wrong schema, please contact Autosubmit support team"):
+        self.databaseName = db
+        self.tableName = table
+        self.sourceException = exp
+        self.message = msg
+        super().__init__(self.message)
+
+
 class ExperimentRun(object):
-  """
+    """
   Class that represents an experiment run
   """
-  def __init__(self, run_id, created=None, modified=None, start=0, finish=0, chunk_unit="NA", chunk_size=0, completed=0, total=0, failed=0, queuing=0, running=0, submitted=0, suspended=0, metadata=""):
-    self.run_id = run_id
-    self.created = get_current_datetime_if_none(created)
-    self.modified = get_current_datetime_if_none(modified) # Added on DB 16
-    self.start = start
-    self.finish = finish
-    self.chunk_unit = chunk_unit # type: str
-    self.chunk_size = chunk_size # type: int
-    self.submitted = submitted # type: int
-    self.queuing = queuing # type: int
-    self.running = running # type: int
-    self.completed = completed # type: int
-    self.failed = failed # type: int
-    self.total = total # type: int
-    self.suspended = suspended # type: int
-    self.metadata = metadata
-
-  @property
-  def created_timestamp(self):
-    return common_utils.tostamp(self.created)
-
-  @property
-  def modified_timestamp(self):
-    return common_utils.tostamp(self.modified)
-
-  def get_wrapper_type(self):
-    if self.metadata:
-      data = json.loads(self.metadata)
-      wrapper_section = data["conf"].get("wrapper", None)
-      if wrapper_section:
-        wrapper_type = wrapper_section.get("TYPE", None)
-        if wrapper_type:
-          return wrapper_type
-    return None
-
-  def getSYPD(self, job_list):
-    # type: (List[JobData]) -> float
-    outlier_free_list = []
-    if job_list:
-        performance_jobs = [SimJob.from_job_data_dc(job_data_dc) for job_data_dc in job_list]
-        outlier_free_list = common_utils.get_jobs_with_no_outliers(performance_jobs)
-    # print("{} -> {}".format(self.run_id, len(outlier_free_list)))
-    if len(outlier_free_list) > 0:
-        years_per_sim = PUtils.datechunk_to_year(self.chunk_unit, self.chunk_size)
-        # print(self.run_id)
-        # print(years_per_sim)
-        seconds_per_day = 86400
-        number_SIM = len(outlier_free_list)
-        # print(len(job_list))
-        total_run_time = sum(job.run_time for job in outlier_free_list)
-        # print("run {3} yps {0} n {1} run_time {2}".format(years_per_sim, number_SIM, total_run_time, self.run_id))
-        if total_run_time > 0:
-            return round((years_per_sim * number_SIM * seconds_per_day) / total_run_time, 2)
-    return None
-
-  def getASYPD(self, job_sim_list, job_post_list, run_id_wrapper_code_to_job_dcs):
-    # type: (List[JobData], List[JobData], Dict[Tuple[int, int], List[JobData]]) -> float
-    SIM_no_outlier_list = []
-    if job_sim_list and len(job_sim_list) > 0:
-        performance_jobs = [SimJob.from_job_data_dc(job_data_dc) for job_data_dc in job_sim_list]
-        SIM_no_outlier_list = common_utils.get_jobs_with_no_outliers(performance_jobs)
-        valid_names = set([job.name for job in SIM_no_outlier_list])
-        job_sim_list = [job for job in job_sim_list if job.job_name in valid_names]
-
-    if job_sim_list and len(job_sim_list) > 0 and job_post_list and len(job_post_list) > 0:
-        years_per_sim = PUtils.datechunk_to_year(self.chunk_unit, self.chunk_size)
-        seconds_per_day = 86400
-        number_SIM = len(job_sim_list)
-        number_POST = len(job_post_list)
-        average_POST = round(sum(job.queuing_time_considering_package(run_id_wrapper_code_to_job_dcs.get((job.run_id, job.rowtype), [])) + job.running_time for job in job_post_list) / number_POST, 2)
-
-        sum_SIM = round(sum(job.queuing_time_considering_package(run_id_wrapper_code_to_job_dcs.get((job.run_id, job.rowtype), [])) + job.running_time for job in job_sim_list), 2)
-        if (sum_SIM + average_POST) > 0:
-            return round((years_per_sim * number_SIM * seconds_per_day) / (sum_SIM + average_POST), 2)
-    return None
-
-  @classmethod
-  def from_model(cls, row):
-    """ Build ExperimentRun from ExperimentRunRow """
-    row_dict = row._asdict()
-    experiment_run = cls(0)
-    experiment_run.run_id = row_dict.get('run_id', 0)
-    experiment_run.created = get_current_datetime_if_none(row_dict.get('created', None))
-    experiment_run.modified = get_current_datetime_if_none(row_dict.get('modified', None))
-    experiment_run.start = int(row_dict.get('start', 0))
-    experiment_run.finish = int(row_dict.get('finish', 0))
-    experiment_run.chunk_unit = row_dict.get('chunk_unit', None)
-    experiment_run.chunk_size = row_dict.get('chunk_size', None)
-    experiment_run.completed = int(row_dict.get('completed', 0))
-    experiment_run.total = row_dict.get('total', 0)
-    experiment_run.failed = row_dict.get('failed', 0)
-    experiment_run.queuing = row_dict.get('queuing', 0)
-    experiment_run.running = row_dict.get('running', 0)
-    experiment_run.submitted = row_dict.get('submitted', 0)
-    experiment_run.suspended = int(row_dict.get('suspended', 0))
-    experiment_run.metadata = row_dict.get('metadata', "")
-    return experiment_run
+
+    def __init__(self, run_id, created=None, modified=None, start=0, finish=0, chunk_unit="NA", chunk_size=0,
+                 completed=0, total=0, failed=0, queuing=0, running=0, submitted=0, suspended=0, metadata=""):
+        self.run_id = run_id
+        self.created = get_current_datetime_if_none(created)
+        self.modified = get_current_datetime_if_none(modified)  # Added on DB 16
+        self.start = start
+        self.finish = finish
+        self.chunk_unit = chunk_unit  # type: str
+        self.chunk_size = chunk_size  # type: int
+        self.submitted = submitted  # type: int
+        self.queuing = queuing  # type: int
+        self.running = running  # type: int
+        self.completed = completed  # type: int
+        self.failed = failed  # type: int
+        self.total = total  # type: int
+        self.suspended = suspended  # type: int
+        self.metadata = metadata
+
+    @property
+    def created_timestamp(self):
+        return common_utils.tostamp(self.created)
+
+    @property
+    def modified_timestamp(self):
+        return common_utils.tostamp(self.modified)
+
+    def get_wrapper_type(self):
+        if self.metadata:
+            data = json.loads(self.metadata)
+            wrapper_section = data["conf"].get("wrapper", None)
+            if wrapper_section:
+                wrapper_type = wrapper_section.get("TYPE", None)
+                if wrapper_type:
+                    return wrapper_type
+        return None
+
+    def getSYPD(self, job_list):
+        # type: (List[JobData]) -> float
+        outlier_free_list = []
+        if job_list:
+            performance_jobs = [SimJob.from_job_data_dc(job_data_dc) for job_data_dc in job_list]
+            outlier_free_list = common_utils.get_jobs_with_no_outliers(performance_jobs)
+        # print("{} -> {}".format(self.run_id, len(outlier_free_list)))
+        if len(outlier_free_list) > 0:
+            years_per_sim = PUtils.datechunk_to_year(self.chunk_unit, self.chunk_size)
+            # print(self.run_id)
+            # print(years_per_sim)
+            seconds_per_day = 86400
+            number_SIM = len(outlier_free_list)
+            # print(len(job_list))
+            total_run_time = sum(job.run_time for job in outlier_free_list)
+            # print("run {3} yps {0} n {1} run_time {2}".format(years_per_sim, number_SIM, total_run_time, self.run_id))
+            if total_run_time > 0:
+                return round((years_per_sim * number_SIM * seconds_per_day) / total_run_time, 2)
+        return None
+
+    def getASYPD(self, job_sim_list, job_post_list, run_id_wrapper_code_to_job_dcs):
+        # type: (List[JobData], List[JobData], Dict[Tuple[int, int], List[JobData]]) -> float
+
+        try:
+
+            SIM_no_outlier_list = []
+            if job_sim_list and len(job_sim_list) > 0:
+                performance_jobs = [SimJob.from_job_data_dc(job_data_dc) for job_data_dc in job_sim_list]
+                SIM_no_outlier_list = common_utils.get_jobs_with_no_outliers(performance_jobs)
+                valid_names = set([job.name for job in SIM_no_outlier_list])
+                job_sim_list = [job for job in job_sim_list if job.job_name in valid_names]
+
+            if job_sim_list and len(job_sim_list) > 0 and job_post_list and len(job_post_list) > 0:
+                years_per_sim = PUtils.datechunk_to_year(self.chunk_unit, self.chunk_size)
+                seconds_per_day = 86400
+                number_SIM = len(job_sim_list)
+                number_POST = len(job_post_list)
+                average_POST = round(sum(job.queuing_time_considering_package(
+                    run_id_wrapper_code_to_job_dcs.get((job.run_id, job.rowtype), [])) + job.running_time for job in
+                                         job_post_list) / number_POST, 2)
+
+                sum_SIM = round(sum(job.queuing_time_considering_package(
+                    run_id_wrapper_code_to_job_dcs.get((job.run_id, job.rowtype), [])) + job.running_time for job in
+                                    job_sim_list), 2)
+                if (sum_SIM + average_POST) > 0:
+                    return round((years_per_sim * number_SIM * seconds_per_day) / (sum_SIM + average_POST), 2)
+            return None
+
+        except Exception as exp:
+            dbexception = DatabaseCorruptedException("job_list_XXX.db", "experiment_run", exp)
+            raise dbexception
+
+    @classmethod
+    def from_model(cls, row):
+        """ Build ExperimentRun from ExperimentRunRow """
+        try:
+            row_dict = row._asdict()
+            experiment_run = cls(0)
+            experiment_run.run_id = row_dict.get('run_id', 0)
+            experiment_run.created = get_current_datetime_if_none(row_dict.get('created', None))
+            experiment_run.modified = get_current_datetime_if_none(row_dict.get('modified', None))
+            experiment_run.start = int(row_dict.get('start', 0))
+            experiment_run.finish = int(row_dict.get('finish', 0))
+            experiment_run.chunk_unit = row_dict.get('chunk_unit', None)
+            experiment_run.chunk_size = row_dict.get('chunk_size', None)
+            experiment_run.completed = int(row_dict.get('completed', 0))
+            experiment_run.total = row_dict.get('total', 0)
+            experiment_run.failed = row_dict.get('failed', 0)
+            experiment_run.queuing = row_dict.get('queuing', 0)
+            experiment_run.running = row_dict.get('running', 0)
+            experiment_run.submitted = row_dict.get('submitted', 0)
+            experiment_run.suspended = int(row_dict.get('suspended', 0))
+            experiment_run.metadata = row_dict.get('metadata', "")
+            return experiment_run
+        except Exception as exp:
+            dbexception = DatabaseCorruptedException("job_list_XXX.db", "experiment_run", exp)
+            raise dbexception
```

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/data_classes/job_data.py` & `autosubmit_api-3.1.0/autosubmit_api/history/data_classes/job_data.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/database_managers/database_manager.py` & `autosubmit_api-3.1.0/autosubmit_api/history/database_managers/database_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/database_managers/database_models.py` & `autosubmit_api-3.1.0/autosubmit_api/history/database_managers/database_models.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/database_managers/experiment_history_db_manager.py` & `autosubmit_api-3.1.0/autosubmit_api/history/database_managers/experiment_history_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/database_managers/experiment_status_db_manager.py` & `autosubmit_api-3.1.0/autosubmit_api/history/database_managers/experiment_status_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/database_managers/test.py` & `autosubmit_api-3.1.0/autosubmit_api/history/database_managers/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/experiment_history.py` & `autosubmit_api-3.1.0/autosubmit_api/history/experiment_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/experiment_status.py` & `autosubmit_api-3.1.0/autosubmit_api/history/experiment_status.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/experiment_status_manager.py` & `autosubmit_api-3.1.0/autosubmit_api/history/experiment_status_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/internal_logging.py` & `autosubmit_api-3.1.0/autosubmit_api/history/internal_logging.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/platform_monitor/platform_monitor.py` & `autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/platform_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/platform_monitor/platform_utils.py` & `autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/platform_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/platform_monitor/slurm_monitor.py` & `autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/slurm_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/platform_monitor/slurm_monitor_item.py` & `autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/slurm_monitor_item.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/platform_monitor/test.py` & `autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/strategies.py` & `autosubmit_api-3.1.0/autosubmit_api/history/strategies.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/test.py` & `autosubmit_api-3.1.0/autosubmit_api/history/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/test_job_history.py` & `autosubmit_api-3.1.0/autosubmit_api/history/test_job_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/test_strategies.py` & `autosubmit_api-3.1.0/autosubmit_api/history/test_strategies.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/test_utils.py` & `autosubmit_api-3.1.0/autosubmit_api/history/test_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/history/utils.py` & `autosubmit_api-3.1.0/autosubmit_api/history/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/monitor/diagram.py` & `autosubmit_api-3.1.0/autosubmit_api/monitor/diagram.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/monitor/monitor.py` & `autosubmit_api-3.1.0/autosubmit_api/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/monitor/utils.py` & `autosubmit_api-3.1.0/autosubmit_api/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/notifications/mail_notifier.py` & `autosubmit_api-3.1.0/autosubmit_api/notifications/mail_notifier.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/notifications/notifier.py` & `autosubmit_api-3.1.0/autosubmit_api/notifications/notifier.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/performance/performance_metrics.py` & `autosubmit_api-3.1.0/autosubmit_api/performance/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/performance/utils.py` & `autosubmit_api-3.1.0/autosubmit_api/performance/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/statistics/job_stat.py` & `autosubmit_api-3.1.0/autosubmit_api/statistics/job_stat.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/statistics/statistics.py` & `autosubmit_api-3.1.0/autosubmit_api/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/statistics/stats_summary.py` & `autosubmit_api-3.1.0/autosubmit_api/statistics/stats_summary.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/statistics/test.py` & `autosubmit_api-3.1.0/autosubmit_api/statistics/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/statistics/utils.py` & `autosubmit_api-3.1.0/autosubmit_api/statistics/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/workers/business/populate_times.py` & `autosubmit_api-3.1.0/autosubmit_api/workers/business/populate_times.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/workers/business/process_graph_drawings.py` & `autosubmit_api-3.1.0/autosubmit_api/workers/business/process_graph_drawings.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/workers/deprecated/fix_historic.py` & `autosubmit_api-3.1.0/autosubmit_api/workers/deprecated/fix_historic.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/workers/deprecated/fix_historic_energy.py` & `autosubmit_api-3.1.0/autosubmit_api/workers/deprecated/fix_historic_energy.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/workers/populate_details/populate.py` & `autosubmit_api-3.1.0/autosubmit_api/workers/populate_details/populate.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/workers/populate_details/test.py` & `autosubmit_api-3.1.0/autosubmit_api/workers/populate_details/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api/workers/test.py` & `autosubmit_api-3.1.0/autosubmit_api/workers/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-2.1.0/autosubmit_api.egg-info/PKG-INFO` & `autosubmit_api-3.1.0/autosubmit_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit-api
-Version: 2.1.0
+Version: 3.1.0
 Summary: An extension to the Autosubmit package that serves its information as an API
 Home-page: https://earth.bsc.es/gitlab/wuruchi/autosubmit_api
 Author: Wilmer Uruchi
 Author-email: wilmer.uruchi@bsc.es
 License: GNU GPL
 Keywords: autosubmit,API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `autosubmit_api-2.1.0/autosubmit_api.egg-info/SOURCES.txt` & `autosubmit_api-3.1.0/autosubmit_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -79,17 +79,20 @@
 autosubmit_api/components/representations/graph/__init__.py
 autosubmit_api/components/representations/graph/edge.py
 autosubmit_api/components/representations/graph/graph.py
 autosubmit_api/components/representations/graph/test.py
 autosubmit_api/components/representations/tree/__init__.py
 autosubmit_api/components/representations/tree/test.py
 autosubmit_api/components/representations/tree/tree.py
+autosubmit_api/config/IConfigStrategy.py
 autosubmit_api/config/__init__.py
 autosubmit_api/config/basicConfig.py
+autosubmit_api/config/confConfigStrategy.py
 autosubmit_api/config/config_common.py
+autosubmit_api/config/ymlConfigStrategy.py
 autosubmit_api/database/__init__.py
 autosubmit_api/database/autosubmit.py
 autosubmit_api/database/db_common.py
 autosubmit_api/database/db_jobdata.py
 autosubmit_api/database/db_manager.py
 autosubmit_api/database/db_structure.py
 autosubmit_api/experiment/__init__.py
```

### Comparing `autosubmit_api-2.1.0/setup.py` & `autosubmit_api-3.1.0/setup.py`

 * *Files identical despite different names*

