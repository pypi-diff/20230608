# Comparing `tmp/datatoolbox-0.5.8.tar.gz` & `tmp/datatoolbox-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatoolbox-0.5.8.tar", last modified: Tue May 23 13:06:22 2023, max compression
+gzip compressed data, was "datatoolbox-0.6.1.tar", last modified: Thu Jun  8 10:02:14 2023, max compression
```

## Comparing `datatoolbox-0.5.8.tar` & `datatoolbox-0.6.1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/
--rwxrwx---   0 root         (0) vboxsf     (999)      159 2022-05-25 07:15:53.000000 datatoolbox-0.5.8/.gitignore
--rwxrwx---   0 root         (0) vboxsf     (999)      950 2022-10-19 13:17:33.000000 datatoolbox-0.5.8/.gitlab-ci.yml
--rwxrwx---   0 root         (0) vboxsf     (999)      703 2020-10-14 14:04:18.000000 datatoolbox-0.5.8/.travis.yml
--rwxrwx---   0 root         (0) vboxsf     (999)     1073 2020-10-14 14:04:18.000000 datatoolbox-0.5.8/LICENSE
--rwxrwx---   0 root         (0) vboxsf     (999)     1037 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)      771 2022-05-25 07:15:53.000000 datatoolbox-0.5.8/README.md
--rwxrwx---   0 root         (0) vboxsf     (999)     1225 2020-10-14 14:04:18.000000 datatoolbox-0.5.8/appveyor.yml
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/ci/
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/ci/appveyor/
--rwxrwx---   0 root         (0) vboxsf     (999)     3111 2020-10-14 14:04:18.000000 datatoolbox-0.5.8/ci/appveyor/install.ps1
--rwxrwx---   0 root         (0) vboxsf     (999)     1842 2020-10-14 14:04:18.000000 datatoolbox-0.5.8/ci/appveyor/run_with_env.cmd
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/datatoolbox/
--rwxrwx---   0 root         (0) vboxsf     (999)     4362 2023-05-04 12:41:44.000000 datatoolbox-0.5.8/datatoolbox/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (999)    15385 2023-03-30 07:48:47.000000 datatoolbox-0.5.8/datatoolbox/admin.py
--rwxrwx---   0 root         (0) vboxsf     (999)     6655 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/config.py
--rwxrwx---   0 root         (0) vboxsf     (999)    18622 2023-05-23 08:37:11.000000 datatoolbox-0.5.8/datatoolbox/converters.py
--rwxrwx---   0 root         (0) vboxsf     (999)    12133 2023-05-12 12:29:10.000000 datatoolbox-0.5.8/datatoolbox/core.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/datatoolbox/data/
--rwxrwx---   0 root         (0) vboxsf     (999)    15781 2020-10-14 14:04:18.000000 datatoolbox-0.5.8/datatoolbox/data/GHG_alternative_naming.pkl
--rwxrwx---   0 root         (0) vboxsf     (999)    13482 2023-05-23 13:04:06.000000 datatoolbox-0.5.8/datatoolbox/data/GHG_properties_2019_CA.csv
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/datatoolbox/data/SANDBOX_datashelf/
--rwxrwx---   0 root         (0) vboxsf     (999)      286 2023-05-23 13:05:21.000000 datatoolbox-0.5.8/datatoolbox/data/SANDBOX_datashelf/inventory.csv
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/datatoolbox/data/SANDBOX_datashelf/mappings/
--rwxrwx---   0 root         (0) vboxsf     (999)    10757 2023-05-23 13:05:19.000000 datatoolbox-0.5.8/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     8466 2023-05-23 13:05:19.000000 datatoolbox-0.5.8/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv
--rwxrwx---   0 root         (0) vboxsf     (999)      999 2023-05-23 13:05:19.000000 datatoolbox-0.5.8/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv
--rwxrwx---   0 root         (0) vboxsf     (999)      161 2023-05-23 13:05:21.000000 datatoolbox-0.5.8/datatoolbox/data/SANDBOX_datashelf/sources.csv
--rwxrwx---   0 root         (0) vboxsf     (999)    22865 2020-10-14 14:04:18.000000 datatoolbox-0.5.8/datatoolbox/data/all.csv
--rwxrwx---   0 root         (0) vboxsf     (999)    14615 2020-10-14 14:04:18.000000 datatoolbox-0.5.8/datatoolbox/data/compatible1_5_unfiltered.xlsx
--rwxrwx---   0 root         (0) vboxsf     (999)    10757 2020-04-20 12:32:09.000000 datatoolbox-0.5.8/datatoolbox/data/continent.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     8466 2021-09-15 15:48:16.000000 datatoolbox-0.5.8/datatoolbox/data/country_codes.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     1711 2022-05-25 07:15:53.000000 datatoolbox-0.5.8/datatoolbox/data/datashelf_contents.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     2923 2021-12-16 12:32:58.000000 datatoolbox-0.5.8/datatoolbox/data/external_mappings.py
--rwxrwx---   0 root         (0) vboxsf     (999)      178 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/data/personal_template.py
--rwxrwx---   0 root         (0) vboxsf     (999)      999 2019-08-14 10:00:22.000000 datatoolbox-0.5.8/datatoolbox/data/regions.csv
--rwxrwx---   0 root         (0) vboxsf     (999)   237054 2023-04-28 11:35:43.000000 datatoolbox-0.5.8/datatoolbox/data_readers.py
--rwxrwx---   0 root         (0) vboxsf     (999)    69372 2023-05-23 08:25:42.000000 datatoolbox-0.5.8/datatoolbox/data_structures.py
--rwxrwx---   0 root         (0) vboxsf     (999)    64211 2023-05-10 08:59:02.000000 datatoolbox-0.5.8/datatoolbox/database.py
--rwxrwx---   0 root         (0) vboxsf     (999)     6730 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/greenhouse_gas_database.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3542 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/init_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)    21652 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/interfaces.py
--rwxrwx---   0 root         (0) vboxsf     (999)    11015 2023-05-23 13:04:54.000000 datatoolbox-0.5.8/datatoolbox/io_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)    41818 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/mapping.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2854 2022-12-01 09:27:15.000000 datatoolbox-0.5.8/datatoolbox/naming_convention.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3305 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/patches.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2189 2023-05-12 10:35:54.000000 datatoolbox-0.5.8/datatoolbox/pint_definitions.txt
--rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.5.8/datatoolbox/relations.py
--rwxrwx---   0 root         (0) vboxsf     (999)    26527 2023-04-05 07:52:48.000000 datatoolbox-0.5.8/datatoolbox/sets.py
--rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.5.8/datatoolbox/storage.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1632 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/templates.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/datatoolbox/tools/
--rwxrwx---   0 root         (0) vboxsf     (999)    16351 2021-04-19 11:31:45.000000 datatoolbox-0.5.8/datatoolbox/tools/CRF_extract_CA_2021.xlsx
--rwxrwx---   0 root         (0) vboxsf     (999)    28022 2021-02-02 15:17:26.000000 datatoolbox-0.5.8/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN
--rwxrwx---   0 root         (0) vboxsf     (999)    17445 2021-02-02 12:48:44.000000 datatoolbox-0.5.8/datatoolbox/tools/IEA_B2DS_4.SCEN
--rwxrwx---   0 root         (0) vboxsf     (999)    17375 2019-12-20 11:46:57.000000 datatoolbox-0.5.8/datatoolbox/tools/WEO_2019_test.SCEN
--rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/tools/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4320 2022-11-17 09:58:39.000000 datatoolbox-0.5.8/datatoolbox/tools/conversion_to_v0.3.py
--rwxrwx---   0 root         (0) vboxsf     (999)    42729 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/tools/excel.py
--rwxrwx---   0 root         (0) vboxsf     (999)      370 2022-11-17 09:58:39.000000 datatoolbox-0.5.8/datatoolbox/tools/export_all.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4441 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/tools/for_datatables.py
--rwxrwx---   0 root         (0) vboxsf     (999)     8132 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/tools/html.py
--rwxrwx---   0 root         (0) vboxsf     (999)      182 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/tools/install_support.py
--rwxrwx---   0 root         (0) vboxsf     (999)     7188 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/tools/kaya_idendentiy_decomposition.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4283 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/tools/magicc6.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5931 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/tools/matplotlib.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3797 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/tools/pandas.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5533 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/tools/py_magicc_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)     7869 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/tools/pyam.py
--rwxrwx---   0 root         (0) vboxsf     (999)      965 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/tools/renaming_DB.py
--rwxrwx---   0 root         (0) vboxsf     (999)    84992 2019-08-14 10:26:08.000000 datatoolbox-0.5.8/datatoolbox/tools/run_MAGICC_startup_simple.xlsx
--rwxrwx---   0 root         (0) vboxsf     (999)     1830 2021-02-02 14:03:36.000000 datatoolbox-0.5.8/datatoolbox/tools/run_magicc6.m
--rwxrwx---   0 root         (0) vboxsf     (999)     1044 2022-11-17 09:58:40.000000 datatoolbox-0.5.8/datatoolbox/tools/statistics.py
--rwxrwx---   0 root         (0) vboxsf     (999)    61174 2021-06-03 14:06:07.000000 datatoolbox-0.5.8/datatoolbox/tools/test.docx
--rwxrwx---   0 root         (0) vboxsf     (999)     8625 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/tools/word.py
--rwxrwx---   0 root         (0) vboxsf     (999)     9617 2023-03-30 13:29:22.000000 datatoolbox-0.5.8/datatoolbox/tools/xarray.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/datatoolbox/tutorials/
--rwxrwx---   0 root         (0) vboxsf     (999)     2996 2022-05-25 07:15:53.000000 datatoolbox-0.5.8/datatoolbox/tutorials/00_search_find_and_access_data.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1019 2020-10-14 14:04:18.000000 datatoolbox-0.5.8/datatoolbox/tutorials/01_emission_comparison.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2096 2022-05-25 07:15:53.000000 datatoolbox-0.5.8/datatoolbox/tutorials/02_unit_conversion.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5685 2020-10-14 14:04:18.000000 datatoolbox-0.5.8/datatoolbox/tutorials/03_intermediate_example.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1416 2020-10-14 14:04:19.000000 datatoolbox-0.5.8/datatoolbox/tutorials/04_sources.py
--rwxrwx---   0 root         (0) vboxsf     (999)      382 2020-10-14 14:04:19.000000 datatoolbox-0.5.8/datatoolbox/tutorials/05_plot_source_content.py
--rwxrwx---   0 root         (0) vboxsf     (999)      734 2020-12-22 15:09:15.000000 datatoolbox-0.5.8/datatoolbox/tutorials/06_xarray_examples.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1142 2021-05-11 13:19:29.000000 datatoolbox-0.5.8/datatoolbox/tutorials/07_renewable_share_compuation.py
--rwxrwx---   0 root         (0) vboxsf     (999)      793 2021-05-11 12:59:38.000000 datatoolbox-0.5.8/datatoolbox/tutorials/08_low_carbon_fuel_computation.py
--rwxrwx---   0 root         (0) vboxsf     (999)   137631 2020-10-14 14:04:19.000000 datatoolbox-0.5.8/datatoolbox/tutorials/introduction_v1.ipynb
--rwxrwx---   0 root         (0) vboxsf     (999)     4631 2022-03-22 14:54:50.000000 datatoolbox-0.5.8/datatoolbox/tutorials/jump_start.py
--rwxrwx---   0 root         (0) vboxsf     (999)      417 2023-05-12 14:15:39.000000 datatoolbox-0.5.8/datatoolbox/units.py
--rwxrwx---   0 root         (0) vboxsf     (999)    43883 2023-05-23 13:02:31.000000 datatoolbox-0.5.8/datatoolbox/util.py
--rwxrwx---   0 root         (0) vboxsf     (999)      176 2023-05-23 13:06:21.000000 datatoolbox-0.5.8/datatoolbox/version.py
--rwxrwx---   0 root         (0) vboxsf     (999)      746 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/datatoolbox/workflows.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/datatoolbox.egg-info/
--rwxrwx---   0 root         (0) vboxsf     (999)     1037 2023-05-23 13:06:21.000000 datatoolbox-0.5.8/datatoolbox.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)     3714 2023-05-23 13:06:21.000000 datatoolbox-0.5.8/datatoolbox.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) vboxsf     (999)        1 2023-05-23 13:06:21.000000 datatoolbox-0.5.8/datatoolbox.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) vboxsf     (999)      149 2023-05-23 13:06:21.000000 datatoolbox-0.5.8/datatoolbox.egg-info/requires.txt
--rwxrwx---   0 root         (0) vboxsf     (999)       12 2023-05-23 13:06:21.000000 datatoolbox-0.5.8/datatoolbox.egg-info/top_level.txt
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/doc/
--rwxrwx---   0 root         (0) vboxsf     (999)     7755 2020-10-14 14:04:19.000000 datatoolbox-0.5.8/doc/Makefile
--rwxrwx---   0 root         (0) vboxsf     (999)     9684 2020-12-22 15:09:15.000000 datatoolbox-0.5.8/doc/conf.py
--rwxrwx---   0 root         (0) vboxsf     (999)       79 2021-01-05 10:54:01.000000 datatoolbox-0.5.8/doc/core.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      149 2020-12-22 15:09:15.000000 datatoolbox-0.5.8/doc/data_structures.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      122 2021-01-11 16:19:59.000000 datatoolbox-0.5.8/doc/database.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       91 2021-01-11 16:18:53.000000 datatoolbox-0.5.8/doc/database_database.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      130 2021-01-11 16:21:50.000000 datatoolbox-0.5.8/doc/database_gitrepomanager.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       93 2021-01-11 16:03:03.000000 datatoolbox-0.5.8/doc/excel.rst
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/doc/figures/
--rwxrwx---   0 root         (0) vboxsf     (999)    21579 2020-11-09 13:08:35.000000 datatoolbox-0.5.8/doc/figures/ID_meta_data.svg
--rwxrwx---   0 root         (0) vboxsf     (999)    67463 2021-05-17 15:08:58.000000 datatoolbox-0.5.8/doc/figures/config_input.png
--rwxrwx---   0 root         (0) vboxsf     (999)     7157 2021-05-17 15:04:37.000000 datatoolbox-0.5.8/doc/first_steps.md
--rwxrwx---   0 root         (0) vboxsf     (999)      100 2020-12-22 15:09:15.000000 datatoolbox-0.5.8/doc/foo.rst_template
--rwxrwx---   0 root         (0) vboxsf     (999)       77 2020-12-22 15:09:15.000000 datatoolbox-0.5.8/doc/help.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      463 2021-01-11 16:06:28.000000 datatoolbox-0.5.8/doc/index.rst
--rwxrwx---   0 root         (0) vboxsf     (999)     1754 2021-05-21 08:03:28.000000 datatoolbox-0.5.8/doc/installation.md
--rwxrwx---   0 root         (0) vboxsf     (999)     1080 2020-12-22 15:09:15.000000 datatoolbox-0.5.8/doc/license.rst
--rwxrwx---   0 root         (0) vboxsf     (999)     7353 2020-10-14 14:04:19.000000 datatoolbox-0.5.8/doc/make.bat
--rwxrwx---   0 root         (0) vboxsf     (999)      103 2021-01-11 16:09:22.000000 datatoolbox-0.5.8/doc/matplotlib.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:10:43.000000 datatoolbox-0.5.8/doc/pandas.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      133 2021-01-11 16:20:57.000000 datatoolbox-0.5.8/doc/tools.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:09:13.000000 datatoolbox-0.5.8/doc/xarray.rst
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/documentation/
--rwxrwx---   0 root         (0) vboxsf     (999)     7761 2020-12-22 15:09:15.000000 datatoolbox-0.5.8/documentation/Datatoolbox - First steps.md
--rwxrwx---   0 root         (0) vboxsf     (999)      385 2023-05-12 12:15:15.000000 datatoolbox-0.5.8/environment.yml
--rwxrwx---   0 root         (0) vboxsf     (999)      418 2020-10-14 14:04:19.000000 datatoolbox-0.5.8/make_proj.sh
--rwxrwx---   0 root         (0) vboxsf     (999)      558 2021-01-12 15:45:18.000000 datatoolbox-0.5.8/readthedocs.yml
--rwxrwx---   0 root         (0) vboxsf     (999)      215 2022-10-19 13:17:33.000000 datatoolbox-0.5.8/requirements.txt
--rwxrwx---   0 root         (0) vboxsf     (999)       38 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/setup.cfg
--rwxrwx---   0 root         (0) vboxsf     (999)     1839 2023-05-03 11:16:28.000000 datatoolbox-0.5.8/setup.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 13:06:22.000000 datatoolbox-0.5.8/tests/
--rwxrwx---   0 root         (0) vboxsf     (999)     7292 2022-12-19 11:29:58.000000 datatoolbox-0.5.8/tests/test_calculations.py
--rwxrwx---   0 root         (0) vboxsf     (999)      696 2022-11-18 16:16:07.000000 datatoolbox-0.5.8/tests/test_converters.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2836 2022-11-21 11:08:31.000000 datatoolbox-0.5.8/tests/test_database.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1640 2023-03-30 13:32:13.000000 datatoolbox-0.5.8/tests/test_dataset.py
--rwxrwx---   0 root         (0) vboxsf     (999)     7741 2022-05-25 07:15:53.000000 datatoolbox-0.5.8/tests/test_datatable.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1063 2022-11-16 11:59:46.000000 datatoolbox-0.5.8/tests/test_io.py
--rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-22 09:54:34.000000 datatoolbox-0.5.8/tests/test_linked_functions.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1563 2023-05-04 07:49:24.000000 datatoolbox-0.5.8/tests/test_pyam.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3570 2022-05-25 07:15:53.000000 datatoolbox-0.5.8/tests/test_tableset.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2610 2022-05-25 07:15:53.000000 datatoolbox-0.5.8/tests/test_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1832 2023-05-23 12:58:33.000000 datatoolbox-0.5.8/tests/test_units.py
--rwxrwx---   0 root         (0) vboxsf     (999)      870 2020-10-14 14:04:19.000000 datatoolbox-0.5.8/tests/test_utilities.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2437 2022-10-19 13:17:33.000000 datatoolbox-0.5.8/tests/test_xarray.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2959 2022-05-25 07:15:53.000000 datatoolbox-0.5.8/tests/util_for_testing.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/
+-rwxrwx---   0 root         (0) vboxsf     (999)      159 2022-05-25 07:15:53.000000 datatoolbox-0.6.1/.gitignore
+-rwxrwx---   0 root         (0) vboxsf     (999)      950 2022-10-19 13:17:33.000000 datatoolbox-0.6.1/.gitlab-ci.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)      703 2020-10-14 14:04:18.000000 datatoolbox-0.6.1/.travis.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)     1073 2020-10-14 14:04:18.000000 datatoolbox-0.6.1/LICENSE
+-rwxrwx---   0 root         (0) vboxsf     (999)     1037 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (999)      771 2022-05-25 07:15:53.000000 datatoolbox-0.6.1/README.md
+-rwxrwx---   0 root         (0) vboxsf     (999)     1225 2020-10-14 14:04:18.000000 datatoolbox-0.6.1/appveyor.yml
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/ci/
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/ci/appveyor/
+-rwxrwx---   0 root         (0) vboxsf     (999)     3111 2020-10-14 14:04:18.000000 datatoolbox-0.6.1/ci/appveyor/install.ps1
+-rwxrwx---   0 root         (0) vboxsf     (999)     1842 2020-10-14 14:04:18.000000 datatoolbox-0.6.1/ci/appveyor/run_with_env.cmd
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/datatoolbox/
+-rwxrwx---   0 root         (0) vboxsf     (999)     4436 2023-06-08 07:56:58.000000 datatoolbox-0.6.1/datatoolbox/__init__.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    15513 2023-06-08 08:12:18.000000 datatoolbox-0.6.1/datatoolbox/admin.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     6655 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/config.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    18634 2023-05-24 14:31:15.000000 datatoolbox-0.6.1/datatoolbox/converters.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    12133 2023-05-12 12:29:10.000000 datatoolbox-0.6.1/datatoolbox/core.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/datatoolbox/data/
+-rwxrwx---   0 root         (0) vboxsf     (999)    15781 2020-10-14 14:04:18.000000 datatoolbox-0.6.1/datatoolbox/data/GHG_alternative_naming.pkl
+-rwxrwx---   0 root         (0) vboxsf     (999)    13482 2023-05-23 13:04:06.000000 datatoolbox-0.6.1/datatoolbox/data/GHG_properties_2019_CA.csv
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/datatoolbox/data/SANDBOX_datashelf/
+-rwxrwx---   0 root         (0) vboxsf     (999)      286 2023-06-08 10:01:09.000000 datatoolbox-0.6.1/datatoolbox/data/SANDBOX_datashelf/inventory.csv
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/datatoolbox/data/SANDBOX_datashelf/mappings/
+-rwxrwx---   0 root         (0) vboxsf     (999)    10757 2023-06-08 10:01:07.000000 datatoolbox-0.6.1/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     8466 2023-06-08 10:01:07.000000 datatoolbox-0.6.1/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)      999 2023-06-08 10:01:07.000000 datatoolbox-0.6.1/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)      161 2023-06-08 10:01:09.000000 datatoolbox-0.6.1/datatoolbox/data/SANDBOX_datashelf/sources.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)    22865 2020-10-14 14:04:18.000000 datatoolbox-0.6.1/datatoolbox/data/all.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)    14615 2020-10-14 14:04:18.000000 datatoolbox-0.6.1/datatoolbox/data/compatible1_5_unfiltered.xlsx
+-rwxrwx---   0 root         (0) vboxsf     (999)    10757 2020-04-20 12:32:09.000000 datatoolbox-0.6.1/datatoolbox/data/continent.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     8466 2021-09-15 15:48:16.000000 datatoolbox-0.6.1/datatoolbox/data/country_codes.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     1711 2022-05-25 07:15:53.000000 datatoolbox-0.6.1/datatoolbox/data/datashelf_contents.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     2923 2021-12-16 12:32:58.000000 datatoolbox-0.6.1/datatoolbox/data/external_mappings.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      178 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/data/personal_template.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      999 2019-08-14 10:00:22.000000 datatoolbox-0.6.1/datatoolbox/data/regions.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)   237054 2023-04-28 11:35:43.000000 datatoolbox-0.6.1/datatoolbox/data_readers.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    69725 2023-05-24 19:10:36.000000 datatoolbox-0.6.1/datatoolbox/data_structures.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    65332 2023-06-08 07:59:33.000000 datatoolbox-0.6.1/datatoolbox/database.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     6730 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/greenhouse_gas_database.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3542 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/init_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    21652 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/interfaces.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    11015 2023-05-23 13:04:54.000000 datatoolbox-0.6.1/datatoolbox/io_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    41818 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/mapping.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2854 2022-12-01 09:27:15.000000 datatoolbox-0.6.1/datatoolbox/naming_convention.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3305 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/patches.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2189 2023-05-12 10:35:54.000000 datatoolbox-0.6.1/datatoolbox/pint_definitions.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.6.1/datatoolbox/relations.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    26527 2023-04-05 07:52:48.000000 datatoolbox-0.6.1/datatoolbox/sets.py
+-rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.6.1/datatoolbox/storage.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1632 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/templates.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/datatoolbox/tools/
+-rwxrwx---   0 root         (0) vboxsf     (999)    16351 2021-04-19 11:31:45.000000 datatoolbox-0.6.1/datatoolbox/tools/CRF_extract_CA_2021.xlsx
+-rwxrwx---   0 root         (0) vboxsf     (999)    28022 2021-02-02 15:17:26.000000 datatoolbox-0.6.1/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN
+-rwxrwx---   0 root         (0) vboxsf     (999)    17445 2021-02-02 12:48:44.000000 datatoolbox-0.6.1/datatoolbox/tools/IEA_B2DS_4.SCEN
+-rwxrwx---   0 root         (0) vboxsf     (999)    17375 2019-12-20 11:46:57.000000 datatoolbox-0.6.1/datatoolbox/tools/WEO_2019_test.SCEN
+-rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/tools/__init__.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     4320 2022-11-17 09:58:39.000000 datatoolbox-0.6.1/datatoolbox/tools/conversion_to_v0.3.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    42729 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/tools/excel.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      370 2022-11-17 09:58:39.000000 datatoolbox-0.6.1/datatoolbox/tools/export_all.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     4441 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/tools/for_datatables.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     8132 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/tools/html.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      182 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/tools/install_support.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     7188 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/tools/kaya_idendentiy_decomposition.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     4283 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/tools/magicc6.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5931 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/tools/matplotlib.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3797 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/tools/pandas.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5533 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/tools/py_magicc_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     7869 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/tools/pyam.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      965 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/tools/renaming_DB.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    84992 2019-08-14 10:26:08.000000 datatoolbox-0.6.1/datatoolbox/tools/run_MAGICC_startup_simple.xlsx
+-rwxrwx---   0 root         (0) vboxsf     (999)     1830 2021-02-02 14:03:36.000000 datatoolbox-0.6.1/datatoolbox/tools/run_magicc6.m
+-rwxrwx---   0 root         (0) vboxsf     (999)     1044 2022-11-17 09:58:40.000000 datatoolbox-0.6.1/datatoolbox/tools/statistics.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    61174 2021-06-03 14:06:07.000000 datatoolbox-0.6.1/datatoolbox/tools/test.docx
+-rwxrwx---   0 root         (0) vboxsf     (999)     8625 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/tools/word.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     9617 2023-03-30 13:29:22.000000 datatoolbox-0.6.1/datatoolbox/tools/xarray.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/datatoolbox/tutorials/
+-rwxrwx---   0 root         (0) vboxsf     (999)     2996 2022-05-25 07:15:53.000000 datatoolbox-0.6.1/datatoolbox/tutorials/00_search_find_and_access_data.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1019 2020-10-14 14:04:18.000000 datatoolbox-0.6.1/datatoolbox/tutorials/01_emission_comparison.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2096 2022-05-25 07:15:53.000000 datatoolbox-0.6.1/datatoolbox/tutorials/02_unit_conversion.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5685 2020-10-14 14:04:18.000000 datatoolbox-0.6.1/datatoolbox/tutorials/03_intermediate_example.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1416 2020-10-14 14:04:19.000000 datatoolbox-0.6.1/datatoolbox/tutorials/04_sources.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      382 2020-10-14 14:04:19.000000 datatoolbox-0.6.1/datatoolbox/tutorials/05_plot_source_content.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      734 2020-12-22 15:09:15.000000 datatoolbox-0.6.1/datatoolbox/tutorials/06_xarray_examples.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1142 2021-05-11 13:19:29.000000 datatoolbox-0.6.1/datatoolbox/tutorials/07_renewable_share_compuation.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      793 2021-05-11 12:59:38.000000 datatoolbox-0.6.1/datatoolbox/tutorials/08_low_carbon_fuel_computation.py
+-rwxrwx---   0 root         (0) vboxsf     (999)   137631 2020-10-14 14:04:19.000000 datatoolbox-0.6.1/datatoolbox/tutorials/introduction_v1.ipynb
+-rwxrwx---   0 root         (0) vboxsf     (999)     4631 2022-03-22 14:54:50.000000 datatoolbox-0.6.1/datatoolbox/tutorials/jump_start.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      417 2023-05-12 14:15:39.000000 datatoolbox-0.6.1/datatoolbox/units.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    43883 2023-05-23 13:02:31.000000 datatoolbox-0.6.1/datatoolbox/util.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      176 2023-06-08 10:02:13.000000 datatoolbox-0.6.1/datatoolbox/version.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      746 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/datatoolbox/workflows.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/datatoolbox.egg-info/
+-rwxrwx---   0 root         (0) vboxsf     (999)     1037 2023-06-08 10:02:13.000000 datatoolbox-0.6.1/datatoolbox.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (999)     3714 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/datatoolbox.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)        1 2023-06-08 10:02:13.000000 datatoolbox-0.6.1/datatoolbox.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)      149 2023-06-08 10:02:13.000000 datatoolbox-0.6.1/datatoolbox.egg-info/requires.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)       12 2023-06-08 10:02:13.000000 datatoolbox-0.6.1/datatoolbox.egg-info/top_level.txt
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/doc/
+-rwxrwx---   0 root         (0) vboxsf     (999)     7755 2020-10-14 14:04:19.000000 datatoolbox-0.6.1/doc/Makefile
+-rwxrwx---   0 root         (0) vboxsf     (999)     9684 2020-12-22 15:09:15.000000 datatoolbox-0.6.1/doc/conf.py
+-rwxrwx---   0 root         (0) vboxsf     (999)       79 2021-01-05 10:54:01.000000 datatoolbox-0.6.1/doc/core.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      149 2020-12-22 15:09:15.000000 datatoolbox-0.6.1/doc/data_structures.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      122 2021-01-11 16:19:59.000000 datatoolbox-0.6.1/doc/database.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       91 2021-01-11 16:18:53.000000 datatoolbox-0.6.1/doc/database_database.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      130 2021-01-11 16:21:50.000000 datatoolbox-0.6.1/doc/database_gitrepomanager.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       93 2021-01-11 16:03:03.000000 datatoolbox-0.6.1/doc/excel.rst
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/doc/figures/
+-rwxrwx---   0 root         (0) vboxsf     (999)    21579 2020-11-09 13:08:35.000000 datatoolbox-0.6.1/doc/figures/ID_meta_data.svg
+-rwxrwx---   0 root         (0) vboxsf     (999)    67463 2021-05-17 15:08:58.000000 datatoolbox-0.6.1/doc/figures/config_input.png
+-rwxrwx---   0 root         (0) vboxsf     (999)     7159 2023-06-08 08:25:46.000000 datatoolbox-0.6.1/doc/first_steps.md
+-rwxrwx---   0 root         (0) vboxsf     (999)      100 2020-12-22 15:09:15.000000 datatoolbox-0.6.1/doc/foo.rst_template
+-rwxrwx---   0 root         (0) vboxsf     (999)       77 2020-12-22 15:09:15.000000 datatoolbox-0.6.1/doc/help.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      463 2021-01-11 16:06:28.000000 datatoolbox-0.6.1/doc/index.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)     1655 2023-06-08 08:19:25.000000 datatoolbox-0.6.1/doc/installation.md
+-rwxrwx---   0 root         (0) vboxsf     (999)     1080 2020-12-22 15:09:15.000000 datatoolbox-0.6.1/doc/license.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)     7353 2020-10-14 14:04:19.000000 datatoolbox-0.6.1/doc/make.bat
+-rwxrwx---   0 root         (0) vboxsf     (999)      103 2021-01-11 16:09:22.000000 datatoolbox-0.6.1/doc/matplotlib.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:10:43.000000 datatoolbox-0.6.1/doc/pandas.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      133 2021-01-11 16:20:57.000000 datatoolbox-0.6.1/doc/tools.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:09:13.000000 datatoolbox-0.6.1/doc/xarray.rst
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/documentation/
+-rwxrwx---   0 root         (0) vboxsf     (999)     7761 2020-12-22 15:09:15.000000 datatoolbox-0.6.1/documentation/Datatoolbox - First steps.md
+-rwxrwx---   0 root         (0) vboxsf     (999)      385 2023-05-12 12:15:15.000000 datatoolbox-0.6.1/environment.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)      418 2020-10-14 14:04:19.000000 datatoolbox-0.6.1/make_proj.sh
+-rwxrwx---   0 root         (0) vboxsf     (999)      558 2021-01-12 15:45:18.000000 datatoolbox-0.6.1/readthedocs.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)      215 2022-10-19 13:17:33.000000 datatoolbox-0.6.1/requirements.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)       38 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/setup.cfg
+-rwxrwx---   0 root         (0) vboxsf     (999)     1839 2023-05-03 11:16:28.000000 datatoolbox-0.6.1/setup.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-06-08 10:02:14.000000 datatoolbox-0.6.1/tests/
+-rwxrwx---   0 root         (0) vboxsf     (999)     7292 2022-12-19 11:29:58.000000 datatoolbox-0.6.1/tests/test_calculations.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      696 2022-11-18 16:16:07.000000 datatoolbox-0.6.1/tests/test_converters.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2836 2022-11-21 11:08:31.000000 datatoolbox-0.6.1/tests/test_database.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1640 2023-03-30 13:32:13.000000 datatoolbox-0.6.1/tests/test_dataset.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     7741 2022-05-25 07:15:53.000000 datatoolbox-0.6.1/tests/test_datatable.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1063 2022-11-16 11:59:46.000000 datatoolbox-0.6.1/tests/test_io.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-22 09:54:34.000000 datatoolbox-0.6.1/tests/test_linked_functions.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1563 2023-05-04 07:49:24.000000 datatoolbox-0.6.1/tests/test_pyam.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3570 2022-05-25 07:15:53.000000 datatoolbox-0.6.1/tests/test_tableset.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2610 2022-05-25 07:15:53.000000 datatoolbox-0.6.1/tests/test_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1832 2023-05-23 12:58:33.000000 datatoolbox-0.6.1/tests/test_units.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      870 2020-10-14 14:04:19.000000 datatoolbox-0.6.1/tests/test_utilities.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2437 2022-10-19 13:17:33.000000 datatoolbox-0.6.1/tests/test_xarray.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2959 2022-05-25 07:15:53.000000 datatoolbox-0.6.1/tests/util_for_testing.py
```

### Comparing `datatoolbox-0.5.8/.gitlab-ci.yml` & `datatoolbox-0.6.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/.travis.yml` & `datatoolbox-0.6.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/LICENSE` & `datatoolbox-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/PKG-INFO` & `datatoolbox-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatoolbox
-Version: 0.5.8
+Version: 0.6.1
 Summary: The Python Data Toolbox
 Home-page: https://gitlab.com/climateanalytics/datatoolbox
 Author: Andreas Geiges
 Author-email: a.geiges@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `datatoolbox-0.5.8/README.md` & `datatoolbox-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/appveyor.yml` & `datatoolbox-0.6.1/appveyor.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/ci/appveyor/install.ps1` & `datatoolbox-0.6.1/ci/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/ci/appveyor/run_with_env.cmd` & `datatoolbox-0.6.1/ci/appveyor/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/__init__.py` & `datatoolbox-0.6.1/datatoolbox/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     remove_source = core.DB.removeSource
     push_source_to_remote = core.DB.gitManager.push_to_remote_datashelf
     pull_source_from_remote = core.DB.pull_update_from_remote
 
     #show available remote data sources
     remote_sourceInfo = core.DB.remote_sourceInfo
     available_remote_data_updates = core.DB.gitManager.available_remote_data_updates
-    
+    test_ssh_remote_connection = core.DB.gitManager.test_ssh_remote_connection
 #%% TOOLS
 # Tools related to packages
 import datatoolbox.tools as tools
 from .tools import pandas as pd
 from .tools import matplotlib as plt
 from .tools import xarray as xr
 from .tools import excel as xl
```

### Comparing `datatoolbox-0.5.8/datatoolbox/admin.py` & `datatoolbox-0.6.1/datatoolbox/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,14 +301,16 @@
     fin = open(os.path.join(modulePath, 'data', 'personal_template.py'), 'r')
 
     fout = open(os.path.join(config.CONFIG_DIR, 'personal.py'), 'w')
     
     if (userName is None) or (file_path_variable is None):
         userName, file_path_variable = _open_dialog_for_user()
     
+    if file_path_variable.startswith('..'):
+        raise(Exception('Please use an absolute path to the datashelf directory.'))
     for line in fin.readlines():
         outLine = line.replace('XX', userName).replace('/PPP/PPP', file_path_variable)
         fout.write(outLine)
     fin.close()
     fout.close()
```

### Comparing `datatoolbox-0.5.8/datatoolbox/config.py` & `datatoolbox-0.6.1/datatoolbox/config.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/converters.py` & `datatoolbox-0.6.1/datatoolbox/converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
         
         table = dt.Datatable.from_multi_indexed_dataframe(sub_df)
         tables.append(table)
     return tables
     #%%
 
 def datatables_to_multi_index_df(tables,
-                                 exclude_meta =['ID', 'creator', 'source_name','source_year'],
+                                 exclude_meta =['ID', 'creator', 'source_name','source_year', 'modified'],
                                  use_index_names = None):
     
     dfs = list()
     for table in tables:
         dfs.append(table.to_multi_index_dataframe(exclude_meta=exclude_meta,
                                                   use_index_names=use_index_names))
     index_names = set([x.index.names for x in dfs])
```

### Comparing `datatoolbox-0.5.8/datatoolbox/core.py` & `datatoolbox-0.6.1/datatoolbox/core.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/data/GHG_alternative_naming.pkl` & `datatoolbox-0.6.1/datatoolbox/data/GHG_alternative_naming.pkl`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/data/GHG_properties_2019_CA.csv` & `datatoolbox-0.6.1/datatoolbox/data/GHG_properties_2019_CA.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv` & `datatoolbox-0.6.1/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv` & `datatoolbox-0.6.1/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv` & `datatoolbox-0.6.1/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/data/all.csv` & `datatoolbox-0.6.1/datatoolbox/data/all.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/data/compatible1_5_unfiltered.xlsx` & `datatoolbox-0.6.1/datatoolbox/data/compatible1_5_unfiltered.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/data/continent.csv` & `datatoolbox-0.6.1/datatoolbox/data/continent.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/data/country_codes.csv` & `datatoolbox-0.6.1/datatoolbox/data/country_codes.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/data/datashelf_contents.csv` & `datatoolbox-0.6.1/datatoolbox/data/datashelf_contents.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/data/external_mappings.py` & `datatoolbox-0.6.1/datatoolbox/data/external_mappings.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/data/regions.csv` & `datatoolbox-0.6.1/datatoolbox/data/regions.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/data_readers.py` & `datatoolbox-0.6.1/datatoolbox/data_readers.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/data_structures.py` & `datatoolbox-0.6.1/datatoolbox/data_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -735,17 +735,17 @@
         from pandas_indexing import assignlevel
         
         if use_index_names is None:
             meta_for_index = {x: self.meta[x] for x in sorted(self.meta.keys()) if not x in exclude_meta}
         else:
             meta_for_index = {x: self.meta[x] for x in sorted(use_index_names) if x!='region' }
         
-        return assignlevel(self, **meta_for_index)
+        return assignlevel(self.copy(), **meta_for_index)
 
-    def convert(self, newUnit, context=None):
+    def convert(self, newUnit, context=None, suffix_dict=dict(), **new_meta):
         """
         Convert datatable to different unit and returns converted
         datatable.
 
         Parameters
         ----------
         newUnit : str
@@ -756,25 +756,32 @@
         Returns
         -------
         datatable
             Datatable converted in the new unit.
 
         """
         if self.meta['unit'] == newUnit:
+            for key, suffix in suffix_dict.items():
+                self.meta[key] =self.meta[key] +suffix
+            self.meta.update(new_meta)
             return self
 
         dfNew = self.copy()
         #        oldUnit = core.getUnit(self.meta['unit'])
         #        factor = (1* oldUnit).to(newUnit).m
 
         factor = core.conversionFactor(self.meta['unit'], newUnit, context)
 
         dfNew.loc[:] = self.values * factor
         dfNew.meta['unit'] = newUnit
         dfNew.meta['modified'] = core.get_time_string()
+        for key, suffix in suffix_dict.items():
+            dfNew.meta[key] =dfNew.meta[key] +suffix
+        dfNew.meta.update(new_meta)
+        # dfNew._update_meta()
         return dfNew
 
 
     def interpolate(self, method="linear", add_missing_years=False):
         """
         Interpoltate missing data between year with the option to add
         missing years in the columns.
```

### Comparing `datatoolbox-0.5.8/datatoolbox/database.py` & `datatoolbox-0.6.1/datatoolbox/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1171,15 +1171,15 @@
         self.gitManager.clone_source_from_remote(remoteName, repoPath)
 
         sourceInventory = pd.read_csv(
             os.path.join(repoPath, "source_inventory.csv"),
             index_col=0,
             dtype={"source_year": str},
         )
-        self.inventory = self.inventory.append(sourceInventory, verify_integrity=True)
+        self.inventory = pd.concat([self.inventory, sourceInventory], verify_integrity=True)
         self._gitCommit("imported " + remoteName)
 
     def exportSourceToRemote(self, sourceID):
         """
         This function exports a new local dataset to the defind remote database.
 
         Input is a local sourceID as a str.
@@ -1781,38 +1781,60 @@
         # if repoName not in rem_sources.index:
         remote_repo.remotes.origin.push(progress=TqdmProgressPrinter())
 
         self[repoName].remotes.origin.push(progress=TqdmProgressPrinter())
 
         self[repoName].remotes.origin.push(progress=TqdmProgressPrinter(), tags=True)
 
+    def test_ssh_remote_connection(self):
+        host = config.DATASHELF_REMOTE.split(':')[0]
+        print(f'Testing connection to host {host}')
+        cmd = f"ssh -T {host}"
+        import subprocess
+        retcode = subprocess.call(cmd,shell=True)
+        if retcode==0:
+            print('Successfully connected')
+        else:
+            print(f'Connection failed with exit code {retcode}')
     def clone_source_from_remote(self, repoName, repoPath):
         """
         Function to clone a remote git repository as a local copy.
 
         Input
         -----
         repoName : str - valid repository in the remove database
         repoPath : str - path of the repository
         """
 
         self._pull_remote_sources()
         try:
-            print("Try cloning source via ssh")
+            print("Try cloning source via ssh...", end='')
             url = config.DATASHELF_REMOTE + repoName + ".git"
             repo = git.Repo.clone_from(
                 url=url, to_path=repoPath, progress=TqdmProgressPrinter()
             )
         except:
-            print("Failed... Try Cloning source via https:")
-            url = config.DATASHELF_REMOTE_HTTPS + repoName + ".git"
-            repo = git.Repo.clone_from(
-                url=url, to_path=repoPath, progress=TqdmProgressPrinter()
-            )
-
+            print('failed.')
+            try:
+                
+                print("Try Cloning source via https...", end='')
+                url = config.DATASHELF_REMOTE_HTTPS + repoName + ".git"
+                repo = git.Repo.clone_from(
+                    url=url, to_path=repoPath, progress=TqdmProgressPrinter()
+                )
+            except Exception:
+                print('failed.')
+                if config.DEBUG:
+                    print(traceback.format_exc())
+                    print("Failed to import source {}".format(repoName))
+                raise(Exception(f"""Both SSH and HTTPs import failed. Check your connection, password or if requrested data exists on remote.
+                Consider the following options:                
+                    1) Does "{repoName}" exists in {config.DATASHELF_REMOTE_HTTPS}
+                    2) Check your ssh connection with: dt.test_ssh_remote_connection())
+                    """))
         self.repositories[repoName] = repo
 
         # Update source file
         sourceMetaDict = util.csv_to_dict(os.path.join(repoPath, "meta.csv"))
         sourceMetaDict["git_commit_hash"] = repo.commit().hexsha
         tag = self.get_tag_of_source(repoName)
         sourceMetaDict["tag"] = tag
```

### Comparing `datatoolbox-0.5.8/datatoolbox/greenhouse_gas_database.py` & `datatoolbox-0.6.1/datatoolbox/greenhouse_gas_database.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/init_tools.py` & `datatoolbox-0.6.1/datatoolbox/init_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/interfaces.py` & `datatoolbox-0.6.1/datatoolbox/interfaces.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/io_tools.py` & `datatoolbox-0.6.1/datatoolbox/io_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/mapping.py` & `datatoolbox-0.6.1/datatoolbox/mapping.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/naming_convention.py` & `datatoolbox-0.6.1/datatoolbox/naming_convention.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/patches.py` & `datatoolbox-0.6.1/datatoolbox/patches.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/pint_definitions.txt` & `datatoolbox-0.6.1/datatoolbox/pint_definitions.txt`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/sets.py` & `datatoolbox-0.6.1/datatoolbox/sets.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/templates.py` & `datatoolbox-0.6.1/datatoolbox/templates.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/CRF_extract_CA_2021.xlsx` & `datatoolbox-0.6.1/datatoolbox/tools/CRF_extract_CA_2021.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN` & `datatoolbox-0.6.1/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/IEA_B2DS_4.SCEN` & `datatoolbox-0.6.1/datatoolbox/tools/IEA_B2DS_4.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/WEO_2019_test.SCEN` & `datatoolbox-0.6.1/datatoolbox/tools/WEO_2019_test.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/conversion_to_v0.3.py` & `datatoolbox-0.6.1/datatoolbox/tools/conversion_to_v0.3.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/excel.py` & `datatoolbox-0.6.1/datatoolbox/tools/excel.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/for_datatables.py` & `datatoolbox-0.6.1/datatoolbox/tools/for_datatables.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/html.py` & `datatoolbox-0.6.1/datatoolbox/tools/html.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/kaya_idendentiy_decomposition.py` & `datatoolbox-0.6.1/datatoolbox/tools/kaya_idendentiy_decomposition.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/magicc6.py` & `datatoolbox-0.6.1/datatoolbox/tools/magicc6.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/matplotlib.py` & `datatoolbox-0.6.1/datatoolbox/tools/matplotlib.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/pandas.py` & `datatoolbox-0.6.1/datatoolbox/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/py_magicc_tools.py` & `datatoolbox-0.6.1/datatoolbox/tools/py_magicc_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/pyam.py` & `datatoolbox-0.6.1/datatoolbox/tools/pyam.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/renaming_DB.py` & `datatoolbox-0.6.1/datatoolbox/tools/renaming_DB.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/run_MAGICC_startup_simple.xlsx` & `datatoolbox-0.6.1/datatoolbox/tools/run_MAGICC_startup_simple.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/run_magicc6.m` & `datatoolbox-0.6.1/datatoolbox/tools/run_magicc6.m`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/statistics.py` & `datatoolbox-0.6.1/datatoolbox/tools/statistics.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/test.docx` & `datatoolbox-0.6.1/datatoolbox/tools/test.docx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/word.py` & `datatoolbox-0.6.1/datatoolbox/tools/word.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tools/xarray.py` & `datatoolbox-0.6.1/datatoolbox/tools/xarray.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tutorials/00_search_find_and_access_data.py` & `datatoolbox-0.6.1/datatoolbox/tutorials/00_search_find_and_access_data.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tutorials/01_emission_comparison.py` & `datatoolbox-0.6.1/datatoolbox/tutorials/01_emission_comparison.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tutorials/02_unit_conversion.py` & `datatoolbox-0.6.1/datatoolbox/tutorials/02_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tutorials/03_intermediate_example.py` & `datatoolbox-0.6.1/datatoolbox/tutorials/03_intermediate_example.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tutorials/04_sources.py` & `datatoolbox-0.6.1/datatoolbox/tutorials/04_sources.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tutorials/06_xarray_examples.py` & `datatoolbox-0.6.1/datatoolbox/tutorials/06_xarray_examples.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tutorials/07_renewable_share_compuation.py` & `datatoolbox-0.6.1/datatoolbox/tutorials/07_renewable_share_compuation.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tutorials/08_low_carbon_fuel_computation.py` & `datatoolbox-0.6.1/datatoolbox/tutorials/08_low_carbon_fuel_computation.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tutorials/introduction_v1.ipynb` & `datatoolbox-0.6.1/datatoolbox/tutorials/introduction_v1.ipynb`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/tutorials/jump_start.py` & `datatoolbox-0.6.1/datatoolbox/tutorials/jump_start.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/util.py` & `datatoolbox-0.6.1/datatoolbox/util.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox/workflows.py` & `datatoolbox-0.6.1/datatoolbox/workflows.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/datatoolbox.egg-info/PKG-INFO` & `datatoolbox-0.6.1/datatoolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatoolbox
-Version: 0.5.8
+Version: 0.6.1
 Summary: The Python Data Toolbox
 Home-page: https://gitlab.com/climateanalytics/datatoolbox
 Author: Andreas Geiges
 Author-email: a.geiges@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `datatoolbox-0.5.8/datatoolbox.egg-info/SOURCES.txt` & `datatoolbox-0.6.1/datatoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/doc/Makefile` & `datatoolbox-0.6.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/doc/conf.py` & `datatoolbox-0.6.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/doc/figures/ID_meta_data.svg` & `datatoolbox-0.6.1/doc/figures/ID_meta_data.svg`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/doc/figures/config_input.png` & `datatoolbox-0.6.1/doc/figures/config_input.png`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/doc/first_steps.md` & `datatoolbox-0.6.1/doc/first_steps.md`

 * *Files 0% similar despite different names*

```diff
@@ -71,19 +71,19 @@
 
 
 ## Find tables
 
 Datatables that contain the search string
 
 ```
-dt.find(variable ='', entity='', category='', scenario ='', model='' source='')
+dt.findp(variable ='', entity='', category='', scenario ='', model='' source='')
 ```
 #%% List all data sources
 ```
-sources = list(dt.find().source.unique())
+sources = list(dt.findp().source.unique())
 sources.sort()
 print(sources)
 ```
 
 #%% List all scenarios within a source
 ```
 res = dt.find(source='PRIMAP_2019')
```

### Comparing `datatoolbox-0.5.8/doc/installation.md` & `datatoolbox-0.6.1/doc/installation.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,15 @@
 
 #### Software installation outside python
 ```bash
 sudo apt install git
 ```
 #### Datatoolbox python dependencies
 
-```bash
-pip install pint==0.9
-pip install pyam-iamc==0.3.0
-pip install pycountry
-pip install datatoolbox --upgrade
-
-```
+See enviroment file.
 
 
 ## Set up datatoolbox and connect to a database
 
 
 
 First time you import datatoolbox, you need to set up the local database and link it to datatoolbox. Otherwise, a simple SANDBOX data structure is loaded for playing around.
```

### Comparing `datatoolbox-0.5.8/doc/license.rst` & `datatoolbox-0.6.1/doc/license.rst`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/doc/make.bat` & `datatoolbox-0.6.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/documentation/Datatoolbox - First steps.md` & `datatoolbox-0.6.1/documentation/Datatoolbox - First steps.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/readthedocs.yml` & `datatoolbox-0.6.1/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/setup.py` & `datatoolbox-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/tests/test_calculations.py` & `datatoolbox-0.6.1/tests/test_calculations.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/tests/test_converters.py` & `datatoolbox-0.6.1/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/tests/test_database.py` & `datatoolbox-0.6.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/tests/test_dataset.py` & `datatoolbox-0.6.1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/tests/test_datatable.py` & `datatoolbox-0.6.1/tests/test_datatable.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/tests/test_io.py` & `datatoolbox-0.6.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/tests/test_pyam.py` & `datatoolbox-0.6.1/tests/test_pyam.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/tests/test_tableset.py` & `datatoolbox-0.6.1/tests/test_tableset.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/tests/test_tools.py` & `datatoolbox-0.6.1/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/tests/test_units.py` & `datatoolbox-0.6.1/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/tests/test_utilities.py` & `datatoolbox-0.6.1/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/tests/test_xarray.py` & `datatoolbox-0.6.1/tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.8/tests/util_for_testing.py` & `datatoolbox-0.6.1/tests/util_for_testing.py`

 * *Files identical despite different names*

