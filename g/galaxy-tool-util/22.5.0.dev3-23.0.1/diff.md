# Comparing `tmp/galaxy-tool-util-22.5.0.dev3.tar.gz` & `tmp/galaxy-tool-util-23.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-tool-util-22.5.0.dev3.tar", last modified: Mon Mar  6 18:36:14 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/tool_util/dist/.tmp-_xnk55yw/galaxy-tool-util-23.0.1.tar", last modified: Thu Jun  8 17:40:47 2023, max compression
```

## Comparing `galaxy-tool-util-22.5.0.dev3.tar` & `galaxy-tool-util-23.0.1.tar`

### file list

```diff
@@ -1,173 +1,178 @@
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.765797 galaxy-tool-util-22.5.0.dev3/
--rw-r--r--   0 mvandenb   (501) staff       (20)     2016 2023-02-17 09:03:53.000000 galaxy-tool-util-22.5.0.dev3/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)    11109 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/LICENSE
--rw-r--r--   0 mvandenb   (501) staff       (20)      320 2023-03-06 18:30:39.000000 galaxy-tool-util-22.5.0.dev3/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) staff       (20)     3469 2023-03-06 18:36:14.765906 galaxy-tool-util-22.5.0.dev3/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      329 2023-03-06 18:30:39.000000 galaxy-tool-util-22.5.0.dev3/README.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)       89 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.695498 galaxy-tool-util-22.5.0.dev3/galaxy/
--rw-r--r--   0 mvandenb   (501) staff       (20)       91 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.699958 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:10.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.701978 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/biotools/
--rw-r--r--   0 mvandenb   (501) staff       (20)      307 2022-11-16 11:10:40.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/biotools/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1683 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/biotools/interface.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3570 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/biotools/source.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.703012 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/client/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-11-16 11:10:40.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/client/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    13735 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/client/staging.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.707828 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/
--rw-r--r--   0 mvandenb   (501) staff       (20)      515 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3956 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/cwltool_deps.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    47654 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/parser.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    18622 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/representation.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      939 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/runnable.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     9509 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/runtime_actions.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3842 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/schema.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    24533 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/util.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.714981 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/
--rw-r--r--   0 mvandenb   (501) staff       (20)    20457 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/__init__.py
--rwxr-xr-x   0 mvandenb   (501) staff       (20)    19465 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/brew_exts.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1124 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/brew_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      373 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/commands.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2931 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/conda_compat.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    22519 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/conda_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    18656 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/container_classes.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.716624 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/container_resolvers/
--rw-r--r--   0 mvandenb   (501) staff       (20)     2464 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/container_resolvers/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     9705 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/container_resolvers/explicit.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    26721 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/container_resolvers/mulled.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2329 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/container_volumes.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    15999 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/containers.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     6859 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/dependencies.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     7041 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/docker_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2675 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/dockerfiles.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2486 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/installable.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.723767 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:10.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      422 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/_cli.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    10920 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/get_tests.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3985 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/invfile.lua
--rw-r--r--   0 mvandenb   (501) staff       (20)    20641 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_build.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4090 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_build_channel.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3797 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_build_files.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1588 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_build_tool.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      887 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_hash.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5062 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_list.py
--rwxr-xr-x   0 mvandenb   (501) staff       (20)    16506 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_search.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     9989 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    16500 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    12174 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/requirements.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.728719 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/
--rw-r--r--   0 mvandenb   (501) staff       (20)    11100 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5378 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    19966 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/conda.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      702 2022-03-24 19:47:10.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)     5389 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/galaxy_packages.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2033 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/homebrew.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     7971 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/lmod.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     8887 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/modules.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2748 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/resolver_mixins.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3571 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/tool_shed_packages.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     7542 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3221 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/singularity_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    17495 2022-12-08 15:40:33.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/views.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2531 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/edam_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      900 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/fetcher.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    12035 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/lint.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.734146 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/
--rw-r--r--   0 mvandenb   (501) staff       (20)       64 2022-03-24 19:47:10.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      333 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1565 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/citations.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1941 2022-11-16 11:10:40.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/command.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1777 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/cwl.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3541 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/general.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1696 2023-02-17 09:03:52.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/help.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    22625 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/inputs.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4970 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/outputs.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2604 2022-12-08 15:40:33.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/stdio.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     9997 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/tests.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1729 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/xml_order.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      391 2022-03-24 19:47:10.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/loader.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     9920 2023-02-17 09:03:52.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/loader_directory.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.735502 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/locations/
--rw-r--r--   0 mvandenb   (501) staff       (20)      697 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/locations/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2392 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/locations/dockstore.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      249 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/locations/file.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      483 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/locations/http.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.738594 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/ontologies/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/ontologies/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      134 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/ontologies/biotools_mappings.tsv
--rw-r--r--   0 mvandenb   (501) staff       (20)       52 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/ontologies/edam_operation_mappings.tsv
--rw-r--r--   0 mvandenb   (501) staff       (20)       27 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/ontologies/edam_topic_mappings.tsv
--rw-r--r--   0 mvandenb   (501) staff       (20)     3651 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/ontologies/ontology_data.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     8618 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/output_checker.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.743706 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/
--rw-r--r--   0 mvandenb   (501) staff       (20)      480 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5721 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/cwl.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4235 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/factory.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    17913 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/interface.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    24927 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/output_actions.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5858 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/output_collection_def.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    14919 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/output_objects.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4171 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/stdio.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      645 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    48851 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/xml.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    11782 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/yaml.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     9392 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/provided_metadata.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.747845 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/
--rw-r--r--   0 mvandenb   (501) staff       (20)      356 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    65270 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/base.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.748887 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/filters/
--rw-r--r--   0 mvandenb   (501) staff       (20)     4454 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/filters/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4726 2022-11-16 11:10:40.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/filters/examples.py.sample
--rw-r--r--   0 mvandenb   (501) staff       (20)     6939 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/integrated_panel.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.750211 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/lineages/
--rw-r--r--   0 mvandenb   (501) staff       (20)      108 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/lineages/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2140 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/lineages/factory.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2751 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/lineages/interface.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     8634 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/panel.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4743 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/parser.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2548 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/tags.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.752842 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/views/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-11-16 11:10:40.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/views/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3741 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/views/definitions.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     7030 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/views/edam.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2546 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/views/interface.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1685 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/views/sources.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     9182 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/views/static.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     6880 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/watcher.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.753623 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/unittest_utils/
--rw-r--r--   0 mvandenb   (501) staff       (20)      320 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/unittest_utils/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      417 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/unittest_utils/sample_data.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.756209 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/
--rw-r--r--   0 mvandenb   (501) staff       (20)    18158 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.759160 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/
--rw-r--r--   0 mvandenb   (501) staff       (20)     3965 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2578 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3503 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/archive.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1387 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/hdf5.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      662 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/size.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1201 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/tabular.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4927 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/text.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4860 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/xml.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    67013 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/interactor.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    21969 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/script.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      850 2022-11-16 11:10:40.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/test_config.sample.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)     3889 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/test_data.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1430 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/wait.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.761419 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/xsd/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1131 2022-03-24 19:47:10.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/xsd/LICENSE
--rw-r--r--   0 mvandenb   (501) staff       (20)     1079 2022-03-24 19:47:10.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/xsd/README.md
--rw-r--r--   0 mvandenb   (501) staff       (20)      694 2022-03-24 19:47:10.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/xsd/galaxy.jxb
--rw-r--r--   0 mvandenb   (501) staff       (20)   314483 2023-03-06 18:30:38.000000 galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/xsd/galaxy.xsd
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:36:14.765442 galaxy-tool-util-22.5.0.dev3/galaxy_tool_util.egg-info/
--rw-r--r--   0 mvandenb   (501) staff       (20)     3469 2023-03-06 18:36:14.000000 galaxy-tool-util-22.5.0.dev3/galaxy_tool_util.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)     5708 2023-03-06 18:36:14.000000 galaxy-tool-util-22.5.0.dev3/galaxy_tool_util.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2023-03-06 18:36:14.000000 galaxy-tool-util-22.5.0.dev3/galaxy_tool_util.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)      653 2023-03-06 18:36:14.000000 galaxy-tool-util-22.5.0.dev3/galaxy_tool_util.egg-info/entry_points.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)      203 2023-03-06 18:36:14.000000 galaxy-tool-util-22.5.0.dev3/galaxy_tool_util.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2023-03-06 18:36:14.000000 galaxy-tool-util-22.5.0.dev3/galaxy_tool_util.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       81 2022-12-08 11:44:37.000000 galaxy-tool-util-22.5.0.dev3/pyproject.toml
--rw-r--r--   0 mvandenb   (501) staff       (20)     2064 2023-03-06 18:36:14.766458 galaxy-tool-util-22.5.0.dev3/setup.cfg
--rw-r--r--   0 mvandenb   (501) staff       (20)       26 2023-03-06 18:30:39.000000 galaxy-tool-util-22.5.0.dev3/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-08 17:37:03.000000 galaxy-tool-util-23.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/biotools/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/biotools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/biotools/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/biotools/source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14527 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/client/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/cwltool_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45995 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18625 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/runtime_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25744 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    57337 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/data/_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19572 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/brew_exts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/brew_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/conda_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/conda_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18484 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/container_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/container_resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/container_resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/container_resolvers/explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26783 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/container_resolvers/mulled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/container_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16061 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/docker_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/dockerfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/installable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/get_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/invfile.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_build_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_build_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_build_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15814 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16359 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12361 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)    11099 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/galaxy_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/homebrew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/lmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/resolver_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/tool_shed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/singularity_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17495 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/deps/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/edam_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/linters/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/linters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/linters/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/linters/citations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/linters/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/linters/cwl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/linters/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/linters/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23859 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/linters/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/linters/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/linters/stdio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/linters/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/linters/xml_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/loader_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/locations/dockstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/locations/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/locations/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/ontologies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/ontologies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53080 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/ontologies/biotools_mappings.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/ontologies/edam_operation_mappings.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/ontologies/edam_topic_mappings.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/ontologies/ontology_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/output_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/parser/cwl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/parser/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18998 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/parser/output_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/parser/output_collection_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15930 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/parser/output_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/parser/stdio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/parser/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49096 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/parser/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12357 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/parser/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/provided_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65911 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/filters/examples.py.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/integrated_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/lineages/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/lineages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/lineages/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/lineages/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/views/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/views/edam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/views/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/views/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/views/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/unittest_utils/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/unittest_utils/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/
+-rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71060 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22759 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/test_config.sample.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/verify/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/xsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/xsd/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/xsd/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/xsd/galaxy.jxb
+-rw-r--r--   0 runner    (1001) docker     (123)   319184 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/galaxy/tool_util/xsd/galaxy.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy_tool_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy_tool_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy_tool_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy_tool_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy_tool_util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy_tool_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/galaxy_tool_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-08 17:40:47.000000 galaxy-tool-util-23.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 17:37:04.000000 galaxy-tool-util-23.0.1/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `galaxy-tool-util-22.5.0.dev3/LICENSE` & `galaxy-tool-util-23.0.1/LICENSE`

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

### Comparing `galaxy-tool-util-22.5.0.dev3/PKG-INFO` & `galaxy-tool-util-23.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-tool-util
-Version: 22.5.0.dev3
+Version: 23.0.1
 Summary: Galaxy tool and tool dependency utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: cwl
 Provides-Extra: mulled
@@ -34,123 +35,145 @@
 
 
 Overview
 --------
 
 The Galaxy_ tool utilities.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy/tree/dev/packages/tool_util
 
 .. _Galaxy: http://galaxyproject.org/
 
 History
 -------
 
 .. to_doc
 
 -------------------
-22.5.0.dev0
+23.0.1 (2023-06-08)
 -------------------
 
 
+=========
+Bug fixes
+=========
+
+* Fix assertion linting to not fail on byte suffixes by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15873 <https://github.com/galaxyproject/galaxy/pull/15873>`_
+* Fix ``get_test_from_anaconda()`` and ``base_image_for_targets()`` functions by `@nsoranzo <https://github.com/nsoranzo>`_ in `#16125 <https://github.com/galaxyproject/galaxy/pull/16125>`_
+* Fix test search for mulled container hashes by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16170 <https://github.com/galaxyproject/galaxy/pull/16170>`_
+
+============
+Enhancements
+============
+
+* Allow setting auto_decompress property in staging interface by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16014 <https://github.com/galaxyproject/galaxy/pull/16014>`_
 
 -------------------
 22.1.5 (2022-11-14)
 -------------------
 
 * Set test status to success on expected failure
 
+-------------------
 22.1.4 (2022-10-28)
 -------------------
 
 * Add missing unittest_utils package to galaxy-tool-util
 
+-------------------
 22.1.3 (2022-10-27)
 -------------------
 
 * Pin minimum pyopenssl version when installing Conda
 * Add ``--strict-channel-priority`` to conda create/install commands if using conda >=4.7.5
 
+-------------------
 22.1.2 (2022-08-29)
 -------------------
 
 * Fix lint context error level
 * Pin galaxy-util to >= 22.1
 * Fix biocontainer resolution without beaker cache
 
+-------------------
 22.1.1 (2022-08-22)
---------------------
+-------------------
 
 * First release from the 22.01 branch of Galaxy
 
----------------------
+-------------------
 21.9.2 (2021-11-23)
----------------------
+-------------------
 
 * Fix linting of ``multiple="true"`` select inputs.
 
----------------------
+-------------------
 21.9.1 (2021-11-03)
----------------------
+-------------------
 
 * Fix tool linting.
 
----------------------
+-------------------
 21.9.0 (2021-11-03)
----------------------
+-------------------
 
 * First release from the 21.09 branch of Galaxy.
 
----------------------
+-------------------
 21.1.2 (2021-06-23)
----------------------
+-------------------
 
 
 
----------------------
+-------------------
 21.1.1 (2021-05-21)
----------------------
+-------------------
 
 
 
----------------------
+-------------------
 21.1.0 (2021-03-19)
----------------------
+-------------------
 
 * First release from the 21.01 branch of Galaxy.
 
----------------------
+-------------------
 20.9.1 (2020-10-28)
----------------------
+-------------------
 
 * Bugfixes to work around & annotate expected tool test failures.
 
----------------------
-20.9.0.dev2
----------------------
+-------------------
+20.9.0 (2020-10-28)
+-------------------
+
+* First release from the 20.09 branch of Galaxy.
+
+------------------------
+20.9.0.dev2 (2020-08-02)
+------------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.05 branch of Galaxy.
 
----------------------
+-------------------
 20.1.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.01 branch of Galaxy.
 
----------------------
+-------------------
 19.9.1 (2019-12-28)
----------------------
+-------------------
 
 * Fix declared dependency problem with package.
 
----------------------
+-------------------
 19.9.0 (2019-12-16)
----------------------
+-------------------
 
 * Initial import from dev branch of Galaxy during 19.09 development cycle.
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/biotools/interface.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/biotools/interface.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/biotools/source.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/biotools/source.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/client/staging.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/client/staging.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,99 +3,113 @@
 Implement as a connector to serve a bridge between galactic_job_json
 utility and a Galaxy API library.
 """
 import abc
 import json
 import logging
 import os
-import warnings
+from typing import (
+    Any,
+    BinaryIO,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    TYPE_CHECKING,
+)
 
 import yaml
+from typing_extensions import Literal
 
 from galaxy.tool_util.cwl.util import (
     DirectoryUploadTarget,
     FileLiteralTarget,
     FileUploadTarget,
     galactic_job_json,
+    ObjectUploadTarget,
     path_or_uri_to_uri,
+    UploadTarget,
 )
 
+if TYPE_CHECKING:
+    from galaxy_test.base.api import ApiTestInteractor
+
 log = logging.getLogger(__name__)
 
 UPLOAD_TOOL_ID = "upload1"
 LOAD_TOOLS_FROM_PATH = True
 DEFAULT_USE_FETCH_API = True
 DEFAULT_FILE_TYPE = "auto"
 DEFAULT_DBKEY = "?"
+DEFAULT_DECOMPRESS = False
 
 
 class StagingInterface(metaclass=abc.ABCMeta):
     """Client that parses a job input and populates files into the Galaxy API.
 
     Abstract class that must override _post (and optionally other things such
     _attach_file, _log, etc..) to adapt to bioblend (for Planemo) or using the
     tool test interactor infrastructure.
     """
 
     @abc.abstractmethod
-    def _post(self, api_path, payload, files_attached=False):
+    def _post(self, api_path: str, payload: Dict[str, Any]) -> Dict[str, Any]:
         """Make a post to the Galaxy API along supplied path."""
 
-    def _attach_file(self, path):
+    def _attach_file(self, path: str) -> BinaryIO:
         return open(path, "rb")
 
-    def _tools_post(self, payload, files_attached=False):
-        tool_response = self._post("tools", payload, files_attached=files_attached)
+    def _tools_post(self, payload: Dict[str, Any]) -> Dict[str, Any]:
+        tool_response = self._post("tools", payload)
         for job in tool_response.get("jobs", []):
             self._handle_job(job)
         return tool_response
 
-    def _fetch_post(self, payload, files_attached=False):
-        tool_response = self._post("tools/fetch", payload, files_attached=files_attached)
+    def _fetch_post(self, payload: Dict[str, Any]) -> Dict[str, Any]:
+        tool_response = self._post("tools/fetch", payload)
         for job in tool_response.get("jobs", []):
             self._handle_job(job)
         return tool_response
 
+    @abc.abstractmethod
     def _handle_job(self, job_response):
         """Implementer can decide if to wait for job(s) individually or not here."""
 
     def stage(
         self,
-        tool_or_workflow,
-        history_id,
-        job=None,
-        job_path=None,
-        use_path_paste=LOAD_TOOLS_FROM_PATH,
-        to_posix_lines=True,
-        job_dir=".",
-    ):
-        files_attached = [False]
-
-        def upload_func_fetch(upload_target):
-            def _attach_file(upload_payload, uri, index=0):
+        tool_or_workflow: Literal["tool", "workflow"],
+        history_id: str,
+        job: Optional[Dict[str, Any]] = None,
+        job_path: Optional[str] = None,
+        use_path_paste: bool = LOAD_TOOLS_FROM_PATH,
+        to_posix_lines: bool = True,
+        job_dir: str = ".",
+    ) -> Tuple[Dict[str, Any], List[Dict[str, Any]]]:
+        def upload_func_fetch(upload_target: UploadTarget) -> Dict[str, Any]:
+            def _attach_file(upload_payload: Dict[str, Any], uri: str, index: int = 0) -> Dict[str, str]:
                 uri = path_or_uri_to_uri(uri)
                 is_path = uri.startswith("file://")
                 if not is_path or use_path_paste:
                     return {"src": "url", "url": uri}
                 else:
-                    files_attached[0] = True
                     path = uri[len("file://") :]
                     upload_payload["__files"][f"files_{index}|file_data"] = self._attach_file(path)
                     return {"src": "files"}
 
             fetch_payload = None
             if isinstance(upload_target, FileUploadTarget):
                 file_path = upload_target.path
                 file_type = upload_target.properties.get("filetype", None) or DEFAULT_FILE_TYPE
                 dbkey = upload_target.properties.get("dbkey", None) or DEFAULT_DBKEY
                 fetch_payload = _fetch_payload(
                     history_id,
                     file_type=file_type,
                     dbkey=dbkey,
                     to_posix_lines=to_posix_lines,
+                    decompress=upload_target.properties.get("decompress") or DEFAULT_DECOMPRESS,
                 )
                 name = _file_path_to_name(file_path)
                 if file_path is not None:
                     src = _attach_file(fetch_payload, file_path)
                     fetch_payload["targets"][0]["elements"][0].update(src)
 
                 if upload_target.composite_data:
@@ -124,39 +138,41 @@
                 )
                 tags = upload_target.properties.get("tags")
                 if tags:
                     fetch_payload["targets"][0]["elements"][0]["tags"] = tags
             elif isinstance(upload_target, DirectoryUploadTarget):
                 fetch_payload = _fetch_payload(history_id, file_type="directory")
                 fetch_payload["targets"][0].pop("elements")
-                tar_path = upload_target.path
+                tar_path = upload_target.tar_path
                 src = _attach_file(fetch_payload, tar_path)
                 fetch_payload["targets"][0]["elements_from"] = src
-            else:
+            elif isinstance(upload_target, ObjectUploadTarget):
                 content = json.dumps(upload_target.object)
                 fetch_payload = _fetch_payload(history_id, file_type="expression.json")
                 fetch_payload["targets"][0]["elements"][0].update(
                     {
                         "src": "pasted",
                         "paste_content": content,
                     }
                 )
                 tags = upload_target.properties.get("tags")
-                fetch_payload["targets"][0]["elements"][0]["tags"] = tags
-            return self._fetch_post(fetch_payload, files_attached=files_attached[0])
+                if tags:
+                    fetch_payload["targets"][0]["elements"][0]["tags"] = tags
+            else:
+                raise ValueError(f"Unsupported type for upload_target: {type(upload_target)}")
+            return self._fetch_post(fetch_payload)
 
         # Save legacy upload_func to target older Galaxy servers
-        def upload_func(upload_target):
-            def _attach_file(upload_payload, uri, index=0):
+        def upload_func(upload_target: UploadTarget) -> Dict[str, Any]:
+            def _attach_file(upload_payload: Dict[str, Any], uri: str, index: int = 0) -> None:
                 uri = path_or_uri_to_uri(uri)
                 is_path = uri.startswith("file://")
                 if not is_path or use_path_paste:
                     upload_payload["inputs"]["files_%d|url_paste" % index] = uri
                 else:
-                    files_attached[0] = True
                     path = uri[len("file://") :]
                     upload_payload["__files"]["files_%d|file_data" % index] = self._attach_file(path)
 
             if isinstance(upload_target, FileUploadTarget):
                 file_path = upload_target.path
                 file_type = upload_target.properties.get("filetype", None) or DEFAULT_FILE_TYPE
                 dbkey = upload_target.properties.get("dbkey", None) or DEFAULT_DBKEY
@@ -183,45 +199,47 @@
 
                 if upload_target.composite_data:
                     for i, composite_data in enumerate(upload_target.composite_data):
                         upload_payload["inputs"][f"files_{i}|type"] = "upload_dataset"
                         _attach_file(upload_payload, composite_data, index=i)
 
                 self._log(f"upload_payload is {upload_payload}")
-                return self._tools_post(upload_payload, files_attached=files_attached[0])
+                return self._tools_post(upload_payload)
             elif isinstance(upload_target, FileLiteralTarget):
                 # For file literals - take them as is - never convert line endings.
                 payload = _upload_payload(history_id, file_type="auto", auto_decompress=False, to_posix_lines=False)
                 payload["inputs"]["files_0|url_paste"] = upload_target.contents
                 return self._tools_post(payload)
             elif isinstance(upload_target, DirectoryUploadTarget):
                 tar_path = upload_target.tar_path
 
                 upload_payload = _upload_payload(
                     history_id,
                     file_type="tar",
                 )
                 upload_payload["inputs"]["files_0|auto_decompress"] = False
                 _attach_file(upload_payload, tar_path)
-                tar_upload_response = self._tools_post(upload_payload, files_attached=files_attached[0])
+                tar_upload_response = self._tools_post(upload_payload)
                 convert_payload = dict(
                     tool_id="CONVERTER_tar_to_directory",
                     tool_inputs={"input1": {"src": "hda", "id": tar_upload_response["outputs"][0]["id"]}},
                     history_id=history_id,
                 )
                 convert_response = self._tools_post(convert_payload)
                 assert "outputs" in convert_response, convert_response
                 return convert_response
-            else:
+            elif isinstance(upload_target, ObjectUploadTarget):
                 content = json.dumps(upload_target.object)
                 payload = _upload_payload(history_id, file_type="expression.json")
                 payload["files_0|url_paste"] = content
                 return self._tools_post(payload)
+            else:
+                raise ValueError(f"Unsupported type for upload_target: {type(upload_target)}")
 
-        def create_collection_func(element_identifiers, collection_type):
+        def create_collection_func(element_identifiers: List[Dict[str, Any]], collection_type: str) -> Dict[str, Any]:
             payload = {
                 "name": "dataset collection",
                 "instance_type": "history",
                 "history_id": history_id,
                 "element_identifiers": element_identifiers,
                 "collection_type": collection_type,
                 "fields": None if collection_type != "record" else "auto",
@@ -231,77 +249,72 @@
         if job_path is not None:
             assert job is None
             with open(job_path) as f:
                 job = yaml.safe_load(f)
             job_dir = os.path.dirname(os.path.abspath(job_path))
         else:
             assert job is not None
-            assert job_dir is not None
 
         if self.use_fetch_api:
             upload = upload_func_fetch
         else:
             upload = upload_func
 
-        job_dict, datasets = galactic_job_json(
+        return galactic_job_json(
             job,
             job_dir,
             upload,
             create_collection_func,
             tool_or_workflow,
         )
-        return job_dict, datasets
 
     # extension point for planemo to override logging
     def _log(self, message):
         log.debug(message)
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def use_fetch_api(self):
         """Return true is this should use (modern) data fetch API."""
 
 
-class StagingInterace(StagingInterface):
-    """For backward compatibility with previous class name"""
-
-    warnings.warn("StagingInterace is deprecated, use StagingInterface instead", DeprecationWarning)
-
-
 class InteractorStaging(StagingInterface):
-    def __init__(self, galaxy_interactor, use_fetch_api=DEFAULT_USE_FETCH_API):
+    def __init__(self, galaxy_interactor: "ApiTestInteractor", use_fetch_api: bool = DEFAULT_USE_FETCH_API) -> None:
         self.galaxy_interactor = galaxy_interactor
         self._use_fetch_api = use_fetch_api
 
-    def _post(self, api_path, payload, files_attached=False):
+    def _post(self, api_path: str, payload: Dict[str, Any]) -> Dict[str, Any]:
         response = self.galaxy_interactor._post(api_path, payload, json=True)
         assert response.status_code == 200, response.text
         return response.json()
 
     def _handle_job(self, job_response):
         self.galaxy_interactor.wait_for_job(job_response["id"])
 
     @property
     def use_fetch_api(self):
         return self._use_fetch_api
 
 
-def _file_path_to_name(file_path):
+def _file_path_to_name(file_path: Optional[str]) -> str:
     if file_path is not None:
         name = os.path.basename(file_path)
     else:
         name = "defaultname"
     return name
 
 
-def _upload_payload(history_id, tool_id=UPLOAD_TOOL_ID, file_type=DEFAULT_FILE_TYPE, dbkey=DEFAULT_DBKEY, **kwd):
-    """Adapted from bioblend tools client."""
-    payload = {}
+def _upload_payload(
+    history_id: str, file_type: str = DEFAULT_FILE_TYPE, dbkey: str = DEFAULT_DBKEY, **kwd
+) -> Dict[str, Any]:
+    """Adapted from BioBlend tools client."""
+    payload: Dict[str, Any] = {}
     payload["history_id"] = history_id
-    payload["tool_id"] = tool_id
-    tool_input = {}
+    payload["tool_id"] = UPLOAD_TOOL_ID
+    tool_input: Dict[str, Any] = {}
     tool_input["file_type"] = file_type
     tool_input["dbkey"] = dbkey
     if not kwd.get("to_posix_lines", True):
         tool_input["files_0|to_posix_lines"] = False
     elif kwd.get("space_to_tab", False):
         tool_input["files_0|space_to_tab"] = "Yes"
     if "file_name" in kwd:
@@ -318,14 +331,16 @@
         "dbkey": dbkey,
     }
     for arg in ["to_posix_lines", "space_to_tab"]:
         if arg in kwd:
             element[arg] = kwd[arg]
     if "file_name" in kwd:
         element["name"] = kwd["file_name"]
+    if "decompress" in kwd:
+        element["auto_decompress"] = kwd["decompress"]
     target = {
         "destination": {"type": "hdas"},
         "elements": [element],
         "auto_decompress": False,
     }
     targets = [target]
     payload = {"history_id": history_id, "targets": targets, "__files": {}}
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/__init__.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/cwltool_deps.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/cwltool_deps.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,14 +84,19 @@
     from schema_salad.utils import yaml_no_ts
 except ImportError:
     schema_salad = None  # type: ignore[assignment]
     ref_resolver = None  # type: ignore[assignment]
     sourceline = None  # type: ignore[assignment]
     yaml_no_ts = None  # type: ignore[assignment]
 
+try:
+    from ruamel.yaml.comments import CommentedMap
+except ImportError:
+    CommentedMap = None  # type: ignore[assignment,misc]
+
 needs_shell_quoting = re.compile(r"""(^$|[\s|&;()<>\'"$@])""").search
 
 # if set to True, file format checking is not performed.
 beta_relaxed_fmt_check = True
 
 
 def ensure_cwltool_available():
@@ -111,14 +116,15 @@
             message += " Library 'shellescape' unavailable."
         if schema_salad is None:
             message += " Library 'schema_salad' unavailable."
         raise ImportError(message)
 
 
 __all__ = (
+    "CommentedMap",
     "default_loader",
     "ensure_cwltool_available",
     "getdefault",
     "load_tool",
     "LoadingContext",
     "main",
     "needs_shell_quoting",
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/parser.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """ This module provides proxy objects around objects from the common
 workflow language reference implementation library cwltool. These proxies
 adapt cwltool to Galaxy features and abstract the library away from the rest
 of the framework.
 """
 
-import base64
 import copy
 import json
 import logging
 import os
-import pickle
 from abc import (
     ABCMeta,
     abstractmethod,
 )
 from typing import (
     Dict,
     List,
@@ -27,15 +25,14 @@
     TypedDict,
 )
 
 from galaxy.exceptions import MessageException
 from galaxy.util import (
     listify,
     safe_makedirs,
-    unicodify,
 )
 from galaxy.util.bunch import Bunch
 from .cwltool_deps import (
     beta_relaxed_fmt_check,
     ensure_cwltool_available,
     getdefault,
     normalizeFilesDirs,
@@ -82,16 +79,14 @@
     "StepInputExpressionRequirement",
     "MultipleInputFeatureRequirement",
 ]
 
 
 SUPPORTED_WORKFLOW_REQUIREMENTS = SUPPORTED_TOOL_REQUIREMENTS + []
 
-PERSISTED_REPRESENTATION = "cwl_tool_object"
-
 ToolStateType = Dict[str, Union[None, str, bool, Dict[str, str]]]
 
 
 class InputInstanceDict(TypedDict, total=False):
     type: str
     name: str
     title: str
@@ -106,184 +101,15 @@
 class InputInstanceArrayDict(TypedDict):
     type: str
     name: str
     title: str
     blocks: List[InputInstanceDict]
 
 
-def tool_proxy(tool_path=None, tool_object=None, strict_cwl_validation=True, tool_directory=None, uuid=None):
-    """Provide a proxy object to cwltool data structures to just
-    grab relevant data.
-    """
-    ensure_cwltool_available()
-    tool = _to_cwl_tool_object(
-        tool_path=tool_path,
-        tool_object=tool_object,
-        strict_cwl_validation=strict_cwl_validation,
-        tool_directory=tool_directory,
-        uuid=uuid,
-    )
-    return tool
-
-
-def tool_proxy_from_persistent_representation(persisted_tool, strict_cwl_validation=True, tool_directory=None):
-    """Load a ToolProxy from a previously persisted representation."""
-    ensure_cwltool_available()
-    if PERSISTED_REPRESENTATION == "cwl_tool_object":
-        kwds = {"cwl_tool_object": ToolProxy.from_persistent_representation(persisted_tool)}
-    else:
-        raw_process_reference = persisted_tool  # ???
-        kwds = {"raw_process_reference": ToolProxy.from_persistent_representation(raw_process_reference)}
-    uuid = persisted_tool["uuid"]
-    tool = _to_cwl_tool_object(
-        uuid=uuid, strict_cwl_validation=strict_cwl_validation, tool_directory=tool_directory, **kwds
-    )
-    return tool
-
-
-def workflow_proxy(workflow_path, strict_cwl_validation=True):
-    ensure_cwltool_available()
-    workflow = _to_cwl_workflow_object(workflow_path, strict_cwl_validation=strict_cwl_validation)
-    return workflow
-
-
-def load_job_proxy(job_directory, strict_cwl_validation=True):
-    ensure_cwltool_available()
-    job_objects_path = os.path.join(job_directory, JOB_JSON_FILE)
-    job_objects = json.load(open(job_objects_path))
-    job_inputs = job_objects["job_inputs"]
-    output_dict = job_objects["output_dict"]
-    # Any reason to retain older tool_path variant of this? Probably not?
-    if "tool_path" in job_objects:
-        tool_path = job_objects["tool_path"]
-        cwl_tool = tool_proxy(tool_path, strict_cwl_validation=strict_cwl_validation)
-    else:
-        persisted_tool = job_objects["tool_representation"]
-        cwl_tool = tool_proxy_from_persistent_representation(
-            persisted_tool=persisted_tool, strict_cwl_validation=strict_cwl_validation
-        )
-    cwl_job = cwl_tool.job_proxy(job_inputs, output_dict, job_directory=job_directory)
-    return cwl_job
-
-
-def _to_cwl_tool_object(
-    tool_path=None,
-    tool_object=None,
-    cwl_tool_object=None,
-    raw_process_reference=None,
-    strict_cwl_validation=False,
-    tool_directory=None,
-    uuid=None,
-):
-    if uuid is None:
-        uuid = str(uuid4())
-    schema_loader = _schema_loader(strict_cwl_validation)
-    if raw_process_reference is None and tool_path is not None:
-        assert cwl_tool_object is None
-        assert tool_object is None
-
-        raw_process_reference = schema_loader.raw_process_reference(tool_path)
-        cwl_tool = schema_loader.tool(
-            raw_process_reference=raw_process_reference,
-        )
-    elif tool_object is not None:
-        assert raw_process_reference is None
-        assert cwl_tool_object is None
-
-        # Allow loading tools from YAML...
-        as_str = json.dumps(tool_object)
-        tool_object = yaml_no_ts().load(as_str)
-        path = tool_directory
-        if path is None:
-            path = os.getcwd()
-        uri = f"{ref_resolver.file_uri(path)}/"
-        sourceline.add_lc_filename(tool_object, uri)
-        raw_process_reference = schema_loader.raw_process_reference_for_object(tool_object, uri=uri)
-        cwl_tool = schema_loader.tool(
-            raw_process_reference=raw_process_reference,
-        )
-    else:
-        cwl_tool = cwl_tool_object
-
-    if isinstance(cwl_tool, int):
-        raise Exception("Failed to load tool.")
-
-    raw_tool = cwl_tool.tool
-    # Apply Galaxy hacks to CWL tool representation to bridge semantic differences
-    # between Galaxy and cwltool.
-    _hack_cwl_requirements(cwl_tool)
-    check_requirements(raw_tool)
-    return _cwl_tool_object_to_proxy(cwl_tool, uuid, raw_process_reference=raw_process_reference, tool_path=tool_path)
-
-
-def _cwl_tool_object_to_proxy(cwl_tool, uuid, raw_process_reference=None, tool_path=None):
-    raw_tool = cwl_tool.tool
-    if "class" not in raw_tool:
-        raise Exception("File does not declare a class, not a valid Draft 3+ CWL tool.")
-
-    process_class = raw_tool["class"]
-    if process_class == "CommandLineTool":
-        proxy_class = CommandLineToolProxy
-    elif process_class == "ExpressionTool":
-        proxy_class = ExpressionToolProxy
-    else:
-        raise Exception("File not a CWL CommandLineTool.")
-    top_level_object = tool_path is not None
-    if top_level_object and ("cwlVersion" not in raw_tool):
-        raise Exception("File does not declare a CWL version, pre-draft 3 CWL tools are not supported.")
-
-    proxy = proxy_class(cwl_tool, uuid, raw_process_reference, tool_path)
-    return proxy
-
-
-def _to_cwl_workflow_object(workflow_path, strict_cwl_validation=None):
-    proxy_class = WorkflowProxy
-    cwl_workflow = _schema_loader(strict_cwl_validation).tool(path=workflow_path)
-    raw_workflow = cwl_workflow.tool
-    check_requirements(raw_workflow, tool=False)
-
-    proxy = proxy_class(cwl_workflow, workflow_path)
-    return proxy
-
-
-def _schema_loader(strict_cwl_validation):
-    target_schema_loader = schema_loader if strict_cwl_validation else non_strict_non_validating_schema_loader
-    return target_schema_loader
-
-
-def _hack_cwl_requirements(cwl_tool):
-    move_to_hints: List[int] = []
-    for i, requirement in enumerate(cwl_tool.requirements):
-        if requirement["class"] == DOCKER_REQUIREMENT:
-            move_to_hints.insert(0, i)
-
-    for i in move_to_hints:
-        del cwl_tool.requirements[i]
-        cwl_tool.hints.append(requirement)
-
-
-def check_requirements(rec, tool=True):
-    if isinstance(rec, dict):
-        if "requirements" in rec:
-            for r in rec["requirements"]:
-                if tool:
-                    possible = SUPPORTED_TOOL_REQUIREMENTS
-                else:
-                    possible = SUPPORTED_WORKFLOW_REQUIREMENTS
-                if r["class"] not in possible:
-                    raise Exception(f"Unsupported requirement {r['class']}")
-        for d in rec:
-            check_requirements(rec[d], tool=tool)
-    if isinstance(rec, list):
-        for d in rec:
-            check_requirements(d, tool=tool)
-
-
 class ToolProxy(metaclass=ABCMeta):
-
     _class: str
 
     def __init__(self, tool, uuid, raw_process_reference=None, tool_path=None):
         self._tool = tool
         self.uuid = uuid
         self._tool_path = tool_path
         self._raw_process_reference = raw_process_reference
@@ -337,39 +163,62 @@
     @abstractmethod
     def label(self):
         """Return label for tool."""
 
     def to_persistent_representation(self):
         """Return a JSON representation of this tool. Not for serialization
         over the wire, but serialization in a database."""
-        # TODO: Replace this with some more readable serialization,
-        # I really don't like using pickle here.
-        if PERSISTED_REPRESENTATION == "cwl_tool_object":
-            persisted_obj = remove_pickle_problems(self._tool)
-        else:
-            persisted_obj = self._raw_process_reference
+        persisted_obj = self._tool.tool
+        persisted_obj["requirements"] = self.requirements
+        if not persisted_obj.get("cwlVersion"):
+            # This happens for any inline process, but getting it from metadata is correct for inline processes at least
+            persisted_obj["cwlVersion"] = self._tool.metadata["cwlVersion"]
         return {
             "class": self._class,
-            "pickle": unicodify(base64.b64encode(pickle.dumps(persisted_obj, pickle.HIGHEST_PROTOCOL))),
+            # Should maybe be yaml instead
+            "raw_process_reference": persisted_obj,
             "uuid": self.uuid,
         }
 
     @staticmethod
-    def from_persistent_representation(as_object):
+    def from_persistent_representation(as_object, strict_cwl_validation=True, tool_directory=None) -> "ToolProxy":
         """Recover an object serialized with to_persistent_representation."""
         if "class" not in as_object:
             raise Exception("Failed to deserialize tool proxy from JSON object - no class found.")
-        if "pickle" not in as_object:
-            raise Exception("Failed to deserialize tool proxy from JSON object - no pickle representation found.")
-        if "uuid" not in as_object:
-            raise Exception("Failed to deserialize tool proxy from JSON object - no uuid found.")
-        to_unpickle = base64.b64decode(as_object["pickle"])
-        loaded_object = pickle.loads(to_unpickle)
+        loaded_object = tool_proxy(
+            tool_object=as_object["raw_process_reference"],
+            strict_cwl_validation=strict_cwl_validation,
+            tool_directory=tool_directory,
+            uuid=as_object.get("uuid"),
+        )
         return loaded_object
 
+    @property
+    def requirements(self) -> List:
+        return getattr(self._tool, "requirements", [])
+
+    def hints_or_requirements_of_class(self, class_name: str) -> List:
+        reqs_and_hints = self.requirements + getattr(self._tool, "hints", [])
+        return [hint for hint in reqs_and_hints if hint["class"] == class_name]
+
+    def software_requirements(self) -> List:
+        # Roughest imaginable pass at parsing requirements, really need to take in specs, handle
+        # multiple versions, etc...
+        requirements = []
+        for hint in self.hints_or_requirements_of_class("SoftwareRequirement"):
+            packages = hint.get("packages", [])
+            for package in packages:
+                versions = package.get("version", [])
+                first_version = None if not versions else versions[0]
+                requirements.append((package["package"], first_version))
+        return requirements
+
+    def resource_requirements(self) -> List:
+        return self.hints_or_requirements_of_class("ResourceRequirement")
+
 
 class CommandLineToolProxy(ToolProxy):
     _class = "CommandLineTool"
 
     def description(self):
         # Don't use description - typically too verbose.
         return ""
@@ -433,43 +282,14 @@
             if "dockerImageId" in hint:
                 return hint["dockerImageId"]
             else:
                 return hint["dockerPull"]
 
         return None
 
-    def hints_or_requirements_of_class(self, class_name):
-        tool = self._tool.tool
-        reqs_and_hints = tool.get("requirements", []) + tool.get("hints", [])
-        for hint in reqs_and_hints:
-            if hint["class"] == class_name:
-                yield hint
-
-    def software_requirements(self):
-        # Roughest imaginable pass at parsing requirements, really need to take in specs, handle
-        # multiple versions, etc...
-        tool = self._tool.tool
-        reqs_and_hints = tool.get("requirements", []) + tool.get("hints", [])
-        requirements = []
-        for hint in reqs_and_hints:
-            if hint["class"] == "SoftwareRequirement":
-                packages = hint.get("packages", [])
-                for package in packages:
-                    versions = package.get("version", [])
-                    first_version = None if not versions else versions[0]
-                    requirements.append((package["package"], first_version))
-        return requirements
-
-    def resource_requirements(self):
-        return [r for r in self.requirements if r["class"] == "ResourceRequirement"]
-
-    @property
-    def requirements(self):
-        return getattr(self._tool, "requirements", [])
-
 
 class ExpressionToolProxy(CommandLineToolProxy):
     _class = "ExpressionTool"
 
 
 class JobProxy:
     def __init__(self, tool_proxy, input_dict, output_dict, job_directory):
@@ -785,15 +605,15 @@
         input_connections_by_step = []
         for step_proxy in step_proxies:
             input_connections_step: Dict[str, List[Dict[str, str]]] = {}
             for input_proxy in step_proxy.input_proxies:
                 cwl_source_id = input_proxy.cwl_source_id
                 input_name = input_proxy.input_name
                 # Consider only allow multiple if MultipleInputFeatureRequirement is enabled
-                for (output_step_name, output_name) in split_step_references(cwl_source_id, workflow_id=self.cwl_id):
+                for output_step_name, output_name in split_step_references(cwl_source_id, workflow_id=self.cwl_id):
                     if "#" in self.cwl_id:
                         sep_on = "/"
                     else:
                         sep_on = "#"
                     output_step_id = self.cwl_id + sep_on + output_step_name
 
                     if output_step_id not in cwl_ids_to_index:
@@ -856,15 +676,14 @@
             "id": i,
             "label": label,
             "position": {"left": 0, "top": 0},
             "annotation": self.cwl_object_to_annotation(input),
             "input_connections": {},  # Should the Galaxy API really require this? - Seems to.
             "workflow_outputs": self.get_outputs_for_label(label),
         }
-
         if input_type == "File" and "default" not in input:
             input_as_dict["type"] = "data_input"
         elif isinstance(input_type, dict) and input_type.get("type") == "array":
             input_as_dict["type"] = "data_collection_input"
             input_as_dict["collection_type"] = "list"
         elif isinstance(input_type, dict) and input_type.get("type") == "record":
             input_as_dict["type"] = "data_collection_input"
@@ -893,14 +712,166 @@
 
         return input_as_dict
 
     def cwl_object_to_annotation(self, cwl_obj):
         return cwl_obj.get("doc", None)
 
 
+def tool_proxy(
+    tool_path=None, tool_object=None, strict_cwl_validation=True, tool_directory=None, uuid=None
+) -> ToolProxy:
+    """Provide a proxy object to cwltool data structures to just
+    grab relevant data.
+    """
+    ensure_cwltool_available()
+    return _to_cwl_tool_object(
+        tool_path=tool_path,
+        tool_object=tool_object,
+        strict_cwl_validation=strict_cwl_validation,
+        tool_directory=tool_directory,
+        uuid=uuid,
+    )
+
+
+def tool_proxy_from_persistent_representation(
+    persisted_tool, strict_cwl_validation=True, tool_directory=None
+) -> ToolProxy:
+    """Load a ToolProxy from a previously persisted representation."""
+    ensure_cwltool_available()
+    return ToolProxy.from_persistent_representation(
+        persisted_tool, strict_cwl_validation=strict_cwl_validation, tool_directory=tool_directory
+    )
+
+
+def workflow_proxy(workflow_path, strict_cwl_validation=True) -> WorkflowProxy:
+    ensure_cwltool_available()
+    return _to_cwl_workflow_object(workflow_path, strict_cwl_validation=strict_cwl_validation)
+
+
+def load_job_proxy(job_directory, strict_cwl_validation=True) -> JobProxy:
+    ensure_cwltool_available()
+    job_objects_path = os.path.join(job_directory, JOB_JSON_FILE)
+    job_objects = json.load(open(job_objects_path))
+    job_inputs = job_objects["job_inputs"]
+    output_dict = job_objects["output_dict"]
+    persisted_tool = job_objects["tool_representation"]
+    cwl_tool = tool_proxy_from_persistent_representation(
+        persisted_tool=persisted_tool, strict_cwl_validation=strict_cwl_validation
+    )
+    return cwl_tool.job_proxy(job_inputs, output_dict, job_directory=job_directory)
+
+
+def _to_cwl_tool_object(
+    tool_path=None,
+    tool_object=None,
+    cwl_tool_object=None,
+    raw_process_reference=None,
+    strict_cwl_validation=False,
+    tool_directory=None,
+    uuid=None,
+) -> ToolProxy:
+    if uuid is None:
+        uuid = str(uuid4())
+    schema_loader = _schema_loader(strict_cwl_validation)
+    if raw_process_reference is None and tool_path is not None:
+        assert cwl_tool_object is None
+        assert tool_object is None
+
+        raw_process_reference = schema_loader.raw_process_reference(tool_path)
+        cwl_tool = schema_loader.tool(
+            raw_process_reference=raw_process_reference,
+        )
+    elif tool_object is not None:
+        assert raw_process_reference is None
+        assert cwl_tool_object is None
+
+        # Allow loading tools from YAML...
+        as_str = json.dumps(tool_object)
+        tool_object = yaml_no_ts().load(as_str)
+        path = tool_directory
+        if path is None:
+            path = os.getcwd()
+        uri = f"{ref_resolver.file_uri(path)}/"
+        sourceline.add_lc_filename(tool_object, uri)
+        raw_process_reference = schema_loader.raw_process_reference_for_object(tool_object, uri=uri)
+        cwl_tool = schema_loader.tool(
+            raw_process_reference=raw_process_reference,
+        )
+    else:
+        cwl_tool = cwl_tool_object
+
+    if isinstance(cwl_tool, int):
+        raise Exception("Failed to load tool.")
+
+    raw_tool = cwl_tool.tool
+    # Apply Galaxy hacks to CWL tool representation to bridge semantic differences
+    # between Galaxy and cwltool.
+    _hack_cwl_requirements(cwl_tool)
+    check_requirements(raw_tool)
+    return _cwl_tool_object_to_proxy(cwl_tool, uuid, raw_process_reference=raw_process_reference, tool_path=tool_path)
+
+
+def _cwl_tool_object_to_proxy(cwl_tool, uuid, raw_process_reference=None, tool_path=None) -> ToolProxy:
+    raw_tool = cwl_tool.tool
+    if "class" not in raw_tool:
+        raise Exception("File does not declare a class, not a valid Draft 3+ CWL tool.")
+
+    process_class = raw_tool["class"]
+    if process_class == "CommandLineTool":
+        proxy_class = CommandLineToolProxy
+    elif process_class == "ExpressionTool":
+        proxy_class = ExpressionToolProxy
+    else:
+        raise Exception("File not a CWL CommandLineTool.")
+    top_level_object = tool_path is not None
+    if top_level_object and ("cwlVersion" not in raw_tool):
+        raise Exception("File does not declare a CWL version, pre-draft 3 CWL tools are not supported.")
+
+    return proxy_class(cwl_tool, uuid, raw_process_reference, tool_path)
+
+
+def _to_cwl_workflow_object(workflow_path, strict_cwl_validation=None) -> WorkflowProxy:
+    cwl_workflow = _schema_loader(strict_cwl_validation).tool(path=workflow_path)
+    raw_workflow = cwl_workflow.tool
+    check_requirements(raw_workflow, tool=False)
+    return WorkflowProxy(cwl_workflow, workflow_path)
+
+
+def _schema_loader(strict_cwl_validation):
+    return schema_loader if strict_cwl_validation else non_strict_non_validating_schema_loader
+
+
+def _hack_cwl_requirements(cwl_tool):
+    move_to_hints: List[int] = []
+    for i, requirement in enumerate(cwl_tool.requirements):
+        if requirement["class"] == DOCKER_REQUIREMENT:
+            move_to_hints.insert(0, i)
+
+    for i in move_to_hints:
+        del cwl_tool.requirements[i]
+        cwl_tool.hints.append(requirement)
+
+
+def check_requirements(rec, tool=True):
+    if isinstance(rec, dict):
+        if "requirements" in rec:
+            for r in rec["requirements"]:
+                if tool:
+                    possible = SUPPORTED_TOOL_REQUIREMENTS
+                else:
+                    possible = SUPPORTED_WORKFLOW_REQUIREMENTS
+                if r["class"] not in possible:
+                    raise Exception(f"Unsupported requirement {r['class']}")
+        for d in rec:
+            check_requirements(rec[d], tool=tool)
+    if isinstance(rec, list):
+        for d in rec:
+            check_requirements(d, tool=tool)
+
+
 def split_step_references(step_references, workflow_id=None, multiple=True):
     """Split a CWL step input or output reference into step id and name."""
     # Trim off the workflow id part of the reference.
     step_references = listify(step_references)
     split_references = []
 
     for step_reference in step_references:
@@ -935,79 +906,22 @@
     if multiple:
         return split_references
     else:
         assert len(split_references) == 1
         return split_references[0]
 
 
-def build_step_proxy(workflow_proxy, step, index):
+def build_step_proxy(workflow_proxy: WorkflowProxy, step, index):
     step_type = step.embedded_tool.tool["class"]
     if step_type == "Workflow":
         return SubworkflowStepProxy(workflow_proxy, step, index)
     else:
         return ToolStepProxy(workflow_proxy, step, index)
 
 
-class BaseStepProxy:
-    def __init__(self, workflow_proxy, step, index):
-        self._workflow_proxy = workflow_proxy
-        self._step = step
-        self._index = index
-        self._uuid = str(uuid4())
-        self._input_proxies = None
-
-    @property
-    def step_class(self):
-        return self.cwl_tool_object.tool["class"]
-
-    @property
-    def cwl_id(self):
-        return self._step.id
-
-    @property
-    def cwl_workflow_id(self):
-        return self._workflow_proxy.cwl_id
-
-    @property
-    def requirements(self):
-        return self._step.requirements
-
-    @property
-    def hints(self):
-        return self._step.hints
-
-    @property
-    def label(self):
-        label = self._workflow_proxy.jsonld_id_to_label(self._step.id)
-        return label
-
-    def galaxy_workflow_outputs_list(self):
-        return self._workflow_proxy.get_outputs_for_label(self.label)
-
-    @property
-    def cwl_tool_object(self):
-        return self._step.embedded_tool
-
-    @property
-    def input_proxies(self):
-        if self._input_proxies is None:
-            input_proxies = []
-            cwl_inputs = self._step.tool["inputs"]
-            for cwl_input in cwl_inputs:
-                input_proxies.append(InputProxy(self, cwl_input))
-            self._input_proxies = input_proxies
-        return self._input_proxies
-
-    def inputs_to_dicts(self):
-        inputs_as_dicts = []
-        for input_proxy in self.input_proxies:
-            inputs_as_dicts.append(input_proxy.to_dict())
-        return inputs_as_dicts
-
-
 class InputProxy:
     def __init__(self, step_proxy, cwl_input):
         self._cwl_input = cwl_input
         self.step_proxy = step_proxy
         self.workflow_proxy = step_proxy._workflow_proxy
 
         cwl_input_id = cwl_input["id"]
@@ -1048,14 +962,62 @@
             # TODO: Add a table for expressions - mark the type as CWL 1.0 JavaScript.
             as_dict["value_from"] = self._cwl_input["valueFrom"]
         if "default" in self._cwl_input:
             as_dict["default"] = self._cwl_input["default"]
         return as_dict
 
 
+class BaseStepProxy:
+    def __init__(self, workflow_proxy: WorkflowProxy, step, index):
+        self._workflow_proxy = workflow_proxy
+        self._step = step
+        self._index = index
+        self._uuid = str(uuid4())
+        cwl_inputs = self._step.tool["inputs"]
+        self.input_proxies = [InputProxy(self, cwl_input) for cwl_input in cwl_inputs]
+
+    @property
+    def step_class(self):
+        return self.cwl_tool_object.tool["class"]
+
+    @property
+    def cwl_id(self):
+        return self._step.id
+
+    @property
+    def cwl_workflow_id(self):
+        return self._workflow_proxy.cwl_id
+
+    @property
+    def requirements(self):
+        return self._step.requirements
+
+    @property
+    def hints(self):
+        return self._step.hints
+
+    @property
+    def label(self):
+        label = self._workflow_proxy.jsonld_id_to_label(self._step.id)
+        return label
+
+    def galaxy_workflow_outputs_list(self):
+        return self._workflow_proxy.get_outputs_for_label(self.label)
+
+    @property
+    def cwl_tool_object(self):
+        return self._step.embedded_tool
+
+    def inputs_to_dicts(self):
+        inputs_as_dicts = []
+        for input_proxy in self.input_proxies:
+            inputs_as_dicts.append(input_proxy.to_dict())
+        return inputs_as_dicts
+
+
 class ToolStepProxy(BaseStepProxy):
     def __init__(self, workflow_proxy, step, index):
         super().__init__(workflow_proxy, step, index)
         self._tool_proxy = None
 
     @property
     def tool_proxy(self):
@@ -1073,25 +1035,29 @@
         # connections. This doesn't seem ideal - consider just making Galaxy
         # handle this.
         tool_state: ToolStateType = {}
         for input_name in input_connections.keys():
             tool_state[input_name] = None
 
         outputs = self.galaxy_workflow_outputs_list()
-        return {
+        when_expression = self._step.tool.get("when")
+        rval = {
             "id": self._index,
             "tool_uuid": self.tool_proxy.uuid,  # TODO: make sure this is respected...
             "label": self.label,
             "position": {"left": 0, "top": 0},
             "type": "tool",
             "annotation": self._workflow_proxy.cwl_object_to_annotation(self._step.tool),
             "input_connections": input_connections,
             "inputs": self.inputs_to_dicts(),
             "workflow_outputs": outputs,
         }
+        if when_expression:
+            rval["when"] = when_expression
+        return rval
 
 
 class SubworkflowStepProxy(BaseStepProxy):
     def __init__(self, workflow_proxy, step, index):
         super().__init__(workflow_proxy, step, index)
         self._subworkflow_proxy = None
 
@@ -1120,37 +1086,14 @@
     @property
     def subworkflow_proxy(self):
         if self._subworkflow_proxy is None:
             self._subworkflow_proxy = WorkflowProxy(self.cwl_tool_object)
         return self._subworkflow_proxy
 
 
-def remove_pickle_problems(obj):
-    """doc_loader does not pickle correctly"""
-    if hasattr(obj, "doc_loader"):
-        obj.doc_loader = None
-    if hasattr(obj, "embedded_tool"):
-        obj.embedded_tool = remove_pickle_problems(obj.embedded_tool)
-    if hasattr(obj, "steps"):
-        obj.steps = [remove_pickle_problems(s) for s in obj.steps]
-    return obj
-
-
-class WorkflowToolReference(metaclass=ABCMeta):
-    pass
-
-
-class EmbeddedWorkflowToolReference(WorkflowToolReference):
-    pass
-
-
-class ExternalWorkflowToolReference(WorkflowToolReference):
-    pass
-
-
 def _outer_field_to_input_instance(field):
     field_type = field_to_field_type(field)  # Must be a list if in here?
     if not isinstance(field_type, list):
         field_type = [field_type]
 
     name, label, description = _field_metadata(field)
 
@@ -1240,15 +1183,14 @@
     def __init__(self, name, case, whens):
         self.input_type = INPUT_TYPE.CONDITIONAL
         self.name = name
         self.case = case
         self.whens = whens
 
     def to_dict(self):
-
         as_dict = dict(
             name=self.name,
             type=INPUT_TYPE.CONDITIONAL,
             test=self.case.to_dict(),
             when={},
         )
         for value, block in self.whens:
@@ -1312,15 +1254,15 @@
             if self.area:
                 as_dict["area"] = True
 
             if self.input_type == INPUT_TYPE.INTEGER:
                 as_dict["value"] = "0"
             if self.input_type == INPUT_TYPE.FLOAT:
                 as_dict["value"] = "0.0"
-            elif self.input_type == INPUT_TYPE.DATA_COLLECTON:
+            elif self.input_type == INPUT_TYPE.DATA_COLLECTION:
                 as_dict["collection_type"] = self.collection_type
             return as_dict
 
 
 OUTPUT_TYPE = Bunch(
     GLOB="glob",
     STDOUT="stdout",
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/representation.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/representation.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     INTEGER = "integer"
     FLOAT = "float"
     TEXT = "text"
     BOOLEAN = "boolean"
     SELECT = "select"
     FIELD = "field"
     CONDITIONAL = "conditional"
-    DATA_COLLECTON = "data_collection"
+    DATA_COLLECTION = "data_collection"
 
 
 # There are two approaches to mapping CWL tool state to Galaxy tool state
 # one is to map CWL types to compound Galaxy tool parameters combinations
 # with conditionals and the other is to use a new Galaxy parameter type that
 # allows unions, optional specifications, etc.... The problem with the former
 # is that it doesn't work with the workflow parameters for instance and is
@@ -73,17 +73,17 @@
     TypeRepresentation("integer", INPUT_TYPE.INTEGER, "an integer", None),
     TypeRepresentation("float", INPUT_TYPE.FLOAT, "a decimal number", None),
     TypeRepresentation("double", INPUT_TYPE.FLOAT, "a decimal number", None),
     TypeRepresentation("file", INPUT_TYPE.DATA, "a dataset", None),
     TypeRepresentation("directory", INPUT_TYPE.DATA, "a directory", None),
     TypeRepresentation("boolean", INPUT_TYPE.BOOLEAN, "a boolean", None),
     TypeRepresentation("text", INPUT_TYPE.TEXT, "a simple text field", None),
-    TypeRepresentation("record", INPUT_TYPE.DATA_COLLECTON, "record as a dataset collection", "record"),
+    TypeRepresentation("record", INPUT_TYPE.DATA_COLLECTION, "record as a dataset collection", "record"),
     TypeRepresentation("json", INPUT_TYPE.TEXT, "arbitrary JSON structure", None),
-    TypeRepresentation("array", INPUT_TYPE.DATA_COLLECTON, "as a dataset list", "list"),
+    TypeRepresentation("array", INPUT_TYPE.DATA_COLLECTION, "as a dataset list", "list"),
     TypeRepresentation("enum", INPUT_TYPE.TEXT, "enum value", None),  # TODO: make this a select...
     TypeRepresentation("field", INPUT_TYPE.FIELD, "arbitrary JSON structure", None),
 ]
 FIELD_TYPE_REPRESENTATION = TYPE_REPRESENTATIONS[-1]
 
 if not USE_FIELD_TYPES:
     CWL_TYPE_TO_REPRESENTATIONS = {
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/runnable.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/runnable.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/runtime_actions.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/runtime_actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,41 +66,35 @@
 
 
 def handle_outputs(job_directory=None):
     # Relocate dynamically collected files to pre-determined locations
     # registered with ToolOutput objects via from_work_dir handling.
     if job_directory is None:
         job_directory = os.path.join(os.getcwd(), os.path.pardir)
-    metadata_directory = os.path.join(job_directory, "metadata")
-    metadata_params_path = os.path.join(metadata_directory, "params.json")
-    try:
-        with open(metadata_params_path) as f:
-            metadata_params = json.load(f)
-    except OSError:
-        raise Exception(f"Failed to find params.json from metadata directory [{metadata_directory}]")
-
     cwl_job_file = os.path.join(job_directory, JOB_JSON_FILE)
     if not os.path.exists(cwl_job_file):
         # Not a CWL job, just continue
         return
     # So we only need to do strict validation when the tool was loaded,
     # no reason to do it again during job execution - so this shortcut
     # allows us to not need Galaxy's full configuration on job nodes.
     job_proxy = load_job_proxy(job_directory, strict_cwl_validation=False)
     tool_working_directory = os.path.join(job_directory, "working")
 
-    job_id_tag = metadata_params["job_id_tag"]
+    cwl_metadata_params_path = os.path.join(job_directory, "cwl_params.json")
+    with open(cwl_metadata_params_path) as f:
+        cwl_metadata_params = json.load(f)
+    job_id_tag = cwl_metadata_params["job_id_tag"]
     from galaxy.job_execution.output_collect import (
         default_exit_code_file,
         read_exit_code_from,
     )
 
     exit_code_file = default_exit_code_file(".", job_id_tag)
     tool_exit_code = read_exit_code_from(exit_code_file, job_id_tag)
-
     outputs = job_proxy.collect_outputs(tool_working_directory, tool_exit_code)
 
     # Build galaxy.json file.
     provided_metadata = {}
 
     def move_directory(output, target_path, output_name=None):
         assert output["class"] == "Directory"
@@ -122,15 +116,14 @@
     def move_output(output, target_path, output_name=None):
         assert output["class"] == "File"
         file_description = file_dict_to_description(output)
         file_description.write_to(target_path)
 
         secondary_files = output.get("secondaryFiles", [])
         if secondary_files:
-
             order = []
             index_contents = {"order": order}
 
             for secondary_file in secondary_files:
                 if output_name is None:
                     raise NotImplementedError("secondaryFiles are unimplemented for dynamic list elements")
 
@@ -224,12 +217,13 @@
             handle_known_output_json(output, output_name)
 
     for output_instance in job_proxy._tool_proxy.output_instances():
         output_name = output_instance.name
         if output_name not in handled_outputs:
             handle_known_output_json(None, output_name)
 
-    with open("galaxy.json", "w") as f:
+    job_metadata = os.path.join(job_directory, cwl_metadata_params["job_metadata"])
+    with open(job_metadata, "w") as f:
         json.dump(provided_metadata, f)
 
 
 __all__ = ("handle_outputs",)
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/schema.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 """Abstraction around cwltool and related libraries for loading a CWL artifact."""
 import os
 import tempfile
-from collections import namedtuple
+from typing import NamedTuple
 
 from .cwltool_deps import (
+    CommentedMap,
     default_loader,
     ensure_cwltool_available,
     load_tool,
     LoadingContext,
     resolve_and_validate_document,
 )
 
-RawProcessReference = namedtuple("RawProcessReference", ["loading_context", "process_object", "uri"])
-ResolvedProcessDefinition = namedtuple("ResolvedProcessDefinition", ["loading_context", "uri", "raw_process_reference"])
+
+class RawProcessReference(NamedTuple):
+    loading_context: LoadingContext
+    process_object: CommentedMap
+    uri: str
+
+
+class ResolvedProcessDefinition(NamedTuple):
+    loading_context: LoadingContext
+    uri: str
+    raw_process_reference: RawProcessReference
+
+
 REWRITE_EXPRESSIONS = False
 
 
 class SchemaLoader:
     def __init__(self, strict=True, validate=True):
         self._strict = strict
         self._validate = validate
@@ -32,54 +44,54 @@
         loading_context.do_validate = self._validate
         loading_context.loader = self.raw_document_loader
         loading_context.do_update = True
         loading_context.relax_path_checks = True
         return loading_context
 
     def raw_process_reference(self, path, loading_context=None):
+        suffix = ""
+        if "#" in path:
+            path, suffix = path.split("#")
+        path = os.path.abspath(path)
+        uri = f"file://{path}"
+        loading_context = loading_context or self.loading_context()
         with tempfile.TemporaryDirectory() as output_dir:
-            suffix = ""
-            if "#" in path:
-                path, suffix = path.split("#")
-            processed_path = os.path.join(output_dir, os.path.basename(path))
-            path = os.path.abspath(path)
-            uri = f"file://{path}"
-            loading_context = loading_context or self.loading_context()
-            if REWRITE_EXPRESSIONS:
-                from cwl_utils import cwl_expression_refactor
-
-                exit_code = cwl_expression_refactor.main([output_dir, path, "--skip-some1", "--skip-some2"])
-                if exit_code == 0:
-                    uri = f"file://{processed_path}"
+            processed_path = os.path.join(output_dir, os.path.basename(path))  # noqa: F841
+            # if REWRITE_EXPRESSIONS:
+            #     The cwl_expression_refactor import below doesn't work any more
+            #     because there are now 3 cwl_v1_X_expression_refactor modules.
+            #     from cwl_utils import cwl_expression_refactor
+            #     exit_code = cwl_expression_refactor.main([output_dir, path, "--skip-some1", "--skip-some2"])
+            #     if exit_code == 0:
+            #         uri = f"file://{processed_path}"
             if suffix:
                 uri = f"{uri}#{suffix}"
             loading_context, process_object, uri = load_tool.fetch_document(uri, loadingContext=loading_context)
         return RawProcessReference(loading_context, process_object, uri)
 
     def raw_process_reference_for_object(self, process_object, uri=None, loading_context=None):
         if uri is None:
             uri = "galaxy://"
         loading_context = loading_context or self.loading_context()
         process_object["id"] = uri
         loading_context, process_object, uri = load_tool.fetch_document(process_object, loadingContext=loading_context)
         return RawProcessReference(loading_context, process_object, uri)
 
-    def process_definition(self, raw_process_reference):
+    def process_definition(self, raw_process_reference: RawProcessReference) -> ResolvedProcessDefinition:
         assert raw_process_reference.loading_context is not None, "No loading context found for raw_process_reference"
         loading_context, uri = resolve_and_validate_document(
             raw_process_reference.loading_context,
             raw_process_reference.process_object,
             raw_process_reference.uri,
         )
-        process_def = ResolvedProcessDefinition(
+        return ResolvedProcessDefinition(
             loading_context,
             uri,
             raw_process_reference,
         )
-        return process_def
 
     def tool(self, **kwds):
         process_definition = kwds.get("process_definition", None)
         if process_definition is None:
             raw_process_reference = kwds.get("raw_process_reference", None)
             if raw_process_reference is None:
                 raw_process_reference = self.raw_process_reference(kwds["path"])
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/cwl/util.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/cwl/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 """Client-centric CWL-related utilities.
 
 Used to share code between the Galaxy test framework
 and other Galaxy CWL clients (e.g. Planemo)."""
+import abc
 import hashlib
 import io
 import json
 import os
 import tarfile
 import tempfile
 import urllib.parse
 from collections import namedtuple
 from typing import (
     Any,
     BinaryIO,
+    Callable,
+    Dict,
     List,
     Optional,
+    Tuple,
 )
 
 import yaml
-from typing_extensions import TypedDict
+from typing_extensions import (
+    Literal,
+    TypedDict,
+)
 
 from galaxy.util import (
     str_removeprefix,
     unicodify,
 )
 
 STORE_SECONDARY_FILES_WITH_BASENAME = True
@@ -54,15 +61,15 @@
 )
 
 
 def output_properties(
     path: Optional[str] = None,
     content: Optional[bytes] = None,
     basename=None,
-    pseduo_location=False,
+    pseudo_location=False,
 ) -> OutputPropertiesType:
     checksum = hashlib.sha1()
     properties: OutputPropertiesType = {"class": "File", "checksum": "", "size": 0}
     f: BinaryIO
     if path is not None:
         properties["path"] = path
         f = open(path, "rb")
@@ -79,103 +86,114 @@
             filesize += len(contents)
             contents = f.read(1024 * 1024)
     finally:
         f.close()
     properties["checksum"] = f"sha1${checksum.hexdigest()}"
     properties["size"] = filesize
     set_basename_and_derived_properties(properties, basename)
-    _handle_pseudo_location(properties, pseduo_location)
+    _handle_pseudo_location(properties, pseudo_location)
     return properties
 
 
-def _handle_pseudo_location(properties, pseduo_location):
-    if pseduo_location:
+def _handle_pseudo_location(properties, pseudo_location):
+    if pseudo_location:
         properties["location"] = properties["basename"]
 
 
-def abs_path_or_uri(path_or_uri, relative_to):
-    """Return an absolute path if this isn't a URI, otherwise keep the URI the same."""
-    is_uri = "://" in path_or_uri
-    if not is_uri:
-        if not os.path.isabs(path_or_uri):
-            path_or_uri = os.path.abspath(os.path.join(relative_to, path_or_uri))
-        _ensure_file_exists(path_or_uri)
-    return path_or_uri
+def abs_path_or_uri(path_or_uri: str, relative_to: str) -> str:
+    """Return the absolute path if this isn't a URI, otherwise keep the URI the same."""
+    if "://" in path_or_uri:
+        return path_or_uri
+    abs_path_ = os.path.abspath(os.path.join(relative_to, path_or_uri))
+    _ensure_file_exists(abs_path_)
+    return abs_path_
 
 
-def abs_path(path_or_uri, relative_to):
-    path_or_uri = abs_path_or_uri(path_or_uri, relative_to)
+def abs_path(path_or_uri: str, relative_to: str) -> str:
+    """Return the absolute path if this is a file:// URI or a local path."""
     if path_or_uri.startswith("file://"):
-        path_or_uri = path_or_uri[len("file://") :]
-
-    return path_or_uri
+        # The path after file:// must be absolute
+        abs_path_ = path_or_uri[len("file://") :]
+    else:
+        index = path_or_uri.find("://")
+        if index != -1:
+            raise ValueError(f"Unsupported URI scheme: {path_or_uri[: index + 3]}")
+        abs_path_ = os.path.abspath(os.path.join(relative_to, path_or_uri))
+    _ensure_file_exists(abs_path_)
+    return abs_path_
 
 
-def path_or_uri_to_uri(path_or_uri):
+def path_or_uri_to_uri(path_or_uri: str) -> str:
     if "://" not in path_or_uri:
         return f"file://{path_or_uri}"
     else:
         return path_or_uri
 
 
-def galactic_job_json(job, test_data_directory, upload_func, collection_create_func, tool_or_workflow="workflow"):
+def galactic_job_json(
+    job: Dict[str, Any],
+    test_data_directory: str,
+    upload_func: Callable[["UploadTarget"], Dict[str, Any]],
+    collection_create_func: Callable[[List[Dict[str, Any]], str], Dict[str, Any]],
+    tool_or_workflow: Literal["tool", "workflow"] = "workflow",
+) -> Tuple[Dict[str, Any], List[Dict[str, Any]]]:
     """Adapt a CWL job object to the Galaxy API.
 
     CWL derived tools in Galaxy can consume a job description sort of like
     CWL job objects via the API but paths need to be replaced with datasets
     and records and arrays with collection references. This function will
     stage files and modify the job description to adapt to these changes
     for Galaxy.
     """
 
     datasets = []
     dataset_collections = []
 
-    def response_to_hda(target, upload_response):
+    def response_to_hda(target: UploadTarget, upload_response: Dict[str, Any]) -> Dict[str, str]:
         assert isinstance(upload_response, dict), upload_response
         assert "outputs" in upload_response, upload_response
         assert len(upload_response["outputs"]) > 0, upload_response
         dataset = upload_response["outputs"][0]
-        datasets.append((dataset, target))
+        datasets.append(dataset)
         dataset_id = dataset["id"]
         return {"src": "hda", "id": dataset_id}
 
-    def upload_file(file_path, secondary_files, **kwargs):
+    def upload_file(file_path: str, secondary_files: Optional[str], **kwargs) -> Dict[str, str]:
         file_path = abs_path_or_uri(file_path, test_data_directory)
         target = FileUploadTarget(file_path, secondary_files, **kwargs)
         upload_response = upload_func(target)
         return response_to_hda(target, upload_response)
 
-    def upload_file_literal(contents, **kwd):
+    def upload_file_literal(contents: str, **kwd) -> Dict[str, str]:
         target = FileLiteralTarget(contents, **kwd)
         upload_response = upload_func(target)
         return response_to_hda(target, upload_response)
 
-    def upload_tar(file_path):
+    def upload_tar(file_path: str) -> Dict[str, str]:
         file_path = abs_path_or_uri(file_path, test_data_directory)
         target = DirectoryUploadTarget(file_path)
         upload_response = upload_func(target)
         return response_to_hda(target, upload_response)
 
-    def upload_file_with_composite_data(file_path, composite_data, **kwargs):
+    def upload_file_with_composite_data(file_path: Optional[str], composite_data, **kwargs) -> Dict[str, str]:
         if file_path is not None:
             file_path = abs_path_or_uri(file_path, test_data_directory)
         composite_data_resolved = []
         for cd in composite_data:
             composite_data_resolved.append(abs_path_or_uri(cd, test_data_directory))
         target = FileUploadTarget(file_path, composite_data=composite_data_resolved, **kwargs)
         upload_response = upload_func(target)
         return response_to_hda(target, upload_response)
 
-    def upload_object(the_object):
+    def upload_object(the_object: Any) -> Dict[str, str]:
         target = ObjectUploadTarget(the_object)
         upload_response = upload_func(target)
         return response_to_hda(target, upload_response)
 
-    def replacement_item(value, force_to_file=False):
+    def replacement_item(value, force_to_file: bool = False):
         is_dict = isinstance(value, dict)
         item_class = None if not is_dict else value.get("class", None)
         is_file = item_class == "File"
         is_directory = item_class == "Directory"
         is_collection = item_class == "Collection"  # Galaxy extension.
 
         if force_to_file:
@@ -201,37 +219,39 @@
             return replacement_collection(value)
         else:
             return replacement_record(value)
 
     def replacement_file(value):
         if value.get("galaxy_id"):
             return {"src": "hda", "id": str(value["galaxy_id"])}
-        file_path = value.get("location", None) or value.get("path", None)
+        file_path = value.get("location") or value.get("path")
         # format to match output definitions in tool, where did filetype come from?
         filetype = value.get("filetype", None) or value.get("format", None)
         composite_data_raw = value.get("composite_data", None)
         kwd = {}
         if "tags" in value:
             kwd["tags"] = value.get("tags")
         if "dbkey" in value:
             kwd["dbkey"] = value.get("dbkey")
+        if "decompress" in value:
+            kwd["decompress"] = value["decompress"]
         if composite_data_raw:
             composite_data = []
             for entry in composite_data_raw:
                 path = None
                 if isinstance(entry, dict):
                     path = entry.get("location", None) or entry.get("path", None)
                 else:
                     path = entry
                 composite_data.append(path)
             rval_c = upload_file_with_composite_data(None, composite_data, filetype=filetype, **kwd)
             return rval_c
 
         if file_path is None:
-            contents = value.get("contents", None)
+            contents = value.get("contents")
             if contents is not None:
                 return upload_file_literal(contents, **kwd)
 
             return value
 
         secondary_files = value.get("secondaryFiles", [])
         secondary_files_tar_path = None
@@ -267,29 +287,29 @@
         tmp = tempfile.NamedTemporaryFile(delete=False)
         tf = tarfile.open(fileobj=tmp, mode="w:")
         tf.add(file_path, ".")
         tf.close()
 
         return upload_tar(tmp.name)
 
-    def replacement_list(value):
+    def replacement_list(value) -> Dict[str, str]:
         collection_element_identifiers = []
         for i, item in enumerate(value):
             dataset = replacement_item(item, force_to_file=True)
             collection_element = dataset.copy()
             collection_element["name"] = str(i)
             collection_element_identifiers.append(collection_element)
 
         # TODO: handle nested lists/arrays
         collection = collection_create_func(collection_element_identifiers, "list")
         dataset_collections.append(collection)
         hdca_id = collection["id"]
         return {"src": "hdca", "id": hdca_id}
 
-    def to_elements(value, rank_collection_type):
+    def to_elements(value, rank_collection_type: str) -> List[Dict[str, Any]]:
         collection_element_identifiers = []
         assert "elements" in value
         elements = value["elements"]
 
         is_nested_collection = ":" in rank_collection_type
         for element in elements:
             if not is_nested_collection:
@@ -307,15 +327,15 @@
                     "collection_type": sub_collection_type,
                     "element_identifiers": to_elements(element, sub_collection_type),
                 }
                 collection_element_identifiers.append(collection_element)
 
         return collection_element_identifiers
 
-    def replacement_collection(value):
+    def replacement_collection(value: Dict[str, Any]) -> Dict[str, str]:
         if value.get("galaxy_id"):
             return {"src": "hdca", "id": str(value["galaxy_id"])}
         assert "collection_type" in value
         collection_type = value["collection_type"]
         elements = to_elements(value, collection_type)
 
         collection = collection_create_func(elements, collection_type)
@@ -326,15 +346,15 @@
     def replacement_record(value):
         collection_element_identifiers = []
         for record_key, record_value in value.items():
             if not isinstance(record_value, dict) or record_value.get("class") != "File":
                 dataset = replacement_item(record_value, force_to_file=True)
                 collection_element = dataset.copy()
             else:
-                dataset = upload_file(record_value["location"], [])
+                dataset = upload_file(record_value["location"], None)
                 collection_element = dataset.copy()
 
             collection_element["name"] = record_key
             collection_element_identifiers.append(collection_element)
 
         collection = collection_create_func(collection_element_identifiers, "record")
         dataset_collections.append(collection)
@@ -345,102 +365,110 @@
     for key, value in job.items():
         replace_keys[key] = replacement_item(value)
 
     job.update(replace_keys)
     return job, datasets
 
 
-def _ensure_file_exists(file_path):
+def _ensure_file_exists(file_path: str) -> None:
     if not os.path.exists(file_path):
         template = "File [%s] does not exist - parent directory [%s] does %sexist, cwd is [%s]"
         parent_directory = os.path.dirname(file_path)
         message = template % (
             file_path,
             parent_directory,
             "" if os.path.exists(parent_directory) else "not ",
             os.getcwd(),
         )
         raise Exception(message)
 
 
-class FileLiteralTarget:
-    def __init__(self, contents, path=None, **kwargs):
+class UploadTarget:
+    @abc.abstractmethod
+    def __str__(self) -> str:
+        pass
+
+
+class FileLiteralTarget(UploadTarget):
+    def __init__(self, contents: str, **kwargs) -> None:
         self.contents = contents
         self.properties = kwargs
-        self.path = path
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"FileLiteralTarget[contents={self.contents}] with {self.properties}"
 
 
-class FileUploadTarget:
-    def __init__(self, path, secondary_files=None, **kwargs):
+class FileUploadTarget(UploadTarget):
+    def __init__(
+        self,
+        path: Optional[str],
+        secondary_files: Optional[str] = None,
+        composite_data: Optional[List[str]] = None,
+        **kwargs,
+    ) -> None:
         self.path = path
         self.secondary_files = secondary_files
-        self.composite_data = kwargs.get("composite_data", [])
+        self.composite_data = composite_data
         self.properties = kwargs
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"FileUploadTarget[path={self.path}] with {self.properties}"
 
 
-class ObjectUploadTarget:
-    def __init__(self, the_object):
+class ObjectUploadTarget(UploadTarget):
+    def __init__(self, the_object: Any) -> None:
         self.object = the_object
-        self.properties = {}
+        self.properties: Dict = {}
 
-    def __str__(self):
-        return f"ObjectUploadTarget[object={self.object} with {self.properties}]"
+    def __str__(self) -> str:
+        return f"ObjectUploadTarget[object={self.object}] with {self.properties}"
 
 
-class DirectoryUploadTarget:
-    def __init__(self, tar_path):
+class DirectoryUploadTarget(UploadTarget):
+    def __init__(self, tar_path: str) -> None:
         self.tar_path = tar_path
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"DirectoryUploadTarget[tar_path={self.tar_path}]"
 
 
 GalaxyOutput = namedtuple("GalaxyOutput", ["history_id", "history_content_type", "history_content_id", "metadata"])
 
 
-def tool_response_to_output(tool_response, history_id, output_id):
+def tool_response_to_output(tool_response, history_id, output_name):
     for output in tool_response["outputs"]:
-        if output["output_name"] == output_id:
+        if output["output_name"] == output_name:
             return GalaxyOutput(history_id, "dataset", output["id"], None)
 
     for output_collection in tool_response["output_collections"]:
-        if output_collection["output_name"] == output_id:
+        if output_collection["output_name"] == output_name:
             return GalaxyOutput(history_id, "dataset_collection", output_collection["id"], None)
 
-    raise Exception(f"Failed to find output with label [{output_id}]")
+    raise Exception(f"Failed to find output with label [{output_name}]")
 
 
-def invocation_to_output(invocation, history_id, output_id):
-    if output_id in invocation["outputs"]:
-        dataset = invocation["outputs"][output_id]
-        galaxy_output = GalaxyOutput(history_id, "dataset", dataset["id"], None)
-    elif output_id in invocation["output_collections"]:
-        collection = invocation["output_collections"][output_id]
-        galaxy_output = GalaxyOutput(history_id, "dataset_collection", collection["id"], None)
-    elif output_id in invocation["output_values"]:
-        output_value = invocation["output_values"][output_id]
-        galaxy_output = GalaxyOutput(None, "raw_value", output_value, None)
-    else:
-        raise Exception(f"Failed to find output with label [{output_id}] in [{invocation}]")
-
-    return galaxy_output
+def invocation_to_output(invocation, history_id, output_name):
+    if output_name in invocation["outputs"]:
+        dataset = invocation["outputs"][output_name]
+        return GalaxyOutput(history_id, "dataset", dataset["id"], None)
+    elif output_name in invocation["output_collections"]:
+        collection = invocation["output_collections"][output_name]
+        return GalaxyOutput(history_id, "dataset_collection", collection["id"], None)
+    elif output_name in invocation["output_values"]:
+        output_value = invocation["output_values"][output_name]
+        return GalaxyOutput(None, "raw_value", output_value, None)
+    raise Exception(f"Failed to find output with label [{output_name}] in [{invocation}]")
 
 
 def output_to_cwl_json(
     galaxy_output,
     get_metadata,
     get_dataset,
     get_extra_files,
-    pseduo_location=False,
+    pseudo_location=False,
 ):
     """Convert objects in a Galaxy history into a CWL object.
 
     Useful in running conformance tests and implementing the cwl-runner
     interface via Galaxy.
     """
 
@@ -455,15 +483,15 @@
         element_output = GalaxyOutput(
             galaxy_output.history_id,
             content_type,
             object["id"],
             metadata,
         )
         return output_to_cwl_json(
-            element_output, get_metadata, get_dataset, get_extra_files, pseduo_location=pseduo_location
+            element_output, get_metadata, get_dataset, get_extra_files, pseudo_location=pseudo_location
         )
 
     output_metadata = galaxy_output.metadata
     if output_metadata is None:
         output_metadata = get_metadata(galaxy_output.history_content_type, galaxy_output.history_content_id)
 
     def dataset_dict_to_json_content(dataset_dict):
@@ -482,15 +510,15 @@
             return dataset_dict_to_json_content(dataset_dict)
         else:
             file_or_directory = "Directory" if ext == "directory" else "File"
             secondary_files = []
 
             if file_or_directory == "File":
                 dataset_dict = get_dataset(output_metadata)
-                properties = output_properties(pseduo_location=pseduo_location, **dataset_dict)
+                properties = output_properties(pseudo_location=pseudo_location, **dataset_dict)
                 basename = properties["basename"]
                 extra_files = get_extra_files(output_metadata)
                 found_index = False
                 for extra_file in extra_files:
                     if extra_file["class"] == "File":
                         path = extra_file["path"]
                         if path == SECONDARY_FILES_INDEX_PATH:
@@ -508,15 +536,15 @@
                             extra_file_basename = os.path.basename(path)
                             if os.path.join(dir_path, extra_file_basename) != path:
                                 continue
 
                             if extra_file_class == "File":
                                 ec = get_dataset(output_metadata, filename=path)
                                 ec["basename"] = extra_file_basename
-                                ec_properties = output_properties(pseduo_location=pseduo_location, **ec)
+                                ec_properties = output_properties(pseudo_location=pseudo_location, **ec)
                             elif extra_file_class == "Directory":
                                 ec_properties = {}
                                 ec_properties["class"] = "Directory"
                                 ec_properties["location"] = ec_basename
                                 ec_properties["listing"] = dir_listing(path)
                             else:
                                 raise Exception("Unknown output type encountered....")
@@ -536,15 +564,15 @@
                                 ec_basename = basename + os.path.basename(path)
                             else:
                                 ec_basename = os.path.basename(path)
 
                             if extra_file_class == "File":
                                 ec = get_dataset(output_metadata, filename=path)
                                 ec["basename"] = ec_basename
-                                ec_properties = output_properties(pseduo_location=pseduo_location, **ec)
+                                ec_properties = output_properties(pseudo_location=pseudo_location, **ec)
                             elif extra_file_class == "Directory":
                                 ec_properties = {}
                                 ec_properties["class"] = "Directory"
                                 ec_properties["location"] = ec_basename
                                 ec_properties["listing"] = dir_listing(path)
                             else:
                                 raise Exception("Unknown output type encountered....")
@@ -564,15 +592,15 @@
 
                 extra_files = get_extra_files(output_metadata)
                 for extra_file in extra_files:
                     if extra_file["class"] == "File":
                         path = extra_file["path"]
                         ec = get_dataset(output_metadata, filename=path)
                         ec["basename"] = os.path.basename(path)
-                        ec_properties = output_properties(pseduo_location=pseduo_location, **ec)
+                        ec_properties = output_properties(pseudo_location=pseudo_location, **ec)
                         listing.append(ec_properties)
 
             if secondary_files:
                 properties["secondaryFiles"] = secondary_files
             return properties
 
     elif output_metadata["history_content_type"] == "dataset_collection":
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/__init__.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,14 @@
             tool_info_kwds["tool_version"] = tool.version
             tool_info_kwds["container_descriptions"] = tool.containers
             tool_info_kwds["requires_galaxy_python_environment"] = tool.requires_galaxy_python_environment
 
         tool_info = ToolInfo(**tool_info_kwds)
 
         for i, resolver in enumerate(self.dependency_resolvers):
-
             if index is not None and i != index:
                 continue
 
             if resolver_type is not None and resolver.resolver_type != resolver_type:
                 continue
 
             if container_type is not None and getattr(resolver, "container_type", None) != container_type:
@@ -300,15 +299,14 @@
                         log.debug(dependency.resolver_msg)
                         requirement_to_dependency[requirement] = dependency
 
                     # Shortcut - resolution complete.
                     break
 
             if not isinstance(resolver, ContainerResolver):
-
                 # Check individual requirements
                 for requirement in resolvable_requirements:
                     if requirement in _requirement_to_dependency:
                         continue
 
                     dependency = resolver.resolve(requirement, **kwds)
                     if require_exact and not dependency.exact:
@@ -427,15 +425,15 @@
 
     def hash_dependencies(self, resolved_dependencies):
         """Return hash for dependencies"""
         resolved_dependencies = [
             (dep.name, dep.version, dep.exact, dep.dependency_type) for dep in resolved_dependencies
         ]
         hash_str = json.dumps(sorted(resolved_dependencies))
-        return hash_util.new_secure_hash(hash_str)[:8]  # short hash
+        return hash_util.new_insecure_hash(hash_str)[:8]  # short hash
 
     def get_hashed_dependencies_path(self, resolved_dependencies):
         """
         Returns the path to the hashed dependencies directory (but does not evaluate whether the path exists).
 
         :param resolved_dependencies: list of resolved dependencies
         :type resolved_dependencies: list
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/brew_exts.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/brew_exts.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 import glob
 import json
 import os
 import re
 import string
 import subprocess
 import sys
+from typing import (
+    List,
+    Tuple,
+)
 
 WHITESPACE_PATTERN = re.compile(r"[\s]+")
 
 DESCRIPTION = "Script built on top of linuxbrew to operate on isolated, versioned brew installed environments."
 
 if sys.platform == "darwin":
     DEFAULT_HOMEBREW_ROOT = "/usr/local"
@@ -72,15 +76,15 @@
         self.brew_context = brew_context or BrewContext()
 
     @property
     def cellar_path(self):
         return recipe_cellar_path(self.brew_context.homebrew_cellar, self.recipe, self.version)
 
     @property
-    def tap_path(self):
+    def tap_path(self) -> str:
         return os.path.join(self.brew_context.homebrew_prefix, "Library", "Taps", self.__tap_path(self.recipe))
 
     def __tap_path(self, recipe):
         parts = recipe.split("/")
         if len(parts) == 1:
             info = brew_info(self.recipe)
             from_url = info["from_url"]
@@ -230,15 +234,15 @@
             with open(v_metadata_path, "w") as f:
                 json.dump(metadata, f)
 
         finally:
             attempt_unlink_all(package, deps)
 
 
-def commit_for_version(recipe_context, package, version):
+def commit_for_version(recipe_context: RecipeContext, package, version):
     tap_path = recipe_context.tap_path
     commit = None
     with brew_head_at_commit("master", tap_path):
         version_to_commit = brew_versions_info(package, tap_path)
         if version is None:
             version = version_to_commit[0][0]
             commit = version_to_commit[0][1]
@@ -316,15 +320,14 @@
     env_statements = []
     for action in actions:
         env_statements.extend(action.to_statements())
     return "\n".join(env_statements)
 
 
 def build_env_actions(deps, cellar_root, cellar_path, relaxed=None, custom_only=False):
-
     path_appends = []
     ld_path_appends = []
     actions = []
 
     def handle_keg(cellar_path):
         bin_path = os.path.join(cellar_path, "bin")
         if os.path.isdir(bin_path):
@@ -486,27 +489,27 @@
             if line.startswith(f"{dep_type}: "):
                 key = f"{dep_type.lower()}_dependencies"
                 raw_val = line[len(f"{dep_type}: ") :]
                 extra_info[key].extend(raw_val.split(", "))
     return extra_info
 
 
-def brew_versions_info(package, tap_path):
-    def versioned(recipe_path):
+def brew_versions_info(package, tap_path: str) -> List[Tuple[str, str, bool]]:
+    def versioned(recipe_path: str):
         if not os.path.isabs(recipe_path):
             recipe_path = os.path.join(os.getcwd(), recipe_path)
         # Dependencies in the same repository should be versioned,
         # core dependencies (presumably in base homebrew) are not
         # versioned.
         return tap_path in recipe_path
 
     # TODO: Also use tags.
     stdout = brew_execute(["versions", package])
     version_parts = [line for line in stdout.split("\n") if line and "git checkout" in line]
-    version_parts = map(lambda l: WHITESPACE_PATTERN.split(l), version_parts)
+    version_parts = [WHITESPACE_PATTERN.split(line) for line in version_parts]
     info = [(p[0], p[3], versioned(p[4])) for p in version_parts]
     return info
 
 
 def __action(sys):
     script_name = os.path.basename(sys.argv[0])
     if script_name.startswith("brew-"):
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/brew_util.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/brew_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ brew_exts defines generic extensions to Homebrew this file
 builds on those abstraction and provides Galaxy specific functionality
 not useful to the brew external commands.
 """
-from ..deps import brew_exts
+from . import brew_exts
 
 DEFAULT_TAP = "homebrew/science"
 
 
 class HomebrewRecipe:
     def __init__(self, recipe, version, tap):
         self.recipe = recipe
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/conda_compat.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/conda_compat.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/conda_util.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/conda_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,183 +4,206 @@
 import logging
 import os
 import re
 import shutil
 import sys
 import tempfile
 from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Iterator,
     List,
     Optional,
+    Tuple,
+    TYPE_CHECKING,
+    Union,
 )
 
 import packaging.version
 
 from galaxy.util import (
     commands,
+    download_to_file,
     listify,
     shlex_join,
     smart_str,
     which,
 )
 from . import installable
 
+if TYPE_CHECKING:
+    from galaxy.tool_util.deps.requirements import ToolRequirement
+
 log = logging.getLogger(__name__)
 
 # Not sure there are security concerns, lets just fail fast if we are going
 # break shell commands we are building.
 SHELL_UNSAFE_PATTERN = re.compile(r"[\s\"']")
 
 IS_OS_X = sys.platform == "darwin"
 
 VERSIONED_ENV_DIR_NAME = re.compile(r"__(.*)@(.*)")
 UNVERSIONED_ENV_DIR_NAME = re.compile(r"__(.*)@_uv_")
 USE_PATH_EXEC_DEFAULT = False
-CONDA_PACKAGE_SPECS = ("conda=4.6.14", "'pyopenssl>=22.1.0'")
-CONDA_BUILD_VERSION = "3.17.8"
+CONDA_PACKAGE_SPECS = ("conda>=22.9.0", "conda-libmamba-solver", "'pyopenssl>=22.1.0'")
+CONDA_BUILD_SPECS = ("conda-build>=3.22.0",)
 USE_LOCAL_DEFAULT = False
 
 
-def conda_link():
+def conda_link() -> str:
     if IS_OS_X:
-        url = "https://repo.anaconda.com/miniconda/Miniconda3-4.6.14-MacOSX-x86_64.sh"
+        url = "https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.sh"
     else:
         if sys.maxsize > 2**32:
-            url = "https://repo.anaconda.com/miniconda/Miniconda3-4.6.14-Linux-x86_64.sh"
+            url = "https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh"
         else:
             url = "https://repo.anaconda.com/miniconda/Miniconda3-4.5.12-Linux-x86.sh"
     return url
 
 
-def find_conda_prefix(conda_prefix=None):
+def find_conda_prefix() -> str:
     """If supplied conda_prefix is not set, default to the default location
     for Miniconda installs.
     """
-    if conda_prefix is None:
-        home = os.path.expanduser("~")
-        miniconda_2_dest = os.path.join(home, "miniconda2")
-        miniconda_3_dest = os.path.join(home, "miniconda3")
-        anaconda_2_dest = os.path.join(home, "anaconda2")
-        anaconda_3_dest = os.path.join(home, "anaconda3")
-        # Prefer miniconda3 install if both available
-        if os.path.exists(miniconda_3_dest):
-            return miniconda_3_dest
-        elif os.path.exists(miniconda_2_dest):
-            return miniconda_2_dest
-        elif os.path.exists(anaconda_3_dest):
-            return anaconda_3_dest
-        elif os.path.exists(anaconda_2_dest):
-            return anaconda_2_dest
-        else:
-            return miniconda_3_dest
-    return conda_prefix
+    home = os.path.expanduser("~")
+    miniconda_2_dest = os.path.join(home, "miniconda2")
+    miniconda_3_dest = os.path.join(home, "miniconda3")
+    anaconda_2_dest = os.path.join(home, "anaconda2")
+    anaconda_3_dest = os.path.join(home, "anaconda3")
+    # Prefer miniconda3 install if both available
+    if os.path.exists(miniconda_3_dest):
+        return miniconda_3_dest
+    elif os.path.exists(miniconda_2_dest):
+        return miniconda_2_dest
+    elif os.path.exists(anaconda_3_dest):
+        return anaconda_3_dest
+    elif os.path.exists(anaconda_2_dest):
+        return anaconda_2_dest
+    else:
+        return miniconda_3_dest
 
 
 class CondaContext(installable.InstallableContext):
     installable_description = "Conda"
+    _conda_build_available: Optional[bool]
+    _conda_version: Optional[Union[packaging.version.Version, packaging.version.LegacyVersion]]
+    _experimental_solver_available: Optional[bool]
 
     def __init__(
         self,
-        conda_prefix=None,
-        conda_exec=None,
-        shell_exec=None,
-        debug=False,
-        ensure_channels="",
-        condarc_override=None,
-        use_path_exec=USE_PATH_EXEC_DEFAULT,
-        copy_dependencies=False,
-        use_local=USE_LOCAL_DEFAULT,
-    ):
+        conda_prefix: Optional[str] = None,
+        conda_exec: Optional[str] = None,
+        shell_exec: Optional[Callable[..., int]] = None,
+        debug: bool = False,
+        ensure_channels: Union[str, List[str]] = "",
+        condarc_override: Optional[str] = None,
+        use_path_exec: bool = USE_PATH_EXEC_DEFAULT,
+        copy_dependencies: bool = False,
+        use_local: bool = USE_LOCAL_DEFAULT,
+    ) -> None:
         self.condarc_override = condarc_override
         if not conda_exec and use_path_exec:
             conda_exec = which("conda")
         if conda_exec and isinstance(conda_exec, str):
             conda_exec = os.path.normpath(conda_exec)
-        self.conda_exec = conda_exec
         self.debug = debug
         self.shell_exec = shell_exec or commands.shell
         self.copy_dependencies = copy_dependencies
 
+        if conda_exec is not None:
+            self.conda_exec = conda_exec
+            if conda_prefix is None:
+                info = self.conda_info()
+                conda_prefix = info.get("default_prefix")
         if conda_prefix is None:
-            info = self.conda_info()
-            if info and "default_prefix" in info:
-                conda_prefix = info["default_prefix"]
-        if conda_prefix is None:
-            conda_prefix = find_conda_prefix(conda_prefix)
+            conda_prefix = find_conda_prefix()
 
         self.conda_prefix = conda_prefix
         if conda_exec is None:
             self.conda_exec = self._bin("conda")
         self.ensure_channels: List[str] = listify(ensure_channels)
         self.use_local = use_local
         self._reset_conda_properties()
 
-    def _reset_conda_properties(self):
+    def _reset_conda_properties(self) -> None:
         self._conda_version = None
         self._conda_build_available = None
+        self._experimental_solver_available = None
 
     @property
-    def conda_version(self):
+    def conda_version(self) -> Union[packaging.version.Version, packaging.version.LegacyVersion]:
         if self._conda_version is None:
             self._guess_conda_properties()
+        assert isinstance(self._conda_version, (packaging.version.Version, packaging.version.LegacyVersion))
         return self._conda_version
 
     @property
-    def conda_build_available(self):
+    def conda_build_available(self) -> bool:
         if self._conda_build_available is None:
             self._guess_conda_properties()
+        assert isinstance(self._conda_build_available, bool)
         return self._conda_build_available
 
-    def _guess_conda_properties(self):
+    def _guess_conda_properties(self) -> None:
         info = self.conda_info()
         self._conda_version = packaging.version.parse(info["conda_version"])
         self._conda_build_available = False
         conda_build_version = info.get("conda_build_version")
         if conda_build_version and conda_build_version != "not installed":
             try:
                 packaging.version.parse(conda_build_version)
                 self._conda_build_available = True
             except Exception:
                 pass
 
     @property
-    def _override_channels_args(self):
+    def _override_channels_args(self) -> List[str]:
         override_channels_args = []
         if self.ensure_channels:
             override_channels_args.append("--override-channels")
             for channel in self.ensure_channels:
                 override_channels_args.extend(["--channel", channel])
         return override_channels_args
 
-    def ensure_conda_build_installed_if_needed(self):
+    @property
+    def _experimental_solver_args(self) -> List[str]:
+        if self._experimental_solver_available is None:
+            self._experimental_solver_available = self.conda_version >= packaging.version.parse(
+                "4.12.0"
+            ) and self.is_package_installed("conda-libmamba-solver")
+        if self._experimental_solver_available:
+            return ["--experimental-solver", "libmamba"]
+        else:
+            return []
+
+    def ensure_conda_build_installed_if_needed(self) -> int:
         if self.use_local and not self.conda_build_available:
-            conda_targets = [CondaTarget("conda-build", version=CONDA_BUILD_VERSION)]
             # Cannot use --use-local during installation of conda-build.
-            return install_conda_targets(conda_targets, conda_context=self, env_name=None, allow_local=False)
+            return self.exec_install(CONDA_BUILD_SPECS, allow_local=False)
         else:
             return 0
 
-    def conda_info(self):
-        if self.conda_exec is not None:
-            cmd = listify(self.conda_exec) + ["info", "--json"]
-            info_out = commands.execute(cmd)
-            info = json.loads(info_out)
-            return info
-        else:
-            return None
+    def conda_info(self) -> Dict[str, Any]:
+        cmd = listify(self.conda_exec) + ["info", "--json"]
+        info_out = commands.execute(cmd)
+        info = json.loads(info_out)
+        return info
 
-    def is_conda_installed(self):
+    def is_conda_installed(self) -> bool:
         """
         Check if conda_exec exists
         """
         if os.path.exists(self.conda_exec):
             return True
         else:
             return False
 
-    def can_install_conda(self):
+    def can_install_conda(self) -> bool:
         """
         If conda_exec is set to a path outside of conda_prefix,
         there is no use installing conda into conda_prefix, since it can't be used by galaxy.
         If conda_exec equals conda_prefix/bin/conda, we can install conda if either conda_prefix
         does not exist or is empty.
         """
         conda_exec = os.path.abspath(self.conda_exec)
@@ -201,15 +224,15 @@
                 "Skipping installation of Conda into conda_prefix '%s', "
                 "since conda_exec '%s' is set to a path outside of conda_prefix.",
                 self.conda_prefix,
                 self.conda_exec,
             )
             return False
 
-    def exec_command(self, operation, args, stdout_path=None):
+    def exec_command(self, operation: str, args: List[str], stdout_path: Optional[str] = None) -> int:
         """
         Execute the requested command.
 
         Return the process exit code (i.e. 0 in case of success).
         """
         cmd = listify(self.conda_exec) + operation.split()
         if self.debug:
@@ -234,81 +257,99 @@
             return 1
         finally:
             if kwds.get("stdout"):
                 kwds["stdout"].close()
             if conda_exec_home:
                 shutil.rmtree(conda_exec_home, ignore_errors=True)
 
-    def exec_create(self, args, allow_local=True, stdout_path=None):
+    def is_package_installed(self, pkg_name: str, version: Optional[str] = None) -> bool:
+        list_args = ["-f", "--json", pkg_name]
+        with tempfile.NamedTemporaryFile("r") as temp:
+            ret = self.exec_command("list", list_args, stdout_path=temp.name)
+            if ret != 0:
+                log.error("Failed to execute 'conda list'")
+                return False
+            out = json.load(temp)
+        if not out:
+            return False
+        if not version:
+            return True
+        return any(match["version"] == version for match in out)
+
+    def exec_create(self, args: Iterable[str], allow_local: bool = True, stdout_path: Optional[str] = None) -> int:
         """
         Return the process exit code (i.e. 0 in case of success).
         """
         for try_strict in [True, False]:
             create_args = ["-y", "--quiet"]
             if try_strict:
                 if self.conda_version >= packaging.version.parse("4.7.5"):
                     create_args.append("--strict-channel-priority")
                 else:
                     continue
             if allow_local and self.use_local:
                 create_args.append("--use-local")
+            create_args.extend(self._experimental_solver_args)
             create_args.extend(self._override_channels_args)
             create_args.extend(args)
             ret = self.exec_command("create", create_args, stdout_path=stdout_path)
             if ret == 0:
                 break
         return ret
 
-    def exec_remove(self, args):
+    def exec_remove(self, args: List[str]) -> int:
         """
         Remove a conda environment using conda env remove -y --name `args`.
 
         Return the process exit code (i.e. 0 in case of success).
         """
         remove_args = ["-y", "--name"]
         remove_args.extend(args)
         return self.exec_command("env remove", remove_args)
 
-    def exec_install(self, args, allow_local=True, stdout_path=None):
+    def exec_install(self, args: Iterable[str], allow_local: bool = True, stdout_path: Optional[str] = None) -> int:
         """
         Return the process exit code (i.e. 0 in case of success).
         """
         for try_strict in [True, False]:
             install_args = ["-y"]
             if try_strict:
                 if self.conda_version >= packaging.version.parse("4.7.5"):
                     install_args.append("--strict-channel-priority")
                 else:
                     continue
             if allow_local and self.use_local:
                 install_args.append("--use-local")
+            install_args.extend(self._experimental_solver_args)
             install_args.extend(self._override_channels_args)
             install_args.extend(args)
             ret = self.exec_command("install", install_args, stdout_path=stdout_path)
             if ret == 0:
                 break
         if ret == 0:
             self._reset_conda_properties()
         return ret
 
-    def exec_clean(self, args=None, quiet=False):
+    def exec_clean(self, args: Optional[List[str]] = None, quiet: bool = False) -> int:
         """
         Clean up after conda installation.
 
         Return the process exit code (i.e. 0 in case of success).
         """
         clean_args = ["--tarballs", "-y"]
         if args:
             clean_args.extend(args)
         stdout_path = None
         if quiet:
             stdout_path = "/dev/null"
         return self.exec_command("clean", clean_args, stdout_path=stdout_path)
 
-    def exec_search(self, args: List[str], json: bool = False, offline: bool = False, platform: Optional[str] = None):
+    def exec_search(
+        self, args: List[str], json: bool = False, offline: bool = False, platform: Optional[str] = None
+    ) -> str:
         """
         Search conda channels for a package
 
         Return the standard output of the conda process.
         """
         cmd = listify(self.conda_exec)[:]
         cmd.append("search")
@@ -318,161 +359,160 @@
         if offline:
             cmd.append("--offline")
         if platform:
             cmd.extend(["--platform", platform])
         cmd.extend(args)
         return commands.execute(cmd)
 
-    def export_list(self, name, path):
+    def export_list(self, name: str, path: str) -> int:
         """
         Return the process exit code (i.e. 0 in case of success).
         """
         return self.exec_command("list", ["--name", name, "--export"], stdout_path=path)
 
-    def env_path(self, env_name):
+    def env_path(self, env_name: str) -> str:
         return os.path.join(self.envs_path, env_name)
 
     @property
-    def envs_path(self):
+    def envs_path(self) -> str:
         return os.path.join(self.conda_prefix, "envs")
 
-    def has_env(self, env_name):
+    def has_env(self, env_name: str) -> bool:
         env_path = self.env_path(env_name)
         return os.path.isdir(env_path)
 
     @property
-    def deactivate(self):
+    def deactivate(self) -> str:
         return self._bin("deactivate")
 
     @property
-    def activate(self):
+    def activate(self) -> str:
         return self._bin("activate")
 
-    def is_installed(self):
+    def is_installed(self) -> bool:
         return self.is_conda_installed()
 
-    def can_install(self):
+    def can_install(self) -> bool:
         return self.can_install_conda()
 
     @property
-    def parent_path(self):
+    def parent_path(self) -> str:
         return os.path.dirname(os.path.abspath(self.conda_prefix))
 
-    def _bin(self, name):
+    def _bin(self, name: str) -> str:
         return os.path.join(self.conda_prefix, "bin", name)
 
 
-def installed_conda_targets(conda_context):
+def installed_conda_targets(conda_context: CondaContext) -> Iterator["CondaTarget"]:
     envs_path = conda_context.envs_path
     dir_contents = os.listdir(envs_path) if os.path.exists(envs_path) else []
     for name in dir_contents:
         versioned_match = VERSIONED_ENV_DIR_NAME.match(name)
         if versioned_match:
             yield CondaTarget(versioned_match.group(1), versioned_match.group(2))
 
         unversioned_match = UNVERSIONED_ENV_DIR_NAME.match(name)
         if unversioned_match:
             yield CondaTarget(unversioned_match.group(1))
 
 
 class CondaTarget:
-    def __init__(self, package, version=None, channel=None):
+    def __init__(self, package: str, version: Optional[str] = None, channel: Optional[str] = None) -> None:
         if SHELL_UNSAFE_PATTERN.search(package) is not None:
             raise ValueError(f"Invalid package [{package}] encountered.")
         self.package = package
         if version and SHELL_UNSAFE_PATTERN.search(version) is not None:
             raise ValueError(f"Invalid version [{version}] encountered.")
         self.version = version
         if channel and SHELL_UNSAFE_PATTERN.search(channel) is not None:
             raise ValueError(f"Invalid version [{channel}] encountered.")
         self.channel = channel
 
-    def __str__(self):
+    def __str__(self) -> str:
         attributes = f"package={self.package}"
         if self.version is not None:
             attributes = f"{self.package},version={self.version}"
         else:
             attributes = f"{self.package},unversioned"
 
         if self.channel:
             attributes = "%s,channel=%s" % self.channel
 
         return f"CondaTarget[{attributes}]"
 
     __repr__ = __str__
 
     @property
-    def package_specifier(self):
+    def package_specifier(self) -> str:
         """Return a package specifier as consumed by conda install/create."""
         if self.version:
             return f"{self.package}={self.version}"
         else:
             return self.package
 
     @property
-    def install_environment(self):
+    def install_environment(self) -> str:
         """The dependency resolution and installation frameworks will
         expect each target to be installed it its own environment with
         a fixed and predictable name given package and version.
         """
         if self.version:
             return f"__{self.package}@{self.version}"
         else:
             return f"__{self.package}@_uv_"
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash((self.package, self.version, self.channel))
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         if isinstance(other, self.__class__):
             return (self.package, self.version, self.channel) == (other.package, other.version, other.channel)
         return False
 
-    def __ne__(self, other):
-        return not (self == other)
 
-
-def hash_conda_packages(conda_packages, conda_target=None):
+def hash_conda_packages(conda_packages: Iterable[CondaTarget]) -> str:
     """Produce a unique hash on supplied packages.
     TODO: Ideally we would do this in such a way that preserved environments.
     """
     h = hashlib.new("sha256")
     for conda_package in conda_packages:
         h.update(smart_str(conda_package.install_environment))
     return h.hexdigest()
 
 
 # shell makes sense for planemo, in Galaxy this should just execute
 # these commands as Python
-def install_conda(conda_context, force_conda_build=False):
+def install_conda(conda_context: CondaContext, force_conda_build: bool = False) -> int:
     with tempfile.NamedTemporaryFile(suffix=".sh", prefix="conda_install", delete=False) as temp:
         script_path = temp.name
-    download_cmd = commands.download_command(conda_link(), to=script_path)
     install_cmd = ["bash", script_path, "-b", "-p", conda_context.conda_prefix]
     package_targets = list(CONDA_PACKAGE_SPECS)
     if force_conda_build or conda_context.use_local:
-        package_targets.append(f"conda-build={CONDA_BUILD_VERSION}")
+        package_targets.extend(CONDA_BUILD_SPECS)
     log.info("Installing conda, this may take several minutes.")
     try:
-        exit_code = conda_context.shell_exec(download_cmd)
-        if exit_code:
-            return exit_code
+        download_to_file(conda_link(), script_path)
         exit_code = conda_context.shell_exec(install_cmd)
     except Exception:
         log.exception("Failed to install conda")
         return 1
     finally:
         if os.path.exists(script_path):
             os.remove(script_path)
     if exit_code:
         return exit_code
     return conda_context.exec_install(package_targets, allow_local=False)
 
 
-def install_conda_targets(conda_targets, conda_context, env_name=None, allow_local=True):
+def install_conda_targets(
+    conda_targets: Iterable[CondaTarget],
+    conda_context: CondaContext,
+    env_name: Optional[str] = None,
+    allow_local: bool = True,
+) -> int:
     """
     Return the process exit code (i.e. 0 in case of success).
     """
     if env_name is not None:
         create_args = [
             "--name",
             env_name,  # environment for package
@@ -480,15 +520,15 @@
         for conda_target in conda_targets:
             create_args.append(conda_target.package_specifier)
         return conda_context.exec_create(create_args, allow_local=allow_local)
     else:
         return conda_context.exec_install([t.package_specifier for t in conda_targets], allow_local=allow_local)
 
 
-def install_conda_target(conda_target, conda_context, skip_environment=False):
+def install_conda_target(conda_target: CondaTarget, conda_context: CondaContext, skip_environment: bool = False) -> int:
     """
     Install specified target into a its own environment.
 
     Return the process exit code (i.e. 0 in case of success).
     """
     if not skip_environment:
         create_args = [
@@ -497,30 +537,33 @@
             conda_target.package_specifier,
         ]
         return conda_context.exec_create(create_args)
     else:
         return conda_context.exec_install([conda_target.package_specifier])
 
 
-def cleanup_failed_install_of_environment(env, conda_context):
+def cleanup_failed_install_of_environment(env: str, conda_context: CondaContext) -> int:
     if conda_context.has_env(env):
-        conda_context.exec_remove([env])
+        return conda_context.exec_remove([env])
+    return 0
 
 
-def cleanup_failed_install(conda_target, conda_context=None):
-    cleanup_failed_install_of_environment(conda_target.install_environment, conda_context=conda_context)
+def cleanup_failed_install(conda_target: CondaTarget, conda_context: CondaContext) -> int:
+    return cleanup_failed_install_of_environment(conda_target.install_environment, conda_context=conda_context)
 
 
 def best_search_result(
-    conda_target, conda_context: CondaContext, offline: bool = False, platform: Optional[str] = None
-):
+    conda_target: CondaTarget, conda_context: CondaContext, offline: bool = False, platform: Optional[str] = None
+) -> Union[Tuple[None, None], Tuple[Dict[str, Any], bool]]:
     """Find best "conda search" result for specified target.
 
     Return ``None`` if no results match.
     """
+    # Cannot specify the version here (i.e. conda_target.package_specifier)
+    # because if the version is not found, the exec_search() call would fail.
     search_args = [conda_target.package]
     try:
         res = conda_context.exec_search(search_args, json=True, offline=offline, platform=platform)
         # Use python's stable list sorting to sort by date,
         # then build_number, then version. The top of the list
         # then is the newest version with the newest build and
         # the latest update time.
@@ -540,41 +583,37 @@
         if is_search_hit_exact(conda_target, hit):
             best_result = (hit, True)
             break
 
     return best_result
 
 
-def is_search_hit_exact(conda_target, search_hit):
+def is_search_hit_exact(conda_target: CondaTarget, search_hit: Dict[str, Any]) -> bool:
     target_version = conda_target.version
     # It'd be nice to make request verson of 1.0 match available
     # version of 1.0.3 or something like that.
-    return not target_version or search_hit["version"] == target_version
+    return bool(not target_version or search_hit["version"] == target_version)
 
 
-def is_conda_target_installed(conda_target, conda_context):
-    # fail by default
-    if conda_context.has_env(conda_target.install_environment):
-        return True
-    else:
-        return False
+def is_conda_target_installed(conda_target: CondaTarget, conda_context: CondaContext) -> bool:
+    return conda_context.has_env(conda_target.install_environment)
 
 
-def filter_installed_targets(conda_targets, conda_context):
+def filter_installed_targets(conda_targets: Iterable[CondaTarget], conda_context: CondaContext) -> List[CondaTarget]:
     installed = functools.partial(is_conda_target_installed, conda_context=conda_context)
     return list(filter(installed, conda_targets))
 
 
 def build_isolated_environment(
-    conda_packages,
-    conda_context,
-    path=None,
-    copy=False,
-    quiet=False,
-):
+    conda_packages: Union[CondaTarget, List[CondaTarget]],
+    conda_context: CondaContext,
+    path: Optional[str] = None,
+    copy: bool = False,
+    quiet: bool = False,
+) -> Tuple[str, int]:
     """Build a new environment (or reuse an existing one from hashes)
     for specified conda packages.
     """
     if not isinstance(conda_packages, list):
         conda_packages = [conda_packages]
 
     # Lots we could do in here, hashing, checking revisions, etc...
@@ -595,17 +634,17 @@
         # Adjust fix if they fix Conda - xref
         # - https://github.com/galaxyproject/galaxy/issues/3635
         # - https://github.com/conda/conda/issues/2035
         offline_works = (conda_context.conda_version < packaging.version.parse("4.3")) or (
             conda_context.conda_version >= packaging.version.parse("4.4")
         )
         if offline_works:
-            create_args.extend(["--offline"])
+            create_args.append("--offline")
         else:
-            create_args.extend(["--use-index-cache"])
+            create_args.append("--use-index-cache")
         if path is None:
             create_args.extend(["--name", tempdir_name])
         else:
             create_args.extend(["--prefix", path])
 
         if copy:
             create_args.append("--copy")
@@ -624,22 +663,22 @@
         return (path or tempdir_name, exit_code)
     finally:
         conda_context.exec_clean(quiet=quiet)
         if tempdir is not None:
             shutil.rmtree(tempdir)
 
 
-def requirement_to_conda_targets(requirement):
+def requirement_to_conda_targets(requirement: "ToolRequirement") -> Optional[CondaTarget]:
     conda_target = None
     if requirement.type == "package":
         conda_target = CondaTarget(requirement.name, version=requirement.version)
     return conda_target
 
 
-def requirements_to_conda_targets(requirements):
+def requirements_to_conda_targets(requirements: Iterable["ToolRequirement"]) -> List[CondaTarget]:
     conda_targets = (requirement_to_conda_targets(_) for _ in requirements)
     return [c for c in conda_targets if c is not None]
 
 
 __all__ = (
     "CondaContext",
     "CondaTarget",
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/container_classes.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/container_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,14 @@
                 end_index = len(volumes_str)
             volumes_str = volumes_str[0:tool_directory_index] + volumes_str[end_index : len(volumes_str)]
 
         return volumes_str
 
 
 class DockerContainer(Container, HasDockerLikeVolumes):
-
     container_type = DOCKER_CONTAINER_TYPE
 
     @property
     def docker_host_props(self):
         docker_host_props = dict(
             docker_cmd=self.prop("cmd", docker_util.DEFAULT_DOCKER_COMMAND),
             sudo=asbool(self.prop("sudo", docker_util.DEFAULT_SUDO)),
@@ -379,15 +378,14 @@
 def docker_cache_path(cache_directory, container_id):
     file_container_id = container_id.replace("/", "_slash_")
     cache_file_name = f"docker_{file_container_id}.tar"
     return os.path.join(cache_directory, cache_file_name)
 
 
 class SingularityContainer(Container, HasDockerLikeVolumes):
-
     container_type = SINGULARITY_CONTAINER_TYPE
 
     def get_singularity_target_kwds(self):
         return dict(
             singularity_cmd=self.prop("cmd", singularity_util.DEFAULT_SINGULARITY_COMMAND),
             sudo=asbool(self.prop("sudo", singularity_util.DEFAULT_SUDO)),
             sudo_cmd=self.prop("sudo_cmd", singularity_util.DEFAULT_SUDO_COMMAND),
@@ -407,15 +405,14 @@
 
     def build_singularity_pull_command(self, cache_path):
         return singularity_util.pull_singularity_command(
             image_identifier=self.container_id, cache_path=cache_path, **self.get_singularity_target_kwds()
         )
 
     def containerize_command(self, command):
-
         env = []
         for pass_through_var in self.tool_info.env_pass_through:
             env.append((pass_through_var, f"${pass_through_var}"))
 
         # Allow destinations to explicitly set environment variables just for
         # docker container. Better approach is to set for destination and then
         # pass through only what tool needs however. (See todo in ToolInfo.)
@@ -447,20 +444,7 @@
         return run_command
 
 
 CONTAINER_CLASSES = dict(
     docker=DockerContainer,
     singularity=SingularityContainer,
 )
-
-
-class NullContainer:
-    def __init__(self):
-        pass
-
-    def __bool__(self):
-        return False
-
-    __nonzero__ = __bool__
-
-
-NULL_CONTAINER = NullContainer()
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/container_resolvers/__init__.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/container_resolvers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """The module defines the abstract interface for resolving container images for tool execution."""
 from abc import (
     ABCMeta,
     abstractmethod,
     abstractproperty,
 )
 from typing import (
+    Any,
     Optional,
     TYPE_CHECKING,
 )
 
 from galaxy.util.bunch import Bunch
 from galaxy.util.dictifiable import Dictifiable
 
 if TYPE_CHECKING:
     from beaker.cache import Cache
 
+    from ..dependencies import AppInfo
+
 
 class ResolutionCache(Bunch):
     """Simple cache for duplicated computation created once per set of requests (likely web request in Galaxy context).
 
     This should not be assumed to be thread safe - resolution using a given cache should all occur
     one resolution at a time in a single thread.
     """
@@ -31,25 +34,25 @@
 
     # Keys for dictification.
     dict_collection_visible_keys = ["resolver_type", "can_uninstall_dependencies", "builds_on_resolution"]
     can_uninstall_dependencies = False
     builds_on_resolution = False
     read_only = True  # not used for containers, but set for when they are used like dependency resolvers
 
-    def __init__(self, app_info=None, **kwds):
+    def __init__(self, app_info: Optional["AppInfo"] = None, **kwds) -> None:
         """Default initializer for ``ContainerResolver`` subclasses."""
         self.app_info = app_info
         self.resolver_kwds = kwds
 
-    def _get_config_option(self, key, default=None):
+    def _get_config_option(self, key: str, default: Any = None) -> Any:
         """Look in resolver-specific settings for option and then fallback to
         global settings.
         """
-        if self.app_info and hasattr(self.app_info, key):
-            return getattr(self.app_info, key)
+        if self.app_info:
+            return getattr(self.app_info, key, default)
         else:
             return default
 
     @abstractmethod
     def resolve(self, enabled_container_types, tool_info, resolution_cache=None, **kwds):
         """Find a container matching all supplied requirements for tool.
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/container_resolvers/explicit.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/container_resolvers/explicit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """This module describes the :class:`ExplicitContainerResolver` ContainerResolver plugin."""
+import copy
 import logging
 import os
 from typing import cast
 
 from galaxy.util.commands import shell
+from . import ContainerResolver
 from .mulled import CliContainerResolver
 from ..container_classes import SingularityContainer
-from ..container_resolvers import ContainerResolver
 from ..requirements import ContainerDescription
 
 log = logging.getLogger(__name__)
 
 DEFAULT_SHELL = "/bin/bash"
 
 
@@ -30,15 +31,14 @@
                 container_description.explicit = True
                 return container_description
 
         return None
 
 
 class ExplicitSingularityContainerResolver(ExplicitContainerResolver):
-
     resolver_type = "explicit_singularity"
     container_type = "singularity"
 
     def resolve(self, enabled_container_types, tool_info, **kwds):
         """Find a container explicitly mentioned in tool description.
 
         This ignores the tool requirements and assumes the tool author crafted
@@ -76,19 +76,18 @@
         """Find a container explicitly mentioned in tool description.
 
         This ignores the tool requirements and assumes the tool author crafted
         a correct container. We use singularity here to fetch docker containers,
         hence the container_description hack here.
         """
         for container_description in tool_info.container_descriptions:  # type: ContainerDescription
+            container_description = copy.copy(container_description)
             if container_description.type == "docker":
-                desc_dict = container_description.to_dict()
-                desc_dict["type"] = self.container_type
-                desc_dict["identifier"] = f"docker://{container_description.identifier}"
-                container_description = container_description.from_dict(desc_dict)
+                container_description.type = self.container_type
+                container_description.identifier = f"docker://{container_description.identifier}"
             if not self._container_type_enabled(container_description, enabled_container_types):
                 return None
             if not self.cli_available:
                 return container_description
             image_id = cast(str, container_description.identifier)
             cache_path = os.path.normpath(os.path.join(self.cache_directory_path, image_id))
             if install and not os.path.exists(cache_path):
@@ -156,39 +155,35 @@
     """Specify an explicit, identified container as a Singularity container resolver."""
 
     resolver_type = "fallback_singularity"
     container_type = "singularity"
 
 
 class FallbackNoRequirementsContainerResolver(FallbackContainerResolver):
-
     resolver_type = "fallback_no_requirements"
 
     def _match(self, enabled_container_types, tool_info, container_description):
         type_matches = super()._match(enabled_container_types, tool_info, container_description)
         return type_matches and (tool_info.requirements is None or len(tool_info.requirements) == 0)
 
 
 class FallbackNoRequirementsSingularityContainerResolver(FallbackNoRequirementsContainerResolver):
-
     resolver_type = "fallback_no_requirements_singularity"
     container_type = "singularity"
 
 
 class RequiresGalaxyEnvironmentContainerResolver(FallbackContainerResolver):
-
     resolver_type = "requires_galaxy_environment"
 
     def _match(self, enabled_container_types, tool_info, container_description):
         type_matches = super()._match(enabled_container_types, tool_info, container_description)
         return type_matches and tool_info.requires_galaxy_python_environment
 
 
 class RequiresGalaxyEnvironmentSingularityContainerResolver(RequiresGalaxyEnvironmentContainerResolver):
-
     resolver_type = "requires_galaxy_environment_singularity"
     container_type = "singularity"
 
 
 class MappingContainerResolver(BaseAdminConfiguredContainerResolver):
     resolver_type = "mapping"
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/container_resolvers/mulled.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/container_resolvers/mulled.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 from abc import (
     ABCMeta,
     abstractmethod,
 )
 from typing import (
     NamedTuple,
     Optional,
+    TYPE_CHECKING,
 )
 
 from galaxy.util import (
     safe_makedirs,
     string_as_bool,
     unicodify,
     which,
 )
 from galaxy.util.commands import shell
-from ..container_classes import CONTAINER_CLASSES
-from ..container_resolvers import (
+from . import (
     ContainerResolver,
     ResolutionCache,
 )
+from ..container_classes import CONTAINER_CLASSES
 from ..docker_util import build_docker_images_command
 from ..mulled.mulled_build import (
     DEFAULT_CHANNELS,
     ensure_installed,
     InvolucroContext,
     mull_targets,
 )
@@ -41,14 +42,17 @@
     version_sorted,
 )
 from ..requirements import (
     ContainerDescription,
     DEFAULT_CONTAINER_SHELL,
 )
 
+if TYPE_CHECKING:
+    from ..dependencies import AppInfo
+
 log = logging.getLogger(__name__)
 
 
 class CachedMulledImageSingleTarget(NamedTuple):
     package_name: str
     version: str
     build: str
@@ -415,15 +419,14 @@
     if name is None:
         unresolved_cache.add(name)
 
     return name
 
 
 class CliContainerResolver(ContainerResolver):
-
     container_type = "docker"
     cli = "docker"
 
     def __init__(self, *args, **kwargs):
         self._cli_available = bool(which(self.cli))
         super().__init__(*args, **kwargs)
 
@@ -437,15 +440,14 @@
             log.info(
                 f"{self.cli} CLI not available, cannot list or pull images in Galaxy process. Does not impact kubernetes."
             )
         self._cli_available = value
 
 
 class SingularityCliContainerResolver(CliContainerResolver):
-
     container_type = "singularity"
     cli = "singularity"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.cache_directory_path = kwargs.get(
             "cache_directory", os.path.join(kwargs["app_info"].container_image_cache_path, "singularity", "mulled")
@@ -457,15 +459,14 @@
     def _init_cache_directory(self):
         cacher_class = get_cache_directory_cacher(self.cache_directory_cacher_type)
         self.cache_directory = cacher_class(self.cache_directory_path, hash_func=self.hash_func)
         safe_makedirs(self.cache_directory.path)
 
 
 class CachedMulledDockerContainerResolver(CliContainerResolver):
-
     resolver_type = "cached_mulled"
     shell = "/bin/bash"
 
     def __init__(self, app_info=None, namespace="biocontainers", hash_func="v2", **kwds):
         super().__init__(app_info=app_info, **kwds)
         self.namespace = namespace
         self.hash_func = hash_func
@@ -486,15 +487,14 @@
         )
 
     def __str__(self):
         return f"CachedMulledDockerContainerResolver[namespace={self.namespace}]"
 
 
 class CachedMulledSingularityContainerResolver(SingularityCliContainerResolver):
-
     resolver_type = "cached_mulled_singularity"
     shell = "/bin/bash"
 
     def __init__(self, app_info=None, hash_func="v2", **kwds):
         super().__init__(app_info=app_info, **kwds)
         self.hash_func = hash_func
         self._init_cache_directory()
@@ -603,15 +603,14 @@
             return container_description
 
     def __str__(self):
         return f"MulledDockerContainerResolver[namespace={self.namespace}]"
 
 
 class MulledSingularityContainerResolver(SingularityCliContainerResolver, MulledDockerContainerResolver):
-
     resolver_type = "mulled_singularity"
     protocol = "docker://"
 
     def __init__(self, app_info=None, namespace="biocontainers", hash_func="v2", auto_install=True, **kwds):
         super().__init__(app_info=app_info, **kwds)
         self.namespace = namespace
         self.hash_func = hash_func
@@ -643,93 +642,96 @@
 class BuildMulledDockerContainerResolver(CliContainerResolver):
     """Build for Docker mulled images matching tool dependencies."""
 
     resolver_type = "build_mulled"
     shell = "/bin/bash"
     builds_on_resolution = True
 
-    def __init__(self, app_info=None, namespace="local", hash_func="v2", auto_install=True, **kwds):
+    def __init__(
+        self,
+        app_info: Optional["AppInfo"] = None,
+        namespace: str = "local",
+        hash_func: str = "v2",
+        auto_install: bool = True,
+        **kwds,
+    ) -> None:
         super().__init__(app_info=app_info, **kwds)
         self._involucro_context_kwds = {"involucro_bin": self._get_config_option("involucro_path", None)}
         self.namespace = namespace
         self.hash_func = hash_func
         self.auto_install = string_as_bool(auto_install)
         self._mulled_kwds = {
             "namespace": namespace,
             "hash_func": self.hash_func,
             "command": "build-and-test",
         }
         self._mulled_kwds["channels"] = default_mulled_conda_channels_from_env() or self._get_config_option(
             "mulled_channels", DEFAULT_CHANNELS
         )
-        self.auto_init = self._get_config_option("involucro_auto_init", True)
+        self.involucro_context = InvolucroContext(**self._involucro_context_kwds)
+        auto_init = self._get_config_option("involucro_auto_init", True)
+        self.enabled = ensure_installed(self.involucro_context, auto_init)
 
     def resolve(self, enabled_container_types, tool_info, install=False, **kwds):
         if tool_info.requires_galaxy_python_environment or self.container_type not in enabled_container_types:
             return None
 
         targets = mulled_targets(tool_info)
         log.debug(f"Image name for tool {tool_info.tool_id}: {image_name(targets, self.hash_func)}")
         if len(targets) == 0:
             return None
         if self.auto_install or install:
-            mull_targets(targets, involucro_context=self._get_involucro_context(), **self._mulled_kwds)
+            mull_targets(targets, involucro_context=self.involucro_context, **self._mulled_kwds)
         return docker_cached_container_description(targets, self.namespace, hash_func=self.hash_func, shell=self.shell)
 
-    def _get_involucro_context(self):
-        involucro_context = InvolucroContext(**self._involucro_context_kwds)
-        self.enabled = ensure_installed(involucro_context, self.auto_init)
-        return involucro_context
-
     def __str__(self):
         return f"BuildDockerContainerResolver[namespace={self.namespace}]"
 
 
 class BuildMulledSingularityContainerResolver(SingularityCliContainerResolver):
     """Build for Singularity mulled images matching tool dependencies."""
 
     resolver_type = "build_mulled_singularity"
     shell = "/bin/bash"
     builds_on_resolution = True
 
-    def __init__(self, app_info=None, hash_func="v2", auto_install=True, **kwds):
+    def __init__(
+        self, app_info: Optional["AppInfo"] = None, hash_func: str = "v2", auto_install: bool = True, **kwds
+    ) -> None:
         super().__init__(app_info=app_info, **kwds)
         self._involucro_context_kwds = {"involucro_bin": self._get_config_option("involucro_path", None)}
         self.hash_func = hash_func
         self._init_cache_directory()
         self.auto_install = string_as_bool(auto_install)
         self._mulled_kwds = {
             "channels": self._get_config_option("mulled_channels", DEFAULT_CHANNELS),
             "hash_func": self.hash_func,
             "command": "build-and-test",
             "singularity": True,
             "singularity_image_dir": self.cache_directory.path,
         }
-        self.auto_init = self._get_config_option("involucro_auto_init", True)
+        self.involucro_context = InvolucroContext(**self._involucro_context_kwds)
+        auto_init = self._get_config_option("involucro_auto_init", True)
+        self.enabled = ensure_installed(self.involucro_context, auto_init)
 
     def resolve(self, enabled_container_types, tool_info, install=False, **kwds):
         if tool_info.requires_galaxy_python_environment or self.container_type not in enabled_container_types:
             return None
 
         targets = mulled_targets(tool_info)
         log.debug(f"Image name for tool {tool_info.tool_id}: {image_name(targets, self.hash_func)}")
         if len(targets) == 0:
             return None
 
         if self.auto_install or install:
-            mull_targets(targets, involucro_context=self._get_involucro_context(), **self._mulled_kwds)
+            mull_targets(targets, involucro_context=self.involucro_context, **self._mulled_kwds)
         return singularity_cached_container_description(
             targets, self.cache_directory, hash_func=self.hash_func, shell=self.shell
         )
 
-    def _get_involucro_context(self):
-        involucro_context = InvolucroContext(**self._involucro_context_kwds)
-        self.enabled = ensure_installed(involucro_context, self.auto_init)
-        return involucro_context
-
     def __str__(self):
         return f"BuildSingularityContainerResolver[cache_directory={self.cache_directory.path}]"
 
 
 def mulled_targets(tool_info):
     return requirements_to_mulled_targets(tool_info.requirements)
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/container_volumes.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/container_volumes.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from abc import (
     ABCMeta,
     abstractmethod,
 )
 
 
 class ContainerVolume(metaclass=ABCMeta):
-
     valid_modes = frozenset({"ro", "rw"})
 
     def __init__(self, path, host_path=None, mode=None):
         self.path = path
         self.host_path = host_path
         self.mode = mode
         if mode and not self.mode_is_valid:
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/containers.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 )
 
 from galaxy.util import (
     asbool,
     plugin_config,
 )
 from .container_classes import (
+    Container,
     CONTAINER_CLASSES,
     DOCKER_CONTAINER_TYPE,
-    NULL_CONTAINER,
     SINGULARITY_CONTAINER_TYPE,
 )
 from .container_resolvers import ResolutionCache
 from .container_resolvers.explicit import (
     ExplicitContainerResolver,
     ExplicitSingularityContainerResolver,
 )
@@ -50,19 +50,19 @@
 
 ResolvedContainerDescription = collections.namedtuple(
     "ResolvedContainerDescription", ["container_resolver", "container_description"]
 )
 
 
 class ContainerFinder:
-    def __init__(self, app_info, mulled_resolution_cache=None):
+    def __init__(self, app_info: "AppInfo", mulled_resolution_cache: Optional["Cache"] = None) -> None:
         self.app_info = app_info
         self.mulled_resolution_cache = mulled_resolution_cache
         self.default_container_registry = ContainerRegistry(app_info, mulled_resolution_cache=mulled_resolution_cache)
-        self.destination_container_registeries = {}
+        self.destination_container_registeries: Dict[str, "ContainerRegistry"] = {}
 
     def _enabled_container_types(self, destination_info):
         return [t for t in ALL_CONTAINER_TYPES if self.__container_type_enabled(t, destination_info)]
 
     def find_best_container_description(self, enabled_container_types, tool_info, **kwds):
         """Regardless of destination properties - find best container for tool.
 
@@ -96,20 +96,20 @@
             and destination_id
             and destination_id in self.destination_container_registeries
         ):
             destination_container_registry = self.destination_container_registeries[destination_id]
 
         return destination_container_registry or self.default_container_registry
 
-    def find_container(self, tool_info, destination_info, job_info):
+    def find_container(self, tool_info, destination_info, job_info) -> Optional[Container]:
         enabled_container_types = self._enabled_container_types(destination_info)
 
         # Short-cut everything else and just skip checks if no container type is enabled.
         if not enabled_container_types:
-            return NULL_CONTAINER
+            return None
 
         def __destination_container(container_description=None, container_id=None, container_type=None):
             if container_description:
                 container_id = container_description.identifier
                 container_type = container_description.type
             container = self.__destination_container(
                 container_id,
@@ -161,15 +161,15 @@
         for container_type in CONTAINER_CLASSES.keys():
             container_id = self.__default_container_id(container_type, destination_info)
             if container_id:
                 container = __destination_container(container_type=container_type, container_id=container_id)
                 if container:
                     return container
 
-        return NULL_CONTAINER
+        return None
 
     def resolution_cache(self):
         return self.default_container_registry.get_resolution_cache()
 
     def __overridden_container_id(self, container_type, destination_info):
         if not self.__container_type_enabled(container_type, destination_info):
             return None
@@ -207,15 +207,15 @@
         return None
 
     def __destination_container(
         self, container_id, container_type, tool_info, destination_info, job_info, container_description=None
     ):
         # TODO: ensure destination_info is dict-like
         if not self.__container_type_enabled(container_type, destination_info):
-            return NULL_CONTAINER
+            return None
 
         # TODO: Right now this assumes all containers available when a
         # container type is - there should be more thought put into this.
         # Checking which are available - settings policies for what can be
         # auto-fetched, etc....
         return CONTAINER_CLASSES[container_type](
             container_id, self.app_info, tool_info, destination_info, job_info, container_description
@@ -223,15 +223,15 @@
 
     def __container_type_enabled(self, container_type, destination_info):
         return asbool(destination_info.get(f"{container_type}_enabled", False))
 
 
 class NullContainerFinder:
     def find_container(self, tool_info, destination_info, job_info):
-        return []
+        return None
 
 
 class ContainerRegistry:
     """Loop through enabled ContainerResolver plugins and find first match."""
 
     def __init__(
         self,
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/dependencies.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/docker_util.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/docker_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -194,24 +194,29 @@
 def parse_port_text(port_text):
     """
 
     >>> slurm_ports = parse_port_text("8888/tcp -> 0.0.0.0:32769")
     >>> slurm_ports[8888]['host']
     '0.0.0.0'
     >>> ports = parse_port_text("5432/tcp -> :::5432")
+    >>> len(ports)
+    0
+    >>> ports_new = parse_port_text("5432/tcp -> [::]:5432")
+    >>> len(ports_new)
+    0
     """
     ports = None
     if port_text is not None:
         ports = {}
         for line in port_text.strip().split("\n"):
             if " -> " not in line:
                 raise Exception(f"Cannot parse host and port from line [{line}]")
             tool, host = line.split(" -> ", 1)
             hostname, port = host.rsplit(":", 1)
-            if hostname == "::":
+            if hostname in ["::", "[::]"]:
                 # Skip unspecified IPv6 address, which is also specified as 0:0:0:0 in another line.
                 # This is brittle of course, but so is parsing the container ports like this.
                 continue
             port = int(port)
             tool_p, tool_prot = tool.split("/")
             tool_p = int(tool_p)
             ports[tool_p] = dict(tool_port=tool_p, host=hostname, port=port, protocol=tool_prot)
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/dockerfiles.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/dockerfiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         host=kwds["docker_host"],
     )
 
 
 def dockerfile_build(path, dockerfile=None, error=log.error, **kwds):
     expected_container_names = set()
     tool_directories = set()
-    for (tool_path, tool_xml) in load_tool_elements_from_path(path):
+    for tool_path, tool_xml in load_tool_elements_from_path(path):
         requirements, containers = parse_requirements_from_xml(tool_xml)
         for container in containers:
             if container.type == "docker":
                 expected_container_names.add(container.identifier)
                 tool_directories.add(os.path.dirname(tool_path))
                 break
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/installable.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/installable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 """Abstractions for installing local software managed and required by Galaxy/galaxy-lib."""
 
+import abc
 import logging
 import os
-from abc import (
-    ABCMeta,
-    abstractmethod,
-    abstractproperty,
-)
 
 from galaxy.util.filelock import (
     FileLock,
     FileLockException,
 )
 
 log = logging.getLogger(__name__)
 
 
-class InstallableContext(metaclass=ABCMeta):
+class InstallableContext(metaclass=abc.ABCMeta):
     """Represent a directory/configuration of something that can be installed."""
 
-    @abstractmethod
+    @abc.abstractmethod
     def is_installed(self):
         """Return bool indicating if the configured software is installed."""
 
-    @abstractmethod
+    @abc.abstractmethod
     def can_install(self):
         """Check preconditions for installation."""
 
-    @abstractproperty
+    @property
+    @abc.abstractmethod
     def installable_description(self):
         """Short description of thing being installed for log statements."""
 
-    @abstractproperty
+    @property
+    @abc.abstractmethod
     def parent_path(self):
         """Return parent path of the location the installable will be created within."""
 
 
 def ensure_installed(installable_context, install_func, auto_init):
     """Make sure target is installed - handle multiple processes potentially attempting installation."""
     parent_path = installable_context.parent_path
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/get_tests.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/get_tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 #!/usr/bin/env python
 
 """
 searches for tests for packages in the bioconda-recipes repo and on Anaconda, looking in different file locations. If no test can be found for the specified version, it will look for tests for other versions of the same package.
 
 A shallow search (default for singularity and conda generation scripts) just checks once on Anaconda for the specified version.
 """
-# import doctest
 import json
 import logging
 from glob import glob
 from typing import (
     Any,
     Dict,
+    List,
     Optional,
 )
 
 import requests
 import yaml
 
 try:
     from jinja2 import Template
     from jinja2.exceptions import UndefinedError
 except ImportError:
     Template = None  # type: ignore[assignment,misc]
     UndefinedError = Exception  # type: ignore[assignment,misc]
 
-from galaxy.util import unicodify
+from galaxy.util import (
+    check_github_api_response_rate_limit,
+    unicodify,
+)
+from galaxy.util.commands import argv_to_str
 from .util import (
-    get_file_from_conda_package,
+    get_files_from_conda_package,
     MULLED_SOCKET_TIMEOUT,
     split_container_name,
 )
 
 INSTALL_JINJA_EXCEPTION = (
     "This mulled functionality required jinja2 but it is unavailable, install condatesting extras."
 )
@@ -62,27 +66,26 @@
     except (KeyError, TypeError):
         logging.info("Error reading imports")
 
     if len(package_tests.get("commands", []) + package_tests.get("imports", [])) == 0:
         return None
 
     # need to know what scripting languages are needed to run the container
+    package_tests["import_lang"] = "python -c"  # python by default
     try:
         requirements = list(meta_yaml["requirements"]["run"])
     except (KeyError, TypeError):
         logging.info("Error reading requirements", exc_info=True)
     else:
         for requirement in requirements:
             if requirement.split()[0] == "perl":
                 package_tests["import_lang"] = "perl -e"
                 break
             # elif ... :
             # other languages if necessary ... hopefully python and perl should suffice though
-        else:  # python by default
-            package_tests["import_lang"] = "python -c"
     return package_tests
 
 
 def get_run_test(file: str) -> Dict[str, Any]:
     r"""
     Get tests from a run_test.sh file
     """
@@ -106,33 +109,35 @@
     return f"https://anaconda.org{url}"
 
 
 def get_test_from_anaconda(url: str) -> Optional[Dict[str, Any]]:
     """
     Given the URL of an anaconda tarball, return tests
     """
-    name, content = get_file_from_conda_package(
+    content_dict = get_files_from_conda_package(
         url, ["info/recipe/meta.yaml", "info/recipe/meta.yaml.template", "info/recipe/run_test.sh"]
     )
-    if name and content and name.startswith("info/recipe/meta.yaml"):
+    content = content_dict.get("info/recipe/meta.yaml", content_dict.get("info/recipe/meta.yaml.template"))
+    if content:
         package_tests = get_commands_from_yaml(content)
         if package_tests:
             return package_tests
-    if name and content and name == "info/recipe/run_test.sh":
-        return get_run_test(unicodify(content))
+    if "info/recipe/run_test.sh" in content_dict:
+        return get_run_test(unicodify(content_dict["info/recipe/run_test.sh"]))
     return None
 
 
 def find_anaconda_versions(name, anaconda_channel="bioconda"):
     """
     Find a list of available anaconda versions for a given container name
     """
     r = requests.get(f"https://anaconda.org/{anaconda_channel}/{name}/files", timeout=MULLED_SOCKET_TIMEOUT)
+    r.raise_for_status()
     urls = []
-    for line in r.text.split("\n"):
+    for line in r.text.splitlines():
         if "download/linux" in line:
             urls.append(line.split('"')[1])
     return urls
 
 
 def open_recipe_file(file, recipes_path=None, github_repo="bioconda/bioconda-recipes"):
     """
@@ -154,20 +159,18 @@
     """
     Return files that match ``filepath/*/filename`` in the bioconda-recipes repository
     """
     if recipes_path:
         return [n.replace(f"{recipes_path}/", "") for n in glob(f"{recipes_path}/{filepath}/*/{filename}")]
     # else use the GitHub API:
     versions = []
-    r = json.loads(
-        requests.get(
-            f"https://api.github.com/repos/{github_repo}/contents/{filepath}", timeout=MULLED_SOCKET_TIMEOUT
-        ).text
-    )
-    for subfile in r:
+    r = requests.get(f"https://api.github.com/repos/{github_repo}/contents/{filepath}", timeout=MULLED_SOCKET_TIMEOUT)
+    check_github_api_response_rate_limit(r)
+    r.raise_for_status()
+    for subfile in json.loads(r.text):
         if subfile["type"] == "dir":
             if (
                 requests.get(
                     f"https://raw.githubusercontent.com/{github_repo}/master/{subfile['path']}/{filename}",
                     timeout=MULLED_SOCKET_TIMEOUT,
                 ).status_code
                 == 200
@@ -255,45 +258,59 @@
     # else shallow
     result = try_a_func(get_test_from_anaconda, get_anaconda_url, (container, anaconda_channel), container)
     if result:
         return result
     return {"container": container}
 
 
+def import_test_to_command_list(import_lang: str, import_: str) -> List[str]:
+    if import_lang == "python -c":
+        return ["python", "-c", f"import {import_}"]
+    elif import_lang == "perl -e":
+        return ["perl", "-e", f"use {import_}"]
+    else:
+        raise ValueError(f"Unsupported import_lang '{import_lang}'")
+
+
 def hashed_test_search(
-    container, recipes_path=None, deep=False, anaconda_channel="bioconda", github_repo="bioconda/bioconda-recipes"
-):
+    container: str, recipes_path=None, deep=False, anaconda_channel="bioconda", github_repo="bioconda/bioconda-recipes"
+) -> Dict[str, Any]:
     """
     Get test for hashed containers
     """
-    package_tests = {"commands": [], "imports": [], "container": container, "import_lang": "python -c"}
+    package_tests: Dict[str, Any] = {"commands": [], "imports": [], "container": container, "import_lang": "python -c"}
 
-    githubpage = requests.get(
+    response = requests.get(
         f"https://raw.githubusercontent.com/BioContainers/multi-package-containers/master/combinations/{container}.tsv",
         timeout=MULLED_SOCKET_TIMEOUT,
     )
-    if githubpage.status_code == 200:
-        packages = githubpage.text.split(",")  # get names of packages from github
-        packages = [package.split("=") for package in packages]
-    else:
-        packages = []
+    response.raise_for_status()
+    for line in response.text.splitlines():
+        if not line.startswith("#"):
+            break
+    concatenated_targets = line.split("\t")[0]
+    targets = concatenated_targets.split(",")
+    packages = [target.split("=") for target in targets]
 
     containers = []
     for package in packages:
         r = requests.get(f"https://anaconda.org/bioconda/{package[0]}/files", timeout=MULLED_SOCKET_TIMEOUT)
+        r.raise_for_status()
         p = "-".join(package)
         for line in r.text.split("\n"):
-            if p in line:
+            # include only linux-64 builds since that is hardcoded in get_anaconda_url and the only target for container builds
+            if p in line and "linux-64" in line:
                 build = line.split(p)[1].split(".tar.bz2")[0]
                 if build == "":
                     containers.append(f"{package[0]}:{package[1]}")
                 else:
                     containers.append(f"{package[0]}:{package[1]}-{build}")
                 break
 
     for container in containers:
         tests = main_test_search(container, recipes_path, deep, anaconda_channel, github_repo)
         package_tests["commands"] += tests.get("commands", [])  # not a very nice solution but probably the simplest
+        # Given that this could be a mix of Python and Perl packages, translate imports to commands
         for imp in tests.get("imports", []):
-            package_tests["imports"].append(f"{tests['import_lang']} 'import {imp}'")
+            package_tests["commands"].append(argv_to_str(import_test_to_command_list(tests["import_lang"], imp)))
 
     return package_tests
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/invfile.lua` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/invfile.lua`

 * *Files 3% similar despite different names*

```diff
@@ -38,21 +38,22 @@
 local test_binds_table = VAR.TEST_BINDS:split(",")
 for i = 1, #test_binds_table do
     table.insert(test_bind_args, test_binds_table[i])
 end
 
 local conda_image = VAR.CONDA_IMAGE
 if conda_image == '' then
-    conda_image = 'continuumio/miniconda3:latest'
+    conda_image = 'quay.io/condaforge/mambaforge:latest'
 end
 
+local conda_bin = VAR.CONDA_BIN
 
 local singularity_image = VAR.SINGULARITY_IMAGE
 if singularity_image == '' then
-    singularity_image = 'quay.io/biocontainers/singularity:2.4.6--0'
+    singularity_image = 'quay.io/singularity/singularity:v3.10.4'
 end
 
 local singularity_image_dir = VAR.SINGULARITY_IMAGE_DIR
 if singularity_image_dir == '' then
     singularity_image_dir = 'singularity_import'
 end
 
@@ -83,15 +84,15 @@
 inv.task('build')
     .using(conda_image)
         .withHostConfig({binds = {"build:/data"}})
         .run('rm', '-rf', '/data/dist')
     .using(conda_image)
         .withHostConfig({binds = bind_args})
         .run('/bin/sh', '-c', preinstall
-            .. 'conda install '
+            .. conda_bin .. ' install '
             .. channel_args .. ' '
             .. target_args
             .. ' --strict-channel-priority -p /usr/local --copy --yes '
             .. verbose
             .. postinstall)
     .wrap('build/dist')
         .at('/usr/local')
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_build.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_build.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,25 +29,26 @@
 from galaxy.tool_util.deps.conda_util import (
     best_search_result,
     CondaContext,
 )
 from galaxy.tool_util.deps.docker_util import command_list as docker_command_list
 from galaxy.util import (
     commands,
+    download_to_file,
     safe_makedirs,
     shlex_join,
     unicodify,
 )
 from ._cli import arg_parser
 from .util import (
     build_target,
     conda_build_target_str,
     create_repository,
     default_mulled_conda_channels_from_env,
-    get_file_from_conda_package,
+    get_files_from_conda_package,
     PrintProgress,
     quay_repository,
     v1_image_name,
     v2_image_name,
 )
 from ..conda_compat import MetaData
 
@@ -166,22 +167,24 @@
     determine base image (DEFAULT_BASE_IMAGE/DEFAULT_EXTENDED_BASE_IMAGE) for a
     list of targets by inspecting the conda package (i.e. if the use of an
     extended image is indicated in info/about.json or info/recipe/meta.yaml
     """
     hits = get_conda_hits_for_targets(targets, conda_context)
     for hit in hits:
         try:
-            name, content = get_file_from_conda_package(hit["url"], ["info/about.json", "info/recipe/meta.yaml"])
-            strcontent = unicodify(content)
-            if name == "info/about.json" and json.loads(strcontent).get("extra", {}).get("container", {}).get(
-                "extended-base", False
-            ):
+            content_dict = get_files_from_conda_package(hit["url"], ["info/about.json", "info/recipe/meta.yaml"])
+            if "info/about.json" in content_dict and json.loads(unicodify(content_dict["info/about.json"])).get(
+                "extra", {}
+            ).get("container", {}).get("extended-base", False):
                 return DEFAULT_EXTENDED_BASE_IMAGE
-            elif name == "info/recipe/meta.yaml" and (
-                yaml.safe_load(strcontent).get("extra", {}).get("container", {}).get("extended-base", False)
+            elif "info/recipe/meta.yaml" in content_dict and (
+                yaml.safe_load(unicodify(content_dict["info/recipe/meta.yaml"]))
+                .get("extra", {})
+                .get("container", {})
+                .get("extended-base", False)
             ):
                 return DEFAULT_EXTENDED_BASE_IMAGE
         except Exception:
             log.warning(
                 "Could not load metadata.yaml for '%s', version '%s'", hit["name"], hit["version"], exc_info=True
             )
     return DEFAULT_BASE_IMAGE
@@ -204,14 +207,16 @@
     test="true",
     test_files=None,
     image_build=None,
     name_override=None,
     repository_template=DEFAULT_REPOSITORY_TEMPLATE,
     dry_run=False,
     conda_version=None,
+    mamba_version=None,
+    use_mamba=False,
     verbose=False,
     binds=DEFAULT_BINDS,
     rebuild=True,
     oauth_token=None,
     hash_func="v2",
     singularity=False,
     singularity_image_dir="singularity_import",
@@ -291,17 +296,36 @@
         singularity_image_name = repo_template_kwds["image"]
         involucro_args.extend(["-set", "SINGULARITY=1"])
         involucro_args.extend(["-set", f"SINGULARITY_IMAGE_NAME={singularity_image_name}"])
         involucro_args.extend(["-set", f"SINGULARITY_IMAGE_DIR={singularity_image_dir}"])
         involucro_args.extend(["-set", f"USER_ID={os.getuid()}:{os.getgid()}"])
     if test:
         involucro_args.extend(["-set", f"TEST={test}"])
-    if conda_version is not None:
-        verbose = "--verbose" if verbose else "--quiet"
-        involucro_args.extend(["-set", f"PREINSTALL=conda install {verbose} --yes conda={conda_version}"])
+
+    verbose = "--verbose" if verbose else "--quiet"
+    conda_bin = "conda"
+    if use_mamba:
+        conda_bin = "mamba"
+        if mamba_version is None:
+            mamba_version = ""
+    involucro_args.extend(["-set", "CONDA_BIN=%s" % conda_bin])
+    if conda_version is not None or mamba_version is not None:
+        mamba_test = "true"
+        specs = []
+        if conda_version is not None:
+            specs.append(f"conda={conda_version}")
+        if mamba_version is not None:
+            specs.append(f"mamba={mamba_version}")
+            if mamba_version == "" and not specs:
+                # If nothing but mamba without a specific version is requested,
+                # then only run conda install if mamba is not already installed.
+                mamba_test = "[ '[]' = \"$( conda list --json --full-name mamba )\" ]"
+        conda_install = f"""conda install {verbose} --yes {" ".join(f"'{spec}'" for spec in specs)}"""
+        involucro_args.extend(["-set", f"PREINSTALL=if {mamba_test} ; then {conda_install} ; fi"])
+
     involucro_args.append(command)
     if test_files:
         test_bind = []
         for test_file in test_files:
             if ":" not in test_file:
                 if os.path.exists(test_file):
                     test_bind.append(f"{test_file}:{DEFAULT_WORKING_DIR}/{test_file}")
@@ -364,15 +388,14 @@
             debug=debug,
             ensure_channels=ensure_channels,
             condarc_override=condarc_override,
         )
 
 
 class InvolucroContext(installable.InstallableContext):
-
     installable_description = "Involucro"
 
     def __init__(self, involucro_bin=None, shell_exec=None, verbose="3"):
         if involucro_bin is None:
             if os.path.exists("./involucro"):
                 self.involucro_bin = "./involucro"
             else:
@@ -414,18 +437,20 @@
 def ensure_installed(involucro_context, auto_init):
     return installable.ensure_installed(involucro_context, install_involucro, auto_init)
 
 
 def install_involucro(involucro_context):
     install_path = os.path.abspath(involucro_context.involucro_bin)
     involucro_context.involucro_bin = install_path
-    download_cmd = commands.download_command(involucro_link(), to=install_path)
-    exit_code = involucro_context.shell_exec(download_cmd)
-    if exit_code:
-        return exit_code
+
+    try:
+        download_to_file(involucro_link(), install_path)
+    except Exception:
+        log.exception(f"Failed to download involucro from url '{involucro_link()}'")
+        return 1
     try:
         os.chmod(install_path, os.stat(install_path).st_mode | stat.S_IXUSR | stat.S_IXGRP | stat.S_IXOTH)
         return 0
     except Exception:
         log.exception("Failed to make file '%s' executable", install_path)
         return 1
 
@@ -464,14 +489,26 @@
     parser.add_argument(
         "--conda-version",
         dest="conda_version",
         default=None,
         help="Change to specified version of Conda before installing packages.",
     )
     parser.add_argument(
+        "--mamba-version",
+        dest="mamba_version",
+        default=None,
+        help="Change to specified version of Mamba before installing packages.",
+    )
+    parser.add_argument(
+        "--use-mamba",
+        dest="use_mamba",
+        action="store_true",
+        help="Use Mamba instead of Conda for package installation.",
+    )
+    parser.add_argument(
         "--oauth-token",
         dest="oauth_token",
         default=None,
         help="If set, use this token when communicating with quay.io API.",
     )
     parser.add_argument("--check-published", dest="rebuild", action="store_false")
     parser.add_argument("--hash", dest="hash", choices=["v1", "v2"], default="v2")
@@ -528,14 +565,18 @@
         kwds["channels"] = args.channels.split(",")
     if hasattr(args, "command"):
         kwds["command"] = args.command
     if hasattr(args, "repository_template"):
         kwds["repository_template"] = args.repository_template
     if hasattr(args, "conda_version"):
         kwds["conda_version"] = args.conda_version
+    if hasattr(args, "mamba_version"):
+        kwds["mamba_version"] = args.mamba_version
+    if hasattr(args, "use_mamba"):
+        kwds["use_mamba"] = args.use_mamba
     if hasattr(args, "oauth_token"):
         kwds["oauth_token"] = args.oauth_token
     if hasattr(args, "rebuild"):
         kwds["rebuild"] = args.rebuild
     if hasattr(args, "hash"):
         kwds["hash_func"] = args.hash
     if hasattr(args, "singularity_image_dir") and args.singularity_image_dir:
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_build_channel.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_build_channel.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_build_files.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_build_files.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_build_tool.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_build_tool.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_hash.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_hash.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_list.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_list.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_search.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python
 
 import argparse
 import json
 import logging
 import sys
 import tempfile
-from datetime import (
-    datetime,
-    timezone,
-)
 
 import requests
 
 from galaxy.tool_util.deps.conda_util import CondaContext
-from galaxy.util import which
+from galaxy.util import (
+    check_github_api_response_rate_limit,
+    which,
+)
 from .mulled_list import get_singularity_containers
 from .util import (
     build_target,
     MULLED_SOCKET_TIMEOUT,
     v2_image_name,
 )
 
@@ -143,37 +142,26 @@
 
 
 class GitHubSearch:
     """
     Tool to search the GitHub bioconda-recipes repo
     """
 
-    @staticmethod
-    def _check_response_rate_limit(response):
-        if response.status_code == 403 and "API rate limit exceeded" in response.json()["message"]:
-            # It can take tens of minutes before the rate limit window resets
-            message = "GitHub API rate limit exceeded."
-            rate_limit_reset_UTC_timestamp = response.headers.get("X-RateLimit-Reset")
-            if rate_limit_reset_UTC_timestamp:
-                rate_limit_reset_datetime = datetime.fromtimestamp(int(rate_limit_reset_UTC_timestamp), tz=timezone.utc)
-                message += f" The rate limit window will reset at {rate_limit_reset_datetime.isoformat()}."
-            raise Exception(message)
-
     def get_json(self, search_string):
         """
         Takes search_string variable and return results from the bioconda-recipes github repository in JSON format
 
         DEPRECATED: this method is currently unreliable because the API query
         sometimes succeeds but returns no items.
         """
         response = requests.get(
             f"https://api.github.com/search/code?q={search_string}+in:path+repo:bioconda/bioconda-recipes+path:recipes",
             timeout=MULLED_SOCKET_TIMEOUT,
         )
-        self._check_response_rate_limit(response)
+        check_github_api_response_rate_limit(response)
         response.raise_for_status()
         return response.json()
 
     def process_json(self, json_response, search_string):
         """
         Take JSON input and process it, returning the required data
         """
@@ -184,15 +172,15 @@
         """
         Check if a recipe exists in bioconda-recipes which matches search_string exactly
         """
         response = requests.get(
             f"https://api.github.com/repos/bioconda/bioconda-recipes/contents/recipes/{search_string}",
             timeout=MULLED_SOCKET_TIMEOUT,
         )
-        self._check_response_rate_limit(response)
+        check_github_api_response_rate_limit(response)
         return response.status_code == 200
 
 
 def get_package_hash(packages, versions):
     """
     Take packages and versions (if the latter are given) and returns a hash for each. Also checks github to see if the container is already present.
     """
@@ -241,15 +229,14 @@
             version = container.split(":")[1]
             results.append({"package": name, "version": version})
 
     return results
 
 
 def readable_output(json, organization="biocontainers", channel="bioconda"):
-
     # if json is empty:
     if sum(len(json[destination][results]) for destination in json for results in json[destination]) == 0:
         sys.stdout.write("No results found for that query.\n")
         return
 
     # return results for quay, conda and singularity together
     if (
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 #!/usr/bin/env python
 
 import argparse
+import os
+import os.path
 import subprocess
 import tempfile
 from glob import glob
 from subprocess import check_output
+from typing import (
+    Any,
+    Dict,
+    List,
+    Union,
+)
 
 from galaxy.util import unicodify
 from .get_tests import (
     hashed_test_search,
+    import_test_to_command_list,
     main_test_search,
 )
 
 
 def get_list_from_file(filename):
     """
     Returns a list of containers stored in a file (one on each line)
@@ -21,66 +30,66 @@
         return [_ for _ in fh.read().splitlines() if _]  # if blank lines are in the file empty strings must be removed
 
 
 def docker_to_singularity(container, installation, filepath, no_sudo=False):
     """
     Convert docker to singularity container.
     """
-    cmd = [installation, "build", "/".join((filepath, container)), f"docker://quay.io/biocontainers/{container}"]
+    cmd = [installation, "build", os.path.join(filepath, container), f"docker://quay.io/biocontainers/{container}"]
     try:
         if no_sudo:
             check_output(cmd, stderr=subprocess.STDOUT)
         else:
             check_output(cmd.insert(0, "sudo"), stderr=subprocess.STDOUT)
             check_output(["sudo", "rm", "-rf", "/root/.singularity/docker/"], stderr=subprocess.STDOUT)
     except subprocess.CalledProcessError as e:
         raise Exception(f"Docker to Singularity conversion failed.\nOutput was:\n{unicodify(e.output)}")
 
 
-def singularity_container_test(tests, installation, filepath):
+def singularity_container_test(
+    tests: Dict[str, Dict[str, Any]], installation: str, filepath: Union[str, os.PathLike]
+) -> Dict[str, List]:
     """
     Run tests, record if they pass or fail
     """
-    test_results = {"passed": [], "failed": [], "notest": []}
+    test_results: Dict[str, List] = {"passed": [], "failed": [], "notest": []}
 
     # create a 'sanitised home' directory in which the containers may be mounted - see http://singularity.lbl.gov/faq#solution-1-specify-the-home-to-mount
     with tempfile.TemporaryDirectory() as tmpdirname:
         for container, test in tests.items():
             if "commands" not in test and "imports" not in test:
                 test_results["notest"].append(container)
-
             else:
-                exec_command = [installation, "exec", "-H", tmpdirname, "/".join((filepath, container))]
+                exec_command = [installation, "exec", "-H", tmpdirname, os.path.join(filepath, container)]
                 test_passed = True
                 errors = []
-                if test.get("commands", False):
-                    for test_command in test["commands"]:
-                        test_command = test_command.replace("$PREFIX", "/usr/local/")
-                        test_command = test_command.replace("${PREFIX}", "/usr/local/")
-                        test_command = test_command.replace("$R ", "Rscript ")
-
+                for test_command in test.get("commands", []):
+                    test_command = test_command.replace("$PREFIX", "/usr/local/")
+                    test_command = test_command.replace("${PREFIX}", "/usr/local/")
+                    test_command = test_command.replace("$R ", "Rscript ")
+
+                    try:
+                        check_output(exec_command + ["bash", "-c", test_command], stderr=subprocess.STDOUT)
+                    except subprocess.CalledProcessError:
                         try:
-                            check_output(exec_command.extend(["bash", "-c", test_command]), stderr=subprocess.STDOUT)
-                        except subprocess.CalledProcessError:
-                            try:
-                                check_output(exec_command.append(test_command), stderr=subprocess.STDOUT)
-                            except subprocess.CalledProcessError as e:
-                                errors.append({"command": test_command, "output": unicodify(e.output)})
-                                test_passed = False
-
-                if test.get("imports", False):
-                    for imp in test["imports"]:
-                        try:
-                            check_output(
-                                exec_command.extend([test["import_lang"], f"import {imp}"]), stderr=subprocess.STDOUT
-                            )
+                            check_output(exec_command + [test_command], stderr=subprocess.STDOUT)
                         except subprocess.CalledProcessError as e:
-                            errors.append({"import": imp, "output": unicodify(e.output)})
+                            errors.append({"command": test_command, "output": unicodify(e.output)})
                             test_passed = False
 
+                for imp in test.get("imports", []):
+                    try:
+                        check_output(
+                            exec_command + import_test_to_command_list(test["import_lang"], imp),
+                            stderr=subprocess.STDOUT,
+                        )
+                    except subprocess.CalledProcessError as e:
+                        errors.append({"import": imp, "output": unicodify(e.output)})
+                        test_passed = False
+
                 if test_passed:
                     test_results["passed"].append(container)
                 else:
                     test["errors"] = errors
                     test_results["failed"].append(test)
     return test_results
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/mulled/util.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/mulled/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 import hashlib
 import logging
 import os
 import re
 import sys
 import threading
 from typing import (
+    Dict,
     Iterable,
     List,
-    Optional,
-    Tuple,
     TYPE_CHECKING,
-    Union,
 )
 
 import packaging.version
 import requests
 from conda_package_streaming.package_streaming import stream_conda_info
 from conda_package_streaming.url import stream_conda_info as stream_conda_info_from_url
 
@@ -75,14 +73,15 @@
         session = requests.session()
     response = session.get(url, timeout=MULLED_SOCKET_TIMEOUT)
     data = response.json()
     return data
 
 
 def _get_namespace(namespace: str) -> List[str]:
+    log.debug(f"Querying {QUAY_REPOSITORY_API_ENDPOINT} for repos within {namespace}")
     next_page = None
     repo_names = []
     repos_headers = {"Accept-encoding": "gzip", "Accept": "application/json"}
     while True:
         repos_parameters = {"public": "true", "namespace": namespace, "next_page": next_page}
         repos_response = requests.get(
             QUAY_REPOSITORY_API_ENDPOINT, headers=repos_headers, params=repos_parameters, timeout=MULLED_SOCKET_TIMEOUT
@@ -346,50 +345,39 @@
             build_suffix = image_build
         suffix = ""
         if version_hash_str or build_suffix:
             suffix = f":{version_hash_str}{build_suffix}"
         return f"mulled-v2-{package_hash.hexdigest()}{suffix}"
 
 
-def get_file_from_conda_package(
-    url: str, checklist: Union[str, Iterable[str]]
-) -> Tuple[Optional[str], Optional[bytes]]:
+def get_files_from_conda_package(url: str, filepaths: Iterable[str]) -> Dict[str, bytes]:
     """
-    Get file content for an element in a conda package.
+    Get content of specified files in a conda package.
     The url can be a path to a local file or an url.
-    The checklist can be the name of the element to etract
-    or a Iterable of potentially desired elements the content
-    of the first that is contained in the conda package
-    is returned.
-    Return the name and content (bytes) of the first found element
-    and None, None otherwise
-
-    >>> name, content = get_file_from_conda_package("https://anaconda.org/conda-forge/chopin2/1.0.6/download/noarch/chopin2-1.0.6-pyhd8ed1ab_0.tar.bz2", "info/recipe/meta.yaml")
-    >>> assert name == "info/recipe/meta.yaml"
-    >>> assert isinstance(content, bytes)
-    >>> name, content = get_file_from_conda_package("https://anaconda.org/conda-forge/chopin2/1.0.7/download/noarch/chopin2-1.0.7-pyhd8ed1ab_1.conda", ["info/about.json", "info/recipe/meta.yaml"])
-    >>> assert name == "info/recipe/meta.yaml"
-    >>> assert isinstance(content, bytes)
+    The filepaths is an iterable of paths to extract from the conda package, if
+    found in it.
+    Return a dictionary mapping each found filepath to the corresponding content
+    (as bytes).
+
+    >>> content_dict = get_files_from_conda_package("https://anaconda.org/conda-forge/chopin2/1.0.6/download/noarch/chopin2-1.0.6-pyhd8ed1ab_0.tar.bz2", ["info/recipe/meta.yaml"])
+    >>> assert "info/recipe/meta.yaml" in content_dict, content_dict
+    >>> assert isinstance(content_dict["info/recipe/meta.yaml"], bytes)
+    >>> content_dict = get_files_from_conda_package("https://anaconda.org/conda-forge/chopin2/1.0.7/download/noarch/chopin2-1.0.7-pyhd8ed1ab_1.conda", ["info/about.json", "info/recipe/meta.yaml", "foo/bar"])
+    >>> assert sorted(content_dict.keys()) == ["info/about.json", "info/recipe/meta.yaml"], content_dict
     """
 
-    if isinstance(checklist, str):
-        checklist = set([checklist])
-    else:
-        checklist = set(checklist)
-    # print(checklist)
     try:
         stream = stream_conda_info(url)
     except FileNotFoundError:
         stream = stream_conda_info_from_url(url)
+    ret = {}
     for tar, member in stream:
-        # print(member.name)
-        if member.name in checklist:
-            return member.name, tar.extractfile(member).read()
-    # print("None")
-    return None, None
+        if member.name in filepaths:
+            ret[member.name] = tar.extractfile(member).read()
+    return ret
 
 
 def split_container_name(name):
     """
     Takes a container name (e.g. samtools:1.7--1) and returns a list (e.g. ['samtools', '1.7', '1'])
     >>> split_container_name('samtools:1.7--1')
     ['samtools', '1.7', '1']
@@ -419,14 +407,15 @@
 
 
 image_name = v1_image_name  # deprecated
 
 __all__ = (
     "build_target",
     "conda_build_target_str",
+    "get_files_from_conda_package",
     "image_name",
     "mulled_tags_for",
     "quay_versions",
     "split_container_name",
     "split_tag",
     "Target",
     "v1_image_name",
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/requirements.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/requirements.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import (
     Any,
     Callable,
     cast,
     Dict,
     List,
     Optional,
+    Tuple,
     Union,
 )
 
 from typing_extensions import (
     get_args,
     Literal,
 )
@@ -228,14 +229,19 @@
 ResourceType = Literal[
     "cores_min",
     "cores_max",
     "ram_min",
     "ram_max",
     "tmpdir_min",
     "tmpdir_max",
+    "cuda_version_min",
+    "cuda_compute_capability",
+    "gpu_memory_min",
+    "cuda_device_count_min",
+    "cuda_device_count_max",
 ]
 VALID_RESOURCE_TYPES = get_args(ResourceType)
 
 
 class ResourceRequirement:
     def __init__(self, value_or_expression: Union[int, float, str], resource_type: ResourceType):
         self.value_or_expression = value_or_expression
@@ -246,19 +252,16 @@
         self.resource_type = resource_type
         try:
             float(self.value_or_expression)
             self.runtime_required = False
         except ValueError:
             self.runtime_required = True
 
-    @staticmethod
-    def from_dict(resource_dict):
-        resource_type = next(iter(resource_dict.keys()))
-        value_or_expression = resource_dict[resource_type]
-        return ResourceRequirement(value_or_expression=value_or_expression, resource_type=resource_type)
+    def to_dict(self) -> Dict:
+        return {"resource_type": self.resource_type, "value_or_expression": self.value_or_expression}
 
     def get_value(self, runtime: Optional[Dict] = None, js_evaluator: Optional[Callable] = None):
         if self.runtime_required:
             # TODO: hook up evaluator
             # return js_evaluator(self.value_or_expression, runtime)
             raise NotImplementedError(
                 f"{self.value_or_expression} is not an integer or float value, expressions currently not implemented"
@@ -270,14 +273,19 @@
     cwl_to_galaxy = {
         "coresMin": "cores_min",
         "coresMax": "cores_max",
         "ramMin": "ram_min",
         "ramMax": "ram_max",
         "tmpdirMin": "tmpdir_min",
         "tmpdirMax": "tmpdir_max",
+        "cudaVersionMin": "cuda_version_min",
+        "cudaComputeCapability": "cuda_compute_capability",
+        "gpuMemoryMin": "gpu_memory_min",
+        "cudaDeviceCountMin": "cuda_device_count_min",
+        "cudaDeviceCountMax": "cuda_device_count_max",
     }
     rr = []
     for r in requirements:
         if r.get("class") == "ResourceRequirement":
             valid_key_set = set(cwl_to_galaxy.keys())
         elif r.get("type") == "resource":
             valid_key_set = set(cwl_to_galaxy.values())
@@ -286,22 +294,19 @@
         for key in valid_key_set.intersection(set(r.keys())):
             value = r[key]
             key = cast(ResourceType, cwl_to_galaxy.get(key, key))
             rr.append(ResourceRequirement(value_or_expression=value, resource_type=key))
     return rr
 
 
-def parse_requirements_from_dict(root_dict):
-    requirements = root_dict.get("requirements", [])
-    resource_requirements = resource_requirements_from_list(requirements)
-    containers = root_dict.get("containers", [])
+def parse_requirements_from_lists(software_requirements, containers, resource_requirements) -> Tuple:
     return (
-        ToolRequirements.from_list(requirements),
+        ToolRequirements.from_list(software_requirements),
         [ContainerDescription.from_dict(c) for c in containers],
-        resource_requirements,
+        resource_requirements_from_list(resource_requirements),
     )
 
 
 def parse_requirements_from_xml(xml_root, parse_resources=False):
     """
     Parses requirements, containers and optionally resource requirements from Xml tree.
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/__init__.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,14 @@
         """
         Return a message describing this dependency
         """
         return f"Using dependency {self.name} version {self.version} of type {self.dependency_type}"
 
 
 class ContainerDependency(Dependency):
-
     dict_collection_visible_keys = Dependency.dict_collection_visible_keys + [
         "environment_path",
         "container_description",
         "container_resolver",
     ]
 
     def __init__(self, container_description, name=None, version=None, container_resolver=None):
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/conda.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/conda.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/galaxy_packages.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/galaxy_packages.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/homebrew.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/homebrew.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/lmod.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/lmod.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/modules.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/modules.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/resolver_mixins.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/resolver_mixins.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/tool_shed_packages.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/tool_shed_packages.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/singularity_util.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/singularity_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     cleanenv=DEFAULT_CLEANENV,
 ):
     volumes = volumes or []
     env = env or []
     command_parts = []
     # http://singularity.lbl.gov/docs-environment-metadata
     home = None
-    for (key, value) in env:
+    for key, value in env:
         if key == "HOME":
             home = value
         command_parts.extend([f"SINGULARITYENV_{key}={value}"])
     command_parts += _singularity_prefix(
         singularity_cmd=singularity_cmd,
         sudo=sudo,
         sudo_cmd=sudo_cmd,
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/deps/views.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/deps/views.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/edam_util.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/edam_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 
 EDAM_PREFIX = "http://edamontology.org/"
 
 ROOT_OPERATION = "operation_0004"
 ROOT_TOPIC = "topic_0003"
 
 
-def load_edam_tree(path: Optional[str] = None):
+def load_edam_tree(path: Optional[str] = None, *included_terms: str):
     if path is not None:
         assert os.path.exists(path), f"Failed to load EDAM tabular data at [{path}] path does not exist."
         handle = open(path)
     else:
         assert (
             tabular_stream is not None
-        ), "Failed to load optional import from edam-onotology package, install using [pip install edam-ontology]."
+        ), "Failed to load optional import from edam-ontology package, install using [pip install edam-ontology]."
         handle = tabular_stream()
-    return load_edam_tree_from_tsv_stream(handle)
+    return load_edam_tree_from_tsv_stream(handle, *included_terms)
 
 
-def load_edam_tree_from_tsv_stream(tsv_stream: TextIO):
+def load_edam_tree_from_tsv_stream(tsv_stream: TextIO, *included_terms: str):
     edam: Dict[str, Dict] = {}
 
     def _recurse_edam_parents(term, path=None):
         if edam[term]["parents"] and len(edam[term]["parents"]) > 0:
             for parent in edam[term]["parents"]:
                 yield from _recurse_edam_parents(parent, path + [parent])
         else:
@@ -43,34 +43,34 @@
         fields = line.split("\t")
         if is_first:
             columns = {}
             for i, field in enumerate(fields):
                 columns[field] = i
             is_first = False
 
-            defintion_column = columns["http://www.geneontology.org/formats/oboInOwl#hasDefinition"]
+            definition_column = columns["http://www.geneontology.org/formats/oboInOwl#hasDefinition"]
             term_column = columns["Class ID"]
             label_column = columns["Preferred Label"]
             parents_column = columns["Parents"]
             continue
 
         term = fields[term_column]
         if not term.startswith(EDAM_PREFIX):
             continue
 
         term_id = term[len(EDAM_PREFIX) :]
 
-        # Only care about formats and operations
-        if not (term_id.startswith("operation_") or term_id.startswith("topic_")):
+        # Only care about included terms
+        if included_terms and not (term_id.startswith(included_terms)):
             continue
 
         parents = fields[parents_column].split("|")
         edam[term_id] = {
-            "label": fields[label_column],
-            "definition": fields[defintion_column].strip('"'),
+            "label": fields[label_column].strip('"'),
+            "definition": fields[definition_column].strip('"'),
             "parents": [x[len(EDAM_PREFIX) :] for x in parents if x.startswith(EDAM_PREFIX)],
         }
 
     for term in sorted(edam.keys()):
         tails = []
         for x in _recurse_edam_parents(term, path=[]):
             if x[-2:] not in tails:
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/fetcher.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/fetcher.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,34 @@
+from typing import (
+    Dict,
+    Type,
+    TYPE_CHECKING,
+)
+
 from galaxy.util import plugin_config
 
+if TYPE_CHECKING:
+    from galaxy.tool_util.locations import ToolLocationResolver
+
 
 class ToolLocationFetcher:
     def __init__(self):
         self.resolver_classes = self.__resolvers_dict()
 
-    def __resolvers_dict(self):
+    def __resolvers_dict(self) -> Dict[str, Type["ToolLocationResolver"]]:
         import galaxy.tool_util.locations
 
         return plugin_config.plugins_dict(galaxy.tool_util.locations, "scheme")
 
-    def to_tool_path(self, path_or_uri_like, **kwds):
+    def to_tool_path(self, path_or_uri_like: str, **kwds) -> str:
         if "://" not in path_or_uri_like:
             path = path_or_uri_like
         else:
             uri_like = path_or_uri_like
             if ":" not in path_or_uri_like:
                 raise Exception("Invalid URI passed to get_tool_source")
-            scheme, rest = uri_like.split(":", 2)
+            scheme = uri_like.split(":", 2)[0]
             if scheme not in self.resolver_classes:
                 raise Exception(f"Unknown tool scheme [{scheme}] for URI [{uri_like}]")
             path = self.resolver_classes[scheme]().get_tool_source_path(uri_like)
 
         return path
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/lint.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/lint.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         return len(self.error_messages) > 0
 
     @property
     def found_warns(self) -> bool:
         return len(self.warn_messages) > 0
 
     def lint(self, name: str, lint_func: Callable[[LintTargetType, "LintContext"], None], lint_target: LintTargetType):
-        name = name.replace("tsts", "tests")[len("lint_") :]
+        name = name[len("lint_") :]
         if name in self.skip_types:
             return
 
         if self.level < LintLevel.SILENT:
             # this is a relict from the past where the lint context
             # was reset when called with a new lint_func, as workaround
             # we save the message list, apply the lint_func (which then
@@ -319,19 +319,19 @@
     import galaxy.tool_util.linters
 
     tool_xml = getattr(tool_source, "xml_tree", None)
     tool_type = tool_source.parse_tool_type() or "default"
     linter_modules = submodules.import_submodules(galaxy.tool_util.linters)
     linter_modules.extend(extra_modules)
     for module in linter_modules:
-        lint_tool_types = getattr(module, "lint_tool_types", ["default"])
+        lint_tool_types = getattr(module, "lint_tool_types", ["default", "manage_data"])
         if not ("*" in lint_tool_types or tool_type in lint_tool_types):
             continue
 
-        for (name, value) in inspect.getmembers(module):
+        for name, value in inspect.getmembers(module):
             if callable(value) and name.startswith("lint_"):
                 # Look at the first argument to the linter to decide
                 # if we should lint the XML description or the abstract
                 # tool parser object.
                 first_arg = inspect.getfullargspec(value).args[0]
                 if first_arg == "tool_xml":
                     if tool_xml is None:
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/citations.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/linters/citations.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/command.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/linters/command.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/cwl.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/linters/cwl.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/general.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/linters/general.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/help.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/linters/help.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/inputs.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/linters/inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     ("./column", ["data_column"]),
 ]
 
 
 def lint_inputs(tool_xml, lint_ctx):
     """Lint parameters in a tool's inputs block."""
     datasource = is_datasource(tool_xml)
+    input_names = set()
     inputs = tool_xml.findall("./inputs//param")
     # determine node to report for general problems with outputs
     tool_node = tool_xml.find("./inputs")
     if tool_node is None:
         tool_node = tool_xml.getroot()
     num_inputs = 0
     for param in inputs:
@@ -138,15 +139,32 @@
                     node=param,
                 )
         if param_name.strip() == "":
             lint_ctx.error("Param input with empty name.", node=param)
         elif not is_valid_cheetah_placeholder(param_name):
             lint_ctx.warn(f"Param input [{param_name}] is not a valid Cheetah placeholder.", node=param)
 
-        # TODO lint for params with duplicated name (in inputs & outputs)
+        # check for parameters with duplicate names
+        path = [param_name]
+        parent = param
+        while True:
+            parent = parent.getparent()
+            if parent.tag == "inputs":
+                break
+            # parameters of the same name in different when branches are allowed
+            # just add the value of the when branch to the path (this also allows
+            # that the conditional select has the same name as params in the whens)
+            if parent.tag == "when":
+                path.append(str(parent.attrib.get("value")))
+            else:
+                path.append(str(parent.attrib.get("name")))
+        path_str = ".".join(reversed(path))
+        if path_str in input_names:
+            lint_ctx.error(f"Tool defines multiple parameters with the same name: '{path_str}'", node=param)
+        input_names.add(path_str)
 
         if "type" not in param_attrib:
             lint_ctx.error(f"Param input [{param_name}] input with no type specified.", node=param)
             continue
         elif param_attrib["type"].strip() == "":
             lint_ctx.error(f"Param input [{param_name}] with empty type specified.", node=param)
             continue
@@ -482,14 +500,24 @@
         lint_ctx.info(f"Found {num_inputs} input parameters.", node=tool_node)
     else:
         if datasource:
             lint_ctx.info("No input parameters, OK for data sources", node=tool_node)
         else:
             lint_ctx.warn("Found no input parameters.", node=tool_node)
 
+    # check if there is an output with the same name as an input
+    outputs = tool_xml.find("./outputs")
+    if outputs is not None:
+        for output in outputs:
+            if output.get("name") in input_names:
+                lint_ctx.error(
+                    f'Tool defines an output with a name equal to the name of an input: \'{output.get("name")}\'',
+                    node=output,
+                )
+
 
 def lint_repeats(tool_xml, lint_ctx):
     """Lint repeat blocks in tool inputs."""
     repeats = tool_xml.findall("./inputs//repeat")
     for repeat in repeats:
         if "name" not in repeat.attrib:
             lint_ctx.error("Repeat does not specify name attribute.", node=repeat)
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/outputs.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/linters/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     # if allowed (e.g. for discover_datasets), ext takes precedence over format
     fmt = None
     if allow_ext:
         fmt = node.attrib.get("ext")
     if fmt is None:
         fmt = node.attrib.get("format")
     if fmt == "input":
-        lint_ctx.warn(
+        lint_ctx.error(
             f"Using format='input' on {node.tag}, format_source attribute is less ambiguous and should be used instead.",
             node=node,
         )
     return fmt is not None
 
 
 def __check_pattern(node):
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/stdio.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/linters/stdio.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/tests.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/linters/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,36 @@
 """This module contains a linting functions for tool tests."""
 import typing
 from inspect import (
     Parameter,
     signature,
 )
 
+from galaxy.util import asbool
 from ._util import is_datasource
 from ..verify import asserts
 
 
-# Misspelled so as not be picked up by nosetests.
-def lint_tsts(tool_xml, lint_ctx):
+def check_compare_attribs(element, lint_ctx, test_idx):
+    COMPARE_COMPATIBILITY = {
+        "sort": ["diff", "re_match", "re_match_multiline"],
+        "lines_diff": ["diff", "re_match", "contains"],
+        "decompress": ["diff"],
+        "delta": ["sim_size"],
+        "delta_frac": ["sim_size"],
+    }
+    compare = element.get("compare", "diff")
+    for attrib in COMPARE_COMPATIBILITY:
+        if attrib in element.attrib and compare not in COMPARE_COMPATIBILITY[attrib]:
+            lint_ctx.error(
+                f'Test {test_idx}: Attribute {attrib} is incompatible with compare="{compare}".', node=element
+            )
+
+
+def lint_tests(tool_xml, lint_ctx):
     # determine node to report for general problems with tests
     tests = tool_xml.findall("./tests/test")
     general_node = tool_xml.find("./tests")
     if general_node is None:
         general_node = tool_xml.getroot()
     datasource = is_datasource(tool_xml)
     if not tests:
@@ -34,19 +50,24 @@
                 break
         test_assert = ("assert_stdout", "assert_stderr", "assert_command")
         for ta in test_assert:
             assertions = test.findall(ta)
             if len(assertions) == 0:
                 continue
             if len(assertions) > 1:
-                lint_ctx.error(f"Test {test_idx}: More than one {ta} found. Only the first is considered.")
+                lint_ctx.error(f"Test {test_idx}: More than one {ta} found. Only the first is considered.", node=test)
             has_test = True
             _check_asserts(test_idx, assertions, lint_ctx)
         _check_asserts(test_idx, test.findall(".//assert_contents"), lint_ctx)
 
+        # check if expect_num_outputs is set if there are outputs with filters
+        filter = tool_xml.findall("./outputs//filter")
+        if len(filter) > 0 and "expect_num_outputs" not in test.attrib:
+            lint_ctx.warn("Test should specify 'expect_num_outputs' if outputs have filters", node=test)
+
         # really simple test that test parameters are also present in the inputs
         for param in test.findall("param"):
             name = param.attrib.get("name", None)
             if not name:
                 lint_ctx.error(f"Test {test_idx}: Found test param tag without a name defined.", node=param)
                 continue
             name = name.split("|")[-1]
@@ -74,14 +95,21 @@
             if name not in output_data_or_collection:
                 lint_ctx.error(
                     f"Test {test_idx}: Found {output.tag} tag with unknown name [{name}], valid names {list(output_data_or_collection)}",
                     node=output,
                 )
                 continue
 
+            if output.tag == "output":
+                check_compare_attribs(output, lint_ctx, test_idx)
+            elements = output.findall("./element")
+            if elements:
+                for element in elements:
+                    check_compare_attribs(element, lint_ctx, test_idx)
+
             # check that
             # - test/output corresponds to outputs/data and
             # - test/collection to outputs/output_collection
             corresponding_output = output_data_or_collection[name]
             if output.tag == "output" and corresponding_output.tag != "data":
                 lint_ctx.error(
                     f"Test {test_idx}: test output {name} does not correspond to a 'data' output, but a '{corresponding_output.tag}'",
@@ -98,34 +126,39 @@
             if discover_datasets is not None:
                 if output.tag == "output":
                     if "count" not in output.attrib and output.find("./discovered_dataset") is None:
                         lint_ctx.error(
                             f"Test {test_idx}: test output '{name}' must have a 'count' attribute and/or 'discovered_dataset' children",
                             node=output,
                         )
-                        pass
                 else:
-                    elements = output.findall("./element")
                     if "count" not in output.attrib and len(elements) == 0:
                         lint_ctx.error(
                             f"Test {test_idx}: test collection '{name}' must have a 'count' attribute or 'element' children",
                             node=output,
                         )
                     if corresponding_output.get("type", "") in ["list:list", "list:paired"]:
                         nested_elements = output.find("./element/element")
                         element_with_count = output.find("./element[@count]")
                         if nested_elements is None and element_with_count is None:
                             lint_ctx.error(
                                 f"Test {test_idx}: test collection '{name}' must contain nested 'element' tags and/or element childen with a 'count' attribute",
                                 node=output,
                             )
 
-        if "expect_failure" in test.attrib and found_output_test:
-            lint_ctx.error(f"Test {test_idx}: Cannot specify outputs in a test expecting failure.", node=test)
-            continue
+        if "expect_failure" in test.attrib and asbool(test.attrib["expect_failure"]):
+            if found_output_test:
+                lint_ctx.error(f"Test {test_idx}: Cannot specify outputs in a test expecting failure.", node=test)
+                continue
+            if "expect_num_outputs" in test.attrib:
+                lint_ctx.error(
+                    f"Test {test_idx}: Cannot make assumptions on the number of outputs in a test expecting failure.",
+                    node=test,
+                )
+                continue
 
         has_test = has_test or found_output_test
         if not has_test:
             lint_ctx.warn(
                 f"Test {test_idx}: No outputs or expectations defined for tests, this test is likely invalid.",
                 node=test,
             )
@@ -148,44 +181,32 @@
             if i == 0:  # skip root note itself
                 continue
             assert_function_name = "assert_" + a.tag
             if assert_function_name not in asserts.assertion_functions:
                 lint_ctx.error(f"Test {test_idx}: unknown assertion '{a.tag}'", node=a)
                 continue
             assert_function_sig = signature(asserts.assertion_functions[assert_function_name])
-            # check type of the attributes (int, float ...)
+            # check of the attributes
             for attrib in a.attrib:
                 if attrib not in assert_function_sig.parameters:
                     lint_ctx.error(f"Test {test_idx}: unknown attribute '{attrib}' for '{a.tag}'", node=a)
                     continue
-                annotation = assert_function_sig.parameters[attrib].annotation
-                annotation = _handle_optionals(annotation)
-                if annotation is not Parameter.empty:
-                    try:
-                        annotation(a.attrib[attrib])
-                    except TypeError:
-                        raise Exception(f"Faild to instantiate {attrib} for {assert_function_name}")
-                    except ValueError:
-                        lint_ctx.error(
-                            f"Test {test_idx}: attribute '{attrib}' for '{a.tag}' needs to be '{annotation.__name__}' got '{a.attrib[attrib]}'",
-                            node=a,
-                        )
             # check missing required attributes
             for p in assert_function_sig.parameters:
                 if p in ["output", "output_bytes", "verify_assertions_function", "children"]:
                     continue
                 if assert_function_sig.parameters[p].default is Parameter.empty and p not in a.attrib:
                     lint_ctx.error(f"Test {test_idx}: missing attribute '{p}' for '{a.tag}'", node=a)
             # has_n_lines, has_n_columns, and has_size need to specify n/value, min, or max
             if a.tag in ["has_n_lines", "has_n_columns"]:
                 if "n" not in a.attrib and "min" not in a.attrib and "max" not in a.attrib:
                     lint_ctx.error(f"Test {test_idx}: '{a.tag}' needs to specify 'n', 'min', or 'max'", node=a)
             if a.tag == "has_size":
                 if "value" not in a.attrib and "min" not in a.attrib and "max" not in a.attrib:
-                    lint_ctx.error(f"Test {test_idx}: '{a.tag}' needs to specify 'n', 'min', or 'max'", node=a)
+                    lint_ctx.error(f"Test {test_idx}: '{a.tag}' needs to specify 'value', 'min', or 'max'", node=a)
 
 
 def _handle_optionals(annotation):
     as_dict = annotation.__dict__
     if "__origin__" in as_dict and as_dict["__origin__"] == typing.Union:
         return as_dict["__args__"][0]
     return annotation
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/linters/xml_order.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/linters/xml_order.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/loader_directory.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/loader_directory.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/locations/__init__.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/locations/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,20 @@
+import abc
 import tempfile
-from abc import (
-    ABCMeta,
-    abstractmethod,
-    abstractproperty,
-)
 
 
-class ToolLocationResolver(metaclass=ABCMeta):
+class ToolLocationResolver(metaclass=abc.ABCMeta):
     """Parse a URI-like string and return a ToolSource object."""
 
-    @abstractproperty
+    @property
+    @abc.abstractmethod
     def scheme(self):
         """Short label for the type of location resolver and URI scheme."""
 
-    @abstractmethod
-    def get_tool_source_path(self, uri_like):
+    @abc.abstractmethod
+    def get_tool_source_path(self, uri_like: str) -> str:
         """Return a local path for the uri_like string."""
 
     def _temp_path(self, uri_like):
         """Create an abstraction for this so we can configure and cache later."""
         with tempfile.NamedTemporaryFile(suffix=uri_like.split("/")[-1], delete=False) as temp:
             return temp.name
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/locations/dockstore.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/locations/dockstore.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from urllib.parse import quote
 
 import requests
 import yaml
 
 from galaxy.util import DEFAULT_SOCKET_TIMEOUT
-from ..locations import ToolLocationResolver
+from . import ToolLocationResolver
 
 
 class DockStoreResolver(ToolLocationResolver):
-
     scheme = "dockstore"
 
-    def get_tool_source_path(self, uri_like):
+    def get_tool_source_path(self, uri_like: str) -> str:
         assert uri_like.startswith("dockstore://")
         tool_id = uri_like[len("dockstore://") :]
         if ":" in tool_id:
             tool_id, version = tool_id.split(":", 1)
         else:
             tool_id, version = tool_id, "latest"
         tmp_path = self._temp_path(f"{uri_like}.cwl")
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/ontologies/ontology_data.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/ontologies/ontology_data.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/output_checker.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/output_checker.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/cwl.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/parser/cwl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+import json
 import logging
 import math
-import os
+from typing import Optional
 
-from galaxy.tool_util.cwl.parser import tool_proxy
+import packaging.version
+
+from galaxy.tool_util.cwl.parser import (
+    tool_proxy,
+    ToolProxy,
+)
 from galaxy.tool_util.deps import requirements
 from .interface import (
     PageSource,
     PagesSource,
     ToolSource,
 )
 from .output_actions import ToolOutputActionGroup
@@ -17,39 +23,37 @@
 )
 from .yaml import YamlInputSource
 
 log = logging.getLogger(__name__)
 
 
 class CwlToolSource(ToolSource):
-
     language = "yaml"
 
-    def __init__(self, tool_file, strict_cwl_validation=True, tool_id=None, tool_proxy=None):
+    def __init__(self, tool_file=None, strict_cwl_validation=True, tool_proxy: Optional[ToolProxy] = None):
         self._cwl_tool_file = tool_file
-        self._id = tool_id or os.path.splitext(os.path.basename(tool_file))[0]
         self._tool_proxy = tool_proxy
         self._source_path = tool_file
         self._strict_cwl_validation = strict_cwl_validation
 
     @property
     def source_path(self):
         return self._source_path
 
     @property
-    def tool_proxy(self):
+    def tool_proxy(self) -> ToolProxy:
         if self._tool_proxy is None:
             self._tool_proxy = tool_proxy(self._source_path, strict_cwl_validation=self._strict_cwl_validation)
         return self._tool_proxy
 
     def parse_tool_type(self):
         return "cwl"
 
     def parse_id(self):
-        return self._id
+        return self.tool_proxy.galaxy_id()
 
     def parse_name(self):
         return self.tool_proxy.label() or self.parse_id()
 
     def parse_command(self):
         return "$__cwl_command"
 
@@ -149,32 +153,34 @@
         containers = []
         docker_identifier = self.tool_proxy.docker_identifier()
         if docker_identifier:
             containers.append({"type": "docker", "identifier": docker_identifier})
 
         software_requirements = self.tool_proxy.software_requirements()
         resource_requirements = self.tool_proxy.resource_requirements()
-        return requirements.parse_requirements_from_dict(
-            dict(
-                requirements=list(
-                    map(lambda r: {"name": r[0], "version": r[1], "type": "package"}, software_requirements)
-                ),
-                containers=containers,
-                resource_requirements=resource_requirements,
-            )
+        return requirements.parse_requirements_from_lists(
+            software_requirements=[{"name": r[0], "version": r[1], "type": "package"} for r in software_requirements],
+            containers=containers,
+            resource_requirements=resource_requirements,
         )
 
     def parse_profile(self):
-        return "16.04"
+        return "17.09"
+
+    def parse_xrefs(self):
+        return []
 
     def parse_license(self):
         return None
 
     def parse_python_template_version(self):
-        return "3.5"
+        return packaging.version.Version("3.5")
+
+    def to_string(self):
+        return json.dumps(self.tool_proxy.to_persistent_representation())
 
 
 class CwlPageSource(PageSource):
     def __init__(self, tool_proxy):
         cwl_instances = tool_proxy.input_instances()
         self._input_list = list(map(self._to_input_source, cwl_instances))
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/factory.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/parser/factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 """Constructors for concrete tool and input source objects."""
 
 import logging
+from typing import (
+    Callable,
+    Dict,
+    List,
+    Optional,
+)
 
 from yaml import safe_load
 
 from galaxy.tool_util.loader import load_tool_with_refereces
-from galaxy.util import parse_xml_string_to_etree
+from galaxy.util import (
+    ElementTree,
+    parse_xml_string_to_etree,
+)
 from galaxy.util.yaml_util import ordered_load
 from .cwl import (
     CwlToolSource,
     tool_proxy,
 )
 from .interface import (
     InputSource,
@@ -24,43 +33,43 @@
     YamlToolSource,
 )
 from ..fetcher import ToolLocationFetcher
 
 log = logging.getLogger(__name__)
 
 
-def build_xml_tool_source(xml_string):
+def build_xml_tool_source(xml_string: str) -> XmlToolSource:
     return XmlToolSource(parse_xml_string_to_etree(xml_string))
 
 
-def build_cwl_tool_source(yaml_string):
-    tool_proxy(tool_object=safe_load(yaml_string))
+def build_cwl_tool_source(yaml_string: str) -> CwlToolSource:
+    proxy = tool_proxy(tool_object=safe_load(yaml_string))
     # regular CwlToolSource sets basename as tool id, but that's not going to cut it in production
-    return CwlToolSource(tool_file=None, tool_id="serialized_cwl_tool", tool_proxy=tool_proxy)
+    return CwlToolSource(tool_proxy=proxy)
 
 
-def build_yaml_tool_source(yaml_string):
+def build_yaml_tool_source(yaml_string: str) -> YamlToolSource:
     return YamlToolSource(safe_load(yaml_string))
 
 
-TOOL_SOURCE_FACTORIES = {
+TOOL_SOURCE_FACTORIES: Dict[str, Callable[[str], ToolSource]] = {
     "XmlToolSource": build_xml_tool_source,
     "YamlToolSource": build_yaml_tool_source,
     "CwlToolSource": build_cwl_tool_source,
 }
 
 
 def get_tool_source(
-    config_file=None,
-    xml_tree=None,
-    enable_beta_formats=True,
-    tool_location_fetcher=None,
-    macro_paths=None,
-    tool_source_class=None,
-    raw_tool_source=None,
+    config_file: Optional[str] = None,
+    xml_tree: Optional[ElementTree] = None,
+    enable_beta_formats: bool = True,
+    tool_location_fetcher: Optional[ToolLocationFetcher] = None,
+    macro_paths: Optional[List[str]] = None,
+    tool_source_class: Optional[str] = None,
+    raw_tool_source: Optional[str] = None,
 ) -> ToolSource:
     """Return a ToolSource object corresponding to supplied source.
 
     The supplied source may be specified as a file path (using the config_file
     parameter) or as an XML object loaded with load_tool_with_refereces.
     """
     if xml_tree is not None:
@@ -71,14 +80,15 @@
     if tool_source_class and raw_tool_source:
         factory = TOOL_SOURCE_FACTORIES[tool_source_class]
         return factory(raw_tool_source)
 
     if tool_location_fetcher is None:
         tool_location_fetcher = ToolLocationFetcher()
 
+    assert config_file
     config_file = tool_location_fetcher.to_tool_path(config_file)
     if not enable_beta_formats:
         tree, macro_paths = load_tool_with_refereces(config_file)
         return XmlToolSource(tree, source_path=config_file, macro_paths=macro_paths)
 
     if config_file.endswith(".yml"):
         log.info("Loading tool from YAML - this is experimental - tool will not function in future.")
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/interface.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/parser/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,34 +3,69 @@
 import re
 from abc import (
     ABCMeta,
     abstractmethod,
 )
 from os.path import join
 from typing import (
+    Any,
     Dict,
     List,
     Optional,
+    Tuple,
+    Union,
 )
 
+import packaging.version
+from typing_extensions import TypedDict
+
 from galaxy.util.path import safe_walk
 from .util import _parse_name
 
 NOT_IMPLEMENTED_MESSAGE = "Galaxy tool format does not yet support this tool feature."
 
 
+class AssertionDict(TypedDict):
+    tag: str
+    attributes: Dict[str, Any]
+    children: Optional[List[Dict[str, Any]]]
+
+
+AssertionList = Optional[List[AssertionDict]]
+XmlInt = Union[str, int]
+
+
+class ToolSourceTest(TypedDict):
+    inputs: Any
+    outputs: Any
+    output_collections: List[Any]
+    stdout: AssertionList
+    stderr: AssertionList
+    expect_exit_code: Optional[XmlInt]
+    expect_failure: bool
+    expect_test_failure: bool
+    maxseconds: Optional[XmlInt]
+    expect_num_outputs: Optional[XmlInt]
+    command: AssertionList
+    command_version: AssertionList
+
+
+class ToolSourceTests(TypedDict):
+    tests: List[ToolSourceTest]
+
+
 class ToolSource(metaclass=ABCMeta):
     """This interface represents an abstract source to parse tool
     information from.
     """
 
     language: str
 
     @abstractmethod
-    def parse_id(self):
+    def parse_id(self) -> Optional[str]:
         """Parse an ID describing the abstract tool. This is not the
         GUID tracked by the tool shed but the simple id (there may be
         multiple tools loaded in Galaxy with this same simple id).
         """
 
     @abstractmethod
     def parse_version(self):
@@ -66,14 +101,15 @@
         """Parse list of edam operation codes."""
         return []
 
     def parse_edam_topics(self) -> List[str]:
         """Parse list of edam topic codes."""
         return []
 
+    @abstractmethod
     def parse_xrefs(self) -> List[Dict[str, str]]:
         """Parse list of external resource URIs and types."""
 
     def parse_display_interface(self, default):
         """Parse display_interface - fallback to default for the tool type
         (supplied as default parameter) if not specified.
         """
@@ -177,15 +213,15 @@
         return False
 
     def parse_required_files(self) -> Optional["RequiredFiles"]:
         """Parse explicit RequiredFiles object or return None to let Galaxy decide implicit logic."""
         return None
 
     @abstractmethod
-    def parse_requirements_and_containers(self):
+    def parse_requirements_and_containers(self) -> Tuple:
         """Return triple of ToolRequirement, ContainerDescription and ResourceRequirement lists."""
 
     @abstractmethod
     def parse_input_pages(self):
         """Return a PagesSource representing inputs by page for tool."""
 
     def parse_provided_metadata_style(self):
@@ -234,15 +270,15 @@
         """Return tool profile version as Galaxy major e.g. 16.01 or 16.04."""
 
     @abstractmethod
     def parse_license(self):
         """Return license corresponding to tool wrapper."""
 
     @abstractmethod
-    def parse_python_template_version(self):
+    def parse_python_template_version(self) -> Optional[packaging.version.Version]:
         """
         Return minimum python version that the tool template has been developed against.
         """
 
     def parse_creator(self):
         """Return list of metadata relating to creator/author of tool.
 
@@ -260,25 +296,29 @@
 
     def paths_and_modtimes(self):
         paths_and_modtimes = {p: os.path.getmtime(p) for p in self.macro_paths}
         if self.source_path:
             paths_and_modtimes[self.source_path] = os.path.getmtime(self.source_path)
         return paths_and_modtimes
 
-    def parse_tests_to_dict(self):
+    def parse_tests_to_dict(self) -> ToolSourceTests:
         return {"tests": []}
 
     def __str__(self):
         source_path = self.source_path
         if source_path:
             as_str = f"{self.__class__.__name__}[{source_path}]"
         else:
             as_str = f"{self.__class__.__name__}[In-memory]"
         return as_str
 
+    @abstractmethod
+    def to_string(self) -> str:
+        """Return the tool source as a string"""
+
 
 class PagesSource:
     """Contains a list of Pages - each a list of InputSources -
     each item in the outer list representing a page of inputs.
     Pages are deprecated so ideally this outer list will always
     be exactly a singleton.
     """
@@ -287,23 +327,14 @@
         self.page_sources = page_sources
 
     @property
     def inputs_defined(self):
         return True
 
 
-class PageSource(metaclass=ABCMeta):
-    def parse_display(self):
-        return None
-
-    @abstractmethod
-    def parse_input_sources(self) -> List:
-        """Return a list of InputSource objects."""
-
-
 class InputSource(metaclass=ABCMeta):
     default_optional = False
 
     def elem(self):
         # For things in transition that still depend on XML - provide a way
         # to grab it and just throw an error if feature is attempted to be
         # used with other tool sources.
@@ -328,14 +359,18 @@
         """Return name of an input source
         returns the name or if absent the argument property
         In the latter case, leading dashes are stripped and
         all remaining dashes are replaced by underscores.
         """
         return _parse_name(self.get("name"), self.get("argument"))
 
+    @abstractmethod
+    def parse_input_type(self) -> str:
+        """Return the type of this input."""
+
     def parse_help(self):
         return self.get("help")
 
     def parse_sanitizer_elem(self):
         """Return an XML description of sanitizers. This is a stop gap
         until we can rework galaxy.tools.parameters.sanitize to not
         explicitly depend on XML.
@@ -346,15 +381,15 @@
         """Return an XML description of sanitizers. This is a stop gap
         until we can rework galaxy.tools.parameters.validation to not
         explicitly depend on XML.
         """
         return []
 
     def parse_optional(self, default=None):
-        """Return boolean indicating wheter parameter is optional."""
+        """Return boolean indicating whether parameter is optional."""
         if default is None:
             default = self.default_optional
         return self.get_bool("optional", default)
 
     def parse_dynamic_options_elem(self):
         """Return an XML elemnt describing dynamic options."""
         return None
@@ -369,22 +404,31 @@
         """Return list of (name, extension) to describe explicit conversions."""
         return []
 
     def parse_nested_inputs_source(self):
         # For repeats
         raise NotImplementedError(NOT_IMPLEMENTED_MESSAGE)
 
-    def parse_test_input_source(self):
+    def parse_test_input_source(self) -> "InputSource":
         # For conditionals
         raise NotImplementedError(NOT_IMPLEMENTED_MESSAGE)
 
     def parse_when_input_sources(self):
         raise NotImplementedError(NOT_IMPLEMENTED_MESSAGE)
 
 
+class PageSource(metaclass=ABCMeta):
+    def parse_display(self):
+        return None
+
+    @abstractmethod
+    def parse_input_sources(self) -> List[InputSource]:
+        """Return a list of InputSource objects."""
+
+
 class TestCollectionDef:
     __test__ = False  # Prevent pytest from discovering this class (issue #12071)
 
     def __init__(self, attrib, name, collection_type, elements):
         self.attrib = attrib
         self.collection_type = collection_type
         self.elements = elements
@@ -496,15 +540,15 @@
         excludes = self.excludes
         if self.extend_default_excludes:
             excludes.append({"path": "tool-data", "path_type": "prefix"})
             excludes.append({"path": "test-data", "path_type": "prefix"})
             excludes.append({"path": ".hg", "path_type": "prefix"})
 
         files: List[str] = []
-        for (dirpath, _, filenames) in safe_walk(tool_directory):
+        for dirpath, _, filenames in safe_walk(tool_directory):
             for filename in filenames:
                 rel_path = join(dirpath, filename).replace(tool_directory + os.path.sep, "")
                 if matches(self.includes, rel_path) and not matches(self.excludes, rel_path):
                     files.append(rel_path)
         return files
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/output_actions.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/parser/output_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 if elem.tag == "conditional":
                     self.actions.append(ToolOutputActionConditional(self, elem))
                 elif elem.tag == "action":
                     self.actions.append(ToolOutputAction.from_elem(self, elem))
                 else:
                     log.debug(f"Unknown ToolOutputAction tag specified: {elem.tag}")
 
-    def apply_action(self, output_dataset, other_values):
+    def apply_action(self, output_dataset, other_values) -> None:
         for action in self.actions:
             action.apply_action(output_dataset, other_values)
 
     @property
     def tool(self):
         return self.parent.tool
 
@@ -58,46 +58,46 @@
                 return DatatypeIsInstanceToolOutputActionConditionalWhen(parent, when_elem, when_value)
         raise TypeError("When type not implemented")
 
     def __init__(self, parent, config_elem, value):
         super().__init__(parent, config_elem)
         self.value = value
 
-    def is_case(self, output_dataset, other_values):
+    def is_case(self, other_values):
         raise TypeError("Not implemented")
 
-    def get_ref(self, output_dataset, other_values):
+    def get_ref(self, other_values):
         ref = other_values
         for ref_name in self.parent.name:
             assert ref_name in ref, f"Required dependency '{ref_name}' not found in incoming values"
             ref = ref.get(ref_name)
         return ref
 
-    def apply_action(self, output_dataset, other_values):
-        if self.is_case(output_dataset, other_values):
-            return super().apply_action(output_dataset, other_values)
+    def apply_action(self, output_dataset, other_values) -> None:
+        if self.is_case(other_values):
+            super().apply_action(output_dataset, other_values)
 
 
 class ValueToolOutputActionConditionalWhen(ToolOutputActionConditionalWhen):
     tag = "when value"
 
-    def is_case(self, output_dataset, other_values):
-        ref = self.get_ref(output_dataset, other_values)
+    def is_case(self, other_values) -> bool:
+        ref = self.get_ref(other_values)
         return ref == self.value
 
 
 class DatatypeIsInstanceToolOutputActionConditionalWhen(ToolOutputActionConditionalWhen):
     tag = "when datatype_isinstance"
 
     def __init__(self, parent, config_elem, value):
         super().__init__(parent, config_elem, value)
         self.value = type(self.tool.app.datatypes_registry.get_datatype_by_extension(value))
 
-    def is_case(self, output_dataset, other_values):
-        ref = self.get_ref(output_dataset, other_values)
+    def is_case(self, other_values) -> bool:
+        ref = self.get_ref(other_values)
         return isinstance(ref.datatype, self.value)
 
 
 class ToolOutputActionConditional:
     tag = "conditional"
 
     def __init__(self, parent, config_elem):
@@ -105,15 +105,15 @@
         self.name = config_elem.get("name", None)
         assert self.name is not None, "Required 'name' attribute missing from ToolOutputActionConditional"
         self.name = self.name.split(".")
         self.cases = []
         for when_elem in config_elem.findall("when"):
             self.cases.append(ToolOutputActionConditionalWhen.from_elem(self, when_elem))
 
-    def apply_action(self, output_dataset, other_values):
+    def apply_action(self, output_dataset, other_values) -> None:
         for case in self.cases:
             case.apply_action(output_dataset, other_values)
 
     @property
     def tool(self):
         return self.parent.tool
 
@@ -299,15 +299,15 @@
     tag = "metadata"
 
     def __init__(self, parent, elem):
         super().__init__(parent, elem)
         self.name = elem.get("name", None)
         assert self.name is not None, "Required 'name' attribute missing from MetadataToolOutputAction"
 
-    def apply_action(self, output_dataset, other_values):
+    def apply_action(self, output_dataset, other_values) -> None:
         value = self.option.get_value(other_values)
         # TODO: figure out correct type based on MetadataElementSpec,
         # but MetadataElementSpec doesn't actually define a type (but it should).
         # That would avoid the ad-hoc comma splitting here for defaults.
         if self.default:
             # For historical reasons the default value takes preference over value,
             # and we only treat the default value as potentially containing cheetah.
@@ -323,15 +323,15 @@
 class FormatToolOutputAction(ToolOutputAction):
     tag = "format"
 
     def __init__(self, parent, elem):
         super().__init__(parent, elem)
         self.default = elem.get("default", None)
 
-    def apply_action(self, output_dataset, other_values):
+    def apply_action(self, output_dataset, other_values) -> None:
         value = self.option.get_value(other_values)
         if value is None and self.default is not None:
             value = self.default
         if value is not None:
             output_dataset.extension = value
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/output_collection_def.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/parser/output_collection_def.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,29 +100,27 @@
 
     @property
     def discover_patterns(self) -> List[str]:
         return []
 
 
 class ToolProvidedMetadataDatasetCollection(DatasetCollectionDescription):
-
     discover_via = "tool_provided_metadata"
 
 
 class FilePatternDatasetCollectionDescription(DatasetCollectionDescription):
-
     discover_via = "pattern"
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         pattern = kwargs.get("pattern", "__default__")
         self.recurse = asbool(kwargs.get("recurse", False))
         self.match_relative_path = asbool(kwargs.get("match_relative_path", False))
         if pattern in NAMED_PATTERNS:
-            pattern = NAMED_PATTERNS.get(pattern)
+            pattern = NAMED_PATTERNS[pattern]
         self.pattern = pattern
         self.sort_by = sort_by = kwargs.get("sort_by", DEFAULT_SORT_BY)
         if sort_by.startswith("reverse_"):
             self.sort_reverse = True
             sort_by = sort_by[len("reverse_") :]
         else:
             self.sort_reverse = False
@@ -145,14 +143,14 @@
                 "recurse": self.recurse,
                 "sort_by": self.sort_by,
             }
         )
         return as_dict
 
     @property
-    def discover_patterns(self):
+    def discover_patterns(self) -> List[str]:
         return [self.pattern]
 
 
 DEFAULT_DATASET_COLLECTOR_DESCRIPTION = FilePatternDatasetCollectionDescription(
     default_dbkey=LEGACY_DEFAULT_DBKEY,
 )
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/output_objects.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/parser/output_objects.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,32 @@
-from typing import List
+from typing import (
+    Any,
+    Dict,
+    List,
+    Optional,
+)
 
+from galaxy.util import Element
 from galaxy.util.dictifiable import Dictifiable
 from .output_actions import ToolOutputActionGroup
 from .output_collection_def import (
     dataset_collector_descriptions_from_output_dict,
     DatasetCollectionDescription,
 )
 
 
 class ToolOutputBase(Dictifiable):
-    def __init__(self, name, label=None, filters=None, hidden=False, from_expression=None):
+    def __init__(
+        self,
+        name: str,
+        label: Optional[str] = None,
+        filters: Optional[List[Element]] = None,
+        hidden: bool = False,
+        from_expression: Optional[str] = None,
+    ) -> None:
         super().__init__()
         self.name = name
         self.label = label
         self.filters = filters or []
         self.hidden = hidden
         self.collection = False
         self.from_expression = from_expression
@@ -46,43 +59,46 @@
         "parent",
         "count",
         "from_work_dir",
     ]
 
     def __init__(
         self,
-        name,
-        format=None,
-        format_source=None,
-        metadata_source=None,
-        parent=None,
-        label=None,
-        filters=None,
-        actions=None,
-        hidden=False,
-        implicit=False,
-        from_expression=None,
-    ):
+        name: str,
+        format: Optional[str] = None,
+        format_source: Optional[str] = None,
+        metadata_source: Optional[str] = None,
+        parent: Optional[str] = None,
+        label: Optional[str] = None,
+        filters: Optional[List[Element]] = None,
+        actions: Optional[ToolOutputActionGroup] = None,
+        hidden: bool = False,
+        implicit: bool = False,
+        from_expression: Optional[str] = None,
+    ) -> None:
         super().__init__(name, label=label, filters=filters, hidden=hidden, from_expression=from_expression)
         self.output_type = "data"
         self.format = format
         self.format_source = format_source
         self.metadata_source = metadata_source
         self.parent = parent
         self.actions = actions
 
         # Initialize default values
-        self.change_format = []
+        self.change_format: List[Element] = []
         self.implicit = implicit
-        self.from_work_dir = None
+        self.from_work_dir: Optional[str] = None
         self.dataset_collector_descriptions: List[DatasetCollectionDescription] = []
+        self.default_identifier_source: Optional[str] = None
+        self.count: Optional[int] = None
+        self.tool: Optional[Any]
 
     # Tuple emulation
 
-    def __len__(self):
+    def __len__(self) -> int:
         return 3
 
     def __getitem__(self, index):
         if index == 0:
             return self.format
         elif index == 1:
             return self.metadata_source
@@ -102,28 +118,28 @@
             as_dict["edam_format"] = edam_format
             edam_data = app.datatypes_registry.edam_data.get(self.format)
             as_dict["edam_data"] = edam_data
         as_dict["discover_datasets"] = list(map(lambda d: d.to_dict(), self.dataset_collector_descriptions))
         return as_dict
 
     @staticmethod
-    def from_dict(name, output_dict, tool=None):
+    def from_dict(name: str, output_dict: Dict[str, Any], tool: Optional[object] = None) -> "ToolOutput":
         output = ToolOutput(name)
         output.format = output_dict.get("format", "data")
         output.change_format = []
         output.format_source = output_dict.get("format_source", None)
         output.default_identifier_source = output_dict.get("default_identifier_source", None)
         output.metadata_source = output_dict.get("metadata_source", "")
         output.parent = output_dict.get("parent", None)
         output.label = output_dict.get("label", None)
         output.count = output_dict.get("count", 1)
         output.filters = []
         output.tool = tool
         output.from_work_dir = output_dict.get("from_work_dir", None)
-        output.hidden = output_dict.get("hidden", "")
+        output.hidden = output_dict.get("hidden", False)
         # TODO: implement tool output action group fixes
         output.actions = ToolOutputActionGroup(output, None)
         output.dataset_collector_descriptions = dataset_collector_descriptions_from_output_dict(output_dict)
         return output
 
     @property
     def output_discover_patterns(self) -> List[str]:
@@ -179,38 +195,38 @@
         "default_metadata_source",
         "inherit_format",
         "inherit_metadata",
     ]
 
     def __init__(
         self,
-        name,
-        structure,
-        label=None,
-        filters=None,
-        hidden=False,
-        default_format="data",
-        default_format_source=None,
-        default_metadata_source=None,
-        inherit_format=False,
-        inherit_metadata=False,
-    ):
+        name: str,
+        structure: "ToolOutputCollectionStructure",
+        label: Optional[str] = None,
+        filters: Optional[List[Element]] = None,
+        hidden: bool = False,
+        default_format: str = "data",
+        default_format_source: Optional[str] = None,
+        default_metadata_source: Optional[str] = None,
+        inherit_format: bool = False,
+        inherit_metadata: bool = False,
+    ) -> None:
         super().__init__(name, label=label, filters=filters, hidden=hidden)
         self.output_type = "collection"
         self.collection = True
         self.default_format = default_format
         self.structure = structure
-        self.outputs = {}
+        self.outputs: Dict[str, str] = {}
 
         self.inherit_format = inherit_format
         self.inherit_metadata = inherit_metadata
 
         self.metadata_source = default_metadata_source
         self.format_source = default_format_source
-        self.change_format = []  # TODO
+        self.change_format: List = []  # TODO: not implemented
 
     def known_outputs(self, inputs, type_registry):
         if self.dynamic_structure:
             return []
 
         # This line is probably not right - should verify structured_like
         # or have outputs and all outputs have name.
@@ -271,21 +287,21 @@
 
     def to_dict(self, view="collection", value_mapper=None, app=None):
         as_dict = super().to_dict(view=view, value_mapper=value_mapper, app=app)
         as_dict["structure"] = self.structure.to_dict()
         return as_dict
 
     @staticmethod
-    def from_dict(name, output_dict, tool=None):
+    def from_dict(name, output_dict, tool=None) -> "ToolOutputCollection":
         structure = ToolOutputCollectionStructure.from_dict(output_dict["structure"])
         rval = ToolOutputCollection(
             name,
             structure=structure,
             label=output_dict.get("label", None),
-            filters=None,
+            filters=[],
             hidden=output_dict.get("hidden", False),
             default_format=output_dict.get("default_format", "data"),
             default_format_source=output_dict.get("default_format_source", None),
             default_metadata_source=output_dict.get("default_metadata_source", None),
             inherit_format=output_dict.get("inherit_format", False),
             inherit_metadata=output_dict.get("inherit_metadata", False),
         )
@@ -295,20 +311,20 @@
     def output_discover_patterns(self) -> List[str]:
         return self.structure.output_discover_patterns
 
 
 class ToolOutputCollectionStructure:
     def __init__(
         self,
-        collection_type,
-        collection_type_source=None,
-        collection_type_from_rules=None,
-        structured_like=None,
-        dataset_collector_descriptions=None,
-    ):
+        collection_type: Optional[str],
+        collection_type_source: Optional[str] = None,
+        collection_type_from_rules: Optional[str] = None,
+        structured_like: Optional[str] = None,
+        dataset_collector_descriptions: Optional[List[DatasetCollectionDescription]] = None,
+    ) -> None:
         self.collection_type = collection_type
         self.collection_type_source = collection_type_source
         self.collection_type_from_rules = collection_type_from_rules
         self.structured_like = structured_like
         self.dataset_collector_descriptions = dataset_collector_descriptions or []
         if collection_type and collection_type_source:
             raise ValueError("Cannot set both type and type_source on collection output.")
@@ -345,15 +361,15 @@
             "collection_type_source": self.collection_type_source,
             "collection_type_from_rules": self.collection_type_from_rules,
             "structured_like": self.structured_like,
             "discover_datasets": [d.to_dict() for d in self.dataset_collector_descriptions],
         }
 
     @staticmethod
-    def from_dict(as_dict):
+    def from_dict(as_dict) -> "ToolOutputCollectionStructure":
         structure = ToolOutputCollectionStructure(
             collection_type=as_dict["collection_type"],
             collection_type_source=as_dict["collection_type_source"],
             collection_type_from_rules=as_dict["collection_type_from_rules"],
             structured_like=as_dict["structured_like"],
             dataset_collector_descriptions=dataset_collector_descriptions_from_output_dict(as_dict),
         )
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/stdio.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/parser/stdio.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/util.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/parser/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/xml.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/parser/xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 import json
 import logging
 import math
 import re
 import uuid
-from typing import Optional
+from typing import (
+    List,
+    Optional,
+)
 
 import packaging.version
 
 from galaxy.tool_util.deps import requirements
 from galaxy.tool_util.parser.util import (
     DEFAULT_DELTA,
     DEFAULT_DELTA_FRAC,
 )
 from galaxy.util import (
+    Element,
+    ElementTree,
     string_as_bool,
     xml_text,
     xml_to_string,
 )
 from .interface import (
+    AssertionList,
     InputSource,
     PageSource,
     PagesSource,
     RequiredFiles,
     TestCollectionDef,
     TestCollectionOutputDef,
     ToolSource,
+    ToolSourceTest,
+    ToolSourceTests,
 )
 from .output_actions import ToolOutputActionGroup
 from .output_collection_def import dataset_collector_descriptions_from_elem
 from .output_objects import (
     ToolExpressionOutput,
     ToolOutput,
     ToolOutputCollection,
@@ -45,16 +53,17 @@
 log = logging.getLogger(__name__)
 
 
 class XmlToolSource(ToolSource):
     """Responsible for parsing a tool from classic Galaxy representation."""
 
     language = "xml"
+    root: Element
 
-    def __init__(self, xml_tree, source_path=None, macro_paths=None):
+    def __init__(self, xml_tree: ElementTree, source_path=None, macro_paths=None):
         self.xml_tree = xml_tree
         self.root = xml_tree.getroot()
         self._source_path = source_path
         self._macro_paths = macro_paths or []
         self.legacy_defaults = self.parse_profile() == "16.01"
 
     def to_string(self):
@@ -532,18 +541,18 @@
     def macro_paths(self):
         return self._macro_paths
 
     @property
     def source_path(self):
         return self._source_path
 
-    def parse_tests_to_dict(self):
+    def parse_tests_to_dict(self) -> ToolSourceTests:
         tests_elem = self.root.find("tests")
-        tests = []
-        rval = dict(tests=tests)
+        tests: List[ToolSourceTest] = []
+        rval: ToolSourceTests = dict(tests=tests)
 
         if tests_elem is not None:
             for i, test_elem in enumerate(tests_elem.findall("test")):
                 profile = self.parse_profile()
                 tests.append(_test_elem_to_dict(test_elem, i, profile))
 
         return rval
@@ -557,17 +566,17 @@
         # - Enable buggy interpreter attribute.
         return self.root.get("profile", "16.01")
 
     def parse_license(self):
         return self.root.get("license")
 
     def parse_python_template_version(self):
-        python_template_version = self.root.get("python_template_version", None)
+        python_template_version = self.root.get("python_template_version")
         if python_template_version is not None:
-            python_template_version = packaging.version.parse(python_template_version)
+            python_template_version = packaging.version.Version(python_template_version)
         return python_template_version
 
     def parse_creator(self):
         creators_el = self.root.find("creator")
         if creators_el is None:
             return None
 
@@ -582,16 +591,16 @@
                 continue
             creator_as_dict["class"] = clazz
             creator_as_dict.update(creator_el.attrib)
             creators.append(creator_as_dict)
         return creators
 
 
-def _test_elem_to_dict(test_elem, i, profile=None):
-    rval = dict(
+def _test_elem_to_dict(test_elem, i, profile=None) -> ToolSourceTest:
+    rval: ToolSourceTest = dict(
         outputs=__parse_output_elems(test_elem),
         output_collections=__parse_output_collection_elems(test_elem, profile=profile),
         inputs=__parse_input_elems(test_elem, i),
         expect_num_outputs=test_elem.get("expect_num_outputs"),
         command=__parse_assert_list_from_elem(test_elem.find("assert_command")),
         command_version=__parse_assert_list_from_elem(test_elem.find("assert_command_version")),
         stdout=__parse_assert_list_from_elem(test_elem.find("assert_stdout")),
@@ -732,15 +741,15 @@
 
 
 def __parse_assert_list(output_elem):
     assert_elem = output_elem.find("assert_contents")
     return __parse_assert_list_from_elem(assert_elem)
 
 
-def __parse_assert_list_from_elem(assert_elem):
+def __parse_assert_list_from_elem(assert_elem) -> AssertionList:
     assert_list = None
 
     def convert_elem(elem):
         """Converts and XML element to a dictionary format, used by assertion checking code."""
         tag = elem.tag
         attributes = dict(elem.attrib)
         converted_children = []
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/parser/yaml.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/parser/yaml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 import json
+from typing import (
+    Dict,
+    List,
+)
 
 import packaging.version
 
 from galaxy.tool_util.deps import requirements
 from galaxy.tool_util.parser.util import (
     DEFAULT_DELTA,
     DEFAULT_DELTA_FRAC,
 )
 from .interface import (
+    AssertionDict,
+    AssertionList,
     InputSource,
     PageSource,
     PagesSource,
     ToolSource,
+    ToolSourceTest,
+    ToolSourceTests,
 )
 from .output_collection_def import dataset_collector_descriptions_from_output_dict
 from .output_objects import (
     ToolOutput,
     ToolOutputCollection,
     ToolOutputCollectionStructure,
 )
 from .stdio import error_on_exit_code
 from .util import is_dict
 
 
 class YamlToolSource(ToolSource):
-
     language = "yaml"
 
-    def __init__(self, root_dict, source_path=None):
+    def __init__(self, root_dict: Dict, source_path=None):
         self.root_dict = root_dict
         self._source_path = source_path
-        self._macro_paths = []
+        self._macro_paths: List[str] = []
 
     @property
     def source_path(self):
         return self._source_path
 
     def parse_tool_type(self):
         return self.root_dict.get("tool_type")
@@ -85,15 +92,20 @@
     def parse_version_command(self):
         return self.root_dict.get("runtime_version", {}).get("command", None)
 
     def parse_version_command_interpreter(self):
         return self.root_dict.get("runtime_version", {}).get("interpreter", None)
 
     def parse_requirements_and_containers(self):
-        return requirements.parse_requirements_from_dict(self.root_dict)
+        mixed_requirements = self.root_dict.get("requirements", [])
+        return requirements.parse_requirements_from_lists(
+            software_requirements=[r for r in mixed_requirements if r.get("type") != "resource"],
+            containers=self.root_dict.get("containers", []),
+            resource_requirements=[r for r in mixed_requirements if r.get("type") == "resource"],
+        )
 
     def parse_input_pages(self):
         # All YAML tools have only one page (feature is deprecated)
         page_source = YamlPageSource(self.root_dict.get("inputs", {}))
         return PagesSource([page_source])
 
     def parse_strict_shell(self):
@@ -164,17 +176,17 @@
             inherit_format=inherit_format,
             inherit_metadata=inherit_metadata,
             default_format_source=default_format_source,
             default_metadata_source=default_metadata_source,
         )
         return output_collection
 
-    def parse_tests_to_dict(self):
-        tests = []
-        rval = dict(tests=tests)
+    def parse_tests_to_dict(self) -> ToolSourceTests:
+        tests: List[ToolSourceTest] = []
+        rval: ToolSourceTests = dict(tests=tests)
 
         for i, test_dict in enumerate(self.root_dict.get("tests", [])):
             tests.append(_parse_test(i, test_dict))
 
         return rval
 
     def parse_profile(self):
@@ -183,25 +195,25 @@
     def parse_license(self):
         return self.root_dict.get("license")
 
     def parse_interactivetool(self):
         return self.root_dict.get("entry_points", [])
 
     def parse_python_template_version(self):
-        python_template_version = self.root_dict.get("python_template_version", None)
+        python_template_version = self.root_dict.get("python_template_version")
         if python_template_version is not None:
-            python_template_version = packaging.version.parse(python_template_version)
+            python_template_version = packaging.version.Version(python_template_version)
         return python_template_version
 
     def to_string(self):
         # TODO: Unit test for dumping/restoring
         return json.dumps(self.root_dict)
 
 
-def _parse_test(i, test_dict):
+def _parse_test(i, test_dict) -> ToolSourceTest:
     inputs = test_dict["inputs"]
     if is_dict(inputs):
         new_inputs = []
         for key, value in inputs.items():
             new_inputs.append({"name": key, "value": value, "attributes": {}})
         test_dict["inputs"] = new_inputs
 
@@ -218,31 +230,29 @@
                 attributes = {}
             new_outputs.append({"name": key, "value": file, "attributes": attributes})
     else:
         for output in outputs:
             name = output["name"]
             value = output.get("file", None)
             attributes = output
-            new_outputs.append((name, value, attributes))
+            new_outputs.append({"name": name, "value": value, "attributes": attributes})
 
     for output in new_outputs:
         attributes = output["attributes"]
         defaults = {
             "compare": "diff",
             "lines_diff": 0,
             "delta": DEFAULT_DELTA,
             "delta_frac": DEFAULT_DELTA_FRAC,
             "sort": False,
         }
         # TODO
         attributes["extra_files"] = []
         # TODO
         attributes["metadata"] = {}
-        # TODO
-        assert_list = []
         assert_list = __to_test_assert_list(attributes.get("asserts", []))
         attributes["assert_list"] = assert_list
         _ensure_has(attributes, defaults)
 
     test_dict["outputs"] = new_outputs
     # TODO: implement output collections for YAML tools.
     test_dict["output_collections"] = []
@@ -251,33 +261,33 @@
     test_dict["stderr"] = __to_test_assert_list(test_dict.get("stderr", []))
     test_dict["expect_exit_code"] = test_dict.get("expect_exit_code", None)
     test_dict["expect_failure"] = test_dict.get("expect_failure", False)
     test_dict["expect_test_failure"] = test_dict.get("expect_test_failure", False)
     return test_dict
 
 
-def __to_test_assert_list(assertions):
+def __to_test_assert_list(assertions) -> AssertionList:
     def expand_dict_form(item):
         key, value = item
         new_value = value.copy()
         new_value["that"] = key
         return new_value
 
     if is_dict(assertions):
         assertions = map(expand_dict_form, assertions.items())
 
-    assert_list = []
+    assert_list: List[AssertionDict] = []
     for assertion in assertions:
         # TODO: not handling nested assertions correctly,
         # not sure these are used though.
         children = []
         if "children" in assertion:
             children = assertion["children"]
             del assertion["children"]
-        assert_dict = dict(
+        assert_dict: AssertionDict = dict(
             tag=assertion["that"],
             attributes=assertion,
             children=children,
         )
         assert_list.append(assert_dict)
 
     return assert_list or None  # XML variant is None if no assertions made
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/provided_metadata.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/provided_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,47 +99,47 @@
     def __init__(self, meta_file, job_wrapper=None):
         self.meta_file = meta_file
         self.tool_provided_job_metadata = []
 
         with open(meta_file) as f:
             for line in f:
                 try:
-                    line = stringify_dictionary_keys(json.loads(line))
-                    assert "type" in line
+                    line_as_dict = stringify_dictionary_keys(json.loads(line))
+                    assert "type" in line_as_dict
                 except Exception as e:
                     message = f'Got JSON data from tool, but line is improperly formatted or no "type" key in: [{line}]'
                     raise ValueError(message) from e
                 # Set the dataset id if it's a dataset entry and isn't set.
                 # This isn't insecure.  We loop the job's output datasets in
                 # the finish method, so if a tool writes out metadata for a
                 # dataset id that it doesn't own, it'll just be ignored.
-                dataset_id_not_specified = line["type"] == "dataset" and "dataset_id" not in line
+                dataset_id_not_specified = line_as_dict["type"] == "dataset" and "dataset_id" not in line_as_dict
                 if dataset_id_not_specified:
-                    dataset_basename = line["dataset"]
+                    dataset_basename = line_as_dict["dataset"]
                     if job_wrapper:
                         try:
-                            line["dataset_id"] = job_wrapper.job_io.get_output_file_id(dataset_basename)
+                            line_as_dict["dataset_id"] = job_wrapper.job_io.get_output_file_id(dataset_basename)
                         except KeyError:
                             log.warning(
                                 f"({job_wrapper.job_id}) Tool provided job dataset-specific metadata without specifying a dataset"
                             )
                             continue
                     else:
                         match = re.match(r"(galaxy_)?dataset_(.*)\.dat", dataset_basename)
                         if match is None:
                             raise Exception(
                                 f"processing tool_provided_metadata (e.g. galaxy.json) entry with invalid dataset name [{dataset_basename}]"
                             )
                         dataset_id = match.group(2)
                         if dataset_id.isdigit():
-                            line["dataset_id"] = dataset_id
+                            line_as_dict["dataset_id"] = dataset_id
                         else:
-                            line["dataset_uuid"] = dataset_id
+                            line_as_dict["dataset_uuid"] = dataset_id
 
-                self.tool_provided_job_metadata.append(line)
+                self.tool_provided_job_metadata.append(line_as_dict)
 
     def get_dataset_meta(self, output_name, dataset_id, dataset_uuid):
         for meta in self.tool_provided_job_metadata:
             if meta["type"] == "dataset" and "dataset_id" in meta and int(meta["dataset_id"]) == dataset_id:
                 return meta
             if meta["type"] == "dataset" and "dataset_uuid" in meta and meta["dataset_uuid"] == dataset_uuid:
                 return meta
@@ -163,15 +163,15 @@
 
         return found_failed
 
     def get_unnamed_outputs(self):
         return []
 
     def rewrite(self):
-        with open(self.meta_file, "wt") as job_metadata_fh:
+        with open(self.meta_file, "w") as job_metadata_fh:
             for meta in self.tool_provided_job_metadata:
                 job_metadata_fh.write(f"{json.dumps(meta)}\n")
 
     def get_new_datasets_for_metadata_collection(self):
         for meta in self.tool_provided_job_metadata:
             if meta["type"] == "new_primary_dataset":
                 yield meta
@@ -226,9 +226,9 @@
         return found_failed
 
     def get_unnamed_outputs(self):
         log.debug(f"unnamed outputs [{self.tool_provided_job_metadata}]")
         return self.tool_provided_job_metadata.get("__unnamed_outputs", [])
 
     def rewrite(self):
-        with open(self.meta_file, "wt") as job_metadata_fh:
+        with open(self.meta_file, "w") as job_metadata_fh:
             json.dump(self.tool_provided_job_metadata, job_metadata_fh)
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/base.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+import abc
 import errno
 import logging
 import os
 import string
 import time
 from collections import namedtuple
 from errno import ENOENT
 from typing import (
+    Any,
     Dict,
     List,
+    Optional,
+    Tuple,
+    Union,
 )
 from urllib.parse import urlparse
 
 from markupsafe import escape
 
 from galaxy.exceptions import (
     ConfigurationError,
@@ -104,20 +109,26 @@
     def get_workflow(self, id: str):
         return self.__toolbox._workflows_by_id[id]
 
     def add_tool_to_tool_panel_view(self, tool, tool_panel_component) -> None:
         self.__toolbox.add_tool_to_tool_panel_view(tool, tool_panel_component)
 
 
+DynamicToolConfDict = Dict[str, Any]
+
+
 class AbstractToolBox(Dictifiable, ManagesIntegratedToolPanelMixin):
     """
     Abstract container for managing a ToolPanel - containing tools and
     workflows optionally in labelled sections.
     """
 
+    _dynamic_tool_confs: List[DynamicToolConfDict]
+    _tool_panel_views: Dict[str, ToolPanelView]
+
     def __init__(
         self,
         config_filenames,
         tool_root_dir,
         app,
         view_sources=None,
         default_panel_view="default",
@@ -183,21 +194,21 @@
                     name=name,
                     description=description,
                     model_class=model_class,
                     view_type=view_type,
                     searchable=True,
                 )
 
-        tool_panel_views_list = [
+        tool_panel_views_list: List[ToolPanelView] = [
             DefaultToolPanelView(),
         ]
 
         for edam_view in listify(self.app.config.edam_panel_views):
             mode = EdamPanelMode[edam_view]
-            tool_panel_views_list.append(EdamToolPanelView(self.app.config.edam_toolbox_ontology_path, mode=mode))
+            tool_panel_views_list.append(EdamToolPanelView(self.app.datatypes_registry.edam, mode=mode))
 
         if view_sources is not None:
             for definition in view_sources.get_definitions():
                 tool_panel_views_list.append(StaticToolPanelView(definition))
 
         self._tool_panel_views = {}
         for tool_panel_view in tool_panel_views_list:
@@ -412,15 +423,15 @@
                     panel_dict,
                     tool_path,
                     integrated_panel_dict,
                     load_panel_dict=load_panel_dict,
                     tool_cache_data_dir=tool_cache_data_dir,
                 )
 
-    def get_shed_config_dict_by_filename(self, filename):
+    def get_shed_config_dict_by_filename(self, filename) -> Optional[DynamicToolConfDict]:
         filename = os.path.abspath(filename)
         dynamic_tool_conf_paths = []
         for shed_config_dict in self._dynamic_tool_confs:
             dynamic_tool_conf_path = os.path.abspath(shed_config_dict["config_filename"])
             dynamic_tool_conf_paths.append(dynamic_tool_conf_path)
             if dynamic_tool_conf_path == filename:
                 return shed_config_dict
@@ -649,16 +660,18 @@
                     raise ObjectNotFound(f"Failed to find a tool with uuid [{tool_uuid}]")
                 tool_id = tool_from_uuid.id
             if tool_id is None:
                 raise AssertionError("get_tool called with tool_id as None")
 
         if "/repos/" in tool_id:  # test if tool came from a toolshed
             tool_id_without_tool_shed = tool_id.split("/repos/")[1]
-            available_tool_sheds = [urlparse(_) for _ in self.app.tool_shed_registry.tool_sheds.values()]
-            available_tool_sheds = [url.geturl().replace(f"{url.scheme}://", "", 1) for url in available_tool_sheds]
+            available_tool_sheds_parsed = [urlparse(_) for _ in self.app.tool_shed_registry.tool_sheds.values()]
+            available_tool_sheds = [
+                url.geturl().replace(f"{url.scheme}://", "", 1) for url in available_tool_sheds_parsed
+            ]
             tool_ids = [f"{tool_shed}repos/{tool_id_without_tool_shed}" for tool_shed in available_tool_sheds]
             if tool_id in tool_ids:  # move original tool_id to the top of tool_ids
                 tool_ids.remove(tool_id)
             tool_ids.insert(0, tool_id)
         else:
             tool_ids = [tool_id]
         for tool_id in tool_ids:
@@ -713,32 +726,32 @@
             if tool_id in self._tools_by_id:
                 if get_all_versions:
                     return [self._tools_by_id[tool_id]]
                 else:
                     return self._tools_by_id[tool_id]
         return None
 
-    def has_tool(self, tool_id, tool_version=None, exact=False):
+    def has_tool(self, tool_id: str, tool_version: Optional[str] = None, exact: bool = False):
         return self.get_tool(tool_id, tool_version=tool_version, exact=exact) is not None
 
-    def is_missing_shed_tool(self, tool_id):
+    def is_missing_shed_tool(self, tool_id: str) -> bool:
         """Confirm that the tool ID does reference a shed tool and is not installed."""
         if tool_id is None:
             # This is not a tool ID.
             return False
         if "repos" not in tool_id:
             # This is not a shed tool.
             return False
         # This is a valid tool, and it is from a toolshed. Check if it's
         # missing from the toolbox.
         if tool_id not in self._tools_by_id:
             return True
         return False
 
-    def get_loaded_tools_by_lineage(self, tool_id):
+    def get_loaded_tools_by_lineage(self, tool_id: str) -> list:
         """Get all loaded tools associated by lineage to the tool whose id is tool_id."""
         tool_lineage = self._lineage_map.get(tool_id)
         if tool_lineage:
             lineage_tool_versions = tool_lineage.get_versions()
             available_tool_versions = []
             for lineage_tool_version in lineage_tool_versions:
                 tool = self._tool_from_lineage_version(lineage_tool_version)
@@ -750,23 +763,23 @@
                 tool = self._tools_by_id[tool_id]
                 return [tool]
         return []
 
     def tools(self):
         return self._tools_by_id.copy().items()
 
-    def dynamic_confs(self, include_migrated_tool_conf=False):
+    def dynamic_confs(self, include_migrated_tool_conf=False) -> List[DynamicToolConfDict]:
         confs = []
         for dynamic_tool_conf_dict in self._dynamic_tool_confs:
             dynamic_tool_conf_filename = dynamic_tool_conf_dict["config_filename"]
             if include_migrated_tool_conf or (dynamic_tool_conf_filename != self.app.config.migrated_tools_config):
                 confs.append(dynamic_tool_conf_dict)
         return confs
 
-    def default_shed_tool_conf_dict(self):
+    def default_shed_tool_conf_dict(self) -> DynamicToolConfDict:
         """If set, returns the first shed_tool_conf_dict corresponding to shed_tool_config_file, else the first dynamic conf."""
         dynamic_confs = self.dynamic_confs(include_migrated_tool_conf=False)
         # Pick the first tool config that doesn't set `is_shed_conf="false"` and that is not a migrated_tool_conf
         try:
             shed_config_dict = dynamic_confs[0]
         except IndexError:
             raise ConfigurationError("No shed_tool_conf file active")
@@ -834,14 +847,17 @@
             if not tool:  # tool was not in cache and is not a tool shed tool.
                 tool = self.load_tool(concrete_path, use_cached=False, tool_cache_data_dir=tool_cache_data_dir)
             if string_as_bool(item.get("hidden", False)):
                 tool.hidden = True
             key = f"tool_{str(tool.id)}"
             if can_load_into_panel_dict:
                 if guid and not from_cache:
+                    assert (
+                        tool_shed_repository is not None
+                    )  # tell type system if can_load_into_panel_dict, this can't be none
                     tool.tool_shed = tool_shed_repository.tool_shed
                     tool.repository_name = tool_shed_repository.name
                     tool.repository_owner = tool_shed_repository.owner
                     tool.installed_changeset_revision = tool_shed_repository.installed_changeset_revision
                     tool.guid = guid
                     tool.version = item.elem.find("version").text
                 if item.has_elem:
@@ -1139,19 +1155,20 @@
         # Make sure the tool is actually loaded.
         if tool_id not in self._tools_by_id:
             raise ObjectNotFound(f"No tool found with id '{escape(tool_id)}'.")
         else:
             tool = self._tools_by_id[tool_id]
             return tool.to_archive()
 
-    def reload_tool_by_id(self, tool_id):
+    def reload_tool_by_id(self, tool_id: str) -> Tuple[Union[str, Dict[str, str]], str]:
         """
         Attempt to reload the tool identified by 'tool_id', if successful
         replace the old tool.
         """
+        message: Union[str, Dict[str, str]]
         if tool_id not in self._tools_by_id:
             message = f"No tool with id '{escape(tool_id)}'."
             status = "error"
         else:
             old_tool = self._tools_by_id[tool_id]
             new_tool = self.load_tool(old_tool.config_file, use_cached=False)
             # The tool may have been installed from a tool shed, so set the tool shed attributes.
@@ -1318,23 +1335,27 @@
         """Return True if tool1 is considered "newer" given its own lineage
         description.
         """
         return tool1.version_object > tool2.version_object
 
     def _tool_from_lineage_version(self, lineage_tool_version):
         if lineage_tool_version.id_based:
-            return self._tools_by_id.get(lineage_tool_version.id, None)
+            return self._tools_by_id.get(lineage_tool_version.id)
         else:
-            return self._tool_versions_by_id.get(lineage_tool_version.id, {}).get(lineage_tool_version.version, None)
+            return self._tool_versions_by_id.get(lineage_tool_version.id, {}).get(lineage_tool_version.version)
 
     def _build_filter_method(self, trans):
         context = Bunch(toolbox=self, trans=trans)
         filters = self._filter_factory.build_filters(trans)
         return lambda element, item_type: _filter_for_panel(element, item_type, filters, context)
 
+    @abc.abstractmethod
+    def _looks_like_a_tool(self, path: str) -> bool:
+        ...
+
 
 def _filter_for_panel(item, item_type, filters, context):
     """
     Filters tool panel elements so that only those that are compatible
     with provided filters are kept.
     """
 
@@ -1447,14 +1468,13 @@
         self._init_dependency_manager()
 
     def load_builtin_converters(self):
         id = "builtin_converters"
         section = ToolSection({"name": "Built-in Converters", "id": id})
         self._tool_panel[id] = section
 
-        converters = self.app.datatypes_registry.datatype_converters
-        for source, targets in converters.items():
-            for target, tool in targets.items():
-                tool.name = f"{source}-to-{target}"
-                tool.description = "converter"
-                tool.hidden = False
-                section.elems.append_tool(tool)
+        converters = {
+            tool for target in self.app.datatypes_registry.datatype_converters.values() for tool in target.values()
+        }
+        for tool in converters:
+            tool.hidden = False
+            section.elems.append_tool(tool)
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/filters/__init__.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/filters/examples.py.sample` & `galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/filters/examples.py.sample`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/integrated_panel.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/integrated_panel.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/lineages/factory.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/lineages/factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/lineages/interface.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/lineages/interface.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/panel.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,19 +226,19 @@
 
     def walk_sections(self):
         for key, item in self.items():
             if isinstance(item, ToolSection):
                 yield (key, item)
 
     def closest_section(self, target_section_id: Optional[str], target_section_name: Optional[str]):
-        for (section_id, section) in self.walk_sections():
+        for section_id, section in self.walk_sections():
             if section_id == target_section_id:
                 return section
 
-        for (_, section) in self.walk_sections():
+        for _, section in self.walk_sections():
             if section.name == target_section_name:
                 return section
 
         return None
 
     def apply_filter(self, f):
         to_remove = []
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/parser.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import yaml
 
 from galaxy.util import (
     parse_xml,
     string_as_bool,
 )
+from galaxy.util.path import StrPath
 
 DEFAULT_MONITOR = False
 
 
 class ToolConfSource(metaclass=ABCMeta):
     """Interface represents a container of tool references."""
 
@@ -35,15 +36,15 @@
 
     def parse_monitor(self):
         """Monitor the toolbox configuration source for changes and reload."""
         return DEFAULT_MONITOR
 
 
 class XmlToolConfSource(ToolConfSource):
-    def __init__(self, config_filename):
+    def __init__(self, config_filename: StrPath):
         tree = parse_xml(config_filename)
         self.root = tree.getroot()
 
     def parse_tool_path(self):
         return self.root.get("tool_path")
 
     def parse_tool_cache_data_dir(self):
@@ -58,15 +59,15 @@
         return has_tool_path and is_shed_conf
 
     def parse_monitor(self):
         return string_as_bool(self.root.get("monitor", DEFAULT_MONITOR))
 
 
 class YamlToolConfSource(ToolConfSource):
-    def __init__(self, config_filename):
+    def __init__(self, config_filename: StrPath):
         with open(config_filename) as f:
             as_dict = yaml.safe_load(f)
         self.as_dict = as_dict
 
     def parse_tool_path(self):
         return self.as_dict.get("tool_path")
 
@@ -153,16 +154,16 @@
         if type != "section":
             return ToolConfItem(type, attributes, elem)
         else:
             items = [ensure_tool_conf_item(_) for _ in elem]
             return ToolConfSection(attributes, items, elem=elem)
 
 
-def get_toolbox_parser(config_filename):
-    is_yaml = any(config_filename.endswith(e) for e in [".yml", ".yaml", ".json"])
+def get_toolbox_parser(config_filename: StrPath):
+    is_yaml = any(str(config_filename).endswith(e) for e in [".yml", ".yaml", ".json"])
     if is_yaml:
         return YamlToolConfSource(config_filename)
     else:
         return XmlToolConfSource(config_filename)
 
 
 __all__ = (
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/tags.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/tags.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/views/definitions.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/views/definitions.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/views/edam.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/views/edam.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import logging
-import os
 from enum import Enum
 from typing import (
     Dict,
     List,
-    Optional,
     Tuple,
 )
 
 from galaxy.tool_util.edam_util import (
-    load_edam_tree,
     ROOT_OPERATION,
     ROOT_TOPIC,
 )
 from galaxy.util import ExecutionTimer
 from .interface import (
     ToolBoxRegistry,
     ToolPanelView,
@@ -32,18 +29,15 @@
 class EdamPanelMode(str, Enum):
     merged = "merged"
     topics = "topics"
     operations = "operations"
 
 
 class EdamToolPanelView(ToolPanelView):
-    def __init__(self, edam_ontology_path: Optional[str], mode: EdamPanelMode = EdamPanelMode.merged):
-        edam = load_edam_tree(
-            None if not edam_ontology_path or not os.path.exists(edam_ontology_path) else edam_ontology_path
-        )
+    def __init__(self, edam: Dict[str, Dict], mode: EdamPanelMode = EdamPanelMode.merged):
         self.edam = edam
         self.mode = mode
         self.include_topics = mode in [EdamPanelMode.merged, EdamPanelMode.topics]
         self.include_operations = mode in [EdamPanelMode.merged, EdamPanelMode.operations]
 
     def apply_view(self, base_tool_panel: ToolPanelElements, toolbox_registry: ToolBoxRegistry) -> ToolPanelElements:
         execution_timer = ExecutionTimer()
@@ -125,15 +119,15 @@
             }
             new_panel[f"label_{term}"] = ToolSectionLabel(label_dict)
 
             for tuple_ in topics[term].values():
                 populate_section(*tuple_)
 
         section = new_panel.get_or_create_section("uncategorized", "Uncategorized")
-        for (tool_id, key, val, val_name) in uncategorized:
+        for tool_id, key, val, val_name in uncategorized:
             toolbox_registry.add_tool_to_tool_panel_view(val, section)
             new_panel.record_section_for_tool_id(tool_id, key, val_name)
         log.debug("Loading EDAM tool panel finished %s", execution_timer)
         return new_panel
 
     def _get_edam_sec(self, tool):
         edam = []
@@ -158,23 +152,23 @@
                 yield term
 
     def to_model(self) -> ToolPanelViewModel:
         mode = self.mode
         if mode == EdamPanelMode.merged:
             model_id = "ontology:edam_merged"
             name = "EDAM Operations and Topics"
-            description = "Tools are grouped using both annotated operation and topic information (if availabled)."
+            description = "Tools are grouped using both annotated operation and topic information (if available)."
         elif mode == EdamPanelMode.operations:
             model_id = "ontology:edam_operations"
             name = "EDAM Operations"
-            description = "Tools are grouped using annotated EDAM operation information (if availabled)."
+            description = "Tools are grouped using annotated EDAM operation information (if available)."
         elif mode == EdamPanelMode.topics:
             model_id = "ontology:edam_topics"
             name = "EDAM Topics"
-            description = "Tools are grouped using annotated EDAM topic information (if availabled)."
+            description = "Tools are grouped using annotated EDAM topic information (if available)."
         else:
             raise AssertionError(f"Invalid EDAM mode encountered {mode}")
         model_class = self.__class__.__name__
         view_type = ToolPanelViewModelType.ontology
         return ToolPanelViewModel(
             id=model_id,
             name=name,
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/views/interface.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/views/interface.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/views/sources.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/views/sources.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/views/static.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/views/static.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             return new_panel
 
         root_defintion = self._definition
         root_items = root_defintion.items_expanded
         if root_items is None:
             root_items = []
             # No items found, use base tool panel and apply filters to that...
-            for (_, panel_type, panel_value) in base_tool_panel.panel_items_iter():
+            for _, panel_type, panel_value in base_tool_panel.panel_items_iter():
                 item: Optional[ExpandedRootContent] = None
                 if panel_type == panel_item_types.TOOL:
                     item = Tool(
                         id=panel_value.id,
                     )
                 elif panel_type == panel_item_types.SECTION:
                     item = SectionAlias(
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/toolbox/watcher.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/toolbox/watcher.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/__init__.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/verify/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 import json
 import logging
 import os
 import os.path
 import re
 import shutil
 import tempfile
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Optional,
+)
 
 try:
     import pysam
 except ImportError:
     pysam = None  # type: ignore[assignment]
 
 from galaxy.tool_util.parser.util import (
@@ -27,34 +33,37 @@
 
 log = logging.getLogger(__name__)
 
 DEFAULT_TEST_DATA_RESOLVER = TestDataResolver()
 
 
 def verify(
-    item_label,
-    output_content,
-    attributes,
-    filename=None,
-    get_filecontent=None,
-    get_filename=None,
-    keep_outputs_dir=None,
-    verify_extra_files=None,
+    item_label: str,
+    output_content: bytes,
+    attributes: Dict[str, Any],
+    filename: Optional[str] = None,
+    get_filecontent: Optional[Callable[[str], bytes]] = None,
+    get_filename: Optional[Callable[[str], str]] = None,
+    keep_outputs_dir: Optional[str] = None,
+    verify_extra_files: Optional[Callable] = None,
     mode="file",
 ):
     """Verify the content of a test output using test definitions described by attributes.
 
     Throw an informative assertion error if any of these tests fail.
     """
     if get_filename is None:
+        get_filecontent_: Callable[[str], bytes]
         if get_filecontent is None:
-            get_filecontent = DEFAULT_TEST_DATA_RESOLVER.get_filecontent
+            get_filecontent_ = DEFAULT_TEST_DATA_RESOLVER.get_filecontent
+        else:
+            get_filecontent_ = get_filecontent
 
-        def get_filename(filename):
-            file_content = get_filecontent(filename)
+        def get_filename(filename: str) -> str:
+            file_content = get_filecontent_(filename)
             local_name = make_temp_fname(fname=filename)
             with open(local_name, "wb") as f:
                 f.write(file_content)
             return local_name
 
     # Check assertions...
     assertions = attributes.get("assert_list", None)
@@ -132,15 +141,17 @@
                 log.debug("## GALAXY_TEST_SAVE=%s. saved %s", keep_outputs_dir, ofn)
 
         if mode == "directory":
             # if verifying a file inside a extra_files_path directory
             # filename already point to a file that exists on disk
             local_name = filename
         else:
-            local_name = get_filename(filename)
+            filename_ = get_filename(filename)
+            assert filename_, f"Failed to find output target for test {filename_}"
+            local_name = filename_
 
         compare = attributes.get("compare", "diff")
         try:
             if attributes.get("ftype", None) in [
                 "bam",
                 "qname_sorted.bam",
                 "qname_input_sorted.bam",
@@ -355,14 +366,15 @@
             local_file = fh.readlines()
     assert len(local_file) == len(history_data), (
         "Data File and Regular Expression File contain a different number of lines (%d != %d)\nHistory Data (first 40 lines):\n%s"
         % (len(local_file), len(history_data), join_char.join(history_data[:40]))
     )
     if attributes.get("sort", False):
         history_data.sort()
+        local_file.sort()
     lines_diff = int(attributes.get("lines_diff", 0))
     line_diff_count = 0
     diffs = []
     for regex_line, data_line in zip(local_file, history_data):
         regex_line = regex_line.rstrip(to_strip)
         data_line = data_line.rstrip(to_strip)
         if not re.match(regex_line, data_line):
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/__init__.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,22 +26,22 @@
         log.exception("Failed to load assertion module: %s", assertion_module_name)
         continue
     for member, value in getmembers(assertion_module):
         if member.startswith("assert_"):
             assertion_functions[member] = value
 
 
-def verify_assertions(data, assertion_description_list):
+def verify_assertions(data: bytes, assertion_description_list):
     """This function takes a list of assertions and a string to check
     these assertions against."""
     for assertion_description in assertion_description_list:
         verify_assertion(data, assertion_description)
 
 
-def verify_assertion(data, assertion_description):
+def verify_assertion(data: bytes, assertion_description):
     tag = assertion_description["tag"]
     assert_function_name = "assert_" + tag
     assert_function = assertion_functions.get(assert_function_name)
 
     if assert_function is None:
         errmsg = f"Unable to find test function associated with XML tag {tag}. Check your tool file syntax."
         raise AssertionError(errmsg)
@@ -56,15 +56,15 @@
     # tool XML attributes. output is passed in as the contents of the
     # output file. verify_assertions_function is passed in as the
     # verify_assertions function defined above, this allows
     # recursively checking assertions on subsections of
     # output. children is the parsed version of the child elements of
     # the XML element describing this assertion. See
     # assert_element_text in test/base/asserts/xml.py as an example of
-    # how to use verify_assertions_function and children in conjuction
+    # how to use verify_assertions_function and children in conjunction
     # to apply assertion checking to a subset of the input. The parsed
     # version of an elements child elements do not need to just define
     # assertions, developers of assertion functions can also use the
     # child elements in novel ways to define inputs the assertion
     # checking function (for instance consider the following fictional
     # assertion function for checking column titles of tabular output
     # - <has_column_titles><with_name name="sequence"><with_name
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/archive.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/archive.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,76 @@
 import io
 import re
 import tarfile
 import tempfile
 import zipfile
-from typing import Optional
+from typing import (
+    Optional,
+    Union,
+)
 
 from galaxy.util import asbool
 from ._util import _assert_presence_number
 
 
-def _extract_from_tar(bytes, fn):
-    with io.BytesIO(bytes) as temp:
+def _extract_from_tar(output_bytes, fn):
+    with io.BytesIO(output_bytes) as temp:
         with tarfile.open(fileobj=temp, mode="r") as tar_temp:
             ti = tar_temp.getmember(fn)
             # zip treats directories like empty files.
             # so make this consistent for tar
             if ti.isdir():
                 return ""
-            with tar_temp.extractfile(fn) as member_fh:
+            tar_file = tar_temp.extractfile(fn)
+            assert tar_file is not None
+            with tar_file as member_fh:
                 return member_fh.read()
 
 
-def _list_from_tar(bytes, path):
+def _list_from_tar(output_bytes, path):
     lst = list()
-    with io.BytesIO(bytes) as temp:
+    with io.BytesIO(output_bytes) as temp:
         with tarfile.open(fileobj=temp, mode="r") as tar_temp:
             for fn in tar_temp.getnames():
                 if not re.match(path, fn):
                     continue
                 lst.append(fn)
     return sorted(lst)
 
 
-def _extract_from_zip(bytes, fn):
-    with io.BytesIO(bytes) as temp:
+def _extract_from_zip(output_bytes, fn):
+    with io.BytesIO(output_bytes) as temp:
         with zipfile.ZipFile(temp, mode="r") as zip_temp:
             with zip_temp.open(fn) as member_fh:
                 return member_fh.read()
 
 
-def _list_from_zip(bytes, path):
+def _list_from_zip(output_bytes, path):
     lst = list()
-    with io.BytesIO(bytes) as temp:
+    with io.BytesIO(output_bytes) as temp:
         with zipfile.ZipFile(temp, mode="r") as zip_temp:
             for fn in zip_temp.namelist():
                 if not re.match(path, fn):
                     continue
                 lst.append(fn)
     return sorted(lst)
 
 
 def assert_has_archive_member(
-    output_bytes,
-    path,
+    output_bytes: bytes,
+    path: str,
     verify_assertions_function,
     children,
-    all="false",
-    n: Optional[int] = None,
-    delta: int = 0,
-    min: Optional[int] = None,
-    max: Optional[int] = None,
-    negate: bool = False,
-):
+    all: Union[bool, str] = False,
+    n: Optional[Union[int, str]] = None,
+    delta: Union[int, str] = 0,
+    min: Optional[Union[int, str]] = None,
+    max: Optional[Union[int, str]] = None,
+    negate: Union[bool, str] = False,
+) -> None:
     """Recursively checks the specified children assertions against the text of
     the first element matching the specified path found within the archive.
     Currently supported formats: .zip, .tar, .tar.gz."""
     all = asbool(all)
     extract_foo = None
     # from python 3.9 is_tarfile supports file like objects then we do not need
     # the tempfile detour but can use io.BytesIO(output_bytes)
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/hdf5.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/hdf5.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,31 +9,30 @@
 
 
 def _assert_h5py():
     if h5py is None:
         raise Exception(IMPORT_MISSING_MESSAGE)
 
 
-def assert_has_h5_attribute(output_bytes, key, value):
+def assert_has_h5_attribute(output_bytes: bytes, key: str, value: str) -> None:
     """Asserts the specified HDF5 output has a given key-value pair as HDF5
     attribute"""
     _assert_h5py()
     output_temp = io.BytesIO(output_bytes)
     local_attrs = h5py.File(output_temp, "r").attrs
     assert (
         key in local_attrs and str(local_attrs[key]) == value
     ), f"Not a HDF5 file or H5 attributes do not match:\n\t{list(local_attrs.items())}\n\n\t({key} : {value})"
 
 
 # TODO the function actually queries groups. so the function and argument name are misleading
-def assert_has_h5_keys(output_bytes, keys):
+def assert_has_h5_keys(output_bytes: bytes, keys: str) -> None:
     """Asserts the specified HDF5 output has the given keys."""
     _assert_h5py()
-    keys = [k.strip() for k in keys.strip().split(",")]
-    h5_keys = sorted(keys)
+    h5_keys = sorted([k.strip() for k in keys.strip().split(",")])
     output_temp = io.BytesIO(output_bytes)
     local_keys = []
 
     def append_keys(key):
         local_keys.append(key)
         return None
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/size.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/size.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from typing import Optional
+from typing import (
+    Optional,
+    Union,
+)
 
 from ._util import _assert_number
 
 
 def assert_has_size(
-    output_bytes,
-    value: Optional[int] = None,
-    delta: int = 0,
-    min: Optional[int] = None,
-    max: Optional[int] = None,
-    negate: bool = False,
-):
+    output_bytes: bytes,
+    value: Optional[Union[int, str]] = None,
+    delta: Union[int, str] = 0,
+    min: Optional[Union[int, str]] = None,
+    max: Optional[Union[int, str]] = None,
+    negate: Union[bool, str] = False,
+) -> None:
     """
     Asserts the specified output has a size of the specified value,
     allowing for absolute (delta) and relative (delta_frac) difference.
     """
     output_size = len(output_bytes)
     _assert_number(
         output_size,
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/tabular.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/tabular.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 import re
-from typing import Optional
+from typing import (
+    Optional,
+    Union,
+)
 
 from ._util import _assert_number
 
 
-def get_first_line(output, comment):
+def get_first_line(output: str, comment: str) -> str:
     """
     get the first non-comment and non-empty line
     """
     if comment != "":
         match = re.search(f"^([^{comment}].*)$", output, flags=re.MULTILINE)
     else:
         match = re.search("^(.+)$", output, flags=re.MULTILINE)
     if match is None:
         return ""
     else:
         return match.group(1)
 
 
 def assert_has_n_columns(
-    output,
-    n: Optional[int] = None,
-    delta: int = 0,
-    min: Optional[int] = None,
-    max: Optional[int] = None,
-    sep="\t",
-    comment="",
-    negate: bool = False,
-):
+    output: str,
+    n: Optional[Union[int, str]] = None,
+    delta: Union[int, str] = 0,
+    min: Optional[Union[int, str]] = None,
+    max: Optional[Union[int, str]] = None,
+    sep: str = "\t",
+    comment: str = "",
+    negate: Union[bool, str] = False,
+) -> None:
     """Asserts the tabular output contains n columns. The optional
     sep argument specifies the column seperator used to determine the
     number of columns. The optional comment argument specifies
     comment characters"""
     first_line = get_first_line(output, comment)
     n_columns = len(first_line.split(sep))
     _assert_number(
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/text.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/text.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import re
-from typing import Optional
+from typing import (
+    Optional,
+    Union,
+)
 
 from ._util import (
     _assert_number,
     _assert_presence_number,
 )
 
 
 def assert_has_text(
-    output,
-    text,
-    n: Optional[int] = None,
-    delta: int = 0,
-    min: Optional[int] = None,
-    max: Optional[int] = None,
-    negate: bool = False,
-):
+    output: str,
+    text: str,
+    n: Optional[Union[int, str]] = None,
+    delta: Union[int, str] = 0,
+    min: Optional[Union[int, str]] = None,
+    max: Optional[Union[int, str]] = None,
+    negate: Union[bool, str] = False,
+) -> None:
     """Asserts specified output contains the substring specified by
     the argument text. The exact number of occurrences can be
     optionally specified by the argument n"""
     assert output is not None, "Checking has_text assertion on empty output (None)"
     _assert_presence_number(
         output,
         text,
@@ -32,58 +35,58 @@
         lambda o, t: len(re.findall(re.escape(t), o)),
         "{expected} text '{text}' in output ('{output}')",
         "{expected} {n}+-{delta} occurences of '{text}' in output ('{output}')",
         "{expected} that the number of occurences of '{text}' in output is in [{min}:{max}] ('{output}')",
     )
 
 
-def assert_not_has_text(output, text):
+def assert_not_has_text(output: str, text: str) -> None:
     """Asserts specified output does not contain the substring
     specified by the argument text"""
     assert output is not None, "Checking not_has_text assertion on empty output (None)"
     assert output.find(text) < 0, f"Output file contains unexpected text '{text}'"
 
 
 def assert_has_line(
-    output,
-    line,
-    n: Optional[int] = None,
-    delta: int = 0,
-    min: Optional[int] = None,
-    max: Optional[int] = None,
-    negate: bool = False,
-):
+    output: str,
+    line: str,
+    n: Optional[Union[int, str]] = None,
+    delta: Union[int, str] = 0,
+    min: Optional[Union[int, str]] = None,
+    max: Optional[Union[int, str]] = None,
+    negate: Union[bool, str] = False,
+) -> None:
     """Asserts the specified output contains the line specified by the
     argument line. The exact number of occurrences can be optionally
     specified by the argument n"""
     assert output is not None, "Checking has_line assertion on empty output (None)"
     _assert_presence_number(
         output,
         line,
         n,
         delta,
         min,
         max,
         negate,
-        lambda o, l: re.search(f"^{re.escape(l)}$", o, flags=re.MULTILINE) is not None,
-        lambda o, l: len(re.findall(f"^{re.escape(l)}$", o, flags=re.MULTILINE)),
+        lambda o, t: re.search(f"^{re.escape(t)}$", o, flags=re.MULTILINE) is not None,
+        lambda o, t: len(re.findall(f"^{re.escape(t)}$", o, flags=re.MULTILINE)),
         "{expected} line '{text}' in output ('{output}')",
         "{expected} {n}+-{delta} lines '{text}' in output ('{output}')",
         "{expected} that the number of lines '{text}' in output is in [{min}:{max}] ('{output}')",
     )
 
 
 def assert_has_n_lines(
-    output,
-    n: Optional[int] = None,
-    delta: int = 0,
-    min: Optional[int] = None,
-    max: Optional[int] = None,
-    negate: bool = False,
-):
+    output: str,
+    n: Optional[Union[int, str]] = None,
+    delta: Union[int, str] = 0,
+    min: Optional[Union[int, str]] = None,
+    max: Optional[Union[int, str]] = None,
+    negate: Union[bool, str] = False,
+) -> None:
     """Asserts the specified output contains ``n`` lines allowing
     for a difference in the number of lines (delta)
     or relative differebce in the number of lines"""
     assert output is not None, "Checking has_n_lines assertion on empty output (None)"
     count = len(output.splitlines())
     _assert_number(
         count,
@@ -94,22 +97,22 @@
         negate,
         "{expected} {n}+-{delta} lines in the output",
         "{expected} the number of line to be in [{min}:{max}]",
     )
 
 
 def assert_has_text_matching(
-    output,
-    expression,
-    n: Optional[int] = None,
-    delta: int = 0,
-    min: Optional[int] = None,
-    max: Optional[int] = None,
-    negate: bool = False,
-):
+    output: str,
+    expression: str,
+    n: Optional[Union[int, str]] = None,
+    delta: Union[int, str] = 0,
+    min: Optional[Union[int, str]] = None,
+    max: Optional[Union[int, str]] = None,
+    negate: Union[bool, str] = False,
+) -> None:
     """Asserts the specified output contains text matching the
     regular expression specified by the argument expression.
     If n is given the assertion checks for exacly n (nonoverlapping)
     occurences.
     """
     _assert_presence_number(
         output,
@@ -124,22 +127,22 @@
         "{expected} text matching expression '{text}' in output ('{output}')",
         "{expected} {n}+-{delta} (non-overlapping) matches for '{text}' in output ('{output}')",
         "{expected} that the number of (non-overlapping) matches for '{text}' in output is in [{min}:{max}] ('{output}')",
     )
 
 
 def assert_has_line_matching(
-    output,
-    expression,
-    n: Optional[int] = None,
-    delta: int = 0,
-    min: Optional[int] = None,
-    max: Optional[int] = None,
-    negate: bool = False,
-):
+    output: str,
+    expression: str,
+    n: Optional[Union[int, str]] = None,
+    delta: Union[int, str] = 0,
+    min: Optional[Union[int, str]] = None,
+    max: Optional[Union[int, str]] = None,
+    negate: Union[bool, str] = False,
+) -> None:
     """Asserts the specified output contains a line matching the
     regular expression specified by the argument expression. If n is given
     the assertion checks for exactly n occurences."""
     _assert_presence_number(
         output,
         expression,
         n,
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/asserts/xml.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/verify/asserts/xml.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,96 +1,103 @@
 import re
-from typing import Optional
+from typing import (
+    Optional,
+    Union,
+)
 
 from lxml.etree import XMLSyntaxError
 
 from galaxy.tool_util.verify import asserts
 from galaxy.util import (
     asbool,
     parse_xml_string,
     unicodify,
 )
 
 
-def assert_is_valid_xml(output):
+def assert_is_valid_xml(output: str) -> None:
     """Simple assertion that just verifies the specified output
     is valid XML."""
     try:
         parse_xml_string(output)
     except XMLSyntaxError as e:
         raise AssertionError(f"Expected valid XML, but could not parse output. {unicodify(e)}")
 
 
-def assert_has_element_with_path(output, path, negate: bool = False):
+def assert_has_element_with_path(output: str, path: str, negate: Union[bool, str] = False) -> None:
     """Asserts the specified output has at least one XML element with a
     path matching the specified path argument. Valid paths are the
     simplified subsets of XPath implemented by lxml.etree;
     https://lxml.de/xpathxslt.html for more information."""
     assert_xml_element(output, path, negate=negate)
 
 
 def assert_has_n_elements_with_path(
-    output,
-    path,
-    n: Optional[int] = None,
-    delta: int = 0,
-    min: Optional[int] = None,
-    max: Optional[int] = None,
-    negate: bool = False,
-):
+    output: str,
+    path: str,
+    n: Optional[Union[int, str]] = None,
+    delta: Union[int, str] = 0,
+    min: Optional[Union[int, str]] = None,
+    max: Optional[Union[int, str]] = None,
+    negate: Union[bool, str] = False,
+) -> None:
     """Asserts the specified output has exactly n elements matching the
     path specified."""
     assert_xml_element(output, path, n=n, delta=delta, min=min, max=max, negate=negate)
 
 
-def assert_element_text_matches(output, path, expression, negate: bool = False):
+def assert_element_text_matches(output: str, path: str, expression: str, negate: Union[bool, str] = False) -> None:
     """Asserts the text of the first element matching the specified
     path matches the specified regular expression."""
     sub = {"tag": "has_text_matching", "attributes": {"expression": expression, "negate": negate}}
     assert_xml_element(output, path, asserts.verify_assertions, [sub])
 
 
-def assert_element_text_is(output, path, text, negate: bool = False):
+def assert_element_text_is(output: str, path: str, text: str, negate: Union[bool, str] = False) -> None:
     """Asserts the text of the first element matching the specified
     path matches exactly the specified text."""
     assert_element_text_matches(output, path, re.escape(text) + "$", negate=negate)
 
 
-def assert_attribute_matches(output, path, attribute, expression, negate: bool = False):
+def assert_attribute_matches(
+    output: str, path: str, attribute, expression: str, negate: Union[bool, str] = False
+) -> None:
     """Asserts the specified attribute of the first element matching
     the specified path matches the specified regular expression."""
     sub = {"tag": "has_text_matching", "attributes": {"expression": expression, "negate": negate}}
     assert_xml_element(output, path, asserts.verify_assertions, [sub], attribute=attribute)
 
 
-def assert_attribute_is(output, path, attribute, text, negate: bool = False):
+def assert_attribute_is(output: str, path: str, attribute: str, text, negate: Union[bool, str] = False) -> None:
     """Asserts the specified attribute of the first element matching
     the specified path matches exactly the specified text."""
     assert_attribute_matches(output, path, attribute, re.escape(text) + "$", negate=negate)
 
 
-def assert_element_text(output, path, verify_assertions_function, children, negate: bool = False):
+def assert_element_text(
+    output: str, path: str, verify_assertions_function, children, negate: Union[bool, str] = False
+) -> None:
     """Recursively checks the specified assertions against the text of
     the first element matching the specified path."""
     assert_xml_element(output, path, verify_assertions_function, children, negate=negate)
 
 
 def assert_xml_element(
-    output,
-    path,
+    output: str,
+    path: str,
     verify_assertions_function=None,
     children=None,
-    attribute=None,
-    all=False,
-    n: Optional[int] = None,
-    delta: int = 0,
-    min: Optional[int] = None,
-    max: Optional[int] = None,
-    negate: bool = False,
-):
+    attribute: Optional[str] = None,
+    all: Union[bool, str] = False,
+    n: Optional[Union[int, str]] = None,
+    delta: Union[int, str] = 0,
+    min: Optional[Union[int, str]] = None,
+    max: Optional[Union[int, str]] = None,
+    negate: Union[bool, str] = False,
+) -> None:
     """
     Check if path occurs in the xml. If n and delta or min and max are given
     also the number of occurences is checked.
     If there are any sub assertions then check them against
     - the element's text if attribute is None
     - the content of the attribute
     If all is True then the sub assertions are checked for all occurences.
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/interactor.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/verify/interactor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import io
 import json
 import os
 import re
 import shutil
 import sys
 import tarfile
@@ -9,33 +10,41 @@
 import time
 import urllib.parse
 import zipfile
 from json import dumps
 from logging import getLogger
 from typing import (
     Any,
+    Callable,
+    cast,
     Dict,
+    Generator,
+    List,
+    NamedTuple,
     Optional,
+    Union,
 )
 
 import requests
-from packaging.version import parse as parse_version
-from packaging.version import Version
+from packaging.version import (
+    parse as parse_version,
+    Version,
+)
+from requests import Response
 from requests.cookies import RequestsCookieJar
-
-try:
-    from nose.tools import nottest
-except ImportError:
-
-    def nottest(x):
-        return x
-
+from typing_extensions import (
+    Literal,
+    NotRequired,
+    Protocol,
+    TypedDict,
+)
 
 from galaxy import util
 from galaxy.tool_util.parser.interface import (
+    AssertionList,
     TestCollectionDef,
     TestCollectionOutputDef,
 )
 from galaxy.util.bunch import Bunch
 from . import verify
 from .asserts import verify_assertions
 from .wait import wait_on
@@ -45,14 +54,16 @@
 # Off by default because it can pound the database pretty heavily
 # and result in sqlite errors on larger tests or larger numbers of
 # tests.
 VERBOSE_ERRORS = util.asbool(os.environ.get("GALAXY_TEST_VERBOSE_ERRORS", False))
 UPLOAD_ASYNC = util.asbool(os.environ.get("GALAXY_TEST_UPLOAD_ASYNC", True))
 ERROR_MESSAGE_DATASET_SEP = "--------------------------------------"
 DEFAULT_TOOL_TEST_WAIT = int(os.environ.get("GALAXY_TEST_DEFAULT_WAIT", 86400))
+CLEANUP_TEST_HISTORIES = "GALAXY_TEST_NO_CLEANUP" not in os.environ
+DEFAULT_TARGET_HISTORY = os.environ.get("GALAXY_TEST_HISTORY_ID", None)
 
 DEFAULT_FTYPE = "auto"
 # This following default dbkey was traditionally hg17 before Galaxy 18.05,
 # restore this behavior by setting GALAXY_TEST_DEFAULT_DBKEY to hg17.
 DEFAULT_DBKEY = os.environ.get("GALAXY_TEST_DEFAULT_DBKEY", "?")
 
 
@@ -69,17 +80,57 @@
     def __getitem__(self, item):
         if isinstance(item, int):
             return self[list(self.keys())[item]]
         else:
             return super().__getitem__(item)
 
 
+JobDataT = Dict[str, Any]
+JobDataCallbackT = Callable[[JobDataT], None]
+
+
+class ValidToolTestDict(TypedDict):
+    inputs: Any
+    outputs: Any
+    output_collections: List[Dict[str, Any]]
+    stdout: NotRequired[AssertionList]
+    stderr: NotRequired[AssertionList]
+    expect_exit_code: NotRequired[int]
+    expect_failure: NotRequired[bool]
+    expect_test_failure: NotRequired[bool]
+    maxseconds: NotRequired[int]
+    num_outputs: NotRequired[int]
+    command_line: NotRequired[AssertionList]
+    command_version: NotRequired[AssertionList]
+    required_files: NotRequired[List[Any]]
+    required_data_tables: NotRequired[List[Any]]
+    required_loc_files: NotRequired[List[str]]
+    error: Literal[False]
+    tool_id: str
+    tool_version: str
+    test_index: int
+
+
+class InvalidToolTestDict(TypedDict):
+    error: Literal[True]
+    tool_id: str
+    tool_version: str
+    test_index: int
+    inputs: Any
+    exception: str
+    maxseconds: Optional[int]
+
+
+ToolTestDict = Union[ValidToolTestDict, InvalidToolTestDict]
+ToolTestDictsT = List[ToolTestDict]
+
+
 def stage_data_in_history(
-    galaxy_interactor,
-    tool_id,
+    galaxy_interactor: "GalaxyInteractorApi",
+    tool_id: str,
     all_test_data,
     history=None,
     force_path_paste=False,
     maxseconds=DEFAULT_TOOL_TEST_WAIT,
     tool_version=None,
 ):
     # Upload any needed files
@@ -110,25 +161,37 @@
                 force_path_paste=force_path_paste,
                 maxseconds=maxseconds,
                 tool_version=tool_version,
             )
             upload_wait()
 
 
+class RunToolResponse(NamedTuple):
+    inputs: Dict[str, Any]
+    outputs: OutputsDict
+    output_collections: Dict[str, Any]
+    jobs: List[Dict[str, Any]]
+
+
 class GalaxyInteractorApi:
+    # api_key and cookies can also be manually set by UsesApiTestCaseMixin._different_user()
+    api_key: Optional[str]
+    cookies: Optional[RequestsCookieJar]
+    keep_outputs_dir: Optional[str]
+
     def __init__(self, **kwds):
         self.api_url = f"{kwds['galaxy_url'].rstrip('/')}/api"
         self.cookies = None
         self.master_api_key = kwds["master_api_key"]
         self.api_key = self.__get_user_key(
             kwds.get("api_key"), kwds.get("master_api_key"), test_user=kwds.get("test_user")
         )
         if kwds.get("user_api_key_is_admin_key", False):
             self.master_api_key = self.api_key
-        self.keep_outputs_dir = kwds["keep_outputs_dir"]
+        self.keep_outputs_dir = kwds.get("keep_outputs_dir", None)
         self.download_attempts = kwds.get("download_attempts", 1)
         self.download_sleep = kwds.get("download_sleep", 1)
         # Local test data directories.
         self.test_data_directories = kwds.get("test_data") or []
 
         self._target_galaxy_version = None
 
@@ -140,33 +203,30 @@
             self._target_galaxy_version = parse_version(self._get("version").json()["version_major"])
         return self._target_galaxy_version
 
     @property
     def supports_test_data_download(self):
         return self.target_galaxy_version >= Version("19.01")
 
-    def __get_user_key(self, user_key, admin_key, test_user=None):
+    def __get_user_key(self, user_key: Optional[str], admin_key: Optional[str], test_user: Optional[str] = None) -> str:
         if not test_user:
             test_user = "test@bx.psu.edu"
         if user_key:
             return user_key
-        test_user = self.ensure_user_with_email(test_user)
-        return self._post(f"users/{test_user['id']}/api_key", key=admin_key).json()
-
-    # def get_tools(self):
-    #    response = self._get("tools?in_panel=false")
-    #    assert response.status_code == 200, "Non 200 response from tool index API. [%s]" % response.content
-    #    return response.json()
+        test_user_response = self.ensure_user_with_email(test_user)
+        if not admin_key:
+            raise Exception("Must specify either a user key or admin key to interact with the Galaxy API")
+        return self._post(f"users/{test_user_response['id']}/api_key", key=admin_key).json()
 
     def get_tests_summary(self):
         response = self._get("tools/tests_summary")
         assert response.status_code == 200, f"Non 200 response from tool tests available API. [{response.content}]"
         return response.json()
 
-    def get_tool_tests(self, tool_id, tool_version=None):
+    def get_tool_tests(self, tool_id: str, tool_version: Optional[str] = None) -> ToolTestDictsT:
         url = f"tools/{tool_id}/test_data"
         params = {"tool_version": tool_version} if tool_version else None
         response = self._get(url, data=params)
         assert response.status_code == 200, f"Non 200 response from tool test API. [{response.content}]"
         return response.json()
 
     def verify_output_collection(
@@ -301,29 +361,30 @@
 
             for key, value in metadata.items():
                 try:
                     dataset_value = dataset.get(key, None)
 
                     def compare(val, expected):
                         if str(val) != str(expected):
-                            msg = f"Dataset metadata verification for [{key}] failed, expected [{value}] but found [{dataset_value}]. Dataset API value was [{dataset}]."
-                            raise Exception(msg)
+                            raise Exception(
+                                f"Dataset metadata verification for [{key}] failed, expected [{value}] but found [{dataset_value}]. Dataset API value was [{dataset}]."  # noqa: B023
+                            )
 
                     if isinstance(dataset_value, list):
                         value = str(value).split(",")
                         if len(value) != len(dataset_value):
-                            msg = f"Dataset metadata verification for [{key}] failed, expected [{value}] but found [{dataset_value}], lists differ in length. Dataset API value was [{dataset}]."
-                            raise Exception(msg)
+                            raise Exception(
+                                f"Dataset metadata verification for [{key}] failed, expected [{value}] but found [{dataset_value}], lists differ in length. Dataset API value was [{dataset}]."
+                            )
                         for val, expected in zip(dataset_value, value):
                             compare(val, expected)
                     else:
                         compare(dataset_value, value)
                 except KeyError:
-                    msg = f"Failed to verify dataset metadata, metadata key [{key}] was not found."
-                    raise Exception(msg)
+                    raise Exception(f"Failed to verify dataset metadata, metadata key [{key}] was not found.")
 
     def wait_for_job(self, job_id, history_id=None, maxseconds=DEFAULT_TOOL_TEST_WAIT):
         self.wait_for(lambda: self.__job_ready(job_id, history_id), maxseconds=maxseconds)
 
     def wait_for(self, func, what="tool test run", **kwd):
         walltime_exceeded = int(kwd.get("maxseconds", DEFAULT_TOOL_TEST_WAIT))
         wait_on(func, what, walltime_exceeded)
@@ -336,42 +397,60 @@
         return self._get(f"jobs/{job_id}")
 
     def __get_job_stdio(self, job_id):
         return self._get(f"jobs/{job_id}?full=true")
 
     def get_history(self, history_name="test_history"):
         # Return the most recent non-deleted history matching the provided name
-        response = self._get(f"histories?q=name&qv={history_name}&order=update_time")
+        filters = urllib.parse.urlencode({"q": "name", "qv": history_name, "order": "update_time"})
+        response = self._get(f"histories?{filters}")
         try:
             return response.json()[-1]
         except IndexError:
             return None
 
+    @contextlib.contextmanager
+    def test_history(
+        self, require_new: bool = True, cleanup_callback: Optional[Callable[[str], None]] = None
+    ) -> Generator[str, None, None]:
+        history_id = None
+        if not require_new:
+            history_id = DEFAULT_TARGET_HISTORY
+
+        cleanup = CLEANUP_TEST_HISTORIES
+        history_id = history_id or self.new_history()
+        try:
+            yield history_id
+        except Exception:
+            self._summarize_history(history_id)
+            raise
+        finally:
+            if cleanup and cleanup_callback is not None:
+                cleanup_callback(history_id)
+
     def new_history(self, history_name="test_history", publish_history=False):
         create_response = self._post("histories", {"name": history_name})
         try:
             create_response.raise_for_status()
         except Exception as e:
-            raise Exception(f"Error occured while creating history with name '{history_name}': {e}")
+            raise Exception(f"Error occurred while creating history with name '{history_name}': {e}")
         history_id = create_response.json()["id"]
         if publish_history:
             self.publish_history(history_id)
         return history_id
 
     def publish_history(self, history_id):
         response = self._put(f"histories/{history_id}", json.dumps({"published": True}))
         response.raise_for_status()
 
-    @nottest
     def test_data_path(self, tool_id, filename, tool_version=None):
         version_fragment = f"&tool_version={tool_version}" if tool_version else ""
         response = self._get(f"tools/{tool_id}/test_data_path?filename={filename}{version_fragment}", admin=True)
         return response.json()
 
-    @nottest
     def test_data_download(self, tool_id, filename, mode="file", is_output=True, tool_version=None):
         result = None
         local_path = None
 
         if self.supports_test_data_download:
             version_fragment = f"&tool_version={tool_version}" if tool_version else ""
             response = self._get(
@@ -429,21 +508,21 @@
             output_id = output_data.get("id")
         except AttributeError:
             output_id = output_data
         return output_id
 
     def stage_data_async(
         self,
-        test_data,
-        history_id,
-        tool_id,
-        force_path_paste=False,
-        maxseconds=DEFAULT_TOOL_TEST_WAIT,
-        tool_version=None,
-    ):
+        test_data: Dict[str, Any],
+        history_id: str,
+        tool_id: str,
+        force_path_paste: bool = False,
+        maxseconds: int = DEFAULT_TOOL_TEST_WAIT,
+        tool_version: Optional[str] = None,
+    ) -> Callable[[], None]:
         fname = test_data["fname"]
         tool_input = {
             "file_type": test_data["ftype"],
             "dbkey": test_data["dbkey"],
         }
         metadata = test_data.get("metadata", {})
         if not hasattr(metadata, "items"):
@@ -499,15 +578,15 @@
         assert (
             "jobs" in submit_response
         ), f"Invalid response from server [{submit_response}], expecting jobs in response."
         jobs = submit_response["jobs"]
         assert len(jobs) > 0, f"Invalid response from server [{submit_response}], expecting a job."
         return lambda: self.wait_for_job(jobs[0]["id"], history_id, maxseconds=maxseconds)
 
-    def run_tool(self, testdef, history_id, resource_parameters=None):
+    def run_tool(self, testdef, history_id, resource_parameters=None) -> RunToolResponse:
         # We need to handle the case where we've uploaded a valid compressed file since the upload
         # tool will have uncompressed it on the fly.
         resource_parameters = resource_parameters or {}
         inputs_tree = testdef.inputs.copy()
         for key, value in inputs_tree.items():
             values = [value] if not isinstance(value, list) else value
             new_values = []
@@ -540,22 +619,24 @@
                 print("Tool inputs not ready yet")
                 time.sleep(1)
                 continue
             else:
                 break
         submit_response_object = ensure_tool_run_response_okay(submit_response, "execute tool", inputs_tree)
         try:
-            return Bunch(
+            return RunToolResponse(
                 inputs=inputs_tree,
                 outputs=self.__dictify_outputs(submit_response_object),
                 output_collections=self.__dictify_output_collections(submit_response_object),
                 jobs=submit_response_object["jobs"],
             )
         except KeyError:
-            message = f"Error creating a job for these tool inputs - {submit_response_object['err_msg']}"
+            message = (
+                f"Error creating a job for these tool inputs - {submit_response_object.get('err_msg', 'unknown error')}"
+            )
             raise RunToolException(message, inputs_tree)
 
     def _create_collection(self, history_id, collection_def):
         create_payload = dict(
             name=collection_def.name,
             element_identifiers=self._element_identifiers(collection_def),
             collection_type=collection_def.collection_type,
@@ -581,21 +662,21 @@
                 element["name"] = element_identifier
                 tags = element_def.get("attributes").get("tags")
                 if tags:
                     element["tags"] = tags.split(",")
             element_identifiers.append(element)
         return element_identifiers
 
-    def __dictify_output_collections(self, submit_response):
+    def __dictify_output_collections(self, submit_response) -> Dict[str, Any]:
         output_collections_dict = {}
         for output_collection in submit_response["output_collections"]:
-            output_collections_dict[output_collection.get("output_name")] = output_collection
+            output_collections_dict[output_collection["output_name"]] = output_collection
         return output_collections_dict
 
-    def __dictify_outputs(self, datasets_object):
+    def __dictify_outputs(self, datasets_object) -> OutputsDict:
         # Convert outputs list to a dictionary that can be accessed by
         # output_name so can be more flexible about ordering of outputs
         # but also allows fallback to legacy access as list mode.
         outputs_dict = OutputsDict()
 
         for output in datasets_object["outputs"]:
             outputs_dict[output.get("output_name")] = output
@@ -613,26 +694,25 @@
         try:
             return self._state_ready(job_id, error_msg="Job in error state.")
         except Exception:
             if VERBOSE_ERRORS and history_id is not None:
                 self._summarize_history(history_id)
             raise
 
-    def _summarize_history(self, history_id):
+    def _summarize_history(self, history_id: str):
         if history_id is None:
             raise ValueError("_summarize_history passed empty history_id")
         print(f"Problem in history with id {history_id} - summary of history's datasets and jobs below.")
         try:
             history_contents = self.__contents(history_id)
         except Exception:
             print("*TEST FRAMEWORK FAILED TO FETCH HISTORY DETAILS*")
             return
 
         for history_content in history_contents:
-
             dataset = history_content
 
             print(ERROR_MESSAGE_DATASET_SEP)
             dataset_id = dataset.get("id", None)
             print(f"| {dataset['hid']} - {dataset['name']} (HID - NAME) ")
             if history_content["history_content_type"] == "dataset_collection":
                 history_contents_json = self._get(
@@ -760,28 +840,41 @@
                 if response.status_code == 500:
                     print(f"Retrying failed download with status code {response.status_code}")
                     time.sleep(self.download_sleep)
                     continue
                 else:
                     break
 
+            assert response
             response.raise_for_status()
             return response.content
 
         return fetcher
 
-    def api_key_header(self, key, admin, anon, headers):
+    def api_key_header(
+        self, key: Optional[str], admin: bool, anon: bool, headers: Optional[Dict[str, Optional[str]]]
+    ) -> Dict[str, Optional[str]]:
         header = headers or {}
         if not anon:
             if not key:
                 key = self.api_key if not admin else self.master_api_key
             header["x-api-key"] = key
         return header
 
-    def _post(self, path, data=None, files=None, key=None, headers=None, admin=False, anon=False, json=False):
+    def _post(
+        self,
+        path: str,
+        data: Optional[Dict[str, Any]] = None,
+        files: Optional[Dict[str, Any]] = None,
+        key: Optional[str] = None,
+        headers: Optional[Dict[str, Optional[str]]] = None,
+        admin: bool = False,
+        anon: bool = False,
+        json: bool = False,
+    ) -> Response:
         headers = self.api_key_header(key=key, admin=admin, anon=anon, headers=headers)
         url = self.get_api_url(path)
         kwd = self._prepare_request_params(data=data, files=files, as_json=json, headers=headers)
         kwd["timeout"] = kwd.pop("timeout", util.DEFAULT_SOCKET_TIMEOUT)
         return requests.post(url, **kwd)
 
     def _delete(self, path, data=None, key=None, headers=None, admin=False, anon=False, json=False):
@@ -804,15 +897,15 @@
         kwd = self._prepare_request_params(data=data, as_json=json, headers=headers)
         kwd["timeout"] = kwd.pop("timeout", util.DEFAULT_SOCKET_TIMEOUT)
         return requests.put(url, **kwd)
 
     def _get(self, path, data=None, key=None, headers=None, admin=False, anon=False):
         headers = self.api_key_header(key=key, admin=admin, anon=anon, headers=headers)
         url = self.get_api_url(path)
-        kwargs = {}
+        kwargs: Dict[str, Any] = {}
         if self.cookies:
             kwargs["cookies"] = self.cookies
         # no data for GET
         return requests.get(url, params=data, headers=headers, timeout=util.DEFAULT_SOCKET_TIMEOUT, **kwargs)
 
     def _head(self, path, data=None, key=None, headers=None, admin=False, anon=False):
         headers = self.api_key_header(key=key, admin=admin, anon=anon, headers=headers)
@@ -828,20 +921,20 @@
             return path
         elif path.startswith("/api/"):
             path = path[len("/api/") :]
         return urllib.parse.urljoin(f"{self.api_url}/", path)
 
     def _prepare_request_params(
         self,
-        data=None,
-        files=None,
+        data: Optional[Dict[str, Any]] = None,
+        files: Optional[Dict[str, Any]] = None,
         as_json: bool = False,
-        params: Optional[dict] = None,
-        headers: Optional[dict] = None,
-    ):
+        params: Optional[Dict[str, Any]] = None,
+        headers: Optional[Dict[str, Optional[str]]] = None,
+    ) -> Dict[str, Any]:
         """Handle some Galaxy conventions and work around requests issues.
 
         This is admittedly kind of hacky, so the interface may change frequently - be
         careful on reuse.
 
         If ``as_json`` is True, use post payload using request's json parameter instead
         of the data parameter (i.e. assume the contents is a json-ified blob instead of
@@ -851,35 +944,35 @@
         """
         return prepare_request_params(
             data=data, files=files, as_json=as_json, params=params, headers=headers, cookies=self.cookies
         )
 
 
 def prepare_request_params(
-    data=None,
-    files=None,
+    data: Optional[Dict[str, Any]] = None,
+    files: Optional[Dict[str, Any]] = None,
     as_json: bool = False,
-    params: Optional[dict] = None,
-    headers: Optional[dict] = None,
+    params: Optional[Dict[str, Any]] = None,
+    headers: Optional[Dict[str, Optional[str]]] = None,
     cookies: Optional[RequestsCookieJar] = None,
-):
+) -> Dict[str, Any]:
     params = params or {}
     data = data or {}
 
     # handle encoded files
     if files is None:
         # if not explicitly passed, check __files... convention used in tool testing
         # and API testing code
-        files = data.get("__files", None)
+        files = data.get("__files")
         if files is not None:
             del data["__files"]
 
     # files doesn't really work with json, so dump the parameters
     # and do a normal POST with request's data parameter.
-    if bool(files) and as_json:
+    if files and as_json:
         as_json = False
         new_items = {}
         for key, val in data.items():
             if isinstance(val, dict) or isinstance(val, list):
                 new_items[key] = dumps(val)
         data.update(new_items)
 
@@ -942,15 +1035,20 @@
         super().__init__(message)
         self.inputs = inputs
         self.dynamic_param_error = dynamic_param_error
 
 
 # Galaxy specific methods - rest of this can be used with arbitrary files and such.
 def verify_hid(
-    filename, hda_id, attributes, test_data_downloader, hid="", dataset_fetcher=None, keep_outputs_dir=False
+    filename: Optional[str],
+    hda_id: str,
+    attributes: Dict[str, Any],
+    test_data_downloader,
+    dataset_fetcher=None,
+    keep_outputs_dir: Optional[str] = None,
 ):
     assert dataset_fetcher is not None
 
     def verify_extra_files(extra_files):
         _verify_extra_files_content(
             extra_files,
             hda_id,
@@ -1042,15 +1140,15 @@
 def _verify_composite_datatype_file_content(
     file_name,
     hda_id,
     base_name=None,
     attributes=None,
     dataset_fetcher=None,
     test_data_downloader=None,
-    keep_outputs_dir=False,
+    keep_outputs_dir: Optional[str] = None,
     mode="file",
 ):
     assert dataset_fetcher is not None
 
     data = dataset_fetcher(hda_id, base_name)
     item_label = f"History item {hda_id}"
     try:
@@ -1065,15 +1163,17 @@
         )
     except AssertionError as err:
         errmsg = f"Composite file ({base_name}) of {item_label} different than expected, difference:\n"
         errmsg += util.unicodify(err)
         raise AssertionError(errmsg)
 
 
-def _verify_extra_files_content(extra_files, hda_id, dataset_fetcher, test_data_downloader, keep_outputs_dir):
+def _verify_extra_files_content(
+    extra_files: List[Dict[str, Any]], hda_id: str, dataset_fetcher, test_data_downloader, keep_outputs_dir
+):
     files_list = []
     cleanup_directories = []
     for extra_file_dict in extra_files:
         extra_file_type = extra_file_dict["type"]
         extra_file_name = extra_file_dict["name"]
         extra_file_attributes = extra_file_dict["attributes"]
         extra_file_value = extra_file_dict["value"]
@@ -1105,20 +1205,25 @@
                 mode=extra_file_type,
             )
     finally:
         for path in cleanup_directories:
             shutil.rmtree(path)
 
 
-class NullClientTestConfig:
+class TestConfig(Protocol):
+    def get_test_config(self, job_data: Dict[str, Any]) -> Optional[Dict[str, Any]]:
+        ...
+
+
+class NullClientTestConfig(TestConfig):
     def get_test_config(self, job_data):
         return None
 
 
-class DictClientTestConfig:
+class DictClientTestConfig(TestConfig):
     def __init__(self, tools):
         self._tools = tools or {}
 
     def get_test_config(self, job_data):
         # TODO: allow short ids, allow versions below outer id instead of key concatenation.
         tool_id = job_data.get("tool_id")
         tool_version = job_data.get("tool_version")
@@ -1148,45 +1253,45 @@
                 return tool_version_test_config["default"]
             elif is_default:
                 return tool_version_test_config
         return None
 
 
 def verify_tool(
-    tool_id,
-    galaxy_interactor,
-    resource_parameters=None,
-    register_job_data=None,
-    test_index=0,
-    tool_version=None,
-    quiet=False,
-    test_history=None,
-    no_history_cleanup=False,
-    publish_history=False,
-    force_path_paste=False,
-    maxseconds=DEFAULT_TOOL_TEST_WAIT,
-    tool_test_dicts=None,
-    client_test_config=None,
-    skip_with_reference_data=False,
-    skip_on_dynamic_param_errors=False,
+    tool_id: str,
+    galaxy_interactor: "GalaxyInteractorApi",
+    resource_parameters: Optional[Dict[str, Any]] = None,
+    register_job_data: Optional[JobDataCallbackT] = None,
+    test_index: int = 0,
+    tool_version: Optional[str] = None,
+    quiet: bool = False,
+    test_history: Optional[str] = None,
+    no_history_cleanup: bool = False,
+    publish_history: bool = False,
+    force_path_paste: bool = False,
+    maxseconds: int = DEFAULT_TOOL_TEST_WAIT,
+    client_test_config: Optional[TestConfig] = None,
+    skip_with_reference_data: bool = False,
+    skip_on_dynamic_param_errors: bool = False,
+    _tool_test_dicts: Optional[ToolTestDictsT] = None,  # extension point only for tests
 ):
     if resource_parameters is None:
         resource_parameters = {}
     if client_test_config is None:
         client_test_config = NullClientTestConfig()
-    tool_test_dicts = tool_test_dicts or galaxy_interactor.get_tool_tests(tool_id, tool_version=tool_version)
+    tool_test_dicts = _tool_test_dicts or galaxy_interactor.get_tool_tests(tool_id, tool_version=tool_version)
     tool_test_dict = tool_test_dicts[test_index]
     if "test_index" not in tool_test_dict:
         tool_test_dict["test_index"] = test_index
     if "tool_id" not in tool_test_dict:
         tool_test_dict["tool_id"] = tool_id
     if tool_version is None and "tool_version" in tool_test_dict:
         tool_version = tool_test_dict.get("tool_version")
 
-    job_data = {
+    job_data: JobDataT = {
         "tool_id": tool_id,
         "tool_version": tool_version,
         "test_index": test_index,
     }
     client_config = client_test_config.get_test_config(job_data)
     skip_message = None
     if client_config is not None:
@@ -1198,21 +1303,21 @@
         required_loc_files = tool_test_dict.get("required_loc_files")
         # TODO: actually hit the API and see if these tables are available.
         if required_data_tables:
             skip_message = f"Skipping test because of required data tables ({required_data_tables})"
         if required_loc_files:
             skip_message = f"Skipping test because of required loc files ({required_loc_files})"
 
-    if skip_message:
+    if skip_message and register_job_data:
         job_data["status"] = "skip"
         register_job_data(job_data)
         return
 
     tool_test_dict.setdefault("maxseconds", maxseconds)
-    testdef = ToolTestDescription(tool_test_dict)
+    testdef = ToolTestDescription(cast(ToolTestDict, tool_test_dict))
     _handle_def_errors(testdef)
 
     created_history = False
     if test_history is None:
         created_history = True
         history_name = f"Tool Test History for {tool_id}/{tool_version}-{test_index}"
         test_history = galaxy_interactor.new_history(history_name=history_name, publish_history=publish_history)
@@ -1220,15 +1325,15 @@
     # Upload data to test_history, run the tool and check the outputs - record
     # API input, job info, tool run exception, as well as exceptions related to
     # job output checking and register they with the test plugin so it can
     # record structured information.
     tool_inputs = None
     job_stdio = None
     job_output_exceptions = None
-    tool_execution_exception = None
+    tool_execution_exception: Optional[Exception] = None
     input_staging_exception = None
     expected_failure_occurred = False
     begin_time = time.time()
     try:
         try:
             stage_data_in_history(
                 galaxy_interactor,
@@ -1314,17 +1419,17 @@
             raise Exception("Test parse failure")
 
 
 def _verify_outputs(testdef, history, jobs, data_list, data_collection_list, galaxy_interactor, quiet=False):
     assert len(jobs) == 1, "Test framework logic error, somehow tool test resulted in more than one job."
     job = jobs[0]
 
-    found_exceptions = []
+    found_exceptions: List[Exception] = []
 
-    def register_exception(e):
+    def register_exception(e: Exception):
         if not found_exceptions and not quiet:
             # Only print this stuff out once.
             for stream in ["stdout", "stderr"]:
                 if stream in job_stdio:
                     print(_format_stream(job_stdio[stream], stream=stream, format=True), file=sys.stderr)
         found_exceptions.append(e)
 
@@ -1345,23 +1450,15 @@
 
     job_stdio = galaxy_interactor.get_job_stdio(job["id"])
 
     if testdef.num_outputs is not None:
         expected = testdef.num_outputs
         actual = len(data_list) + len(data_collection_list)
         if expected != actual:
-            message = f"Incorrect number of outputs - expected {expected}, found {actual}: datasets {data_list.keys()} collections {data_collection_list.keys()}"
-            error = AssertionError(message)
-            register_exception(error)
-
-    if testdef.num_outputs is not None:
-        expected = testdef.num_outputs
-        actual = len(data_list) + len(data_collection_list)
-        if expected != actual:
-            message = f"Incorrect number of outputs - expected {expected}, found {actual}: datasets {data_list.keys()} collections {data_collection_list.keys()}"
+            message = f"Incorrect number of outputs - expected {expected}, found {actual} (dataset(s): {','.join(data_list.keys())} collection(s): {' '.join(data_collection_list.keys())})"
             error = AssertionError(message)
             register_exception(error)
 
     if not job_failed and testdef.expect_failure:
         error = AssertionError("Expected job to fail but Galaxy indicated the job successfully completed.")
         register_exception(error)
 
@@ -1460,14 +1557,17 @@
                 output_collection_def, data_collection_id, history, job["tool_id"]
             )
         except Exception as e:
             register_exception(e)
 
     if found_exceptions and not testdef.expect_test_failure:
         raise JobOutputsError(found_exceptions, job_stdio)
+    elif not found_exceptions and testdef.expect_test_failure:
+        register_exception(AssertionError("Expected job to miss at least one test assumption but all were met."))
+        raise JobOutputsError(found_exceptions, job_stdio)
     else:
         return job_stdio
 
 
 def _format_stream(output, stream, format):
     output = output or ""
     if format:
@@ -1490,23 +1590,29 @@
 class ToolTestDescription:
     """
     Encapsulates information about a tool test, and allows creation of a
     dynamic TestCase class (the unittest framework is very class oriented,
     doing dynamic tests in this way allows better integration)
     """
 
-    def __init__(self, processed_test_dict):
+    def __init__(self, processed_test_dict: ToolTestDict):
         assert (
             "test_index" in processed_test_dict
         ), "Invalid processed test description, must have a 'test_index' for naming, etc.."
         test_index = processed_test_dict["test_index"]
         name = processed_test_dict.get("name", f"Test-{test_index + 1}")
-        maxseconds = processed_test_dict.get("maxseconds", DEFAULT_TOOL_TEST_WAIT)
-        if maxseconds is not None:
-            maxseconds = int(maxseconds)
+        error_in_test_definition = processed_test_dict["error"]
+        if not error_in_test_definition:
+            processed_test_dict = cast(ValidToolTestDict, processed_test_dict)
+            maxseconds = int(processed_test_dict.get("maxseconds") or DEFAULT_TOOL_TEST_WAIT or 86400)
+            output_collections = processed_test_dict.get("output_collections", [])
+        else:
+            processed_test_dict = cast(InvalidToolTestDict, processed_test_dict)
+            maxseconds = DEFAULT_TOOL_TEST_WAIT
+            output_collections = []
 
         self.test_index = test_index
         assert (
             "tool_id" in processed_test_dict
         ), "Invalid processed test description, must have a 'tool_id' for naming, etc.."
         self.tool_id = processed_test_dict["tool_id"]
         self.tool_version = processed_test_dict.get("tool_version")
@@ -1527,17 +1633,15 @@
         self.inputs = loaded_inputs
         self.outputs = processed_test_dict.get("outputs", [])
         self.num_outputs = processed_test_dict.get("num_outputs", None)
 
         self.error = processed_test_dict.get("error", False)
         self.exception = processed_test_dict.get("exception", None)
 
-        self.output_collections = [
-            TestCollectionOutputDef.from_dict(d) for d in processed_test_dict.get("output_collections", [])
-        ]
+        self.output_collections = [TestCollectionOutputDef.from_dict(d) for d in output_collections]
         self.command_line = processed_test_dict.get("command_line", None)
         self.command_version = processed_test_dict.get("command_version", None)
         self.stdout = processed_test_dict.get("stdout", None)
         self.stderr = processed_test_dict.get("stderr", None)
         self.expect_exit_code = processed_test_dict.get("expect_exit_code", None)
         self.expect_failure = processed_test_dict.get("expect_failure", False)
         self.expect_test_failure = processed_test_dict.get("expect_test_failure", False)
@@ -1576,15 +1680,14 @@
             "required_data_tables": self.required_data_tables,
             "required_loc_files": self.required_loc_files,
             "error": self.error,
             "exception": self.exception,
         }
 
 
-@nottest
 def test_data_iter(required_files):
     for fname, extra in required_files:
         data_dict = dict(
             fname=fname,
             metadata=extra.get("metadata", {}),
             composite_data=extra.get("composite_data", []),
             ftype=extra.get("ftype", DEFAULT_FTYPE),
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/script.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/verify/script.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,96 +1,116 @@
 #!/usr/bin/env python
 
 import argparse
+import concurrent.futures.thread
 import datetime as dt
 import json
 import logging
 import os
 import sys
 import tempfile
-from collections import namedtuple
 from concurrent.futures import (
     thread,
     ThreadPoolExecutor,
 )
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    NamedTuple,
+    Optional,
+)
 
 import yaml
 
 from galaxy.tool_util.verify.interactor import (
     DictClientTestConfig,
     GalaxyInteractorApi,
+    ToolTestDictsT,
     verify_tool,
 )
 
 DESCRIPTION = """Script to quickly run a tool test against a running Galaxy instance."""
 DEFAULT_SUITE_NAME = "Galaxy Tool Tests"
 ALL_TESTS = -1
 ALL_TOOLS = "*"
 ALL_VERSION = "*"
 LATEST_VERSION = None
 
 
-TestReference = namedtuple("TestReference", ["tool_id", "tool_version", "test_index"])
-TestException = namedtuple("TestException", ["tool_id", "exception", "was_recorded"])
+class TestReference(NamedTuple):
+    tool_id: str
+    tool_version: Optional[str]
+    test_index: int
+
+
+class TestException(NamedTuple):
+    tool_id: str
+    exception: Exception
+    was_recorded: bool
 
 
 class Results:
-    def __init__(self, default_suitename, test_json, append=False, galaxy_url=None):
+    test_exceptions: List[TestException]
+
+    def __init__(
+        self, default_suitename: str, test_json: str, append: bool = False, galaxy_url: Optional[str] = None
+    ) -> None:
         self.test_json = test_json or "-"
         self.galaxy_url = galaxy_url
         test_results = []
-        test_exceptions = []
         suitename = default_suitename
         if append:
             assert test_json != "-"
             with open(test_json) as f:
                 previous_results = json.load(f)
                 test_results = previous_results["tests"]
                 if "suitename" in previous_results:
                     suitename = previous_results["suitename"]
         self.test_results = test_results
-        self.test_exceptions = test_exceptions
+        self.test_exceptions = []
         self.suitename = suitename
 
-    def register_result(self, result):
+    def register_result(self, result: Dict[str, Any]) -> None:
         self.test_results.append(result)
 
-    def register_exception(self, test_exception):
+    def register_exception(self, test_exception: TestException) -> None:
         self.test_exceptions.append(test_exception)
 
-    def already_successful(self, test_reference):
+    def already_successful(self, test_reference: TestReference) -> bool:
         test_data = self._previous_test_data(test_reference)
         if test_data:
             if "status" in test_data and test_data["status"] == "success":
                 return True
 
         return False
 
-    def already_executed(self, test_reference):
+    def already_executed(self, test_reference: TestReference) -> bool:
         test_data = self._previous_test_data(test_reference)
         if test_data:
             if "status" in test_data and test_data["status"] != "skipped":
                 return True
 
         return False
 
-    def _previous_test_data(self, test_reference):
+    def _previous_test_data(self, test_reference: TestReference) -> Optional[Dict[str, Any]]:
         test_id = _test_id_for_reference(test_reference)
         for test_result in self.test_results:
             if test_result.get("id") != test_id:
                 continue
 
             has_data = test_result.get("has_data", False)
             if has_data:
                 test_data = test_result.get("data", {})
                 return test_data
 
         return None
 
-    def write(self):
+    def write(self) -> None:
         tests = sorted(self.test_results, key=lambda el: el["id"])
         n_passed, n_failures, n_skips = 0, 0, 0
         n_errors = len([e for e in self.test_exceptions if not e.was_recorded])
         for test in tests:
             has_data = test.get("has_data", False)
             if has_data:
                 test_data = test.get("data", {})
@@ -120,64 +140,45 @@
             report_obj["galaxy_url"] = self.galaxy_url
         if self.test_json == "-":
             print(json.dumps(report_obj))
         else:
             with open(self.test_json, "w") as f:
                 json.dump(report_obj, f)
 
-    def info_message(self):
+    def info_message(self) -> str:
         messages = []
         passed_tests = self._tests_with_status("success")
         messages.append("Passed tool tests ({}): {}".format(len(passed_tests), [t["id"] for t in passed_tests]))
         failed_tests = self._tests_with_status("failure")
         messages.append("Failed tool tests ({}): {}".format(len(failed_tests), [t["id"] for t in failed_tests]))
-        skiped_tests = self._tests_with_status("skip")
-        messages.append("Skipped tool tests ({}): {}".format(len(skiped_tests), [t["id"] for t in skiped_tests]))
+        skipped_tests = self._tests_with_status("skip")
+        messages.append("Skipped tool tests ({}): {}".format(len(skipped_tests), [t["id"] for t in skipped_tests]))
         errored_tests = self._tests_with_status("error")
         messages.append("Errored tool tests ({}): {}".format(len(errored_tests), [t["id"] for t in errored_tests]))
         return "\n".join(messages)
 
-    @property
-    def success_count(self):
-        self._tests_with_status("success")
-
-    @property
-    def skip_count(self):
-        self._tests_with_status("skip")
-
-    @property
-    def error_count(self):
-        return self._tests_with_status("error") + len(self.test_exceptions)
-
-    @property
-    def failure_count(self):
-        return self._tests_with_status("failure")
-
-    def _tests_with_status(self, status):
+    def _tests_with_status(self, status: str) -> List[Dict[str, Any]]:
         return [t for t in self.test_results if t.get("data", {}).get("status") == status]
 
 
 def test_tools(
-    galaxy_interactor,
-    test_references,
-    results,
-    log=None,
-    parallel_tests=1,
-    history_per_test_case=False,
-    history_name=None,
-    no_history_reuse=False,
-    no_history_cleanup=False,
-    publish_history=False,
-    retries=0,
-    verify_kwds=None,
-):
-    """Run through tool tests and write report.
-
-    Refactor this into Galaxy in 21.01.
-    """
+    galaxy_interactor: GalaxyInteractorApi,
+    test_references: List[TestReference],
+    results: Results,
+    log: Optional[logging.Logger] = None,
+    parallel_tests: int = 1,
+    history_per_test_case: bool = False,
+    history_name: Optional[str] = None,
+    no_history_reuse: bool = False,
+    no_history_cleanup: bool = False,
+    publish_history: bool = False,
+    retries: int = 0,
+    verify_kwds: Optional[Dict[str, Any]] = None,
+) -> None:
+    """Run through tool tests and write report."""
     verify_kwds = (verify_kwds or {}).copy()
     tool_test_start = dt.datetime.now()
     history_created = False
     test_history = None
     if not history_per_test_case:
         if not history_name:
             history_name = f"History for {results.suitename}"
@@ -214,30 +215,30 @@
                     publish_history=publish_history,
                 )
         finally:
             # Always write report, even if test was cancelled.
             try:
                 executor.shutdown(wait=True)
             except KeyboardInterrupt:
-                executor._threads.clear()
-                thread._threads_queues.clear()
+                executor._threads.clear()  # type: ignore[attr-defined]
+                thread._threads_queues.clear()  # type: ignore[attr-defined]
             results.write()
             if log:
                 if results.test_json == "-":
                     destination = "standard output"
                 else:
                     destination = os.path.abspath(results.test_json)
                 log.info(f"Report written to '{destination}'")
                 log.info(results.info_message())
                 log.info(f"Total tool test time: {dt.datetime.now() - tool_test_start}")
             if history_created and not no_history_cleanup:
                 galaxy_interactor.delete_history(test_history)
 
 
-def _test_id_for_reference(test_reference):
+def _test_id_for_reference(test_reference: "TestReference") -> str:
     tool_id = test_reference.tool_id
     tool_version = test_reference.tool_version
     test_index = test_reference.test_index
 
     if tool_version and tool_id.endswith(f"/{tool_version}"):
         tool_id = tool_id[: -len(f"/{tool_version}")]
 
@@ -246,34 +247,34 @@
         label_base += f"/{str(tool_version)}"
 
     test_id = f"{label_base}-{str(test_index)}"
     return test_id
 
 
 def _test_tool(
-    executor,
-    test_reference,
-    results,
-    galaxy_interactor,
-    log,
-    retries,
-    publish_history,
-    verify_kwds,
-):
+    executor: concurrent.futures.thread.ThreadPoolExecutor,
+    test_reference: "TestReference",
+    results: Results,
+    galaxy_interactor: GalaxyInteractorApi,
+    log: Optional[logging.Logger],
+    retries: int,
+    publish_history: bool,
+    verify_kwds: Dict[str, Any],
+) -> None:
     tool_id = test_reference.tool_id
     tool_version = test_reference.tool_version
     test_index = test_reference.test_index
     # If given a tool_id with a version suffix, strip it off so we can treat tool_version
     # correctly at least in client_test_config.
     if tool_version and tool_id.endswith(f"/{tool_version}"):
         tool_id = tool_id[: -len(f"/{tool_version}")]
 
     test_id = _test_id_for_reference(test_reference)
 
-    def run_test():
+    def run_test() -> None:
         run_retries = retries
         job_data = None
         job_exception = None
 
         def register(job_data_):
             nonlocal job_data
             job_data = job_data_
@@ -316,76 +317,83 @@
                 test_exception = TestException(tool_id, job_exception, was_recorded)
                 results.register_exception(test_exception)
 
     executor.submit(run_test)
 
 
 def build_case_references(
-    galaxy_interactor,
-    tool_id=ALL_TOOLS,
-    tool_version=LATEST_VERSION,
-    test_index=ALL_TESTS,
-    page_size=0,
-    page_number=0,
-    test_filters=None,
-    log=None,
-):
-    test_references = []
+    galaxy_interactor: GalaxyInteractorApi,
+    tool_id: str = ALL_TOOLS,
+    tool_version: Optional[str] = LATEST_VERSION,
+    test_index: int = ALL_TESTS,
+    page_size: int = 0,
+    page_number: int = 0,
+    test_filters: Optional[List[Callable[[TestReference], bool]]] = None,
+    log: Optional[logging.Logger] = None,
+) -> List[TestReference]:
+    test_references: List[TestReference] = []
     if tool_id == ALL_TOOLS:
         tests_summary = galaxy_interactor.get_tests_summary()
         for tool_id, tool_versions_dict in tests_summary.items():
             for tool_version, summary in tool_versions_dict.items():
                 for test_index in range(summary["count"]):
                     test_reference = TestReference(tool_id, tool_version, test_index)
                     test_references.append(test_reference)
     else:
         assert tool_id
-        tool_test_dicts = galaxy_interactor.get_tool_tests(tool_id, tool_version=tool_version) or {}
+        tool_test_dicts: ToolTestDictsT = galaxy_interactor.get_tool_tests(tool_id, tool_version=tool_version)
         for i, tool_test_dict in enumerate(tool_test_dicts):
             this_tool_version = tool_test_dict.get("tool_version", tool_version)
             this_test_index = i
             if test_index == ALL_TESTS or i == test_index:
                 test_reference = TestReference(tool_id, this_tool_version, this_test_index)
                 test_references.append(test_reference)
 
     if test_filters is not None and len(test_filters) > 0:
-        filtered_test_references = []
+        filtered_test_references: List[TestReference] = []
         for test_reference in test_references:
             skip_test = False
             for test_filter in test_filters:
                 if test_filter(test_reference):
                     if log is not None:
                         log.debug(f"Filtering test for {test_reference}, skipping")
                     skip_test = True
             if not skip_test:
                 filtered_test_references.append(test_reference)
-        log.info(f"Skipping {len(test_references)-len(filtered_test_references)} out of {len(test_references)} tests.")
+        if log is not None:
+            log.info(
+                f"Skipping {len(test_references)-len(filtered_test_references)} out of {len(test_references)} tests."
+            )
         test_references = filtered_test_references
 
     if page_size > 0:
         slice_start = page_size * page_number
         slice_end = page_size * (page_number + 1)
         test_references = test_references[slice_start:slice_end]
 
     return test_references
 
 
-def main(argv=None):
+def main(argv=None) -> None:
     if argv is None:
         argv = sys.argv[1:]
 
     args = arg_parser().parse_args(argv)
     try:
         run_tests(args)
     except Exception as exc:
         print(f"ERROR: {exc}", file=sys.stderr)
         sys.exit(1)
 
 
-def run_tests(args, test_filters=None, log=None):
+def run_tests(
+    args: argparse.Namespace,
+    test_filters: Optional[List[Callable[[TestReference], bool]]] = None,
+    log: Optional[logging.Logger] = None,
+) -> None:
     # Split out argument parsing so we can quickly build other scripts - such as a script
     # to run all tool tests for a workflow by just passing in a custom test_filters.
     test_filters = test_filters or []
     log = log or setup_global_logger(__name__, verbose=args.verbose)
 
     client_test_config_path = args.client_test_config
     if client_test_config_path is not None:
@@ -457,20 +465,18 @@
         no_history_cleanup=args.no_history_cleanup,
         publish_history=get_option("publish_history"),
         verify_kwds=verify_kwds,
     )
     exceptions = results.test_exceptions
     if exceptions:
         exception = exceptions[0]
-        if hasattr(exception, "exception"):
-            exception = exception.exception
-        raise exception
+        raise exception.exception
 
 
-def setup_global_logger(name, log_file=None, verbose=False):
+def setup_global_logger(name: str, log_file: Optional[str] = None, verbose: bool = False) -> logging.Logger:
     formatter = logging.Formatter("%(asctime)s %(levelname)-5s - %(message)s")
     console = logging.StreamHandler()
     console.setFormatter(formatter)
 
     logger = logging.getLogger(name)
     logger.setLevel(logging.DEBUG if verbose else logging.INFO)
     logger.addHandler(console)
@@ -483,15 +489,15 @@
         log_file = temp.name
     file_handler = logging.FileHandler(log_file)
     logger.addHandler(file_handler)
     logger.info(f"Storing log file in: {log_file}")
     return logger
 
 
-def arg_parser():
+def arg_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(description=DESCRIPTION)
     parser.add_argument("-u", "--galaxy-url", default="http://localhost:8080", help="Galaxy URL")
     parser.add_argument("-k", "--key", default=None, help="Galaxy User API Key")
     parser.add_argument("-a", "--admin-key", default=None, help="Galaxy Admin API Key")
     parser.add_argument(
         "--force_path_paste",
         default=False,
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/test_config.sample.yml` & `galaxy-tool-util-23.0.1/galaxy/tool_util/verify/test_config.sample.yml`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/test_data.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/verify/test_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,31 +31,36 @@
         if file_dirs is None:
             file_dirs = "test-data,https://github.com/galaxyproject/galaxy-test-data.git"
         if file_dirs:
             self.resolvers = [build_resolver(u, environ) for u in LIST_SEP.split(file_dirs)]
         else:
             self.resolvers = []
 
-    def get_filename(self, name):
+    def get_filename(self, name: str) -> str:
         for resolver in self.resolvers or []:
             if not resolver.exists(name):
                 continue
             filename = resolver.path(name)
             if filename:
                 return os.path.abspath(filename)
+        raise TestDataNotFoundError(f"Failed to find test file {name} against any test data resolvers")
 
-    def get_filecontent(self, name):
+    def get_filecontent(self, name: str) -> bytes:
         filename = self.get_filename(name=name)
         with open(filename, mode="rb") as f:
             return f.read()
 
-    def get_directory(self, name):
+    def get_directory(self, name: str) -> str:
         return self.get_filename(name=name)
 
 
+class TestDataNotFoundError(ValueError):
+    pass
+
+
 def build_resolver(uri, environ):
     if uri.startswith("http") and uri.endswith(".git"):
         return GitDataResolver(uri, environ)
     else:
         return FileDataResolver(uri)
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/verify/wait.py` & `galaxy-tool-util-23.0.1/galaxy/tool_util/verify/wait.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/xsd/LICENSE` & `galaxy-tool-util-23.0.1/galaxy/tool_util/xsd/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/xsd/README.md` & `galaxy-tool-util-23.0.1/galaxy/tool_util/xsd/README.md`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/xsd/galaxy.jxb` & `galaxy-tool-util-23.0.1/galaxy/tool_util/xsd/galaxy.jxb`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/xsd/galaxy.xsd` & `galaxy-tool-util-23.0.1/galaxy/tool_util/xsd/galaxy.xsd`

 * *Files 1% similar despite different names*

#### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy/tool_util/xsd/galaxy.xsd` & `galaxy-tool-util-23.0.1/galaxy/tool_util/xsd/galaxy.xsd`

```diff
@@ -49,14 +49,19 @@
 - Exit immediately if a command exits with a non-zero status (`set -e`).
 - Assume sort order for collection elements.
 
 ### 21.09
 
 - Do not strip leading and trailing whitespaces in `from_work_dir` attribute.
 
+### 23.0
+
+- Text parameters that are inferred to be optional (i.e the `optional` tag is not set, but the tool parameter accepts an empty string)
+  are set to `None` for templating in Cheetah. Older tools receive the empty string `""` as the templated value.
+
 ### Examples
 
 A normal tool:
 
 ```xml
 <tool id="seqtk_seq"
       name="Convert FASTQ to FASTA"
@@ -224,15 +229,15 @@
       <xs:attribute name="license" type="xs:string">
         <xs:annotation>
           <xs:documentation xml:lang="en">This string specifies any full URI or a
 a short [SPDX](https://spdx.org/licenses/) identifier for a license for this tool
 wrapper. The tool wrapper version can be indepedent of the underlying tool. This
 license covers the tool XML and associated scripts shipped with the tool.
 
-This is interpreted as [schema.org/license](https://schema.org/license)).</xs:documentation>
+This is interpreted as [schema.org/license](https://schema.org/license) property.</xs:documentation>
         </xs:annotation>
       </xs:attribute>
       <xs:attribute name="python_template_version" type="xs:float">
         <xs:annotation>
           <xs:documentation xml:lang="en">This string specifies the minimum Python
 version that is able to fill the Cheetah sections of the tool. If unset defaults
 to 2.7 if the profile is older than 19.05, otherwise defaults to 3.5. Galaxy will
@@ -1535,14 +1540,37 @@
 This tag set defines the variable that names the output dataset for the
 functional test framework. The functional test framework will execute the tool
 using the parameters defined in the ``<param>`` tag sets and generate a
 temporary file, which will either be compared with the file named in the
 ``file`` attribute value or checked against assertions made by a child
 ``assert_contents`` tag to verify that the tool is functionally correct.
 
+Different methods can be chosen for the comparison with the local file specified
+by ``file`` using the ``compare`` attribute:
+
+- ``diff``: uses diff to compare the history data set and the file provided by
+  ``file``. Compressed files are decompressed before the compariopm if
+  ``decompress`` is set to ``true``. BAM files are converted to SAM before the
+  comparision and for pdf some special rules are implemented. The number of
+  allowed differences can be set with ``lines_diff``.  If ``sort="true"`` history
+  and local data is sorted before the comparison.
+- ``re_match``: each line of the history data set is compared to the regular
+  expression specified in the corresponding line of the ``file``. The allowed
+  number of non matching lines can be set with ``lines_diff`` and the history
+  dataset is sorted if ``sort`` is set to ``true``.
+- ``re_match_multiline``: it is checked if the history data sets matches the
+  multi line regular expression given in ``file``. The history dataset is sorted
+  before the comparison if the ``sort`` atrribute is set to ``true``.
+- ``contains``: check if each line in ``file`` is contained in the history data set.
+  The allowed number of lines that are not contained in the history dataset
+  can be set with ``lines_diff``.
+- ``sim_size``: compares the size of the history dataset and the ``file`` subject to
+  the values of the ``delta`` and ``delta_frac`` attributes. Note that a ``has_size``
+  content assertion should be preferred, because this avoids storing the test file.
+
         ]]></xs:documentation>
     </xs:annotation>
     <xs:sequence>
       <xs:group ref="TestOutputElement" minOccurs="0" maxOccurs="unbounded"/>
     </xs:sequence>
     <!-- TODO: This would be more percise if this was required if at the top-level. -->
     <xs:attribute name="name" type="xs:string">
@@ -1584,17 +1612,20 @@
 data type. If these do not match, the test will fail.
 
 ]]></xs:documentation>
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="sort" type="PermissiveBoolean">
       <xs:annotation>
-        <xs:documentation xml:lang="en">This flag causes the lines of the output
-to be sorted before they are compared to the expected output. This could be
-useful for non-deterministic output.</xs:documentation>
+        <xs:documentation xml:lang="en"><![CDATA[
+
+Applies only if ``compare`` is ``diff``, ``re_match`` or ``re_match_multiline``. This flag causes the lines of the history data set to be sorted before the comparison. In case of ``diff`` and ``re_match`` also the local file is sorted. This could be
+useful for non-deterministic output.
+
+]]></xs:documentation>
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="value" type="xs:string">
       <xs:annotation>
         <xs:documentation xml:lang="en">An alias for ``file``.</xs:documentation>
       </xs:annotation>
     </xs:attribute>
@@ -1620,15 +1651,15 @@
 
 ]]></xs:documentation>
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="compare" type="TestOutputCompareType"/>
     <xs:attribute name="lines_diff" type="xs:integer">
       <xs:annotation>
-        <xs:documentation xml:lang="en">If ``compare`` is set to ``diff``, the number of lines of difference to allow (each line with a modification is a line added and a line removed so this counts as two lines).</xs:documentation>
+        <xs:documentation xml:lang="en">Applies only if ``compare`` is set to ``diff``, ``re_match``, and ``contains``. If ``compare`` is set to ``diff``, the number of lines of difference to allow (each line with a modification is a line added and a line removed so this counts as two lines).</xs:documentation>
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="decompress" type="PermissiveBoolean">
       <xs:annotation>
         <xs:documentation xml:lang="en"><![CDATA[
 When this attribute is true and ``compare`` is set to ``diff``, try to decompress files if needed. This flag is useful for testing compressed outputs that are non-deterministic despite having deterministic decompressed contents. By default, only files compressed with bz2, gzip and zip will be automatically decompressed. This is available in Galaxy since release 17.05 and was introduced in [pull request #3550](https://github.com/galaxyproject/galaxy/pull/3550).
 ]]></xs:documentation>
@@ -1999,15 +2030,15 @@
       <xs:group ref="TestAssertionsArchive" minOccurs="0" maxOccurs="unbounded"/>
       <xs:group ref="TestAssertionsXml" minOccurs="0" maxOccurs="unbounded"/>
       <xs:group ref="TestAssertionsH5" minOccurs="0" maxOccurs="unbounded"/>
     </xs:choice>
   </xs:complexType>
   <xs:group name="TestAssertionsGeneral">
     <xs:annotation>
-      <xs:documentation xml:lang="en"><![CDATA[General asserions]]></xs:documentation>
+      <xs:documentation xml:lang="en"><![CDATA[General assertions]]></xs:documentation>
     </xs:annotation>
     <xs:choice>
       <xs:element name="has_size" type="AssertHasSize"/>
     </xs:choice>
   </xs:group>
   <xs:group name="TestAssertionsText">
     <xs:annotation>
@@ -2217,14 +2248,19 @@
 number of columns.
 
 $attribute_list::5
 ]]></xs:documentation>
     </xs:annotation>
     <xs:attributeGroup ref="AssertAttributeN"/>
     <xs:attributeGroup ref="AssertAttributeNegate"/>
+    <xs:attribute name="comment" type="xs:string">
+      <xs:annotation>
+        <xs:documentation xml:lang="en">Comment character(s) used to skip comment lines (which should not be used for counting columns)</xs:documentation>
+      </xs:annotation>
+    </xs:attribute>
   </xs:complexType>
   <xs:complexType name="AssertHasArchiveMember">
     <xs:annotation>
       <xs:documentation xml:lang="en"><![CDATA[
 This tag allows to check if ``path`` is contained in a compressed file. The path
 is a regular expression that is matched against the full paths of the objects in
 the compressed file (remember that "matching" means it is checked if a prefix of
@@ -3371,15 +3407,19 @@
 Used only when the ``type`` attribute value is ``data_column``, ``group_tag``,
 or ``select``.
             ]]></xs:documentation>
           </xs:annotation>
         </xs:attribute>
         <xs:attribute name="accept_default" type="PermissiveBoolean">
           <xs:annotation>
-            <xs:documentation xml:lang="en"/>
+            <xs:documentation xml:lang="en"><![CDATA[
+Deprecated. Take the value given by ``default_value`` (or ``value``) and ``1``
+if no ``value`` is given. Applies to ``data_column`` and ``group_tag``
+parameters.
+            ]]></xs:documentation>
           </xs:annotation>
         </xs:attribute>
         <xs:attribute name="refresh_on_change" type="PermissiveBoolean">
           <xs:annotation>
             <xs:documentation xml:lang="en">Force a reload of the tool panel
 when the value of this parameter changes to allow ``code`` file processing.
 See deprecation-like notice for ``code`` blocks.</xs:documentation>
@@ -3669,14 +3709,15 @@
 ``$__root_dir__`` | Top-level Galaxy source directory made absolute via ``os.path.abspath()``
 ``$__datatypes_config__`` | ``config/galaxy.ini``'s datatypes_config value
 ``$__user_id__`` | Email's numeric ID (id column of ``galaxy_user`` table in the database)
 ``$__user_email__`` | User's email address
 ``$__app__`` | The ``galaxy.app.UniverseApplication`` instance, gives access to all other configuration file variables (e.g. $__app__.config.output_size_limit). Should be used as a last resort, may go away in future releases.
 ``$__target_datatype__`` | Only available in converter tools when run internally by Galaxy. Contains the target datatype of the conversion
 
+
 Additional runtime properties are available as environment variables. Since these
 are not Cheetah variables (the values aren't available until runtime) these should likely
 be escaped with a backslash (``\``) when appearing in ``command`` or ``configfile`` elements.
 
 For internal converter tools using ``$__target_datatype__`` it is recommended to add a select
 input parameter with name ``__target_datatype__`` in order to make the tool testable, see
 for instance the [biom converter](https://github.com/galaxyproject/galaxy/blob/master/lib/galaxy/datatypes/converters/biom.xml).
@@ -4125,15 +4166,15 @@
 ```xml
 <options from_dataset="input1">
     <column name="name" index="0"/>
     <column name="value" index="0"/>
 </options>
 ```
 
-The [interval2maf](https://github.com/galaxyproject/galaxy/blob/dev/tools/maf/interval2maf.xml)
+The [gff_filter_by_feature_count](tools/filters/gff/gff_filter_by_feature_count.xml)
 tool makes use of this tag with files from a history, and the
 [star_fusion](https://github.com/galaxyproject/tools-iuc/blob/master/tools/star_fusion/star_fusion.xml)
 tool makes use of this to reference a data table.
 ]]></xs:documentation>
     </xs:annotation>
     <xs:attribute name="name" type="xs:string" use="required">
       <xs:annotation>
@@ -4572,18 +4613,18 @@
 * ``param_value`` filter options for which the entry in a given ``column`` of the referenced file based on properties of another input parameter specified by ``ref``. This property is by default the value of the parameter, but also the values of another attribute (``ref_attribute``) of the parameter can be used, e.g. the extension of a data input.
 * ``data_meta`` populate or filter options based on the metadata of another input parameter specified by ``ref``. If a ``column`` is given options are filtered for which the entry in this column ``column`` is equal to metadata of the input parameter specified by ``ref``.
 If no ``column`` is given the metadata value of the referenced input is added to the options list (in this case the corresponding ``options`` tag must not have the ``from_data_table`` or ``from_dataset`` attributes).
 In both cases the desired metadata is selected by ``key``.
 
 The ``static_value`` and ``regexp`` filters can be inverted by setting ``keep`` to true.
 
-* ``add_value``: add an option with a given ``name`` and ``value`` to the options. By default the new option is appended, with ``index`` the insertion position can be specified.
-* ``remove_value``: remove a value from the options. Either specified explicitly with ``value``, the value of another input specifified with ``ref``, or the metatdata ``key`` of another input ``meta_ref``.
+* ``add_value``: add an option with a given ``name`` and ``value`` to the options. By default, the new option is appended, with ``index`` the insertion position can be specified.
+* ``remove_value``: remove a value from the options. Either specified explicitly with ``value``, the value of another input specified with ``ref``, or the metadata ``key`` of another input ``meta_ref``.
 * ``unique_value``: remove options that have duplicate entries in the given ``column``.
-* ``sort_by``: sort options by the entries of a given ``column``.
+* ``sort_by``: sort options by the entries of a given ``column``. If ``reverse_sort_order`` is set to ``true``, reverse sort order from ascending to descending.
 * ``multiple_splitter``: split the entries of the specified ``column``(s) in the referenced file using a ``separator``. Thereby the number of columns is increased.
 
 ### Examples
 
 The following example from Mothur's
 [remove.groups.xml](https://github.com/galaxyproject/tools-iuc/blob/master/tools/mothur/remove.groups.xml)
 tool demonstrates filtering a select list based on the metadata of an input to
@@ -4763,14 +4804,21 @@
     <xs:attribute name="meta_ref" type="xs:string">
       <xs:annotation>
         <xs:documentation xml:lang="en">Only used when ``type`` is
 ``remove_value``. Dataset to look for the value of metadata ``key`` to remove
 from the list.</xs:documentation>
       </xs:annotation>
     </xs:attribute>
+    <xs:attribute name="reverse_sort_order" type="xs:boolean" default="false">
+      <xs:annotation>
+        <xs:documentation xml:lang="en">Used when ``type`` is ``sort_by``, if set to
+        ``true`` it will reverse the sort order from ascending to descending. Default
+        is ``false``.</xs:documentation>
+      </xs:annotation>
+    </xs:attribute>
   </xs:complexType>
   <xs:complexType name="Outputs">
     <xs:annotation>
       <xs:documentation xml:lang="en"><![CDATA[
 Container tag set for the ``<data>`` and ``<collection>`` tag sets.
 The files and collections created by tools as a result of their execution are
 named by Galaxy. You specify the number and type of your output files using the
@@ -5363,14 +5411,19 @@
                 </action>
             </when>
         </conditional>
     </actions>
 </data>
 ```
 
+Note that the value given in ``when`` tags needs to be the python string representation
+of the value of the referred parameter, e.g. ``True`` or ``False`` if the referred
+parameter is a boolean.
+
+
 ### Unconditional Actions and Column Names
 
 For a static file that contains a fixed number of columns, it is straight forward:
 
 ```xml
 <outputs>
     <data format="tabular" name="table">
@@ -5594,15 +5647,16 @@
     </xs:annotation>
     <xs:sequence>
       <xs:group ref="ActionsElement" minOccurs="1" maxOccurs="unbounded"/>
     </xs:sequence>
     <xs:attribute name="value" type="xs:string" use="optional">
       <xs:annotation>
         <xs:documentation xml:lang="en">Value to match conditional input value
-against.</xs:documentation>
+against. This needs to be the python string representation of the parameter value,
+e.g. ``True`` or ``False`` if the referred parameter is a boolean.</xs:documentation>
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="datatype_isinstance" type="xs:string" use="optional">
       <xs:annotation>
         <xs:documentation xml:lang="en">Datatype to match against (if ``value`` is unspecified). This should be the short string describing the format (e.g. ``interval``).</xs:documentation>
       </xs:annotation>
     </xs:attribute>
@@ -6645,14 +6699,39 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="tmpdir_max">
         <xs:annotation>
           <xs:documentation xml:lang="en">Maximum reserved filesystem based storage for the designated temporary directory, in mebibytes (2**20 bytes), if runtime allows it (not yet implemented in Galaxy).</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="cuda_version_min">
+        <xs:annotation>
+          <xs:documentation xml:lang="en">Minimum CUDA (runtime link library) runtime version, if runtime allows it (not yet implemented in Galaxy).</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="cuda_compute_capability">
+        <xs:annotation>
+          <xs:documentation xml:lang="en">Minimum NVIDIA (hardware+driver) Compute capabilities (major, minor (can be a range or a list), if runtime allows it (not yet implemented in Galaxy).</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="gpu_memory_min">
+        <xs:annotation>
+          <xs:documentation xml:lang="en">Minimum Memory of the GPU in mebibytes, if runtime allows it (not yet implemented in Galaxy).</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="cuda_device_count_min">
+        <xs:annotation>
+          <xs:documentation xml:lang="en">Minimum CUDA device count, if runtime allows it (not yet implemented in Galaxy).</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
+      <xs:enumeration value="cuda_device_count_max">
+        <xs:annotation>
+          <xs:documentation xml:lang="en">Maximum CUDA device count, if runtime allows it (not yet implemented in Galaxy).</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
     </xs:restriction>
   </xs:simpleType>
   <xs:simpleType name="ContainerType">
     <xs:annotation>
       <xs:documentation xml:lang="en">Type of container for tool execution.</xs:documentation>
     </xs:annotation>
     <xs:restriction base="xs:string">
@@ -6831,15 +6910,15 @@
     </xs:restriction>
   </xs:simpleType>
   <xs:simpleType name="TestOutputCompareType">
     <xs:annotation>
       <xs:documentation xml:lang="en">Type of comparison to use when comparing
 test generated output files to expected output files. Currently valid value are
 ``diff`` (the default), ``re_match``, ``re_match_multiline``,
-and ``contains``. In addtion there is ``sim_size`` which is discouraged in fafour of a ``has_size`` assertion.</xs:documentation>
+and ``contains``. In addition there is ``sim_size`` which is discouraged in favour of a ``has_size`` assertion.</xs:documentation>
     </xs:annotation>
     <xs:restriction base="xs:string">
       <xs:enumeration value="diff"/>
       <xs:enumeration value="re_match"/>
       <xs:enumeration value="sim_size"/>
       <xs:enumeration value="re_match_multiline"/>
       <xs:enumeration value="contains"/>
@@ -6858,15 +6937,15 @@
       <xs:enumeration value="False"/>
       <xs:enumeration value="yes"/>
       <xs:enumeration value="no"/>
     </xs:restriction>
   </xs:simpleType>
   <xs:simpleType name="Bytes">
     <xs:annotation>
-      <xs:documentation xml:lang="en">Number of bytes alowing for suffix (k|K|M|G|P|E)i?</xs:documentation>
+      <xs:documentation xml:lang="en">Number of bytes allowing for suffix (k|K|M|G|P|E)i?</xs:documentation>
     </xs:annotation>
     <xs:restriction base="xs:string">
       <xs:pattern value="(0|[1-9][0-9]*)([kKMGTPE]i?)?"/>
     </xs:restriction>
   </xs:simpleType>
   <xs:complexType name="EdamTopics">
     <xs:annotation>
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy_tool_util.egg-info/PKG-INFO` & `galaxy-tool-util-23.0.1/galaxy_tool_util.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-tool-util
-Version: 22.5.0.dev3
+Version: 23.0.1
 Summary: Galaxy tool and tool dependency utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: cwl
 Provides-Extra: mulled
@@ -34,123 +35,145 @@
 
 
 Overview
 --------
 
 The Galaxy_ tool utilities.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy/tree/dev/packages/tool_util
 
 .. _Galaxy: http://galaxyproject.org/
 
 History
 -------
 
 .. to_doc
 
 -------------------
-22.5.0.dev0
+23.0.1 (2023-06-08)
 -------------------
 
 
+=========
+Bug fixes
+=========
+
+* Fix assertion linting to not fail on byte suffixes by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15873 <https://github.com/galaxyproject/galaxy/pull/15873>`_
+* Fix ``get_test_from_anaconda()`` and ``base_image_for_targets()`` functions by `@nsoranzo <https://github.com/nsoranzo>`_ in `#16125 <https://github.com/galaxyproject/galaxy/pull/16125>`_
+* Fix test search for mulled container hashes by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16170 <https://github.com/galaxyproject/galaxy/pull/16170>`_
+
+============
+Enhancements
+============
+
+* Allow setting auto_decompress property in staging interface by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16014 <https://github.com/galaxyproject/galaxy/pull/16014>`_
 
 -------------------
 22.1.5 (2022-11-14)
 -------------------
 
 * Set test status to success on expected failure
 
+-------------------
 22.1.4 (2022-10-28)
 -------------------
 
 * Add missing unittest_utils package to galaxy-tool-util
 
+-------------------
 22.1.3 (2022-10-27)
 -------------------
 
 * Pin minimum pyopenssl version when installing Conda
 * Add ``--strict-channel-priority`` to conda create/install commands if using conda >=4.7.5
 
+-------------------
 22.1.2 (2022-08-29)
 -------------------
 
 * Fix lint context error level
 * Pin galaxy-util to >= 22.1
 * Fix biocontainer resolution without beaker cache
 
+-------------------
 22.1.1 (2022-08-22)
---------------------
+-------------------
 
 * First release from the 22.01 branch of Galaxy
 
----------------------
+-------------------
 21.9.2 (2021-11-23)
----------------------
+-------------------
 
 * Fix linting of ``multiple="true"`` select inputs.
 
----------------------
+-------------------
 21.9.1 (2021-11-03)
----------------------
+-------------------
 
 * Fix tool linting.
 
----------------------
+-------------------
 21.9.0 (2021-11-03)
----------------------
+-------------------
 
 * First release from the 21.09 branch of Galaxy.
 
----------------------
+-------------------
 21.1.2 (2021-06-23)
----------------------
+-------------------
 
 
 
----------------------
+-------------------
 21.1.1 (2021-05-21)
----------------------
+-------------------
 
 
 
----------------------
+-------------------
 21.1.0 (2021-03-19)
----------------------
+-------------------
 
 * First release from the 21.01 branch of Galaxy.
 
----------------------
+-------------------
 20.9.1 (2020-10-28)
----------------------
+-------------------
 
 * Bugfixes to work around & annotate expected tool test failures.
 
----------------------
-20.9.0.dev2
----------------------
+-------------------
+20.9.0 (2020-10-28)
+-------------------
+
+* First release from the 20.09 branch of Galaxy.
+
+------------------------
+20.9.0.dev2 (2020-08-02)
+------------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.05 branch of Galaxy.
 
----------------------
+-------------------
 20.1.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.01 branch of Galaxy.
 
----------------------
+-------------------
 19.9.1 (2019-12-28)
----------------------
+-------------------
 
 * Fix declared dependency problem with package.
 
----------------------
+-------------------
 19.9.0 (2019-12-16)
----------------------
+-------------------
 
 * Initial import from dev branch of Galaxy during 19.09 development cycle.
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy_tool_util.egg-info/SOURCES.txt` & `galaxy-tool-util-23.0.1/galaxy_tool_util.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 MANIFEST.in
 README.rst
 dev-requirements.txt
 pyproject.toml
 setup.cfg
 test-requirements.txt
 galaxy/__init__.py
+galaxy/py.typed
 galaxy/tool_util/__init__.py
 galaxy/tool_util/edam_util.py
 galaxy/tool_util/fetcher.py
 galaxy/tool_util/lint.py
 galaxy/tool_util/loader.py
 galaxy/tool_util/loader_directory.py
 galaxy/tool_util/output_checker.py
@@ -24,14 +25,16 @@
 galaxy/tool_util/cwl/cwltool_deps.py
 galaxy/tool_util/cwl/parser.py
 galaxy/tool_util/cwl/representation.py
 galaxy/tool_util/cwl/runnable.py
 galaxy/tool_util/cwl/runtime_actions.py
 galaxy/tool_util/cwl/schema.py
 galaxy/tool_util/cwl/util.py
+galaxy/tool_util/data/__init__.py
+galaxy/tool_util/data/_schema.py
 galaxy/tool_util/deps/__init__.py
 galaxy/tool_util/deps/brew_exts.py
 galaxy/tool_util/deps/brew_util.py
 galaxy/tool_util/deps/commands.py
 galaxy/tool_util/deps/conda_compat.py
 galaxy/tool_util/deps/conda_util.py
 galaxy/tool_util/deps/container_classes.py
@@ -118,14 +121,15 @@
 galaxy/tool_util/toolbox/views/__init__.py
 galaxy/tool_util/toolbox/views/definitions.py
 galaxy/tool_util/toolbox/views/edam.py
 galaxy/tool_util/toolbox/views/interface.py
 galaxy/tool_util/toolbox/views/sources.py
 galaxy/tool_util/toolbox/views/static.py
 galaxy/tool_util/unittest_utils/__init__.py
+galaxy/tool_util/unittest_utils/interactor.py
 galaxy/tool_util/unittest_utils/sample_data.py
 galaxy/tool_util/verify/__init__.py
 galaxy/tool_util/verify/interactor.py
 galaxy/tool_util/verify/script.py
 galaxy/tool_util/verify/test_config.sample.yml
 galaxy/tool_util/verify/test_data.py
 galaxy/tool_util/verify/wait.py
```

### Comparing `galaxy-tool-util-22.5.0.dev3/galaxy_tool_util.egg-info/entry_points.txt` & `galaxy-tool-util-23.0.1/galaxy_tool_util.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-22.5.0.dev3/setup.cfg` & `galaxy-tool-util-23.0.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -9,39 +9,41 @@
 	Natural Language :: English
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy tool and tool dependency utilities
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-tool-util
 url = https://github.com/galaxyproject/galaxy
-version = 22.5.0.dev3
+version = 23.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util>=22.1
 	conda-package-streaming
 	lxml
 	MarkupSafe
 	packaging<22
 	pydantic
 	PyYAML
+	requests
 	sortedcontainers
 	typing-extensions
 packages = find:
 python_requires = >=3.7
 
 [options.entry_points]
 console_scripts = 
@@ -53,15 +55,15 @@
 	mulled-hash = galaxy.tool_util.deps.mulled.mulled_hash:main
 	mulled-list = galaxy.tool_util.deps.mulled.mulled_list:main
 	mulled-search = galaxy.tool_util.deps.mulled.mulled_search:main
 	mulled-update-singularity-containers = galaxy.tool_util.deps.mulled.mulled_update_singularity_containers:main
 
 [options.extras_require]
 cwl = 
-	cwltool==3.1.20211107152837
+	cwltool==3.1.20221109155812
 mulled = 
 	jinja2
 	Whoosh
 edam = 
 	edam-ontology
 
 [options.packages.find]
```

