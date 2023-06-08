# Comparing `tmp/ansys-templates-0.3.1.tar.gz` & `tmp/ansys_templates-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-templates-0.3.1.tar", last modified: Sat Jul  9 14:47:20 2022, max compression
+gzip compressed data, was "ansys_templates-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys-templates-0.3.1.tar` & `ansys_templates-0.8.0.tar`

### file list

```diff
@@ -1,145 +1,254 @@
--rw-r--r--   0        0        0     1089 2022-07-09 14:47:02.748433 ansys-templates-0.3.1/LICENSE
--rw-r--r--   0        0        0     7905 2022-07-09 14:47:02.748433 ansys-templates-0.3.1/README.rst
--rw-r--r--   0        0        0     1386 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1042 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/__init__.py
--rw-r--r--   0        0        0      137 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/__main__.py
--rw-r--r--   0        0        0     2280 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/cli.py
--rw-r--r--   0        0        0     1106 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/licenses/LICENSE_MIT
--rw-r--r--   0        0        0      199 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/licenses/__init__.py
--rw-r--r--   0        0        0     2257 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/paths.py
--rw-r--r--   0        0        0      398 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/cookiecutter.json
--rw-r--r--   0        0        0       86 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
--rw-r--r--   0        0        0      265 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0       59 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
--rw-r--r--   0        0        0      298 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0      119 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
--rw-r--r--   0        0        0      594 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
--rw-r--r--   0        0        0     3436 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     2780 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
--rw-r--r--   0        0        0     2982 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      478 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0       11 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0     2689 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       17 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0      282 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0     1052 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
--rw-r--r--   0        0        0      657 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rwxr-xr-x   0        0        0      753 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      970 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       64 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0       50 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rw-r--r--   0        0        0      459 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
--rwxr-xr-x   0        0        0     3506 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0       11 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0     2584 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0      196 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
--rw-r--r--   0        0        0       26 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0       79 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
--rw-r--r--   0        0        0       32 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0     1104 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      140 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     2191 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1076 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/doc_project/cookiecutter.json
--rw-r--r--   0        0        0     2104 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3240 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     1184 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1134 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0        0 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
--rw-r--r--   0        0        0      826 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1560 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
--rw-r--r--   0        0        0     2922 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
--rw-r--r--   0        0        0     1131 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker-compose.yml
--rw-r--r--   0        0        0      731 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0       43 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/README.md
--rw-r--r--   0        0        0       10 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       49 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      110 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       21 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0     1461 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      997 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      186 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      687 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1558 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/cookiecutter.json
--rw-r--r--   0        0        0     3089 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
--rw-r--r--   0        0        0     1132 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker-compose.yml
--rw-r--r--   0        0        0      695 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0       43 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/README.md
--rw-r--r--   0        0        0       10 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       57 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      103 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2022-07-09 14:47:02.752433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       25 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
--rw-r--r--   0        0        0      621 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
--rw-r--r--   0        0        0      525 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
--rw-r--r--   0        0        0       21 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0       28 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1475 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0     1877 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      955 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
--rw-r--r--   0        0        0        0 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     1062 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1557 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/cookiecutter.json
--rw-r--r--   0        0        0     3080 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
--rw-r--r--   0        0        0     1144 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker-compose.yml
--rw-r--r--   0        0        0      862 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0       43 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/README.md
--rw-r--r--   0        0        0       10 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0      630 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
--rw-r--r--   0        0        0       43 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      115 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      265 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0      841 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
--rw-r--r--   0        0        0        0 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1409 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      851 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0       23 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
--rw-r--r--   0        0        0      905 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
--rw-r--r--   0        0        0      408 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
--rw-r--r--   0        0        0        0 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      641 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      961 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1556 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_pkg/cookiecutter.json
--rw-r--r--   0        0        0     2815 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
--rw-r--r--   0        0        0     1138 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/Dockerfile
--rw-r--r--   0        0        0     1121 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker-compose.yaml
--rw-r--r--   0        0        0      445 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0     1299 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
--rw-r--r--   0        0        0      622 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
--rw-r--r--   0        0        0      184 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0     1458 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys/cookiecutter.json
--rw-r--r--   0        0        0     1159 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3462 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1540 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
--rw-r--r--   0        0        0     2480 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
--rw-r--r--   0        0        0     6613 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1879 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
--rw-r--r--   0        0        0     1010 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
--rw-r--r--   0        0        0      241 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0     1599 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
--rw-r--r--   0        0        0     1883 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
--rw-r--r--   0        0        0     1726 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
--rw-r--r--   0        0        0     4317 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
--rw-r--r--   0        0        0        0 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
--rw-r--r--   0        0        0      975 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pybasic/cookiecutter.json
--rw-r--r--   0        0        0     1084 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3221 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      896 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      253 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
--rw-r--r--   0        0        0     2888 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/testing.py
--rw-r--r--   0        0        0     5506 2022-07-09 14:47:02.756433 ansys-templates-0.3.1/src/ansys/templates/utils.py
--rw-r--r--   0        0        0     8607 1970-01-01 00:00:00.000000 ansys-templates-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-06-08 09:01:59.005198 ansys_templates-0.8.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     9947 2023-06-08 09:01:59.005198 ansys_templates-0.8.0/README.rst
+-rw-r--r--   0        0        0     3132 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2266 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/__init__.py
+-rw-r--r--   0        0        0     1284 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/__main__.py
+-rw-r--r--   0        0        0     3776 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/cli.py
+-rw-r--r--   0        0        0     1106 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/licenses/LICENSE_MIT
+-rw-r--r--   0        0        0      199 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/licenses/__init__.py
+-rw-r--r--   0        0        0     3894 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/paths.py
+-rw-r--r--   0        0        0      398 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/cookiecutter.json
+-rw-r--r--   0        0        0       86 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
+-rw-r--r--   0        0        0      356 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
+-rw-r--r--   0        0        0      265 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0       59 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
+-rw-r--r--   0        0        0      418 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0      119 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
+-rw-r--r--   0        0        0      594 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
+-rw-r--r--   0        0        0     3729 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     2779 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
+-rw-r--r--   0        0        0     2987 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      764 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       11 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0     2689 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0      282 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0     1052 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
+-rw-r--r--   0        0        0      657 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rwxr-xr-x   0        0        0     1026 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      969 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       63 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0       50 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rwxr-xr-x   0        0        0     4076 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0      928 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
+-rw-r--r--   0        0        0       11 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     3414 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
+-rw-r--r--   0        0        0       27 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0       81 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
+-rw-r--r--   0        0        0       32 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0     1104 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      140 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     2377 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1087 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/doc_project/cookiecutter.json
+-rw-r--r--   0        0        0     2046 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3238 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     1187 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1134 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0        0 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
+-rw-r--r--   0        0        0      825 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1495 2023-06-08 09:01:59.009198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/cookiecutter.json
+-rw-r--r--   0        0        0     4461 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      283 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0     5008 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3052 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      599 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      453 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       11 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     7566 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      655 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      928 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0     3349 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     4322 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0    38829 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      105 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      421 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0       47 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
+-rw-r--r--   0        0        0       46 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
+-rw-r--r--   0        0        0       47 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
+-rw-r--r--   0        0        0      959 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py
+-rw-r--r--   0        0        0      725 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0    10963 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/monitoring_step.py
+-rw-r--r--   0        0        0    10614 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py
+-rw-r--r--   0        0        0      916 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0     9913 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png
+-rw-r--r--   0        0        0      756 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/style.css
+-rw-r--r--   0        0        0      585 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/colorscale.py
+-rw-r--r--   0        0        0    16026 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_page.py
+-rw-r--r--   0        0        0     2533 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/design_table_page.py
+-rw-r--r--   0        0        0     5572 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/project_summary_page.py
+-rw-r--r--   0        0        0      647 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/result_files_page.py
+-rw-r--r--   0        0        0      962 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/scenery_page.py
+-rw-r--r--   0        0        0      742 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/status_overview_page.py
+-rw-r--r--   0        0        0     4962 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/summary_page.py
+-rw-r--r--   0        0        0    12146 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/monitoring_tabs/visualization_page.py
+-rw-r--r--   0        0        0     5165 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/page.py
+-rw-r--r--   0        0        0    11879 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/problem_setup_page.py
+-rw-r--r--   0        0        0       20 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1498 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1560 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
+-rw-r--r--   0        0        0     2903 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      800 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1132 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       49 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      111 2023-06-08 09:01:59.013198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       21 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0     1461 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      997 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      186 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      687 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1558 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/cookiecutter.json
+-rw-r--r--   0        0        0     3070 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      763 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1133 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       58 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      104 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       25 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
+-rw-r--r--   0        0        0      621 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
+-rw-r--r--   0        0        0      525 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
+-rw-r--r--   0        0        0       21 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0       28 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1475 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0     1877 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      955 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
+-rw-r--r--   0        0        0        0 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     1062 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1557 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json
+-rw-r--r--   0        0        0     3055 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      951 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1145 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0      630 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
+-rw-r--r--   0        0        0       44 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      116 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      265 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0      850 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
+-rw-r--r--   0        0        0        0 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1409 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      851 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0       23 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
+-rw-r--r--   0        0        0      902 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
+-rw-r--r--   0        0        0      408 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      641 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      961 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1556 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json
+-rw-r--r--   0        0        0     2831 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      860 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1129 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0      445 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0     1299 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
+-rw-r--r--   0        0        0      622 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
+-rw-r--r--   0        0        0      184 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0     1458 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys/cookiecutter.json
+-rw-r--r--   0        0        0     1110 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3398 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1540 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
+-rw-r--r--   0        0        0     2619 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     6537 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1879 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
+-rw-r--r--   0        0        0     1010 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      241 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0     1599 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
+-rw-r--r--   0        0        0     1857 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
+-rw-r--r--   0        0        0     1726 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
+-rw-r--r--   0        0        0     4317 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
+-rw-r--r--   0        0        0        0 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
+-rw-r--r--   0        0        0      975 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pybasic/cookiecutter.json
+-rw-r--r--   0        0        0     1035 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3170 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      896 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      253 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1027 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/solution/cookiecutter.json
+-rw-r--r--   0        0        0     2852 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2023-06-08 09:01:59.017198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      187 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.env
+-rw-r--r--   0        0        0      283 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0     5020 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3061 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      599 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      453 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       11 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     8363 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0     1545 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml
+-rw-r--r--   0        0        0      655 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      928 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0     3349 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     3781 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0    35407 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      105 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      583 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0       52 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
+-rw-r--r--   0        0        0       52 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
+-rw-r--r--   0        0        0      803 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0      570 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
+-rw-r--r--   0        0        0      274 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/intro_step.py
+-rw-r--r--   0        0        0      263 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
+-rw-r--r--   0        0        0      916 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0     9913 2023-06-08 09:01:59.021198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/ansys-solutions-horizontal-logo.png
+-rw-r--r--   0        0        0   749872 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/Graphics/solution-workflow-sketch.png
+-rw-r--r--   0        0        0      121 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/style.css
+-rw-r--r--   0        0        0     2030 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/first_page.py
+-rw-r--r--   0        0        0     4695 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/intro_page.py
+-rw-r--r--   0        0        0     5241 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/page.py
+-rw-r--r--   0        0        0      593 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/second_page.py
+-rw-r--r--   0        0        0       20 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1498 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     4035 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/testing.py
+-rw-r--r--   0        0        0     6698 2023-06-08 09:01:59.025198 ansys_templates-0.8.0/src/ansys/templates/utils.py
+-rw-r--r--   0        0        0    11435 1970-01-01 00:00:00.000000 ansys_templates-0.8.0/PKG-INFO
```

### Comparing `ansys-templates-0.3.1/LICENSE` & `ansys_templates-0.8.0/src/ansys/templates/licenses/LICENSE_MIT`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 ANSYS, Inc. All rights reserved.
+Copyright (c) {% now 'utc', '%Y' %} ANSYS, Inc. All rights reserved.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/licenses/LICENSE_MIT` & `ansys_templates-0.8.0/LICENSES/MIT.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 MIT License
 
-Copyright (c) {% now 'utc', '%Y' %} ANSYS, Inc. All rights reserved.
+Copyright (c) 2023 ANSYS, Inc. and/or its affiliates.
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml` & `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml` & `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
       with:
         repo-token: {{ '${{ secrets.GITHUB_TOKEN }}' }}
         sync-labels: ''
 
     # Label based on branch name
     - uses: actions-ecosystem/action-add-labels@v1
       if: |
-        startsWith(github.event.pull_request.head.ref, 'doc') || 
+        startsWith(github.event.pull_request.head.ref, 'doc') ||
         startsWith(github.event.pull_request.head.ref, 'docs')
       with:
         labels: documentation
 
     - uses: actions-ecosystem/action-add-labels@v1
       if: |
         startsWith(github.event.pull_request.head.ref, 'maint') ||
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
 .tox/
 .nox/
+.cov
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml` & `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-0.8.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	exit /b 1
 )
 
 %SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
 goto end
 
 :clean
-rmdir /s /q %BUILDDIR% > /NUL 2>&1 
+rmdir /s /q %BUILDDIR% > /NUL 2>&1
 for /d /r %SOURCEDIR% %%d in (_autosummary) do @if exist "%%d" rmdir /s /q "%%d"
 goto end
 
 :help
 %SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
 
 :end
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 """Sphinx documentation configuration file."""
 from datetime import datetime
+import os
 
+from ansys_sphinx_theme import get_version_match
 {%- if cookiecutter.__logo == "ansys" and cookiecutter.__logo_color == "white" %}
 from ansys_sphinx_theme import ansys_logo_white as logo
 {%- elif cookiecutter.__logo == "ansys" and cookiecutter.__logo_color == "black" %}
 from ansys_sphinx_theme import ansys_logo_black as logo
 {%- elif cookiecutter.__logo == "pyansys" and cookiecutter.__logo_color == "white" %}
 from ansys_sphinx_theme import pyansys_logo_white as logo
 {%- elif cookiecutter.__logo == "pyansys" and cookiecutter.__logo_color == "black" %}
 from ansys_sphinx_theme import pyansys_logo_black as logo
 {%- endif %}
 
+{%- if cookiecutter.__template_name != "doc-project" %}
+from {{cookiecutter.__pkg_namespace}} import __version__
+{%- endif %}
+
+
 # Project information
 {%- if cookiecutter.__template_name in ["doc-project"] %}
 project = "{{ cookiecutter.__project_name_slug }}"
 {%- else %}
 project = "{{ cookiecutter.__pkg_name }}"
 {%- endif %}
 copyright = f"(c) {datetime.now().year} ANSYS, Inc. All rights reserved"
 author = "ANSYS, Inc."
+{%- if cookiecutter.__template_name != "doc-project" %}
+release = version = __version__
+{%- elif cookiecutter.__template_name == "doc-project" %}
 release = version = "{{ cookiecutter.__version }}"
+{%- endif %}
+cname = os.getenv("DOCUMENTATION_CNAME", "docs.pyansys.com")
 
 # Select desired logo, theme, and declare the html title
 html_logo = logo
 html_theme = "ansys_sphinx_theme"
 html_short_title = html_title = "{{ cookiecutter.__project_name_slug }}"
 
 # specify the location of your github repo
@@ -34,28 +46,33 @@
     "additional_breadcrumbs": [
         {%- if cookiecutter.__logo == "ansys" %}
         ("Ansys", "https://dev.docs.ansys.com/"),
         {%- elif cookiecutter.__logo == "pyansys" %}
         ("PyAnsys", "https://docs.pyansys.com/"),
         {%- endif %}
     ],
+    "switcher": {
+        "json_url": f"https://{cname}/versions.json",
+        "version_match": get_version_match(__version__),
+    },
+    "check_switcher": False,
 }
 
 # Sphinx extensions
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "numpydoc",
     "sphinx.ext.intersphinx",
     "sphinx_copybutton",
 ]
 
 # Intersphinx mapping
 intersphinx_mapping = {
-    "python": ("https://docs.python.org/dev", None),
+    "python": ("https://docs.python.org/3", None),
     # kept here as an example
     # "scipy": ("https://docs.scipy.org/doc/scipy/reference", None),
     # "numpy": ("https://numpy.org/devdocs", None),
     # "matplotlib": ("https://matplotlib.org/stable", None),
     # "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
     # "pyvista": ("https://docs.pyvista.org/", None),
     # "grpc": ("https://grpc.github.io/grpc/python/", None),
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -32,27 +32,43 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "importlib-metadata >=4.0",
 ]
 
+[project.optional-dependencies]
+tests = [
+    "pytest==7.3.0",
+    "pytest-cov==4.0.0",
+]
+doc = [
+    "ansys-sphinx-theme==0.9.7",
+    "numpydoc==1.5.0",
+    "sphinx==5.3.0",
+    "sphinx-copybutton==0.5.1",
+]
+
+
 [tool.flit.module]
 name = "{{ cookiecutter.__pkg_namespace }}"
 
 [project.urls]
 Source = "{{ cookiecutter.__repository_url }}"
+Tracker = "{{ cookiecutter.__repository_url }}/issues"
+Homepage = "{{ cookiecutter.__repository_url }}"
+
 {% elif cookiecutter.__build_system == "poetry"  %}
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "{{ cookiecutter.__pkg_name }}"
 version = "{{ cookiecutter.__version }}"
 description = "{{ cookiecutter.__short_description }}"
 license = "MIT"
-authors = ["ANSYS, Inc. <ansys.support@ansys.com>"]
+authors = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 maintainers = ["PyAnsys developers <pyansys.maintainers@ansys.com>"]
 readme = "README.rst"
 repository = "{{ cookiecutter.__repository_url }}"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -61,14 +77,38 @@
 packages = [
     { include = "ansys", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">={{ cookiecutter.__requires_python }},<4.0"
 importlib-metadata = {version = "^4.0", python = "<3.8"}
+
+# Optional documentation dependencies
+[tool.poetry.group.doc]
+optional = true
+
+[tool.poetry.group.doc.dependencies]
+Sphinx = "^5.3.0"
+numpydoc = "^1.5.0"
+ansys-sphinx-theme = "^0.9.7"
+sphinx-copybutton = "^0.5.1"
+
+# Optional testing dependencies
+[tool.poetry.group.tests]
+optional = true
+[tool.poetry.group.tests.dependencies]
+pytest = "^7.3.0"
+pytest-cov = "^4.0.0"
+
+# Optional build requirements
+[tool.poetry.group.build]
+optional = true
+[tool.poetry.group.build.dependencies]
+build = "^0.10.0"
+twine = "^4.0.2"
 {% endif %}
 [tool.black]
 line-length = {{ cookiecutter.__max_linelength }}
 
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys_templates-0.8.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/doc_project/cookiecutter.json` & `ansys_templates-0.8.0/src/ansys/templates/python/doc_project/cookiecutter.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'project_name'": "'doc-project'"}*

```diff
@@ -22,15 +22,15 @@
         "setuptools"
     ],
     "logo": [
         "Ansys",
         "PyAnsys"
     ],
     "max_linelength": "100",
-    "project_name": "",
+    "project_name": "doc-project",
     "repository_url": "https://github.com/pyansys/{{ cookiecutter.__project_name_slug }}",
     "requires_python": [
         "3.7",
         "3.8",
         "3.9",
         "3.10"
     ],
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/doc_project/hooks/post_gen_project.py` & `ansys_templates-0.8.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,27 +20,25 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".github/dependabot.yml",
     ".github/labeler.yml",
     ".github/labels.yml",
     ".github/workflows/ci_cd.yml",
     ".github/workflows/label.yml",
     ".gitignore",
     "LICENSE",
     "README.rst",
     ".pre-commit-config.yaml",
-    "ignore_words.txt",
     "requirements/requirements_build.txt",
     "requirements/requirements_doc.txt",
     "tox.ini",
 ]
 """A list holding all desired files to be included in the project."""
 
 
@@ -59,17 +57,17 @@
 
     # Apply isort with desired config
     isort_config = isort.settings.Config(
         line_length="{{ cookiecutter.__max_linelength }}",
         profile="black",
     )
     filepaths_list = [
-        project_path / "doc/source/conf.py",
+        project_path / "doc" / "source" / "conf.py",
     ]
     for filepath in filepaths_list:
-        isort.api.sort_file(filepath, isort_config)
+        isort.api.sort_file(filepath, config=isort_config)
 
     # Apply the desired structure to the project
     keep_files(DESIRED_STRUCTURE)
 
 if __name__ == "__main__":
     main()
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         run: tox -e style
 
   docs-style:
     name: Documentation Style Check
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
-  
+
       - name: Running Vale
         uses: errata-ai/vale-action@reviewdog
         env:
           GITHUB_TOKEN: {{ '${{secrets.GITHUB_TOKEN}}' }}
         with:
           files: doc
           reporter: github-pr-check
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 repos:
 
 - repo: https://github.com/psf/black
-  rev: 22.3.0
+  rev: 23.1.0
   hooks:
   - id: black
-    args: ["doc/source/conf.py"]
+    args: ["doc/"]
 
 - repo: https://github.com/pycqa/isort
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
   - id: isort
     args: [
       "--profile", "black",
       "--force-sort-within-sections",
       "--line-length", "100",
     ]
 
 - repo: https://gitlab.com/PyCQA/flake8
-  rev: 3.9.2
+  rev: 6.0.0
   hooks:
   - id: flake8
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.1.0
+  rev: v2.2.2
   hooks:
   - id: codespell
-    args: [--ignore-words=ignore_words.txt, -S \*.pyc\,\*.xml\,\*.txt\,\*.gif\,\*.png\,\*.jpg\,\*.js\,\*.html\,\*.doctree\,\*.ttf\,\*.woff\,\*.woff2\,\*.eot\,\*.mp4\,\*.inv\,\*.pickle\,\*.ipynb\,flycheck\*\,./.git/\*\,./.hypothesis/\*\,\*.yml\,./doc/build/\*\,./doc/images/\*\,./dist/\*\,\*~\,.hypothesis\*\,./doc/source/examples/\*\,\*cover\,\*.dat\,\*.mac]
+    args: [--ignore-words=doc/styles/Vocab/ANSYS/accept.txt, -S \*.pyc\,\*.xml\,\*.txt\,\*.gif\,\*.png\,\*.jpg\,\*.js\,\*.html\,\*.doctree\,\*.ttf\,\*.woff\,\*.woff2\,\*.eot\,\*.mp4\,\*.inv\,\*.pickle\,\*.ipynb\,flycheck\*\,./.git/\*\,./.hypothesis/\*\,\*.yml\,./doc/build/\*\,./doc/images/\*\,./dist/\*\,\*~\,.hypothesis\*\,./doc/source/examples/\*\,\*cover\,\*.dat\,\*.mac]
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.1.0
+  rev: v4.4.0
   hooks:
   - id: check-merge-conflict
   - id: debug-statements
 
 - repo: https://github.com/python-jsonschema/check-jsonschema
-  rev: 0.16.0
+  rev: 0.21.0
   hooks:
     - id: check-github-workflows
       name: "Check GitHub workflows"
       files: ^\.github/workflows/
       types: [yaml]
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-0.8.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 
 [testenv:doc]
 description = Checks if project documentation properly builds
 skip_install = false
 deps =
     -r{toxinidir}/requirements/requirements_doc.txt
 allowlist_externals=*
-commands = 
+commands =
     sphinx-build -d "{toxworkdir}/doc_doctree" doc/source "{toxworkdir}/doc_out_html" --color -vW -b html
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/cookiecutter.json` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,19 +16,16 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
-    "docker/Dockerfile",
-    "docker/README.md",
     ".flake8",
     ".gitattributes",
     ".gitignore",
     "LICENSE",
     ".pre-commit-config.yaml",
     "pyproject.toml",
     "README.rst",
@@ -40,16 +37,15 @@
     "src/_version.py",
     "src/server.py",
     "src/models/__init__.py",
     "src/observability/logger.py",
     "tests/test_metadata.py",
     "tests/test_server.py",
     "tests/conftest.py",
-    "tox.ini",
-    "docker-compose.yml",
+    "tox.ini"
 ]
 """A list holding all desired files to be included in the project."""
 
 
 def main():
     """Entry point of the script."""
     # Get baked project location path
@@ -88,16 +84,18 @@
         )
     if ci_cd == 'Azure DevOps':
         DESIRED_STRUCTURE.append("azure-pipeline.yml")
 
     # Remove docker non desired files
     enable_docker = "{{ cookiecutter.enable_docker }}"
     if enable_docker == 'Yes':
+        DESIRED_STRUCTURE.append("docker/compose.yaml")
         DESIRED_STRUCTURE.append("docker/Dockerfile")
-        DESIRED_STRUCTURE.append("docker/README.md")
+        DESIRED_STRUCTURE.append("docker/Docker.md")
+        DESIRED_STRUCTURE.append(".dockerignore")
 
     # Remove non-desired files
     keep_files(DESIRED_STRUCTURE)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker-compose.yml` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 version: '3.9'
 
 services:
-  {{ cookiecutter.library_name }}-api:
-    image: {{ cookiecutter.__project_name_slug }}/{{ cookiecutter.__library_name_slug }}-api
+
+  {{ cookiecutter.library_name }}:
+    image: {{ cookiecutter.__project_name_slug }}/{{ cookiecutter.__library_name_slug }}
     build:
-      context: .
+      context: ..
       dockerfile: ./docker/Dockerfile
-    ports:
-      - "50050:80"
+    stdin_open: true
+    tty: true
     networks:
       - {{ cookiecutter.__project_name_slug }}
 
 {% if cookiecutter.enable_full_observability_stack == 'Yes' -%}
 
   # OPENTELEMETRY COLLECTOR
 
   otel-collector:
-    image: otel/opentelemetry-collector-contrib:latest
+    image: otel/opentelemetry-collector-contrib:0.55.0
     command: [ "--config=/etc/otel-collector-config.yaml" ]
     volumes:
       - ./_deploy/otel-collector-config.yaml:/etc/otel-collector-config.yaml
       - /mnt/{{ cookiecutter.__project_name_slug }}/AppData/Local/Otel:/etc/output:rw # Store the logs
     ports:
       - "8888:8888"   # Prometheus metrics exposed by the collector
       - "8889:8889"   # Prometheus exporter metrics
@@ -30,8 +31,8 @@
       - {{ cookiecutter.__project_name_slug }}
 {% endif %}
 
 
 
 networks:
   {{ cookiecutter.__project_name_slug }}:
-    name: {{ cookiecutter.__project_name_slug }}-stream
+    name: {{ cookiecutter.__project_name_slug }}-stream
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-FROM python:{{ cookiecutter.requires_python }} AS base
+# ---------------------------
+FROM python:{{ cookiecutter.requires_python }}-slim AS base
 
+# Keeps Python from generating .pyc files in the container
 ENV PYTHONDONTWRITEBYTECODE=1
-ENV PYTHONUNBUFFERED=1
 
-RUN apt-get update && apt-get install -y
+# Turns off buffering for easier container logging
+ENV PYTHONUNBUFFERED=1
 
-RUN mkdir /app
-RUN mkdir /src
+RUN apt-get update \
+    && apt-get install -y \
+    && rm -rf /var/lib/apt/lists/*
 
-COPY ../src /app/src/
-COPY requirements/requirements_build.txt /app/src/
+COPY requirements/requirements_build.txt ./
 
-WORKDIR /app/src
+RUN pip install --no-cache-dir --upgrade pip && \
+    pip install --no-cache-dir -r requirements_build.txt
 
-RUN python -m pip install --no-cache-dir --upgrade pip
-RUN python -m pip install --no-cache-dir -r requirements_build.txt
+WORKDIR /app
 
+# ---------------------------
 FROM base AS test
 
-COPY requirements/requirements_tests.txt ./
+COPY requirements/requirements_test.txt ./
 
-RUN pip install --no-cache-dir -r requirements_tests.txt
+RUN pip install --no-cache-dir -r requirements_test.txt
 
-COPY /tests ../tests/
-
-WORKDIR /app
+COPY . .
 
 RUN pytest tests
 
-
+# ---------------------------
 FROM base AS final
+LABEL org.opencontainers.image.authors={{ cookiecutter.__project_name_slug }}
 
-LABEL org.opencontainers.image.authors=ericsson
-
-EXPOSE 80
+COPY src .
 
-ENTRYPOINT [ "uvicorn", "server:app", "--host", "0.0.0.0", "--port", "80" ]
+ENTRYPOINT [ "python", "main.py" ]
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/cookiecutter.json` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".gitattributes",
     ".gitignore",
     "LICENSE",
     ".pre-commit-config.yaml",
@@ -40,21 +39,18 @@
     "src/blueprints/__init__.py",
     "src/blueprints/health.py",
     "src/blueprints/version.py",
     "src/models/__init__.py",
     "src/observability/__init__.py",
     "src/observability/logger.py",
     "src/static/swagger.json",
-    "docker/Dockerfile",
-    "docker/README.md",
     "tests/test_metadata.py",
     "tests/test_server.py",
     "tests/conftest.py",
-    "tox.ini",
-    "docker-compose.yml",
+    "tox.ini"
 ]
 """A list holding all desired files to be included in the project."""
 
 
 def main():
     """Entry point of the script."""
     # Get baked project location path
@@ -93,16 +89,18 @@
         )
     if ci_cd == 'Azure DevOps':
         DESIRED_STRUCTURE.append("azure-pipeline.yml")
 
     # Remove docker non desired files
     enable_docker = "{{ cookiecutter.enable_docker }}"
     if enable_docker == 'Yes':
+        DESIRED_STRUCTURE.append("docker/compose.yaml")
         DESIRED_STRUCTURE.append("docker/Dockerfile")
-        DESIRED_STRUCTURE.append("docker/README.md")
+        DESIRED_STRUCTURE.append("docker/Docker.md")
+        DESIRED_STRUCTURE.append(".dockerignore")
 
     # Remove non-desired files
     keep_files(DESIRED_STRUCTURE)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker-compose.yml` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 version: '3.9'
 
 services:
   {{ cookiecutter.library_name }}-api:
     image: {{ cookiecutter.__project_name_slug }}/{{ cookiecutter.__library_name_slug }}-api
     build:
-      context: .
+      context: ..
       dockerfile: ./docker/Dockerfile
     ports:
-      - "5000:5000"
+      - "50050:80"
     networks:
       - {{ cookiecutter.__project_name_slug }}
 
 {% if cookiecutter.enable_full_observability_stack == 'Yes' -%}
 
   # OPENTELEMETRY COLLECTOR
 
   otel-collector:
-    image: otel/opentelemetry-collector-contrib:latest
+    image: otel/opentelemetry-collector-contrib:0.55.0
     command: [ "--config=/etc/otel-collector-config.yaml" ]
     volumes:
       - ./_deploy/otel-collector-config.yaml:/etc/otel-collector-config.yaml
       - /mnt/{{ cookiecutter.__project_name_slug }}/AppData/Local/Otel:/etc/output:rw # Store the logs
     ports:
       - "8888:8888"   # Prometheus metrics exposed by the collector
       - "8889:8889"   # Prometheus exporter metrics
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-FROM python:{{ cookiecutter.requires_python }} AS base
+# ---------------------------
+FROM python:{{ cookiecutter.requires_python }}-slim AS base
 
 ENV PYTHONDONTWRITEBYTECODE=1
 ENV PYTHONUNBUFFERED=1
 
-RUN apt-get update && apt-get install -y
+RUN apt-get update \
+    && apt-get install -y \
+    && rm -rf /var/lib/apt/lists/*
 
-RUN mkdir /app
-RUN mkdir /src
-
-COPY ../src/ /app/src/
-COPY requirements/requirements_build.txt /app/src/
+WORKDIR /app
 
-WORKDIR /app/src
+COPY requirements/requirements_build.txt .
 
-RUN python -m pip install --no-cache-dir --upgrade pip
-RUN python -m pip install --no-cache-dir -r requirements_build.txt
+RUN pip install --no-cache-dir --upgrade pip && \
+    pip install --no-cache-dir -r requirements_build.txt
 
+# ---------------------------
 FROM base AS test
 
-COPY requirements/requirements_tests.txt ./
+COPY requirements/requirements_tests.txt .
 
-RUN pip install --no-cache-dir -r requirements_tests.txt
+RUN pip install --no-cache-dir -r requirements_test.txt
 
-COPY /tests ../tests/
-
-WORKDIR /app
+COPY . .
 
 RUN pytest tests
 
-
+# ---------------------------
 FROM base AS final
-
-LABEL org.opencontainers.image.authors=ericsson
+LABEL org.opencontainers.image.authors={{ cookiecutter.__project_name_slug }}
 
 EXPOSE 5000
 
+COPY src .
+
 ENTRYPOINT [ "python", "server.py" ]
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/cookiecutter.json` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".gitattributes",
     ".gitignore",
     "LICENSE",
     ".pre-commit-config.yaml",
@@ -43,16 +42,15 @@
     "src/services/__init__.py",
     "src/services/pinger.py",
     "src/stubs/__init__.py",
     "tests/test_metadata.py",
     "tox.ini",
     "protobufs/pingerserver.proto",
     "tests/test_server.py",
-    "tests/conftest.py",
-    "docker-compose.yml",
+    "tests/conftest.py"
 ]
 """A list holding all desired files to be included in the project."""
 
 
 def main():
     """Entry point of the script."""
     # Get baked project location path
@@ -91,17 +89,18 @@
         )
     if ci_cd == 'Azure DevOps':
         DESIRED_STRUCTURE.append("azure-pipeline.yml")
 
     # Remove docker non desired files
     enable_docker = "{{ cookiecutter.enable_docker }}"
     if enable_docker == 'Yes':
-        DESIRED_STRUCTURE.append("docker-compose.yml")
+        DESIRED_STRUCTURE.append("docker/compose.yaml")
         DESIRED_STRUCTURE.append("docker/Dockerfile")
-        DESIRED_STRUCTURE.append("docker/README.md")
+        DESIRED_STRUCTURE.append("docker/Docker.md")
+        DESIRED_STRUCTURE.append(".dockerignore")
 
     # Remove non-desired files
     keep_files(DESIRED_STRUCTURE)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker-compose.yml` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 version: '3.9'
 
 services:
   {{ cookiecutter.library_name }}-grpc-api:
     image: {{ cookiecutter.__project_name_slug }}/{{ cookiecutter.__library_name_slug }}-grpc-api
     build:
-      context: .
+      context: ..
       dockerfile: ./docker/Dockerfile
     ports:
       - "50051:50051"
     networks:
       - {{ cookiecutter.__project_name_slug }}
 
 {% if cookiecutter.enable_full_observability_stack == 'Yes' -%}
 
   # OPENTELEMETRY COLLECTOR
 
   otel-collector:
-    image: otel/opentelemetry-collector-contrib:latest
+    image: otel/opentelemetry-collector-contrib:0.55.0
     command: [ "--config=/etc/otel-collector-config.yaml" ]
     volumes:
       - ./_deploy/otel-collector-config.yaml:/etc/otel-collector-config.yaml
       - /mnt/{{ cookiecutter.__project_name_slug }}/AppData/Local/Otel:/etc/output:rw # Store the logs
     ports:
       - "8888:8888"   # Prometheus metrics exposed by the collector
       - "8889:8889"   # Prometheus exporter metrics
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 from pathlib import Path
 import sys
 
 import grpc
 
 sys.path.insert(0, os.path.join(Path(os.path.dirname(os.path.realpath(__file__))).parent, "stubs"))
 
-import pingserver_pb2
-import pingserver_pb2_grpc
+import stubs.pingserver_pb2 as pb2
+import stubs.pingserver_pb2_grpc as pb2_grpc
 
 
 def run():
     """Run client."""
     with grpc.insecure_channel("localhost:50051") as channel:
-        stub = pingserver_pb2_grpc.PingerStub(channel)
-        response = stub.WhoPing(pingserver_pb2.UserRequest(name="you"))
+        stub = pb2_grpc.PingerStub(channel)
+        response = stub.WhoPing(pb2.UserRequest(name="you"))
     print(response.message)
 
 
 if __name__ == "__main__":
     logging.basicConfig()
     run()
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 {% endif %}
 
 """
 {{ cookiecutter.project_name }}.
 
 {{ cookiecutter.library_name }}
 """
-import pingserver_pb2
-import pingserver_pb2_grpc
+from stubs.pingserver_pb2 import PingReply
+from stubs.pingserver_pb2_grpc import PingerServicer
 
 NumberPing = 0
 
 
-class Pinger(pingserver_pb2_grpc.PingerServicer):
+class Pinger(PingerServicer):
     """Pinger class."""
 
     def PingServer(self, request, context):
         """Ping the server."""
         global NumberPing
         NumberPing += 1
-        return pingserver_pb2.PingReply(
+        return PingReply(
             message=f"Hello, the server is healthy and it had been pinged {NumberPing} times!"
         )
 
     def WhoPing(self, request, context):
         """Check who ping the server."""
         global NumberPing
         NumberPing += 1
-        return pingserver_pb2.PingReply(message=f"Hello, the server is pinged by {request.name}!")
+        return PingReply(message=f"Hello, the server is pinged by {request.name}!")
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_pkg/cookiecutter.json` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".gitattributes",
     ".gitignore",
     "LICENSE",
     ".pre-commit-config.yaml",
@@ -36,17 +35,15 @@
     "setup.py",
     "src/__init__.py",
     "src/logger.py",
     "src/main.py",
     "tests/test_metadata.py",
     "tox.ini",
     "tests/__init__.py",
-    "tests/conftest.py",
-    "Dockerfile",
-    "docker-compose.yaml",
+    "tests/conftest.py"
 ]
 """A list holding all desired files to be included in the project."""
 
 
 def main():
     """Entry point of the script."""
     # Get baked project location path
@@ -85,16 +82,18 @@
         )
     if ci_cd == 'Azure DevOps':
         DESIRED_STRUCTURE.append("azure-pipeline.yml")
 
     # Remove docker non desired files
     enable_docker = "{{ cookiecutter.enable_docker }}"
     if enable_docker == 'Yes':
-        DESIRED_STRUCTURE.append("Dockerfile")
-        DESIRED_STRUCTURE.append("docker-compose.yml")
+        DESIRED_STRUCTURE.append("docker/compose.yaml")
+        DESIRED_STRUCTURE.append("docker/Dockerfile")
+        DESIRED_STRUCTURE.append("docker/Docker.md")
+        DESIRED_STRUCTURE.append(".dockerignore")
 
     # Remove non-desired files
     keep_files(DESIRED_STRUCTURE)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/Dockerfile` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 # ---------------------------
 FROM python:{{ cookiecutter.requires_python }}-slim AS base
 
-# Keeps Python from generating .pyc files in the container
 ENV PYTHONDONTWRITEBYTECODE=1
-
-# Turns off buffering for easier container logging
 ENV PYTHONUNBUFFERED=1
 
-RUN apt-get update && apt-get install -y
+RUN apt-get update \
+    && apt-get install -y \
+    && rm -rf /var/lib/apt/lists/*
+
+WORKDIR /app
 
-COPY requirements/requirements.txt ./
+COPY requirements/requirements_build.txt .
 
 RUN pip install --no-cache-dir --upgrade pip && \
-    pip install --no-cache-dir -r requirements.txt
+    pip install --no-cache-dir -r requirements_build.txt
 
-WORKDIR /app
+RUN mkdir stubs
+
+ADD protobufs/ ./protobufs/
+RUN python -m grpc_tools.protoc  \
+    -I ./protobufs  \
+    --python_out=./stubs \
+    --grpc_python_out=./stubs  \
+    ./protobufs/*.proto
 
 # ---------------------------
 FROM base AS test
 
-COPY requirements/requirements_test.txt ./
+COPY requirements/requirements_tests.txt .
 
 RUN pip install --no-cache-dir -r requirements_test.txt
 
 COPY . .
 
 RUN pytest tests
 
 # ---------------------------
 FROM base AS final
 LABEL org.opencontainers.image.authors={{ cookiecutter.__project_name_slug }}
 
-COPY src .
+EXPOSE 50051
 
-# Creates a non-root user with an explicit UID and adds permission to access the /app folder
-# For more info, please refer to https://aka.ms/vscode-docker-python-configure-containers
-# TODO Disable to be able to write to /var/log/
-# RUN adduser -u 5678 --disabled-password --gecos "" appuser && chown -R appuser /app
-# USER appuser
+COPY src .
 
-ENTRYPOINT [ "python", "main.py" ]
+ENTRYPOINT [ "python", "server.py" ]
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker-compose.yaml` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-version: '3.5'
+version: '3.9'
 
 services:
-
-  {{ cookiecutter.library_name }}:
-    image: {{ cookiecutter.__project_name_slug }}/{{ cookiecutter.__library_name_slug }}
+  {{ cookiecutter.library_name }}-api:
+    image: {{ cookiecutter.__project_name_slug }}/{{ cookiecutter.__library_name_slug }}-api
     build:
-      context: .
-      dockerfile: ./Dockerfile
-    stdin_open: true
-    tty: true
+      context: ..
+      dockerfile: ./docker/Dockerfile
+    ports:
+      - "5000:5000"
     networks:
       - {{ cookiecutter.__project_name_slug }}
 
 {% if cookiecutter.enable_full_observability_stack == 'Yes' -%}
 
   # OPENTELEMETRY COLLECTOR
 
   otel-collector:
-    image: otel/opentelemetry-collector-contrib:latest
+    image: otel/opentelemetry-collector-contrib:0.55.0
     command: [ "--config=/etc/otel-collector-config.yaml" ]
     volumes:
       - ./_deploy/otel-collector-config.yaml:/etc/otel-collector-config.yaml
       - /mnt/{{ cookiecutter.__project_name_slug }}/AppData/Local/Otel:/etc/output:rw # Store the logs
     ports:
       - "8888:8888"   # Prometheus metrics exposed by the collector
       - "8889:8889"   # Prometheus exporter metrics
@@ -31,8 +30,8 @@
       - {{ cookiecutter.__project_name_slug }}
 {% endif %}
 
 
 
 networks:
   {{ cookiecutter.__project_name_slug }}:
-    name: {{ cookiecutter.__project_name_slug }}-stream
+    name: {{ cookiecutter.__project_name_slug }}-stream
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyansys/cookiecutter.json` & `ansys_templates-0.8.0/src/ansys/templates/python/pyansys/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyansys/hooks/post_gen_project.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
     "LICENSE",
     "pyproject.toml",
     "README.rst",
     "requirements_build.txt",
     "requirements_doc.txt",
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-0.8.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -20,66 +20,66 @@
 
 For developers
 ^^^^^^^^^^^^^^
 
 Installing Py{{ cookiecutter.product_name }} {{ cookiecutter.library_name }} in developer mode allows
 you to modify the source and enhance it.
 
-Before contributing to the project, please refer to the `PyAnsys Developer's guide`_. You will 
+Before contributing to the project, please refer to the `PyAnsys Developer's guide`_. You will
 need to follow these steps:
 
 #. Start by cloning this repository:
 
-    .. code:: bash
+   .. code:: bash
 
-        git clone {{ cookiecutter.repository_url }}
+      git clone {{ cookiecutter.repository_url }}
 
 #. Create a fresh-clean Python environment and activate it. Refer to the
    official `venv`_ documentation if you require further information:
 
-    .. code:: bash
+   .. code:: bash
 
-        # Create a virtual environment
-        python -m venv .venv
+      # Create a virtual environment
+      python -m venv .venv
 
-        # Activate it in a POSIX system
-        source .venv/bin/activate
+      # Activate it in a POSIX system
+      source .venv/bin/activate
 
-        # Activate it in Windows CMD environment
-        .venv\Scripts\activate.bat
+      # Activate it in Windows CMD environment
+      .venv\Scripts\activate.bat
 
-        # Activate it in Windows Powershell
-        .venv\Scripts\Activate.ps1
+      # Activate it in Windows Powershell
+      .venv\Scripts\Activate.ps1
 
 #. Make sure you have the latest version of `pip`_:
 
-    .. code:: bash
+   .. code:: bash
 
-        python -m pip install -U pip
+      python -m pip install -U pip
 
 #. Install the project in editable mode:
 
-    .. code:: bash
-    
-        python -m pip install --editable {{ cookiecutter.__pkg_name }}
+   .. code:: bash
+
+      python -m pip install --editable {{ cookiecutter.__pkg_name }}
 
 #. Install additional requirements (if needed):
 
-     .. code:: bash
+   .. code:: bash
 
-        python -m pip install -r requirements/requirements_build.txt
-        python -m pip install -r requirements/requirements_doc.txt
-        python -m pip install -r requirements/requirements_tests.txt
+      python -m pip install -r requirements/requirements_build.txt
+      python -m pip install -r requirements/requirements_doc.txt
+      python -m pip install -r requirements/requirements_tests.txt
 
 #. Finally, verify your development installation by running:
 
-    .. code:: bash
-        
-        python -m pip install -r requirements/requirements_tests.txt
-        pytest tests -v
+   .. code:: bash
+
+      python -m pip install -r requirements/requirements_tests.txt
+      pytest tests -v
 
 
 Style and Testing
 -----------------
 
 If required, you can always call the style commands (`black`_, `isort`_,
 `flake8`_...) or unit testing ones (`pytest`_) from the command line. However,
@@ -109,18 +109,18 @@
 
 .. code:: bash
 
     python -m pip install -r requirements/requirements_build.txt
 
 Then, you can execute:
 
-    .. code:: bash
+.. code:: bash
 
-        python -m build
-        python -m twine check dist/*
+    python -m build
+    python -m twine check dist/*
 
 
 .. LINKS AND REFERENCES
 .. _black: https://github.com/psf/black
 .. _flake8: https://flake8.pycqa.org/en/latest/
 .. _isort: https://github.com/PyCQA/isort
 .. _PyAnsys Developer's guide: https://dev.docs.pyansys.com/
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyansys_advanced/cookiecutter.json` & `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Post-processing script for cleaning the raw rendered project."""
 import os
 import shutil
 from pathlib import Path
 
 import isort
 
-from ansys.templates.utils import keep_files
+from ansys.templates.utils import keep_files, remove_file
 
 ALLOWED_BUILD_SYSTEMS = ["flit", "poetry", "setuptools"]
 """A list of all allowed build systems by the template."""
 
 DESIRED_STRUCTURE = [
     "CHANGELOG.md",
     "CODE_OF_CONDUCT.md",
@@ -19,32 +19,28 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".github/dependabot.yml",
     ".github/labeler.yml",
     ".github/labels.yml",
     ".github/workflows/ci_cd.yml",
     ".github/workflows/label.yml",
     ".gitattributes",
     ".gitignore",
     "LICENSE",
     ".pre-commit-config.yaml",
     "pyproject.toml",
     "README.rst",
-    "requirements/requirements_build.txt",
-    "requirements/requirements_doc.txt",
-    "requirements/requirements_tests.txt",
     "src/ansys/{{ cookiecutter.__product_name_slug }}/{{ cookiecutter.__library_name_slug }}/__init__.py",
     "tests/test_metadata.py",
     "tox.ini",
 ]
 """A list holding all desired files to be included in the project."""
 
 def main():
@@ -52,20 +48,27 @@
     # Get baked project location path
     project_path = Path(os.getcwd())
 
     # Get the desired build system
     build_system = "{{ cookiecutter.build_system }}"
 
     # Move all requirements files into a requirements/ directory
-    os.mkdir(project_path / "requirements")
     requirements_files = [
-            f"requirements_{name}.txt" for name in ["build", "doc", "tests"]
+        f"requirements_{name}.txt" for name in ["build", "doc", "tests"]
     ]
-    for file in requirements_files:
-        shutil.move(str(project_path / file), str(project_path / "requirements"))
+    if build_system == "poetry":
+        # Poetry required and extra dependencies are collected inside the
+        # 'pyproject.toml' file. Thus, there is no need to have requirements
+        # files
+        for file in requirements_files:
+            remove_file(file, project_path)
+    else:
+        os.mkdir(project_path / "requirements")
+        for file in requirements_files:
+            shutil.move(str(project_path / file), str(project_path / "requirements"))
 
     # Apply isort with desired config
     isort_config = isort.settings.Config(
         line_length="{{ cookiecutter.__max_linelength }}",
         profile="black",
     )
     filepaths_list = [
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 {{ '=' * (cookiecutter.__project_name_slug | length) }}
 |pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
-.. |python| image:: https://img.shields.io/badge/Python-%3E%3D{{cookiecutter.__requires_python}}-blue
+.. |python| image:: https://img.shields.io/pypi/pyversions/{{cookiecutter.__project_name_slug}}?logo=pypi
    :target: https://pypi.org/project/{{cookiecutter.__project_name_slug}}/
    :alt: Python
 
 .. |pypi| image:: https://img.shields.io/pypi/v/{{cookiecutter.__project_name_slug}}.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/{{cookiecutter.__project_name_slug}}
    :alt: PyPI
 
@@ -58,88 +58,88 @@
     python -m pip install {{ cookiecutter.__pkg_name }}
 
 {% elif cookiecutter.build_system == "poetry" -%}
 
 .. code:: bash
 
     poetry run python -m pip install {{ cookiecutter.__pkg_name }}
-    
+
 {% endif -%}
 
 
 For developers
 ^^^^^^^^^^^^^^
 
 Installing Py{{ cookiecutter.product_name }} {{ cookiecutter.library_name }} in developer mode allows
 you to modify the source and enhance it.
 
-Before contributing to the project, please refer to the `PyAnsys Developer's guide`_. You will 
+Before contributing to the project, please refer to the `PyAnsys Developer's guide`_. You will
 need to follow these steps:
 
 #. Start by cloning this repository:
 
-    .. code:: bash
+   .. code:: bash
 
-        git clone {{ cookiecutter.repository_url }}
+      git clone {{ cookiecutter.repository_url }}
 
 #. Create a fresh-clean Python environment and activate it:
 
-    .. code:: bash
+   .. code:: bash
 
-        # Create a virtual environment
-        python -m venv .venv
+      # Create a virtual environment
+      python -m venv .venv
 
-        # Activate it in a POSIX system
-        source .venv/bin/activate
+      # Activate it in a POSIX system
+      source .venv/bin/activate
 
-        # Activate it in Windows CMD environment
-        .venv\Scripts\activate.bat
+      # Activate it in Windows CMD environment
+      .venv\Scripts\activate.bat
 
-        # Activate it in Windows Powershell
-        .venv\Scripts\Activate.ps1
+      # Activate it in Windows Powershell
+      .venv\Scripts\Activate.ps1
 
 #. Make sure you have the latest required build system and doc, testing, and CI tools:
 
-    .. code:: bash
+   .. code:: bash
 
-        python -m pip install -U pip {{ cookiecutter.build_system }} tox
-        python -m pip install -r requirements/requirements_build.txt
-        python -m pip install -r requirements/requirements_doc.txt
-        python -m pip install -r requirements/requirements_tests.txt
+      python -m pip install -U pip {{ cookiecutter.build_system }} tox
+      python -m pip install -r requirements/requirements_build.txt
+      python -m pip install -r requirements/requirements_doc.txt
+      python -m pip install -r requirements/requirements_tests.txt
 
 
 #. Install the project in editable mode:
 
     {% if cookiecutter.build_system in ["flit", "setuptools"] -%}
-    
-    .. code:: bash
-    
-        python -m pip install --editable {{ cookiecutter.__pkg_name }}
-    
+
+   .. code:: bash
+
+      python -m pip install --editable {{ cookiecutter.__pkg_name }}
+
     {% elif cookiecutter.build_system == "poetry" -%}
-    
-    .. code:: bash
-    
-        poetry run python -m pip install {{ cookiecutter.__pkg_name }}
-        
+
+   .. code:: bash
+
+      poetry run python -m pip install {{ cookiecutter.__pkg_name }}
+
     {% endif -%}
 
 #. Finally, verify your development installation by running:
 
-    .. code:: bash
-        
-        tox
+   .. code:: bash
+
+      tox
 
 
 How to testing
 --------------
 
 This project takes advantage of `tox`_. This tool allows to automate common
 development tasks (similar to Makefile) but it is oriented towards Python
-development. 
+development.
 
 Using tox
 ^^^^^^^^^
 
 As Makefile has rules, `tox`_ has environments. In fact, the tool creates its
 own virtual environment so anything being tested is isolated from the project in
 order to guarantee project's integrity. The following environments commands are provided:
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json` & `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml` & `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml` & `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml`

 * *Files 9% similar despite different names*

```diff
@@ -18,36 +18,36 @@
     steps:
     - name: Get Bot Application Token
       id: get_workflow_token
       uses: peter-murray/workflow-application-token-action@v1
       with:
         application_id: {{ '${{ secrets.BOT_APPLICATION_ID }}' }}
         application_private_key: {{ '${{ secrets.BOT_APPLICATION_PRIVATE_KEY }}' }}
-    
+
     - uses: actions/checkout@v2
       with:
         token: {{ '${{ steps.get_workflow_token.outputs.token }}' }}
-    
+
     - name: Set up JDK 11
       uses: actions/setup-java@v2
       with:
         java-version: '11'
         distribution: 'adopt'
         cache: maven
-    
+
     - name: Clean library folder
       run: rm -rf {{ cookiecutter.__pkg_name }}
-      
+
     - name: Build client library
       run: mvn -Dbuild-id={{ '${{ github.run_number }}' }} -s .m2/settings.xml compile
       env:
         MAVEN_OPTS: "-Dlog4j2.formatMsgNoLookups=true"
         SERVER_USERNAME: {{ '${{ secrets.REPO_USER }}' }}
         SERVER_PASSWORD: {{ '${{ secrets.REPO_TOKEN }}' }}
-        
+
     - name: Create Pull Request
       uses: peter-evans/create-pull-request@v3
       with:
         commit-message: Update client library
         committer: GitHub <noreply@github.com>
         author: {{ '${{ github.actor }}' }} <{{ '${{ github.actor }}' }}@users.noreply.github.com>
         signoff: false
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml` & `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml` & `ansys_templates-0.8.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pybasic/cookiecutter.json` & `ansys_templates-0.8.0/src/ansys/templates/python/pybasic/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pybasic/hooks/post_gen_project.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     "doc/.vale.ini",
     "doc/styles/.gitignore",
     "doc/styles/Vocab/ANSYS/accept.txt",
     "doc/styles/Vocab/ANSYS/reject.txt",
     "doc/source/conf.py",
     "doc/source/index.rst",
     "doc/source/_static/README.md",
-    "doc/source/_templates/sidebar-nav-bs.html",
     "doc/source/_templates/README.md",
     "examples/README.md",
     ".flake8",
     ".gitattributes",
     ".gitignore",
     "LICENSE",
     "pyproject.toml",
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-0.8.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -22,62 +22,62 @@
 ^^^^^^^^^^^^^^
 
 Before contributing to the project, please refer to the `PyAnsys Developer's
 guide`_. You will need to follow these steps:
 
 #. Start by cloning this repository:
 
-    .. code:: bash
+   .. code:: bash
 
-        git clone {{ cookiecutter.repository_url }}
+      git clone {{ cookiecutter.repository_url }}
 
 #. Create a fresh-clean Python environment and activate it. Refer to the
    official `venv`_ documentation if you require further information:
 
-    .. code:: bash
+   .. code:: bash
 
-        # Create a virtual environment
-        python -m venv .venv
+      # Create a virtual environment
+      python -m venv .venv
 
-        # Activate it in a POSIX system
-        source .venv/bin/activate
+      # Activate it in a POSIX system
+      source .venv/bin/activate
 
-        # Activate it in Windows CMD environment
-        .venv\Scripts\activate.bat
+      # Activate it in Windows CMD environment
+      .venv\Scripts\activate.bat
 
-        # Activate it in Windows Powershell
-        .venv\Scripts\Activate.ps1
+      # Activate it in Windows Powershell
+      .venv\Scripts\Activate.ps1
 
 #. Make sure you have the latest version of `pip`_:
 
-    .. code:: bash
+   .. code:: bash
 
-        python -m pip install -U pip
+      python -m pip install -U pip
 
 #. Install the project in editable mode:
 
-    .. code:: bash
-    
-        python -m pip install --editable {{ cookiecutter.__pkg_name }}
+   .. code:: bash
+
+      python -m pip install --editable {{ cookiecutter.__pkg_name }}
 
 #. Install additional requirements (if needed):
 
-     .. code:: bash
+   .. code:: bash
 
-        python -m pip install -r requirements_build.txt
-        python -m pip install -r requirements_doc.txt
-        python -m pip install -r requirements_tests.txt
+      python -m pip install -r requirements_build.txt
+      python -m pip install -r requirements_doc.txt
+      python -m pip install -r requirements_tests.txt
 
 
 #. Finally, verify your development installation by running:
 
-    .. code:: bash
-        
-        python -m pip install -r requirements_tests.txt
-        pytest tests -vv
+   .. code:: bash
+
+      python -m pip install -r requirements_tests.txt
+      pytest tests -vv
 
 
 Style and Testing
 -----------------
 
 If required, you can always call the style commands (`black`_, `isort`_,
 `flake8`_...) or unit testing ones (`pytest`_) from the command line. However,
```

### Comparing `ansys-templates-0.3.1/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys_templates-0.8.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-templates-0.3.1/src/ansys/templates/testing.py` & `ansys_templates-0.8.0/src/ansys/templates/testing.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+# Copyright (C) 2023 ANSYS, Inc. and/or its affiliates.
+# SPDX-License-Identifier: MIT
+#
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """A collection of routines focused on testing."""
 
 import os
 
 from ansys.templates.utils import bake_template
```

### Comparing `ansys-templates-0.3.1/PKG-INFO` & `ansys_templates-0.8.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-Metadata-Version: 2.1
-Name: ansys-templates
-Version: 0.3.1
-Summary: Creates Python projects according to PyAnsys guidelines
-Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
-Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Dist: importlib-metadata >=4.0
-Requires-Dist: click>=7.0,<8.0.0
-Requires-Dist: cookiecutter>=2.1.0
-Requires-Dist: isort>=5.10.1
-Project-URL: Source, https://github.com/pyansys/pyansys-template
-
-Welcome to Ansys templates
-==========================
-|pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
+.. Copyright (C) 2023 ANSYS, Inc. and/or its affiliates.
+.. SPDX-License-Identifier: MIT
+..
+..
+.. Permission is hereby granted, free of charge, to any person obtaining a copy
+.. of this software and associated documentation files (the "Software"), to deal
+.. in the Software without restriction, including without limitation the rights
+.. to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+.. copies of the Software, and to permit persons to whom the Software is
+.. furnished to do so, subject to the following conditions:
+..
+.. The above copyright notice and this permission notice shall be included in all
+.. copies or substantial portions of the Software.
+..
+.. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+.. IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+.. FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+.. AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+.. LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+.. OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+.. SOFTWARE.
+
+Ansys templates
+===============
+|ansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
 
-.. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
-   :target: https://docs.pyansys.com/
+.. |ansys| image:: https://img.shields.io/badge/Ansys-ffc107.svg?labelColor=black&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
+   :target: https://github.com/ansys
    :alt: PyAnsys
 
-.. |python| image:: https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+.. |python| image:: https://img.shields.io/pypi/pyversions/ansys-templates?logo=pypi
    :target: https://pypi.org/project/ansys-templates/
    :alt: Python
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-templates.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-templates/
    :alt: PyPI
 
@@ -44,14 +48,16 @@
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
    :target: https://github.com/psf/black
    :alt: Black
 
+.. |implemented| image:: <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24"><path d="M21.03 5.72a.75.75 0 0 1 0 1.06l-11.5 11.5a.747.747 0 0 1-1.072-.012l-5.5-5.75a.75.75 0 1 1 1.084-1.036l4.97 5.195L19.97 5.72a.75.75 0 0 1 1.06 0Z"></path></svg>
+
 
 The ``ansys-templates`` repository holds a collection of useful templates compliant
 with PyAnsys guidelines. It also provides the ``ansys-templates`` command line tool
 for interactively generating new projects based on previous templates.
 
 The main advantages of using this tool are:
 
@@ -59,25 +65,25 @@
 - Output of the project can easily be customized during the rendering process.
 - Generated projects are compliant with `PyAnsys Developer's Guidelines`_.
 
 .. _PyAnsys Developer's Guidelines: https://dev.docs.pyansys.com/
 
 For information on using this tool, see the `Ansys Templates Documentation`_.
 
-.. _Ansys Templates Documentation: https://templates.pyansys.com/ 
+.. _Ansys Templates Documentation: https://templates.ansys.com/
 
 .. image:: https://github.com/ansys/ansys-templates/raw/main/doc/source/_static/basic_usage.gif
 
 
 How to install
 --------------
 Users can install ``ansys-templates`` by running:
 
 .. code-block:: text
-        
+
     python -m pip install ansys-templates
 
 The usage of `pipx`_ is encouraged too. See `installing ansys-templates using
 pipx`_.
 
 .. _pipx: https://pypa.github.io/pipx/
 .. _installing ansys-templates using pipx: https://templates.pyansys.com/getting_started/index.html#installing-pipx
@@ -87,28 +93,28 @@
 --------------
 The following commands are provided with ``ansys-templates``:
 
 - ``ansys-templates --help``: lists information about the tool.
 - ``ansys-templates list``: lists all available templates.
 - ``ansys-templates new <template name>``: creates a new project from template.
 
-
 Available templates
 -------------------
 Available templates in ``ansys-templates`` are:
 
 - ``doc-project``: Create a documentation project using Sphinx.
 - ``pybasic``: Create a basic Python Package.
 - ``pyansys``: Create a PyAnsys Python Package project.
 - ``pyansys-advanced``: Create an advanced PyAnsys Python Package project.
 - ``pyansys-openapi-client``: Create an OpenAPI Client Package project.
 - ``pyace``: Create a Python project for any method developers.
 - ``pyace-flask``: Create a Flask project initialized for any developer.
 - ``pyace-grpc``: Create gRPC project initialized for any developer.
 - ``pyace-fast``: Create a FastAPI project initialized for any developer.
+- ``solution``: Create a Solution based on the Solution Application Framework. **For Ansys Internal Use Only**
 
 
 Template features
 -----------------
 The following table summarizes the main properties for each of the templates
 available in ``ansys-templates``:
 
@@ -129,15 +135,19 @@
 +-------------------------+-----------------------+-----------------+---------+----------+----------------+---------+
 | pyace-fast              |  ``X``                |  ``X``          |  ``X``  |  ``X``   |  ``X``         |  ``X``  |
 +-------------------------+-----------------------+-----------------+---------+----------+----------------+---------+
 | pyace-flask             |  ``X``                |  ``X``          |  ``X``  |  ``X``   |  ``X``         |  ``X``  |
 +-------------------------+-----------------------+-----------------+---------+----------+----------------+---------+
 | pyace-grpc              |  ``X``                |  ``X``          |  ``X``  |  ``X``   |  ``X``         |  ``X``  |
 +-------------------------+-----------------------+-----------------+---------+----------+----------------+---------+
+| solution "*"            |                       |  ``X``          |  ``X``  |  ``X``   |  ``X``         |         |
++-------------------------+-----------------------+-----------------+---------+----------+----------------+---------+
 
+.. warning::
+    "*" This template is for **Ansys Internal Use Only**.
 
 Demo branches
 -------------
 To have a better idea on how each template will look once it gets rendered, see
 its corresponding demonstration branch.
 
 * Demo branch for `doc-project`_
@@ -146,19 +156,24 @@
 * Demo branch for `pyansys-advanced using flit`_
 * Demo branch for `pyansys-advanced using poetry`_
 * Demo branch for `pyansys-advanced using setuptools`_
 * Demo branch for `pyace`_
 * Demo branch for `pyace-fast`_
 * Demo branch for `pyace-flask`_
 * Demo branch for `pyace-grpc`_
+* Demo branch for `solution`_
+* Demo branch for `osl-solution`_
+
 
 .. _doc-project: https://github.com/ansys/ansys-templates/tree/demo/doc-project
 .. _pybasic: https://github.com/ansys/ansys-templates/tree/demo/pybasic
 .. _pyansys: https://github.com/ansys/ansys-templates/tree/demo/pyansys
 .. _pyansys-advanced using flit: https://github.com/ansys/ansys-templates/tree/demo/pyansys-advanced-flit
 .. _pyansys-advanced using poetry: https://github.com/ansys/ansys-templates/tree/demo/pyansys-advanced-poetry
 .. _pyansys-advanced using setuptools: https://github.com/ansys/ansys-templates/tree/demo/pyansys-advanced-setuptools
 .. _pyace: https://github.com/ansys/ansys-templates/tree/demo/pyace-pkg
 .. _pyace-fast: https://github.com/ansys/ansys-templates/tree/demo/pyace-fast
 .. _pyace-flask: https://github.com/ansys/ansys-templates/tree/demo/pyace-flask
 .. _pyace-grpc: https://github.com/ansys/ansys-templates/tree/demo/pyace-grpc
+.. _solution: https://github.com/ansys/ansys-templates/tree/demo/solution
+.. _osl-solution: https://github.com/ansys/ansys-templates/tree/demo/solution
```

