# Comparing `tmp/pulumiverse_buildkite-2.0.0.tar.gz` & `tmp/pulumiverse_buildkite-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_buildkite-2.0.0.tar", last modified: Mon Jun  5 13:14:34 2023, max compression
+gzip compressed data, was "pulumiverse_buildkite-2.1.0.tar", last modified: Thu Jun  8 07:13:55 2023, max compression
```

## Comparing `pulumiverse_buildkite-2.0.0.tar` & `pulumiverse_buildkite-2.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:14:34.123654 pulumiverse_buildkite-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-06-05 13:14:34.123654 pulumiverse_buildkite-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:14:34.119654 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:14:34.119654 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/agent/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/agent/agent_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:14:34.119654 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/get_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:14:34.119654 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/organization/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/organization/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/organization/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:14:34.119654 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/pipeline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/pipeline/get_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    16858 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/pipeline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59566 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    20524 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/pipeline/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:14:34.123654 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/team/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/team/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/team/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/team/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    18253 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/team/team.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:14:34.119654 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-06-05 13:14:34.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-05 13:14:34.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:14:34.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:14:34.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 13:14:34.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 13:14:34.000000 pulumiverse_buildkite-2.0.0/pulumiverse_buildkite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:14:34.123654 pulumiverse_buildkite-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-05 13:14:33.000000 pulumiverse_buildkite-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:13:55.058591 pulumiverse_buildkite-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-08 07:13:55.058591 pulumiverse_buildkite-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:13:55.058591 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:13:55.058591 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/agent/agent_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:13:55.058591 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/get_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:13:55.058591 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/organization/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/organization/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:13:55.058591 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/pipeline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/pipeline/get_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16858 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/pipeline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59566 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20524 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/pipeline/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:13:55.058591 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/team/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/team/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/team/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/team/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18253 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/team/team.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:13:55.058591 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-08 07:13:55.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-08 07:13:55.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:13:55.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:13:55.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 07:13:55.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 07:13:55.000000 pulumiverse_buildkite-2.1.0/pulumiverse_buildkite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 07:13:55.058591 pulumiverse_buildkite-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-08 07:13:54.000000 pulumiverse_buildkite-2.1.0/setup.py
```

### Comparing `pulumiverse_buildkite-2.0.0/PKG-INFO` & `pulumiverse_buildkite-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_buildkite
-Version: 2.0.0
+Version: 2.1.0
 Summary: A Pulumi package for creating and managing Buildkite resources.
 Home-page: https://github.com/pulumiverse/pulumi-buildkite
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-buildkite
 Keywords: pulumi buildkite
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -15,16 +15,16 @@
 [![](https://img.shields.io/github/license/pulumiverse/pulumi-buildkite?style=for-the-badge)](LICENSE)
 [![](https://img.shields.io/github/actions/workflow/status/pulumiverse/pulumi-buildkite/verify.yml?style=for-the-badge)](https://github.com/pulumiverse/pulumi-buildkite/actions/workflows/verify.yml)
 [![](https://img.shields.io/github/release-date/pulumiverse/pulumi-buildkite?style=for-the-badge)](https://github.com/pulumiverse/pulumi-buildkite/releases)
 [![](https://img.shields.io/pypi/v/pulumiverse-buildkite?style=for-the-badge)](https://pypi.org/project/pulumiverse-buildkite/)
 [![](https://img.shields.io/pypi/dm/pulumiverse-buildkite?style=for-the-badge)](https://pypi.org/project/pulumiverse-buildkite/)
 [![](https://img.shields.io/nuget/v/Pulumiverse.Buildkite?style=for-the-badge)](https://www.nuget.org/packages/Pulumiverse.Buildkite/)
 [![](https://img.shields.io/nuget/dt/Pulumiverse.Buildkite?style=for-the-badge)](https://www.nuget.org/packages/Pulumiverse.Buildkite/)
-[![](https://img.shields.io/npm/v/@pulumiverse/pulumi-buildkite?style=for-the-badge)](https://www.npmjs.com/package/@pulumiverse/pulumi-buildkite)
-[![](https://img.shields.io/npm/dm/@pulumiverse/pulumi-buildkite?style=for-the-badge)](https://www.npmjs.com/package/@pulumiverse/pulumi-buildkite)
+[![](https://img.shields.io/npm/v/@pulumiverse/buildkite?style=for-the-badge)](https://www.npmjs.com/package/@pulumiverse/buildkite)
+[![](https://img.shields.io/npm/dm/@pulumiverse/buildkite?style=for-the-badge)](https://www.npmjs.com/package/@pulumiverse/buildkite)
 [![](https://img.shields.io/github/all-contributors/pulumiverse/pulumi-buildkite?color=ee8449&style=for-the-badge)](#contributors)
 
 The Buildkite Resource Provider lets you manage [Buildkite](http://buildkite.com) resources.
 
 The provider is built on https://github.com/buildkite/terraform-provider-buildkite.
 
 ## Installing
@@ -90,15 +90,15 @@
   'token',
   args,
 );
 ```
 
 ## Reference
 
-For detailed reference documentation, please visit the upstream Terraform provider's documentation at: https://registry.terraform.io/providers/buildkite/buildkite/latest>
+For detailed reference documentation, please visit the upstream Terraform provider's documentation at: https://registry.terraform.io/providers/buildkite/buildkite/latest
 
 ## Contributors
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
```

### Comparing `pulumiverse_buildkite-2.0.0/README.md` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,30 @@
+Metadata-Version: 2.1
+Name: pulumiverse-buildkite
+Version: 2.1.0
+Summary: A Pulumi package for creating and managing Buildkite resources.
+Home-page: https://github.com/pulumiverse/pulumi-buildkite
+License: Apache-2.0
+Project-URL: Repository, https://github.com/pulumiverse/pulumi-buildkite
+Keywords: pulumi buildkite
+Platform: UNKNOWN
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # Buildkite Resource Provider
 
 [![](https://img.shields.io/github/license/pulumiverse/pulumi-buildkite?style=for-the-badge)](LICENSE)
 [![](https://img.shields.io/github/actions/workflow/status/pulumiverse/pulumi-buildkite/verify.yml?style=for-the-badge)](https://github.com/pulumiverse/pulumi-buildkite/actions/workflows/verify.yml)
 [![](https://img.shields.io/github/release-date/pulumiverse/pulumi-buildkite?style=for-the-badge)](https://github.com/pulumiverse/pulumi-buildkite/releases)
 [![](https://img.shields.io/pypi/v/pulumiverse-buildkite?style=for-the-badge)](https://pypi.org/project/pulumiverse-buildkite/)
 [![](https://img.shields.io/pypi/dm/pulumiverse-buildkite?style=for-the-badge)](https://pypi.org/project/pulumiverse-buildkite/)
 [![](https://img.shields.io/nuget/v/Pulumiverse.Buildkite?style=for-the-badge)](https://www.nuget.org/packages/Pulumiverse.Buildkite/)
 [![](https://img.shields.io/nuget/dt/Pulumiverse.Buildkite?style=for-the-badge)](https://www.nuget.org/packages/Pulumiverse.Buildkite/)
-[![](https://img.shields.io/npm/v/@pulumiverse/pulumi-buildkite?style=for-the-badge)](https://www.npmjs.com/package/@pulumiverse/pulumi-buildkite)
-[![](https://img.shields.io/npm/dm/@pulumiverse/pulumi-buildkite?style=for-the-badge)](https://www.npmjs.com/package/@pulumiverse/pulumi-buildkite)
+[![](https://img.shields.io/npm/v/@pulumiverse/buildkite?style=for-the-badge)](https://www.npmjs.com/package/@pulumiverse/buildkite)
+[![](https://img.shields.io/npm/dm/@pulumiverse/buildkite?style=for-the-badge)](https://www.npmjs.com/package/@pulumiverse/buildkite)
 [![](https://img.shields.io/github/all-contributors/pulumiverse/pulumi-buildkite?color=ee8449&style=for-the-badge)](#contributors)
 
 The Buildkite Resource Provider lets you manage [Buildkite](http://buildkite.com) resources.
 
 The provider is built on https://github.com/buildkite/terraform-provider-buildkite.
 
 ## Installing
@@ -78,15 +90,15 @@
   'token',
   args,
 );
 ```
 
 ## Reference
 
-For detailed reference documentation, please visit the upstream Terraform provider's documentation at: https://registry.terraform.io/providers/buildkite/buildkite/latest>
+For detailed reference documentation, please visit the upstream Terraform provider's documentation at: https://registry.terraform.io/providers/buildkite/buildkite/latest
 
 ## Contributors
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
@@ -104,7 +116,9 @@
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+
```

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/__init__.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/_utilities.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/agent/agent_token.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/agent/agent_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/config/vars.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/get_meta.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/get_meta.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/organization/get_organization.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/organization/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/organization/settings.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/organization/settings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/pipeline/_inputs.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/pipeline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/pipeline/get_pipeline.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/pipeline/get_pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/pipeline/outputs.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/pipeline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/pipeline/pipeline.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/pipeline/schedule.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/pipeline/schedule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/provider.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/team/get_team.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/team/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/team/member.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/team/member.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite/team/team.py` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite/team/team.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite.egg-info/PKG-INFO` & `pulumiverse_buildkite-2.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,18 @@
-Metadata-Version: 2.1
-Name: pulumiverse-buildkite
-Version: 2.0.0
-Summary: A Pulumi package for creating and managing Buildkite resources.
-Home-page: https://github.com/pulumiverse/pulumi-buildkite
-License: Apache-2.0
-Project-URL: Repository, https://github.com/pulumiverse/pulumi-buildkite
-Keywords: pulumi buildkite
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # Buildkite Resource Provider
 
 [![](https://img.shields.io/github/license/pulumiverse/pulumi-buildkite?style=for-the-badge)](LICENSE)
 [![](https://img.shields.io/github/actions/workflow/status/pulumiverse/pulumi-buildkite/verify.yml?style=for-the-badge)](https://github.com/pulumiverse/pulumi-buildkite/actions/workflows/verify.yml)
 [![](https://img.shields.io/github/release-date/pulumiverse/pulumi-buildkite?style=for-the-badge)](https://github.com/pulumiverse/pulumi-buildkite/releases)
 [![](https://img.shields.io/pypi/v/pulumiverse-buildkite?style=for-the-badge)](https://pypi.org/project/pulumiverse-buildkite/)
 [![](https://img.shields.io/pypi/dm/pulumiverse-buildkite?style=for-the-badge)](https://pypi.org/project/pulumiverse-buildkite/)
 [![](https://img.shields.io/nuget/v/Pulumiverse.Buildkite?style=for-the-badge)](https://www.nuget.org/packages/Pulumiverse.Buildkite/)
 [![](https://img.shields.io/nuget/dt/Pulumiverse.Buildkite?style=for-the-badge)](https://www.nuget.org/packages/Pulumiverse.Buildkite/)
-[![](https://img.shields.io/npm/v/@pulumiverse/pulumi-buildkite?style=for-the-badge)](https://www.npmjs.com/package/@pulumiverse/pulumi-buildkite)
-[![](https://img.shields.io/npm/dm/@pulumiverse/pulumi-buildkite?style=for-the-badge)](https://www.npmjs.com/package/@pulumiverse/pulumi-buildkite)
+[![](https://img.shields.io/npm/v/@pulumiverse/buildkite?style=for-the-badge)](https://www.npmjs.com/package/@pulumiverse/buildkite)
+[![](https://img.shields.io/npm/dm/@pulumiverse/buildkite?style=for-the-badge)](https://www.npmjs.com/package/@pulumiverse/buildkite)
 [![](https://img.shields.io/github/all-contributors/pulumiverse/pulumi-buildkite?color=ee8449&style=for-the-badge)](#contributors)
 
 The Buildkite Resource Provider lets you manage [Buildkite](http://buildkite.com) resources.
 
 The provider is built on https://github.com/buildkite/terraform-provider-buildkite.
 
 ## Installing
@@ -90,15 +78,15 @@
   'token',
   args,
 );
 ```
 
 ## Reference
 
-For detailed reference documentation, please visit the upstream Terraform provider's documentation at: https://registry.terraform.io/providers/buildkite/buildkite/latest>
+For detailed reference documentation, please visit the upstream Terraform provider's documentation at: https://registry.terraform.io/providers/buildkite/buildkite/latest
 
 ## Contributors
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
@@ -116,9 +104,7 @@
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
-
-
```

### Comparing `pulumiverse_buildkite-2.0.0/pulumiverse_buildkite.egg-info/SOURCES.txt` & `pulumiverse_buildkite-2.1.0/pulumiverse_buildkite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.0.0/setup.py` & `pulumiverse_buildkite-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.0.0"
-PLUGIN_VERSION = "2.0.0"
+VERSION = "2.1.0"
+PLUGIN_VERSION = "2.1.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'buildkite', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse/pulumi-buildkite'])
         except OSError as error:
```

