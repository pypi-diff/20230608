# Comparing `tmp/c2cwsgiutils-5.2.2.tar.gz` & `tmp/c2cwsgiutils-6.0.0.dev88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c2cwsgiutils-5.2.2.tar", max compression
+gzip compressed data, was "c2cwsgiutils-6.0.0.dev88.tar", max compression
```

## Comparing `c2cwsgiutils-5.2.2.tar` & `c2cwsgiutils-6.0.0.dev88.tar`

### file list

```diff
@@ -1,65 +1,61 @@
--rw-r--r--   0        0        0     1304 2023-03-13 09:54:12.392344 c2cwsgiutils-5.2.2/LICENSE
--rw-r--r--   0        0        0    28624 2023-03-13 09:54:12.392344 c2cwsgiutils-5.2.2/README.md
--rw-r--r--   0        0        0     3997 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/__init__.py
--rw-r--r--   0        0        0     1500 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/__init__.py
--rw-r--r--   0        0        0     4620 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/composition.py
--rw-r--r--   0        0        0     9195 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/connection.py
--rw-r--r--   0        0        0     4491 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/image.py
--rw-r--r--   0        0        0     2329 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/print.py
--rw-r--r--   0        0        0     2072 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/utils.py
--rw-r--r--   0        0        0     9314 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/auth.py
--rw-r--r--   0        0        0     4160 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/__init__.py
--rw-r--r--   0        0        0      615 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/interface.py
--rw-r--r--   0        0        0     1062 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/local.py
--rw-r--r--   0        0        0     5058 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/redis.py
--rw-r--r--   0        0        0      272 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/utils.py
--rw-r--r--   0        0        0     3050 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/client_info.py
--rw-r--r--   0        0        0     1496 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/config_utils.py
--rw-r--r--   0        0        0      839 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/coverage_setup.py
--rw-r--r--   0        0        0    16140 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/db.py
--rw-r--r--   0        0        0     3049 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/db_maintenance_view.py
--rw-r--r--   0        0        0     1239 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/debug/__init__.py
--rw-r--r--   0        0        0     4364 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/debug/_listeners.py
--rw-r--r--   0        0        0     7507 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/debug/_views.py
--rw-r--r--   0        0        0     2328 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/debug/utils.py
--rw-r--r--   0        0        0     6723 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/errors.py
--rw-r--r--   0        0        0    20766 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/health_check.py
--rw-r--r--   0        0        0    17356 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/index.py
--rw-r--r--   0        0        0      628 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/loader.py
--rw-r--r--   0        0        0     3337 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/logging_view.py
--rw-r--r--   0        0        0     3425 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/metrics.py
--rw-r--r--   0        0        0     2691 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/models_graph.py
--rw-r--r--   0        0        0     1698 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/pretty_json.py
--rw-r--r--   0        0        0      739 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/profiler.py
--rw-r--r--   0        0        0     2062 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/prometheus.py
--rw-r--r--   0        0        0        0 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/py.typed
--rw-r--r--   0        0        0     1346 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/pyramid.py
--rw-r--r--   0        0        0     3703 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/pyramid_logging.py
--rw-r--r--   0        0        0     1478 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/redis_stats.py
--rw-r--r--   0        0        0     4527 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/redis_utils.py
--rw-r--r--   0        0        0     3823 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/request_tracking/__init__.py
--rw-r--r--   0        0        0      577 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/request_tracking/_sql.py
--rw-r--r--   0        0        0        0 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/__init__.py
--rwxr-xr-x   0        0        0     4147 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/check_es.py
--rwxr-xr-x   0        0        0     1998 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/genversion.py
--rwxr-xr-x   0        0        0     9594 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/stats_db.py
--rwxr-xr-x   0        0        0     2096 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/test_print.py
--rw-r--r--   0        0        0     5002 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sentry.py
--rw-r--r--   0        0        0     1567 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/services.py
--rw-r--r--   0        0        0     3494 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/setup_process.py
--rw-r--r--   0        0        0      876 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sql_profiler/__init__.py
--rw-r--r--   0        0        0     3680 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sql_profiler/_impl.py
--rw-r--r--   0        0        0     1552 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/README.md
--rw-r--r--   0        0        0        0 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/__init__.py
--rw-r--r--   0        0        0      752 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/_filters.py
--rw-r--r--   0        0        0     1477 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/_models.py
--rw-r--r--   0        0        0      460 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/examples/example.py
--rw-r--r--   0        0        0     4809 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/handlers.py
--rw-r--r--   0        0        0    11480 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/stats.py
--rw-r--r--   0        0        0      971 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/stats_pyramid/__init__.py
--rw-r--r--   0        0        0     2840 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/stats_pyramid/_db_spy.py
--rw-r--r--   0        0        0     2943 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/stats_pyramid/_pyramid_spy.py
--rw-r--r--   0        0        0      527 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/stats_pyramid/_views.py
--rw-r--r--   0        0        0     1817 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/version.py
--rw-r--r--   0        0        0     5299 2023-03-13 10:01:29.045817 c2cwsgiutils-5.2.2/pyproject.toml
--rw-r--r--   0        0        0    31538 1970-01-01 00:00:00.000000 c2cwsgiutils-5.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1304 2023-06-08 13:52:33.095343 c2cwsgiutils-6.0.0.dev88/LICENSE
+-rw-r--r--   0        0        0    29113 2023-06-08 13:52:33.099343 c2cwsgiutils-6.0.0.dev88/README.md
+-rw-r--r--   0        0        0     3997 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/__init__.py
+-rw-r--r--   0        0        0     1500 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/acceptance/__init__.py
+-rw-r--r--   0        0        0     5331 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/acceptance/composition.py
+-rw-r--r--   0        0        0     9109 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/acceptance/connection.py
+-rw-r--r--   0        0        0     4491 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/acceptance/image.py
+-rw-r--r--   0        0        0     2329 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/acceptance/print.py
+-rw-r--r--   0        0        0     2078 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/acceptance/utils.py
+-rw-r--r--   0        0        0     9313 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/auth.py
+-rw-r--r--   0        0        0     4372 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/broadcast/__init__.py
+-rw-r--r--   0        0        0      615 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/broadcast/interface.py
+-rw-r--r--   0        0        0     1062 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/broadcast/local.py
+-rw-r--r--   0        0        0     5064 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/broadcast/redis.py
+-rw-r--r--   0        0        0      272 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/broadcast/utils.py
+-rw-r--r--   0        0        0     3050 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/client_info.py
+-rw-r--r--   0        0        0     1496 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/config_utils.py
+-rw-r--r--   0        0        0      839 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/coverage_setup.py
+-rw-r--r--   0        0        0    16140 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/db.py
+-rw-r--r--   0        0        0     3049 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/db_maintenance_view.py
+-rw-r--r--   0        0        0     1239 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/debug/__init__.py
+-rw-r--r--   0        0        0     4370 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/debug/_listeners.py
+-rw-r--r--   0        0        0     7507 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/debug/_views.py
+-rw-r--r--   0        0        0     2328 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/debug/utils.py
+-rw-r--r--   0        0        0     6723 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/errors.py
+-rw-r--r--   0        0        0    20028 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/health_check.py
+-rw-r--r--   0        0        0    17356 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/index.py
+-rw-r--r--   0        0        0      628 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/loader.py
+-rw-r--r--   0        0        0     3337 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/logging_view.py
+-rw-r--r--   0        0        0     2691 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/models_graph.py
+-rw-r--r--   0        0        0     1698 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/pretty_json.py
+-rw-r--r--   0        0        0      739 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/profiler.py
+-rw-r--r--   0        0        0     6587 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/prometheus.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/py.typed
+-rw-r--r--   0        0        0     1388 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/pyramid.py
+-rw-r--r--   0        0        0     3703 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/pyramid_logging.py
+-rw-r--r--   0        0        0     1545 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/redis_stats.py
+-rw-r--r--   0        0        0     4689 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/redis_utils.py
+-rw-r--r--   0        0        0     4025 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/request_tracking/__init__.py
+-rw-r--r--   0        0        0      577 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/request_tracking/_sql.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/scripts/__init__.py
+-rwxr-xr-x   0        0        0     1998 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/scripts/genversion.py
+-rwxr-xr-x   0        0        0    10445 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/scripts/stats_db.py
+-rwxr-xr-x   0        0        0     2096 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/scripts/test_print.py
+-rw-r--r--   0        0        0     5002 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sentry.py
+-rw-r--r--   0        0        0     1567 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/services.py
+-rw-r--r--   0        0        0     3434 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/setup_process.py
+-rw-r--r--   0        0        0      876 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sql_profiler/__init__.py
+-rw-r--r--   0        0        0     3680 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sql_profiler/_impl.py
+-rw-r--r--   0        0        0     1552 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sqlalchemylogger/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sqlalchemylogger/__init__.py
+-rw-r--r--   0        0        0      752 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sqlalchemylogger/_filters.py
+-rw-r--r--   0        0        0     1477 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sqlalchemylogger/_models.py
+-rw-r--r--   0        0        0      460 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sqlalchemylogger/examples/example.py
+-rw-r--r--   0        0        0     4813 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sqlalchemylogger/handlers.py
+-rw-r--r--   0        0        0      747 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/stats_pyramid/__init__.py
+-rw-r--r--   0        0        0     2917 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/stats_pyramid/_db_spy.py
+-rw-r--r--   0        0        0     3209 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/stats_pyramid/_pyramid_spy.py
+-rw-r--r--   0        0        0     2877 2023-06-08 13:52:33.103343 c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/version.py
+-rw-r--r--   0        0        0     5186 2023-06-08 14:00:28.175231 c2cwsgiutils-6.0.0.dev88/pyproject.toml
+-rw-r--r--   0        0        0    31968 1970-01-01 00:00:00.000000 c2cwsgiutils-6.0.0.dev88/PKG-INFO
```

### Comparing `c2cwsgiutils-5.2.2/LICENSE` & `c2cwsgiutils-6.0.0.dev88/LICENSE`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/README.md` & `c2cwsgiutils-6.0.0.dev88/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Camptocamp WSGI utilities
 
 This is a Python 3 library (>=3.5) providing common tools for Camptocamp WSGI
 applications:
 
-- Provide a small framework for gathering performance statistics about
-  a web application (statsd protocol)
+- Provide prometheus metrics
 - Allow to use a master/slave PostgresQL configuration
 - Logging handler for CEE/UDP logs
   - An optional view to change runtime the log levels
 - SQL profiler to debug DB performance problems, disabled by default. Warning, it will slow down everything.
 - A view to get the version information about the application and the installed packages
 - A framework for implementing a health_check service
 - Error handlers to send JSON messages to the client in case of error
@@ -39,36 +38,36 @@
 - [gunicorn.conf.py](acceptance_tests/app/gunicorn.conf.py).
   Then replace `c2cwsgiutils_app` by your package name.
 
 You should install `c2cwsgiutils` with the tool you use to manage your pip dependencies.
 
 In the `Dockerfile` you should add the following lines:
 
-```
+```dockerfile
 # Generate the version file.
 RUN c2cwsgiutils-genversion $(git rev-parse HEAD)
 
 CMD ["gunicorn", "--paste=/app/production.ini"]
 
 # Default values for the environment variables
 ENV \
-    DEVELOPMENT=0 \
-    SQLALCHEMY_POOL_RECYCLE=30 \
-    SQLALCHEMY_POOL_SIZE=5 \
-    SQLALCHEMY_MAX_OVERFLOW=25 \
-    SQLALCHEMY_SLAVE_POOL_RECYCLE=30 \
-    SQLALCHEMY_SLAVE_POOL_SIZE=5 \
-    SQLALCHEMY_SLAVE_MAX_OVERFLOW=25\
-    LOG_TYPE=console \
-    OTHER_LOG_LEVEL=WARNING \
-    GUNICORN_LOG_LEVEL=WARNING \
-    GUNICORN_ACCESS_LOG_LEVEL=INFO \
-    SQL_LOG_LEVEL=WARNING \
-    C2CWSGIUTILS_LOG_LEVEL=WARNING \
-    LOG_LEVEL=INFO
+  DEVELOPMENT=0 \
+  SQLALCHEMY_POOL_RECYCLE=30 \
+  SQLALCHEMY_POOL_SIZE=5 \
+  SQLALCHEMY_MAX_OVERFLOW=25 \
+  SQLALCHEMY_SLAVE_POOL_RECYCLE=30 \
+  SQLALCHEMY_SLAVE_POOL_SIZE=5 \
+  SQLALCHEMY_SLAVE_MAX_OVERFLOW=25\
+  LOG_TYPE=console \
+  OTHER_LOG_LEVEL=WARNING \
+  GUNICORN_LOG_LEVEL=WARNING \
+  GUNICORN_ACCESS_LOG_LEVEL=INFO \
+  SQL_LOG_LEVEL=WARNING \
+  C2CWSGIUTILS_LOG_LEVEL=WARNING \
+  LOG_LEVEL=INFO
 ```
 
 Add in your `main` function.
 
 ```python
 config.include("c2cwsgiutils.pyramid")
 dbsession = c2cwsgiutils.db.init(config, "sqlalchemy", "sqlalchemy_slave")
@@ -266,55 +265,14 @@
 `c2c_request_id` attribute on the Pyramid Request objects. The `requests` module is patched to automatically
 add this header.
 
 The requests module is also patched to monitor requests done without timeout. In that case, you can
 configure a default timeout with the `C2C_REQUESTS_DEFAULT_TIMEOUT` environment variable
 (`c2c.requests_default_timeout`). If no timeout and no default is specified, a warning is issued.
 
-## Metrics
-
-To enable and configure the metrics framework, you can use:
-
-- STATS_VIEW (c2c.stats_view): if defined, will enable the stats view `{C2C_BASE_PATH}/stats.json`
-- STATSD_ADDRESS (c2c.statsd_address): if defined, send stats to the given statsd server
-- STATSD_PREFIX (c2c.statsd_prefix): prefix to add to every metric names
-- STATSD_USE_TAGS: If true, automatic metrics will use tags
-- STATSD*TAG*{tag_name}: To set a global tag for the service
-
-If enabled, some metrics are automatically generated:
-
-- {STATSD_PREFIX}.route.{verb}.{route_name}.{status}: The time to process a query (includes rendering)
-- {STATSD_PREFIX}.render.{verb}.{route_name}.{status}: The time to render a query
-- {STATSD_PREFIX}.sql.{query}: The time to execute the given SQL query (simplified and normalized)
-- {STATSD_PREFIX}.requests.{scheme}.{hostname}.{port}.{verb}.{status}: The time to execute HTTP requests to
-  outside services (only the time between the start of sending of the request and when the header is
-  back with a chunk of the body)
-- {STATSD_PREFIX}.redis.{command}: The time to execute the given Redis command
-
-You can manually measure the time spent on something like that:
-
-```python
-from c2cwsgiutils import stats
-with stats.timer_context(['toto', 'tutu']):
-    do_something()
-```
-
-It will only add a timer event in case of success. If you want to measure both success and failures, do that:
-
-```python
-from c2cwsgiutils import stats
-with stats.outcome_timer_context(['toto', 'tutu']):
-    do_something()
-```
-
-Other functions exists to generate metrics. Look at the `c2cwsgiutils.stats` module.
-
-Look at the `c2cwsgiutils-stats-db` utility if you want to generate statistics (gauges) about the
-row counts.
-
 ## SQL profiler
 
 The SQL profiler must be configured with the `C2C_SQL_PROFILER_ENABLED` environment variable. That enables a view
 to query the status of the profiler (`{C2C_BASE_PATH}/sql_profiler?secret={C2C_SECRET}`) or to
 enable/disable it (`{C2C_BASE_PATH}/sql_profiler?secret={C2C_SECRET}&enable={1|0}`).
 
 If enabled, for each `SELECT` query sent by SQLAlchemy, another query it done with `EXPLAIN ANALYZE`
@@ -454,35 +412,108 @@
 
 ## Version information
 
 If the `/app/versions.json` exists, a view is added (`{C2C_BASE_PATH}/versions.json`) to query the current
 version of a app. This file is generated by calling the `c2cwsgiutils-genversion [$GIT_TAG] $GIT_HASH`
 command line. Usually done in the [Dockerfile](acceptance_tests/app/Dockerfile) of the WSGI application.
 
-## Metrics
+## Prometheus
+
+[Prometheus client](https://github.com/prometheus/client_python) is integrated in c2cwsgiutils.
+
+It will work in multi process mode with the limitation listed in the
+[`prometheus_client` documentation](https://github.com/prometheus/client_python#multiprocess-mode-eg-gunicorn).
+
+To enable it you should provide the `PROMETHEUS_PORT` environment variable.
+For security reason, this port should not be exposed.
+
+We can customize it with the following environment variables:
+
+- `PROMETHEUS_PREFIX`: to customize the prefix, default is `c2cwsggiutils-`.
+- `C2C_PROMETHEUS_PACKAGES` the packages that will be present in the version information, default is `c2cwsgiutils,pyramid,gunicorn,sqlalchemy`.
+- `C2C_PROMETHEUS_APPLICATION_PACKAGES` the packages that will be present in the version information as application.
+
+And you should add in your `gunicorn.conf.py`:
+
+```python
+from prometheus_client import multiprocess
+
+
+def on_starting(server):
+    from c2cwsgiutils import prometheus
+
+    del server
+
+    prometheus.start()
+
+
+def post_fork(server, worker):
+    from c2cwsgiutils import prometheus
 
-The path `/metrics` provide some metrics for Prometheus.
-By default we have the `smap` `pss`, but we can easily add the `rss`, `size` or your custom settings:
+    del server, worker
 
-Example:
+    prometheus.cleanup()
 
+
+def child_exit(server, worker):
+    del server
+
+    multiprocess.mark_process_dead(worker.pid)
+```
+
+In your `Dockerfile` you should add:
+
+```dockerfile
+RUN mkdir -p /prometheus-metrics \
+    chmod a+rwx /prometheus-metrics
+ENV PROMETHEUS_MULTIPROC_DIR=/prometheus-metrics
 ```
-from import c2cwsgiutils.metrics import add_provider, Provider, MemoryMapProvider
 
-class CustomProvider(Provider):
-    def __init__(self):
-        super().__init__("my_metrics", "My Metric")
+### Add custom metric collector
+
+See [official documentation](https://github.com/prometheus/client_python#custom-collectors).
+
+Related to the Unix process.
+
+```python
+from c2cwsgiutils import broadcast, prometheus
+
+prometheus.MULTI_PROCESS_COLLECTOR_BROADCAST_CHANNELS.append("prometheus_collector_custom")
+broadcast.subscribe("c2cwsgiutils_prometheus_collect_gc", _broadcast_collector_custom)
+my_custom_collector_instance = MyCustomCollector()
 
-    def get_data(self):
-        return [({'metadata_key': 'matadata_value'}, metrics_value)]
 
-add_provider(MemoryMapProvider('rss'))
-add_provider(CustomProvider())
+def _broadcast_collector_custom() -> List[prometheus.SerializedGauge]:
+    """Get the collected GC gauges."""
+
+    return prometheus.serialize_collected_data(my_custom_collector_instance)
 ```
 
+Related to the host, use that in the `gunicorn.conf.py`:
+
+```python
+def on_starting(server):
+    from c2cwsgiutils import prometheus
+
+    del server
+
+    registry = CollectorRegistry()
+    registry.register(MyCollector())
+    prometheus.start(registry)
+```
+
+### Database metrics
+
+Look at the `c2cwsgiutils-stats-db` utility if you want to generate statistics (gauges) about the
+row counts.
+
+### Usage of metrics
+
+With c2cwsgiutils each instance (Pod) has its own metrics, so we need to aggregate them to have the metrics for the service you probably need to use `sum by (<fields>) (<metric>)` to get the metric (especially for counters).
+
 ## Custom scripts
 
 To have the application initialized in a script you should use the
 `c2cwsgiutils.setup_process.bootstrap_application_from_options` function.
 
 Example of `main` function:
 
@@ -527,15 +558,15 @@
 To enable the debugging interface, you must set the `C2C_DEBUG_VIEW_ENABLED` environment variable. Then you can
 have dumps of a few things:
 
 - every threads' stacktrace: `{C2C_BASE_PATH}/debug/stacks?secret={C2C_SECRET}`
 - memory usage: `{C2C_BASE_PATH}/debug/memory?secret={C2C_SECRET}&limit=30&analyze_type=builtins.dict&python_internals_map=false`
 - object ref: `{C2C_BASE_PATH}/debug/show_refs.dot?secret={C2C_SECRET}&analyze_type=gunicorn.app.wsgiapp.WSGIApplication&analyze_id=12345&max_depth=3&too_many=10&filter=1024&no_extra_info&backrefs`
   `analyze_type` and `analyze_id` should not ve used toogether, you can use it like:
-  ```
+  ```bash
   curl "<URL>" > /tmp/show_refs.dot
   dot -Lg -Tpng /tmp/show_refs.dot > /tmp/show_refs.png
   ```
 - memory increase when calling another API: `{C2C_BASE_PATH}/debug/memory_diff?path={path_info}&secret={C2C_SECRET}&limit=30&no_warmup`
 - sleep the given number of seconds (to test load balancer timeouts): `{C2C_BASE_PATH}/debug/sleep?secret={C2C_SECRET}&time=60.2`
 - see the HTTP headers received by WSGI: `{C2C_BASE_PATH}/debug/headers?secret={C2C_SECRET}&status=500`
 - return an HTTP error: `{C2C_BASE_PATH}/debug/error?secret={C2C_SECRET}&status=500`
@@ -588,15 +619,15 @@
 You can enable this by setting `C2C_ENABLE_EXCEPTION_HANDLING` (`c2c.enable_exception_handling`) to "1".
 
 In development mode (`DEVELOPMENT=1`), all the details (SQL statement, stacktrace, ...) are sent to the
 client. In production mode, you can still get them by sending the secret defined in `C2C_SECRET` in the query.
 
 If you want to use pyramid_debugtoolbar, you need to disable exception handling and configure it like that:
 
-```
+```ini
 pyramid.includes =
     pyramid_debugtoolbar
 debugtoolbar.enabled = true
 debugtoolbar.hosts = 0.0.0.0/0
 debugtoolbar.intercept_exc = debug
 debugtoolbar.show_on_exc_only = true
 c2c.enable_exception_handling = 0
@@ -661,7 +692,16 @@
 To make a release:
 
 - Change the the version in [setup.py](setup.py).
 - Commit and push to master.
 - Tag the GIT commit.
 - Add the new branch name in the `.github/workflows/rebuild.yaml` and
   `.github/workflows/audit.yaml` files.
+
+## Contributing
+
+Install the pre-commit hooks:
+
+```bash
+pip install pre-commit
+pre-commit install --allow-missing-config
+```
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/__init__.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/__init__.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/acceptance/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/composition.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/acceptance/composition.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     return None
 
 
 class Composition:
     """The Docker composition."""
 
     def __init__(self, request: Request, composition: str, coverage_paths: Optional[str] = None) -> None:
-        warnings.warn("The c2cwsgiutils.acceptance.composition should be used only if it's relay needed.")
+        warnings.warn("The c2cwsgiutils.acceptance.composition should be used only if it's really needed.")
         self.cwd = os.path.dirname(composition)
         filename = os.path.basename(composition)
         self.docker_compose = ["docker-compose"]
         if filename != "docker-compose.yaml":
             self.docker_compose.append("--file=" + filename)
         self.coverage_paths = coverage_paths
         env = Composition._get_env()
@@ -60,39 +60,50 @@
         request.addfinalizer(log_watcher.kill)
         if os.environ.get("docker_stop", "1") == "1":
             request.addfinalizer(self.stop_all)
 
     def dc(self, args: List[str], **kwargs: Any) -> str:
         return cast(
             str,
-            subprocess.check_output(  # nosec
+            subprocess.run(  # nosec
                 self.docker_compose + args,
                 cwd=self.cwd,
                 env=Composition._get_env(),
                 stderr=subprocess.STDOUT,
+                stdout=subprocess.PIPE,
+                check=True,
                 **kwargs,
-            ).decode(),
+            ).stdout.decode(),
         )
 
+    def dc_process(self, args: List[str], **kwargs: Any) -> subprocess.CompletedProcess[str]:
+        kwargs = {
+            "cwd": self.cwd,
+            "env": Composition._get_env(),
+            **kwargs,
+        }
+        return subprocess.run(  # type: ignore[no-any-return, call-overload] # pylint: disable=subprocess-run-check # noqa
+            self.docker_compose + args,
+            **{"encoding": "utf-8", **kwargs},
+        )  # nosec
+
     def dc_try(self, args: List[str], **kwargs: Any) -> None:
         _try(
             lambda: self.dc(args),
             **kwargs,
         )
 
     def stop_all(self) -> None:
         self.dc_try(["stop"])
         if self.coverage_paths:
             target_dir = "/reports/"
             os.makedirs(target_dir, exist_ok=True)
             for path in self.coverage_paths:
                 try:
-                    subprocess.check_call(  # nosec
-                        ["docker", "cp", path, target_dir], stderr=subprocess.STDOUT
-                    )
+                    subprocess.run(["docker", "cp", path, target_dir], check=True, timeout=60)  # nosec
                 except Exception:
                     self.dc(["ps"])
                     raise
 
     def stop(self, container: str) -> None:
         self.dc_try(["stop", container])
 
@@ -101,14 +112,22 @@
 
     def run(self, container: str, *command: str, **kwargs: Dict[str, Any]) -> str:
         return self.dc(
             ["run", "--rm", container] + list(command),
             **kwargs,
         )
 
+    def run_proc(
+        self, container: str, *command: str, **kwargs: Dict[str, Any]
+    ) -> subprocess.CompletedProcess[str]:
+        return self.dc_process(
+            ["run", "--rm", container] + list(command),
+            **kwargs,
+        )
+
     def exec(self, container: str, *command: str, **kwargs: Dict[str, Any]) -> str:
         return self.dc(["exec", "-T", container] + list(command), **kwargs)
 
     @staticmethod
     def _get_env() -> Mapping[str, str]:
         """
         Make sure the DOCKER_TAG environment variable.
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/connection.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/acceptance/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         cache_expected: CacheExpected = CacheExpected.NO,
         **kwargs: Any,
     ) -> Optional[str]:
         """Get the given URL (relative to the root of API)."""
         with self.session.get(self.base_url + url, headers=self._merge_headers(headers, cors), **kwargs) as r:
             check_response(r, expected_status, cache_expected=cache_expected)
             self._check_cors(cors, r)
-            return None if r.status_code == 204 else r.text  # type: ignore
+            return None if r.status_code == 204 else r.text
 
     def get_raw(
         self,
         url: str,
         expected_status: int = 200,
         headers: Optional[Mapping[str, str]] = None,
         cors: bool = True,
@@ -86,17 +86,16 @@
             self.base_url + url,
             headers=self._merge_headers(headers, cors),
             stream=True,
             **kwargs,
         ) as r:
             check_response(r, expected_status, cache_expected=cache_expected)
             self._check_cors(cors, r)
-            r.raw.decode_content = True  # type: ignore
-            raw = r.raw  # type: ignore
-            doc = etree.parse(raw)  # nosec
+            r.raw.decode_content = True
+            doc = etree.parse(r.raw)  # nosec
             if schema is not None:
                 with open(schema, encoding="utf-8") as schema_file:
                     xml_schema = etree.XMLSchema(etree.parse(schema_file))  # nosec
                 xml_schema.assertValid(doc)
             return doc
 
     def post_json(
@@ -144,15 +143,15 @@
     ) -> Optional[str]:
         """POST the given URL (relative to the root of API)."""
         with self.session.post(
             self.base_url + url, headers=self._merge_headers(headers, cors), **kwargs
         ) as r:
             check_response(r, expected_status, cache_expected)
             self._check_cors(cors, r)
-            return None if r.status_code == 204 else r.text  # type: ignore
+            return None if r.status_code == 204 else r.text
 
     def put_json(
         self,
         url: str,
         expected_status: int = 200,
         headers: Optional[Mapping[str, str]] = None,
         cors: bool = True,
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/image.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/acceptance/image.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/print.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/acceptance/print.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/utils.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/acceptance/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,27 +41,27 @@
 
     Arguments:
 
         what: the function to try
         timeout: the timeout to get a success
         interval: the interval between try
     """
-    timeout = time.monotonic() + timeout
+    timeout = time.perf_counter() + timeout
     while True:
         error = ""
         try:
             ret = what()
             if ret:
                 return ret
         except NameError:
             raise
         except Exception as e:  # pylint: disable=broad-except
             error = str(e)
             LOG.info("  Failed: %s", e)
-        if time.monotonic() > timeout:
+        if time.perf_counter() > timeout:
             assert False, "Timeout: " + error
         time.sleep(interval)
 
 
 def approx(struct: Any, **kwargs: Any) -> Any:
     """
     Make float values in deep structures approximative.
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/auth.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,14 @@
         request.response.set_cookie(SECRET_ENV, secret_hash, max_age=COOKIE_AGE, httponly=True)
         # since this could be used from outside c2cwsgiutils views, we cannot set the path to c2c
         return True
     return False
 
 
 def _is_auth_user_github(request: pyramid.request.Request) -> Tuple[bool, UserDetails]:
-
     settings = request.registry.settings
     cookie = request.cookies.get(
         env_or_settings(
             settings,
             GITHUB_AUTH_COOKIE_ENV,
             GITHUB_AUTH_COOKIE_PROP,
             "c2c-auth-jwt",
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/__init__.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/broadcast/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,33 +32,41 @@
     broadcast_prefix = config_utils.env_or_config(
         config, BROADCAST_ENV_KEY, BROADCAST_CONFIG_KEY, "broadcast_api_"
     )
     master, slave, _ = redis_utils.get(config.get_settings() if config else None)
     if _broadcaster is None:
         if master is not None and slave is not None:
             _broadcaster = redis.RedisBroadcaster(broadcast_prefix, master, slave)
+            LOG.info("Broadcast service setup using Redis implementation")
         else:
             _broadcaster = local.LocalBroadcaster()
             LOG.info("Broadcast service setup using local implementation")
     elif isinstance(_broadcaster, local.LocalBroadcaster) and master is not None and slave is not None:
-        LOG.info("Switching from a local broadcaster to a redis broadcaster")
+        LOG.info("Switching from a local broadcaster to a Redis broadcaster")
         prev_broadcaster = _broadcaster
         _broadcaster = redis.RedisBroadcaster(broadcast_prefix, master, slave)
         _broadcaster.copy_local_subscriptions(prev_broadcaster)
 
 
 def _get(need_init: bool = False) -> interface.BaseBroadcaster:
     global _broadcaster
     if _broadcaster is None:
         if need_init:
             LOG.error("Broadcast functionality used before it is setup")
         _broadcaster = local.LocalBroadcaster()
     return _broadcaster
 
 
+def cleanup() -> None:
+    """Cleanup the broadcaster to force to reinitialize it."""
+
+    global _broadcaster
+    _broadcaster = None
+
+
 def subscribe(channel: str, callback: Callable[..., Any]) -> None:
     """
     Subscribe to a broadcast channel with the given callback.
 
     The callback will be called with its parameters
     taken from the dict provided in the _broadcaster.broadcast "params" parameter.
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/interface.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/broadcast/interface.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/local.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/broadcast/local.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/redis.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/broadcast/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,18 +89,18 @@
         LOG.debug("Subscribing for broadcast answers on %s", answer_channel)
         self._pub_sub.subscribe(**{answer_channel: callback})
         message = {"params": params, "answer_channel": answer_channel}
 
         try:
             nb_received = self._broadcast(channel, message)
 
-            timeout_time = time.monotonic() + timeout
+            timeout_time = time.perf_counter() + timeout
             with cond:
                 while len(answers) < nb_received:
-                    to_wait = timeout_time - time.monotonic()
+                    to_wait = timeout_time - time.perf_counter()
                     if to_wait <= 0.0:  # pragma: no cover
                         LOG.warning(
                             "timeout waiting for %d/%d answers on %s",
                             len(answers),
                             nb_received,
                             answer_channel,
                         )
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/client_info.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/client_info.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/config_utils.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/coverage_setup.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/coverage_setup.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/db.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/db.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/db_maintenance_view.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/db_maintenance_view.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/debug/__init__.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/debug/_listeners.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/debug/_listeners.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     }
 
     if python_internals_map and not analyze_type:
         analyze_type = "builtins.dict"
 
     if analyze_type:
         # timeout after one minute, must be set to a bit less that the timeout of the broadcast in _views.py
-        timeout = time.monotonic() + 60
+        timeout = time.perf_counter() + 60
 
         mod_counts: Dict[str, int] = {}
         biggest_objects: List[Tuple[float, Any]] = []
         result[analyze_type] = {}
         for obj in objgraph.by_type(analyze_type):
             if analyze_type == "builtins.function":
                 short = obj.__module__.split(".")[0] if obj.__module__ is not None else ""
@@ -76,15 +76,15 @@
                         continue
                 size = get_size(obj) / 1024
                 if len(biggest_objects) < limit or size > biggest_objects[0][0]:
                     biggest_objects.append((size, obj))
                     biggest_objects.sort(key=lambda x: x[0])
                     if len(biggest_objects) > limit:
                         biggest_objects = biggest_objects[-limit:]
-            if time.monotonic() > timeout:
+            if time.perf_counter() > timeout:
                 result[analyze_type]["timeout"] = True
                 break
         if analyze_type == "builtins.function":
             result[analyze_type]["modules"] = [
                 {"module": i[0], "nb_func": i[1]}
                 for i in sorted(mod_counts.items(), key=lambda x: -x[1])[:limit]
             ]
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/debug/_views.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/debug/_views.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/debug/utils.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/debug/utils.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/errors.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/errors.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/health_check.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/health_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import copy
 import logging
 import os
 import re
 import subprocess  # nosec
 import time
 import traceback
-from collections import Counter
 from enum import Enum
 from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
@@ -26,33 +25,53 @@
     Optional,
     Tuple,
     Type,
     Union,
     cast,
 )
 
+import prometheus_client
 import pyramid.config
 import pyramid.request
 import requests
 import sqlalchemy.engine
 import sqlalchemy.orm
 import sqlalchemy.sql
 from pyramid.httpexceptions import HTTPNotFound
 
 import c2cwsgiutils.db
-from c2cwsgiutils import auth, broadcast, config_utils, redis_utils, stats, version
+from c2cwsgiutils import auth, broadcast, config_utils, prometheus, redis_utils, version
 
 if TYPE_CHECKING:
     scoped_session = sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]
 else:
     scoped_session = sqlalchemy.orm.scoped_session
 
 LOG = logging.getLogger(__name__)
 ALEMBIC_HEAD_RE = re.compile(r"^([a-f0-9]+) \(head\)\n$")
 
+_PROMETHEUS_DB_SUMMARY = prometheus_client.Summary(
+    prometheus.build_metric_name("health_check_db"),
+    "The to do a database query",
+    ["configuration", "connection", "check"],
+    unit="seconds",
+)
+_PROMETHEUS_ALEMBIC_VERSION = prometheus_client.Gauge(
+    prometheus.build_metric_name("alembic_version"),
+    "The alembic version of the database",
+    ["version", "name", "configuration"],
+    multiprocess_mode="liveall",
+)
+_PROMETHEUS_HEALTH_CHECKS_FAILURE = prometheus_client.Gauge(
+    prometheus.build_metric_name("health_check_failure"),
+    "The health check",
+    ["name"],
+    multiprocess_mode="livemax",
+)
+
 
 class EngineType(Enum):
     """The type of engine."""
 
     READ_ONLY = 1
     WRITE_ONLY = 2
     READ_AND_WRITE = 3
@@ -279,43 +298,29 @@
                 self.session = session
 
             def __call__(self, request: pyramid.request.Request) -> str:
                 assert version_schema
                 assert version_table
                 for binding in _get_bindings(self.session, EngineType.READ_AND_WRITE):
                     with binding as binded_session:
-                        if stats.USE_TAGS:
-                            key = ["sql", "manual", "health_check", "alembic"]
-                            tags: Optional[Dict[str, str]] = {"conf": alembic_ini_path, "con": binding.name()}
-                        else:
-                            key = [
-                                "sql",
-                                "manual",
-                                "health_check",
-                                "alembic",
-                                alembic_ini_path,
-                                binding.name(),
-                            ]
-                            tags = None
-                        with stats.timer_context(key, tags):
+                        with _PROMETHEUS_DB_SUMMARY.labels(
+                            configuration=alembic_ini_path, connection=binding.name(), check="alembic"
+                        ).time():
                             result = binded_session.execute(
                                 sqlalchemy.text(
                                     "SELECT version_num FROM "  # nosec
                                     f"{sqlalchemy.sql.quoted_name(version_schema, True)}."
                                     f"{sqlalchemy.sql.quoted_name(version_table, True)}"
                                 )
                             ).fetchone()
                             assert result is not None
                             (actual_version,) = result
-                            if stats.USE_TAGS:
-                                stats.increment_counter(
-                                    ["alembic_version"], 1, tags={"version": actual_version, "name": name}
-                                )
-                            else:
-                                stats.increment_counter(["alembic_version", name, actual_version], 1)
+                            _PROMETHEUS_ALEMBIC_VERSION.labels(
+                                version=actual_version, name=name, configuration=alembic_ini_path
+                            ).set(1)
                             if actual_version != version_:
                                 raise Exception(  # pylint: disable=broad-exception-raised
                                     f"Invalid alembic version (db: {actual_version}, code: {version_})"
                                 )
                 return version_
 
         self._checks.append(
@@ -424,26 +429,19 @@
         Keyword Arguments:
 
             name: the name of the check (defaults to "version")
             level: the level of the health check
         """
 
         def check(request: pyramid.request.Request) -> Dict[str, Any]:
+            ref = version.get_version()
             all_versions = _get_all_versions()
             assert all_versions
             versions = [e for e in all_versions if e is not None]
-            # Output the versions we see on the monitoring
-            v: Optional[str]
-            for v, count in Counter(versions).items():
-                if stats.USE_TAGS:
-                    stats.increment_counter(["version"], count, tags={"version": v})
-                else:
-                    stats.increment_counter(["version", v], count)
 
-                ref = versions[0]
             assert all(v == ref for v in versions), "Non identical versions: " + ", ".join(versions)
             return {"version": ref, "count": len(versions)}
 
         assert name
         self._checks.append((name, check, level))
 
     def add_custom_check(
@@ -489,51 +487,41 @@
         check: Callable[[pyramid.request.Request], Any],
         is_auth: bool,
         level: int,
         name: str,
         request: pyramid.request.Request,
         results: Dict[str, Dict[str, Any]],
     ) -> None:
-        start = time.monotonic()
+        start = time.perf_counter()
         try:
             result = check(request)
-            results["successes"][name] = {"timing": time.monotonic() - start, "level": level}
+            results["successes"][name] = {"timing": time.perf_counter() - start, "level": level}
             if result is not None:
                 results["successes"][name]["result"] = result
-            if stats.USE_TAGS:
-                stats.increment_counter(["health_check"], 1, tags={"name": name, "outcome": "success"})
-            else:
-                stats.increment_counter(["health_check", name, "success"], 1)
+            _set_success(check_name=name)
         except Exception as e:  # pylint: disable=broad-except
-            if stats.USE_TAGS:
-                stats.increment_counter(["health_check"], 1, tags={"name": name, "outcome": "failure"})
-            else:
-                stats.increment_counter(["health_check", name, "failure"], 1)
+            _PROMETHEUS_HEALTH_CHECKS_FAILURE.labels(name=name).set(1)
             LOG.warning("Health check %s failed", name, exc_info=True)
-            failure = {"message": str(e), "timing": time.monotonic() - start, "level": level}
+            failure = {"message": str(e), "timing": time.perf_counter() - start, "level": level}
             if isinstance(e, JsonCheckException) and e.json_data() is not None:
                 failure["result"] = e.json_data()
             if is_auth or os.environ.get("DEVELOPMENT", "0") != "0":
                 failure["stacktrace"] = traceback.format_exc()
             results["failures"][name] = failure
 
     @staticmethod
     def _create_db_engine_check(
         binding: _Binding,
         query_cb: Callable[[scoped_session], None],
     ) -> Tuple[str, Callable[[pyramid.request.Request], None]]:
         def check(request: pyramid.request.Request) -> None:
             with binding as session:
-                if stats.USE_TAGS:
-                    key = ["sql", "manual", "health_check", "db"]
-                    tags: Optional[Dict[str, str]] = {"con": binding.name()}
-                else:
-                    key = ["sql", "manual", "health_check", "db", binding.name()]
-                    tags = None
-                with stats.timer_context(key, tags):
+                with _PROMETHEUS_DB_SUMMARY.labels(
+                    connection=binding.name(), check="database", configuration="<default>"
+                ).time():
                     return query_cb(session)
 
         return "db_engine_" + binding.name(), check
 
     @staticmethod
     def _at_least_one(model: Any) -> Callable[[scoped_session], Any]:
         def query(session: scoped_session) -> None:
@@ -544,10 +532,17 @@
         return query
 
 
 def _maybe_function(what: Any, request: pyramid.request.Request) -> Any:
     return what(request) if callable(what) else what
 
 
+@broadcast.decorator(expect_answers=False)
+def _set_success(check_name: str) -> None:
+    """Set check in success in all process."""
+
+    _PROMETHEUS_HEALTH_CHECKS_FAILURE.labels(name=check_name).set(0)
+
+
 @broadcast.decorator(expect_answers=True)
 def _get_all_versions() -> Optional[str]:
     return version.get_version()
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/index.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/index.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/loader.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/loader.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/logging_view.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/logging_view.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/models_graph.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/models_graph.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/pretty_json.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/pretty_json.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/profiler.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/profiler.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/pyramid.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/pyramid.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,26 @@
     broadcast,
     coverage_setup,
     db_maintenance_view,
     debug,
     errors,
     index,
     logging_view,
-    metrics,
     pretty_json,
+    prometheus,
     redis_stats,
     request_tracking,
     sentry,
     sql_profiler,
     stats_pyramid,
     version,
 )
 
+_LOG = logging.getLogger(__name__)
+
 
 def includeme(config: pyramid.config.Configurator) -> None:
     """
     Initialize all the pyramid services and event handlers provided by this library.
 
     Arguments:
 
@@ -42,11 +44,11 @@
     config.include(stats_pyramid.includeme)
     config.include(request_tracking.includeme)
     config.include(redis_stats.includeme)
     config.include(db_maintenance_view.includeme)
     config.include(logging_view.includeme)
     config.include(sql_profiler.includeme)
     config.include(version.includeme)
+    config.include(prometheus.includeme)
     config.include(debug.includeme)
-    config.include(metrics.includeme)
     config.include(errors.includeme)
     config.include(index.includeme)
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/pyramid_logging.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/pyramid_logging.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/redis_stats.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/redis_stats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import logging
 import warnings
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Optional
 
+import prometheus_client
 import pyramid.config
 
-from c2cwsgiutils import config_utils, stats
+from c2cwsgiutils import config_utils, prometheus
 
 LOG = logging.getLogger(__name__)
 ORIG: Optional[Callable[..., Any]] = None
 
+_PROMETHEUS_REDIS_SUMMARY = prometheus_client.Summary(
+    prometheus.build_metric_name("redis"),
+    "Number of redis commands",
+    ["command"],
+    unit="seconds",
+)
 
-def _execute_command_patch(self: Any, *args: Any, **options: Any) -> Any:
-    if stats.USE_TAGS:
-        key = ["redis"]
-        tags: Optional[Dict[str, str]] = {"cmd": args[0]}
-    else:
-        key = ["redis", args[0]]
-        tags = None
+
+def _execute_command_patch(self: Any, command: str, *args: Any, **options: Any) -> Any:
     assert ORIG is not None
-    with stats.outcome_timer_context(key, tags):
-        return ORIG(self, *args, **options)
+    with _PROMETHEUS_REDIS_SUMMARY.labels(command=command).time():
+        return ORIG(self, command, *args, **options)
 
 
 def init(config: Optional[pyramid.config.Configurator] = None) -> None:
     """Initialize the Redis tracking, for backward compatibility."""
     warnings.warn("init function is deprecated; use includeme instead")
     includeme(config)
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/redis_utils.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/redis_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,22 @@
 REDIS_DB_KEY_PROP = "c2c.redis_db"
 
 _master: Optional["redis.client.Redis[str]"] = None
 _slave: Optional["redis.client.Redis[str]"] = None
 _sentinel: Optional[redis.sentinel.Sentinel] = None
 
 
+def cleanup() -> None:
+    """Cleanup the redis connections."""
+    global _master, _slave, _sentinel
+    _master = None
+    _slave = None
+    _sentinel = None
+
+
 def get(
     settings: Optional[Mapping[str, bytes]] = None,
 ) -> Tuple[
     Optional["redis.client.Redis[str]"],
     Optional["redis.client.Redis[str]"],
     Optional[redis.sentinel.Sentinel],
 ]:
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/request_tracking/__init__.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/request_tracking/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,86 @@
 """
 Allows to track the request_id in the logs, the DB and others.
 
 Adds a c2c_request_id attribute to the Pyramid Request class to access it.
 """
 import logging
+import time
 import urllib.parse
 import uuid
 import warnings
-from typing import Any, Dict, List, Optional, Sequence
+from typing import List, Mapping, Optional, Tuple, Union
 
+import prometheus_client
 import pyramid.request
 import requests.adapters
 import requests.models
 from pyramid.threadlocal import get_current_request
 
-from c2cwsgiutils import config_utils, stats
+from c2cwsgiutils import config_utils, prometheus
 
 ID_HEADERS: List[str] = []
 _HTTPAdapter_send = requests.adapters.HTTPAdapter.send
 LOG = logging.getLogger(__name__)
 DEFAULT_TIMEOUT: Optional[float] = None
+_PROMETHEUS_REQUESTS_SUMMARY = prometheus_client.Summary(
+    prometheus.build_metric_name("requests"),
+    "Requests requests",
+    ["scheme", "hostname", "port", "method", "status", "group"],
+    unit="seconds",
+)
 
 
 def _gen_request_id(request: pyramid.request.Request) -> str:
     for id_header in ID_HEADERS:
         if id_header in request.headers:
             return request.headers[id_header]  # type: ignore
     return str(uuid.uuid4())
 
 
 def _patch_requests() -> None:
     def send_wrapper(
         self: requests.adapters.HTTPAdapter,
         request: requests.models.PreparedRequest,
-        timeout: Optional[float] = None,
-        **kwargs: Any,
+        stream: bool = False,
+        timeout: Union[None, float, Tuple[float, float], Tuple[float, None]] = None,
+        verify: Union[bool, str] = True,
+        cert: Union[None, bytes, str, Tuple[Union[bytes, str], Union[bytes, str]]] = None,
+        proxies: Optional[Mapping[str, str]] = None,
     ) -> requests.Response:
         pyramid_request = get_current_request()
         header = ID_HEADERS[0]
         if pyramid_request is not None and header not in request.headers:
             request.headers[header] = pyramid_request.c2c_request_id
 
         if timeout is None:
             if DEFAULT_TIMEOUT is not None:
                 timeout = DEFAULT_TIMEOUT
             else:
                 LOG.warning("Doing a %s request without timeout to %s", request.method, request.url)
 
-        status = 999
-        timer = stats.timer()
-        try:
-            response = _HTTPAdapter_send(self, request, timeout=timeout, **kwargs)
-            status = response.status_code
-            return response
-        finally:
-            if request.url is not None:
-                parsed = urllib.parse.urlparse(request.url)
-                port = parsed.port or (80 if parsed.scheme == "http" else 443)
-                if stats.USE_TAGS:
-                    key: Sequence[Any] = ["requests"]
-                    tags: Optional[Dict[str, Any]] = {
-                        "scheme": parsed.scheme,
-                        "host": parsed.hostname,
-                        "port": port,
-                        "method": request.method,
-                        "status": status,
-                    }
-                else:
-                    key = ["requests", parsed.scheme, parsed.hostname, port, request.method, status]
-                    tags = None
-                timer.stop(key, tags)
+        assert request.url
+        parsed = urllib.parse.urlparse(request.url)
+        port = parsed.port or (80 if parsed.scheme == "http" else 443)
+        start = time.perf_counter()
+        response = _HTTPAdapter_send(
+            self, request, timeout=timeout, stream=stream, verify=verify, cert=cert, proxies=proxies
+        )
+
+        _PROMETHEUS_REQUESTS_SUMMARY.labels(
+            scheme=parsed.scheme,
+            hostname=parsed.hostname,
+            port=str(port),
+            method=request.method,
+            status=str(response.status_code),
+            group=str(response.status_code // 100 * 100),
+        ).observe(time.perf_counter() - start)
+        return response
 
-    requests.adapters.HTTPAdapter.send = send_wrapper  # type: ignore
+    requests.adapters.HTTPAdapter.send = send_wrapper  # type: ignore[method-assign]
 
 
 def init(config: Optional[pyramid.config.Configurator] = None) -> None:
     """Initialize the request tracking, for backward compatibility."""
     warnings.warn("init function is deprecated; use includeme instead")
     includeme(config)
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/request_tracking/_sql.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/request_tracking/_sql.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/genversion.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/scripts/genversion.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/stats_db.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/scripts/stats_db.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 #!/usr/bin/env python3
-"""Emits statsd gauges for every tables of a database."""
+"""Provide prometheus gauges for every tables of a database."""
+
 import argparse
 import logging
 import os
 import sys
 import time
 from typing import TYPE_CHECKING, Dict, List, Optional
+from wsgiref.simple_server import make_server
 
 import sqlalchemy
 import sqlalchemy.exc
 import sqlalchemy.orm
 import transaction
+from prometheus_client import CollectorRegistry, Gauge, push_to_gateway
+from prometheus_client.exposition import make_wsgi_app
 from zope.sqlalchemy import register
 
 import c2cwsgiutils.setup_process
-from c2cwsgiutils import stats
-from c2cwsgiutils.prometheus import PushgatewayGroupPublisher
+from c2cwsgiutils import prometheus
 
 if TYPE_CHECKING:
     scoped_session = sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]
 else:
     scoped_session = sqlalchemy.orm.scoped_session
 
 LOG = logging.getLogger(__name__)
@@ -29,21 +32,25 @@
     parser = argparse.ArgumentParser(description=__doc__)
     c2cwsgiutils.setup_process.fill_arguments(parser)
     parser.add_argument("--db", type=str, required=True, help="DB connection string")
     parser.add_argument(
         "--schema", type=str, action="append", required=True, default=["public"], help="schema to dump"
     )
     parser.add_argument(
-        "--extra", type=str, action="append", help="A SQL query that returns a metric name and a value"
-    )
-    parser.add_argument(
-        "--statsd-address", "--statsd_address", type=str, help="address:port for the statsd daemon"
+        "--extra",
+        type=str,
+        action="append",
+        help="A SQL query that returns a metric name and a value",
     )
     parser.add_argument(
-        "--statsd-prefix", "--statsd_prefix", type=str, default="c2c", help="prefix for the statsd metrics"
+        "--extra-gauge",
+        type=str,
+        action="append",
+        nargs=3,
+        help="A SQL query that returns a metric name and a value, with gauge name and help",
     )
     parser.add_argument(
         "--prometheus-url", "--prometheus_url", type=str, help="Base URL for the Prometheus Pushgateway"
     )
     parser.add_argument(
         "--prometheus-instance",
         "--prometheus_instance",
@@ -55,51 +62,47 @@
 
 
 class Reporter:
     """The stats reporter."""
 
     def __init__(self, args: argparse.Namespace) -> None:
         self._error: Optional[Exception] = None
-        if args.statsd_address:
-            self.statsd: Optional[stats.StatsDBackend] = stats.StatsDBackend(
-                args.statsd_address, args.statsd_prefix, tags=stats.get_env_tags()
+        self.registry = CollectorRegistry()
+        self.prometheus_push = args.prometheus_url is not None
+        self.args = args
+        self.gauges: Dict[str, Gauge] = {}
+
+    def get_gauge(self, kind: str, kind_help: str, labels: List[str]) -> Gauge:
+        if kind not in self.gauges:
+            self.gauges[kind] = Gauge(
+                prometheus.build_metric_name(f"database_{kind}"),
+                kind_help,
+                labels,
+                registry=self.registry,
             )
-        else:
-            self.statsd = None
-
-        if args.prometheus_url:
-            self.prometheus: Optional[PushgatewayGroupPublisher] = PushgatewayGroupPublisher(
-                args.prometheus_url,
-                "db_counts",
-                instance=args.prometheus_instance,
-                labels=stats.get_env_tags(),
-            )
-        else:
-            self.prometheus = None
+        return self.gauges[kind]
 
     def do_report(
-        self, metric: List[str], value: int, kind: str, tags: Optional[Dict[str, str]] = None
+        self, metric: List[str], value: int, kind: str, kind_help: str, tags: Dict[str, str]
     ) -> None:
         LOG.debug("%s.%s -> %d", kind, ".".join(metric), value)
-        if value > 0:  # Don't export 0 values. We can always set null=0 in grafana...
-            if self.statsd is not None:
-                if stats.USE_TAGS and tags is not None:
-                    self.statsd.gauge([kind], value, tags=tags)
-                else:
-                    self.statsd.gauge([kind] + metric, value)
-            if self.prometheus is not None:
-                self.prometheus.add("database_table_" + kind, value, metric_labels=tags)
+        gauge = self.get_gauge(kind, kind_help, list(tags.keys()))
+        gauge.labels(**tags).set(value)
 
     def commit(self) -> None:
-        if self.prometheus is not None:
-            self.prometheus.commit()
+        if self.prometheus_push:
+            push_to_gateway(self.args.prometheus_url, job="db_counts", registry=self.registry)
+        else:
+            port = int(os.environ.get("PROMETHEUS_PORT", "9090"))
+            app = make_wsgi_app(self.registry)
+            with make_server("", port, app) as httpd:
+                print(f"Waiting that Prometheus get the metrics served on port {port}...")
+                httpd.handle_request()
 
     def error(self, metric: List[str], error_: Exception) -> None:
-        if self.statsd is not None:
-            self.statsd.counter(["error"] + metric, 1)
         if self._error is None:
             self._error = error_
 
     def report_error(self) -> None:
         if self._error is not None:
             raise self._error
 
@@ -147,22 +150,24 @@
         ),
         params={"schema": schema, "table": table},
     ):
         for fork, value in (("main", size_main), ("fsm", size_fsm)):
             reporter.do_report(
                 [schema, table, index_name, fork],
                 value,
-                kind="index_size",
+                kind="table_index_size",
+                kind_help="Size of the index",
                 tags={"schema": schema, "table": table, "index": index_name, "fork": fork},
             )
         for action, value in (("scan", number_of_scans), ("read", tuples_read), ("fetch", tuples_fetched)):
             reporter.do_report(
                 [schema, table, index_name, action],
                 value,
-                kind="index_usage",
+                kind="table_index_usage",
+                kind_help="Usage of the index",
                 tags={"schema": schema, "table": table, "index": index_name, "action": action},
             )
 
 
 def _do_table_size(
     reporter: Reporter,
     schema: str,
@@ -179,41 +184,57 @@
     """
         ),
         params={"schema": schema, "table": table},
     ).fetchone()
     assert result is not None
     size: int
     (size,) = result
-    reporter.do_report([schema, table], size, kind="size", tags={"schema": schema, "table": table})
+    reporter.do_report(
+        [schema, table],
+        size,
+        kind="table_size",
+        kind_help="Size of the table",
+        tags={"schema": schema, "table": table},
+    )
 
 
 def _do_table_count(
     reporter: Reporter,
     schema: str,
     session: scoped_session,
     table: str,
 ) -> None:
     # We request and estimation of the count as a real count is very slow on big tables
     # and seems to cause replicatin lags. This estimate is updated on ANALYZE and VACUUM.
     result = session.execute(
-        sqlalchemy.text(  # nosec
-            "SELECT reltuples::bigint AS count FROM pg_class "
+        # Bandit does not recognize that `sqlalchemy.sql.quoted_name` as a safe function.
+        sqlalchemy.text(
+            "SELECT reltuples::bigint AS count FROM pg_class "  # nosec
             f"WHERE oid = '{sqlalchemy.sql.quoted_name(schema, True)}."
             f"{sqlalchemy.sql.quoted_name(table, True)}'::regclass;"
         )
     ).fetchone()
     assert result is not None
     (count,) = result
-    reporter.do_report([schema, table], count, kind="count", tags={"schema": schema, "table": table})
+    reporter.do_report(
+        [schema, table],
+        count,
+        kind="table_count",
+        kind_help="The number of row in the table",
+        tags={"schema": schema, "table": table},
+    )
 
 
-def do_extra(session: scoped_session, extra: str, reporter: Reporter) -> None:
+def do_extra(session: scoped_session, sql: str, kind: str, gauge_help: str, reporter: Reporter) -> None:
     """Do an extra report."""
-    for metric, count in session.execute(sqlalchemy.text(extra)):
-        reporter.do_report(str(metric).split("."), count, kind="count", tags={"metric": metric})
+
+    for metric, count in session.execute(sqlalchemy.text(sql)):
+        reporter.do_report(
+            str(metric).split("."), count, kind=kind, kind_help=gauge_help, tags={"metric": metric}
+        )
 
 
 def _do_dtats_db(args: argparse.Namespace) -> None:
     reporter = Reporter(args)
     try:
         engine = sqlalchemy.create_engine(args.db)
         factory = sqlalchemy.orm.sessionmaker(bind=engine)
@@ -240,34 +261,43 @@
             LOG.exception("Process table %s.%s error.", schema, table)
             reporter.error([schema, table], e)
 
     if args.extra:
         for pos, extra in enumerate(args.extra):
             LOG.info("Process extra %s.", extra)
             try:
-                do_extra(session, extra, reporter)
+                do_extra(session, extra, "extra", "Extra metric", reporter)
             except Exception as e:  # pylint: disable=broad-except
                 LOG.exception("Process extra %s error.", extra)
                 reporter.error(["extra", str(pos + 1)], e)
+    if args.extra_gauge:
+        for pos, extra in enumerate(args.extra_gauge):
+            sql, gauge, gauge_help = extra
+            LOG.info("Process extra %s.", extra)
+            try:
+                do_extra(session, sql, gauge, gauge_help, reporter)
+            except Exception as e:  # pylint: disable=broad-except
+                LOG.exception("Process extra %s error.", extra)
+                reporter.error(["extra", str(len(args.extra) + pos + 1)], e)
 
     reporter.commit()
     transaction.abort()
     reporter.report_error()
 
 
 def main() -> None:
     """Run the command."""
     success = False
     args = _parse_args()
-    c2cwsgiutils.setup_process.bootstrap_application_from_options(args)
+    c2cwsgiutils.setup_process.init_logging(args.config_uri)
     for _ in range(int(os.environ.get("C2CWSGIUTILS_STATS_DB_TRYNUMBER", 10))):
         try:
             _do_dtats_db(args)
             success = True
-            continue
+            break
         except:  # pylint: disable=bare-except
             LOG.exception("Exception during run")
         time.sleep(float(os.environ.get("C2CWSGIUTILS_STATS_DB_SLEEP", 1)))
 
     if not success:
         LOG.error("Not in success, exiting")
         sys.exit(1)
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/test_print.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/scripts/test_print.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/sentry.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sentry.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/services.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/services.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/setup_process.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/setup_process.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pyramid.config
 import pyramid.registry
 import pyramid.request
 import pyramid.router
 from pyramid.paster import bootstrap
 from pyramid.scripts.common import get_config_loader, parse_vars
 
-from c2cwsgiutils import broadcast, coverage_setup, redis_stats, sentry, sql_profiler, stats
+from c2cwsgiutils import broadcast, coverage_setup, redis_stats, sentry, sql_profiler
 
 
 def fill_arguments(
     parser: argparse.ArgumentParser,
     use_attribute: bool = False,
     default_config_uri: str = "c2c:///app/production.ini",
 ) -> None:
@@ -47,38 +47,34 @@
     loader = get_config_loader(config_file)
     loader.setup_logging(None)
     settings = loader.get_settings()
     config = pyramid.config.Configurator(settings=settings)
     coverage_setup.includeme()
     sentry.includeme(config)
     broadcast.includeme(config)
-    stats.init_backends(settings)
     redis_stats.includeme(config)
     sql_profiler.includeme(config)
 
 
 def init_logging(config_file: str = "c2c:///app/production.ini") -> None:
     """Initialize the non-WSGI application."""
     warnings.warn("init_logging function is deprecated; use init instead so that all features are enabled")
     loader = get_config_loader(config_file)
     loader.setup_logging(None)
 
 
-PyramidEnv = TypedDict(
-    "PyramidEnv",
-    {
-        "root": Any,
-        "closer": Callable[..., Any],
-        "registry": pyramid.registry.Registry,
-        "request": pyramid.request.Request,
-        "root_factory": object,
-        "app": Callable[[Dict[str, str], Any], Any],
-    },
-    total=True,
-)
+class PyramidEnv(TypedDict, total=True):
+    """The return type of the bootstrap functions."""
+
+    root: Any
+    closer: Callable[..., Any]
+    registry: pyramid.registry.Registry
+    request: pyramid.request.Request
+    root_factory: object
+    app: Callable[[Dict[str, str], Any], Any]
 
 
 def bootstrap_application_from_options(options: argparse.Namespace) -> PyramidEnv:
     """
     Initialize all the application from the command line arguments.
 
     :return: This function returns a dictionary as in bootstrap, see:
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/sql_profiler/__init__.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sql_profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/sql_profiler/_impl.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sql_profiler/_impl.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/README.md` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sqlalchemylogger/README.md`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/_filters.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sqlalchemylogger/_filters.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/_models.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sqlalchemylogger/_models.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/handlers.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/sqlalchemylogger/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,37 +50,37 @@
         if contains_expression:
             self.addFilter(ContainsExpression(contains_expression))
 
     def _processor(self) -> None:
         LOG.debug("%s: starting processor thread", __name__)
         while True:
             logs = []
-            time_since_last = time.monotonic()
+            time_since_last = time.perf_counter()
             while True:
                 with self.condition:
                     self.condition.wait(timeout=self.MAX_TIMEOUT)
                     if not self.log_queue.empty():
                         logs.append(self.log_queue.get())
                         self.log_queue.task_done()
                 if logs:
                     # try to reduce the number of INSERT requests to the DB
                     # by writing chunks of self.MAX_NB_LOGS size,
                     # but also do not wait forever before writing stuff (self.MAX_TIMOUT)
                     if (len(logs) >= self.MAX_NB_LOGS) or (
-                        time.monotonic() >= (time_since_last + self.MAX_TIMEOUT)
+                        time.perf_counter() >= (time_since_last + self.MAX_TIMEOUT)
                     ):
                         self._write_logs(logs)
                         break
         LOG.debug("%s: stopping processor thread", __name__)
 
     def _write_logs(self, logs: List[Any]) -> None:
         try:
             self.session.bulk_save_objects(logs)
             self.session.commit()
-        except (SQLAlchemyError):
+        except SQLAlchemyError:
             try:
                 self.create_db()
                 self.session.rollback()
                 self.session.bulk_save_objects(logs)
                 self.session.commit()
             except Exception as e:  # pylint: disable=broad-except
                 # if we really cannot commit the log to DB, do not lock the
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/stats_pyramid/__init__.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/stats_pyramid/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 """Generate statsd metrics for pyramid and SQLAlchemy events."""
+
 import warnings
 
 import pyramid.config
 import pyramid.request
 
-from c2cwsgiutils import stats
+from c2cwsgiutils.stats_pyramid import _pyramid_spy
 
 
 def init(config: pyramid.config.Configurator) -> None:
     """Initialize the whole stats module, for backward compatibility."""
+
     warnings.warn("init function is deprecated; use includeme instead")
     includeme(config)
 
 
 def includeme(config: pyramid.config.Configurator) -> None:
     """
-    Initialize the whole stats module.
+    Initialize the whole stats pyramid module.
 
     Arguments:
 
         config: The Pyramid config
     """
-    stats.init_backends(config.get_settings())
-    if stats.BACKENDS:  # pragma: nocover
-        if "memory" in stats.BACKENDS:  # pragma: nocover
-            from . import _views
 
-            _views.init(config)
-        from . import _pyramid_spy
-
-        _pyramid_spy.init(config)
-        init_db_spy()
+    _pyramid_spy.init(config)
+    init_db_spy()
 
 
 def init_db_spy() -> None:
     """Initialize the database spy."""
+
     from . import _db_spy
 
     _db_spy.init()
```

### Comparing `c2cwsgiutils-5.2.2/c2cwsgiutils/stats_pyramid/_db_spy.py` & `c2cwsgiutils-6.0.0.dev88/c2cwsgiutils/stats_pyramid/_db_spy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 import logging
 import re
-from typing import Any, Callable, Dict, Optional
+import time
+from typing import Any, Callable
 
+import prometheus_client
 import sqlalchemy.event
 from sqlalchemy.engine import Connection, Engine
 from sqlalchemy.orm import Session
 
-from c2cwsgiutils import stats
+from c2cwsgiutils import prometheus
 
 LOG = logging.getLogger(__name__)
 
+_PROMETHEUS_DB_SUMMARY = prometheus_client.Summary(
+    prometheus.build_metric_name("database"),
+    "Database requests",
+    ["what"],
+    unit="seconds",
+)
+
 
 def _jump_string(content: str, pos: int) -> int:
     quote_char = content[pos]
     pos += 1
     while pos < len(content):
         cur = content[pos]
         if cur == quote_char:
@@ -54,25 +63,19 @@
         before = sql[0 : in_.start()]
         after = _eat_parenthesis(sql[in_.end() - 1 :])
         sql = before + " IN (?)" + after
     return re.sub(r"%\(\w+\)\w", "?", sql)
 
 
 def _create_sqlalchemy_timer_cb(what: str) -> Callable[..., Any]:
-    if stats.USE_TAGS and what != "commit":
-        key = ["sql"]
-        tags: Optional[Dict[str, str]] = {"query": what}
-    else:
-        key = ["sql", what]
-        tags = None
-    measure = stats.timer(key, tags)
+    start = time.perf_counter()
 
     def after(*_args: Any, **_kwargs: Any) -> None:
-        duration = measure.stop()
-        LOG.debug("Execute statement '%s' in %d.", what, duration)
+        _PROMETHEUS_DB_SUMMARY.labels({"query": what}).observe(time.perf_counter() - start)
+        LOG.debug("Execute statement '%s' in %d.", what, time.perf_counter() - start)
 
     return after
 
 
 def _before_cursor_execute(
     conn: Connection, _cursor: Any, statement: str, _parameters: Any, _context: Any, _executemany: Any
 ) -> None:
```

### Comparing `c2cwsgiutils-5.2.2/pyproject.toml` & `c2cwsgiutils-6.0.0.dev88/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 [tool.black]
 line-length = 110
 target-version = ['py310']
 
 [tool.isort]
-known_third_party = "pyramid2"
-known_first_party = "c2cwsgiutils"
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = false
-use_parentheses = true
+profile = "black"
 line_length = 110
 
 [tool.mypy]
 python_version = 3.10
 ignore_missing_imports = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 strict = true
 
 [tool.poetry]
 name = "c2cwsgiutils"
-version = "5.2.2"
+version = "6.0.0.dev88"
 description = "Common utilities for Camptocamp WSGI applications"
 readme = "README.md"
 authors = ["Camptocamp <info@camptocamp.com>"]
 keywords = ["geo", "gis", "sqlalchemy", "orm", "wsgi"]
 repository = "https://github.com/camptocamp/c2cwsgiutils"
 license = "BSD-2-Clause"
 classifiers = [
@@ -64,39 +59,40 @@
 
 [tool.poetry.plugins."paste.filter_factory"]
 client_info = "c2cwsgiutils.client_info:filter_factory"
 sentry = "c2cwsgiutils.sentry:filter_factory"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-requests = { version = "2.28.2" }
+requests = { version = "2.31.0" }
 pyyaml = { version = "6.0" }
-alembic = { version = "1.9.4", optional = true }
-boltons = { version = "21.0.0", optional = true }
+alembic = { version = "1.11.1", optional = true }
+boltons = { version = "23.0.0", optional = true }
 cornice = { version = "6.0.1", optional = true }
-redis = { version = "4.4.2", optional = true }
+redis = { version = "4.5.4", optional = true }
 gunicorn = { version = "20.1.0", optional = true }
 lxml = { version = "4.9.2", optional = true }
 netifaces = { version = "0.11.0", optional = true }
 objgraph = { version = "3.5.0", optional = true }
-psycopg2 = { version = "2.9.5", optional = true }
+psycopg2 = { version = "2.9.6", optional = true }
 pyramid = { version = "2.0.1", optional = true }
 pyramid-tm = { version = "2.5", optional = true }
-sentry-sdk = { version = "1.14.0", optional = true }
+sentry-sdk = { version = "1.24.0", optional = true }
 ujson = { version = "5.7.0", optional = true }
 cee_syslog_handler = { version = "0.6.0", optional = true }
-SQLAlchemy = { version = "2.0.4", optional = true }
-SQLAlchemy-Utils = { version = "0.39.0", optional = true }
-"zope.interface" = { version = "5.5.2", optional = true }
-"zope.sqlalchemy" = { version = "1.6", optional = true }
-pyjwt = { version = "2.6.0", optional = true }
+SQLAlchemy = { version = "2.0.15", optional = true }
+SQLAlchemy-Utils = { version = "0.41.1", optional = true }
+"zope.interface" = { version = "6.0", optional = true }
+"zope.sqlalchemy" = { version = "3.0", optional = true }
+pyjwt = { version = "2.7.0", optional = true }
 requests-oauthlib = { version = "1.3.1", optional = true }
 waitress = { version = "2.1.2", optional = true }
-scikit-image = { version = "0.19.3", optional = true }
-certifi = "2022.12.7"
+scikit-image = { version = "0.20.0", optional = true }
+certifi = "2023.5.7"
+prometheus-client = "0.16.0"
 
 [tool.poetry.extras]
 standard = [
   "alembic",
   "boltons",
   "cornice",
   "redis",
@@ -142,26 +138,26 @@
   "waitress",
   "redis"
 ]
 test_images = ["scikit-image"]
 
 [tool.poetry.dev-dependencies]
 # pylint = { version = "2.15.6" }
-prospector = { extras = ["with_bandit", "with_mypy", "with_pyroma"], version = "1.8.4" }
-coverage = "7.1.0"
+prospector = { extras = ["with_bandit", "with_mypy", "with_pyroma"], version = "1.10.2" }
+coverage = "7.2.7"
 junit2html = "30.1.3"
-pytest = "7.2.1"
-pytest-cov = "4.0.0"
+pytest = "7.3.1"
+pytest-cov = "4.1.0"
 pytest-html = "3.2.0"
-types-pyyaml = "6.0.12.8"
-types-requests = "2.28.11.15"
-types-redis = "4.4.0.6"
-types-ujson = "5.7.0.1"
-types-python-dateutil = "2.8.19.10"
-typing_extensions = "4.4.0"
+types-pyyaml = "6.0.12.10"
+types-requests = "2.31.0.1"
+types-redis = "4.5.4.1"
+types-ujson = "5.7.0.5"
+types-python-dateutil = "2.8.19.13"
+typing_extensions = "4.6.3"
 
 [build-system]
 requires = [
   "poetry-core>=1.0.0",
   "poetry-dynamic-versioning[plugin]",
   "poetry-plugin-tweak-dependencies-version"
 ]
@@ -169,15 +165,15 @@
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 pattern = "^(?P<base>\\d+(\\.\\d+)*)"
 format-jinja = """
 {%- if env.get("VERSION_TYPE") == "version_branch" -%}
-{{serialize_pep440(bump_version(base, 1 if env.get("IS_MASTER") == "TRUE" else 2), dev=distance)}}
+{{serialize_pep440(bump_version(base, 0 if env.get("IS_MASTER") == "TRUE" else 2), dev=distance)}}
 {%- elif distance == 0 -%}
 {{serialize_pep440(base)}}
 {%- else -%}
 {{serialize_pep440(bump_version(base), dev=distance)}}
 {%- endif -%}
 """
```

### Comparing `c2cwsgiutils-5.2.2/PKG-INFO` & `c2cwsgiutils-6.0.0.dev88/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c2cwsgiutils
-Version: 5.2.2
+Version: 6.0.0.dev88
 Summary: Common utilities for Camptocamp WSGI applications
 Home-page: https://github.com/camptocamp/c2cwsgiutils
 License: BSD-2-Clause
 Keywords: geo,gis,sqlalchemy,orm,wsgi
 Author: Camptocamp
 Author-email: info@camptocamp.com
 Requires-Python: >=3.8,<4.0
@@ -17,16 +17,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Typing :: Typed
 Provides-Extra: all
 Provides-Extra: broadcast
 Provides-Extra: dev
 Provides-Extra: oauth2
 Provides-Extra: standard
@@ -38,14 +36,15 @@
 Requires-Dist: cee_syslog_handler ; extra == "standard" or extra == "all"
 Requires-Dist: certifi
 Requires-Dist: cornice ; extra == "standard" or extra == "all"
 Requires-Dist: gunicorn ; extra == "standard" or extra == "all"
 Requires-Dist: lxml ; extra == "standard" or extra == "all"
 Requires-Dist: netifaces ; extra == "standard" or extra == "all"
 Requires-Dist: objgraph ; extra == "standard" or extra == "all"
+Requires-Dist: prometheus-client
 Requires-Dist: psycopg2 ; extra == "standard" or extra == "all"
 Requires-Dist: pyjwt ; extra == "oauth2" or extra == "all"
 Requires-Dist: pyramid ; extra == "standard" or extra == "all"
 Requires-Dist: pyramid-tm ; extra == "standard" or extra == "all"
 Requires-Dist: pyyaml
 Requires-Dist: redis ; extra == "standard" or extra == "broadcast" or extra == "all" or extra == "all"
 Requires-Dist: requests
@@ -60,16 +59,15 @@
 Description-Content-Type: text/markdown
 
 # Camptocamp WSGI utilities
 
 This is a Python 3 library (>=3.5) providing common tools for Camptocamp WSGI
 applications:
 
-- Provide a small framework for gathering performance statistics about
-  a web application (statsd protocol)
+- Provide prometheus metrics
 - Allow to use a master/slave PostgresQL configuration
 - Logging handler for CEE/UDP logs
   - An optional view to change runtime the log levels
 - SQL profiler to debug DB performance problems, disabled by default. Warning, it will slow down everything.
 - A view to get the version information about the application and the installed packages
 - A framework for implementing a health_check service
 - Error handlers to send JSON messages to the client in case of error
@@ -100,36 +98,36 @@
 - [gunicorn.conf.py](acceptance_tests/app/gunicorn.conf.py).
   Then replace `c2cwsgiutils_app` by your package name.
 
 You should install `c2cwsgiutils` with the tool you use to manage your pip dependencies.
 
 In the `Dockerfile` you should add the following lines:
 
-```
+```dockerfile
 # Generate the version file.
 RUN c2cwsgiutils-genversion $(git rev-parse HEAD)
 
 CMD ["gunicorn", "--paste=/app/production.ini"]
 
 # Default values for the environment variables
 ENV \
-    DEVELOPMENT=0 \
-    SQLALCHEMY_POOL_RECYCLE=30 \
-    SQLALCHEMY_POOL_SIZE=5 \
-    SQLALCHEMY_MAX_OVERFLOW=25 \
-    SQLALCHEMY_SLAVE_POOL_RECYCLE=30 \
-    SQLALCHEMY_SLAVE_POOL_SIZE=5 \
-    SQLALCHEMY_SLAVE_MAX_OVERFLOW=25\
-    LOG_TYPE=console \
-    OTHER_LOG_LEVEL=WARNING \
-    GUNICORN_LOG_LEVEL=WARNING \
-    GUNICORN_ACCESS_LOG_LEVEL=INFO \
-    SQL_LOG_LEVEL=WARNING \
-    C2CWSGIUTILS_LOG_LEVEL=WARNING \
-    LOG_LEVEL=INFO
+  DEVELOPMENT=0 \
+  SQLALCHEMY_POOL_RECYCLE=30 \
+  SQLALCHEMY_POOL_SIZE=5 \
+  SQLALCHEMY_MAX_OVERFLOW=25 \
+  SQLALCHEMY_SLAVE_POOL_RECYCLE=30 \
+  SQLALCHEMY_SLAVE_POOL_SIZE=5 \
+  SQLALCHEMY_SLAVE_MAX_OVERFLOW=25\
+  LOG_TYPE=console \
+  OTHER_LOG_LEVEL=WARNING \
+  GUNICORN_LOG_LEVEL=WARNING \
+  GUNICORN_ACCESS_LOG_LEVEL=INFO \
+  SQL_LOG_LEVEL=WARNING \
+  C2CWSGIUTILS_LOG_LEVEL=WARNING \
+  LOG_LEVEL=INFO
 ```
 
 Add in your `main` function.
 
 ```python
 config.include("c2cwsgiutils.pyramid")
 dbsession = c2cwsgiutils.db.init(config, "sqlalchemy", "sqlalchemy_slave")
@@ -327,55 +325,14 @@
 `c2c_request_id` attribute on the Pyramid Request objects. The `requests` module is patched to automatically
 add this header.
 
 The requests module is also patched to monitor requests done without timeout. In that case, you can
 configure a default timeout with the `C2C_REQUESTS_DEFAULT_TIMEOUT` environment variable
 (`c2c.requests_default_timeout`). If no timeout and no default is specified, a warning is issued.
 
-## Metrics
-
-To enable and configure the metrics framework, you can use:
-
-- STATS_VIEW (c2c.stats_view): if defined, will enable the stats view `{C2C_BASE_PATH}/stats.json`
-- STATSD_ADDRESS (c2c.statsd_address): if defined, send stats to the given statsd server
-- STATSD_PREFIX (c2c.statsd_prefix): prefix to add to every metric names
-- STATSD_USE_TAGS: If true, automatic metrics will use tags
-- STATSD*TAG*{tag_name}: To set a global tag for the service
-
-If enabled, some metrics are automatically generated:
-
-- {STATSD_PREFIX}.route.{verb}.{route_name}.{status}: The time to process a query (includes rendering)
-- {STATSD_PREFIX}.render.{verb}.{route_name}.{status}: The time to render a query
-- {STATSD_PREFIX}.sql.{query}: The time to execute the given SQL query (simplified and normalized)
-- {STATSD_PREFIX}.requests.{scheme}.{hostname}.{port}.{verb}.{status}: The time to execute HTTP requests to
-  outside services (only the time between the start of sending of the request and when the header is
-  back with a chunk of the body)
-- {STATSD_PREFIX}.redis.{command}: The time to execute the given Redis command
-
-You can manually measure the time spent on something like that:
-
-```python
-from c2cwsgiutils import stats
-with stats.timer_context(['toto', 'tutu']):
-    do_something()
-```
-
-It will only add a timer event in case of success. If you want to measure both success and failures, do that:
-
-```python
-from c2cwsgiutils import stats
-with stats.outcome_timer_context(['toto', 'tutu']):
-    do_something()
-```
-
-Other functions exists to generate metrics. Look at the `c2cwsgiutils.stats` module.
-
-Look at the `c2cwsgiutils-stats-db` utility if you want to generate statistics (gauges) about the
-row counts.
-
 ## SQL profiler
 
 The SQL profiler must be configured with the `C2C_SQL_PROFILER_ENABLED` environment variable. That enables a view
 to query the status of the profiler (`{C2C_BASE_PATH}/sql_profiler?secret={C2C_SECRET}`) or to
 enable/disable it (`{C2C_BASE_PATH}/sql_profiler?secret={C2C_SECRET}&enable={1|0}`).
 
 If enabled, for each `SELECT` query sent by SQLAlchemy, another query it done with `EXPLAIN ANALYZE`
@@ -515,35 +472,108 @@
 
 ## Version information
 
 If the `/app/versions.json` exists, a view is added (`{C2C_BASE_PATH}/versions.json`) to query the current
 version of a app. This file is generated by calling the `c2cwsgiutils-genversion [$GIT_TAG] $GIT_HASH`
 command line. Usually done in the [Dockerfile](acceptance_tests/app/Dockerfile) of the WSGI application.
 
-## Metrics
+## Prometheus
+
+[Prometheus client](https://github.com/prometheus/client_python) is integrated in c2cwsgiutils.
+
+It will work in multi process mode with the limitation listed in the
+[`prometheus_client` documentation](https://github.com/prometheus/client_python#multiprocess-mode-eg-gunicorn).
+
+To enable it you should provide the `PROMETHEUS_PORT` environment variable.
+For security reason, this port should not be exposed.
+
+We can customize it with the following environment variables:
+
+- `PROMETHEUS_PREFIX`: to customize the prefix, default is `c2cwsggiutils-`.
+- `C2C_PROMETHEUS_PACKAGES` the packages that will be present in the version information, default is `c2cwsgiutils,pyramid,gunicorn,sqlalchemy`.
+- `C2C_PROMETHEUS_APPLICATION_PACKAGES` the packages that will be present in the version information as application.
+
+And you should add in your `gunicorn.conf.py`:
+
+```python
+from prometheus_client import multiprocess
+
+
+def on_starting(server):
+    from c2cwsgiutils import prometheus
+
+    del server
+
+    prometheus.start()
+
 
-The path `/metrics` provide some metrics for Prometheus.
-By default we have the `smap` `pss`, but we can easily add the `rss`, `size` or your custom settings:
+def post_fork(server, worker):
+    from c2cwsgiutils import prometheus
 
-Example:
+    del server, worker
 
+    prometheus.cleanup()
+
+
+def child_exit(server, worker):
+    del server
+
+    multiprocess.mark_process_dead(worker.pid)
+```
+
+In your `Dockerfile` you should add:
+
+```dockerfile
+RUN mkdir -p /prometheus-metrics \
+    chmod a+rwx /prometheus-metrics
+ENV PROMETHEUS_MULTIPROC_DIR=/prometheus-metrics
+```
+
+### Add custom metric collector
+
+See [official documentation](https://github.com/prometheus/client_python#custom-collectors).
+
+Related to the Unix process.
+
+```python
+from c2cwsgiutils import broadcast, prometheus
+
+prometheus.MULTI_PROCESS_COLLECTOR_BROADCAST_CHANNELS.append("prometheus_collector_custom")
+broadcast.subscribe("c2cwsgiutils_prometheus_collect_gc", _broadcast_collector_custom)
+my_custom_collector_instance = MyCustomCollector()
+
+
+def _broadcast_collector_custom() -> List[prometheus.SerializedGauge]:
+    """Get the collected GC gauges."""
+
+    return prometheus.serialize_collected_data(my_custom_collector_instance)
 ```
-from import c2cwsgiutils.metrics import add_provider, Provider, MemoryMapProvider
 
-class CustomProvider(Provider):
-    def __init__(self):
-        super().__init__("my_metrics", "My Metric")
+Related to the host, use that in the `gunicorn.conf.py`:
 
-    def get_data(self):
-        return [({'metadata_key': 'matadata_value'}, metrics_value)]
+```python
+def on_starting(server):
+    from c2cwsgiutils import prometheus
+
+    del server
 
-add_provider(MemoryMapProvider('rss'))
-add_provider(CustomProvider())
+    registry = CollectorRegistry()
+    registry.register(MyCollector())
+    prometheus.start(registry)
 ```
 
+### Database metrics
+
+Look at the `c2cwsgiutils-stats-db` utility if you want to generate statistics (gauges) about the
+row counts.
+
+### Usage of metrics
+
+With c2cwsgiutils each instance (Pod) has its own metrics, so we need to aggregate them to have the metrics for the service you probably need to use `sum by (<fields>) (<metric>)` to get the metric (especially for counters).
+
 ## Custom scripts
 
 To have the application initialized in a script you should use the
 `c2cwsgiutils.setup_process.bootstrap_application_from_options` function.
 
 Example of `main` function:
 
@@ -588,15 +618,15 @@
 To enable the debugging interface, you must set the `C2C_DEBUG_VIEW_ENABLED` environment variable. Then you can
 have dumps of a few things:
 
 - every threads' stacktrace: `{C2C_BASE_PATH}/debug/stacks?secret={C2C_SECRET}`
 - memory usage: `{C2C_BASE_PATH}/debug/memory?secret={C2C_SECRET}&limit=30&analyze_type=builtins.dict&python_internals_map=false`
 - object ref: `{C2C_BASE_PATH}/debug/show_refs.dot?secret={C2C_SECRET}&analyze_type=gunicorn.app.wsgiapp.WSGIApplication&analyze_id=12345&max_depth=3&too_many=10&filter=1024&no_extra_info&backrefs`
   `analyze_type` and `analyze_id` should not ve used toogether, you can use it like:
-  ```
+  ```bash
   curl "<URL>" > /tmp/show_refs.dot
   dot -Lg -Tpng /tmp/show_refs.dot > /tmp/show_refs.png
   ```
 - memory increase when calling another API: `{C2C_BASE_PATH}/debug/memory_diff?path={path_info}&secret={C2C_SECRET}&limit=30&no_warmup`
 - sleep the given number of seconds (to test load balancer timeouts): `{C2C_BASE_PATH}/debug/sleep?secret={C2C_SECRET}&time=60.2`
 - see the HTTP headers received by WSGI: `{C2C_BASE_PATH}/debug/headers?secret={C2C_SECRET}&status=500`
 - return an HTTP error: `{C2C_BASE_PATH}/debug/error?secret={C2C_SECRET}&status=500`
@@ -649,15 +679,15 @@
 You can enable this by setting `C2C_ENABLE_EXCEPTION_HANDLING` (`c2c.enable_exception_handling`) to "1".
 
 In development mode (`DEVELOPMENT=1`), all the details (SQL statement, stacktrace, ...) are sent to the
 client. In production mode, you can still get them by sending the secret defined in `C2C_SECRET` in the query.
 
 If you want to use pyramid_debugtoolbar, you need to disable exception handling and configure it like that:
 
-```
+```ini
 pyramid.includes =
     pyramid_debugtoolbar
 debugtoolbar.enabled = true
 debugtoolbar.hosts = 0.0.0.0/0
 debugtoolbar.intercept_exc = debug
 debugtoolbar.show_on_exc_only = true
 c2c.enable_exception_handling = 0
@@ -723,7 +753,16 @@
 
 - Change the the version in [setup.py](setup.py).
 - Commit and push to master.
 - Tag the GIT commit.
 - Add the new branch name in the `.github/workflows/rebuild.yaml` and
   `.github/workflows/audit.yaml` files.
 
+## Contributing
+
+Install the pre-commit hooks:
+
+```bash
+pip install pre-commit
+pre-commit install --allow-missing-config
+```
+
```

