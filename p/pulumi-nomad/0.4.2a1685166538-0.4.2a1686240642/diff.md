# Comparing `tmp/pulumi_nomad-0.4.2a1685166538.tar.gz` & `tmp/pulumi_nomad-0.4.2a1686240642.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_nomad-0.4.2a1685166538.tar", last modified: Sat May 27 06:02:20 2023, max compression
+gzip compressed data, was "pulumi_nomad-0.4.2a1686240642.tar", last modified: Thu Jun  8 16:14:45 2023, max compression
```

## Comparing `pulumi_nomad-0.4.2a1685166538.tar` & `pulumi_nomad-0.4.2a1686240642.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:02:20.197675 pulumi_nomad-0.4.2a1685166538/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-27 06:02:20.197675 pulumi_nomad-0.4.2a1685166538/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:02:20.193675 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39088 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/acl_auth_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/acl_binding_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/acl_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/acl_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    27631 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/acl_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:02:20.197675 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    52267 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/external_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_acl_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_acl_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_acl_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_acl_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_acl_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_acl_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_job_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_scaling_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_scaling_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_scheduler_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)    40679 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    55024 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20563 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/quote_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/scheduler_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15554 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/sentinel_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    56839 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:02:20.193675 pulumi_nomad-0.4.2a1685166538/pulumi_nomad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-27 06:02:20.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-27 06:02:20.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:02:20.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:02:20.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 06:02:20.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-27 06:02:20.000000 pulumi_nomad-0.4.2a1685166538/pulumi_nomad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 06:02:20.197675 pulumi_nomad-0.4.2a1685166538/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-27 06:02:19.000000 pulumi_nomad-0.4.2a1685166538/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:14:45.955285 pulumi_nomad-0.4.2a1686240642/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-08 16:14:45.955285 pulumi_nomad-0.4.2a1686240642/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:14:45.951285 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40373 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/acl_auth_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/acl_binding_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/acl_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/acl_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28545 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/acl_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:14:45.955285 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52267 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/external_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_acl_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_acl_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_acl_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_acl_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_acl_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_acl_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_job_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_scaling_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_scaling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_scheduler_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40679 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56309 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20563 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/quote_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/scheduler_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/sentinel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56839 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:14:45.955285 pulumi_nomad-0.4.2a1686240642/pulumi_nomad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/pulumi_nomad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 16:14:45.955285 pulumi_nomad-0.4.2a1686240642/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-08 16:14:45.000000 pulumi_nomad-0.4.2a1686240642/setup.py
```

### Comparing `pulumi_nomad-0.4.2a1685166538/PKG-INFO` & `pulumi_nomad-0.4.2a1686240642/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: pulumi_nomad
-Version: 0.4.2a1685166538
-Summary: A Pulumi package for creating and managing nomad cloud resources.
-Home-page: https://pulumi.io
-License: Apache-2.0
-Project-URL: Repository, https://github.com/pulumi/pulumi-nomad
-Keywords: pulumi nomad
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 [![Actions Status](https://github.com/pulumi/pulumi-nomad/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-nomad/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fnomad.svg)](https://www.npmjs.com/package/@pulumi/nomad)
 [![Python version](https://badge.fury.io/py/pulumi-nomad.svg)](https://pypi.org/project/pulumi-nomad)
 [![NuGet version](https://badge.fury.io/nu/pulumi.nomad.svg)](https://badge.fury.io/nu/pulumi.nomad)
 [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-nomad/sdk/go)](https://pkg.go.dev/github.com/pulumi/pulumi-nomad/sdk/go)
 [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-nomad/blob/master/LICENSE)
@@ -86,9 +74,7 @@
 - `name` - The name of the header.
 - `value` - The value of the header.
 
 ## Reference
 
 For further information, please visit [the Nomad provider docs](https://www.pulumi.com/docs/intro/cloud-providers/nomad)
 or for detailed reference documentation, please visit [the API docs](https://www.pulumi.com/docs/reference/pkg/nomad).
-
-
```

### Comparing `pulumi_nomad-0.4.2a1685166538/README.md` & `pulumi_nomad-0.4.2a1686240642/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: pulumi_nomad
+Version: 0.4.2a1686240642
+Summary: A Pulumi package for creating and managing nomad cloud resources.
+Home-page: https://pulumi.io
+License: Apache-2.0
+Project-URL: Repository, https://github.com/pulumi/pulumi-nomad
+Keywords: pulumi nomad
+Platform: UNKNOWN
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 [![Actions Status](https://github.com/pulumi/pulumi-nomad/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-nomad/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fnomad.svg)](https://www.npmjs.com/package/@pulumi/nomad)
 [![Python version](https://badge.fury.io/py/pulumi-nomad.svg)](https://pypi.org/project/pulumi-nomad)
 [![NuGet version](https://badge.fury.io/nu/pulumi.nomad.svg)](https://badge.fury.io/nu/pulumi.nomad)
 [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-nomad/sdk/go)](https://pkg.go.dev/github.com/pulumi/pulumi-nomad/sdk/go)
 [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-nomad/blob/master/LICENSE)
@@ -74,7 +86,9 @@
 - `name` - The name of the header.
 - `value` - The value of the header.
 
 ## Reference
 
 For further information, please visit [the Nomad provider docs](https://www.pulumi.com/docs/intro/cloud-providers/nomad)
 or for detailed reference documentation, please visit [the API docs](https://www.pulumi.com/docs/reference/pkg/nomad).
+
+
```

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/__init__.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/_inputs.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,23 +307,29 @@
 
 @pulumi.input_type
 class ExternalVolumeTopologyArgs:
     def __init__(__self__, *,
                  segments: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: `(map[string]string)` - Define the attributes for the topology request.
+               
+               In addition to the above arguments, the following attributes are exported and
+               can be referenced:
         """
         if segments is not None:
             pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         `(map[string]string)` - Define the attributes for the topology request.
+
+        In addition to the above arguments, the following attributes are exported and
+        can be referenced:
         """
         return pulumi.get(self, "segments")
 
     @segments.setter
     def segments(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "segments", value)
 
@@ -385,22 +391,28 @@
 
 @pulumi.input_type
 class ExternalVolumeTopologyRequestPreferredTopologyArgs:
     def __init__(__self__, *,
                  segments: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         """
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: `(map[string]string)` - Define the attributes for the topology request.
+               
+               In addition to the above arguments, the following attributes are exported and
+               can be referenced:
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> pulumi.Input[Mapping[str, pulumi.Input[str]]]:
         """
         `(map[string]string)` - Define the attributes for the topology request.
+
+        In addition to the above arguments, the following attributes are exported and
+        can be referenced:
         """
         return pulumi.get(self, "segments")
 
     @segments.setter
     def segments(self, value: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         pulumi.set(self, "segments", value)
 
@@ -423,22 +435,28 @@
 
 @pulumi.input_type
 class ExternalVolumeTopologyRequestRequiredTopologyArgs:
     def __init__(__self__, *,
                  segments: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         """
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: `(map[string]string)` - Define the attributes for the topology request.
+               
+               In addition to the above arguments, the following attributes are exported and
+               can be referenced:
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> pulumi.Input[Mapping[str, pulumi.Input[str]]]:
         """
         `(map[string]string)` - Define the attributes for the topology request.
+
+        In addition to the above arguments, the following attributes are exported and
+        can be referenced:
         """
         return pulumi.get(self, "segments")
 
     @segments.setter
     def segments(self, value: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         pulumi.set(self, "segments", value)
 
@@ -954,23 +972,29 @@
 
 @pulumi.input_type
 class VolumeTopologyArgs:
     def __init__(__self__, *,
                  segments: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: `(map[string]string)` - Define the attributes for the topology request.
+               
+               In addition to the above arguments, the following attributes are exported and
+               can be referenced:
         """
         if segments is not None:
             pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         `(map[string]string)` - Define the attributes for the topology request.
+
+        In addition to the above arguments, the following attributes are exported and
+        can be referenced:
         """
         return pulumi.get(self, "segments")
 
     @segments.setter
     def segments(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "segments", value)
 
@@ -1016,22 +1040,28 @@
 
 @pulumi.input_type
 class VolumeTopologyRequestRequiredTopologyArgs:
     def __init__(__self__, *,
                  segments: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         """
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] segments: `(map[string]string)` - Define the attributes for the topology request.
+               
+               In addition to the above arguments, the following attributes are exported and
+               can be referenced:
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> pulumi.Input[Mapping[str, pulumi.Input[str]]]:
         """
         `(map[string]string)` - Define the attributes for the topology request.
+
+        In addition to the above arguments, the following attributes are exported and
+        can be referenced:
         """
         return pulumi.get(self, "segments")
 
     @segments.setter
     def segments(self, value: pulumi.Input[Mapping[str, pulumi.Input[str]]]):
         pulumi.set(self, "segments", value)
```

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/_utilities.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/acl_auth_method.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/acl_auth_method.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/acl_binding_rule.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/acl_binding_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/acl_policy.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/acl_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/acl_role.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/acl_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/acl_token.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/acl_token.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,17 @@
         """
         The set of arguments for constructing a AclToken resource.
         :param pulumi.Input[str] type: `(string: <required>)` - The type of token this is. Use `client`
                for tokens that will have policies associated with them. Use `management`
                for tokens that can perform any action.
         :param pulumi.Input[str] expiration_ttl: `(string: "")` - Provides a TTL for the token in the form of
                a time duration such as `"5m"` or `"1h"`.
+               
+               In addition to the above arguments, the following attributes are exported and
+               can be referenced:
         :param pulumi.Input[bool] global_: `(bool: false)` - Whether the token should be replicated to all
                regions, or if it will only be used in the region it was created in.
         :param pulumi.Input[str] name: `(string: "")` - A human-friendly name for this token.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] policies: `(set: [])` - A set of policy names to associate with this
                token. Must be set on `client`-type tokens, must not be set on
                `management`-type tokens. Policies do not need to exist before being
                used here.
@@ -67,14 +70,17 @@
 
     @property
     @pulumi.getter(name="expirationTtl")
     def expiration_ttl(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: "")` - Provides a TTL for the token in the form of
         a time duration such as `"5m"` or `"1h"`.
+
+        In addition to the above arguments, the following attributes are exported and
+        can be referenced:
         """
         return pulumi.get(self, "expiration_ttl")
 
     @expiration_ttl.setter
     def expiration_ttl(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "expiration_ttl", value)
 
@@ -150,14 +156,17 @@
         :param pulumi.Input[str] accessor_id: `(string)` - A non-sensitive identifier for this token that
                can be logged and shared safely without granting any access to the cluster.
         :param pulumi.Input[str] create_time: `(string)` - The timestamp the token was created.
         :param pulumi.Input[str] expiration_time: `(string)` - The timestamp after which the token is
                considered expired and eligible for destruction.
         :param pulumi.Input[str] expiration_ttl: `(string: "")` - Provides a TTL for the token in the form of
                a time duration such as `"5m"` or `"1h"`.
+               
+               In addition to the above arguments, the following attributes are exported and
+               can be referenced:
         :param pulumi.Input[bool] global_: `(bool: false)` - Whether the token should be replicated to all
                regions, or if it will only be used in the region it was created in.
         :param pulumi.Input[str] name: `(string: "")` - A human-friendly name for this token.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] policies: `(set: [])` - A set of policy names to associate with this
                token. Must be set on `client`-type tokens, must not be set on
                `management`-type tokens. Policies do not need to exist before being
                used here.
@@ -230,14 +239,17 @@
 
     @property
     @pulumi.getter(name="expirationTtl")
     def expiration_ttl(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: "")` - Provides a TTL for the token in the form of
         a time duration such as `"5m"` or `"1h"`.
+
+        In addition to the above arguments, the following attributes are exported and
+        can be referenced:
         """
         return pulumi.get(self, "expiration_ttl")
 
     @expiration_ttl.setter
     def expiration_ttl(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "expiration_ttl", value)
 
@@ -387,14 +399,17 @@
         pulumi.export("nomadToken", token.secret_id)
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] expiration_ttl: `(string: "")` - Provides a TTL for the token in the form of
                a time duration such as `"5m"` or `"1h"`.
+               
+               In addition to the above arguments, the following attributes are exported and
+               can be referenced:
         :param pulumi.Input[bool] global_: `(bool: false)` - Whether the token should be replicated to all
                regions, or if it will only be used in the region it was created in.
         :param pulumi.Input[str] name: `(string: "")` - A human-friendly name for this token.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] policies: `(set: [])` - A set of policy names to associate with this
                token. Must be set on `client`-type tokens, must not be set on
                `management`-type tokens. Policies do not need to exist before being
                used here.
@@ -537,14 +552,17 @@
         :param pulumi.Input[str] accessor_id: `(string)` - A non-sensitive identifier for this token that
                can be logged and shared safely without granting any access to the cluster.
         :param pulumi.Input[str] create_time: `(string)` - The timestamp the token was created.
         :param pulumi.Input[str] expiration_time: `(string)` - The timestamp after which the token is
                considered expired and eligible for destruction.
         :param pulumi.Input[str] expiration_ttl: `(string: "")` - Provides a TTL for the token in the form of
                a time duration such as `"5m"` or `"1h"`.
+               
+               In addition to the above arguments, the following attributes are exported and
+               can be referenced:
         :param pulumi.Input[bool] global_: `(bool: false)` - Whether the token should be replicated to all
                regions, or if it will only be used in the region it was created in.
         :param pulumi.Input[str] name: `(string: "")` - A human-friendly name for this token.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] policies: `(set: [])` - A set of policy names to associate with this
                token. Must be set on `client`-type tokens, must not be set on
                `management`-type tokens. Policies do not need to exist before being
                used here.
@@ -600,14 +618,17 @@
 
     @property
     @pulumi.getter(name="expirationTtl")
     def expiration_ttl(self) -> pulumi.Output[Optional[str]]:
         """
         `(string: "")` - Provides a TTL for the token in the form of
         a time duration such as `"5m"` or `"1h"`.
+
+        In addition to the above arguments, the following attributes are exported and
+        can be referenced:
         """
         return pulumi.get(self, "expiration_ttl")
 
     @property
     @pulumi.getter(name="global")
     def global_(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/config/outputs.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/config/vars.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/external_volume.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/external_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_acl_policies.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_acl_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_acl_policy.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_acl_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_acl_role.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_acl_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_acl_roles.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_acl_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_acl_token.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_acl_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_acl_tokens.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_acl_tokens.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_datacenters.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_deployments.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_deployments.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_job.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_job_parser.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_job_parser.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_namespace.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_namespaces.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_namespaces.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_plugin.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_plugins.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_plugins.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_regions.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_scaling_policies.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_scaling_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_scaling_policy.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_scaling_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_scheduler_policy.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_scheduler_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/get_volumes.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/get_volumes.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/job.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/job.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/namespace.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/outputs.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -328,23 +328,29 @@
 
 @pulumi.output_type
 class ExternalVolumeTopology(dict):
     def __init__(__self__, *,
                  segments: Optional[Mapping[str, str]] = None):
         """
         :param Mapping[str, str] segments: `(map[string]string)` - Define the attributes for the topology request.
+               
+               In addition to the above arguments, the following attributes are exported and
+               can be referenced:
         """
         if segments is not None:
             pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Optional[Mapping[str, str]]:
         """
         `(map[string]string)` - Define the attributes for the topology request.
+
+        In addition to the above arguments, the following attributes are exported and
+        can be referenced:
         """
         return pulumi.get(self, "segments")
 
 
 @pulumi.output_type
 class ExternalVolumeTopologyRequest(dict):
     def __init__(__self__, *,
@@ -390,22 +396,28 @@
 
 @pulumi.output_type
 class ExternalVolumeTopologyRequestPreferredTopology(dict):
     def __init__(__self__, *,
                  segments: Mapping[str, str]):
         """
         :param Mapping[str, str] segments: `(map[string]string)` - Define the attributes for the topology request.
+               
+               In addition to the above arguments, the following attributes are exported and
+               can be referenced:
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Mapping[str, str]:
         """
         `(map[string]string)` - Define the attributes for the topology request.
+
+        In addition to the above arguments, the following attributes are exported and
+        can be referenced:
         """
         return pulumi.get(self, "segments")
 
 
 @pulumi.output_type
 class ExternalVolumeTopologyRequestRequired(dict):
     def __init__(__self__, *,
@@ -420,22 +432,28 @@
 
 @pulumi.output_type
 class ExternalVolumeTopologyRequestRequiredTopology(dict):
     def __init__(__self__, *,
                  segments: Mapping[str, str]):
         """
         :param Mapping[str, str] segments: `(map[string]string)` - Define the attributes for the topology request.
+               
+               In addition to the above arguments, the following attributes are exported and
+               can be referenced:
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Mapping[str, str]:
         """
         `(map[string]string)` - Define the attributes for the topology request.
+
+        In addition to the above arguments, the following attributes are exported and
+        can be referenced:
         """
         return pulumi.get(self, "segments")
 
 
 @pulumi.output_type
 class JobHcl2(dict):
     @staticmethod
@@ -963,23 +981,29 @@
 
 @pulumi.output_type
 class VolumeTopology(dict):
     def __init__(__self__, *,
                  segments: Optional[Mapping[str, str]] = None):
         """
         :param Mapping[str, str] segments: `(map[string]string)` - Define the attributes for the topology request.
+               
+               In addition to the above arguments, the following attributes are exported and
+               can be referenced:
         """
         if segments is not None:
             pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Optional[Mapping[str, str]]:
         """
         `(map[string]string)` - Define the attributes for the topology request.
+
+        In addition to the above arguments, the following attributes are exported and
+        can be referenced:
         """
         return pulumi.get(self, "segments")
 
 
 @pulumi.output_type
 class VolumeTopologyRequest(dict):
     def __init__(__self__, *,
@@ -1013,22 +1037,28 @@
 
 @pulumi.output_type
 class VolumeTopologyRequestRequiredTopology(dict):
     def __init__(__self__, *,
                  segments: Mapping[str, str]):
         """
         :param Mapping[str, str] segments: `(map[string]string)` - Define the attributes for the topology request.
+               
+               In addition to the above arguments, the following attributes are exported and
+               can be referenced:
         """
         pulumi.set(__self__, "segments", segments)
 
     @property
     @pulumi.getter
     def segments(self) -> Mapping[str, str]:
         """
         `(map[string]string)` - Define the attributes for the topology request.
+
+        In addition to the above arguments, the following attributes are exported and
+        can be referenced:
         """
         return pulumi.get(self, "segments")
 
 
 @pulumi.output_type
 class GetAclPoliciesPolicyResult(dict):
     def __init__(__self__, *,
```

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/provider.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/quote_specification.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/quote_specification.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/scheduler_config.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/scheduler_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/sentinel_policy.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/sentinel_policy.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,17 @@
         """
         The set of arguments for constructing a SentinelPolicy resource.
         :param pulumi.Input[str] enforcement_level: `(strings: <required>)` - The [enforcement level][enforcement-level]
                for this policy.
         :param pulumi.Input[str] policy: `(string: <required>)` - The contents of the policy to register.
         :param pulumi.Input[str] scope: `(strings: <required>)` - The [scope][scope] for this policy.
         :param pulumi.Input[str] description: `(string: "")` - A description of the policy.
+               
+               [scope]: https://www.nomadproject.io/guides/sentinel-policy.html#policy-scope
+               [enforcement-level]: https://www.nomadproject.io/guides/sentinel-policy.html#enforcement-level
         :param pulumi.Input[str] name: `(string: <required>)` - A unique name for the policy.
         """
         pulumi.set(__self__, "enforcement_level", enforcement_level)
         pulumi.set(__self__, "policy", policy)
         pulumi.set(__self__, "scope", scope)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -74,14 +77,17 @@
         pulumi.set(self, "scope", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: "")` - A description of the policy.
+
+        [scope]: https://www.nomadproject.io/guides/sentinel-policy.html#policy-scope
+        [enforcement-level]: https://www.nomadproject.io/guides/sentinel-policy.html#enforcement-level
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -105,14 +111,17 @@
                  enforcement_level: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  policy: Optional[pulumi.Input[str]] = None,
                  scope: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SentinelPolicy resources.
         :param pulumi.Input[str] description: `(string: "")` - A description of the policy.
+               
+               [scope]: https://www.nomadproject.io/guides/sentinel-policy.html#policy-scope
+               [enforcement-level]: https://www.nomadproject.io/guides/sentinel-policy.html#enforcement-level
         :param pulumi.Input[str] enforcement_level: `(strings: <required>)` - The [enforcement level][enforcement-level]
                for this policy.
         :param pulumi.Input[str] name: `(string: <required>)` - A unique name for the policy.
         :param pulumi.Input[str] policy: `(string: <required>)` - The contents of the policy to register.
         :param pulumi.Input[str] scope: `(strings: <required>)` - The [scope][scope] for this policy.
         """
         if description is not None:
@@ -127,14 +136,17 @@
             pulumi.set(__self__, "scope", scope)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
         `(string: "")` - A description of the policy.
+
+        [scope]: https://www.nomadproject.io/guides/sentinel-policy.html#policy-scope
+        [enforcement-level]: https://www.nomadproject.io/guides/sentinel-policy.html#enforcement-level
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -228,14 +240,17 @@
         \"\"\",
             scope="submit-job")
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: `(string: "")` - A description of the policy.
+               
+               [scope]: https://www.nomadproject.io/guides/sentinel-policy.html#policy-scope
+               [enforcement-level]: https://www.nomadproject.io/guides/sentinel-policy.html#enforcement-level
         :param pulumi.Input[str] enforcement_level: `(strings: <required>)` - The [enforcement level][enforcement-level]
                for this policy.
         :param pulumi.Input[str] name: `(string: <required>)` - A unique name for the policy.
         :param pulumi.Input[str] policy: `(string: <required>)` - The contents of the policy to register.
         :param pulumi.Input[str] scope: `(strings: <required>)` - The [scope][scope] for this policy.
         """
         ...
@@ -333,14 +348,17 @@
         Get an existing SentinelPolicy resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: `(string: "")` - A description of the policy.
+               
+               [scope]: https://www.nomadproject.io/guides/sentinel-policy.html#policy-scope
+               [enforcement-level]: https://www.nomadproject.io/guides/sentinel-policy.html#enforcement-level
         :param pulumi.Input[str] enforcement_level: `(strings: <required>)` - The [enforcement level][enforcement-level]
                for this policy.
         :param pulumi.Input[str] name: `(string: <required>)` - A unique name for the policy.
         :param pulumi.Input[str] policy: `(string: <required>)` - The contents of the policy to register.
         :param pulumi.Input[str] scope: `(strings: <required>)` - The [scope][scope] for this policy.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -355,14 +373,17 @@
         return SentinelPolicy(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
         `(string: "")` - A description of the policy.
+
+        [scope]: https://www.nomadproject.io/guides/sentinel-policy.html#policy-scope
+        [enforcement-level]: https://www.nomadproject.io/guides/sentinel-policy.html#enforcement-level
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="enforcementLevel")
     def enforcement_level(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad/volume.py` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad.egg-info/PKG-INFO` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-nomad
-Version: 0.4.2a1685166538
+Version: 0.4.2a1686240642
 Summary: A Pulumi package for creating and managing nomad cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-nomad
 Keywords: pulumi nomad
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_nomad-0.4.2a1685166538/pulumi_nomad.egg-info/SOURCES.txt` & `pulumi_nomad-0.4.2a1686240642/pulumi_nomad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1685166538/setup.py` & `pulumi_nomad-0.4.2a1686240642/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.4.2a1685166538"
-PLUGIN_VERSION = "0.4.2-alpha.1685166538+a7c556c1"
+VERSION = "0.4.2a1686240642"
+PLUGIN_VERSION = "0.4.2-alpha.1686240642+350d5a02"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'nomad', PLUGIN_VERSION])
         except OSError as error:
```

