# Comparing `tmp/proxystore-0.5.0.tar.gz` & `tmp/proxystore-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxystore-0.5.0.tar", last modified: Fri May 12 22:52:30 2023, max compression
+gzip compressed data, was "proxystore-0.5.1.tar", last modified: Thu Jun  8 01:01:09 2023, max compression
```

## Comparing `proxystore-0.5.0.tar` & `proxystore-0.5.1.tar`

### file list

```diff
@@ -1,232 +1,235 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.652859 proxystore-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.608859 proxystore-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.608859 proxystore-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-12 22:52:19.000000 proxystore-0.5.0/.github/ISSUE_TEMPLATE/01_bug.yml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-12 22:52:19.000000 proxystore-0.5.0/.github/ISSUE_TEMPLATE/02_feature.yml
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-12 22:52:19.000000 proxystore-0.5.0/.github/ISSUE_TEMPLATE/03_docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-12 22:52:19.000000 proxystore-0.5.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-12 22:52:19.000000 proxystore-0.5.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-12 22:52:19.000000 proxystore-0.5.0/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-12 22:52:19.000000 proxystore-0.5.0/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.608859 proxystore-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-12 22:52:19.000000 proxystore-0.5.0/.github/workflows/cache.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-12 22:52:19.000000 proxystore-0.5.0/.github/workflows/check-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-12 22:52:19.000000 proxystore-0.5.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-12 22:52:19.000000 proxystore-0.5.0/.github/workflows/integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-12 22:52:19.000000 proxystore-0.5.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-12 22:52:19.000000 proxystore-0.5.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-12 22:52:19.000000 proxystore-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-12 22:52:19.000000 proxystore-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-12 22:52:19.000000 proxystore-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-05-12 22:52:30.652859 proxystore-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-12 22:52:19.000000 proxystore-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.612859 proxystore-0.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.612859 proxystore-0.5.0/docs/_overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/_overrides/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.604859 proxystore-0.5.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.604859 proxystore-0.5.0/docs/_templates/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.612859 proxystore-0.5.0/docs/_templates/python/material/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.612859 proxystore-0.5.0/docs/_templates/python/material/docstring/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/_templates/python/material/docstring/admonition.html
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/_templates/python/material/function.html
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/_templates/python/material/module.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.612859 proxystore-0.5.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/api/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/api/legacy-docs.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.612859 proxystore-0.5.0/docs/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/concepts/connector.md
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/concepts/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/concepts/proxy.md
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/concepts/store.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.612859 proxystore-0.5.0/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/contributing/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/contributing/issues-pull-requests.md
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/contributing/releases.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/contributing/style-guide.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.612859 proxystore-0.5.0/docs/css/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/generate_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/get-started.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.616860 proxystore-0.5.0/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/guides/endpoints-debugging.md
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/guides/endpoints.md
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/guides/globus-compute.md
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/guides/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/guides/performance.md
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/known-issues.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.616860 proxystore-0.5.0/docs/static/
--rw-r--r--   0 runner    (1001) docker     (123)   134472 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/static/endpoint-overview.svg
--rw-r--r--   0 runner    (1001) docker     (123)   149176 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/static/endpoint-peering.svg
--rw-r--r--   0 runner    (1001) docker     (123)    46990 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)    45464 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/static/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    31401 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/static/logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    31236 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/static/logo-light.png
--rw-r--r--   0 runner    (1001) docker     (123)   106893 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/static/proxystore-overview.svg
--rw-r--r--   0 runner    (1001) docker     (123)   106939 2023-05-12 22:52:19.000000 proxystore-0.5.0/docs/static/proxystore-schematic.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.620859 proxystore-0.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-12 22:52:19.000000 proxystore-0.5.0/examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-12 22:52:19.000000 proxystore-0.5.0/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.620859 proxystore-0.5.0/examples/globus-compute/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-12 22:52:19.000000 proxystore-0.5.0/examples/globus-compute/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-12 22:52:19.000000 proxystore-0.5.0/examples/globus-compute/mapreduce_globus_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-12 22:52:19.000000 proxystore-0.5.0/examples/globus-compute/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.620859 proxystore-0.5.0/examples/parsl/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-12 22:52:19.000000 proxystore-0.5.0/examples/parsl/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-12 22:52:19.000000 proxystore-0.5.0/examples/parsl/mapreduce_parsl.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-12 22:52:19.000000 proxystore-0.5.0/examples/parsl/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-12 22:52:19.000000 proxystore-0.5.0/examples/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-12 22:52:19.000000 proxystore-0.5.0/examples/store_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-12 22:52:19.000000 proxystore-0.5.0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.620859 proxystore-0.5.0/proxystore/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.624859 proxystore-0.5.0/proxystore/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/connectors/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.628859 proxystore-0.5.0/proxystore/connectors/dim/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/connectors/dim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/connectors/dim/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18851 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/connectors/dim/margo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/connectors/dim/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    18547 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/connectors/dim/ucx.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/connectors/dim/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/connectors/dim/zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/connectors/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/connectors/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    22457 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/connectors/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/connectors/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/connectors/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/connectors/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.628859 proxystore-0.5.0/proxystore/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/endpoint/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/endpoint/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/endpoint/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/endpoint/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/endpoint/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17315 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/endpoint/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/endpoint/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/endpoint/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/endpoint/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/endpoint/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/globus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.632859 proxystore-0.5.0/proxystore/p2p/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/p2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/p2p/chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15126 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/p2p/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/p2p/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/p2p/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/p2p/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/p2p/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/p2p/relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/p2p/relay_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/p2p/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.632859 proxystore-0.5.0/proxystore/store/
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23797 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/store/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/store/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/store/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/store/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/store/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/store/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/store/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/store/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/store/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/store/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-12 22:52:19.000000 proxystore-0.5.0/proxystore/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.624859 proxystore-0.5.0/proxystore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-05-12 22:52:30.000000 proxystore-0.5.0/proxystore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-12 22:52:30.000000 proxystore-0.5.0/proxystore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 22:52:30.000000 proxystore-0.5.0/proxystore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 22:52:30.000000 proxystore-0.5.0/proxystore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-12 22:52:30.000000 proxystore-0.5.0/proxystore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-12 22:52:30.000000 proxystore-0.5.0/proxystore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-12 22:52:19.000000 proxystore-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 22:52:30.652859 proxystore-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.636860 proxystore-0.5.0/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.636860 proxystore-0.5.0/testing/mocked/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/mocked/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/mocked/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/mocked/pymargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/mocked/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/mocked/ucx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/mocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/relay_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.636860 proxystore-0.5.0/testing/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/scripts/peer_connection_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/scripts/peer_endpoint_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/scripts/peer_manager_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-12 22:52:19.000000 proxystore-0.5.0/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.640859 proxystore-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.640859 proxystore-0.5.0/tests/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/connectors/connector_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.644859 proxystore-0.5.0/tests/connectors/dim/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/connectors/dim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/connectors/dim/margo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/connectors/dim/ucx_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/connectors/dim/zmq_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/connectors/endpoint_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/connectors/file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/connectors/globus_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/connectors/local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/connectors/multi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/connectors/redis_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.644859 proxystore-0.5.0/tests/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/endpoint/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/endpoint/client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/endpoint/commands_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/endpoint/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/endpoint/endpoint_peering_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/endpoint/endpoint_solo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/endpoint/serve_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/endpoint/storage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/globus_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.644859 proxystore-0.5.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/integration/endpoints_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.648859 proxystore-0.5.0/tests/p2p/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/p2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/p2p/chunks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/p2p/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/p2p/counter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/p2p/manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/p2p/messages_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/p2p/relay_cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/p2p/relay_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/p2p/relay_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/p2p/task_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/serialization_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:52:30.652859 proxystore-0.5.0/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/store/cache_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/store/init_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/store/metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/store/store_basics_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/store/store_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/store/store_proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/store/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/timer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-12 22:52:19.000000 proxystore-0.5.0/tests/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-12 22:52:19.000000 proxystore-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.569710 proxystore-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/ISSUE_TEMPLATE/01_bug.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/ISSUE_TEMPLATE/02_feature.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/ISSUE_TEMPLATE/03_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/workflows/cache.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/workflows/check-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/workflows/integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-08 01:01:00.000000 proxystore-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-08 01:01:00.000000 proxystore-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-08 01:01:00.000000 proxystore-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-08 01:01:09.569710 proxystore-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-08 01:01:00.000000 proxystore-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/docs/_overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/_overrides/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.545709 proxystore-0.5.1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.545709 proxystore-0.5.1/docs/_templates/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/docs/_templates/python/material/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/docs/_templates/python/material/docstring/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/_templates/python/material/docstring/admonition.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/_templates/python/material/function.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/_templates/python/material/module.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/api/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/api/legacy-docs.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.553709 proxystore-0.5.1/docs/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/concepts/connector.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/concepts/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/concepts/proxy.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/concepts/store.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.553709 proxystore-0.5.1/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/contributing/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/contributing/issues-pull-requests.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/contributing/releases.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/contributing/style-guide.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.553709 proxystore-0.5.1/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/generate_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/get-started.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.553709 proxystore-0.5.1/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/guides/endpoints-debugging.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/guides/endpoints.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/guides/globus-compute.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/guides/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/guides/performance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/known-issues.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.553709 proxystore-0.5.1/docs/publications/
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/publications/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.553709 proxystore-0.5.1/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   134472 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/endpoint-overview.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   149176 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/endpoint-peering.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46990 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45464 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31401 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31236 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/logo-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)   106893 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/proxystore-overview.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   106939 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/proxystore-schematic.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.553709 proxystore-0.5.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.557709 proxystore-0.5.1/examples/globus-compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/globus-compute/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/globus-compute/mapreduce_globus_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/globus-compute/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.557709 proxystore-0.5.1/examples/parsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/parsl/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/parsl/mapreduce_parsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/parsl/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/store_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-08 01:01:00.000000 proxystore-0.5.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.557709 proxystore-0.5.1/proxystore/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.557709 proxystore-0.5.1/proxystore/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.557709 proxystore-0.5.1/proxystore/connectors/dim/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/dim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/dim/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19432 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/dim/margo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/dim/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18547 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/dim/ucx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/dim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/dim/zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23197 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.561710 proxystore-0.5.1/proxystore/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17312 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/globus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.561710 proxystore-0.5.1/proxystore/p2p/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/relay_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.561710 proxystore-0.5.1/proxystore/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31043 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.557709 proxystore-0.5.1/proxystore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-08 01:01:09.000000 proxystore-0.5.1/proxystore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-08 01:01:09.000000 proxystore-0.5.1/proxystore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 01:01:09.000000 proxystore-0.5.1/proxystore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-08 01:01:09.000000 proxystore-0.5.1/proxystore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-08 01:01:09.000000 proxystore-0.5.1/proxystore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 01:01:09.000000 proxystore-0.5.1/proxystore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-06-08 01:01:00.000000 proxystore-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 01:01:09.569710 proxystore-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.565709 proxystore-0.5.1/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.565709 proxystore-0.5.1/testing/mocked/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/mocked/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/mocked/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/mocked/pymargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/mocked/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/mocked/ucx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/mocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/relay_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.565709 proxystore-0.5.1/testing/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/scripts/peer_connection_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/scripts/peer_endpoint_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/scripts/peer_manager_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.565709 proxystore-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.565709 proxystore-0.5.1/tests/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/connector_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.565709 proxystore-0.5.1/tests/connectors/dim/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/dim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/dim/margo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/dim/ucx_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/dim/zmq_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/endpoint_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/globus_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/multi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/redis_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.569710 proxystore-0.5.1/tests/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/commands_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/endpoint_peering_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/endpoint_solo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/serve_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/storage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/globus_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.569710 proxystore-0.5.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/integration/endpoints_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.569710 proxystore-0.5.1/tests/p2p/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/chunks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/counter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/messages_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/relay_cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/relay_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/relay_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/task_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/serialization_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.569710 proxystore-0.5.1/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/cache_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/init_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/shims_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/store_basics_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/store_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/store_proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/timer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-08 01:01:00.000000 proxystore-0.5.1/tox.ini
```

### Comparing `proxystore-0.5.0/.github/ISSUE_TEMPLATE/01_bug.yml` & `proxystore-0.5.1/.github/ISSUE_TEMPLATE/01_bug.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/.github/ISSUE_TEMPLATE/02_feature.yml` & `proxystore-0.5.1/.github/ISSUE_TEMPLATE/02_feature.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/.github/pull_request_template.md` & `proxystore-0.5.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/.github/release.yml` & `proxystore-0.5.1/.github/release.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/.github/workflows/cache.yml` & `proxystore-0.5.1/.github/workflows/cache.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/.github/workflows/check-docs.yml` & `proxystore-0.5.1/.github/workflows/check-docs.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/.github/workflows/docs.yml` & `proxystore-0.5.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/.github/workflows/integration.yml` & `proxystore-0.5.1/.github/workflows/integration.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/.github/workflows/publish.yml` & `proxystore-0.5.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/.github/workflows/tests.yml` & `proxystore-0.5.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/.gitignore` & `proxystore-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/.pre-commit-config.yaml` & `proxystore-0.5.1/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -17,22 +17,22 @@
     hooks:
       - id: black
   - repo: 'https://github.com/codespell-project/codespell'
     rev: v2.2.4
     hooks:
       - id: codespell
   - repo: 'https://github.com/charliermarsh/ruff-pre-commit'
-    rev: v0.0.265
+    rev: v0.0.270
     hooks:
       - id: ruff
         args:
           - '--fix'
           - '--exit-non-zero-on-fix'
   - repo: 'https://github.com/pre-commit/mirrors-mypy'
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
       - id: mypy
         additional_dependencies:
           - globus-sdk
           - parsl
           - quart
           - types-redis
```

### Comparing `proxystore-0.5.0/LICENSE` & `proxystore-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/PKG-INFO` & `proxystore-0.5.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxystore
-Version: 0.5.0
+Version: 0.5.1
 Summary: Lazy object proxy interface for distributed stores.
 Author: Globus Labs
 Author-email: Greg Pauloski <jgpauloski@uchicago.edu>
 Maintainer-email: Greg Pauloski <jgpauloski@uchicago.edu>, Valerie Hayot-Sasson <vhayot@uchicago.edu>
 License: FILE
 Project-URL: homepage, https://proxystore.dev
 Project-URL: documentation, https://docs.proxystore.dev
@@ -100,7 +100,21 @@
     assert isinstance(x, MyDataType)
 
 my_function(proxy)  # Succeeds
 ```
 
 Check out the [Get Started](https://docs.proxystore.dev/main/get-started)
 guide to learn more!
+
+## Citation
+
+If you use ProxyStore or any of this code in your work, please cite the following [paper](https://arxiv.org/abs/2305.09593).
+```
+@misc{pauloski2023proxystore,
+    author = {J. Gregory Pauloski and Valerie Hayot-Sasson and Logan Ward and Nathaniel Hudson and Charlie Sabino and Matt Baughman and Kyle Chard and Ian Foster},
+    title = {{Accelerating Communications in Federated Applications with Transparent Object Proxies}},
+    archiveprefix = {arXiv},
+    eprint = {2305.09593},
+    primaryclass = {cs.DC},
+    year = {2023}
+}
+```
```

### Comparing `proxystore-0.5.0/README.md` & `proxystore-0.5.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -75,7 +75,21 @@
     assert isinstance(x, MyDataType)
 
 my_function(proxy)  # Succeeds
 ```
 
 Check out the [Get Started](https://docs.proxystore.dev/main/get-started)
 guide to learn more!
+
+## Citation
+
+If you use ProxyStore or any of this code in your work, please cite the following [paper](https://arxiv.org/abs/2305.09593).
+```
+@misc{pauloski2023proxystore,
+    author = {J. Gregory Pauloski and Valerie Hayot-Sasson and Logan Ward and Nathaniel Hudson and Charlie Sabino and Matt Baughman and Kyle Chard and Ian Foster},
+    title = {{Accelerating Communications in Federated Applications with Transparent Object Proxies}},
+    archiveprefix = {arXiv},
+    eprint = {2305.09593},
+    primaryclass = {cs.DC},
+    year = {2023}
+}
+```
```

### Comparing `proxystore-0.5.0/docs/_templates/python/material/function.html` & `proxystore-0.5.1/docs/_templates/python/material/function.html`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,16 @@
       {% with labels = function.labels %}
         {% include "labels.html" with context %}
       {% endwith %}
 
     {% endfilter %}
 
     {% if config.separate_signature %}
-      {% filter highlight(language="python", inline=False) %}
-        {% filter format_signature(config.line_length) %}
-          {% if show_full_path %}{{ function.path }}{% else %}{{ function.name }}{% endif %}
-          {% include "signature.html" with context %}
-        {% endfilter %}
+      {% filter format_signature(function, config.line_length, crossrefs=config.signature_crossrefs) %}
+        {% if show_full_path %}{{ function.path }}{% else %}{{ function.name }}{% endif %}
       {% endfilter %}
     {% endif %}
 
   {% else %}
     {% if config.show_root_toc_entry %}
       {% filter heading(heading_level,
           role="function",
```

### Comparing `proxystore-0.5.0/docs/_templates/python/material/module.html` & `proxystore-0.5.1/docs/_templates/python/material/module.html`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/api/cli.md` & `proxystore-0.5.1/docs/api/cli.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/concepts/connector.md` & `proxystore-0.5.1/docs/concepts/connector.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/concepts/index.md` & `proxystore-0.5.1/docs/concepts/index.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/concepts/proxy.md` & `proxystore-0.5.1/docs/concepts/proxy.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/concepts/store.md` & `proxystore-0.5.1/docs/concepts/store.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/contributing/index.md` & `proxystore-0.5.1/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/contributing/issues-pull-requests.md` & `proxystore-0.5.1/docs/contributing/issues-pull-requests.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/contributing/releases.md` & `proxystore-0.5.1/docs/contributing/releases.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/contributing/style-guide.md` & `proxystore-0.5.1/docs/contributing/style-guide.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/css/extra.css` & `proxystore-0.5.1/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/css/mkdocstrings.css` & `proxystore-0.5.1/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/examples.md` & `proxystore-0.5.1/docs/examples.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/generate_api.py` & `proxystore-0.5.1/docs/generate_api.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/get-started.md` & `proxystore-0.5.1/docs/get-started.md`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 ```python title="Basic ProxyStore Usage" linenums="1"
 from proxystore.connectors.redis import RedisConnector
 from proxystore.store import get_store
 from proxystore.store import register_store
 from proxystore.store import Store
 
-store = Store(name='my-store', RedisConnector(hostname='localhost', port=1234))
+store = Store('my-store', RedisConnector(hostname='localhost', port=1234))
 register_store(store)
 
 store = get_store('my-store')  # (1)!
 
 key = store.put(my_object)  # (2)!
 assert my_object == store.get(key)
```

### Comparing `proxystore-0.5.0/docs/guides/endpoints-debugging.md` & `proxystore-0.5.1/docs/guides/endpoints-debugging.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/guides/endpoints.md` & `proxystore-0.5.1/docs/guides/endpoints.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/guides/globus-compute.md` & `proxystore-0.5.1/docs/guides/globus-compute.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/guides/performance.md` & `proxystore-0.5.1/docs/guides/performance.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/installation.md` & `proxystore-0.5.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/static/endpoint-overview.svg` & `proxystore-0.5.1/docs/static/endpoint-overview.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/static/endpoint-peering.svg` & `proxystore-0.5.1/docs/static/endpoint-peering.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/static/favicon.png` & `proxystore-0.5.1/docs/static/favicon.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/static/icon.png` & `proxystore-0.5.1/docs/static/icon.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/static/logo-dark.png` & `proxystore-0.5.1/docs/static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/static/logo-light.png` & `proxystore-0.5.1/docs/static/logo-light.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/static/proxystore-overview.svg` & `proxystore-0.5.1/docs/static/proxystore-overview.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/docs/static/proxystore-schematic.svg` & `proxystore-0.5.1/docs/static/proxystore-schematic.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/examples/README.md` & `proxystore-0.5.1/examples/README.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/examples/globus-compute/README.md` & `proxystore-0.5.1/examples/globus-compute/README.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/examples/globus-compute/mapreduce_globus_compute.py` & `proxystore-0.5.1/examples/globus-compute/mapreduce_globus_compute.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/examples/globus-compute/run.sh` & `proxystore-0.5.1/examples/globus-compute/run.sh`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/examples/parsl/mapreduce_parsl.py` & `proxystore-0.5.1/examples/parsl/mapreduce_parsl.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/examples/parsl/run.sh` & `proxystore-0.5.1/examples/parsl/run.sh`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/examples/store_metrics.py` & `proxystore-0.5.1/examples/store_metrics.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/mkdocs.yml` & `proxystore-0.5.1/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,16 @@
       - CLI Reference: api/cli.md
       - Legacy Docs: api/legacy-docs.md
   - Contributing:
       - contributing/index.md
       - Style Guide: contributing/style-guide.md
       - Issues and Pull Requests: contributing/issues-pull-requests.md
       - Releases: contributing/releases.md
+  - Publications:
+      - publications/index.md
 
 plugins:
   - gen-files:
       scripts:
         - docs/generate_api.py
   - literate-nav:
       nav_file: SUMMARY.md
```

### Comparing `proxystore-0.5.0/proxystore/__init__.py` & `proxystore-0.5.1/proxystore/__init__.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/connectors/__init__.py` & `proxystore-0.5.1/proxystore/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/connectors/connector.py` & `proxystore-0.5.1/proxystore/connectors/connector.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/connectors/dim/margo.py` & `proxystore-0.5.1/proxystore/connectors/dim/margo.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,42 +74,46 @@
         protocol: The communication protocol to use.
         address: The network IP to use for transfer. Has precedence over `interface`
             if both are provided.
         interface: The network interface to use. `addr` has precedence over
             this attribute if both are provided.
         timeout: Timeout in seconds to try connecting to a local server before
             spawning one.
+        force_spawn_server: Force spawn a server rather than waiting to check
+            if one is already running.
 
     Raises:
         ServerTimeoutError: If a local server cannot be connected to within
             `timeout` seconds, and a new local server does not respond within
             `timeout` seconds after being started.
     """
 
     def __init__(
         self,
         port: int,
         protocol: Protocol | str,
         address: str | None = None,
         interface: str | None = None,
         timeout: float = 1,
+        force_spawn_server: bool = False,
     ) -> None:
         # Py-Mochi-Margo is not a required dependency and requires the user
         # to install it themselves.
         if pymargo_import_error is not None:  # pragma: no cover
             raise pymargo_import_error
 
         self._address = address
         self._interface = interface
         self.port = port
         self.protocol = (
             protocol if isinstance(protocol, str) else protocol.value
         )
 
         self.timeout = timeout
+        self.force_spawn_server = force_spawn_server
 
         self.engine = Engine(
             self.protocol,
             mode=pymargo.client,
             use_progress_thread=True,
         )
 
@@ -126,33 +130,38 @@
         self._rpcs = {
             'evict': self.engine.register('evict'),
             'exists': self.engine.register('exists'),
             'get': self.engine.register('get'),
             'put': self.engine.register('put'),
         }
 
+        server_available = False
+        if not force_spawn_server:
+            try:
+                logger.info(
+                    f'Connecting to local server (address={self.url})...',
+                )
+                wait_for_server(
+                    self.protocol,
+                    self.address,
+                    self.port,
+                    self.timeout,
+                )
+                logger.info(
+                    f'Connected to local server (address={self.url})',
+                )
+                server_available = True
+            except ServerTimeoutError:
+                logger.info(
+                    'Failed to connect to local server '
+                    f'(address={self.url}, timeout={self.timeout})',
+                )
+
         self.server: multiprocessing.context.SpawnProcess | None
-        try:
-            logger.info(
-                f'Connecting to local server (address={self.url})...',
-            )
-            wait_for_server(
-                self.protocol,
-                self.address,
-                self.port,
-                self.timeout,
-            )
-            logger.info(
-                f'Connected to local server (address={self.url})',
-            )
-        except ServerTimeoutError:
-            logger.info(
-                'Failed to connect to local server '
-                f'(address={self.url}, timeout={self.timeout})',
-            )
+        if not server_available or force_spawn_server:
             self.server = spawn_server(
                 self.protocol,
                 self.address,
                 self.port,
                 spawn_timeout=self.timeout,
             )
             logger.info(f'Spawned local server (address={self.url})')
@@ -240,14 +249,15 @@
         """
         return {
             'address': self._address,
             'interface': self._interface,
             'port': self.port,
             'protocol': self.protocol,
             'timeout': self.timeout,
+            'force_spawn_server': self.force_spawn_server,
         }
 
     @classmethod
     def from_config(cls, config: dict[str, Any]) -> MargoConnector:
         """Create a new connector instance from a configuration.
 
         Args:
@@ -540,23 +550,24 @@
     server_process = ctx.Process(
         target=start_server,
         args=(url,),
     )
     server_process.start()
 
     def _kill_on_exit() -> None:  # pragma: no cover
-        server_process.terminate()
-        server_process.join(timeout=kill_timeout)
         if server_process.is_alive():
-            server_process.kill()
-            server_process.join()
-        logger.debug(
-            'Server terminated on parent process exit '
-            f'(pid={server_process.pid})',
-        )
+            server_process.terminate()
+            server_process.join(timeout=kill_timeout)
+            if server_process.is_alive():
+                server_process.kill()
+                server_process.join()
+            logger.debug(
+                'Server terminated on parent process exit '
+                f'(pid={server_process.pid})',
+            )
 
     atexit.register(_kill_on_exit)
     logger.debug('Registered server cleanup atexit callback')
 
     wait_for_server(protocol, address, port, timeout=spawn_timeout)
     logger.debug(
         f'Server started (address={url}, pid={server_process.pid})',
```

### Comparing `proxystore-0.5.0/proxystore/connectors/dim/models.py` & `proxystore-0.5.1/proxystore/connectors/dim/models.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/connectors/dim/ucx.py` & `proxystore-0.5.1/proxystore/connectors/dim/ucx.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/connectors/dim/utils.py` & `proxystore-0.5.1/proxystore/connectors/dim/utils.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/connectors/dim/zmq.py` & `proxystore-0.5.1/proxystore/connectors/dim/zmq.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/connectors/endpoint.py` & `proxystore-0.5.1/proxystore/connectors/endpoint.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/connectors/file.py` & `proxystore-0.5.1/proxystore/connectors/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,18 +31,22 @@
 
 class FileConnector:
     """Connector to shared file system.
 
     Args:
         store_dir: Path to directory to store data in. Note this
             directory will be deleted upon closing the store.
+        clear: Clear all objects on
+            [`close()`][proxystore.connectors.file.FileConnector] by removing
+            `store_dir`.
     """
 
-    def __init__(self, store_dir: str) -> None:
+    def __init__(self, store_dir: str, clear: bool = True) -> None:
         self.store_dir = os.path.abspath(store_dir)
+        self.clear = clear
 
         if not os.path.exists(self.store_dir):
             os.makedirs(self.store_dir, exist_ok=True)
 
     def __enter__(self) -> Self:
         return self
 
@@ -53,34 +57,42 @@
         exc_traceback: TracebackType | None,
     ) -> None:
         self.close()
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}(directory={self.store_dir})'
 
-    def close(self) -> None:
+    def close(self, clear: bool | None = None) -> None:
         """Close the connector and clean up.
 
         Warning:
-            This will delete the `store_dir` directory.
+            This will delete the `store_dir` directory by default.
 
         Warning:
             This method should only be called at the end of the program
             when the connector will no longer be used, for example once all
             proxies have been resolved.
+
+        Args:
+            clear: Remove the store directory. Overrides the default
+                value of `clear` provided when the
+                [`FileConnector`][proxystore.connectors.file.FileConnector]
+                was instantiated.
         """
-        shutil.rmtree(self.store_dir)
+        clear = self.clear if clear is None else clear
+        if clear and os.path.isdir(self.store_dir):
+            shutil.rmtree(self.store_dir)
 
     def config(self) -> dict[str, Any]:
         """Get the connector configuration.
 
         The configuration contains all the information needed to reconstruct
         the connector object.
         """
-        return {'store_dir': self.store_dir}
+        return {'store_dir': self.store_dir, 'clear': self.clear}
 
     @classmethod
     def from_config(cls, config: dict[str, Any]) -> FileConnector:
         """Create a new connector instance from a configuration.
 
         Args:
             config: Configuration returned by `#!python .config()`.
```

### Comparing `proxystore-0.5.0/proxystore/connectors/globus.py` & `proxystore-0.5.1/proxystore/connectors/globus.py`

 * *Files 3% similar despite different names*

```diff
@@ -289,14 +289,17 @@
         endpoints: Globus endpoints to keep in sync. If passed as a `dict`,
             the dictionary must match the format expected by
             [`GlobusEndpoints.from_dict()`][proxystore.store.globus.GlobusEndpoints.from_dict].
         polling_interval: Interval in seconds to check if Globus
             tasks have finished.
         sync_level: Globus transfer sync level.
         timeout: Timeout in seconds for waiting on Globus tasks.
+        clear: Clear all objects on
+            [`close()`][proxystore.connectors.globus.GlobusConnector.close] by
+            deleting the `local_path` of each endpoint.
 
     Raises:
         GlobusAuthFileError: If the Globus authentication file cannot be found.
         ValueError: If `endpoints` is of an incorrect type.
         ValueError: If the `#!python len(endpoints) != 2` because this
             implementation can currently only keep two endpoints in sync.
     """
@@ -306,14 +309,15 @@
         endpoints: GlobusEndpoints
         | list[GlobusEndpoint]
         | dict[str, dict[str, str]],
         polling_interval: int = 1,
         sync_level: int
         | Literal['exists', 'size', 'mtime', 'checksum'] = 'mtime',
         timeout: int = 60,
+        clear: bool = True,
     ) -> None:
         if isinstance(endpoints, GlobusEndpoints):
             self.endpoints = endpoints
         elif isinstance(endpoints, list):
             self.endpoints = GlobusEndpoints(endpoints)
         elif isinstance(endpoints, dict):
             self.endpoints = GlobusEndpoints.from_dict(endpoints)
@@ -325,14 +329,15 @@
         if len(endpoints) != 2:
             raise ValueError(
                 'ProxyStore only supports two endpoints at a time',
             )
         self.polling_interval = polling_interval
         self.sync_level = sync_level
         self.timeout = timeout
+        self.clear = clear
 
         try:
             authorizer = get_proxystore_authorizer()
         except GlobusAuthFileError as e:
             raise GlobusAuthFileError(
                 'Error loading Globus auth tokens. Complete the '
                 'authentication process with the proxystore-globus-auth tool.',
@@ -464,49 +469,62 @@
                 )
             else:
                 raise AssertionError('Unreachable.')
 
         tdata = _submit_transfer_action(self._transfer_client, transfer_task)
         return tdata['task_id']
 
-    def close(self) -> None:
+    def close(self, clear: bool | None = None) -> None:
         """Close the connector and clean up.
 
         Warning:
-            This will delete the directory at `local_path` on each endpoint.
+            This will delete the directory at `local_path` on each endpoint
+            by default.
 
         Warning:
             This method should only be called at the end of the program when
             the store will no longer be used, for example once all proxies
             have been resolved.
+
+        Args:
+            clear: Remove the store directory. Overrides the default
+                value of `clear` provided when the
+                [`GlobusConnector`][proxystore.connectors.globus.GlobusConnector]
+                was instantiated.
         """
-        for endpoint in self.endpoints:
-            delete_task = globus_sdk.DeleteData(
-                self._transfer_client,
-                endpoint=endpoint.uuid,
-                recursive=True,
-            )
-            delete_task['notify_on_succeeded'] = False
-            delete_task['notify_on_failed'] = False
-            delete_task['notify_on_inactive'] = False
-            delete_task.add_item(endpoint.endpoint_path)
-            tdata = _submit_transfer_action(self._transfer_client, delete_task)
-            self._wait_on_tasks(tdata['task_id'])
+        clear = self.clear if clear is None else clear
+        if clear:
+            for endpoint in self.endpoints:
+                delete_task = globus_sdk.DeleteData(
+                    self._transfer_client,
+                    endpoint=endpoint.uuid,
+                    recursive=True,
+                )
+                delete_task['notify_on_succeeded'] = False
+                delete_task['notify_on_failed'] = False
+                delete_task['notify_on_inactive'] = False
+                delete_task.add_item(endpoint.endpoint_path)
+                tdata = _submit_transfer_action(
+                    self._transfer_client,
+                    delete_task,
+                )
+                self._wait_on_tasks(tdata['task_id'])
 
     def config(self) -> dict[str, Any]:
         """Get the connector configuration.
 
         The configuration contains all the information needed to reconstruct
         the connector object.
         """
         return {
             'endpoints': self.endpoints.dict(),
             'polling_interval': self.polling_interval,
             'sync_level': self.sync_level,
             'timeout': self.timeout,
+            'clear': self.clear,
         }
 
     @classmethod
     def from_config(cls, config: dict[str, Any]) -> GlobusConnector:
         """Create a new connector instance from a configuration.
 
         Args:
```

### Comparing `proxystore-0.5.0/proxystore/connectors/local.py` & `proxystore-0.5.1/proxystore/connectors/local.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/connectors/multi.py` & `proxystore-0.5.1/proxystore/connectors/multi.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/connectors/redis.py` & `proxystore-0.5.1/proxystore/connectors/redis.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,19 +28,24 @@
 
 class RedisConnector:
     """Redis server connector.
 
     Args:
         hostname: Redis server hostname.
         port: Redis server port.
+        clear: Remove all keys from the Redis server when
+            [`close()`][proxystore.connectors.redis.RedisConnector.close]
+            is called. This will delete keys regardless of if they were
+            created by ProxyStore or not.
     """
 
-    def __init__(self, hostname: str, port: int) -> None:
+    def __init__(self, hostname: str, port: int, clear: bool = False) -> None:
         self.hostname = hostname
         self.port = port
+        self.clear = clear
         self._redis_client = redis.StrictRedis(host=hostname, port=port)
 
     def __enter__(self) -> Self:
         return self
 
     def __exit__(
         self,
@@ -52,25 +57,43 @@
 
     def __repr__(self) -> str:
         return (
             f'{self.__class__.__name__}(hostname={self.hostname}, '
             f'port={self.port})'
         )
 
-    def close(self) -> None:
-        """Close the connector and clean up."""
-        pass
+    def close(self, clear: bool | None = None) -> None:
+        """Close the connector and clean up.
+
+        Warning:
+            Passing `clear=True` will result in **ALL** keys in the Redis
+            server being deleted regardless of if they were created by
+            ProxyStore or not.
+
+        Args:
+            clear: Remove all keys in the Redis server. Overrides the default
+                value of `clear` provided when the
+                [`RedisConnector`][proxystore.connectors.redis.RedisConnector]
+                was instantiated.
+        """
+        if self.clear if clear is None else clear:
+            self._redis_client.flushdb()
+        self._redis_client.close()
 
     def config(self) -> dict[str, Any]:
         """Get the connector configuration.
 
         The configuration contains all the information needed to reconstruct
         the connector object.
         """
-        return {'hostname': self.hostname, 'port': self.port}
+        return {
+            'hostname': self.hostname,
+            'port': self.port,
+            'clear': self.clear,
+        }
 
     @classmethod
     def from_config(cls, config: dict[str, Any]) -> RedisConnector:
         """Create a new connector instance from a configuration.
 
         Args:
             config: Configuration returned by `#!python .config()`.
```

### Comparing `proxystore-0.5.0/proxystore/endpoint/__init__.py` & `proxystore-0.5.1/proxystore/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/endpoint/cli.py` & `proxystore-0.5.1/proxystore/endpoint/cli.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/endpoint/client.py` & `proxystore-0.5.1/proxystore/endpoint/client.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/endpoint/commands.py` & `proxystore-0.5.1/proxystore/endpoint/commands.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/endpoint/config.py` & `proxystore-0.5.1/proxystore/endpoint/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,21 +151,21 @@
 
     if os.path.exists(path):
         with open(path) as f:
             try:
                 cfg_json = json.load(f)
             except json.decoder.JSONDecodeError as e:
                 raise ValueError(
-                    f'Unable to parse ({path}): {str(e)}.',
+                    f'Unable to parse ({path}): {e!s}.',
                 ) from None
         try:
             cfg = EndpointConfig(**cfg_json)
         except TypeError as e:
             raise ValueError(
-                f'Keys in config ({path}) do not match expected: {str(e)}.',
+                f'Keys in config ({path}) do not match expected: {e!s}.',
             ) from None
         return cfg
     else:
         raise FileNotFoundError(
             f'Endpoint directory {endpoint_dir} does not contain a valid '
             'configuration.',
         )
```

### Comparing `proxystore-0.5.0/proxystore/endpoint/endpoint.py` & `proxystore-0.5.1/proxystore/endpoint/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,15 @@
             f'id={request.uuid} and key={request.key}) to {endpoint}',
         )
         try:
             await self._peer_manager.send(endpoint, serialize(request))
         except Exception as e:
             self._pending_requests[request.uuid].set_exception(
                 PeerRequestError(
-                    f'Request to peer {endpoint} failed: {str(e)}',
+                    f'Request to peer {endpoint} failed: {e!s}',
                 ),
             )
         return self._pending_requests[request.uuid]
 
     def _is_peer_request(self, endpoint: UUID | None) -> bool:
         """Check if this request should be forwarded to peer endpoint."""
         if self._mode == EndpointMode.SOLO:
```

### Comparing `proxystore-0.5.0/proxystore/endpoint/exceptions.py` & `proxystore-0.5.1/proxystore/endpoint/exceptions.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/endpoint/messages.py` & `proxystore-0.5.1/proxystore/endpoint/messages.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/endpoint/serve.py` & `proxystore-0.5.1/proxystore/endpoint/serve.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/endpoint/storage.py` & `proxystore-0.5.1/proxystore/endpoint/storage.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/factory.py` & `proxystore-0.5.1/proxystore/factory.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/globus.py` & `proxystore-0.5.1/proxystore/globus.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/p2p/__init__.py` & `proxystore-0.5.1/proxystore/p2p/__init__.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/p2p/chunks.py` & `proxystore-0.5.1/proxystore/p2p/chunks.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/p2p/connection.py` & `proxystore-0.5.1/proxystore/p2p/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
         Args:
             message: Message received from the relay server.
         """
         if message.error is not None:
             self._handshake_success.set_exception(
                 PeerConnectionError(
                     'Received error message from relay server: '
-                    f'{str(message.error)}',
+                    f'{message.error!s}',
                 ),
             )
             return
 
         if message.description_type == 'offer':
             logger.info(
                 f'{self._log_prefix}: received offer from '
```

### Comparing `proxystore-0.5.0/proxystore/p2p/counter.py` & `proxystore-0.5.1/proxystore/p2p/counter.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/p2p/manager.py` & `proxystore-0.5.1/proxystore/p2p/manager.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/p2p/messages.py` & `proxystore-0.5.1/proxystore/p2p/messages.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/p2p/relay.py` & `proxystore-0.5.1/proxystore/p2p/relay.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/p2p/relay_client.py` & `proxystore-0.5.1/proxystore/p2p/relay_client.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/p2p/task.py` & `proxystore-0.5.1/proxystore/p2p/task.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/proxy.py` & `proxystore-0.5.1/proxystore/proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,14 +78,28 @@
     Note:
         When a proxy instance is pickled, only the `factory` is pickled, not
         the wrapped object. Thus, proxy instances can be pickled and passed
         around cheaply, and once the proxy is unpickled and used, the `factory`
         will be called again to resolve the object.
 
     Warning:
+        A proxy of a singleton type (e.g., `True`, `False`, and `None`) will
+        not behave exactly as a singleton type would. This is because the
+        proxy itself is not a singleton.
+
+        ```python
+        >>> from proxystore.proxy import Proxy
+        >>> p = Proxy(lambda: True)
+        >>> p == True
+        True
+        >>> p is True
+        False
+        ```
+
+    Warning:
         Python bindings to other languages (e.g., C, C++) may throw type
         errors when receiving a [`Proxy`][proxystore.proxy.Proxy] instance.
         Casting the proxy or extracting the target object may be needed.
 
         ```python
         >>> import io
         >>> from proxystore.proxy import Proxy
```

### Comparing `proxystore-0.5.0/proxystore/serialize.py` & `proxystore-0.5.1/proxystore/serialize.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/store/base.py` & `proxystore-0.5.1/proxystore/store/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,71 @@
 """Store implementation."""
 from __future__ import annotations
 
 import logging
 import sys
+import threading
 from concurrent.futures import Future
 from concurrent.futures import ThreadPoolExecutor
 from types import TracebackType
 from typing import Any
 from typing import Callable
 from typing import cast
 from typing import Generic
+from typing import List
+from typing import overload
 from typing import Sequence
 from typing import Tuple
 from typing import TypeVar
+from typing import Union
+
+if sys.version_info >= (3, 9):  # pragma: >=3.9 cover
+    from typing import Literal
+else:  # pragma: <3.9 cover
+    from typing_extensions import Literal
 
 if sys.version_info >= (3, 11):  # pragma: >=3.11 cover
     from typing import Self
 else:  # pragma: <3.11 cover
     from typing_extensions import Self
 
 import proxystore
 import proxystore.serialize
 from proxystore.connectors.connector import Connector
 from proxystore.proxy import Proxy
 from proxystore.proxy import ProxyLocker
 from proxystore.store.cache import LRUCache
+from proxystore.store.exceptions import NonProxiableTypeError
 from proxystore.store.exceptions import ProxyResolveMissingKeyError
 from proxystore.store.metrics import StoreMetrics
 from proxystore.timer import Timer
 from proxystore.utils import get_class_path
 from proxystore.utils import import_class
 
 _default_pool = ThreadPoolExecutor()
+_factory_get_store_lock = threading.Lock()
 logger = logging.getLogger(__name__)
 
 T = TypeVar('T')
+NonProxiableT = TypeVar('NonProxiableT', bool, None)
+
 ConnectorT = TypeVar('ConnectorT', bound=Connector[Any])
 """Connector type variable."""
 ConnectorKeyT = Tuple[Any, ...]
 """Connector key type alias."""
 SerializerT = Callable[[Any], bytes]
 """Serializer type alias."""
 DeserializerT = Callable[[bytes], Any]
 """Deserializer type alias."""
 
+# These should be kept in sync with NonProxiableT
+_NON_PROXIABLE_TYPES = (bool, type(None))
+
+_MISSING_OBJECT = object()
+
 
 class StoreFactory(Generic[ConnectorT, T]):
     """Factory that resolves an object from a store.
 
     Adds support for asynchronously retrieving objects from a
     [`Store`][proxystore.store.base.Store] instance.
 
@@ -113,32 +131,37 @@
     def get_store(self) -> Store[ConnectorT]:
         """Get store and reinitialize if necessary.
 
         Raises:
             ValueError: If the type of the returned store does not match the
                 expected store type passed to the factory constructor.
         """
-        store = proxystore.store.get_store(self.store_config['name'])
-        if store is None:
-            store = Store.from_config(self.store_config)
-            proxystore.store.register_store(store)
-        return store
+        with _factory_get_store_lock:
+            store = proxystore.store.get_store(self.store_config['name'])
+            if store is None:
+                store = Store.from_config(self.store_config)
+                proxystore.store.register_store(store)
+            return store
 
     def resolve(self) -> T:
         """Get object associated with key from store.
 
         Raises:
             ProxyResolveMissingKeyError: If the key associated with this
                 factory does not exist in the store.
         """
         with Timer() as timer:
             store = self.get_store()
-            obj = store.get(self.key, deserializer=self.deserializer)
+            obj = store.get(
+                self.key,
+                deserializer=self.deserializer,
+                default=_MISSING_OBJECT,
+            )
 
-            if obj is None:
+            if obj is _MISSING_OBJECT:
                 raise ProxyResolveMissingKeyError(
                     self.key,
                     type(store),
                     store.name,
                 )
 
             if self.evict:
@@ -258,23 +281,29 @@
         """Deserializer for this instance."""
         return (
             self._deserializer
             if self._deserializer is not None
             else proxystore.serialize.deserialize
         )
 
-    def close(self) -> None:
+    def close(self, *args: Any, **kwargs: Any) -> None:
         """Close the connector associated with the store.
 
         Warning:
             This method should only be called at the end of the program
             when the store will no longer be used, for example once all
             proxies have been resolved.
+
+        Args:
+            args: Positional arguments to pass to
+                [`Connector.close()`][proxystore.connectors.connector.Connector.close].
+            kwargs: Keyword arguments to pass to
+                [`Connector.close()`][proxystore.connectors.connector.Connector.close].
         """
-        self.connector.close()
+        self.connector.close(*args, **kwargs)
 
     def config(self) -> dict[str, Any]:
         """Get the store configuration.
 
         Example:
             ```python
             >>> store = Store(...)
@@ -446,38 +475,90 @@
             key: Key potentially associated with stored object.
 
         Returns:
             If the object is cached.
         """
         return self.cache.exists(key)
 
+    # MyPy raises the following error which seems more of a lint than a type
+    # error because NonProxiableT is a subset of T.
+    #     Overloaded function signatures 1 and 2 overlap with
+    #     incompatible return types  [misc]
+    @overload
+    def proxy(  # type: ignore[misc]
+        self,
+        obj: NonProxiableT,
+        *,
+        evict: bool = ...,
+        serializer: SerializerT | None = ...,
+        deserializer: DeserializerT | None = ...,
+        skip_nonproxiable: Literal[True] = ...,
+        **kwargs: Any,
+    ) -> NonProxiableT:
+        ...
+
+    @overload
     def proxy(
         self,
         obj: T,
         *,
+        evict: bool = ...,
+        serializer: SerializerT | None = ...,
+        deserializer: DeserializerT | None = ...,
+        skip_nonproxiable: bool = ...,
+        **kwargs: Any,
+    ) -> Proxy[T]:
+        ...
+
+    def proxy(
+        self,
+        obj: T | NonProxiableT,
+        *,
         evict: bool = False,
         serializer: SerializerT | None = None,
         deserializer: DeserializerT | None = None,
+        skip_nonproxiable: bool = False,
         **kwargs: Any,
-    ) -> Proxy[T]:
+    ) -> Proxy[T] | NonProxiableT:
         """Create a proxy that will resolve to an object in the store.
 
         Args:
             obj: The object to place in store and return a proxy for.
             evict: If the proxy should evict the object once resolved.
             serializer: Optionally override the default serializer for the
                 store instance.
             deserializer: Optionally override the default deserializer for the
                 store instance.
+            skip_nonproxiable: Return non-proxiable types (e.g., built-in
+                constants like `bool` or `None`) rather than raising a
+                [`NonProxiableTypeError`][proxystore.store.exceptions.NonProxiableTypeError].
             kwargs: Additional keyword arguments to pass to
                 [`Connector.put()`][proxystore.connectors.connector.Connector.put].
 
         Returns:
-            A proxy of the object.
-        """
+            A proxy of the object unless `obj` is a non-proxiable type \
+            `#!python skip_nonproxiable is True` in which case `obj` is \
+            returned directly.
+
+        Raises:
+            NonProxiableTypeError: If `obj` is a non-proxiable type. This
+                behavior can be overridden by setting
+                `#!python skip_nonproxiable=True`.
+        """
+        if isinstance(obj, _NON_PROXIABLE_TYPES):
+            if skip_nonproxiable:
+                # MyPy raises the following error which is not correct:
+                #     Incompatible return value type (got "Optional[bool]",
+                #     expected "Optional[Proxy[T]]")  [return-value]
+                return obj  # type: ignore[return-value]
+            else:
+                raise NonProxiableTypeError(
+                    f'Object of {type(obj)} is not proxiable.',
+                )
+
         with Timer() as timer:
             key = self.put(obj, serializer=serializer, **kwargs)
             factory: StoreFactory[ConnectorT, T] = StoreFactory(
                 key,
                 store_config=self.config(),
                 deserializer=deserializer,
                 evict=evict,
@@ -490,57 +571,126 @@
 
         logger.debug(
             f'Store(name="{self.name}"): PROXY {key} in '
             f'{timer.elapsed_ms:.3f} ms',
         )
         return proxy
 
+    # This method has the same MyPy complaint as Store.proxy()
+    @overload
+    def proxy_batch(  # type: ignore[misc]
+        self,
+        objs: Sequence[NonProxiableT],
+        *,
+        evict: bool = ...,
+        serializer: SerializerT | None = ...,
+        deserializer: DeserializerT | None = ...,
+        skip_nonproxiable: Literal[True] = ...,
+        **kwargs: Any,
+    ) -> list[NonProxiableT]:
+        ...
+
+    @overload
     def proxy_batch(
         self,
         objs: Sequence[T],
         *,
+        evict: bool = ...,
+        serializer: SerializerT | None = ...,
+        deserializer: DeserializerT | None = ...,
+        skip_nonproxiable: bool = ...,
+        **kwargs: Any,
+    ) -> list[Proxy[T]]:
+        ...
+
+    # MyPy raises the following:
+    #    Overloaded function implementation cannot produce return type of
+    #    signature 1
+    def proxy_batch(  # type: ignore[misc]
+        self,
+        objs: Sequence[T | NonProxiableT],
+        *,
         evict: bool = False,
         serializer: SerializerT | None = None,
         deserializer: DeserializerT | None = None,
+        skip_nonproxiable: bool = False,
         **kwargs: Any,
-    ) -> list[Proxy[T]]:
+    ) -> list[Proxy[T] | NonProxiableT]:
         """Create proxies that will resolve to an object in the store.
 
         Args:
             objs: The objects to place in store and return a proxies for.
             evict: If a proxy should evict its object once resolved.
             serializer: Optionally override the default serializer for the
                 store instance.
             deserializer: Optionally override the default deserializer for the
                 store instance.
+            skip_nonproxiable: Return non-proxiable types (e.g., built-in
+                constants like `bool` or `None`) rather than raising a
+                [`NonProxiableTypeError`][proxystore.store.exceptions.NonProxiableTypeError].
             kwargs: Additional keyword arguments to pass to
                 [`Connector.put_batch()`][proxystore.connectors.connector.Connector.put_batch].
 
         Returns:
-            A list of proxies of the objects.
+            A list of proxies of each object or the object itself if said \
+            object is not proxiable and `#!python skip_nonproxiable is True`.
+
+        Raises:
+            NonProxiableTypeError: If `obj` is a non-proxiable type. This
+                behavior can be overridden by setting
+                `#!python skip_nonproxiable=True`.
         """
         with Timer() as timer:
-            keys = self.put_batch(objs, serializer=serializer, **kwargs)
+            # Find if there are non-proxiable types and if that's okay
+            non_proxiable: list[tuple[int, Any]] = []
+            for i, obj in enumerate(objs):
+                if isinstance(obj, _NON_PROXIABLE_TYPES):
+                    non_proxiable.append((i, obj))
+
+            if len(non_proxiable) > 0 and not skip_nonproxiable:
+                raise NonProxiableTypeError(
+                    f'Input sequence contains {len(non_proxiable)} '
+                    'objects that are not proxiable.',
+                )
+
+            # Pop non-proxiable types so we can batch proxy the proxiable ones
+            non_proxiable_indicies = [i for i, _ in non_proxiable]
+            proxiable_objs = [
+                obj
+                for i, obj in enumerate(objs)
+                if i not in non_proxiable_indicies
+            ]
+
+            keys = self.put_batch(
+                proxiable_objs,
+                serializer=serializer,
+                **kwargs,
+            )
             proxies: list[Proxy[T]] = [
                 self.proxy_from_key(
                     key,
                     evict=evict,
                     deserializer=deserializer,
                 )
                 for key in keys
             ]
 
+            # Put non-proxiable objects back in their original positions.
+            # The indices of non_proxiable must still be sorted
+            for original_index, original_object in non_proxiable:
+                proxies.insert(original_index, original_object)
+
         if self.metrics is not None:
             self.metrics.add_time('store.proxy_batch', keys, timer.elapsed_ns)
 
         logger.debug(
             f'Store(name="{self.name}"): PROXY_BATCH ({len(proxies)} items) '
             f'in {timer.elapsed_ms:.3f} ms',
         )
-        return proxies
+        return cast(List[Union[Proxy[T], NonProxiableT]], proxies)
 
     def proxy_from_key(
         self,
         key: ConnectorKeyT,
         *,
         evict: bool = False,
         deserializer: DeserializerT | None = None,
@@ -562,48 +712,90 @@
             deserializer=deserializer,
             evict=evict,
             metrics=self.metrics is not None,
         )
         logger.debug(f'Store(name="{self.name}"): PROXY_FROM_KEY {key}')
         return Proxy(factory)
 
+    # This method has the same MyPy complaint as Store.proxy()
+    @overload
+    def locked_proxy(  # type: ignore[misc]
+        self,
+        obj: NonProxiableT,
+        *,
+        evict: bool = ...,
+        serializer: SerializerT | None = ...,
+        deserializer: DeserializerT | None = ...,
+        skip_nonproxiable: Literal[True] = ...,
+        **kwargs: Any,
+    ) -> NonProxiableT:
+        ...
+
+    @overload
     def locked_proxy(
         self,
         obj: T,
         *,
+        evict: bool = ...,
+        serializer: SerializerT | None = ...,
+        deserializer: DeserializerT | None = ...,
+        skip_nonproxiable: bool = ...,
+        **kwargs: Any,
+    ) -> ProxyLocker[T]:
+        ...
+
+    def locked_proxy(
+        self,
+        obj: T | NonProxiableT,
+        *,
         evict: bool = False,
         serializer: SerializerT | None = None,
         deserializer: DeserializerT | None = None,
+        skip_nonproxiable: bool = True,
         **kwargs: Any,
-    ) -> ProxyLocker[T]:
+    ) -> ProxyLocker[T] | NonProxiableT:
         """Proxy an object and return [`ProxyLocker`][proxystore.proxy.ProxyLocker].
 
         Args:
             obj: The object to place in store and return a proxy for.
             evict: If the proxy should evict the object once resolved.
             serializer: Optionally override the default serializer for the
                 store instance.
             deserializer: Optionally override the default deserializer for the
                 store instance.
+            skip_nonproxiable: Return non-proxiable types (e.g., built-in
+                constants like `bool` or `None`) rather than raising a
+                [`NonProxiableTypeError`][proxystore.store.exceptions.NonProxiableTypeError].
             kwargs: Additional keyword arguments to pass to
                 [`Connector.put()`][proxystore.connectors.connector.Connector.put].
 
         Returns:
-            A proxy wrapped in a [`ProxyLocker`][proxystore.proxy.ProxyLocker].
+            A proxy wrapped in a \
+            [`ProxyLocker`][proxystore.proxy.ProxyLocker] unless `obj` is a \
+            non-proxiable type `#!python skip_nonproxiable is True` in which \
+            case `obj` is returned directly.
+
+        Raises:
+            NonProxiableTypeError: If `obj` is a non-proxiable type. This
+                behavior can be overridden by setting
+                `#!python skip_nonproxiable=True`.
         """
-        return ProxyLocker(
-            self.proxy(
-                obj,
-                evict=evict,
-                serializer=serializer,
-                deserializer=deserializer,
-                **kwargs,
-            ),
+        possible_proxy = self.proxy(
+            obj,
+            evict=evict,
+            serializer=serializer,
+            deserializer=deserializer,
+            skip_nonproxiable=skip_nonproxiable,
+            **kwargs,
         )
 
+        if isinstance(possible_proxy, Proxy):
+            return ProxyLocker(possible_proxy)
+        return possible_proxy
+
     def put(
         self,
         obj: Any,
         *,
         serializer: SerializerT | None = None,
         **kwargs: Any,
     ) -> ConnectorKeyT:
```

### Comparing `proxystore-0.5.0/proxystore/store/cache.py` & `proxystore-0.5.1/proxystore/store/cache.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/store/endpoint.py` & `proxystore-0.5.1/proxystore/store/endpoint.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/store/exceptions.py` & `proxystore-0.5.1/proxystore/store/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,7 +45,11 @@
         self.store_type = store_type
         self.store_name = store_name
         super().__init__(
             f"Proxy cannot resolve target object with key='{self.key}' "
             f"from {self.store_type.__name__}(name='{self.store_name}'): "
             'store returned NoneType with key.',
         )
+
+
+class NonProxiableTypeError(Exception):
+    """Exception raised when proxying an unproxiable type."""
```

### Comparing `proxystore-0.5.0/proxystore/store/file.py` & `proxystore-0.5.1/proxystore/store/file.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/store/globus.py` & `proxystore-0.5.1/proxystore/store/globus.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/store/local.py` & `proxystore-0.5.1/proxystore/store/local.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/store/metrics.py` & `proxystore-0.5.1/proxystore/store/metrics.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/store/multi.py` & `proxystore-0.5.1/proxystore/store/multi.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/store/redis.py` & `proxystore-0.5.1/proxystore/store/redis.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/store/utils.py` & `proxystore-0.5.1/proxystore/store/utils.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/timer.py` & `proxystore-0.5.1/proxystore/timer.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore/utils.py` & `proxystore-0.5.1/proxystore/utils.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/proxystore.egg-info/PKG-INFO` & `proxystore-0.5.1/proxystore.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxystore
-Version: 0.5.0
+Version: 0.5.1
 Summary: Lazy object proxy interface for distributed stores.
 Author: Globus Labs
 Author-email: Greg Pauloski <jgpauloski@uchicago.edu>
 Maintainer-email: Greg Pauloski <jgpauloski@uchicago.edu>, Valerie Hayot-Sasson <vhayot@uchicago.edu>
 License: FILE
 Project-URL: homepage, https://proxystore.dev
 Project-URL: documentation, https://docs.proxystore.dev
@@ -100,7 +100,21 @@
     assert isinstance(x, MyDataType)
 
 my_function(proxy)  # Succeeds
 ```
 
 Check out the [Get Started](https://docs.proxystore.dev/main/get-started)
 guide to learn more!
+
+## Citation
+
+If you use ProxyStore or any of this code in your work, please cite the following [paper](https://arxiv.org/abs/2305.09593).
+```
+@misc{pauloski2023proxystore,
+    author = {J. Gregory Pauloski and Valerie Hayot-Sasson and Logan Ward and Nathaniel Hudson and Charlie Sabino and Matt Baughman and Kyle Chard and Ian Foster},
+    title = {{Accelerating Communications in Federated Applications with Transparent Object Proxies}},
+    archiveprefix = {arXiv},
+    eprint = {2305.09593},
+    primaryclass = {cs.DC},
+    year = {2023}
+}
+```
```

### Comparing `proxystore-0.5.0/proxystore.egg-info/SOURCES.txt` & `proxystore-0.5.1/proxystore.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 docs/css/extra.css
 docs/css/mkdocstrings.css
 docs/guides/endpoints-debugging.md
 docs/guides/endpoints.md
 docs/guides/globus-compute.md
 docs/guides/index.md
 docs/guides/performance.md
+docs/publications/index.md
 docs/static/endpoint-overview.svg
 docs/static/endpoint-peering.svg
 docs/static/favicon.png
 docs/static/icon.png
 docs/static/logo-dark.png
 docs/static/logo-light.png
 docs/static/proxystore-overview.svg
@@ -184,11 +185,12 @@
 tests/p2p/relay_client_test.py
 tests/p2p/relay_test.py
 tests/p2p/task_test.py
 tests/store/__init__.py
 tests/store/cache_test.py
 tests/store/init_test.py
 tests/store/metrics_test.py
+tests/store/shims_test.py
 tests/store/store_basics_test.py
 tests/store/store_metrics_test.py
 tests/store/store_proxy_test.py
 tests/store/utils_test.py
```

### Comparing `proxystore-0.5.0/proxystore.egg-info/requires.txt` & `proxystore-0.5.1/proxystore.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 black
 mkdocs-click
 mkdocs-gen-files
 mkdocs-literate-nav
 mkdocs-material
 mkdocs-section-index
 mkdocstrings
-mkdocstrings-python==0.10.1
+mkdocstrings-python
 mike
 proxystore[all]
 
 [endpoints]
 aiortc>=1.3.2
 aiosqlite
 uvicorn[standard]
```

### Comparing `proxystore-0.5.0/pyproject.toml` & `proxystore-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proxystore"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
     {name = "Globus Labs"},
     {name = "Greg Pauloski", email = "jgpauloski@uchicago.edu"},
 ]
 maintainers = [
     {name = "Greg Pauloski", email = "jgpauloski@uchicago.edu"},
     {name = "Valerie Hayot-Sasson", email = "vhayot@uchicago.edu"},
@@ -73,15 +73,15 @@
     "black",
     "mkdocs-click",
     "mkdocs-gen-files",
     "mkdocs-literate-nav",
     "mkdocs-material",
     "mkdocs-section-index",
     "mkdocstrings",
-    "mkdocstrings-python==0.10.1",
+    "mkdocstrings-python",
     "mike",
     # Needed for generating CLI docs
     "proxystore[all]",
 ]
 
 [project.scripts]
 proxystore-endpoint = "proxystore.endpoint.cli:cli"
```

### Comparing `proxystore-0.5.0/testing/compat.py` & `proxystore-0.5.1/testing/compat.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/testing/connectors.py` & `proxystore-0.5.1/testing/connectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,15 @@
         timeout = 0.01
 
     with ctx():
         connector = margo.MargoConnector(
             protocol=protocol,
             port=port,
             timeout=timeout,
+            force_spawn_server=True,
         )
 
     yield connector
 
     with ctx():
         connector.close()
```

### Comparing `proxystore-0.5.0/testing/endpoint.py` & `proxystore-0.5.1/testing/endpoint.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/testing/mocked/globus.py` & `proxystore-0.5.1/testing/mocked/globus.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/testing/mocked/pymargo.py` & `proxystore-0.5.1/testing/mocked/pymargo.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/testing/mocked/redis.py` & `proxystore-0.5.1/testing/mocked/redis.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,31 @@
 
 class MockStrictRedis:
     """Mock StrictRedis."""
 
     def __init__(self, data: dict[str, Any], *args, **kwargs):
         self.data = data
 
+    def close(self) -> None:
+        """Close the client."""
+        pass
+
     def delete(self, key: str) -> None:
         """Delete key."""
         if key in self.data:
             del self.data[key]
 
     def exists(self, key: str) -> bool:
         """Check if key exists."""
         return key in self.data
 
+    def flushdb(self) -> None:
+        """Remove all keys."""
+        self.data.clear()
+
     def get(self, key: str) -> bytes | None:
         """Get value with key."""
         if key in self.data:
             return self.data[key]
         return None
 
     def mget(self, keys: list[str]) -> list[bytes | None]:
```

### Comparing `proxystore-0.5.0/testing/mocked/ucx.py` & `proxystore-0.5.1/testing/mocked/ucx.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/testing/mocking.py` & `proxystore-0.5.1/testing/mocking.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/testing/relay_server.py` & `proxystore-0.5.1/testing/relay_server.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/testing/scripts/peer_connection_bandwidth.py` & `proxystore-0.5.1/testing/scripts/peer_connection_bandwidth.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/testing/scripts/peer_endpoint_bandwidth.py` & `proxystore-0.5.1/testing/scripts/peer_endpoint_bandwidth.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/testing/scripts/peer_manager_bandwidth.py` & `proxystore-0.5.1/testing/scripts/peer_manager_bandwidth.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/testing/utils.py` & `proxystore-0.5.1/testing/utils.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/conftest.py` & `proxystore-0.5.1/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,21 +39,15 @@
 from testing.connectors import margo_connector
 from testing.connectors import multi_connector
 from testing.connectors import redis_connector
 from testing.connectors import ucx_connector
 from testing.connectors import zmq_connector
 from testing.endpoint import endpoint
 from testing.relay_server import relay_server
-from testing.stores import endpoint_store
-from testing.stores import file_store
-from testing.stores import globus_store
-from testing.stores import local_store
-from testing.stores import multi_store
-from testing.stores import redis_store
-from testing.stores import store_implementation
+from testing.stores import store
 
 
 def pytest_addoption(parser):
     """Add custom command line options for tests."""
     parser.addoption(
         '--use-uvloop',
         action='store_true',
```

### Comparing `proxystore-0.5.0/tests/connectors/connector_test.py` & `proxystore-0.5.1/tests/connectors/connector_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/connectors/dim/margo_test.py` & `proxystore-0.5.1/tests/connectors/dim/margo_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 def test_multiple_connectors() -> None:  # pragma: no cover
     port = open_port()
     # C1 creates the server
     c1 = MargoConnector(
         protocol='tcp',
         port=port,
         timeout=TIMEOUT,
+        force_spawn_server=True,
     )
     c2 = MargoConnector(
         protocol='tcp',
         port=port,
         timeout=TIMEOUT,
     )
```

### Comparing `proxystore-0.5.0/tests/connectors/dim/ucx_test.py` & `proxystore-0.5.1/tests/connectors/dim/ucx_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/connectors/dim/zmq_test.py` & `proxystore-0.5.1/tests/connectors/dim/zmq_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/connectors/endpoint_test.py` & `proxystore-0.5.1/tests/connectors/endpoint_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/connectors/globus_test.py` & `proxystore-0.5.1/tests/connectors/globus_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -290,7 +290,46 @@
     """Test GlobusKey custom equality."""
     key = GlobusKey('a', 'b')
     assert key == GlobusKey('a', 'b')
     assert key == ('a', 'b')
     assert key != ('b', 'b')
     assert key == ('a', 'c')
     assert key != 'a'
+
+
+@pytest.mark.parametrize(
+    ('clear_default', 'clear_override', 'should_exist'),
+    ((True, None, False), (False, True, False), (False, False, True)),
+)
+def test_delete_local_paths_on_close(
+    clear_default: bool,
+    clear_override: bool | None,
+    should_exist: bool,
+) -> None:
+    endpoints = GlobusEndpoints(
+        [
+            GlobusEndpoint(
+                uuid='EP1UUID',
+                endpoint_path='/~/',
+                local_path='/tmp/proxystore-test-1',
+                host_regex='localhost',
+            ),
+            GlobusEndpoint(
+                uuid='EP2UUID',
+                endpoint_path='/~/',
+                local_path='/tmp/proxystore-test-2',
+                host_regex='localhost',
+            ),
+        ],
+    )
+
+    with mock.patch('globus_sdk.TransferClient'), mock.patch(
+        'proxystore.connectors.globus._submit_transfer_action',
+        return_value={'task_id': 'ABCD'},
+    ) as mocked:
+        connector = GlobusConnector(endpoints=endpoints, clear=clear_default)
+        connector.close(clear=clear_override)
+
+    if should_exist:
+        assert mocked.call_count == 0
+    else:
+        assert mocked.call_count == len(endpoints)
```

### Comparing `proxystore-0.5.0/tests/connectors/local_test.py` & `proxystore-0.5.1/tests/connectors/local_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/connectors/multi_test.py` & `proxystore-0.5.1/tests/connectors/multi_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/endpoint/cli_test.py` & `proxystore-0.5.1/tests/endpoint/cli_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/endpoint/client_test.py` & `proxystore-0.5.1/tests/endpoint/client_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/endpoint/commands_test.py` & `proxystore-0.5.1/tests/endpoint/commands_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/endpoint/config_test.py` & `proxystore-0.5.1/tests/endpoint/config_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/endpoint/endpoint_peering_test.py` & `proxystore-0.5.1/tests/endpoint/endpoint_peering_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/endpoint/endpoint_solo_test.py` & `proxystore-0.5.1/tests/endpoint/endpoint_solo_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/endpoint/serve_test.py` & `proxystore-0.5.1/tests/endpoint/serve_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/endpoint/storage_test.py` & `proxystore-0.5.1/tests/endpoint/storage_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/factory_test.py` & `proxystore-0.5.1/tests/factory_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/globus_test.py` & `proxystore-0.5.1/tests/globus_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/integration/endpoints_test.py` & `proxystore-0.5.1/tests/integration/endpoints_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/p2p/chunks_test.py` & `proxystore-0.5.1/tests/p2p/chunks_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/p2p/connection_test.py` & `proxystore-0.5.1/tests/p2p/connection_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/p2p/counter_test.py` & `proxystore-0.5.1/tests/p2p/counter_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/p2p/manager_test.py` & `proxystore-0.5.1/tests/p2p/manager_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/p2p/messages_test.py` & `proxystore-0.5.1/tests/p2p/messages_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/p2p/relay_cli_test.py` & `proxystore-0.5.1/tests/p2p/relay_cli_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/p2p/relay_client_test.py` & `proxystore-0.5.1/tests/p2p/relay_client_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/p2p/relay_test.py` & `proxystore-0.5.1/tests/p2p/relay_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/p2p/task_test.py` & `proxystore-0.5.1/tests/p2p/task_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/proxy_test.py` & `proxystore-0.5.1/tests/proxy_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/serialization_test.py` & `proxystore-0.5.1/tests/serialization_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/store/cache_test.py` & `proxystore-0.5.1/tests/store/cache_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/store/init_test.py` & `proxystore-0.5.1/tests/store/init_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 import pytest
 
 from proxystore.connectors.local import LocalConnector
 from proxystore.factory import SimpleFactory
 from proxystore.proxy import Proxy
 from proxystore.store import get_store
 from proxystore.store import register_store
+from proxystore.store import store_registration
 from proxystore.store import unregister_store
 from proxystore.store.base import Store
 from proxystore.store.exceptions import ProxyStoreFactoryError
 from proxystore.store.exceptions import StoreExistsError
 
 
-def test_store_registration() -> None:
-    """Test registering and unregistering stores directly."""
+def test_register_unregister_store() -> None:
     store = Store('test', connector=LocalConnector())
 
     register_store(store)
     assert get_store('test') == store
 
     with pytest.raises(StoreExistsError):
         register_store(store)
@@ -37,34 +37,51 @@
 
     register_store(store)
     assert get_store('test') == store
     unregister_store(store)
     assert get_store('test') is None
 
 
-def test_lookup_by_proxy(local_connector, redis_connector) -> None:
-    """Make sure get_store works with a proxy."""
+def test_lookup_by_proxy() -> None:
     local1 = Store('local1', connector=LocalConnector())
     local2 = Store('local2', connector=LocalConnector())
-    register_store(local1)
-    register_store(local2)
 
-    # Make a proxy with both
-    local1_proxy: Proxy[list[int]] = local1.proxy([1, 2, 3])
-    local2_proxy: Proxy[list[int]] = local2.proxy([1, 2, 3])
-
-    # Make sure both look up correctly
-    sl1 = get_store(local1_proxy)
-    assert sl1 is not None
-    assert sl1.name == local1.name
-    sl2 = get_store(local2_proxy)
-    assert sl2 is not None
-    assert sl2.name == local2.name
-
-    # Make a proxy without an associated store
-    f = SimpleFactory([1, 2, 3])
-    p = Proxy(f)
-    with pytest.raises(ProxyStoreFactoryError):
-        get_store(p)
+    with store_registration(local1, local2):
+        # Make a proxy with both
+        local1_proxy: Proxy[list[int]] = local1.proxy([1, 2, 3])
+        local2_proxy: Proxy[list[int]] = local2.proxy([1, 2, 3])
+
+        # Make sure both look up correctly
+        sl1 = get_store(local1_proxy)
+        assert sl1 is not None
+        assert sl1.name == local1.name
+        sl2 = get_store(local2_proxy)
+        assert sl2 is not None
+        assert sl2.name == local2.name
+
+        # Make a proxy without an associated store
+        f = SimpleFactory([1, 2, 3])
+        p = Proxy(f)
+        with pytest.raises(ProxyStoreFactoryError):
+            get_store(p)
+
+
+def test_store_registration() -> None:
+    local1 = Store('local1', connector=LocalConnector())
+    local2 = Store('local2', connector=LocalConnector())
+
+    assert get_store(local1.name) is None
+    assert get_store(local2.name) is None
+
+    with store_registration(local1, local2):
+        assert get_store(local1.name) is local1
+        assert get_store(local2.name) is local2
+
+        with pytest.raises(StoreExistsError):
+            with store_registration(local1):
+                pass  # pragma: no cover
+
+        with store_registration(local1, exist_ok=True):
+            pass
 
-    unregister_store('local1')
-    unregister_store('local2')
+    assert get_store(local1.name) is None
+    assert get_store(local2.name) is None
```

### Comparing `proxystore-0.5.0/tests/store/metrics_test.py` & `proxystore-0.5.1/tests/store/metrics_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/store/store_metrics_test.py` & `proxystore-0.5.1/tests/store/store_metrics_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,31 +3,28 @@
 import pathlib
 from typing import Generator
 
 import pytest
 
 from proxystore.connectors.file import FileConnector
 from proxystore.serialize import serialize
-from proxystore.store import register_store
-from proxystore.store import unregister_store
+from proxystore.store import store_registration
 from proxystore.store.base import Store
 
 
 @pytest.fixture()
 def store(
     tmp_path: pathlib.Path,
 ) -> Generator[Store[FileConnector], None, None]:
-    with Store(
-        'test-store',
-        connector=FileConnector(str(tmp_path)),
-        metrics=True,
-    ) as store:
-        register_store(store)
-        yield store
-        unregister_store(store.name)
+    # We use FileConnector here instead of LocalConnector (as in the rest of
+    # the tests) because FileConnector operations take *some* amount of time.
+    path = str(tmp_path)
+    with Store('test', connector=FileConnector(path), metrics=True) as store:
+        with store_registration(store):
+            yield store
 
 
 def test_store_single_key_operations(store: Store[FileConnector]) -> None:
     value = 'value'
     key = store.put(value)
     assert store.exists(key)
     assert store.get(key) == value
```

### Comparing `proxystore-0.5.0/tests/store/utils_test.py` & `proxystore-0.5.1/tests/store/utils_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/timer_test.py` & `proxystore-0.5.1/tests/timer_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tests/utils_test.py` & `proxystore-0.5.1/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.0/tox.ini` & `proxystore-0.5.1/tox.ini`

 * *Files identical despite different names*

