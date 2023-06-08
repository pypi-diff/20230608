# Comparing `tmp/flowrunner-0.2.2.tar.gz` & `tmp/flowrunner-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowrunner-0.2.2.tar", last modified: Sat Jun  3 12:58:38 2023, max compression
+gzip compressed data, was "flowrunner-0.2.3.tar", last modified: Thu Jun  8 15:59:41 2023, max compression
```

## Comparing `flowrunner-0.2.2.tar` & `flowrunner-0.2.3.tar`

### file list

```diff
@@ -1,114 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.387430 flowrunner-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.375429 flowrunner-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.375429 flowrunner-0.2.2/.github/issue_template/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/issue_template/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/issue_template/documentation_improvement.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/issue_template/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.375429 flowrunner-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/workflows/code_scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/workflows/release_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-03 12:58:27.000000 flowrunner-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-03 12:58:27.000000 flowrunner-0.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-06-03 12:58:38.387430 flowrunner-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-03 12:58:27.000000 flowrunner-0.2.2/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.375429 flowrunner-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.379429 flowrunner-0.2.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.379429 flowrunner-0.2.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   955116 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/_static/flowrunner_databricks_example.html
--rw-r--r--   0 runner    (1001) docker     (123)   601383 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/_static/flowrunner_pandas_notebook_example.html
--rw-r--r--   0 runner    (1001) docker     (123)   607135 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/_static/flowrunner_pyspark_example.html
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/contributing_guide_code.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/contributing_guide_docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/creating_flowrunner_projects.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/creating_your_development_environment.rst
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/docutils.conf
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/flowrunner.core.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/flowrunner.core.templates.rst
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/flowrunner.rst
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/flowrunner.runner.rst
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/flowrunner.system.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/notebook_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/pandas_example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/pyspark_example.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.379429 flowrunner-0.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-03 12:58:27.000000 flowrunner-0.2.2/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-03 12:58:27.000000 flowrunner-0.2.2/examples/pandas_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-03 12:58:27.000000 flowrunner-0.2.2/examples/pyspark_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/flowrunner/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/flowrunner/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14889 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/core/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/flowrunner/core/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/core/templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/flowrunner/runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/runner/flow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/flowrunner/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/system/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/system/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/flowrunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-06-03 12:58:38.000000 flowrunner-0.2.2/flowrunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-03 12:58:38.000000 flowrunner-0.2.2/flowrunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:58:38.000000 flowrunner-0.2.2/flowrunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-03 12:58:38.000000 flowrunner-0.2.2/flowrunner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-03 12:58:38.000000 flowrunner-0.2.2/flowrunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-03 12:58:38.000000 flowrunner-0.2.2/flowrunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-03 12:58:27.000000 flowrunner-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-06-03 12:58:27.000000 flowrunner-0.2.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 12:58:38.387430 flowrunner-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-03 12:58:27.000000 flowrunner-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.371429 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/html_dags/
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/html_dags/dagsexamplepandas.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/my_flows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/my_flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/my_flows/pandas_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/tests/test_flowrunner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.387430 flowrunner-0.2.2/tests/test_flowrunner/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/core/examplepandas.html
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/core/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/core/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/core/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.387430 flowrunner-0.2.2/tests/test_flowrunner/runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/runner/test_flow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.387430 flowrunner-0.2.2/tests/test_flowrunner/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/system/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.387430 flowrunner-0.2.2/tests/test_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_templates/test_cookiecutter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.181581 flowrunner-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.173581 flowrunner-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.173581 flowrunner-0.2.3/.github/issue_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-08 15:59:30.000000 flowrunner-0.2.3/.github/issue_template/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-08 15:59:30.000000 flowrunner-0.2.3/.github/issue_template/documentation_improvement.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-08 15:59:30.000000 flowrunner-0.2.3/.github/issue_template/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-08 15:59:30.000000 flowrunner-0.2.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.173581 flowrunner-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-08 15:59:30.000000 flowrunner-0.2.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-08 15:59:30.000000 flowrunner-0.2.3/.github/workflows/code_scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-08 15:59:30.000000 flowrunner-0.2.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-08 15:59:30.000000 flowrunner-0.2.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-08 15:59:30.000000 flowrunner-0.2.3/.github/workflows/release_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-08 15:59:30.000000 flowrunner-0.2.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-06-08 15:59:30.000000 flowrunner-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-08 15:59:30.000000 flowrunner-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-08 15:59:30.000000 flowrunner-0.2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-08 15:59:30.000000 flowrunner-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-08 15:59:30.000000 flowrunner-0.2.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-06-08 15:59:41.181581 flowrunner-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-08 15:59:30.000000 flowrunner-0.2.3/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.173581 flowrunner-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.173581 flowrunner-0.2.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.177581 flowrunner-0.2.3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   955116 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/_static/flowrunner_databricks_example.html
+-rw-r--r--   0 runner    (1001) docker     (123)   601383 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/_static/flowrunner_pandas_notebook_example.html
+-rw-r--r--   0 runner    (1001) docker     (123)   607135 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/_static/flowrunner_pyspark_example.html
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/contributing_guide_code.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/contributing_guide_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/creating_flowrunner_projects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/creating_your_development_environment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/docutils.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/flowrunner.core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/flowrunner.core.templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/flowrunner.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/flowrunner.runner.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/flowrunner.system.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/notebook_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/pandas_example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-08 15:59:30.000000 flowrunner-0.2.3/docs/source/pyspark_example.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.177581 flowrunner-0.2.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-08 15:59:30.000000 flowrunner-0.2.3/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-08 15:59:30.000000 flowrunner-0.2.3/examples/pandas_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-08 15:59:30.000000 flowrunner-0.2.3/examples/pyspark_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.177581 flowrunner-0.2.3/flowrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.181581 flowrunner-0.2.3/flowrunner/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14889 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/core/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.181581 flowrunner-0.2.3/flowrunner/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/core/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.181581 flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.169581 flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.181581 flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/html_dags/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/html_dags/dagsexamplepandas.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.181581 flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/my_flows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/my_flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/my_flows/pandas_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.181581 flowrunner-0.2.3/flowrunner/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/runner/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.181581 flowrunner-0.2.3/flowrunner/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/system/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-08 15:59:30.000000 flowrunner-0.2.3/flowrunner/system/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.177581 flowrunner-0.2.3/flowrunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-06-08 15:59:41.000000 flowrunner-0.2.3/flowrunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-08 15:59:41.000000 flowrunner-0.2.3/flowrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:59:41.000000 flowrunner-0.2.3/flowrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 15:59:41.000000 flowrunner-0.2.3/flowrunner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-08 15:59:41.000000 flowrunner-0.2.3/flowrunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 15:59:41.000000 flowrunner-0.2.3/flowrunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-08 15:59:30.000000 flowrunner-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-06-08 15:59:30.000000 flowrunner-0.2.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:59:41.181581 flowrunner-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-08 15:59:30.000000 flowrunner-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.181581 flowrunner-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.181581 flowrunner-0.2.3/tests/test_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/test_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/test_examples/test_example_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/test_examples/test_example_notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.181581 flowrunner-0.2.3/tests/test_flowrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/test_flowrunner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.181581 flowrunner-0.2.3/tests/test_flowrunner/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/test_flowrunner/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/test_flowrunner/core/examplepandas.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.181581 flowrunner-0.2.3/tests/test_flowrunner/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/test_flowrunner/core/templates/test_cookiecutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/test_flowrunner/core/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/test_flowrunner/core/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/test_flowrunner/core/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.181581 flowrunner-0.2.3/tests/test_flowrunner/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/test_flowrunner/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/test_flowrunner/runner/test_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:41.181581 flowrunner-0.2.3/tests/test_flowrunner/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/test_flowrunner/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/test_flowrunner/system/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-08 15:59:30.000000 flowrunner-0.2.3/tests/test_flowrunner/test_cli.py
```

### Comparing `flowrunner-0.2.2/.github/issue_template/bug_report.md` & `flowrunner-0.2.3/.github/issue_template/bug_report.md`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/.github/issue_template/feature_request.md` & `flowrunner-0.2.3/.github/issue_template/feature_request.md`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/.github/workflows/build.yml` & `flowrunner-0.2.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/.github/workflows/code_scan.yml` & `flowrunner-0.2.3/.github/workflows/code_scan.yml`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/.github/workflows/docs.yml` & `flowrunner-0.2.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/.github/workflows/release.yml` & `flowrunner-0.2.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/.github/workflows/release_test.yml` & `flowrunner-0.2.3/.github/workflows/release_test.yml`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/.github/workflows/tests.yml` & `flowrunner-0.2.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/.gitignore` & `flowrunner-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/.pre-commit-config.yaml` & `flowrunner-0.2.3/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
-exclude:
-    '[^docs/source/_static/]' # the databricks notebook is larger but required, compression did not work, and templates because that makes an issue for cookic
 
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v3.2.0
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
```

### Comparing `flowrunner-0.2.2/.readthedocs.yaml` & `flowrunner-0.2.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/LICENSE` & `flowrunner-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/Makefile` & `flowrunner-0.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/PKG-INFO` & `flowrunner-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowrunner
-Version: 0.2.2
+Version: 0.2.3
 Summary: Flowrunner is a lightweight package to organize and represent Data Engineering/Science workflows
 Author-email: Prithvijit Guha <prithvijit_guha2@hotmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Prithvijit
         All rights reserved.
```

### Comparing `flowrunner-0.2.2/changelog.md` & `flowrunner-0.2.3/changelog.md`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/Makefile` & `flowrunner-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/make.bat` & `flowrunner-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/source/_static/flowrunner_databricks_example.html` & `flowrunner-0.2.3/docs/source/_static/flowrunner_databricks_example.html`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/source/_static/flowrunner_pandas_notebook_example.html` & `flowrunner-0.2.3/docs/source/_static/flowrunner_pandas_notebook_example.html`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/source/_static/flowrunner_pyspark_example.html` & `flowrunner-0.2.3/docs/source/_static/flowrunner_pyspark_example.html`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/source/conf.py` & `flowrunner-0.2.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/source/contributing_guide_code.rst` & `flowrunner-0.2.3/docs/source/contributing_guide_code.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/source/contributing_guide_docs.rst` & `flowrunner-0.2.3/docs/source/contributing_guide_docs.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/source/creating_flowrunner_projects.rst` & `flowrunner-0.2.3/docs/source/creating_flowrunner_projects.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/source/creating_your_development_environment.rst` & `flowrunner-0.2.3/docs/source/creating_your_development_environment.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/source/flowrunner.core.rst` & `flowrunner-0.2.3/docs/source/flowrunner.core.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/source/flowrunner.system.rst` & `flowrunner-0.2.3/docs/source/flowrunner.system.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/source/getting_started.rst` & `flowrunner-0.2.3/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/source/introduction.rst` & `flowrunner-0.2.3/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/source/notebook_examples.rst` & `flowrunner-0.2.3/docs/source/notebook_examples.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/source/pandas_example.rst` & `flowrunner-0.2.3/docs/source/pandas_example.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/docs/source/pyspark_example.rst` & `flowrunner-0.2.3/docs/source/pyspark_example.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/examples/example.py` & `flowrunner-0.2.3/examples/example.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/examples/pandas_example.py` & `flowrunner-0.2.3/examples/pandas_example.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/examples/pyspark_example.py` & `flowrunner-0.2.3/examples/pyspark_example.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/flowrunner/__init__.py` & `flowrunner-0.2.3/flowrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/flowrunner/cli.py` & `flowrunner-0.2.3/flowrunner/cli.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/flowrunner/core/base.py` & `flowrunner-0.2.3/flowrunner/core/base.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/flowrunner/core/decorators.py` & `flowrunner-0.2.3/flowrunner/core/decorators.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/flowrunner/core/helpers.py` & `flowrunner-0.2.3/flowrunner/core/helpers.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/flowrunner/core/templates/base.html` & `flowrunner-0.2.3/flowrunner/core/templates/base.html`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/flowrunner/runner/flow.py` & `flowrunner-0.2.3/flowrunner/runner/flow.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/flowrunner.egg-info/PKG-INFO` & `flowrunner-0.2.3/flowrunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowrunner
-Version: 0.2.2
+Version: 0.2.3
 Summary: Flowrunner is a lightweight package to organize and represent Data Engineering/Science workflows
 Author-email: Prithvijit Guha <prithvijit_guha2@hotmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Prithvijit
         All rights reserved.
```

### Comparing `flowrunner-0.2.2/flowrunner.egg-info/SOURCES.txt` & `flowrunner-0.2.3/flowrunner.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -54,34 +54,36 @@
 flowrunner.egg-info/top_level.txt
 flowrunner/core/__init__.py
 flowrunner/core/base.py
 flowrunner/core/decorators.py
 flowrunner/core/helpers.py
 flowrunner/core/templates/__init__.py
 flowrunner/core/templates/base.html
+flowrunner/core/templates/{{ cookiecutter.project_name }}/.gitignore
+flowrunner/core/templates/{{ cookiecutter.project_name }}/changelog.md
+flowrunner/core/templates/{{ cookiecutter.project_name }}/pyproject.toml
+flowrunner/core/templates/{{ cookiecutter.project_name }}/readme.md
+flowrunner/core/templates/{{ cookiecutter.project_name }}/setup.py
+flowrunner/core/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/html_dags/dagsexamplepandas.html
+flowrunner/core/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/my_flows/__init__.py
+flowrunner/core/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/my_flows/pandas_example.py
 flowrunner/runner/__init__.py
 flowrunner/runner/flow.py
 flowrunner/system/__init__.py
 flowrunner/system/exceptions.py
 flowrunner/system/logger.py
-templates/cookiecutter.json
-templates/{{ cookiecutter.project_name }}/.gitignore
-templates/{{ cookiecutter.project_name }}/changelog.md
-templates/{{ cookiecutter.project_name }}/pyproject.toml
-templates/{{ cookiecutter.project_name }}/readme.md
-templates/{{ cookiecutter.project_name }}/setup.py
-templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/html_dags/dagsexamplepandas.html
-templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/my_flows/__init__.py
-templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/my_flows/pandas_example.py
 tests/__init__.py
+tests/test_examples/__init__.py
+tests/test_examples/test_example_notebook.ipynb
+tests/test_examples/test_example_notebook.py
 tests/test_flowrunner/__init__.py
 tests/test_flowrunner/test_cli.py
 tests/test_flowrunner/core/__init__.py
 tests/test_flowrunner/core/examplepandas.html
 tests/test_flowrunner/core/test_base.py
 tests/test_flowrunner/core/test_decorators.py
 tests/test_flowrunner/core/test_helpers.py
+tests/test_flowrunner/core/templates/test_cookiecutter.py
 tests/test_flowrunner/runner/__init__.py
 tests/test_flowrunner/runner/test_flow.py
 tests/test_flowrunner/system/__init__.py
-tests/test_flowrunner/system/test_logger.py
-tests/test_templates/test_cookiecutter.py
+tests/test_flowrunner/system/test_logger.py
```

### Comparing `flowrunner-0.2.2/flowrunner.egg-info/requires.txt` & `flowrunner-0.2.3/flowrunner.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 pre-commit>=3.1.1
 pandas>=1.5.3
 ipython>=8.11.0
 matplotlib>=3.7.1
 pylint>=2.17.0
 pyspark>=3.3.2
 cookiecutter>=2.1.1
-colorama<=0.4.6
+coloredlogs<=15.0.1
+ipytest>=0.13.3
 
 [doc]
 click>=8.1.3
 Jinja2>=3.1.2
 Sphinx>=6.1.3
 sphinxcontrib-mermaid>=0.8.1
 sphinx-autoapi>=2.0.1
@@ -38,15 +39,16 @@
 sphinx-rtd-theme>=1.2.0
 isort>=5.12.0
 black>=23.1.0
 pre-commit>=3.1.1
 coverage<=7.2.1
 pytest>=7.2.1
 pylint>=2.17.0
-colorama<=0.4.6
+coloredlogs<=15.0.1
+ipytest>=0.13.3
 
 [pandas]
 pandas>=1.5.3
 
 [pyspark]
 pyspark>=3.3.2
 
@@ -61,8 +63,9 @@
 pre-commit>=3.1.1
 pandas>=1.5.3
 ipython>=8.11.0
 matplotlib>=3.7.1
 pylint>=2.17.0
 pyspark>=3.3.2
 cookiecutter>=2.1.1
-colorama<=0.4.6
+coloredlogs<=15.0.1
+ipytest>=0.13.3
```

### Comparing `flowrunner-0.2.2/pyproject.toml` & `flowrunner-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [project]
 name = "flowrunner"
 authors = [
     {name = "Prithvijit Guha", email = "prithvijit_guha2@hotmail.com"},
 ]
 
-version = "0.2.2"
+version = "0.2.3"
 
 
 description = "Flowrunner is a lightweight package to organize and represent Data Engineering/Science workflows"
 readme = "readme.md"
 requires-python = ">=3.8"
 keywords = ["Data Engineering", "Data Science"]
 license = {file = "LICENSE"}
@@ -30,14 +30,18 @@
     'Jinja2>=3.1.2',
     'coloredlogs>=15.0.1',
     'ipython>=8.11.0',
     'matplotlib>=3.7.1',
     'cookiecutter>=2.1.1'
 ]
 
+[tool.setuptools]
+packages = [
+    "flowrunner"
+]
 
 
 
 [project.urls]
 Homepage = "https://github.com/prithvijitguha/flowrunner"
 Documentation = "https://flowrunner.readthedocs.io/en/latest/"
 Issues = "https://github.com/prithvijitguha/flowrunner/issues"
@@ -57,15 +61,16 @@
     "sphinx-rtd-theme>=1.2.0",
     "isort>=5.12.0",
     "black>=23.1.0",
     "pre-commit>=3.1.1",
     "coverage<=7.2.1",
     "pytest>=7.2.1",
     "pylint>=2.17.0",
-    "colorama<=0.4.6"
+    "coloredlogs<=15.0.1",
+    "ipytest>=0.13.3"
 ]
 
 dev = [
     "click>=8.1.3",
     "Jinja2>=3.1.2",
     "pylint>=2.16.4",
     "black>=23.1.0",
@@ -76,15 +81,16 @@
     "pre-commit>=3.1.1",
     "pandas>=1.5.3",
     "ipython>=8.11.0",
     "matplotlib>=3.7.1",
     "pylint>=2.17.0",
     "pyspark>=3.3.2",
     "cookiecutter>=2.1.1",
-    "colorama<=0.4.6"
+    "coloredlogs<=15.0.1",
+    "ipytest>=0.13.3"
 ]
 test = [
     "click>=8.1.3",
     "Jinja2>=3.1.2",
     "pytest>=7.2.1",
     "pytest-cookies>=0.7.0",
     "black>=23.1.0",
@@ -93,47 +99,40 @@
     "pre-commit>=3.1.1",
     "pandas>=1.5.3",
     "ipython>=8.11.0",
     "matplotlib>=3.7.1",
     "pylint>=2.17.0",
     "pyspark>=3.3.2",
     "cookiecutter>=2.1.1",
-    "colorama<=0.4.6"
+    "coloredlogs<=15.0.1",
+    "ipytest>=0.13.3"
 ]
 pandas = [
     "pandas>=1.5.3"
 ]
 
 pyspark = [
     "pyspark>=3.3.2"
 ]
 
 
-[options]
-package_dir=[
-    "flowrunner"
-]
-
 
 [options.packages.find]
 where=[
     "flowrunner"
 ]
 
 
 [project.scripts]
 cli = "flowrunner.cli:cli"
 
-[tool.setuptools]
-py-modules = ["flowrunner"]
 
 [tool.pytest.ini_options]
 pythonpath = [
     "flowrunner",
-    "templates",
     "tests"
     ]
 testpaths = [
     "tests"
 ]
 addopts = [
     "--cache-clear",
@@ -157,15 +156,15 @@
 ]
 
 [tool.pylint.main]
 fail-under=6
 ignore-paths = [
     # we skip lintingcheck for docs and examples
     "^examples/.*$",
-    "^docs/source/.*$",
+    "^docs/source/.*$"
 ]
 ignored-modules=[
     "pandas",
     "pytest",
     "flowrunner"
 ]
```

### Comparing `flowrunner-0.2.2/readme.md` & `flowrunner-0.2.3/readme.md`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/.gitignore` & `flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/pyproject.toml` & `flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/readme.md` & `flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/readme.md`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/html_dags/dagsexamplepandas.html` & `flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/html_dags/dagsexamplepandas.html`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/my_flows/pandas_example.py` & `flowrunner-0.2.3/flowrunner/core/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/my_flows/pandas_example.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/tests/test_flowrunner/core/examplepandas.html` & `flowrunner-0.2.3/tests/test_flowrunner/core/examplepandas.html`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/tests/test_flowrunner/core/test_base.py` & `flowrunner-0.2.3/tests/test_flowrunner/core/test_base.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/tests/test_flowrunner/core/test_decorators.py` & `flowrunner-0.2.3/tests/test_flowrunner/core/test_decorators.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/tests/test_flowrunner/core/test_helpers.py` & `flowrunner-0.2.3/tests/test_flowrunner/core/test_helpers.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/tests/test_flowrunner/runner/test_flow.py` & `flowrunner-0.2.3/tests/test_flowrunner/runner/test_flow.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/tests/test_flowrunner/system/test_logger.py` & `flowrunner-0.2.3/tests/test_flowrunner/system/test_logger.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/tests/test_flowrunner/test_cli.py` & `flowrunner-0.2.3/tests/test_flowrunner/test_cli.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.2/tests/test_templates/test_cookiecutter.py` & `flowrunner-0.2.3/tests/test_flowrunner/core/templates/test_cookiecutter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+# -*- coding: utf-8 -*-
 """Module to test that cookie cutter is working as expected"""
 import pytest
 
+# pylint: disable=redefined-outer-name
+
 @pytest.fixture
 def custom_template(tmpdir):
     """Function to create cookie cutter template"""
     template = tmpdir.ensure("cookiecutter-template", dir=True)
     template.join("cookiecutter.json").write('{"repo_name": "example-project"}')
 
     repo_dir = template.ensure("{{cookiecutter.repo_name}}", dir=True)
@@ -17,8 +20,8 @@
     """Test for 'cookiecutter-template'."""
     result = cookies.bake(template=str(custom_template))
 
     assert result.exit_code == 0
     assert result.exception is None
 
     assert result.project_path.name == "example-project"
-    assert result.project_path.is_dir()
+    assert result.project_path.is_dir()
```

