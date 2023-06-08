# Comparing `tmp/dbt-core-1.6.0b2.tar.gz` & `tmp/dbt-core-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-core-1.6.0b2.tar", last modified: Thu May 25 15:44:07 2023, max compression
+gzip compressed data, was "dbt-core-1.6.0b3.tar", last modified: Thu Jun  8 20:55:13 2023, max compression
```

## Comparing `dbt-core-1.6.0b2.tar` & `dbt-core-1.6.0b3.tar`

### file list

```diff
@@ -1,318 +1,331 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.796684 dbt-core-1.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-25 15:44:07.796684 dbt-core-1.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.760683 dbt-core-1.6.0b2/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.760683 dbt-core-1.6.0b2/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.760683 dbt-core-1.6.0b2/dbt/adapters/base/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    55757 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14899 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/base/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/reference_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.760683 dbt-core-1.6.0b2/dbt/adapters/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/sql/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/adapters/sql/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.764683 dbt-core-1.6.0b2/dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    16689 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/option_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.764683 dbt-core-1.6.0b2/dbt/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/_jinja_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/agate_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    21425 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/jinja_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/clients/yaml_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22085 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/compilation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.764683 dbt-core-1.6.0b2/dbt/config/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/config/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/config/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.768683 dbt-core-1.6.0b2/dbt/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22966 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/configured.py
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/context_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/exceptions_jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/macro_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    59345 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/context/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.768683 dbt-core-1.6.0b2/dbt/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.772683 dbt-core-1.6.0b2/dbt/contracts/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49014 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/manifest_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    20939 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    48275 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20957 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/unparsed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/graph/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/publication.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/contracts/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/dataclass_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deprecations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.772683 dbt-core-1.6.0b2/dbt/deps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deps/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deps/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deps/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deps/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deps/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/deps/tarball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.752683 dbt-core-1.6.0b2/dbt/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.772683 dbt-core-1.6.0b2/dbt/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.772683 dbt-core-1.6.0b2/dbt/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/docs/source/_ext/dbt_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.772683 dbt-core-1.6.0b2/dbt/events/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/adapter_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/eventmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    62446 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)   104888 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/events/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    79669 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.772683 dbt-core-1.6.0b2/dbt/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/graph/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/graph/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/graph/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/graph/selector_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/graph/selector_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/helper_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.776683 dbt-core-1.6.0b2/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.776683 dbt-core-1.6.0b2/dbt/include/global_project/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.776683 dbt-core-1.6.0b2/dbt/include/global_project/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/docs/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.756683 dbt-core-1.6.0b2/dbt/include/global_project/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.776683 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/drop_relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/freshness.sql
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/schema.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.776683 dbt-core-1.6.0b2/dbt/include/global_project/macros/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/etc/datetime.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/etc/statement.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.780683 dbt-core-1.6.0b2/dbt/include/global_project/macros/generic_test_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/generic_test_sql/not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/generic_test_sql/relationships.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/generic_test_sql/unique.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.780683 dbt-core-1.6.0b2/dbt/include/global_project/macros/get_custom_name/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.780683 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/configs.sql
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/hooks.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.752683 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.780683 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.780683 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.780683 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.780683 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/seeds/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.784684 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.784684 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/tests/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.784684 dbt-core-1.6.0b2/dbt/include/global_project/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/data_types.sql
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/literal.sql
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/replace.sql
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/split_part.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.756683 dbt-core-1.6.0b2/dbt/include/global_project/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/global_project/tests/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/global_project/tests/generic/builtin.sql
--rw-r--r--   0 runner    (1001) docker     (123)  1497701 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/starter_project/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/starter_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/starter_project/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.756683 dbt-core-1.6.0b2/dbt/include/starter_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/starter_project/models/example/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/starter_project/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/seeds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/starter_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.788684 dbt-core-1.6.0b2/dbt/include/starter_project/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/include/starter_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/internal_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/node_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.792684 dbt-core-1.6.0b2/dbt/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    16910 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/generic_test_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)    76488 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    51437 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/partial.py
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    16830 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/schema_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/schema_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/schema_yaml_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)    37437 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/parser/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/selected_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/semver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.796684 dbt-core-1.6.0b2/dbt/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/freshness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/list.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/run_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21324 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/task/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.796684 dbt-core-1.6.0b2/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.796684 dbt-core-1.6.0b2/dbt/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/tests/fixtures/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/dbt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:07.796684 dbt-core-1.6.0b2/dbt_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-25 15:44:07.000000 dbt-core-1.6.0b2/dbt_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-05-25 15:44:07.000000 dbt-core-1.6.0b2/dbt_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:44:07.000000 dbt-core-1.6.0b2/dbt_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 15:44:07.000000 dbt-core-1.6.0b2/dbt_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:44:07.000000 dbt-core-1.6.0b2/dbt_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-25 15:44:07.000000 dbt-core-1.6.0b2/dbt_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 15:44:07.000000 dbt-core-1.6.0b2/dbt_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:44:07.796684 dbt-core-1.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-25 15:43:54.000000 dbt-core-1.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.969807 dbt-core-1.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-08 20:55:13.969807 dbt-core-1.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.933807 dbt-core-1.6.0b3/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.937807 dbt-core-1.6.0b3/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.937807 dbt-core-1.6.0b3/dbt/adapters/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/base/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/base/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56543 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/base/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/base/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/base/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/base/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/base/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/reference_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.937807 dbt-core-1.6.0b3/dbt/adapters/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/relation_configs/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/relation_configs/config_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/relation_configs/config_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.937807 dbt-core-1.6.0b3/dbt/adapters/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/sql/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/adapters/sql/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.937807 dbt-core-1.6.0b3/dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16778 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17511 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/cli/option_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/cli/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/cli/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.941807 dbt-core-1.6.0b3/dbt/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/clients/_jinja_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/clients/agate_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/clients/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/clients/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/clients/jinja_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/clients/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/clients/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/clients/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22186 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/compilation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.941807 dbt-core-1.6.0b3/dbt/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25258 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/config/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.941807 dbt-core-1.6.0b3/dbt/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22966 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/context/configured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/context/context_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/context/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/context/exceptions_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/context/macro_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/context/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/context/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59435 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/context/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/context/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/context/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.945807 dbt-core-1.6.0b3/dbt/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.945807 dbt-core-1.6.0b3/dbt/contracts/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51957 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/graph/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/graph/manifest_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/graph/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/graph/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51765 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/graph/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/graph/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22212 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/graph/unparsed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/graph/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/publication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/contracts/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/dataclass_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/deprecations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.945807 dbt-core-1.6.0b3/dbt/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/deps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/deps/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/deps/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/deps/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/deps/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/deps/tarball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.929807 dbt-core-1.6.0b3/dbt/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.945807 dbt-core-1.6.0b3/dbt/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.945807 dbt-core-1.6.0b3/dbt/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/docs/source/_ext/dbt_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.949807 dbt-core-1.6.0b3/dbt/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/events/adapter_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/events/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/events/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/events/eventmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/events/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/events/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/events/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62857 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105442 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/events/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79891 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.949807 dbt-core-1.6.0b3/dbt/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/graph/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/graph/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/graph/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29727 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/graph/selector_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/graph/selector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/helper_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.949807 dbt-core-1.6.0b3/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.949807 dbt-core-1.6.0b3/dbt/include/global_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.949807 dbt-core-1.6.0b3/dbt/include/global_project/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/docs/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.929807 dbt-core-1.6.0b3/dbt/include/global_project/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.953807 dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/drop_relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.953807 dbt-core-1.6.0b3/dbt/include/global_project/macros/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/etc/datetime.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/etc/statement.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.953807 dbt-core-1.6.0b3/dbt/include/global_project/macros/generic_test_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/generic_test_sql/not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/generic_test_sql/relationships.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/generic_test_sql/unique.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.953807 dbt-core-1.6.0b3/dbt/include/global_project/macros/get_custom_name/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.953807 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/configs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/hooks.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.929807 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.953807 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.953807 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/materialized_view/create_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/materialized_view/refresh_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.953807 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.957807 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/view/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.957807 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/seeds/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.957807 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.957807 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.957807 dbt-core-1.6.0b3/dbt/include/global_project/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.961807 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/data_types.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/literal.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/split_part.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.929807 dbt-core-1.6.0b3/dbt/include/global_project/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.961807 dbt-core-1.6.0b3/dbt/include/global_project/tests/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/global_project/tests/generic/builtin.sql
+-rw-r--r--   0 runner    (1001) docker     (123)  1497701 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.961807 dbt-core-1.6.0b3/dbt/include/starter_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/starter_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/starter_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/starter_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.961807 dbt-core-1.6.0b3/dbt/include/starter_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/starter_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.961807 dbt-core-1.6.0b3/dbt/include/starter_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/starter_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.933807 dbt-core-1.6.0b3/dbt/include/starter_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.961807 dbt-core-1.6.0b3/dbt/include/starter_project/models/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.961807 dbt-core-1.6.0b3/dbt/include/starter_project/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/starter_project/seeds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.961807 dbt-core-1.6.0b3/dbt/include/starter_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/starter_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.961807 dbt-core-1.6.0b3/dbt/include/starter_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/include/starter_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/internal_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/node_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.965807 dbt-core-1.6.0b3/dbt/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17933 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/generic_test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78441 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51437 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16830 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/schema_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/schema_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16499 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/schema_yaml_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38214 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/parser/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/selected_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/semver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.969807 dbt-core-1.6.0b3/dbt/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18661 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/freshness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/run_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/task/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.969807 dbt-core-1.6.0b3/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.969807 dbt-core-1.6.0b3/dbt/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/tests/fixtures/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/dbt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:13.969807 dbt-core-1.6.0b3/dbt_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-08 20:55:13.000000 dbt-core-1.6.0b3/dbt_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-06-08 20:55:13.000000 dbt-core-1.6.0b3/dbt_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:55:13.000000 dbt-core-1.6.0b3/dbt_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-08 20:55:13.000000 dbt-core-1.6.0b3/dbt_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:55:13.000000 dbt-core-1.6.0b3/dbt_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-08 20:55:13.000000 dbt-core-1.6.0b3/dbt_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 20:55:13.000000 dbt-core-1.6.0b3/dbt_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:55:13.969807 dbt-core-1.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-08 20:55:01.000000 dbt-core-1.6.0b3/setup.py
```

### Comparing `dbt-core-1.6.0b2/PKG-INFO` & `dbt-core-1.6.0b3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7.2
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt-core/fa1ea14ddfb1d5ae319d5141844910dd53ab2834/etc/dbt-core.svg" alt="dbt logo" width="750"/>
 </p>
 <p align="center">
   <a href="https://github.com/dbt-labs/dbt-core/actions/workflows/main.yml">
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b2 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b3 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >=3.7.2 Description-Content-Type:
-text/markdown
+Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
+Description-Content-Type: text/markdown
                                   [dbt logo]
                                   [CI_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. ![architecture](https://raw.githubusercontent.com/dbt-labs/
 dbt-core/6c6649f9129d5d108aa3b0526f634cd8f3a9d1ed/etc/dbt-arch.png) ##
 Understanding dbt Analysts using dbt can transform their data by simply writing
```

### Comparing `dbt-core-1.6.0b2/README.md` & `dbt-core-1.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/adapters/base/__init__.py` & `dbt-core-1.6.0b3/dbt/adapters/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/adapters/base/column.py` & `dbt-core-1.6.0b3/dbt/adapters/base/column.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/adapters/base/connections.py` & `dbt-core-1.6.0b3/dbt/adapters/base/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/adapters/base/impl.py` & `dbt-core-1.6.0b3/dbt/adapters/base/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1315,28 +1315,34 @@
         except Exception:
             raise DbtValidationError(f"Could not parse constraint: {raw_constraint}")
 
     @classmethod
     def render_column_constraint(cls, constraint: ColumnLevelConstraint) -> Optional[str]:
         """Render the given constraint as DDL text. Should be overriden by adapters which need custom constraint
         rendering."""
-        if constraint.type == ConstraintType.check and constraint.expression:
-            return f"check {constraint.expression}"
+        constraint_expression = constraint.expression or ""
+
+        rendered_column_constraint = None
+        if constraint.type == ConstraintType.check and constraint_expression:
+            rendered_column_constraint = f"check ({constraint_expression})"
         elif constraint.type == ConstraintType.not_null:
-            return "not null"
+            rendered_column_constraint = f"not null {constraint_expression}"
         elif constraint.type == ConstraintType.unique:
-            return "unique"
+            rendered_column_constraint = f"unique {constraint_expression}"
         elif constraint.type == ConstraintType.primary_key:
-            return "primary key"
-        elif constraint.type == ConstraintType.foreign_key:
-            return "foreign key"
-        elif constraint.type == ConstraintType.custom and constraint.expression:
-            return constraint.expression
-        else:
-            return None
+            rendered_column_constraint = f"primary key {constraint_expression}"
+        elif constraint.type == ConstraintType.foreign_key and constraint_expression:
+            rendered_column_constraint = f"references {constraint_expression}"
+        elif constraint.type == ConstraintType.custom and constraint_expression:
+            rendered_column_constraint = constraint_expression
+
+        if rendered_column_constraint:
+            rendered_column_constraint = rendered_column_constraint.strip()
+
+        return rendered_column_constraint
 
     @available
     @classmethod
     def render_raw_columns_constraints(cls, raw_columns: Dict[str, Dict[str, Any]]) -> List:
         rendered_column_constraints = []
 
         for v in raw_columns.values():
@@ -1395,21 +1401,23 @@
     @classmethod
     def render_model_constraint(cls, constraint: ModelLevelConstraint) -> Optional[str]:
         """Render the given constraint as DDL text. Should be overriden by adapters which need custom constraint
         rendering."""
         constraint_prefix = f"constraint {constraint.name} " if constraint.name else ""
         column_list = ", ".join(constraint.columns)
         if constraint.type == ConstraintType.check and constraint.expression:
-            return f"{constraint_prefix}check {constraint.expression}"
+            return f"{constraint_prefix}check ({constraint.expression})"
         elif constraint.type == ConstraintType.unique:
-            return f"{constraint_prefix}unique ({column_list})"
+            constraint_expression = f" {constraint.expression}" if constraint.expression else ""
+            return f"{constraint_prefix}unique{constraint_expression} ({column_list})"
         elif constraint.type == ConstraintType.primary_key:
-            return f"{constraint_prefix}primary key ({column_list})"
-        elif constraint.type == ConstraintType.foreign_key:
-            return f"{constraint_prefix}foreign key ({column_list})"
+            constraint_expression = f" {constraint.expression}" if constraint.expression else ""
+            return f"{constraint_prefix}primary key{constraint_expression} ({column_list})"
+        elif constraint.type == ConstraintType.foreign_key and constraint.expression:
+            return f"{constraint_prefix}foreign key ({column_list}) references {constraint.expression}"
         elif constraint.type == ConstraintType.custom and constraint.expression:
             return f"{constraint_prefix}{constraint.expression}"
         else:
             return None
 
 
 COLUMNS_EQUAL_SQL = """
```

### Comparing `dbt-core-1.6.0b2/dbt/adapters/base/meta.py` & `dbt-core-1.6.0b3/dbt/adapters/base/meta.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/adapters/base/plugin.py` & `dbt-core-1.6.0b3/dbt/adapters/base/plugin.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/adapters/base/query_headers.py` & `dbt-core-1.6.0b3/dbt/adapters/base/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/adapters/base/relation.py` & `dbt-core-1.6.0b3/dbt/adapters/base/relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,14 +324,18 @@
     def is_cte(self) -> bool:
         return self.type == RelationType.CTE
 
     @property
     def is_view(self) -> bool:
         return self.type == RelationType.View
 
+    @property
+    def is_materialized_view(self) -> bool:
+        return self.type == RelationType.MaterializedView
+
     @classproperty
     def Table(cls) -> str:
         return str(RelationType.Table)
 
     @classproperty
     def CTE(cls) -> str:
         return str(RelationType.CTE)
@@ -341,14 +345,18 @@
         return str(RelationType.View)
 
     @classproperty
     def External(cls) -> str:
         return str(RelationType.External)
 
     @classproperty
+    def MaterializedView(cls) -> str:
+        return str(RelationType.MaterializedView)
+
+    @classproperty
     def get_relation_type(cls) -> Type[RelationType]:
         return RelationType
 
 
 Info = TypeVar("Info", bound="InformationSchema")
```

### Comparing `dbt-core-1.6.0b2/dbt/adapters/cache.py` & `dbt-core-1.6.0b3/dbt/adapters/cache.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/adapters/factory.py` & `dbt-core-1.6.0b3/dbt/adapters/factory.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/adapters/protocol.py` & `dbt-core-1.6.0b3/dbt/adapters/protocol.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/adapters/reference_keys.py` & `dbt-core-1.6.0b3/dbt/adapters/reference_keys.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/adapters/sql/connections.py` & `dbt-core-1.6.0b3/dbt/adapters/sql/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/adapters/sql/impl.py` & `dbt-core-1.6.0b3/dbt/adapters/sql/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/cli/exceptions.py` & `dbt-core-1.6.0b3/dbt/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/cli/flags.py` & `dbt-core-1.6.0b3/dbt/cli/flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,15 +333,17 @@
         if k in prnt_args:
 
             def add_fn(x):
                 res.insert(0, x)
 
         spinal_cased = k.replace("_", "-")
 
-        if v in (None, False):
+        if k == "macro" and command == CliCommand.RUN_OPERATION:
+            add_fn(v)
+        elif v in (None, False):
             add_fn(f"--no-{spinal_cased}")
         elif v is True:
             add_fn(f"--{spinal_cased}")
         else:
             add_fn(f"--{spinal_cased}={v}")
 
     return res
@@ -380,14 +382,15 @@
         CliCommand.RUN: cli.run,
         CliCommand.RUN_OPERATION: cli.run_operation,
         CliCommand.SEED: cli.seed,
         CliCommand.SHOW: cli.show,
         CliCommand.SNAPSHOT: cli.snapshot,
         CliCommand.SOURCE_FRESHNESS: cli.freshness,
         CliCommand.TEST: cli.test,
+        CliCommand.RETRY: cli.retry,
     }
     click_cmd: Optional[ClickCommand] = CMD_DICT.get(command, None)
     if click_cmd is None:
         raise DbtInternalError(f"No command found for name '{command.name}'")
     return format_params(click_cmd.params)
```

### Comparing `dbt-core-1.6.0b2/dbt/cli/main.py` & `dbt-core-1.6.0b3/dbt/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from dbt.task.compile import CompileTask
 from dbt.task.debug import DebugTask
 from dbt.task.deps import DepsTask
 from dbt.task.freshness import FreshnessTask
 from dbt.task.generate import GenerateTask
 from dbt.task.init import InitTask
 from dbt.task.list import ListTask
+from dbt.task.retry import RetryTask
 from dbt.task.run import RunTask
 from dbt.task.run_operation import RunOperationTask
 from dbt.task.seed import SeedTask
 from dbt.task.serve import ServeTask
 from dbt.task.show import ShowTask
 from dbt.task.snapshot import SnapshotTask
 from dbt.task.test import TestTask
@@ -175,14 +176,15 @@
 @p.profiles_dir
 @p.project_dir
 @p.resource_type
 @p.select
 @p.selector
 @p.show
 @p.state
+@p.defer_state
 @p.deprecated_state
 @p.store_failures
 @p.target
 @p.target_path
 @p.threads
 @p.vars
 @p.version_check
@@ -246,14 +248,15 @@
 @p.profile
 @p.profiles_dir
 @p.project_dir
 @p.select
 @p.selector
 @p.empty_catalog
 @p.state
+@p.defer_state
 @p.deprecated_state
 @p.target
 @p.target_path
 @p.threads
 @p.vars
 @p.version_check
 @requires.postflight
@@ -318,14 +321,15 @@
 @p.profile
 @p.profiles_dir
 @p.project_dir
 @p.select
 @p.selector
 @p.inline
 @p.state
+@p.defer_state
 @p.deprecated_state
 @p.target
 @p.target_path
 @p.threads
 @p.vars
 @p.version_check
 @requires.postflight
@@ -364,14 +368,15 @@
 @p.profile
 @p.profiles_dir
 @p.project_dir
 @p.select
 @p.selector
 @p.inline
 @p.state
+@p.defer_state
 @p.deprecated_state
 @p.target
 @p.target_path
 @p.threads
 @p.vars
 @p.version_check
 @requires.postflight
@@ -393,25 +398,26 @@
     success = task.interpret_results(results)
     return results, success
 
 
 # dbt debug
 @cli.command("debug")
 @click.pass_context
+@p.debug_connection
 @p.config_dir
 @p.profile
 @p.profiles_dir_exists_false
 @p.project_dir
 @p.target
 @p.vars
 @p.version_check
 @requires.postflight
 @requires.preflight
 def debug(ctx, **kwargs):
-    """Test the database connection and show information for debugging purposes. Not to be confused with the --debug option which increases verbosity."""
+    """Show information on the current dbt environment and check dependencies, then test the database connection. Not to be confused with the --debug option which increases verbosity."""
 
     task = DebugTask(
         ctx.obj["flags"],
         None,
     )
 
     results = task.run()
@@ -472,14 +478,15 @@
 @p.profile
 @p.profiles_dir
 @p.project_dir
 @p.resource_type
 @p.raw_select
 @p.selector
 @p.state
+@p.defer_state
 @p.deprecated_state
 @p.target
 @p.target_path
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
@@ -541,14 +548,15 @@
 @p.full_refresh
 @p.profile
 @p.profiles_dir
 @p.project_dir
 @p.select
 @p.selector
 @p.state
+@p.defer_state
 @p.deprecated_state
 @p.target
 @p.target_path
 @p.threads
 @p.vars
 @p.version_check
 @requires.postflight
@@ -566,24 +574,55 @@
     )
 
     results = task.run()
     success = task.interpret_results(results)
     return results, success
 
 
+# dbt run
+@cli.command("retry")
+@click.pass_context
+@p.project_dir
+@p.profiles_dir
+@p.vars
+@p.profile
+@p.target
+@p.state
+@p.threads
+@p.fail_fast
+@requires.postflight
+@requires.preflight
+@requires.profile
+@requires.project
+@requires.runtime_config
+@requires.manifest
+def retry(ctx, **kwargs):
+    """Retry the nodes that failed in the previous run."""
+    task = RetryTask(
+        ctx.obj["flags"],
+        ctx.obj["runtime_config"],
+        ctx.obj["manifest"],
+    )
+
+    results = task.run()
+    success = task.interpret_results(results)
+    return results, success
+
+
 # dbt run operation
 @cli.command("run-operation")
 @click.pass_context
 @click.argument("macro")
 @p.args
 @p.profile
 @p.profiles_dir
 @p.project_dir
 @p.target
 @p.target_path
+@p.threads
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest
@@ -608,14 +647,15 @@
 @p.profile
 @p.profiles_dir
 @p.project_dir
 @p.select
 @p.selector
 @p.show
 @p.state
+@p.defer_state
 @p.deprecated_state
 @p.target
 @p.target_path
 @p.threads
 @p.vars
 @p.version_check
 @requires.postflight
@@ -646,14 +686,15 @@
 @p.deprecated_favor_state
 @p.profile
 @p.profiles_dir
 @p.project_dir
 @p.select
 @p.selector
 @p.state
+@p.defer_state
 @p.deprecated_state
 @p.target
 @p.target_path
 @p.threads
 @p.vars
 @requires.postflight
 @requires.preflight
@@ -688,14 +729,15 @@
 @p.output_path  # TODO: Is this ok to re-use?  We have three different output params, how much can we consolidate?
 @p.profile
 @p.profiles_dir
 @p.project_dir
 @p.select
 @p.selector
 @p.state
+@p.defer_state
 @p.deprecated_state
 @p.target
 @p.target_path
 @p.threads
 @p.vars
 @requires.postflight
 @requires.preflight
@@ -734,14 +776,15 @@
 @p.indirect_selection
 @p.profile
 @p.profiles_dir
 @p.project_dir
 @p.select
 @p.selector
 @p.state
+@p.defer_state
 @p.deprecated_state
 @p.store_failures
 @p.target
 @p.target_path
 @p.threads
 @p.vars
 @p.version_check
```

### Comparing `dbt-core-1.6.0b2/dbt/cli/option_types.py` & `dbt-core-1.6.0b3/dbt/cli/option_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from click import ParamType, Choice
 
-from dbt.config.utils import parse_cli_vars
-from dbt.exceptions import ValidationError
+from dbt.config.utils import parse_cli_yaml_string
+from dbt.exceptions import ValidationError, DbtValidationError, OptionNotYamlDictError
 
 from dbt.helper_types import WarnErrorOptions
 
 
 class YAML(ParamType):
     """The Click YAML type. Converts YAML strings into objects."""
 
     name = "YAML"
 
     def convert(self, value, param, ctx):
         # assume non-string values are a problem
         if not isinstance(value, str):
             self.fail(f"Cannot load YAML from type {type(value)}", param, ctx)
         try:
-            return parse_cli_vars(value)
-        except ValidationError:
+            param_option_name = param.opts[0] if param.opts else param.name
+            return parse_cli_yaml_string(value, param_option_name.strip("-"))
+        except (ValidationError, DbtValidationError, OptionNotYamlDictError):
             self.fail(f"String '{value}' is not valid YAML", param, ctx)
 
 
 class WarnErrorOptionsType(YAML):
     """The Click WarnErrorOptions type. Converts YAML strings into objects."""
 
     name = "WarnErrorOptionsType"
```

### Comparing `dbt-core-1.6.0b2/dbt/cli/options.py` & `dbt-core-1.6.0b3/dbt/cli/options.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/cli/params.py` & `dbt-core-1.6.0b3/dbt/cli/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,20 +422,33 @@
     default=False,
     is_flag=True,
 )
 
 state = click.option(
     "--state",
     envvar="DBT_STATE",
-    help="If set, use the given directory as the source for JSON files to compare with this project.",
+    help="Unless overridden, use this state directory for both state comparison and deferral.",
     type=click.Path(
         dir_okay=True,
         file_okay=False,
         readable=True,
-        resolve_path=True,
+        resolve_path=False,
+        path_type=Path,
+    ),
+)
+
+defer_state = click.option(
+    "--defer-state",
+    envvar="DBT_DEFER_STATE",
+    help="Override the state directory for deferral only.",
+    type=click.Path(
+        dir_okay=True,
+        file_okay=False,
+        readable=True,
+        resolve_path=False,
         path_type=Path,
     ),
 )
 
 deprecated_state = click.option(
     "--deprecated-state",
     envvar="DBT_ARTIFACT_STATE_PATH",
@@ -474,14 +487,21 @@
 target_path = click.option(
     "--target-path",
     envvar="DBT_TARGET_PATH",
     help="Configure the 'target-path'. Only applies this setting for the current run. Overrides the 'DBT_TARGET_PATH' if it is set.",
     type=click.Path(),
 )
 
+debug_connection = click.option(
+    "--connection",
+    envvar=None,
+    help="Test the connection to the target database independent of dependency checks.",
+    is_flag=True,
+)
+
 threads = click.option(
     "--threads",
     envvar=None,
     help="Specify number of threads to use while executing models. Overrides settings in profiles.yml.",
     default=None,
     type=click.INT,
 )
```

### Comparing `dbt-core-1.6.0b2/dbt/cli/requires.py` & `dbt-core-1.6.0b3/dbt/cli/requires.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
                     runtime_config,
                     write_perf_info=write_perf_info,
                     publications=ctx.obj.get("_publications"),
                 )
 
                 ctx.obj["manifest"] = manifest
                 if write and ctx.obj["flags"].write_json:
-                    write_manifest(manifest, ctx.obj["runtime_config"].target_path)
+                    write_manifest(manifest, ctx.obj["runtime_config"].project_target_path)
 
             return func(*args, **kwargs)
 
         return update_wrapper(wrapper, func)
 
     # if there are no args, the decorator was used without params @decorator
     # otherwise, the decorator was called with params @decorator(arg)
```

### Comparing `dbt-core-1.6.0b2/dbt/cli/resolvers.py` & `dbt-core-1.6.0b3/dbt/cli/resolvers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/cli/types.py` & `dbt-core-1.6.0b3/dbt/cli/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     RUN = "run"
     RUN_OPERATION = "run-operation"
     SEED = "seed"
     SHOW = "show"
     SNAPSHOT = "snapshot"
     SOURCE_FRESHNESS = "freshness"
     TEST = "test"
+    RETRY = "retry"
 
     @classmethod
     def from_str(cls, s: str) -> "Command":
         try:
             return cls(s)
         except ValueError:
             raise DbtInternalError(f"No value '{s}' exists in Command enum")
```

### Comparing `dbt-core-1.6.0b2/dbt/clients/_jinja_blocks.py` & `dbt-core-1.6.0b3/dbt/clients/_jinja_blocks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/clients/agate_helper.py` & `dbt-core-1.6.0b3/dbt/clients/agate_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/clients/git.py` & `dbt-core-1.6.0b3/dbt/clients/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/clients/jinja.py` & `dbt-core-1.6.0b3/dbt/clients/jinja.py`

 * *Files 1% similar despite different names*

```diff
@@ -561,38 +561,52 @@
 # performance note: Local benmcharking (so take it with a big grain of salt!)
 # on this indicates that it is is on average slightly slower than
 # checking two separate patterns, but the standard deviation is smaller with
 # one pattern. The time difference between the two was ~2 std deviations, which
 # is small enough that I've just chosen the more readable option.
 _HAS_RENDER_CHARS_PAT = re.compile(r"({[{%#]|[#}%]})")
 
+_render_cache: Dict[str, Any] = dict()
+
 
 def get_rendered(
     string: str,
     ctx: Dict[str, Any],
     node=None,
     capture_macros: bool = False,
     native: bool = False,
-) -> str:
+) -> Any:
     # performance optimization: if there are no jinja control characters in the
     # string, we can just return the input. Fall back to jinja if the type is
     # not a string or if native rendering is enabled (so '1' -> 1, etc...)
     # If this is desirable in the native env as well, we could handle the
     # native=True case by passing the input string to ast.literal_eval, like
     # the native renderer does.
-    if not native and isinstance(string, str) and _HAS_RENDER_CHARS_PAT.search(string) is None:
-        return string
+    has_render_chars = not isinstance(string, str) or _HAS_RENDER_CHARS_PAT.search(string)
+
+    if not has_render_chars:
+        if not native:
+            return string
+        elif string in _render_cache:
+            return _render_cache[string]
+
     template = get_template(
         string,
         ctx,
         node,
         capture_macros=capture_macros,
         native=native,
     )
-    return render_template(template, ctx, node)
+
+    rendered = render_template(template, ctx, node)
+
+    if not has_render_chars and native:
+        _render_cache[string] = rendered
+
+    return rendered
 
 
 def undefined_error(msg) -> NoReturn:
     raise jinja2.exceptions.UndefinedError(msg)
 
 
 def extract_toplevel_blocks(
```

### Comparing `dbt-core-1.6.0b2/dbt/clients/jinja_static.py` & `dbt-core-1.6.0b3/dbt/clients/jinja_static.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/clients/registry.py` & `dbt-core-1.6.0b3/dbt/clients/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/clients/system.py` & `dbt-core-1.6.0b3/dbt/clients/system.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/clients/yaml_helper.py` & `dbt-core-1.6.0b3/dbt/clients/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/compilation.py` & `dbt-core-1.6.0b3/dbt/compilation.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,15 +268,15 @@
 
 
 class Compiler:
     def __init__(self, config):
         self.config = config
 
     def initialize(self):
-        make_directory(self.config.target_path)
+        make_directory(self.config.project_target_path)
         make_directory(self.config.packages_install_path)
 
     # creates a ModelContext which is converted to
     # a dict for jinja rendering of SQL
     def _create_node_context(
         self,
         node: ManifestSQLNode,
@@ -508,15 +508,17 @@
             manifest.build_parent_and_child_maps()
             linker.add_test_edges(manifest)
 
             # Create another diagnostic summary, just as above, but this time
             # including the test edges.
             summaries["with_test_edges"] = linker.get_graph_summary(manifest)
 
-        with open(os.path.join(self.config.target_path, "graph_summary.json"), "w") as out_stream:
+        with open(
+            os.path.join(self.config.project_target_path, "graph_summary.json"), "w"
+        ) as out_stream:
             try:
                 out_stream.write(json.dumps(summaries))
             except Exception as e:  # This is non-essential information, so merely note failures.
                 fire_event(
                     Note(
                         msg=f"An error was encountered writing the graph summary information: {e}"
                     )
@@ -535,32 +537,31 @@
             stats = _generate_stats(manifest)
             print_compile_stats(stats)
 
         return Graph(linker.graph)
 
     def write_graph_file(self, linker: Linker, manifest: Manifest):
         filename = graph_file_name
-        graph_path = os.path.join(self.config.target_path, filename)
+        graph_path = os.path.join(self.config.project_target_path, filename)
         flags = get_flags()
         if flags.WRITE_JSON:
             linker.write_graph(graph_path, manifest)
 
     # writes the "compiled_code" into the target/compiled directory
     def _write_node(self, node: ManifestSQLNode) -> ManifestSQLNode:
         if not node.extra_ctes_injected or node.resource_type in (
             NodeType.Snapshot,
             NodeType.Seed,
         ):
             return node
         fire_event(WritingInjectedSQLForNode(node_info=get_node_info()))
 
         if node.compiled_code:
-            node.compiled_path = node.write_node(
-                self.config.target_path, "compiled", node.compiled_code
-            )
+            node.compiled_path = node.get_target_write_path(self.config.target_path, "compiled")
+            node.write_node(self.config.project_root, node.compiled_path, node.compiled_code)
         return node
 
     def compile_node(
         self,
         node: ManifestSQLNode,
         manifest: Manifest,
         extra_context: Optional[Dict[str, Any]] = None,
```

### Comparing `dbt-core-1.6.0b2/dbt/config/profile.py` & `dbt-core-1.6.0b3/dbt/config/profile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/config/project.py` & `dbt-core-1.6.0b3/dbt/config/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,18 +311,18 @@
                 )
                 raise DbtProjectError(
                     msg.format(deprecated_path=deprecated_path, expected_path=expected_path)
                 )
             # this field is no longer supported, but many projects may specify it with the default value
             # if so, let's only raise this deprecation warning if they set a custom value
             if not default_value or project_dict[deprecated_path] != default_value:
-                deprecations.warn(
-                    f"project-config-{deprecated_path}",
-                    deprecated_path=deprecated_path,
-                )
+                kwargs = {"deprecated_path": deprecated_path}
+                if expected_path:
+                    kwargs.update({"exp_path": expected_path})
+                deprecations.warn(f"project-config-{deprecated_path}", **kwargs)
 
     def create_project(self, rendered: RenderComponents) -> "Project":
         unrendered = RenderComponents(
             project_dict=self.project_dict,
             packages_dict=self.packages_dict,
             selectors_dict=self.selectors_dict,
         )
@@ -696,7 +696,12 @@
         return None
 
     def get_macro_search_order(self, macro_namespace: str):
         for dispatch_entry in self.dispatch:
             if dispatch_entry["macro_namespace"] == macro_namespace:
                 return dispatch_entry["search_order"]
         return None
+
+    @property
+    def project_target_path(self):
+        # If target_path is absolute, project_root will not be included
+        return os.path.join(self.project_root, self.target_path)
```

### Comparing `dbt-core-1.6.0b2/dbt/config/renderer.py` & `dbt-core-1.6.0b3/dbt/config/renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/config/runtime.py` & `dbt-core-1.6.0b3/dbt/config/runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,19 @@
         return cls.from_parts(
             project=project,
             profile=profile,
             args=args,
         )
 
     def get_metadata(self) -> ManifestMetadata:
-        return ManifestMetadata(project_id=self.hashed_name(), adapter_type=self.credentials.type)
+        return ManifestMetadata(
+            project_name=self.project_name,
+            project_id=self.hashed_name(),
+            adapter_type=self.credentials.type,
+        )
 
     def _get_v2_config_paths(
         self,
         config,
         path: FQNPath,
         paths: MutableSet[FQNPath],
     ) -> PathSet:
```

### Comparing `dbt-core-1.6.0b2/dbt/config/selectors.py` & `dbt-core-1.6.0b3/dbt/config/selectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from dbt.graph.selector_spec import SelectionCriteria
 
 MALFORMED_SELECTOR_ERROR = """\
 The selectors.yml file in this project is malformed. Please double check
 the contents of this file and fix any errors before retrying.
 
 You can find more information on the syntax for this file here:
-https://docs.getdbt.com/docs/package-management
+https://docs.getdbt.com/reference/node-selection/yaml-selectors
 
 Validator Error:
 {error}
 """
 
 
 class SelectorConfig(Dict[str, Dict[str, Union[SelectionSpec, bool]]]):
```

### Comparing `dbt-core-1.6.0b2/dbt/config/utils.py` & `dbt-core-1.6.0b3/dbt/config/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,10 +15,10 @@
     try:
         cli_vars = yaml_helper.load_yaml_text(var_string)
         var_type = type(cli_vars)
         if var_type is dict:
             return cli_vars
         else:
             raise OptionNotYamlDictError(var_type, cli_option_name)
-    except DbtValidationError:
+    except (DbtValidationError, OptionNotYamlDictError):
         fire_event(InvalidOptionYAML(option_name=cli_option_name))
         raise
```

### Comparing `dbt-core-1.6.0b2/dbt/context/base.py` & `dbt-core-1.6.0b3/dbt/context/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/context/configured.py` & `dbt-core-1.6.0b3/dbt/context/configured.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/context/context_config.py` & `dbt-core-1.6.0b3/dbt/context/context_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/context/docs.py` & `dbt-core-1.6.0b3/dbt/context/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/context/exceptions_jinja.py` & `dbt-core-1.6.0b3/dbt/context/exceptions_jinja.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     DuplicatePatchPathError,
     DuplicateResourceNameError,
     PropertyYMLError,
     NotImplementedError,
     RelationWrongTypeError,
     ContractError,
     ColumnTypeMissingError,
+    FailFastError,
 )
 
 
 def warn(msg, node=None):
     warn_or_error(JinjaLogWarning(msg=msg), node=node)
     return ""
 
@@ -103,14 +104,18 @@
     raise RelationWrongTypeError(relation, expected_type, model)
 
 
 def column_type_missing(column_names) -> NoReturn:
     raise ColumnTypeMissingError(column_names)
 
 
+def raise_fail_fast_error(msg, node=None) -> NoReturn:
+    raise FailFastError(msg, node=node)
+
+
 # Update this when a new function should be added to the
 # dbt context's `exceptions` key!
 CONTEXT_EXPORTS = {
     fn.__name__: fn
     for fn in [
         warn,
         missing_config,
@@ -127,14 +132,15 @@
         raise_duplicate_patch_name,
         raise_duplicate_resource_name,
         raise_invalid_property_yml_version,
         raise_not_implemented,
         relation_wrong_type,
         raise_contract_error,
         column_type_missing,
+        raise_fail_fast_error,
     ]
 }
 
 
 # wraps context based exceptions in node info
 def wrapper(model):
     def wrap(func):
```

### Comparing `dbt-core-1.6.0b2/dbt/context/macro_resolver.py` & `dbt-core-1.6.0b3/dbt/context/macro_resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/context/macros.py` & `dbt-core-1.6.0b3/dbt/context/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/context/manifest.py` & `dbt-core-1.6.0b3/dbt/context/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/context/providers.py` & `dbt-core-1.6.0b3/dbt/context/providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -829,15 +829,16 @@
         )
 
     @contextmember
     def write(self, payload: str) -> str:
         # macros/source defs aren't 'writeable'.
         if isinstance(self.model, (Macro, SourceDefinition)):
             raise MacrosSourcesUnWriteableError(node=self.model)
-        self.model.build_path = self.model.write_node(self.config.target_path, "run", payload)
+        self.model.build_path = self.model.get_target_write_path(self.config.target_path, "run")
+        self.model.write_node(self.config.project_root, self.model.build_path, payload)
         return ""
 
     @contextmember
     def render(self, string: str) -> str:
         return get_rendered(string, self._ctx, self.model)
 
     @contextmember
```

### Comparing `dbt-core-1.6.0b2/dbt/context/secret.py` & `dbt-core-1.6.0b3/dbt/context/secret.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/context/target.py` & `dbt-core-1.6.0b3/dbt/context/target.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/contracts/connection.py` & `dbt-core-1.6.0b3/dbt/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/contracts/files.py` & `dbt-core-1.6.0b3/dbt/contracts/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,14 +224,15 @@
     tests: Dict[str, Any] = field(default_factory=dict)
     sources: List[str] = field(default_factory=list)
     exposures: List[str] = field(default_factory=list)
     metrics: List[str] = field(default_factory=list)
     groups: List[str] = field(default_factory=list)
     # node patches contain models, seeds, snapshots, analyses
     ndp: List[str] = field(default_factory=list)
+    semantic_nodes: List[str] = field(default_factory=list)
     # any macro patches in this file by macro unique_id.
     mcp: Dict[str, str] = field(default_factory=dict)
     # any source patches in this file. The entries are package, name pairs
     # Patches are only against external sources. Sources can be
     # created too, but those are in 'sources'
     sop: List[SourceKey] = field(default_factory=list)
     env_vars: Dict[str, Any] = field(default_factory=dict)
```

### Comparing `dbt-core-1.6.0b2/dbt/contracts/graph/manifest.py` & `dbt-core-1.6.0b3/dbt/contracts/graph/manifest.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,28 +21,30 @@
 )
 from typing_extensions import Protocol
 from uuid import UUID
 
 from dbt.contracts.publication import ProjectDependencies, PublicationConfig, PublicModel
 
 from dbt.contracts.graph.nodes import (
-    Macro,
+    BaseNode,
     Documentation,
-    SourceDefinition,
-    GenericTestNode,
     Exposure,
-    Metric,
+    GenericTestNode,
+    GraphMemberNode,
     Group,
-    UnpatchedSourceDefinition,
+    Macro,
     ManifestNode,
-    GraphMemberNode,
-    ResultNode,
-    BaseNode,
     ManifestOrPublicNode,
+    Metric,
     ModelNode,
+    RelationalNode,
+    ResultNode,
+    SemanticModel,
+    SourceDefinition,
+    UnpatchedSourceDefinition,
 )
 from dbt.contracts.graph.unparsed import SourcePatch, NodeVersion, UnparsedVersion
 from dbt.contracts.graph.manifest_upgrade import upgrade_manifest_json
 from dbt.contracts.files import SourceFile, SchemaSourceFile, FileHash, AnySourceFile
 from dbt.contracts.util import BaseArtifactMetadata, SourceKey, ArtifactMixin, schema_version
 from dbt.dataclass_schema import dbtClassMixin
 from dbt.exceptions import (
@@ -56,14 +58,17 @@
 from dbt.events.functions import fire_event
 from dbt.events.types import MergedFromState, UnpinnedRefNewVersionAvailable
 from dbt.events.contextvars import get_node_info
 from dbt.node_types import NodeType
 from dbt.flags import get_flags, MP_CONTEXT
 from dbt import tracking
 import dbt.utils
+from dbt_semantic_interfaces.implementations.metric import PydanticMetric
+from dbt_semantic_interfaces.implementations.semantic_manifest import PydanticSemanticManifest
+from dbt_semantic_interfaces.implementations.semantic_model import PydanticSemanticModel
 
 NodeEdgeMap = Dict[str, List[str]]
 PackageName = str
 DocName = str
 RefName = str
 UniqueID = str
 
@@ -200,15 +205,15 @@
                 max_version: UnparsedVersion = max(
                     [
                         UnparsedVersion(v.version)
                         for v in manifest.nodes.values()
                         if v.name == node.name and v.version is not None
                     ]
                 )
-                assert node.latest_version  # for mypy, whenever i may find it
+                assert node.latest_version is not None  # for mypy, whenever i may find it
                 if max_version > UnparsedVersion(node.latest_version):
                     fire_event(
                         UnpinnedRefNewVersionAvailable(
                             node_info=get_node_info(),
                             ref_node_name=node.name,
                             ref_node_package=node.package_name,
                             ref_node_version=str(node.version),
@@ -364,18 +369,24 @@
 @dataclass
 class ManifestMetadata(BaseArtifactMetadata):
     """Metadata for the manifest."""
 
     dbt_schema_version: str = field(
         default_factory=lambda: str(WritableManifest.dbt_schema_version)
     )
+    project_name: Optional[str] = field(
+        default=None,
+        metadata={
+            "description": "Name of the root project",
+        },
+    )
     project_id: Optional[str] = field(
         default=None,
         metadata={
-            "description": "A unique identifier for the project",
+            "description": "A unique identifier for the project, hashed from the project name",
         },
     )
     user_id: Optional[UUID] = field(
         default=None,
         metadata={
             "description": "A unique identifier for the user",
         },
@@ -598,34 +609,44 @@
             root_project_name=root_project_name,
             filter=filter,
         )
 
         return candidates.last()
 
     def find_generate_macro_by_name(
-        self, component: str, root_project_name: str
+        self, component: str, root_project_name: str, imported_package: Optional[str] = None
     ) -> Optional[Macro]:
         """
-        The `generate_X_name` macros are similar to regular ones, but ignore
-        imported packages.
+        The default `generate_X_name` macros are similar to regular ones, but only
+        includes imported packages when searching for a package.
+        - if package is not provided:
             - if there is a `generate_{component}_name` macro in the root
               project, return it
             - return the `generate_{component}_name` macro from the 'dbt'
               internal project
+        - if package is provided
+            - return the `generate_{component}_name` macro from the imported
+              package, if one exists
         """
 
         def filter(candidate: MacroCandidate) -> bool:
-            return candidate.locality != Locality.Imported
+            if imported_package:
+                return (
+                    candidate.locality == Locality.Imported
+                    and imported_package == candidate.macro.package_name
+                )
+            else:
+                return candidate.locality != Locality.Imported
 
         candidates: CandidateList = self._find_macros_by_name(
             name=f"generate_{component}_name",
             root_project_name=root_project_name,
-            # filter out imported packages
             filter=filter,
         )
+
         return candidates.last()
 
     def _find_macros_by_name(
         self,
         name: str,
         root_project_name: str,
         filter: Optional[Callable[[MacroCandidate], bool]] = None,
@@ -685,14 +706,15 @@
     state_check: ManifestStateCheck = field(default_factory=ManifestStateCheck)
     source_patches: MutableMapping[SourceKey, SourcePatch] = field(default_factory=dict)
     disabled: MutableMapping[str, List[GraphMemberNode]] = field(default_factory=dict)
     env_vars: MutableMapping[str, str] = field(default_factory=dict)
     public_nodes: MutableMapping[str, PublicModel] = field(default_factory=dict)
     project_dependencies: Optional[ProjectDependencies] = None
     publications: MutableMapping[str, PublicationConfig] = field(default_factory=dict)
+    semantic_nodes: MutableMapping[str, SemanticModel] = field(default_factory=dict)
 
     _doc_lookup: Optional[DocLookup] = field(
         default=None, metadata={"serialize": lambda x: None, "deserialize": lambda x: None}
     )
     _source_lookup: Optional[SourceLookup] = field(
         default=None, metadata={"serialize": lambda x: None, "deserialize": lambda x: None}
     )
@@ -873,15 +895,15 @@
         )
         group_map = {group.name: [] for group in self.groups.values()}
         for node in groupable_nodes:
             if node.group is not None:
                 group_map[node.group].append(node.unique_id)
         self.group_map = group_map
 
-    def writable_manifest(self):
+    def writable_manifest(self) -> "WritableManifest":
         self.build_parent_and_child_maps()
         self.build_group_map()
         return WritableManifest(
             nodes=self.nodes,
             sources=self.sources,
             macros=self.macros,
             docs=self.docs,
@@ -891,14 +913,15 @@
             selectors=self.selectors,
             metadata=self.metadata,
             disabled=self.disabled,
             public_nodes=self.public_nodes,
             child_map=self.child_map,
             parent_map=self.parent_map,
             group_map=self.group_map,
+            semantic_nodes=self.semantic_nodes,
         )
 
     def write(self, path):
         self.writable_manifest().write(path)
 
     # Called in dbt.compilation.Linker.write_graph and
     # dbt.graph.queue.get and ._include_in_cost
@@ -961,14 +984,28 @@
 
     @property
     def analysis_lookup(self) -> AnalysisLookup:
         if self._analysis_lookup is None:
             self._analysis_lookup = AnalysisLookup(self)
         return self._analysis_lookup
 
+    @property
+    def pydantic_semantic_manifest(self) -> PydanticSemanticManifest:
+        pydantic_semantic_manifest = PydanticSemanticManifest(metrics=[], semantic_models=[])
+
+        for semantic_model in self.semantic_nodes.values():
+            pydantic_semantic_manifest.semantic_models.append(
+                PydanticSemanticModel.parse_obj(semantic_model.to_dict())
+            )
+
+        for metric in self.metrics.values():
+            pydantic_semantic_manifest.metrics.append(PydanticMetric.parse_obj(metric.to_dict()))
+
+        return pydantic_semantic_manifest
+
     def resolve_refs(
         self, source_node: GraphMemberNode, current_project: str
     ) -> List[MaybeNonSource]:
         resolved_refs: List[MaybeNonSource] = []
         for ref in source_node.refs:
             resolved = self.resolve_ref(
                 source_node,
@@ -1123,14 +1160,31 @@
         # now that we've deferred some nodes
         self.build_flat_graph()
 
         # log up to 5 items
         sample = list(islice(merged, 5))
         fire_event(MergedFromState(num_merged=len(merged), sample=sample))
 
+    # Called by CloneTask.defer_to_manifest
+    def add_from_artifact(
+        self,
+        other: "WritableManifest",
+    ) -> None:
+        """Update this manifest by *adding* information about each node's location
+        in the other manifest.
+
+        Only non-ephemeral refable nodes are examined.
+        """
+        refables = set(NodeType.refable())
+        for unique_id, node in other.nodes.items():
+            current = self.nodes.get(unique_id)
+            if current and (node.resource_type in refables and not node.is_ephemeral):
+                state_relation = RelationalNode(node.database, node.schema, node.alias)
+                self.nodes[unique_id] = current.replace(state_relation=state_relation)
+
     # Methods that were formerly in ParseResult
 
     def add_macro(self, source_file: SourceFile, macro: Macro):
         if macro.unique_id in self.macros:
             # detect that the macro exists and emit an error
             raise DuplicateMacroInPackageError(macro=macro, macro_mapping=self.macros)
 
@@ -1208,14 +1262,19 @@
             source_file.nodes.append(node.unique_id)
 
     def add_doc(self, source_file: SourceFile, doc: Documentation):
         _check_duplicates(doc, self.docs)
         self.docs[doc.unique_id] = doc
         source_file.docs.append(doc.unique_id)
 
+    def add_semantic_model(self, source_file: SchemaSourceFile, semantic_model: SemanticModel):
+        _check_duplicates(semantic_model, self.semantic_nodes)
+        self.semantic_nodes[semantic_model.unique_id] = semantic_model
+        source_file.semantic_nodes.append(semantic_model.unique_id)
+
     # end of methods formerly in ParseResult
 
     # Provide support for copy.deepcopy() - we just need to avoid the lock!
     # pickle and deepcopy use this. It returns a callable object used to
     # create the initial version of the object and a tuple of arguments
     # for the object, i.e. the Manifest.
     # The order of the arguments must match the order of the attributes
@@ -1307,14 +1366,17 @@
         metadata=dict(
             description="A mapping from group names to their nodes",
         )
     )
     public_nodes: Mapping[UniqueID, PublicModel] = field(
         metadata=dict(description=("The public models used in the dbt project"))
     )
+    semantic_nodes: Mapping[UniqueID, SemanticModel] = field(
+        metadata=dict(description=("The semantic models defined in the dbt project"))
+    )
     metadata: ManifestMetadata = field(
         metadata=dict(
             description="Metadata about the manifest",
         )
     )
 
     @classmethod
@@ -1328,16 +1390,17 @@
             ("manifest", 9),
         ]
 
     @classmethod
     def upgrade_schema_version(cls, data):
         """This overrides the "upgrade_schema_version" call in VersionedSchema (via
         ArtifactMixin) to modify the dictionary passed in from earlier versions of the manifest."""
-        if get_manifest_schema_version(data) <= 9:
-            data = upgrade_manifest_json(data)
+        manifest_schema_version = get_manifest_schema_version(data)
+        if manifest_schema_version <= 9:
+            data = upgrade_manifest_json(data, manifest_schema_version)
         return cls.from_dict(data)
 
     def __post_serialize__(self, dct):
         for unique_id, node in dct["nodes"].items():
             if "config_call_dict" in node:
                 del node["config_call_dict"]
             if "state_relation" in node:
```

### Comparing `dbt-core-1.6.0b2/dbt/contracts/graph/metrics.py` & `dbt-core-1.6.0b3/dbt/contracts/graph/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/contracts/graph/model_config.py` & `dbt-core-1.6.0b3/dbt/contracts/graph/model_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from dataclasses import field, Field, dataclass
 from enum import Enum
 from itertools import chain
 from typing import Any, List, Optional, Dict, Union, Type, TypeVar, Callable
+
 from dbt.dataclass_schema import (
     dbtClassMixin,
     ValidationError,
     register_pattern,
+    StrEnum,
 )
 from dbt.contracts.graph.unparsed import AdditionalPropertiesAllowed, Docs
 from dbt.contracts.graph.utils import validate_color
-from dbt.exceptions import DbtInternalError, CompilationError
 from dbt.contracts.util import Replaceable, list_str
+from dbt.exceptions import DbtInternalError, CompilationError
 from dbt import hooks
 from dbt.node_types import NodeType
 
 
 M = TypeVar("M", bound="Metadata")
 
 
@@ -185,14 +187,24 @@
 class Severity(str):
     pass
 
 
 register_pattern(Severity, insensitive_patterns("warn", "error"))
 
 
+class OnConfigurationChangeOption(StrEnum):
+    Apply = "apply"
+    Continue = "continue"
+    Fail = "fail"
+
+    @classmethod
+    def default(cls) -> "OnConfigurationChangeOption":
+        return cls.Apply
+
+
 @dataclass
 class ContractConfig(dbtClassMixin, Replaceable):
     enforced: bool = False
 
 
 @dataclass
 class Hook(dbtClassMixin, Replaceable):
@@ -283,19 +295,25 @@
         for key in chain(unrendered, other):
             if key not in seen:
                 seen.add(key)
                 if not cls.compare_key(unrendered, other, key):
                     return False
         return True
 
-    # This is used in 'add_config_call' to created the combined config_call_dict.
+    # This is used in 'add_config_call' to create the combined config_call_dict.
     # 'meta' moved here from node
     mergebehavior = {
         "append": ["pre-hook", "pre_hook", "post-hook", "post_hook", "tags"],
-        "update": ["quoting", "column_types", "meta", "docs", "contract"],
+        "update": [
+            "quoting",
+            "column_types",
+            "meta",
+            "docs",
+            "contract",
+        ],
         "dict_key_append": ["grants"],
     }
 
     @classmethod
     def _merge_dicts(cls, src: Dict[str, Any], data: Dict[str, Any]) -> Dict[str, Any]:
         """Find all the items in data that match a target_field on this class,
         and merge them with the data found in `src` for target_field, using the
@@ -441,14 +459,17 @@
         metadata=MergeBehavior.Update.meta(),
     )
     full_refresh: Optional[bool] = None
     # 'unique_key' doesn't use 'Optional' because typing.get_type_hints was
     # sometimes getting the Union order wrong, causing serialization failures.
     unique_key: Union[str, List[str], None] = None
     on_schema_change: Optional[str] = "ignore"
+    on_configuration_change: OnConfigurationChangeOption = field(
+        default_factory=OnConfigurationChangeOption.default
+    )
     grants: Dict[str, Any] = field(
         default_factory=dict, metadata=MergeBehavior.DictKeyAppend.meta()
     )
     packages: List[str] = field(
         default_factory=list,
         metadata=MergeBehavior.Append.meta(),
     )
```

### Comparing `dbt-core-1.6.0b2/dbt/contracts/graph/nodes.py` & `dbt-core-1.6.0b3/dbt/contracts/graph/nodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,39 +2,31 @@
 from datetime import datetime
 import time
 from dataclasses import dataclass, field
 from enum import Enum
 import hashlib
 
 from mashumaro.types import SerializableType
-from typing import (
-    Optional,
-    Union,
-    List,
-    Dict,
-    Any,
-    Sequence,
-    Tuple,
-    Iterator,
-)
+from typing import Optional, Union, List, Dict, Any, Sequence, Tuple, Iterator, Protocol
 
 from dbt.dataclass_schema import dbtClassMixin, ExtensibleDbtClassMixin
 
 from dbt.clients.system import write_file
 from dbt.contracts.files import FileHash
 from dbt.contracts.graph.unparsed import (
+    Dimension,
     Docs,
+    Entity,
     ExposureType,
     ExternalTable,
     FreshnessThreshold,
     HasYamlMetadata,
     MacroArgument,
     MaturityType,
-    MetricFilter,
-    MetricTime,
+    Measure,
     Owner,
     Quoting,
     TestDef,
     NodeVersion,
     UnparsedSourceDefinition,
     UnparsedSourceTableDefinition,
     UnparsedColumn,
@@ -47,31 +39,29 @@
     SeedExceedsLimitSamePath,
     SeedExceedsLimitAndPathChanged,
     SeedExceedsLimitChecksumChanged,
 )
 from dbt.events.contextvars import set_contextvars
 from dbt.flags import get_flags
 from dbt.node_types import ModelLanguage, NodeType, AccessType
+from dbt_semantic_interfaces.references import MeasureReference
+from dbt_semantic_interfaces.references import MetricReference as DSIMetricReference
+from dbt_semantic_interfaces.type_enums.metric_type import MetricType
+from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
 
 from .model_config import (
     NodeConfig,
     SeedConfig,
     TestConfig,
     SourceConfig,
     MetricConfig,
     ExposureConfig,
     EmptySnapshotConfig,
     SnapshotConfig,
 )
-import sys
-
-if sys.version_info >= (3, 8):
-    from typing import Protocol
-else:
-    from typing_extensions import Protocol
 
 
 # =====================================================================
 # This contains the classes for all of the nodes and node-like objects
 # in the manifest. In the "nodes" dictionary of the manifest we find
 # all of the objects in the ManifestNode union below. In addition the
 # manifest contains "macros", "sources", "metrics", "exposures", "docs",
@@ -189,14 +179,17 @@
         return True
 
 
 @dataclass
 class ColumnLevelConstraint(dbtClassMixin):
     type: ConstraintType
     name: Optional[str] = None
+    # expression is a user-provided field that will depend on the constraint type.
+    # It could be a predicate (check type), or a sequence sql keywords (e.g. unique type),
+    # so the vague naming of 'expression' is intended to capture this range.
     expression: Optional[str] = None
     warn_unenforced: bool = (
         True  # Warn if constraint cannot be enforced by platform but will be in DDL
     )
     warn_unsupported: bool = (
         True  # Warn if constraint is not supported by the platform and won't be in DDL
     )
@@ -253,14 +246,23 @@
     # 'in' on lists is O(n) so this is O(n^2) for # of macros
     def add_macro(self, value: str):
         if value not in self.macros:
             self.macros.append(value)
 
 
 @dataclass
+class RelationalNode(HasRelationMetadata):
+    alias: str
+
+    @property
+    def identifier(self):
+        return self.alias
+
+
+@dataclass
 class DependsOn(MacroDependsOn):
     nodes: List[str] = field(default_factory=list)
     public_nodes: List[str] = field(default_factory=list)
 
     def add_node(self, value: str):
         if value not in self.nodes:
             self.nodes.append(value)
@@ -341,25 +343,31 @@
     deferred: bool = False
     unrendered_config: Dict[str, Any] = field(default_factory=dict)
     created_at: float = field(default_factory=lambda: time.time())
     config_call_dict: Dict[str, Any] = field(default_factory=dict)
     relation_name: Optional[str] = None
     raw_code: str = ""
 
-    def write_node(self, target_path: str, subdirectory: str, payload: str):
+    def get_target_write_path(self, target_path: str, subdirectory: str):
+        # This is called for both the "compiled" subdirectory of "target" and the "run" subdirectory
         if os.path.basename(self.path) == os.path.basename(self.original_file_path):
             # One-to-one relationship of nodes to files.
             path = self.original_file_path
         else:
             #  Many-to-one relationship of nodes to files.
             path = os.path.join(self.original_file_path, self.path)
-        full_path = os.path.join(target_path, subdirectory, self.package_name, path)
+        target_write_path = os.path.join(target_path, subdirectory, self.package_name, path)
+        return target_write_path
 
-        write_file(full_path, payload)
-        return full_path
+    def write_node(self, project_root: str, compiled_path, compiled_code: str):
+        if os.path.isabs(compiled_path):
+            full_path = compiled_path
+        else:
+            full_path = os.path.join(project_root, compiled_path)
+        write_file(full_path, compiled_code)
 
     def _serialize(self):
         return self.to_dict()
 
     def __post_serialize__(self, dct):
         dct = super().__post_serialize__(dct)
         if "_event_status" in dct:
@@ -542,14 +550,38 @@
         return self.depends_on.public_nodes
 
     @property
     def depends_on_macros(self):
         return self.depends_on.macros
 
 
+@dataclass
+class FileSlice(dbtClassMixin, Replaceable):
+    """Provides file slice level context about what something was created from.
+
+    Implementation of the dbt-semantic-interfaces `FileSlice` protocol
+    """
+
+    filename: str
+    content: str
+    start_line_number: int
+    end_line_number: int
+
+
+@dataclass
+class SourceFileMetadata(dbtClassMixin, Replaceable):
+    """Provides file context about what something was created from.
+
+    Implementation of the dbt-semantic-interfaces `Metadata` protocol
+    """
+
+    repo_file_path: str
+    file_slice: FileSlice
+
+
 # ====================================
 # CompiledNode subclasses
 # ====================================
 
 
 @dataclass
 class AnalysisNode(CompiledNode):
@@ -1276,34 +1308,83 @@
 
 # ====================================
 # Metric node
 # ====================================
 
 
 @dataclass
+class WhereFilter(dbtClassMixin):
+    where_sql_template: str
+
+
+@dataclass
+class MetricInputMeasure(dbtClassMixin):
+    name: str
+    filter: Optional[WhereFilter] = None
+    alias: Optional[str] = None
+
+    def measure_reference(self) -> MeasureReference:
+        return MeasureReference(element_name=self.name)
+
+    def post_aggregation_measure_referenc(self) -> MeasureReference:
+        return MeasureReference(element_name=self.alias or self.name)
+
+
+@dataclass
+class MetricTimeWindow(dbtClassMixin):
+    count: int
+    granularity: TimeGranularity
+
+
+@dataclass
+class MetricInput(dbtClassMixin):
+    name: str
+    filter: Optional[WhereFilter] = None
+    alias: Optional[str] = None
+    offset_window: Optional[MetricTimeWindow] = None
+    offset_to_grain: Optional[TimeGranularity] = None
+
+    def as_reference(self) -> DSIMetricReference:
+        return DSIMetricReference(element_name=self.name)
+
+
+@dataclass
+class MetricTypeParams(dbtClassMixin):
+    measure: Optional[MetricInputMeasure] = None
+    measures: Optional[List[MetricInputMeasure]] = None
+    numerator: Optional[MetricInputMeasure] = None
+    denominator: Optional[MetricInputMeasure] = None
+    expr: Optional[str] = None
+    window: Optional[MetricTimeWindow] = None
+    grain_to_date: Optional[TimeGranularity] = None
+    metrics: Optional[List[MetricInput]] = None
+
+    def numerator_measure_reference(self) -> Optional[MeasureReference]:
+        return self.numerator.measure_reference() if self.numerator else None
+
+    def denominator_measure_reference(self) -> Optional[MeasureReference]:
+        return self.denominator.measure_reference() if self.denominator else None
+
+
+@dataclass
 class MetricReference(dbtClassMixin, Replaceable):
-    sql: Optional[Union[str, int]]
-    unique_id: Optional[str]
+    sql: Optional[Union[str, int]] = None
+    unique_id: Optional[str] = None
 
 
 @dataclass
 class Metric(GraphNode):
     name: str
     description: str
     label: str
-    calculation_method: str
-    expression: str
-    filters: List[MetricFilter]
-    time_grains: List[str]
-    dimensions: List[str]
+    type: MetricType
+    type_params: MetricTypeParams
+    filter: Optional[WhereFilter] = None
+    metadata: Optional[SourceFileMetadata] = None
     resource_type: NodeType = field(metadata={"restrict": [NodeType.Metric]})
-    timestamp: Optional[str] = None
-    window: Optional[MetricTime] = None
-    model: Optional[str] = None
-    model_unique_id: Optional[str] = None
     meta: Dict[str, Any] = field(default_factory=dict)
     tags: List[str] = field(default_factory=list)
     config: MetricConfig = field(default_factory=MetricConfig)
     unrendered_config: Dict[str, Any] = field(default_factory=dict)
     sources: List[List[str]] = field(default_factory=list)
     depends_on: DependsOn = field(default_factory=DependsOn)
     refs: List[RefArgs] = field(default_factory=list)
@@ -1319,67 +1400,72 @@
     def depends_on_public_nodes(self):
         return self.depends_on.public_nodes
 
     @property
     def search_name(self):
         return self.name
 
-    def same_model(self, old: "Metric") -> bool:
-        return self.model == old.model
+    @property
+    def input_measures(self) -> List[MetricInputMeasure]:
+        tp = self.type_params
+        res = tp.measures or []
+        if tp.measure:
+            res.append(tp.measure)
+        if tp.numerator:
+            res.append(tp.numerator)
+        if tp.denominator:
+            res.append(tp.denominator)
 
-    def same_window(self, old: "Metric") -> bool:
-        return self.window == old.window
+        return res
 
-    def same_dimensions(self, old: "Metric") -> bool:
-        return self.dimensions == old.dimensions
+    @property
+    def measure_references(self) -> List[MeasureReference]:
+        return [x.measure_reference() for x in self.input_measures]
 
-    def same_filters(self, old: "Metric") -> bool:
-        return self.filters == old.filters
+    @property
+    def input_metrics(self) -> List[MetricInput]:
+        return self.type_params.metrics or []
 
     def same_description(self, old: "Metric") -> bool:
         return self.description == old.description
 
     def same_label(self, old: "Metric") -> bool:
         return self.label == old.label
 
-    def same_calculation_method(self, old: "Metric") -> bool:
-        return self.calculation_method == old.calculation_method
-
-    def same_expression(self, old: "Metric") -> bool:
-        return self.expression == old.expression
-
-    def same_timestamp(self, old: "Metric") -> bool:
-        return self.timestamp == old.timestamp
-
-    def same_time_grains(self, old: "Metric") -> bool:
-        return self.time_grains == old.time_grains
-
     def same_config(self, old: "Metric") -> bool:
         return self.config.same_contents(
             self.unrendered_config,
             old.unrendered_config,
         )
 
+    def same_filter(self, old: "Metric") -> bool:
+        return True  # TODO
+
+    def same_metadata(self, old: "Metric") -> bool:
+        return True  # TODO
+
+    def same_type(self, old: "Metric") -> bool:
+        return self.type == old.type
+
+    def same_type_params(self, old: "Metric") -> bool:
+        return True  # TODO
+
     def same_contents(self, old: Optional["Metric"]) -> bool:
         # existing when it didn't before is a change!
         # metadata/tags changes are not "changes"
         if old is None:
             return True
 
         return (
-            self.same_model(old)
-            and self.same_window(old)
-            and self.same_dimensions(old)
-            and self.same_filters(old)
+            self.same_filter(old)
+            and self.same_metadata(old)
+            and self.same_type(old)
+            and self.same_type_params(old)
             and self.same_description(old)
             and self.same_label(old)
-            and self.same_calculation_method(old)
-            and self.same_expression(old)
-            and self.same_timestamp(old)
-            and self.same_time_grains(old)
             and self.same_config(old)
             and True
         )
 
 
 # ====================================
 # Group node
@@ -1390,14 +1476,36 @@
 class Group(BaseNode):
     name: str
     owner: Owner
     resource_type: NodeType = field(metadata={"restrict": [NodeType.Group]})
 
 
 # ====================================
+# SemanticModel and related classes
+# ====================================
+
+
+@dataclass
+class NodeRelation(dbtClassMixin):
+    alias: str
+    schema_name: str  # TODO: Could this be called simply "schema" so we could reuse StateRelation?
+    database: Optional[str] = None
+
+
+@dataclass
+class SemanticModel(GraphNode):
+    description: Optional[str]
+    model: str
+    node_relation: Optional[NodeRelation]
+    entities: Sequence[Entity]
+    measures: Sequence[Measure]
+    dimensions: Sequence[Dimension]
+
+
+# ====================================
 # Patches
 # ====================================
 
 
 @dataclass
 class ParsedPatch(HasYamlMetadata, Replaceable):
     name: str
```

### Comparing `dbt-core-1.6.0b2/dbt/contracts/graph/unparsed.py` & `dbt-core-1.6.0b3/dbt/contracts/graph/unparsed.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from dbt import deprecations
 from dbt.node_types import NodeType
 from dbt.contracts.util import (
     AdditionalPropertiesMixin,
     Mergeable,
     Replaceable,
 )
-from dbt.contracts.graph.manifest_upgrade import rename_metric_attr
 
 # trigger the PathEncoder
 import dbt.helper_types  # noqa:F401
 from dbt.exceptions import CompilationError, ParsingError, DbtInternalError
 
 from dbt.dataclass_schema import dbtClassMixin, StrEnum, ExtensibleDbtClassMixin, ValidationError
 
@@ -590,33 +589,56 @@
     period: Optional[MetricTimePeriod] = None
 
     def __bool__(self):
         return self.count is not None and self.period is not None
 
 
 @dataclass
-class UnparsedMetric(dbtClassMixin, Replaceable):
+class UnparsedMetricInputMeasure(dbtClassMixin):
+    name: str
+    filter: Optional[str] = None
+    alias: Optional[str] = None
+
+
+@dataclass
+class UnparsedMetricInput(dbtClassMixin):
+    name: str
+    filter: Optional[str] = None
+    alias: Optional[str] = None
+    offset_window: Optional[str] = None
+    offset_to_grain: Optional[str] = None  # str is really a TimeGranularity Enum
+
+
+@dataclass
+class UnparsedMetricTypeParams(dbtClassMixin):
+    measure: Optional[Union[UnparsedMetricInputMeasure, str]] = None
+    measures: Optional[List[Union[UnparsedMetricInputMeasure, str]]] = None
+    numerator: Optional[Union[UnparsedMetricInputMeasure, str]] = None
+    denominator: Optional[Union[UnparsedMetricInputMeasure, str]] = None
+    expr: Optional[str] = None
+    window: Optional[str] = None
+    grain_to_date: Optional[str] = None  # str is really a TimeGranularity Enum
+    metrics: Optional[List[Union[UnparsedMetricInput, str]]] = None
+
+
+@dataclass
+class UnparsedMetric(dbtClassMixin):
     name: str
     label: str
-    calculation_method: str
-    expression: str
+    type: str
+    type_params: UnparsedMetricTypeParams
     description: str = ""
-    timestamp: Optional[str] = None
-    time_grains: List[str] = field(default_factory=list)
-    dimensions: List[str] = field(default_factory=list)
-    window: Optional[MetricTime] = None
-    model: Optional[str] = None
-    filters: List[MetricFilter] = field(default_factory=list)
+    filter: Optional[str] = None
+    # metadata: Optional[Unparsedetadata] = None # TODO
     meta: Dict[str, Any] = field(default_factory=dict)
     tags: List[str] = field(default_factory=list)
     config: Dict[str, Any] = field(default_factory=dict)
 
     @classmethod
     def validate(cls, data):
-        data = rename_metric_attr(data, raise_deprecation_warning=True)
         super(UnparsedMetric, cls).validate(data)
         if "name" in data:
             errors = []
             if " " in data["name"]:
                 errors.append("cannot contain spaces")
             # This handles failing queries due to too long metric names.
             # It only occurs in BigQuery and Snowflake (Postgres/Redshift truncate)
@@ -628,43 +650,81 @@
                 errors.append("must contain only letters, numbers and underscores")
 
             if errors:
                 raise ParsingError(
                     f"The metric name '{data['name']}' is invalid.  It {', '.join(e for e in errors)}"
                 )
 
-        if data.get("timestamp") is None and data.get("time_grains") is not None:
-            raise ValidationError(
-                f"The metric '{data['name']} has time_grains defined but is missing a timestamp dimension."
-            )
-
-        if data.get("timestamp") is None and data.get("window") is not None:
-            raise ValidationError(
-                f"The metric '{data['name']} has a window defined but is missing a timestamp dimension."
-            )
-
-        if data.get("model") is None and data.get("calculation_method") != "derived":
-            raise ValidationError("Non-derived metrics require a 'model' property")
-
-        if data.get("model") is not None and data.get("calculation_method") == "derived":
-            raise ValidationError("Derived metrics cannot have a 'model' property")
-
 
 @dataclass
 class UnparsedGroup(dbtClassMixin, Replaceable):
     name: str
     owner: Owner
 
     @classmethod
     def validate(cls, data):
         super(UnparsedGroup, cls).validate(data)
         if data["owner"].get("name") is None and data["owner"].get("email") is None:
             raise ValidationError("Group owner must have at least one of 'name' or 'email'.")
 
 
+#
+# semantic interfaces unparsed objects
+#
+
+
+@dataclass
+class Entity(dbtClassMixin):
+    name: str
+    type: str  # actually an enum
+    description: Optional[str] = None
+    role: Optional[str] = None
+    expr: Optional[str] = None
+
+
+@dataclass
+class MeasureAggregationParameters(dbtClassMixin):
+    percentile: Optional[float] = None
+    use_discrete_percentile: bool = False
+    use_approximate_percentile: bool = False
+
+
+@dataclass
+class Measure(dbtClassMixin):
+    name: str
+    agg: str  # actually an enum
+    description: Optional[str] = None
+    create_metric: Optional[bool] = None
+    expr: Optional[str] = None
+    agg_params: Optional[MeasureAggregationParameters] = None
+    non_additive_dimension: Optional[Dict[str, Any]] = None
+    agg_time_dimension: Optional[str] = None
+
+
+@dataclass
+class Dimension(dbtClassMixin):
+    name: str
+    type: str  # actually an enum
+    description: Optional[str] = None
+    is_partition: Optional[bool] = False
+    type_params: Optional[Dict[str, Any]] = None
+    expr: Optional[str] = None
+    # TODO metadata: Optional[Metadata] (this would actually be the YML for the dimension)
+
+
+@dataclass
+class UnparsedSemanticModel(dbtClassMixin):
+    name: str
+    description: Optional[str]
+    model: str  # looks like "ref(...)"
+    entities: List[Entity] = field(default_factory=list)
+    measures: List[Measure] = field(default_factory=list)
+    dimensions: List[Dimension] = field(default_factory=list)
+
+
 def normalize_date(d: Optional[datetime.date]) -> Optional[datetime.datetime]:
     """Convert date to datetime (at midnight), and add local time zone if naive"""
     if d is None:
         return None
 
     # convert date to datetime
     dt = d if type(d) == datetime.datetime else datetime.datetime(d.year, d.month, d.day)
```

### Comparing `dbt-core-1.6.0b2/dbt/contracts/graph/utils.py` & `dbt-core-1.6.0b3/dbt/contracts/graph/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/contracts/project.py` & `dbt-core-1.6.0b3/dbt/contracts/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/contracts/publication.py` & `dbt-core-1.6.0b3/dbt/contracts/publication.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,14 @@
 class PublicationMandatory:
     project_name: str
 
 
 @dataclass
 @schema_version("publication", 1)
 class PublicationArtifact(ArtifactMixin, PublicationMandatory):
-    """This represents the <project_name>_publication.json artifact"""
-
     public_models: Dict[str, PublicModel] = field(default_factory=dict)
     metadata: PublicationMetadata = field(default_factory=PublicationMetadata)
     # list of project name strings
     dependencies: List[str] = field(default_factory=list)
 
 
 @dataclass
```

### Comparing `dbt-core-1.6.0b2/dbt/contracts/relation.py` & `dbt-core-1.6.0b3/dbt/contracts/relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from dbt.utils import deep_merge
 
 
 class RelationType(StrEnum):
     Table = "table"
     View = "view"
     CTE = "cte"
-    MaterializedView = "materializedview"
+    MaterializedView = "materialized_view"
     External = "external"
 
 
 class ComponentName(StrEnum):
     Database = "database"
     Schema = "schema"
     Identifier = "identifier"
```

### Comparing `dbt-core-1.6.0b2/dbt/contracts/results.py` & `dbt-core-1.6.0b3/dbt/contracts/results.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/contracts/selection.py` & `dbt-core-1.6.0b3/dbt/contracts/selection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/contracts/sql.py` & `dbt-core-1.6.0b3/dbt/contracts/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/contracts/util.py` & `dbt-core-1.6.0b3/dbt/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/dataclass_schema.py` & `dbt-core-1.6.0b3/dbt/dataclass_schema.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/deprecations.py` & `dbt-core-1.6.0b3/dbt/deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/deps/base.py` & `dbt-core-1.6.0b3/dbt/deps/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/deps/git.py` & `dbt-core-1.6.0b3/dbt/deps/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/deps/local.py` & `dbt-core-1.6.0b3/dbt/deps/local.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/deps/registry.py` & `dbt-core-1.6.0b3/dbt/deps/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/deps/resolver.py` & `dbt-core-1.6.0b3/dbt/deps/resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/deps/tarball.py` & `dbt-core-1.6.0b3/dbt/deps/tarball.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/docs/source/_ext/dbt_click.py` & `dbt-core-1.6.0b3/dbt/docs/source/_ext/dbt_click.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/docs/source/conf.py` & `dbt-core-1.6.0b3/dbt/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/events/adapter_endpoint.py` & `dbt-core-1.6.0b3/dbt/events/adapter_endpoint.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/events/base_types.py` & `dbt-core-1.6.0b3/dbt/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/events/contextvars.py` & `dbt-core-1.6.0b3/dbt/events/contextvars.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/events/eventmgr.py` & `dbt-core-1.6.0b3/dbt/events/eventmgr.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/events/format.py` & `dbt-core-1.6.0b3/dbt/events/format.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/events/functions.py` & `dbt-core-1.6.0b3/dbt/events/functions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/events/helpers.py` & `dbt-core-1.6.0b3/dbt/events/helpers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/events/types.py` & `dbt-core-1.6.0b3/dbt/events/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,27 +277,27 @@
 
 class ConfigSourcePathDeprecation(WarnLevel):
     def code(self):
         return "D003"
 
     def message(self):
         description = (
-            f"The `{self.deprecated_path}` config has been renamed to `{self.exp_path}`."
+            f"The `{self.deprecated_path}` config has been renamed to `{self.exp_path}`. "
             "Please update your `dbt_project.yml` configuration to reflect this change."
         )
         return line_wrap_message(warning_tag(f"Deprecated functionality\n\n{description}"))
 
 
 class ConfigDataPathDeprecation(WarnLevel):
     def code(self):
         return "D004"
 
     def message(self):
         description = (
-            f"The `{self.deprecated_path}` config has been renamed to `{self.exp_path}`."
+            f"The `{self.deprecated_path}` config has been renamed to `{self.exp_path}`. "
             "Please update your `dbt_project.yml` configuration to reflect this change."
         )
         return line_wrap_message(warning_tag(f"Deprecated functionality\n\n{description}"))
 
 
 class AdapterDeprecationWarning(WarnLevel):
     def code(self):
@@ -1199,14 +1199,27 @@
                 f"v='{self.ref_model_latest_version}') }}}}."
             )
             msg = msg + coda
 
         return msg
 
 
+class UnsupportedConstraintMaterialization(WarnLevel):
+    def code(self):
+        return "I068"
+
+    def message(self) -> str:
+        msg = (
+            f"Constraint types are not supported for {self.materialized} materializations and will "
+            "be ignored.  Set 'warn_unsupported: false' on this constraint to ignore this warning."
+        )
+
+        return line_wrap_message(warning_tag(msg))
+
+
 # =======================================================
 # M - Deps generation
 # =======================================================
 
 
 class GitSparseCheckoutSubdirectory(DebugLevel):
     def code(self):
```

### Comparing `dbt-core-1.6.0b2/dbt/events/types_pb2.py` & `dbt-core-1.6.0b3/dbt/events/types_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0btypes.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x91\x02\n\tEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x05\x65xtra\x18\t \x03(\x0b\x32!.proto_types.EventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x7f\n\rTimingInfoMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"V\n\x0cNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x91\x02\n\x08NodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\rnode_relation\x18\n \x01(\x0b\x32\x19.proto_types.NodeRelation\"\xd1\x01\n\x0cRunResultMsg\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x0btiming_info\x18\x03 \x03(\x0b\x32\x1a.proto_types.TimingInfoMsg\x12\x0e\n\x06thread\x18\x04 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x31\n\x10\x61\x64\x61pter_response\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"G\n\x0fReferenceKeyMsg\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\"6\n\x0eGenericMessage\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\"9\n\x11MainReportVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0blog_version\x18\x02 \x01(\x05\"j\n\x14MainReportVersionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.MainReportVersion\"r\n\x0eMainReportArgs\x12\x33\n\x04\x61rgs\x18\x01 \x03(\x0b\x32%.proto_types.MainReportArgs.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11MainReportArgsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainReportArgs\"+\n\x15MainTrackingUserState\x12\x12\n\nuser_state\x18\x01 \x01(\t\"r\n\x18MainTrackingUserStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainTrackingUserState\"5\n\x0fMergedFromState\x12\x12\n\nnum_merged\x18\x01 \x01(\x05\x12\x0e\n\x06sample\x18\x02 \x03(\t\"f\n\x12MergedFromStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.MergedFromState\"A\n\x14MissingProfileTarget\x12\x14\n\x0cprofile_name\x18\x01 \x01(\t\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\"p\n\x17MissingProfileTargetMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MissingProfileTarget\"(\n\x11InvalidOptionYAML\x12\x13\n\x0boption_name\x18\x01 \x01(\t\"j\n\x14InvalidOptionYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.InvalidOptionYAML\"!\n\x12LogDbtProjectError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15LogDbtProjectErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProjectError\"3\n\x12LogDbtProfileError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08profiles\x18\x02 \x03(\t\"l\n\x15LogDbtProfileErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProfileError\"!\n\x12StarterProjectPath\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"l\n\x15StarterProjectPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StarterProjectPath\"$\n\x15\x43onfigFolderDirectory\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"r\n\x18\x43onfigFolderDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConfigFolderDirectory\"\'\n\x14NoSampleProfileFound\x12\x0f\n\x07\x61\x64\x61pter\x18\x01 \x01(\t\"p\n\x17NoSampleProfileFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NoSampleProfileFound\"6\n\x18ProfileWrittenWithSample\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"x\n\x1bProfileWrittenWithSampleMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProfileWrittenWithSample\"B\n$ProfileWrittenWithTargetTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x90\x01\n\'ProfileWrittenWithTargetTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.ProfileWrittenWithTargetTemplateYAML\"C\n%ProfileWrittenWithProjectTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x92\x01\n(ProfileWrittenWithProjectTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.ProfileWrittenWithProjectTemplateYAML\"\x12\n\x10SettingUpProfile\"h\n\x13SettingUpProfileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SettingUpProfile\"\x1c\n\x1aInvalidProfileTemplateYAML\"|\n\x1dInvalidProfileTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.InvalidProfileTemplateYAML\"(\n\x18ProjectNameAlreadyExists\x12\x0c\n\x04name\x18\x01 \x01(\t\"x\n\x1bProjectNameAlreadyExistsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProjectNameAlreadyExists\"K\n\x0eProjectCreated\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocs_url\x18\x02 \x01(\t\x12\x11\n\tslack_url\x18\x03 \x01(\t\"d\n\x11ProjectCreatedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ProjectCreated\"@\n\x1aPackageRedirectDeprecation\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1dPackageRedirectDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PackageRedirectDeprecation\"\x1f\n\x1dPackageInstallPathDeprecation\"\x82\x01\n PackageInstallPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.PackageInstallPathDeprecation\"H\n\x1b\x43onfigSourcePathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"~\n\x1e\x43onfigSourcePathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigSourcePathDeprecation\"F\n\x19\x43onfigDataPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"z\n\x1c\x43onfigDataPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConfigDataPathDeprecation\"?\n\x19\x41\x64\x61pterDeprecationWarning\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"z\n\x1c\x41\x64\x61pterDeprecationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.AdapterDeprecationWarning\".\n\x17MetricAttributesRenamed\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\"v\n\x1aMetricAttributesRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.MetricAttributesRenamed\"+\n\x17\x45xposureNameDeprecation\x12\x10\n\x08\x65xposure\x18\x01 \x01(\t\"v\n\x1a\x45xposureNameDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.ExposureNameDeprecation\"^\n\x13InternalDeprecation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x18\n\x10suggested_action\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"n\n\x16InternalDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.InternalDeprecation\"@\n\x1a\x45nvironmentVariableRenamed\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1d\x45nvironmentVariableRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.EnvironmentVariableRenamed\"3\n\x18\x43onfigLogPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"x\n\x1b\x43onfigLogPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ConfigLogPathDeprecation\"6\n\x1b\x43onfigTargetPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"~\n\x1e\x43onfigTargetPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigTargetPathDeprecation\"!\n\x1f\x43ollectFreshnessReturnSignature\"\x86\x01\n\"CollectFreshnessReturnSignatureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.CollectFreshnessReturnSignature\"\x87\x01\n\x11\x41\x64\x61pterEventDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"j\n\x14\x41\x64\x61pterEventDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventDebug\"\x86\x01\n\x10\x41\x64\x61pterEventInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"h\n\x13\x41\x64\x61pterEventInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.AdapterEventInfo\"\x89\x01\n\x13\x41\x64\x61pterEventWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"n\n\x16\x41\x64\x61pterEventWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.AdapterEventWarning\"\x99\x01\n\x11\x41\x64\x61pterEventError\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x10\n\x08\x65xc_info\x18\x05 \x01(\t\"j\n\x14\x41\x64\x61pterEventErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventError\"_\n\rNewConnection\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"b\n\x10NewConnectionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NewConnection\"=\n\x10\x43onnectionReused\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x16\n\x0eorig_conn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionReusedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionReused\"0\n\x1b\x43onnectionLeftOpenInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"~\n\x1e\x43onnectionLeftOpenInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConnectionLeftOpenInCleanup\".\n\x19\x43onnectionClosedInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"z\n\x1c\x43onnectionClosedInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConnectionClosedInCleanup\"_\n\x0eRollbackFailed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"d\n\x11RollbackFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RollbackFailed\"O\n\x10\x43onnectionClosed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionClosedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionClosed\"Q\n\x12\x43onnectionLeftOpen\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"l\n\x15\x43onnectionLeftOpenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ConnectionLeftOpen\"G\n\x08Rollback\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"X\n\x0bRollbackMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.Rollback\"@\n\tCacheMiss\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\"Z\n\x0c\x43\x61\x63heMissMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.CacheMiss\"b\n\rListRelations\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12/\n\trelations\x18\x03 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10ListRelationsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ListRelations\"`\n\x0e\x43onnectionUsed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"d\n\x11\x43onnectionUsedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ConnectionUsed\"T\n\x08SQLQuery\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x0b\n\x03sql\x18\x03 \x01(\t\"X\n\x0bSQLQueryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.SQLQuery\"[\n\x0eSQLQueryStatus\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x03 \x01(\x02\"d\n\x11SQLQueryStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SQLQueryStatus\"H\n\tSQLCommit\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"Z\n\x0cSQLCommitMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.SQLCommit\"a\n\rColTypeChange\x12\x11\n\torig_type\x18\x01 \x01(\t\x12\x10\n\x08new_type\x18\x02 \x01(\t\x12+\n\x05table\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10\x43olTypeChangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ColTypeChange\"@\n\x0eSchemaCreation\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"d\n\x11SchemaCreationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SchemaCreation\"<\n\nSchemaDrop\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"\\\n\rSchemaDropMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SchemaDrop\"\xde\x01\n\x0b\x43\x61\x63heAction\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\t\x12-\n\x07ref_key\x18\x02 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_2\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_3\x18\x04 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12.\n\x08ref_list\x18\x05 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"^\n\x0e\x43\x61\x63heActionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.CacheAction\"\x98\x01\n\x0e\x43\x61\x63heDumpGraph\x12\x33\n\x04\x64ump\x18\x01 \x03(\x0b\x32%.proto_types.CacheDumpGraph.DumpEntry\x12\x14\n\x0c\x62\x65\x66ore_after\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x1a+\n\tDumpEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11\x43\x61\x63heDumpGraphMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CacheDumpGraph\"!\n\x12\x41\x64\x61pterImportError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15\x41\x64\x61pterImportErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.AdapterImportError\"#\n\x0fPluginLoadError\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"f\n\x12PluginLoadErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.PluginLoadError\"Z\n\x14NewConnectionOpening\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x18\n\x10\x63onnection_state\x18\x02 \x01(\t\"p\n\x17NewConnectionOpeningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NewConnectionOpening\"8\n\rCodeExecution\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x14\n\x0c\x63ode_content\x18\x02 \x01(\t\"b\n\x10\x43odeExecutionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.CodeExecution\"6\n\x13\x43odeExecutionStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x02 \x01(\x02\"n\n\x16\x43odeExecutionStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.CodeExecutionStatus\"%\n\x16\x43\x61talogGenerationError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"t\n\x19\x43\x61talogGenerationErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.CatalogGenerationError\"-\n\x13WriteCatalogFailure\x12\x16\n\x0enum_exceptions\x18\x01 \x01(\x05\"n\n\x16WriteCatalogFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.WriteCatalogFailure\"\x1e\n\x0e\x43\x61talogWritten\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43\x61talogWrittenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CatalogWritten\"\x14\n\x12\x43\x61nnotGenerateDocs\"l\n\x15\x43\x61nnotGenerateDocsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.CannotGenerateDocs\"\x11\n\x0f\x42uildingCatalog\"f\n\x12\x42uildingCatalogMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.BuildingCatalog\"-\n\x18\x44\x61tabaseErrorRunningHook\x12\x11\n\thook_type\x18\x01 \x01(\t\"x\n\x1b\x44\x61tabaseErrorRunningHookMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DatabaseErrorRunningHook\"4\n\x0cHooksRunning\x12\x11\n\tnum_hooks\x18\x01 \x01(\x05\x12\x11\n\thook_type\x18\x02 \x01(\t\"`\n\x0fHooksRunningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.HooksRunning\"T\n\x14\x46inishedRunningStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\x12\x11\n\texecution\x18\x02 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x03 \x01(\x02\"p\n\x17\x46inishedRunningStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.FinishedRunningStats\"<\n\x15\x43onstraintNotEnforced\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"r\n\x18\x43onstraintNotEnforcedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConstraintNotEnforced\"=\n\x16\x43onstraintNotSupported\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"t\n\x19\x43onstraintNotSupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.ConstraintNotSupported\"7\n\x12InputFileDiffError\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"l\n\x15InputFileDiffErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InputFileDiffError\"t\n\x1aPublicationArtifactChanged\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\t\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"|\n\x1dPublicationArtifactChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PublicationArtifactChanged\"?\n\x14InvalidValueForField\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_value\x18\x02 \x01(\t\"p\n\x17InvalidValueForFieldMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.InvalidValueForField\"Q\n\x11ValidationWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12\x11\n\tnode_name\x18\x03 \x01(\t\"j\n\x14ValidationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ValidationWarning\"!\n\x11ParsePerfInfoPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"j\n\x14ParsePerfInfoPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ParsePerfInfoPath\"1\n!PartialParsingErrorProcessingFile\x12\x0c\n\x04\x66ile\x18\x01 \x01(\t\"\x8a\x01\n$PartialParsingErrorProcessingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.PartialParsingErrorProcessingFile\"\x86\x01\n\x13PartialParsingError\x12?\n\x08\x65xc_info\x18\x01 \x03(\x0b\x32-.proto_types.PartialParsingError.ExcInfoEntry\x1a.\n\x0c\x45xcInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"n\n\x16PartialParsingErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.PartialParsingError\"\x1b\n\x19PartialParsingSkipParsing\"z\n\x1cPartialParsingSkipParsingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.PartialParsingSkipParsing\"&\n\x14UnableToPartialParse\x12\x0e\n\x06reason\x18\x01 \x01(\t\"p\n\x17UnableToPartialParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.UnableToPartialParse\"f\n\x12StateCheckVarsHash\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\x12\x0c\n\x04vars\x18\x02 \x01(\t\x12\x0f\n\x07profile\x18\x03 \x01(\t\x12\x0e\n\x06target\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\"l\n\x15StateCheckVarsHashMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StateCheckVarsHash\"\x1a\n\x18PartialParsingNotEnabled\"x\n\x1bPartialParsingNotEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.PartialParsingNotEnabled\"C\n\x14ParsedFileLoadFailed\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"p\n\x17ParsedFileLoadFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParsedFileLoadFailed\"H\n\x15PartialParsingEnabled\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x05\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hanged\x18\x03 \x01(\x05\"r\n\x18PartialParsingEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.PartialParsingEnabled\"8\n\x12PartialParsingFile\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\"l\n\x15PartialParsingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.PartialParsingFile\"\xaf\x01\n\x1fInvalidDisabledTargetInTestNode\x12\x1b\n\x13resource_type_title\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1a\n\x12original_file_path\x18\x03 \x01(\t\x12\x13\n\x0btarget_kind\x18\x04 \x01(\t\x12\x13\n\x0btarget_name\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\"\x86\x01\n\"InvalidDisabledTargetInTestNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.InvalidDisabledTargetInTestNode\"7\n\x18UnusedResourceConfigPath\x12\x1b\n\x13unused_config_paths\x18\x01 \x03(\t\"x\n\x1bUnusedResourceConfigPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.UnusedResourceConfigPath\"3\n\rSeedIncreased\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"b\n\x10SeedIncreasedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.SeedIncreased\">\n\x18SeedExceedsLimitSamePath\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"x\n\x1bSeedExceedsLimitSamePathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.SeedExceedsLimitSamePath\"D\n\x1eSeedExceedsLimitAndPathChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x84\x01\n!SeedExceedsLimitAndPathChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.SeedExceedsLimitAndPathChanged\"\\\n\x1fSeedExceedsLimitChecksumChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rchecksum_name\x18\x03 \x01(\t\"\x86\x01\n\"SeedExceedsLimitChecksumChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.SeedExceedsLimitChecksumChanged\"%\n\x0cUnusedTables\x12\x15\n\runused_tables\x18\x01 \x03(\t\"`\n\x0fUnusedTablesMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.UnusedTables\"\x87\x01\n\x17WrongResourceSchemaFile\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x1c\n\x14plural_resource_type\x18\x03 \x01(\t\x12\x10\n\x08yaml_key\x18\x04 \x01(\t\x12\x11\n\tfile_path\x18\x05 \x01(\t\"v\n\x1aWrongResourceSchemaFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.WrongResourceSchemaFile\"K\n\x10NoNodeForYamlKey\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x10\n\x08yaml_key\x18\x02 \x01(\t\x12\x11\n\tfile_path\x18\x03 \x01(\t\"h\n\x13NoNodeForYamlKeyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.NoNodeForYamlKey\"+\n\x15MacroNotFoundForPatch\x12\x12\n\npatch_name\x18\x01 \x01(\t\"r\n\x18MacroNotFoundForPatchMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MacroNotFoundForPatch\"\xb8\x01\n\x16NodeNotFoundOrDisabled\x12\x1a\n\x12original_file_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1b\n\x13resource_type_title\x18\x03 \x01(\t\x12\x13\n\x0btarget_name\x18\x04 \x01(\t\x12\x13\n\x0btarget_kind\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\x12\x10\n\x08\x64isabled\x18\x07 \x01(\t\"t\n\x19NodeNotFoundOrDisabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.NodeNotFoundOrDisabled\"H\n\x0fJinjaLogWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"f\n\x12JinjaLogWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.JinjaLogWarning\"E\n\x0cJinjaLogInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"`\n\x0fJinjaLogInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.JinjaLogInfo\"F\n\rJinjaLogDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"b\n\x10JinjaLogDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.JinjaLogDebug\"\xae\x01\n\x1eUnpinnedRefNewVersionAvailable\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rref_node_name\x18\x02 \x01(\t\x12\x18\n\x10ref_node_package\x18\x03 \x01(\t\x12\x18\n\x10ref_node_version\x18\x04 \x01(\t\x12\x17\n\x0fref_max_version\x18\x05 \x01(\t\"\x84\x01\n!UnpinnedRefNewVersionAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.UnpinnedRefNewVersionAvailable\"V\n\x0f\x44\x65precatedModel\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65precation_date\x18\x03 \x01(\t\"f\n\x12\x44\x65precatedModelMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DeprecatedModel\"\xc6\x01\n\x1cUpcomingReferenceDeprecation\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"\x80\x01\n\x1fUpcomingReferenceDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.UpcomingReferenceDeprecation\"\xbd\x01\n\x13\x44\x65precatedReference\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"n\n\x16\x44\x65precatedReferenceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DeprecatedReference\"/\n\x1dGitSparseCheckoutSubdirectory\x12\x0e\n\x06subdir\x18\x01 \x01(\t\"\x82\x01\n GitSparseCheckoutSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.GitSparseCheckoutSubdirectory\"/\n\x1bGitProgressCheckoutRevision\x12\x10\n\x08revision\x18\x01 \x01(\t\"~\n\x1eGitProgressCheckoutRevisionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.GitProgressCheckoutRevision\"4\n%GitProgressUpdatingExistingDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x92\x01\n(GitProgressUpdatingExistingDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.GitProgressUpdatingExistingDependency\".\n\x1fGitProgressPullingNewDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x86\x01\n\"GitProgressPullingNewDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressPullingNewDependency\"\x1d\n\x0eGitNothingToDo\x12\x0b\n\x03sha\x18\x01 \x01(\t\"d\n\x11GitNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.GitNothingToDo\"E\n\x1fGitProgressUpdatedCheckoutRange\x12\x11\n\tstart_sha\x18\x01 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x02 \x01(\t\"\x86\x01\n\"GitProgressUpdatedCheckoutRangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressUpdatedCheckoutRange\"*\n\x17GitProgressCheckedOutAt\x12\x0f\n\x07\x65nd_sha\x18\x01 \x01(\t\"v\n\x1aGitProgressCheckedOutAtMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.GitProgressCheckedOutAt\")\n\x1aRegistryProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"|\n\x1dRegistryProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.RegistryProgressGETRequest\"=\n\x1bRegistryProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"~\n\x1eRegistryProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RegistryProgressGETResponse\"_\n\x1dSelectorReportInvalidSelector\x12\x17\n\x0fvalid_selectors\x18\x01 \x01(\t\x12\x13\n\x0bspec_method\x18\x02 \x01(\t\x12\x10\n\x08raw_spec\x18\x03 \x01(\t\"\x82\x01\n SelectorReportInvalidSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.SelectorReportInvalidSelector\"\x15\n\x13\x44\x65psNoPackagesFound\"n\n\x16\x44\x65psNoPackagesFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsNoPackagesFound\"/\n\x17\x44\x65psStartPackageInstall\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"v\n\x1a\x44\x65psStartPackageInstallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsStartPackageInstall\"\'\n\x0f\x44\x65psInstallInfo\x12\x14\n\x0cversion_name\x18\x01 \x01(\t\"f\n\x12\x44\x65psInstallInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DepsInstallInfo\"-\n\x13\x44\x65psUpdateAvailable\x12\x16\n\x0eversion_latest\x18\x01 \x01(\t\"n\n\x16\x44\x65psUpdateAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsUpdateAvailable\"\x0e\n\x0c\x44\x65psUpToDate\"`\n\x0f\x44\x65psUpToDateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUpToDate\",\n\x14\x44\x65psListSubdirectory\x12\x14\n\x0csubdirectory\x18\x01 \x01(\t\"p\n\x17\x44\x65psListSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.DepsListSubdirectory\".\n\x1a\x44\x65psNotifyUpdatesAvailable\x12\x10\n\x08packages\x18\x01 \x03(\t\"|\n\x1d\x44\x65psNotifyUpdatesAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.DepsNotifyUpdatesAvailable\"1\n\x11RetryExternalCall\x12\x0f\n\x07\x61ttempt\x18\x01 \x01(\x05\x12\x0b\n\x03max\x18\x02 \x01(\x05\"j\n\x14RetryExternalCallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.RetryExternalCall\"#\n\x14RecordRetryException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17RecordRetryExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.RecordRetryException\".\n\x1fRegistryIndexProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x86\x01\n\"RegistryIndexProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryIndexProgressGETRequest\"B\n RegistryIndexProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x88\x01\n#RegistryIndexProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12;\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32-.proto_types.RegistryIndexProgressGETResponse\"2\n\x1eRegistryResponseUnexpectedType\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseUnexpectedTypeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseUnexpectedType\"2\n\x1eRegistryResponseMissingTopKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseMissingTopKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseMissingTopKeys\"5\n!RegistryResponseMissingNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8a\x01\n$RegistryResponseMissingNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.RegistryResponseMissingNestedKeys\"3\n\x1fRegistryResponseExtraNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x86\x01\n\"RegistryResponseExtraNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryResponseExtraNestedKeys\"(\n\x18\x44\x65psSetDownloadDirectory\x12\x0c\n\x04path\x18\x01 \x01(\t\"x\n\x1b\x44\x65psSetDownloadDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsSetDownloadDirectory\"-\n\x0c\x44\x65psUnpinned\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0b\n\x03git\x18\x02 \x01(\t\"`\n\x0f\x44\x65psUnpinnedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUnpinned\"/\n\x1bNoNodesForSelectionCriteria\x12\x10\n\x08spec_raw\x18\x01 \x01(\t\"~\n\x1eNoNodesForSelectionCriteriaMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.NoNodesForSelectionCriteria\"M\n\x1cPublicationArtifactAvailable\x12-\n\x0cpub_artifact\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x80\x01\n\x1fPublicationArtifactAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.PublicationArtifactAvailable\"*\n\x1bRunningOperationCaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"~\n\x1eRunningOperationCaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RunningOperationCaughtError\"\x11\n\x0f\x43ompileComplete\"f\n\x12\x43ompileCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.CompileComplete\"\x18\n\x16\x46reshnessCheckComplete\"t\n\x19\x46reshnessCheckCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessCheckComplete\"\x1c\n\nSeedHeader\x12\x0e\n\x06header\x18\x01 \x01(\t\"\\\n\rSeedHeaderMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SeedHeader\"3\n\x12SQLRunnerException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x02 \x01(\t\"l\n\x15SQLRunnerExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SQLRunnerException\"\xa8\x01\n\rLogTestResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\x12\n\nnum_models\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"b\n\x10LogTestResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogTestResult\"k\n\x0cLogStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"`\n\x0fLogStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.LogStartLine\"\x95\x01\n\x0eLogModelResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogModelResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogModelResult\"\xfa\x01\n\x11LogSnapshotResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x34\n\x03\x63\x66g\x18\x07 \x03(\x0b\x32\'.proto_types.LogSnapshotResult.CfgEntry\x1a*\n\x08\x43\x66gEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"j\n\x14LogSnapshotResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogSnapshotResult\"\xb9\x01\n\rLogSeedResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x16\n\x0eresult_message\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12\x10\n\x08relation\x18\x08 \x01(\t\"b\n\x10LogSeedResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogSeedResult\"\xad\x01\n\x12LogFreshnessResult\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x13\n\x0bsource_name\x18\x06 \x01(\t\x12\x12\n\ntable_name\x18\x07 \x01(\t\"l\n\x15LogFreshnessResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogFreshnessResult\"\"\n\rLogCancelLine\x12\x11\n\tconn_name\x18\x01 \x01(\t\"b\n\x10LogCancelLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogCancelLine\"\x1f\n\x0f\x44\x65\x66\x61ultSelector\x12\x0c\n\x04name\x18\x01 \x01(\t\"f\n\x12\x44\x65\x66\x61ultSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DefaultSelector\"5\n\tNodeStart\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"Z\n\x0cNodeStartMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.NodeStart\"g\n\x0cNodeFinished\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12-\n\nrun_result\x18\x02 \x01(\x0b\x32\x19.proto_types.RunResultMsg\"`\n\x0fNodeFinishedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.NodeFinished\"+\n\x1bQueryCancelationUnsupported\x12\x0c\n\x04type\x18\x01 \x01(\t\"~\n\x1eQueryCancelationUnsupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.QueryCancelationUnsupported\"O\n\x0f\x43oncurrencyLine\x12\x13\n\x0bnum_threads\x18\x01 \x01(\x05\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\x12\x12\n\nnode_count\x18\x03 \x01(\x05\"f\n\x12\x43oncurrencyLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ConcurrencyLine\"E\n\x19WritingInjectedSQLForNode\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1cWritingInjectedSQLForNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.WritingInjectedSQLForNode\"9\n\rNodeCompiling\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeCompilingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeCompiling\"9\n\rNodeExecuting\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeExecutingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeExecuting\"m\n\x10LogHookStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"h\n\x13LogHookStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.LogHookStartLine\"\x93\x01\n\x0eLogHookEndLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogHookEndLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogHookEndLine\"\x93\x01\n\x0fSkippingDetails\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x11\n\tnode_name\x18\x04 \x01(\t\x12\r\n\x05index\x18\x05 \x01(\x05\x12\r\n\x05total\x18\x06 \x01(\x05\"f\n\x12SkippingDetailsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SkippingDetails\"\r\n\x0bNothingToDo\"^\n\x0eNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.NothingToDo\",\n\x1dRunningOperationUncaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x82\x01\n RunningOperationUncaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.RunningOperationUncaughtError\"\x93\x01\n\x0c\x45ndRunResult\x12*\n\x07results\x18\x01 \x03(\x0b\x32\x19.proto_types.RunResultMsg\x12\x14\n\x0c\x65lapsed_time\x18\x02 \x01(\x02\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07success\x18\x04 \x01(\x08\"`\n\x0f\x45ndRunResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.EndRunResult\"\x11\n\x0fNoNodesSelected\"f\n\x12NoNodesSelectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.NoNodesSelected\"w\n\x10\x43ommandCompleted\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x65lapsed\x18\x04 \x01(\x02\"h\n\x13\x43ommandCompletedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.CommandCompleted\"k\n\x08ShowNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0f\n\x07preview\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"X\n\x0bShowNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.ShowNode\"p\n\x0c\x43ompiledNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x10\n\x08\x63ompiled\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"`\n\x0f\x43ompiledNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.CompiledNode\"b\n\x17\x43\x61tchableExceptionOnRun\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"v\n\x1a\x43\x61tchableExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.CatchableExceptionOnRun\"5\n\x12InternalErrorOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\"l\n\x15InternalErrorOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InternalErrorOnRun\"K\n\x15GenericExceptionOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"r\n\x18GenericExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.GenericExceptionOnRun\"N\n\x1aNodeConnectionReleaseError\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"|\n\x1dNodeConnectionReleaseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.NodeConnectionReleaseError\"\x1f\n\nFoundStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\"\\\n\rFoundStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.FoundStats\"\x17\n\x15MainKeyboardInterrupt\"r\n\x18MainKeyboardInterruptMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainKeyboardInterrupt\"#\n\x14MainEncounteredError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17MainEncounteredErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MainEncounteredError\"%\n\x0eMainStackTrace\x12\x13\n\x0bstack_trace\x18\x01 \x01(\t\"d\n\x11MainStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainStackTrace\"@\n\x13SystemCouldNotWrite\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"n\n\x16SystemCouldNotWriteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.SystemCouldNotWrite\"!\n\x12SystemExecutingCmd\x12\x0b\n\x03\x63md\x18\x01 \x03(\t\"l\n\x15SystemExecutingCmdMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SystemExecutingCmd\"\x1c\n\x0cSystemStdOut\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdOut\"\x1c\n\x0cSystemStdErr\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdErrMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdErr\",\n\x16SystemReportReturnCode\x12\x12\n\nreturncode\x18\x01 \x01(\x05\"t\n\x19SystemReportReturnCodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.SystemReportReturnCode\"p\n\x13TimingInfoCollected\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12/\n\x0btiming_info\x18\x02 \x01(\x0b\x32\x1a.proto_types.TimingInfoMsg\"n\n\x16TimingInfoCollectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.TimingInfoCollected\"&\n\x12LogDebugStackTrace\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"l\n\x15LogDebugStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDebugStackTrace\"\x1e\n\x0e\x43heckCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43heckCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CheckCleanPath\" \n\x10\x43onfirmCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"h\n\x13\x43onfirmCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConfirmCleanPath\"\"\n\x12ProtectedCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"l\n\x15ProtectedCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ProtectedCleanPath\"\x14\n\x12\x46inishedCleanPaths\"l\n\x15\x46inishedCleanPathsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FinishedCleanPaths\"5\n\x0bOpenCommand\x12\x10\n\x08open_cmd\x18\x01 \x01(\t\x12\x14\n\x0cprofiles_dir\x18\x02 \x01(\t\"^\n\x0eOpenCommandMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.OpenCommand\"\x19\n\nFormatting\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rFormattingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.Formatting\"0\n\x0fServingDocsPort\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"f\n\x12ServingDocsPortMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ServingDocsPort\"%\n\x15ServingDocsAccessInfo\x12\x0c\n\x04port\x18\x01 \x01(\t\"r\n\x18ServingDocsAccessInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ServingDocsAccessInfo\"\x15\n\x13ServingDocsExitInfo\"n\n\x16ServingDocsExitInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.ServingDocsExitInfo\"J\n\x10RunResultWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultWarning\"J\n\x10RunResultFailure\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultFailure\"k\n\tStatsLine\x12\x30\n\x05stats\x18\x01 \x03(\x0b\x32!.proto_types.StatsLine.StatsEntry\x1a,\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"Z\n\x0cStatsLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.StatsLine\"\x1d\n\x0eRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11RunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RunResultError\")\n\x17RunResultErrorNoMessage\x12\x0e\n\x06status\x18\x01 \x01(\t\"v\n\x1aRunResultErrorNoMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultErrorNoMessage\"\x1f\n\x0fSQLCompiledPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"f\n\x12SQLCompiledPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SQLCompiledPath\"-\n\x14\x43heckNodeTestFailure\x12\x15\n\rrelation_name\x18\x01 \x01(\t\"p\n\x17\x43heckNodeTestFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.CheckNodeTestFailure\"\"\n\x13\x46irstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"n\n\x16\x46irstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.FirstRunResultError\"\'\n\x18\x41\x66terFirstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"x\n\x1b\x41\x66terFirstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.AfterFirstRunResultError\"W\n\x0f\x45ndOfRunSummary\x12\x12\n\nnum_errors\x18\x01 \x01(\x05\x12\x14\n\x0cnum_warnings\x18\x02 \x01(\x05\x12\x1a\n\x12keyboard_interrupt\x18\x03 \x01(\x08\"f\n\x12\x45ndOfRunSummaryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.EndOfRunSummary\"U\n\x13LogSkipBecauseError\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x10\n\x08relation\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"n\n\x16LogSkipBecauseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.LogSkipBecauseError\"\x14\n\x12\x45nsureGitInstalled\"l\n\x15\x45nsureGitInstalledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.EnsureGitInstalled\"\x1a\n\x18\x44\x65psCreatingLocalSymlink\"x\n\x1b\x44\x65psCreatingLocalSymlinkMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsCreatingLocalSymlink\"\x19\n\x17\x44\x65psSymlinkNotAvailable\"v\n\x1a\x44\x65psSymlinkNotAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsSymlinkNotAvailable\"\x11\n\x0f\x44isableTracking\"f\n\x12\x44isableTrackingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DisableTracking\"\x1e\n\x0cSendingEvent\x12\x0e\n\x06kwargs\x18\x01 \x01(\t\"`\n\x0fSendingEventMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SendingEvent\"\x12\n\x10SendEventFailure\"h\n\x13SendEventFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SendEventFailure\"\r\n\x0b\x46lushEvents\"^\n\x0e\x46lushEventsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.FlushEvents\"\x14\n\x12\x46lushEventsFailure\"l\n\x15\x46lushEventsFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FlushEventsFailure\"-\n\x19TrackingInitializeFailure\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"z\n\x1cTrackingInitializeFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.TrackingInitializeFailure\"&\n\x17RunResultWarningMessage\x12\x0b\n\x03msg\x18\x01 \x01(\t\"v\n\x1aRunResultWarningMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultWarningMessage\"\x1a\n\x0b\x44\x65\x62ugCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"^\n\x0e\x44\x65\x62ugCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.DebugCmdOut\"\x1d\n\x0e\x44\x65\x62ugCmdResult\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11\x44\x65\x62ugCmdResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DebugCmdResult\"\x19\n\nListCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rListCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.ListCmdOut\"\x13\n\x04Note\x12\x0b\n\x03msg\x18\x01 \x01(\t\"P\n\x07NoteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x1f\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x11.proto_types.Noteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0btypes.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x91\x02\n\tEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x05\x65xtra\x18\t \x03(\x0b\x32!.proto_types.EventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x7f\n\rTimingInfoMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"V\n\x0cNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x91\x02\n\x08NodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\rnode_relation\x18\n \x01(\x0b\x32\x19.proto_types.NodeRelation\"\xd1\x01\n\x0cRunResultMsg\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x0btiming_info\x18\x03 \x03(\x0b\x32\x1a.proto_types.TimingInfoMsg\x12\x0e\n\x06thread\x18\x04 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x31\n\x10\x61\x64\x61pter_response\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"G\n\x0fReferenceKeyMsg\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\"6\n\x0eGenericMessage\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\"9\n\x11MainReportVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0blog_version\x18\x02 \x01(\x05\"j\n\x14MainReportVersionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.MainReportVersion\"r\n\x0eMainReportArgs\x12\x33\n\x04\x61rgs\x18\x01 \x03(\x0b\x32%.proto_types.MainReportArgs.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11MainReportArgsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainReportArgs\"+\n\x15MainTrackingUserState\x12\x12\n\nuser_state\x18\x01 \x01(\t\"r\n\x18MainTrackingUserStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainTrackingUserState\"5\n\x0fMergedFromState\x12\x12\n\nnum_merged\x18\x01 \x01(\x05\x12\x0e\n\x06sample\x18\x02 \x03(\t\"f\n\x12MergedFromStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.MergedFromState\"A\n\x14MissingProfileTarget\x12\x14\n\x0cprofile_name\x18\x01 \x01(\t\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\"p\n\x17MissingProfileTargetMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MissingProfileTarget\"(\n\x11InvalidOptionYAML\x12\x13\n\x0boption_name\x18\x01 \x01(\t\"j\n\x14InvalidOptionYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.InvalidOptionYAML\"!\n\x12LogDbtProjectError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15LogDbtProjectErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProjectError\"3\n\x12LogDbtProfileError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08profiles\x18\x02 \x03(\t\"l\n\x15LogDbtProfileErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProfileError\"!\n\x12StarterProjectPath\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"l\n\x15StarterProjectPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StarterProjectPath\"$\n\x15\x43onfigFolderDirectory\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"r\n\x18\x43onfigFolderDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConfigFolderDirectory\"\'\n\x14NoSampleProfileFound\x12\x0f\n\x07\x61\x64\x61pter\x18\x01 \x01(\t\"p\n\x17NoSampleProfileFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NoSampleProfileFound\"6\n\x18ProfileWrittenWithSample\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"x\n\x1bProfileWrittenWithSampleMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProfileWrittenWithSample\"B\n$ProfileWrittenWithTargetTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x90\x01\n\'ProfileWrittenWithTargetTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.ProfileWrittenWithTargetTemplateYAML\"C\n%ProfileWrittenWithProjectTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x92\x01\n(ProfileWrittenWithProjectTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.ProfileWrittenWithProjectTemplateYAML\"\x12\n\x10SettingUpProfile\"h\n\x13SettingUpProfileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SettingUpProfile\"\x1c\n\x1aInvalidProfileTemplateYAML\"|\n\x1dInvalidProfileTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.InvalidProfileTemplateYAML\"(\n\x18ProjectNameAlreadyExists\x12\x0c\n\x04name\x18\x01 \x01(\t\"x\n\x1bProjectNameAlreadyExistsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProjectNameAlreadyExists\"K\n\x0eProjectCreated\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocs_url\x18\x02 \x01(\t\x12\x11\n\tslack_url\x18\x03 \x01(\t\"d\n\x11ProjectCreatedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ProjectCreated\"@\n\x1aPackageRedirectDeprecation\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1dPackageRedirectDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PackageRedirectDeprecation\"\x1f\n\x1dPackageInstallPathDeprecation\"\x82\x01\n PackageInstallPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.PackageInstallPathDeprecation\"H\n\x1b\x43onfigSourcePathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"~\n\x1e\x43onfigSourcePathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigSourcePathDeprecation\"F\n\x19\x43onfigDataPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"z\n\x1c\x43onfigDataPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConfigDataPathDeprecation\"?\n\x19\x41\x64\x61pterDeprecationWarning\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"z\n\x1c\x41\x64\x61pterDeprecationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.AdapterDeprecationWarning\".\n\x17MetricAttributesRenamed\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\"v\n\x1aMetricAttributesRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.MetricAttributesRenamed\"+\n\x17\x45xposureNameDeprecation\x12\x10\n\x08\x65xposure\x18\x01 \x01(\t\"v\n\x1a\x45xposureNameDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.ExposureNameDeprecation\"^\n\x13InternalDeprecation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x18\n\x10suggested_action\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"n\n\x16InternalDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.InternalDeprecation\"@\n\x1a\x45nvironmentVariableRenamed\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1d\x45nvironmentVariableRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.EnvironmentVariableRenamed\"3\n\x18\x43onfigLogPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"x\n\x1b\x43onfigLogPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ConfigLogPathDeprecation\"6\n\x1b\x43onfigTargetPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"~\n\x1e\x43onfigTargetPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigTargetPathDeprecation\"!\n\x1f\x43ollectFreshnessReturnSignature\"\x86\x01\n\"CollectFreshnessReturnSignatureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.CollectFreshnessReturnSignature\"\x87\x01\n\x11\x41\x64\x61pterEventDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"j\n\x14\x41\x64\x61pterEventDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventDebug\"\x86\x01\n\x10\x41\x64\x61pterEventInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"h\n\x13\x41\x64\x61pterEventInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.AdapterEventInfo\"\x89\x01\n\x13\x41\x64\x61pterEventWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"n\n\x16\x41\x64\x61pterEventWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.AdapterEventWarning\"\x99\x01\n\x11\x41\x64\x61pterEventError\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x10\n\x08\x65xc_info\x18\x05 \x01(\t\"j\n\x14\x41\x64\x61pterEventErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventError\"_\n\rNewConnection\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"b\n\x10NewConnectionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NewConnection\"=\n\x10\x43onnectionReused\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x16\n\x0eorig_conn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionReusedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionReused\"0\n\x1b\x43onnectionLeftOpenInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"~\n\x1e\x43onnectionLeftOpenInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConnectionLeftOpenInCleanup\".\n\x19\x43onnectionClosedInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"z\n\x1c\x43onnectionClosedInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConnectionClosedInCleanup\"_\n\x0eRollbackFailed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"d\n\x11RollbackFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RollbackFailed\"O\n\x10\x43onnectionClosed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionClosedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionClosed\"Q\n\x12\x43onnectionLeftOpen\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"l\n\x15\x43onnectionLeftOpenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ConnectionLeftOpen\"G\n\x08Rollback\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"X\n\x0bRollbackMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.Rollback\"@\n\tCacheMiss\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\"Z\n\x0c\x43\x61\x63heMissMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.CacheMiss\"b\n\rListRelations\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12/\n\trelations\x18\x03 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10ListRelationsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ListRelations\"`\n\x0e\x43onnectionUsed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"d\n\x11\x43onnectionUsedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ConnectionUsed\"T\n\x08SQLQuery\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x0b\n\x03sql\x18\x03 \x01(\t\"X\n\x0bSQLQueryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.SQLQuery\"[\n\x0eSQLQueryStatus\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x03 \x01(\x02\"d\n\x11SQLQueryStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SQLQueryStatus\"H\n\tSQLCommit\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"Z\n\x0cSQLCommitMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.SQLCommit\"a\n\rColTypeChange\x12\x11\n\torig_type\x18\x01 \x01(\t\x12\x10\n\x08new_type\x18\x02 \x01(\t\x12+\n\x05table\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10\x43olTypeChangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ColTypeChange\"@\n\x0eSchemaCreation\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"d\n\x11SchemaCreationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SchemaCreation\"<\n\nSchemaDrop\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"\\\n\rSchemaDropMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SchemaDrop\"\xde\x01\n\x0b\x43\x61\x63heAction\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\t\x12-\n\x07ref_key\x18\x02 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_2\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_3\x18\x04 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12.\n\x08ref_list\x18\x05 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"^\n\x0e\x43\x61\x63heActionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.CacheAction\"\x98\x01\n\x0e\x43\x61\x63heDumpGraph\x12\x33\n\x04\x64ump\x18\x01 \x03(\x0b\x32%.proto_types.CacheDumpGraph.DumpEntry\x12\x14\n\x0c\x62\x65\x66ore_after\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x1a+\n\tDumpEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11\x43\x61\x63heDumpGraphMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CacheDumpGraph\"!\n\x12\x41\x64\x61pterImportError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15\x41\x64\x61pterImportErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.AdapterImportError\"#\n\x0fPluginLoadError\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"f\n\x12PluginLoadErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.PluginLoadError\"Z\n\x14NewConnectionOpening\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x18\n\x10\x63onnection_state\x18\x02 \x01(\t\"p\n\x17NewConnectionOpeningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NewConnectionOpening\"8\n\rCodeExecution\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x14\n\x0c\x63ode_content\x18\x02 \x01(\t\"b\n\x10\x43odeExecutionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.CodeExecution\"6\n\x13\x43odeExecutionStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x02 \x01(\x02\"n\n\x16\x43odeExecutionStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.CodeExecutionStatus\"%\n\x16\x43\x61talogGenerationError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"t\n\x19\x43\x61talogGenerationErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.CatalogGenerationError\"-\n\x13WriteCatalogFailure\x12\x16\n\x0enum_exceptions\x18\x01 \x01(\x05\"n\n\x16WriteCatalogFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.WriteCatalogFailure\"\x1e\n\x0e\x43\x61talogWritten\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43\x61talogWrittenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CatalogWritten\"\x14\n\x12\x43\x61nnotGenerateDocs\"l\n\x15\x43\x61nnotGenerateDocsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.CannotGenerateDocs\"\x11\n\x0f\x42uildingCatalog\"f\n\x12\x42uildingCatalogMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.BuildingCatalog\"-\n\x18\x44\x61tabaseErrorRunningHook\x12\x11\n\thook_type\x18\x01 \x01(\t\"x\n\x1b\x44\x61tabaseErrorRunningHookMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DatabaseErrorRunningHook\"4\n\x0cHooksRunning\x12\x11\n\tnum_hooks\x18\x01 \x01(\x05\x12\x11\n\thook_type\x18\x02 \x01(\t\"`\n\x0fHooksRunningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.HooksRunning\"T\n\x14\x46inishedRunningStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\x12\x11\n\texecution\x18\x02 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x03 \x01(\x02\"p\n\x17\x46inishedRunningStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.FinishedRunningStats\"<\n\x15\x43onstraintNotEnforced\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"r\n\x18\x43onstraintNotEnforcedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConstraintNotEnforced\"=\n\x16\x43onstraintNotSupported\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"t\n\x19\x43onstraintNotSupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.ConstraintNotSupported\"7\n\x12InputFileDiffError\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"l\n\x15InputFileDiffErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InputFileDiffError\"t\n\x1aPublicationArtifactChanged\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\t\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"|\n\x1dPublicationArtifactChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PublicationArtifactChanged\"?\n\x14InvalidValueForField\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_value\x18\x02 \x01(\t\"p\n\x17InvalidValueForFieldMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.InvalidValueForField\"Q\n\x11ValidationWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12\x11\n\tnode_name\x18\x03 \x01(\t\"j\n\x14ValidationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ValidationWarning\"!\n\x11ParsePerfInfoPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"j\n\x14ParsePerfInfoPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ParsePerfInfoPath\"1\n!PartialParsingErrorProcessingFile\x12\x0c\n\x04\x66ile\x18\x01 \x01(\t\"\x8a\x01\n$PartialParsingErrorProcessingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.PartialParsingErrorProcessingFile\"\x86\x01\n\x13PartialParsingError\x12?\n\x08\x65xc_info\x18\x01 \x03(\x0b\x32-.proto_types.PartialParsingError.ExcInfoEntry\x1a.\n\x0c\x45xcInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"n\n\x16PartialParsingErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.PartialParsingError\"\x1b\n\x19PartialParsingSkipParsing\"z\n\x1cPartialParsingSkipParsingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.PartialParsingSkipParsing\"&\n\x14UnableToPartialParse\x12\x0e\n\x06reason\x18\x01 \x01(\t\"p\n\x17UnableToPartialParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.UnableToPartialParse\"f\n\x12StateCheckVarsHash\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\x12\x0c\n\x04vars\x18\x02 \x01(\t\x12\x0f\n\x07profile\x18\x03 \x01(\t\x12\x0e\n\x06target\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\"l\n\x15StateCheckVarsHashMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StateCheckVarsHash\"\x1a\n\x18PartialParsingNotEnabled\"x\n\x1bPartialParsingNotEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.PartialParsingNotEnabled\"C\n\x14ParsedFileLoadFailed\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"p\n\x17ParsedFileLoadFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParsedFileLoadFailed\"H\n\x15PartialParsingEnabled\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x05\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hanged\x18\x03 \x01(\x05\"r\n\x18PartialParsingEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.PartialParsingEnabled\"8\n\x12PartialParsingFile\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\"l\n\x15PartialParsingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.PartialParsingFile\"\xaf\x01\n\x1fInvalidDisabledTargetInTestNode\x12\x1b\n\x13resource_type_title\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1a\n\x12original_file_path\x18\x03 \x01(\t\x12\x13\n\x0btarget_kind\x18\x04 \x01(\t\x12\x13\n\x0btarget_name\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\"\x86\x01\n\"InvalidDisabledTargetInTestNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.InvalidDisabledTargetInTestNode\"7\n\x18UnusedResourceConfigPath\x12\x1b\n\x13unused_config_paths\x18\x01 \x03(\t\"x\n\x1bUnusedResourceConfigPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.UnusedResourceConfigPath\"3\n\rSeedIncreased\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"b\n\x10SeedIncreasedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.SeedIncreased\">\n\x18SeedExceedsLimitSamePath\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"x\n\x1bSeedExceedsLimitSamePathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.SeedExceedsLimitSamePath\"D\n\x1eSeedExceedsLimitAndPathChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x84\x01\n!SeedExceedsLimitAndPathChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.SeedExceedsLimitAndPathChanged\"\\\n\x1fSeedExceedsLimitChecksumChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rchecksum_name\x18\x03 \x01(\t\"\x86\x01\n\"SeedExceedsLimitChecksumChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.SeedExceedsLimitChecksumChanged\"%\n\x0cUnusedTables\x12\x15\n\runused_tables\x18\x01 \x03(\t\"`\n\x0fUnusedTablesMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.UnusedTables\"\x87\x01\n\x17WrongResourceSchemaFile\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x1c\n\x14plural_resource_type\x18\x03 \x01(\t\x12\x10\n\x08yaml_key\x18\x04 \x01(\t\x12\x11\n\tfile_path\x18\x05 \x01(\t\"v\n\x1aWrongResourceSchemaFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.WrongResourceSchemaFile\"K\n\x10NoNodeForYamlKey\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x10\n\x08yaml_key\x18\x02 \x01(\t\x12\x11\n\tfile_path\x18\x03 \x01(\t\"h\n\x13NoNodeForYamlKeyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.NoNodeForYamlKey\"+\n\x15MacroNotFoundForPatch\x12\x12\n\npatch_name\x18\x01 \x01(\t\"r\n\x18MacroNotFoundForPatchMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MacroNotFoundForPatch\"\xb8\x01\n\x16NodeNotFoundOrDisabled\x12\x1a\n\x12original_file_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1b\n\x13resource_type_title\x18\x03 \x01(\t\x12\x13\n\x0btarget_name\x18\x04 \x01(\t\x12\x13\n\x0btarget_kind\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\x12\x10\n\x08\x64isabled\x18\x07 \x01(\t\"t\n\x19NodeNotFoundOrDisabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.NodeNotFoundOrDisabled\"H\n\x0fJinjaLogWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"f\n\x12JinjaLogWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.JinjaLogWarning\"E\n\x0cJinjaLogInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"`\n\x0fJinjaLogInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.JinjaLogInfo\"F\n\rJinjaLogDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"b\n\x10JinjaLogDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.JinjaLogDebug\"\xae\x01\n\x1eUnpinnedRefNewVersionAvailable\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rref_node_name\x18\x02 \x01(\t\x12\x18\n\x10ref_node_package\x18\x03 \x01(\t\x12\x18\n\x10ref_node_version\x18\x04 \x01(\t\x12\x17\n\x0fref_max_version\x18\x05 \x01(\t\"\x84\x01\n!UnpinnedRefNewVersionAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.UnpinnedRefNewVersionAvailable\"V\n\x0f\x44\x65precatedModel\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65precation_date\x18\x03 \x01(\t\"f\n\x12\x44\x65precatedModelMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DeprecatedModel\"\xc6\x01\n\x1cUpcomingReferenceDeprecation\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"\x80\x01\n\x1fUpcomingReferenceDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.UpcomingReferenceDeprecation\"\xbd\x01\n\x13\x44\x65precatedReference\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"n\n\x16\x44\x65precatedReferenceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DeprecatedReference\"<\n$UnsupportedConstraintMaterialization\x12\x14\n\x0cmaterialized\x18\x01 \x01(\t\"\x90\x01\n\'UnsupportedConstraintMaterializationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.UnsupportedConstraintMaterialization\"/\n\x1dGitSparseCheckoutSubdirectory\x12\x0e\n\x06subdir\x18\x01 \x01(\t\"\x82\x01\n GitSparseCheckoutSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.GitSparseCheckoutSubdirectory\"/\n\x1bGitProgressCheckoutRevision\x12\x10\n\x08revision\x18\x01 \x01(\t\"~\n\x1eGitProgressCheckoutRevisionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.GitProgressCheckoutRevision\"4\n%GitProgressUpdatingExistingDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x92\x01\n(GitProgressUpdatingExistingDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.GitProgressUpdatingExistingDependency\".\n\x1fGitProgressPullingNewDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x86\x01\n\"GitProgressPullingNewDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressPullingNewDependency\"\x1d\n\x0eGitNothingToDo\x12\x0b\n\x03sha\x18\x01 \x01(\t\"d\n\x11GitNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.GitNothingToDo\"E\n\x1fGitProgressUpdatedCheckoutRange\x12\x11\n\tstart_sha\x18\x01 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x02 \x01(\t\"\x86\x01\n\"GitProgressUpdatedCheckoutRangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressUpdatedCheckoutRange\"*\n\x17GitProgressCheckedOutAt\x12\x0f\n\x07\x65nd_sha\x18\x01 \x01(\t\"v\n\x1aGitProgressCheckedOutAtMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.GitProgressCheckedOutAt\")\n\x1aRegistryProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"|\n\x1dRegistryProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.RegistryProgressGETRequest\"=\n\x1bRegistryProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"~\n\x1eRegistryProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RegistryProgressGETResponse\"_\n\x1dSelectorReportInvalidSelector\x12\x17\n\x0fvalid_selectors\x18\x01 \x01(\t\x12\x13\n\x0bspec_method\x18\x02 \x01(\t\x12\x10\n\x08raw_spec\x18\x03 \x01(\t\"\x82\x01\n SelectorReportInvalidSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.SelectorReportInvalidSelector\"\x15\n\x13\x44\x65psNoPackagesFound\"n\n\x16\x44\x65psNoPackagesFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsNoPackagesFound\"/\n\x17\x44\x65psStartPackageInstall\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"v\n\x1a\x44\x65psStartPackageInstallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsStartPackageInstall\"\'\n\x0f\x44\x65psInstallInfo\x12\x14\n\x0cversion_name\x18\x01 \x01(\t\"f\n\x12\x44\x65psInstallInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DepsInstallInfo\"-\n\x13\x44\x65psUpdateAvailable\x12\x16\n\x0eversion_latest\x18\x01 \x01(\t\"n\n\x16\x44\x65psUpdateAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsUpdateAvailable\"\x0e\n\x0c\x44\x65psUpToDate\"`\n\x0f\x44\x65psUpToDateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUpToDate\",\n\x14\x44\x65psListSubdirectory\x12\x14\n\x0csubdirectory\x18\x01 \x01(\t\"p\n\x17\x44\x65psListSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.DepsListSubdirectory\".\n\x1a\x44\x65psNotifyUpdatesAvailable\x12\x10\n\x08packages\x18\x01 \x03(\t\"|\n\x1d\x44\x65psNotifyUpdatesAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.DepsNotifyUpdatesAvailable\"1\n\x11RetryExternalCall\x12\x0f\n\x07\x61ttempt\x18\x01 \x01(\x05\x12\x0b\n\x03max\x18\x02 \x01(\x05\"j\n\x14RetryExternalCallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.RetryExternalCall\"#\n\x14RecordRetryException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17RecordRetryExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.RecordRetryException\".\n\x1fRegistryIndexProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x86\x01\n\"RegistryIndexProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryIndexProgressGETRequest\"B\n RegistryIndexProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x88\x01\n#RegistryIndexProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12;\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32-.proto_types.RegistryIndexProgressGETResponse\"2\n\x1eRegistryResponseUnexpectedType\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseUnexpectedTypeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseUnexpectedType\"2\n\x1eRegistryResponseMissingTopKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseMissingTopKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseMissingTopKeys\"5\n!RegistryResponseMissingNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8a\x01\n$RegistryResponseMissingNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.RegistryResponseMissingNestedKeys\"3\n\x1fRegistryResponseExtraNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x86\x01\n\"RegistryResponseExtraNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryResponseExtraNestedKeys\"(\n\x18\x44\x65psSetDownloadDirectory\x12\x0c\n\x04path\x18\x01 \x01(\t\"x\n\x1b\x44\x65psSetDownloadDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsSetDownloadDirectory\"-\n\x0c\x44\x65psUnpinned\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0b\n\x03git\x18\x02 \x01(\t\"`\n\x0f\x44\x65psUnpinnedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUnpinned\"/\n\x1bNoNodesForSelectionCriteria\x12\x10\n\x08spec_raw\x18\x01 \x01(\t\"~\n\x1eNoNodesForSelectionCriteriaMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.NoNodesForSelectionCriteria\"M\n\x1cPublicationArtifactAvailable\x12-\n\x0cpub_artifact\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x80\x01\n\x1fPublicationArtifactAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.PublicationArtifactAvailable\"*\n\x1bRunningOperationCaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"~\n\x1eRunningOperationCaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RunningOperationCaughtError\"\x11\n\x0f\x43ompileComplete\"f\n\x12\x43ompileCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.CompileComplete\"\x18\n\x16\x46reshnessCheckComplete\"t\n\x19\x46reshnessCheckCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessCheckComplete\"\x1c\n\nSeedHeader\x12\x0e\n\x06header\x18\x01 \x01(\t\"\\\n\rSeedHeaderMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SeedHeader\"3\n\x12SQLRunnerException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x02 \x01(\t\"l\n\x15SQLRunnerExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SQLRunnerException\"\xa8\x01\n\rLogTestResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\x12\n\nnum_models\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"b\n\x10LogTestResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogTestResult\"k\n\x0cLogStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"`\n\x0fLogStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.LogStartLine\"\x95\x01\n\x0eLogModelResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogModelResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogModelResult\"\xfa\x01\n\x11LogSnapshotResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x34\n\x03\x63\x66g\x18\x07 \x03(\x0b\x32\'.proto_types.LogSnapshotResult.CfgEntry\x1a*\n\x08\x43\x66gEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"j\n\x14LogSnapshotResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogSnapshotResult\"\xb9\x01\n\rLogSeedResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x16\n\x0eresult_message\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12\x10\n\x08relation\x18\x08 \x01(\t\"b\n\x10LogSeedResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogSeedResult\"\xad\x01\n\x12LogFreshnessResult\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x13\n\x0bsource_name\x18\x06 \x01(\t\x12\x12\n\ntable_name\x18\x07 \x01(\t\"l\n\x15LogFreshnessResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogFreshnessResult\"\"\n\rLogCancelLine\x12\x11\n\tconn_name\x18\x01 \x01(\t\"b\n\x10LogCancelLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogCancelLine\"\x1f\n\x0f\x44\x65\x66\x61ultSelector\x12\x0c\n\x04name\x18\x01 \x01(\t\"f\n\x12\x44\x65\x66\x61ultSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DefaultSelector\"5\n\tNodeStart\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"Z\n\x0cNodeStartMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.NodeStart\"g\n\x0cNodeFinished\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12-\n\nrun_result\x18\x02 \x01(\x0b\x32\x19.proto_types.RunResultMsg\"`\n\x0fNodeFinishedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.NodeFinished\"+\n\x1bQueryCancelationUnsupported\x12\x0c\n\x04type\x18\x01 \x01(\t\"~\n\x1eQueryCancelationUnsupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.QueryCancelationUnsupported\"O\n\x0f\x43oncurrencyLine\x12\x13\n\x0bnum_threads\x18\x01 \x01(\x05\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\x12\x12\n\nnode_count\x18\x03 \x01(\x05\"f\n\x12\x43oncurrencyLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ConcurrencyLine\"E\n\x19WritingInjectedSQLForNode\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1cWritingInjectedSQLForNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.WritingInjectedSQLForNode\"9\n\rNodeCompiling\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeCompilingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeCompiling\"9\n\rNodeExecuting\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeExecutingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeExecuting\"m\n\x10LogHookStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"h\n\x13LogHookStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.LogHookStartLine\"\x93\x01\n\x0eLogHookEndLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogHookEndLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogHookEndLine\"\x93\x01\n\x0fSkippingDetails\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x11\n\tnode_name\x18\x04 \x01(\t\x12\r\n\x05index\x18\x05 \x01(\x05\x12\r\n\x05total\x18\x06 \x01(\x05\"f\n\x12SkippingDetailsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SkippingDetails\"\r\n\x0bNothingToDo\"^\n\x0eNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.NothingToDo\",\n\x1dRunningOperationUncaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x82\x01\n RunningOperationUncaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.RunningOperationUncaughtError\"\x93\x01\n\x0c\x45ndRunResult\x12*\n\x07results\x18\x01 \x03(\x0b\x32\x19.proto_types.RunResultMsg\x12\x14\n\x0c\x65lapsed_time\x18\x02 \x01(\x02\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07success\x18\x04 \x01(\x08\"`\n\x0f\x45ndRunResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.EndRunResult\"\x11\n\x0fNoNodesSelected\"f\n\x12NoNodesSelectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.NoNodesSelected\"w\n\x10\x43ommandCompleted\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x65lapsed\x18\x04 \x01(\x02\"h\n\x13\x43ommandCompletedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.CommandCompleted\"k\n\x08ShowNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0f\n\x07preview\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"X\n\x0bShowNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.ShowNode\"p\n\x0c\x43ompiledNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x10\n\x08\x63ompiled\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"`\n\x0f\x43ompiledNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.CompiledNode\"b\n\x17\x43\x61tchableExceptionOnRun\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"v\n\x1a\x43\x61tchableExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.CatchableExceptionOnRun\"5\n\x12InternalErrorOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\"l\n\x15InternalErrorOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InternalErrorOnRun\"K\n\x15GenericExceptionOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"r\n\x18GenericExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.GenericExceptionOnRun\"N\n\x1aNodeConnectionReleaseError\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"|\n\x1dNodeConnectionReleaseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.NodeConnectionReleaseError\"\x1f\n\nFoundStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\"\\\n\rFoundStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.FoundStats\"\x17\n\x15MainKeyboardInterrupt\"r\n\x18MainKeyboardInterruptMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainKeyboardInterrupt\"#\n\x14MainEncounteredError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17MainEncounteredErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MainEncounteredError\"%\n\x0eMainStackTrace\x12\x13\n\x0bstack_trace\x18\x01 \x01(\t\"d\n\x11MainStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainStackTrace\"@\n\x13SystemCouldNotWrite\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"n\n\x16SystemCouldNotWriteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.SystemCouldNotWrite\"!\n\x12SystemExecutingCmd\x12\x0b\n\x03\x63md\x18\x01 \x03(\t\"l\n\x15SystemExecutingCmdMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SystemExecutingCmd\"\x1c\n\x0cSystemStdOut\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdOut\"\x1c\n\x0cSystemStdErr\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdErrMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdErr\",\n\x16SystemReportReturnCode\x12\x12\n\nreturncode\x18\x01 \x01(\x05\"t\n\x19SystemReportReturnCodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.SystemReportReturnCode\"p\n\x13TimingInfoCollected\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12/\n\x0btiming_info\x18\x02 \x01(\x0b\x32\x1a.proto_types.TimingInfoMsg\"n\n\x16TimingInfoCollectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.TimingInfoCollected\"&\n\x12LogDebugStackTrace\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"l\n\x15LogDebugStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDebugStackTrace\"\x1e\n\x0e\x43heckCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43heckCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CheckCleanPath\" \n\x10\x43onfirmCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"h\n\x13\x43onfirmCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConfirmCleanPath\"\"\n\x12ProtectedCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"l\n\x15ProtectedCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ProtectedCleanPath\"\x14\n\x12\x46inishedCleanPaths\"l\n\x15\x46inishedCleanPathsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FinishedCleanPaths\"5\n\x0bOpenCommand\x12\x10\n\x08open_cmd\x18\x01 \x01(\t\x12\x14\n\x0cprofiles_dir\x18\x02 \x01(\t\"^\n\x0eOpenCommandMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.OpenCommand\"\x19\n\nFormatting\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rFormattingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.Formatting\"0\n\x0fServingDocsPort\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"f\n\x12ServingDocsPortMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ServingDocsPort\"%\n\x15ServingDocsAccessInfo\x12\x0c\n\x04port\x18\x01 \x01(\t\"r\n\x18ServingDocsAccessInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ServingDocsAccessInfo\"\x15\n\x13ServingDocsExitInfo\"n\n\x16ServingDocsExitInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.ServingDocsExitInfo\"J\n\x10RunResultWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultWarning\"J\n\x10RunResultFailure\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultFailure\"k\n\tStatsLine\x12\x30\n\x05stats\x18\x01 \x03(\x0b\x32!.proto_types.StatsLine.StatsEntry\x1a,\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"Z\n\x0cStatsLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.StatsLine\"\x1d\n\x0eRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11RunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RunResultError\")\n\x17RunResultErrorNoMessage\x12\x0e\n\x06status\x18\x01 \x01(\t\"v\n\x1aRunResultErrorNoMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultErrorNoMessage\"\x1f\n\x0fSQLCompiledPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"f\n\x12SQLCompiledPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SQLCompiledPath\"-\n\x14\x43heckNodeTestFailure\x12\x15\n\rrelation_name\x18\x01 \x01(\t\"p\n\x17\x43heckNodeTestFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.CheckNodeTestFailure\"\"\n\x13\x46irstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"n\n\x16\x46irstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.FirstRunResultError\"\'\n\x18\x41\x66terFirstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"x\n\x1b\x41\x66terFirstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.AfterFirstRunResultError\"W\n\x0f\x45ndOfRunSummary\x12\x12\n\nnum_errors\x18\x01 \x01(\x05\x12\x14\n\x0cnum_warnings\x18\x02 \x01(\x05\x12\x1a\n\x12keyboard_interrupt\x18\x03 \x01(\x08\"f\n\x12\x45ndOfRunSummaryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.EndOfRunSummary\"U\n\x13LogSkipBecauseError\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x10\n\x08relation\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"n\n\x16LogSkipBecauseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.LogSkipBecauseError\"\x14\n\x12\x45nsureGitInstalled\"l\n\x15\x45nsureGitInstalledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.EnsureGitInstalled\"\x1a\n\x18\x44\x65psCreatingLocalSymlink\"x\n\x1b\x44\x65psCreatingLocalSymlinkMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsCreatingLocalSymlink\"\x19\n\x17\x44\x65psSymlinkNotAvailable\"v\n\x1a\x44\x65psSymlinkNotAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsSymlinkNotAvailable\"\x11\n\x0f\x44isableTracking\"f\n\x12\x44isableTrackingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DisableTracking\"\x1e\n\x0cSendingEvent\x12\x0e\n\x06kwargs\x18\x01 \x01(\t\"`\n\x0fSendingEventMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SendingEvent\"\x12\n\x10SendEventFailure\"h\n\x13SendEventFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SendEventFailure\"\r\n\x0b\x46lushEvents\"^\n\x0e\x46lushEventsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.FlushEvents\"\x14\n\x12\x46lushEventsFailure\"l\n\x15\x46lushEventsFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FlushEventsFailure\"-\n\x19TrackingInitializeFailure\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"z\n\x1cTrackingInitializeFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.TrackingInitializeFailure\"&\n\x17RunResultWarningMessage\x12\x0b\n\x03msg\x18\x01 \x01(\t\"v\n\x1aRunResultWarningMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultWarningMessage\"\x1a\n\x0b\x44\x65\x62ugCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"^\n\x0e\x44\x65\x62ugCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.DebugCmdOut\"\x1d\n\x0e\x44\x65\x62ugCmdResult\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11\x44\x65\x62ugCmdResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DebugCmdResult\"\x19\n\nListCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rListCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.ListCmdOut\"\x13\n\x04Note\x12\x0b\n\x03msg\x18\x01 \x01(\t\"P\n\x07NoteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x1f\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x11.proto_types.Noteb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'types_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _EVENTINFO_EXTRAENTRY._options = None
@@ -452,444 +452,448 @@
   _UPCOMINGREFERENCEDEPRECATION._serialized_end=19618
   _UPCOMINGREFERENCEDEPRECATIONMSG._serialized_start=19621
   _UPCOMINGREFERENCEDEPRECATIONMSG._serialized_end=19749
   _DEPRECATEDREFERENCE._serialized_start=19752
   _DEPRECATEDREFERENCE._serialized_end=19941
   _DEPRECATEDREFERENCEMSG._serialized_start=19943
   _DEPRECATEDREFERENCEMSG._serialized_end=20053
-  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_start=20055
-  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_end=20102
-  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_start=20105
-  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_end=20235
-  _GITPROGRESSCHECKOUTREVISION._serialized_start=20237
-  _GITPROGRESSCHECKOUTREVISION._serialized_end=20284
-  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_start=20286
-  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_end=20412
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_start=20414
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_end=20466
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_start=20469
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_end=20615
-  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_start=20617
-  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_end=20663
-  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_start=20666
-  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_end=20800
-  _GITNOTHINGTODO._serialized_start=20802
-  _GITNOTHINGTODO._serialized_end=20831
-  _GITNOTHINGTODOMSG._serialized_start=20833
-  _GITNOTHINGTODOMSG._serialized_end=20933
-  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_start=20935
-  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_end=21004
-  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_start=21007
-  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_end=21141
-  _GITPROGRESSCHECKEDOUTAT._serialized_start=21143
-  _GITPROGRESSCHECKEDOUTAT._serialized_end=21185
-  _GITPROGRESSCHECKEDOUTATMSG._serialized_start=21187
-  _GITPROGRESSCHECKEDOUTATMSG._serialized_end=21305
-  _REGISTRYPROGRESSGETREQUEST._serialized_start=21307
-  _REGISTRYPROGRESSGETREQUEST._serialized_end=21348
-  _REGISTRYPROGRESSGETREQUESTMSG._serialized_start=21350
-  _REGISTRYPROGRESSGETREQUESTMSG._serialized_end=21474
-  _REGISTRYPROGRESSGETRESPONSE._serialized_start=21476
-  _REGISTRYPROGRESSGETRESPONSE._serialized_end=21537
-  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_start=21539
-  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_end=21665
-  _SELECTORREPORTINVALIDSELECTOR._serialized_start=21667
-  _SELECTORREPORTINVALIDSELECTOR._serialized_end=21762
-  _SELECTORREPORTINVALIDSELECTORMSG._serialized_start=21765
-  _SELECTORREPORTINVALIDSELECTORMSG._serialized_end=21895
-  _DEPSNOPACKAGESFOUND._serialized_start=21897
-  _DEPSNOPACKAGESFOUND._serialized_end=21918
-  _DEPSNOPACKAGESFOUNDMSG._serialized_start=21920
-  _DEPSNOPACKAGESFOUNDMSG._serialized_end=22030
-  _DEPSSTARTPACKAGEINSTALL._serialized_start=22032
-  _DEPSSTARTPACKAGEINSTALL._serialized_end=22079
-  _DEPSSTARTPACKAGEINSTALLMSG._serialized_start=22081
-  _DEPSSTARTPACKAGEINSTALLMSG._serialized_end=22199
-  _DEPSINSTALLINFO._serialized_start=22201
-  _DEPSINSTALLINFO._serialized_end=22240
-  _DEPSINSTALLINFOMSG._serialized_start=22242
-  _DEPSINSTALLINFOMSG._serialized_end=22344
-  _DEPSUPDATEAVAILABLE._serialized_start=22346
-  _DEPSUPDATEAVAILABLE._serialized_end=22391
-  _DEPSUPDATEAVAILABLEMSG._serialized_start=22393
-  _DEPSUPDATEAVAILABLEMSG._serialized_end=22503
-  _DEPSUPTODATE._serialized_start=22505
-  _DEPSUPTODATE._serialized_end=22519
-  _DEPSUPTODATEMSG._serialized_start=22521
-  _DEPSUPTODATEMSG._serialized_end=22617
-  _DEPSLISTSUBDIRECTORY._serialized_start=22619
-  _DEPSLISTSUBDIRECTORY._serialized_end=22663
-  _DEPSLISTSUBDIRECTORYMSG._serialized_start=22665
-  _DEPSLISTSUBDIRECTORYMSG._serialized_end=22777
-  _DEPSNOTIFYUPDATESAVAILABLE._serialized_start=22779
-  _DEPSNOTIFYUPDATESAVAILABLE._serialized_end=22825
-  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_start=22827
-  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_end=22951
-  _RETRYEXTERNALCALL._serialized_start=22953
-  _RETRYEXTERNALCALL._serialized_end=23002
-  _RETRYEXTERNALCALLMSG._serialized_start=23004
-  _RETRYEXTERNALCALLMSG._serialized_end=23110
-  _RECORDRETRYEXCEPTION._serialized_start=23112
-  _RECORDRETRYEXCEPTION._serialized_end=23147
-  _RECORDRETRYEXCEPTIONMSG._serialized_start=23149
-  _RECORDRETRYEXCEPTIONMSG._serialized_end=23261
-  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_start=23263
-  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_end=23309
-  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_start=23312
-  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_end=23446
-  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_start=23448
-  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_end=23514
-  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_start=23517
-  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_end=23653
-  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_start=23655
-  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_end=23705
-  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_start=23708
-  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_end=23840
-  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_start=23842
-  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_end=23892
-  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_start=23895
-  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_end=24027
-  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_start=24029
-  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_end=24082
-  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_start=24085
-  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_end=24223
-  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_start=24225
-  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_end=24276
-  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_start=24279
-  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_end=24413
-  _DEPSSETDOWNLOADDIRECTORY._serialized_start=24415
-  _DEPSSETDOWNLOADDIRECTORY._serialized_end=24455
-  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_start=24457
-  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_end=24577
-  _DEPSUNPINNED._serialized_start=24579
-  _DEPSUNPINNED._serialized_end=24624
-  _DEPSUNPINNEDMSG._serialized_start=24626
-  _DEPSUNPINNEDMSG._serialized_end=24722
-  _NONODESFORSELECTIONCRITERIA._serialized_start=24724
-  _NONODESFORSELECTIONCRITERIA._serialized_end=24771
-  _NONODESFORSELECTIONCRITERIAMSG._serialized_start=24773
-  _NONODESFORSELECTIONCRITERIAMSG._serialized_end=24899
-  _PUBLICATIONARTIFACTAVAILABLE._serialized_start=24901
-  _PUBLICATIONARTIFACTAVAILABLE._serialized_end=24978
-  _PUBLICATIONARTIFACTAVAILABLEMSG._serialized_start=24981
-  _PUBLICATIONARTIFACTAVAILABLEMSG._serialized_end=25109
-  _RUNNINGOPERATIONCAUGHTERROR._serialized_start=25111
-  _RUNNINGOPERATIONCAUGHTERROR._serialized_end=25153
-  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_start=25155
-  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_end=25281
-  _COMPILECOMPLETE._serialized_start=25283
-  _COMPILECOMPLETE._serialized_end=25300
-  _COMPILECOMPLETEMSG._serialized_start=25302
-  _COMPILECOMPLETEMSG._serialized_end=25404
-  _FRESHNESSCHECKCOMPLETE._serialized_start=25406
-  _FRESHNESSCHECKCOMPLETE._serialized_end=25430
-  _FRESHNESSCHECKCOMPLETEMSG._serialized_start=25432
-  _FRESHNESSCHECKCOMPLETEMSG._serialized_end=25548
-  _SEEDHEADER._serialized_start=25550
-  _SEEDHEADER._serialized_end=25578
-  _SEEDHEADERMSG._serialized_start=25580
-  _SEEDHEADERMSG._serialized_end=25672
-  _SQLRUNNEREXCEPTION._serialized_start=25674
-  _SQLRUNNEREXCEPTION._serialized_end=25725
-  _SQLRUNNEREXCEPTIONMSG._serialized_start=25727
-  _SQLRUNNEREXCEPTIONMSG._serialized_end=25835
-  _LOGTESTRESULT._serialized_start=25838
-  _LOGTESTRESULT._serialized_end=26006
-  _LOGTESTRESULTMSG._serialized_start=26008
-  _LOGTESTRESULTMSG._serialized_end=26106
-  _LOGSTARTLINE._serialized_start=26108
-  _LOGSTARTLINE._serialized_end=26215
-  _LOGSTARTLINEMSG._serialized_start=26217
-  _LOGSTARTLINEMSG._serialized_end=26313
-  _LOGMODELRESULT._serialized_start=26316
-  _LOGMODELRESULT._serialized_end=26465
-  _LOGMODELRESULTMSG._serialized_start=26467
-  _LOGMODELRESULTMSG._serialized_end=26567
-  _LOGSNAPSHOTRESULT._serialized_start=26570
-  _LOGSNAPSHOTRESULT._serialized_end=26820
-  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_start=26778
-  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_end=26820
-  _LOGSNAPSHOTRESULTMSG._serialized_start=26822
-  _LOGSNAPSHOTRESULTMSG._serialized_end=26928
-  _LOGSEEDRESULT._serialized_start=26931
-  _LOGSEEDRESULT._serialized_end=27116
-  _LOGSEEDRESULTMSG._serialized_start=27118
-  _LOGSEEDRESULTMSG._serialized_end=27216
-  _LOGFRESHNESSRESULT._serialized_start=27219
-  _LOGFRESHNESSRESULT._serialized_end=27392
-  _LOGFRESHNESSRESULTMSG._serialized_start=27394
-  _LOGFRESHNESSRESULTMSG._serialized_end=27502
-  _LOGCANCELLINE._serialized_start=27504
-  _LOGCANCELLINE._serialized_end=27538
-  _LOGCANCELLINEMSG._serialized_start=27540
-  _LOGCANCELLINEMSG._serialized_end=27638
-  _DEFAULTSELECTOR._serialized_start=27640
-  _DEFAULTSELECTOR._serialized_end=27671
-  _DEFAULTSELECTORMSG._serialized_start=27673
-  _DEFAULTSELECTORMSG._serialized_end=27775
-  _NODESTART._serialized_start=27777
-  _NODESTART._serialized_end=27830
-  _NODESTARTMSG._serialized_start=27832
-  _NODESTARTMSG._serialized_end=27922
-  _NODEFINISHED._serialized_start=27924
-  _NODEFINISHED._serialized_end=28027
-  _NODEFINISHEDMSG._serialized_start=28029
-  _NODEFINISHEDMSG._serialized_end=28125
-  _QUERYCANCELATIONUNSUPPORTED._serialized_start=28127
-  _QUERYCANCELATIONUNSUPPORTED._serialized_end=28170
-  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_start=28172
-  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_end=28298
-  _CONCURRENCYLINE._serialized_start=28300
-  _CONCURRENCYLINE._serialized_end=28379
-  _CONCURRENCYLINEMSG._serialized_start=28381
-  _CONCURRENCYLINEMSG._serialized_end=28483
-  _WRITINGINJECTEDSQLFORNODE._serialized_start=28485
-  _WRITINGINJECTEDSQLFORNODE._serialized_end=28554
-  _WRITINGINJECTEDSQLFORNODEMSG._serialized_start=28556
-  _WRITINGINJECTEDSQLFORNODEMSG._serialized_end=28678
-  _NODECOMPILING._serialized_start=28680
-  _NODECOMPILING._serialized_end=28737
-  _NODECOMPILINGMSG._serialized_start=28739
-  _NODECOMPILINGMSG._serialized_end=28837
-  _NODEEXECUTING._serialized_start=28839
-  _NODEEXECUTING._serialized_end=28896
-  _NODEEXECUTINGMSG._serialized_start=28898
-  _NODEEXECUTINGMSG._serialized_end=28996
-  _LOGHOOKSTARTLINE._serialized_start=28998
-  _LOGHOOKSTARTLINE._serialized_end=29107
-  _LOGHOOKSTARTLINEMSG._serialized_start=29109
-  _LOGHOOKSTARTLINEMSG._serialized_end=29213
-  _LOGHOOKENDLINE._serialized_start=29216
-  _LOGHOOKENDLINE._serialized_end=29363
-  _LOGHOOKENDLINEMSG._serialized_start=29365
-  _LOGHOOKENDLINEMSG._serialized_end=29465
-  _SKIPPINGDETAILS._serialized_start=29468
-  _SKIPPINGDETAILS._serialized_end=29615
-  _SKIPPINGDETAILSMSG._serialized_start=29617
-  _SKIPPINGDETAILSMSG._serialized_end=29719
-  _NOTHINGTODO._serialized_start=29721
-  _NOTHINGTODO._serialized_end=29734
-  _NOTHINGTODOMSG._serialized_start=29736
-  _NOTHINGTODOMSG._serialized_end=29830
-  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_start=29832
-  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_end=29876
-  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_start=29879
-  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_end=30009
-  _ENDRUNRESULT._serialized_start=30012
-  _ENDRUNRESULT._serialized_end=30159
-  _ENDRUNRESULTMSG._serialized_start=30161
-  _ENDRUNRESULTMSG._serialized_end=30257
-  _NONODESSELECTED._serialized_start=30259
-  _NONODESSELECTED._serialized_end=30276
-  _NONODESSELECTEDMSG._serialized_start=30278
-  _NONODESSELECTEDMSG._serialized_end=30380
-  _COMMANDCOMPLETED._serialized_start=30382
-  _COMMANDCOMPLETED._serialized_end=30501
-  _COMMANDCOMPLETEDMSG._serialized_start=30503
-  _COMMANDCOMPLETEDMSG._serialized_end=30607
-  _SHOWNODE._serialized_start=30609
-  _SHOWNODE._serialized_end=30716
-  _SHOWNODEMSG._serialized_start=30718
-  _SHOWNODEMSG._serialized_end=30806
-  _COMPILEDNODE._serialized_start=30808
-  _COMPILEDNODE._serialized_end=30920
-  _COMPILEDNODEMSG._serialized_start=30922
-  _COMPILEDNODEMSG._serialized_end=31018
-  _CATCHABLEEXCEPTIONONRUN._serialized_start=31020
-  _CATCHABLEEXCEPTIONONRUN._serialized_end=31118
-  _CATCHABLEEXCEPTIONONRUNMSG._serialized_start=31120
-  _CATCHABLEEXCEPTIONONRUNMSG._serialized_end=31238
-  _INTERNALERRORONRUN._serialized_start=31240
-  _INTERNALERRORONRUN._serialized_end=31293
-  _INTERNALERRORONRUNMSG._serialized_start=31295
-  _INTERNALERRORONRUNMSG._serialized_end=31403
-  _GENERICEXCEPTIONONRUN._serialized_start=31405
-  _GENERICEXCEPTIONONRUN._serialized_end=31480
-  _GENERICEXCEPTIONONRUNMSG._serialized_start=31482
-  _GENERICEXCEPTIONONRUNMSG._serialized_end=31596
-  _NODECONNECTIONRELEASEERROR._serialized_start=31598
-  _NODECONNECTIONRELEASEERROR._serialized_end=31676
-  _NODECONNECTIONRELEASEERRORMSG._serialized_start=31678
-  _NODECONNECTIONRELEASEERRORMSG._serialized_end=31802
-  _FOUNDSTATS._serialized_start=31804
-  _FOUNDSTATS._serialized_end=31835
-  _FOUNDSTATSMSG._serialized_start=31837
-  _FOUNDSTATSMSG._serialized_end=31929
-  _MAINKEYBOARDINTERRUPT._serialized_start=31931
-  _MAINKEYBOARDINTERRUPT._serialized_end=31954
-  _MAINKEYBOARDINTERRUPTMSG._serialized_start=31956
-  _MAINKEYBOARDINTERRUPTMSG._serialized_end=32070
-  _MAINENCOUNTEREDERROR._serialized_start=32072
-  _MAINENCOUNTEREDERROR._serialized_end=32107
-  _MAINENCOUNTEREDERRORMSG._serialized_start=32109
-  _MAINENCOUNTEREDERRORMSG._serialized_end=32221
-  _MAINSTACKTRACE._serialized_start=32223
-  _MAINSTACKTRACE._serialized_end=32260
-  _MAINSTACKTRACEMSG._serialized_start=32262
-  _MAINSTACKTRACEMSG._serialized_end=32362
-  _SYSTEMCOULDNOTWRITE._serialized_start=32364
-  _SYSTEMCOULDNOTWRITE._serialized_end=32428
-  _SYSTEMCOULDNOTWRITEMSG._serialized_start=32430
-  _SYSTEMCOULDNOTWRITEMSG._serialized_end=32540
-  _SYSTEMEXECUTINGCMD._serialized_start=32542
-  _SYSTEMEXECUTINGCMD._serialized_end=32575
-  _SYSTEMEXECUTINGCMDMSG._serialized_start=32577
-  _SYSTEMEXECUTINGCMDMSG._serialized_end=32685
-  _SYSTEMSTDOUT._serialized_start=32687
-  _SYSTEMSTDOUT._serialized_end=32715
-  _SYSTEMSTDOUTMSG._serialized_start=32717
-  _SYSTEMSTDOUTMSG._serialized_end=32813
-  _SYSTEMSTDERR._serialized_start=32815
-  _SYSTEMSTDERR._serialized_end=32843
-  _SYSTEMSTDERRMSG._serialized_start=32845
-  _SYSTEMSTDERRMSG._serialized_end=32941
-  _SYSTEMREPORTRETURNCODE._serialized_start=32943
-  _SYSTEMREPORTRETURNCODE._serialized_end=32987
-  _SYSTEMREPORTRETURNCODEMSG._serialized_start=32989
-  _SYSTEMREPORTRETURNCODEMSG._serialized_end=33105
-  _TIMINGINFOCOLLECTED._serialized_start=33107
-  _TIMINGINFOCOLLECTED._serialized_end=33219
-  _TIMINGINFOCOLLECTEDMSG._serialized_start=33221
-  _TIMINGINFOCOLLECTEDMSG._serialized_end=33331
-  _LOGDEBUGSTACKTRACE._serialized_start=33333
-  _LOGDEBUGSTACKTRACE._serialized_end=33371
-  _LOGDEBUGSTACKTRACEMSG._serialized_start=33373
-  _LOGDEBUGSTACKTRACEMSG._serialized_end=33481
-  _CHECKCLEANPATH._serialized_start=33483
-  _CHECKCLEANPATH._serialized_end=33513
-  _CHECKCLEANPATHMSG._serialized_start=33515
-  _CHECKCLEANPATHMSG._serialized_end=33615
-  _CONFIRMCLEANPATH._serialized_start=33617
-  _CONFIRMCLEANPATH._serialized_end=33649
-  _CONFIRMCLEANPATHMSG._serialized_start=33651
-  _CONFIRMCLEANPATHMSG._serialized_end=33755
-  _PROTECTEDCLEANPATH._serialized_start=33757
-  _PROTECTEDCLEANPATH._serialized_end=33791
-  _PROTECTEDCLEANPATHMSG._serialized_start=33793
-  _PROTECTEDCLEANPATHMSG._serialized_end=33901
-  _FINISHEDCLEANPATHS._serialized_start=33903
-  _FINISHEDCLEANPATHS._serialized_end=33923
-  _FINISHEDCLEANPATHSMSG._serialized_start=33925
-  _FINISHEDCLEANPATHSMSG._serialized_end=34033
-  _OPENCOMMAND._serialized_start=34035
-  _OPENCOMMAND._serialized_end=34088
-  _OPENCOMMANDMSG._serialized_start=34090
-  _OPENCOMMANDMSG._serialized_end=34184
-  _FORMATTING._serialized_start=34186
-  _FORMATTING._serialized_end=34211
-  _FORMATTINGMSG._serialized_start=34213
-  _FORMATTINGMSG._serialized_end=34305
-  _SERVINGDOCSPORT._serialized_start=34307
-  _SERVINGDOCSPORT._serialized_end=34355
-  _SERVINGDOCSPORTMSG._serialized_start=34357
-  _SERVINGDOCSPORTMSG._serialized_end=34459
-  _SERVINGDOCSACCESSINFO._serialized_start=34461
-  _SERVINGDOCSACCESSINFO._serialized_end=34498
-  _SERVINGDOCSACCESSINFOMSG._serialized_start=34500
-  _SERVINGDOCSACCESSINFOMSG._serialized_end=34614
-  _SERVINGDOCSEXITINFO._serialized_start=34616
-  _SERVINGDOCSEXITINFO._serialized_end=34637
-  _SERVINGDOCSEXITINFOMSG._serialized_start=34639
-  _SERVINGDOCSEXITINFOMSG._serialized_end=34749
-  _RUNRESULTWARNING._serialized_start=34751
-  _RUNRESULTWARNING._serialized_end=34825
-  _RUNRESULTWARNINGMSG._serialized_start=34827
-  _RUNRESULTWARNINGMSG._serialized_end=34931
-  _RUNRESULTFAILURE._serialized_start=34933
-  _RUNRESULTFAILURE._serialized_end=35007
-  _RUNRESULTFAILUREMSG._serialized_start=35009
-  _RUNRESULTFAILUREMSG._serialized_end=35113
-  _STATSLINE._serialized_start=35115
-  _STATSLINE._serialized_end=35222
-  _STATSLINE_STATSENTRY._serialized_start=35178
-  _STATSLINE_STATSENTRY._serialized_end=35222
-  _STATSLINEMSG._serialized_start=35224
-  _STATSLINEMSG._serialized_end=35314
-  _RUNRESULTERROR._serialized_start=35316
-  _RUNRESULTERROR._serialized_end=35345
-  _RUNRESULTERRORMSG._serialized_start=35347
-  _RUNRESULTERRORMSG._serialized_end=35447
-  _RUNRESULTERRORNOMESSAGE._serialized_start=35449
-  _RUNRESULTERRORNOMESSAGE._serialized_end=35490
-  _RUNRESULTERRORNOMESSAGEMSG._serialized_start=35492
-  _RUNRESULTERRORNOMESSAGEMSG._serialized_end=35610
-  _SQLCOMPILEDPATH._serialized_start=35612
-  _SQLCOMPILEDPATH._serialized_end=35643
-  _SQLCOMPILEDPATHMSG._serialized_start=35645
-  _SQLCOMPILEDPATHMSG._serialized_end=35747
-  _CHECKNODETESTFAILURE._serialized_start=35749
-  _CHECKNODETESTFAILURE._serialized_end=35794
-  _CHECKNODETESTFAILUREMSG._serialized_start=35796
-  _CHECKNODETESTFAILUREMSG._serialized_end=35908
-  _FIRSTRUNRESULTERROR._serialized_start=35910
-  _FIRSTRUNRESULTERROR._serialized_end=35944
-  _FIRSTRUNRESULTERRORMSG._serialized_start=35946
-  _FIRSTRUNRESULTERRORMSG._serialized_end=36056
-  _AFTERFIRSTRUNRESULTERROR._serialized_start=36058
-  _AFTERFIRSTRUNRESULTERROR._serialized_end=36097
-  _AFTERFIRSTRUNRESULTERRORMSG._serialized_start=36099
-  _AFTERFIRSTRUNRESULTERRORMSG._serialized_end=36219
-  _ENDOFRUNSUMMARY._serialized_start=36221
-  _ENDOFRUNSUMMARY._serialized_end=36308
-  _ENDOFRUNSUMMARYMSG._serialized_start=36310
-  _ENDOFRUNSUMMARYMSG._serialized_end=36412
-  _LOGSKIPBECAUSEERROR._serialized_start=36414
-  _LOGSKIPBECAUSEERROR._serialized_end=36499
-  _LOGSKIPBECAUSEERRORMSG._serialized_start=36501
-  _LOGSKIPBECAUSEERRORMSG._serialized_end=36611
-  _ENSUREGITINSTALLED._serialized_start=36613
-  _ENSUREGITINSTALLED._serialized_end=36633
-  _ENSUREGITINSTALLEDMSG._serialized_start=36635
-  _ENSUREGITINSTALLEDMSG._serialized_end=36743
-  _DEPSCREATINGLOCALSYMLINK._serialized_start=36745
-  _DEPSCREATINGLOCALSYMLINK._serialized_end=36771
-  _DEPSCREATINGLOCALSYMLINKMSG._serialized_start=36773
-  _DEPSCREATINGLOCALSYMLINKMSG._serialized_end=36893
-  _DEPSSYMLINKNOTAVAILABLE._serialized_start=36895
-  _DEPSSYMLINKNOTAVAILABLE._serialized_end=36920
-  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_start=36922
-  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_end=37040
-  _DISABLETRACKING._serialized_start=37042
-  _DISABLETRACKING._serialized_end=37059
-  _DISABLETRACKINGMSG._serialized_start=37061
-  _DISABLETRACKINGMSG._serialized_end=37163
-  _SENDINGEVENT._serialized_start=37165
-  _SENDINGEVENT._serialized_end=37195
-  _SENDINGEVENTMSG._serialized_start=37197
-  _SENDINGEVENTMSG._serialized_end=37293
-  _SENDEVENTFAILURE._serialized_start=37295
-  _SENDEVENTFAILURE._serialized_end=37313
-  _SENDEVENTFAILUREMSG._serialized_start=37315
-  _SENDEVENTFAILUREMSG._serialized_end=37419
-  _FLUSHEVENTS._serialized_start=37421
-  _FLUSHEVENTS._serialized_end=37434
-  _FLUSHEVENTSMSG._serialized_start=37436
-  _FLUSHEVENTSMSG._serialized_end=37530
-  _FLUSHEVENTSFAILURE._serialized_start=37532
-  _FLUSHEVENTSFAILURE._serialized_end=37552
-  _FLUSHEVENTSFAILUREMSG._serialized_start=37554
-  _FLUSHEVENTSFAILUREMSG._serialized_end=37662
-  _TRACKINGINITIALIZEFAILURE._serialized_start=37664
-  _TRACKINGINITIALIZEFAILURE._serialized_end=37709
-  _TRACKINGINITIALIZEFAILUREMSG._serialized_start=37711
-  _TRACKINGINITIALIZEFAILUREMSG._serialized_end=37833
-  _RUNRESULTWARNINGMESSAGE._serialized_start=37835
-  _RUNRESULTWARNINGMESSAGE._serialized_end=37873
-  _RUNRESULTWARNINGMESSAGEMSG._serialized_start=37875
-  _RUNRESULTWARNINGMESSAGEMSG._serialized_end=37993
-  _DEBUGCMDOUT._serialized_start=37995
-  _DEBUGCMDOUT._serialized_end=38021
-  _DEBUGCMDOUTMSG._serialized_start=38023
-  _DEBUGCMDOUTMSG._serialized_end=38117
-  _DEBUGCMDRESULT._serialized_start=38119
-  _DEBUGCMDRESULT._serialized_end=38148
-  _DEBUGCMDRESULTMSG._serialized_start=38150
-  _DEBUGCMDRESULTMSG._serialized_end=38250
-  _LISTCMDOUT._serialized_start=38252
-  _LISTCMDOUT._serialized_end=38277
-  _LISTCMDOUTMSG._serialized_start=38279
-  _LISTCMDOUTMSG._serialized_end=38371
-  _NOTE._serialized_start=38373
-  _NOTE._serialized_end=38392
-  _NOTEMSG._serialized_start=38394
-  _NOTEMSG._serialized_end=38474
+  _UNSUPPORTEDCONSTRAINTMATERIALIZATION._serialized_start=20055
+  _UNSUPPORTEDCONSTRAINTMATERIALIZATION._serialized_end=20115
+  _UNSUPPORTEDCONSTRAINTMATERIALIZATIONMSG._serialized_start=20118
+  _UNSUPPORTEDCONSTRAINTMATERIALIZATIONMSG._serialized_end=20262
+  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_start=20264
+  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_end=20311
+  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_start=20314
+  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_end=20444
+  _GITPROGRESSCHECKOUTREVISION._serialized_start=20446
+  _GITPROGRESSCHECKOUTREVISION._serialized_end=20493
+  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_start=20495
+  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_end=20621
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_start=20623
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_end=20675
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_start=20678
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_end=20824
+  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_start=20826
+  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_end=20872
+  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_start=20875
+  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_end=21009
+  _GITNOTHINGTODO._serialized_start=21011
+  _GITNOTHINGTODO._serialized_end=21040
+  _GITNOTHINGTODOMSG._serialized_start=21042
+  _GITNOTHINGTODOMSG._serialized_end=21142
+  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_start=21144
+  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_end=21213
+  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_start=21216
+  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_end=21350
+  _GITPROGRESSCHECKEDOUTAT._serialized_start=21352
+  _GITPROGRESSCHECKEDOUTAT._serialized_end=21394
+  _GITPROGRESSCHECKEDOUTATMSG._serialized_start=21396
+  _GITPROGRESSCHECKEDOUTATMSG._serialized_end=21514
+  _REGISTRYPROGRESSGETREQUEST._serialized_start=21516
+  _REGISTRYPROGRESSGETREQUEST._serialized_end=21557
+  _REGISTRYPROGRESSGETREQUESTMSG._serialized_start=21559
+  _REGISTRYPROGRESSGETREQUESTMSG._serialized_end=21683
+  _REGISTRYPROGRESSGETRESPONSE._serialized_start=21685
+  _REGISTRYPROGRESSGETRESPONSE._serialized_end=21746
+  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_start=21748
+  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_end=21874
+  _SELECTORREPORTINVALIDSELECTOR._serialized_start=21876
+  _SELECTORREPORTINVALIDSELECTOR._serialized_end=21971
+  _SELECTORREPORTINVALIDSELECTORMSG._serialized_start=21974
+  _SELECTORREPORTINVALIDSELECTORMSG._serialized_end=22104
+  _DEPSNOPACKAGESFOUND._serialized_start=22106
+  _DEPSNOPACKAGESFOUND._serialized_end=22127
+  _DEPSNOPACKAGESFOUNDMSG._serialized_start=22129
+  _DEPSNOPACKAGESFOUNDMSG._serialized_end=22239
+  _DEPSSTARTPACKAGEINSTALL._serialized_start=22241
+  _DEPSSTARTPACKAGEINSTALL._serialized_end=22288
+  _DEPSSTARTPACKAGEINSTALLMSG._serialized_start=22290
+  _DEPSSTARTPACKAGEINSTALLMSG._serialized_end=22408
+  _DEPSINSTALLINFO._serialized_start=22410
+  _DEPSINSTALLINFO._serialized_end=22449
+  _DEPSINSTALLINFOMSG._serialized_start=22451
+  _DEPSINSTALLINFOMSG._serialized_end=22553
+  _DEPSUPDATEAVAILABLE._serialized_start=22555
+  _DEPSUPDATEAVAILABLE._serialized_end=22600
+  _DEPSUPDATEAVAILABLEMSG._serialized_start=22602
+  _DEPSUPDATEAVAILABLEMSG._serialized_end=22712
+  _DEPSUPTODATE._serialized_start=22714
+  _DEPSUPTODATE._serialized_end=22728
+  _DEPSUPTODATEMSG._serialized_start=22730
+  _DEPSUPTODATEMSG._serialized_end=22826
+  _DEPSLISTSUBDIRECTORY._serialized_start=22828
+  _DEPSLISTSUBDIRECTORY._serialized_end=22872
+  _DEPSLISTSUBDIRECTORYMSG._serialized_start=22874
+  _DEPSLISTSUBDIRECTORYMSG._serialized_end=22986
+  _DEPSNOTIFYUPDATESAVAILABLE._serialized_start=22988
+  _DEPSNOTIFYUPDATESAVAILABLE._serialized_end=23034
+  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_start=23036
+  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_end=23160
+  _RETRYEXTERNALCALL._serialized_start=23162
+  _RETRYEXTERNALCALL._serialized_end=23211
+  _RETRYEXTERNALCALLMSG._serialized_start=23213
+  _RETRYEXTERNALCALLMSG._serialized_end=23319
+  _RECORDRETRYEXCEPTION._serialized_start=23321
+  _RECORDRETRYEXCEPTION._serialized_end=23356
+  _RECORDRETRYEXCEPTIONMSG._serialized_start=23358
+  _RECORDRETRYEXCEPTIONMSG._serialized_end=23470
+  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_start=23472
+  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_end=23518
+  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_start=23521
+  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_end=23655
+  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_start=23657
+  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_end=23723
+  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_start=23726
+  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_end=23862
+  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_start=23864
+  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_end=23914
+  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_start=23917
+  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_end=24049
+  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_start=24051
+  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_end=24101
+  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_start=24104
+  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_end=24236
+  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_start=24238
+  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_end=24291
+  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_start=24294
+  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_end=24432
+  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_start=24434
+  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_end=24485
+  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_start=24488
+  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_end=24622
+  _DEPSSETDOWNLOADDIRECTORY._serialized_start=24624
+  _DEPSSETDOWNLOADDIRECTORY._serialized_end=24664
+  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_start=24666
+  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_end=24786
+  _DEPSUNPINNED._serialized_start=24788
+  _DEPSUNPINNED._serialized_end=24833
+  _DEPSUNPINNEDMSG._serialized_start=24835
+  _DEPSUNPINNEDMSG._serialized_end=24931
+  _NONODESFORSELECTIONCRITERIA._serialized_start=24933
+  _NONODESFORSELECTIONCRITERIA._serialized_end=24980
+  _NONODESFORSELECTIONCRITERIAMSG._serialized_start=24982
+  _NONODESFORSELECTIONCRITERIAMSG._serialized_end=25108
+  _PUBLICATIONARTIFACTAVAILABLE._serialized_start=25110
+  _PUBLICATIONARTIFACTAVAILABLE._serialized_end=25187
+  _PUBLICATIONARTIFACTAVAILABLEMSG._serialized_start=25190
+  _PUBLICATIONARTIFACTAVAILABLEMSG._serialized_end=25318
+  _RUNNINGOPERATIONCAUGHTERROR._serialized_start=25320
+  _RUNNINGOPERATIONCAUGHTERROR._serialized_end=25362
+  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_start=25364
+  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_end=25490
+  _COMPILECOMPLETE._serialized_start=25492
+  _COMPILECOMPLETE._serialized_end=25509
+  _COMPILECOMPLETEMSG._serialized_start=25511
+  _COMPILECOMPLETEMSG._serialized_end=25613
+  _FRESHNESSCHECKCOMPLETE._serialized_start=25615
+  _FRESHNESSCHECKCOMPLETE._serialized_end=25639
+  _FRESHNESSCHECKCOMPLETEMSG._serialized_start=25641
+  _FRESHNESSCHECKCOMPLETEMSG._serialized_end=25757
+  _SEEDHEADER._serialized_start=25759
+  _SEEDHEADER._serialized_end=25787
+  _SEEDHEADERMSG._serialized_start=25789
+  _SEEDHEADERMSG._serialized_end=25881
+  _SQLRUNNEREXCEPTION._serialized_start=25883
+  _SQLRUNNEREXCEPTION._serialized_end=25934
+  _SQLRUNNEREXCEPTIONMSG._serialized_start=25936
+  _SQLRUNNEREXCEPTIONMSG._serialized_end=26044
+  _LOGTESTRESULT._serialized_start=26047
+  _LOGTESTRESULT._serialized_end=26215
+  _LOGTESTRESULTMSG._serialized_start=26217
+  _LOGTESTRESULTMSG._serialized_end=26315
+  _LOGSTARTLINE._serialized_start=26317
+  _LOGSTARTLINE._serialized_end=26424
+  _LOGSTARTLINEMSG._serialized_start=26426
+  _LOGSTARTLINEMSG._serialized_end=26522
+  _LOGMODELRESULT._serialized_start=26525
+  _LOGMODELRESULT._serialized_end=26674
+  _LOGMODELRESULTMSG._serialized_start=26676
+  _LOGMODELRESULTMSG._serialized_end=26776
+  _LOGSNAPSHOTRESULT._serialized_start=26779
+  _LOGSNAPSHOTRESULT._serialized_end=27029
+  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_start=26987
+  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_end=27029
+  _LOGSNAPSHOTRESULTMSG._serialized_start=27031
+  _LOGSNAPSHOTRESULTMSG._serialized_end=27137
+  _LOGSEEDRESULT._serialized_start=27140
+  _LOGSEEDRESULT._serialized_end=27325
+  _LOGSEEDRESULTMSG._serialized_start=27327
+  _LOGSEEDRESULTMSG._serialized_end=27425
+  _LOGFRESHNESSRESULT._serialized_start=27428
+  _LOGFRESHNESSRESULT._serialized_end=27601
+  _LOGFRESHNESSRESULTMSG._serialized_start=27603
+  _LOGFRESHNESSRESULTMSG._serialized_end=27711
+  _LOGCANCELLINE._serialized_start=27713
+  _LOGCANCELLINE._serialized_end=27747
+  _LOGCANCELLINEMSG._serialized_start=27749
+  _LOGCANCELLINEMSG._serialized_end=27847
+  _DEFAULTSELECTOR._serialized_start=27849
+  _DEFAULTSELECTOR._serialized_end=27880
+  _DEFAULTSELECTORMSG._serialized_start=27882
+  _DEFAULTSELECTORMSG._serialized_end=27984
+  _NODESTART._serialized_start=27986
+  _NODESTART._serialized_end=28039
+  _NODESTARTMSG._serialized_start=28041
+  _NODESTARTMSG._serialized_end=28131
+  _NODEFINISHED._serialized_start=28133
+  _NODEFINISHED._serialized_end=28236
+  _NODEFINISHEDMSG._serialized_start=28238
+  _NODEFINISHEDMSG._serialized_end=28334
+  _QUERYCANCELATIONUNSUPPORTED._serialized_start=28336
+  _QUERYCANCELATIONUNSUPPORTED._serialized_end=28379
+  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_start=28381
+  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_end=28507
+  _CONCURRENCYLINE._serialized_start=28509
+  _CONCURRENCYLINE._serialized_end=28588
+  _CONCURRENCYLINEMSG._serialized_start=28590
+  _CONCURRENCYLINEMSG._serialized_end=28692
+  _WRITINGINJECTEDSQLFORNODE._serialized_start=28694
+  _WRITINGINJECTEDSQLFORNODE._serialized_end=28763
+  _WRITINGINJECTEDSQLFORNODEMSG._serialized_start=28765
+  _WRITINGINJECTEDSQLFORNODEMSG._serialized_end=28887
+  _NODECOMPILING._serialized_start=28889
+  _NODECOMPILING._serialized_end=28946
+  _NODECOMPILINGMSG._serialized_start=28948
+  _NODECOMPILINGMSG._serialized_end=29046
+  _NODEEXECUTING._serialized_start=29048
+  _NODEEXECUTING._serialized_end=29105
+  _NODEEXECUTINGMSG._serialized_start=29107
+  _NODEEXECUTINGMSG._serialized_end=29205
+  _LOGHOOKSTARTLINE._serialized_start=29207
+  _LOGHOOKSTARTLINE._serialized_end=29316
+  _LOGHOOKSTARTLINEMSG._serialized_start=29318
+  _LOGHOOKSTARTLINEMSG._serialized_end=29422
+  _LOGHOOKENDLINE._serialized_start=29425
+  _LOGHOOKENDLINE._serialized_end=29572
+  _LOGHOOKENDLINEMSG._serialized_start=29574
+  _LOGHOOKENDLINEMSG._serialized_end=29674
+  _SKIPPINGDETAILS._serialized_start=29677
+  _SKIPPINGDETAILS._serialized_end=29824
+  _SKIPPINGDETAILSMSG._serialized_start=29826
+  _SKIPPINGDETAILSMSG._serialized_end=29928
+  _NOTHINGTODO._serialized_start=29930
+  _NOTHINGTODO._serialized_end=29943
+  _NOTHINGTODOMSG._serialized_start=29945
+  _NOTHINGTODOMSG._serialized_end=30039
+  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_start=30041
+  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_end=30085
+  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_start=30088
+  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_end=30218
+  _ENDRUNRESULT._serialized_start=30221
+  _ENDRUNRESULT._serialized_end=30368
+  _ENDRUNRESULTMSG._serialized_start=30370
+  _ENDRUNRESULTMSG._serialized_end=30466
+  _NONODESSELECTED._serialized_start=30468
+  _NONODESSELECTED._serialized_end=30485
+  _NONODESSELECTEDMSG._serialized_start=30487
+  _NONODESSELECTEDMSG._serialized_end=30589
+  _COMMANDCOMPLETED._serialized_start=30591
+  _COMMANDCOMPLETED._serialized_end=30710
+  _COMMANDCOMPLETEDMSG._serialized_start=30712
+  _COMMANDCOMPLETEDMSG._serialized_end=30816
+  _SHOWNODE._serialized_start=30818
+  _SHOWNODE._serialized_end=30925
+  _SHOWNODEMSG._serialized_start=30927
+  _SHOWNODEMSG._serialized_end=31015
+  _COMPILEDNODE._serialized_start=31017
+  _COMPILEDNODE._serialized_end=31129
+  _COMPILEDNODEMSG._serialized_start=31131
+  _COMPILEDNODEMSG._serialized_end=31227
+  _CATCHABLEEXCEPTIONONRUN._serialized_start=31229
+  _CATCHABLEEXCEPTIONONRUN._serialized_end=31327
+  _CATCHABLEEXCEPTIONONRUNMSG._serialized_start=31329
+  _CATCHABLEEXCEPTIONONRUNMSG._serialized_end=31447
+  _INTERNALERRORONRUN._serialized_start=31449
+  _INTERNALERRORONRUN._serialized_end=31502
+  _INTERNALERRORONRUNMSG._serialized_start=31504
+  _INTERNALERRORONRUNMSG._serialized_end=31612
+  _GENERICEXCEPTIONONRUN._serialized_start=31614
+  _GENERICEXCEPTIONONRUN._serialized_end=31689
+  _GENERICEXCEPTIONONRUNMSG._serialized_start=31691
+  _GENERICEXCEPTIONONRUNMSG._serialized_end=31805
+  _NODECONNECTIONRELEASEERROR._serialized_start=31807
+  _NODECONNECTIONRELEASEERROR._serialized_end=31885
+  _NODECONNECTIONRELEASEERRORMSG._serialized_start=31887
+  _NODECONNECTIONRELEASEERRORMSG._serialized_end=32011
+  _FOUNDSTATS._serialized_start=32013
+  _FOUNDSTATS._serialized_end=32044
+  _FOUNDSTATSMSG._serialized_start=32046
+  _FOUNDSTATSMSG._serialized_end=32138
+  _MAINKEYBOARDINTERRUPT._serialized_start=32140
+  _MAINKEYBOARDINTERRUPT._serialized_end=32163
+  _MAINKEYBOARDINTERRUPTMSG._serialized_start=32165
+  _MAINKEYBOARDINTERRUPTMSG._serialized_end=32279
+  _MAINENCOUNTEREDERROR._serialized_start=32281
+  _MAINENCOUNTEREDERROR._serialized_end=32316
+  _MAINENCOUNTEREDERRORMSG._serialized_start=32318
+  _MAINENCOUNTEREDERRORMSG._serialized_end=32430
+  _MAINSTACKTRACE._serialized_start=32432
+  _MAINSTACKTRACE._serialized_end=32469
+  _MAINSTACKTRACEMSG._serialized_start=32471
+  _MAINSTACKTRACEMSG._serialized_end=32571
+  _SYSTEMCOULDNOTWRITE._serialized_start=32573
+  _SYSTEMCOULDNOTWRITE._serialized_end=32637
+  _SYSTEMCOULDNOTWRITEMSG._serialized_start=32639
+  _SYSTEMCOULDNOTWRITEMSG._serialized_end=32749
+  _SYSTEMEXECUTINGCMD._serialized_start=32751
+  _SYSTEMEXECUTINGCMD._serialized_end=32784
+  _SYSTEMEXECUTINGCMDMSG._serialized_start=32786
+  _SYSTEMEXECUTINGCMDMSG._serialized_end=32894
+  _SYSTEMSTDOUT._serialized_start=32896
+  _SYSTEMSTDOUT._serialized_end=32924
+  _SYSTEMSTDOUTMSG._serialized_start=32926
+  _SYSTEMSTDOUTMSG._serialized_end=33022
+  _SYSTEMSTDERR._serialized_start=33024
+  _SYSTEMSTDERR._serialized_end=33052
+  _SYSTEMSTDERRMSG._serialized_start=33054
+  _SYSTEMSTDERRMSG._serialized_end=33150
+  _SYSTEMREPORTRETURNCODE._serialized_start=33152
+  _SYSTEMREPORTRETURNCODE._serialized_end=33196
+  _SYSTEMREPORTRETURNCODEMSG._serialized_start=33198
+  _SYSTEMREPORTRETURNCODEMSG._serialized_end=33314
+  _TIMINGINFOCOLLECTED._serialized_start=33316
+  _TIMINGINFOCOLLECTED._serialized_end=33428
+  _TIMINGINFOCOLLECTEDMSG._serialized_start=33430
+  _TIMINGINFOCOLLECTEDMSG._serialized_end=33540
+  _LOGDEBUGSTACKTRACE._serialized_start=33542
+  _LOGDEBUGSTACKTRACE._serialized_end=33580
+  _LOGDEBUGSTACKTRACEMSG._serialized_start=33582
+  _LOGDEBUGSTACKTRACEMSG._serialized_end=33690
+  _CHECKCLEANPATH._serialized_start=33692
+  _CHECKCLEANPATH._serialized_end=33722
+  _CHECKCLEANPATHMSG._serialized_start=33724
+  _CHECKCLEANPATHMSG._serialized_end=33824
+  _CONFIRMCLEANPATH._serialized_start=33826
+  _CONFIRMCLEANPATH._serialized_end=33858
+  _CONFIRMCLEANPATHMSG._serialized_start=33860
+  _CONFIRMCLEANPATHMSG._serialized_end=33964
+  _PROTECTEDCLEANPATH._serialized_start=33966
+  _PROTECTEDCLEANPATH._serialized_end=34000
+  _PROTECTEDCLEANPATHMSG._serialized_start=34002
+  _PROTECTEDCLEANPATHMSG._serialized_end=34110
+  _FINISHEDCLEANPATHS._serialized_start=34112
+  _FINISHEDCLEANPATHS._serialized_end=34132
+  _FINISHEDCLEANPATHSMSG._serialized_start=34134
+  _FINISHEDCLEANPATHSMSG._serialized_end=34242
+  _OPENCOMMAND._serialized_start=34244
+  _OPENCOMMAND._serialized_end=34297
+  _OPENCOMMANDMSG._serialized_start=34299
+  _OPENCOMMANDMSG._serialized_end=34393
+  _FORMATTING._serialized_start=34395
+  _FORMATTING._serialized_end=34420
+  _FORMATTINGMSG._serialized_start=34422
+  _FORMATTINGMSG._serialized_end=34514
+  _SERVINGDOCSPORT._serialized_start=34516
+  _SERVINGDOCSPORT._serialized_end=34564
+  _SERVINGDOCSPORTMSG._serialized_start=34566
+  _SERVINGDOCSPORTMSG._serialized_end=34668
+  _SERVINGDOCSACCESSINFO._serialized_start=34670
+  _SERVINGDOCSACCESSINFO._serialized_end=34707
+  _SERVINGDOCSACCESSINFOMSG._serialized_start=34709
+  _SERVINGDOCSACCESSINFOMSG._serialized_end=34823
+  _SERVINGDOCSEXITINFO._serialized_start=34825
+  _SERVINGDOCSEXITINFO._serialized_end=34846
+  _SERVINGDOCSEXITINFOMSG._serialized_start=34848
+  _SERVINGDOCSEXITINFOMSG._serialized_end=34958
+  _RUNRESULTWARNING._serialized_start=34960
+  _RUNRESULTWARNING._serialized_end=35034
+  _RUNRESULTWARNINGMSG._serialized_start=35036
+  _RUNRESULTWARNINGMSG._serialized_end=35140
+  _RUNRESULTFAILURE._serialized_start=35142
+  _RUNRESULTFAILURE._serialized_end=35216
+  _RUNRESULTFAILUREMSG._serialized_start=35218
+  _RUNRESULTFAILUREMSG._serialized_end=35322
+  _STATSLINE._serialized_start=35324
+  _STATSLINE._serialized_end=35431
+  _STATSLINE_STATSENTRY._serialized_start=35387
+  _STATSLINE_STATSENTRY._serialized_end=35431
+  _STATSLINEMSG._serialized_start=35433
+  _STATSLINEMSG._serialized_end=35523
+  _RUNRESULTERROR._serialized_start=35525
+  _RUNRESULTERROR._serialized_end=35554
+  _RUNRESULTERRORMSG._serialized_start=35556
+  _RUNRESULTERRORMSG._serialized_end=35656
+  _RUNRESULTERRORNOMESSAGE._serialized_start=35658
+  _RUNRESULTERRORNOMESSAGE._serialized_end=35699
+  _RUNRESULTERRORNOMESSAGEMSG._serialized_start=35701
+  _RUNRESULTERRORNOMESSAGEMSG._serialized_end=35819
+  _SQLCOMPILEDPATH._serialized_start=35821
+  _SQLCOMPILEDPATH._serialized_end=35852
+  _SQLCOMPILEDPATHMSG._serialized_start=35854
+  _SQLCOMPILEDPATHMSG._serialized_end=35956
+  _CHECKNODETESTFAILURE._serialized_start=35958
+  _CHECKNODETESTFAILURE._serialized_end=36003
+  _CHECKNODETESTFAILUREMSG._serialized_start=36005
+  _CHECKNODETESTFAILUREMSG._serialized_end=36117
+  _FIRSTRUNRESULTERROR._serialized_start=36119
+  _FIRSTRUNRESULTERROR._serialized_end=36153
+  _FIRSTRUNRESULTERRORMSG._serialized_start=36155
+  _FIRSTRUNRESULTERRORMSG._serialized_end=36265
+  _AFTERFIRSTRUNRESULTERROR._serialized_start=36267
+  _AFTERFIRSTRUNRESULTERROR._serialized_end=36306
+  _AFTERFIRSTRUNRESULTERRORMSG._serialized_start=36308
+  _AFTERFIRSTRUNRESULTERRORMSG._serialized_end=36428
+  _ENDOFRUNSUMMARY._serialized_start=36430
+  _ENDOFRUNSUMMARY._serialized_end=36517
+  _ENDOFRUNSUMMARYMSG._serialized_start=36519
+  _ENDOFRUNSUMMARYMSG._serialized_end=36621
+  _LOGSKIPBECAUSEERROR._serialized_start=36623
+  _LOGSKIPBECAUSEERROR._serialized_end=36708
+  _LOGSKIPBECAUSEERRORMSG._serialized_start=36710
+  _LOGSKIPBECAUSEERRORMSG._serialized_end=36820
+  _ENSUREGITINSTALLED._serialized_start=36822
+  _ENSUREGITINSTALLED._serialized_end=36842
+  _ENSUREGITINSTALLEDMSG._serialized_start=36844
+  _ENSUREGITINSTALLEDMSG._serialized_end=36952
+  _DEPSCREATINGLOCALSYMLINK._serialized_start=36954
+  _DEPSCREATINGLOCALSYMLINK._serialized_end=36980
+  _DEPSCREATINGLOCALSYMLINKMSG._serialized_start=36982
+  _DEPSCREATINGLOCALSYMLINKMSG._serialized_end=37102
+  _DEPSSYMLINKNOTAVAILABLE._serialized_start=37104
+  _DEPSSYMLINKNOTAVAILABLE._serialized_end=37129
+  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_start=37131
+  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_end=37249
+  _DISABLETRACKING._serialized_start=37251
+  _DISABLETRACKING._serialized_end=37268
+  _DISABLETRACKINGMSG._serialized_start=37270
+  _DISABLETRACKINGMSG._serialized_end=37372
+  _SENDINGEVENT._serialized_start=37374
+  _SENDINGEVENT._serialized_end=37404
+  _SENDINGEVENTMSG._serialized_start=37406
+  _SENDINGEVENTMSG._serialized_end=37502
+  _SENDEVENTFAILURE._serialized_start=37504
+  _SENDEVENTFAILURE._serialized_end=37522
+  _SENDEVENTFAILUREMSG._serialized_start=37524
+  _SENDEVENTFAILUREMSG._serialized_end=37628
+  _FLUSHEVENTS._serialized_start=37630
+  _FLUSHEVENTS._serialized_end=37643
+  _FLUSHEVENTSMSG._serialized_start=37645
+  _FLUSHEVENTSMSG._serialized_end=37739
+  _FLUSHEVENTSFAILURE._serialized_start=37741
+  _FLUSHEVENTSFAILURE._serialized_end=37761
+  _FLUSHEVENTSFAILUREMSG._serialized_start=37763
+  _FLUSHEVENTSFAILUREMSG._serialized_end=37871
+  _TRACKINGINITIALIZEFAILURE._serialized_start=37873
+  _TRACKINGINITIALIZEFAILURE._serialized_end=37918
+  _TRACKINGINITIALIZEFAILUREMSG._serialized_start=37920
+  _TRACKINGINITIALIZEFAILUREMSG._serialized_end=38042
+  _RUNRESULTWARNINGMESSAGE._serialized_start=38044
+  _RUNRESULTWARNINGMESSAGE._serialized_end=38082
+  _RUNRESULTWARNINGMESSAGEMSG._serialized_start=38084
+  _RUNRESULTWARNINGMESSAGEMSG._serialized_end=38202
+  _DEBUGCMDOUT._serialized_start=38204
+  _DEBUGCMDOUT._serialized_end=38230
+  _DEBUGCMDOUTMSG._serialized_start=38232
+  _DEBUGCMDOUTMSG._serialized_end=38326
+  _DEBUGCMDRESULT._serialized_start=38328
+  _DEBUGCMDRESULT._serialized_end=38357
+  _DEBUGCMDRESULTMSG._serialized_start=38359
+  _DEBUGCMDRESULTMSG._serialized_end=38459
+  _LISTCMDOUT._serialized_start=38461
+  _LISTCMDOUT._serialized_end=38486
+  _LISTCMDOUTMSG._serialized_start=38488
+  _LISTCMDOUTMSG._serialized_end=38580
+  _NOTE._serialized_start=38582
+  _NOTE._serialized_end=38601
+  _NOTEMSG._serialized_start=38603
+  _NOTEMSG._serialized_end=38683
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dbt-core-1.6.0b2/dbt/exceptions.py` & `dbt-core-1.6.0b3/dbt/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1250,20 +1250,23 @@
         return (
             f"Node {self.unique_id} attempted to reference node {self.ref_unique_id}, "
             f"which is not allowed because the referenced node is private to the {self.group} group."
         )
 
 
 class InvalidAccessTypeError(ParsingError):
-    def __init__(self, unique_id: str, field_value: str):
+    def __init__(self, unique_id: str, field_value: str, materialization: Optional[str] = None):
         self.unique_id = unique_id
         self.field_value = field_value
-        msg = (
-            f"Node {self.unique_id} has an invalid value ({self.field_value}) for the access field"
+        self.materialization = materialization
+
+        with_materialization = (
+            f"with '{self.materialization}' materialization " if self.materialization else ""
         )
+        msg = f"Node {self.unique_id} {with_materialization}has an invalid value ({self.field_value}) for the access field"
         super().__init__(msg=msg)
 
 
 class SameKeyNestedError(CompilationError):
     def __init__(self):
         msg = "Test cannot have the same key at the top-level and in config"
         super().__init__(msg=msg)
```

### Comparing `dbt-core-1.6.0b2/dbt/flags.py` & `dbt-core-1.6.0b3/dbt/flags.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/graph/cli.py` & `dbt-core-1.6.0b3/dbt/graph/cli.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/graph/graph.py` & `dbt-core-1.6.0b3/dbt/graph/graph.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/graph/queue.py` & `dbt-core-1.6.0b3/dbt/graph/queue.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/graph/selector.py` & `dbt-core-1.6.0b3/dbt/graph/selector.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/graph/selector_methods.py` & `dbt-core-1.6.0b3/dbt/graph/selector_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 SELECTOR_DELIMITER = ":"
 
 
 class MethodName(StrEnum):
     FQN = "fqn"
     Tag = "tag"
     Group = "group"
+    Access = "access"
     Source = "source"
     Path = "path"
     File = "file"
     Package = "package"
     Config = "config"
     TestName = "test_name"
     TestType = "test_type"
@@ -226,14 +227,24 @@
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """yields nodes from included in the specified group"""
         for node, real_node in self.groupable_nodes(included_nodes):
             if selector == real_node.config.get("group"):
                 yield node
 
 
+class AccessSelectorMethod(SelectorMethod):
+    def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
+        """yields model nodes matching the specified access level"""
+        for node, real_node in self.parsed_nodes(included_nodes):
+            if not isinstance(real_node, ModelNode):
+                continue
+            if selector == real_node.access:
+                yield node
+
+
 class SourceSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """yields nodes from included are the specified source."""
         parts = selector.split(".")
         target_package = SELECTOR_GLOB
         if len(parts) == 1:
             target_source, target_table = parts[0], SELECTOR_GLOB
@@ -709,14 +720,15 @@
 
 
 class MethodManager:
     SELECTOR_METHODS: Dict[MethodName, Type[SelectorMethod]] = {
         MethodName.FQN: QualifiedNameSelectorMethod,
         MethodName.Tag: TagSelectorMethod,
         MethodName.Group: GroupSelectorMethod,
+        MethodName.Access: AccessSelectorMethod,
         MethodName.Source: SourceSelectorMethod,
         MethodName.Path: PathSelectorMethod,
         MethodName.File: FileSelectorMethod,
         MethodName.Package: PackageSelectorMethod,
         MethodName.Config: ConfigSelectorMethod,
         MethodName.TestName: TestNameSelectorMethod,
         MethodName.TestType: TestTypeSelectorMethod,
```

### Comparing `dbt-core-1.6.0b2/dbt/graph/selector_spec.py` & `dbt-core-1.6.0b3/dbt/graph/selector_spec.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/helper_types.py` & `dbt-core-1.6.0b3/dbt/helper_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/README.md` & `dbt-core-1.6.0b3/dbt/include/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/docs/overview.md` & `dbt-core-1.6.0b3/dbt/include/global_project/docs/overview.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/apply_grants.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/columns.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/columns.sql`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,26 @@
   {% for row in table %}
     {% do columns.append(api.Column(*row)) %}
   {% endfor %}
   {{ return(columns) }}
 {% endmacro %}
 
 
-{% macro get_empty_subquery_sql(select_sql) -%}
-  {{ return(adapter.dispatch('get_empty_subquery_sql', 'dbt')(select_sql)) }}
+{% macro get_empty_subquery_sql(select_sql, select_sql_header=none) -%}
+  {{ return(adapter.dispatch('get_empty_subquery_sql', 'dbt')(select_sql, select_sql_header)) }}
 {% endmacro %}
 
 {#
   Builds a query that results in the same schema as the given select_sql statement, without necessitating a data scan.
   Useful for running a query in a 'pre-flight' context, such as model contract enforcement (assert_columns_equivalent macro).
 #}
-{% macro default__get_empty_subquery_sql(select_sql) %}
+{% macro default__get_empty_subquery_sql(select_sql, select_sql_header=none) %}
+    {%- if select_sql_header is not none -%}
+    {{ select_sql_header }}
+    {%- endif -%}
     select * from (
         {{ select_sql }}
     ) as __dbt_sbq
     where false
     limit 0
 {% endmacro %}
 
@@ -49,18 +52,18 @@
       cast(null as {{ col['data_type'] }}) as {{ col['name'] }}{{ ", " if not loop.last }}
     {%- endfor -%}
     {%- if (col_err | length) > 0 -%}
       {{ exceptions.column_type_missing(column_names=col_err) }}
     {%- endif -%}
 {% endmacro %}
 
-{% macro get_column_schema_from_query(select_sql) -%}
+{% macro get_column_schema_from_query(select_sql, select_sql_header=none) -%}
     {% set columns = [] %}
     {# -- Using an 'empty subquery' here to get the same schema as the given select_sql statement, without necessitating a data scan.#}
-    {% set sql = get_empty_subquery_sql(select_sql) %}
+    {% set sql = get_empty_subquery_sql(select_sql, select_sql_header) %}
     {% set column_schema = adapter.get_column_schema_from_query(sql) %}
     {{ return(column_schema) }}
 {% endmacro %}
 
 -- here for back compat
 {% macro get_columns_in_query(select_sql) -%}
   {{ return(adapter.dispatch('get_columns_in_query', 'dbt')(select_sql)) }}
```

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/drop_relation.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/drop_relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/freshness.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/metadata.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/persist_docs.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/relation.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/schema.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/adapters/timestamps.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/adapters/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/etc/datetime.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/etc/datetime.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/etc/statement.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/configs.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/configs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/hooks.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 {#
   Compares the column schema provided by a model's sql file to the column schema provided by a model's schema file.
   If any differences in name, data_type or number of columns exist between the two schemas, raises a compiler error
 #}
 {% macro assert_columns_equivalent(sql) %}
   {#-- Obtain the column schema provided by sql file. #}
-  {%- set sql_file_provided_columns = get_column_schema_from_query(sql) -%}
+  {%- set sql_file_provided_columns = get_column_schema_from_query(sql, config.get('sql_header', none)) -%}
   {#--Obtain the column schema provided by the schema file by generating an 'empty schema' query from the model's columns. #}
   {%- set schema_file_provided_columns = get_column_schema_from_query(get_empty_schema_sql(model['columns'])) -%}
 
   {#-- create dictionaries with name and formatted data type and strings for exception #}
   {%- set sql_columns = format_columns(sql_file_provided_columns) -%}
   {%- set yaml_columns = format_columns(schema_file_provided_columns)  -%}
```

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/table/table.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/models/view/view.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/seeds/helpers.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/seeds/seed.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/seeds/seed.sql`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   {%- set old_relation = adapter.get_relation(database=database, schema=schema, identifier=identifier) -%}
 
   {%- set exists_as_table = (old_relation is not none and old_relation.is_table) -%}
   {%- set exists_as_view = (old_relation is not none and old_relation.is_view) -%}
 
   {%- set grant_config = config.get('grants') -%}
   {%- set agate_table = load_agate_table() -%}
-  -- grab current tables grants config for comparision later on
+  -- grab current tables grants config for comparison later on
 
   {%- do store_result('agate_table', response='OK', agate_table=agate_table) -%}
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
 
   -- `BEGIN` happens here:
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
```

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/tests/helpers.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/materializations/tests/test.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/python_model/python.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/data_types.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/listagg.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/macros/utils/split_part.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/global_project/tests/generic/builtin.sql` & `dbt-core-1.6.0b3/dbt/include/global_project/tests/generic/builtin.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/index.html` & `dbt-core-1.6.0b3/dbt/include/index.html`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/starter_project/README.md` & `dbt-core-1.6.0b3/dbt/include/starter_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/include/starter_project/dbt_project.yml` & `dbt-core-1.6.0b3/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/internal_deprecations.py` & `dbt-core-1.6.0b3/dbt/internal_deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/logger.py` & `dbt-core-1.6.0b3/dbt/logger.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/node_types.py` & `dbt-core-1.6.0b3/dbt/node_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     SqlOperation = "sql operation"
     Documentation = "doc"
     Source = "source"
     Macro = "macro"
     Exposure = "exposure"
     Metric = "metric"
     Group = "group"
+    SemanticModel = "semantic model"
 
     @classmethod
     def executable(cls) -> List["NodeType"]:
         return [
             cls.Model,
             cls.Test,
             cls.Snapshot,
```

### Comparing `dbt-core-1.6.0b2/dbt/parser/__init__.py` & `dbt-core-1.6.0b3/dbt/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/analysis.py` & `dbt-core-1.6.0b3/dbt/parser/analysis.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/base.py` & `dbt-core-1.6.0b3/dbt/parser/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,28 +67,52 @@
     ) -> None:
         super().__init__(project, manifest)
         self.root_project = root_project
 
 
 class RelationUpdate:
     def __init__(self, config: RuntimeConfig, manifest: Manifest, component: str) -> None:
-        macro = manifest.find_generate_macro_by_name(
+        default_macro = manifest.find_generate_macro_by_name(
             component=component,
             root_project_name=config.project_name,
         )
-        if macro is None:
+        if default_macro is None:
             raise DbtInternalError(f"No macro with name generate_{component}_name found")
 
-        root_context = generate_generate_name_macro_context(macro, config, manifest)
-        self.updater = MacroGenerator(macro, root_context)
+        default_macro_context = generate_generate_name_macro_context(
+            default_macro, config, manifest
+        )
+        self.default_updater = MacroGenerator(default_macro, default_macro_context)
+
+        package_names = config.dependencies.keys() if config.dependencies else {}
+        package_updaters = {}
+        for package_name in package_names:
+            package_macro = manifest.find_generate_macro_by_name(
+                component=component,
+                root_project_name=config.project_name,
+                imported_package=package_name,
+            )
+            if package_macro:
+                imported_macro_context = generate_generate_name_macro_context(
+                    package_macro, config, manifest
+                )
+                package_updaters[package_macro.package_name] = MacroGenerator(
+                    package_macro, imported_macro_context
+                )
+
+        self.package_updaters = package_updaters
         self.component = component
 
     def __call__(self, parsed_node: Any, config_dict: Dict[str, Any]) -> None:
         override = config_dict.get(self.component)
-        new_value = self.updater(override, parsed_node)
+        if parsed_node.package_name in self.package_updaters:
+            new_value = self.package_updaters[parsed_node.package_name](override, parsed_node)
+        else:
+            new_value = self.default_updater(override, parsed_node)
+
         if isinstance(new_value, str):
             new_value = new_value.strip()
         setattr(parsed_node, self.component, new_value)
 
 
 class ConfiguredParser(
     Parser[FinalNode],
```

### Comparing `dbt-core-1.6.0b2/dbt/parser/common.py` & `dbt-core-1.6.0b3/dbt/parser/common.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/docs.py` & `dbt-core-1.6.0b3/dbt/parser/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/generic_test.py` & `dbt-core-1.6.0b3/dbt/parser/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/generic_test_builders.py` & `dbt-core-1.6.0b3/dbt/parser/generic_test_builders.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/hooks.py` & `dbt-core-1.6.0b3/dbt/parser/hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/macros.py` & `dbt-core-1.6.0b3/dbt/parser/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/manifest.py` & `dbt-core-1.6.0b3/dbt/parser/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,20 @@
 from dbt.flags import get_flags
 
 from dbt.adapters.factory import (
     get_adapter,
     get_relation_class_by_name,
     get_adapter_package_names,
 )
-from dbt.constants import DEPENDENCIES_FILE_NAME, MANIFEST_FILE_NAME, PARTIAL_PARSE_FILE_NAME
+from dbt.constants import (
+    DEPENDENCIES_FILE_NAME,
+    MANIFEST_FILE_NAME,
+    PARTIAL_PARSE_FILE_NAME,
+    SEMANTIC_MANIFEST_FILE_NAME,
+)
 from dbt.helper_types import PathSet
 from dbt.clients.yaml_helper import load_yaml_text
 from dbt.events.functions import fire_event, get_invocation_id, warn_or_error
 from dbt.events.helpers import datetime_to_json_string
 from dbt.events.types import (
     PartialParsingErrorProcessingFile,
     PartialParsingError,
@@ -53,14 +58,15 @@
     Note,
     PublicationArtifactChanged,
     PublicationArtifactAvailable,
     DeprecatedModel,
     DeprecatedReference,
     UpcomingReferenceDeprecation,
 )
+from dbt_extractor import py_extract_from_source  # type: ignore
 from dbt.logger import DbtProcessState
 from dbt.node_types import NodeType, AccessType
 from dbt.clients.jinja import get_rendered, MacroStack
 from dbt.clients.jinja_static import statically_extract_macro_calls
 from dbt.clients.system import (
     make_directory,
     path_exists,
@@ -95,14 +101,15 @@
     Macro,
     Exposure,
     Metric,
     SeedNode,
     ManifestNode,
     ResultNode,
     ModelNode,
+    NodeRelation,
 )
 from dbt.contracts.graph.unparsed import NodeVersion
 from dbt.contracts.util import Writable
 from dbt.contracts.publication import (
     PublicationConfig,
     PublicationArtifact,
     PublicationMetadata,
@@ -110,14 +117,15 @@
     ProjectDependencies,
 )
 from dbt.exceptions import (
     TargetNotFoundError,
     AmbiguousAliasError,
     PublicationConfigNotFound,
     ProjectDependencyCycleError,
+    InvalidAccessTypeError,
 )
 from dbt.parser.base import Parser
 from dbt.parser.analysis import AnalysisParser
 from dbt.parser.generic_test import GenericTestParser
 from dbt.parser.singular_test import SingularTestParser
 from dbt.parser.docs import DocumentationParser
 from dbt.parser.hooks import HookParser
@@ -239,15 +247,19 @@
         macro_hook: Optional[Callable[[Manifest], Any]] = None,
         file_diff: Optional[FileDiff] = None,
         publications: Optional[List[PublicationArtifact]] = None,
     ) -> None:
         self.root_project: RuntimeConfig = root_project
         self.all_projects: Mapping[str, Project] = all_projects
         self.file_diff = file_diff
-        self.publications = publications
+        self.publications: Mapping[str, PublicationArtifact] = (
+            {publication.project_name: publication for publication in publications}
+            if publications
+            else {}
+        )
         self.manifest: Manifest = Manifest()
         self.new_manifest = self.manifest
         self.manifest.metadata = root_project.get_metadata()
         self.macro_resolver = None  # built after macros are loaded
         self.started_at = time.time()
         # This is a MacroQueryStringSetter callable, which is called
         # later after we set the MacroManifest in the adapter. It sets
@@ -322,15 +334,15 @@
             loader.save_macros_to_adapter(adapter)
 
             # Save performance info
             loader._perf_info.load_all_elapsed = time.perf_counter() - start_load_all
             loader.track_project_load()
 
             if write_perf_info:
-                loader.write_perf_info(config.target_path)
+                loader.write_perf_info(config.project_target_path)
 
         return manifest
 
     # This is where the main action happens
     def load(self):
         start_read_files = time.perf_counter()
 
@@ -520,15 +532,17 @@
             # These check the created_at time on the nodes to
             # determine whether they need processing.
             start_process = time.perf_counter()
             self.process_sources(self.root_project.project_name)
             self.process_refs(self.root_project.project_name)
             self.process_docs(self.root_project)
             self.process_metrics(self.root_project)
+            self.process_semantic_models()
             self.check_valid_group_config()
+            self.check_valid_access_property()
 
             # update tracking data
             self._perf_info.process_manifest_elapsed = time.perf_counter() - start_process
             self._perf_info.static_analysis_parsed_path_count = (
                 self.manifest._parsing_info.static_analysis_parsed_path_count
             )
             self._perf_info.static_analysis_path_count = (
@@ -545,17 +559,18 @@
             self.manifest.build_parent_and_child_maps()
             public_nodes_changed = self.build_public_nodes()
             if public_nodes_changed:
                 self.manifest.rebuild_ref_lookup()
                 self.process_refs(self.root_project.project_name)
                 # parent and child maps will be rebuilt by write_manifest
 
-        if not skip_parsing or public_nodes_changed:
-            # Write out the <project_name>_publication.json file for this project
-            log_publication_artifact(self.root_project, self.manifest)
+        # Log the publication artifact for this project
+        log_publication_artifact(self.root_project, self.manifest)
+
+        if not skip_parsing:
             # write out the fully parsed manifest
             self.write_manifest_for_partial_parse()
 
         self.check_for_model_deprecations()
 
         return self.manifest
 
@@ -725,17 +740,15 @@
                 if "." in macro_name:
                     package_name, macro_name = macro_name.split(".")
                 dep_macro_id = self.macro_resolver.get_macro_id(package_name, macro_name)
                 if dep_macro_id:
                     macro.depends_on.add_macro(dep_macro_id)  # will check for dupes
 
     def write_manifest_for_partial_parse(self):
-        path = os.path.join(
-            self.root_project.project_root, self.root_project.target_path, PARTIAL_PARSE_FILE_NAME
-        )
+        path = os.path.join(self.root_project.project_target_path, PARTIAL_PARSE_FILE_NAME)
         try:
             # This shouldn't be necessary, but we have gotten bug reports (#3757) of the
             # saved manifest not matching the code version.
             if self.manifest.metadata.dbt_version != __version__:
                 fire_event(
                     UnableToPartialParse(reason="saved manifest contained the wrong version")
                 )
@@ -778,33 +791,35 @@
 
         # collect the names of the projects for later use
         project_dependency_names = []
         if self.manifest.project_dependencies:
             for project in self.manifest.project_dependencies.projects:
                 project_dependency_names.append(project.name)
 
-        # clean up previous publications that are no longer specified
-        # and save previous publications, for later removal of references
-        saved_manifest_publications: MutableMapping[str, PublicationConfig] = {}
+        # Save previous publications, for later removal of references
+        saved_manifest_publications: MutableMapping[str, PublicationConfig] = deepcopy(
+            self.manifest.publications
+        )
         if self.manifest.publications:
             for project_name, publication in self.manifest.publications.items():
                 if project_name not in project_dependency_names:
                     remove_dependent_project_references(self.manifest, publication)
-                    self.manifest.publications.pop(project_name)
+                    saved_manifest_publications.pop(project_name)
                     fire_event(
                         PublicationArtifactChanged(
                             action="removed",
                             project_name=project_name,
                             generated_at=datetime_to_json_string(
                                 publication.metadata.generated_at
                             ),
                         )
                     )
                     public_nodes_changed = True
-            saved_manifest_publications = self.manifest.publications
+
+            # clean up previous publications that are no longer specified
             self.manifest.publications = {}
             # Empty public_nodes since we're re-generating them all
             self.manifest.public_nodes = {}
 
         if self.manifest.project_dependencies:
             self.load_new_public_nodes()
 
@@ -837,28 +852,26 @@
                 )
                 public_nodes_changed = True
 
         return public_nodes_changed
 
     def load_new_public_nodes(self):
         for project in self.manifest.project_dependencies.projects:
-            publication = (
-                next(p for p in self.publications if p.project_name == project.name)
-                if self.publications
-                else None
-            )
-            if publication:
-                publication_config = PublicationConfig.from_publication(publication)
-                self.manifest.publications[project.name] = publication_config
-                # Add to dictionary of public_nodes and save id in PublicationConfig
-                for public_node in publication.public_models.values():
-                    self.manifest.public_nodes[public_node.unique_id] = public_node
-            else:
+            try:
+                publication = self.publications[project.name]
+            except KeyError:
                 raise PublicationConfigNotFound(project=project.name)
 
+            publication_config = PublicationConfig.from_publication(publication)
+            self.manifest.publications[project.name] = publication_config
+
+            # Add to dictionary of public_nodes and save id in PublicationConfig
+            for public_node in publication.public_models.values():
+                self.manifest.public_nodes[public_node.unique_id] = public_node
+
     def is_partial_parsable(self, manifest: Manifest) -> Tuple[bool, Optional[str]]:
         """Compare the global hashes of the read-in parse results' values to
         the known ones, and return if it is ok to re-use the results.
         """
         valid = True
         reparse_reason = None
 
@@ -940,17 +953,15 @@
                     return True
         return False
 
     def read_manifest_for_partial_parse(self) -> Optional[Manifest]:
         if not get_flags().PARTIAL_PARSE:
             fire_event(PartialParsingNotEnabled())
             return None
-        path = os.path.join(
-            self.root_project.project_root, self.root_project.target_path, PARTIAL_PARSE_FILE_NAME
-        )
+        path = os.path.join(self.root_project.project_target_path, PARTIAL_PARSE_FILE_NAME)
 
         reparse_reason = None
 
         if os.path.exists(path):
             try:
                 with open(path, "rb") as fp:
                     manifest_mp = fp.read()
@@ -1173,14 +1184,36 @@
                 continue
             _process_metrics_for_node(self.manifest, current_project, metric)
         for exposure in self.manifest.exposures.values():
             if exposure.created_at < self.started_at:
                 continue
             _process_metrics_for_node(self.manifest, current_project, exposure)
 
+    def process_semantic_models(self) -> None:
+        for semantic_model in self.manifest.semantic_nodes.values():
+            if semantic_model.model:
+                statically_parsed = py_extract_from_source(f"{{{{ {semantic_model.model} }}}}")
+                if statically_parsed["refs"]:
+
+                    ref = statically_parsed["refs"][0]
+                    if len(ref) == 2:
+                        input_package_name, input_model_name = ref
+                    else:
+                        input_package_name, input_model_name = None, ref[0]
+
+                    refd_node = self.manifest.ref_lookup.find(
+                        input_model_name, input_package_name, None, self.manifest
+                    )
+                    if isinstance(refd_node, ModelNode):
+                        semantic_model.node_relation = NodeRelation(
+                            alias=refd_node.alias,
+                            schema_name=refd_node.schema,
+                            database=refd_node.database,
+                        )
+
     # nodes: node and column descriptions
     # sources: source and table descriptions, column descriptions
     # macros: macro argument descriptions
     # exposures: exposure descriptions
     def process_docs(self, config: RuntimeConfig):
         for node in self.manifest.nodes.values():
             if node.created_at < self.started_at:
@@ -1290,14 +1323,27 @@
         groupable_node_group = groupable_node.group
         if groupable_node_group and groupable_node_group not in valid_group_names:
             raise dbt.exceptions.ParsingError(
                 f"Invalid group '{groupable_node_group}', expected one of {sorted(list(valid_group_names))}",
                 node=groupable_node,
             )
 
+    def check_valid_access_property(self):
+        for node in self.manifest.nodes.values():
+            if (
+                isinstance(node, ModelNode)
+                and node.access == AccessType.Public
+                and node.get_materialization() == "ephemeral"
+            ):
+                raise InvalidAccessTypeError(
+                    unique_id=node.unique_id,
+                    field_value=node.access,
+                    materialization=node.get_materialization(),
+                )
+
     def write_perf_info(self, target_path: str):
         path = os.path.join(target_path, PERF_INFO_FILE_NAME)
         write_file(path, json.dumps(self._perf_info, cls=dbt.utils.JSONEncoder, indent=4))
         fire_event(ParsePerfInfoPath(path=path))
 
 
 def invalid_target_fail_unless_test(
@@ -1825,10 +1871,17 @@
         public_models=public_models,
         dependencies=dependencies,
     )
 
     fire_event(PublicationArtifactAvailable(pub_artifact=publication.to_dict()))
 
 
+def write_semantic_manifest(manifest: Manifest, target_path: str) -> None:
+    path = os.path.join(target_path, SEMANTIC_MANIFEST_FILE_NAME)
+    write_file(path, manifest.pydantic_semantic_manifest.json())
+
+
 def write_manifest(manifest: Manifest, target_path: str):
     path = os.path.join(target_path, MANIFEST_FILE_NAME)
     manifest.write(path)
+
+    write_semantic_manifest(manifest=manifest, target_path=target_path)
```

### Comparing `dbt-core-1.6.0b2/dbt/parser/models.py` & `dbt-core-1.6.0b3/dbt/parser/models.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/partial.py` & `dbt-core-1.6.0b3/dbt/parser/partial.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/read_files.py` & `dbt-core-1.6.0b3/dbt/parser/read_files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/schema_generic_tests.py` & `dbt-core-1.6.0b3/dbt/parser/schema_generic_tests.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/schema_renderer.py` & `dbt-core-1.6.0b3/dbt/parser/schema_renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/schemas.py` & `dbt-core-1.6.0b3/dbt/parser/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,18 +42,19 @@
     YamlLoadError,
     YamlParseDictError,
     YamlParseListError,
     InvalidAccessTypeError,
 )
 from dbt.events.functions import warn_or_error
 from dbt.events.types import (
-    WrongResourceSchemaFile,
-    NoNodeForYamlKey,
     MacroNotFoundForPatch,
+    NoNodeForYamlKey,
     ValidationWarning,
+    UnsupportedConstraintMaterialization,
+    WrongResourceSchemaFile,
 )
 from dbt.node_types import NodeType, AccessType
 from dbt.parser.base import SimpleParser
 from dbt.parser.search import FileBlock
 from dbt.parser.common import (
     YamlBlock,
     TargetBlock,
@@ -70,14 +71,15 @@
     "seeds",
     "snapshots",
     "sources",
     "macros",
     "analyses",
     "exposures",
     "metrics",
+    "semantic_models",
 )
 
 
 # ===============================================================================
 #  Schema Parser classes
 #
 # The SchemaParser is a subclass of the SimpleParser from base.py, as is
@@ -213,14 +215,20 @@
             # GroupParser.parse()
             if "groups" in dct:
                 from dbt.parser.schema_yaml_readers import GroupParser
 
                 group_parser = GroupParser(self, yaml_block)
                 group_parser.parse()
 
+            if "semantic_models" in dct:
+                from dbt.parser.schema_yaml_readers import SemanticModelParser
+
+                semantic_model_parser = SemanticModelParser(self, yaml_block)
+                semantic_model_parser.parse()
+
 
 Parsed = TypeVar("Parsed", UnpatchedSourceDefinition, ParsedNodePatch, ParsedMacroPatch)
 NodeTarget = TypeVar("NodeTarget", UnparsedNodeUpdate, UnparsedAnalysisUpdate, UnparsedModelUpdate)
 NonSourceTarget = TypeVar(
     "NonSourceTarget",
     UnparsedNodeUpdate,
     UnparsedAnalysisUpdate,
@@ -813,31 +821,44 @@
                     f"Invalid constraint type on model {node.name}: "
                     f"Type must be one of {[ct.value for ct in ConstraintType]}"
                 )
 
             node.constraints = [ModelLevelConstraint.from_dict(c) for c in constraints]
 
     def _validate_constraint_prerequisites(self, model_node: ModelNode):
+
+        column_warn_unsupported = [
+            constraint.warn_unsupported
+            for column in model_node.columns.values()
+            for constraint in column.constraints
+        ]
+        model_warn_unsupported = [
+            constraint.warn_unsupported for constraint in model_node.constraints
+        ]
+        warn_unsupported = column_warn_unsupported + model_warn_unsupported
+
+        # if any constraint has `warn_unsupported` as True then send the warning
+        if any(warn_unsupported) and not model_node.materialization_enforces_constraints:
+            warn_or_error(
+                UnsupportedConstraintMaterialization(materialized=model_node.config.materialized),
+                node=model_node,
+            )
+
         errors = []
         if not model_node.columns:
             errors.append(
                 "Constraints must be defined in a `yml` schema configuration file like `schema.yml`."
             )
 
-        if model_node.config.materialized not in ["table", "view", "incremental"]:
-            errors.append(
-                f"Only table, view, and incremental materializations are supported for constraints, but found '{model_node.config.materialized}'"
-            )
-
         if str(model_node.language) != "sql":
             errors.append(f"Language Error: Expected 'sql' but found '{model_node.language}'")
 
         if errors:
             raise ParsingError(
-                f"Constraint validation failed for: ({model_node.original_file_path})\n"
+                f"Contract enforcement failed for: ({model_node.original_file_path})\n"
                 + "\n".join(errors)
             )
 
 
 class AnalysisPatchParser(NodePatchParser[UnparsedAnalysisUpdate]):
     def get_block(self, node: UnparsedAnalysisUpdate) -> TargetBlock:
         return TargetBlock.from_yaml_block(self.yaml, node)
```

### Comparing `dbt-core-1.6.0b2/dbt/parser/search.py` & `dbt-core-1.6.0b3/dbt/parser/search.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/seeds.py` & `dbt-core-1.6.0b3/dbt/parser/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/singular_test.py` & `dbt-core-1.6.0b3/dbt/parser/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/snapshots.py` & `dbt-core-1.6.0b3/dbt/parser/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/sources.py` & `dbt-core-1.6.0b3/dbt/parser/sources.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/parser/sql.py` & `dbt-core-1.6.0b3/dbt/parser/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/semver.py` & `dbt-core-1.6.0b3/dbt/semver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/task/base.py` & `dbt-core-1.6.0b3/dbt/task/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/task/build.py` & `dbt-core-1.6.0b3/dbt/task/build.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/task/clean.py` & `dbt-core-1.6.0b3/dbt/task/clean.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/task/compile.py` & `dbt-core-1.6.0b3/dbt/task/compile.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,22 +96,22 @@
                 )
             )
 
     def _get_deferred_manifest(self) -> Optional[WritableManifest]:
         if not self.args.defer:
             return None
 
-        state = self.previous_state
-        if state is None:
+        state = self.previous_defer_state or self.previous_state
+        if not state:
             raise DbtRuntimeError(
                 "Received a --defer argument, but no value was provided to --state"
             )
 
-        if state.manifest is None:
-            raise DbtRuntimeError(f'Could not find manifest in --state path: "{self.args.state}"')
+        if not state.manifest:
+            raise DbtRuntimeError(f'Could not find manifest in --state path: "{state}"')
         return state.manifest
 
     def defer_to_manifest(self, adapter, selected_uids: AbstractSet[str]):
         deferred_manifest = self._get_deferred_manifest()
         if deferred_manifest is None:
             return
         if self.manifest is None:
@@ -121,15 +121,15 @@
         self.manifest.merge_from_artifact(
             adapter=adapter,
             other=deferred_manifest,
             selected=selected_uids,
             favor_state=bool(self.args.favor_state),
         )
         # TODO: is it wrong to write the manifest here? I think it's right...
-        write_manifest(self.manifest, self.config.target_path)
+        write_manifest(self.manifest, self.config.project_target_path)
 
     def _runtime_initialize(self):
         if getattr(self.args, "inline", None):
             block_parser = SqlBlockParser(
                 project=self.config, manifest=self.manifest, root_project=self.config
             )
             sql_node = block_parser.parse_remote(self.args.inline, "inline_query")
```

### Comparing `dbt-core-1.6.0b2/dbt/task/debug.py` & `dbt-core-1.6.0b3/dbt/task/debug.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # coding=utf-8
+import importlib
 import os
 import platform
 import sys
-from typing import Optional, Dict, Any, List
+
+from collections import namedtuple
+from enum import Flag
+from typing import Optional, Dict, Any, List, Tuple
 
 from dbt.events.functions import fire_event
 from dbt.events.types import (
     OpenCommand,
     DebugCmdOut,
     DebugCmdResult,
 )
 import dbt.clients.system
 import dbt.exceptions
 from dbt.adapters.factory import get_adapter, register_adapter
 from dbt.config import PartialProject, Project, Profile
 from dbt.config.renderer import DbtProjectYamlRenderer, ProfileRenderer
+from dbt.contracts.results import RunStatus
 from dbt.clients.yaml_helper import load_yaml_text
 from dbt.links import ProfileConfigDocs
 from dbt.ui import green, red
 from dbt.events.format import pluralize
 from dbt.version import get_installed_version
 
 from dbt.task.base import BaseTask, get_nearest_project_dir
@@ -54,14 +59,24 @@
 
 {url}
 """.lstrip()
 
 FILE_NOT_FOUND = "file not found"
 
 
+SubtaskStatus = namedtuple(
+    "SubtaskStatus", ["log_msg", "run_status", "details", "summary_message"]
+)
+
+
+class DebugRunStatus(Flag):
+    SUCCESS = True
+    FAIL = False
+
+
 class DebugTask(BaseTask):
     def __init__(self, args, config):
         super().__init__(args, config)
         self.profiles_dir = args.PROFILES_DIR
         self.profile_path = os.path.join(self.profiles_dir, "profiles.yml")
         try:
             self.project_dir = get_nearest_project_dir(self.args.project_dir)
@@ -73,107 +88,166 @@
             else:
                 self.project_dir = os.getcwd()
         self.project_path = os.path.join(self.project_dir, "dbt_project.yml")
         self.cli_vars: Dict[str, Any] = args.vars
 
         # set by _load_*
         self.profile: Optional[Profile] = None
-        self.profile_fail_details = ""
         self.raw_profile_data: Optional[Dict[str, Any]] = None
         self.profile_name: Optional[str] = None
         self.project: Optional[Project] = None
-        self.project_fail_details = ""
-        self.any_failure = False
-        self.messages: List[str] = []
 
     @property
     def project_profile(self):
         if self.project is None:
             return None
         return self.project.profile_name
 
     def path_info(self):
         open_cmd = dbt.clients.system.open_dir_cmd()
         fire_event(OpenCommand(open_cmd=open_cmd, profiles_dir=self.profiles_dir))
 
-    def run(self):
+    def run(self) -> bool:
         if self.args.config_dir:
             self.path_info()
-            return not self.any_failure
+            return DebugRunStatus.SUCCESS.value
 
-        version = get_installed_version().to_version_string(skip_matcher=True)
+        version: str = get_installed_version().to_version_string(skip_matcher=True)
         fire_event(DebugCmdOut(msg="dbt version: {}".format(version)))
         fire_event(DebugCmdOut(msg="python version: {}".format(sys.version.split()[0])))
         fire_event(DebugCmdOut(msg="python path: {}".format(sys.executable)))
         fire_event(DebugCmdOut(msg="os info: {}".format(platform.platform())))
+
+        # Load profile if possible, then load adapter info (which requires the profile)
+        load_profile_status: SubtaskStatus = self._load_profile()
+        fire_event(DebugCmdOut(msg="Using profiles dir at {}".format(self.profiles_dir)))
         fire_event(DebugCmdOut(msg="Using profiles.yml file at {}".format(self.profile_path)))
         fire_event(DebugCmdOut(msg="Using dbt_project.yml file at {}".format(self.project_path)))
-        self.test_configuration()
-        self.test_dependencies()
-        self.test_connection()
+        if load_profile_status.run_status == RunStatus.Success:
+            if self.profile is None:
+                raise dbt.exceptions.DbtInternalError(
+                    "Profile should not be None if loading profile completed"
+                )
+            else:
+                adapter_type: str = self.profile.credentials.type
 
-        if self.any_failure:
-            fire_event(
-                DebugCmdResult(msg=red(f"{(pluralize(len(self.messages), 'check'))} failed:"))
+            adapter_version: str = self._read_adapter_version(
+                f"dbt.adapters.{adapter_type}.__version__"
             )
+            fire_event(DebugCmdOut(msg="adapter type: {}".format(adapter_type)))
+            fire_event(DebugCmdOut(msg="adapter version: {}".format(adapter_version)))
+
+        # Get project loaded to do additional checks
+        load_project_status: SubtaskStatus = self._load_project()
+
+        dependencies_statuses: List[SubtaskStatus] = []
+        if self.args.connection:
+            fire_event(DebugCmdOut(msg="Skipping steps before connection verification"))
         else:
-            fire_event(DebugCmdResult(msg=green("All checks passed!")))
+            # this job's status not logged since already accounted for in _load_* commands
+            self.test_configuration(load_profile_status.log_msg, load_project_status.log_msg)
+            dependencies_statuses = self.test_dependencies()
+
+        # Test connection
+        self.test_connection()
+
+        # Log messages from any fails
+        all_statuses: List[SubtaskStatus] = [
+            load_profile_status,
+            load_project_status,
+            *dependencies_statuses,
+        ]
+        all_failing_statuses: List[SubtaskStatus] = list(
+            filter(lambda status: status.run_status == RunStatus.Error, all_statuses)
+        )
 
-        for message in self.messages:
-            fire_event(DebugCmdResult(msg=f"{message}\n"))
+        failure_count: int = len(all_failing_statuses)
+        if failure_count > 0:
+            fire_event(DebugCmdResult(msg=red(f"{(pluralize(failure_count, 'check'))} failed:")))
+            for status in all_failing_statuses:
+                fire_event(DebugCmdResult(msg=f"{status.summary_message}\n"))
+            return DebugRunStatus.FAIL.value
+        else:
+            fire_event(DebugCmdResult(msg=green("All checks passed!")))
+            return DebugRunStatus.SUCCESS.value
 
-        return not self.any_failure
+    # ==============================
+    # Override for elsewhere in core
+    # ==============================
 
     def interpret_results(self, results):
         return results
 
-    def _load_project(self):
-        if not os.path.exists(self.project_path):
-            self.project_fail_details = FILE_NOT_FOUND
-            return red("ERROR not found")
+    # ===============
+    # Loading profile
+    # ===============
 
-        renderer = DbtProjectYamlRenderer(self.profile, self.cli_vars)
-
-        try:
-            self.project = Project.from_project_root(
-                self.project_dir,
-                renderer,
-                verify_version=self.args.VERSION_CHECK,
+    def _load_profile(self) -> SubtaskStatus:
+        """
+        Side effects: load self.profile
+                      load self.target_name
+                      load self.raw_profile_data
+        """
+        if not os.path.exists(self.profile_path):
+            return SubtaskStatus(
+                log_msg=red("ERROR not found"),
+                run_status=RunStatus.Error,
+                details=FILE_NOT_FOUND,
+                summary_message=MISSING_PROFILE_MESSAGE.format(
+                    path=self.profile_path, url=ProfileConfigDocs
+                ),
             )
-        except dbt.exceptions.DbtConfigError as exc:
-            self.project_fail_details = str(exc)
-            return red("ERROR invalid")
 
-        return green("OK found and valid")
+        raw_profile_data = load_yaml_text(dbt.clients.system.load_file_contents(self.profile_path))
+        if isinstance(raw_profile_data, dict):
+            self.raw_profile_data = raw_profile_data
 
-    def _profile_found(self):
-        if not self.raw_profile_data:
-            return red("ERROR not found")
-        assert self.raw_profile_data is not None
-        if self.profile_name in self.raw_profile_data:
-            return green("OK found")
-        else:
-            return red("ERROR not found")
+        profile_errors = []
+        profile_names, summary_message = self._choose_profile_names()
+        renderer = ProfileRenderer(self.cli_vars)
+        for profile_name in profile_names:
+            try:
+                profile: Profile = Profile.render(
+                    renderer,
+                    profile_name,
+                    self.args.profile,
+                    self.args.target,
+                    # TODO: Generalize safe access to flags.THREADS:
+                    # https://github.com/dbt-labs/dbt-core/issues/6259
+                    getattr(self.args, "threads", None),
+                )
+            except dbt.exceptions.DbtConfigError as exc:
+                profile_errors.append(str(exc))
+            else:
+                if len(profile_names) == 1:
+                    # if a profile was specified, set it on the task
+                    self.target_name = self._choose_target_name(profile_name)
+                    self.profile = profile
 
-    def _target_found(self):
-        requirements = self.raw_profile_data and self.profile_name and self.target_name
-        if not requirements:
-            return red("ERROR not found")
-        # mypy appeasement, we checked just above
-        assert self.raw_profile_data is not None
-        assert self.profile_name is not None
-        assert self.target_name is not None
-        if self.profile_name not in self.raw_profile_data:
-            return red("ERROR not found")
-        profiles = self.raw_profile_data[self.profile_name]["outputs"]
-        if self.target_name not in profiles:
-            return red("ERROR not found")
-        return green("OK found")
+        if profile_errors:
+            details = "\n\n".join(profile_errors)
+            return SubtaskStatus(
+                log_msg=red("ERROR invalid"),
+                run_status=RunStatus.Error,
+                details=details,
+                summary_message=(
+                    summary_message + f"Profile loading failed for the following reason:"
+                    f"\n{details}"
+                    f"\n"
+                ),
+            )
+        else:
+            return SubtaskStatus(
+                log_msg=green("OK found and valid"),
+                run_status=RunStatus.Success,
+                details="",
+                summary_message="Profile is valid",
+            )
 
-    def _choose_profile_names(self) -> Optional[List[str]]:
+    def _choose_profile_names(self) -> Tuple[List[str], str]:
         project_profile: Optional[str] = None
         if os.path.exists(self.project_path):
             try:
                 partial = PartialProject.from_project_root(
                     os.path.dirname(self.project_path),
                     verify_version=bool(self.args.VERSION_CHECK),
                 )
@@ -181,33 +255,47 @@
                 project_profile = partial.render_profile_name(renderer)
             except dbt.exceptions.DbtProjectError:
                 pass
 
         args_profile: Optional[str] = getattr(self.args, "profile", None)
 
         try:
-            return [Profile.pick_profile_name(args_profile, project_profile)]
+            return [Profile.pick_profile_name(args_profile, project_profile)], ""
         except dbt.exceptions.DbtConfigError:
             pass
         # try to guess
 
         profiles = []
         if self.raw_profile_data:
             profiles = [k for k in self.raw_profile_data if k != "config"]
             if project_profile is None:
-                self.messages.append("Could not load dbt_project.yml")
+                summary_message = "Could not load dbt_project.yml\n"
             elif len(profiles) == 0:
-                self.messages.append("The profiles.yml has no profiles")
+                summary_message = "The profiles.yml has no profiles\n"
             elif len(profiles) == 1:
-                self.messages.append(ONLY_PROFILE_MESSAGE.format(profiles[0]))
+                summary_message = ONLY_PROFILE_MESSAGE.format(profiles[0])
             else:
-                self.messages.append(
-                    MULTIPLE_PROFILE_MESSAGE.format("\n".join(" - {}".format(o) for o in profiles))
+                summary_message = MULTIPLE_PROFILE_MESSAGE.format(
+                    "\n".join(" - {}".format(o) for o in profiles)
                 )
-        return profiles
+        return profiles, summary_message
+
+    def _read_adapter_version(self, module) -> str:
+        """read the version out of a standard adapter file"""
+        try:
+            version = importlib.import_module(module).version
+        except ModuleNotFoundError:
+            version = red("ERROR not found")
+        except Exception as exc:
+            version = red("ERROR {}".format(exc))
+            raise dbt.exceptions.DbtInternalError(
+                f"Error when reading adapter version from {module}: {exc}"
+            )
+
+        return version
 
     def _choose_target_name(self, profile_name: str):
         has_raw_profile = (
             self.raw_profile_data is not None and profile_name in self.raw_profile_data
         )
 
         if not has_raw_profile:
@@ -223,163 +311,182 @@
             raw_profile=raw_profile,
             profile_name=profile_name,
             target_override=getattr(self.args, "target", None),
             renderer=renderer,
         )
         return target_name
 
-    def _load_profile(self):
-        if not os.path.exists(self.profile_path):
-            self.profile_fail_details = FILE_NOT_FOUND
-            self.messages.append(
-                MISSING_PROFILE_MESSAGE.format(path=self.profile_path, url=ProfileConfigDocs)
+    # ===============
+    # Loading project
+    # ===============
+
+    def _load_project(self) -> SubtaskStatus:
+        """
+        Side effect: load self.project
+        """
+        if not os.path.exists(self.project_path):
+            return SubtaskStatus(
+                log_msg=red("ERROR not found"),
+                run_status=RunStatus.Error,
+                details=FILE_NOT_FOUND,
+                summary_message=(
+                    f"Project loading failed for the following reason:"
+                    f"\n project path <{self.project_path}> not found"
+                ),
             )
-            self.any_failure = True
-            return red("ERROR not found")
+
+        renderer = DbtProjectYamlRenderer(self.profile, self.cli_vars)
 
         try:
-            raw_profile_data = load_yaml_text(
-                dbt.clients.system.load_file_contents(self.profile_path)
+            self.project = Project.from_project_root(
+                self.project_dir,
+                renderer,
+                verify_version=self.args.VERSION_CHECK,
+            )
+        except dbt.exceptions.DbtConfigError as exc:
+            return SubtaskStatus(
+                log_msg=red("ERROR invalid"),
+                run_status=RunStatus.Error,
+                details=str(exc),
+                summary_message=(
+                    f"Project loading failed for the following reason:" f"\n{str(exc)}" f"\n"
+                ),
             )
-        except Exception:
-            pass  # we'll report this when we try to load the profile for real
         else:
-            if isinstance(raw_profile_data, dict):
-                self.raw_profile_data = raw_profile_data
+            return SubtaskStatus(
+                log_msg=green("OK found and valid"),
+                run_status=RunStatus.Success,
+                details="",
+                summary_message="Project is valid",
+            )
 
-        profile_errors = []
-        profile_names = self._choose_profile_names()
-        renderer = ProfileRenderer(self.cli_vars)
-        for profile_name in profile_names:
-            try:
-                profile: Profile = Profile.render(
-                    renderer,
-                    profile_name,
-                    self.args.profile,
-                    self.args.target,
-                    # TODO: Generalize safe access to flags.THREADS:
-                    # https://github.com/dbt-labs/dbt-core/issues/6259
-                    getattr(self.args, "threads", None),
-                )
-            except dbt.exceptions.DbtConfigError as exc:
-                profile_errors.append(str(exc))
-            else:
-                if len(profile_names) == 1:
-                    # if a profile was specified, set it on the task
-                    self.target_name = self._choose_target_name(profile_name)
-                    self.profile = profile
+    def _profile_found(self) -> str:
+        if not self.raw_profile_data:
+            return red("ERROR not found")
+        assert self.raw_profile_data is not None
+        if self.profile_name in self.raw_profile_data:
+            return green("OK found")
+        else:
+            return red("ERROR not found")
 
-        if profile_errors:
-            self.profile_fail_details = "\n\n".join(profile_errors)
-            return red("ERROR invalid")
-        return green("OK found and valid")
+    def _target_found(self) -> str:
+        requirements = self.raw_profile_data and self.profile_name and self.target_name
+        if not requirements:
+            return red("ERROR not found")
+        # mypy appeasement, we checked just above
+        assert self.raw_profile_data is not None
+        assert self.profile_name is not None
+        assert self.target_name is not None
+        if self.profile_name not in self.raw_profile_data:
+            return red("ERROR not found")
+        profiles = self.raw_profile_data[self.profile_name]["outputs"]
+        if self.target_name not in profiles:
+            return red("ERROR not found")
+        else:
+            return green("OK found")
+
+    # ============
+    # Config tests
+    # ============
 
-    def test_git(self):
+    def test_git(self) -> SubtaskStatus:
         try:
             dbt.clients.system.run_cmd(os.getcwd(), ["git", "--help"])
         except dbt.exceptions.ExecutableError as exc:
-            self.messages.append("Error from git --help: {!s}".format(exc))
-            self.any_failure = True
-            return red("ERROR")
-        return green("OK found")
+            return SubtaskStatus(
+                log_msg=red("ERROR"),
+                run_status=RunStatus.Error,
+                details="git error",
+                summary_message="Error from git --help: {!s}".format(exc),
+            )
+        else:
+            return SubtaskStatus(
+                log_msg=green("OK found"),
+                run_status=RunStatus.Success,
+                details="",
+                summary_message="git is installed and on the path",
+            )
 
-    def test_dependencies(self):
+    def test_dependencies(self) -> List[SubtaskStatus]:
         fire_event(DebugCmdOut(msg="Required dependencies:"))
 
-        logline_msg = self.test_git()
-        fire_event(DebugCmdResult(msg=f" - git [{logline_msg}]\n"))
+        git_test_status = self.test_git()
+        fire_event(DebugCmdResult(msg=f" - git [{git_test_status.log_msg}]\n"))
 
-    def test_configuration(self):
-        fire_event(DebugCmdOut(msg="Configuration:"))
-
-        profile_status = self._load_profile()
-        fire_event(DebugCmdOut(msg=f"  profiles.yml file [{profile_status}]"))
+        return [git_test_status]
 
-        project_status = self._load_project()
-        fire_event(DebugCmdOut(msg=f"  dbt_project.yml file [{project_status}]"))
+    def test_configuration(self, profile_status_msg, project_status_msg):
+        fire_event(DebugCmdOut(msg="Configuration:"))
+        fire_event(DebugCmdOut(msg=f"  profiles.yml file [{profile_status_msg}]"))
+        fire_event(DebugCmdOut(msg=f"  dbt_project.yml file [{project_status_msg}]"))
 
         # skip profile stuff if we can't find a profile name
         if self.profile_name is not None:
             fire_event(
                 DebugCmdOut(
                     msg="  profile: {} [{}]\n".format(self.profile_name, self._profile_found())
                 )
             )
             fire_event(
                 DebugCmdOut(
                     msg="  target: {} [{}]\n".format(self.target_name, self._target_found())
                 )
             )
 
-        self._log_project_fail()
-        self._log_profile_fail()
-
-    def _log_project_fail(self):
-        if not self.project_fail_details:
-            return
-
-        self.any_failure = True
-        if self.project_fail_details == FILE_NOT_FOUND:
-            return
-        msg = (
-            f"Project loading failed for the following reason:"
-            f"\n{self.project_fail_details}"
-            f"\n"
-        )
-        self.messages.append(msg)
-
-    def _log_profile_fail(self):
-        if not self.profile_fail_details:
-            return
-
-        self.any_failure = True
-        if self.profile_fail_details == FILE_NOT_FOUND:
-            return
-        msg = (
-            f"Profile loading failed for the following reason:"
-            f"\n{self.profile_fail_details}"
-            f"\n"
-        )
-        self.messages.append(msg)
+    # ===============
+    # Connection test
+    # ===============
 
     @staticmethod
-    def attempt_connection(profile):
-        """Return a string containing the error message, or None if there was
-        no error.
-        """
+    def attempt_connection(profile) -> Optional[str]:
+        """Return a string containing the error message, or None if there was no error."""
         register_adapter(profile)
         adapter = get_adapter(profile)
         try:
             with adapter.connection_named("debug"):
+                # is defined in adapter class
                 adapter.debug_query()
         except Exception as exc:
             return COULD_NOT_CONNECT_MESSAGE.format(
                 err=str(exc),
                 url=ProfileConfigDocs,
             )
-
         return None
 
-    def _connection_result(self):
-        result = self.attempt_connection(self.profile)
-        if result is not None:
-            self.messages.append(result)
-            self.any_failure = True
-            return red("ERROR")
-        return green("OK connection ok")
-
-    def test_connection(self):
-        if not self.profile:
-            return
+    def test_connection(self) -> SubtaskStatus:
+        if self.profile is None:
+            fire_event(DebugCmdOut(msg="Connection test skipped since no profile was found"))
+            return SubtaskStatus(
+                log_msg=red("SKIPPED"),
+                run_status=RunStatus.Skipped,
+                details="No profile found",
+                summary_message="Connection test skipped since no profile was found",
+            )
+
         fire_event(DebugCmdOut(msg="Connection:"))
         for k, v in self.profile.credentials.connection_info():
             fire_event(DebugCmdOut(msg=f"  {k}: {v}"))
 
-        res = self._connection_result()
-        fire_event(DebugCmdOut(msg=f"  Connection test: [{res}]\n"))
+        connection_result = self.attempt_connection(self.profile)
+        if connection_result is None:
+            status = SubtaskStatus(
+                log_msg=green("OK connection ok"),
+                run_status=RunStatus.Success,
+                details="",
+                summary_message="Connection test passed",
+            )
+        else:
+            status = SubtaskStatus(
+                log_msg=red("ERROR"),
+                run_status=RunStatus.Error,
+                details="Failure in connecting to db",
+                summary_message=connection_result,
+            )
+        fire_event(DebugCmdOut(msg=f"  Connection test: [{status.log_msg}]\n"))
+        return status
 
     @classmethod
     def validate_connection(cls, target_dict):
         """Validate a connection dictionary. On error, raises a DbtConfigError."""
         target_name = "test"
         # make a fake profile that we can parse
         profile_data = {
```

### Comparing `dbt-core-1.6.0b2/dbt/task/deps.py` & `dbt-core-1.6.0b3/dbt/task/deps.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/task/freshness.py` & `dbt-core-1.6.0b3/dbt/task/freshness.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         # freshness don't defer
         return
 
     def result_path(self):
         if self.args.output:
             return os.path.realpath(self.args.output)
         else:
-            return os.path.join(self.config.target_path, RESULT_FILE_NAME)
+            return os.path.join(self.config.project_target_path, RESULT_FILE_NAME)
 
     def raise_on_first_error(self):
         return False
 
     def get_node_selector(self):
         if self.manifest is None or self.graph is None:
             raise DbtInternalError("manifest and graph must be set to get perform node selection")
```

### Comparing `dbt-core-1.6.0b2/dbt/task/generate.py` & `dbt-core-1.6.0b3/dbt/task/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,18 +210,20 @@
                     nodes={},
                     sources={},
                     generated_at=datetime.utcnow(),
                     errors=None,
                     compile_results=compile_results,
                 )
 
-        shutil.copyfile(DOCS_INDEX_FILE_PATH, os.path.join(self.config.target_path, "index.html"))
+        shutil.copyfile(
+            DOCS_INDEX_FILE_PATH, os.path.join(self.config.project_target_path, "index.html")
+        )
 
         for asset_path in self.config.asset_paths:
-            to_asset_path = os.path.join(self.config.target_path, asset_path)
+            to_asset_path = os.path.join(self.config.project_target_path, asset_path)
 
             if os.path.exists(to_asset_path):
                 shutil.rmtree(to_asset_path)
 
             if os.path.exists(asset_path):
                 shutil.copytree(asset_path, to_asset_path)
 
@@ -253,18 +255,18 @@
             nodes=nodes,
             sources=sources,
             generated_at=datetime.utcnow(),
             compile_results=compile_results,
             errors=errors,
         )
 
-        path = os.path.join(self.config.target_path, CATALOG_FILENAME)
+        path = os.path.join(self.config.project_target_path, CATALOG_FILENAME)
         results.write(path)
         if self.args.compile:
-            write_manifest(self.manifest, self.config.target_path)
+            write_manifest(self.manifest, self.config.project_target_path)
 
         if exceptions:
             fire_event(WriteCatalogFailure(num_exceptions=len(exceptions)))
         fire_event(CatalogWritten(path=os.path.abspath(path)))
         return results
 
     def get_catalog_results(
```

### Comparing `dbt-core-1.6.0b2/dbt/task/init.py` & `dbt-core-1.6.0b3/dbt/task/init.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/task/list.py` & `dbt-core-1.6.0b3/dbt/task/list.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/task/printer.py` & `dbt-core-1.6.0b3/dbt/task/printer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/task/run.py` & `dbt-core-1.6.0b3/dbt/task/run.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/task/run_operation.py` & `dbt-core-1.6.0b3/dbt/task/run_operation.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,26 +45,28 @@
             )
 
         return res
 
     def run(self) -> RunResultsArtifact:
         start = datetime.utcnow()
         self.compile_manifest()
+
+        success = True
+
         try:
             self._run_unsafe()
         except dbt.exceptions.Exception as exc:
             fire_event(RunningOperationCaughtError(exc=str(exc)))
             fire_event(LogDebugStackTrace(exc_info=traceback.format_exc()))
             success = False
         except Exception as exc:
             fire_event(RunningOperationUncaughtError(exc=str(exc)))
             fire_event(LogDebugStackTrace(exc_info=traceback.format_exc()))
             success = False
-        else:
-            success = True
+
         end = datetime.utcnow()
 
         package_name, macro_name = self._get_macro_parts()
         fqn = [NodeType.Operation, package_name, macro_name]
         unique_id = ".".join(fqn)
 
         run_result = RunResult(
@@ -97,16 +99,17 @@
                 k: v
                 for k, v in self.args.__dict__.items()
                 if k.islower() and type(v) in (str, int, float, bool, list, dict)
             },
             results=[run_result],
         )
 
-        result_path = os.path.join(self.config.target_path, RESULT_FILE_NAME)
+        result_path = os.path.join(self.config.project_target_path, RESULT_FILE_NAME)
 
         if self.args.write_json:
             results.write(result_path)
 
         return results
 
-    def interpret_results(self, results):
+    @classmethod
+    def interpret_results(cls, results):
         return results.results[0].status == RunStatus.Success
```

### Comparing `dbt-core-1.6.0b2/dbt/task/runnable.py` & `dbt-core-1.6.0b3/dbt/task/runnable.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,35 +56,41 @@
 import dbt.utils
 
 RESULT_FILE_NAME = "run_results.json"
 RUNNING_STATE = DbtProcessState("running")
 
 
 class GraphRunnableTask(ConfiguredTask):
-
     MARK_DEPENDENT_ERRORS_STATUSES = [NodeStatus.Error]
 
     def __init__(self, args, config, manifest):
         super().__init__(args, config, manifest)
         self._flattened_nodes: Optional[List[ResultNode]] = None
         self._raise_next_tick = None
         self._skipped_children = {}
         self.job_queue: Optional[GraphQueue] = None
         self.node_results = []
         self.num_nodes: int = 0
         self.previous_state: Optional[PreviousState] = None
+        self.previous_defer_state: Optional[PreviousState] = None
         self.run_count: int = 0
         self.started_at: float = 0
 
-        self.set_previous_state()
-
-    def set_previous_state(self):
-        if self.args.state is not None:
+        if self.args.state:
             self.previous_state = PreviousState(
-                path=self.args.state, current_path=Path(self.config.target_path)
+                state_path=self.args.state,
+                target_path=Path(self.config.target_path),
+                project_root=Path(self.config.project_root),
+            )
+
+        if self.args.defer_state:
+            self.previous_defer_state = PreviousState(
+                state_path=self.args.defer_state,
+                target_path=Path(self.config.target_path),
+                project_root=Path(self.config.project_root),
             )
 
     def index_offset(self, value: int) -> int:
         return value
 
     @property
     def selection_arg(self):
@@ -152,15 +158,15 @@
     def raise_on_first_error(self):
         return False
 
     def get_runner_type(self, node):
         raise NotImplementedError("Not Implemented")
 
     def result_path(self):
-        return os.path.join(self.config.target_path, RESULT_FILE_NAME)
+        return os.path.join(self.config.project_target_path, RESULT_FILE_NAME)
 
     def get_runner(self, node):
         adapter = get_adapter(self.config)
         run_count: int = 0
         num_nodes: int = 0
 
         if node.is_ephemeral_model:
@@ -451,15 +457,15 @@
                     generated_at=result.generated_at.strftime("%Y-%m-%dT%H:%M:%SZ"),
                     elapsed_time=result.elapsed_time,
                     success=GraphRunnableTask.interpret_results(result.results),
                 )
             )
 
         if self.args.write_json:
-            write_manifest(self.manifest, self.config.target_path)
+            write_manifest(self.manifest, self.config.project_target_path)
             if hasattr(result, "write"):
                 result.write(self.result_path())
 
         self.task_end_messages(result.results)
         return result
 
     @classmethod
```

### Comparing `dbt-core-1.6.0b2/dbt/task/seed.py` & `dbt-core-1.6.0b3/dbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/task/serve.py` & `dbt-core-1.6.0b3/dbt/task/serve.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from dbt.include.global_project import DOCS_INDEX_FILE_PATH
 from dbt.task.base import ConfiguredTask
 
 
 class ServeTask(ConfiguredTask):
     def run(self):
-        os.chdir(self.config.target_path)
+        os.chdir(self.config.project_target_path)
         shutil.copyfile(DOCS_INDEX_FILE_PATH, "index.html")
 
         port = self.args.port
 
         if self.args.browser:
             webbrowser.open_new_tab(f"http://localhost:{port}")
```

### Comparing `dbt-core-1.6.0b2/dbt/task/show.py` & `dbt-core-1.6.0b3/dbt/task/show.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/task/snapshot.py` & `dbt-core-1.6.0b3/dbt/task/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/task/sql.py` & `dbt-core-1.6.0b3/dbt/task/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/task/test.py` & `dbt-core-1.6.0b3/dbt/task/test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/tests/fixtures/project.py` & `dbt-core-1.6.0b3/dbt/tests/fixtures/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/tests/util.py` & `dbt-core-1.6.0b3/dbt/tests/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/tracking.py` & `dbt-core-1.6.0b3/dbt/tracking.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/ui.py` & `dbt-core-1.6.0b3/dbt/ui.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/utils.py` & `dbt-core-1.6.0b3/dbt/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b2/dbt/version.py` & `dbt-core-1.6.0b3/dbt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,9 +228,9 @@
             # the path is like .../dbt/adapters/{plugin_name}/__version__.py
             # except it could be \\ on windows!
             plugin_root, _ = os.path.split(version_path)
             _, plugin_name = os.path.split(plugin_root)
             yield plugin_name
 
 
-__version__ = "1.6.0b2"
+__version__ = "1.6.0b3"
 installed = get_installed_version()
```

### Comparing `dbt-core-1.6.0b2/dbt_core.egg-info/PKG-INFO` & `dbt-core-1.6.0b3/dbt_core.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7.2
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt-core/fa1ea14ddfb1d5ae319d5141844910dd53ab2834/etc/dbt-core.svg" alt="dbt logo" width="750"/>
 </p>
 <p align="center">
   <a href="https://github.com/dbt-labs/dbt-core/actions/workflows/main.yml">
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b2 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b3 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >=3.7.2 Description-Content-Type:
-text/markdown
+Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
+Description-Content-Type: text/markdown
                                   [dbt logo]
                                   [CI_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. ![architecture](https://raw.githubusercontent.com/dbt-labs/
 dbt-core/6c6649f9129d5d108aa3b0526f634cd8f3a9d1ed/etc/dbt-arch.png) ##
 Understanding dbt Analysts using dbt can transform their data by simply writing
```

### Comparing `dbt-core-1.6.0b2/dbt_core.egg-info/SOURCES.txt` & `dbt-core-1.6.0b3/dbt_core.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 dbt/adapters/base/column.py
 dbt/adapters/base/connections.py
 dbt/adapters/base/impl.py
 dbt/adapters/base/meta.py
 dbt/adapters/base/plugin.py
 dbt/adapters/base/query_headers.py
 dbt/adapters/base/relation.py
+dbt/adapters/relation_configs/__init__.py
+dbt/adapters/relation_configs/config_base.py
+dbt/adapters/relation_configs/config_change.py
+dbt/adapters/relation_configs/config_validation.py
 dbt/adapters/sql/__init__.py
 dbt/adapters/sql/connections.py
 dbt/adapters/sql/impl.py
 dbt/cli/__init__.py
 dbt/cli/context.py
 dbt/cli/exceptions.py
 dbt/cli/flags.py
@@ -151,14 +155,20 @@
 dbt/include/global_project/macros/materializations/hooks.sql
 dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
 dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
 dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
 dbt/include/global_project/macros/materializations/models/incremental/merge.sql
 dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
 dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
+dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql
+dbt/include/global_project/macros/materializations/models/materialized_view/create_materialized_view.sql
+dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql
+dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql
+dbt/include/global_project/macros/materializations/models/materialized_view/refresh_materialized_view.sql
+dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql
 dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
 dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
 dbt/include/global_project/macros/materializations/models/table/table.sql
 dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
 dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
 dbt/include/global_project/macros/materializations/models/view/helpers.sql
 dbt/include/global_project/macros/materializations/models/view/view.sql
@@ -241,14 +251,15 @@
 dbt/task/deps.py
 dbt/task/freshness.py
 dbt/task/generate.py
 dbt/task/init.py
 dbt/task/list.py
 dbt/task/parse.py
 dbt/task/printer.py
+dbt/task/retry.py
 dbt/task/run.py
 dbt/task/run_operation.py
 dbt/task/runnable.py
 dbt/task/seed.py
 dbt/task/serve.py
 dbt/task/show.py
 dbt/task/snapshot.py
```

### Comparing `dbt-core-1.6.0b2/setup.py` & `dbt-core-1.6.0b3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 import os
 import sys
 
-if sys.version_info < (3, 7, 2):
+if sys.version_info < (3, 8):
     print("Error: dbt does not support this version of Python.")
-    print("Please upgrade to Python 3.7.2 or higher.")
+    print("Please upgrade to Python 3.8 or higher.")
     sys.exit(1)
 
 
 from setuptools import setup
 
 try:
     from setuptools import find_namespace_packages
@@ -21,15 +21,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
 package_name = "dbt-core"
-package_version = "1.6.0b2"
+package_version = "1.6.0b3"
 description = """With dbt, data analysts and engineers can build analytics \
 the way engineers build applications."""
 
 
 setup(
     name=package_name,
     version=package_version,
@@ -51,39 +51,38 @@
         "click>=7.0,<9",
         "colorama>=0.3.9,<0.4.7",
         "hologram>=0.0.14,<=0.0.16",
         "isodate>=0.6,<0.7",
         "logbook>=1.5,<1.6",
         "mashumaro[msgpack]==3.6",
         "minimal-snowplow-tracker==0.0.2",
-        "networkx>=2.3,<2.8.1;python_version<'3.8'",
-        "networkx>=2.3,<3;python_version>='3.8'",
+        "networkx>=2.3,<3",
         "packaging>20.9",
         "sqlparse>=0.2.3,<0.4.4",
         "dbt-extractor~=0.4.1",
         "typing-extensions>=3.7.4",
         "werkzeug>=1,<3",
         "pathspec>=0.9,<0.12",
         "protobuf>=4.0.0",
         "pytz>=2015.7",
         # the following are all to match snowflake-connector-python
         "requests<3.0.0",
         "idna>=2.5,<4",
         "cffi>=1.9,<2.0.0",
         "pyyaml>=5.3",
         "urllib3~=1.0",
+        "dbt-semantic-interfaces==0.1.0.dev3",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    python_requires=">=3.7.2",
+    python_requires=">=3.8",
 )
```

