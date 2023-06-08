# Comparing `tmp/SATOSA-8.2.0.tar.gz` & `tmp/SATOSA-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SATOSA-8.2.0.tar", last modified: Thu Nov 17 18:09:22 2022, max compression
+gzip compressed data, was "SATOSA-8.3.0.tar", last modified: Thu Jun  8 17:00:28 2023, max compression
```

## Comparing `SATOSA-8.2.0.tar` & `SATOSA-8.3.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2022-11-17 18:09:22.226084 SATOSA-8.2.0/
--rw-r--r--   0 ivan       (501) staff       (20)    10177 2021-05-24 16:59:06.000000 SATOSA-8.2.0/LICENSE
--rw-r--r--   0 ivan       (501) staff       (20)     1313 2021-05-24 16:59:06.000000 SATOSA-8.2.0/NOTICE
--rw-r--r--   0 ivan       (501) staff       (20)      527 2022-11-17 18:09:22.226160 SATOSA-8.2.0/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)     3666 2022-11-15 12:05:51.000000 SATOSA-8.2.0/README.md
--rw-r--r--   0 ivan       (501) staff       (20)      433 2022-11-17 18:09:22.226437 SATOSA-8.2.0/setup.cfg
--rw-r--r--   0 ivan       (501) staff       (20)     1133 2022-11-17 18:04:03.000000 SATOSA-8.2.0/setup.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2022-11-17 18:09:22.209232 SATOSA-8.2.0/src/
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2022-11-17 18:09:22.211659 SATOSA-8.2.0/src/SATOSA.egg-info/
--rw-r--r--   0 ivan       (501) staff       (20)      527 2022-11-17 18:09:22.000000 SATOSA-8.2.0/src/SATOSA.egg-info/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)     2597 2022-11-17 18:09:22.000000 SATOSA-8.2.0/src/SATOSA.egg-info/SOURCES.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2022-11-17 18:09:22.000000 SATOSA-8.2.0/src/SATOSA.egg-info/dependency_links.txt
--rw-r--r--   0 ivan       (501) staff       (20)      101 2022-11-17 18:09:22.000000 SATOSA-8.2.0/src/SATOSA.egg-info/entry_points.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2021-05-24 17:00:24.000000 SATOSA-8.2.0/src/SATOSA.egg-info/not-zip-safe
--rw-r--r--   0 ivan       (501) staff       (20)      180 2022-11-17 18:09:22.000000 SATOSA-8.2.0/src/SATOSA.egg-info/requires.txt
--rw-r--r--   0 ivan       (501) staff       (20)        7 2022-11-17 18:09:22.000000 SATOSA-8.2.0/src/SATOSA.egg-info/top_level.txt
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2022-11-17 18:09:22.215458 SATOSA-8.2.0/src/satosa/
--rw-r--r--   0 ivan       (501) staff       (20)      139 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     9928 2021-06-29 12:33:38.000000 SATOSA-8.2.0/src/satosa/attribute_mapping.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2022-11-17 18:09:22.217482 SATOSA-8.2.0/src/satosa/backends/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/backends/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)    12829 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/backends/apple.py
--rw-r--r--   0 ivan       (501) staff       (20)     2616 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/backends/base.py
--rw-r--r--   0 ivan       (501) staff       (20)     3385 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/backends/bitbucket.py
--rw-r--r--   0 ivan       (501) staff       (20)     4519 2022-04-18 11:24:27.000000 SATOSA-8.2.0/src/satosa/backends/github.py
--rw-r--r--   0 ivan       (501) staff       (20)     4749 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/backends/linkedin.py
--rw-r--r--   0 ivan       (501) staff       (20)    14092 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/backends/oauth.py
--rw-r--r--   0 ivan       (501) staff       (20)    12055 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/backends/openid_connect.py
--rw-r--r--   0 ivan       (501) staff       (20)     4222 2022-11-15 11:31:39.000000 SATOSA-8.2.0/src/satosa/backends/orcid.py
--rw-r--r--   0 ivan       (501) staff       (20)     2895 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/backends/reflector.py
--rw-r--r--   0 ivan       (501) staff       (20)    26768 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/backends/saml2.py
--rw-r--r--   0 ivan       (501) staff       (20)    10977 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/base.py
--rw-r--r--   0 ivan       (501) staff       (20)     2674 2022-04-18 11:24:27.000000 SATOSA-8.2.0/src/satosa/context.py
--rw-r--r--   0 ivan       (501) staff       (20)      138 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/cookies.py
--rw-r--r--   0 ivan       (501) staff       (20)     1283 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/exception.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2022-11-17 18:09:22.218432 SATOSA-8.2.0/src/satosa/frontends/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/frontends/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     3091 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/frontends/base.py
--rw-r--r--   0 ivan       (501) staff       (20)    22308 2022-11-15 11:31:39.000000 SATOSA-8.2.0/src/satosa/frontends/openid_connect.py
--rw-r--r--   0 ivan       (501) staff       (20)     1916 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/frontends/ping.py
--rw-r--r--   0 ivan       (501) staff       (20)    48306 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/frontends/saml2.py
--rw-r--r--   0 ivan       (501) staff       (20)     4478 2022-04-18 11:24:27.000000 SATOSA-8.2.0/src/satosa/internal.py
--rw-r--r--   0 ivan       (501) staff       (20)      756 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/logging_util.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2022-11-17 18:09:22.218997 SATOSA-8.2.0/src/satosa/metadata_creation/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/metadata_creation/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     6949 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/metadata_creation/description.py
--rw-r--r--   0 ivan       (501) staff       (20)     6718 2022-04-18 11:24:27.000000 SATOSA-8.2.0/src/satosa/metadata_creation/saml_metadata.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2022-11-17 18:09:22.223963 SATOSA-8.2.0/src/satosa/micro_services/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/micro_services/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     6542 2021-08-08 14:35:57.000000 SATOSA-8.2.0/src/satosa/micro_services/account_linking.py
--rw-r--r--   0 ivan       (501) staff       (20)     3811 2022-11-16 15:32:44.000000 SATOSA-8.2.0/src/satosa/micro_services/attribute_authorization.py
--rw-r--r--   0 ivan       (501) staff       (20)     4915 2022-11-15 11:31:39.000000 SATOSA-8.2.0/src/satosa/micro_services/attribute_generation.py
--rw-r--r--   0 ivan       (501) staff       (20)     2265 2022-05-31 11:28:59.000000 SATOSA-8.2.0/src/satosa/micro_services/attribute_modifications.py
--rw-r--r--   0 ivan       (501) staff       (20)     1091 2021-06-29 12:33:38.000000 SATOSA-8.2.0/src/satosa/micro_services/attribute_policy.py
--rw-r--r--   0 ivan       (501) staff       (20)     2312 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/micro_services/attribute_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)     1720 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/micro_services/base.py
--rw-r--r--   0 ivan       (501) staff       (20)     9180 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/micro_services/consent.py
--rw-r--r--   0 ivan       (501) staff       (20)     4352 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/micro_services/custom_logging.py
--rw-r--r--   0 ivan       (501) staff       (20)     5560 2022-04-18 11:24:27.000000 SATOSA-8.2.0/src/satosa/micro_services/custom_routing.py
--rw-r--r--   0 ivan       (501) staff       (20)     2245 2022-04-18 11:24:27.000000 SATOSA-8.2.0/src/satosa/micro_services/disco.py
--rw-r--r--   0 ivan       (501) staff       (20)     3497 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/micro_services/hasher.py
--rw-r--r--   0 ivan       (501) staff       (20)     1773 2022-04-18 11:24:27.000000 SATOSA-8.2.0/src/satosa/micro_services/idp_hinting.py
--rw-r--r--   0 ivan       (501) staff       (20)    24072 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/micro_services/ldap_attribute_store.py
--rw-r--r--   0 ivan       (501) staff       (20)    13493 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/micro_services/primary_identifier.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2022-11-17 18:09:22.225545 SATOSA-8.2.0/src/satosa/micro_services/processors/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/micro_services/processors/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)      133 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/micro_services/processors/base_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)      654 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/micro_services/processors/gender_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)     1103 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/micro_services/processors/hash_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)     1891 2021-10-24 15:05:53.000000 SATOSA-8.2.0/src/satosa/micro_services/processors/regex_sub_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)     1695 2021-06-29 12:33:38.000000 SATOSA-8.2.0/src/satosa/micro_services/processors/scope_extractor_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)      678 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/micro_services/processors/scope_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)      686 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/micro_services/processors/scope_remover_processor.py
--rw-r--r--   0 ivan       (501) staff       (20)    10452 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/plugin_loader.py
--rw-r--r--   0 ivan       (501) staff       (20)     6486 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/proxy_server.py
--rw-r--r--   0 ivan       (501) staff       (20)     3148 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/response.py
--rw-r--r--   0 ivan       (501) staff       (20)     6934 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/routing.py
--rw-r--r--   0 ivan       (501) staff       (20)      489 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/saml_util.py
--rw-r--r--   0 ivan       (501) staff       (20)     5075 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/satosa_config.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2022-11-17 18:09:22.225917 SATOSA-8.2.0/src/satosa/scripts/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/scripts/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     3277 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/scripts/satosa_saml_metadata.py
--rw-r--r--   0 ivan       (501) staff       (20)     7954 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/state.py
--rw-r--r--   0 ivan       (501) staff       (20)     2538 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/util.py
--rw-r--r--   0 ivan       (501) staff       (20)      250 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/version.py
--rw-r--r--   0 ivan       (501) staff       (20)     1062 2021-05-24 16:59:06.000000 SATOSA-8.2.0/src/satosa/wsgi.py
--rw-r--r--   0 ivan       (501) staff       (20)     1547 2022-11-15 12:05:51.000000 SATOSA-8.2.0/src/satosa/yaml.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.663773 SATOSA-8.3.0/
+-rw-r--r--   0 ivan       (501) staff       (20)    10177 2021-05-24 16:59:06.000000 SATOSA-8.3.0/LICENSE
+-rw-r--r--   0 ivan       (501) staff       (20)     1313 2021-05-24 16:59:06.000000 SATOSA-8.3.0/NOTICE
+-rw-r--r--   0 ivan       (501) staff       (20)      527 2023-06-08 17:00:28.663859 SATOSA-8.3.0/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)     3666 2022-11-15 12:05:51.000000 SATOSA-8.3.0/README.md
+-rw-r--r--   0 ivan       (501) staff       (20)      433 2023-06-08 17:00:28.664256 SATOSA-8.3.0/setup.cfg
+-rw-r--r--   0 ivan       (501) staff       (20)     1133 2023-06-08 16:56:21.000000 SATOSA-8.3.0/setup.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.647627 SATOSA-8.3.0/src/
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.650202 SATOSA-8.3.0/src/SATOSA.egg-info/
+-rw-r--r--   0 ivan       (501) staff       (20)      527 2023-06-08 17:00:28.000000 SATOSA-8.3.0/src/SATOSA.egg-info/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)     2597 2023-06-08 17:00:28.000000 SATOSA-8.3.0/src/SATOSA.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2023-06-08 17:00:28.000000 SATOSA-8.3.0/src/SATOSA.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan       (501) staff       (20)      101 2023-06-08 17:00:28.000000 SATOSA-8.3.0/src/SATOSA.egg-info/entry_points.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2021-05-24 17:00:24.000000 SATOSA-8.3.0/src/SATOSA.egg-info/not-zip-safe
+-rw-r--r--   0 ivan       (501) staff       (20)      180 2023-06-08 17:00:28.000000 SATOSA-8.3.0/src/SATOSA.egg-info/requires.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        7 2023-06-08 17:00:28.000000 SATOSA-8.3.0/src/SATOSA.egg-info/top_level.txt
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.654048 SATOSA-8.3.0/src/satosa/
+-rw-r--r--   0 ivan       (501) staff       (20)      139 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     9928 2021-06-29 12:33:38.000000 SATOSA-8.3.0/src/satosa/attribute_mapping.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.656088 SATOSA-8.3.0/src/satosa/backends/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/backends/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)    12829 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/backends/apple.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2616 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/backends/base.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3385 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/backends/bitbucket.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4519 2022-04-18 11:24:27.000000 SATOSA-8.3.0/src/satosa/backends/github.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4749 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/backends/linkedin.py
+-rw-r--r--   0 ivan       (501) staff       (20)    14092 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/backends/oauth.py
+-rw-r--r--   0 ivan       (501) staff       (20)    12243 2023-06-08 16:54:50.000000 SATOSA-8.3.0/src/satosa/backends/openid_connect.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4222 2022-11-15 11:31:39.000000 SATOSA-8.3.0/src/satosa/backends/orcid.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2895 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/backends/reflector.py
+-rw-r--r--   0 ivan       (501) staff       (20)    26768 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/backends/saml2.py
+-rw-r--r--   0 ivan       (501) staff       (20)    10977 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/base.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2674 2022-04-18 11:24:27.000000 SATOSA-8.3.0/src/satosa/context.py
+-rw-r--r--   0 ivan       (501) staff       (20)      138 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/cookies.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1283 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/exception.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.657190 SATOSA-8.3.0/src/satosa/frontends/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/frontends/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3091 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/frontends/base.py
+-rw-r--r--   0 ivan       (501) staff       (20)    22308 2022-11-15 11:31:39.000000 SATOSA-8.3.0/src/satosa/frontends/openid_connect.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1961 2022-11-29 13:48:33.000000 SATOSA-8.3.0/src/satosa/frontends/ping.py
+-rw-r--r--   0 ivan       (501) staff       (20)    48292 2023-06-08 16:54:50.000000 SATOSA-8.3.0/src/satosa/frontends/saml2.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4478 2022-04-18 11:24:27.000000 SATOSA-8.3.0/src/satosa/internal.py
+-rw-r--r--   0 ivan       (501) staff       (20)      756 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/logging_util.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.658000 SATOSA-8.3.0/src/satosa/metadata_creation/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/metadata_creation/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     6949 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/metadata_creation/description.py
+-rw-r--r--   0 ivan       (501) staff       (20)     6718 2022-04-18 11:24:27.000000 SATOSA-8.3.0/src/satosa/metadata_creation/saml_metadata.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.661726 SATOSA-8.3.0/src/satosa/micro_services/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     6542 2021-08-08 14:35:57.000000 SATOSA-8.3.0/src/satosa/micro_services/account_linking.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3811 2022-11-16 15:32:44.000000 SATOSA-8.3.0/src/satosa/micro_services/attribute_authorization.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4915 2022-11-15 11:31:39.000000 SATOSA-8.3.0/src/satosa/micro_services/attribute_generation.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4296 2023-06-07 16:46:41.000000 SATOSA-8.3.0/src/satosa/micro_services/attribute_modifications.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1091 2021-06-29 12:33:38.000000 SATOSA-8.3.0/src/satosa/micro_services/attribute_policy.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2312 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/micro_services/attribute_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1720 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/base.py
+-rw-r--r--   0 ivan       (501) staff       (20)     9180 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/micro_services/consent.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4352 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/micro_services/custom_logging.py
+-rw-r--r--   0 ivan       (501) staff       (20)     5720 2022-11-29 13:44:11.000000 SATOSA-8.3.0/src/satosa/micro_services/custom_routing.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2245 2022-04-18 11:24:27.000000 SATOSA-8.3.0/src/satosa/micro_services/disco.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3497 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/hasher.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1773 2022-04-18 11:24:27.000000 SATOSA-8.3.0/src/satosa/micro_services/idp_hinting.py
+-rw-r--r--   0 ivan       (501) staff       (20)    24072 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/ldap_attribute_store.py
+-rw-r--r--   0 ivan       (501) staff       (20)    13447 2023-06-08 16:39:00.000000 SATOSA-8.3.0/src/satosa/micro_services/primary_identifier.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.663323 SATOSA-8.3.0/src/satosa/micro_services/processors/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)      133 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/base_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)      654 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/gender_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1103 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/hash_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1891 2021-10-24 15:05:53.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/regex_sub_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1695 2021-06-29 12:33:38.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/scope_extractor_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)      678 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/scope_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)      686 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/micro_services/processors/scope_remover_processor.py
+-rw-r--r--   0 ivan       (501) staff       (20)    10452 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/plugin_loader.py
+-rw-r--r--   0 ivan       (501) staff       (20)     6486 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/proxy_server.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3148 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/response.py
+-rw-r--r--   0 ivan       (501) staff       (20)     6934 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/routing.py
+-rw-r--r--   0 ivan       (501) staff       (20)      489 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/saml_util.py
+-rw-r--r--   0 ivan       (501) staff       (20)     5075 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/satosa_config.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-08 17:00:28.663637 SATOSA-8.3.0/src/satosa/scripts/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/scripts/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3277 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/scripts/satosa_saml_metadata.py
+-rw-r--r--   0 ivan       (501) staff       (20)     7954 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/state.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2538 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/util.py
+-rw-r--r--   0 ivan       (501) staff       (20)      250 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/version.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1062 2021-05-24 16:59:06.000000 SATOSA-8.3.0/src/satosa/wsgi.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1547 2022-11-15 12:05:51.000000 SATOSA-8.3.0/src/satosa/yaml.py
```

### Comparing `SATOSA-8.2.0/LICENSE` & `SATOSA-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/NOTICE` & `SATOSA-8.3.0/NOTICE`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/PKG-INFO` & `SATOSA-8.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SATOSA
-Version: 8.2.0
+Version: 8.3.0
 Summary: Protocol proxy (SAML/OIDC).
 Home-page: https://github.com/SUNET/SATOSA
 Author: DIRG
 Author-email: satosa-dev@lists.sunet.se
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `SATOSA-8.2.0/README.md` & `SATOSA-8.3.0/README.md`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/setup.py` & `SATOSA-8.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 setup.py
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='SATOSA',
-    version='8.2.0',
+    version='8.3.0',
     description='Protocol proxy (SAML/OIDC).',
     author='DIRG',
     author_email='satosa-dev@lists.sunet.se',
     license='Apache 2.0',
     url='https://github.com/SUNET/SATOSA',
     packages=find_packages('src/'),
     package_dir={'': 'src'},
```

### Comparing `SATOSA-8.2.0/src/SATOSA.egg-info/PKG-INFO` & `SATOSA-8.3.0/src/SATOSA.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SATOSA
-Version: 8.2.0
+Version: 8.3.0
 Summary: Protocol proxy (SAML/OIDC).
 Home-page: https://github.com/SUNET/SATOSA
 Author: DIRG
 Author-email: satosa-dev@lists.sunet.se
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `SATOSA-8.2.0/src/SATOSA.egg-info/SOURCES.txt` & `SATOSA-8.3.0/src/SATOSA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/attribute_mapping.py` & `SATOSA-8.3.0/src/satosa/attribute_mapping.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/backends/apple.py` & `SATOSA-8.3.0/src/satosa/backends/apple.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/backends/base.py` & `SATOSA-8.3.0/src/satosa/backends/base.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/backends/bitbucket.py` & `SATOSA-8.3.0/src/satosa/backends/bitbucket.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/backends/github.py` & `SATOSA-8.3.0/src/satosa/backends/github.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/backends/linkedin.py` & `SATOSA-8.3.0/src/satosa/backends/linkedin.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/backends/oauth.py` & `SATOSA-8.3.0/src/satosa/backends/oauth.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/backends/openid_connect.py` & `SATOSA-8.3.0/src/satosa/backends/openid_connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from oic import oic
 from oic import rndstr
 from oic.oic.message import AuthorizationResponse
 from oic.oic.message import ProviderConfigurationResponse
 from oic.oic.message import RegistrationRequest
 from oic.utils.authn.authn_context import UNSPECIFIED
 from oic.utils.authn.client import CLIENT_AUTHN_METHOD
+from oic.utils.settings import PyoidcSettings
 
 import satosa.logging_util as lu
 from satosa.internal import AuthenticationInformation
 from satosa.internal import InternalData
 from .base import BackendModule
 from .oauth import get_metadata_desc_for_oauth_backend
 from ..exception import SATOSAAuthenticationError, SATOSAError
@@ -51,18 +52,20 @@
         :type config: dict[str, dict[str, str] | list[str]]
         :type base_url: str
         :type name: str
         """
         super().__init__(auth_callback_func, internal_attributes, base_url, name)
         self.auth_callback_func = auth_callback_func
         self.config = config
+        cfg_verify_ssl = config["client"].get("verify_ssl", True)
+        oidc_settings = PyoidcSettings(verify_ssl=cfg_verify_ssl)
         self.client = _create_client(
-            config["provider_metadata"],
-            config["client"]["client_metadata"],
-            config["client"].get("verify_ssl", True),
+            provider_metadata=config["provider_metadata"],
+            client_metadata=config["client"]["client_metadata"],
+            settings=oidc_settings,
         )
         if "scope" not in config["client"]["auth_req_params"]:
             config["auth_req_params"]["scope"] = "openid"
         if "response_type" not in config["client"]["auth_req_params"]:
             config["auth_req_params"]["response_type"] = "code"
 
     def start_auth(self, context, request_info):
@@ -239,26 +242,26 @@
         """
         See satosa.backends.oauth.get_metadata_desc
         :rtype: satosa.metadata_creation.description.MetadataDescription
         """
         return get_metadata_desc_for_oauth_backend(self.config["provider_metadata"]["issuer"], self.config)
 
 
-def _create_client(provider_metadata, client_metadata, verify_ssl=True):
+def _create_client(provider_metadata, client_metadata, settings=None):
     """
     Create a pyoidc client instance.
     :param provider_metadata: provider configuration information
     :type provider_metadata: Mapping[str, Union[str, Sequence[str]]]
     :param client_metadata: client metadata
     :type client_metadata: Mapping[str, Union[str, Sequence[str]]]
     :return: client instance to use for communicating with the configured provider
     :rtype: oic.oic.Client
     """
     client = oic.Client(
-        client_authn_method=CLIENT_AUTHN_METHOD, verify_ssl=verify_ssl
+        client_authn_method=CLIENT_AUTHN_METHOD, settings=settings
     )
 
     # Provider configuration information
     if "authorization_endpoint" in provider_metadata:
         # no dynamic discovery necessary
         client.handle_provider_config(ProviderConfigurationResponse(**provider_metadata),
                                       provider_metadata["issuer"])
```

### Comparing `SATOSA-8.2.0/src/satosa/backends/orcid.py` & `SATOSA-8.3.0/src/satosa/backends/orcid.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/backends/reflector.py` & `SATOSA-8.3.0/src/satosa/backends/reflector.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/backends/saml2.py` & `SATOSA-8.3.0/src/satosa/backends/saml2.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/base.py` & `SATOSA-8.3.0/src/satosa/base.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/context.py` & `SATOSA-8.3.0/src/satosa/context.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/exception.py` & `SATOSA-8.3.0/src/satosa/exception.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/frontends/base.py` & `SATOSA-8.3.0/src/satosa/frontends/base.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/frontends/openid_connect.py` & `SATOSA-8.3.0/src/satosa/frontends/openid_connect.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/frontends/ping.py` & `SATOSA-8.3.0/src/satosa/frontends/ping.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import logging
 
 import satosa.logging_util as lu
-import satosa.micro_services.base
+from satosa.frontends.base import FrontendModule
 from satosa.response import Response
 
 
 logger = logging.getLogger(__name__)
 
 
-class PingFrontend(satosa.frontends.base.FrontendModule):
+class PingFrontend(FrontendModule):
     """
     SATOSA frontend that responds to a query with a simple
     200 OK, intended to be used as a simple heartbeat monitor.
     """
 
     def __init__(self, auth_req_callback_func, internal_attributes, config, base_url, name):
         super().__init__(auth_req_callback_func, internal_attributes, base_url, name)
 
         self.config = config
 
-    def handle_authn_response(self, context, internal_resp, extra_id_token_claims=None):
+    def handle_authn_response(self, context, internal_resp):
         """
         See super class method satosa.frontends.base.FrontendModule#handle_authn_response
         :type context: satosa.context.Context
         :type internal_response: satosa.internal.InternalData
-        :rtype oic.utils.http_util.Response
+        :rtype: satosa.response.Response
         """
         raise NotImplementedError()
 
     def handle_backend_error(self, exception):
         """
         See super class satosa.frontends.base.FrontendModule
         :type exception: satosa.exception.SATOSAError
-        :rtype: oic.utils.http_util.Response
+        :rtype: satosa.response.Response
         """
         raise NotImplementedError()
 
     def register_endpoints(self, backend_names):
         """
         See super class satosa.frontends.base.FrontendModule
         :type backend_names: list[str]
@@ -45,14 +45,16 @@
         """
         url_map = [("^{}".format(self.name), self.ping_endpoint)]
 
         return url_map
 
     def ping_endpoint(self, context):
         """
+        :type context: satosa.context.Context
+        :rtype: satosa.response.Response
         """
         msg = "Ping returning 200 OK"
         logline = lu.LOG_FMT.format(id=lu.get_session_id(context.state), message=msg)
         logger.debug(logline)
 
         msg = " "
         return Response(msg)
```

### Comparing `SATOSA-8.2.0/src/satosa/frontends/saml2.py` & `SATOSA-8.3.0/src/satosa/frontends/saml2.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
         name_format = idp_policy.get_name_form(sp_entity_id)
         attrconvs = idp.config.attribute_converters
         idp_policy.acs = attrconvs
         attribute_filter = []
         for aconv in attrconvs:
             if aconv.name_format == name_format:
                 all_attributes = {v: None for v in aconv._fro.values()}
-                attribute_filter = list(idp_policy.restrict(all_attributes, sp_entity_id, idp.metadata).keys())
+                attribute_filter = list(idp_policy.restrict(all_attributes, sp_entity_id).keys())
                 break
         attribute_filter = self.converter.to_internal_filter(self.attribute_profile, attribute_filter)
         msg = "Filter: {}".format(attribute_filter)
         logline = lu.LOG_FMT.format(id=lu.get_session_id(state), message=msg)
         logger.debug(logline)
         return attribute_filter
```

### Comparing `SATOSA-8.2.0/src/satosa/internal.py` & `SATOSA-8.3.0/src/satosa/internal.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/logging_util.py` & `SATOSA-8.3.0/src/satosa/logging_util.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/metadata_creation/description.py` & `SATOSA-8.3.0/src/satosa/metadata_creation/description.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/metadata_creation/saml_metadata.py` & `SATOSA-8.3.0/src/satosa/metadata_creation/saml_metadata.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/account_linking.py` & `SATOSA-8.3.0/src/satosa/micro_services/account_linking.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/attribute_authorization.py` & `SATOSA-8.3.0/src/satosa/micro_services/attribute_authorization.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/attribute_generation.py` & `SATOSA-8.3.0/src/satosa/micro_services/attribute_generation.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/attribute_policy.py` & `SATOSA-8.3.0/src/satosa/micro_services/attribute_policy.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/attribute_processor.py` & `SATOSA-8.3.0/src/satosa/micro_services/attribute_processor.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/base.py` & `SATOSA-8.3.0/src/satosa/micro_services/base.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/consent.py` & `SATOSA-8.3.0/src/satosa/micro_services/consent.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/custom_logging.py` & `SATOSA-8.3.0/src/satosa/micro_services/custom_logging.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/custom_routing.py` & `SATOSA-8.3.0/src/satosa/micro_services/custom_routing.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,27 +63,29 @@
     Select which backend should be used based on who the requester is.
     """
 
     def __init__(self, config, *args, **kwargs):
         """
         Constructor.
         :param config: mapping from requester identifier to
-        backend module name under the key 'requester_mapping'
+        backend module name under the key 'requester_mapping'.
+        May also include default backend under key 'default_backend'.
         :type config: Dict[str, Dict[str, str]]
         """
         super().__init__(*args, **kwargs)
         self.requester_mapping = config['requester_mapping']
+        self.default_backend = config.get('default_backend')
 
     def process(self, context, data):
         """
         Will modify the context.target_backend attribute based on the requester identifier.
         :param context: request context
         :param data: the internal request
         """
-        context.target_backend = self.requester_mapping[data.requester]
+        context.target_backend = self.requester_mapping.get(data.requester) or self.default_backend
         return super().process(context, data)
 
 
 class DecideIfRequesterIsAllowed(RequestMicroService):
     """
     Decide whether a requester is allowed to send an authentication request to the target entity.
```

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/disco.py` & `SATOSA-8.3.0/src/satosa/micro_services/disco.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/hasher.py` & `SATOSA-8.3.0/src/satosa/micro_services/hasher.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/idp_hinting.py` & `SATOSA-8.3.0/src/satosa/micro_services/idp_hinting.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/ldap_attribute_store.py` & `SATOSA-8.3.0/src/satosa/micro_services/ldap_attribute_store.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/primary_identifier.py` & `SATOSA-8.3.0/src/satosa/micro_services/primary_identifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
             logger.debug(logline)
 
             # If one of the configured attribute names is name_id then if there is also a configured
             # name_id_format add the value for the NameID of that format if it was asserted by the IdP
             # or else add the value None.
             if 'name_id' in candidate['attribute_names']:
                 candidate_nameid_value = None
-                candidate_nameid_value = None
                 candidate_name_id_format = candidate.get('name_id_format')
                 name_id_value = data.subject_id
                 name_id_format = data.subject_type
                 if (
                     name_id_value
                     and candidate_name_id_format
                     and candidate_name_id_format == name_id_format
```

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/processors/gender_processor.py` & `SATOSA-8.3.0/src/satosa/micro_services/processors/gender_processor.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/processors/hash_processor.py` & `SATOSA-8.3.0/src/satosa/micro_services/processors/hash_processor.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/processors/regex_sub_processor.py` & `SATOSA-8.3.0/src/satosa/micro_services/processors/regex_sub_processor.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/processors/scope_extractor_processor.py` & `SATOSA-8.3.0/src/satosa/micro_services/processors/scope_extractor_processor.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/processors/scope_processor.py` & `SATOSA-8.3.0/src/satosa/micro_services/processors/scope_processor.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/micro_services/processors/scope_remover_processor.py` & `SATOSA-8.3.0/src/satosa/micro_services/processors/scope_remover_processor.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/plugin_loader.py` & `SATOSA-8.3.0/src/satosa/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/proxy_server.py` & `SATOSA-8.3.0/src/satosa/proxy_server.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/response.py` & `SATOSA-8.3.0/src/satosa/response.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/routing.py` & `SATOSA-8.3.0/src/satosa/routing.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/satosa_config.py` & `SATOSA-8.3.0/src/satosa/satosa_config.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/scripts/satosa_saml_metadata.py` & `SATOSA-8.3.0/src/satosa/scripts/satosa_saml_metadata.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/state.py` & `SATOSA-8.3.0/src/satosa/state.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/util.py` & `SATOSA-8.3.0/src/satosa/util.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/wsgi.py` & `SATOSA-8.3.0/src/satosa/wsgi.py`

 * *Files identical despite different names*

### Comparing `SATOSA-8.2.0/src/satosa/yaml.py` & `SATOSA-8.3.0/src/satosa/yaml.py`

 * *Files identical despite different names*

