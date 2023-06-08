# Comparing `tmp/quickmpc-0.3.9.tar.gz` & `tmp/quickmpc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-1wkr63ag/quickmpc-0.3.9.tar", last modified: Tue May 23 12:38:08 2023, max compression
+gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-jwzx7ry0/quickmpc-0.4.0.tar", last modified: Thu Jun  8 06:09:02 2023, max compression
```

## Comparing `quickmpc-0.3.9.tar` & `quickmpc-0.4.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:38:08.000000 quickmpc-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-23 12:37:53.000000 quickmpc-0.3.9/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-23 12:37:53.000000 quickmpc-0.3.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-23 12:37:53.000000 quickmpc-0.3.9/.isort.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:38:08.000000 quickmpc-0.3.9/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-23 12:37:53.000000 quickmpc-0.3.9/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 12:37:53.000000 quickmpc-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-23 12:37:53.000000 quickmpc-0.3.9/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-23 12:38:08.000000 quickmpc-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-23 12:37:53.000000 quickmpc-0.3.9/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-05-23 12:37:53.000000 quickmpc-0.3.9/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-23 12:37:53.000000 quickmpc-0.3.9/README-ja.md
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-23 12:37:53.000000 quickmpc-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-23 12:37:53.000000 quickmpc-0.3.9/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-23 12:37:53.000000 quickmpc-0.3.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:38:08.000000 quickmpc-0.3.9/quickmpc/
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 12:38:08.000000 quickmpc-0.3.9/quickmpc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:38:08.000000 quickmpc-0.3.9/quickmpc/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/proto/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:38:08.000000 quickmpc-0.3.9/quickmpc/proto/common_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/proto/common_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/proto/common_types/common_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/proto/common_types/common_types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/proto/libc_to_manage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/proto/libc_to_manage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/proto/libc_to_manage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/qmpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/share.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:38:08.000000 quickmpc-0.3.9/quickmpc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/utils/if_present.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/utils/make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/utils/overload_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/utils/parse_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/utils/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-23 12:37:53.000000 quickmpc-0.3.9/quickmpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:38:08.000000 quickmpc-0.3.9/quickmpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-23 12:38:08.000000 quickmpc-0.3.9/quickmpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-23 12:38:08.000000 quickmpc-0.3.9/quickmpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:38:08.000000 quickmpc-0.3.9/quickmpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 12:38:08.000000 quickmpc-0.3.9/quickmpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 12:38:08.000000 quickmpc-0.3.9/quickmpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-23 12:38:08.000000 quickmpc-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 12:37:53.000000 quickmpc-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:38:08.000000 quickmpc-0.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:38:08.000000 quickmpc-0.3.9/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:38:08.000000 quickmpc-0.3.9/tests/unit_tests/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/certificates/server1.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/certificates/server1.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/certificates/server2.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/certificates/server2.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/certificates/server3.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/certificates/server3.pem
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/local_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:38:08.000000 quickmpc-0.3.9/tests/unit_tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_files/bitvector.csv
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_files/diff_col.csv
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_files/edge_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_files/empty.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_files/none.csv
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_files/normal.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_files/not_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_files/over_number.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_files/string_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_over_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_share_recons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tests/unit_tests/test_share_sharize.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-23 12:37:53.000000 quickmpc-0.3.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-08 06:08:46.000000 quickmpc-0.4.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 06:08:46.000000 quickmpc-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-08 06:08:46.000000 quickmpc-0.4.0/.isort.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-08 06:08:46.000000 quickmpc-0.4.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 06:08:46.000000 quickmpc-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-08 06:08:46.000000 quickmpc-0.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-08 06:09:02.000000 quickmpc-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-08 06:08:46.000000 quickmpc-0.4.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-06-08 06:08:46.000000 quickmpc-0.4.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-08 06:08:46.000000 quickmpc-0.4.0/README-ja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-08 06:08:46.000000 quickmpc-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-08 06:08:46.000000 quickmpc-0.4.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 06:08:46.000000 quickmpc-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc/proto/common_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/common_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/common_types/common_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/common_types/common_types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/qmpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/share.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/utils/if_present.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/utils/make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/utils/overload_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/utils/parse_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/utils/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-08 06:09:02.000000 quickmpc-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 06:08:46.000000 quickmpc-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/tests/unit_tests/certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/certificates/server1.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/certificates/server1.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/certificates/server2.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/certificates/server2.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/certificates/server3.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/certificates/server3.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/local_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/tests/unit_tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/bitvector.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/diff_col.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/edge_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/none.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/normal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/not_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/over_number.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/string_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_over_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_share_recons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_share_sharize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tox.ini
```

### Comparing `quickmpc-0.3.9/.vscode/settings.json` & `quickmpc-0.4.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/LICENSE` & `quickmpc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/Pipfile.lock` & `quickmpc-0.4.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/README-ja.md` & `quickmpc-0.4.0/README-ja.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/README.md` & `quickmpc-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/mypy.ini` & `quickmpc-0.4.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/quickmpc/proto/common_types/common_types_pb2.py` & `quickmpc-0.4.0/quickmpc/proto/common_types/common_types_pb2.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/quickmpc/proto/common_types/common_types_pb2.pyi` & `quickmpc-0.4.0/quickmpc/proto/common_types/common_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/quickmpc/proto/libc_to_manage_pb2.py` & `quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14libc_to_manage.proto\x12\x0clibctomanage\x1a\x1f\x63ommon_types/common_types.proto\x1a\x1bgoogle/protobuf/empty.proto\"\xa8\x01\n\x11SendSharesRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\t\x12\x0e\n\x06shares\x18\x02 \x01(\t\x12\'\n\x06schema\x18\x03 \x03(\x0b\x32\x17.pb_common_types.Schema\x12\x10\n\x08piece_id\x18\x04 \x01(\x05\x12\x0f\n\x07sent_at\x18\x05 \x01(\t\x12\x17\n\x0fmatching_column\x18\x06 \x01(\x05\x12\r\n\x05token\x18\x07 \x01(\t\"5\n\x13\x44\x65leteSharesRequest\x12\x0f\n\x07\x64\x61taIds\x18\x01 \x03(\t\x12\r\n\x05token\x18\x02 \x01(\t\"2\n\x10GetSchemaRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"<\n\x11GetSchemaResponse\x12\'\n\x06schema\x18\x01 \x03(\x0b\x32\x17.pb_common_types.Schema\"9\n\tJoinOrder\x12\x0f\n\x07\x64\x61taIds\x18\x01 \x03(\t\x12\x0c\n\x04join\x18\x02 \x03(\x05\x12\r\n\x05index\x18\x03 \x03(\x05\"$\n\x05Input\x12\x0b\n\x03src\x18\x01 \x03(\x05\x12\x0e\n\x06target\x18\x02 \x03(\x05\"\xab\x01\n\x19\x45xecuteComputationRequest\x12\x35\n\tmethod_id\x18\x01 \x01(\x0e\x32\".pb_common_types.ComputationMethod\x12\r\n\x05token\x18\x02 \x01(\t\x12&\n\x05table\x18\x03 \x01(\x0b\x32\x17.libctomanage.JoinOrder\x12 \n\x03\x61rg\x18\x04 \x01(\x0b\x32\x13.libctomanage.Input\".\n\x1a\x45xecuteComputationResponse\x12\x10\n\x08job_uuid\x18\x03 \x01(\t\">\n\x1bGetComputationResultRequest\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"\x8f\x02\n\x1cGetComputationResultResponse\x12\x0e\n\x06result\x18\x03 \x03(\t\x12\x15\n\rcolumn_number\x18\x04 \x01(\x05\x12*\n\x06status\x18\x05 \x01(\x0e\x32\x1a.pb_common_types.JobStatus\x12\x10\n\x08piece_id\x18\x06 \x01(\x05\x12\x33\n\x08progress\x18\x07 \x01(\x0b\x32\x1c.pb_common_types.JobProgressH\x01\x88\x01\x01\x12\x11\n\x07is_dim1\x18\x08 \x01(\x08H\x00\x12\x11\n\x07is_dim2\x18\t \x01(\x08H\x00\x12\x13\n\tis_schema\x18\n \x01(\x08H\x00\x42\r\n\x0bresult_typeB\x0b\n\t_progress\"#\n\x12GetDataListRequest\x12\r\n\x05token\x18\x01 \x01(\t\"%\n\x13GetDataListResponse\x12\x0e\n\x06result\x18\x01 \x01(\t\"8\n\x15GetElapsedTimeRequest\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\".\n\x16GetElapsedTimeResponse\x12\x14\n\x0c\x65lapsed_time\x18\x01 \x01(\x01\"9\n\x16GetJobErrorInfoRequest\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"h\n\x17GetJobErrorInfoResponse\x12:\n\x0ejob_error_info\x18\x01 \x01(\x0b\x32\x1d.pb_common_types.JobErrorInfoH\x00\x88\x01\x01\x42\x11\n\x0f_job_error_info2\xe9\x05\n\x0cLibcToManage\x12G\n\nSendShares\x12\x1f.libctomanage.SendSharesRequest\x1a\x16.google.protobuf.Empty\"\x00\x12K\n\x0c\x44\x65leteShares\x12!.libctomanage.DeleteSharesRequest\x1a\x16.google.protobuf.Empty\"\x00\x12N\n\tGetSchema\x12\x1e.libctomanage.GetSchemaRequest\x1a\x1f.libctomanage.GetSchemaResponse\"\x00\x12i\n\x12\x45xecuteComputation\x12\'.libctomanage.ExecuteComputationRequest\x1a(.libctomanage.ExecuteComputationResponse\"\x00\x12q\n\x14GetComputationResult\x12).libctomanage.GetComputationResultRequest\x1a*.libctomanage.GetComputationResultResponse\"\x00\x30\x01\x12T\n\x0bGetDataList\x12 .libctomanage.GetDataListRequest\x1a!.libctomanage.GetDataListResponse\"\x00\x12]\n\x0eGetElapsedTime\x12#.libctomanage.GetElapsedTimeRequest\x1a$.libctomanage.GetElapsedTimeResponse\"\x00\x12`\n\x0fGetJobErrorInfo\x12$.libctomanage.GetJobErrorInfoRequest\x1a%.libctomanage.GetJobErrorInfoResponse\"\x00\x42\x45ZCgithub.com/acompany-develop/QuickMPC/proto/libc_to_manage_containerb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14libc_to_manage.proto\x12\x0clibctomanage\x1a\x1f\x63ommon_types/common_types.proto\x1a\x1bgoogle/protobuf/empty.proto\"\xa8\x01\n\x11SendSharesRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\t\x12\x0e\n\x06shares\x18\x02 \x01(\t\x12\'\n\x06schema\x18\x03 \x03(\x0b\x32\x17.pb_common_types.Schema\x12\x10\n\x08piece_id\x18\x04 \x01(\x05\x12\x0f\n\x07sent_at\x18\x05 \x01(\t\x12\x17\n\x0fmatching_column\x18\x06 \x01(\x05\x12\r\n\x05token\x18\x07 \x01(\t\"5\n\x13\x44\x65leteSharesRequest\x12\x0f\n\x07\x64\x61taIds\x18\x01 \x03(\t\x12\r\n\x05token\x18\x02 \x01(\t\"2\n\x10GetSchemaRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"<\n\x11GetSchemaResponse\x12\'\n\x06schema\x18\x01 \x03(\x0b\x32\x17.pb_common_types.Schema\"1\n\tJoinOrder\x12\x10\n\x08\x64\x61ta_ids\x18\x01 \x03(\t\x12\x12\n\ndebug_mode\x18\x02 \x01(\x08\"$\n\x05Input\x12\x0b\n\x03src\x18\x01 \x03(\x05\x12\x0e\n\x06target\x18\x02 \x03(\x05\"\xab\x01\n\x19\x45xecuteComputationRequest\x12\x35\n\tmethod_id\x18\x01 \x01(\x0e\x32\".pb_common_types.ComputationMethod\x12\r\n\x05token\x18\x02 \x01(\t\x12&\n\x05table\x18\x03 \x01(\x0b\x32\x17.libctomanage.JoinOrder\x12 \n\x03\x61rg\x18\x04 \x01(\x0b\x32\x13.libctomanage.Input\".\n\x1a\x45xecuteComputationResponse\x12\x10\n\x08job_uuid\x18\x03 \x01(\t\">\n\x1bGetComputationResultRequest\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"\x8f\x02\n\x1cGetComputationResultResponse\x12\x0e\n\x06result\x18\x03 \x03(\t\x12\x15\n\rcolumn_number\x18\x04 \x01(\x05\x12*\n\x06status\x18\x05 \x01(\x0e\x32\x1a.pb_common_types.JobStatus\x12\x10\n\x08piece_id\x18\x06 \x01(\x05\x12\x33\n\x08progress\x18\x07 \x01(\x0b\x32\x1c.pb_common_types.JobProgressH\x01\x88\x01\x01\x12\x11\n\x07is_dim1\x18\x08 \x01(\x08H\x00\x12\x11\n\x07is_dim2\x18\t \x01(\x08H\x00\x12\x13\n\tis_schema\x18\n \x01(\x08H\x00\x42\r\n\x0bresult_typeB\x0b\n\t_progress\"#\n\x12GetDataListRequest\x12\r\n\x05token\x18\x01 \x01(\t\"%\n\x13GetDataListResponse\x12\x0e\n\x06result\x18\x01 \x01(\t\"8\n\x15GetElapsedTimeRequest\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\".\n\x16GetElapsedTimeResponse\x12\x14\n\x0c\x65lapsed_time\x18\x01 \x01(\x01\"9\n\x16GetJobErrorInfoRequest\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"h\n\x17GetJobErrorInfoResponse\x12:\n\x0ejob_error_info\x18\x01 \x01(\x0b\x32\x1d.pb_common_types.JobErrorInfoH\x00\x88\x01\x01\x42\x11\n\x0f_job_error_info2\xe9\x05\n\x0cLibcToManage\x12G\n\nSendShares\x12\x1f.libctomanage.SendSharesRequest\x1a\x16.google.protobuf.Empty\"\x00\x12K\n\x0c\x44\x65leteShares\x12!.libctomanage.DeleteSharesRequest\x1a\x16.google.protobuf.Empty\"\x00\x12N\n\tGetSchema\x12\x1e.libctomanage.GetSchemaRequest\x1a\x1f.libctomanage.GetSchemaResponse\"\x00\x12i\n\x12\x45xecuteComputation\x12\'.libctomanage.ExecuteComputationRequest\x1a(.libctomanage.ExecuteComputationResponse\"\x00\x12q\n\x14GetComputationResult\x12).libctomanage.GetComputationResultRequest\x1a*.libctomanage.GetComputationResultResponse\"\x00\x30\x01\x12T\n\x0bGetDataList\x12 .libctomanage.GetDataListRequest\x1a!.libctomanage.GetDataListResponse\"\x00\x12]\n\x0eGetElapsedTime\x12#.libctomanage.GetElapsedTimeRequest\x1a$.libctomanage.GetElapsedTimeResponse\"\x00\x12`\n\x0fGetJobErrorInfo\x12$.libctomanage.GetJobErrorInfoRequest\x1a%.libctomanage.GetJobErrorInfoResponse\"\x00\x42\x45ZCgithub.com/acompany-develop/QuickMPC/proto/libc_to_manage_containerb\x06proto3')
 
 
 _SENDSHARESREQUEST = DESCRIPTOR.message_types_by_name['SendSharesRequest']
 _DELETESHARESREQUEST = DESCRIPTOR.message_types_by_name['DeleteSharesRequest']
 _GETSCHEMAREQUEST = DESCRIPTOR.message_types_by_name['GetSchemaRequest']
 _GETSCHEMARESPONSE = DESCRIPTOR.message_types_by_name['GetSchemaResponse']
 _JOINORDER = DESCRIPTOR.message_types_by_name['JoinOrder']
@@ -155,33 +155,33 @@
     _DELETESHARESREQUEST._serialized_start = 271
     _DELETESHARESREQUEST._serialized_end = 324
     _GETSCHEMAREQUEST._serialized_start = 326
     _GETSCHEMAREQUEST._serialized_end = 376
     _GETSCHEMARESPONSE._serialized_start = 378
     _GETSCHEMARESPONSE._serialized_end = 438
     _JOINORDER._serialized_start = 440
-    _JOINORDER._serialized_end = 497
-    _INPUT._serialized_start = 499
-    _INPUT._serialized_end = 535
-    _EXECUTECOMPUTATIONREQUEST._serialized_start = 538
-    _EXECUTECOMPUTATIONREQUEST._serialized_end = 709
-    _EXECUTECOMPUTATIONRESPONSE._serialized_start = 711
-    _EXECUTECOMPUTATIONRESPONSE._serialized_end = 757
-    _GETCOMPUTATIONRESULTREQUEST._serialized_start = 759
-    _GETCOMPUTATIONRESULTREQUEST._serialized_end = 821
-    _GETCOMPUTATIONRESULTRESPONSE._serialized_start = 824
-    _GETCOMPUTATIONRESULTRESPONSE._serialized_end = 1095
-    _GETDATALISTREQUEST._serialized_start = 1097
-    _GETDATALISTREQUEST._serialized_end = 1132
-    _GETDATALISTRESPONSE._serialized_start = 1134
-    _GETDATALISTRESPONSE._serialized_end = 1171
-    _GETELAPSEDTIMEREQUEST._serialized_start = 1173
-    _GETELAPSEDTIMEREQUEST._serialized_end = 1229
-    _GETELAPSEDTIMERESPONSE._serialized_start = 1231
-    _GETELAPSEDTIMERESPONSE._serialized_end = 1277
-    _GETJOBERRORINFOREQUEST._serialized_start = 1279
-    _GETJOBERRORINFOREQUEST._serialized_end = 1336
-    _GETJOBERRORINFORESPONSE._serialized_start = 1338
-    _GETJOBERRORINFORESPONSE._serialized_end = 1442
-    _LIBCTOMANAGE._serialized_start = 1445
-    _LIBCTOMANAGE._serialized_end = 2190
+    _JOINORDER._serialized_end = 489
+    _INPUT._serialized_start = 491
+    _INPUT._serialized_end = 527
+    _EXECUTECOMPUTATIONREQUEST._serialized_start = 530
+    _EXECUTECOMPUTATIONREQUEST._serialized_end = 701
+    _EXECUTECOMPUTATIONRESPONSE._serialized_start = 703
+    _EXECUTECOMPUTATIONRESPONSE._serialized_end = 749
+    _GETCOMPUTATIONRESULTREQUEST._serialized_start = 751
+    _GETCOMPUTATIONRESULTREQUEST._serialized_end = 813
+    _GETCOMPUTATIONRESULTRESPONSE._serialized_start = 816
+    _GETCOMPUTATIONRESULTRESPONSE._serialized_end = 1087
+    _GETDATALISTREQUEST._serialized_start = 1089
+    _GETDATALISTREQUEST._serialized_end = 1124
+    _GETDATALISTRESPONSE._serialized_start = 1126
+    _GETDATALISTRESPONSE._serialized_end = 1163
+    _GETELAPSEDTIMEREQUEST._serialized_start = 1165
+    _GETELAPSEDTIMEREQUEST._serialized_end = 1221
+    _GETELAPSEDTIMERESPONSE._serialized_start = 1223
+    _GETELAPSEDTIMERESPONSE._serialized_end = 1269
+    _GETJOBERRORINFOREQUEST._serialized_start = 1271
+    _GETJOBERRORINFOREQUEST._serialized_end = 1328
+    _GETJOBERRORINFORESPONSE._serialized_start = 1330
+    _GETJOBERRORINFORESPONSE._serialized_end = 1434
+    _LIBCTOMANAGE._serialized_start = 1437
+    _LIBCTOMANAGE._serialized_end = 2182
 # @@protoc_insertion_point(module_scope)
```

### Comparing `quickmpc-0.3.9/quickmpc/proto/libc_to_manage_pb2.pyi` & `quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -120,31 +120,26 @@
 class JoinOrder(google.protobuf.message.Message):
     """*
     the message of ExecuteComputationRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DATAIDS_FIELD_NUMBER: builtins.int
-    JOIN_FIELD_NUMBER: builtins.int
-    INDEX_FIELD_NUMBER: builtins.int
+    DATA_IDS_FIELD_NUMBER: builtins.int
+    DEBUG_MODE_FIELD_NUMBER: builtins.int
     @property
-    def dataIds(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    @property
-    def join(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
-    @property
-    def index(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+    def data_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    debug_mode: builtins.bool
     def __init__(
         self,
         *,
-        dataIds: collections.abc.Iterable[builtins.str] | None = ...,
-        join: collections.abc.Iterable[builtins.int] | None = ...,
-        index: collections.abc.Iterable[builtins.int] | None = ...,
+        data_ids: collections.abc.Iterable[builtins.str] | None = ...,
+        debug_mode: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dataIds", b"dataIds", "index", b"index", "join", b"join"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["data_ids", b"data_ids", "debug_mode", b"debug_mode"]) -> None: ...
 
 global___JoinOrder = JoinOrder
 
 class Input(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SRC_FIELD_NUMBER: builtins.int
```

### Comparing `quickmpc-0.3.9/quickmpc/proto/libc_to_manage_pb2_grpc.py` & `quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/quickmpc/proto/libc_to_manage_pb2_grpc.pyi` & `quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/quickmpc/qmpc.py` & `quickmpc-0.4.0/quickmpc/qmpc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from dataclasses import dataclass, field, InitVar
 from typing import Dict, List, Optional, Tuple
 
 from .proto.common_types import common_types_pb2
 from .qmpc_server import QMPCServer
 from .share import Share
-from .utils.parse_csv import (parse, parse_csv)
+from .utils.parse_csv import parse, parse_csv
 from .utils.restore import restore
 
 logger = logging.getLogger(__name__)
 # qmpc.JobStatus でアクセスできるようにエイリアスを設定する
 JobStatus \
     = common_types_pb2.JobStatus
 ComputationMethod \
@@ -20,23 +20,25 @@
 
 
 @dataclass(frozen=True)
 class QMPC:
     endpoints: InitVar[List[str]]
     # tokenがちゃんと使用されるようになったらデフォルト値を外す
     token: InitVar[str] = "token_demo"
+    retry_num: InitVar[int] = 10
+    retry_wait_time: InitVar[int] = 5
 
     __qmpc_server: QMPCServer = field(init=False)
     __party_size: int = field(init=False)
 
     def __post_init__(self, endpoints: List[str],
-                      token: str):
+                      token: str, retry_num: int, retry_wait_time: int):
         logger.info(f"[QuickMPC server IP]={endpoints}")
         object.__setattr__(self, "_QMPC__qmpc_server", QMPCServer(
-            endpoints, token))
+            endpoints, token, retry_num, retry_wait_time))
         object.__setattr__(self, "_QMPC__party_size", len(endpoints))
 
     def send_share_from_csv_file(self,
                                  filename: str,
                                  matching_column: int = 1,
                                  piece_size: int = 1_000_000) -> Dict:
         secrets, schema = parse_csv(filename, matching_column)
@@ -58,90 +60,82 @@
             secrets, schema, matching_column, piece_size)
 
     def delete_share(self, data_ids: List[str]) -> Dict:
         logger.info("delete_share request. "
                     f"[delete id list]={data_ids}")
         return self.__qmpc_server.delete_share(data_ids)
 
-    def mean(self, join_order: Tuple[List[str], List[int], List[int]],
-             src: List) -> Dict:
+    def mean(self, data_ids: List[str], src: List,
+             *, debug_mode: bool = False) -> Dict:
         logger.info("mean request. "
-                    f"[data_id list]={join_order[0]} "
-                    f"[join method]={join_order[1]} "
-                    f"[matching ID columns]={join_order[2]} "
-                    f"[src columns]={src}")
+                    f"[data_id list]={data_ids} "
+                    f"[src columns]={src} "
+                    f"[debug_mode]={debug_mode}")
         return self.__qmpc_server.execute_computation(
             ComputationMethod.Value("COMPUTATION_METHOD_MEAN"),
-            join_order, (src, []))
+            data_ids, (src, []), debug_mode=debug_mode)
 
-    def variance(self, join_order: Tuple[List[str], List[int], List[int]],
-                 src: List) -> Dict:
+    def variance(self, data_ids: List[str], src: List,
+                 *, debug_mode: bool = False) -> Dict:
         logger.info("variance request. "
-                    f"[data_id list]={join_order[0]} "
-                    f"[join method]={join_order[1]} "
-                    f"[matching ID columns]={join_order[2]} "
-                    f"[src columns]={src}")
+                    f"[data_id list]={data_ids} "
+                    f"[src columns]={src} "
+                    f"[debug_mode]={debug_mode}")
         return self.__qmpc_server.execute_computation(
             ComputationMethod.Value("COMPUTATION_METHOD_VARIANCE"),
-            join_order, (src, []))
+            data_ids, (src, []), debug_mode=debug_mode)
 
-    def sum(self, join_order: Tuple[List[str], List[int], List[int]],
-            src: List) -> Dict:
+    def sum(self, data_ids: List[str], src: List,
+            *, debug_mode: bool = False) -> Dict:
         logger.info("sum request. "
-                    f"[data_id list]={join_order[0]} "
-                    f"[join method]={join_order[1]} "
-                    f"[matching ID columns]={join_order[2]} "
-                    f"[src columns]={src}")
+                    f"[data_id list]={data_ids} "
+                    f"[src columns]={src} "
+                    f"[debug_mode]={debug_mode}")
         return self.__qmpc_server.execute_computation(
             ComputationMethod.Value("COMPUTATION_METHOD_SUM"),
-            join_order, (src, []))
+            data_ids, (src, []), debug_mode=debug_mode)
 
-    def correl(self, join_order: Tuple[List[str], List[int], List[int]],
-               inp: Tuple[List[int], List[int]]) -> Dict:
+    def correl(self, data_ids: List[str], inp: Tuple[List[int], List[int]],
+               *, debug_mode: bool = False) -> Dict:
         logger.info("correl request. "
-                    f"[data_id list]={join_order[0]} "
-                    f"[join method]={join_order[1]} "
-                    f"[matching ID columns]={join_order[2]} "
+                    f"[data_id list]={data_ids} "
                     f"[src columns]={inp[0]}"
-                    f"[target columns]={inp[1]}")
+                    f"[target columns]={inp[1]} "
+                    f"[debug_mode]={debug_mode}")
         return self.__qmpc_server.execute_computation(
             ComputationMethod.Value("COMPUTATION_METHOD_CORREL"),
-            join_order, inp)
+            data_ids, inp, debug_mode=debug_mode)
 
-    def meshcode(self, join_order: Tuple[List[str], List[int], List[int]],
-                 src: List) -> Dict:
+    def meshcode(self, data_ids: List[str], src: List,
+                 *, debug_mode: bool = False) -> Dict:
         logger.info("meshcode request. "
-                    f"[data_id list]={join_order[0]} "
-                    f"[join method]={join_order[1]} "
-                    f"[matching ID columns]={join_order[2]} "
-                    f"[src columns]={src}")
+                    f"[data_id list]={data_ids} "
+                    f"[src columns]={src} "
+                    f"[debug_mode]={debug_mode}")
         return self.__qmpc_server.execute_computation(
             ComputationMethod.Value("COMPUTATION_METHOD_MESH_CODE"),
-            join_order, (src, []))
+            data_ids, (src, []), debug_mode=debug_mode)
 
-    def get_join_table(self,
-                       join_order: Tuple[List[str], List[int], List[int]]) \
-            -> Dict:
+    def get_join_table(self, data_ids: List[str],
+                       *, debug_mode: bool = False) -> Dict:
         logger.info("get_join_table request. "
-                    f"[data_id list]={join_order[0]} "
-                    f"[join method]={join_order[1]} "
-                    f"[matching ID columns]={join_order[2]}")
+                    f"[data_id list]={data_ids} "
+                    f"[debug_mode]={debug_mode}")
         return self.__qmpc_server.execute_computation(
             ComputationMethod.Value("COMPUTATION_METHOD_JOIN_TABLE"),
-            join_order, (join_order[2], []))
+            data_ids, ([], []), debug_mode=debug_mode)
 
     def get_computation_result(self, job_uuid: str,
                                path: Optional[str] = None) -> Dict:
         logger.info("get_computation_result request. "
                     f"[job_uuid]={job_uuid} "
                     f"[path]={path}")
         return self.__qmpc_server.get_computation_result(job_uuid, path)
 
-    def get_data_list(self) \
-            -> Dict:
+    def get_data_list(self) -> Dict:
         logger.info("get_data_list request.")
         return self.__qmpc_server.get_data_list()
 
     def demo_sharize(self, secrets: List) -> Dict:
         logger.info("demo_sharize request. "
                     f"[secrets size]={len(secrets)}x{len(secrets[0])}")
         share = Share.sharize(secrets, self.__party_size)
```

### Comparing `quickmpc-0.3.9/quickmpc/qmpc_server.py` & `quickmpc-0.4.0/quickmpc/qmpc_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,29 +73,14 @@
         else:
             logger.error(f'仕様を満たさない形式のendpointが渡された: {endpoint}')
             raise ArgumentError(
                 "endpointsにサポートされてないプロトコルが指定されています．http/httpsのいずれかを指定してください．")
 
         return channel
 
-    @staticmethod
-    def _argument_check(join_order: Tuple[List, List, List]):
-        if len(join_order[0]) - 1 != len(join_order[1]):
-            logger.error(
-                'the size of join must be one less than the size of dataIds')
-            return False
-        if len(join_order[0]) != len(join_order[2]):
-            logger.error('the size of index must match the size of dataIds')
-            return False
-        # TODO joinをenumにする
-        if not all([0 <= join <= 2 for join in join_order[1]]):
-            logger.error('join value must be in the range of 0 to 2')
-            return False
-        return True
-
     def __retry(self, f: Callable, *request: Any) -> Any:
         for ch in self.__client_channels:
             # channelの接続チェック
             is_channel_ready = False
             for _ in range(self.retry_num):
                 try:
                     grpc.channel_ready_future(ch).result(self.retry_wait_time)
@@ -273,24 +258,21 @@
         with ThreadPoolExecutor() as executor:
             futures = [executor.submit(self.__retry, stub.DeleteShares, req)
                        for stub in self.__client_stubs]
         is_ok, _ = QMPCServer.__futures_result(futures)
         return {"is_ok": is_ok}
 
     def execute_computation(self, method_id: int,
-                            join_order: Tuple[List, List, List],
-                            inp: Tuple[List, List]) -> Dict:
-        if not self._argument_check(join_order):
-            raise ArgumentError("引数が正しくありません．")
-
+                            data_ids: List[str],
+                            inp: Tuple[List, List],
+                            *, debug_mode: bool = False) -> Dict:
         """ 計算リクエストを送信 """
         join_order_req = JoinOrder(
-            dataIds=join_order[0],
-            join=join_order[1],
-            index=join_order[2])
+            data_ids=data_ids,
+            debug_mode=debug_mode)
         input_req = Input(
             src=inp[0],
             target=inp[1])
         req = ExecuteComputationRequest(
             method_id=method_id,
             token=self.token,
             table=join_order_req,
```

### Comparing `quickmpc-0.3.9/quickmpc/share.py` & `quickmpc-0.4.0/quickmpc/share.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/quickmpc/utils/make_pieces.py` & `quickmpc-0.4.0/quickmpc/utils/make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/quickmpc/utils/overload_tools.py` & `quickmpc-0.4.0/quickmpc/utils/overload_tools.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/quickmpc/utils/parse_csv.py` & `quickmpc-0.4.0/quickmpc/utils/parse_csv.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/quickmpc/utils/random.py` & `quickmpc-0.4.0/quickmpc/utils/random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/quickmpc/utils/restore.py` & `quickmpc-0.4.0/quickmpc/utils/restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/quickmpc.egg-info/SOURCES.txt` & `quickmpc-0.4.0/quickmpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/certificates/server1.key` & `quickmpc-0.4.0/tests/unit_tests/certificates/server1.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/certificates/server1.pem` & `quickmpc-0.4.0/tests/unit_tests/certificates/server1.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/certificates/server2.key` & `quickmpc-0.4.0/tests/unit_tests/certificates/server2.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/certificates/server2.pem` & `quickmpc-0.4.0/tests/unit_tests/certificates/server2.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/certificates/server3.key` & `quickmpc-0.4.0/tests/unit_tests/certificates/server3.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/certificates/server3.pem` & `quickmpc-0.4.0/tests/unit_tests/certificates/server3.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/conftest.py` & `quickmpc-0.4.0/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/local_server.py` & `quickmpc-0.4.0/tests/unit_tests/local_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
             rich_status = status_pb2.Status(
                 code=code_pb2.INVALID_ARGUMENT,
                 details=[detail]
             )
             context.abort_with_status(rpc_status.to_status(rich_status))
             return libc_to_manage_pb2.ExecuteComputationResponse()
 
-        if len(request.table.dataIds) > 0 \
-                and request.table.dataIds[0] == "UnregisteredDataId":
+        if len(request.table.data_ids) > 0 \
+                and request.table.data_ids[0] == "UnregisteredDataId":
             # QMPCServerError
             # MC で Internal Server Error が発生している場合を再現
             context.set_code(grpc.StatusCode.UNKNOWN)
             return libc_to_manage_pb2.ExecuteComputationResponse()
 
         res = libc_to_manage_pb2.ExecuteComputationResponse(
             job_uuid="jobjobjob"
```

### Comparing `quickmpc-0.3.9/tests/unit_tests/test_files/edge_data.csv` & `quickmpc-0.4.0/tests/unit_tests/test_files/edge_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/test_files/string_data.csv` & `quickmpc-0.4.0/tests/unit_tests/test_files/string_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/test_make_pieces.py` & `quickmpc-0.4.0/tests/unit_tests/test_make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/test_over_load.py` & `quickmpc-0.4.0/tests/unit_tests/test_over_load.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/test_parse.py` & `quickmpc-0.4.0/tests/unit_tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/test_qmpc.py` & `quickmpc-0.4.0/tests/unit_tests/test_qmpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,17 @@
                      matching_column=1,
                      piece_size=1_000_000):
     return (secrets, schema, matching_column, piece_size)
 
 
 def execute_computation_param(method_id=1,
                               data_ids=["data_id1", "data_id2"],
-                              join=[1],
-                              index=[1, 1],
                               src=[0],
                               target=[1]):
-    return (method_id, (data_ids, join, index), (src, target))
+    return (method_id, data_ids, (src, target))
 
 
 class TestQMPC:
     qmpc: QMPCServer = QMPCServer(
         ["http://localhost:50001",
          "http://localhost:50002",
          "http://localhost:50003"],
@@ -91,25 +89,14 @@
                                  run_server1, run_server2, run_server3):
         """ serverに計算リクエストを送れるかのTest"""
         response: Dict[str, Any] = self.qmpc.execute_computation(*params)
         assert (response["is_ok"])
 
     @pytest.mark.parametrize(
         ("params", "expected_exception"), [
-            # data_idsの要素数-1とjoinの要素数が一致していない
-            (execute_computation_param(data_ids=["id1", "id2"], join=[1, 1]),
-             ArgumentError),
-            # data_idsの要素数とindexの要素数が一致していない
-            (execute_computation_param(data_ids=["id1", "id2"], index=[1]),
-             ArgumentError),
-            # joinの値が範囲外
-            (execute_computation_param(join=[-1]),
-             ArgumentError),
-            (execute_computation_param(join=[3]),
-             ArgumentError),
             # QMPCJobErrorとして例外がthrowされるか
             (execute_computation_param(src=[1000000000]),
              QMPCJobError),
             # QMPCServerErrorとして例外がthrowされるか
             (execute_computation_param(data_ids=["UnregisteredDataId", "id2"]),
              QMPCServerError),
         ]
```

### Comparing `quickmpc-0.3.9/tests/unit_tests/test_random.py` & `quickmpc-0.4.0/tests/unit_tests/test_random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/test_restore.py` & `quickmpc-0.4.0/tests/unit_tests/test_restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/test_share_recons.py` & `quickmpc-0.4.0/tests/unit_tests/test_share_recons.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.9/tests/unit_tests/test_share_sharize.py` & `quickmpc-0.4.0/tests/unit_tests/test_share_sharize.py`

 * *Files identical despite different names*

