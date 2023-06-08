# Comparing `tmp/pdm_backend-2.0.7.tar.gz` & `tmp/pdm_backend-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_backend-2.0.7.tar", last modified: Mon May 15 03:57:50 2023, max compression
+gzip compressed data, was "pdm_backend-2.1.0.tar", last modified: Thu Jun  8 08:15:25 2023, max compression
```

## Comparing `pdm_backend-2.0.7.tar` & `pdm_backend-2.1.0.tar`

### file list

```diff
@@ -1,180 +1,181 @@
--rw-r--r--   0        0        0     1067 2023-05-15 03:57:35.038082 pdm_backend-2.0.7/LICENSE
--rw-r--r--   0        0        0     1725 2023-05-15 03:57:35.038082 pdm_backend-2.0.7/README.md
--rw-r--r--   0        0        0     2271 2023-05-15 03:57:50.543192 pdm_backend-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     3282 2023-05-15 03:57:35.038082 pdm_backend-2.0.7/src/pdm/backend/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 03:57:35.038082 pdm_backend-2.0.7/src/pdm/backend/_vendor/__init__.py
--rw-r--r--   0        0        0      197 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/LICENSE
--rw-r--r--   0        0        0    10174 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/LICENSE.BSD
--rw-r--r--   0        0        0      661 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3265 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8813 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     9606 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5115 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     7928 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/markers.py
--rw-r--r--   0        0        0        0 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     3264 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    38937 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    16469 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16315 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/version.py
--rw-r--r--   0        0        0     1113 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/pyproject_metadata/LICENSE
--rw-r--r--   0        0        0    19827 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/pyproject_metadata/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/pyproject_metadata/py.typed
--rw-r--r--   0        0        0     1072 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/LICENSE
--rw-r--r--   0        0        0      396 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/py.typed
--rw-r--r--   0        0        0     1072 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli_w/LICENSE
--rw-r--r--   0        0        0      177 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli_w/__init__.py
--rw-r--r--   0        0        0     6132 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli_w/_writer.py
--rw-r--r--   0        0        0       26 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli_w/py.typed
--rw-r--r--   0        0        0       70 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/_vendor/vendor.txt
--rw-r--r--   0        0        0    11746 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/base.py
--rw-r--r--   0        0        0     9411 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/config.py
--rw-r--r--   0        0        0     4063 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/editable.py
--rw-r--r--   0        0        0      452 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/exceptions.py
--rw-r--r--   0        0        0      108 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/hooks/__init__.py
--rw-r--r--   0        0        0     4069 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/hooks/base.py
--rw-r--r--   0        0        0     6364 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/hooks/setuptools.py
--rw-r--r--   0        0        0     4894 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/hooks/version/__init__.py
--rw-r--r--   0        0        0    10064 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/hooks/version/scm.py
--rw-r--r--   0        0        0      759 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/intree.py
--rw-r--r--   0        0        0    14958 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/macosx_platform.py
--rw-r--r--   0        0        0        0 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/py.typed
--rw-r--r--   0        0        0     3604 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/sdist.py
--rw-r--r--   0        0        0     1381 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/structures.py
--rw-r--r--   0        0        0     7080 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/utils.py
--rw-r--r--   0        0        0    10581 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/src/pdm/backend/wheel.py
--rw-r--r--   0        0        0       72 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/tests/__init__.py
--rw-r--r--   0        0        0      747 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/tests/conftest.py
--rw-r--r--   0        0        0      856 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/tests/fixtures/hooks/hook_class.py
--rw-r--r--   0        0        0      599 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/tests/fixtures/hooks/hook_module.py
--rw-r--r--   0        0        0      599 2023-05-15 03:57:35.042082 pdm_backend-2.0.7/tests/fixtures/hooks/local_hook.py
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension-in-src/LICENSE
--rw-r--r--   0        0        0      138 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
--rw-r--r--   0        0        0      234 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension-in-src/pdm_build.py
--rw-r--r--   0        0        0      558 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
--rw-r--r--   0        0        0      478 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension/LICENSE
--rw-r--r--   0        0        0       22 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension/my_package/__init__.py
--rw-r--r--   0        0        0      478 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
--rw-r--r--   0        0        0      138 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension/pdm.lock
--rw-r--r--   0        0        0      230 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension/pdm_build.py
--rw-r--r--   0        0        0      554 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension/pyproject.toml
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-combined-extras/LICENSE
--rw-r--r--   0        0        0       26 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      379 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-explicit-package-dir/README.md
--rw-r--r--   0        0        0       16 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
--rw-r--r--   0        0        0       22 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
--rw-r--r--   0        0        0      433 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
--rw-r--r--   0        0        0       21 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       60 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      402 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-no-license/README.md
--rw-r--r--   0        0        0      406 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-no-license/pyproject.toml
--rw-r--r--   0        0        0       36 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-no-license/src/foo_module.py
--rw-r--r--   0        0        0        0 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-no-version/README.md
-lrwxr-xr-x   0        0        0        0 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
--rw-r--r--   0        0        0      330 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-no-version/pyproject.toml
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/LICENSE
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/README.md
--rw-r--r--   0        0        0       16 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/data_out.json
--rw-r--r--   0        0        0       22 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/pdm.lock
--rw-r--r--   0        0        0      555 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/requirements.txt
--rw-r--r--   0        0        0      604 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/single_module.py
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/LICENSE
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/README.md
--rw-r--r--   0        0        0       16 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/data_out.json
--rw-r--r--   0        0        0       22 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/pdm.lock
--rw-r--r--   0        0        0      555 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/requirements.txt
--rw-r--r--   0        0        0      604 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/single_module.py
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-deep-path/README.md
--rw-r--r--   0        0        0       22 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
--rw-r--r--   0        0        0       16 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
--rw-r--r--   0        0        0      574 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/LICENSE
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/README.md
--rw-r--r--   0        0        0       22 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.046083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
--rw-r--r--   0        0        0     7700 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/pdm.lock
--rw-r--r--   0        0        0      513 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/my_package/data.json
--rwxr-xr-x   0        0        0        0 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/my_package/executable
--rw-r--r--   0        0        0     2461 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      598 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0     4259 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      604 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0       21 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-pep420-package/LICENSE
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-pep420-package/README.md
--rw-r--r--   0        0        0       22 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
--rw-r--r--   0        0        0        3 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
--rw-r--r--   0        0        0      464 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-pep420-package/pyproject.toml
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-purelib-with-build/LICENSE
--rw-r--r--   0        0        0      277 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-purelib-with-build/my_build.py
--rw-r--r--   0        0        0       22 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
--rw-r--r--   0        0        0      138 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
--rw-r--r--   0        0        0      549 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
--rw-r--r--   0        0        0       26 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-reuse-spec/README.md
--rw-r--r--   0        0        0      413 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
--rw-r--r--   0        0        0       36 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package-include/LICENSE
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package-include/README.md
--rw-r--r--   0        0        0       16 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package-include/data_out.json
--rw-r--r--   0        0        0      500 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package-include/pyproject.toml
--rw-r--r--   0        0        0       21 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package-include/single_module.py
--rw-r--r--   0        0        0       22 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      395 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-pymodule/LICENSE
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-pymodule/README.md
--rw-r--r--   0        0        0      406 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
--rw-r--r--   0        0        0       36 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
--rw-r--r--   0        0        0       36 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-using-scm/.gitignore
--rw-r--r--   0        0        0       12 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-using-scm/LICENSE
--rw-r--r--   0        0        0       24 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-using-scm/README.md
--rw-r--r--   0        0        0       36 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-using-scm/foo/__init__.py
--rw-r--r--   0        0        0      369 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/fixtures/projects/demo-using-scm/pyproject.toml
--rw-r--r--   0        0        0    16264 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/test_api.py
--rw-r--r--   0        0        0     5324 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/test_file_finder.py
--rw-r--r--   0        0        0     1632 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/test_hooks.py
--rw-r--r--   0        0        0     3058 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/test_metadata.py
--rw-r--r--   0        0        0      311 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/test_utils.py
--rw-r--r--   0        0        0     1176 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/test_wheel.py
--rw-r--r--   0        0        0      598 2023-05-15 03:57:35.050083 pdm_backend-2.0.7/tests/testutils.py
--rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 pdm_backend-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1725 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/README.md
+-rw-r--r--   0        0        0     2271 2023-06-08 08:15:25.005818 pdm_backend-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3282 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/LICENSE
+-rw-r--r--   0        0        0    10174 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/LICENSE.BSD
+-rw-r--r--   0        0        0      661 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3265 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8813 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     9606 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5115 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     7928 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0        0 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     3264 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    38937 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    16469 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16315 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     1113 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/pyproject_metadata/LICENSE
+-rw-r--r--   0        0        0    19827 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/pyproject_metadata/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/pyproject_metadata/py.typed
+-rw-r--r--   0        0        0     1072 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/tomli/LICENSE
+-rw-r--r--   0        0        0      396 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0     1072 2023-06-08 08:15:04.705250 pdm_backend-2.1.0/src/pdm/backend/_vendor/tomli_w/LICENSE
+-rw-r--r--   0        0        0      177 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/_vendor/tomli_w/__init__.py
+-rw-r--r--   0        0        0     6132 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/_vendor/tomli_w/_writer.py
+-rw-r--r--   0        0        0       26 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/_vendor/tomli_w/py.typed
+-rw-r--r--   0        0        0       70 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/_vendor/vendor.txt
+-rw-r--r--   0        0        0    11948 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/base.py
+-rw-r--r--   0        0        0     9775 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/config.py
+-rw-r--r--   0        0        0     4063 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/editable.py
+-rw-r--r--   0        0        0      452 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/exceptions.py
+-rw-r--r--   0        0        0      108 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/hooks/__init__.py
+-rw-r--r--   0        0        0     4429 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/hooks/base.py
+-rw-r--r--   0        0        0     6364 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/hooks/setuptools.py
+-rw-r--r--   0        0        0     4894 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/hooks/version/__init__.py
+-rw-r--r--   0        0        0    10129 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/hooks/version/scm.py
+-rw-r--r--   0        0        0      759 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/intree.py
+-rw-r--r--   0        0        0    14958 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/macosx_platform.py
+-rw-r--r--   0        0        0        0 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/py.typed
+-rw-r--r--   0        0        0     3604 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/sdist.py
+-rw-r--r--   0        0        0     1381 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/structures.py
+-rw-r--r--   0        0        0     7080 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/utils.py
+-rw-r--r--   0        0        0    11706 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/src/pdm/backend/wheel.py
+-rw-r--r--   0        0        0       72 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      747 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      856 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/hooks/hook_class.py
+-rw-r--r--   0        0        0      599 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/hooks/hook_module.py
+-rw-r--r--   0        0        0      599 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/hooks/local_hook.py
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-cextension-in-src/LICENSE
+-rw-r--r--   0        0        0      138 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
+-rw-r--r--   0        0        0      234 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-cextension-in-src/pdm_build.py
+-rw-r--r--   0        0        0      558 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-cextension/LICENSE
+-rw-r--r--   0        0        0       22 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-cextension/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
+-rw-r--r--   0        0        0      138 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-cextension/pdm.lock
+-rw-r--r--   0        0        0      230 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-cextension/pdm_build.py
+-rw-r--r--   0        0        0      554 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-cextension/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-combined-extras/LICENSE
+-rw-r--r--   0        0        0       26 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      379 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-explicit-package-dir/README.md
+-rw-r--r--   0        0        0       16 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
+-rw-r--r--   0        0        0       22 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
+-rw-r--r--   0        0        0      433 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       60 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      402 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-no-license/README.md
+-rw-r--r--   0        0        0      406 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-no-license/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-no-license/src/foo_module.py
+-rw-r--r--   0        0        0        0 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-no-version/README.md
+lrwxr-xr-x   0        0        0        0 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
+-rw-r--r--   0        0        0      330 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-no-version/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include-error/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include-error/README.md
+-rw-r--r--   0        0        0       16 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include-error/data_out.json
+-rw-r--r--   0        0        0       22 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include-error/my_package/data.json
+-rw-r--r--   0        0        0     7700 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include-error/pdm.lock
+-rw-r--r--   0        0        0      555 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include-error/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include-error/requirements.txt
+-rw-r--r--   0        0        0      604 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include-error/single_module.py
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include/README.md
+-rw-r--r--   0        0        0       16 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include/data_out.json
+-rw-r--r--   0        0        0       22 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include/my_package/data.json
+-rw-r--r--   0        0        0     7700 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include/pdm.lock
+-rw-r--r--   0        0        0      639 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include/requirements.txt
+-rw-r--r--   0        0        0      604 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include/requirements_simple.txt
+-rwxr-xr-x   0        0        0       32 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include/scripts/my_script.sh
+-rw-r--r--   0        0        0       21 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include/single_module.py
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-deep-path/README.md
+-rw-r--r--   0        0        0       22 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
+-rw-r--r--   0        0        0       16 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
+-rw-r--r--   0        0        0      574 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-tests/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-tests/README.md
+-rw-r--r--   0        0        0       22 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
+-rw-r--r--   0        0        0     7700 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-tests/pdm.lock
+-rw-r--r--   0        0        0      513 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package/my_package/data.json
+-rwxr-xr-x   0        0        0        0 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package/my_package/executable
+-rw-r--r--   0        0        0     2461 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      598 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0     4259 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      604 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-pep420-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-pep420-package/README.md
+-rw-r--r--   0        0        0       22 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
+-rw-r--r--   0        0        0        3 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
+-rw-r--r--   0        0        0      464 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-pep420-package/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.709250 pdm_backend-2.1.0/tests/fixtures/projects/demo-purelib-with-build/LICENSE
+-rw-r--r--   0        0        0      277 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-purelib-with-build/my_build.py
+-rw-r--r--   0        0        0       22 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
+-rw-r--r--   0        0        0      138 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
+-rw-r--r--   0        0        0      549 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-reuse-spec/README.md
+-rw-r--r--   0        0        0      413 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-package-include/README.md
+-rw-r--r--   0        0        0       16 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-package-include/data_out.json
+-rw-r--r--   0        0        0      500 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-package-include/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-package-include/single_module.py
+-rw-r--r--   0        0        0       22 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      395 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-pymodule/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-pymodule/README.md
+-rw-r--r--   0        0        0      406 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
+-rw-r--r--   0        0        0       36 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-using-scm/.gitignore
+-rw-r--r--   0        0        0       12 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-using-scm/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-using-scm/README.md
+-rw-r--r--   0        0        0       36 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-using-scm/foo/__init__.py
+-rw-r--r--   0        0        0      369 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/fixtures/projects/demo-using-scm/pyproject.toml
+-rw-r--r--   0        0        0    18382 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/test_api.py
+-rw-r--r--   0        0        0     5324 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/test_file_finder.py
+-rw-r--r--   0        0        0     1632 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/test_hooks.py
+-rw-r--r--   0        0        0     3058 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/test_metadata.py
+-rw-r--r--   0        0        0      311 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1176 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/test_wheel.py
+-rw-r--r--   0        0        0      598 2023-06-08 08:15:04.713250 pdm_backend-2.1.0/tests/testutils.py
+-rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 pdm_backend-2.1.0/PKG-INFO
```

### Comparing `pdm_backend-2.0.7/LICENSE` & `pdm_backend-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/README.md` & `pdm_backend-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/pyproject.toml` & `pdm_backend-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "importlib-metadata>=3.6; python_version < \"3.10\"",
 ]
-version = "2.0.7"
+version = "2.1.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/pdm-project/pdm-backend"
 Repository = "https://github.com/pdm-project/pdm-backend"
```

### Comparing `pdm_backend-2.0.7/src/pdm/backend/__init__.py` & `pdm_backend-2.1.0/src/pdm/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/LICENSE.APACHE` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/LICENSE.BSD` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/__about__.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_elffile.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_manylinux.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_musllinux.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_parser.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_structures.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/_tokenizer.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/markers.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/requirements.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/specifiers.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/tags.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/utils.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/packaging/version.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/pyproject_metadata/LICENSE` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/pyproject_metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/pyproject_metadata/__init__.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/pyproject_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/LICENSE` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/tomli/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/_parser.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli/_re.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli_w/LICENSE` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/tomli_w/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/_vendor/tomli_w/_writer.py` & `pdm_backend-2.1.0/src/pdm/backend/_vendor/tomli_w/_writer.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/base.py` & `pdm_backend-2.1.0/src/pdm/backend/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             result.append(path)
     return result
 
 
 class Builder:
     """Base class for building and distributing a package from given path."""
 
-    DEFAULT_EXCLUDES = ["build"]
+    DEFAULT_EXCLUDES = [".pdm-build"]
 
     target: str
     hooks: list[BuildHookInterface] = [DynamicVersionBuildHook()]
 
     def __init__(
         self,
         location: str | Path,
@@ -134,15 +134,15 @@
             if hasattr(hook, "pdm_build_hook_enabled"):
                 if not hook.pdm_build_hook_enabled(context):
                     continue
             if hasattr(hook, hook_name):
                 getattr(hook, hook_name)(context, *args, **kwargs)
 
     def build_context(self, destination: Path, **kwargs: Any) -> Context:
-        build_dir = self.location / "build"
+        build_dir = self.location / ".pdm-build"
         if not destination.exists():
             destination.mkdir(0o700, parents=True)
         return Context(
             build_dir=build_dir, dist_dir=destination, kwargs=kwargs, builder=self
         )
 
     def __enter__(self: T) -> T:
@@ -177,19 +177,28 @@
 
     def finalize(self, context: Context, artifact: Path) -> None:
         self.call_hook("pdm_build_finalize", context, artifact)
 
     def build(self, build_dir: str, **kwargs: Any) -> Path:
         """Build the package and return the path to the artifact."""
         context = self.build_context(Path(build_dir), **kwargs)
-        if (
-            not self.config_settings.get("no-clean-build")
-            or os.getenv("PDM_BUILD_NO_CLEAN", "false").lower() == "false"
-        ):
+        should_clean = True
+
+        if "no-clean-build" in self.config_settings:
+            should_clean = False
+        elif "PDM_BUILD_NO_CLEAN" in os.environ:
+            should_clean = os.getenv("PDM_BUILD_NO_CLEAN", "0").lower() in (
+                "0",
+                "false",
+                "no",
+            )
+
+        if should_clean:
             self.clean(context)
+
         self.initialize(context)
         files = sorted(self.get_files(context))
         artifact = self.build_artifact(context, files)
         self.finalize(context, artifact)
         return artifact
 
     def build_artifact(
```

### Comparing `pdm_backend-2.0.7/src/pdm/backend/config.py` & `pdm_backend-2.1.0/src/pdm/backend/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 from __future__ import annotations
 
 import glob
 import os
 import sys
 from pathlib import Path
-from typing import Any, TypeVar
+from typing import TYPE_CHECKING, Any, TypeVar
 
 from pdm.backend._vendor import tomli_w
 from pdm.backend._vendor.pyproject_metadata import ConfigurationError, StandardMetadata
 from pdm.backend.exceptions import ConfigError, ValidationError
 from pdm.backend.structures import Table
 from pdm.backend.utils import find_packages_iter
 
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import pdm.backend._vendor.tomli as tomllib
 
 T = TypeVar("T")
 
+if TYPE_CHECKING:
+    from typing import TypedDict
+
+    DataSpecDict = TypedDict(
+        "DataSpecDict", {"path": str, "relative-to": str}, total=False
+    )
+    DataSpec = DataSpecDict | str
+
 
 class Config:
     """The project config object for pdm backend.
 
     Parameters:
         root: The root directory of the project
         data: The parsed pyproject.toml data
@@ -253,7 +261,12 @@
     @property
     def editable_backend(self) -> str:
         """Currently only two backends are supported:
         - editables: Proxy modules via editables
         - path: the legacy .pth file method(default)
         """
         return self.get("editable-backend", "path")
+
+    @property
+    def wheel_data(self) -> dict[str, list[DataSpec]]:
+        """The wheel data configuration"""
+        return self.get("wheel-data", {})
```

### Comparing `pdm_backend-2.0.7/src/pdm/backend/editable.py` & `pdm_backend-2.1.0/src/pdm/backend/editable.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/hooks/base.py` & `pdm_backend-2.1.0/src/pdm/backend/hooks/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import dataclasses
 from pathlib import Path
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Iterable
 
 from pdm.backend.config import Config
 
 if TYPE_CHECKING:
     from typing import Protocol
 
     from pdm.backend.base import Builder
@@ -52,17 +52,25 @@
     def config_settings(self) -> dict[str, str]:
         """The config settings passed to the hook"""
         return self.builder.config_settings
 
     def ensure_build_dir(self) -> Path:
         """Return the build dir and create if it doesn't exist"""
         if not self.build_dir.exists():
-            self.build_dir.mkdir(mode=0o700, parents=True)
+            self.build_dir.mkdir(mode=0o700, parents=True, exist_ok=True)
+            (self.build_dir / ".gitignore").write_text("*\n")
         return self.build_dir
 
+    def expand_paths(self, path: str) -> Iterable[Path]:
+        plib_path = Path(path)
+        if plib_path.parts and plib_path.parts[0] == "${BUILD_DIR}":
+            return self.build_dir.glob(Path(*plib_path.parts[1:]).as_posix())
+
+        return self.root.glob(path)
+
 
 class BuildHookInterface(Protocol):
     """The interface definition for build hooks.
 
     Custom hooks can implement part of the methods to provide corresponding abilities.
     """
```

### Comparing `pdm_backend-2.0.7/src/pdm/backend/hooks/setuptools.py` & `pdm_backend-2.1.0/src/pdm/backend/hooks/setuptools.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/hooks/version/__init__.py` & `pdm_backend-2.1.0/src/pdm/backend/hooks/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/hooks/version/scm.py` & `pdm_backend-2.1.0/src/pdm/backend/hooks/version/scm.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,31 +9,34 @@
 import shlex
 import shutil
 import subprocess
 import warnings
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
-from typing import Any, Iterable, NamedTuple
+from typing import TYPE_CHECKING, Iterable, NamedTuple
 
 from pdm.backend._vendor.packaging.version import Version
 
+if TYPE_CHECKING:
+    from _typeshed import StrPath
+
 DEFAULT_TAG_REGEX = re.compile(
     r"^(?:[\w-]+-)?(?P<version>[vV]?\d+(?:\.\d+){0,2}[^\+]*)(?:\+.*)?$"
 )
 
 
 @dataclass(frozen=True)
 class Config:
     tag_regex: re.Pattern
 
 
 def _subprocess_call(
     cmd: str | list[str],
-    cwd: os.PathLike | None = None,
+    cwd: StrPath | None = None,
     extra_env: dict[str, str] | None = None,
 ) -> tuple[int, str, str]:
     # adapted from pre-commit
     # Too many bugs dealing with environment variables and GIT:
     # https://github.com/pre-commit/pre-commit/issues/300
     env = {
         k: v
@@ -74,34 +77,34 @@
     branch: str | None = None,
 ) -> VersionInfo:
     if isinstance(tag, str):
         tag = tag_to_version(config, tag)
     return VersionInfo(tag, distance, dirty, node, branch)
 
 
-def _git_get_branch(root: os.PathLike[Any]) -> str | None:
+def _git_get_branch(root: StrPath) -> str | None:
     ret, out, _ = _subprocess_call("git rev-parse --abbrev-ref HEAD", root)
     if not ret:
         return out
     return None
 
 
-def _git_is_dirty(root: os.PathLike[Any]) -> bool:
+def _git_is_dirty(root: StrPath) -> bool:
     _, out, _ = _subprocess_call("git status --porcelain --untracked-files=no", root)
     return bool(out)
 
 
-def _git_get_node(root: os.PathLike[Any]) -> str | None:
+def _git_get_node(root: StrPath) -> str | None:
     ret, out, _ = _subprocess_call("git rev-parse --verify --quiet HEAD", root)
     if not ret:
         return out[:7]
     return None
 
 
-def _git_count_all_nodes(root: os.PathLike[Any]) -> int:
+def _git_count_all_nodes(root: StrPath) -> int:
     _, out, _ = _subprocess_call("git rev-list HEAD", root)
     return out.count("\n") + 1
 
 
 def _git_parse_describe(describe_output: str) -> tuple[str, int, str, bool]:
     # 'describe_output' looks e.g. like 'v1.5.0-0-g4060507' or
     # 'v1.15.1rc1-37-g9bd1298-dirty'.
@@ -165,43 +168,43 @@
     take tags that might be prefixed with a keyword and return only the version part
     :param tags: an iterable of tags
     :param config: optional configuration object
     """
     return [tag_to_version(config, tag) for tag in tags if tag]
 
 
-def git_parse_version(root: os.PathLike[Any], config: Config) -> VersionInfo | None:
+def git_parse_version(root: StrPath, config: Config) -> VersionInfo | None:
     GIT = shutil.which("git")
     if not GIT:
         return None
 
     ret, repo, _ = _subprocess_call([GIT, "rev-parse", "--show-toplevel"], root)
-    if ret or not os.path.samefile(root, repo):
+    if ret or not repo:
         return None
 
-    if os.path.isfile(os.path.join(root, ".git/shallow")):
-        warnings.warn(f"{root!r} is shallow and may cause errors")
+    if os.path.isfile(os.path.join(repo, ".git/shallow")):
+        warnings.warn(f"{repo!r} is shallow and may cause errors")
     describe_cmd = [GIT, "describe", "--dirty", "--tags", "--long", "--match", "*.*"]
-    ret, output, err = _subprocess_call(describe_cmd, root)
-    branch = _git_get_branch(root)
+    ret, output, err = _subprocess_call(describe_cmd, repo)
+    branch = _git_get_branch(repo)
 
     if ret:
-        rev_node = _git_get_node(root)
-        dirty = _git_is_dirty(root)
+        rev_node = _git_get_node(repo)
+        dirty = _git_is_dirty(repo)
         if rev_node is None:
             return meta(config, "0.0", 0, dirty)
         return meta(
-            config, "0.0", _git_count_all_nodes(root), dirty, f"g{rev_node}", branch
+            config, "0.0", _git_count_all_nodes(repo), dirty, f"g{rev_node}", branch
         )
     else:
         tag, number, node, dirty = _git_parse_describe(output)
         return meta(config, tag, number or None, dirty, node, branch)
 
 
-def get_latest_normalizable_tag(root: os.PathLike[Any]) -> str:
+def get_latest_normalizable_tag(root: StrPath) -> str:
     # Gets all tags containing a '.' from oldest to newest
     cmd = [
         "hg",
         "log",
         "-r",
         "ancestors(.) and tag('re:\\.')",
         "--template",
@@ -211,22 +214,22 @@
     outlines = output.split()
     if not outlines:
         return "null"
     tag = outlines[-1].split()[-1]
     return tag
 
 
-def hg_get_graph_distance(root: os.PathLike[Any], rev1: str, rev2: str = ".") -> int:
+def hg_get_graph_distance(root: StrPath, rev1: str, rev2: str = ".") -> int:
     cmd = ["hg", "log", "-q", "-r", f"{rev1}::{rev2}"]
     _, out, _ = _subprocess_call(cmd, root)
     return len(out.strip().splitlines()) - 1
 
 
 def _hg_tagdist_normalize_tagcommit(
-    config: Config, root: os.PathLike[Any], tag: str, dist: int, node: str, branch: str
+    config: Config, root: StrPath, tag: str, dist: int, node: str, branch: str
 ) -> VersionInfo:
     dirty = node.endswith("+")
     node = "h" + node.strip("+")
 
     # Detect changes since the specified tag
     revset = (
         "(branch(.)"  # look for revisions in this branch only
@@ -271,15 +274,15 @@
 def _bump_regex(version: str) -> str:
     match = re.match(r"(.*?)(\d+)$", version)
     assert match is not None
     prefix, tail = match.groups()
     return "%s%d" % (prefix, int(tail) + 1)
 
 
-def hg_parse_version(root: os.PathLike[Any], config: Config) -> VersionInfo | None:
+def hg_parse_version(root: StrPath, config: Config) -> VersionInfo | None:
     if not shutil.which("hg"):
         return None
     _, output, _ = _subprocess_call("hg id -i -b -t", root)
     identity_data = output.split()
     if not identity_data:
         return None
     node = identity_data.pop(0)
@@ -325,12 +328,13 @@
 
 
 def get_version_from_scm(root: str | Path, *, tag_regex: str | None = None) -> str:
     config = Config(tag_regex=re.compile(tag_regex) if tag_regex else DEFAULT_TAG_REGEX)
     for func in (git_parse_version, hg_parse_version):
         version = func(root, config)  # type: ignore
         if version:
-            break
-    else:
-        version = meta(config, "0.0.0")
-    assert version is not None
-    return format_version(version)
+            return format_version(version)
+    raise ValueError(
+        "Cannot find the version from SCM or SCM isn't detected. \n"
+        "You can still specify the version via environment variable "
+        "`PDM_BUILD_SCM_VERSION`."
+    )
```

### Comparing `pdm_backend-2.0.7/src/pdm/backend/intree.py` & `pdm_backend-2.1.0/src/pdm/backend/intree.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/macosx_platform.py` & `pdm_backend-2.1.0/src/pdm/backend/macosx_platform.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/sdist.py` & `pdm_backend-2.1.0/src/pdm/backend/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/structures.py` & `pdm_backend-2.1.0/src/pdm/backend/structures.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/utils.py` & `pdm_backend-2.1.0/src/pdm/backend/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/src/pdm/backend/wheel.py` & `pdm_backend-2.1.0/src/pdm/backend/wheel.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     expand_vars,
     get_abi_tag,
     get_platform,
     safe_version,
     to_filename,
 )
 
+SCHEME_NAMES = frozenset(
+    ["purelib", "platlib", "include", "platinclude", "scripts", "data"]
+)
+
 if sys.version_info < (3, 8):
     from importlib_metadata import version as get_version
 else:
     from importlib.metadata import version as get_version
 
 WHEEL_FILE_FORMAT = """\
 Wheel-Version: 1.0
@@ -68,14 +72,21 @@
 
     def __init__(
         self, location: str | Path, config_settings: Mapping[str, Any] | None = None
     ) -> None:
         super().__init__(location, config_settings)
         self.__tag: str | None = None
 
+    def scheme_path(self, name: str, relative: str) -> str:
+        if name not in SCHEME_NAMES:
+            raise ValueError(
+                f"Unknown scheme name {name!r}, must be one of {SCHEME_NAMES}"
+            )
+        return f"{self.name_version}.data/{name}/{relative}"
+
     def _get_platform_tags(self) -> tuple[str | None, str | None, str | None]:
         python_tag: str | None = None
         py_limited_api: str | None = None
         plat_name: str | None = None
         if not self.config_settings:
             return python_tag, py_limited_api, plat_name
         if "--python-tag" in self.config_settings:
@@ -114,14 +125,30 @@
         package_dir = self.config.build_config.package_dir
         for relpath, path in super().get_files(context):
             # remove the package-dir part from the relative paths
             if package_dir and relpath.startswith(package_dir + "/"):
                 relpath = relpath[len(package_dir) + 1 :]
             yield relpath, path
         yield from self._get_metadata_files(context)
+        yield from self._get_wheel_data(context)
+
+    def _get_wheel_data(self, context: Context) -> Iterable[tuple[str, Path]]:
+        for name, paths in context.config.build_config.wheel_data.items():
+            for path in paths:
+                relative_to: str | None = None
+                if not isinstance(path, str):
+                    relative_to = path.get("relative-to")
+                    path = path["path"]
+                for child in context.expand_paths(path):
+                    relpath = (
+                        child.relative_to(relative_to).as_posix()
+                        if relative_to
+                        else child.name
+                    )
+                    yield self.scheme_path(name, relpath), child
 
     def build_artifact(
         self, context: Context, files: Iterable[tuple[str, Path]]
     ) -> Path:
         records: list[RecordEntry] = []
         with tempfile.NamedTemporaryFile(suffix=".whl", delete=False) as fp:
             with zipfile.ZipFile(fp, "w", compression=zipfile.ZIP_DEFLATED) as zf:
@@ -180,15 +207,15 @@
                 tag in supported_tags
             ), f"would build wheel with unsupported tag {tag}"
         return "-".join(tag)  # type: ignore[arg-type]
 
     def _write_dist_info(self, parent: Path) -> Path:
         """write the dist-info directory and return the path to it"""
         dist_info = parent / self.dist_info_name
-        dist_info.mkdir(0o700, parents=True, exist_ok=True)
+        dist_info.mkdir(0o700, exist_ok=True)
         meta = self.config.metadata
         entry_points = meta.entry_points
         if entry_points:
             with _open_for_write(dist_info / "entry_points.txt") as f:
                 self._write_entry_points(f, entry_points)
 
         with _open_for_write(dist_info / "WHEEL") as f:
@@ -267,15 +294,15 @@
             fp.write("\n")
 
     def _get_metadata_files(self, context: Context) -> Iterable[tuple[str, Path]]:
         """Generate the metadata files for the wheel."""
         if context.kwargs.get("metadata_directory"):
             return self._iter_files_in_directory(context.kwargs["metadata_directory"])
         else:
-            dist_info = self._write_dist_info(context.build_dir)
+            dist_info = self._write_dist_info(context.ensure_build_dir())
             return self._iter_files_in_directory(str(dist_info))
 
     def _iter_files_in_directory(self, path: str) -> Iterable[tuple[str, Path]]:
         for root, _, files in os.walk(path):
             relroot = os.path.relpath(root, os.path.dirname(path))
             for file in files:
                 yield (Path(relroot, file).as_posix(), Path(root) / file)
```

### Comparing `pdm_backend-2.0.7/tests/conftest.py` & `pdm_backend-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/hooks/hook_class.py` & `pdm_backend-2.1.0/tests/fixtures/hooks/hook_class.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/hooks/hook_module.py` & `pdm_backend-2.1.0/tests/fixtures/hooks/hook_module.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/hooks/local_hook.py` & `pdm_backend-2.1.0/tests/fixtures/hooks/local_hook.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-cextension/pyproject.toml` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-cextension/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/pdm.lock` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include-error/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/pyproject.toml` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include-error/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/requirements.txt` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include-error/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/pdm.lock` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/requirements.txt` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-include/requirements_simple.txt` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-package-include/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/pdm.lock` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-tests/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-package-with-tests/pyproject.toml` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-package-with-tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-package/pdm.lock` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-package/requirements.txt` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-package/requirements_simple.txt` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-package/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml` & `pdm_backend-2.1.0/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/test_api.py` & `pdm_backend-2.1.0/tests/test_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import email
+import os
 import sys
 import zipfile
 from pathlib import Path
 
 import pytest
 
 import pdm.backend as api
@@ -79,25 +80,31 @@
     with build_fixture_project("demo-package-include"):
         wheel_name = api.build_wheel(tmp_path.as_posix())
         sdist_name = api.build_sdist(tmp_path.as_posix())
         assert sdist_name == "demo_package-0.1.0.tar.gz"
         assert wheel_name == "demo_package-0.1.0-py3-none-any.whl"
 
         tar_names = get_tarball_names(tmp_path / sdist_name)
-        zip_names = get_wheel_names(tmp_path / wheel_name)
 
         assert "demo_package-0.1.0/my_package/__init__.py" in tar_names
         assert "demo_package-0.1.0/my_package/data.json" not in tar_names
         assert "demo_package-0.1.0/requirements.txt" in tar_names
         assert "demo_package-0.1.0/data_out.json" in tar_names
 
-        assert "my_package/__init__.py" in zip_names
-        assert "my_package/data.json" not in zip_names
-        assert "requirements.txt" in zip_names
-        assert "data_out.json" in zip_names
+        with zipfile.ZipFile(tmp_path / wheel_name) as zf:
+            zip_names = zf.namelist()
+            assert "my_package/__init__.py" in zip_names
+            assert "my_package/data.json" not in zip_names
+            assert "requirements.txt" in zip_names
+            assert "data_out.json" in zip_names
+            assert "demo_package-0.1.0.data/scripts/my_script.sh" in zip_names
+            if os.name != "nt":
+                info = zf.getinfo("demo_package-0.1.0.data/scripts/my_script.sh")
+                filemode = info.external_attr >> 16
+                assert filemode & 0o111
 
 
 def test_namespace_package_by_include(tmp_path: Path) -> None:
     with build_fixture_project("demo-pep420-package"):
         wheel_name = api.build_wheel(tmp_path.as_posix())
         sdist_name = api.build_sdist(tmp_path.as_posix())
         assert sdist_name == "demo_package-0.1.0.tar.gz"
@@ -374,7 +381,63 @@
     )
     with builder:
         wheel_name = builder.build(project_with_scm / "dist")
         assert wheel_name.name == "foo-1.1.1-py3-none-any.whl"
         with zipfile.ZipFile(wheel_name) as zf:
             version = zf.read("foo/__version__.py").decode("utf-8").strip()
         assert version == "1.1.1"
+
+
+@pytest.mark.parametrize(
+    "settings, cleanup", [("true", False), ("false", True), ("0", True), ("1", False)]
+)
+def test_clean_not_called_if_envset(
+    project_with_scm: Path,
+    monkeypatch: pytest.MonkeyPatch,
+    settings: str,
+    cleanup: bool,
+) -> None:
+    monkeypatch.setenv("PDM_BUILD_NO_CLEAN", settings)
+    builder = WheelBuilder(project_with_scm)
+    builder.config.data.setdefault("tool", {}).setdefault("pdm", {})["version"] = {
+        "source": "scm",
+        "write_to": "foo/__version__.py",
+    }
+
+    test_file = project_with_scm / ".pdm-build" / "testfile"
+    os.makedirs(project_with_scm / ".pdm-build", exist_ok=True)
+    test_file.touch()
+    assert os.path.exists(test_file)
+
+    with builder:
+        builder.build(project_with_scm / "dist")
+        if cleanup:
+            assert not os.path.exists(test_file)
+        else:
+            assert os.path.exists(test_file)
+
+
+@pytest.mark.parametrize(
+    "settings, cleanup", [("", False), (True, False), (None, False)]
+)
+def test_clean_not_called_if_config_settings_exist(
+    project_with_scm: Path, settings: bool, cleanup: bool
+) -> None:
+    builder = WheelBuilder(
+        project_with_scm, config_settings={"no-clean-build": settings}
+    )
+    builder.config.data.setdefault("tool", {}).setdefault("pdm", {})["version"] = {
+        "source": "scm",
+        "write_to": "foo/__version__.py",
+    }
+
+    test_file = project_with_scm / ".pdm-build" / "testfile"
+    os.makedirs(project_with_scm / ".pdm-build", exist_ok=True)
+    test_file.touch()
+    assert os.path.exists(test_file)
+
+    with builder:
+        builder.build(project_with_scm / "dist")
+        if cleanup:
+            assert not os.path.exists(test_file)
+        else:
+            assert os.path.exists(test_file)
```

### Comparing `pdm_backend-2.0.7/tests/test_file_finder.py` & `pdm_backend-2.1.0/tests/test_file_finder.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/test_hooks.py` & `pdm_backend-2.1.0/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/test_metadata.py` & `pdm_backend-2.1.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/test_wheel.py` & `pdm_backend-2.1.0/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/tests/testutils.py` & `pdm_backend-2.1.0/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.0.7/PKG-INFO` & `pdm_backend-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-backend
-Version: 2.0.7
+Version: 2.1.0
 Summary: The build backend used by PDM that supports latest packaging standards
 Keywords: packaging PEP 517 build
 Author-Email: Frost Ming <me@frostming.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdm-backend Version: 2.0.7 Summary: The build
+Metadata-Version: 2.1 Name: pdm-backend Version: 2.1.0 Summary: The build
 backend used by PDM that supports latest packaging standards Keywords:
 packaging PEP 517 build Author-Email: Frost Ming
 frostming.com> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

