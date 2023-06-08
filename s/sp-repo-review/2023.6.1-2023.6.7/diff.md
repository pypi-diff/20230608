# Comparing `tmp/sp_repo_review-2023.6.1.tar.gz` & `tmp/sp_repo_review-2023.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Wed Jun  7 22:19:41 2023, max compression
```

## Comparing `sp_repo_review-2023.6.1.tar` & `sp_repo_review-2023.6.7.tar`

### file list

```diff
@@ -1,108 +1,116 @@
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/.readthedocs.yml
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/.ruby-version
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/Gemfile
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/Gemfile.lock
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/_config.yml
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/cookiecutter.json
--rw-r--r--   0        0        0     6729 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/noxfile.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/.github/dependabot.yml
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/.github/workflows/reusable-change-detection.yml
--rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/.github/workflows/reusable-cookie.yml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/.github/workflows/reusable-rr-tests.yml
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/LICENSE
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/README.md
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/_includes/head.html
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/_includes/head_custom.html
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/_includes/interactive_repo_review.html
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/_includes/rr.html
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/_includes/toc.html
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/_sass/color_schemes/skhep.scss
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/_sass/custom/custom.scss
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/assets/favicon.ico
--rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/assets/images/logo.svg
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/assets/js/tabs.js
--rw-r--r--   0        0        0     9750 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/assets/js/webapp.js
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/index.md
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/guides/coverage.md
--rw-r--r--   0        0        0    11293 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/guides/gha_basic.md
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/guides/gha_pure.md
--rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/guides/gha_wheels.md
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/guides/index.md
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/guides/mypy.md
--rw-r--r--   0        0        0     8853 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/guides/nox.md
--rw-r--r--   0        0        0    17927 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/guides/packaging_classic.md
--rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/guides/packaging_simple.md
--rw-r--r--   0        0        0    14552 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/guides/pytest.md
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/guides/repo_review.md
--rw-r--r--   0        0        0    28595 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/guides/style.md
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/guides/writing-docs.md
--rw-r--r--   0        0        0     7027 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/patterns/data_files.md
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/patterns/index.md
--rw-r--r--   0        0        0    11200 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/principles/design.md
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/principles/index.md
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/principles/process.md
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/tutorials/dev-environment.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/tutorials/index.md
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/tutorials/module.md
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/tutorials/packaging.md
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/docs/pages/tutorials/test.md
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/hooks/post_gen_project.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/src/sp_repo_review/__init__.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/src/sp_repo_review/families.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/src/sp_repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/src/sp_repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/src/sp_repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/src/sp_repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/src/sp_repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/src/sp_repo_review/checks/__init__.py
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/src/sp_repo_review/checks/general.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/src/sp_repo_review/checks/github.py
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/src/sp_repo_review/checks/mypy.py
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/src/sp_repo_review/checks/precommit.py
--rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/src/sp_repo_review/checks/pyproject.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/src/sp_repo_review/checks/ruff.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/tests/test_cmd.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/tests/test_package.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.gitattributes
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.readthedocs.yml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/CMakeLists-skbuild.txt
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/Cargo-maturin.toml
--rw-r--r--   0        0        0    14162 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/LICENSE
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/MANIFEST-setuptools,pybind11.in
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/meson-mesonpy.build
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/noxfile.py
--rw-r--r--   0        0        0     8580 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/setup-pybind11.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/setup-setuptools,pybind11.cfg
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/setup-setuptools.py
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.github/matchers/pylint.json
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.github/workflows/wheels-pybind11,skbuild,mesonpy,maturin.yml
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/docs/conf.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/docs/index.rst
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/src/lib-maturin.rs
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/src/main-pybind11,skbuild,mesonpy.cpp
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_core-pybind11,skbuild,mesonpy,maturin.pyi
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_version-setuptools,pybind11.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/py.typed
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_compat/__init__.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_compat/typing.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/tests/test_compiled-pybind11,skbuild,mesonpy,maturin.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/tests/test_package.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/LICENSE
--rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/README.md
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/pyproject.toml
--rw-r--r--   0        0        0    10879 2020-02-02 00:00:00.000000 sp_repo_review-2023.6.1/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.gitattributes
+-rw-r--r--   0        0        0     2227 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      179 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      571 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.readthedocs.yml
+-rw-r--r--   0        0        0        6 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.ruby-version
+-rw-r--r--   0        0        0     1294 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/Gemfile
+-rw-r--r--   0        0        0     2171 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/Gemfile.lock
+-rw-r--r--   0        0        0     8658 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/README.md
+-rw-r--r--   0        0        0     1160 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/_config.yml
+-rw-r--r--   0        0        0      763 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/action.yml
+-rw-r--r--   0        0        0      563 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/cookiecutter.json
+-rw-r--r--   0        0        0     7033 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/noxfile.py
+-rw-r--r--   0        0        0      640 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/dependabot.yml
+-rw-r--r--   0        0        0      726 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1219 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2018 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/reusable-change-detection.yml
+-rw-r--r--   0        0        0     5153 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/reusable-cookie.yml
+-rw-r--r--   0        0        0      919 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.github/workflows/reusable-rr-tests.yml
+-rw-r--r--   0        0        0      251 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/LICENSE
+-rw-r--r--   0        0        0      730 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/README.md
+-rw-r--r--   0        0        0     2180 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/head.html
+-rw-r--r--   0        0        0     1019 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/head_custom.html
+-rw-r--r--   0        0        0      547 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/interactive_repo_review.html
+-rw-r--r--   0        0        0       92 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/rr.html
+-rw-r--r--   0        0        0      150 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_includes/toc.html
+-rw-r--r--   0        0        0       22 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_sass/color_schemes/skhep.scss
+-rw-r--r--   0        0        0     2611 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/_sass/custom/custom.scss
+-rw-r--r--   0        0        0    15086 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     8070 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0      652 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/js/tabs.js
+-rw-r--r--   0        0        0    10234 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/assets/js/webapp.js
+-rw-r--r--   0        0        0     2219 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/index.md
+-rw-r--r--   0        0        0     4512 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/coverage.md
+-rw-r--r--   0        0        0    11293 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/gha_basic.md
+-rw-r--r--   0        0        0     9205 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/gha_pure.md
+-rw-r--r--   0        0        0     8224 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/gha_wheels.md
+-rw-r--r--   0        0        0     2162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/index.md
+-rw-r--r--   0        0        0     8606 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/mypy.md
+-rw-r--r--   0        0        0    17927 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/packaging_classic.md
+-rw-r--r--   0        0        0     9182 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/packaging_simple.md
+-rw-r--r--   0        0        0    14552 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/pytest.md
+-rw-r--r--   0        0        0      932 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/repo_review.md
+-rw-r--r--   0        0        0    28595 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/style.md
+-rw-r--r--   0        0        0     8853 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/tasks.md
+-rw-r--r--   0        0        0     5310 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/guides/writing-docs.md
+-rw-r--r--   0        0        0     7027 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/patterns/data_files.md
+-rw-r--r--   0        0        0      517 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/patterns/index.md
+-rw-r--r--   0        0        0    11200 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/principles/design.md
+-rw-r--r--   0        0        0      561 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/principles/index.md
+-rw-r--r--   0        0        0     2209 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/principles/process.md
+-rw-r--r--   0        0        0     4816 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/dev-environment.md
+-rw-r--r--   0        0        0      998 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/index.md
+-rw-r--r--   0        0        0     2557 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/module.md
+-rw-r--r--   0        0        0     3272 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/packaging.md
+-rw-r--r--   0        0        0     4621 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/docs/pages/tutorials/test.md
+-rw-r--r--   0        0        0     1063 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      168 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      228 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/__init__.py
+-rw-r--r--   0        0        0      166 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_version.py
+-rw-r--r--   0        0        0      118 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_version.pyi
+-rw-r--r--   0        0        0      753 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/families.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0      290 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/__init__.py
+-rw-r--r--   0        0        0     2849 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/general.py
+-rw-r--r--   0        0        0     5018 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/github.py
+-rw-r--r--   0        0        0     4133 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/mypy.py
+-rw-r--r--   0        0        0     3162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/precommit.py
+-rw-r--r--   0        0        0     5339 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/pyproject.py
+-rw-r--r--   0        0        0     2868 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/src/sp_repo_review/checks/ruff.py
+-rw-r--r--   0        0        0      412 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/tests/test_cmd.py
+-rw-r--r--   0        0        0      597 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/tests/test_package.py
+-rw-r--r--   0        0        0      125 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.gitattributes
+-rw-r--r--   0        0        0     2218 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0     2930 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      456 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.readthedocs.yml
+-rw-r--r--   0        0        0      280 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/CMakeLists-skbuild.txt
+-rw-r--r--   0        0        0      685 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/Cargo-maturin.toml
+-rw-r--r--   0        0        0    14162 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/LICENSE
+-rw-r--r--   0        0        0      123 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/MANIFEST-setuptools,pybind11.in
+-rw-r--r--   0        0        0     1910 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      909 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/meson-mesonpy.build
+-rw-r--r--   0        0        0     2312 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/noxfile.py
+-rw-r--r--   0        0        0     8580 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      723 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-pybind11.py
+-rw-r--r--   0        0        0     1980 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-setuptools,pybind11.cfg
+-rw-r--r--   0        0        0      374 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-setuptools.py
+-rw-r--r--   0        0        0     2533 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      163 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     3414 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1573 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/wheels-pybind11,skbuild,mesonpy,maturin.yml
+-rw-r--r--   0        0        0     2031 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/docs/conf.py
+-rw-r--r--   0        0        0      286 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/docs/index.rst
+-rw-r--r--   0        0        0      562 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/lib-maturin.rs
+-rw-r--r--   0        0        0      632 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/main-pybind11,skbuild,mesonpy.cpp
+-rw-r--r--   0        0        0      430 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/__init__.py
+-rw-r--r--   0        0        0      117 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_core-pybind11,skbuild,mesonpy,maturin.pyi
+-rw-r--r--   0        0        0      118 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_version-setuptools,pybind11.pyi
+-rw-r--r--   0        0        0        0 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/py.typed
+-rw-r--r--   0        0        0      213 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_compat/__init__.py
+-rw-r--r--   0        0        0      498 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/{{cookiecutter.project_slug}}/_compat/typing.py
+-rw-r--r--   0        0        0      188 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/tests/test_compiled-pybind11,skbuild,mesonpy,maturin.py
+-rw-r--r--   0        0        0      431 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/tests/test_package.py
+-rw-r--r--   0        0        0     2248 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/.gitignore
+-rw-r--r--   0        0        0     1525 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/LICENSE
+-rw-r--r--   0        0        0     2375 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/README-rr.md
+-rw-r--r--   0        0        0     5180 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/pyproject.toml
+-rw-r--r--   0        0        0     3894 2023-06-07 22:19:41.000000 sp_repo_review-2023.6.7/PKG-INFO
```

### Comparing `sp_repo_review-2023.6.1/.pre-commit-config.yaml` & `sp_repo_review-2023.6.7/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v2.7.1"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
-        exclude: ^docs/_includes/rr.html$
 
   - repo: https://github.com/codespell-project/codespell
     rev: "v2.2.4"
     hooks:
       - id: codespell
         exclude: ^Gemfile\.lock$
         args: ["-Lnd"]
```

### Comparing `sp_repo_review-2023.6.1/.readthedocs.yml` & `sp_repo_review-2023.6.7/.readthedocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -10,8 +10,10 @@
   os: ubuntu-22.04
   commands:
     - asdf plugin add ruby https://github.com/asdf-vm/asdf-ruby.git
     - asdf install ruby 3.1.2
     - asdf global ruby 3.1.2
     - gem install bundler
     - bundle install
-    - bundle exec jekyll build --destination _readthedocs/html --baseurl $(echo -n "$READTHEDOCS_CANONICAL_URL" | cut -d '/' -f 4-)
+    - >
+      bundle exec jekyll build --destination _readthedocs/html --baseurl $(echo
+      -n "$READTHEDOCS_CANONICAL_URL" | cut -d '/' -f 4-)
```

### Comparing `sp_repo_review-2023.6.1/Gemfile` & `sp_repo_review-2023.6.7/Gemfile`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/Gemfile.lock` & `sp_repo_review-2023.6.7/Gemfile.lock`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/_config.yml` & `sp_repo_review-2023.6.7/_config.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/cookiecutter.json` & `sp_repo_review-2023.6.7/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/noxfile.py` & `sp_repo_review-2023.6.7/noxfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+Nox runner for cookie & sp-repo-review.
+
+sp-repo-review checks start with "rr-".
+"""
+
+
 from __future__ import annotations
 
 import json
 import re
 import shutil
 import urllib.request
 from pathlib import Path
@@ -155,17 +162,20 @@
 
 
 GHA_VERS = re.compile(r"[\s\-]+uses: (.*?)@([^\s]+)")
 
 
 @nox.session(reuse_venv=True)
 def pc_bump(session: nox.Session) -> None:
+    """
+    Bump the pre-commit versions mentioned in the pages.
+    """
     session.install("lastversion")
 
-    style = Path("docs/pages/developers/style.md")
+    style = Path("docs/pages/guides/style.md")
     txt = style.read_text()
     old_versions = {m[1]: m[2].strip('"') for m in PC_VERS.finditer(txt)}
 
     for proj, old_version in old_versions.items():
         new_version = session.run("lastversion", proj, silent=True).strip()
 
         if old_version.lstrip("v") == new_version:
@@ -181,28 +191,33 @@
         txt = txt.replace(before, after)
 
     style.write_text(txt)
 
 
 @nox.session(venv_backend="none")
 def gha_bump(session: nox.Session) -> None:
-    pages = list(Path("docs/pages/developers").glob("gha_*.md"))
-    pages.append(Path("docs/pages/developers/style.md"))
+    """
+    Bump the GitHub Actions mentioned in the pages.
+    """
+    pages = list(Path("docs/pages/guides").glob("gha_*.md"))
+    pages.append(Path("docs/pages/guides/style.md"))
     full_txt = "\n".join(page.read_text() for page in pages)
 
     # This assumes there is a single version per action
     old_versions = {m[1]: m[2] for m in GHA_VERS.finditer(full_txt)}
 
     for repo, old_version in old_versions.items():
         session.log(f"{repo}: {old_version}")
         response = urllib.request.urlopen(f"https://api.github.com/repos/{repo}/tags")
         tags_js = json.loads(response.read())
         tags = [
             x["name"] for x in tags_js if x["name"].count(".") == old_version.count(".")
         ]
+        if not tags:
+            continue
         new_version = tags[0]
         if new_version != old_version:
             session.log(f"Convert {repo}: {old_version} -> {new_version}")
             for page in pages:
                 txt = page.read_text()
                 txt = txt.replace(
                     f"uses: {repo}@{old_version}", f"uses: {repo}@{new_version}"
@@ -212,15 +227,15 @@
 
 # -- Repo review --
 
 
 @nox.session(reuse_venv=True)
 def rr_run(session: nox.Session) -> None:
     """
-    Run the program
+    Run sp-repo-review.
     """
 
     session.install("-e", ".[cli]")
     session.run("python", "-m", "repo_review", *session.posargs)
 
 
 @nox.session
@@ -242,24 +257,24 @@
     session.install("-e.[cli]", "pylint")
     session.run("pylint", "src", *session.posargs)
 
 
 @nox.session
 def rr_tests(session: nox.Session) -> None:
     """
-    Run the unit and regular tests.
+    Run the unit and regular tests for sp-repo-review.
     """
     session.install("-e.[test,cli]")
     session.run("pytest", *session.posargs)
 
 
 @nox.session(reuse_venv=True)
 def rr_build(session: nox.Session) -> None:
     """
-    Build an SDist and wheel.
+    Build an SDist and wheel for sp-repo-review.
     """
 
     build_p = DIR.joinpath("build")
     if build_p.exists():
         shutil.rmtree(build_p)
 
     session.install("build")
```

### Comparing `sp_repo_review-2023.6.1/.devcontainer/devcontainer.json` & `sp_repo_review-2023.6.7/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/.github/workflows/ci.yml` & `sp_repo_review-2023.6.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/.github/workflows/reusable-change-detection.yml` & `sp_repo_review-2023.6.7/.github/workflows/reusable-change-detection.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/.github/workflows/reusable-cookie.yml` & `sp_repo_review-2023.6.7/.github/workflows/reusable-cookie.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/.github/workflows/reusable-rr-tests.yml` & `sp_repo_review-2023.6.7/.github/workflows/reusable-rr-tests.yml`

 * *Files 10% similar despite different names*

```diff
@@ -14,19 +14,32 @@
       fail-fast: false
       matrix:
         python-version: ["3.10", "3.11", "3.12-dev"]
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
 
     steps:
       - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
 
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install package
         run: python -m pip install .[test,cli]
 
       - name: Test package
         run: python -m pytest -ra
         env:
           PYTHONUTF8: "1"
+
+  action:
+    name: Action
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+
+      - name: Run sp-repo-review action
+        uses: ./
```

### Comparing `sp_repo_review-2023.6.1/docs/README.md` & `sp_repo_review-2023.6.7/docs/README.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/_includes/head.html` & `sp_repo_review-2023.6.7/docs/_includes/head.html`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/_includes/head_custom.html` & `sp_repo_review-2023.6.7/docs/_includes/head_custom.html`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/_sass/custom/custom.scss` & `sp_repo_review-2023.6.7/docs/_sass/custom/custom.scss`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/assets/favicon.ico` & `sp_repo_review-2023.6.7/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/assets/images/logo.svg` & `sp_repo_review-2023.6.7/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/assets/js/tabs.js` & `sp_repo_review-2023.6.7/docs/assets/js/tabs.js`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/assets/js/webapp.js` & `sp_repo_review-2023.6.7/docs/assets/js/webapp.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -20,30 +20,72 @@
         MaterialUI.Typography variant = "h6"
         component = "div"
         sx = {
             {
                 flexGrow: 1
             }
         } >
-        Scikit - HEP - Repo - Review <
+        Repo - Review <
         /MaterialUI.Typography> <
-        MaterialUI.Button href = "https://scientific-python-cookie.readthedocs.io"
-        color = "inherit" >
-        Developer Guidelines <
-        /MaterialUI.Button> <
-        MaterialUI.Button href = "https://github.com/scikit-hep/repo-review"
+        MaterialUI.Button href = "https://github.com/scientific-python/repo-review"
         color = "inherit" >
         Source <
         /MaterialUI.Button> <
         /MaterialUI.Toolbar> <
         /MaterialUI.AppBar> <
         /MaterialUI.Box>
     );
 }
 
+function IfUrlLink({
+    name,
+    url,
+    color
+}) {
+    if (url) {
+        return ( <
+            MaterialUI.Typography sx = {
+                {
+                    display: "inline"
+                }
+            }
+            component = "span"
+            variant = "body2"
+            color = {
+                color
+            }
+            component = "a"
+            href = {
+                url
+            }
+            target = "_blank" >
+            {
+                name
+            } <
+            /MaterialUI.Typography>
+        );
+    }
+    return ( <
+        MaterialUI.Typography sx = {
+            {
+                display: "inline"
+            }
+        }
+        component = "span"
+        variant = "body2"
+        color = {
+            color
+        } >
+        {
+            name
+        } <
+        /MaterialUI.Typography>
+    );
+}
+
 function Results(props) {
     const output = [];
     for (const key in props.results) {
         const inner_results = props.results[key];
         const results_components = inner_results.map((result) => {
             const text_color =
                 result.state === false ?
@@ -92,28 +134,34 @@
                     " [skipped]"
                 } <
                 /MaterialUI.Typography>
             );
             const msg = ( <
                 React.Fragment >
                 <
-                MaterialUI.Typography sx = {
-                    {
-                        display: "inline"
-                    }
+                IfUrlLink name = {
+                    result.name
+                }
+                url = {
+                    result.url
                 }
-                component = "span"
-                variant = "body2"
                 color = {
                     text_color
-                } >
-                {
-                    result.name + ": "
-                } <
-                /MaterialUI.Typography> <
+                }
+                /> <
+                IfUrlLink name = {
+                    ": "
+                }
+                url = {
+                    ""
+                }
+                color = {
+                    text_color
+                }
+                /> <
                 React.Fragment >
                 <
                 MaterialUI.Typography sx = {
                     {
                         display: "inline"
                     }
                 }
@@ -140,14 +188,17 @@
                 } < /MaterialUI.ListItemIcon> <
                 MaterialUI.ListItemText primary = {
                     msg
                 }
                 secondary = {
                     details
                 }
+                href = {
+                    result.url
+                }
                 /> <
                 /MaterialUI.ListItem>
             );
         });
 
         output.push( <
             li key = {
@@ -181,27 +232,26 @@
             output
         } <
         /MaterialUI.List> <
         /MaterialUI.Box>
     );
 }
 
-async function prepare_pyodide() {
+async function prepare_pyodide(deps) {
+    const deps_str = deps.map((i) => `"${i}"`).join(", ");
     const pyodide = await loadPyodide();
 
     await pyodide.loadPackage("micropip");
     await pyodide.runPythonAsync(`
         import micropip
-        await micropip.install(["scikit_hep_repo_review==0.6.1"])
+        await micropip.install([${deps_str}])
     `);
     return pyodide;
 }
 
-const pyodide_promise = prepare_pyodide();
-
 function MyThemeProvider(props) {
     const prefersDarkMode = MaterialUI.useMediaQuery(
         "(prefers-color-scheme: dark)"
     );
 
     const theme = React.useMemo(
         () =>
@@ -222,22 +272,25 @@
         /MaterialUI.ThemeProvider>
     );
 }
 
 class App extends React.Component {
     constructor(props) {
         super(props);
+        const deps_str = props.deps.map((i) => `"${i}"`).join(", ");
         this.state = {
             results: [],
             repo: urlParams.get("repo") || "",
             branch: urlParams.get("branch") || "",
-            msg: DEFAULT_MSG,
+            msg: `${DEFAULT_MSG} Packages: ${deps_str}`,
             progress: false,
             err_msg: "",
+            url: "",
         };
+        this.pyodide_promise = prepare_pyodide(props.deps);
     }
 
     handleCompute() {
         if (!this.state.repo || !this.state.branch) {
             this.setState({
                 results: [],
                 msg: DEFAULT_MSG
@@ -255,21 +308,21 @@
         window.history.replaceState(null, "", `${baseurl}?${local_params}`);
         this.setState({
             results: [],
             msg: "Running Python via Pyodide",
             progress: true,
         });
         const state = this.state;
-        pyodide_promise.then((pyodide) => {
+        this.pyodide_promise.then((pyodide) => {
             var families_checks;
             try {
                 families_checks = pyodide.runPython(`
             from pyodide.http import open_url
-            from scikit_hep_repo_review.processor import process
-            from scikit_hep_repo_review.ghpath import GHPath
+            from repo_review.processor import process
+            from repo_review.ghpath import GHPath
 
             GHPath.open_url = staticmethod(open_url)
 
             package = GHPath(repo="${state.repo}", branch="${state.branch}")
             process(package)
         `);
             } catch (e) {
@@ -300,23 +353,25 @@
             console.log(families);
             for (const val of results_list) {
                 results[val.family].push({
                     name: val.name.toString(),
                     description: val.description.toString(),
                     state: val.result,
                     err_msg: val.err_markdown().toString(),
+                    url: val.url.toString(),
                 });
             }
 
             this.setState({
                 results: results,
                 families: families,
                 msg: `Results for ${state.repo}@${state.branch}`,
                 progress: false,
                 err_msg: "",
+                url: "",
             });
 
             results_list.destroy();
             families_dict.destroy();
         });
     }
```

### Comparing `sp_repo_review-2023.6.1/docs/pages/index.md` & `sp_repo_review-2023.6.7/docs/pages/index.md`

 * *Files 17% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 maintainable, reusable, and shareable form? Start at the
 [tutorial]({% link pages/tutorials/index.md %}).
 
 **Learn recommended tools and best practices.** [Topical
 guides]({% link pages/guides/index.md %}) provide task-based instruction on
 topics that scientists and research software engineers may encounter as their
 projects evolve and grow. This covers everything from writing and building
-documentation to modern Python packaging.
+documentation to modern Python packaging. This comes with a cookiecutter for
+making new repos, [scientific-python/cookie][], and [sp-repo-review][], a tool
+for comparing your repository with the guidelines, runnable in WebAssembly.
 
 **Learn to write better research code.** A high-level document on
 [principles]({% link pages/principles/index.md %}) provides advice based on the
 community's collective experience building code that is easier for researchers
 to use successfully and easier to maintain over time.
 
 **Use our solutions for common tasks.** A growing collection of
@@ -36,7 +38,12 @@
 
 This guide does _not_ cover the basics of Python itself or the scientific Python
 libraries. We recommend the [SciPy Lecture Notes](https://scipy-lectures.org/).
 
 This guide also does not cover version control, but it is essential to have a
 basic facility with git to use these tools successfully. We recommend the
 [Software Carpentry lesson on git](https://swcarpentry.github.io/git-novice/).
+
+<!-- prettier-ignore-start -->
+[scientific-python/cookie]: https://github.com/scientific-python/cookie
+[sp-repo-review]: {% link pages/guides/repo_review.md %}
+<!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.6.1/docs/pages/guides/coverage.md` & `sp_repo_review-2023.6.7/docs/pages/guides/coverage.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/guides/gha_basic.md` & `sp_repo_review-2023.6.7/docs/pages/guides/gha_basic.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 layout: page
 title: "GHA: GitHub Actions intro"
-permalink: /guides/gha_basic/
+permalink: /guides/gha-basic/
 nav_order: 11
 parent: Topical Guides
 custom_title: GitHub Actions introduction
 ---
 
 {% include toc.html %}
```

### Comparing `sp_repo_review-2023.6.1/docs/pages/guides/gha_pure.md` & `sp_repo_review-2023.6.7/docs/pages/guides/gha_pure.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 layout: page
 title: "GHA: Pure Python wheels"
-permalink: /guides/gha_pure/
+permalink: /guides/gha-pure/
 nav_order: 12
 parent: Topical Guides
 custom_title: GitHub Actions for pure Python wheels
 ---
 
 {% include toc.html %}
```

### Comparing `sp_repo_review-2023.6.1/docs/pages/guides/gha_wheels.md` & `sp_repo_review-2023.6.7/docs/pages/guides/gha_wheels.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 layout: page
 title: "GHA: Binary wheels"
-permalink: /guides/gha_wheels/
+permalink: /guides/gha-wheels/
 nav_order: 13
 parent: Topical Guides
 custom_title: GitHub Actions for Binary Wheels
 ---
 
 {% include toc.html %}
 
@@ -35,18 +35,17 @@
 This will run on releases. If you use a develop branch, you could include
 `pull_request: branches: [stable]`, since it changes rarely. GitHub actions also
 [has a `workflow_dispatch` option][workflow_dispatch], which will allow you to
 click a button in the GUI to trigger a build, which is perfect for testing
 wheels before making a release; you can download them from "artifacts". You can
 even define variables that you can set in the GUI and access in the CI!
 
-[workflow_dispatch]:
-  https://github.blog/changelog/2020-07-06-github-actions-manual-triggers-with-workflow_dispatch/
-
 <!-- prettier-ignore-start -->
+[workflow_dispatch]: https://github.blog/changelog/2020-07-06-github-actions-manual-triggers-with-workflow_dispatch/
+
 ### Useful suggestion:
 {: .no_toc }
 <!-- prettier-ignore-end -->
 
 Since these variables will be used by all jobs, you could make them available in
 your `pyproject.toml` file, so they can be used everywhere (even locally for
 Linux and Windows):
@@ -116,15 +115,15 @@
 
   steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
         submodules: true
 
-    - uses: pypa/cibuildwheel@v2.12.3
+    - uses: pypa/cibuildwheel@v2.13.0
 
     - name: Upload wheels
       uses: actions/upload-artifact@v3
       with:
         path: wheelhouse/*.whl
 ```
```

### Comparing `sp_repo_review-2023.6.1/docs/pages/guides/index.md` & `sp_repo_review-2023.6.7/docs/pages/guides/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 layout: page
 title: Topical Guides
 permalink: /guides/
-nav_order: 3
+nav_order: 2
 has_children: true
 ---
 
 The pages here are intended for developers who are making or maintaining a
 package and want to follow modern best practices in Python.
 
 New developers are encouraged to read the following pages. Veteran developers
```

### Comparing `sp_repo_review-2023.6.1/docs/pages/guides/mypy.md` & `sp_repo_review-2023.6.7/docs/pages/guides/mypy.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/guides/nox.md` & `sp_repo_review-2023.6.7/docs/pages/guides/tasks.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/guides/packaging_classic.md` & `sp_repo_review-2023.6.7/docs/pages/guides/packaging_classic.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/guides/packaging_simple.md` & `sp_repo_review-2023.6.7/docs/pages/guides/packaging_simple.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/guides/pytest.md` & `sp_repo_review-2023.6.7/docs/pages/guides/pytest.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/guides/repo_review.md` & `sp_repo_review-2023.6.7/docs/pages/guides/repo_review.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/guides/style.md` & `sp_repo_review-2023.6.7/docs/pages/guides/style.md`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 updating your pre-commit hook.
 
 [ruff docs]: https://beta.ruff.rs
 [ruff]: https://github.com/charliermarsh/ruff
 
 ```yaml
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: "v0.0.267"
+  rev: "v0.0.271"
   hooks:
     - id: ruff
       args: ["--fix", "--show-fixes"]
 ```
 
 {% include rr.html id="PC191" %} The `--fix` argument is optional, but
 recommended, since you can inspect and undo changes in git.
@@ -285,15 +285,15 @@
 [PyCln][] will clean up your imports if you have any that are not needed. There
 is a Flake8 check for this, but it's usually nicer to automatically do the
 cleanup instead of forcing a user to manually delete unneeded imports. If you
 use the manual stage, it's opt-in instead of automatic.
 
 ```yaml
 - repo: https://github.com/hadialqattan/pycln
-  rev: "v2.1.3"
+  rev: "v2.1.5"
   hooks:
     - id: pycln
       args: [--all]
       stages: [manual]
 ```
 
 ### Flake8
@@ -585,15 +585,15 @@
 
 There is a tool that keeps your `setup.cfg` organized, and makes sure that
 important parts (like Python classifiers) are in sync. This tool,
 `setup-cfg-fmt`, has native support for pre-commit:
 
 ```yaml
 - repo: https://github.com/asottile/setup-cfg-fmt
-  rev: "v2.2.0"
+  rev: "v2.3.0"
   hooks:
     - id: setup-cfg-fmt
       args: [--include-version-classifiers, --max-py-version=3.12]
 ```
 
 Make sure you list the highest version of Python you are testing with here.
 
@@ -676,15 +676,15 @@
 ## Clang-format (C++ only)
 
 If you have C++ code, you should have a `.clang-format` file and use the
 following pre-commit config:
 
 ```yaml
 - repo: https://github.com/pre-commit/mirrors-clang-format
-  rev: "v16.0.3"
+  rev: "v16.0.4"
   hooks:
     - id: clang-format
       types_or: [c++, c, cuda]
 ```
 
 This will use 1-2 MB binary wheels from PyPI on all common platforms. You can
 generated such a file using
@@ -693,15 +693,15 @@
 ## Shellcheck (shell scripts only)
 
 If you have shell scripts, you can protect against common mistakes using
 [shellcheck](https://github.com/koalaman/shellcheck).
 
 ```yaml
 - repo: https://github.com/shellcheck-py/shellcheck-py
-  rev: "v0.9.0.2"
+  rev: "v0.9.0.5"
   hooks:
     - id: shellcheck
 ```
 
 ## Prettier
 
 {% include rr.html id="PC180" %} The [prettier](https://prettier.io) tool can
```

### Comparing `sp_repo_review-2023.6.1/docs/pages/guides/writing-docs.md` & `sp_repo_review-2023.6.7/docs/pages/guides/writing-docs.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/patterns/data_files.md` & `sp_repo_review-2023.6.7/docs/pages/patterns/data_files.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/patterns/index.md` & `sp_repo_review-2023.6.7/docs/pages/patterns/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/principles/design.md` & `sp_repo_review-2023.6.7/docs/pages/principles/design.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/principles/index.md` & `sp_repo_review-2023.6.7/docs/pages/principles/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 layout: page
 title: Principles
 permalink: /principles/
-nav_order: 2
+nav_order: 3
 has_children: true
 ---
 
 # Principles
 
 These pages are focused on designing good software, with a focus on end-user
 research code. [Process recommendations][] discusses the process of writing
```

### Comparing `sp_repo_review-2023.6.1/docs/pages/principles/process.md` & `sp_repo_review-2023.6.7/docs/pages/principles/process.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/tutorials/dev-environment.md` & `sp_repo_review-2023.6.7/docs/pages/tutorials/dev-environment.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/tutorials/index.md` & `sp_repo_review-2023.6.7/docs/pages/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/tutorials/module.md` & `sp_repo_review-2023.6.7/docs/pages/tutorials/module.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/tutorials/packaging.md` & `sp_repo_review-2023.6.7/docs/pages/tutorials/packaging.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/docs/pages/tutorials/test.md` & `sp_repo_review-2023.6.7/docs/pages/tutorials/test.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/hooks/post_gen_project.py` & `sp_repo_review-2023.6.7/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/src/sp_repo_review/families.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/families.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/src/sp_repo_review/checks/general.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,61 +9,61 @@
 
 class General:
     family = "general"
 
 
 class PY001(General):
     "Has a pyproject.toml"
-    url = mk_url("packaging_simple")
+    url = mk_url("packaging-simple")
 
     @staticmethod
     def check(package: Traversable) -> bool:
         """
         All projects should have a `pyproject.toml` file to support a modern
         build system and support wheel installs properly.
         """
         return package.joinpath("pyproject.toml").is_file()
 
 
 class PY002(General):
     "Has a README.(md|rst) file"
-    url = mk_url("packaging_simple")
+    url = mk_url("packaging-simple")
 
     @staticmethod
     def check(root: Traversable) -> bool:
         "Projects must have a readme file"
         return (
             root.joinpath("README.md").is_file()
             or root.joinpath("README.rst").is_file()
         )
 
 
 class PY003(General):
     "Has a LICENSE* file"
-    url = mk_url("packaging_simple")
+    url = mk_url("packaging-simple")
 
     @staticmethod
     def check(package: Traversable) -> bool:
         "Projects must have a license"
         return len([p for p in package.iterdir() if "LICENSE" in p.name]) > 0
 
 
 class PY004(General):
     "Has docs folder"
-    url = mk_url("packaging_simple")
+    url = mk_url("packaging-simple")
 
     @staticmethod
     def check(package: Traversable) -> bool:
         "Projects must have documentation in a folder called docs (disable if not applicable)"
         return len([p for p in package.iterdir() if "doc" in p.name]) > 0
 
 
 class PY005(General):
     "Has tests folder"
-    url = mk_url("packaging_simple")
+    url = mk_url("packaging-simple")
 
     @staticmethod
     def check(package: Traversable) -> bool:
         "Projects must have a folder called `*test*` or `src/*/*test*`"
         # Out-of-source tests
         if len([p for p in package.iterdir() if "test" in p.name]) > 0:
             return True
@@ -85,15 +85,15 @@
     def check(root: Traversable) -> bool:
         "Projects must have a `.pre-commit-config.yaml` file"
         return root.joinpath(".pre-commit-config.yaml").is_file()
 
 
 class PY007(General):
     "Supports an easy task runner (nox or tox)"
-    url = mk_url("nox")
+    url = mk_url("tasks")
 
     @staticmethod
     def check(root: Traversable) -> bool:
         """
         Projects must have a `noxfile.py` or `tox.ini` to encourage new contributors.
         """
         return (
```

### Comparing `sp_repo_review-2023.6.1/src/sp_repo_review/checks/github.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/github.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,63 +36,63 @@
 
 class GitHub:
     family = "github"
 
 
 class GH100(GitHub):
     "Has GitHub Actions config"
-    url = mk_url("gha_basic")
+    url = mk_url("gha-basic")
 
     @staticmethod
     def check(workflows: dict[str, Any]) -> bool:
         """
         All projects should have GitHub Actions config for this series of
         checks.  If there are no `.yml` files in `.github/workflows`, the
         remaining checks will be skipped.
         """
         return bool(workflows)
 
 
 class GH101(GitHub):
     "Has nice names"
     requires = {"GH100"}
-    url = mk_url("gha_basic")
+    url = mk_url("gha-basic")
 
     @staticmethod
     def check(workflows: dict[str, Any]) -> bool:
         """
         All workflows should have a nice readable `name:` field to pass this
         check. Feel free to ignore if you are happy with the filenames as names.
         """
         return all("name" in w for w in workflows.values())
 
 
 class GH102(GitHub):
     "Auto-cancel on repeated PRs"
     requires = {"GH100"}
-    url = mk_url("gha_basic")
+    url = mk_url("gha-basic")
 
     @staticmethod
     def check(workflows: dict[str, Any]) -> bool:
         """
         At least one workflow should auto-cancel.
 
         ```yaml
         concurrency:
-          group: ${{ github.workflow }}-${{ github.head_ref }}
+          group: ${{{{ github.workflow }}}}-${{{{ github.head_ref }}}}
           cancel-in-progress: true
         ```
         """
         return any("concurrency" in w for w in workflows.values())
 
 
 class GH103(GitHub):
     "At least one workflow with manual dispatch trigger"
     requires = {"GH100"}
-    url = mk_url("gha_basic")
+    url = mk_url("gha-basic")
 
     @staticmethod
     def check(workflows: dict[str, Any]) -> bool:
         """
         At least one workflow should have manual dispatch to allow easy triggering from the web.
 
         ```yaml
@@ -101,15 +101,15 @@
         ```
         """
         return any("workflow_dispatch" in w.get(True, {}) for w in workflows.values())
 
 
 class GH200(GitHub):
     "Maintained by Dependabot"
-    url = mk_url("gha_basic")
+    url = mk_url("gha-basic")
 
     @staticmethod
     def check(dependabot: dict[str, Any]) -> bool:
         """
         All projects should have a `.github/dependabot.yml` file to support at least
         GitHub Actions regular updates. Something like this:
 
@@ -125,15 +125,15 @@
         """
         return bool(dependabot)
 
 
 class GH210(GitHub):
     "Maintains the GitHub action versions with Dependabot"
     requires = {"GH200"}
-    url = mk_url("gha_basic")
+    url = mk_url("gha-basic")
 
     @staticmethod
     def check(dependabot: dict[str, Any]) -> bool:
         """
         All projects should maintain the GH Actions with dependabot.
 
         ```yaml
@@ -151,15 +151,15 @@
                 return True
         return False
 
 
 class GH211(GitHub):
     "Do not pin core actions as major versions"
     requires = {"GH200", "GH210"}  # Currently listing both helps - TODO: remove GH200
-    url = mk_url("gha_basic")
+    url = mk_url("gha-basic")
 
     @staticmethod
     def check(dependabot: dict[str, Any]) -> bool:
         """
         Projects should not pin major versions for official actions. This is now
         supported by dependabot respecting the tag style you are already using
         since April 2022.
```

### Comparing `sp_repo_review-2023.6.1/src/sp_repo_review/checks/mypy.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/mypy.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/src/sp_repo_review/checks/precommit.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/precommit.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/src/sp_repo_review/checks/pyproject.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/pyproject.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     family = "pyproject"
 
 
 class PP002(PyProject):
     "Has a proper build-system table"
 
     requires = {"PY001"}
-    url = mk_url("packaging_simple")
+    url = mk_url("packaging-simple")
 
     @staticmethod
     def check(pyproject: dict[str, Any]) -> bool:
         """
         Must have `build-system.requires` *and* `build-system.backend`. Both
         should be present in all modern packages.
         """
@@ -29,15 +29,15 @@
                 return False
 
 
 class PP003(PyProject):
     "Does not list wheel as a build-dep"
 
     requires = {"PY001"}
-    url = mk_url("packaging_classic")
+    url = mk_url("packaging-classic")
 
     @staticmethod
     def check(pyproject: dict[str, Any]) -> bool:
         """
         Do not include `"wheel"` in your `build-system.requires`, setuptools
         does this via PEP 517 already. Setuptools will also only require this
         for actual wheel builds, and might have version limits.
```

### Comparing `sp_repo_review-2023.6.1/src/sp_repo_review/checks/ruff.py` & `sp_repo_review-2023.6.7/src/sp_repo_review/checks/ruff.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/tests/test_package.py` & `sp_repo_review-2023.6.7/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.gitignore` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.pre-commit-config.yaml` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/Cargo-maturin.toml` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/Cargo-maturin.toml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/LICENSE` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/LICENSE`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/README.md` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/meson-mesonpy.build` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/meson-mesonpy.build`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/noxfile.py` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/noxfile.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/pyproject.toml` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/setup-pybind11.py` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-pybind11.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/setup-setuptools,pybind11.cfg` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/setup-setuptools,pybind11.cfg`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.github/matchers/pylint.json` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.github/workflows/ci.yml` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/.github/workflows/wheels-pybind11,skbuild,mesonpy,maturin.yml` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/.github/workflows/wheels-pybind11,skbuild,mesonpy,maturin.yml`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/docs/conf.py` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/src/lib-maturin.rs` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/lib-maturin.rs`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/{{cookiecutter.project_name}}/src/main-pybind11,skbuild,mesonpy.cpp` & `sp_repo_review-2023.6.7/{{cookiecutter.project_name}}/src/main-pybind11,skbuild,mesonpy.cpp`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/.gitignore` & `sp_repo_review-2023.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/LICENSE` & `sp_repo_review-2023.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sp_repo_review-2023.6.1/README.md` & `sp_repo_review-2023.6.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 # Scientific Python: cookie
 
 [![Actions Status][actions-badge]][actions-link]
 [![GitHub Discussion][github-discussions-badge]][github-discussions-link]
+[![Live ReadTheDocs][rtd-badge]][rtd-link]
+
+[![PyPI version][pypi-version]][pypi-link]
+[![PyPI platforms][pypi-platforms]][pypi-link]
 
 A cookiecutter template for new Python projects based on the Scientific Python
 Developer Guide. What makes this different from other cookie cutter templates
 for Python packages?
 
-- Designed from the [Scientific Python Developer Guide][]: Every decision is
+- Lives with the [Scientific-Python Development Guide][]: Every decision is
   clearly documented and every tool described.
-- Template generation tested in GitHub Actions using nox.
 - Twelve different backends to choose from for building packages.
+- Template generation tested in GitHub Actions using nox.
 - Includes several compiled backends using pybind11, with wheels produced for
   all platforms using cibuildwheel.
-- Follows PyPA best practices.
+- Follows PyPA best practices and regularly updated.
+- Provides [`sp-repo-review`][pypi-link] to evaluate existing repos against the
+  guidelines, with a WebAssembly version integrated with the guide. All checks
+  cross-linked.
 
-Be sure you have read the [Scientific Python Developer Guide][] first, and
+Be sure you have read the [Scientific-Python Development Guide][] first, and
 possibly used them on a project or two. This is _not_ a minimal example or
 tutorial. It is a collection of useful tooling for starting a new project using
 cookiecutter, or for copying in individual files for an existing project (by
 hand, from `{{cookiecutter.project_name}}/`).
 
 During generation you can select from the following backends for your package:
 
@@ -40,15 +47,15 @@
    all-in-one. Makes some bad default assumptions for libraries.
 8. [flit][]: A modern, lightweight [PEP 621][] build system for pure Python
    projects. Replaces setuptools, no MANIFEST.in, setup.py, or setup.cfg. Low
    learning curve. Easy to bootstrap into new distributions. Difficult to get
    the right files included, little dynamic metadata support.
 9. [pdm][]: A modern, less opinionated all-in-one solution to pure Python
    projects supporting standards. Replaces setuptools, venv/pipenv, pip, wheel,
-   and twine. Supports [PEP 621][], and also the unaccepted [PEP 582][].
+   and twine. Supports [PEP 621][].
 10. [trampolim][]: A modern [PEP 621][] builder with support for tasks, allowing
     arbitrary Python to run during the build process if needed.
 11. [whey][]: A modern [PEP 621][] builder with some automation options for
     Trove classifiers. Development seems to be stalled, possibly.
 12. [maturin][]: A [PEP 621][] builder for Rust binary extensions.
     **(Recommended for Rust projects)**
 
@@ -58,15 +65,15 @@
 #### To use:
 
 Install cookiecutter, ideally with `brew install cookiecutter` if you use brew,
 otherwise with `pipx install cookiecutter` (or prepend `pipx run` to the command
 below, and skip installation). Then run:
 
 ```bash
-cookiecutter gh:scikit-hep/cookie
+cookiecutter gh:scientific-python/cookie
 ```
 
 You can also use `pipx run cookiecutter` without installing.
 
 Check the key setup files, `pyproject.toml`, and possibly `setup.cfg` and
 `setup.py` (pybind11 example). Update README.md. Also update and add docs to
 `docs/`.
@@ -139,35 +146,43 @@
 focus on GitHub Actions - most our guide could be adapted to a different CI
 system fairly easily if you don't want to use GHA. It also forces the use of
 Poetry (instead of having a backend selection), and doesn't support compiled
 projects. It currently dumps all development dependencies into a shared
 environment, causing long solve times and high chance of conflicts. It also does
 not use pre-commit properly. It also has quite a bit of custom code.
 
+#### History
+
+A lot of the guide, cookiecutter, and repo-review started out as part of
+Scikit-HEP. These projects were merged, generalized, and combined with the
+NSLS-II guide during the 2023 Scientific-Python Developers Summit.
+
 <!-- prettier-ignore-start -->
 
 [actions-badge]: https://github.com/scikit-hep/cookie/workflows/CI/badge.svg
 [actions-link]: https://github.com/scikit-hep/cookie/actions
-[conda-badge]: https://img.shields.io/conda/vn/conda-forge/cookie
-[conda-link]: https://github.com/conda-forge/cookie-feedstock
-[github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
-[github-discussions-link]: https://github.com/scikit-hep/cookie/discussions
-[scikit-hep developer guidelines]: https://scikit-hep.org/developer
 [cibuildwheel]: https://cibuildwheel.readthedocs.io/en/stable/
-[scikit-build]: https://scikit-build.readthedocs.io/en/latest/
 [flit]: https://flit.readthedocs.io/en/latest/
+[github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
+[github-discussions-link]: https://github.com/scikit-hep/cookie/discussions
+[hatch]: https://github.com/ofek/hatch
+[hypermodern]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+[maturin]: https://maturin.rs
+[meson-python]: https://meson-python.readthedocs.io
 [nox]: https://nox.thea.codes/en/stable/
 [pdm]: https://pdm.fming.dev
+[pep 621]: https://www.python.org/dev/peps/pep-0621
+[pipx]: https://pypa.github.io/pipx/
 [poetry]: https://python-poetry.org
 [pybind11]: https://pybind11.readthedocs.io/en/stable/
+[pypi-link]: https://pypi.org/project/sp-repo-review/
+[pypi-platforms]: https://img.shields.io/pypi/pyversions/sp-repo-review
+[pypi-version]: https://badge.fury.io/py/sp-repo-review.svg
+[rtd-badge]: https://readthedocs.org/projects/scientific-python-cookie/badge/?version=latest
+[rtd-link]: https://scientific-python-cookie.readthedocs.io/en/latest/?badge=latest
+[scientific-python development guide]: https://learn.scientific-python.org/development
+[scikit-build]: https://scikit-build.readthedocs.io/en/latest/
 [setuptools]: https://setuptools.readthedocs.io/en/latest/
 [trampolim]: https://trampolim.readthedocs.io/en/latest/
-[pipx]: https://pypa.github.io/pipx/
 [whey]: https://whey.readthedocs.io/en/latest/
-[maturin]: https://maturin.rs
-[hypermodern]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
-[hatch]: https://github.com/ofek/hatch
-[meson-python]: https://meson-python.readthedocs.io
-[pep 582]: https://www.python.org/dev/peps/pep-0582
-[pep 621]: https://www.python.org/dev/peps/pep-0621
 
 <!-- prettier-ignore-end -->
```

### Comparing `sp_repo_review-2023.6.1/pyproject.toml` & `sp_repo_review-2023.6.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "sp_repo_review"
 authors = [
   { name = "Henry Schreiner", email = "henryfs@princeton.edu" },
 ]
-license = { file = "LICENSE" }
 description = "Review repos for compliance to the Scientific-Python development guidelines"
-readme = "README.md"
+readme = "README-rr.md"
 requires-python = ">=3.10"
 classifiers = [
-  "License :: OSI Approved :: BSD License",
-  "Topic :: Scientific/Engineering",
-  "Intended Audience :: Science/Research",
+  "Development Status :: 4 - Beta",
+  "Environment :: Console",
+  "Environment :: WebAssembly :: Emscripten",
   "Intended Audience :: Developers",
-  "Operating System :: OS Independent",
+  "Intended Audience :: Science/Research",
   "License :: OSI Approved :: BSD License",
-  "Programming Language :: Python",
+  "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
-  "Development Status :: 4 - Beta",
+  "Programming Language :: Python",
+  "Topic :: Scientific/Engineering",
+  "Topic :: Software Development :: Libraries :: Python Modules",
+  "Topic :: Software Development :: Quality Assurance",
+  "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
   "pyyaml",
   "repo-review>=0.7.0b4,<0.8",
 ]
 
@@ -40,18 +43,20 @@
   "pytest >=7",
 ]
 dev = [
   "pytest >=7",
 ]
 
 [project.urls]
-homepage = "https://github.com/scientific-python/cookie"
-webpage = "https://scientific-python.github.io/cookie"
+Homepage = "https://github.com/scientific-python/cookie"
+Webpage = "https://scientific-python.github.io/cookie"
+Preview = "https://scientific-python-cookie.readthedocs.io"
+
 
-[project.scripts]
+[project.entry-points."pipx.run"]
 sp-repo-review = "repo_review.__main__:main"
 
 [project.entry-points."repo_review.checks"]
 general = "sp_repo_review.checks.general:repo_review_checks"
 pyproject = "sp_repo_review.checks.pyproject:repo_review_checks"
 precommit = "sp_repo_review.checks.precommit:repo_review_checks"
 ruff = "sp_repo_review.checks.ruff:repo_review_checks"
@@ -63,15 +68,16 @@
 dependabot = "sp_repo_review.checks.github:dependabot"
 precommit = "sp_repo_review.checks.precommit:precommit"
 
 [project.entry-points."repo_review.families"]
 scikit-hep = "sp_repo_review.families:get_familes"
 
 [tool.hatch]
-version.path = "src/sp_repo_review/__init__.py"
+version.source = "vcs"
+build.hooks.vcs.version-file = "src/sp_repo_review/_version.py"
 
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = ["-ra", "--strict-markers", "--strict-config"]
 xfail_strict = true
 log_cli_level = "INFO"
```

