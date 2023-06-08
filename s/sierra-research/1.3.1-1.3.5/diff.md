# Comparing `tmp/sierra-research-1.3.1.tar.gz` & `tmp/sierra-research-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sierra-research-1.3.1.tar", last modified: Wed Jan 25 20:42:52 2023, max compression
+gzip compressed data, was "sierra-research-1.3.5.tar", last modified: Thu Jun  8 03:06:36 2023, max compression
```

## Comparing `sierra-research-1.3.1.tar` & `sierra-research-1.3.5.tar`

### file list

```diff
@@ -1,317 +1,317 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.174615 sierra-research-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.coveragerc
--rwxr-xr-x   0 runner    (1001) docker     (123)     1473 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.dir-locals.el
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.134615 sierra-research-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.134615 sierra-research-1.3.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.142615 sierra-research-1.3.1/.github/actions/publish/
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.github/actions/publish/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.142615 sierra-research-1.3.1/.github/actions/sample-project-setup/
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.github/actions/sample-project-setup/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.142615 sierra-research-1.3.1/.github/actions/sierra-setup/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.github/actions/sierra-setup/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.142615 sierra-research-1.3.1/.github/actions/slurm-setup/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.github/actions/slurm-setup/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.142615 sierra-research-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.github/workflows/argos.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.github/workflows/exec-env-plugins.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.github/workflows/integration-all.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.github/workflows/ros1gazebo.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.github/workflows/ros1robot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.github/workflows/sierra-core.yml
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.github/workflows/static-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.github/workflows/unit-tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1252 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)       39 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.projectile
--rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.pylintrc
--rwxr-xr-x   0 runner    (1001) docker     (123)      681 2023-01-25 20:39:53.000000 sierra-research-1.3.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-01-25 20:39:53.000000 sierra-research-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-01-25 20:42:52.170616 sierra-research-1.3.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    14452 2023-01-25 20:39:53.000000 sierra-research-1.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.142615 sierra-research-1.3.1/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.134615 sierra-research-1.3.1/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.146615 sierra-research-1.3.1/docs/_build/man/
--rw-r--r--   0 runner    (1001) docker     (123)    54227 2023-01-25 20:42:23.000000 sierra-research-1.3.1/docs/_build/man/sierra-cli.1
--rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-01-25 20:42:23.000000 sierra-research-1.3.1/docs/_build/man/sierra-examples.7
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-01-25 20:42:23.000000 sierra-research-1.3.1/docs/_build/man/sierra-exec-envs.7
--rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-01-25 20:42:23.000000 sierra-research-1.3.1/docs/_build/man/sierra-glossary.7
--rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-01-25 20:42:23.000000 sierra-research-1.3.1/docs/_build/man/sierra-platforms.7
--rw-r--r--   0 runner    (1001) docker     (123)    24455 2023-01-25 20:42:23.000000 sierra-research-1.3.1/docs/_build/man/sierra-usage.7
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-01-25 20:42:23.000000 sierra-research-1.3.1/docs/_build/man/sierra.7
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.146615 sierra-research-1.3.1/docs/_ext/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1044 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/_ext/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.134615 sierra-research-1.3.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.146615 sierra-research-1.3.1/docs/_templates/autoapi/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1697 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/_templates/autoapi/module.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)    11754 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.146615 sierra-research-1.3.1/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (123)   175198 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/figures/architecture.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2632 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.146615 sierra-research-1.3.1/docs/man/
--rwxr-xr-x   0 runner    (1001) docker     (123)      897 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/man/sierra-cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/man/sierra-examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/man/sierra-exec-envs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/man/sierra-glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/man/sierra-platforms.rst
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/man/sierra-usage.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/man/sierra.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      154 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.146615 sierra-research-1.3.1/docs/src/
--rwxr-xr-x   0 runner    (1001) docker     (123)      156 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/api.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2944 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/contributing.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      725 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/description.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.150615 sierra-research-1.3.1/docs/src/exec_env/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7330 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/exec_env/hpc.rst
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/exec_env/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1284 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/exec_env/robot.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     8755 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/faq.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     7247 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/getting_started.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)    10817 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/matrix.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/packages.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/philosophy.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.150615 sierra-research-1.3.1/docs/src/platform/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.150615 sierra-research-1.3.1/docs/src/platform/argos/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4659 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/platform/argos/batch_criteria.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/platform/argos/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/platform/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.150615 sierra-research-1.3.1/docs/src/platform/ros1gazebo/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/platform/ros1gazebo/batch_criteria.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/platform/ros1gazebo/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.150615 sierra-research-1.3.1/docs/src/platform/ros1robot/
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/platform/ros1robot/batch_criteria.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/platform/ros1robot/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.150615 sierra-research-1.3.1/docs/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/plugins/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16751 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/roadmap.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.150615 sierra-research-1.3.1/docs/src/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/storage/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     8760 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/trial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.150615 sierra-research-1.3.1/docs/src/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.150615 sierra-research-1.3.1/docs/src/tutorials/hpc/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2277 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/hpc/cluster_setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/hpc/local_setup.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.138615 sierra-research-1.3.1/docs/src/tutorials/plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.150615 sierra-research-1.3.1/docs/src/tutorials/plugin/exec_env/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/plugin/exec_env/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/plugin/exec_env/plugin.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.150615 sierra-research-1.3.1/docs/src/tutorials/plugin/platform/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/plugin/platform/cmdline.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/plugin/platform/generators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/plugin/platform/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/plugin/platform/plugin.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.150615 sierra-research-1.3.1/docs/src/tutorials/plugin/storage/
--rwxr-xr-x   0 runner    (1001) docker     (123)      802 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/plugin/storage/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/plugin/storage/plugin.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.150615 sierra-research-1.3.1/docs/src/tutorials/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/project/cmdline.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2964 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/project/generators.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     6370 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/project/graphs_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/project/hooks.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.154615 sierra-research-1.3.1/docs/src/tutorials/project/main_config/
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/project/main_config/controllers.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      496 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/project/main_config/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/project/main_config/main.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/project/main_config/perf.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/project/models.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     5688 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/project/new_bc.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     6362 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/project/project.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/project/stage5_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/tutorials/project/template_input_file.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.154615 sierra-research-1.3.1/docs/src/usage/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/usage/cli-argos.rst
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/usage/cli-core.rst
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/usage/cli-ros1gazebo.rst
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/usage/cli-ros1robot.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      691 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/usage/cli.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4608 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/usage/environment.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16360 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/usage/examples.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      699 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/usage/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4439 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/usage/pipeline.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     6039 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/usage/rendering.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     8617 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/usage/run_time_tree.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/usage/stage5.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      897 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/usage/subprograms.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1795 2023-01-25 20:39:53.000000 sierra-research-1.3.1/docs/src/usage/variables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-01-25 20:39:53.000000 sierra-research-1.3.1/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.154615 sierra-research-1.3.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)    26821 2023-01-25 20:39:53.000000 sierra-research-1.3.1/scripts/argos-integration-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4951 2023-01-25 20:39:53.000000 sierra-research-1.3.1/scripts/core-integration-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     8637 2023-01-25 20:39:53.000000 sierra-research-1.3.1/scripts/ros1gazebo-integration-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4192 2023-01-25 20:39:53.000000 sierra-research-1.3.1/scripts/ros1robot-integration-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-01-25 20:39:53.000000 sierra-research-1.3.1/scripts/slurm-test.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-01-25 20:39:53.000000 sierra-research-1.3.1/scripts/slurm.conf
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 20:42:52.174615 sierra-research-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-01-25 20:39:53.000000 sierra-research-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.154615 sierra-research-1.3.1/sierra/
--rwxr-xr-x   0 runner    (1001) docker     (123)      186 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.158615 sierra-research-1.3.1/sierra/core/
--rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58191 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/cmdline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4557 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.158615 sierra-research-1.3.1/sierra/core/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/experiment/bindings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11458 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/experiment/definition.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/experiment/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/experiment/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.158615 sierra-research-1.3.1/sierra/core/generators/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/generators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      873 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/generators/controller_generator_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15596 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/generators/exp_creator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5574 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/generators/exp_generators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8919 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/generators/generator_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.158615 sierra-research-1.3.1/sierra/core/graphs/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/graphs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12218 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/graphs/heatmap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3685 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/graphs/scatterplot2D.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9057 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/graphs/stacked_line_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8125 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/graphs/stacked_surface_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13573 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/graphs/summary_line_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.158615 sierra-research-1.3.1/sierra/core/hpc/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/hpc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5186 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/hpc/cmdline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      985 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.158615 sierra-research-1.3.1/sierra/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3340 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/models/graphs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6729 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/models/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.162615 sierra-research-1.3.1/sierra/core/pipeline/
--rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7487 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.162615 sierra-research-1.3.1/sierra/core/pipeline/stage1/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage1/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3304 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage1/pipeline_stage1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.162615 sierra-research-1.3.1/sierra/core/pipeline/stage2/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage2/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10718 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage2/exp_runner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage2/pipeline_stage2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.162615 sierra-research-1.3.1/sierra/core/pipeline/stage3/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage3/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5032 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage3/imagizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4572 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage3/pipeline_stage3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12585 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage3/run_collator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18186 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage3/statistics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.162615 sierra-research-1.3.1/sierra/core/pipeline/stage4/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage4/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12042 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage4/graph_collator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9591 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage4/inter_exp_graph_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13814 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage4/intra_exp_graph_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6745 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage4/model_runner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18911 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage4/pipeline_stage4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9385 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage4/rendering.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage4/yaml_config_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.162615 sierra-research-1.3.1/sierra/core/pipeline/stage5/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage5/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14183 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage5/inter_scenario_comparator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43936 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage5/intra_scenario_comparator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10600 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/pipeline/stage5/pipeline_stage5.py
--rw-r--r--   0 runner    (1001) docker     (123)    17359 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12535 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/plugin_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8173 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/root_dirpath_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.162615 sierra-research-1.3.1/sierra/core/ros1/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/ros1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/ros1/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/ros1/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/ros1/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.162615 sierra-research-1.3.1/sierra/core/ros1/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/ros1/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/ros1/variables/exp_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/startup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6030 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/stat_kernels.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/types.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12471 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.166615 sierra-research-1.3.1/sierra/core/variables/
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/variables/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1562 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/variables/base_variable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25747 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/variables/batch_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/variables/exp_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/variables/population_size.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/variables/variable_density.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3843 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/core/vector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6619 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.166615 sierra-research-1.3.1/sierra/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.166615 sierra-research-1.3.1/sierra/plugins/hpc/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/hpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.166615 sierra-research-1.3.1/sierra/plugins/hpc/adhoc/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/hpc/adhoc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4046 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/hpc/adhoc/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.166615 sierra-research-1.3.1/sierra/plugins/hpc/local/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/hpc/local/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2501 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/hpc/local/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.166615 sierra-research-1.3.1/sierra/plugins/hpc/pbs/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/hpc/pbs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3858 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/hpc/pbs/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.166615 sierra-research-1.3.1/sierra/plugins/hpc/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/hpc/slurm/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4164 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/hpc/slurm/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.166615 sierra-research-1.3.1/sierra/plugins/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.166615 sierra-research-1.3.1/sierra/plugins/platform/argos/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/argos/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15855 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/argos/cmdline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.166615 sierra-research-1.3.1/sierra/plugins/platform/argos/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/argos/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15432 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/argos/generators/platform_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13128 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/argos/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.166615 sierra-research-1.3.1/sierra/plugins/platform/argos/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/argos/variables/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6062 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/argos/variables/arena_shape.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9031 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/argos/variables/cameras.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4618 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/argos/variables/constant_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/argos/variables/exp_setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19636 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/argos/variables/physics_engines.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6577 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/argos/variables/population_constant_density.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3539 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/argos/variables/population_size.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4967 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/argos/variables/population_variable_density.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3699 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/argos/variables/rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.170616 sierra-research-1.3.1/sierra/plugins/platform/ros1gazebo/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/ros1gazebo/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9920 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/ros1gazebo/cmdline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.170616 sierra-research-1.3.1/sierra/plugins/platform/ros1gazebo/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/ros1gazebo/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/ros1gazebo/generators/platform_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13097 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/ros1gazebo/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.170616 sierra-research-1.3.1/sierra/plugins/platform/ros1gazebo/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/ros1gazebo/variables/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8463 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/ros1gazebo/variables/population_size.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.170616 sierra-research-1.3.1/sierra/plugins/platform/ros1robot/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/ros1robot/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6972 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/ros1robot/cmdline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.170616 sierra-research-1.3.1/sierra/plugins/platform/ros1robot/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/ros1robot/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/ros1robot/generators/platform_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/ros1robot/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.170616 sierra-research-1.3.1/sierra/plugins/platform/ros1robot/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/ros1robot/variables/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5485 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/platform/ros1robot/variables/population_size.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.170616 sierra-research-1.3.1/sierra/plugins/robot/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/robot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.170616 sierra-research-1.3.1/sierra/plugins/robot/turtlebot3/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/robot/turtlebot3/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/robot/turtlebot3/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.170616 sierra-research-1.3.1/sierra/plugins/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.170616 sierra-research-1.3.1/sierra/plugins/storage/csv/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/storage/csv/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/plugins/storage/csv/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-01-25 20:39:53.000000 sierra-research-1.3.1/sierra/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.170616 sierra-research-1.3.1/sierra_research.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-01-25 20:42:52.000000 sierra-research-1.3.1/sierra_research.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-01-25 20:42:52.000000 sierra-research-1.3.1/sierra_research.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 20:42:52.000000 sierra-research-1.3.1/sierra_research.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-25 20:42:52.000000 sierra-research-1.3.1/sierra_research.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-01-25 20:42:52.000000 sierra-research-1.3.1/sierra_research.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-25 20:42:52.000000 sierra-research-1.3.1/sierra_research.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:42:52.170616 sierra-research-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-01-25 20:39:53.000000 sierra-research-1.3.1/tests/arena_extent_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-01-25 20:39:53.000000 sierra-research-1.3.1/tests/exp_def_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-01-25 20:39:53.000000 sierra-research-1.3.1/tests/test1.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-01-25 20:39:53.000000 sierra-research-1.3.1/tests/vector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-01-25 20:39:53.000000 sierra-research-1.3.1/todo.org
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.coveragerc
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1473 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.dir-locals.el
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.525962 sierra-research-1.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.525962 sierra-research-1.3.5/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.529962 sierra-research-1.3.5/.github/actions/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/actions/publish/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.529962 sierra-research-1.3.5/.github/actions/sample-project-setup/
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/actions/sample-project-setup/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.529962 sierra-research-1.3.5/.github/actions/sierra-setup/
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/actions/sierra-setup/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.529962 sierra-research-1.3.5/.github/actions/slurm-setup/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/actions/slurm-setup/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.533962 sierra-research-1.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/argos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/exec-env-plugins.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/integration-all.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/ros1gazebo.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/ros1robot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/sierra-core.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/static-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.github/workflows/unit-tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1252 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)       39 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.projectile
+-rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.pylintrc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      681 2023-06-08 03:03:32.000000 sierra-research-1.3.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-08 03:03:32.000000 sierra-research-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-06-08 03:06:36.557962 sierra-research-1.3.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14452 2023-06-08 03:03:32.000000 sierra-research-1.3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.533962 sierra-research-1.3.5/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.525962 sierra-research-1.3.5/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.533962 sierra-research-1.3.5/docs/_build/man/
+-rw-r--r--   0 runner    (1001) docker     (123)    54227 2023-06-08 03:06:04.000000 sierra-research-1.3.5/docs/_build/man/sierra-cli.1
+-rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-06-08 03:06:04.000000 sierra-research-1.3.5/docs/_build/man/sierra-examples.7
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-06-08 03:06:04.000000 sierra-research-1.3.5/docs/_build/man/sierra-exec-envs.7
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-06-08 03:06:04.000000 sierra-research-1.3.5/docs/_build/man/sierra-glossary.7
+-rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-06-08 03:06:04.000000 sierra-research-1.3.5/docs/_build/man/sierra-platforms.7
+-rw-r--r--   0 runner    (1001) docker     (123)    24455 2023-06-08 03:06:04.000000 sierra-research-1.3.5/docs/_build/man/sierra-usage.7
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-08 03:06:04.000000 sierra-research-1.3.5/docs/_build/man/sierra.7
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.533962 sierra-research-1.3.5/docs/_ext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1044 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/_ext/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.525962 sierra-research-1.3.5/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.533962 sierra-research-1.3.5/docs/_templates/autoapi/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1697 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/_templates/autoapi/module.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.533962 sierra-research-1.3.5/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)   175198 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/figures/architecture.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2632 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.533962 sierra-research-1.3.5/docs/man/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      897 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/man/sierra-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/man/sierra-examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/man/sierra-exec-envs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/man/sierra-glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/man/sierra-platforms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/man/sierra-usage.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/man/sierra.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      154 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      156 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2996 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/contributing.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      725 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/description.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/exec_env/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7330 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/exec_env/hpc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/exec_env/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1284 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/exec_env/robot.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8755 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/faq.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7274 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/getting_started.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10817 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/matrix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/packages.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/philosophy.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/platform/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/platform/argos/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4659 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/platform/argos/batch_criteria.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/platform/argos/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/platform/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/platform/ros1gazebo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/platform/ros1gazebo/batch_criteria.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/platform/ros1gazebo/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/platform/ros1robot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/platform/ros1robot/batch_criteria.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/platform/ros1robot/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/plugins/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/roadmap.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/storage/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8787 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/trial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/tutorials/hpc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2277 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/hpc/cluster_setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/hpc/local_setup.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.525962 sierra-research-1.3.5/docs/src/tutorials/plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/tutorials/plugin/exec_env/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/exec_env/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/exec_env/plugin.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/tutorials/plugin/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/platform/cmdline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/platform/generators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/platform/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/platform/plugin.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.537962 sierra-research-1.3.5/docs/src/tutorials/plugin/storage/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      802 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/storage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/plugin/storage/plugin.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.541962 sierra-research-1.3.5/docs/src/tutorials/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/cmdline.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2964 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/generators.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6370 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/graphs_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/hooks.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.541962 sierra-research-1.3.5/docs/src/tutorials/project/main_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/main_config/controllers.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      496 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/main_config/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/main_config/main.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/main_config/perf.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3955 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/models.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5688 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/new_bc.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6362 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/stage5_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/tutorials/project/template_input_file.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.541962 sierra-research-1.3.5/docs/src/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/cli-argos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/cli-core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/cli-ros1gazebo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/cli-ros1robot.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      691 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/cli.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4608 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/environment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16360 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/examples.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      699 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4439 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/pipeline.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6039 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/rendering.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8617 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/run_time_tree.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/stage5.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      897 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/subprograms.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1795 2023-06-08 03:03:32.000000 sierra-research-1.3.5/docs/src/usage/variables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-08 03:03:32.000000 sierra-research-1.3.5/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.541962 sierra-research-1.3.5/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26821 2023-06-08 03:03:32.000000 sierra-research-1.3.5/scripts/argos-integration-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4951 2023-06-08 03:03:32.000000 sierra-research-1.3.5/scripts/core-integration-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8637 2023-06-08 03:03:32.000000 sierra-research-1.3.5/scripts/ros1gazebo-integration-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4192 2023-06-08 03:03:32.000000 sierra-research-1.3.5/scripts/ros1robot-integration-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-08 03:03:32.000000 sierra-research-1.3.5/scripts/slurm-test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-08 03:03:32.000000 sierra-research-1.3.5/scripts/slurm.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 03:06:36.557962 sierra-research-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-08 03:03:32.000000 sierra-research-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.541962 sierra-research-1.3.5/sierra/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      186 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.545962 sierra-research-1.3.5/sierra/core/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58191 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/cmdline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4557 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.545962 sierra-research-1.3.5/sierra/core/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/experiment/bindings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11458 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/experiment/definition.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/experiment/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/experiment/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.545962 sierra-research-1.3.5/sierra/core/generators/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/generators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      873 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/generators/controller_generator_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15596 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/generators/exp_creator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5574 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/generators/exp_generators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8919 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/generators/generator_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.545962 sierra-research-1.3.5/sierra/core/graphs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/graphs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12218 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/graphs/heatmap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3685 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/graphs/scatterplot2D.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9125 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/graphs/stacked_line_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8125 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/graphs/stacked_surface_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13573 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/graphs/summary_line_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.545962 sierra-research-1.3.5/sierra/core/hpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/hpc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5186 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/hpc/cmdline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      985 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.545962 sierra-research-1.3.5/sierra/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3330 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/models/graphs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6729 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/models/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.545962 sierra-research-1.3.5/sierra/core/pipeline/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7487 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/pipeline/stage1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage1/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3304 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage1/pipeline_stage1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/pipeline/stage2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage2/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10734 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage2/exp_runner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage2/pipeline_stage2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/pipeline/stage3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage3/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5094 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage3/imagizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4572 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage3/pipeline_stage3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12585 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage3/run_collator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18186 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage3/statistics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/pipeline/stage4/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12042 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/graph_collator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9591 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/inter_exp_graph_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13814 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/intra_exp_graph_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6745 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/model_runner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18911 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/pipeline_stage4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9385 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/rendering.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage4/yaml_config_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/pipeline/stage5/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage5/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14183 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage5/inter_scenario_comparator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43936 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage5/intra_scenario_comparator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10600 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/pipeline/stage5/pipeline_stage5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17359 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12535 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/plugin_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8173 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/root_dirpath_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/ros1/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/ros1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/ros1/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/ros1/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/ros1/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/ros1/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/ros1/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/ros1/variables/exp_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/startup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6030 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/stat_kernels.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/types.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12471 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/core/variables/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/variables/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1562 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/variables/base_variable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25747 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/variables/batch_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/variables/exp_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/variables/population_size.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/variables/variable_density.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3843 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/core/vector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6618 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.549962 sierra-research-1.3.5/sierra/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/hpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/hpc/adhoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/adhoc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4046 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/adhoc/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/hpc/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/local/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2501 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/local/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/hpc/pbs/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/pbs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3858 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/pbs/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/hpc/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/slurm/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4164 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/hpc/slurm/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/platform/argos/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15855 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/cmdline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/platform/argos/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15432 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/generators/platform_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13128 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6062 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/arena_shape.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9031 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/cameras.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4618 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/constant_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/exp_setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19636 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/physics_engines.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6577 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/population_constant_density.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3539 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/population_size.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4967 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/population_variable_density.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3699 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/argos/variables/rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.553962 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9920 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/cmdline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/generators/platform_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13097 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/variables/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8463 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/variables/population_size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6972 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/cmdline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/generators/platform_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/variables/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5485 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/platform/ros1robot/variables/population_size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/robot/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/robot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/robot/turtlebot3/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/robot/turtlebot3/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/robot/turtlebot3/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra/plugins/storage/csv/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/storage/csv/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/plugins/storage/csv/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 03:03:32.000000 sierra-research-1.3.5/sierra/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/sierra_research.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-06-08 03:06:36.000000 sierra-research-1.3.5/sierra_research.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-08 03:06:36.000000 sierra-research-1.3.5/sierra_research.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 03:06:36.000000 sierra-research-1.3.5/sierra_research.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 03:06:36.000000 sierra-research-1.3.5/sierra_research.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-08 03:06:36.000000 sierra-research-1.3.5/sierra_research.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 03:06:36.000000 sierra-research-1.3.5/sierra_research.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:06:36.557962 sierra-research-1.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-08 03:03:32.000000 sierra-research-1.3.5/tests/arena_extent_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-08 03:03:32.000000 sierra-research-1.3.5/tests/exp_def_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-06-08 03:03:32.000000 sierra-research-1.3.5/tests/test1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-08 03:03:32.000000 sierra-research-1.3.5/tests/vector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-06-08 03:03:32.000000 sierra-research-1.3.5/todo.org
```

### Comparing `sierra-research-1.3.1/.dir-locals.el` & `sierra-research-1.3.5/.dir-locals.el`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/.github/actions/publish/action.yml` & `sierra-research-1.3.5/.github/actions/publish/action.yml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
       shell: bash
       run: |
         python3 -m build
 
     - name: Set tag
       if: github.ref == 'refs/heads/devel'
       shell: bash
-      run: echo "RELEASE_TAG=v$(python3 setup.py --version).beta" >> $GITHUB_ENV
+      run: echo "RELEASE_TAG=$(python3 setup.py --version).beta" >> $GITHUB_ENV
 
     - name: Github beta release
       if: github.ref == 'refs/heads/devel'
       uses: "marvinpinto/action-automatic-releases@latest"
       with:
         repo_token: "${{ inputs.github-token }}"
         automatic_release_tag: ${{ env.RELEASE_TAG }}
@@ -41,15 +41,15 @@
         user: __token__
         password: ${{ inputs.testpypi-token }}
         repository_url: https://test.pypi.org/legacy/
 
     - name: Set tag
       if: github.ref == 'refs/heads/master'
       shell: bash
-      run: echo "RELEASE_TAG=v$(python3 setup.py --version)" >> $GITHUB_ENV
+      run: echo "RELEASE_TAG=$(python3 setup.py --version)" >> $GITHUB_ENV
 
     - name: Github release
       if: github.ref == 'refs/heads/master'
       uses: "marvinpinto/action-automatic-releases@latest"
       with:
         repo_token: "${{ inputs.github-token }}"
         automatic_release_tag: ${{ env.RELEASE_TAG }}
```

### Comparing `sierra-research-1.3.1/.github/actions/sample-project-setup/action.yml` & `sierra-research-1.3.5/.github/actions/sample-project-setup/action.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/.github/actions/sierra-setup/action.yml` & `sierra-research-1.3.5/.github/actions/sierra-setup/action.yml`

 * *Files 23% similar despite different names*

```diff
@@ -17,34 +17,14 @@
     ############################################################################
     - name: Setup python (ubuntu)
       uses: actions/setup-python@v4
       if: runner.os == 'Linux'
       with:
         python-version: ${{ matrix.python-version }}
 
-    # - uses: Setup python (ubuntu)
-    #   if: runner.os == 'Linux'
-    #   shell: bash
-    #   run: |
-    #     # apt fails randomly on microsoft's azure servers...
-    #     sudo sed -i 's/azure\.//' /etc/apt/sources.list
-    #     sudo add-apt-repository -y ppa:deadsnakes/ppa
-
-    #     sudo apt-get update
-
-    #     sudo apt-get install python${{ matrix.python-version }} python${{ matrix.python-version }}-dev
-    #     sudo apt-get install python${{ matrix.python-version }}-venv python3-apt
-    #     sudo apt-get install python3-pip python3-cairo intltool python3-wheel strace
-    #     sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python${{ matrix.python-version }} 1
-
-    #     # HACK HACK HACK!
-    #     sudo ln -s /usr/lib/python3/dist-packages/apt_pkg.cpython-38-x86_64-linux-gnu.so  /usr/lib/python3/dist-packages/apt_pkg.so
-    #     sudo ln -s /usr/lib/python3/dist-packages/netifaces.cpython-38-x86_64-linux-gnu.so  /usr/lib/python3/dist-packages/netifaces.so
-
-
     - name: Install system deps (ubuntu)
       if: runner.os == 'Linux'
       shell: bash
       run: |
         sudo apt-get update
         sudo apt-get install parallel cm-super texlive-fonts-recommended
         sudo apt-get install texlive-latex-extra dvipng pssh ffmpeg xvfb
@@ -57,26 +37,30 @@
 
     - name: Setup python (OSX)
       uses: actions/setup-python@v4
       if: runner.os == 'macOS'
       with:
         python-version: ${{ matrix.python-version }}
 
-    - name: Install system deps (OSX)
-      shell: bash
+    - uses: nick-fields/retry@v2
+      name: Install system deps (OSX)
       if: runner.os == 'macOS'
-      run: |
-        # 2023/01/16: || true needed because homebrew installation of whatever
-        # dependencies these packages requires manual intervention to fix, and I
-        # don't have a mac.
-        brew install parallel pssh ffmpeg || true
-        brew install --cask mactex || true
-        brew install --cask xquartz || true
-        python -m pip install --upgrade pip
-        python -m pip install wheel
+      with:
+        timeout_minutes: 10000
+        max_attempts: 3
+        shell: bash
+        command: |
+          # 2023/01/16: || true needed because homebrew installation of whatever
+          # dependencies these packages requires manual intervention to fix, and I
+          # don't have a mac.
+          brew update && brew install parallel pssh ffmpeg
+          brew update && brew install --cask mactex
+          brew update && brew install --cask xquartz
+          python -m pip install --upgrade pip
+          python -m pip install wheel
 
     ############################################################################
     # SIERRA install
     ############################################################################
     - name: Install SIERRA
       shell: bash
       run: |
```

### Comparing `sierra-research-1.3.1/.github/actions/slurm-setup/action.yml` & `sierra-research-1.3.5/.github/actions/slurm-setup/action.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/.github/workflows/argos.yml` & `sierra-research-1.3.5/.github/workflows/argos.yml`

 * *Files 14% similar despite different names*

```diff
@@ -20,18 +20,21 @@
     steps:
       - uses: actions/checkout@v3
       - uses: ./.github/actions/sierra-setup
       - uses: ./.github/actions/sample-project-setup
         with:
           platform: argos
 
-      - name: Integration tests
-        shell: bash
-        run: |
-          ./scripts/argos-integration-tests.sh -f bc_univar_sanity_test
+      - uses: nick-fields/retry@v2
+        name: Integration tests
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/argos-integration-tests.sh -f bc_univar_sanity_test
 
       - uses: actions/upload-artifact@v3
         with:
           name: ci-platform-argos-bc-univar-sanity-${{ runner.os }}-${{ matrix.python-version }}-coverage
           path: .coverage.*
 
   physics-engines:
@@ -45,18 +48,21 @@
     steps:
       - uses: actions/checkout@v3
       - uses: ./.github/actions/sierra-setup
       - uses: ./.github/actions/sample-project-setup
         with:
           platform: argos
 
-      - name: Integration tests
-        shell: bash
-        run: |
-          ./scripts/argos-integration-tests.sh -f physics_engines_test
+      - uses: nick-fields/retry@v2
+        name: Integration tests
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/argos-integration-tests.sh -f physics_engines_test
 
       - uses: actions/upload-artifact@v3
         with:
           name: ci-platform-argos-physics-engines-${{ runner.os }}-${{ matrix.python-version }}-coverage
           path: .coverage.*
 
   stage1-univar:
@@ -69,18 +75,21 @@
     steps:
       - uses: actions/checkout@v3
       - uses: ./.github/actions/sierra-setup
       - uses: ./.github/actions/sample-project-setup
         with:
           platform: argos
 
-      - name: Integration tests
-        shell: bash
-        run: |
-          ./scripts/argos-integration-tests.sh -f stage1_univar_test
+      - uses: nick-fields/retry@v2
+        name: Integration tests
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/argos-integration-tests.sh -f stage1_univar_test
 
       - uses: actions/upload-artifact@v3
         with:
           name: ci-platform-argos-stage1-${{ runner.os }}-${{ matrix.python-version }}-coverage
           path: .coverage.*
 
   stage2-univar:
@@ -93,18 +102,21 @@
     steps:
       - uses: actions/checkout@v3
       - uses: ./.github/actions/sierra-setup
       - uses: ./.github/actions/sample-project-setup
         with:
           platform: argos
 
-      - name: Integration tests
-        shell: bash
-        run: |
-          ./scripts/argos-integration-tests.sh -f stage2_univar_test -e hpc.local
+      - uses: nick-fields/retry@v2
+        name: Integration tests
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/argos-integration-tests.sh -f stage2_univar_test -e hpc.local
 
       - uses: actions/upload-artifact@v3
         with:
           name: ci-platform-argos-stage2-${{ runner.os }}-${{ matrix.python-version }}-coverage
           path: .coverage.*
 
 
@@ -119,18 +131,21 @@
     steps:
       - uses: actions/checkout@v3
       - uses: ./.github/actions/sierra-setup
       - uses: ./.github/actions/sample-project-setup
         with:
           platform: argos
 
-      - name: Integration tests
-        shell: bash
-        run: |
-          ./scripts/argos-integration-tests.sh -f vc_test
+      - uses: nick-fields/retry@v2
+        name: Integration tests
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/argos-integration-tests.sh -f vc_test
 
       - uses: actions/upload-artifact@v3
         with:
           name: ci-platform-argos-vc-${{ runner.os }}-${{ matrix.python-version }}-coverage
           path: .coverage.*
 
   cmdline:
@@ -144,16 +159,19 @@
     steps:
       - uses: actions/checkout@v3
       - uses: ./.github/actions/sierra-setup
       - uses: ./.github/actions/sample-project-setup
         with:
           platform: argos
 
-      - name: Integration tests
-        shell: bash
-        run: |
-          ./scripts/argos-integration-tests.sh -f cmdline_test
+      - uses: nick-fields/retry@v2
+        name: Integration tests
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/argos-integration-tests.sh -f cmdline_test
 
       - uses: actions/upload-artifact@v3
         with:
           name: ci-platform-argos-cmdline-${{ runner.os }}-${{ matrix.python-version }}-coverage
           path: .coverage.*
```

### Comparing `sierra-research-1.3.1/.github/workflows/coverage.yml` & `sierra-research-1.3.5/.github/workflows/coverage.yml`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 on:
   push:
     paths:
       - 'sierra/**'
   schedule:
     - cron: '0 0 1 * *'
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 jobs:
   argos-ci:
     uses: ./.github/workflows/argos.yml
     secrets: inherit
     with:
       os: ubuntu-20.04
```

### Comparing `sierra-research-1.3.1/.github/workflows/exec-env-plugins.yml` & `sierra-research-1.3.5/.github/workflows/exec-env-plugins.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 
   # push:
   #   branches:
   #     # - master
   #     # - devel
   #   paths:
   #     - 'sierra/**'
-
 jobs:
-
   adhoc:
     runs-on: ${{ inputs.os }}
     strategy:
       matrix:
         # You CANNOT use python 3.9 with ubuntu 20.04 with ROS, because 3.8 is
         # the system python and things just don't work otherwise...
         python-version:
```

### Comparing `sierra-research-1.3.1/.github/workflows/integration-all.yml` & `sierra-research-1.3.5/.github/workflows/integration-all.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/.github/workflows/ros1gazebo.yml` & `sierra-research-1.3.5/.github/workflows/ros1gazebo.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/.github/workflows/ros1robot.yml` & `sierra-research-1.3.5/.github/workflows/ros1robot.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/.github/workflows/sierra-core.yml` & `sierra-research-1.3.5/.github/workflows/sierra-core.yml`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,14 @@
   workflow_call:
     inputs:
       os:
         required: True
         type: string
 
 jobs:
-
   cmdline-opts:
     runs-on: ${{ inputs.os }}
     strategy:
       matrix:
         python-version:
           - 3.8
           - 3.9
@@ -20,17 +19,21 @@
     steps:
       - uses: actions/checkout@v3
       - uses: ./.github/actions/sierra-setup
       - uses: ./.github/actions/sample-project-setup
         with:
           platform: argos
 
-      - name: Cmdline Options
-        run: |
-          ./scripts/core-integration-tests.sh -f cmdline_opts_test
+      - uses: nick-fields/retry@v2
+        name: Cmdline options
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/core-integration-tests.sh -f cmdline_opts_test
 
       - uses: actions/upload-artifact@v3
         with:
           name: ci-core-cmdline-opts-${{ runner.os }}-${{ matrix.python-version }}-coverage
           path: .coverage.*
 
   env-vars:
@@ -44,17 +47,21 @@
     steps:
       - uses: actions/checkout@v3
       - uses: ./.github/actions/sierra-setup
       - uses: ./.github/actions/sample-project-setup
         with:
           platform: argos
 
-      - name: Environment variables
-        run: |
-          ./scripts/core-integration-tests.sh -f env_vars_test
+      - uses: nick-fields/retry@v2
+        name: Environment variables
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/core-integration-tests.sh -f env_vars_test
 
       - uses: actions/upload-artifact@v3
         with:
           name: ci-core-env-vars-${{ runner.os }}-${{ matrix.python-version }}-coverage
           path: .coverage.*
 
   bc-bivar-sanity:
@@ -74,22 +81,30 @@
 
       - uses: ./.github/actions/sample-project-setup
         if: runner.os == 'Linux'
         with:
           platform: ros1gazebo
           rosdistro: noetic
 
-      - name: Bivariate batch criteria sanity (ARGoS)
-        run: |
-          ./scripts/argos-integration-tests.sh -f bc_bivar_sanity_test
+      - uses: nick-fields/retry@v2
+        name: Bivariate batch criteria sanity (ARGoS)
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/argos-integration-tests.sh -f bc_bivar_sanity_test
 
-      - name: Bivariate batch criteria sanity (ROS1+Gazebo)
+      - uses: nick-fields/retry@v2
         if: runner.os == 'Linux'
-        run: |
-          ./scripts/ros1gazebo-integration-tests.sh -f bc_bivar_sanity_test
+        name: Bivariate batch criteria sanity (ROS1+Gazebo)
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/ros1gazebo-integration-tests.sh -f bc_bivar_sanity_test
 
       - uses: actions/upload-artifact@v3
         with:
           name: ci-core-bc-bivar-sanity-${{ runner.os }}-${{ matrix.python-version }}-coverage
           path: .coverage.*
 
   stage1-bivar:
@@ -109,22 +124,30 @@
 
       - uses: ./.github/actions/sample-project-setup
         if: runner.os == 'Linux'
         with:
           platform: ros1gazebo
           rosdistro: noetic
 
-      - name: Bivariate batch criteria stage 1 (ARGoS)
-        run: |
-          ./scripts/argos-integration-tests.sh -f stage1_bivar_test
+      - uses: nick-fields/retry@v2
+        name: Bivariate batch criteria stage 1 (ARGoS)
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/argos-integration-tests.sh -f stage1_bivar_test
 
-      - name: Bivariate batch criteria stage 1 (ROS1+Gazebo)
+      - uses: nick-fields/retry@v2
         if: runner.os == 'Linux'
-        run: |
-          ./scripts/ros1gazebo-integration-tests.sh -f stage1_bivar_test
+        name: Bivariate batch criteria stage 1 (ROS1+Gazebo)
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/ros1gazebo-integration-tests.sh -f stage1_bivar_test
 
       - uses: actions/upload-artifact@v3
         with:
           name: ci-core-stage1-bivar-${{ runner.os }}-${{ matrix.python-version }}-coverage
           path: .coverage.*
 
   stage3-univar:
@@ -137,18 +160,21 @@
     steps:
       - uses: actions/checkout@v3
       - uses: ./.github/actions/sierra-setup
       - uses: ./.github/actions/sample-project-setup
         with:
           platform: argos
 
-      - name: Integration tests
-        shell: bash
-        run: |
-          ./scripts/argos-integration-tests.sh -f stage3_univar_test
+      - uses: nick-fields/retry@v2
+        name: Stage3 univariate tests
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/argos-integration-tests.sh -f stage3_univar_test
 
       - uses: actions/upload-artifact@v3
         with:
           name: ci-core-stage3-univar-${{ runner.os }}-${{ matrix.python-version }}-coverage
           path: .coverage.*
 
   stage3-bivar:
@@ -161,18 +187,21 @@
     steps:
       - uses: actions/checkout@v3
       - uses: ./.github/actions/sierra-setup
       - uses: ./.github/actions/sample-project-setup
         with:
           platform: argos
 
-      - name: Integration tests
-        shell: bash
-        run: |
-          ./scripts/argos-integration-tests.sh -f stage3_bivar_test
+      - uses: nick-fields/retry@v2
+        name: Stage3 bivariate tests
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/argos-integration-tests.sh -f stage3_bivar_test
 
       - uses: actions/upload-artifact@v3
         with:
           name: ci-core-stage3-univar-${{ runner.os }}-${{ matrix.python-version }}-coverage
           path: .coverage.*
 
   stage4-univar:
@@ -185,18 +214,21 @@
     steps:
       - uses: actions/checkout@v3
       - uses: ./.github/actions/sierra-setup
       - uses: ./.github/actions/sample-project-setup
         with:
           platform: argos
 
-      - name: Integration tests
-        shell: bash
-        run: |
-          ./scripts/argos-integration-tests.sh -f stage4_univar_test
+      - uses: nick-fields/retry@v2
+        name: Stage4 univariate tests
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/argos-integration-tests.sh -f stage4_univar_test
 
       - uses: actions/upload-artifact@v3
         with:
           name: ci-core-stage4-univar-${{ runner.os }}-${{ matrix.python-version }}-coverage
           path: .coverage.*
 
   stage5-univar:
@@ -209,18 +241,21 @@
     steps:
       - uses: actions/checkout@v3
       - uses: ./.github/actions/sierra-setup
       - uses: ./.github/actions/sample-project-setup
         with:
           platform: argos
 
-      - name: Integration tests
-        shell: bash
-        run: |
-          ./scripts/argos-integration-tests.sh -f stage5_univar_test
+      - uses: nick-fields/retry@v2
+        name: Stage5 univariate tests
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/argos-integration-tests.sh -f stage5_univar_test
 
       - uses: actions/upload-artifact@v3
         with:
           name: ci-core-stage5-univar-${{ runner.os }}-${{ matrix.python-version }}-coverage
           path: .coverage.*
 
   stage5-bivar:
@@ -233,16 +268,19 @@
     steps:
       - uses: actions/checkout@v3
       - uses: ./.github/actions/sierra-setup
       - uses: ./.github/actions/sample-project-setup
         with:
           platform: argos
 
-      - name: Integration tests
-        shell: bash
-        run: |
-          ./scripts/argos-integration-tests.sh -f stage5_bivar_test
+      - uses: nick-fields/retry@v2
+        name: Stage5 univariate tests
+        with:
+          timeout_minutes: 3600
+          max_attempts: 3
+          shell: bash
+          command: ./scripts/argos-integration-tests.sh -f stage5_bivar_test
 
       - uses: actions/upload-artifact@v3
         with:
           name: ci-core-stage5-bivar-${{ runner.os }}-${{ matrix.python-version }}-coverage
           path: .coverage.*
```

### Comparing `sierra-research-1.3.1/.github/workflows/static-analysis.yml` & `sierra-research-1.3.5/.github/workflows/static-analysis.yml`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 on:
   push:
     paths:
       - 'sierra/**'
   schedule:
     - cron: '0 0 1 * *'
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
 
 jobs:
   analyze:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os:
```

### Comparing `sierra-research-1.3.1/.github/workflows/unit-tests.yml` & `sierra-research-1.3.5/.github/workflows/unit-tests.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/.gitignore` & `sierra-research-1.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/.pylintrc` & `sierra-research-1.3.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/.readthedocs.yml` & `sierra-research-1.3.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/LICENSE` & `sierra-research-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/PKG-INFO` & `sierra-research-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sierra-research
-Version: 1.3.1
+Version: 1.3.5
 Summary: Automation framework for the scientific method in AI research
 Home-page: https://github.com/jharwell/sierra
 Author: John Harwell
 Author-email: john.r.harwell@gmail.com
 License: MIT
 Keywords: research,automation,robotics,agent-based modeling,reproducibility,reusability
 Platform: linux
```

### Comparing `sierra-research-1.3.1/README.rst` & `sierra-research-1.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/Makefile` & `sierra-research-1.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/_build/man/sierra-cli.1` & `sierra-research-1.3.5/docs/_build/man/sierra-cli.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SIERRA-CLI" "1" "Jan 25, 2023" "1.3.1" "SIERRA"
+.TH "SIERRA-CLI" "1" "Jun 08, 2023" "1.3.5" "SIERRA"
 .SH NAME
 sierra-cli \- The SIERRA Command Line Interface (CLI).
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `sierra-research-1.3.1/docs/_build/man/sierra-examples.7` & `sierra-research-1.3.5/docs/_build/man/sierra-examples.7`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SIERRA-EXAMPLES" "7" "Jan 25, 2023" "1.3.1" "SIERRA"
+.TH "SIERRA-EXAMPLES" "7" "Jun 08, 2023" "1.3.5" "SIERRA"
 .SH NAME
 sierra-examples \- Examples of SIERRA usage. These examples all assume that you have successfully set up SIERRA with a project of your choice.
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `sierra-research-1.3.1/docs/_build/man/sierra-exec-envs.7` & `sierra-research-1.3.5/docs/_build/man/sierra-exec-envs.7`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SIERRA-EXEC-ENVS" "7" "Jan 25, 2023" "1.3.1" "SIERRA"
+.TH "SIERRA-EXEC-ENVS" "7" "Jun 08, 2023" "1.3.5" "SIERRA"
 .SH NAME
 sierra-exec-envs \- The execution environments SIERRA supports.
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `sierra-research-1.3.1/docs/_build/man/sierra-glossary.7` & `sierra-research-1.3.5/docs/_build/man/sierra-glossary.7`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SIERRA-GLOSSARY" "7" "Jan 25, 2023" "1.3.1" "SIERRA"
+.TH "SIERRA-GLOSSARY" "7" "Jun 08, 2023" "1.3.5" "SIERRA"
 .SH NAME
 sierra-glossary \- Glossary of SIERRA terminology.
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `sierra-research-1.3.1/docs/_build/man/sierra-platforms.7` & `sierra-research-1.3.5/docs/_build/man/sierra-platforms.7`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SIERRA-PLATFORMS" "7" "Jan 25, 2023" "1.3.1" "SIERRA"
+.TH "SIERRA-PLATFORMS" "7" "Jun 08, 2023" "1.3.5" "SIERRA"
 .SH NAME
 sierra-platforms \- The platforms SIERRA supports, and platform-specific Batch Criteria.
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `sierra-research-1.3.1/docs/_build/man/sierra-usage.7` & `sierra-research-1.3.5/docs/_build/man/sierra-usage.7`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SIERRA-USAGE" "7" "Jan 25, 2023" "1.3.1" "SIERRA"
+.TH "SIERRA-USAGE" "7" "Jun 08, 2023" "1.3.5" "SIERRA"
 .SH NAME
 sierra-usage \- How to use SIERRA. This covers all non-command line interface aspects.
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `sierra-research-1.3.1/docs/_build/man/sierra.7` & `sierra-research-1.3.5/docs/_build/man/sierra.7`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "SIERRA" "7" "Jan 25, 2023" "1.3.1" "SIERRA"
+.TH "SIERRA" "7" "Jun 08, 2023" "1.3.5" "SIERRA"
 .SH NAME
 sierra \- reSearch pIpEline for Reproducability, Reusability, and Automation.
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
```

### Comparing `sierra-research-1.3.1/docs/_ext/xref.py` & `sierra-research-1.3.5/docs/_ext/xref.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/_templates/autoapi/module.rst` & `sierra-research-1.3.5/docs/_templates/autoapi/module.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/conf.py` & `sierra-research-1.3.5/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,14 @@
                       "https://github.com:jharwell/sierra.git"),
     "SIERRA_SAMPLE_PROJECT": ("https://github.com:jharwell/sierra-sample-project.git",
                               "https://github.com:jharwell/sierra-sample-project.git"),
     "SIERRA_DOCS": ("https://sierra.readthedocs.io/en/master",
                     "https://sierra.readthedocs.io/en/master"),
     "FORDYCA": ("FORDYCA", "https://swarm-robotics-fordyca.readthedocs.io"),
     "PRISM": ("PRISM", "https://swarm-robotics-prism.readthedocs.io"),
-    "LIBRA": ("LIBRA", "https://swarm-robotics-libra.readthedocs.io"),
     "2022-aamas-demo": ("2022 AAMAS Demo",
                         "https://www-users.cse.umn.edu/~harwe006/showcase/aamas-2022-demo")
 
 }
 
 sphinx_tabs_disable_tab_closing = True
 # sphinx_tabs_disable_css_loading = True # True=tabs render more as buttons -_-
@@ -299,22 +298,24 @@
     (master_doc, 'Sierra', 'Sierra Documentation',
      author, 'Sierra', 'One line description of project.',
      'Miscellaneous'),
 ]
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'python3': ('https://docs.python.org/3', None),
-                       'numpy': ('https://numpy.org/doc/stable/', None),
-                       'scipy': ('https://docs.scipy.org/doc/scipy/reference', None),
-                       'matplotlib': ('https://matplotlib.org', None),
-                       'sphinx': ('https://www.sphinx-doc.org/en/stable/', None),
-                       'pandas': ('https://pandas.pydata.org/pandas-docs/dev', None),
-                       'implements': ('https://implements.readthedocs.io/en/latest/', None)
-                       }
+intersphinx_mapping = {
+    'python3': ('https://docs.python.org/3', None),
+    'numpy': ('https://numpy.org/doc/stable/', None),
+    'scipy': ('https://docs.scipy.org/doc/scipy/reference', None),
+    'matplotlib': ('https://matplotlib.org', None),
+    'sphinx': ('https://www.sphinx-doc.org/en/stable/', None),
+    'pandas': ('https://pandas.pydata.org/pandas-docs/dev', None),
+    'implements': ('https://implements.readthedocs.io/en/latest/', None),
+    'libra': ('https://libra2.readthedocs.io/en/master', None)
+}
 
 # This is the expected signature of the handler for this event, cf doc
 
 
 def autodoc_skip_member_handler(app, what, name, obj, skip, options):
     # Basic approach; you might want a regex instead
     return 'flycheck' in name
```

### Comparing `sierra-research-1.3.1/docs/figures/architecture.png` & `sierra-research-1.3.5/docs/figures/architecture.png`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/index.rst` & `sierra-research-1.3.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/man/sierra-cli.rst` & `sierra-research-1.3.5/docs/man/sierra-cli.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/man/sierra.rst` & `sierra-research-1.3.5/docs/man/sierra.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/contributing.rst` & `sierra-research-1.3.5/docs/src/contributing.rst`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 Mechanics
 =========
 
 Writing the code
 ----------------
 
 To contribute to the SIERRA core, in you should follow the general workflow and
-python development guide outlined in :xref:`LIBRA`. For the static analysis
-step:
+python development guide outlined in :ref:`ln-libra-python-dev-guide` and
+:ref:`ln-libra-dev-workflow`. For the static analysis step:
 
 #. Install development packages for SIERRA (from the SIERRA repo root)::
 
      pip3 install .[devel]
 
 #. Run ``nox`` to check most things prior to commiting/pushing your changes. If
    there are errors *you* have introduced, fix them. Some checkers (such as
```

### Comparing `sierra-research-1.3.1/docs/src/description.rst` & `sierra-research-1.3.5/docs/src/description.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/exec_env/hpc.rst` & `sierra-research-1.3.5/docs/src/exec_env/hpc.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/exec_env/robot.rst` & `sierra-research-1.3.5/docs/src/exec_env/robot.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/faq.rst` & `sierra-research-1.3.5/docs/src/faq.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/getting_started.rst` & `sierra-research-1.3.5/docs/src/getting_started.rst`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
               Install the following required packages with ``apt install``:
 
               - ``parallel``
               - ``cm-super``
               - ``texlive-fonts-recommended``
               - ``texlive-latex-extra``
               - ``dvipng``
+              - ``psmisc``
 
               Install the following optional packages with ``apt install``:
 
               - ``pssh``
               - ``ffmpeg``
               - ``xvfb``
```

### Comparing `sierra-research-1.3.1/docs/src/glossary.rst` & `sierra-research-1.3.5/docs/src/glossary.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/matrix.rst` & `sierra-research-1.3.5/docs/src/matrix.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/packages.rst` & `sierra-research-1.3.5/docs/src/packages.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/philosophy.rst` & `sierra-research-1.3.5/docs/src/philosophy.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/platform/argos/batch_criteria.rst` & `sierra-research-1.3.5/docs/src/platform/argos/batch_criteria.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/platform/argos/index.rst` & `sierra-research-1.3.5/docs/src/platform/argos/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/platform/ros1gazebo/batch_criteria.rst` & `sierra-research-1.3.5/docs/src/platform/ros1gazebo/batch_criteria.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/platform/ros1gazebo/index.rst` & `sierra-research-1.3.5/docs/src/platform/ros1gazebo/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/platform/ros1robot/batch_criteria.rst` & `sierra-research-1.3.5/docs/src/platform/ros1robot/batch_criteria.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/platform/ros1robot/index.rst` & `sierra-research-1.3.5/docs/src/platform/ros1robot/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/requirements.rst` & `sierra-research-1.3.5/docs/src/requirements.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,29 +12,35 @@
 .. _ln-sierra-req-OS:
 
 OS Requirements
 ===============
 
 One of the following:
 
-- Recent linux. SIERRA is tested with ubuntu 20.04+, though it will probably
+- Recent linux. SIERRA is tested with Ubuntu 20.04+, though it will probably
   work on less recent versions/other distros as well.
 
 - Recent OSX. SIERRA is tested with OSX 12+, though it *might* work on less
   recent versions.
 
 
 .. NOTE:: Windows is not supported currently. Not because it can't be supported,
           but because there are not current any platform plugins that which work
           on windows. SIERRA is written in pure python, and could be made to
           work on windows with a little work.
 
           If windows support would be helpful for your intended usage of SIERRA,
           please get in touch with me.
 
+Python Requirements
+===================
+
+Python 3.8+. Tested with 3.8-3.9. It may work for newer versions, probably won't
+for older.
+
 .. _ln-sierra-req-exp:
 
 Experimental Definition Requirements
 ====================================
 
 General
 -------
@@ -328,14 +334,27 @@
    (e.g., an appropriate ``setup.bash`` is sourced in ``.bashrc``).
 
 #. All robots have :envvar:`ROS_IP` or :envvar:`ROS_HOSTNAME` populated, or
    otherwise can correctly report their address to the ROS master. You can
    verify this by trying to launch a ROS master on each robot: if it launches
    without errors, then these values are setup properly.
 
+.. _ln-sierra-req-models:
+
+============================
+Model Framework Requirements
+============================
+
+When running models during stage 4 (see
+:ref:`ln-sierra-tutorials-project-models`) SIERRA requires that:
+
+- All models return :class:`pandas.DataFrame` (if they don't do this natively,
+  then their python bindings will have to do it). This is enforced by the
+  interfaces models must implement.
+
 .. _ln-sierra-req-xml:
 
 XML Content Requirements
 ========================
 
 Reserved Tokens
 ---------------
```

### Comparing `sierra-research-1.3.1/docs/src/roadmap.rst` & `sierra-research-1.3.5/docs/src/roadmap.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/storage/index.rst` & `sierra-research-1.3.5/docs/src/storage/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/trial.rst` & `sierra-research-1.3.5/docs/src/trial.rst`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
               Install the following required packages with ``apt install``:
 
               - ``parallel``
               - ``cm-super``
               - ``texlive-fonts-recommended``
               - ``texlive-latex-extra``
               - ``dvipng``
+              - ``psmisc``
 
               Install the following optional packages with ``apt install``:
 
               - ``pssh``
               - ``ffmpeg``
               - ``xvfb``
```

### Comparing `sierra-research-1.3.1/docs/src/tutorials/hpc/cluster_setup.rst` & `sierra-research-1.3.5/docs/src/tutorials/hpc/cluster_setup.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/index.rst` & `sierra-research-1.3.5/docs/src/tutorials/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/plugin/exec_env/index.rst` & `sierra-research-1.3.5/docs/src/tutorials/plugin/exec_env/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/plugin/exec_env/plugin.rst` & `sierra-research-1.3.5/docs/src/tutorials/plugin/exec_env/plugin.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/plugin/platform/cmdline.rst` & `sierra-research-1.3.5/docs/src/tutorials/plugin/platform/cmdline.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/plugin/platform/generators.rst` & `sierra-research-1.3.5/docs/src/tutorials/plugin/platform/generators.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/plugin/platform/index.rst` & `sierra-research-1.3.5/docs/src/tutorials/plugin/platform/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/plugin/platform/plugin.rst` & `sierra-research-1.3.5/docs/src/tutorials/plugin/platform/plugin.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/plugin/storage/index.rst` & `sierra-research-1.3.5/docs/src/tutorials/plugin/storage/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/plugin/storage/plugin.rst` & `sierra-research-1.3.5/docs/src/tutorials/plugin/storage/plugin.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/project/cmdline.rst` & `sierra-research-1.3.5/docs/src/tutorials/project/cmdline.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/project/generators.rst` & `sierra-research-1.3.5/docs/src/tutorials/project/generators.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/project/graphs_config.rst` & `sierra-research-1.3.5/docs/src/tutorials/project/graphs_config.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/project/hooks.rst` & `sierra-research-1.3.5/docs/src/tutorials/project/hooks.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/project/main_config/controllers.rst` & `sierra-research-1.3.5/docs/src/tutorials/project/main_config/controllers.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/project/main_config/main.rst` & `sierra-research-1.3.5/docs/src/tutorials/project/main_config/main.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/project/main_config/perf.rst` & `sierra-research-1.3.5/docs/src/tutorials/project/main_config/perf.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/project/new_bc.rst` & `sierra-research-1.3.5/docs/src/tutorials/project/new_bc.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/project/project.rst` & `sierra-research-1.3.5/docs/src/tutorials/project/project.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/project/stage5_config.rst` & `sierra-research-1.3.5/docs/src/tutorials/project/stage5_config.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/tutorials/project/template_input_file.rst` & `sierra-research-1.3.5/docs/src/tutorials/project/template_input_file.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/usage/cli-core.rst` & `sierra-research-1.3.5/docs/src/usage/cli-core.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/usage/cli.rst` & `sierra-research-1.3.5/docs/src/usage/cli.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/usage/environment.rst` & `sierra-research-1.3.5/docs/src/usage/environment.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/usage/examples.rst` & `sierra-research-1.3.5/docs/src/usage/examples.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/usage/index.rst` & `sierra-research-1.3.5/docs/src/usage/index.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/usage/pipeline.rst` & `sierra-research-1.3.5/docs/src/usage/pipeline.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/usage/rendering.rst` & `sierra-research-1.3.5/docs/src/usage/rendering.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/usage/run_time_tree.rst` & `sierra-research-1.3.5/docs/src/usage/run_time_tree.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/usage/stage5.rst` & `sierra-research-1.3.5/docs/src/usage/stage5.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/usage/subprograms.rst` & `sierra-research-1.3.5/docs/src/usage/subprograms.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/docs/src/usage/variables.rst` & `sierra-research-1.3.5/docs/src/usage/variables.rst`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/noxfile.py` & `sierra-research-1.3.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/scripts/argos-integration-tests.sh` & `sierra-research-1.3.5/scripts/argos-integration-tests.sh`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/scripts/core-integration-tests.sh` & `sierra-research-1.3.5/scripts/core-integration-tests.sh`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/scripts/ros1gazebo-integration-tests.sh` & `sierra-research-1.3.5/scripts/ros1gazebo-integration-tests.sh`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/scripts/ros1robot-integration-tests.sh` & `sierra-research-1.3.5/scripts/ros1robot-integration-tests.sh`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/scripts/slurm-test.sh` & `sierra-research-1.3.5/scripts/slurm-test.sh`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/scripts/slurm.conf` & `sierra-research-1.3.5/scripts/slurm.conf`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/setup.py` & `sierra-research-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,29 +101,30 @@
             # checkers, CI, etc.
             'pylint==2.14.5',  # Temporarily, until the default 2.15.0 is fixed/superseded
             'pytype',
             'pydocstyle',
             'xenon',
             'flake8',
             'nox',
+            'psutil',
             'pytest',
             'pytest-cov',
             'mypy',
             'xmldiff',
             'coverage',
             'coveralls',
             'mypy-runner',
 
             # Deployment packages
             'build',
             'twine',
             'setuptools',
 
             # Sphinx packages
-            "sphinx",
+            "sphinx==4.4.0",
             "docutils==0.16",
             "sphinx-rtd-theme",
             "sphinx-argparse",
             "sphinx-tabs",
             "sphinxcontrib-napoleon",
             "sphinx-last-updated-by-git",
             "autoapi",
```

### Comparing `sierra-research-1.3.1/sierra/core/cmdline.py` & `sierra-research-1.3.5/sierra/core/cmdline.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/config.py` & `sierra-research-1.3.5/sierra/core/config.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/experiment/bindings.py` & `sierra-research-1.3.5/sierra/core/experiment/bindings.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/experiment/definition.py` & `sierra-research-1.3.5/sierra/core/experiment/definition.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/experiment/spec.py` & `sierra-research-1.3.5/sierra/core/experiment/spec.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/experiment/xml.py` & `sierra-research-1.3.5/sierra/core/experiment/xml.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/generators/controller_generator_parser.py` & `sierra-research-1.3.5/sierra/core/generators/controller_generator_parser.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/generators/exp_creator.py` & `sierra-research-1.3.5/sierra/core/generators/exp_creator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/generators/exp_generators.py` & `sierra-research-1.3.5/sierra/core/generators/exp_generators.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/generators/generator_factory.py` & `sierra-research-1.3.5/sierra/core/generators/generator_factory.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/graphs/heatmap.py` & `sierra-research-1.3.5/sierra/core/graphs/heatmap.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/graphs/scatterplot2D.py` & `sierra-research-1.3.5/sierra/core/graphs/scatterplot2D.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/graphs/stacked_line_graph.py` & `sierra-research-1.3.5/sierra/core/graphs/stacked_line_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     def _plot_legend(self, ax, model_legend: tp.List[str], ncols: int) -> None:
         # Should always use one column: If a small number of lines are plotted,
         # then 1 vs. > 1 column makes no difference. If a large number of lines
         # are plotted, this will make the figures more portrait than landscape,
         # which is more amenable to inclusion in academic papers.
 
         # If the legend is not specified, then we assume this is not a graph
-        # that will contain any models.
+        # that will contain any models and/or no legend is desired.
         legend = self.legend
 
         if self.legend is not None:
             legend = copy.deepcopy(self.legend)
             if model_legend:
                 legend.extend(model_legend)
 
@@ -193,29 +193,32 @@
             ax.legend(lines,
                       legend,
                       loc='lower center',
                       bbox_to_anchor=(0.5, -0.5),
                       ncol=1,
                       fontsize=self.text_size['legend_label'])
         else:
-            ax.legend(loc='lower center',
-                      bbox_to_anchor=(0.5, -0.5),
-                      ncol=1,
-                      fontsize=self.text_size['legend_label'])
+            ax.legend().remove()
+        #     ax.legend(loc='lower center',
+        #               bbox_to_anchor=(0.5, -0.5),
+        #               ncol=1,
+        #               fontsize=self.text_size['legend_label'])
 
     def _read_stats(self) -> tp.Dict[str, pd.DataFrame]:
         dfs = {}
+
         reader = storage.DataFrameReader('storage.csv')
         if self.stats in ['conf95', 'all']:
             exts = config.kStats['conf95'].exts
+
             for k in exts:
                 ipath = self.stats_root / (self.input_stem + exts[k])
 
                 if utils.path_exists(ipath):
-                    dfs[exts[k]] = reader(ipath)
+                    dfs[k] = reader(ipath)
                 else:
                     self.logger.warning("%sfile not found for '%s'",
                                         exts[k],
                                         self.input_stem)
 
         return dfs
```

### Comparing `sierra-research-1.3.1/sierra/core/graphs/stacked_surface_graph.py` & `sierra-research-1.3.5/sierra/core/graphs/stacked_surface_graph.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/graphs/summary_line_graph.py` & `sierra-research-1.3.5/sierra/core/graphs/summary_line_graph.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/hpc/cmdline.py` & `sierra-research-1.3.5/sierra/core/hpc/cmdline.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/logging.py` & `sierra-research-1.3.5/sierra/core/logging.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/models/graphs.py` & `sierra-research-1.3.5/sierra/core/models/graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 Graphs which can always be generated, irrespective of model specifics.
 
 For example, you can always compare the model value to the empirical value, and
 plot the difference as error.
 """
 # Core packages
-import os
 import pathlib
 
 # 3rd party packages
 
 # Project packages
 from sierra.core.graphs.heatmap import HeatmapSet
 from sierra.core import utils, config, storage
```

### Comparing `sierra-research-1.3.1/sierra/core/models/interface.py` & `sierra-research-1.3.5/sierra/core/models/interface.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/pipeline.py` & `sierra-research-1.3.5/sierra/core/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage1/pipeline_stage1.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage1/pipeline_stage1.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage2/exp_runner.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage2/exp_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,18 +203,18 @@
 
             runner = ExpRunner(self.cmdopts,
                                exec_times_fpath,
                                generator,
                                shell)
             runner(exp, exp_num)
 
-        # Run cmds to cleanup platform-specific things now that the experiment
-        # is done (if needed).
-        for spec in generator.post_exp_cmds():
-            shell.run_from_spec(spec)
+            # Run cmds to cleanup platform-specific things now that the experiment
+            # is done (if needed).
+            for spec in generator.post_exp_cmds():
+                shell.run_from_spec(spec)
 
 
 class ExpRunner:
     """
     Execute each :term:`Experimental Run` in an :term:`Experiment`.
 
     In parallel if the selected execution environment supports it, otherwise
```

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage2/pipeline_stage2.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage2/pipeline_stage2.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage3/imagizer.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage3/imagizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,16 @@
                 Heatmap(input_fpath=ipath,
                         output_fpath=opath,
                         title=match['title'],
                         xlabel='X',
                         ylabel='Y').generate()
 
             else:
-                self.logger.warning("No match for graph with src_stem=%s found",
+                self.logger.warning(("No match for graph with src_stem='%s' "
+                                     "found in configuration"),
                                     imagize_opts['graph_stem'])
 
 
 __api__ = [
     'BatchExpParallelImagizer',
     'ExpImagizer'
 ]
```

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage3/pipeline_stage3.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage3/pipeline_stage3.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage3/run_collator.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage3/run_collator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage3/statistics_calculator.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage3/statistics_calculator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage4/graph_collator.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage4/graph_collator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage4/inter_exp_graph_generator.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage4/inter_exp_graph_generator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage4/intra_exp_graph_generator.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage4/intra_exp_graph_generator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage4/model_runner.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage4/model_runner.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage4/pipeline_stage4.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage4/pipeline_stage4.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage4/rendering.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage4/rendering.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage4/yaml_config_loader.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage4/yaml_config_loader.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage5/inter_scenario_comparator.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage5/inter_scenario_comparator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage5/intra_scenario_comparator.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage5/intra_scenario_comparator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/pipeline/stage5/pipeline_stage5.py` & `sierra-research-1.3.5/sierra/core/pipeline/stage5/pipeline_stage5.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/platform.py` & `sierra-research-1.3.5/sierra/core/platform.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/plugin.py` & `sierra-research-1.3.5/sierra/core/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/plugin_manager.py` & `sierra-research-1.3.5/sierra/core/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/root_dirpath_generator.py` & `sierra-research-1.3.5/sierra/core/root_dirpath_generator.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/ros1/callbacks.py` & `sierra-research-1.3.5/sierra/core/ros1/callbacks.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/ros1/cmdline.py` & `sierra-research-1.3.5/sierra/core/ros1/cmdline.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/ros1/generators.py` & `sierra-research-1.3.5/sierra/core/ros1/generators.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/ros1/variables/exp_setup.py` & `sierra-research-1.3.5/sierra/core/ros1/variables/exp_setup.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/startup.py` & `sierra-research-1.3.5/sierra/core/startup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
                                        'debian',
                                        pkgs={
                                            'parallel': True,
                                            'cm-super': True,
                                            'texlive-fonts-recommended': True,
                                            'texlive-latex-extra': True,
                                            'dvipng': True,
+                                           'psmisc': True,
                                            'pssh': False,
                                            'ffmpeg': False,
                                            'xvfb': False
                                        })
 """
 The required/optional .deb packages for debian-based distributions.
 """
```

### Comparing `sierra-research-1.3.1/sierra/core/stat_kernels.py` & `sierra-research-1.3.5/sierra/core/stat_kernels.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/storage.py` & `sierra-research-1.3.5/sierra/core/storage.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/types.py` & `sierra-research-1.3.5/sierra/core/types.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/utils.py` & `sierra-research-1.3.5/sierra/core/utils.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/variables/base_variable.py` & `sierra-research-1.3.5/sierra/core/variables/base_variable.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/variables/batch_criteria.py` & `sierra-research-1.3.5/sierra/core/variables/batch_criteria.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/variables/exp_setup.py` & `sierra-research-1.3.5/sierra/core/variables/exp_setup.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/variables/population_size.py` & `sierra-research-1.3.5/sierra/core/variables/population_size.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/variables/variable_density.py` & `sierra-research-1.3.5/sierra/core/variables/variable_density.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/core/vector.py` & `sierra-research-1.3.5/sierra/core/vector.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/main.py` & `sierra-research-1.3.5/sierra/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         install_root = pathlib.Path(this_file.parent)
 
         # Load plugins
         self.logger.info("Loading plugins")
         project = bootstrap_args.project
         plugin_core_path = [install_root / 'plugins' / 'hpc',
                             install_root / 'plugins' / 'storage',
-                            install_root / 'plugins' / 'robots',
+                            install_root / 'plugins' / 'robot',
                             install_root / 'plugins' / 'platform']
         plugin_search_path = plugin_core_path
         env = os.environ.get('SIERRA_PLUGIN_PATH')
         if env is not None:
             for p in env.split(os.pathsep):
                 plugin_search_path.append(pathlib.Path(p))
```

### Comparing `sierra-research-1.3.1/sierra/plugins/hpc/adhoc/plugin.py` & `sierra-research-1.3.5/sierra/plugins/hpc/adhoc/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/hpc/local/plugin.py` & `sierra-research-1.3.5/sierra/plugins/hpc/local/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/hpc/pbs/plugin.py` & `sierra-research-1.3.5/sierra/plugins/hpc/pbs/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/hpc/slurm/plugin.py` & `sierra-research-1.3.5/sierra/plugins/hpc/slurm/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/argos/cmdline.py` & `sierra-research-1.3.5/sierra/plugins/platform/argos/cmdline.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/argos/generators/platform_generators.py` & `sierra-research-1.3.5/sierra/plugins/platform/argos/generators/platform_generators.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/argos/plugin.py` & `sierra-research-1.3.5/sierra/plugins/platform/argos/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/argos/variables/arena_shape.py` & `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/arena_shape.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/argos/variables/cameras.py` & `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/cameras.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/argos/variables/constant_density.py` & `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/constant_density.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/argos/variables/exp_setup.py` & `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/exp_setup.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/argos/variables/physics_engines.py` & `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/physics_engines.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/argos/variables/population_constant_density.py` & `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/population_constant_density.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/argos/variables/population_size.py` & `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/population_size.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/argos/variables/population_variable_density.py` & `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/population_variable_density.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/argos/variables/rendering.py` & `sierra-research-1.3.5/sierra/plugins/platform/argos/variables/rendering.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/ros1gazebo/cmdline.py` & `sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/cmdline.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/ros1gazebo/generators/platform_generators.py` & `sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/generators/platform_generators.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/ros1gazebo/plugin.py` & `sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/ros1gazebo/variables/population_size.py` & `sierra-research-1.3.5/sierra/plugins/platform/ros1gazebo/variables/population_size.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/ros1robot/cmdline.py` & `sierra-research-1.3.5/sierra/plugins/platform/ros1robot/cmdline.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/ros1robot/generators/platform_generators.py` & `sierra-research-1.3.5/sierra/plugins/platform/ros1robot/generators/platform_generators.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/ros1robot/plugin.py` & `sierra-research-1.3.5/sierra/plugins/platform/ros1robot/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/platform/ros1robot/variables/population_size.py` & `sierra-research-1.3.5/sierra/plugins/platform/ros1robot/variables/population_size.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/robot/turtlebot3/plugin.py` & `sierra-research-1.3.5/sierra/plugins/robot/turtlebot3/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra/plugins/storage/csv/plugin.py` & `sierra-research-1.3.5/sierra/plugins/storage/csv/plugin.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/sierra_research.egg-info/PKG-INFO` & `sierra-research-1.3.5/sierra_research.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sierra-research
-Version: 1.3.1
+Version: 1.3.5
 Summary: Automation framework for the scientific method in AI research
 Home-page: https://github.com/jharwell/sierra
 Author: John Harwell
 Author-email: john.r.harwell@gmail.com
 License: MIT
 Keywords: research,automation,robotics,agent-based modeling,reproducibility,reusability
 Platform: linux
```

### Comparing `sierra-research-1.3.1/sierra_research.egg-info/SOURCES.txt` & `sierra-research-1.3.5/sierra_research.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/tests/arena_extent_test.py` & `sierra-research-1.3.5/tests/arena_extent_test.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/tests/exp_def_test.py` & `sierra-research-1.3.5/tests/exp_def_test.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/tests/test1.xml` & `sierra-research-1.3.5/tests/test1.xml`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/tests/vector_test.py` & `sierra-research-1.3.5/tests/vector_test.py`

 * *Files identical despite different names*

### Comparing `sierra-research-1.3.1/todo.org` & `sierra-research-1.3.5/todo.org`

 * *Files identical despite different names*

