# Comparing `tmp/uciparse-0.1.8.tar.gz` & `tmp/uciparse-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uciparse-0.1.8.tar", last modified: Mon Jan 18 20:11:37 2021, max compression
+gzip compressed data, was "uciparse-0.1.9.tar", last modified: Sun Feb  7 18:30:00 2021, max compression
```

## Comparing `uciparse-0.1.8.tar` & `uciparse-0.1.9.tar`

### file list

```diff
@@ -1,74 +1,75 @@
--rw-r--r--   0        0        0     1725 2021-01-18 20:11:31.752115 uciparse-0.1.8/Changelog
--rw-r--r--   0        0        0    11324 2021-01-17 02:17:09.724540 uciparse-0.1.8/LICENSE
--rw-r--r--   0        0        0     4334 2021-01-17 17:20:28.718858 uciparse-0.1.8/PyPI.md
--rw-r--r--   0        0        0     4533 2021-01-18 20:10:05.048096 uciparse-0.1.8/README.md
--rw-r--r--   0        0        0       22 2021-01-17 02:17:09.728540 uciparse-0.1.8/docs/.gitignore
--rw-r--r--   0        0        0     6814 2021-01-17 02:17:09.728540 uciparse-0.1.8/docs/Makefile
--rw-r--r--   0        0        0      120 2021-01-17 02:17:09.728540 uciparse-0.1.8/docs/README.md
--rw-r--r--   0        0        0      130 2021-01-17 02:17:09.728540 uciparse-0.1.8/docs/_static/custom.css
--rw-r--r--   0        0        0     1861 2021-01-17 02:17:09.728540 uciparse-0.1.8/docs/_themes/LICENSE
--rw-r--r--   0        0        0     3905 2021-01-17 02:17:09.728540 uciparse-0.1.8/docs/_themes/flask_theme_support.py
--rw-r--r--   0        0        0    12721 2021-01-17 17:20:28.722859 uciparse-0.1.8/docs/conf.py
--rw-r--r--   0        0        0     4693 2021-01-17 17:20:28.722859 uciparse-0.1.8/docs/index.rst
--rw-r--r--   0        0        0     6709 2021-01-17 02:17:09.728540 uciparse-0.1.8/docs/make.bat
--rw-r--r--   0        0        0     7344 2021-01-18 20:10:09.632097 uciparse-0.1.8/docs/requirements.txt
--rw-r--r--   0        0        0     1456 2021-01-18 20:11:31.748115 uciparse-0.1.8/pyproject.toml
--rwxr-xr-x   0        0        0      404 2021-01-18 15:35:54.136410 uciparse-0.1.8/scripts/install
--rwxr-xr-x   0        0        0       61 2021-01-17 02:17:09.732540 uciparse-0.1.8/scripts/ucidiff
--rwxr-xr-x   0        0        0       63 2021-01-17 02:17:09.732540 uciparse-0.1.8/scripts/uciparse
--rw-r--r--   0        0        0       29 2021-01-17 02:17:09.732540 uciparse-0.1.8/src/uciparse/__init__.py
--rw-r--r--   0        0        0     1869 2021-01-17 02:17:09.732540 uciparse-0.1.8/src/uciparse/cli.py
--rw-r--r--   0        0        0       68 2021-01-17 02:17:09.732540 uciparse-0.1.8/src/uciparse/py.typed
--rw-r--r--   0        0        0    17066 2021-01-17 02:17:09.732540 uciparse-0.1.8/src/uciparse/uci.py
--rw-r--r--   0        0        0       29 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0       14 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/invalid/config-empty
--rw-r--r--   0        0        0       23 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/invalid/config-quotes1
--rw-r--r--   0        0        0       22 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/invalid/config-quotes2
--rw-r--r--   0        0        0       18 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/invalid/list-empty
--rw-r--r--   0        0        0       27 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/invalid/list-quotes1
--rw-r--r--   0        0        0       28 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/invalid/list-quotes2
--rw-r--r--   0        0        0       30 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/invalid/option-empty
--rw-r--r--   0        0        0       37 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/invalid/option-quotes1
--rw-r--r--   0        0        0       38 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/invalid/option-quotes2
--rw-r--r--   0        0        0       10 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/invalid/package-empty
--rw-r--r--   0        0        0       17 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/invalid/package-quotes
--rw-r--r--   0        0        0       22 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/invalid/unknown-line
--rw-r--r--   0        0        0      290 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/normalized/comments
--rw-r--r--   0        0        0       21 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/normalized/config-only
--rw-r--r--   0        0        0      158 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/normalized/double-quote
--rw-r--r--   0        0        0       23 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/normalized/list-empty-value
--rw-r--r--   0        0        0       28 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/normalized/list-only
--rw-r--r--   0        0        0      138 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/normalized/no-config-name
--rw-r--r--   0        0        0      143 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/normalized/no-quote
--rw-r--r--   0        0        0       21 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/normalized/option-empty-value
--rw-r--r--   0        0        0       26 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/normalized/option-only
--rw-r--r--   0        0        0       16 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/normalized/package-only
--rw-r--r--   0        0        0      158 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/normalized/single-quote
--rw-r--r--   0        0        0      321 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/original/comments
--rw-r--r--   0        0        0       19 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/original/config-only
--rw-r--r--   0        0        0      211 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/original/double-quote
--rw-r--r--   0        0        0       23 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/original/list-empty-value
--rw-r--r--   0        0        0       26 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/original/list-only
--rw-r--r--   0        0        0      170 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/original/no-config-name
--rw-r--r--   0        0        0      174 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/original/no-quote
--rw-r--r--   0        0        0       31 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/original/option-empty-value
--rw-r--r--   0        0        0       34 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/original/option-only
--rw-r--r--   0        0        0       15 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/original/package-only
--rw-r--r--   0        0        0      211 2021-01-17 02:17:09.732540 uciparse-0.1.8/tests/fixtures/test_uci/original/single-quote
--rw-r--r--   0        0        0      117 2021-01-17 02:17:09.736539 uciparse-0.1.8/tests/fixtures/test_uci/real/README.md
--rw-r--r--   0        0        0     2329 2021-01-17 02:17:09.736539 uciparse-0.1.8/tests/fixtures/test_uci/real/dhcp
--rw-r--r--   0        0        0       86 2021-01-17 02:17:09.736539 uciparse-0.1.8/tests/fixtures/test_uci/real/dropbear
--rw-r--r--   0        0        0     1728 2021-01-17 02:17:09.736539 uciparse-0.1.8/tests/fixtures/test_uci/real/firewall
--rw-r--r--   0        0        0      992 2021-01-17 02:17:09.736539 uciparse-0.1.8/tests/fixtures/test_uci/real/luci
--rw-r--r--   0        0        0      992 2021-01-17 02:17:09.736539 uciparse-0.1.8/tests/fixtures/test_uci/real/network
--rw-r--r--   0        0        0      121 2021-01-17 02:17:09.736539 uciparse-0.1.8/tests/fixtures/test_uci/real/p910nd
--rw-r--r--   0        0        0      160 2021-01-17 02:17:09.736539 uciparse-0.1.8/tests/fixtures/test_uci/real/rpcd
--rw-r--r--   0        0        0     1597 2021-01-17 02:17:09.736539 uciparse-0.1.8/tests/fixtures/test_uci/real/system
--rw-r--r--   0        0        0        0 2021-01-17 02:17:09.736539 uciparse-0.1.8/tests/fixtures/test_uci/real/ubootenv
--rw-r--r--   0        0        0      892 2021-01-17 02:17:09.736539 uciparse-0.1.8/tests/fixtures/test_uci/real/ucitrack
--rw-r--r--   0        0        0     4140 2021-01-17 02:17:09.736539 uciparse-0.1.8/tests/fixtures/test_uci/real/uhttpd
--rw-r--r--   0        0        0     1615 2021-01-17 02:17:09.736539 uciparse-0.1.8/tests/fixtures/test_uci/real/wireless
--rw-r--r--   0        0        0     4043 2021-01-17 02:17:09.736539 uciparse-0.1.8/tests/test_cli.py
--rw-r--r--   0        0        0    11811 2021-01-17 02:17:09.736539 uciparse-0.1.8/tests/test_uci.py
--rw-r--r--   0        0        0     5239 2021-01-18 20:11:37.093987 uciparse-0.1.8/setup.py
--rw-r--r--   0        0        0     5122 2021-01-18 20:11:37.094499 uciparse-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1881 2021-02-07 18:29:46.609739 uciparse-0.1.9/Changelog
+-rw-r--r--   0        0        0       22 2021-01-17 02:13:27.820753 uciparse-0.1.9/docs/.gitignore
+-rw-r--r--   0        0        0      142 2021-02-07 17:27:55.121641 uciparse-0.1.9/docs/.sphinxignore
+-rw-r--r--   0        0        0      130 2021-01-17 02:13:27.820753 uciparse-0.1.9/docs/_static/custom.css
+-rw-r--r--   0        0        0     3905 2021-01-17 02:13:27.821760 uciparse-0.1.9/docs/_themes/flask_theme_support.py
+-rw-r--r--   0        0        0     1861 2021-01-17 02:13:27.821760 uciparse-0.1.9/docs/_themes/LICENSE
+-rw-r--r--   0        0        0    12721 2021-01-17 16:25:58.222791 uciparse-0.1.9/docs/conf.py
+-rw-r--r--   0        0        0     4693 2021-01-17 16:27:10.748530 uciparse-0.1.9/docs/index.rst
+-rwxr-xr-x   0        0        0     6709 2021-01-17 02:13:27.822753 uciparse-0.1.9/docs/make.bat
+-rw-r--r--   0        0        0     6814 2021-01-17 02:13:27.820753 uciparse-0.1.9/docs/Makefile
+-rw-r--r--   0        0        0      120 2021-01-17 02:13:27.820753 uciparse-0.1.9/docs/README.md
+-rw-r--r--   0        0        0     6320 2021-02-07 18:29:17.304435 uciparse-0.1.9/docs/requirements.txt
+-rw-r--r--   0        0        0    11324 2021-01-17 02:13:27.819753 uciparse-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4334 2021-01-17 16:25:51.660940 uciparse-0.1.9/PyPI.md
+-rw-r--r--   0        0        0     1475 2021-02-07 18:29:46.556741 uciparse-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4533 2021-02-03 20:32:28.405151 uciparse-0.1.9/README.md
+-rw-r--r--   0        0        0      404 2021-01-17 21:23:41.979490 uciparse-0.1.9/scripts/install
+-rw-r--r--   0        0        0       61 2021-01-17 02:13:27.824761 uciparse-0.1.9/scripts/ucidiff
+-rw-r--r--   0        0        0       63 2021-01-17 02:13:27.824761 uciparse-0.1.9/scripts/uciparse
+-rw-r--r--   0        0        0       29 2021-01-17 02:13:27.825756 uciparse-0.1.9/src/uciparse/__init__.py
+-rw-r--r--   0        0        0     1869 2021-01-17 02:13:27.825756 uciparse-0.1.9/src/uciparse/cli.py
+-rw-r--r--   0        0        0       68 2021-01-17 02:13:27.825756 uciparse-0.1.9/src/uciparse/py.typed
+-rw-r--r--   0        0        0    17066 2021-01-17 02:13:27.826753 uciparse-0.1.9/src/uciparse/uci.py
+-rw-r--r--   0        0        0       29 2021-01-17 02:13:27.826753 uciparse-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0       14 2021-01-17 02:13:27.827755 uciparse-0.1.9/tests/fixtures/test_uci/invalid/config-empty
+-rw-r--r--   0        0        0       23 2021-01-17 02:13:27.827755 uciparse-0.1.9/tests/fixtures/test_uci/invalid/config-quotes1
+-rw-r--r--   0        0        0       22 2021-01-17 02:13:27.827755 uciparse-0.1.9/tests/fixtures/test_uci/invalid/config-quotes2
+-rw-r--r--   0        0        0       18 2021-01-17 02:13:27.828572 uciparse-0.1.9/tests/fixtures/test_uci/invalid/list-empty
+-rw-r--r--   0        0        0       27 2021-01-17 02:13:27.828572 uciparse-0.1.9/tests/fixtures/test_uci/invalid/list-quotes1
+-rw-r--r--   0        0        0       28 2021-01-17 02:13:27.828572 uciparse-0.1.9/tests/fixtures/test_uci/invalid/list-quotes2
+-rw-r--r--   0        0        0       30 2021-01-17 02:13:27.828572 uciparse-0.1.9/tests/fixtures/test_uci/invalid/option-empty
+-rw-r--r--   0        0        0       37 2021-01-17 02:13:27.829576 uciparse-0.1.9/tests/fixtures/test_uci/invalid/option-quotes1
+-rw-r--r--   0        0        0       38 2021-01-17 02:13:27.829576 uciparse-0.1.9/tests/fixtures/test_uci/invalid/option-quotes2
+-rw-r--r--   0        0        0       10 2021-01-17 02:13:27.829576 uciparse-0.1.9/tests/fixtures/test_uci/invalid/package-empty
+-rw-r--r--   0        0        0       17 2021-01-17 02:13:27.829576 uciparse-0.1.9/tests/fixtures/test_uci/invalid/package-quotes
+-rw-r--r--   0        0        0       22 2021-01-17 02:13:27.829576 uciparse-0.1.9/tests/fixtures/test_uci/invalid/unknown-line
+-rw-r--r--   0        0        0      290 2021-01-17 02:13:27.830577 uciparse-0.1.9/tests/fixtures/test_uci/normalized/comments
+-rw-r--r--   0        0        0       21 2021-01-17 02:13:27.830577 uciparse-0.1.9/tests/fixtures/test_uci/normalized/config-only
+-rw-r--r--   0        0        0      158 2021-01-17 02:13:27.830577 uciparse-0.1.9/tests/fixtures/test_uci/normalized/double-quote
+-rw-r--r--   0        0        0       23 2021-01-17 02:13:27.831702 uciparse-0.1.9/tests/fixtures/test_uci/normalized/list-empty-value
+-rw-r--r--   0        0        0       28 2021-01-17 02:13:27.831702 uciparse-0.1.9/tests/fixtures/test_uci/normalized/list-only
+-rw-r--r--   0        0        0      138 2021-01-17 02:13:27.831702 uciparse-0.1.9/tests/fixtures/test_uci/normalized/no-config-name
+-rw-r--r--   0        0        0      143 2021-01-17 02:13:27.831702 uciparse-0.1.9/tests/fixtures/test_uci/normalized/no-quote
+-rw-r--r--   0        0        0       21 2021-01-17 02:13:27.831702 uciparse-0.1.9/tests/fixtures/test_uci/normalized/option-empty-value
+-rw-r--r--   0        0        0       26 2021-01-17 02:13:27.832706 uciparse-0.1.9/tests/fixtures/test_uci/normalized/option-only
+-rw-r--r--   0        0        0       16 2021-01-17 02:13:27.832706 uciparse-0.1.9/tests/fixtures/test_uci/normalized/package-only
+-rw-r--r--   0        0        0      158 2021-01-17 02:13:27.832706 uciparse-0.1.9/tests/fixtures/test_uci/normalized/single-quote
+-rw-r--r--   0        0        0      321 2021-01-17 02:13:27.832706 uciparse-0.1.9/tests/fixtures/test_uci/original/comments
+-rw-r--r--   0        0        0       19 2021-01-17 02:13:27.833706 uciparse-0.1.9/tests/fixtures/test_uci/original/config-only
+-rw-r--r--   0        0        0      211 2021-01-17 02:13:27.833706 uciparse-0.1.9/tests/fixtures/test_uci/original/double-quote
+-rw-r--r--   0        0        0       23 2021-01-17 02:13:27.833706 uciparse-0.1.9/tests/fixtures/test_uci/original/list-empty-value
+-rw-r--r--   0        0        0       26 2021-01-17 02:13:27.833706 uciparse-0.1.9/tests/fixtures/test_uci/original/list-only
+-rw-r--r--   0        0        0      170 2021-01-17 02:13:27.834706 uciparse-0.1.9/tests/fixtures/test_uci/original/no-config-name
+-rw-r--r--   0        0        0      174 2021-01-17 02:13:27.834706 uciparse-0.1.9/tests/fixtures/test_uci/original/no-quote
+-rw-r--r--   0        0        0       31 2021-01-17 02:13:27.834706 uciparse-0.1.9/tests/fixtures/test_uci/original/option-empty-value
+-rw-r--r--   0        0        0       34 2021-01-17 02:13:27.834706 uciparse-0.1.9/tests/fixtures/test_uci/original/option-only
+-rw-r--r--   0        0        0       15 2021-01-17 02:13:27.835705 uciparse-0.1.9/tests/fixtures/test_uci/original/package-only
+-rw-r--r--   0        0        0      211 2021-01-17 02:13:27.835705 uciparse-0.1.9/tests/fixtures/test_uci/original/single-quote
+-rw-r--r--   0        0        0     2329 2021-01-17 02:13:27.836706 uciparse-0.1.9/tests/fixtures/test_uci/real/dhcp
+-rw-r--r--   0        0        0       86 2021-01-17 02:13:27.836706 uciparse-0.1.9/tests/fixtures/test_uci/real/dropbear
+-rw-r--r--   0        0        0     1728 2021-01-17 02:13:27.836706 uciparse-0.1.9/tests/fixtures/test_uci/real/firewall
+-rw-r--r--   0        0        0      992 2021-01-17 02:13:27.836706 uciparse-0.1.9/tests/fixtures/test_uci/real/luci
+-rw-r--r--   0        0        0      992 2021-01-17 02:13:27.836706 uciparse-0.1.9/tests/fixtures/test_uci/real/network
+-rw-r--r--   0        0        0      121 2021-01-17 02:13:27.837706 uciparse-0.1.9/tests/fixtures/test_uci/real/p910nd
+-rw-r--r--   0        0        0      117 2021-01-17 02:13:27.835705 uciparse-0.1.9/tests/fixtures/test_uci/real/README.md
+-rw-r--r--   0        0        0      160 2021-01-17 02:13:27.837706 uciparse-0.1.9/tests/fixtures/test_uci/real/rpcd
+-rw-r--r--   0        0        0     1597 2021-01-17 02:13:27.837706 uciparse-0.1.9/tests/fixtures/test_uci/real/system
+-rw-r--r--   0        0        0        0 2021-01-17 02:13:27.838706 uciparse-0.1.9/tests/fixtures/test_uci/real/ubootenv
+-rw-r--r--   0        0        0      892 2021-01-17 02:13:27.838706 uciparse-0.1.9/tests/fixtures/test_uci/real/ucitrack
+-rw-r--r--   0        0        0     4140 2021-01-17 02:13:27.838706 uciparse-0.1.9/tests/fixtures/test_uci/real/uhttpd
+-rw-r--r--   0        0        0     1615 2021-01-17 02:13:27.838706 uciparse-0.1.9/tests/fixtures/test_uci/real/wireless
+-rw-r--r--   0        0        0     4043 2021-01-17 02:13:27.839706 uciparse-0.1.9/tests/test_cli.py
+-rw-r--r--   0        0        0    11811 2021-01-17 02:13:27.839706 uciparse-0.1.9/tests/test_uci.py
+-rw-r--r--   0        0        0     5239 2021-02-07 18:30:00.863776 uciparse-0.1.9/setup.py
+-rw-r--r--   0        0        0     5122 2021-02-07 18:30:00.863776 uciparse-0.1.9/PKG-INFO
```

### Comparing `uciparse-0.1.8/Changelog` & `uciparse-0.1.9/Changelog`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Version 0.1.9     07 Feb 2021
+
+	* Update build process to include security scans using Safety.
+	* Make other structural improvements to the build process.
+
 Version 0.1.8     18 Jan 2021
 
 	* Update PyCharm inspection profile.
 	* Add documentation for PyCharm on Linux.
 	* Add release history for v0.1.0 through v0.1.5 into Changelog.
 	* Validate the release process on Linux.
```

### Comparing `uciparse-0.1.8/LICENSE` & `uciparse-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/PyPI.md` & `uciparse-0.1.9/PyPI.md`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/README.md` & `uciparse-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/docs/Makefile` & `uciparse-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/docs/_themes/LICENSE` & `uciparse-0.1.9/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/docs/_themes/flask_theme_support.py` & `uciparse-0.1.9/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/docs/conf.py` & `uciparse-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/docs/index.rst` & `uciparse-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/docs/make.bat` & `uciparse-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/docs/requirements.txt` & `uciparse-0.1.9/docs/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,63 @@
-alabaster==0.7.12; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5"
+alabaster==0.7.12; python_version >= "3.6"
 appdirs==1.4.4; python_version >= "3.6" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version >= "3.6"
-astroid==2.4.2; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5"
+astroid==2.4.2; python_version >= "3.6"
 atomicwrites==1.4.0; python_version >= "3.6" and python_full_version < "3.0.0" and sys_platform == "win32" or sys_platform == "win32" and python_version >= "3.6" and python_full_version >= "3.4.0"
 attrs==20.3.0; python_version >= "3.6" and python_full_version < "3.0.0" or python_full_version >= "3.4.0" and python_version >= "3.6"
-babel==2.9.0; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5"
+babel==2.9.0; python_version >= "3.6" and python_full_version < "3.0.0" or python_full_version >= "3.4.0" and python_version >= "3.6"
 black==20.8b1; python_version >= "3.6"
 certifi==2020.12.5; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version >= "3.5"
 cfgv==3.2.0; python_full_version >= "3.6.1"
 chardet==4.0.0; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version >= "3.5"
 click==7.1.2; python_version >= "3.6" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version >= "3.6"
-colorama==0.4.4; python_version >= "3.6" and python_full_version < "3.0.0" and sys_platform == "win32" and platform_system == "Windows" and (python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5") or sys_platform == "win32" and python_version >= "3.6" and python_full_version >= "3.5.0" and platform_system == "Windows" and (python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5")
-coverage==5.3.1; (python_version >= "2.7" and python_full_version < "3.0.0") or (python_full_version >= "3.5.0" and python_version < "4")
+colorama==0.4.4; python_version >= "3.6" and python_full_version < "3.0.0" and sys_platform == "win32" and platform_system == "Windows" or sys_platform == "win32" and python_version >= "3.6" and python_full_version >= "3.5.0" and platform_system == "Windows"
+coverage==5.4; (python_version >= "2.7" and python_full_version < "3.0.0") or (python_full_version >= "3.5.0" and python_version < "4")
 distlib==0.3.1; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
-docutils==0.16; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5"
+docutils==0.16; python_version >= "3.6" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version >= "3.6"
+dparse==0.5.1; python_version >= "3.5"
 filelock==3.0.12; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
-identify==1.5.12; python_full_version >= "3.6.1"
+identify==1.5.13; python_full_version >= "3.6.1"
 idna==2.10; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version >= "3.5"
-imagesize==1.2.0; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5"
+imagesize==1.2.0; python_version >= "3.6" and python_full_version < "3.0.0" or python_full_version >= "3.4.0" and python_version >= "3.6"
 importlib-metadata==3.4.0; python_version < "3.8" and python_version >= "3.6" and (python_version >= "3.6" and python_full_version < "3.0.0" and python_version < "3.8" or python_full_version >= "3.5.0" and python_version < "3.8" and python_version >= "3.6") and python_full_version >= "3.6.1" and (python_version >= "3.6" and python_full_version < "3.0.0" and python_version < "3.8" or python_full_version >= "3.4.0" and python_version >= "3.6" and python_version < "3.8")
 iniconfig==1.1.1; python_version >= "3.6"
 isort==5.7.0; python_version >= "3.6" and python_version < "4.0"
-jinja2==2.11.2; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5"
+jinja2==2.11.3; python_version >= "3.6" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version >= "3.6"
 lazy-object-proxy==1.4.3; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.4.0" and python_version >= "3.5"
 markupsafe==1.1.1; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version >= "3.5"
 mccabe==0.6.1; python_version >= "3.5"
 mypy-extensions==0.4.3; python_version >= "3.6"
 mypy==0.790; python_version >= "3.5"
 nodeenv==1.5.0; python_full_version >= "3.6.1"
-packaging==20.8; python_version >= "3.6" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.6"
+packaging==20.9; python_version >= "3.6" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version >= "3.6"
 pathspec==0.8.1; python_version >= "3.6" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version >= "3.6"
 pluggy==0.13.1; python_version >= "3.6" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version >= "3.6"
-pre-commit==2.9.3; python_full_version >= "3.6.1"
+pre-commit==2.10.1; python_full_version >= "3.6.1"
 py==1.10.0; python_version >= "3.6" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version >= "3.6"
-pygments==2.7.4; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5"
+pygments==2.7.4; python_version >= "3.6"
 pylint==2.6.0; python_version >= "3.5"
 pyparsing==2.4.7; python_version >= "3.6" and python_full_version < "3.0.0" or python_full_version >= "3.4.0" and python_version >= "3.6"
-pytest==6.2.1; python_version >= "3.6"
-pytz==2020.5; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.4.0" and python_version >= "3.5"
-pyyaml==5.3.1; python_full_version >= "3.6.1"
+pytest==6.2.2; python_version >= "3.6"
+pytz==2021.1; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.4.0" and python_version >= "3.5"
+pyyaml==5.4.1; python_full_version >= "3.6.1" and python_version >= "3.6" and (python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5")
 regex==2020.11.13; python_version >= "3.6"
-requests==2.25.1; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5"
+requests==2.25.1; python_version >= "3.6" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version >= "3.6"
+safety==1.10.3; python_version >= "3.5"
 six==1.15.0; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version >= "3.5"
-snowballstemmer==2.0.0; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5"
-sphinx-autoapi==1.5.1; (python_version >= "2.7" and python_full_version < "3.0.0") or (python_full_version >= "3.6.0")
+snowballstemmer==2.1.0; python_version >= "3.6"
+sphinx-autoapi==1.7.0; python_version >= "3.6"
 sphinx==3.4.3; python_version >= "3.5"
-sphinxcontrib-applehelp==1.0.2; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5"
-sphinxcontrib-devhelp==1.0.2; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5"
-sphinxcontrib-htmlhelp==1.0.3; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5"
-sphinxcontrib-jsmath==1.0.1; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5"
-sphinxcontrib-qthelp==1.0.3; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5"
-sphinxcontrib-serializinghtml==1.1.4; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.6.0" and python_version >= "3.5"
+sphinxcontrib-applehelp==1.0.2; python_version >= "3.6"
+sphinxcontrib-devhelp==1.0.2; python_version >= "3.6"
+sphinxcontrib-htmlhelp==1.0.3; python_version >= "3.6"
+sphinxcontrib-jsmath==1.0.1; python_version >= "3.6"
+sphinxcontrib-qthelp==1.0.3; python_version >= "3.6"
+sphinxcontrib-serializinghtml==1.1.4; python_version >= "3.6"
 toml==0.10.2; (python_version >= "2.6" and python_full_version < "3.0.0") or (python_full_version >= "3.3.0")
-tox==3.21.1; (python_version >= "2.7" and python_full_version < "3.0.0") or (python_full_version >= "3.5.0")
+tox==3.21.4; (python_version >= "2.7" and python_full_version < "3.0.0") or (python_full_version >= "3.5.0")
 typed-ast==1.4.2; implementation_name == "cpython" and python_version < "3.8" and python_version >= "3.6"
 typing-extensions==3.7.4.3; python_version < "3.8" and python_version >= "3.6"
-unidecode==1.1.2; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.6.0"
-urllib3==1.26.2; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version < "4" and python_version >= "3.5"
-virtualenv==20.3.1; python_full_version >= "3.6.1"
+unidecode==1.2.0; python_version >= "3.6" and python_full_version < "3.0.0" or python_full_version >= "3.4.0" and python_version >= "3.6"
+urllib3==1.26.3; python_version >= "3.5" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version < "4" and python_version >= "3.5"
+virtualenv==20.4.2; python_full_version >= "3.6.1"
 wrapt==1.12.1; python_version >= "3.5"
 zipp==3.4.0; python_version < "3.8" and python_version >= "3.6"
```

### Comparing `uciparse-0.1.8/pyproject.toml` & `uciparse-0.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uciparse"
-version = "0.1.8"
+version = "0.1.9"
 description = "Parse and emit OpenWRT uci-format files"
 authors = ["Kenneth J. Pronovici <pronovic@ieee.org>"]
 license = "Apache-2.0"
 readme = "PyPI.md"
 homepage = "https://pypi.org/project/uciparse/"
 include = [ "Changelog", "LICENSE", "README.md", "docs", "tests", "scripts", ]
 packages = [ { include = "uciparse", from = "src" } ]
@@ -33,14 +33,15 @@
 sphinx = "^3.4.3"
 toml = "^0.10.1"
 pre-commit = "^2.4.0"
 black = "^20.8b1"
 mypy = "^0.790"
 isort = "^5.0.0"
 sphinx-autoapi = "^1.3.0"
+safety = "^1.10.3"
 
 [tool.black]
 line-length = 132
 target-version = ['py37', 'py38']
 include = '(src\/scripts\/.*$|\.pyi?$)'
 exclude = '''
 /(
```

### Comparing `uciparse-0.1.8/src/uciparse/cli.py` & `uciparse-0.1.9/src/uciparse/cli.py`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/src/uciparse/uci.py` & `uciparse-0.1.9/src/uciparse/uci.py`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/tests/fixtures/test_uci/real/dhcp` & `uciparse-0.1.9/tests/fixtures/test_uci/real/dhcp`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/tests/fixtures/test_uci/real/firewall` & `uciparse-0.1.9/tests/fixtures/test_uci/real/firewall`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/tests/fixtures/test_uci/real/luci` & `uciparse-0.1.9/tests/fixtures/test_uci/real/luci`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/tests/fixtures/test_uci/real/network` & `uciparse-0.1.9/tests/fixtures/test_uci/real/network`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/tests/fixtures/test_uci/real/system` & `uciparse-0.1.9/tests/fixtures/test_uci/real/system`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/tests/fixtures/test_uci/real/ucitrack` & `uciparse-0.1.9/tests/fixtures/test_uci/real/ucitrack`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/tests/fixtures/test_uci/real/uhttpd` & `uciparse-0.1.9/tests/fixtures/test_uci/real/uhttpd`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/tests/fixtures/test_uci/real/wireless` & `uciparse-0.1.9/tests/fixtures/test_uci/real/wireless`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/tests/test_cli.py` & `uciparse-0.1.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/tests/test_uci.py` & `uciparse-0.1.9/tests/test_uci.py`

 * *Files identical despite different names*

### Comparing `uciparse-0.1.8/setup.py` & `uciparse-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 entry_points = \
 {'console_scripts': ['ucidiff = uciparse.cli:diff',
                      'uciparse = uciparse.cli:parse']}
 
 setup_kwargs = {
     'name': 'uciparse',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Parse and emit OpenWRT uci-format files',
     'long_description': "# UCI Parse Library\n\n[![pypi](https://img.shields.io/pypi/v/uciparse.svg)](https://pypi.org/project/uciparse/)\n[![license](https://img.shields.io/pypi/l/uciparse.svg)](https://github.com/pronovic/uci-parse/blob/master/LICENSE)\n[![wheel](https://img.shields.io/pypi/wheel/uciparse.svg)](https://pypi.org/project/uciparse/)\n[![python](https://img.shields.io/pypi/pyversions/uciparse.svg)](https://pypi.org/project/uciparse/)\n[![Test Suite](https://github.com/pronovic/uci-parse/workflows/Test%20Suite/badge.svg)](https://github.com/pronovic/uci-parse/actions?query=workflow%3A%22Test+Suite%22)\n[![docs](https://readthedocs.org/projects/uci-parse/badge/?version=stable&style=flat)](https://uci-parse.readthedocs.io/en/stable/)\n\nPython 3 library and command line tools to parse, diff, and normalize OpenWRT\n[UCI](https://openwrt.org/docs/guide-user/base-system/uci) configuration files.\n\nThese tools were written to ease OpenWRT upgrades, making it easier to see the\ndifferences between two config files.  As of this writing (mid-2020), OpenWRT\nupgrades often don't normalize upgraded config files in the same way from\nversion to version.  For instance, the new version from `opkg upgrade` (saved\noff with a `-opkg` filename) might use single quotes on all lines, while the\noriginal version on disk might not use quotes at all.  This makes it very\ndifficult understand the often-minimal differences between an upgraded file and\nthe original file.\n\n## Installing the Package\n\nInstalling this package on your OpenWRT router is not as simple as it could be.\nA lot of routers do not have enough space available to install a full version\nof Python including `pip` or `setuptools`.  If yours does have lots of space,\nit's as simple as this:\n\n```\n$ opkg update\n$ opkg install python3-pip\n$ pip3 install uciparse\n```\n\nIf not, it gets a little ugly.  First, install `wget` with support for HTTPS:\n\n```\n$ opkg update\n$ opkg install wget libustream-openssl20150806 ca-bundle ca-certificates\n```\n\nThen, go to [PyPI](https://pypi.org/project/uciparse/#files) and copy the\nURL for the source package `.tar.gz` file.  Retrieve the source package \nwith `wget` and then manually extract it:\n\n```\n$ wget https://files.pythonhosted.org/.../uciparse-0.1.2.tar.gz\n$ tar zxvf uciparse-0.1.2.tar.gz\n$ cd uciparse-0.1.2\n```\n\nFinally, run the custom install script provided with the source package:\n\n```\n$ sh ./scripts/install\n```\n\nThis installs the OpenWRT `python3-light` package, then copies the Python\npackages into the right `site-packages` directory and the `uciparse` and\n`ucidiff` scripts to `/usr/bin`.\n\n## Using the Tools\n\nOnce you have installed the package as described above, the `uciparse` and\n`ucidiff` tools will be available in your path.  \n\n### ucidiff\n\nThe `ucidiff` tool is probably the tool you'll use most often when updating\nyour router.  It reads two UCI configuration files from disk, normalizes both in\nmemory (without making changes on disk), and then compares them.  The result is\na unified diff, like `diff -Naur`.  This gives you a way to understand the real\ndifferences between two files without ever having to change anything on disk.\n\n```\n$ ucidiff --help\nusage: ucidiff [-h] a b\n\nDiff two UCI configuration files.\n\npositional arguments:\n  a           Path to the first UCI file to compare\n  b           Path to the second UCI file to compare\n\noptional arguments:\n  -h, --help  show this help message and exit\n\nThe comparison is equivalent to a 'diff -Naur' between the normalized versions\nof the files. If either file can't be parsed, then an error will be returned\nand no diff will be shown.\n```\n\n### uciparse\n\nIf you would prefer to clean up and normalize your configuration files on disk,\nthen you can use the `uciparse` tool.  It reads a UCI config file from disk or\nfrom `stdin`, parses it, and prints normalized output to `stdout`.  \n\n```\n$ uciparse --help\nusage: uciparse [-h] uci\n\nParse and normalize a UCI configuration file.\n\npositional arguments:\n  uci         Path to the UCI file to normalize, or '-' for stdin\n\noptional arguments:\n  -h, --help  show this help message and exit\n\nResults will be printed to stdout. If the file can't be parsed then an error\nwill be returned and no output will be generated.\n```\n\nBefore using ``uciparse``, you should make a backup of any config file that you\nare going to normalized.\n",
     'author': 'Kenneth J. Pronovici',
     'author_email': 'pronovic@ieee.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://pypi.org/project/uciparse/',
```

### Comparing `uciparse-0.1.8/PKG-INFO` & `uciparse-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uciparse
-Version: 0.1.8
+Version: 0.1.9
 Summary: Parse and emit OpenWRT uci-format files
 Home-page: https://pypi.org/project/uciparse/
 License: Apache-2.0
 Author: Kenneth J. Pronovici
 Author-email: pronovic@ieee.org
 Requires-Python: >=3.7,<4
 Classifier: Environment :: Console
```

