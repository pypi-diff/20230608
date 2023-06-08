# Comparing `tmp/dls-servbase-1.7.0.tar.gz` & `tmp/dls-servbase-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-servbase-1.7.0.tar", last modified: Wed Jun  7 14:24:08 2023, max compression
+gzip compressed data, was "dls-servbase-1.7.1.tar", last modified: Thu Jun  8 08:17:51 2023, max compression
```

## Comparing `dls-servbase-1.7.0.tar` & `dls-servbase-1.7.1.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.635095 dls-servbase-1.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.603094 dls-servbase-1.7.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.603094 dls-servbase-1.7.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/docs/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.603094 dls-servbase-1.7.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.603094 dls-servbase-1.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.599094 dls-servbase-1.7.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.603094 dls-servbase-1.7.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.607095 dls-servbase-1.7.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.607095 dls-servbase-1.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.607095 dls-servbase-1.7.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-07 14:24:08.631095 dls-servbase-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.607095 dls-servbase-1.7.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.599094 dls-servbase-1.7.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.607095 dls-servbase-1.7.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.607095 dls-servbase-1.7.0/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/explanations/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/explanations/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/explanations/todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.611095 dls-servbase-1.7.0/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/how-to/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/how-to/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/how-to/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/how-to/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/how-to/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.611095 dls-servbase-1.7.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.611095 dls-servbase-1.7.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/reference/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/reference/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.611095 dls-servbase-1.7.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/docs/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:24:08.635095 dls-servbase-1.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.599094 dls-servbase-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.611095 dls-servbase-1.7.0/src/dls_servbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-07 14:24:08.000000 dls-servbase-1.7.0/src/dls_servbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-07 14:24:08.000000 dls-servbase-1.7.0/src/dls_servbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:24:08.000000 dls-servbase-1.7.0/src/dls_servbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-07 14:24:08.000000 dls-servbase-1.7.0/src/dls_servbase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-07 14:24:08.000000 dls-servbase-1.7.0/src/dls_servbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-07 14:24:08.000000 dls-servbase-1.7.0/src/dls_servbase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.615095 dls-servbase-1.7.0/src/dls_servbase_api/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.615095 dls-servbase-1.7.0/src/dls_servbase_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.615095 dls-servbase-1.7.0/src/dls_servbase_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.615095 dls-servbase-1.7.0/src/dls_servbase_api/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_api/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.615095 dls-servbase-1.7.0/src/dls_servbase_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.615095 dls-servbase-1.7.0/src/dls_servbase_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.619095 dls-servbase-1.7.0/src/dls_servbase_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 14:24:08.000000 dls-servbase-1.7.0/src/dls_servbase_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    30611 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.619095 dls-servbase-1.7.0/src/dls_servbase_lib/cookies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/cookies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/cookies/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/cookies/cookie_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/cookies/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/cookies/dataface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.623095 dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/normsql.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.623095 dls-servbase-1.7.0/src/dls_servbase_lib/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.623095 dls-servbase-1.7.0/src/dls_servbase_lib/guis/html/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.627095 dls-servbase-1.7.0/src/dls_servbase_lib/guis/html/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/guis/html/javascript/version.js
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/src/dls_servbase_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.627095 dls-servbase-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/base_context_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/base_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:24:08.631095 dls-servbase-1.7.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/configurations/mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/configurations/sqlite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/test_dataface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/test_dataface_takeover.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-07 14:23:55.000000 dls-servbase-1.7.0/tests/test_parse_cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.092016 dls-servbase-1.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.072016 dls-servbase-1.7.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.072016 dls-servbase-1.7.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.072016 dls-servbase-1.7.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.072016 dls-servbase-1.7.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.064015 dls-servbase-1.7.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.072016 dls-servbase-1.7.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.072016 dls-servbase-1.7.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.076016 dls-servbase-1.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.076016 dls-servbase-1.7.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-08 08:17:51.092016 dls-servbase-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.076016 dls-servbase-1.7.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.068016 dls-servbase-1.7.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.076016 dls-servbase-1.7.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.076016 dls-servbase-1.7.1/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.080016 dls-servbase-1.7.1/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.080016 dls-servbase-1.7.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.080016 dls-servbase-1.7.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.080016 dls-servbase-1.7.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 08:17:51.092016 dls-servbase-1.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.068016 dls-servbase-1.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.080016 dls-servbase-1.7.1/src/dls_servbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-06-08 08:17:51.000000 dls-servbase-1.7.1/src/dls_servbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-08 08:17:51.000000 dls-servbase-1.7.1/src/dls_servbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:17:51.000000 dls-servbase-1.7.1/src/dls_servbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-08 08:17:51.000000 dls-servbase-1.7.1/src/dls_servbase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-08 08:17:51.000000 dls-servbase-1.7.1/src/dls_servbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-08 08:17:51.000000 dls-servbase-1.7.1/src/dls_servbase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.084015 dls-servbase-1.7.1/src/dls_servbase_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.084015 dls-servbase-1.7.1/src/dls_servbase_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.084015 dls-servbase-1.7.1/src/dls_servbase_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.084015 dls-servbase-1.7.1/src/dls_servbase_api/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_api/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.084015 dls-servbase-1.7.1/src/dls_servbase_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.084015 dls-servbase-1.7.1/src/dls_servbase_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.088016 dls-servbase-1.7.1/src/dls_servbase_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 08:17:50.000000 dls-servbase-1.7.1/src/dls_servbase_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30611 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.088016 dls-servbase-1.7.1/src/dls_servbase_lib/cookies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/cookies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/cookies/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/cookies/cookie_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/cookies/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/cookies/dataface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.088016 dls-servbase-1.7.1/src/dls_servbase_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/datafaces/normsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.092016 dls-servbase-1.7.1/src/dls_servbase_lib/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.092016 dls-servbase-1.7.1/src/dls_servbase_lib/guis/html/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/guis/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.092016 dls-servbase-1.7.1/src/dls_servbase_lib/guis/html/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/guis/html/javascript/version.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/src/dls_servbase_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.092016 dls-servbase-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/tests/base_context_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/tests/base_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:17:51.092016 dls-servbase-1.7.1/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/tests/configurations/mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/tests/configurations/sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/tests/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/tests/test_dataface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/tests/test_dataface_takeover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-08 08:17:39.000000 dls-servbase-1.7.1/tests/test_parse_cookie.py
```

### Comparing `dls-servbase-1.7.0/.dae-devops/Makefile` & `dls-servbase-1.7.1/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.dae-devops/docs/conventions.rst` & `dls-servbase-1.7.1/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.dae-devops/docs/developing.rst` & `dls-servbase-1.7.1/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.dae-devops/docs/devops.rst` & `dls-servbase-1.7.1/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.dae-devops/docs/docs_structure.rst` & `dls-servbase-1.7.1/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.dae-devops/docs/documenting.rst` & `dls-servbase-1.7.1/.dae-devops/docs/documenting.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.dae-devops/docs/installing.rst` & `dls-servbase-1.7.1/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.dae-devops/docs/testing.rst` & `dls-servbase-1.7.1/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.dae-devops/project.yaml` & `dls-servbase-1.7.1/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.devcontainer/Dockerfile` & `dls-servbase-1.7.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.devcontainer/devcontainer.json` & `dls-servbase-1.7.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.github/CONTRIBUTING.rst` & `dls-servbase-1.7.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.github/actions/install_requirements/action.yml` & `dls-servbase-1.7.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.github/dependabot.yml` & `dls-servbase-1.7.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.github/pages/make_switcher.py` & `dls-servbase-1.7.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.github/workflows/code.yml` & `dls-servbase-1.7.1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.github/workflows/docs.yml` & `dls-servbase-1.7.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.github/workflows/docs_clean.yml` & `dls-servbase-1.7.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.github/workflows/linkcheck.yml` & `dls-servbase-1.7.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.gitignore` & `dls-servbase-1.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.gitlab-ci.yml` & `dls-servbase-1.7.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/.vscode/launch.json` & `dls-servbase-1.7.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/LICENSE` & `dls-servbase-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/PKG-INFO` & `dls-servbase-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-servbase
-Version: 1.7.0
+Version: 1.7.1
 Summary: Simple HTTP service for database operations.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-servbase-1.7.0/docs/conf.py` & `dls-servbase-1.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/docs/images/dls-favicon.ico` & `dls-servbase-1.7.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/docs/images/dls-logo.svg` & `dls-servbase-1.7.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/pyproject.toml` & `dls-servbase-1.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase.egg-info/PKG-INFO` & `dls-servbase-1.7.1/src/dls_servbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-servbase
-Version: 1.7.0
+Version: 1.7.1
 Summary: Simple HTTP service for database operations.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-servbase-1.7.0/src/dls_servbase.egg-info/SOURCES.txt` & `dls-servbase-1.7.1/src/dls_servbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_api/aiohttp_client.py` & `dls-servbase-1.7.1/src/dls_servbase_api/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_api/databases/database_definition.py` & `dls-servbase-1.7.1/src/dls_servbase_api/databases/database_definition.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_api/databases/table_definitions.py` & `dls-servbase-1.7.1/src/dls_servbase_api/databases/table_definitions.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_api/datafaces/aiohttp.py` & `dls-servbase-1.7.1/src/dls_servbase_api/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_api/datafaces/context.py` & `dls-servbase-1.7.1/src/dls_servbase_api/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_api/datafaces/datafaces.py` & `dls-servbase-1.7.1/src/dls_servbase_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_api/guis/aiohttp.py` & `dls-servbase-1.7.1/src/dls_servbase_api/guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_api/guis/context.py` & `dls-servbase-1.7.1/src/dls_servbase_api/guis/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_api/guis/guis.py` & `dls-servbase-1.7.1/src/dls_servbase_api/guis/guis.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_cli/main.py` & `dls-servbase-1.7.1/src/dls_servbase_cli/main.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_cli/subcommands/base.py` & `dls-servbase-1.7.1/src/dls_servbase_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_cli/subcommands/service.py` & `dls-servbase-1.7.1/src/dls_servbase_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_cli/version.py` & `dls-servbase-1.7.1/src/dls_servbase_cli/version.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_lib/__main__.py` & `dls-servbase-1.7.1/src/dls_servbase_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_lib/base_aiohttp.py` & `dls-servbase-1.7.1/src/dls_servbase_lib/base_aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_lib/cookies/base.py` & `dls-servbase-1.7.1/src/dls_servbase_lib/cookies/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_lib/cookies/cookie_parser.py` & `dls-servbase-1.7.1/src/dls_servbase_lib/cookies/cookie_parser.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_lib/cookies/cookies.py` & `dls-servbase-1.7.1/src/dls_servbase_lib/cookies/cookies.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_lib/cookies/dataface.py` & `dls-servbase-1.7.1/src/dls_servbase_lib/cookies/dataface.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/aiohttp.py` & `dls-servbase-1.7.1/src/dls_servbase_lib/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/context.py` & `dls-servbase-1.7.1/src/dls_servbase_lib/datafaces/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,30 +59,30 @@
 
         # Not running as a service?
         elif start_as == "direct":
             # We need to activate the tick() task.
             await self.server.activate()
 
     # ----------------------------------------------------------------------------------------
-    async def aexit(self, type, value, traceback) -> None:
+    async def aexit(self, type=None, value=None, traceback=None):
         """
         Asyncio context exit.
 
         Stop service if one was started and releases any client resources.
         """
+        logger.debug(f"[DISSHU] {thing_type} aexit")
 
         if self.server is not None:
             start_as = self.context_specification.get("start_as")
 
             if start_as == "process":
-                logger.info(
-                    "[DISSHU] in context exit, sending shutdown to client process"
-                )
-                # Put in request to shutdown the server.
-                await self.server.client_shutdown()
-                logger.info("[DISSHU] in context exit, sent shutdown to client process")
+                # The server associated with this context is running?
+                if await self.is_process_alive():
+                    logger.debug(f"[DISSHU] {thing_type} calling client_shutdown")
+                    # Put in request to shutdown the server.
+                    await self.server.client_shutdown()
 
             if start_as == "coro":
                 await self.server.direct_shutdown()
 
             if start_as == "direct":
                 await self.server.deactivate()
```

### Comparing `dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/datafaces.py` & `dls-servbase-1.7.1/src/dls_servbase_lib/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_lib/datafaces/normsql.py` & `dls-servbase-1.7.1/src/dls_servbase_lib/datafaces/normsql.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_lib/envvar.py` & `dls-servbase-1.7.1/src/dls_servbase_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_lib/guis/aiohttp.py` & `dls-servbase-1.7.1/src/dls_servbase_lib/guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_lib/guis/context.py` & `dls-servbase-1.7.1/src/dls_servbase_lib/guis/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,16 +33,27 @@
         elif self.context_specification.get("start_as") == "thread":
             await self.server.start_thread()
 
         elif self.context_specification.get("start_as") == "process":
             await self.server.start_process()
 
     # ----------------------------------------------------------------------------------------
-    async def aexit(self, type, value, traceback):
-        """ """
+    async def aexit(self, type=None, value=None, traceback=None):
+        """
+        Asyncio context exit.
+
+        Stop service if one was started and releases any client resources.
+        """
+        logger.debug(f"[DISSHU] {thing_type} aexit")
 
         if self.server is not None:
-            # Put in request to shutdown the server.
-            await self.server.client_shutdown()
+            start_as = self.context_specification.get("start_as")
+
+            if start_as == "process":
+                # The server associated with this context is running?
+                if await self.is_process_alive():
+                    logger.debug(f"[DISSHU] {thing_type} calling client_shutdown")
+                    # Put in request to shutdown the server.
+                    await self.server.client_shutdown()
 
-            # Release a client connection if we had one.
-            await self.server.close_client_session()
+            if start_as == "coro":
+                await self.server.direct_shutdown()
```

### Comparing `dls-servbase-1.7.0/src/dls_servbase_lib/guis/guis.py` & `dls-servbase-1.7.1/src/dls_servbase_lib/guis/guis.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/src/dls_servbase_lib/version.py` & `dls-servbase-1.7.1/src/dls_servbase_lib/version.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/tests/base_context_tester.py` & `dls-servbase-1.7.1/tests/base_context_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/tests/base_tester.py` & `dls-servbase-1.7.1/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/tests/configurations/mysql.yaml` & `dls-servbase-1.7.1/tests/configurations/mysql.yaml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/tests/configurations/sqlite.yaml` & `dls-servbase-1.7.1/tests/configurations/sqlite.yaml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/tests/conftest.py` & `dls-servbase-1.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/tests/test_aiohttp.py` & `dls-servbase-1.7.1/tests/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/tests/test_cli.py` & `dls-servbase-1.7.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/tests/test_database.py` & `dls-servbase-1.7.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/tests/test_dataface.py` & `dls-servbase-1.7.1/tests/test_dataface.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/tests/test_dataface_takeover.py` & `dls-servbase-1.7.1/tests/test_dataface_takeover.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/tests/test_gui.py` & `dls-servbase-1.7.1/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.7.0/tests/test_parse_cookie.py` & `dls-servbase-1.7.1/tests/test_parse_cookie.py`

 * *Files identical despite different names*

