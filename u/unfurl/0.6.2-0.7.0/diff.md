# Comparing `tmp/unfurl-0.6.2.tar.gz` & `tmp/unfurl-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unfurl-0.6.2.tar", last modified: Sat Apr 29 08:02:00 2023, max compression
+gzip compressed data, was "unfurl-0.7.0.tar", last modified: Thu Jun  8 17:15:46 2023, max compression
```

## Comparing `unfurl-0.6.2.tar` & `unfurl-0.7.0.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.987374 unfurl-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 08:01:57.000000 unfurl-0.6.2/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      282 2023-04-29 08:01:57.000000 unfurl-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-04-29 08:02:00.987374 unfurl-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-29 08:01:57.000000 unfurl-0.6.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1218 2023-04-29 08:02:00.987374 unfurl-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-29 08:01:57.000000 unfurl-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.971373 unfurl-0.6.2/unfurl/
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43551 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/changelog-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    34224 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/cloudmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    49950 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/configurators/
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/dns-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/docker-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/helm-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16491 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/kompose.py
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/supervisor-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20779 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/configurators/terraform.py
--rw-r--r--   0 runner    (1001) docker     (123)    29526 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/filter_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/filter_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/filter_plugins/ref.py
--rw-r--r--   0 runner    (1001) docker     (123)    45647 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    57578 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    55961 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/localenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/lookup_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/lookup_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/lookup_plugins/unfurl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/manifest-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    28145 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    25759 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    17046 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    41448 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    44834 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/planrequests.py
--rw-r--r--   0 runner    (1001) docker     (123)    21883 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/projectpaths.py
--rw-r--r--   0 runner    (1001) docker     (123)    30903 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    26994 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    39427 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    51978 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    58230 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/aws/unfurl.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/dashboard/manifest.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/dashboard/unfurl.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/digitalocean/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/digitalocean/unfurl.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/gcp/unfurl.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/gitignore.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/home/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/home/manifest-template.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/home/unfurl.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/local/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/local/ensemble-examples.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/local-unfurl-template.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/manifest-template.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/manifest.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/python3.10/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.10/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    72466 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.10/Pipfile.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.975373 unfurl-0.6.2/unfurl/templates/python3.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.11/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    68311 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.11/Pipfile.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.979373 unfurl-0.6.2/unfurl/templates/python3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.7/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    74406 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.7/Pipfile.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.979373 unfurl-0.6.2/unfurl/templates/python3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.8/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    74070 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.8/Pipfile.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.979373 unfurl-0.6.2/unfurl/templates/python3.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.9/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    73509 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/python3.9/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/secrets.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/service-template.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/unfurl.local.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/templates/unfurl.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    64983 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/to_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    55031 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/tosca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.979373 unfurl-0.6.2/unfurl/tosca_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/tosca_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/tosca_plugins/artifacts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/tosca_plugins/googlecloud.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/tosca_plugins/k8s.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/tosca_plugins/localhost.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18452 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/tosca_plugins/tosca-ext.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/unfurl-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    23855 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.979373 unfurl-0.6.2/unfurl/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.979373 unfurl-0.6.2/unfurl/vendor/sphinx-jsonschema/
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/vendor/sphinx-jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/vendor/sphinx-jsonschema/wide_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/dataentity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/
--rw-r--r--   0 runner    (1001) docker     (123)    32477 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    33031 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/artifacttype.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/attribute_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/capabilitytype.py
--rw-r--r--   0 runner    (1001) docker     (123)    24807 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/grouptype.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    15138 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/nodetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/policytype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/portspectype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/property_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/relationshiptype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/scalarunit.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/statefulentitytype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/elements/tosca_type_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17924 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/entity_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/exttools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/mec/
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/mec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.967373 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py
--rw-r--r--   0 runner    (1001) docker     (123)    39174 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    16716 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    25407 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/nodetemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.983373 unfurl-0.6.2/unfurl/vendor/toscaparser/prereq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/prereq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/prereq/csar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/relationship_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/substitution_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19241 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/topology_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    15317 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/tosca_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/tpl_relationship_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/unsupportedtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.987374 unfurl-0.6.2/unfurl/vendor/toscaparser/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/utils/gettextutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/utils/urlutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/utils/validateutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/utils/yamlparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-29 08:01:58.000000 unfurl-0.6.2/unfurl/vendor/toscaparser/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    28193 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/yamlloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    39094 2023-04-29 08:01:57.000000 unfurl-0.6.2/unfurl/yamlmanifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 08:02:00.971373 unfurl-0.6.2/unfurl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 08:02:00.000000 unfurl-0.6.2/unfurl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.951974 unfurl-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-08 17:15:43.000000 unfurl-0.7.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      282 2023-06-08 17:15:43.000000 unfurl-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-06-08 17:15:46.951974 unfurl-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-06-08 17:15:43.000000 unfurl-0.7.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-06-08 17:15:46.951974 unfurl-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-08 17:15:43.000000 unfurl-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.939973 unfurl-0.7.0/unfurl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44262 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/changelog-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50240 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/cloudmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50040 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/configurators/
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/configurators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/configurators/ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    17357 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/configurators/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/configurators/dns-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/configurators/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/configurators/docker-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/configurators/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/configurators/helm-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16659 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/configurators/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/configurators/kompose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/configurators/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/configurators/supervisor-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/configurators/supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20833 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/configurators/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30685 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/filter_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/filter_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/filter_plugins/ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45653 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57945 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56589 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/localenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/lookup_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/lookup_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/lookup_plugins/unfurl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16094 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/manifest-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30360 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25719 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17599 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44296 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45532 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/planrequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22039 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/projectpaths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33741 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26997 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43549 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53433 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61741 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/templates/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/aws/unfurl.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/dashboard/manifest.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/dashboard/unfurl.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/templates/digitalocean/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/digitalocean/unfurl.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/templates/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/gcp/unfurl.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/gitignore.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/templates/home/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/home/manifest-template.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/home/unfurl.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/templates/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/local/ensemble-examples.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/local-unfurl-template.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/manifest-template.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/manifest.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/templates/python3.10/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/python3.10/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    72466 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/python3.10/Pipfile.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/templates/python3.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/python3.11/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    68311 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/python3.11/Pipfile.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/templates/python3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/python3.7/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    74406 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/python3.7/Pipfile.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/templates/python3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/python3.8/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    74070 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/python3.8/Pipfile.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/templates/python3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/python3.9/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    73509 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/python3.9/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/secrets.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/service-template.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/unfurl.local.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/templates/unfurl.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    74712 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/to_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60896 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/tosca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.943974 unfurl-0.7.0/unfurl/tosca_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/tosca_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/tosca_plugins/artifacts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/tosca_plugins/googlecloud.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/tosca_plugins/k8s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/tosca_plugins/localhost.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18452 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/tosca_plugins/tosca-ext.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/unfurl-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23855 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.947974 unfurl-0.7.0/unfurl/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.947974 unfurl-0.7.0/unfurl/vendor/sphinx-jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/vendor/sphinx-jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/vendor/sphinx-jsonschema/wide_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.947974 unfurl-0.7.0/unfurl/vendor/toscaparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/activities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.947974 unfurl-0.7.0/unfurl/vendor/toscaparser/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/dataentity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.951974 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)    32477 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    33031 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/artifacttype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/attribute_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/capabilitytype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24807 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/grouptype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15138 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/nodetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/policytype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/portspectype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/property_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/relationshiptype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/scalarunit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/statefulentitytype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/elements/tosca_type_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/entity_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.951974 unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/exttools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.951974 unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/mec/
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/mec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.951974 unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/nfv/
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/nfv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.935974 unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/nfv/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.951974 unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/nfv/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39174 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26876 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/nodetemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.951974 unfurl-0.7.0/unfurl/vendor/toscaparser/prereq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/prereq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/prereq/csar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/relationship_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/substitution_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/topology_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/tosca_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/tpl_relationship_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/unsupportedtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.951974 unfurl-0.7.0/unfurl/vendor/toscaparser/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/utils/gettextutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/utils/urlutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/utils/validateutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/utils/yamlparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-08 17:15:44.000000 unfurl-0.7.0/unfurl/vendor/toscaparser/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33567 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/yamlloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40399 2023-06-08 17:15:43.000000 unfurl-0.7.0/unfurl/yamlmanifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:15:46.939973 unfurl-0.7.0/unfurl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-06-08 17:15:46.000000 unfurl-0.7.0/unfurl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-08 17:15:46.000000 unfurl-0.7.0/unfurl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:15:46.000000 unfurl-0.7.0/unfurl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-08 17:15:46.000000 unfurl-0.7.0/unfurl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:15:46.000000 unfurl-0.7.0/unfurl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-08 17:15:46.000000 unfurl-0.7.0/unfurl.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-08 17:15:46.000000 unfurl-0.7.0/unfurl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:15:46.000000 unfurl-0.7.0/unfurl.egg-info/top_level.txt
```

### Comparing `unfurl-0.6.2/LICENSE` & `unfurl-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/PKG-INFO` & `unfurl-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfurl
-Version: 0.6.2
+Version: 0.7.0
 Summary: use Git to record and deploy changes to your DevOps infrastructure
 Home-page: https://github.com/onecommons/unfurl
 Author: Adam Souzis
 Author-email: adam@onecommons.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: full
+Provides-Extra: server
 Provides-Extra: test
 License-File: LICENSE
 
 <p align="center">
   <img src="https://docs.unfurl.run/_images/unfurl_logo.svg" width="400px">
 </p>
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: unfurl Version: 0.6.2 Summary: use Git to record
+Metadata-Version: 2.1 Name: unfurl Version: 0.7.0 Summary: use Git to record
 and deploy changes to your DevOps infrastructure Home-page: https://github.com/
 onecommons/unfurl Author: Adam Souzis Author-email: adam@onecommons.org
 License: MIT Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-Provides-Extra: full Provides-Extra: test License-File: LICENSE
+Provides-Extra: full Provides-Extra: server Provides-Extra: test License-File:
+LICENSE
                [https://docs.unfurl.run/_images/unfurl_logo.svg]
                                 [PyPI_version]
 # Introduction Unfurl is a command line tool for managing your DevOps
 infrastructure. Unfurl lets you easily track configuration, secrets, software
 and code dependencies, and deployment history all in git. Unfurl can integrate
 with the DevOps tools you are already using -- like Terraform, Ansible, and
 Helm -- allowing you to encapsulate your DevOps processes into reusable
```

### Comparing `unfurl-0.6.2/README.md` & `unfurl-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/setup.cfg` & `unfurl-0.7.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 	supervisor
 	google-cloud-compute==1.3.2
 	google-cloud-dns==0.34.0
 	google-auth
 	python-gitlab<=3.4.0
 	gunicorn==20.1.0
 	redis==4.3.5
+server = 
+	gunicorn==20.1.0
+	redis==4.3.5
 
 [bdist_wheel]
 universal = 1
 
 [pbr]
 skip_git_sdist = True
 skip_authors = True
```

### Comparing `unfurl-0.6.2/unfurl/__init__.py` & `unfurl-0.7.0/unfurl/__init__.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/__main__.py` & `unfurl-0.7.0/unfurl/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,14 +447,23 @@
     rv = subprocess.call(remote, env=env, shell=shell)
     if options.get("standalone_mode") is False:
         return rv
     else:
         sys.exit(rv)
 
 
+def _print_query(query, result):
+    click.echo("Query: " + query)
+    if result is None:
+        click.echo("No results found")
+    else:
+        click.echo("Result:")
+        click.echo(result)
+
+
 def _print_summary(job: "Job", options) -> str:
     jsonSummary: Any = {}
     text = ""
     summary = options.get("output")
     if summary == "text" and not job.jobOptions.planOnly:
         text = job.print_summary_table()
     elif summary == "json":
@@ -466,19 +475,15 @@
     query = options.get("query")
     if query:
         result = job.run_query(query, options.get("trace"))
         if summary == "json":
             jsonSummary["query"] = query
             jsonSummary["result"] = result
         else:
-            click.echo("query: " + query)
-            if result is None:
-                click.echo("No results found")
-            else:
-                click.echo(result)
+            _print_query(query, result)
     if jsonSummary:
         text = json.dumps(jsonSummary, indent=2)
         click.echo(text)
     return text
 
 
 def yesno(prompt):
@@ -1209,26 +1214,21 @@
         options.get("home"),
         override_context=options.get("use_environment") or "",
         readonly=True,
     )
     logger = logging.getLogger("unfurl")
     manifest = localEnv.get_manifest()
     summary = manifest.status_summary()
-    click.echo(summary)
-    logger.debug("Status summary:\n%s", summary)
+    logger.info("Status summary:\n%s", summary, extra=dict(truncate=0))
     query = options.get("query")
     if query:
         trace = options.get("trace")
         assert manifest.rootResource
         result = manifest.rootResource.query(query, trace=trace)
-        click.echo("query: " + query)
-        if result is None:
-            click.echo("No results found")
-        else:
-            click.echo(result)
+        _print_query(query, result)
 
 
 @cli.command()
 @click.pass_context
 @click.argument("ensemble", default=".", type=click.Path(exists=False))
 def validate(ctx, ensemble, **options):
     """Validate the given ensemble."""
@@ -1309,30 +1309,32 @@
     "--cors",
     envvar="UNFURL_SERVE_CORS",
     help='enable CORS with origin (e.g. "*")',
 )
 def serve(
     ctx, port, address, secret, clone_root, project_or_ensemble_path, cors, **options
 ):
+    """Run unfurl as a server."""
     options.update(ctx.obj)
     # env vars need to set before importing serve
     if cors:
         os.environ["UNFURL_SERVE_CORS"] = cors
     os.environ["UNFURL_SERVE_PATH"] = project_or_ensemble_path
     os.environ["UNFURL_CLONE_ROOT"] = clone_root
     from .server import serve as _serve
 
     _serve(address, port, secret, clone_root, project_or_ensemble_path, options)
 
 
 @cli.command(short_help="Manage a cloud map")
 @click.pass_context
 @click.argument("cloudmap", default="cloudmap")
-@click.option("--sync", default=None, help='Sync the given repository host ("local", name or url).')
-@click.option("--import", default=None, help='Update the cloudmap with the given repository host ("local", name or url).')
+@click.option("--sync", default=None, help='Sync the given repository host ("local", name, or url).')
+@click.option("--import", default=None, help='Update the cloudmap with the given repository host ("local", name, or url).')
+@click.option("--export", default=None, help='Update the given repository host ("local", name, or url) with the local repositories recorded in the cloudmap.')
 @click.option(
     "--namespace",
     default=None,
     help="Limit sync to the given repositories that match the given pattern.",
 )
 @click.option(
     "--clone-root",
@@ -1346,50 +1348,74 @@
 )
 @click.option(
     "--project",
     type=click.Path(exists=True),
     default=".",
     help='Unfurl project to use. (Default: ".")',
 )
+@click.option(
+    "--skip-analysis",
+    default=False,
+    is_flag=True,
+    help="Don't analyze files in repositories",
+)
+@click.option(
+    "--force",
+    default=False,
+    is_flag=True,
+    help="Force push to repository host",
+)
+@click.option(
+    "--dryrun",
+    default=False,
+    is_flag=True,
+    help="Do not modify the repository host, just do a dry run.",
+)
 def cloudmap(
     ctx,
     cloudmap: str,
     sync: str,
     project: str,
     namespace: Optional[str] = None,
     clone_root: Optional[str] = None,
     visibility: Optional[str] = None,
+    skip_analysis: bool = False,
+    force: bool = False,
+    dryrun: bool = False,
     **options,
 ):
     """Manage a cloud map.
 
     [CLOUDMAP] is either a named cloudmap, a git url, or a local path.
     (Default: "cloudmap")
     """
     from .cloudmap import CloudMap
 
     options.update(ctx.obj)
     localEnv = LocalEnv(project, options.get("home"), can_be_empty=True, readonly=True)
+    # --sync, --import, --export set the name of the repository host
+    host_name = sync or options.get("import", "") or options.get("export", "")
+    if not host_name:
+        print("nothing to do for (use one of --export, --import, or --sync)", cloudmap)
+        return
     cloud_map = CloudMap.from_name(
-        localEnv, cloudmap, clone_root or "", sync, namespace or ""
+        localEnv, cloudmap, clone_root or "", host_name, namespace or "", skip_analysis
     )
-    if sync:
-        # sync is the provider name
-        cloud_map.sync(cloud_map.get_host(localEnv, sync, namespace or "", visibility))
-    elif options.get("import"):
-        host = cloud_map.get_host(localEnv, options.get("import") or "", namespace or "", visibility)
-        host.from_host(cloud_map.directory)
-        cloud_map.save(
-            f"Update cloudmap with latest from {'/'.join([host.name, host.path])}"
-        )
+    host = cloud_map.get_host(localEnv, host_name, namespace or "", visibility)
+    host.dryrun = dryrun
+    if options.get("import") or sync:
+        changed = cloud_map.from_host(host)
+    else:
+        changed = False
+    if options.get("export") or sync:
+        cloud_map.to_host(host, changed, force)
+
     # elif clone_root:
     #     cloud_map = CloudMap.from_name(localEnv, cloudmap, "local")
     #     cloud_map.from_provider(namespace, download)
-    else:
-        print("nothing to do for", cloud_map)
 
 
 def main():
     obj = {"standalone_mode": False}
     try:
         rv = cli(standalone_mode=False, obj=obj)
         sys.exit(rv or 0)
```

### Comparing `unfurl-0.6.2/unfurl/cloudmap.py` & `unfurl-0.7.0/unfurl/cloudmap.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,54 +6,73 @@
 
 You can use a cloud map to manage servers that host git repositories and synchronize mirrors of git repositories.
 Three types of repository hosts are currently supported: local, gitlab, and unfurl.cloud
 For example, the following commands can be used push projects on a staging instance to production:
 
 ```bash
 # sync latest in staging with the cloudmap
-unfurl cloudmap --sync staging --namespace onecommons/blueprint --namespace onecommons/blueprints
+unfurl cloudmap --sync staging --namespace onecommons/blueprints
 
 # now sync the cloudmap with production
 unfurl cloudmap --sync production --namespace onecommons/blueprints
 
 # only push the main branch to the public repo
 git --push origin main
 ```
 """
 
 import collections
 from dataclasses import dataclass, field, asdict
 from io import StringIO
+from operator import attrgetter
 from pathlib import Path
 import tempfile
 import os
 import os.path
-from typing import Any, Iterator, Optional, List, Dict, Tuple, cast
+from typing import (
+    Any,
+    Iterator,
+    Optional,
+    List,
+    Dict,
+    Sequence,
+    Set,
+    Tuple,
+    Type,
+    TypeVar,
+    cast,
+)
 import logging
 from urllib.parse import urljoin, urlparse
 import git
 import git.cmd
+from git.objects import IndexObject
 import gitlab
 from gitlab.v4.objects import Project, Group, ProjectTag, ProjectBranch
-from ruamel.yaml import YAML
 
-from .repo import GitRepo, is_git_worktree, normalize_git_url, split_git_url
+from .tosca import NodeSpec, ToscaSpec
 
-from .util import UnfurlError
+from .support import ContainerImage
 
+from .to_json import blueprint_metadata
+from .repo import (
+    GitRepo,
+    is_git_worktree,
+    normalize_git_url,
+    sanitize_url,
+    split_git_url,
+)
+from .util import UnfurlError
 from .localenv import LocalEnv
-
 from .yamlloader import YamlConfig, urlopen as _urlopen
-
 from .logs import getLogger
+from . import DefaultNames
 
 logger = getLogger("unfurl")
 
-yaml = YAML()
-
 
 # Data classes
 @dataclass
 class Namespace:
     name: str
     path: str
     url: str
@@ -110,14 +129,15 @@
     metadata: RepositoryMetadata = field(default_factory=RepositoryMetadata)
     mirror_of: Optional[str] = None
     fork_of: Optional[str] = None
     private: Optional[bool] = None
     default_branch: str = ""
     branches: Dict[str, str] = field(default_factory=dict)
     tags: Dict[str, str] = field(default_factory=dict)
+    notable: Dict[str, dict] = field(default_factory=dict)
 
     def __post_init__(self):
         if isinstance(self.metadata, dict):
             self.metadata = RepositoryMetadata(**self.metadata)
 
     def get_metadata(self, directory: "RepositoryDict") -> dict:
         if self.mirror_of and self.mirror_of in directory:
@@ -163,157 +183,476 @@
     # match url and path?
     # def get_namespace(self, directory) -> Optional[Namespace]:
     #     path.split("/")
 
     def update_branch(self, repo: GitRepo, branch: str = "main"):
         self.branches[branch] = repo.revision
 
+    def add_notables(self, notables: List["Notable"]) -> None:
+        notables.sort(key=attrgetter("path"))
+        self.notable = {n.path: n.asdict() for n in notables}
+
+    def get_default_branch(self):
+        return self.default_branch or "main"
+
+
+ArtifactDict = Dict[str, dict]
+
 
 RepositoryDict = Dict[str, Repository]
 
 
 def find_git_repos(rootDir, gitDir=".git") -> Iterator[str]:
     for root, dirs, files in os.walk(rootDir):
         if gitDir in dirs and is_git_worktree(root, gitDir):
             del dirs[:]  # don't visit sub directories
             yield os.path.abspath(root)
 
 
 def force_merge_local_and_push_to_remote(
     repo: GitRepo, remote_name: str, dest_branch: str, merge=False, force=False
-):
-    """Update existing project repo with changes from upstream and"""
+) -> None:
+    """Make the remote repo match the local repo using force push or merge "ours" strategy."""
     if merge:
+        assert not force  # why do you want to do both?
         # merge the remote branch into the current local HEAD
         # Use "ours" merge strategy so the resulting tree of the merge is always that of the current branch head, effectively
         # ignoring all changes from all other branches.
         # This creates a merge commit equivalent to a force push without rewriting history
-        repo.repo.git.merge(dest_branch, s="ours")
+        repo.repo.git.merge(
+            dest_branch, s="ours", m=f"set {dest_branch} to {repo.repo.active_branch}"
+        )
 
     # push local HEAD to remote "main" branch
     # skip the pipeline because that might cause additional commits
-    pushinfo = repo.repo.remotes[remote_name].push(
-        o="ci.skip", follow_tags=True, force=force
-    )[0]
-    logger.info(f"pushed to {repo.safe_url}: {pushinfo.summary}")
+    remote = repo.repo.remotes[remote_name]
+    pushinfolist = remote.push(o="ci.skip", follow_tags=True, force=force)
+    pushinfo = pushinfolist[0]
+    if pushinfolist.error:
+        logger.error(f"pushed to {sanitize_url(remote.url, True)} failed: {pushinfo.summary}")
+    else:
+        logger.info(f"pushed to {sanitize_url(remote.url, True)}: {pushinfo.summary}")
+
+
+T = TypeVar("T", bound="Notable")
+
+
+class EntitySchema:
+    Schema = "unfurl.cloud/onecommons/unfurl-types"
+    GenericFile = "artifact.File"
+    ContainerFile = "artifact.Containerfile"
+    CloudBlueprint = "artifact.tosca.ServiceTemplate"
+    TOSCASchema = "artifact.tosca.TypeLibrary"
+    Ensemble = "artifact.tosca.UnfurlEnsemble"
+    UnfurlProject = "artifact.tosca.UnfurlProject"
+    OCIImage = "artifacts.OCIImage"
+
+
+class Notable:
+    files: Sequence[str] = ()
+    folders: Sequence[str] = ()
+    artifact_type = EntitySchema.GenericFile
+
+    def __init__(self, root_path: str, folder: str, file: str):
+        self.root_path = root_path
+        self.folder = folder
+        self.file = file
+        self.metadata: Dict[str, Any] = {}
+        self.artifacts: List[ArtifactDict] = []
+
+    @property
+    def path(self) -> str:
+        if self.file:
+            return os.path.join(self.folder, self.file)
+        else:
+            return self.folder
+
+    @property
+    def full_path(self) -> str:
+        return os.path.join(self.root_path, self.folder, self.file)
+
+    @classmethod
+    def _exist_in_folder(cls, folder: str, notables: List["Notable"]):
+        for n in notables:
+            if cls is n.__class__ and n.folder == folder:
+                return True
+        return False
+
+    @classmethod
+    def init(cls: Type[T], root_path: str, folder: str, file: str) -> Optional[T]:
+        return cls(root_path, folder, file)
+
+    def asdict(self) -> Dict[str, Any]:
+        metadata = dict(artifact_type=self.artifact_type)
+        metadata.update(filter_dict(self.metadata))
+        return metadata
+
+
+class ContainerBuilderNotable(Notable):
+    files = ("Containerfile", "Dockerfile")
+    artifact_type = EntitySchema.ContainerFile
+
+    def __init__(self, root_path: str, folder: str, file: str):
+        super().__init__(root_path, folder, file)
+
+
+class UnfurlNotable(Notable):
+    files = [
+        DefaultNames.LocalConfig,
+        DefaultNames.EnsembleTemplate,
+        DefaultNames.Ensemble,
+        "dummy-ensemble.yaml",  # DefaultNames.ServiceTemplate,  # XXX fix unfurl-types hack
+    ]
+    folders = [DefaultNames.ProjectDirectory, DefaultNames.EnsembleDirectory]
+
+    def __init__(self, root_path: str, folder: str, file: str):
+        super().__init__(root_path, folder, file)
+        # XXX set readonly=True after adding representers for AnsibleUnicode etc.
+        localenv = LocalEnv(
+            self.full_path,
+            can_be_empty=True,
+        )
+        if localenv.manifestPath:
+            self.artifact_type = self._get_artifacttype(localenv.manifestPath)
+            manifest = localenv.get_manifest()
+            rel_path = str(
+                Path(localenv.manifestPath).relative_to(Path(self.root_path))
+            )
+            self.folder, self.file = os.path.split(rel_path)
+            spec = manifest.tosca
+            assert spec
+            assert spec.template
+            metadata = spec.template.tpl.get("metadata") or spec.template.tpl or {}
+            self.metadata.update(
+                dict(
+                    name=metadata.get("template_name"),
+                    version=metadata.get("template_version"),
+                    description=spec.template.description,
+                )
+            )
+            node = self._get_root_node(spec)
+            schema_repo = manifest.repositories.get("types")
+            if schema_repo:
+                self.metadata["schema"] = schema_repo.url.strip(":")
+            if node:
+                self.metadata.update(
+                    dict(
+                        type=node.type,
+                        dependencies=list(self.find_dependencies(node).values()),
+                    )
+                )
+                image_name = self.find_image_dependency(node)
+                if image_name:
+                    self.artifacts.append(
+                        {image_name: dict(type=EntitySchema.OCIImage)}
+                    )
+                    self.metadata["artifacts"] = [image_name]
+        else:
+            self.artifact_type = EntitySchema.UnfurlProject
+
+    @classmethod
+    def init(cls, root_path: str, folder: str, file: str) -> Optional["UnfurlNotable"]:
+        try:
+            return UnfurlNotable(root_path, folder, file)
+        except UnfurlError:
+            return None
+
+    def find_dependencies(self, node: NodeSpec):
+        return {
+            name: req.get("node")
+            for name, req in node.toscaEntityTemplate.missing_requirements.items()
+        }
+
+    def find_image_dependency(self, node: NodeSpec):
+        container_service = node.get_relationship("container")
+        if container_service and container_service.target:
+            image = container_service.target.properties.get("container", {}).get(
+                "image"
+            )
+            if image:
+                name, tag, digest, hostname = ContainerImage.split(image)
+                return os.path.join(hostname or "docker.io", name or "")
+        return None
+
+    def _get_artifacttype(self, path: str) -> str:
+        if path.endswith(DefaultNames.EnsembleTemplate):
+            return EntitySchema.CloudBlueprint
+        elif path.endswith("dummy-ensemble.yaml"):
+            return EntitySchema.TOSCASchema
+        else:
+            return EntitySchema.Ensemble
+
+    def _get_root_node(self, spec: ToscaSpec) -> Optional[NodeSpec]:
+        topology = spec.template.topology_template
+        node = topology.substitution_mappings and topology.substitution_mappings.node
+        if node:
+            assert spec.topology
+            return spec.topology.get_node_template(node)
+        return None
+
+
+class Analyzer:
+    max_analyze_depth = 4
+
+    def __init__(self, notables: List[Type[Notable]]):
+        self.files: Dict[str, Type[Notable]] = {}
+        self.folders: Dict[str, Type[Notable]] = {}
+        for n in notables:
+            self.add_notable_class(n)
+
+    def add_notable_class(self, cls: Type[Notable]):
+        for file in cls.files:
+            self.files[file] = cls
+        for folder in cls.folders:
+            self.folders[folder] = cls
+
+    def analyze_local(self, rootDir) -> List[Notable]:
+        notables: List[Notable] = []
+        for root, dirs, files in os.walk(rootDir):
+            notable = None
+            notable_cls = None
+            notables_found: List[Type[Notable]] = []
+            rel_root = str(Path(root).relative_to(Path(rootDir)))
+            for folder in dirs:
+                notable_cls = self.folders.get(folder)
+                if notable_cls:
+                    if notable_cls not in notables_found:
+                        notable = notable_cls.init(rootDir, rel_root, "")
+                if notable:
+                    dirs.remove(folder)  # don't visit folder
+            for filename in files:
+                notable_cls = self.files.get(filename)
+                if notable_cls and notable_cls not in notables_found:
+                    notable = notable_cls.init(rootDir, rel_root, filename)
+            if notable:
+                notables.append(notable)
+                assert notable_cls
+                notables_found.append(notable_cls)
+        return notables
+
+    def analyze_repo_tree(
+        self,
+        root_path: str,
+        children: List[IndexObject],
+        notables: List[Notable],
+        depth=-1,
+    ):
+        descend: List[IndexObject] = []
+        if depth > self.max_analyze_depth:
+            return descend
+        notables_found: List[Type[Notable]] = []
+        for item in children:
+            notable = None
+            notable_cls = None
+            dirname, filename = os.path.split(item.path)
+            if item.type == "tree":
+                notable_cls = self.folders.get(filename)
+                if notable_cls:
+                    if notable_cls not in notables_found:
+                        notable = notable_cls.init(root_path, cast(str, item.path), "")
+                else:
+                    descend.append(item)
+            elif item.type == "blob":
+                notable_cls = self.files.get(filename)
+                if notable_cls and notable_cls not in notables_found:
+                    notable = notable_cls.init(root_path, dirname, filename)
+            if notable:
+                notables.append(notable)
+                assert notable_cls
+                notables_found.append(notable_cls)
+        return descend
 
 
 class _LocalGitRepos:
     def __init__(self, local_repo_root: str = "") -> None:
         self._set_repos(os.path.expanduser(local_repo_root))
 
-    @staticmethod
-    def _add_repo(working_dir: str, repos: Dict[str, GitRepo]):
-        repo = GitRepo(git.Repo(working_dir))
+    def _add_repo(self, working_dir: str) -> Optional[GitRepo]:
+        gitrepo = git.Repo(working_dir)
+        repo = GitRepo(gitrepo)
         if not repo.remote:
             logger.debug(f"skipping git repo in {working_dir}: no remote set")
         else:
-            # XXX get all remotes
-            if "canonical" in repo.repo.remotes:
-                remote_url = repo.repo.remotes["canonical"].url
-            else:
-                remote_url = repo.remote.url
-            url = get_remote_git_url(remote_url)
-            if url:
+            for remote in gitrepo.remotes:
+                if not remote.url:
+                    continue
+                url = get_remote_git_url(remote.url)
+                self.remotes.setdefault(url, []).append(remote)
                 logger.debug(f"found git repo {url} in {working_dir}")
-                repos[url] = repo
-                return repo
-            else:
-                logger.debug(f"skipping git repo in {working_dir}: no remote set")
+            self.repos[working_dir] = repo
         return None
 
-    def _set_repos(self, root: str):
-        repos: Dict[str, GitRepo] = {}
+    def _set_repos(self, root: str) -> None:
+        # note: there can be a many to many relationship between upstream and local repos
+        # url => remotes
+        self.remotes: Dict[str, List[git.Remote]] = {}
+        # working_dir => repo
+        self.repos: Dict[str, GitRepo] = {}
         logger.debug(f"looking for repos in {root}")
         if root:
             for working_dir in find_git_repos(root):
-                self._add_repo(working_dir, repos)
-        self.repos = repos
+                self._add_repo(working_dir)
         self.repos_root = root
 
+    @staticmethod
+    def _choose_remote(remotes: List[git.Remote], hint: str):
+        host = origin = canonical = None
+        for remote in remotes:
+            if remote.name == hint:
+                host = remote
+            elif remote.name == "origin":
+                origin = remote
+            elif remote.name == "canonical":
+                canonical = remote
+        # find best candidate
+        return origin or host or canonical or remotes[0]
+
+    def find_repo(self, url: str, hint: str) -> Optional[GitRepo]:
+        remotes = self.remotes.get(get_remote_git_url(url))
+        if remotes:
+            # find best candidate
+            remote = self._choose_remote(remotes, hint)
+            return self.repos[cast(str, remote.repo.working_tree_dir)]
+        return None
+
 
 class Directory(_LocalGitRepos):
     """
     Loads and saves a yaml file
     """
 
     DEFAULT_NAME = "cloudmap.yml"
 
-    def __init__(self, path=".", local_repo_root: str = "") -> None:
+    def __init__(
+        self, path=".", local_repo_root: str = "", skip_analysis=False
+    ) -> None:
+        self.do_analysis = not skip_analysis
         self._load(path)
         self.tmp_dir: Optional[tempfile.TemporaryDirectory] = None
         super().__init__(local_repo_root)
+        self.analyzer = Analyzer([UnfurlNotable, ContainerBuilderNotable])
 
     def _load(self, path: str):
         if os.path.isdir(path):
             path = os.path.join(path, self.DEFAULT_NAME)
         default_db = dict(apiVersion="unfurl/v1alpha1", kind="CloudMap")
         self.config = YamlConfig(
             default_db,
             path,
             # validate,
             # os.path.join(_basepath, "cloudmap-schema.json"),
         )
         db = self.config.config
-        repositories = cast(Dict, db and db.get("repositories") or {})
+        assert isinstance(db, dict)
+        repositories = cast(Dict, db.get("repositories") or {})
         self.repositories: RepositoryDict = {
             url: Repository(**r) for url, r in repositories.items()
         }
+        self.artifacts: ArtifactDict = db.get("artifacts") or {}
         self.db = cast(Dict[str, Any], db)
 
     def reload(self):
         assert self.config.path
         self._load(self.config.path)
 
-    def find_local_repos_for_host(self, host: "RepositoryHost"):
-        """for each repo that matches host.host and host.namespace, check that HEAD matches the repository entry"""
-        for url, repo in self.repos.items():
+    def find_local_repos_for_host(
+        self, host: "RepositoryHost"
+    ) -> Iterator[Tuple[git.Remote, GitRepo, Repository]]:
+        """for each repo that matches host.host and host.namespace, yield matching remote and Repository"""
+        for url, remotes in self.remotes.items():
             repo_info = self.repositories.get(url)
             if repo_info and host.has_repository(repo_info):
-                yield repo, repo_info
+                remote = self._choose_remote(remotes, host.name)
+                working_dir = cast(str, remote.repo.working_tree_dir)
+                yield remote, self.repos[working_dir], repo_info
 
     def find_mismatched_repo(self, host: "RepositoryHost") -> Optional[GitRepo]:
-        for repo, repo_info in self.find_local_repos_for_host(host):
+        for remote, repo, repo_info in self.find_local_repos_for_host(host):
             if repo.revision != repo_info.branches["main"]:
                 return repo
         return None
 
-    def merge(self, host: "RepositoryHost"):
-        """For each git repo that has a branch for the repository host, merge it into main"""
-        host_branch = f"{host.name}/main"
-        for repo in self.repos.values():
-            if host_branch in repo.repo.branches:  # type: ignore
-                repo.repo.git.merge(host_branch)
+    def merge_from_host(self, host: "RepositoryHost") -> None:
+        """For each local repo that has a remote that matches the repository host, pull the default branch."""
+        for remote, repo, repo_info in self.find_local_repos_for_host(host):
+            default_branch = repo_info.get_default_branch()
+            host_branch = f"{remote.name}/{default_branch}"
+            if host_branch in remote.repo.git.branch(r=True).split():
+                remote.repo.git.checkout(default_branch, with_exceptions=True)
+                # should be a ff merge
+                remote.repo.git.merge(host_branch, ff_only=True, with_exceptions=True)
 
     def ensure_local(self):
         if not self.repos_root:
             self.tmp_dir = tempfile.TemporaryDirectory(prefix="oc-repo-update-")
             self.repos_root = self.tmp_dir.name
             logger.debug(f"setting {self.tmp_dir.name} as repo_root")
 
     def cleanup_local(self):
         if self.tmp_dir:
             self.tmp_dir.cleanup()
 
     def save(self):
         # maintain order of repositories so git merge is effective
         # we want to support mirrors
+        self.db["schema"] = EntitySchema.Schema
         self.db["repositories"] = {
             k: self.repositories[k].asdict() for k in sorted(self.repositories)
         }
+        self.db.pop("artifacts", None)
+        if self.artifacts:
+            self.db["artifacts"] = {
+                a: self.artifacts[a] for a in sorted(self.artifacts)
+            }
         self.config.save()
 
-    def find_repo(self, url: str) -> Optional[GitRepo]:
-        return self.repos.get(get_remote_git_url(url))
-
     def clone_repo(self, repo_info: Repository, url: str) -> GitRepo:
         download_path = str(Path(self.repos_root) / repo_info.path)
         repo = git.Repo.clone_from(url or repo_info.git_url(), download_path)
         return GitRepo(repo)
 
+    def analyze_repo(self, repo: GitRepo) -> List[Notable]:
+        notables: List[Notable] = []
+
+        root = repo.repo.head.commit.tree
+        items = [root]
+        seen = set()
+        while items:
+            item = items.pop(0)
+            # sort so blobs are before trees
+            children = sorted(
+                root._get_intermediate_items(item), key=attrgetter("type")
+            )
+            # analyze return trees to descend into
+            # XXX track and pass depth argument
+            for tree in self.analyzer.analyze_repo_tree(
+                repo.working_dir, children, notables
+            ):
+                if tree.type == "tree" and tree not in seen:
+                    items.append(tree)
+                    seen.add(tree)
+        return notables
+
+    def maybe_analyze(
+        self, repo_info: Repository, repo: GitRepo, previous_notables: dict
+    ) -> Optional[List[Notable]]:
+        if self.do_analysis:
+            return self.analyze(repo_info, repo)
+        else:  # preserve previous analysis
+            repo_info.notable = previous_notables
+        return None
+
+    def analyze(self, repo_info: Repository, repo: GitRepo) -> List[Notable]:
+        notables = self.analyze_repo(repo)
+        repo_info.add_notables(notables)
+        for n in notables:
+            for a in n.artifacts:
+                self.artifacts.update(a)
+        return notables
+
 
 def get_remote_git_url(url):
     """Return the location of the git server without the scheme or user"""
     parts = urlparse(url)
     if not parts.netloc and not parts.scheme and "@" in url:
         # scp style used by git: user@server:project.git
         parts = urlparse("ssh://" + url.replace(":", "/", 1))
@@ -323,14 +662,15 @@
     return url
 
 
 class RepositoryHost:
     name: str = ""
     path: str = ""
     canonical_url: str = ""
+    dryrun: bool = False
 
     def has_repository(self, repo_info: Repository) -> bool:
         return False
 
     def from_host(self, directory: Directory):
         """
         Update the directory with latest from this host.
@@ -347,23 +687,30 @@
         """
         return False
 
     def fetch_repo(
         self, push_url: str, dest: Repository, local: "Directory"
     ) -> GitRepo:
         # add remote for target repo
-        repo = local.find_repo(push_url)
+        repo = local.find_repo(push_url, self.name)
         if not repo:
-            repo = local.find_repo(dest.git)
+            repo = local.find_repo(dest.git, self.name)
         if not repo:
             repo = local.clone_repo(dest, push_url)
+        remote_name = self.name or "origin"
         try:
-            dest_remote = repo.repo.remote(self.name or "origin")
+            dest_remote = repo.repo.remote(remote_name)
         except ValueError:
-            dest_remote = git.Remote.create(repo.repo, self.name or "origin", push_url)
+            dest_remote = git.Remote.create(repo.repo, remote_name, push_url)
+        else:
+            if normalize_git_url(dest_remote.url) != normalize_git_url(dest.git_url()):
+                logger.warning(
+                    f"{dest_remote.url} doesn't match {dest.git_url()} for remote '{remote_name}' in {repo.working_dir}"
+                )
+                # XXX should we set the url?
         if self.canonical_url and push_url != dest.git_url():
             # add a remote so we can match this repository with mirror hosts
             canonical_remote_name = "canonical"
             try:
                 canonical_remote = repo.repo.remote(canonical_remote_name)
                 if canonical_remote.url != dest.git_url():
                     logger.warning(
@@ -377,40 +724,45 @@
 
 class LocalRepositoryHost(RepositoryHost, _LocalGitRepos):
     """
     Locally manage git repositories from any origin using the git protocol.
     """
 
     def has_repository(self, repo_info: Repository) -> bool:
-        return repo_info.git in self.repos
+        return repo_info.git in self.remotes
 
     def include_local_repo(self, repo: GitRepo) -> bool:
         return bool(repo.remote)  # XXX check host and namespace filters too
 
     def from_host(self, directory: Directory):
         """Pull latest and update the cloudmap to match the local repositories."""
-        for url, repo in self.repos.items():
+        for repo in self.repos.values():
             if self.include_local_repo(repo):
                 repo.pull()  # XXX make optional?
                 assert repo.repo.working_dir
                 path = str(
                     Path(repo.repo.working_dir).relative_to(
                         Path(os.path.abspath(self.repos_root))
                     )
                 )
                 repository = self.git_to_repository(repo, path)
+                previous = directory.repositories.get(repository.key)
                 directory.repositories[repository.key] = repository
+                directory.maybe_analyze(
+                    repository, repo, previous.notable if previous else {}
+                )
 
     def to_host(self, directory: Directory, merge: bool, force: bool) -> bool:
         """Push cloudmap revisions to origin."""
         matched = False
-        for url, repo in self.repos.items():
+        for repo in self.repos.values():
             if self.include_local_repo(repo):
-                if directory.repos_root and self.repos_root != directory.repos_root:
-                    cloudmap_local_repo = directory.repos.get(url)
+                # if we're looking at different local clones than the cloudmap's
+                if self.repos_root != directory.repos_root:
+                    cloudmap_local_repo = directory.find_repo(repo.url, self.name)
                     if cloudmap_local_repo:
                         repo.pull(cloudmap_local_repo.working_dir)
                 repo.push()
                 matched = True
         return matched
 
     @staticmethod
@@ -493,21 +845,40 @@
     def _import_projects_from_host(self, projects, directory: Directory):
         # XXX delete removed projects
         repositories = directory.repositories
         for p in projects:
             dest_proj: Project = self.gitlab.projects.get(p.id)
             if self.visibility == "public" and dest_proj.visibility != "public":
                 continue
+            try:
+                dest_proj.default_branch
+            except AttributeError:
+                # project without repositories will throw error, skip those
+                logger.warning(
+                    f"skipping project {dest_proj.web_url}, it doesn't have a git repository"
+                )
+                continue
             r = self.gitlab_project_to_repository(dest_proj)
+
+            previous = repositories.get(r.key)
             repositories[r.key] = r
             if directory.repos_root:
                 # add remote branches to local repository
                 # XXX pull mirror = True and merge all branches not just main?
                 remote_url = self.git_url_with_auth(dest_proj)
-                self.fetch_repo(remote_url, r, directory)
+                repo = self.fetch_repo(remote_url, r, directory)
+                directory.maybe_analyze(r, repo, previous.notable if previous else {})
+
+    def _get_projects_from_group(self, group, projects):
+        for p in group.projects.list(iterator=True):
+            projects[p.path_with_namespace][0] = p  # type: ignore
+        for subgroup in group.subgroups.list(iterator=True):
+            self._get_projects_from_group(
+                self.gitlab.groups.get(subgroup.id), projects
+            )
 
     def to_host(self, directory: Directory, merge: bool, force: bool) -> bool:
         """
         Create or update projects in a gitlab instance.
         If the target project has changed, update the records.
 
         If merge is True and there a local repositories associate with the directory,
@@ -523,92 +894,118 @@
         dest_path = self.path
         logger.info(f"syncing to {dest_path}")
         if not repositories:
             logger.info("no matches")
             return False
 
         dest_group = self.ensure_group(dest_path)
+        if not dest_group:
+            logger.info("%s doesn't exist", dest_path)
+            return False
         # XXX look up Namespace and sync it?
 
         projects = cast(
             Dict[str, Tuple[Optional[Project], Optional[Repository]]],
             collections.defaultdict(lambda: [None, None]),
         )
-        for p in dest_group.projects.list(iterator=True):
-            projects[p.path_with_namespace][0] = p  # type: ignore
+        self._get_projects_from_group(dest_group, projects)
         for r in repositories:
             projects[r.path][1] = r  # type: ignore
 
         for name in projects:
             dest, repo_info = projects[name]
             if repo_info:
                 if dest:
                     # if both exist, update any changed metadata
-                    self.update_project_metadata(repo_info, dest)
-                    do_merge = merge
+                    if self.dryrun:
+                        logger.info("dry run: skipping creating updating project %s", name)
+                    else:
+                        self.update_project_metadata(repo_info, dest)
+                    do_merge = not force and merge
                 else:
+                    if self.dryrun:
+                        logger.info("dry run: skipping creating project %s", name)
+                        continue
                     # create the project
                     dest = self.create_project(repo_info, dest_group)
                     do_merge = False
                 assert dest
                 if directory.repos_root:
                     remote_url = self.git_url_with_auth(dest)
-                    repo = directory.find_repo(dest.http_url_to_repo)
+                    repo = directory.find_repo(dest.http_url_to_repo, self.name)
                     if not repo:
-                        repo = directory.find_repo(repo_info.git)
+                        repo = directory.find_repo(repo_info.git, self.name)
                     if repo:
-                        # now update project repository
-                        logger.info(
-                            f"{force and '(force) ' or ' '}{do_merge and 'merging' or 'pushing'} local repository to {repo.safe_url}"
-                        )
                         # there's a local mirror that might have changed
                         try:
                             repo = self.fetch_repo(remote_url, repo_info, directory)
                             # clone source repo and push to dest
-                            dest_branch = f"{self.name}/main"
-                            force_merge_local_and_push_to_remote(
-                                repo,
-                                self.name,
-                                dest_branch,
-                                merge=do_merge,
-                                force=force,
+                            dest_branch = (
+                                f"{self.name}/{repo_info.get_default_branch()}"
                             )
-                            if do_merge:
-                                # we might have create a merge commit, update the directory
-                                repo_info.update_branch(repo, "main")
+                            commit = repo.repo.head.commit
+                            branch_exists = dest_branch in repo.repo.references
+                            if not branch_exists or commit != repo.repo.references[dest_branch].commit:
+                                # now update project repository
+                                logger.info(
+                                    f"{force and '(force) ' or ' '}{do_merge and 'merging' or 'pushing'} local repository to {repo.safe_url}"
+                                )
+                                if self.dryrun:
+                                    summary = cast(str, commit.summary)
+                                    logger.info(
+                                        f"dry run: would have pushed commit {commit.hexsha[:6]} {commit.committed_datetime} {summary}"
+                                    )
+                                else:
+                                    force_merge_local_and_push_to_remote(
+                                        repo,
+                                        self.name,
+                                        dest_branch,
+                                        merge=branch_exists and do_merge,
+                                        force=force,
+                                    )
+                                if do_merge:
+                                    # we might have create a merge commit, update the directory
+                                    repo_info.update_branch(repo, "main")
+                            else:
+                                logger.debug(
+                                    f"skipping push: no change detected on branch {dest_branch} for {repo.safe_url}"
+                                )
                         except Exception:
                             logger.error(
                                 f"Unexpected error updating upstream git for {repo_info.git}",
                                 exc_info=True,
                             )
             # delete any extra projects
             # XXX: enable when ready
             if not repo_info and dest:
                 logger.info(f"would delete {dest_path}")
                 # full_proj = staging_gitlab.projects.get(staging.id)
                 # full_proj.delete()
         return True
 
     def git_url_with_auth(self, project: Project) -> str:
-        return f"https://{self.user}:{self.token}@{project.http_url_to_repo.lstrip('https://')}"
+        scheme, sep, url = project.http_url_to_repo.rpartition("://")
+        return f"{scheme}://{self.user}:{self.token}@{url}"
 
     # only fetch group, don't create it
     def _get_group(self, path: str) -> Optional[Group]:
         try:
             return cast(Group, self.gitlab.groups.get(path))
         except Exception:
             return None
 
-    def ensure_group(self, path: str) -> Group:
+    def ensure_group(self, path: str) -> Optional[Group]:
         """Get or create the given group in the Gitlab instance"""
         gitlab = self.gitlab
         logger.info(f"ensuring group {path} on {gitlab.url}")
 
         # see if group exists first
         group = self._get_group(path)
+        if self.dryrun:
+            return group
 
         # create if missing
         if group is None:
             parent = None
             path_so_far = []
 
             for name in path.split("/"):
@@ -628,19 +1025,20 @@
                     group = self.gitlab.groups.get(full_path)
 
                 parent = group
         assert group
         return group
 
     def create_project(self, repo_info: Repository, dest_group: Group) -> Project:
-        logger.info(f"  creating {repo_info.path}")
+        logger.info(f"creating project {repo_info.path}")
 
-        project_path, namespace = os.path.split(repo_info.path)
+        namespace, project_path = os.path.split(repo_info.path)
         if namespace != self.path:
-            dest_group = self.ensure_group(namespace)
+            dest_group = self.ensure_group(namespace)  # type: ignore
+            assert dest_group
         proj_data = {
             "name": repo_info.name,
             "path": project_path,
             "namespace_id": dest_group.id,
             "description": repo_info.metadata.description,
             "topics": repo_info.metadata.topics,
             "default_branch": repo_info.default_branch,
@@ -685,16 +1083,16 @@
             return url
 
     def gitlab_project_to_repository(self, project: Project) -> Repository:
         kw = {}
         # XXX
         # if project.license:
         #    kw["license"] = project.license.key in spdx_ids # or nickname or name
-        if project.avatar_url:
-            kw["avatar_url"] = self.canonize(project.avatar_url)
+        # if project.avatar_url:
+        #     kw["avatar_url"] = project.avatar_url
         if project.issues_enabled:
             kw["issues_url"] = self.canonize(project.web_url + "/-/issues")
 
         # https://docs.gitlab.com/ee/api/projects.html#get-single-project
         metadata = RepositoryMetadata(
             description=project.description,
             topics=project.topics,
@@ -711,15 +1109,15 @@
         repository = Repository(
             initial_revision="",  # XXX
             git=git_url,
             name=project.name,
             protocols=protocols,
             path=project.path_with_namespace,
             default_branch=project.default_branch,
-            internal_id=str(project.get_id()),
+            # internal_id=str(project.get_id()),
             project_url=self.canonize(project.web_url),
             metadata=metadata,
             private=project.visibility != "public",
             branches={
                 b.name: b.commit["id"] for b in project.branches.list(iterator=True)
             },
             tags={t.name: t.target for t in project.tags.list(iterator=True)},
@@ -732,32 +1130,36 @@
     Manages a cloudmap repository with a cloudmap.yaml file.
     Sync operations create a separate branch for each repository host to reflect its remote state.
     """
 
     def __init__(
         self,
         repo: GitRepo,
-        provider_branch: str,
+        host_branch: str,
         localrepo_root: str = "",
         path: str = "",
+        skip_analysis: bool = False,
     ):
         self.repo = repo
-        self.branch = provider_branch
+        self.branch = host_branch
         self.directory = Directory(
-            str(Path(repo.working_dir) / (path or "cloudmap.yaml")), localrepo_root
+            str(Path(repo.working_dir) / (path or "cloudmap.yaml")),
+            localrepo_root,
+            skip_analysis,
         )
 
     @classmethod
     def from_name(
         cls,
         local_env: "LocalEnv",
         name: str,
         clone_root: str,
-        provider_name: str,
+        host_name: str,
         namespace: str,
+        skip_analysis: bool,
     ) -> "CloudMap":
         environment = local_env.get_context().get("cloudmaps", {})
         # for now name is just the name of repository
         repository = environment.get("repositories", {}).get(name)
         if repository:
             cloudmap_url = repository["url"]
             localrepo_root = repository.get("clone_root", clone_root)
@@ -765,19 +1167,19 @@
             # assume name is an url or local path
             cloudmap_url = name
             localrepo_root = clone_root
         url, path, revision = split_git_url(cloudmap_url)
         url = normalize_git_url(url)
 
         # what if branch only exists locally?
-        if not provider_name:
+        if not host_name:
             branch = revision or "main"
             branch_exists = True
         else:
-            branch = f"hosts/{provider_name}/{namespace}".rstrip("/")
+            branch = f"hosts/{host_name}"
             local_repo = local_env.find_git_repo(url, branch)
             if local_repo and branch in local_repo.repo.branches:  # type: ignore
                 branch_exists = True
             else:
                 branch_exists = bool(git.cmd.Git().ls_remote(url, branch, heads=True))
         if branch_exists:  # branch exists
             # clone or checkout branch
@@ -785,96 +1187,105 @@
         else:
             # clone or checkout main and create branch
             repo, _, _ = local_env.find_or_create_working_dir(
                 url, "main", checkout_args=dict(b=branch)
             )
         if not repo:
             raise UnfurlError(f"couldn't clone {url}")
-        return CloudMap(repo, branch, localrepo_root, path)
+        return CloudMap(repo, branch, localrepo_root, path, skip_analysis)
 
     def get_host(
         self,
         local_env: "LocalEnv",
         name: str,
         namespace: str,
         visibility: Optional[str] = None,
     ) -> RepositoryHost:
         environment = local_env.get_context().get("cloudmaps", {})
-        provider_config: Optional[dict] = environment.get("hosts", {}).get(name)
+        host_config: Optional[dict] = environment.get("hosts", {}).get(name)
         clone_root = self.directory.repos_root
-        if provider_config is None:
+        if host_config is None:
             if name == "local":
-                provider_config = dict(type="local", clone_root=clone_root)
+                host_config = dict(type="local", clone_root=clone_root)
             elif ":" in name:
                 # assume it's an url pointing to gitlab or unfurl cloud instance
-                provider_config = dict(type="gitlab", url=name)
+                host_config = dict(type="gitlab", url=name)
             else:
                 raise UnfurlError(f"no repository host named {name} found")
-        if provider_config["type"] == "local":
-            return LocalRepositoryHost(provider_config.get("clone_root", clone_root))
+        if host_config["type"] == "local":
+            return LocalRepositoryHost(host_config.get("clone_root", clone_root))
 
-        assert provider_config["type"] in ["gitlab", "unfurl.cloud"]
-        config = local_env.map_value(provider_config, environment.get("variables"))
+        assert host_config["type"] in ["gitlab", "unfurl.cloud"]
+        config = local_env.map_value(host_config, environment.get("variables"))
         if visibility:
             config["visibility"] = visibility
         return GitlabManager(name, config, namespace)
 
+    def from_host(self, host: RepositoryHost) -> bool:
+        host.from_host(self.directory)
+        changed = self.save(
+            f"Update {self.branch} with latest from {'/'.join([host.name, host.path])}"
+        )
+        return changed
+
     def sync(self, host: RepositoryHost, force=False) -> None:
         """
         Synchronize the cloudmap with the given the repository host.
 
         First, update a branch named "hosts/{host_name}/{namespace}" with the latest from the repository host.
-        Then merge the provider branch into "main".
+        Then merge the host branch into "main".
         If a conflict is detected, abort with a merge error in the cloudmap repository.
         For example, if a repository branch or tags was changed in both branches there will be a merge conflict.
         If so, manually merge the changes in the local repo (they will be on the remote branch), sync them with the cloudmap, then re-run this command.
 
         Finally, update the repository host with any changes it needs to match the cloudmap.
         New project will be create or with existing project metadata updated and changes in local repository clones will be pushed to the host.
 
         The user is responsible for pushing changes to cloudmap repository back upstream.
         """
-        host.from_host(self.directory)
-        changed = self.save(
-            f"Update {self.branch} with latest from {'/'.join([host.name, host.path])}"
-        )
+        changed = self.from_host(host)
+        return self.to_host(host, changed, force)
 
+    def to_host(self, host: RepositoryHost, merge_host: bool, force=False) -> None:
         if self.branch != "main":
             self.repo.checkout("main")
             self.directory.reload()  # map may have changed, reload the directory
             # make sure local repos matches the cloudmap
             mismatched = self.directory.find_mismatched_repo(host)
             if mismatched:
                 raise UnfurlError(
                     f"Aborting sync, cloudmap is out of sync with {mismatched.working_dir}"
                 )
-            # merge the provider branch into main
+            # merge the host branch into main
             # there will be a merge conflict if a repository branch or tags was changed in both branches
             # if so, manually merge the changes in the local repo (they will be on the remote branch), sync them with the cloudmap, then re-run
-            if changed:
-                self.repo.repo.git.merge(self.branch)  # --commit --no-edit
-            self.directory.reload()  # map changed, reload the directory
+            if merge_host:
+                self.repo.repo.git.merge(
+                    self.branch, m=f"merge changes from syncing {self.branch}"
+                )
+                self.directory.reload()  # map changed, reload the directory
 
-            # for each repository merge the provider's branch
-            # (which was fetched during from_provider()) into main
+            # for each repository merge the host's default branch (it was already fetched during from_host())
+            # into the local repo's default branch
             # since the cloudmap merge was successful this will just be a fast-forward merge
-            self.directory.merge(host)
+            self.directory.merge_from_host(host)
 
-        # deploy main to the provider
+        # deploy main to the host
         host.to_host(self.directory, True, force=force)
 
         # if force we might have created merge commits, update the cloudmap with those
         self.save(f"synced {host.name}")
         if self.branch != "main":
-            # set provider branch match to main because we are even now
+            # set host branch head to match to main because we are even now
             self.repo.repo.git.branch(self.branch, f=True)
 
     def save(self, msg: str) -> bool:
         self.directory.save()
-        if self.repo.is_dirty(True):
-            self.repo.add_all(self.repo.working_dir)
+        if self.repo.is_dirty(True, self.directory.config.path):
+            assert self.directory.config.path
+            self.repo.commit_files([self.directory.config.path], msg)
             self.repo.repo.index.commit(msg)
             logger.debug(f"committed: {msg}")
             return True
         else:
             logger.debug(f"nothing to commit for: {msg}")
             return False
```

### Comparing `unfurl-0.6.2/unfurl/configurator.py` & `unfurl-0.7.0/unfurl/configurator.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     (Titlecase recommended)"""
 
     exclude_from_digest: Tuple[str, ...] = ()
 
     attribute_output_metadata_key: Optional[str] = None
 
     @classmethod
-    def set_config_spec_args(klass, kw: dict, target: None) -> dict:
+    def set_config_spec_args(klass, kw: dict, target: EntityInstance) -> dict:
         return kw
 
     def __init__(self, configurationSpec: ConfigurationSpec) -> None:
         self.configSpec = configurationSpec
 
     def get_generator(self, task: "TaskView") -> Generator:
         return self.run(task)
@@ -659,40 +659,41 @@
             operation=self.configSpec.operation,
             timeout=self.configSpec.timeout,
             target=self.target.name,
             reason=self.reason,
             cwd=self.cwd,
         )
 
+    @staticmethod
     def find_connection(
-        self, target: NodeInstance, relation: str = "tosca.relationships.ConnectsTo"
+        ctx: RefContext, target: NodeInstance, relation: str = "tosca.relationships.ConnectsTo"
     ) -> Optional[RelationshipInstance]:
         """
         Find a relationship that this task can use to connect to the given instance.
         First look for relationship between the task's target instance and the given instance.
         If none is found, see if there a default connection of the given type.
 
         Args:
             target (NodeInstance): The instance to connect to.
             relation (str, optional): The relationship type. Defaults to "tosca.relationships.ConnectsTo".
 
         Returns:
             RelationshipInstance or None: The connection instance.
         """
-        connection = self.query(
+        connection = cast(Optional[RelationshipInstance], Ref(
             f"$OPERATION_HOST::.requirements::*[.type={relation}][.target=$target]",
-            vars=dict(target=target),
-        )
+            vars=dict(target=target)).resolve_one(ctx))
+
         # alternative query: [.type=unfurl.nodes.K8sCluster]::.capabilities::.relationships::[.type=unfurl.relationships.ConnectsTo.K8sCluster][.source=$OPERATION_HOST]
         if not connection:
             # no connection, see if there's a default relationship template defined for this target
             endpoints = target.get_default_relationships(relation)
             if endpoints:
                 connection = endpoints[0]
-        if connection:  # type: ignore
+        if connection:
             assert isinstance(connection, RelationshipInstance)
             return connection
         return None
 
     def sensitive(self, value: object) -> Union[sensitive, object]:
         """Mark the given value as sensitive. Sensitive values will be encrypted or redacted when outputed.
 
@@ -963,21 +964,21 @@
             updated = True
 
         template = resourceSpec.get("template")
         if template:
             assert self._manifest.tosca
             if isinstance(template, dict):
                 tname = existingResource.template.name
-                existingResource.template = self._manifest.tosca.add_node_template(
+                existingResource.template = existingResource.template.topology.add_node_template(
                     tname, template
                 )
             elif (
                 isinstance(template, str) and template != existingResource.template.name
             ):
-                nodeSpec = self._manifest.tosca.nodeTemplates.get(template)
+                nodeSpec = existingResource.template.topology.get_node_template(template)
                 if not nodeSpec:
                     raise UnfurlTaskError(
                         self,
                         f"couldn't update TOSCA template for {existingResource.name}: '{template}' is not defined",
                     )
                 existingResource.template = nodeSpec
             updated = True
```

### Comparing `unfurl-0.6.2/unfurl/configurators/__init__.py` & `unfurl-0.7.0/unfurl/configurators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 from ..eval import Ref, map_value
 from ..configurator import Configurator, TaskView
 from ..result import Results, ResultsMap
 from ..util import register_short_names
 from ..support import Status
 from ..planrequests import set_default_command
+from ..runtime import EntityInstance
 import importlib
 from typing import Sequence, Tuple
 from collections.abc import Mapping
 
 # need to define these now because these configurators are lazily imported
 # and so won't register themselves through AutoRegisterClass
 register_short_names(
@@ -19,15 +20,15 @@
         for name in "Ansible Shell Supervisor Terraform DNS Kompose".split()
     }
 )
 
 
 class CmdConfigurator(Configurator):
     @classmethod
-    def set_config_spec_args(klass, kw: dict, target):
+    def set_config_spec_args(klass, kw: dict, target: EntityInstance):
         return set_default_command(kw, "")
 
 
 class PythonPackageCheckConfigurator(Configurator):
     def run(self, task):
         try:
             importlib.import_module(task.target.file)
```

### Comparing `unfurl-0.6.2/unfurl/configurators/ansible.py` & `unfurl-0.7.0/unfurl/configurators/ansible.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             if "keys" in creds:
                 hostVars.update(creds["keys"])
         hostVars.update(connection.attributes.get("hostvars", {}))
 
     def _make_inventory(self, host, allVars, task):
         if host:
             hostVars = self._get_host_vars(host)
-            connection = task.find_connection(
+            connection = task.find_connection(task.inputs.context,
                 host, "unfurl.relationships.ConnectsTo.Ansible"
             )
             if connection:
                 self._update_vars(connection, hostVars)
 
             if "ansible_host" not in hostVars:
                 ip_address = host.attributes.get("public_ip") or host.attributes.get(
```

### Comparing `unfurl-0.6.2/unfurl/configurators/dns-template.yaml` & `unfurl-0.7.0/unfurl/configurators/dns-template.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/configurators/dns.py` & `unfurl-0.7.0/unfurl/configurators/dns.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/configurators/docker-template.yaml` & `unfurl-0.7.0/unfurl/configurators/docker-template.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/configurators/gcp.py` & `unfurl-0.7.0/unfurl/configurators/gcp.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/configurators/helm-template.yaml` & `unfurl-0.7.0/unfurl/configurators/helm-template.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/configurators/k8s.py` & `unfurl-0.7.0/unfurl/configurators/k8s.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Copyright (c) 2020 Adam Souzis
 # SPDX-License-Identifier: MIT
 from __future__ import absolute_import
 import re
 from base64 import b64encode
-from typing import Dict, Union
-from ..configurator import Configurator
-from ..support import Status, Priority
-from ..runtime import RelationshipInstance
+from typing import Dict, Mapping, Union, cast
+from ..configurator import Configurator, TaskView
+from ..support import Status, Priority, to_kubernetes_label
+from ..runtime import EntityInstance, NodeInstance, RelationshipInstance
 from ..util import UnfurlTaskError, wrap_sensitive_value, sensitive_dict
 from .ansible import AnsibleConfigurator
 from ..yamlloader import yaml
-from ..eval import set_eval_func, map_value
+from ..eval import Ref, RefContext, set_eval_func, map_value
 import subprocess
 import json
 from ansible_collections.kubernetes.core.plugins.module_utils.common import (
     K8sAnsibleMixin,
 )
 
 # XXX need to define fail_json
@@ -27,15 +27,15 @@
     # https://docs.ansible.com/ansible/latest/collections/kubernetes/core/k8s_module.html
     #  for connection settings
     # https://github.com/ansible-collections/kubernetes.core/blob/7f7008fecc9e5d16340e9b0bff510b7cde2f2cfd/plugins/connection/kubectl.py
     if not instance:
         return {}
     connection: Dict[str, Union[str, bool]] = {}
     if isinstance(instance, RelationshipInstance):
-        connect = instance.attributes
+        connect: Mapping = instance.attributes
         # the parent of a relationship will be the capability it connects to
         # or root if relationship is a default connection
         assert instance.parent
         if instance.parent is not instance.root:
             endpoint = instance.parent.attributes
         else:
             endpoint = {}
@@ -111,59 +111,65 @@
     "client_key": "--client-key",
     "ca_cert": "--certificate-authority",
     "api_key": "--token",
     "as": "--as",
 }
 
 
-def _get_connection(task) -> dict:
+def _get_connection(ctx: RefContext) -> dict:
     # get the cluster that the target resource is hosted on
-    cluster = task.query("[.type=unfurl.nodes.K8sCluster]")
+    cluster = Ref("[.type=unfurl.nodes.K8sCluster]").resolve_one(ctx)
     relation = "unfurl.relationships.ConnectsTo.K8sCluster"
     if cluster:
-        instance = task.find_connection(cluster, relation)
+        instance = TaskView.find_connection(ctx, cast(NodeInstance, cluster), relation)
     else:
-        relationships = task.target.get_default_relationships(relation)
+        relationships = cast(
+            EntityInstance, ctx.currentResource
+        ).get_default_relationships(relation)
         if relationships:
             instance = relationships[0]
         else:
             instance = None
     if instance:
         config = _get_connection_config(instance)
     else:
         config = {}
 
     # check if we are in a namespace, fall back to "default"
-    namespace = task.query("[.type=unfurl.nodes.K8sNamespace]")
+    namespace = Ref("[.type=unfurl.nodes.K8sNamespace]").resolve_one(ctx)
     if namespace:
-        config["namespace"] = namespace.attributes["name"]
-    else:
-        config["namespace"] = "default"
+        config["namespace"] = cast(NodeInstance, namespace).attributes["name"]
     return config
 
 
-def get_kubectl_args(task):
-    connection = _get_connection(task)
+set_eval_func(
+    "kubernetes_current_namespace",
+    lambda args, ctx: _get_connection(ctx).get("namespace") if ctx.task else None,
+)
+
+
+def get_kubectl_args(ctx: RefContext):
+    connection = _get_connection(ctx)
     options = []
     for key, value in connection.items():
         if value and key in CONNECTION_OPTIONS:
             options.append(CONNECTION_OPTIONS[key])
             options.append(value)
     if "validate_certs" in connection and not connection["validate_certs"]:
         options.append("--insecure-skip-tls-verify")
     groups = connection.get("as-group") or []
     for group in groups:
         options.append("--as-group")
         options.append(group)
     return options
 
 
-def kubectl(cmd, ctx):
+def kubectl(cmd, ctx: RefContext):
     cmd = map_value(cmd, ctx)
-    args = get_kubectl_args(ctx.task)
+    args = get_kubectl_args(ctx)
     if not isinstance(cmd, list):
         cmd = cmd.split()
     full_cmd = ["kubectl"] + args + cmd
     if ctx.kw.get("execute"):
         return subprocess.run(full_cmd, capture_output=True).stdout
     else:
         return full_cmd
@@ -335,25 +341,21 @@
                 raise UnfurlTaskError(
                     task, 'invalid Kubernetes resource definition, "kind" is missing'
                 )
             if kind == "Secret" and "data" in definition:
                 definition["data"] = wrap_sensitive_value(definition["data"])
             return definition
 
-    def update_metadata(self, definition, task):
-        namespace = None
-        if task.target.parent.template.is_compatible_type("unfurl.nodes.K8sNamespace"):
-            namespace = task.target.parent.attributes["name"]
+    def update_metadata(self, definition, task, namespace):
         md = definition.setdefault("metadata", {})
         if namespace and "namespace" not in md:
             md["namespace"] = namespace
         # else: error if namespace mismatch?
 
-        # XXX if using target.name, convert into kube friendly dns-style name
-        name = task.target.attributes.get("name", task.target.name)
+        name = to_kubernetes_label(task.target.attributes.get("name", task.target.name))
         if "name" in md and md["name"] != name:
             task.target.attributes["name"] = md["name"]
         else:
             md["name"] = name
 
     def _make_check(self, connectionConfig, definition, extra_configuration):
         moduleSpec = connectionConfig.copy()
@@ -364,16 +366,16 @@
         if extra_configuration:
             moduleSpec.update(extra_configuration)
         return [{"kubernetes.core.k8s_info": moduleSpec}]
 
     def find_playbook(self, task):
         # this is called by AnsibleConfigurator.get_playbook()
         definition = self.get_definition(task)
-        self.update_metadata(definition, task)
-        connectionConfig = _get_connection(task)
+        connectionConfig = _get_connection(task.inputs.context)
+        self.update_metadata(definition, task, connectionConfig.get("namespace"))
         extra_configuration = task.inputs.get("configuration")
         extra_playbook = task.inputs.get("playbook")
 
         if task.configSpec.operation in ["check", "discover"]:
             return self._make_check(connectionConfig, definition, extra_configuration)
 
         delete = task.configSpec.operation in ["Standard.delete", "delete"]
```

### Comparing `unfurl-0.6.2/unfurl/configurators/kompose.py` & `unfurl-0.7.0/unfurl/configurators/kompose.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/configurators/shell.py` & `unfurl-0.7.0/unfurl/configurators/shell.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/configurators/supervisor-template.yaml` & `unfurl-0.7.0/unfurl/configurators/supervisor-template.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/configurators/supervisor.py` & `unfurl-0.7.0/unfurl/configurators/supervisor.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/configurators/terraform.py` & `unfurl-0.7.0/unfurl/configurators/terraform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Copyright (c) 2020 Adam Souzis
 # SPDX-License-Identifier: MIT
 from typing import TYPE_CHECKING
+
+from ..runtime import EntityInstance
 from ..util import save_to_file, UnfurlTaskError, wrap_var, which
 from .shell import ShellConfigurator, clean_output, make_regex_filter
 from ..support import Status
 from ..result import Result
 from ..projectpaths import get_path, FilePath, Folders
 import json
 import os
@@ -157,15 +159,15 @@
         "key_material",
         "password",
         "private_key",
         "server_ca_cert",
     ]
 
     @classmethod
-    def set_config_spec_args(klass, kw: dict, target):
+    def set_config_spec_args(klass, kw: dict, target: EntityInstance):
         if not which("terraform"):
             artifact = target.template.find_or_create_artifact(
                 "terraform", predefined=True
             )
             if artifact:
                 kw["dependencies"].append(artifact)
         return kw
```

### Comparing `unfurl-0.6.2/unfurl/eval.py` & `unfurl-0.7.0/unfurl/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 Internal:
 
 eval_ref() given expression (string or dictionary) return list of Result
 Expr.resolve() given expression string, return list of Result
 Results._map_value same as map_value but with lazily evaluation
 """
+from functools import partial
 from typing import (
     Any,
     Dict,
     List,
     Tuple,
     Optional,
     Union,
@@ -44,20 +45,24 @@
 
 if TYPE_CHECKING:
     from .configurator import TaskView
 
 
 logger = cast(UnfurlLogger, logging.getLogger("unfurl.eval"))
 
+class UnfurlEvalError(UnfurlError):
+    pass
 
 def map_value(
     value: Any,
     resourceOrCxt: Union["RefContext", "ResourceRef"],
     applyTemplates: bool = True,
 ) -> Any:
+    """Resolves any expressions or template strings embedded in the given map or list.
+    """
     if not isinstance(resourceOrCxt, RefContext):
         resourceOrCxt = RefContext(resourceOrCxt)
     return _map_value(value, resourceOrCxt, False, applyTemplates)
 
 
 def _map_value(
     value: Any, ctx: "RefContext", wantList: bool = False, applyTemplates: bool = True
@@ -263,14 +268,26 @@
         del state["referenced"]
         return state
 
     def __setstate__(self, d: dict) -> None:
         self.__dict__ = d
         self.referenced = _Tracker()
 
+    def __getattr__(self, key):
+        func = self._Funcs.get(key)
+        if not func:
+            raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{key}'")
+
+        def _eval_func(*args, **kw):
+            self.currentFunc = key
+            self.kw = kw
+            assert func
+            return func(args, self)
+        return _eval_func
+
 
 class Expr:
     def __init__(self, exp, vars=None):
         self.vars = {"true": True, "false": False, "null": None}
 
         if vars:
             self.vars.update(vars)
@@ -356,15 +373,15 @@
         """
         if self.strict is not None:
             # overrides RefContext's strict
             strict = self.strict
         ctx = ctx.copy(
             vars=self.vars, wantList=wantList, trace=self.trace, strict=strict
         )
-        base_dir = getattr(self.source, "base_dir", None)
+        base_dir = getattr(self.source, "base_dir", "")
         if base_dir:
             ctx.base_dir = base_dir
         # $start is set in eval_ref but the user use that to override currentResource
         if "start" in self.vars:
             ctx.currentResource = ctx.resolve_var("$start")
         ctx.trace(
             f"Ref.resolve(wantList={wantList}) start strict {ctx.strict}",
@@ -479,14 +496,18 @@
     return val
 
 
 def quote_func(arg, ctx):
     return arg
 
 
+def func_defined_func(arg, ctx):
+    return map_value(arg, ctx) in ctx._Funcs
+
+
 def eq_func(arg, ctx):
     args = map_value(arg, ctx)
     assert_form(args, MutableSequence, len(args) == 2)
     return args[0] == args[1]
 
 
 def validate_schema_func(arg, ctx):
@@ -601,14 +622,15 @@
     "and": and_func,
     "or": or_func,
     "not": not_func,
     "q": quote_func,
     "eq": eq_func,
     "validate": validate_schema_func,
     "foreach": for_each_func,
+    "is_function_defined": func_defined_func,
 }
 RefContext._Funcs = _CoreFuncs.copy()
 _FuncsTop = ["q"]
 
 
 class SafeRefContext(RefContext):
     _Funcs = _CoreFuncs.copy()
@@ -648,27 +670,36 @@
                 if "var" in val:
                     unexpected: Union[bool, str] = "var"
                 elif key != "foreach" and "foreach" in val:
                     unexpected = "foreach"
                 else:
                     unexpected = False
                 if unexpected:
-                    raise UnfurlError(
+                    raise UnfurlEvalError(
                         f"unexpected '{unexpected}' found, did you intend it for the parent?"
                     )
                 val = func(args, ctx)
                 if key == "q":
                     if isinstance(val, Result):
                         return [val]
                     else:
                         return [Result(val)]
                 break
         else:
             if "ref" not in val and "eval" not in val:
-                raise UnfurlError(f"Function missing in {dict(val)}")
+                if isinstance(ctx, SafeRefContext):
+                    msg = f"function unsafe or missing in {dict(val)}"
+                    if not ctx.strict:
+                        logger.warning("In safe mode, skipping unsafe eval: " + msg, stack_info=True)
+                        return [Result("Error: in safe mode, skipping unsafe eval")]
+                    else:
+                        msg = "Error: unsafe eval: " + msg
+                else:
+                    msg = f"Function missing in {dict(val)}"
+                raise UnfurlEvalError(msg)
     elif isinstance(val, six.string_types):
         if is_template(val, ctx):
             return [Result(apply_template(val, ctx))]
         else:
             expr = Expr(val, ctx.vars)
             results = expr.resolve(ctx)  # returns a list of Result
             ctx.trace("expr.resolve", results)
```

### Comparing `unfurl-0.6.2/unfurl/filter_plugins/ref.py` & `unfurl-0.7.0/unfurl/filter_plugins/ref.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/init.py` & `unfurl-0.7.0/unfurl/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,15 +485,15 @@
         homeProject = newProject.parentProject
         assert homeProject
         homeProject.register_project(newProject, create_context)
 
     if not kw.get("render"):
         if password_vault:
             yaml = make_yaml(password_vault)
-            commit_secrets(os.path.dirname(projectConfigPath), yaml)
+            commit_secrets(os.path.dirname(projectConfigPath), yaml, repo)
 
         _commit_repos(
             projectdir,
             repo,
             not mono and ensembleRepo,
             shared,
             kw,
```

### Comparing `unfurl-0.6.2/unfurl/job.py` & `unfurl-0.7.0/unfurl/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 A Job is generated by comparing a list of specs with the last known state of the system.
 Job runs tasks, each of which has a configuration spec that is executed on the running system
 Each task tracks and records its modifications to the system's state
 """
 
 import collections
 from datetime import datetime, timedelta
-import types
 import itertools
 import os
 import json
 from typing import (
     Any,
     Iterable,
     List,
@@ -34,15 +33,15 @@
     Reason,
     NodeState,
     AttributeChanges,
 )
 from .result import ResourceRef, serialize_value, ChangeRecord
 from .util import UnfurlError, UnfurlTaskError, to_enum, change_cwd
 from .merge import merge_dicts
-from .runtime import EntityInstance, NodeInstance, Operational, OperationalInstance
+from .runtime import EntityInstance, TopologyInstance, Operational, OperationalInstance
 from .logs import end_collapsible, start_collapsible, getLogger
 from .configurator import (
     TaskView,
     ConfiguratorResult,
     Configurator,
 )
 from .projectpaths import Folders, rmtree
@@ -54,16 +53,17 @@
     SetStateRequest,
     JobRequest,
     do_render_requests,
     get_render_requests,
     set_fulfilled,
     set_fulfilled_stragglers,
     create_instance_from_spec,
+    get_success_status,
 )
-from .plan import Plan, get_success_status
+from .plan import Plan
 from .localenv import LocalEnv
 from . import display
 from . import configurators  # need to import configurators even though it is unused
 from .reporting import JobReporter
 
 from time import perf_counter
 
@@ -130,22 +130,32 @@
         requiredOnly=False,
         commit=False,
         dirty="auto",  # run the job even if the repository has uncommitted changrs
         message=None,
     )
 
     parentJob = None
-    masterJob: Optional["Job"] =None
+    masterJob: Optional["Job"] = None
     instance = None
     workflow = Defaults.workflow
     planOnly = False
     verbose = 0
     message: Optional[str] = None
     commit = False
     push = False
+    template: Optional[str] = None
+    add: bool = True
+    skip_new: bool = False
+    change_detection: str = "evaluate"
+    repair: str = "error"
+    force: bool = False
+    check: bool = False
+    prune: bool = False
+    destroyunmanaged: bool = False
+    upgrade: bool = False
 
     defaults = dict(
         global_defaults,
         parentJob=parentJob,
         instance=instance,
         instances=None,
         template=None,
@@ -216,15 +226,15 @@
         # for summary:
         self.modified_target = False
         self.target_status = target.status
         self.target_state = target.state
 
         # set the attribute manager on the root resource
         self._attributeManager = AttributeManager(self._manifest.yaml, self)
-        self.target.root.attributeManager = self._attributeManager
+        self.target.root.set_attribute_manager(self._attributeManager)
         self._resolved_inputs = {}
 
     def _status(self, seen: Dict[int, Operational]) -> Status:
         status = self.local_status
         # if not status:
         #     return Status.unknown
         return status  # type: ignore
@@ -265,15 +275,15 @@
         finally:
             # serialize configuration changes
             self.commit_changes()
         return result
 
     def start(self) -> None:
         self.start_run()
-        self.target.root.attributeManager = self._attributeManager
+        self.target.root.set_attribute_manager(self._attributeManager)
         self.target_status = self.target.status
         self.target_state = self.target.state
         self.set_envvars()
 
     def _update_status(self, result) -> bool:
         """
         Update the instances status with the result of the operation.
@@ -569,15 +579,15 @@
     """
 
     MAX_NESTED_SUBTASKS = 100
 
     def __init__(
         self,
         manifest: "YamlManifest",
-        rootResource: NodeInstance,
+        rootResource: TopologyInstance,
         jobOptions: JobOptions,
         previousId: Optional[str] = None,
     ) -> None:
         assert isinstance(jobOptions, JobOptions)
         self.__dict__.update(jobOptions.__dict__)
         super().__init__(self.parentJob, self.startTime, Status.ok, previousId)  # type: ignore
         self.dry_run = jobOptions.dryrun  # type: ignore
@@ -1126,15 +1136,17 @@
             return None, True
 
         task = req.task or self.create_task(
             req.configSpec, req.target, reason=req.reason
         )
         if task:
             start_collapsible(f"Task {req.target.name} ({req}", hash(req), True)
-            task.logger.info("started task.", extra=dict(json=task.summary(asJson=True)))
+            task.logger.info(
+                "started task.", extra=dict(json=task.summary(asJson=True))
+            )
 
             resource = req.target
             startingStatus = resource._localStatus
             if req.startState is not None:
                 resource.state = req.startState
             startingState = resource.state
             self.add_work(task)
@@ -1175,16 +1187,18 @@
             #     task.target.state,
             #     req.startState,
             # )
             end_collapsible(hash(req))
             task_success = task.result and task.result.success
             status = task.target.status.name.upper()
             state_status = task.target.state.name if task.target.state else ""
-            extra = dict(rich=dict(style=task.target.status.color),
-                         json=task.summary(asJson=True))
+            extra = dict(
+                rich=dict(style=task.target.status.color),
+                json=task.summary(asJson=True),
+            )
             if task_success:
                 task.logger.info(
                     "Task succeeded, Resource Status: %s State: %s",
                     status,
                     state_status,
                     extra=extra,
                 )
@@ -1205,15 +1219,15 @@
         * Notification of add or removing dependency on a resource or properties of a resource
         * Notification of creation or deletion of a resource
         * Requests a resource with requested metadata, if it doesn't exist, a task is run to make it so
         (e.g. add a dns entry, install a package).
 
         Returns a task.
         """
-        task.target.root.attributeManager = task._attributeManager
+        task.target.root.set_attribute_manager(task._attributeManager)
         errors: Any = None
         ok, errors = self.can_run_task(task)
         if not ok:
             return task.finished(ConfiguratorResult(False, False, result=errors))
 
         task.start()
         change = None
@@ -1271,15 +1285,17 @@
     # Job Reporting methods
     ###########################################################################
 
     def stats(self, asMessage: bool = False) -> Union[Dict[str, int], str]:
         return JobReporter.stats(self.workDone.values(), asMessage)
 
     def get_end_time(self) -> str:
-        return (self.startTime + timedelta(seconds=self.timeElapsed)).strftime(self.DateTimeFormat)
+        return (self.startTime + timedelta(seconds=self.timeElapsed)).strftime(
+            self.DateTimeFormat
+        )
 
     def print_summary_table(self) -> str:
         try:
             return JobReporter.summary_table(self)
         except Exception:
             logger.error("Error while creating job summary", exc_info=True)
             return "Error while creating job summary"
```

### Comparing `unfurl-0.6.2/unfurl/localenv.py` & `unfurl-0.7.0/unfurl/localenv.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,15 +260,15 @@
         while os.path.exists(os.path.join(self.projectRoot, name)):
             name = basename + str(counter)
             counter += 1
         return os.path.join(self.projectRoot, name)
 
     def _find_git_repo(
         self, repoURL: str, revision: Optional[str] = None
-    ) -> Union[GitRepo, str]:
+    ) -> Union[RepoView, str]:
         # if repo isn't found, return the repo url, possibly rewritten to include server credentials
         apply_credentials = self.overrides.get("apply_url_credentials")
         candidate = None
         repourl_parts = urlsplit(repoURL)
         normalized = normalize_git_url_hard(repoURL)
         for dir, repository in self.workingDirs.items():
             repo = repository.repo
@@ -277,19 +277,19 @@
                 initialCommit = urlparse(repoURL).netloc.partition(":")[0]
                 match = initialCommit == repo.get_initial_revision()
             else:
                 match = normalized == normalize_git_url_hard(repo.url)
             if match:
                 if revision:
                     if repo.revision == repo.resolve_rev_spec(revision):
-                        return repo
+                        return repository
                     # revisions don't match but we'll return it if we don't find a better candidate
-                    candidate = repo
+                    candidate = repository
                 else:
-                    return repo
+                    return repository
             elif apply_credentials:
                 # if an existing repository has the same hostname as the new repository's url
                 # and has credentials, update the new url with those credentials
                 candidate_parts = urlsplit(repo.url)
                 password = candidate_parts.password
                 if password:
                     if (
@@ -304,15 +304,15 @@
 
     def find_git_repo(
         self, repoURL: str, revision: Optional[str] = None
     ) -> Optional[GitRepo]:
         repo_or_url = self._find_git_repo(repoURL, revision)
         if isinstance(repo_or_url, str):
             return None
-        return repo_or_url
+        return repo_or_url.repo
 
     def find_path_in_repos(
         self, path: str, importLoader: Optional[Any] = None
     ) -> Tuple[Optional[GitRepo], Optional[str], Optional[str], Optional[bool]]:
         """If the given path is part of the working directory of a git repository
         return that repository and a path relative to it"""
         # importloader is unused until pinned revisions are supported
@@ -604,16 +604,16 @@
         self.localConfig.register_project(project, for_context, changed, save_project)
         self.workingDirs[
             project.project_repoview.working_dir
         ] = project.project_repoview
 
     def load_yaml_include(
         self,
-        yamlConfig,
-        templatePath,
+        yamlConfig: YamlConfig,
+        templatePath: Union[str, dict],
         baseDir,
         warnWhenNotFound=False,
         expanded=None,
         action=None,
     ):
         """
         This is called while the YAML config is being loaded.
@@ -629,15 +629,15 @@
         url_vars = {}
         url_vars.update(self.overrides)
         if action:
             if action.get_key:
                 return substitute_env(action.get_key, url_vars)
             if action.check_include:
                 return True
-            return None  # unsupported action 
+            return None  # unsupported action
 
         if merge == "maplist" and "ENVIRONMENT" not in self.overrides:
             # don't load remote includes for LocalEnv that don't specify an environment
             # XXX (hackish way to avoid loads for transitory LocalEnv objects)
             logger.trace("skipping retrieving url with ENVIRONMENT: %s", key)
             return key, None
 
@@ -1046,46 +1046,59 @@
             msg = "No vault password found"
             if self.manifest_context_name:
                 msg += f" for environment {self.manifest_context_name}"
             self.logger.debug(msg)
         return vault
 
     def get_manifest(
-        self, path: Optional[str] = None, skip_validation: bool = False
+        self,
+        path: Optional[str] = None,
+        skip_validation: bool = False,
+        safe_mode: Optional[bool] = None,
     ) -> "YamlManifest":
         from .yamlmanifest import YamlManifest
 
         if path and path != self.manifestPath:
             # share projects and ensembles
-            localEnv = LocalEnv(path, parent=self)
+            localEnv = LocalEnv(path, parent=self, readonly=self.readonly)
             return localEnv.get_manifest()
         else:
             assert self.manifestPath
             manifest = self._manifests.get(self.manifestPath)
             if not manifest:
                 # should load vault ids from context
                 vault = self.get_vault()
                 manifest = YamlManifest(
-                    localEnv=self, vault=vault, skip_validation=skip_validation
+                    localEnv=self,
+                    vault=vault,
+                    skip_validation=skip_validation,
+                    safe_mode=bool(safe_mode),
                 )
                 self._manifests[self.manifestPath] = manifest
             return manifest
 
     def get_project(self, path: str, homeProject: Optional[Project]) -> Project:
         path = Project.normalize_path(path)
         project = self._projects.get(path)
         if not project:
             project = Project(path, homeProject, self.overrides, readonly=self.readonly)
             self._projects[path] = project
         return project
 
-    def get_external_manifest(self, location: dict) -> Optional["YamlManifest"]:
+    def get_external_manifest(
+        self,
+        location: dict,
+        skip_validation: bool,
+        safe_mode: bool,
+    ) -> Optional["YamlManifest"]:
         localEnv = self._get_external_localenv(location)
         if localEnv:
-            return localEnv.get_manifest()
+            return localEnv.get_manifest(
+                skip_validation=skip_validation, safe_mode=safe_mode
+            )
         else:
             return None
 
     def _get_external_localenv(
         self, location: dict, currentProject: Optional[Project] = None
     ) -> Optional["LocalEnv"]:
         # currentProject because this method might be called before self.project was set
@@ -1118,15 +1131,17 @@
                 file = os.path.join(file, project.get("file"))
 
         if not repo:
             return None
 
         projectRoot = os.path.join(repo.working_dir, file)
         return LocalEnv(
-            os.path.join(projectRoot, location.get("file") or ""), parent=self
+            os.path.join(projectRoot, location.get("file") or ""),
+            parent=self,
+            readonly=self.readonly,
         )
 
     def _find_given_manifest_or_project(
         self, manifestPath: str
     ) -> Tuple[Optional[str], Optional[Project]]:
         if not os.path.exists(manifestPath):
             return None, None
@@ -1234,38 +1249,38 @@
         return (
             self.config.create_local_instance(name.rstrip("s"), attributes),
             spec,
         )
 
     def _find_git_repo(
         self, repoURL: str, revision: Optional[str] = None
-    ) -> Union[GitRepo, str]:
+    ) -> Union[RepoView, str]:
         project = self.project or self.homeProject
         count = 0
         while project:
             count += 1
             assert count < 4, (
                 project.projectRoot,
                 project.parentProject and project.parentProject.projectRoot,
             )
             candidate = project._find_git_repo(repoURL, revision)
-            if isinstance(candidate, GitRepo):
+            if isinstance(candidate, RepoView):
                 return candidate
             elif candidate != repoURL:
                 repoURL = candidate
             project = project.parentProject
         return repoURL
 
     def find_git_repo(
         self, repoURL: str, revision: Optional[str] = None
     ) -> Optional[GitRepo]:
         repo_or_url = self._find_git_repo(repoURL, revision)
         if isinstance(repo_or_url, str):
             return None
-        return repo_or_url
+        return repo_or_url.repo
 
     def _create_working_dir(self, repoURL, revision, basepath):
         project = self.project or self.homeProject
         if not project:
             logger.warning(
                 "Can not create clone repository, ensemble is not in an Unfurl project."
             )
@@ -1284,41 +1299,46 @@
     def find_or_create_working_dir(
         self,
         repoURL: str,
         revision: Optional[str] = None,
         basepath: Optional[str] = None,
         checkout_args: dict = {},
     ) -> Tuple[Optional[GitRepo], Optional[str], Optional[bool]]:
-        repo = self._find_git_repo(repoURL, revision)
-        if isinstance(repo, GitRepo):
+        repoview_or_url = self._find_git_repo(repoURL, revision)
+        if isinstance(repoview_or_url, RepoView):
+            repo = repoview_or_url.repo
+            assert repo
             logger.debug(
                 "Using existing repository at %s for %s", repo.working_dir, repoURL
             )
             if (
                 not self.overrides.get("UNFURL_SKIP_UPSTREAM_CHECK")
                 and not repo.is_dirty()
             ):
                 repo.pull(revision=revision)
         else:
             assert isinstance(
-                repo, str
-            ), repo  # it's the repoUrl (possibly rewritten) at this point
+                repoview_or_url, str
+            ), repoview_or_url  # it's the repoUrl (possibly rewritten) at this point
+            url = repoview_or_url
             # git-local repos must already exist locally
-            if repo.startswith("git-local://"):
+            if url.startswith("git-local://"):
                 return None, None, None
 
-            repo = self._create_working_dir(repo, revision, basepath)
+            repo = self._create_working_dir(url, revision, basepath)
             if not repo:
                 return None, None, None
 
         assert isinstance(repo, GitRepo)
         if revision:
             if repo.revision != repo.resolve_rev_spec(revision) or checkout_args:
                 if repo.is_dirty():
-                    logger.warning(f"{repo.working_dir} is dirty, skipping checking out revision {revision}")
+                    logger.warning(
+                        f"{repo.working_dir} is dirty, skipping checking out revision {revision}"
+                    )
                 else:
                     repo.checkout(revision, **checkout_args)
             return repo, repo.revision, False
         else:
             return repo, repo.revision, False
 
     def find_path_in_repos(
```

### Comparing `unfurl-0.6.2/unfurl/logs.py` & `unfurl-0.7.0/unfurl/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         Levels.VERBOSE: "white on bright_blue",
         Levels.DEBUG: "white on black",
         Levels.TRACE: "white on bright_black",
     }
 
     def emit(self, record: logging.LogRecord) -> None:
         message = self.format(record)
-        if not record.exc_info:
+        if not record.exc_info and not record.stack_info:
             truncate_length = getattr(record, "truncate", DEFAULT_TRUNCATE_LENGTH)
             if truncate_length:
                 message = truncate(message, truncate_length)
         # Hide meta job output because it seems to also be logged captured by
         # the root logger.
         if record.name.startswith(HIDDEN_MSG_LOGGER):
             return
```

### Comparing `unfurl-0.6.2/unfurl/lookup_plugins/unfurl.py` & `unfurl-0.7.0/unfurl/lookup_plugins/unfurl.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/manifest.py` & `unfurl-0.7.0/unfurl/manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,39 +4,40 @@
 import datetime
 import os.path
 import hashlib
 import json
 from typing import Dict, List, Optional, Any, Sequence, TYPE_CHECKING, cast
 from ruamel.yaml.comments import CommentedMap
 
-from .tosca import ToscaSpec, TOSCA_VERSION, ArtifactSpec
+from .tosca import EntitySpec, NodeSpec, ToscaSpec, TOSCA_VERSION, ArtifactSpec
 
 from .support import (
     ResourceChanges,
     AttributeManager,
     Status,
     Priority,
     NodeState,
     Imports,
 )
 from .runtime import (
+    EntityInstance,
     HasInstancesInstance,
     OperationalInstance,
     NodeInstance,
     CapabilityInstance,
     RelationshipInstance,
     ArtifactInstance,
     TopologyInstance,
 )
 from .util import UnfurlError, to_enum, sensitive_str, get_base_dir, taketwo
 from .repo import split_git_url, RepoView, GitRepo
 from .packages import Package, PackageSpec, PackagesType
 from .merge import merge_dicts
 from .result import ChangeRecord
-from .yamlloader import yaml, ImportResolver, yaml_dict_type
+from .yamlloader import yaml, ImportResolver, yaml_dict_type, SimpleCacheResolver
 from .logs import getLogger
 import toscaparser.imports
 from toscaparser.repositories import Repository
 
 if TYPE_CHECKING:
     from .localenv import LocalEnv
     from ansible.parsing.yaml.loader import AnsibleLoader
@@ -199,15 +200,15 @@
 
     def _ready(self, rootResource):
         """
         Set the instance model.
         """
         self.rootResource = rootResource
         if rootResource:
-            rootResource.attributeManager = self
+            rootResource.set_attribute_manager(self)
 
     def get_root_resource(self):
         return self.rootResource
 
     def get_base_dir(self):
         return "."
 
@@ -222,24 +223,37 @@
             and self.rootResource.templar
             and self.rootResource.templar._loader
         )
 
     def save_job(self, job):
         pass
 
-    def load_template(self, name, lastChange=None):
+    def load_error(self, msg: str) -> None:
+        if self.validate:
+            raise UnfurlError(msg)
+        else:
+            logger.error(msg)
+        return None
+
+    def load_template(
+        self, name: str, parent: Optional[EntityInstance], lastChange=None
+    ) -> Optional[EntitySpec]:
         if lastChange:
             return None
             # XXX implement revisions
             # try:
             #     return self.revisions.get_revision(lastChange).tosca.get_template(name)
             # except Exception:
             #     return None
+        elif parent:
+            return parent.template.get_template(name)
+        elif self.tosca:
+            return self.tosca.get_template(name)
         else:
-            return self.tosca and self.tosca.get_template(name)
+            return None
 
     #  load instances
     #    create a resource with the given template
     #  or generate a template setting interface with the referenced implementations
 
     @staticmethod
     def load_status(status, instance=None):
@@ -344,52 +358,95 @@
     #         workflow=spec.get("workflow", Defaults.workflow),
     #         inputs=spec.get("inputs"),
     #         inputSchema=spec.get("inputSchema"),
     #         preConditions=spec.get("preConditions"),
     #         postConditions=spec.get("postConditions"),
     #     )
 
-    def _create_requirement(self, key, val) -> Optional[RelationshipInstance]:
+    def _create_requirement(self, key, val, root) -> Optional[RelationshipInstance]:
         # parent will be the capability, should have already been created
         capabilityId = val.get("capability")
         if not capabilityId:
             nodeId = val.get("node")
             if not nodeId:
-                logger.warning(f"skipping requirement {key}: no node or capability specified")
+                logger.warning(
+                    f"skipping requirement {key}: no node or capability specified"
+                )
                 return None
-        capability = capabilityId and self.get_root_resource().query(capabilityId)
+        capability = capabilityId and root.query(capabilityId)
         if not capability or not isinstance(capability, CapabilityInstance):
-            raise UnfurlError(f"can not find capability {capabilityId}")
+            return self.load_error(f"can not find capability {capabilityId}")  # type: ignore
         if capability._relationships is None:
             capability._relationships = []
         return self._create_entity_instance(RelationshipInstance, key, val, capability)
 
-    def create_node_instance(self, rname, resourceSpec, parent=None) -> NodeInstance:
+    def _create_substituted_topology(
+        self, rname: str, resourceSpec: dict, parent: Optional[EntityInstance]
+    ) -> Optional[TopologyInstance]:
+        root = parent.root if parent else self.get_root_resource()
+        assert root
+        templateName = resourceSpec.get("template", rname)
+        template = cast(NodeSpec, self.load_template(templateName, parent))
+        if template is None:
+            return self.load_error(
+                f"missing template definition for '{templateName}' while instantiating instance '{rname}'"
+            )  # type: ignore
+        substitution = template.substitution
+        if substitution is None:
+            return self.load_error(  # type: ignore
+                f"missing substitution in template while instantiating instance '{rname}'"
+            )
+        status = resourceSpec["substitution"]
+        operational = self.load_status(status)
+        topology_instance = root.create_nested_topology(substitution, operational)
+        assert root.imports is not None
+        inner_name = (
+            substitution.substitution_node and substitution.substitution_node.name
+        )
+        for key, val in status.get("instances", {}).items():
+            self.create_node_instance(key, val, topology_instance)
+        if inner_name:
+            inner = topology_instance.find_instance(inner_name)
+            if inner:
+                root.imports.add_import(":" + inner.template.nested_name, inner)
+        return topology_instance
+
+    def create_node_instance(
+        self,
+        rname: str,
+        resourceSpec: Dict[str, Any],
+        parent: HasInstancesInstance,
+    ) -> NodeInstance:
         # if parent property is set it overrides the parent argument
+        root = parent.root
+        assert root
         pname = resourceSpec.get("parent")
         if pname:
-            parent = self.get_root_resource().find_resource(pname)
+            parent = root.find_instance(pname)  # type: ignore
             if parent is None:
-                raise UnfurlError(f"can not find parent instance {pname}")
+                self.load_error(f"can not find parent instance {pname} for {rname}")
+
+        if resourceSpec.get("substitution"):
+            # need to create the nested topology before a NodeInstance that has "imported"
+            self._create_substituted_topology(rname, resourceSpec, parent)
 
         resource = self._create_entity_instance(
             NodeInstance, rname, resourceSpec, parent
         )
         if resourceSpec.get("capabilities"):
             for key, val in resourceSpec["capabilities"].items():
                 self._create_entity_instance(CapabilityInstance, key, val, resource)
 
         if resourceSpec.get("requirements"):
             for req in resourceSpec["requirements"]:
                 key, val = next(iter(req.items()))
-                requirement = self._create_requirement(key, val)
+                requirement = self._create_requirement(key, val, root)
                 if not requirement:
                     continue
                 requirement._source = resource
-                # XXX investigate and re-enable this assert
                 assert (
                     requirement in resource.requirements
                 ), f"{requirement} not in {resource.requirements} for {rname}"
 
         if resourceSpec.get("artifacts"):
             for key, val in resourceSpec["artifacts"].items():
                 self._create_entity_instance(ArtifactInstance, key, val, resource)
@@ -403,36 +460,38 @@
         if not operational.last_config_change:
             return None
         if not self.changeSets:  # XXX load changesets if None
             return None
         jobId = ChangeRecord.get_job_id(operational.last_config_change)
         return self.changeSets.get(jobId)
 
-    def _create_entity_instance(self, ctor, name, status, parent):
+    def _create_entity_instance(
+        self, ctor, name: str, status: Dict[str, Any], parent: EntityInstance
+    ):
         templateName = status.get("template", name)
 
         imported = None
         importName = status.get("imported")
         if importName is not None:
             imported = self.imports.find_import(importName)
             if not imported:
-                raise UnfurlError(f"missing import {importName}")
+                self.load_error(f"missing import {importName}")
 
         if imported:
             operational = self.load_status(dict(readyState=imported.local_status))
         else:
             operational = self.load_status(status)
-        template = self.load_template(templateName)
+        template = self.load_template(templateName, parent)
         if template is None:
             # not defined in the current model any more, try to retrieve the old version
             if operational.last_config_change:
                 changerecord = self._get_last_change(operational)
-                template = self.load_template(templateName, changerecord)
+                template = self.load_template(templateName, parent, changerecord)
         if template is None:
-            raise UnfurlError(
+            return self.load_error(
                 f"missing template definition for '{templateName}' while instantiating instance '{name}'"
             )
         # logger.debug("creating instance for template %s: %s", templateName, template)
 
         # omit keys that match <<REDACTED>> so can we use the computed property
         attributes = {
             k: v
@@ -487,23 +546,22 @@
             repo = self.repo
             filePath = repo.find_repo_path(path)
             if filePath is not None:
                 return repo, filePath, repo.revision, False
         return None, None, None, None
 
     # NOTE: all the methods below may be called during config parse time via loadYamlInclude()
-    def find_repo_from_git_url(self, path, isFile, importLoader):
+    def find_repo_from_git_url(self, path, base):
         revision: Optional[str]
         repoURL, filePath, revision = split_git_url(path)
         if not repoURL:
             raise UnfurlError(f"invalid git URL {path}")
         assert self.localEnv
-        basePath = get_base_dir(importLoader.path)  # checks if dir or not
         repo, revision, bare = self.localEnv.find_or_create_working_dir(
-            repoURL, revision, basePath
+            repoURL, revision, base
         )
         return repo, filePath, revision, bare
 
     def add_repository(
         self, repo: Optional[GitRepo], toscaRepository: Repository, file_name: str
     ) -> RepoView:
         # add or replace the repository
@@ -660,25 +718,25 @@
             get_base_dir(baseDir),
             repositories=repositories,
             resolver=resolver,
         )
         import_spec = dict(
             file=artifactTpl["file"], repository=artifactTpl.get("repository")
         )
-        path, doc = loader._load_import_template(None, import_spec)
+        path, doc = loader.load_yaml(import_spec)
         if doc is None:
             logger.warning(
                 f"document include {templatePath} does not exist (base: {baseDir})"
             )
         return path, doc
 
     def get_import_resolver(
         self, ignoreFileNotFound=False, expand=False, config=None
     ) -> ImportResolver:
-        return ImportResolver(self, ignoreFileNotFound, expand, config)
+        return SimpleCacheResolver(self, ignoreFileNotFound, expand, config)
 
     def last_commit_time(self) -> Optional[datetime.datetime]:
         # return seconds (0 if not found)
         repo = self.repo
         if not repo:
             return None
         try:
```

### Comparing `unfurl-0.6.2/unfurl/merge.py` & `unfurl-0.7.0/unfurl/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,14 @@
     return factory
 
 
 # XXX?? because json keys are strings allow number keys to merge with lists
 # other values besides delete not supported because current code can leave those keys in final result
 mergeStrategyKey = "+%"  # supported values: "whiteout", "nullout", "merge", "error"
 
-# b is the merge patch, a is original dict
 def merge_dicts(
     b: Mapping,
     a: Mapping,
     cls=None,
     replaceKeys=None,
     defaultStrategy="merge",
     listStrategy="append_unique",
@@ -476,16 +475,16 @@
         templates.append(cp)
         while templates:
             cls = getattr(templates[0], "mapCtor", cls)
             accum = merge_dicts(accum, templates.pop(0), cls)
         return accum
     else:
         return cp
-    # e,g, mergeDicts(mergeDicts(a, b), cp)
-    # return includes, reduce(lambda accum, next: mergeDicts(accum, next, cls), templates, {}), cp
+    # e,g, merge_dicts(merge_dicts(a, b), cp)
+    # return includes, reduce(lambda accum, next: merge_dicts(accum, next, cls), templates, {}), cp
 
 
 def _find_missing_includes(includes):
     for x in includes.values():
         for i in x:
             if isinstance(i, _MissingInclude):
                 yield i
```

### Comparing `unfurl-0.6.2/unfurl/packages.py` & `unfurl-0.7.0/unfurl/packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,23 +84,25 @@
     url: Optional[str]
     revision: Optional[str]
 
 
 class PackageSpec:
     def __init__(
         self, package_spec: str, url: Optional[str], minimum_version: Optional[str]
-    ):
-        # url can be package, and url prefix, url with a revision or branch, #
+    ) -> None:
+        # url can be package id, a url prefix, or an url with a revision or branch
         self.package_spec = package_spec
         if url:
             self.package_id, self.url, revision = get_package_id_from_url(url)
         else:
             self.url = None
             self.package_id = None
+            revision = None
         self.revision = minimum_version or revision
+        self.lock_to_commit: str = ""
 
     def __str__(self):
         return f"PackageSpec({self.package_spec}:{self.package_id} {self.revision} {self.url})"
 
     def matches(self, package: "Package") -> bool:
         # * use the package name (or prefix) as the name of the repository to specify replacement or name resolution
         candidate = package.package_id
@@ -125,24 +127,26 @@
                 replaced_id = package.package_id
                 package.package_id = self.package_id.replace(
                     "*", package.package_id[len(self.package_spec) - 1 :]
                 )
                 package.url = ""
                 return replaced_id
             elif self.revision:
-                # if (only) the revsion was set and the package didn't set one itself, set it
+                # if (only) the revision was set and the package didn't set one itself, set it
                 if not package.revision:
                     package.revision = self.revision
                 return ""
             else:
                 # package_specs
                 raise UnfurlError(
                     f"Malformed package spec: {self.package_spec}: missing url or package id"
                 )
 
+        if self.lock_to_commit:
+            package.lock_to_commit = self.lock_to_commit
         if self.revision:
             package.revision = self.revision
         if self.url:
             package.url = self.url
         if self.package_id:
             replaced_id = package.package_id
             if replaced_id != self.package_id:
@@ -249,14 +253,15 @@
         self.package_id = package_id
         self.revision = minimum_version
         if url is None:
             self.set_url_from_package_id()
         self.url = cast(str, url)
         self.repositories: List[RepoView] = []
         self.discovered_revision = False
+        self.lock_to_commit = ""
 
     def __str__(self):
         return f"Package({self.package_id} {self.revision} {self.url})"
 
     def version_tag_prefix(self) -> str:
         # see https://go.dev/ref/mod#vcs-version
         url, repopath, urlrevision = split_git_url(self.url)
@@ -294,14 +299,21 @@
             return ""
         if not self.has_semver(True):
             return self.revision
         else:
             # since "^v" is in the semver regex, make sure don't end up with "vv"
             return self.version_tag_prefix() + self.revision.lstrip("v")
 
+    def is_mutable_ref(self) -> bool:
+        # is this package pointing to ref that could change?
+        return not self.lock_to_commit
+        # XXX if revision, see if its tag or branch
+        # treat tags immutable unless it looks like a non-exact semver tag:
+        # return not self.revision or self.has_semver() or self.revision_is_branch()
+
     def add_reference(self, repoview: RepoView) -> bool:
         if repoview not in self.repositories:
             self.repositories.append(repoview)
             repoview.package = self
             # we need to set the path, url, and revision to match the package
             if self.revision:
                 url, repopath, urlrevision = split_git_url(self.url)
```

### Comparing `unfurl-0.6.2/unfurl/plan.py` & `unfurl-0.7.0/unfurl/plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 # Copyright (c) 2020 Adam Souzis
 # SPDX-License-Identifier: MIT
-from typing import Dict, List, Optional
+from typing import Dict, Iterator, List, Optional, TYPE_CHECKING, Set, cast
 
-from .runtime import InstanceKey, NodeInstance, EntityInstance
+if TYPE_CHECKING:
+    from .job import JobOptions
+
+from .runtime import InstanceKey, NodeInstance, EntityInstance, TopologyInstance
 from .util import UnfurlError
 from .result import ChangeRecord
 from .support import Status, NodeState, Reason
 from .planrequests import (
     TaskRequest,
     TaskRequestGroup,
     SetStateRequest,
     JobRequest,
     create_task_request,
     filter_task_request,
     ConfigurationSpec,
     find_parent_resource,
     find_resources_from_template_name,
     _find_implementation,
-    get_success_status,
 )
-from .tosca import NodeSpec, Workflow, find_standard_interface, EntitySpec, ToscaSpec
+from .tosca import (
+    NodeSpec,
+    TopologySpec,
+    Workflow,
+    find_standard_interface,
+    EntitySpec,
+    ToscaSpec,
+)
 from .logs import getLogger
 
 
 logger = getLogger("unfurl")
 
 
 def is_external_template_compatible(
@@ -57,43 +66,48 @@
             run=RunNowPlan,
             check=ReadOnlyPlan,
             discover=ReadOnlyPlan,
         ).get(workflow, WorkflowPlan)
 
     interface: Optional[str] = None
 
-    def __init__(self, root, toscaSpec: ToscaSpec, jobOptions):
+    def __init__(
+        self, root: TopologyInstance, toscaSpec: ToscaSpec, jobOptions: "JobOptions"
+    ):
         self.jobOptions = jobOptions
         self.workflow = jobOptions.workflow
         self.root = root
         self.tosca = toscaSpec
         self._checked_connection_task = False
         assert self.tosca
         if jobOptions.template:
             filterTemplate = self.tosca.get_template(jobOptions.template)
             if not filterTemplate:
                 raise UnfurlError(
                     f"specified template not found: {jobOptions.template}"
                 )
-            self.filterTemplate = filterTemplate
+            self.filterTemplate: Optional[EntitySpec] = filterTemplate
         else:
             self.filterTemplate = None
 
-    def find_shadow_instance(self, template: EntitySpec, match=is_external_template_compatible):
+    def find_shadow_instance(
+        self, template: EntitySpec, match=is_external_template_compatible
+    ):
         imported = template.tpl.get("imported")
+        assert self.root.imports is not None
         if imported:
-            external = self.root.imports.find_import(imported)
-            if not external:
+            _external = self.root.imports.find_import(imported)
+            if not _external:
                 return None
-            if external.shadow and external.root is self.root:
+            if _external.shadow and _external.root is self.root:
                 # shadowed instance already created
-                return external
+                return _external
             else:
                 import_name = imported.partition(":")[0]
-                return self.create_shadow_instance(external, import_name, template)
+                return self.create_shadow_instance(_external, import_name, template)
 
         searchAll = []
         for name, record in self.root.imports.items():
             external = record.external_instance
             # XXX if external is a Relationship and template isn't, get it's target template
             #  if no target, create with status == unknown
 
@@ -104,22 +118,27 @@
                     return self.create_shadow_instance(external, name, template)
             if record.spec.get("instance") in ["root", "*"]:
                 # add root instance
                 searchAll.append((name, external))
 
         # look in the topologies where were are importing everything
         for name, root in searchAll:
-            for external in root.get_self_and_descendants():
-                if match(name, external.template, template):
-                    return self.create_shadow_instance(external, name, template)
+            for external_descendant in root.get_self_and_descendants():
+                if match(name, external_descendant.template, template):
+                    return self.create_shadow_instance(
+                        external_descendant, name, template
+                    )
 
         return None
 
-    def create_shadow_instance(self, external, import_name, template):
+    def create_shadow_instance(
+        self, external: EntityInstance, import_name: str, template: EntitySpec
+    ) -> EntityInstance:
         # create a local instance that "shadows" the external one we imported
+        assert self.root.imports is not None
         name = import_name + ":" + external.name
         instance_name = template.name
         # XXX import the parent too by creating a template and setting its name to name?
         parent = self.root
         logger.debug(
             "creating local instance %s for external instance %s",
             instance_name or name,
@@ -129,37 +148,65 @@
         shadowInstance = external.__class__(
             instance_name, {}, parent, template, external.status
         )
         shadowInstance.imported = name
         self.root.imports.set_shadow(name, shadowInstance, external)
         return shadowInstance
 
-    def find_resources_from_template(self, template):
+    def find_resources_from_template(self, template: EntitySpec):
         if template.abstract == "select":
             # XXX also match node_filter if present
             shadowInstance = self.find_shadow_instance(template)
             if shadowInstance:
                 logger.debug('found imported instance "%s"', shadowInstance.name)
                 yield shadowInstance
             else:
                 logger.warning(
                     "could not find external instance for template %s", template.name
                 )
             # XXX also yield newly created parents that needed to be checked?
         else:
-            for resource in find_resources_from_template_name(self.root, template.name):
+            if self.root.template.topology is not template.topology:
+                name = ":" + template.topology.nested_name
+                assert self.root.imports is not None
+                root = self.root.imports.find_import(name)
+                if not root:
+                    self.root.create_nested_topology(template.topology)
+                    return
+            else:
+                root = self.root
+            for resource in find_resources_from_template_name(root, template.name):
                 yield resource
 
-    def create_resource(self, template):
+    def create_resource(self, template: NodeSpec) -> NodeInstance:
         parent = find_parent_resource(self.root, template)
-        if self.jobOptions.check:
+        if self.jobOptions.check or "check" in template.directives:
             status = Status.unknown
         else:
             status = Status.pending
-        return NodeInstance(template.name, None, parent, template, status)
+        instance = NodeInstance(template.name, None, parent, template, status)
+        if template.substitution:
+            # set shadow to inner node instance
+            assert template.substitution.substitution_node
+            assert self.root.imports is not None
+            # get the nested TopologyInstance
+            nested_root_name = ":" + template.substitution.nested_name
+            nested_root = self.root.imports.find_import(nested_root_name)
+            assert nested_root, f"{nested_root_name} should already have been created"
+            name = template.substitution.substitution_node.name
+            inner = nested_root.find_instance(name)
+            assert (
+                inner
+            ), f"{name} in {nested_root_name} should have already been created before {instance.name}"
+            assert inner is not instance
+            instance.imported = (
+                ":" + template.substitution.substitution_node.nested_name
+            )
+            self.root.imports.set_shadow(instance.imported, instance, inner)
+        return instance
 
     def _run_operation(self, startState, op, resource, reason=None, inputs=None):
         req = create_task_request(
             self.jobOptions, op, resource, reason, inputs, startState
         )
         if req:
             yield req
@@ -480,15 +527,15 @@
             return None
         try:
             # push resource._workflow_inputs
             return self.execute_steps(workflow, steps, resource)
         finally:
             pass  # pop _workflow_inputs
 
-    def execute_steps(self, workflow: Workflow, steps: List, resource: EntityInstance):
+    def execute_steps(self, workflow: Workflow, steps: list, resource: EntityInstance):
         queue = steps[:]
         while queue:
             step = queue.pop()
             if not workflow.match_step_filter(step.name, resource):
                 logger.debug(
                     "step did not match filter %s with %s", step.name, resource.name
                 )
@@ -543,30 +590,22 @@
                 for req in filter(None, configGenerator):
                     reqGroup.add_request(req)
 
         # XXX  yield step.on_failure  # list of steps
         yield reqGroup
         yield step.on_success  # list of steps
 
-    def _get_templates(self):
-        templates = (
-            [] if not self.tosca.nodeTemplates else self.tosca.nodeTemplates.values()
-        )
-
+    def _get_templates(self) -> List[NodeSpec]:
+        assert self.tosca.topology
+        filter = self.filterTemplate and self.filterTemplate.name
+        seen: Set[NodeSpec] = set()
         # order by ancestors
         return list(
-            order_templates(
-                {
-                    t.name: t
-                    for t in templates
-                    if "virtual" not in t.directives
-                    and interface_requirements_ok(self.tosca, t)
-                },
-                self.filterTemplate and self.filterTemplate.name,
-                self.interface,
+            _get_templates_from_topology(
+                self.tosca.topology, seen, self.interface, filter
             )
         )
 
     def include_not_found(self, template):
         return True
 
     def is_last_workflow_op(self, taskrequest: TaskRequest) -> str:
@@ -581,34 +620,36 @@
 
         yields TaskRequests
         """
         opts = self.jobOptions
         templates = self._get_templates()
 
         logger.verbose(
-            "checking for tasks for templates %s", [t.name for t in templates]
+            "checking for tasks for templates %s", [t.nested_name for t in templates]
         )
         visited = set()
         for template in templates:
             found = False
             for resource in self.find_resources_from_template(template):
                 found = True
                 visited.add(id(resource))
                 yield from self._generate_workflow_configurations(resource, template)
 
-            if (
-                not found
-                and not template.abstract
-                and "dependent" not in template.directives
-            ):
+            if not found and "dependent" not in template.directives:
+                abstract = template.abstract
+                if abstract == "select":
+                    continue
                 include = self.include_not_found(template)
-                if include:
+                if include or abstract == "substitute":
                     resource = self.create_resource(template)
                     visited.add(id(resource))
-                    yield from self._generate_workflow_configurations(resource, None)
+                    if abstract != "substitute":
+                        yield from self._generate_workflow_configurations(
+                            resource, None
+                        )
 
         if opts.prune:
             # XXX warn or error if prune used with a filter option
             test = (
                 lambda resource: Reason.prune if id(resource) not in visited else False
             )
             yield from self.generate_delete_configurations(test)
@@ -618,15 +659,15 @@
     interface = "Standard"
 
     def include_not_found(self, template):
         if self.jobOptions.add or self.jobOptions.force:
             return Reason.add
         return None
 
-    def include_instance(self, template, instance):
+    def include_instance(self, template: EntitySpec, instance: EntityInstance):
         """Return whether or not the given instance should be included in the current plan,
         based on the current job's options and whether the template changed or the instance in need of repair?
 
         Args:
             template (EntitySpec): The template to be deployed.
             instance (EntityInstance): The instance as it last deployed.
 
@@ -654,21 +695,21 @@
                 if True:  # XXX if isMinorDifference(template, oldTemplate)
                     return Reason.update
                 elif jobOptions.upgrade:
                     return Reason.upgrade
 
         reason = self.check_for_repair(instance)
         # there isn't a new config to run, see if the last applied config needs to be re-run
-        if (
-            not reason
-            and (jobOptions.change_detection != "skip")
-            and instance.last_change
-        ):
+        if not reason:
+            if "check" in instance.template.directives:
+                instance.local_status = Status.unknown
+                return Reason.check
+            if jobOptions.change_detection != "skip" and instance.last_change:
             # XXX distinguish between "spec" and "evaluate" change_detection
-            return Reason.reconfigure
+                return Reason.reconfigure
         return reason
 
     def check_for_repair(self, instance):
         jobOptions = self.jobOptions
         assert instance
         if jobOptions.repair == "none":
             return None
@@ -826,22 +867,23 @@
             raise UnfurlError(f'workflow not found: "{self.jobOptions.workflow}"')
         for step in workflow.initial_steps():
             if self.filterTemplate and not self.filterTemplate.is_compatible_target(
                 step.target
             ):
                 continue
             if self.tosca.is_type_name(step.target):
-                templates = self.tosca.find_matching_templates(step.target)
+                templates = workflow.topology.find_matching_templates(step.target)
             else:
-                template = self.tosca.nodeTemplates.get(step.target)
+                template = workflow.topology.get_node_template(step.target)
                 if not template:
                     continue
                 templates = [template]
 
             for template in templates:
+                assert template
                 for resource in self.find_resources_from_template(template):
                     gen = self.execute_steps(workflow, [step], resource)
                     result = None
                     try:
                         while True:
                             configuration = gen.send(result)
                             result = yield configuration
@@ -876,36 +918,38 @@
         instanceFilter = self.jobOptions.instance
         if instanceFilter:
             resource = self.root.find_resource(instanceFilter)
             if not resource:
                 # see if there's a template with the same name and create the resource
                 template = self.tosca.get_template(instanceFilter)
                 if template:
+                    assert isinstance(template, NodeSpec)
                     resource = self.create_resource(template)
                 else:
                     raise UnfurlError(f"specified instance not found: {instanceFilter}")
             resources = [resource]
         else:
             resources = [self.root]
 
         # userConfig has the job options explicitly set by the user
-        operation = self.jobOptions.userConfig.get("operation")
+        operation = cast(Optional[str], self.jobOptions.userConfig.get("operation"))
         operation_host = self.jobOptions.userConfig.get("host")
         if not operation:
             configSpec = self._create_configurator(self.jobOptions.userConfig, "run")
         else:
             configSpec = None
             interface, sep, action = operation.rpartition(".")
             if not interface and find_standard_interface(operation):  # shortcut
                 operation = find_standard_interface(operation) + "." + operation
         for resource in resources:
             if configSpec:
                 req = TaskRequest(configSpec, resource, "run")
                 yield filter_task_request(self.jobOptions, req)
             else:
+                assert operation
                 req = create_task_request(
                     self.jobOptions,
                     operation,
                     resource,
                     Reason.run,
                     operation_host=operation_host,
                 )
@@ -944,47 +988,69 @@
                     template.name,
                     reqs,
                 )
                 return False
     return True
 
 
-def order_templates(templates: Dict[str, NodeSpec], filter=None, interface=None):
-    seen = set()
+def _get_templates_from_topology(
+    topology: TopologySpec, seen: Set[NodeSpec], interface, filter=None
+) -> Iterator[NodeSpec]:
+    templates = topology.node_templates.values()
+    # order by ancestors
+    return order_templates(
+        {
+            t.name: t
+            for t in templates
+            if "virtual" not in t.directives
+            and interface_requirements_ok(topology.spec, t)
+            and (not filter or t.name == filter)
+        },
+        seen,
+        interface,
+    )
+
+
+def order_templates(
+    templates: Dict[str, NodeSpec], seen: Set[NodeSpec], interface=None
+) -> Iterator[NodeSpec]:
     for source in templates.values():
-        if filter and source.name != filter:
-            continue
         if source in seen:
             continue
 
         if interface:
             for operation_host in find_explicit_operation_hosts(source, interface):
                 operationHostSpec = templates.get(operation_host)
                 if operationHostSpec:
                     if operationHostSpec in seen:
                         continue
                     seen.add(operationHostSpec)
                     yield operationHostSpec
 
-        for spec in get_ancestor_templates(source, templates):
-            if spec:
-                if spec is not source:
-                    # ancestor is required by source
-                    spec._isReferencedBy.append(source)  # type: ignore
-                if spec in seen:
-                    continue
-                seen.add(spec)
-                yield spec
+        for nodespec in get_ancestor_templates(source, templates):
+            if nodespec is not source:
+                # ancestor is required by source
+                nodespec._isReferencedBy.append(source)  # type: ignore
+            if nodespec in seen:
+                continue
+            seen.add(nodespec)
+            if nodespec.substitution:
+                yield from _get_templates_from_topology(
+                    nodespec.substitution, seen, interface
+                )
+            yield nodespec
 
 
-def get_ancestor_templates(source, templates):
+def get_ancestor_templates(
+    source: NodeSpec, templates: Dict[str, NodeSpec]
+) -> Iterator[NodeSpec]:
     if not source.abstract:
         # NodeTemplate.relationships return the node's requirements
         # (the opposite of NodeSpec.relationships)
-        for (rel, req, reqDef) in source.toscaEntityTemplate.relationships:
+        for rel, req, reqDef in source.toscaEntityTemplate.relationships:
             if rel.target is not source.toscaEntityTemplate:
                 target = rel.target and templates.get(rel.target.name)
                 if target:
                     for ancestor in get_ancestor_templates(target, templates):
                         yield ancestor
     yield source
```

### Comparing `unfurl-0.6.2/unfurl/planrequests.py` & `unfurl-0.7.0/unfurl/planrequests.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,29 +17,32 @@
     cast,
 )
 import shlex
 import sys
 import os
 import os.path
 
+from toscaparser.nodetemplate import NodeTemplate
+from .tosca import EntitySpec
+
 if TYPE_CHECKING:
     from .job import Job, ConfigTask, JobOptions
     from .configurator import Dependency
 
 from .util import (
     lookup_class,
     load_module,
     find_schema_errors,
     UnfurlError,
     UnfurlTaskError,
     to_enum,
 )
 from .result import Result, ResultsList, serialize_value
 from .support import Defaults, NodeState, Priority, Status
-from .runtime import EntityInstance, InstanceKey, HasInstancesInstance
+from .runtime import EntityInstance, InstanceKey, HasInstancesInstance, TopologyInstance
 from .logs import getLogger
 import logging
 
 logger = getLogger("unfurl")
 
 
 # we want ConfigurationSpec to be independent of our object model and easily serializable
@@ -429,39 +432,39 @@
             # the same global artifact can have different local names when declared on a node template
             # but are uniquely identified by (file, repository) so use that to generate a unique node template name
             name = "__artifact__" + artifact.get_name_from_artifact_spec(
                 artifact.as_import_spec()
             )
             operation_host = (
                 find_operation_host(self.target, self.configSpec.operation_host)
-                or self.target.root
+                or self.target.apex
             )
             existing = operation_host.root.find_instance(name)
             if existing:
                 if existing.operational:
                     return None
                 else:
                     return JobRequest([existing])
             else:
-                if not operation_host.template.spec.get_template(name):
+                if not operation_host.template.get_template(name):
                     # template isn't defined, define inline
                     artifact_tpl = artifact.toscaEntityTemplate.entity_tpl
                     template = dict(
                         name=name,
                         directives=["protected"],
                         type="unfurl.nodes.ArtifactInstaller",
                         artifacts={"install": artifact_tpl},
                     )
                     artifact_type = artifact_tpl["type"]
                     if (
                         artifact_type
-                        not in operation_host.template.spec.template.topology_template.custom_defs
+                        not in operation_host.template.topology.topology_template.custom_defs
                     ):
                         # operation_host must be in an external ensemble that doesn't have the type def
-                        artifact_type_def = self.target.template.spec.template.topology_template.custom_defs[
+                        artifact_type_def = self.target.template.topology.topology_template.custom_defs[
                             artifact_type
                         ]
                         template["custom_types"] = {artifact_type: artifact_type_def}
                 else:
                     template = name
 
                 return JobRequest(
@@ -750,15 +753,15 @@
 
 def _prepare_request(job: "Job", req: PlanRequest, errors: List) -> bool:
     if not isinstance(req, TaskRequest):
         return True
     if req.task:
         task = req.task
         task._attributeManager.attributes = {}
-        task.target.root.attributeManager = task._attributeManager
+        task.target.root.set_attribute_manager(task._attributeManager)
     else:
         task = req.task = job.create_task(req.configSpec, req.target, reason=req.reason)
     error = None
     try:
         task.set_envvars()
         proceed, msg = job.should_run_task(task)
         if not proceed:
@@ -798,15 +801,15 @@
     requests: Sequence[PlanRequest],
     check_target: str,
 ) -> Tuple[Optional[bool], Optional[UnfurlError]]:
     # req is a taskrequests, future_requests are (grouprequest, taskrequest) pairs
     assert req.task
     task = req.task
     task._attributeManager.attributes = {}
-    task.target.root.attributeManager = task._attributeManager
+    task.target.root.set_attribute_manager(task._attributeManager)
 
     error = None
     error_info = None
     try:
         task.logger.debug("rendering %s %s", task.target.name, task.name)
         task._rendering = True
         task.inputs
@@ -866,17 +869,17 @@
 
 
 def _add_to_req_list(reqs, request):
     if request not in reqs:
         reqs.append(request)
 
 
-def _reevaluate_not_required(not_required, render_requests):
+def _reevaluate_not_required(not_required: List[PlanRequest], render_requests) -> List[PlanRequest]:
     # keep rendering if a not_required template was referenced and is now required
-    new_not_required = []
+    new_not_required: List[PlanRequest] = []
     for request in not_required:
         if request.include_in_plan():
             request.target.validate()
             render_requests.append(request)
         else:
             new_not_required.append(request)
     return new_not_required
@@ -890,15 +893,15 @@
 ) -> Tuple[List[PlanRequest], List[PlanRequest], List[UnfurlError]]:
     ready: List[PlanRequest] = []
     notReady: List[PlanRequest] = []
     errors: List[UnfurlError] = []
     flattened_requests = list(
         r for r in get_render_requests(requests) if _prepare_request(job, r, errors)
     )
-    not_required = []
+    not_required: List[PlanRequest] = []
     render_requests = collections.deque(flattened_requests)
 
     notready_group = None
     while render_requests:
         request = render_requests.popleft()
         if request.completed:
             continue
@@ -961,15 +964,15 @@
             filterReason,
         )
         return None  # treat as filtered step
 
     return req
 
 
-def _find_implementation(interface, operation, template):
+def _find_implementation(interface: str, operation: str, template: EntitySpec):
     default = None
     for iDef in template.get_interfaces():
         if iDef.interfacename == interface or iDef.type == interface:
             if iDef.name == operation:
                 return iDef
     return default
 
@@ -977,62 +980,71 @@
 def find_resources_from_template_name(root: HasInstancesInstance, name: str):
     # XXX make faster
     for resource in root.get_self_and_descendants():
         if resource.template.name == name:
             yield resource
 
 
-def find_parent_template(source):
+def find_parent_template(source: NodeTemplate) -> Optional[NodeTemplate]:
     for rel, req, reqDef in source.relationships:
         # special case "host" so it can be declared without full set of relationship / capability types
         if rel.is_derived_from("tosca.relationships.HostedOn") or "host" in req:
             return rel.target
     return None
 
 
-def find_parent_resource(root, source):
-    parentTemplate = find_parent_template(source.toscaEntityTemplate)
+def find_parent_resource(root: TopologyInstance, source: EntitySpec) -> HasInstancesInstance:
+    source_nodetemplate = cast(NodeTemplate, source.toscaEntityTemplate)
+    parentTemplate = find_parent_template(source_nodetemplate)
+    source_root = root.get_root_instance(source_nodetemplate)
     if not parentTemplate:
-        return root
+        return source_root
+    root = root.get_root_instance(parentTemplate)
+    if root is not source_root:
+        # parent must be in the same topology
+        return source_root
     for parent in find_resources_from_template_name(root, parentTemplate.name):
         # XXX need to evaluate matches
         return parent
     raise UnfurlError(
         f"could not find parent instance {parentTemplate.name} for child {source.name}"
     )
 
 
-def create_instance_from_spec(_manifest, target, rname, resourceSpec):
+def create_instance_from_spec(_manifest, target: EntityInstance, rname: str, resourceSpec):
     pname = resourceSpec.get("parent")
     # get the actual parent if pname is a reserved name:
     if pname in [".self", "SELF"]:
         resourceSpec["parent"] = target.name
     elif pname == "HOST":
-        resourceSpec["parent"] = target.parent.name if target.parent else "root"
+        if target.parent:
+            resourceSpec["parent"] = target.parent.name
+        else:
+            resourceSpec["parent"] = "root"
 
     if isinstance(resourceSpec.get("template"), dict):
         # inline node template, add it to the spec
         tname = resourceSpec["template"].pop("name", rname)
-        nodeSpec = _manifest.tosca.add_node_template(tname, resourceSpec["template"])
+        nodeSpec = target.template.topology.add_node_template(tname, resourceSpec["template"])
         resourceSpec["template"] = nodeSpec.name
 
     if resourceSpec.get("readyState") and "created" not in resourceSpec:
         # setting "created" to the target's key indicates that
         # the target is responsible for deletion
         # if "created" is not defined, set it if readyState is set
         resourceSpec["created"] = target.key
 
     if "parent" not in resourceSpec and "template" in resourceSpec:
         tname = resourceSpec["template"]
-        nodeSpec = _manifest.tosca.get_template(tname)
+        nodeSpec = target.template.topology.get_template(tname)
         if not nodeSpec:
             raise UnfurlError(
                 f'Can not find template "{tname}" when trying to create instance "{rname}".'
             )
-        parent = find_parent_resource(target.root, nodeSpec)
+        parent = find_parent_resource(cast(TopologyInstance, target.root), nodeSpec)
     else:
         parent = target.root
     # note: if resourceSpec[parent] is set it overrides the parent keyword
     return _manifest.create_node_instance(rname, resourceSpec, parent=parent)
 
 
 def _maybe_mock(iDef, template):
```

### Comparing `unfurl-0.6.2/unfurl/projectpaths.py` & `unfurl-0.7.0/unfurl/projectpaths.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 
 import os.path
 import os
 import stat
 import shutil
 import codecs
 from collections.abc import MutableSequence
-from .eval import set_eval_func, map_value
+
+from .eval import RefContext, set_eval_func, map_value
 from .result import ExternalValue
 from .util import (
     UnfurlError,
     wrap_sensitive_value,
     save_to_tempfile,
     save_to_file,
 )
@@ -551,27 +552,31 @@
     :spec.home: Directory unique to the current instance's TOSCA template (committed to the spec repository).
     :spec.local: Local directory unique to the current instance's TOSCA template (excluded from repository).
     :project: The root directory of the current project.
     :unfurl.home: The location of home project (UNFURL_HOME).
 
     Otherwise look for a repository with the given name and return its path or None if not found.
     """
+    
     instance = ctx.currentResource
+    spec = instance.template and instance.template.spec
     if not name or name == ".":
         # the folder of the current resource's ensemble
         return instance.base_dir
     elif name == "src":
         # folder of the source file
         base_dir = getattr(ctx.kw, "base_dir", None)  # ctx.kw is the "eval:" dict
         if base_dir and os.path.isabs(base_dir):
             return base_dir
         if os.path.isabs(ctx.base_dir):
             return ctx.base_dir
-        else:  # XXX ctx.base_dir should be abs
+        elif instance.template:  # XXX ctx.base_dir should be abs
             return os.path.join(instance.template.base_dir, ctx.base_dir or "")
+        else:
+            return ctx.base_dir
     elif name == "tmp":
         return os.path.join(instance.root.tmp_dir, _get_instance_dir_name(instance))
     elif name in Folders.Persistent:
         return os.path.join(instance.base_dir, name, _get_instance_dir_name(instance))
     elif name in Folders.Job:
         # these will always in "planned" while a task is running
         if ctx.task and instance is ctx.task.target:
@@ -584,24 +589,26 @@
                 _get_instance_dir_name(instance),
             )
         else:
             assert (
                 False
             ), f"cant get_path {name}, {ctx.task and ctx.task.target.name} is not {instance.name}"
     elif name == "project":
-        return instance.template.spec._get_project_dir() or instance.base_dir
+        return spec and spec._get_project_dir() or instance.base_dir
     elif name == "unfurl.home":
-        return instance.template.spec._get_project_dir(True) or instance.base_dir
+        return spec and spec._get_project_dir(True) or instance.base_dir
     else:
+        template = instance.template
+        assert template
+        assert template.spec
         start, sep, rest = name.partition(".")
         if sep:
             if start == "spec":
-                template = instance.template
                 specHome = os.path.join(template.spec.base_dir, "spec", template.name)
                 if rest == "src":
                     return template.base_dir
                 if rest == "home":
                     return specHome
                 elif rest == "local":
                     return os.path.join(specHome, "local")
             # XXX elif start == 'project' and rest == 'local'
-        return instance.template.spec.get_repository_path(name)
+        return template.spec.get_repository_path(name)
```

### Comparing `unfurl-0.6.2/unfurl/repo.py` & `unfurl-0.7.0/unfurl/repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pathlib import Path
 import sys
 from functools import lru_cache
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union, cast
 from typing_extensions import Literal
 import git
 import git.exc
+from git.objects import Commit
 
 from .logs import getLogger, PY_COLORS
 from urllib.parse import urlparse
 from .util import UnfurlError, save_to_file
 from toscaparser.repositories import Repository
 from ruamel.yaml.comments import CommentedMap
 import logging
@@ -113,15 +114,25 @@
     RepoURL will be an empty string if it isn't a path to a git repo
     """
     if url.startswith("--"):
         # security: see https://github.com/gitpython-developers/GitPython/issues/1517
         return "", "", ""
     parts = urlparse(url)
     if parts.scheme == "git-local":
-        return parts.scheme + "://" + parts.netloc, parts.path[1:], parts.fragment
+        giturl, path, fragment = (
+            parts.scheme + "://" + parts.netloc,
+            parts.path[1:],
+            parts.fragment,
+        )
+        if fragment:
+            revision, sep, frag_path = parts.fragment.partition(":")
+            path = os.path.join(path, frag_path)
+        else:
+            revision = ""
+        return giturl, path, revision
 
     if parts.fragment:
         # treat fragment as a git revision spec; see https://git-scm.com/docs/gitrevisions
         # or https://docs.docker.com/engine/reference/commandline/build/#git-repositories
         # just support <ref>:<path> for now
         # e.g. myrepo.git#mybranch, myrepo.git#pull/42/head, myrepo.git#:myfolder, myrepo.git#master:myfolder
         revision, sep, path = parts.fragment.partition(":")
@@ -302,38 +313,41 @@
             raise UnfurlError(
                 f'couldn\'t create working directory, clone failed: "{err._cmdline}"\nTry re-running that command to diagnose the problem.'
             )
         Repo.ignore_dir(localRepoPath)
         return GitRepo(repo)
 
 
-def commit_secrets(working_dir, yaml):
+def commit_secrets(working_dir, yaml, repo: "GitRepo"):
     vault = yaml and getattr(yaml.representer, "vault", None)
     if not vault or not vault.secrets:
         return []
     saved = []
-    for filepath, dotsecrets in find_dirty_secrets(working_dir):
+    for filepath, dotsecrets in find_dirty_secrets(working_dir, repo):
         with open(filepath, "r") as vf:
             vaultContents = vf.read()
         encoding = None if vaultContents.startswith("$ANSIBLE_VAULT;") else "vault"
         secretpath = dotsecrets / filepath.name
         logger.verbose("encrypting file to %s with %s", secretpath, vault.secrets[0][0])
         save_to_file(str(secretpath), vaultContents, yaml, encoding)
         saved.append(secretpath)
     return saved
 
 
-def find_dirty_secrets(working_dir):
-    # compare .secrets with secrets
+def find_dirty_secrets(working_dir: str, repo: "GitRepo"):
     for root, dirs, files in os.walk(working_dir):
         if "secrets" not in Path(root).parts:
             continue
         for filename in files:
             dotsecrets = Path(root.replace("secrets", ".secrets"))
             filepath = Path(root) / filename
+            local_path = str((dotsecrets / filename).relative_to(working_dir))
+            if repo.is_path_excluded(local_path):
+                continue
+            # compare .secrets with secrets
             if (
                 not dotsecrets.is_dir()
                 or filename not in list([p.name for p in dotsecrets.iterdir()])
                 or filepath.stat().st_mtime > (dotsecrets / filename).stat().st_mtime
             ):
                 yield filepath, dotsecrets
 
@@ -352,49 +366,64 @@
             repository = Repository(name, tpl)
         assert repository or repo
         self.repository: Repository = repository
         self.yaml = None
         self.revision: Optional[str] = None
         self.file_refs: List[str] = []
         self.set_repo_and_path(repo, path)
+        self.read_only = False
         self.package: Optional[Union[Literal[False], "Package"]] = None
 
     def set_repo_and_path(self, repo: Optional["GitRepo"], path: str):
         self.repo = repo
         self.path = path
         if repo and path and self.repository:
             self.repository.url = repo.get_url_with_path(
                 path, False, self.revision or ""
             )
-        self.readOnly = not repo
 
     @property
     def working_dir(self) -> str:
         if self.repo:
             return os.path.join(self.repo.working_dir, self.path)
         else:
             return os.path.join(self.repository.url, self.path)
 
     @property
     def name(self):
         return self.repository.name if self.repository else ""
 
     @property
-    def url(self):
+    def url(self) -> str:
         if self.repository:
             url = self.repository.url
             if self.repository.credential:
                 credential = self.repository.credential
                 return add_user_to_url(url, credential["user"], credential["token"])
             else:
                 return url
         else:
             assert self.repo
             return self.repo.url
 
+    def as_git_url(self, sanitize=False) -> str:
+        hard = 2 if sanitize else 0
+        url, path, revision = split_git_url(self.url)
+        if self.package:
+            revision = self.package.revision_tag
+        else:
+            revision = self.revision or ""
+        return (
+            normalize_git_url(url, hard)
+            + "#"
+            + revision
+            + ":"
+            + os.path.join(path, self.path)
+        )
+
     def is_local_only(self):
         # if it doesn't have a repo then it most be local
         return not self.repo or self.repo.is_local_only()
 
     @property
     def origin(self):
         if (
@@ -402,26 +431,26 @@
             and normalize_git_url(self.repo.url) != split_git_url(self.url)[0]
             and self.repo.url != self.repo.working_dir
         ):
             return self.repo.url
         return ""
 
     def is_dirty(self):
-        if self.readOnly or not self.repo:
+        if self.read_only or not self.repo:
             return False
-        for filepath, dotsecrets in find_dirty_secrets(self.working_dir):
+        for filepath, dotsecrets in find_dirty_secrets(self.working_dir, self.repo):
             return True
         return self.repo.is_dirty(untracked_files=True, path=self.path)
 
     def add_file_ref(self, file_name: str):
         if file_name not in self.file_refs:
             self.file_refs.append(file_name)
 
     def add_all(self):
-        assert not self.readOnly and self.repo
+        assert not self.read_only and self.repo
         self.repo.repo.git.add("--all", self.path or ".")
 
     def load_secrets(self, _loader):
         logger.trace("looking for secrets %s", self.working_dir)
         for root, dirs, files in os.walk(self.working_dir):
             if ".secrets" not in Path(root).parts:
                 continue
@@ -444,40 +473,39 @@
                         os.makedirs(dir)
                     with open(target_path, "w") as f:
                         f.write(contents)
                     os.utime(target, (stinfo.st_atime, stinfo.st_mtime))
                     logger.verbose("decrypted secret file to %s", target)
 
     def save_secrets(self):
-        return commit_secrets(self.working_dir, self.yaml)
+        assert self.repo
+        return commit_secrets(self.working_dir, self.yaml, self.repo)
 
     def commit(self, msg: str, add_all: bool = False) -> int:
-        assert not self.readOnly
+        assert not self.read_only
         assert self.repo
         if self.yaml:
             for saved in self.save_secrets():
                 local_path = str(saved.relative_to(self.repo.working_dir))
-                if not self.repo.is_path_excluded(local_path):
-                    self.repo.repo.git.add(local_path)
+                self.repo.repo.git.add(local_path)
         if add_all:
             self.add_all()
         self.repo.repo.index.commit(msg)
         return 1
 
     def git_status(self):
-        assert not self.readOnly
         assert self.repo
         return self.repo.run_cmd(["status", self.path or "."])[1]
 
     def _secrets_status(self):
         assert self.repo
         modified = "\n   ".join(
             [
                 str(filepath.relative_to(self.repo.working_dir))
-                for filepath, dotsecrets in find_dirty_secrets(self.working_dir)
+                for filepath, dotsecrets in find_dirty_secrets(self.working_dir, self.repo)
             ]
         )
         if modified:
             return f"\n\nSecrets to be committed:\n   {modified}"
         return ""
 
     def get_repo_status(self, dirty=False):
@@ -493,30 +521,39 @@
             return ""
 
     def get_initial_revision(self):
         if not self.repo:
             return ""
         return self.repo.get_initial_revision()
 
-    def get_current_revision(self):
+    def get_current_commit(self):
         if not self.repo:
             return ""
         if self.is_dirty():
             return self.repo.revision + "-dirty"
         else:
             return self.repo.revision
 
-    def lock(self):
+    def lock(self) -> CommentedMap:
         record = CommentedMap(
             [
                 ("url", normalize_git_url(self.url, 1)),
-                ("revision", self.get_current_revision()),
+                ("commit", self.get_current_commit()),
                 ("initial", self.get_initial_revision()),
             ]
         )
+        if self.package and self.package.revision:
+            # intended revision (branch or tag) declared by user
+            record["revision"] = self.package.revision
+        if self.repo and self.repo.active_branch:
+            # current commit is on this branch
+            record["branch"] = self.repo.active_branch
+        if self.repo and self.repo.current_tag:
+            # current commit is on this tag
+            record["tag"] = self.repo.current_tag
         if self.name:
             record["name"] = self.name
         if self.origin:
             record["origin"] = normalize_git_url(self.origin, 1)
         return record
 
 
@@ -567,30 +604,47 @@
         dir = str(dir)
         if dir[-1] == "/":
             return dir
         else:
             return dir + "/"
 
     @property
-    def revision(self):
+    def revision(self) -> str:
         if not self.repo.head.is_valid():
             return ""
         return self.repo.head.commit.hexsha
 
     @property
     def remote(self) -> Optional[git.Remote]:
         gitrepo = self.repo
         if gitrepo.remotes:
-            # note: these might not look like absolute urls, e.g. git@github.com:onecommons/unfurl.git
             try:
                 return gitrepo.remotes["origin"]
             except Exception:
                 return gitrepo.remotes[0]
         return None
 
+    @property
+    def active_branch(self) -> str:
+        try:
+            return self.repo.active_branch.name
+        except Exception:
+            # no head or detached
+            return ""
+
+    @property
+    def current_tag(self) -> str:
+        try:
+            return self.repo.git.describe(self.repo.heads[0].object, exact_match=True)
+        except Exception:
+            # e.g.:
+            # git.exc.GitCommandError: Cmd('git') failed due to: exit code(128)
+            #   stderr: 'fatal: no tag exactly matches 'ed915a383336a085eaabeb8f2a461e656ec8a5c9''
+            return ""
+
     def resolve_rev_spec(self, revision):
         try:
             return self.repo.commit(revision).hexsha
         except Exception:
             return None
 
     def get_url_with_path(self, path: str, sanitize: bool = False, revision: str = ""):
@@ -655,22 +709,24 @@
         if not os.path.exists(path):
             os.makedirs(path)
         exclude_path = os.path.join(path, "exclude")
         with open(exclude_path, "a") as f:
             f.write("\n" + rule + "\n")
         return exclude_path
 
-    def show(self, path, commitId):
+    def show(self, path, commitId, stdout_as_string=True):
         if self.working_dir and os.path.isabs(path):
             path = os.path.abspath(path)[len(self.working_dir) :]
         # XXX this won't work if path is in a submodule
         # if in path startswith a submodule: git log -1 -p [commitid] --  [submodule]
         # submoduleCommit = re."\+Subproject commit (.+)".group(1)
         # return self.repo.submodules[submodule].git.show(submoduleCommit+':'+path[len(submodule)+1:])
-        return self.repo.git.show(commitId + ":" + path)
+        return self.repo.git.show(
+            commitId + ":" + path, stdout_as_string=stdout_as_string
+        )
 
     def checkout(self, revision="", **kw):
         # if revision isn't specified and repo is not pinned:
         #  save the ref of current head
         self.repo.git.checkout(revision, **kw)
         logger.info(
             "checking out '%s' at %s to %s",
@@ -696,30 +752,30 @@
         firstCommit = next(self.repo.iter_commits("HEAD", max_parents=0))
         return firstCommit.hexsha
 
     def add_all(self, path="."):
         path = os.path.relpath(path, self.working_dir)
         self.repo.git.add("--all", path)
 
-    def commit_files(self, files, msg):
+    def commit_files(self, files: List[str], msg: str) -> Commit:
         # note: this will also commit existing changes in the index
         index = self.repo.index
         index.add([os.path.abspath(f) for f in files])
         return index.commit(msg)
 
-    def is_dirty(self, untracked_files=False, path=None):
+    def is_dirty(self, untracked_files=False, path: Optional[str] = None) -> bool:
         # diff = self.repo.git.diff()  # "--abbrev=40", "--full-index", "--raw")
         # https://gitpython.readthedocs.io/en/stable/reference.html?highlight=is_dirty#git.repo.base.Repo.is_dirty
         return self.repo.is_dirty(untracked_files=untracked_files, path=path or None)
 
     def pull(
         self, remote="origin", revision=None, ff_only=True, with_exceptions=False, **kw
     ) -> bool:
         if remote in self.repo.remotes:
-            cmd = ["pull", remote, revision or "HEAD", "--tags"]
+            cmd = ["pull", remote, revision or "HEAD", "--tags", "--update-shallow"]
             if ff_only:
                 cmd.append("--ff-only")
             code, out, err = self.run_cmd(cmd, with_exceptions=with_exceptions, **kw)
             if code:
                 logger.info(
                     "attempt to pull latest from %s %s into %s failed: %s %s",
                     sanitize_url(self.url, True),
@@ -738,19 +794,40 @@
                     out,
                     err,
                 )
                 return True
         else:
             return False
 
-    def push(self, url: Optional[str] = None) -> None:
+    def _push(self, url: Optional[str] = None, **kw) -> None:
         if url:
-            self.run_cmd(["push", url], with_exceptions=True)
+            self.run_cmd(["push", url], with_exceptions=True, **kw)
         elif self.remote:
-            self.remote.push().raise_if_error()
+            self.remote.push(**kw).raise_if_error()
+
+    def push(self, url: Optional[str] = None, pull_on_rejected=True, **kw) -> None:
+        try:
+            self._push(url, **kw)
+        except git.exc.GitCommandError as e:  # type: ignore
+            retry = pull_on_rejected and (
+                not url
+                # pull() doesn't support alternative urls
+                or normalize_git_url_hard(url) == normalize_git_url_hard(self.url)
+            )
+            if retry and "[rejected]" in e.stderr:
+                self.pull(
+                    ff_only=False,
+                    no_rebase=True,
+                    commit=True,
+                    no_edit=True,
+                    with_exceptions=True,
+                )
+                self._push(url, **kw)
+            else:
+                raise e
 
     def clone(self, newPath):
         # note: repo.clone uses bare path, which breaks submodule path resolution
         cloned = git.Repo.clone_from(
             self.working_dir, os.path.abspath(newPath), recurse_submodules=True
         )
         Repo.ignore_dir(newPath)
```

### Comparing `unfurl-0.6.2/unfurl/reporting.py` & `unfurl-0.7.0/unfurl/reporting.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
                     nodeStr = f'Job for "{request.name}":'
                     output.append(" " * indent + nodeStr)
                     continue
                 if not job.is_filtered() and job.jobOptions.workflow == "deploy":
                     if not request.include_in_plan():
                         logger.trace(
                             'excluding "%s" from plan: not required',
-                            request.target.name,
+                            request.target.template.nested_name,
                         )
                         continue
                 if request.target is not target:
                     target = request.target
                     assert target
                     status = ", ".join(
                         filter(
@@ -250,15 +250,15 @@
                             (
                                 target.status.name if target.status is not None else "",  # type: ignore
                                 target.state.name if target.state is not None else "",  # type: ignore
                                 "managed" if target.created else "",  # type: ignore
                             ),
                         )
                     )
-                    nodeStr = f'Node "{target.name}" ({status}):'  # type: ignore
+                    nodeStr = f'Node "{target.template.nested_name}" ({status}):'  # type: ignore
                     output.append(" " * indent + nodeStr)
                 if isGroup:
                     output.append(
                         "%s- %s:" % (" " * indent, (request.workflow or "sequence"))  # type: ignore
                     )
                     _summary(request.children, target, indent + INDENT)  # type: ignore
                 else:
```

### Comparing `unfurl-0.6.2/unfurl/result.py` & `unfurl-0.7.0/unfurl/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,26 +80,28 @@
         ctor = sensitive_list if isSensitive else list
         return ctor(serialize_value(item, **kw) for item in value)
     else:
         return value
 
 
 class ResourceRef(ABC):
-
     parent = None  # must be defined by subclass
     template: Optional["EntitySpec"] = None
-    base_dir = ""
     name = ""
 
     @abstractmethod
     def _resolve(self, key):
         ...
 
     _templar: Optional["Templar"] = None
 
+    @property
+    def base_dir(self) -> str:
+        return ""
+
     def _get_prop(self, name):
         if name == ".":
             return self
         elif name == "..":
             return self.parent
         name = name[1:]
         # XXX3 use propmap
@@ -726,15 +728,14 @@
         self._deleted.pop(key, None)
 
     def __delitem__(self, index):
         if self.context.currentResource.readonly:
             raise UnfurlError(
                 "Attempting to delete item {item} on a readonly instance {self.context.currentResource}"
             )
-        self.context.currentResource.name
         val = self._attributes[index]
         self._deleted[index] = val
         del self._attributes[index]
 
     def __len__(self):
         return len(self._attributes)
```

### Comparing `unfurl-0.6.2/unfurl/runtime.py` & `unfurl-0.7.0/unfurl/runtime.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     AnyStr,
 )
 from collections.abc import Mapping
 
 from ansible.parsing.dataloader import DataLoader
 
 from .util import UnfurlError, load_class, to_enum, make_temp_dir, ChainMap
-from .result import ResourceRef, ChangeAware
+from .result import ResourceRef, ChangeAware, ResultsMap
 
 from .support import (
     AttributeManager,
     Defaults,
     Imports,
     Status,
     Priority,
@@ -43,14 +43,15 @@
     CapabilitySpec,
     RelationshipSpec,
     NodeSpec,
     TopologySpec,
     ArtifactSpec,
 )
 from .logs import getLogger
+from toscaparser.nodetemplate import NodeTemplate
 
 if TYPE_CHECKING:
     from unfurl.configurator import Dependency
     import toscaparser.repositories
     from .yamlmanifest import YamlManifest
 
 
@@ -84,42 +85,60 @@
 
     def has_state(self, state: NodeState) -> bool:
         if state == NodeState.initial:
             return True
         if self.state is None:
             # self.state is sometimes None even though it shouldn't be
             return False
-        if state == NodeState.error:
+        if state == NodeState.error or self.state == NodeState.error:
             return self.state == state
         if state < NodeState.stopping:
-            return self.state < NodeState.stopping and self.state >= state
+            if self.state < NodeState.stopping:
+                # progressive states on both sides
+                return self.state >= state
+            elif self.state in [NodeState.stopping, NodeState.stopped]:
+                if state < NodeState.starting:
+                    # created, configured, etc. still true even if node is stopped
+                    return True
+            else:
+                assert (
+                    self.state
+                    in [NodeState.deleting, NodeState.deleted]
+                    and state < NodeState.stopping
+                ), (self.state.name, state.name)
+                return False
         if self.state > NodeState.stopping:
+            assert state >= NodeState.stopping
             return self.state >= state
         return False
 
     def get_operational_dependencies(self) -> Iterable["Operational"]:
         """
         Return an iterator of `Operational` object that this instance depends on to be operational.
         """
         return ()  # type: ignore  # mypy doesn't like empty tuples
 
     def get_operational_dependents(self) -> List["Operational"]:  # type: ignore
         return ()  # type: ignore  # mypy doesn't like empty tuples
 
     @property
-    def manual_overide_status(self) -> None:
+    def manual_override_status(self) -> None:
         return None
 
     # derived properties:
     @property
     def operational(self) -> bool:
         return self.status == Status.ok or self.status == Status.degraded
 
     @property
     def active(self) -> bool:
+        # if task.target.has_state(NodeState.created):
+        # unknown, ok, degraded
+        if self.state and self.state > NodeState.initial:
+            return self.has_state(NodeState.created)
         return self.status <= Status.error
 
     @property
     def present(self) -> bool:
         return self.operational or self.status == Status.error
 
     @property
@@ -132,16 +151,16 @@
         then the aggregate status' of its dependencies (see `aggregate_status()`
         and `get_operational_dependencies()`).
 
         If the local_status is non-operational, that takes precedence.
         Otherwise the local_status is compared with its aggregate dependent status
         and worser value is choosen.
         """
-        if self.manual_overide_status is not None:
-            status = self.manual_overide_status
+        if self.manual_override_status is not None:
+            status = self.manual_override_status
             if status >= Status.error:
                 return status
         else:
             status = self.local_status
 
         if not status:
             return Status.unknown
@@ -303,26 +322,26 @@
         def fdel(self: "OperationalInstance") -> None:
             del self._localStatus
 
         return locals()
 
     local_status: Optional[Status] = property(**__local_status())  # type: ignore
 
-    def __manual_overide_status() -> Dict[str, Any]:  # type: ignore
+    def __manual_override_status() -> Dict[str, Any]:  # type: ignore
         doc = "The manualOverideStatus property."
 
         def fget(self: "OperationalInstance") -> Optional[Status]:
             return self._manualOverideStatus
 
         def fset(self: "OperationalInstance", value: Status) -> None:
             self._manualOverideStatus = value
 
         return locals()
 
-    manual_overide_status: Optional[Status] = property(**__manual_overide_status())  # type: ignore
+    manual_override_status: Optional[Status] = property(**__manual_override_status())  # type: ignore
 
     def __priority():  # type: ignore
         doc = "The priority property."
 
         def fget(self: "OperationalInstance") -> Optional[Priority]:
             return self._priority
 
@@ -370,15 +389,15 @@
 
 
 class EntityInstance(OperationalInstance, ResourceRef):
     attributeManager: Optional[AttributeManager] = None
     created: Optional[Union[bool, str]] = None
     protected: Optional[bool] = None
     imports: Optional[Imports] = None
-    imported = None
+    imported: Optional[str] = None
     _baseDir = ""
     templateType = EntitySpec  # must defined by subtype
     parentRelation = ""
 
     def __init__(
         self, name="", attributes=None, parent=None, template=None, status=Status.ok
     ):
@@ -515,50 +534,62 @@
         return manifest.deployment if manifest else ""
 
     @property
     def artifacts(self):
         return {}
 
     @property
-    def attributes(self):
+    def attributes(self) -> ResultsMap:
         """attributes are live values but _attributes will be the serialized value"""
         if not self.root.attributeManager:
             if not self.attributeManager:
                 # inefficient but create a local one for now
                 self.attributeManager = AttributeManager()
-            # XXX3 changes to self.attributes aren't saved
             return self.attributeManager.get_attributes(self)
 
         # returned registered attribute or create a new one
         # attribute class getter resolves references
         return self.root.attributeManager.get_attributes(self)
 
     @property
     def names(self):
         return self.attributes
 
-    def get_default_relationships(self, relation=None):
+    def get_default_relationships(self, relation=None) -> List["RelationshipInstance"]:
         return self.root.get_default_relationships(relation)
 
     @property
-    def shadow(self):
+    def shadow(self) -> Optional["EntityInstance"]:
         if self.imported:
             imports = self.root.imports
             if imports and self.imported in imports:
                 return imports[self.imported].external_instance
             else:
                 raise UnfurlError(
                     f'could not find imported instance "{self.imported}" for local instance "{self.name}"'
                 )
         return None
 
     @property
+    def nested_name(self) -> str:
+        if self.template.topology.substitute_of:
+            return self.template.topology.substitute_of.nested_name + ":" + self.name
+        return self.name
+
+    @property
     def readonly(self) -> bool:
         return bool(self.imported)  # imported instances are readonly
 
+    @property
+    def apex(self):
+        if isinstance(self.root, TopologyInstance):
+            if self.root.parent_topology:  # type: ignore
+                return cast(TopologyInstance, self.root.parent_topology).apex  # type: ignore
+        return self.root
+
     def validate(self) -> None:
         """
         Raises UnfurlValidationError on failure.
         """
         if self.shadow:
             self.shadow.validate()
         elif self.template:
@@ -633,29 +664,41 @@
 
     @property
     def descendents(self):
         # backward compatibility
         return self.descendants
 
     # XXX use find_instance instead and remove find_resource
-    def find_resource(self, resourceid):
+    def find_resource(self, qualified_name) -> Optional["HasInstancesInstance"]:
+        resourceid, sep, inner = qualified_name.partition(":")
         if self.name == resourceid:
+            if inner:
+                if self.shadow:
+                    return self.shadow.root.find_resource(inner)
+                return None
             return self
         for r in self.instances:
             child = r.find_resource(resourceid)
             if child:
+                if inner:
+                    if child.shadow:
+                        return child.shadow.root.find_resource(inner)
+                    return None
                 return child
         return None
 
     find_instance = find_resource
 
     def find_instance_or_external(self, resourceid):
         instance = self.find_instance(resourceid)
         if instance:
             return instance
+        instance = self.apex.find_instance(resourceid)
+        if instance:
+            return instance
         if self.imports:
             return self.imports.find_import(resourceid)
         return None
 
     @property
     def requirements(self) -> List["RelationshipInstance"]:
         return []
@@ -685,15 +728,15 @@
 
 # both have occurrences
 # only need to configure capabilities as required by a relationship
 class CapabilityInstance(EntityInstance):
     # 3.7.2 Capability definition p. 97
     # 3.8.1 Capability assignment p. 114
     parentRelation = "_capabilities"
-    templateType = CapabilitySpec
+    templateType = CapabilitySpec  # type: ignore
     _relationships: Optional[List["RelationshipInstance"]] = None
 
     @property
     def relationships(self) -> List["RelationshipInstance"]:
         if self._relationships is None:
             self._relationships = []
         assert isinstance(self.template, CapabilitySpec)
@@ -746,15 +789,17 @@
         else:
             return None
 
     @property
     def source(self) -> Optional["NodeInstance"]:
         if self._source is None:
             if self.template.source:
-                sourceNode = self.root.find_instance(self.template.source.name)
+                sourceNode = self.root.get_root_instance(
+                    self.template.source.toscaEntityTemplate
+                ).find_instance(self.template.source.name)
                 if sourceNode:
                     self._source = sourceNode
         return self._source
 
     @property
     def capability(self) -> Optional[CapabilityInstance]:
         return self.parent
@@ -816,20 +861,14 @@
     def file(self):
         return self.template.file
 
     @property
     def repository(self) -> Optional["toscaparser.repositories.Repository"]:
         return self.template.repository
 
-    def get_path(self, resolver=None):
-        return self.template.get_path_and_fragment(resolver)
-
-    def get_path_and_fragment(self, resolver=None, tpl=None):
-        return self.template.get_path_and_fragment(resolver, tpl)
-
     def as_import_spec(self):
         return self.template.as_import_spec()
 
     def get_operational_dependencies(self):
         # skip dependency on the parent
         for d in self.dependencies:
             yield d
@@ -851,36 +890,41 @@
             if parent.root.find_resource(name):
                 raise UnfurlError(
                     f'can not create node instance "{name}", its name is already in use'
                 )
 
         # next three may be initialized either by Manifest.createNodeInstance or by its property
         self._capabilities = []
-        self._requirements = []
+        self._requirements: List["RelationshipInstance"] = []
         self._artifacts = []
         self._named_artifacts = None
         HasInstancesInstance.__init__(self, name, attributes, parent, template, status)
 
         self._interfaces = {}
         # preload
         self.get_interface("inherit")
         self.get_interface("default")
 
-    def _find_relationship(self, relationship) -> Optional[RelationshipInstance]:
+    def _find_relationship(
+        self, relationship: RelationshipSpec
+    ) -> Optional[RelationshipInstance]:
         """
         Find RelationshipInstance that has the give relationship template
         """
         assert relationship and relationship.capability and relationship.target
         # find the Capability instance that corresponds to this relationship template's capability
-        targetNodeInstance = self.root.find_resource(relationship.target.name)
+        targetNodeInstance = self.root.get_root_instance(
+            relationship.target.toscaEntityTemplate
+        ).find_resource(relationship.target.name)
         if not targetNodeInstance:
             logger.warning(
-                f"target instance {relationship.target.name} should have already been created -- is {self.name} out of sync with latest templates?"
+                f'target instance "{relationship.target.nested_name}" should have already been created -- is "{self.name}" out of sync with latest templates?'
             )
             return None
+        assert isinstance(targetNodeInstance, NodeInstance)
         for cap in targetNodeInstance.capabilities:
             if cap.template is relationship.capability:
                 for relInstance in cap.relationships:
                     if relInstance.template is relationship:
                         return relInstance
         return None
 
@@ -897,16 +941,29 @@
                 if id(template.relationship) not in instantiated:
                     relInstance = self._find_relationship(template.relationship)
                     if not relInstance:
                         logger.warning(
                             f'can not find relation instance for requirement "{name}" on node "{self.name}"'
                         )
                         continue
-                    assert template.relationship is relInstance.template
-                    assert self.template is relInstance.template.source
+                    assert template.relationship is relInstance.template, (
+                        template.relationship,
+                        relInstance.template,
+                    )
+                    assert relInstance.template.source
+                    assert (
+                        self.template is relInstance.template.source
+                        or self.template.topology.substitute_of
+                        is relInstance.template.source
+                        or self.template
+                        is relInstance.template.source.topology.substitute_of
+                    ), (
+                        self.template,
+                        relInstance.template.source,
+                    )
                     self._requirements.append(relInstance)
 
         return self._requirements
 
     @property
     def capabilities(self) -> List[CapabilityInstance]:
         if len(self._capabilities) != len(self.template.capabilities):
@@ -961,15 +1018,15 @@
         if self.root is self:
             return
         for rel in self.root.get_default_relationships(relation):
             for capability in self.capabilities:
                 if rel.template.matches_target(capability.template):
                     yield rel
 
-    def get_default_relationships(self, relation=None):
+    def get_default_relationships(self, relation=None) -> List[RelationshipInstance]:
         return list(self._get_default_relationships(relation))
 
     @property
     def sources(self):
         dep: Dict[str, Union[EntityInstance, List[EntityInstance]]] = {}
         for cap in self.capabilities:
             for rel in cap.relationships:
@@ -1087,47 +1144,60 @@
         return None
 
     def __repr__(self):
         return f"NodeInstance('{self.name}')"
 
 
 class TopologyInstance(HasInstancesInstance):
-    templateType = TopologySpec
+    templateType = TopologySpec  # type: ignore
 
-    def __init__(self, template, status=None):
+    def __init__(
+        self,
+        template: "TopologySpec",
+        status=None,
+        parent_topology: Optional["TopologyInstance"] = None,
+    ):
         attributes = dict(inputs=template.inputs, outputs=template.outputs)
         HasInstancesInstance.__init__(self, "root", attributes, None, template, status)
 
-        self._relationships = None
-        self._tmpDir = None
+        self._relationships: Optional[List["RelationshipInstance"]] = None
+        self._tmpDir: Optional[str] = None
+        self.parent_topology = parent_topology
 
-    def set_base_dir(self, baseDir):
+    def set_base_dir(self, baseDir: str) -> None:
         self._baseDir = baseDir
         if not self._templar or self._templar._basedir != baseDir:
             loader = DataLoader()
             loader.set_basedir(baseDir)
             self._templar = Templar(loader)
 
+    def set_attribute_manager(
+        self, attribute_manager: Optional[AttributeManager]
+    ) -> None:
+        self.attributeManager = attribute_manager
+        if self.parent_topology:
+            self.parent_topology.set_attribute_manager(attribute_manager)
+
     @property
     def requirements(self) -> List[RelationshipInstance]:
         """
         The root node returns RelationshipInstances representing default relationship templates
         """
         if self._relationships is None:
             self._relationships = []
-            relTemplates = self.template.spec.relationshipTemplates
-            for name, template in relTemplates.items():
-                # template will be a RelationshipSpec
-                if template.toscaEntityTemplate.default_for:
-                    # the constructor will add itself to _relationships
-                    RelationshipInstance(name, parent=self, template=template)
+            relTemplates = cast(TopologySpec, self.template).default_relationships
+            for template in relTemplates:
+                # this constructor will add itself to _relationships
+                RelationshipInstance(template.name, parent=self, template=template)
 
         return self._relationships
 
-    def get_default_relationships(self, relation=None):
+    def get_default_relationships(
+        self, relation: Optional[str] = None
+    ) -> List[RelationshipInstance]:
         # for root, this is the same as self.requirements
         if not relation:
             return self.requirements
         return [
             rel
             for rel in self.requirements
             if rel.template.is_compatible_type(relation)
@@ -1138,7 +1208,31 @@
             yield instance
 
     @property
     def tmp_dir(self):
         if not self._tmpDir:
             self._tmpDir = make_temp_dir()
         return self._tmpDir
+
+    def create_nested_topology(
+        self, topology: TopologySpec, status=None
+    ) -> "TopologyInstance":
+        nested_root = TopologyInstance(topology, status, self)
+        nested_root.set_attribute_manager(self.attributeManager)
+        nested_root.set_base_dir(self._baseDir)
+        nested_root.imports = self.imports
+        nested_root._environ = self._environ
+        if self.imports:
+            self.imports.add_import(":" + topology.nested_name, nested_root)
+        return nested_root
+
+    def get_root_instance(self, source: "NodeTemplate") -> "TopologyInstance":
+        topology = self.template.spec.get_topology(source)
+        assert topology
+        if self.template.topology is not topology:
+            assert self.imports is not None
+            nested_root = self.imports.find_import(":" + topology.nested_name)
+            if nested_root:
+                return cast(TopologyInstance, nested_root)
+            else:
+                return self.create_nested_topology(topology)
+        return self
```

### Comparing `unfurl-0.6.2/unfurl/server.py` & `unfurl-0.7.0/unfurl/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,23 @@
+# Copyright (c) 2023 Adam Souzis
+# SPDX-License-Identifier: MIT
+"""
+API server for the unfurl front-end app that provides JSON representations of ensembles and TOSCA service templates 
+and a patch api for updating them.
+
+The server manage local clones of remote git repositories and uses a in-memory or redis cache for efficient access. 
+"""
+
 from dataclasses import dataclass
 from functools import partial
 import json
 import os
+from pathlib import Path
 import time
+import traceback
 from typing import (
     Dict,
     List,
     Optional,
     Tuple,
     Any,
     Union,
@@ -22,23 +33,23 @@
 import flask.json
 from flask_caching import Cache
 from flask_cors import CORS
 
 import git
 from git.objects import Commit
 
-from unfurl.projectpaths import rmtree
+from .projectpaths import rmtree
 from .localenv import LocalEnv, Project
 from .repo import GitRepo, Repo, add_user_to_url, normalize_git_url_hard, sanitize_url
 from .util import UnfurlError, get_package_digest
 from .logs import getLogger, add_log_file
 from .yamlmanifest import YamlManifest
+from . import __version__, DefaultNames
 from . import to_json
 from . import init
-from . import __version__
 
 __logfile = os.getenv("UNFURL_LOGFILE")
 if __logfile:
     add_log_file(__logfile)
 logger = getLogger("unfurl.server")
 
 # note: export FLASK_ENV=development to see error stacks
@@ -265,15 +276,15 @@
     ) -> Tuple[Any, Union[bool, Optional["Commit"]]]:
         """Look up a cached value and then check if it out of date by checking if the file path in the key was modified after the given commit
         (also store the last_commit so we don't have to do that check everytime)
         we assume latest_commit is the last commit the client has seen but it might be older than the local copy
         """
         full_key = self.cache_key()
         value = cast(CacheValueType, cache.get(full_key))
-        if not value:
+        if value is None:
             logger.info("cache miss for %s", full_key)
             self.hit = False
             return None, False  # cache miss
         response, last_commit, cached_latest_commit = value
         if not latest_commit or latest_commit == cached_latest_commit:
             # this is the latest (or we aren't checking)
             logger.info("cache hit for %s with %s", full_key, latest_commit)
@@ -359,14 +370,15 @@
         return None, False
 
     def _cancel_inflight(self, cache: Cache):
         return cache.delete(self._inflight_key())
 
     def _do_work(self, work, latest_commit) -> Tuple[Optional[Any], Any, str]:
         try:
+            # NB: work shouldn't modify the working directory
             err, value = work(self, latest_commit)
         except Exception as exc:
             logger.error("unexpected error doing work for cache", exc_info=True)
             return exc, None, latest_commit
         if not self.repo or self.strict:
             # self.strict might reclone the repo
             self._set_project_repo()
@@ -491,14 +503,23 @@
     else:
         # repo doesn't exists, clone it
         os.makedirs(os.path.dirname(repo_path), exist_ok=True)
         git_url = get_project_url(project_id, username, password)
         Repo.create_working_dir(git_url, repo_path, branch)
         repo = _get_project_repo(project_id, branch)
         if repo:
+            path = Path(repo.working_dir)
+            if (path / DefaultNames.LocalConfigTemplate).is_file() and not (
+                path / "local" / DefaultNames.LocalConfig
+            ).is_file():
+                # create local/unfurl.yaml in the new project
+                new_project = Project(repo.working_dir)
+                created_local = init._create_local_config(new_project, logger, {})
+                if not created_local:
+                    logger.error(f"creating local/unfurl.yaml in {new_project.projectRoot} failed")
             logger.info("clone success: %s to %s", repo.safe_url, repo.working_dir)
     return repo and repo.working_dir or None
 
 
 def _get_filepath(format, deployment_path):
     if deployment_path:
         if not deployment_path.endswith(".yaml"):
@@ -624,15 +645,17 @@
             json_summary, request.args.get("pretty"), sort_keys=False
         )
         if latest_commit:
             response.headers["Etag"] = _make_etag(latest_commit)
         return response
     else:
         if isinstance(err, Exception):
-            return create_error_response("INTERNAL_ERROR", "An internal error occurred")
+            return create_error_response(
+                "INTERNAL_ERROR", "An internal error occurred", err
+            )
         else:
             return err
 
 
 @app.route("/populate_cache", methods=["POST"])
 def populate_cache():
     project_id = get_project_id(request)
@@ -661,15 +684,17 @@
             logger.info("skipping populate cache for private repository %s", project_id)
             return "OK"
     err, json_summary = cache_entry.get_or_set(
         cache, partial(_export_cache_work, request.args), latest_commit
     )
     if err:
         if isinstance(err, Exception):
-            return create_error_response("INTERNAL_ERROR", "An internal error occurred")
+            return create_error_response(
+                "INTERNAL_ERROR", "An internal error occurred", err
+            )
         else:
             return err
     else:
         return "OK"
 
 
 @app.route("/clear_project_file_cache", methods=["POST"])
@@ -746,15 +771,15 @@
 
     repo = _get_project_repo(project_id, branch, args)
     return CacheEntry(
         project_id, branch, "unfurl.yaml", "localenv", repo, bool(latest_commit)
     ).get_or_set(cache, _cache_localenv_work, latest_commit, _validate_localenv)
 
 
-def _localenv_from_cache_pull(
+def _localenv_from_cache_checked(
     cache,
     project_id: str,
     branch: str,
     deployment_path: str,
     latest_commit: str,
     args: dict,
     check_lastcommit: bool = True,
@@ -795,15 +820,15 @@
         and parent_localenv.project.project_repoview.repo
     )
     working_dir = parent_localenv.project.project_repoview.repo.working_dir
     clone_location = os.path.join(working_dir, deployment_path)
     err, local_env = _make_readonly_localenv(clone_location, parent_localenv)
     if err:
         return (
-            create_error_response("INTERNAL_ERROR", "An internal error occurred"),
+            create_error_response("INTERNAL_ERROR", "An internal error occurred", err),
             None,
         )
     assert local_env
     if args.get("environment"):
         local_env.manifest_context_name = args["environment"]
 
     exporter = getattr(to_json, "to_" + requested_format)
@@ -894,15 +919,18 @@
             assert isinstance(
                 value, list
             ), f"bad patch value {value} for {key} in {patch}"
             for prop in value:
                 assert isinstance(
                     prop, dict
                 ), f"bad {prop} in {value} for {key} in {patch}"
-                props[prop["name"]] = prop["value"]
+                if prop["value"] == {"__deleted": True}:
+                    props.pop(prop["name"], None)
+                else:
+                    props[prop["name"]] = prop["value"]
         elif key == "dependencies":
             requirements = [
                 {dependency["name"]: _make_requirement(dependency)}
                 for dependency in value
                 if "match" in dependency
             ]
             if requirements or "requirements" in tpl:
@@ -990,15 +1018,15 @@
 
 
 def _patch_environment(body: dict, project_id: str):
     patch = body.get("patch")
     assert isinstance(patch, list)
     latest_commit = body.get("latest_commit") or ""
     branch = body.get("branch", DEFAULT_BRANCH)
-    err, readonly_localEnv = _localenv_from_cache_pull(
+    err, readonly_localEnv = _localenv_from_cache_checked(
         cache, project_id, branch, "", latest_commit, body
     )
     if err:
         return err
     assert readonly_localEnv and readonly_localEnv.project
     invalidate_cache(body, "environments", project_id)
     localEnv = LocalEnv(readonly_localEnv.project.projectRoot, can_be_empty=True)
@@ -1105,15 +1133,15 @@
     username = body.get("username")
     password = body.get("private_token", body.get("password"))
     push_url = existing_repo.url if existing_repo else app.config["UNFURL_CLOUD_SERVER"]
     if push_url and not password and push_url.startswith("http"):
         return create_error_response("UNAUTHORIZED", "Missing credentials")
 
     latest_commit = body.get("latest_commit") or ""
-    err, parent_localenv = _localenv_from_cache_pull(
+    err, parent_localenv = _localenv_from_cache_checked(
         cache, project_id, branch, "", latest_commit, body, check_lastcommit
     )
     if err:
         return err
     assert (
         parent_localenv
         and parent_localenv.project
@@ -1156,15 +1184,15 @@
     overrides = dict(
         ENVIRONMENT=environment,
         UNFURL_CLOUD_VARS_URL=cloud_vars_url,
         apply_url_credentials=True,
     )
     # don't validate in case we are still an incomplete draft
     manifest = LocalEnv(clone_location, overrides=overrides).get_manifest(
-        skip_validation=True
+        skip_validation=True, safe_mode=True
     )
     # logger.info("vault secrets %s", manifest.manifest.vault.secrets)
     _apply_ensemble_patch(patch, manifest)
     manifest.manifest.save()
     if was_dirty:
         logger.warning(
             "local repository at %s was dirty, not committing or pushing",
@@ -1180,21 +1208,21 @@
                 try:
                     if password:
                         url = add_user_to_url(manifest.repo.url, username, password)
                     else:
                         url = None
                     manifest.repo.push(url)
                     logger.info("pushed")
-                except Exception:
+                except Exception as err:
                     # discard the last commit that we couldn't push
                     # this is mainly for security if we couldn't push because the user wasn't authorized
                     manifest.repo.reset(f"--hard {starting_revision or 'HEAD~1'}")
                     logger.error("push failed", exc_info=True)
                     return create_error_response(
-                        "INTERNAL_ERROR", "Could not push repository"
+                        "INTERNAL_ERROR", "Could not push repository", err
                     )
         else:
             logger.info(f"no changes where made, nothing commited")
     return _patch_response(manifest.repo)
 
 
 # no longer used
@@ -1262,20 +1290,20 @@
     if password:
         url = add_user_to_url(repo.url, username, password)
     else:
         url = None
     try:
         repo.push(url)
         logger.info("pushed")
-    except Exception:
+    except Exception as err:
         # discard the last commit that we couldn't push
         # this is mainly for security if we couldn't push because the user wasn't authorized
         repo.reset(f"--hard {starting_revision or 'HEAD~1'}")
         logger.error("push failed", exc_info=True)
-        return create_error_response("INTERNAL_ERROR", "Could not push repository")
+        return create_error_response("INTERNAL_ERROR", "Could not push repository", err)
     return None
 
 
 def _fetch_working_dir(
     project_path: str, branch: str, args: dict, pull: bool
 ) -> Optional[str]:
     # if successful, returns the repository's working directory or None if clone failed
@@ -1299,25 +1327,30 @@
             return clone_location
     # XXX: deployment_path must be in the project repo, split repos are not supported
     # we want the caching and staging infrastructure to only know about git, not unfurl projects
     # so we can't reference a file path outside of the git repository
     return clone_location
 
 
-def create_error_response(code, message):
+def create_error_response(code: str, message: str, err: Optional[Exception] = None):
     http_code = 400  # Default to BAD_REQUEST
     if code == "BAD_REQUEST":
         http_code = 400
     elif code == "UNAUTHORIZED":
         http_code = 401
     elif code == "INTERNAL_ERROR":
         http_code = 500
     elif code == "CONFLICT":
         http_code = 409
-    return jsonify({"code": code, "message": message}), http_code
+    response = {"code": code, "message": message}
+    if err:
+        response["details"] = "".join(
+            traceback.TracebackException.from_exception(err).format()
+        )
+    return jsonify(response), http_code
 
 
 # UNFURL_HOME="" gunicorn --log-level debug -w 4 unfurl.server:app
 def serve(
     host: str,
     port: int,
     secret: str,
```

### Comparing `unfurl-0.6.2/unfurl/support.py` & `unfurl-0.7.0/unfurl/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,19 @@
     Dict,
     Optional,
     Any,
     NewType,
 )
 from typing_extensions import Protocol, NoReturn
 from enum import Enum
-from urllib.parse import urlsplit
-
+from urllib.parse import quote, quote_plus, urlsplit
 
 if TYPE_CHECKING:
     from .manifest import Manifest
-    from .runtime import EntityInstance, InstanceKey
+    from .runtime import EntityInstance, InstanceKey, HasInstancesInstance, TopologyInstance
     from .configurator import Dependency
 
 from .eval import RefContext, set_eval_func, Ref, map_value, SafeRefContext
 from .result import (
     Results,
     ResultsList,
     ResultsMap,
@@ -128,14 +127,15 @@
     upgrade = "upgrade"
     update = "update"
     missing = "missing"
     error = "error"
     degraded = "degraded"
     prune = "prune"
     run = "run"
+    check = "check"
 
 
 class Defaults:
     shouldRun = Priority.required
     workflow = "deploy"
 
 
@@ -161,15 +161,17 @@
         funcName = mod.__name__ + "." + fragment
     else:
         funcName = arg
     func = load_class(funcName)
     if not func:
         raise UnfurlError(f"Could not find python function {funcName}")
     if not callable(func):
-        raise UnfurlError(f"Invalid python function {funcName}: {type(funcName)} is not callable.")
+        raise UnfurlError(
+            f"Invalid python function {funcName}: {type(funcName)} is not callable."
+        )
 
     kw = ctx.kw
     if "args" in kw:
         args = map_value(kw["args"], ctx)
         return func(ctx, args)
     else:
         return func(ctx)
@@ -312,25 +314,26 @@
     v_type = type(v)
     return v_type(wrap_var(item) for item in v)
 
 
 unsafe_proxy._wrap_sequence = _wrap_sequence
 
 
-def _sandboxed_template(value: str, ctx: SafeRefContext, _UnfurlUndefined):
+def _sandboxed_template(value: str, ctx: SafeRefContext, vars, _UnfurlUndefined):
     from jinja2.sandbox import SandboxedEnvironment
     from jinja2.nativetypes import NativeCodeGenerator, native_concat
 
     SandboxedEnvironment.code_generator_class = NativeCodeGenerator
     SandboxedEnvironment.concat = staticmethod(native_concat)  # type: ignore
     env = SandboxedEnvironment()
 
     if not ctx.strict:
         env.undefined = _UnfurlUndefined
-    return env.from_string(value).render(ctx.vars)
+    ctx.templar = None
+    return env.from_string(value).render(vars)
 
 
 def apply_template(value: str, ctx: RefContext, overrides=None) -> Any:
     if not isinstance(value, str):
         msg = f"Error rendering template: source must be a string, not {type(value)}"
         if ctx.strict:
             raise UnfurlError(msg)
@@ -401,17 +404,14 @@
             self._log_message()
             return super().__bool__()  # type: ignore
 
         # see ChainableUndefined
         def __html__(self) -> str:
             return str(self)
 
-    if isinstance(ctx, SafeRefContext):
-        return _sandboxed_template(value, ctx, _UnfurlUndefined)
-
     # implementation notes:
     #   see https://github.com/ansible/ansible/test/units/template/test_templar.py
     #   dataLoader is only used by _lookup and to set _basedir (else ./)
     if not ctx.templar or (ctx.base_dir and ctx.templar._basedir != ctx.base_dir):
         # we need to create a new templar
         loader = DataLoader()
         if ctx.base_dir:
@@ -453,15 +453,18 @@
     # set referenced to track references (set by Ref.resolve)
     # need a way to turn on and off
     try:
         # strip whitespace so jinija native types resolve even with extra whitespace
         # disable caching so we don't need to worry about the value of a cached var changing
         # use do_template because we already know it's a template
         try:
-            value = templar.template(value, fail_on_undefined=fail_on_undefined)
+            if isinstance(ctx, SafeRefContext):
+                value = _sandboxed_template(value, ctx, vars, _UnfurlUndefined)
+            else:
+                value = templar.template(value, fail_on_undefined=fail_on_undefined)
         except Exception as e:
             msg = str(e)
             # XXX have _UnfurlUndefined throw an exception with the missing obj and key
             match = re.search(r"has no attribute '(\w+)'", msg)
             if match:
                 msg = f'missing attribute or key: "{match.group(1)}"'
             else:
@@ -613,14 +616,15 @@
 def token(args, ctx):
     args = map_value(args, ctx)
     return args[0].split(args[1])[args[2]]
 
 
 set_eval_func("token", token, True, True)
 
+
 # XXX this doesn't work with node_filters, need an instance to get a specific result
 def get_tosca_property(args, ctx):
     from toscaparser.functions import get_function
 
     tosca_tpl = ctx.currentResource.root.template.toscaEntityTemplate
     node_template = ctx.currentResource.template.toscaEntityTemplate
     return get_function(tosca_tpl, node_template, {"get_property": args}).result()
@@ -665,35 +669,38 @@
         default = cast(Optional[str], map_value(default, ctx))
         return default
 
 
 set_eval_func("get_env", get_env, True)
 
 
-def set_context_vars(vars, resource):
-    root = resource.root
+def set_context_vars(vars, resource: "EntityInstance"):
+    root = cast("TopologyInstance", resource.root)
     ROOT: Dict[str, Any] = {}
     vars.update(dict(NODES=TopologyMap(root), ROOT=ROOT, TOPOLOGY=ROOT))
     if "inputs" in root._attributes:
         ROOT.update(
             dict(
                 inputs=root._attributes["inputs"],
                 outputs=root._attributes["outputs"],
             )
         )
-    app_template = root.template.spec.substitution_template
+    app_template = root.template.topology.substitution_node  # type: ignore
     if app_template:
         app = root.find_instance(app_template.name)
         if app:
             ROOT["app"] = app.attributes
         for name, req in app_template.requirements.items():
             if req.relationship and req.relationship.target:
-                target = root.find_instance(req.relationship.target.name)
+                target = root.get_root_instance(
+                    req.relationship.target.toscaEntityTemplate  # type: ignore
+                ).find_instance(req.relationship.target.name)
                 if target:
                     ROOT[name] = target.attributes
+
     return vars
 
 
 class _EnvMapper(dict):
     """Resolve environment variable name to instance properties via the root template's requirements.
     Pattern should match _generate_env_names in to_json.py and set_context_vars above.
     """
@@ -703,15 +710,15 @@
     def copy(self):
         return _EnvMapper(self)
 
     def __missing__(self, key):
         objname, sep, prop = key.partition("_")
         assert self.ctx
         root = self.ctx.currentResource.root
-        app = root.template.spec.substitution_template
+        app = root.template.spec.substitution_node
         if app and objname and prop:
             obj = None
             if objname == "APP":
                 obj = app
             else:
                 for name, req in app.requirements.items():
                     if name.upper() == objname:
@@ -1023,29 +1030,78 @@
         query = start + "::" + candidate_name
     return ctx.query(query)
 
 
 set_eval_func("get_attribute", get_attribute, True, True)
 
 
-def get_nodes_of_type(type_name: str, ctx: RefContext) :
+def get_nodes_of_type(type_name: str, ctx: RefContext):
     return [
         r
         for r in ctx.currentResource.root.get_self_and_descendants()
         if r.template.is_compatible_type(type_name)
         and r.name not in ["inputs", "outputs"]
     ]
 
 
 set_eval_func("get_nodes_of_type", get_nodes_of_type, True, True)
 
 
 set_eval_func("_generate", lambda arg, ctx: get_random_password(10, ""), True, True)
 
 
+def _urljoin(scheme, host, port=None, path=None, query=None, frag=None):
+    """
+    Evaluate a list of url components to a relative or absolute URL,
+    where the list is ``[scheme, host, port, path, query, fragment]``.
+
+    The list must have at least two items (``scheme`` and ``host``) present
+    but if either or both are empty a relative or scheme-relative URL is generated.
+    If all items are empty, ``null`` is returned.
+    The ``path``, ``query``, and ``fragment`` items are url-escaped if present.
+    Default ports (80 and 443 for ``http`` and ``https`` URLs respectively) are omitted even if specified.
+    """
+    if not scheme and not host and not path and not query and not frag:
+        return None
+
+    if port and (
+        not (scheme == "https" and int(port) == 443)
+        and not (scheme == "http" and int(port) == 80)
+    ):
+        netloc = f"{host}:{port}"
+    else:
+        # omit default ports
+        netloc = host or ""
+    if path:
+        path = quote(path)
+    if netloc and path and path[0] != "/":
+        path = "/" + path
+    if query:
+        query = "?" + quote_plus(query)
+    else:
+        query = ""
+    if frag:
+        frag = "#" + quote(frag)
+    else:
+        frag = ""
+
+    prefix = ""  # relative url
+    if scheme:
+        # absolute url or relative url with scheme
+        prefix = scheme + ":"
+    if netloc:
+        # its an absolute url or scheme-relative url if scheme is missing
+        prefix += "//"
+
+    return prefix + netloc + (path or "") + query + frag
+
+
+set_eval_func("urljoin", lambda args, ctx: _urljoin(*args), False, True)
+
+
 class ContainerImage(ExternalValue):
     """
     Represents a container image.
     get() returns name of the image, which may be qualified
     with the registry url, repository name, tag, or digest
 
     All of the following are valid:
@@ -1069,20 +1125,20 @@
     # A name component may not start or end with a separator.
     # A tag name must be valid ASCII and may contain lowercase and uppercase letters, digits, underscores, periods and dashes.
     # # A tag name may not start with a period or a dash and may contain a maximum of 128 characters.
 
     def __init__(
         self,
         name: str,
-        tag=None,
-        digest=None,
-        registry_host=None,
-        username=None,
-        password=None,
-        source_digest=None,
+        tag: Optional[str] = None,
+        digest: Optional[str] = None,
+        registry_host: Optional[str] = None,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        source_digest: Optional[str] = None,
     ):
         self.name = name.lstrip("/").lower()
         self.tag = tag
         self.digest = digest
         self.registry_host = registry_host
         self.username = username
         self.password = password
@@ -1104,38 +1160,50 @@
         if self.digest:
             if "@" == self.digest[0]:
                 return name + self.digest
             else:
                 return f"{name}@sha256:{self.digest}"
         return name
 
+    def full_name(self, default_hostname="docker.io") -> str:
+        if not self.registry_host:
+            return os.path.join(default_hostname, self.get())
+        else:
+            return self.get()
+
     @staticmethod
-    def split(artifact_name):
+    def split(
+        artifact_name: str,
+    ) -> Tuple[Optional[str], Optional[str], Optional[str], Optional[str]]:
         if not artifact_name:
             return None, None, None, None
         hostname = None
         namespace, sep, name = artifact_name.partition("/")
         if sep and (":" in namespace or artifact_name.count("/") > 1):
             # heuristic because name can look like a hostname
             hostname = namespace
         else:
             name = artifact_name
 
         tag = None
         name, sep, digest = name.partition("@")
         if not sep:
-            digest = None
+            digest = None  # type: ignore
             name, sep, qualifier = artifact_name.partition(":")
             if sep:
                 tag = qualifier
         return name.lower(), tag, digest, hostname
 
     @staticmethod
-    def make(artifact_name):
-        return ContainerImage(*ContainerImage.split(artifact_name))
+    def make(artifact_name: str) -> Optional["ContainerImage"]:
+        parts = ContainerImage.split(artifact_name)
+        if parts[0]:
+            return ContainerImage(*parts)  # type: ignore
+        else:
+            return None
 
     @staticmethod
     def resolve_name(base_name: str, artifact_name: str):
         if not base_name:
             return artifact_name
         # support more qualified name such as image name or tag
         name, sep, qualifier = artifact_name.partition("@")
@@ -1184,34 +1252,38 @@
         # XXX implement instance.artifacts
         artifact = instance.template.artifacts.get(artifact_name)
         if artifact:
             return artifact
     return None
 
 
-def _get_container_image_from_repository(entity, artifact_name):
+def _get_container_image_from_repository(
+    entity, artifact_name
+) -> Optional["ContainerImage"]:
     # aka get_artifact_as_value
     name, tag, digest, hostname = ContainerImage.split(artifact_name)
     attr = entity.attributes
 
     repository_id = attr.get("repository_id")
     if repository_id and name:
         name = ContainerImage.resolve_name(repository_id, name)
     else:
         name = repository_id or name
 
     tag = tag or attr.get("repository_tag")
 
     if attr.get("registry_url"):
-        hostname = attr["registry_url"]
+        hostname = cast(str, attr["registry_url"])
         if "//" in hostname:
             hostname = urlsplit(attr["registry_url"]).netloc
     username = attr.get("username")
     password = attr.get("password")
     source_digest = attr.get("revision")
+    if not name:
+        return None
     return ContainerImage(
         name, tag, digest, hostname, username, password, source_digest
     )
 
 
 def get_artifact(ctx: RefContext, entity, artifact_name, location=None, remove=None):
     """
@@ -1222,15 +1294,17 @@
     "registry/repository/name:tag" or "registry/repository/name@sha256:digest"
 
     If entity_name or artifact_name is not found return None.
     """
     from .runtime import NodeInstance, ArtifactInstance
 
     if not entity:
-        return ContainerImage.make(artifact_name)  # XXX assume its a container image
+        return ContainerImage.make(
+            artifact_name
+        )  # XXX this assumes its a container image
     if isinstance(entity, ArtifactInstance):
         return entity.template.as_value()
     if isinstance(entity, str):
         instances = _get_instances_from_keyname(ctx, entity)
     elif isinstance(entity, NodeInstance):
         if entity.template.is_compatible_type("unfurl.nodes.Repository"):
             # XXX retrieve method from template definition
@@ -1275,52 +1349,66 @@
 
 set_eval_func("external", get_import)
 
 
 class _Import:
     def __init__(
         self,
-        external_instance: "EntityInstance",
+        external_instance: "HasInstancesInstance",
         spec: dict,
-        local_instance: Optional["EntityInstance"] = None,
+        local_instance: Optional["HasInstancesInstance"] = None,
     ):
         self.external_instance = external_instance
         self.spec = spec
         self.local_instance = local_instance
 
 
-class Imports(collections.OrderedDict):
+if TYPE_CHECKING:  # for python 3.7
+    ImportsBase = collections.OrderedDict[str, _Import]
+else:
+    ImportsBase = collections.OrderedDict
+
+
+class Imports(ImportsBase):
     manifest: Optional["Manifest"] = None
 
-    def find_import(self, qualified_name):
+    def find_import(self, qualified_name: str) -> Optional["HasInstancesInstance"]:
         # return a local shadow of the imported instance
         # or the imported instance itself if no local shadow exist (yet).
         imported = self._find_import(qualified_name)
         if imported:
             return imported
         iName, sep, rName = qualified_name.partition(":")
+        if not iName:
+            # name is in the current ensemble (but maybe a different topology)
+            return None
         assert self.manifest
         localEnv = self.manifest.localEnv
         if iName not in self and localEnv:
             project = localEnv.project or localEnv.homeProject
             tpl = project and project.find_ensemble_by_name(iName)
             if tpl:
                 self.manifest.load_external_ensemble(iName, dict(manifest=tpl))  # type: ignore
                 return self._find_import(qualified_name)
         return None
 
-    def _find_import(self, name):
+    def _find_import(self, name: str) -> Optional["HasInstancesInstance"]:
         if name in self:
             # fully qualified name already added
             return self[name].local_instance or self[name].external_instance
         iName, sep, rName = name.partition(":")
+        if not iName:
+            # name is in the current ensemble (but maybe a different topology)
+            assert self.manifest and self.manifest.rootResource
+            assert sep and rName
+            return self.manifest.rootResource.find_instance(rName)
         if iName not in self:
             return None
         # do a unqualified look up to find the declared import
-        imported = self[iName].external_instance.root.find_resource(rName or "root")
+        imported = self[iName].external_instance.root.find_instance(rName or "root")
         if imported:
             self.add_import(iName, imported)
         return imported
 
     def set_shadow(self, key, local_instance, external_instance):
         if key not in self:
             record = self.add_import(key, external_instance)
@@ -1564,14 +1652,16 @@
     (if it is defined in a spec.)
     Changing an overridden attribute definition in the spec will have no effect
     -- if a configurator wants to re-evaluate that attribute, it can create a dependency on it
     so to treat that as changed configuration.
     """
 
     validate = True
+    safe_mode = False
+    strict: Optional[bool] = None
 
     # what about an attribute that is added to the spec that already exists in status?
     # XXX2 tests for the above behavior
     def __init__(self, yaml=None, task=None):
         self.attributes: Dict[str, Tuple[EntityInstance, ResultsMap]] = {}
         self.statuses = {}
         self._yaml = yaml  # hack to safely expose the yaml context
@@ -1596,37 +1686,42 @@
         assert newvalue is None or isinstance(newvalue, Status)
         if resource.key not in self.statuses:
             self.statuses[resource.key] = [resource._localStatus, newvalue]
         else:
             self.statuses[resource.key][1] = newvalue
 
     def mark_referenced_templates(self, template):
-        for (resource, attr) in self.attributes.values():
+        for resource, attr in self.attributes.values():
             if (
                 resource.template is not template
                 and template not in resource.template._isReferencedBy
             ):
                 resource.template._isReferencedBy.append(template)  # type: ignore
 
     def _get_context(self, resource):
-        if self._context_vars is None:
+        if (
+            self._context_vars is None
+            or self._context_vars["NODES"].resource is not resource.root
+        ):
             self._context_vars = {}
             set_context_vars(self._context_vars, resource)
-        return RefContext(resource, self._context_vars, task=self.task)
+        ctor = SafeRefContext if self.safe_mode else RefContext
+        return ctor(resource, self._context_vars, task=self.task, strict=self.strict)
 
-    def get_attributes(self, resource: "EntityInstance"):
+    def get_attributes(self, resource: "EntityInstance") -> ResultsMap:
         if resource.key not in self.attributes:
             if resource.shadow:
                 return resource.shadow.attributes
 
             if resource.template:
                 specAttributes = resource.template.defaultAttributes
+                properties = resource.template.properties  # type: ignore
                 _attributes = ChainMap(
                     resource._attributes,
-                    resource.template.properties,
+                    properties,
                     specAttributes,
                 )
             else:
                 _attributes = ChainMap(resource._attributes)
             ctx = self._get_context(resource)
             mode = os.getenv("UNFURL_VALIDATION_MODE")
             if mode is not None and "nopropcheck" in mode:
```

### Comparing `unfurl-0.6.2/unfurl/templates/aws/unfurl.yaml.j2` & `unfurl-0.7.0/unfurl/templates/aws/unfurl.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/dashboard/manifest.yaml.j2` & `unfurl-0.7.0/unfurl/templates/dashboard/manifest.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/digitalocean/unfurl.yaml.j2` & `unfurl-0.7.0/unfurl/templates/digitalocean/unfurl.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/gcp/unfurl.yaml.j2` & `unfurl-0.7.0/unfurl/templates/gcp/unfurl.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/home/manifest-template.yaml.j2` & `unfurl-0.7.0/unfurl/templates/home/manifest-template.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/home/unfurl.yaml.j2` & `unfurl-0.7.0/unfurl/templates/home/unfurl.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/local/ensemble-examples.yaml` & `unfurl-0.7.0/unfurl/templates/local/ensemble-examples.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/local-unfurl-template.yaml.j2` & `unfurl-0.7.0/unfurl/templates/local-unfurl-template.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/manifest-template.yaml.j2` & `unfurl-0.7.0/unfurl/templates/manifest-template.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/manifest.yaml.j2` & `unfurl-0.7.0/unfurl/templates/manifest.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/python3.10/Pipfile` & `unfurl-0.7.0/unfurl/templates/python3.10/Pipfile`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/python3.10/Pipfile.lock` & `unfurl-0.7.0/unfurl/templates/python3.10/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/python3.11/Pipfile` & `unfurl-0.7.0/unfurl/templates/python3.11/Pipfile`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/python3.11/Pipfile.lock` & `unfurl-0.7.0/unfurl/templates/python3.11/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/python3.7/Pipfile` & `unfurl-0.7.0/unfurl/templates/python3.7/Pipfile`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/python3.7/Pipfile.lock` & `unfurl-0.7.0/unfurl/templates/python3.7/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/python3.8/Pipfile` & `unfurl-0.7.0/unfurl/templates/python3.8/Pipfile`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/python3.8/Pipfile.lock` & `unfurl-0.7.0/unfurl/templates/python3.8/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/python3.9/Pipfile` & `unfurl-0.7.0/unfurl/templates/python3.9/Pipfile`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/python3.9/Pipfile.lock` & `unfurl-0.7.0/unfurl/templates/python3.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/secrets.yaml.j2` & `unfurl-0.7.0/unfurl/templates/secrets.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/service-template.yaml.j2` & `unfurl-0.7.0/unfurl/templates/service-template.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/unfurl.local.yaml.j2` & `unfurl-0.7.0/unfurl/templates/unfurl.local.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/templates/unfurl.yaml.j2` & `unfurl-0.7.0/unfurl/templates/unfurl.yaml.j2`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/to_json.py` & `unfurl-0.7.0/unfurl/to_json.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,42 +13,78 @@
 import re
 import os
 import os.path
 import sys
 import itertools
 import json
 import datetime
-from typing import Any, Dict, List, Optional, Tuple, Union, cast, TYPE_CHECKING
+from time import perf_counter
+from typing import (
+    Any,
+    Dict,
+    Iterator,
+    List,
+    NewType,
+    Optional,
+    Tuple,
+    Union,
+    cast,
+    TYPE_CHECKING,
+)
 from collections import Counter
 from collections.abc import Mapping, MutableSequence
+from typing_extensions import TypedDict
 from urllib.parse import urlparse
+from toscaparser.substitution_mappings import SubstitutionMappings
 from toscaparser.properties import Property
 from toscaparser.elements.constraints import Schema
 from toscaparser.elements.property_definition import PropertyDef
 from toscaparser.elements.nodetype import NodeType
 from toscaparser.elements.relationshiptype import RelationshipType
 from toscaparser.elements.statefulentitytype import StatefulEntityType
 from toscaparser.entity_template import EntityTemplate
 from toscaparser.common.exception import ExceptionCollector
 from toscaparser.elements.scalarunit import get_scalarunit_class
 from toscaparser.elements.datatype import DataType
 from toscaparser.elements.portspectype import PortSpec
 from toscaparser.activities import ConditionClause
+from toscaparser.nodetemplate import NodeTemplate
+from toscaparser.relationship_template import RelationshipTemplate
+from .runtime import EntityInstance, TopologyInstance
 from .yamlmanifest import YamlManifest
 from .merge import merge_dicts, patch_dict
 from .logs import sensitive, is_sensitive, getLogger
-from .tosca import is_function, get_nodefilters
+from .tosca import (
+    EntitySpec,
+    NodeSpec,
+    TopologySpec,
+    ToscaSpec,
+    is_function,
+    get_nodefilters,
+)
 from .util import to_enum, UnfurlError
 from .support import Status, is_template
 from .result import ChangeRecord
-from .localenv import LocalEnv
+from .localenv import LocalEnv, Project
 
 logger = getLogger("unfurl")
 
 
+GraphqlObject = NewType("GraphqlObject", Dict[str, Any])
+GraphqlObjectsByName = Dict[str, GraphqlObject]
+ResourceType = NewType("ResourceType", GraphqlObject)
+ResourceTypesByName = Dict[str, ResourceType]
+GraphqlDB = NewType("GraphqlDB", Dict[str, GraphqlObjectsByName])
+CustomDefs = Dict[str, dict]
+
+
+def _get_types(db: GraphqlDB) -> ResourceTypesByName:
+    return cast(ResourceTypesByName, db["ResourceType"])
+
+
 def _print(*args):
     print(*args, file=sys.stderr)
 
 
 def js_timestamp(ts: datetime.datetime) -> str:
     jsts = ts.isoformat(" ", "seconds")
     if ts.utcoffset() is None:
@@ -143,18 +179,20 @@
         # "scalar-unit.bitrate": _SCALAR_TYPE, # XXX add parser support 3.3.6.7 scalar-unit.bitrate
         "tosca.datatypes.network.PortDef": VALUE_TYPES["PortDef"],
         "tosca.datatypes.network.PortSpec": VALUE_TYPES["PortSpec"],
     }
 )
 
 
-def tosca_type_to_jsonschema(spec, propdefs, toscatype):
+def tosca_type_to_jsonschema(custom_defs: CustomDefs, propdefs, toscatype):
     jsonschema = dict(
         type="object",
-        properties={p.name: tosca_schema_to_jsonschema(p, spec) for p in propdefs},
+        properties={
+            p.name: tosca_schema_to_jsonschema(p, custom_defs) for p in propdefs
+        },
     )
     # add typeid:
     if toscatype:
         jsonschema["properties"].update({"$toscatype": dict(const=toscatype)})  # type: ignore
     return jsonschema
 
 
@@ -192,21 +230,21 @@
         return {"type": "number", "default_unit": default_unit}
     else:
         return {"type": "string"}
     # XXX add format specifier
     # regex: "|".join(get_scalarunit_class(value_type).SCALAR_UNIT_DICT)
 
 
-def tosca_schema_to_jsonschema(p, spec):
+def tosca_schema_to_jsonschema(p: PropertyDef, custom_defs: CustomDefs):
     # convert a PropertyDef to a property (this creates the Schema object we need)
     prop = Property(
         p.name,
         p.default,
         p.schema or dict(type="string"),
-        spec.template.topology_template.custom_defs,
+        custom_defs,
     )
     toscaSchema = prop.schema
     tosca_type = toscaSchema.type
     schema = {}
     if toscaSchema.title or p.name:
         schema["title"] = toscaSchema.title or p.name
     if toscaSchema.default is not None and not is_value_computed(toscaSchema.default):
@@ -220,81 +258,84 @@
     if metadata:
         # set "sensitive" if present
         schema.update(metadata)
     constraints = toscaSchema.constraints or []
     if tosca_type in VALUE_TYPES:
         type_schema = _get_valuetype_schema(tosca_type, metadata)
     else:
-        dt = DataType(tosca_type, spec.template.topology_template.custom_defs)
+        dt = DataType(tosca_type, custom_defs)
         if dt.value_type:  # it's a simple type
             type_schema, valuetype_schema = get_valuetype(dt, metadata)
             if valuetype_schema.constraints:  # merge constraints
                 constraints = valuetype_schema.constraints + constraints
         else:  # it's a complex type with properties:
             propdefs = [
                 p
                 for p in dt.get_properties_def_objects()
                 if is_property_user_visible(p)
             ]
-            type_schema = tosca_type_to_jsonschema(spec, propdefs, dt.type)
+            type_schema = tosca_type_to_jsonschema(custom_defs, propdefs, dt.type)
     if tosca_type not in ONE_TO_ONE_TYPES and "properties" not in schema:
         schema["$toscatype"] = tosca_type
     schema.update(type_schema)
 
     if toscaSchema.entry_schema:
         entrySchema = tosca_schema_to_jsonschema(
-            PropertyDef("", None, toscaSchema.entry_schema), spec
+            PropertyDef("", None, toscaSchema.entry_schema), custom_defs
         )
         if tosca_type == "list":
             schema["items"] = entrySchema
         else:
             schema["additionalProperties"] = entrySchema
 
     if constraints:
         schema.update(map_constraints(schema["type"], toscaSchema.constraints, schema))
     return schema
 
 
-def _requirement_visibility(spec, name, req):
+def _requirement_visibility(topology: TopologySpec, name: str, req) -> str:
     if name in ["dependency", "installer"]:
         # skip artifact requirements and the base TOSCA relationship type that every node has
         return "omit"
     node = req.get("node")
     metadata = req.get("metadata") or {}
     if metadata.get("visibility"):
         return metadata["visibility"]
     if metadata.get("internal"):
         return "hidden"
-    if node and node in spec.nodeTemplates:
-        # if there's already a resource template assigned and it is marked internal
-        node_metadata = (
-            spec.nodeTemplates[node].toscaEntityTemplate.entity_tpl.get("metadata")
-            or {}
-        )
-        if not node_metadata.get("user_settable") and not metadata.get("user_settable"):
-            return "hidden"
-        else:
-            return "visible"
+    if node:
+        nodespec = topology.get_node_template(node)
+        if nodespec:
+            # if there's already a resource template assigned and it is marked internal
+            node_metadata = (
+                nodespec.toscaEntityTemplate.entity_tpl.get("metadata") or {}
+            )
+            if not node_metadata.get("user_settable") and not metadata.get(
+                "user_settable"
+            ):
+                return "hidden"
+            else:
+                return "visible"
     return "inherit"
 
 
 def _get_req(req_dict) -> Tuple[str, dict]:
     name, req = list(req_dict.items())[0]
     if isinstance(req, str):
         req = dict(node=req)
     else:
         assert isinstance(req, dict), f"bad {req} in {req_dict}"
     return name, req
 
 
-def expand_prefix(spec, nodetype: str):
+def expand_prefix(nodetype: str):
     return nodetype.replace("tosca:", "tosca.nodes.")  # XXX
 
 
-def _find_req_typename(types, typename, reqname) -> str:
+def _find_req_typename(types: ResourceTypesByName, typename, reqname) -> str:
     # have types[typename] go first
     for target_reqs in types[typename]["requirements"]:
         if target_reqs["name"] == reqname:
             return target_reqs["resourceType"]
 
     # XXX not very efficient
     for t in types.values():
@@ -305,20 +346,27 @@
             # type is typename or derived from typename
             for target_reqs in t["requirements"]:
                 if target_reqs["name"] == reqname:
                     return target_reqs["resourceType"]
     return ""  # not found
 
 
-def _make_req(req_dict: dict, types=None, typename=None) -> Tuple[str, dict, dict]:
+def _make_req(
+    req_dict: dict,
+    topology: Optional[TopologySpec] = None,
+    types: Optional[ResourceTypesByName] = None,
+    typename: Optional[str] = None,
+) -> Tuple[str, dict, GraphqlObject]:
     name, req = _get_req(req_dict)
-    reqobj: Dict[str, Any] = dict(
-        name=name,
-        description=req.get("description") or "",
-        __typename="RequirementConstraint",
+    reqobj = GraphqlObject(
+        dict(
+            name=name,
+            description=req.get("description") or "",
+            __typename="RequirementConstraint",
+        )
     )
     metadata = req.get("metadata")
 
     if metadata:
         if "badge" in metadata:
             reqobj["badge"] = metadata["badge"]
         if "title" in metadata:
@@ -329,24 +377,27 @@
     if "occurrences" in req:
         reqobj["min"] = req["occurrences"][0]
         reqobj["max"] = req["occurrences"][1]
 
     if req.get("node_filter"):
         reqobj["node_filter"] = req["node_filter"]
         if types is not None:
+            assert topology
             assert typename is not None
             # we're called from annotate_requirements annotating a nested requirements constraint
             reqtypename = _find_req_typename(types, typename, name)
             if reqtypename:
-                _annotate_requirement(reqobj, reqtypename, types)
+                _annotate_requirement(reqobj, reqtypename, topology, types)
 
     return name, req, reqobj
 
 
-def requirement_to_graphql(spec, req_dict):
+def requirement_to_graphql(
+    topology: TopologySpec, req_dict: dict
+) -> Optional[GraphqlObject]:
     """
     type RequirementConstraint {
         name: String!
         title: String
         description: String
         resourceType: ResourceType!
         match: ResourceTemplate
@@ -361,73 +412,78 @@
     """
     name, req, reqobj = _make_req(req_dict)
     if "min" not in reqobj:
         # set defaults
         reqobj["min"] = 1
         reqobj["max"] = 1
 
-    visibility = _requirement_visibility(spec, name, req)
+    visibility = _requirement_visibility(topology, name, req)
     if visibility == "omit":
         return None
 
     if visibility != "inherit":
         reqobj["visibility"] = visibility
 
     if reqobj["max"] == 0:
         return None
 
     reqobj["match"] = None
     nodetype = req.get("node")
     if nodetype:
         # req['node'] can be a node_template instead of a type
-        expand_prefix(spec, nodetype)
-        if nodetype in spec.nodeTemplates:
+        if nodetype in topology.node_templates:
             reqobj["match"] = nodetype
-            nodetype = spec.nodeTemplates[nodetype].type
+            nodetype = topology.node_templates[nodetype].type
+        nodetype = expand_prefix(nodetype)
     else:
         nodetype = req.get("capability")
         if not nodetype:
             logger.warning(
                 "skipping constraint %s, there was no type specified ", req_dict
             )
             return None
     reqobj["resourceType"] = nodetype
     return reqobj
 
 
-def _get_extends(spec, typedef, extends: list, types):
+def _get_extends(
+    topology: TopologySpec,
+    typedef: StatefulEntityType,
+    extends: list,
+    types: Optional[ResourceTypesByName],
+) -> None:
     if not typedef:
         return
     name = typedef.type
     if name not in extends:
         extends.append(name)
     if types is not None and name not in types:
-        node_type_to_graphql(spec, typedef, types)
+        node_type_to_graphql(topology, typedef, types)
     for p in typedef.parent_types():
-        _get_extends(spec, p, extends, types)
+        _get_extends(topology, p, extends, types)
 
 
-def template_visibility(spec, t, for_resource):
-    metadata = t.entity_tpl.get("metadata")
+def template_visibility(t: EntitySpec, discovered):
+    metadata = t.toscaEntityTemplate.entity_tpl.get("metadata")
     if metadata:
         if metadata.get("visibility"):
             return metadata["visibility"]
         if metadata.get("internal"):
             return "hidden"
 
     if t.type in ["unfurl.nodes.ArtifactInstaller", "unfurl.nodes.LocalRepository"]:
         return "omit"  # skip artifacts
     if "default" in t.directives:
         return "hidden"
-    if not for_resource and spec.discovered and t.name in spec.discovered:
+    if discovered and t.nested_name in discovered:
         return "omit"
     return "inherit"
 
 
-def is_property_user_visible(p):
+def is_property_user_visible(p: PropertyDef):
     user_settable = p.schema.get("metadata", {}).get("user_settable")
     if user_settable is not None:
         return user_settable
     if p.default is not None or is_computed(p):
         return False
     return True
 
@@ -450,31 +506,53 @@
         p.name in ["tosca_id", "state", "tosca_name"]
         or is_value_computed(p.value)
         or (p.value is None and is_value_computed(p.default))
         or metadata.get("computed")
     )
 
 
-def always_export(p):
+def always_export(p: Property) -> bool:
     if isinstance(p.schema, Schema):
         metadata = p.schema.metadata
     else:
         metadata = p.schema.get("metadata") or {}
-    return metadata.get("export")
+    return bool(metadata.get("export"))
+
+
+def maybe_export_value(prop: Property, instance: EntityInstance, attrs: List[dict]):
+    export = always_export(prop)
+    if export:
+        # evaluate computed property now
+        try:
+            value = instance.attributes[prop.name]
+        except Exception as e:
+            # this can be raised if the evaluation is unsafe
+            logger.warning(
+                f"export could not evaluate property {prop.name} on {instance}: {e}"
+            )
+        else:
+            attrs.append(
+                dict(
+                    name=prop.name,
+                    value=attribute_value_to_json(prop, value),
+                )
+            )
+    return export
 
 
 # def property_value_to_json(p, value):
 #     if is_computed(p):
 #         return None
 #     return attribute_value_to_json(p, value)
 
 
-def _is_get_env_or_secret(value):
+def _is_get_env_or_secret(value) -> bool:
     if isinstance(value, dict):
         return "get_env" in value or "secret" in value or "_generate" in value
+    return False
 
 
 class PropertyVisitor:
     redacted = False
     user_settable = False
 
     def redact_if_sensitive(self, value):
@@ -511,15 +589,19 @@
 
 
 def attribute_value_to_json(p, value):
     return PropertyVisitor().attribute_value_to_json(p, value)
 
 
 # XXX outputs: only include "public" attributes?
-def node_type_to_graphql(spec, type_definition, types: dict):
+def node_type_to_graphql(
+    topology: TopologySpec,
+    type_definition: StatefulEntityType,
+    types: ResourceTypesByName,
+) -> ResourceType:
     """
     type ResourceType {
       name: String!
       title: String
       extends: [ResourceType!]
       description: String
       badge: String
@@ -530,18 +612,23 @@
       computedPropertiesSchema: JSON
       outputsSchema: JSON
       requirements: [RequirementConstraint!]
       implementations: [String]
       implementation_requirements: [String]
     }
     """
-    jsontype = dict(
-        name=type_definition.type,  # fully qualified name
-        title=type_definition.type.split(".")[-1],  # short, readable name
-        description=type_definition.get_value("description") or "",
+    custom_defs = topology.topology_template.custom_defs
+    jsontype = ResourceType(
+        GraphqlObject(
+            dict(
+                name=type_definition.type,  # fully qualified name
+                title=type_definition.type.split(".")[-1],  # short, readable name
+                description=type_definition.get_value("description") or "",
+            )
+        )
     )
     types[
         type_definition.type
     ] = jsontype  # set now to avoid circular reference via _get_extends
     metadata = type_definition.get_value("metadata")
     inherited_metadata = type_definition.get_value("metadata", parent=True)
     visibility = "inherit"
@@ -560,53 +647,55 @@
     jsontype["visibility"] = visibility
 
     propertydefs = list(
         (p, is_property_user_visible(p))
         for p in type_definition.get_properties_def_objects()
     )
     jsontype["inputsSchema"] = tosca_type_to_jsonschema(
-        spec, (p[0] for p in propertydefs if p[1]), None
+        custom_defs, (p[0] for p in propertydefs if p[1]), None
     )
     jsontype["computedPropertiesSchema"] = tosca_type_to_jsonschema(
-        spec, (p[0] for p in propertydefs if not p[1]), None
+        custom_defs, (p[0] for p in propertydefs if not p[1]), None
     )
 
     extends: List[str] = []
     # add ancestors classes to extends
-    _get_extends(spec, type_definition, extends, types)
+    _get_extends(topology, type_definition, extends, types)
     jsontype["extends"] = extends
     if not type_definition.is_derived_from("tosca.nodes.Root"):
         return jsontype
     if type_definition.defs is None:
         logger.warning("%s is missing type definition", type_definition.type)
         return jsontype
 
     # add capabilities types to extends
     for cap in type_definition.get_capability_typedefs():
-        _get_extends(spec, cap, extends, None)
+        _get_extends(topology, cap, extends, None)
 
     # treat each capability as a complex property
     add_capabilities_as_properties(
-        jsontype["inputsSchema"]["properties"], type_definition, spec
+        jsontype["inputsSchema"]["properties"], type_definition, custom_defs
     )
     # XXX only include "public" attributes?
     attributedefs = (
         p
         for p in type_definition.get_attributes_def_objects()
         if is_property_user_visible(p)
     )
-    jsontype["outputsSchema"] = tosca_type_to_jsonschema(spec, attributedefs, None)
+    jsontype["outputsSchema"] = tosca_type_to_jsonschema(
+        custom_defs, attributedefs, None
+    )
     # XXX capabilities can hava attributes too
-    # add_capabilities_as_attributes(jsontype["outputs"], type_definition, spec)
+    # add_capabilities_as_attributes(jsontype["outputs"], type_definition, custom_defs)
 
     jsontype["requirements"] = list(
         filter(
             None,
             [
-                requirement_to_graphql(spec, req)
+                requirement_to_graphql(topology, req)
                 for req in type_definition.get_all_requirements()
             ],
         )
     )
 
     operations = set(
         op.name
@@ -616,56 +705,96 @@
     jsontype["implementations"] = sorted(operations)
     jsontype[
         "implementation_requirements"
     ] = type_definition.get_interface_requirements()
     return jsontype
 
 
-def _make_typedef(typename, custom_defs):
+def _make_typedef(
+    typename: str, custom_defs: CustomDefs
+) -> Optional[StatefulEntityType]:
     typedef = None
     # prefix is only used to expand "tosca:Type"
     test_typedef = StatefulEntityType(
         typename, StatefulEntityType.NODE_PREFIX, custom_defs
     )
     if test_typedef.is_derived_from("tosca.nodes.Root"):
         typedef = NodeType(typename, custom_defs)
     elif test_typedef.is_derived_from("tosca.relationships.Root"):
         typedef = RelationshipType(typename, custom_defs)
     return typedef
 
 
-def to_graphql_nodetypes(spec):
+def _update_root_type(jsontype: GraphqlObject, sub_map: SubstitutionMappings):
+    "Modify a type representation so that it can be used with template with a nested topology."
+
+    # don't display any properties set by the inner topology
+    for name, value in sub_map.get_declared_properties().items():
+        inputsSchema = jsontype["inputsSchema"]["properties"].get(name)
+        if inputsSchema:
+            if is_value_computed(value):
+                del jsontype["inputsSchema"]["properties"][name]
+            else:
+                inputsSchema["default"] = value
+        else:
+            jsontype["computedPropertiesSchema"]["properties"].pop(name, None)
+
+    # make optional any requirements that were set in the inner topology
+    names = sub_map.get_declared_requirement_names()
+    for req in jsontype["requirements"]:
+        if req["name"] in names:
+            req["min"] = 0
+    # templates created with this type need to have the substitute directive
+    jsontype["directives"] = ["substitute"]
+
+
+def to_graphql_nodetypes(spec: ToscaSpec, include_all=True) -> ResourceTypesByName:
     # node types are readonly, so mapping doesn't need to be bijective
-    types: Dict[str, Dict[str, Any]] = {}
-    custom_defs = spec.template.topology_template.custom_defs
-    for typename in custom_defs:
-        if typename in types:
-            continue
-        typedef = _make_typedef(typename, custom_defs)
-        if typedef:
-            node_type_to_graphql(spec, typedef, types)
-    for typename in StatefulEntityType.TOSCA_DEF:  # builtin types
-        if typename.startswith("unfurl.nodes") or typename.startswith(
-            "unfurl.relationships"
-        ):
+    types = cast(ResourceTypesByName, {})
+    topology = spec.topology
+    assert topology
+    custom_defs = topology.topology_template.custom_defs
+    # create these ones first
+    # XXX detect error later if these types are being used elsewhere
+    for nested_topology in spec.nested_topologies:
+        sub_map = nested_topology.topology_template.substitution_mappings
+        if sub_map:
+            typedef = sub_map.node_type
+            if typedef:
+                jsontype = node_type_to_graphql(nested_topology, typedef, types)
+                _update_root_type(jsontype, sub_map)
+
+    if include_all:
+        for typename in custom_defs:
             if typename in types:
                 continue
-            # only include our extensions
             typedef = _make_typedef(typename, custom_defs)
             if typedef:
-                node_type_to_graphql(spec, typedef, types)
+                node_type_to_graphql(topology, typedef, types)
+        for typename in StatefulEntityType.TOSCA_DEF:  # builtin types
+            if typename.startswith("unfurl.nodes") or typename.startswith(
+                "unfurl.relationships"
+            ):
+                if typename in types:
+                    continue
+                # only include our extensions
+                typedef = _make_typedef(typename, custom_defs)
+                if typedef:
+                    node_type_to_graphql(topology, typedef, types)
 
-    for node_spec in spec.nodeTemplates.values():
+    for node_spec in topology.node_templates.values():
         type_definition = node_spec.toscaEntityTemplate.type_definition
         typename = type_definition.type
         if typename not in types:
-            node_type_to_graphql(spec, type_definition, types)
+            node_type_to_graphql(topology, type_definition, types)
 
     mark_leaf_types(types)
-    annotate_requirements(types)
+    assert spec.topology
+    annotate_requirements(spec.topology, types)
+
     return types
 
 
 # currently unused:
 # def deduce_valuetype(value):
 #     typemap = {
 #         int: "number",
@@ -676,44 +805,44 @@
 #     }
 #     for pythontype in typemap:
 #         if isinstance(value, pythontype):
 #             return dict(type=typemap[pythontype])
 #     return {}
 
 
-def add_capabilities_as_properties(schema, nodetype, spec):
+def add_capabilities_as_properties(schema, nodetype, custom_defs: CustomDefs):
     """treat each capability as a property and add them to props"""
     for cap in nodetype.get_capability_typedefs():
         if not cap.get_definition("properties"):
             continue
         propdefs = [
             p for p in cap.get_properties_def_objects() if is_property_user_visible(p)
         ]
-        schema[cap.name] = tosca_type_to_jsonschema(spec, propdefs, cap.type)
+        schema[cap.name] = tosca_type_to_jsonschema(custom_defs, propdefs, cap.type)
 
 
-def add_capabilities_as_attributes(schema, nodetype, spec):
+def add_capabilities_as_attributes(schema, nodetype, custom_defs: CustomDefs):
     """treat each capability as an attribute and add them to props"""
     for cap in nodetype.get_capability_typedefs():
         if not cap.get_definition("attributes"):
             continue
         propdefs = [
             p for p in cap.get_attributes_def_objects() if is_property_user_visible(p)
         ]
-        schema[cap.name] = tosca_type_to_jsonschema(spec, propdefs, cap.type)
+        schema[cap.name] = tosca_type_to_jsonschema(custom_defs, propdefs, cap.type)
 
 
-def _get_typedef(name: str, spec):
-    typedef = spec.template.topology_template.custom_defs.get(name)
+def _get_typedef(name: str, custom_defs: CustomDefs) -> Optional[StatefulEntityType]:
+    typedef = custom_defs.get(name)
     if not typedef:
         typedef = StatefulEntityType.TOSCA_DEF.get(name)
     return typedef
 
 
-def template_properties_to_json(nodetemplate, visitor):
+def template_properties_to_json(nodetemplate: NodeTemplate, visitor):
     # if they aren't only include ones with an explicity value
     for p in nodetemplate.get_properties_objects():
         computed = is_computed(p)
         if computed and not _is_get_env_or_secret(p.value):
             # don't expose values that are expressions to the user
             value = None
         else:
@@ -727,39 +856,71 @@
                 continue
             if computed:
                 # preserve the expression
                 value = p.value
         yield dict(name=p.name, value=value)
 
 
-def _get_requirement(req, nodetemplate, spec, types):
+def _get_requirement(
+    req: dict, nodespec: EntitySpec, types: ResourceTypesByName
+) -> Optional[GraphqlObject]:
     name, req_dict = _get_req(req)
     # we need to call _get_explicit_relationship() to make sure all the requirements relationships are created
     # _get_explicit_relationship returns req_dict merged with its type definition
-    req_dict, rel_template = nodetemplate._get_explicit_relationship(name, req_dict)
+    req_dict, rel_template = nodespec.toscaEntityTemplate._get_explicit_relationship(
+        name, req_dict
+    )
     if "constraint" in req_dict.get("metadata", {}):
         # this happens when we import graphql json directly
         reqconstraint = req_dict["metadata"]["constraint"]
     else:
-        reqconstraint = requirement_to_graphql(spec, {name: req_dict})
+        reqconstraint = requirement_to_graphql(nodespec.topology, {name: req_dict})
     if reqconstraint is None:
         return None
-    _annotate_requirement(reqconstraint, reqconstraint["resourceType"], types)
-    reqjson = dict(
-        constraint=reqconstraint, name=name, match=None, __typename="Requirement"
+
+    typeobj = types[nodespec.type]
+    if "substitute" in typeobj.get("directives", []):
+        # we've might have modified the type in _update_root_type()
+        # and the tosca object won't know about that change so set it now
+        for typeconstraint in typeobj["requirements"]:
+            if name == typeconstraint["name"]:
+                reqconstraint["min"] = typeconstraint["min"]
+
+    _annotate_requirement(
+        reqconstraint, reqconstraint["resourceType"], nodespec.topology, types
     )
-    if req_dict.get("node") and not _get_typedef(req_dict["node"], spec):
+    reqjson = GraphqlObject(
+        dict(constraint=reqconstraint, name=name, match=None, __typename="Requirement")
+    )
+    if req_dict.get("node") and not _get_typedef(
+        req_dict["node"], nodespec.topology.topology_template.custom_defs
+    ):
         # it's not a type, assume it's a node template
         # (the node template name might not match a template if it is only defined in the deployment blueprints)
         match = req_dict["node"]
         reqjson["match"] = match
     return reqjson
 
 
-def nodetemplate_to_json(nodetemplate, spec, types, for_resource=False):
+def _find_typename(
+    nodetemplate: EntityTemplate,
+    types: ResourceTypesByName,
+) -> str:
+    # XXX
+    # if we substituting template, generate a new type
+    # json type for root of imported blueprint only include unfulfilled requirements 
+    # and set defaults on properties set by the inner root
+    return nodetemplate.type
+
+
+def nodetemplate_to_json(
+    node_spec: EntitySpec,
+    types: ResourceTypesByName,
+    for_resource: bool = False,
+) -> GraphqlObject:
     """
     Returns json object as a ResourceTemplate:
 
     type ResourceTemplate {
       name: String!
       title: String
       type: ResourceType!
@@ -778,49 +939,55 @@
     type Requirement {
       name: String!
       constraint: RequirementConstraint!
       match: ResourceTemplate
       target: Resource
     }
     """
+    nodetemplate = node_spec.toscaEntityTemplate
+    spec = node_spec.spec
     if "__typename" in nodetemplate.entity_tpl:
         # previously imported from the json, just return it
         ogprops = nodetemplate.entity_tpl.pop("_original_properties", None)
         if ogprops is not None:
             nodetemplate.entity_tpl["properties"] = ogprops
         return nodetemplate.entity_tpl
 
-    json = dict(
-        type=nodetemplate.type,
-        name=nodetemplate.name,
-        title=nodetemplate.entity_tpl.get("metadata", {}).get("title")
-        or nodetemplate.name,
-        description=nodetemplate.entity_tpl.get("description") or "",
-        directives=nodetemplate.directives,
-        # __typename="ResourceTemplate",  # XXX
+    json = GraphqlObject(
+        dict(
+            type=_find_typename(nodetemplate, types),
+            name=nodetemplate.name,
+            title=nodetemplate.entity_tpl.get("metadata", {}).get("title")
+            or nodetemplate.name,
+            description=nodetemplate.entity_tpl.get("description") or "",
+            directives=nodetemplate.directives,
+            # __typename="ResourceTemplate",  # XXX
+        )
     )
     if "imported" in nodetemplate.entity_tpl:
         json["imported"] = nodetemplate.entity_tpl.get("imported")
 
     visitor = PropertyVisitor()
     json["properties"] = list(template_properties_to_json(nodetemplate, visitor))
     # if visitor.redacted and "predefined" not in nodetemplate.directives:
     #     json["directives"].append("predefined")
     #     logger.warning(
     #         "Adding 'predefined' directive to '%s' because it has redacted properties",
     #         nodetemplate.name,
     #     )
     json["dependencies"] = []
-    visibility = template_visibility(spec, nodetemplate, for_resource)
+    discovered = None if not for_resource else spec.discovered
+    visibility = template_visibility(node_spec, discovered)
     if visibility != "inherit":
         json["visibility"] = visibility
         logger.debug(f"setting visibility {visibility} on template {nodetemplate.name}")
 
     if not nodetemplate.type_definition.is_derived_from("tosca.nodes.Root"):
         return json
+
     # treat each capability as a complex property
     capabilities = nodetemplate.get_capabilities()
     for prop in json["properties"]:
         # properties are already added via the type definition
         cap = capabilities.get(prop["name"])
         if cap:
             # XXX need to map property values like property_value_to_json above
@@ -829,15 +996,15 @@
     # XXX
     # this is the same as on the type because of the bug where attribute set on a node_template are ignored
     # json["outputs"] = jsonnodetype["outputs"]
 
     has_visible_dependency = False
     ExceptionCollector.start()
     for req in nodetemplate.all_requirements:
-        reqjson = _get_requirement(req, nodetemplate, spec, types)
+        reqjson = _get_requirement(req, node_spec, types)
         if reqjson is None:
             continue
         if reqjson["constraint"].get("visibility") != "hidden":
             has_visible_dependency = True
         json["dependencies"].append(reqjson)
 
     if (
@@ -855,100 +1022,115 @@
             )
     return json
 
 
 primary_name = "__primary"
 
 
-def _generate_primary(spec, db, node_tpl=None):
+def _generate_primary(spec: ToscaSpec, db: GraphqlDB, node_tpl=None) -> NodeTemplate:
     base_type = node_tpl["type"] if node_tpl else "tosca.nodes.Root"
     topology = spec.template.topology_template
     # generate a node type and node template that represents root of the topology
     # generate a type that exposes the topology's inputs and outputs as properties and attributes
     attributes = {  # XXX is this computed?
         o.name: dict(default=o.value, type="string", description=o.description or "")
         for o in topology.outputs
     }
     nodetype_tpl = dict(
         derived_from=base_type, properties=topology._tpl_inputs(), attributes=attributes
     )
     # set as requirements all the node templates that aren't the target of any other requirements
+    assert spec.topology
     roots = [
         node.toscaEntityTemplate
-        for node in spec.nodeTemplates.values()
+        for node in spec.topology.node_templates.values()
         if not node.toscaEntityTemplate.get_relationship_templates()
         and "default" not in node.directives
     ]
     nodetype_tpl["requirements"] = [{node.name: dict(node=node.type)} for node in roots]
 
     topology.custom_defs[primary_name] = nodetype_tpl
     tpl = node_tpl or {}
     tpl["type"] = primary_name
     tpl.setdefault("properties", {}).update(
         {name: dict(get_input=name) for name in topology._tpl_inputs()}
     )
     # if create new template, need to assign the nodes explicitly (needed if multiple templates have the same type)
     if not node_tpl:
         tpl["requirements"] = [{node.name: dict(node=node.name)} for node in roots]
-    node_spec = spec.add_node_template(primary_name, tpl, False)
-    node_template = node_spec.toscaEntityTemplate
+    node_spec = spec.topology.add_node_template(primary_name, tpl, False)
+    node_template = cast(NodeTemplate, node_spec.toscaEntityTemplate)
 
-    types = db["ResourceType"]
-    node_type_to_graphql(spec, node_template.type_definition, types)
-    db["ResourceTemplate"][node_template.name] = nodetemplate_to_json(
-        node_template, spec, types
-    )
+    types = _get_types(db)
+    assert node_template.type_definition
+    node_type_to_graphql(spec.topology, node_template.type_definition, types)
+    db["ResourceTemplate"][node_template.name] = nodetemplate_to_json(node_spec, types)
     return node_template
 
 
 # if a node type or template is specified, use that, but it needs to be compatible with the generated type
-def _get_or_make_primary(spec, db):
+def _get_or_make_primary(spec: ToscaSpec, db: GraphqlDB) -> Tuple[str, str]:
     ExceptionCollector.start()  # topology.add_template may generate validation exceptions
+    assert spec.template
     topology = spec.template.topology_template
+    assert topology
     # we need to generate a root template
     root_type = None
     root = None
     if topology.substitution_mappings:
-        if topology.substitution_mappings.node:
-            root = topology.node_templates.get(topology.substitution_mappings.node)
-            if root:
-                root_type = root.type_definition
-        else:
-            assert topology.substitution_mappings.type
-            root_type = NodeType(
-                topology.substitution_mappings.type, topology.custom_defs
-            )
+        root_type = topology.substitution_mappings.node_type
+        root = topology.substitution_mappings._node_template
 
     if root_type:
         properties_tpl = root_type.get_definition("properties") or {}
-        for input in topology.inputs:
-            if input.name not in properties_tpl:
-                root = _generate_primary(spec, db, root and root.entity_tpl)
-                break
+        # if no property mapping in use, generate a new root template if there are any missing inputs
+        if (
+            not topology.substitution_mappings
+            or not topology.substitution_mappings.has_property_mapping()
+        ):
+            for input in topology.inputs:
+                if input.name not in properties_tpl:
+                    # there's an input that isn't handled by the type, generate a new one
+                    root = _generate_primary(spec, db, root and root.entity_tpl)
+                    break
         if not root:
             root = topology.node_templates.get(primary_name)
             if not root:
                 properties = {
                     name: dict(get_input=name) for name in topology._tpl_inputs()
                 }
                 tpl = dict(type=root_type.type, properties=properties)
-                node_spec = spec.add_node_template(primary_name, tpl, False)
+                assert spec.topology
+                node_spec = spec.topology.add_node_template(primary_name, tpl, False)
                 root = node_spec.toscaEntityTemplate
                 # XXX connections are missing
                 db["ResourceTemplate"][root.name] = nodetemplate_to_json(
-                    root, spec, db["ResourceType"]
+                    node_spec, _get_types(db)
                 )
     else:
         root = _generate_primary(spec, db)
 
     assert root
     return root.name, root.type
 
 
-def to_graphql_blueprint(spec, db):
+def blueprint_metadata(spec: ToscaSpec, root_name: str) -> GraphqlObject:
+    title, name = _template_title(spec, root_name)
+    blueprint = GraphqlObject(dict(name=name, title=title))
+    blueprint["description"] = spec.template.description
+    metadata = spec.template.tpl.get("metadata") or {}
+    blueprint["livePreview"] = metadata.get("livePreview")
+    blueprint["sourceCodeUrl"] = metadata.get("sourceCodeUrl")
+    blueprint["image"] = metadata.get("image")
+    blueprint["projectIcon"] = metadata.get("projectIcon")
+    blueprint["primaryDeploymentBlueprint"] = metadata.get("primaryDeploymentBlueprint")
+    return blueprint
+
+
+def to_graphql_blueprint(spec: ToscaSpec, db: GraphqlDB) -> Tuple[GraphqlObject, str]:
     """
     Returns json object as ApplicationBlueprint
 
     ApplicationBlueprint: {
       name: String!
       title: String
       description: String
@@ -960,25 +1142,18 @@
       sourceCodeUrl: String
       image: String
       projectIcon: String
     }
     """
     # note: root_resource_template is derived from inputs, outputs and substitution_template from topology_template
     root_name, root_type = _get_or_make_primary(spec, db)
-    title, name = _template_title(spec, root_name)
-    blueprint = dict(__typename="ApplicationBlueprint", name=name, title=title)
+    blueprint = blueprint_metadata(spec, root_name)
+    blueprint["__typename"] = "ApplicationBlueprint"
     blueprint["primary"] = root_type
-    blueprint["deploymentTemplates"] = []
-    blueprint["description"] = spec.template.description
-    metadata = spec.template.tpl.get("metadata") or {}
-    blueprint["livePreview"] = metadata.get("livePreview")
-    blueprint["sourceCodeUrl"] = metadata.get("sourceCodeUrl")
-    blueprint["image"] = metadata.get("image")
-    blueprint["projectIcon"] = metadata.get("projectIcon")
-    blueprint["primaryDeploymentBlueprint"] = metadata.get("primaryDeploymentBlueprint")
+    blueprint["deploymentTemplates"] = []  # type: ignore
     return blueprint, root_name
 
 
 def slugify(text):
     # XXX only allow env var names?
     text = text.lower().strip()
     text = re.sub(r"\s+", "-", text)
@@ -1006,33 +1181,37 @@
             "string",
             "boolean",
             "number",
         ]:
             yield f"{reqname}_{propdef.name.upper()}"
 
 
-def _generate_env_names(spec, root_name):
-    primary = spec.nodeTemplates[root_name]
+def _generate_env_names(spec: ToscaSpec, root_name: str) -> Iterator[str]:
+    assert spec.topology
+    primary = spec.topology.get_node_template(root_name)
+    assert primary
     custom_defs = spec.template.topology_template.custom_defs
     primary_type = primary.toscaEntityTemplate.type_definition
     yield from _generate_env_names_from_type("APP", primary_type, custom_defs)
     # primary.toscaEntityTemplate.type_definition
     for req in primary_type.get_all_requirements():
         # get the target type
-        req_json = requirement_to_graphql(spec, req)
+        req_json = requirement_to_graphql(spec.topology, req)
         if not req_json:
             continue
         name = req_json["name"]
         target_type = req_json["resourceType"]
         typedef = _make_typedef(target_type, custom_defs)
         assert typedef, target_type
         yield from _generate_env_names_from_type(name.upper(), typedef, custom_defs)
 
 
-def get_deployment_blueprints(manifest, blueprint, root_name, db):
+def get_deployment_blueprints(
+    manifest: YamlManifest, blueprint: GraphqlObject, root_name: str, db: GraphqlDB
+) -> dict:
     """
     The blueprint will include deployement blueprints that follows this syntax in the manifest:
 
     .. code-block:: YAML
 
       spec:
         deployment_blueprints:
@@ -1060,29 +1239,31 @@
       environmentVariableNames: [String!]
     }
     """
     deployment_blueprints = (
         manifest.manifest.expanded.get("spec", {}).get("deployment_blueprints") or {}
     )
     spec = manifest.tosca
+    assert spec and spec.topology
     deployment_templates = {}
     for name, tpl in deployment_blueprints.items():
         slug = slugify(name)
         template = tpl.copy()
         local_resource_templates = {}
         resource_templates = template.pop("resource_templates", None)
         if resource_templates:
+            topology = spec.topology.copy()
             for node_name, node_tpl in resource_templates.items():
                 # nodes here overrides node_templates
-                node_spec = spec.add_node_template(node_name, node_tpl, False)
-                node_template = node_spec.toscaEntityTemplate
+                node_spec = topology.add_node_template(node_name, node_tpl, False)
             # convert to json in second-pass template requirements can reference each other
             for node_name, node_tpl in resource_templates.items():
-                node_template = spec.nodeTemplates[node_name].toscaEntityTemplate
-                t = nodetemplate_to_json(node_template, spec, db["ResourceType"])
+                node_spec = topology.get_node_template(node_name)
+                assert node_spec
+                t = nodetemplate_to_json(node_spec, _get_types(db))
                 if t.get("visibility") == "omit":
                     continue
                 local_resource_templates[node_name] = t
 
         # XXX assert that db["ResourceTemplate"] has already has all the node_templates
         # names of ResourceTemplates:
         resourceTemplates = sorted(
@@ -1111,15 +1292,15 @@
 def _project_path(url):
     pp = urlparse(url).path.lstrip("/")
     if pp.endswith(".git"):
         return pp[:-4]
     return pp
 
 
-def get_blueprint_from_topology(manifest: YamlManifest, db):
+def get_blueprint_from_topology(manifest: YamlManifest, db: GraphqlDB):
     spec = manifest.tosca
     assert spec
     # XXX cloud = spec.topology.primary_provider
     blueprint, root_name = to_graphql_blueprint(spec, db)
     templates = get_deployment_blueprints(manifest, blueprint, root_name, db)
 
     template = {}
@@ -1159,70 +1340,152 @@
     template["environmentVariableNames"] = list(_generate_env_names(spec, root_name))
     last_commit_time = manifest.last_commit_time()
     if last_commit_time:
         template["commitTime"] = js_timestamp(last_commit_time)
     return blueprint, template
 
 
-def _to_graphql(localEnv):
+def _to_graphql(
+    localEnv: LocalEnv,
+) -> Tuple[GraphqlDB, YamlManifest, GraphqlObject, ResourceTypesByName]:
     # set skip_validation because we want to be able to dump incomplete service templates
-    manifest = localEnv.get_manifest(skip_validation=True)
-    db = {}
+    manifest = localEnv.get_manifest(skip_validation=True, safe_mode=True)
+    db = GraphqlDB({})
     spec = manifest.tosca
-    types_repo = spec.template.tpl.get("repositories").get("types")
+    assert spec
+    tpl = spec.template.tpl
+    assert spec.topology and tpl
+    types_repo = tpl.get("repositories").get("types")
     if types_repo:  # only export types, avoid built-in repositories
         db["repositories"] = {"types": types_repo}
     types = to_graphql_nodetypes(spec)
     db["ResourceType"] = types
     db["ResourceTemplate"] = {}
     environment_instances = {}
-    connection_types = {}
-    for node_spec in spec.nodeTemplates.values():
+    connection_types = cast(ResourceTypesByName, {})
+    for node_spec in spec.topology.node_templates.values():
         toscaEntityTemplate = node_spec.toscaEntityTemplate
-        t = nodetemplate_to_json(toscaEntityTemplate, spec, types)
+        t = nodetemplate_to_json(node_spec, types)
         if t.get("visibility") == "omit":
             continue
         name = t["name"]
         if "virtual" in toscaEntityTemplate.directives:
             # virtual is only set when loading resources from an environment
             # or from "spec/resource_templates"
             environment_instances[name] = t
             typename = toscaEntityTemplate.type_definition.type
             connection_types[typename] = types[typename]
         else:
             db["ResourceTemplate"][name] = t
 
     connections = {}
-    for template in spec.template.relationship_templates:
+    assert spec.topology
+    for relationship_spec in spec.topology.relationship_templates.values():
+        template = cast(RelationshipTemplate, relationship_spec.toscaEntityTemplate)
         if template.default_for:
             type_definition = template.type_definition
+            assert type_definition
             typename = type_definition.type
             if typename in types:
                 connection_types[typename] = types[typename]
             elif typename not in connection_types:
-                node_type_to_graphql(spec, type_definition, connection_types)
-            connection_template = nodetemplate_to_json(template, spec, connection_types)
+                node_type_to_graphql(spec.topology, type_definition, connection_types)
+            # this is actually a RelationshipTemplate
+            connection_template = nodetemplate_to_json(
+                relationship_spec, connection_types
+            )
             if connection_template.get("visibility") == "omit":
                 continue
             name = connection_template["name"]
             assert name not in db["ResourceTemplate"], f"template name conflict: {name}"
             # db["ResourceTemplate"][name] = connection_template
             connections[name] = connection_template
 
-    db["Overview"] = manifest.tosca.template.tpl.get("metadata") or {}
-    env = dict(
-        connections=connections,
-        primary_provider=connections.get("primary_provider"),
-        instances=environment_instances,
-        repositories=manifest.context.get("repositories") or {},
+    db["Overview"] = tpl.get("metadata") or {}
+    env = GraphqlObject(
+        dict(
+            connections=connections,
+            primary_provider=connections.get("primary_provider"),
+            instances=environment_instances,
+            repositories=manifest.context.get("repositories") or {},
+        )
     )
     return db, manifest, env, connection_types
 
 
-def add_graphql_deployment(manifest: YamlManifest, db, dtemplate):
+def _add_resources(
+    db: GraphqlDB,
+    relationships: Dict[str, List[GraphqlObject]],
+    root: TopologyInstance,
+    resources: List[GraphqlObject],
+    shadowed: Optional[EntityInstance],
+) -> None:
+    for instance in root.get_self_and_descendants():
+        # don't include the nested template that is a shadow of the outer template
+        if instance is not root and instance is not shadowed:
+            resource = to_graphql_resource(instance, db, relationships)
+            if not resource:
+                continue
+            resources.append(resource)
+            if cast(NodeSpec, instance.template).substitution and instance.shadow:
+                assert instance.shadow.root is not instance.root
+                _add_resources(
+                    db,
+                    relationships,
+                    cast(TopologyInstance, instance.shadow.root),
+                    resources,
+                    instance.shadow,
+                )
+
+
+def _add_lastjob(last_job: dict, deployment: GraphqlObject) -> None:
+    readyState = last_job.get("readyState")
+    workflow = last_job.get("workflow")
+    deployment["workflow"] = workflow
+    if isinstance(readyState, dict):
+        deployment["status"] = to_enum(
+            Status, readyState.get("effective", readyState.get("local"))
+        )
+        if workflow == "undeploy" and deployment["status"] == Status.ok:
+            deployment["status"] = Status.absent
+    deployment["summary"] = last_job.get("summary")
+    deployTimeString = last_job.get("endTime", last_job["startTime"])
+    deployment["deployTime"] = js_timestamp(
+        datetime.datetime.strptime(deployTimeString, ChangeRecord.DateTimeFormat)
+    )
+
+
+def _set_deployment_url(
+    manifest, deployment: GraphqlObject, primary_resource: Optional[GraphqlObject]
+):
+    outputs = manifest.get_saved_outputs()
+    if outputs and "url" in outputs:
+        url = outputs["url"]
+    else:
+        # computed outputs might not be saved, so try to evaluate it now
+        try:
+            url = manifest.rootResource.attributes["outputs"].get("url")
+        except UnfurlError as e:
+            url = None  # this can be raised if the evaluation is unsafe
+            logger.warning(
+                f"export could not evaluate output 'url': {e}"
+            )
+
+    if url:
+        deployment["url"] = url
+    elif primary_resource and primary_resource.get("attributes"):
+        for prop in primary_resource["attributes"]:
+            if prop["name"] == "url":
+                deployment["url"] = prop["value"]
+                break
+
+
+def add_graphql_deployment(
+    manifest: YamlManifest, db: GraphqlDB, dtemplate
+) -> GraphqlObject:
     """
     type Deployment {
       title: String!
       primary: Resource
       resources: [Resource!]
       deploymentTemplate: DeploymentTemplate!
       url: url
@@ -1230,139 +1493,128 @@
       summary: String
       workflow: String
       deployTime: String
     }
     """
     name = dtemplate["name"]
     title = dtemplate.get("title") or name
-    deployment = dict(name=name, title=title, __typename="Deployment")
+    deployment = GraphqlObject(dict(name=name, title=title, __typename="Deployment"))
     templates = db["ResourceTemplate"]
-    relationships: Dict[str, List[Dict]] = {}
+    relationships: Dict[str, List[GraphqlObject]] = {}
     for t in templates.values():
         if "dependencies" in t:
             for c in t["dependencies"]:
                 if c.get("match"):
                     relationships.setdefault(c["match"], []).append(c)
     assert manifest.rootResource
-    resources = [
-        to_graphql_resource(instance, manifest, db, relationships)
-        for instance in manifest.rootResource.get_self_and_descendants()
-        if instance is not manifest.rootResource
-    ]
-    db["Resource"] = {r["name"]: r for r in resources if r}
+    resources: List[GraphqlObject] = []
+    _add_resources(db, relationships, manifest.rootResource, resources, None)
+    db["Resource"] = {r["name"]: r for r in resources}
     deployment["resources"] = list(db["Resource"])
     primary_name = deployment["primary"] = dtemplate["primary"]
     deployment["deploymentTemplate"] = dtemplate["name"]
     if manifest.lastJob:
-        readyState = manifest.lastJob.get("readyState")
-        workflow = manifest.lastJob.get("workflow")
-        deployment["workflow"] = workflow
-        if isinstance(readyState, dict):
-            deployment["status"] = to_enum(
-                Status, readyState.get("effective", readyState.get("local"))
-            )
-            if workflow == "undeploy" and deployment["status"] == Status.ok:
-                deployment["status"] = Status.absent
-        deployment["summary"] = manifest.lastJob.get("summary")
-        deployTimeString = manifest.lastJob.get(
-            "endTime", manifest.lastJob["startTime"]
-        )
-        deployment["deployTime"] = js_timestamp(
-            datetime.datetime.strptime(deployTimeString, ChangeRecord.DateTimeFormat)
-        )
+        _add_lastjob(manifest.lastJob, deployment)
 
-    url = manifest.rootResource.attributes["outputs"].get("url")
     primary_resource = db["Resource"].get(primary_name)
+    _set_deployment_url(manifest, deployment, primary_resource)
     if primary_resource and primary_resource["title"] == primary_name:
         primary_resource["title"] = deployment["title"]
-    if url:
-        deployment["url"] = url
-    elif primary_resource and primary_resource.get("attributes"):
-        for prop in primary_resource["attributes"]:
-            if prop["name"] == "url":
-                deployment["url"] = prop["value"]
-                break
     db["Deployment"] = {name: deployment}
     return deployment
 
 
-def to_blueprint(localEnv, existing=None):
+def to_blueprint(localEnv: LocalEnv, existing: Optional[str] = None) -> GraphqlDB:
     db, manifest, env, env_types = _to_graphql(localEnv)
+    assert manifest.tosca
     blueprint, root_name = to_graphql_blueprint(manifest.tosca, db)
     deployment_blueprints = get_deployment_blueprints(
         manifest, blueprint, root_name, db
     )
     db["DeploymentTemplate"] = deployment_blueprints
     blueprint["deploymentTemplates"] = list(deployment_blueprints)
     db["ApplicationBlueprint"] = {blueprint["name"]: blueprint}
     return db
 
 
 # NB! to_deployment is the default export format used by __main__.export (but you won't find that via grep)
-def to_deployment(localEnv, existing=None):
+def to_deployment(localEnv: LocalEnv, existing: Optional[str] = None) -> GraphqlDB:
     logger.debug("exporting deployment %s", localEnv.manifestPath)
     db, manifest, env, env_types = _to_graphql(localEnv)
     blueprint, dtemplate = get_blueprint_from_topology(manifest, db)
     db["DeploymentTemplate"] = {dtemplate["name"]: dtemplate}
     db["ApplicationBlueprint"] = {blueprint["name"]: blueprint}
     add_graphql_deployment(manifest, db, dtemplate)
     # don't include base node type:
     db["ResourceType"].pop("tosca.nodes.Root")
     logger.debug("finished exporting deployment %s", localEnv.manifestPath)
     return db
 
 
-def mark_leaf_types(types):
+def mark_leaf_types(types) -> None:
     # types without implementations can't be instantiated by users
     # treat non-leaf types as abstract types that shouldn't be instatiated
     # treat leaf types that have requirements as having implementations
     counts: Counter = Counter()
     for rt in types.values():
         for name in rt["extends"]:
             counts[name] += 1
-    for (name, count) in counts.most_common():
+    for name, count in counts.most_common():
         jsontype = types.get(name)
         if not jsontype:
             continue
         if count == 1:
             # not subtyped so assume its a concrete type
             if not jsontype.get("implementations") and jsontype.get("requirements"):
                 # hack: if we're a "compound" type that is just a sum of its requirement, add an implementation so it is included
                 jsontype["implementations"] = ["create"]
         elif jsontype.get("implementations"):
             jsontype["implementations"] = []
 
 
-def annotate_requirements(types):
-    for jsontype in types.values():
+def annotate_requirements(topology: TopologySpec, types: ResourceTypesByName) -> None:
+    for jsontype in list(types.values()):  # _annotate_requirement() might modify types
         for req in jsontype.get("requirements") or []:
-            _annotate_requirement(req, req["resourceType"], types)
+            _annotate_requirement(req, req["resourceType"], topology, types)
 
 
-def _annotate_requirement(req: dict, reqtypename: str, types: dict) -> None:
+def _annotate_requirement(
+    req: GraphqlObject,
+    reqtypename: str,
+    topology: TopologySpec,
+    types: ResourceTypesByName,
+) -> None:
     # req is a RequirementConstraint dict
+    reqtype = types.get(reqtypename)
+    if not reqtype:
+        custom_defs = topology.topology_template.custom_defs
+        typedef = _make_typedef(reqtypename, custom_defs)
+        if typedef:
+            reqtype = node_type_to_graphql(topology, typedef, types)
+        else:
+            return
+
     if "node_filter" not in req:
         return
     node_filter = req["node_filter"]
-    reqtype = types[reqtypename]
     req_filters = node_filter.get("requirements")
     # node_filter properties might refer to properties that are only present on some subtypes
     prop_filters: Dict = {}
     for typename in reqtype["extends"]:
         if typename not in types:
             continue
         subtype: Dict = types[typename]
         inputsSchemaProperties = subtype["inputsSchema"]["properties"]
         _map_nodefilter_properties(req, inputsSchemaProperties, prop_filters)
 
     if prop_filters:
         req["inputsSchema"] = dict(properties=prop_filters)
     if req_filters:
         req["requirementsFilter"] = [
-            _make_req(rf, types, reqtypename)[2] for rf in req_filters
+            _make_req(rf, topology, types, reqtypename)[2] for rf in req_filters
         ]
     req.pop("node_filter")
 
 
 def _map_nodefilter_properties(filters, inputsSchemaProperties, jsonprops) -> dict:
     ONE_TO_ONE_MAP = dict(object="map", array="list")
     # {i["name"]: inputsSchemaProperties
@@ -1395,78 +1647,66 @@
     if instances:
         for instance_name, value in instances.items():
             if "imported" in value:
                 env_instances[instance_name] = value
     return env_instances
 
 
-def to_environments(localEnv, existing=None):
+def to_environments(localEnv: LocalEnv, existing: Optional[str] = None) -> GraphqlDB:
     """
-      Map environments in unfurl.yaml to DeploymentEnvironments
-      Map registered ensembles to deployments just with path reference to the ensemble's json
+    Map the environments in the project's unfurl.yaml to a json collection of Graphql objects.
+    Each environment is be represented as:
 
-      type DeploymentEnvironment {
-        name: String!
-        connections: [ResourceTemplate!]
-        instances: [ResourceTemplate!]
+    type DeploymentEnvironment {
+      name: String!
+      connections: [ResourceTemplate!]
+      instances: [ResourceTemplate!]
+      primary_provider: ResourceTemplate
+      repositories: JSON!
+    }
 
-        primary_provider: ResourceTemplate
-        deployments: [String!]
-      }
+    Unlike the other JSON exports, the ResourceTemplates are included inline
+    instead of referenced by name (so the json can be included directly into unfurl.yaml).
 
-    # save service templates in this format so we can include this json in unfurl.yaml
-    {
-      "DeploymentEnvironment": {
-        name: {
-          "connections": { name: <ResourceTemplate>},
-          "instances": { name: <ResourceTemplate>}
-        }
-      },
-
-      "ResourceType": {
-        name: <ResourceType>
-      },
-    }
+    Each registered ensembles will be represents as a DeploymentPath object
+    with the ensemble's path as its name.
+
+    Also include ResourceType objects for any types referenced in the environments' connections and instances.
     """
 
     # XXX one manifest and blueprint per environment
-    if existing and os.path.exists(existing):
-        with open(existing) as f:
-            db = json.load(f)
-    else:
-        db = {}
+    db = _load_db(existing)
     environments = {}
-    all_connection_types = {}
+    all_connection_types = cast(ResourceTypesByName, {})
     blueprintdb = None
-    deployments = set_deploymentpaths(localEnv.project)["DeploymentPath"]
+    assert localEnv.project
+    deployment_paths = get_deploymentpaths(localEnv.project)
     env_deployments = {}
-    for ensemble_info in deployments.values():
+    for ensemble_info in deployment_paths.values():
         env_deployments[ensemble_info["environment"]] = ensemble_info["name"]
+    assert localEnv.project
     defaults = localEnv.project.contexts.get("defaults")
     default_imported_instances = _set_shared_instances(
         defaults and defaults.get("instances")
     )
+    default_manifest_path = localEnv.manifestPath
     for name in localEnv.project.contexts:
         try:
+            # we can reuse the localEnv if there's a distinct manifest that uses this environment
+            localEnv.manifest_context_name = name
             if name in env_deployments:
-                # we can reuse the localEnv if there's a distinct manifest that uses this environment
-                localEnv.manifest_context_name = name
                 localEnv.manifestPath = os.path.join(
                     localEnv.project.projectRoot, env_deployments[name], "ensemble.yaml"
                 )
-                localLocalEnv = localEnv
             else:
-                # this environment doesn't have any deployments so we have to create a new localEnv
-                # because we need to instantiate a different ToscaSpec object
-                localLocalEnv = LocalEnv(
-                    localEnv.manifestPath,
-                    project=localEnv.project,
-                    override_context=name,
-                    readonly=True,
-                )
+                # this environment doesn't have any deployments, reuse the default one
+                # delete existing because we need to instantiate a different ToscaSpec object
+                localEnv._manifests.pop(default_manifest_path, None)
+                localEnv.manifestPath = default_manifest_path
+            localLocalEnv = localEnv
             blueprintdb, manifest, env, env_types = _to_graphql(localLocalEnv)
             env["name"] = name
             env["instances"].update(default_imported_instances)
             instances = localEnv.project.contexts[name].get("instances")
             env["instances"].update(_set_shared_instances(instances))
             environments[name] = env
             all_connection_types.update(env_types)
@@ -1479,120 +1719,152 @@
         # if blueprintdb.get("repositories", {}).get("types"):
         #     # don't include ResourceTypes if we are including a types repository
         #     db["ResourceType"] = all_connection_types
         #     return db
 
         # add the rest of the types too
         # XXX is it safe to only include types with "connect" implementations?
-        all_connection_types.update(blueprintdb["ResourceType"])
-    db["ResourceType"] = all_connection_types
-    db["DeploymentPath"] = deployments
+        all_connection_types.update(_get_types(blueprintdb))
+    db["ResourceType"] = cast(GraphqlObjectsByName, all_connection_types)
+    db["DeploymentPath"] = deployment_paths
     return db
 
 
-def to_deployments(localEnv, existing=None):
-    db = set_deploymentpaths(localEnv.project)
-    deployments = db["deployments"] = []
+class DeploymentPaths(TypedDict):
+    DeploymentPath: GraphqlObjectsByName
+
+
+class Deployments(DeploymentPaths):
+    deployments: List[GraphqlDB]
+
+
+def to_deployments(localEnv: LocalEnv, existing: Optional[str] = None) -> Deployments:
+    assert localEnv.project
+    db = cast(Deployments, set_deploymentpaths(localEnv.project))
+    deployments: List[GraphqlDB] = []
+    db["deployments"] = deployments
     for manifest_path, dp in db["DeploymentPath"].items():
+        # start_time = perf_counter()
         try:
             # optimization: reuse localenv
             localEnv.manifestPath = os.path.join(
                 localEnv.project.projectRoot, manifest_path, "ensemble.yaml"
             )
             environment = dp.get("environment") or "defaults"
             localEnv.manifest_context_name = environment
             deployments.append(to_deployment(localEnv))
         except Exception:
             logger.error("error exporting deployment %s", manifest_path, exc_info=True)
+        # _print(f"{perf_counter() - start_time}s export for {manifest_path}")
 
     # from .yamlloader import yaml_perf
     # _print(f"exported {len(deployments)} deployments, {yaml_perf} seconds parsing yaml")
+    # from .manifest import _cache
+    # _print("cached files with access count", json.dumps([(k, v[1]) for k, v in _cache.items()], indent=2))
     return db
 
 
-def get_deploymentpaths(project):
+def get_deploymentpaths(project: Project) -> GraphqlObjectsByName:
     return set_deploymentpaths(project)["DeploymentPath"]
 
 
-def set_deploymentpaths(project, existing=None):
-    if existing:
+def _load_db(existing: Optional[str]) -> GraphqlDB:
+    if existing and os.path.exists(existing):
         with open(existing) as f:
-            db = json.load(f)
+            return cast(GraphqlDB, json.load(f))
     else:
-        db = {}
+        return GraphqlDB({})
+
+
+def set_deploymentpaths(
+    project: Project, existing: Optional[str] = None
+) -> DeploymentPaths:
+    """
+    Deployments identified by their file path.
+
+    type DeploymentPath {
+      name: String!
+      environment: String!
+      project_id: String
+      pipelines: [JSON!]
+      incremental_deploy: boolean!
+    }
+    """
+    db = cast(DeploymentPaths, _load_db(existing))
     deployment_paths = db.setdefault("DeploymentPath", {})
     for ensemble_info in project.localConfig.ensembles:
         if "environment" in ensemble_info and "project" not in ensemble_info:
             # exclude external ensembles
             path = os.path.dirname(ensemble_info["file"])
             if os.path.isabs(path):
                 path = project.get_relative_path(path)
-            obj = {
-                "__typename": "DeploymentPath",
-                "name": path,
-                "project_id": ensemble_info.get("project_id"),
-                "pipelines": ensemble_info.get("pipelines", []),
-                "environment": ensemble_info["environment"],
-                "incremental_deploy": ensemble_info.get("incremental_deploy", False),
-            }
+            obj = GraphqlObject(
+                {
+                    "__typename": "DeploymentPath",
+                    "name": path,
+                    "project_id": ensemble_info.get("project_id"),
+                    "pipelines": ensemble_info.get("pipelines", []),
+                    "environment": ensemble_info["environment"],
+                    "incremental_deploy": ensemble_info.get(
+                        "incremental_deploy", False
+                    ),
+                }
+            )
             if path in deployment_paths:
                 # merge duplicate entries
                 deployment_paths[path].update(obj)
             else:
                 deployment_paths[path] = obj
     return db
 
 
-def add_attributes(instance):
+def add_attributes(instance: EntityInstance) -> List[Dict[str, Any]]:
     attrs = []
     attributeDefs = instance.template.attributeDefs.copy()
     # instance._attributes only has values that were set by the instance, not spec properties or attribute defaults
     # instance._attributes should already be serialized
-    if instance._attributes:
-        for name, value in instance._attributes.items():
+    if instance.shadow:
+        _attributes = instance.shadow._attributes
+    else:
+        _attributes = instance._attributes
+    if _attributes:
+        for name, value in _attributes.items():
             p = attributeDefs.pop(name, None)
             if not p:
-                # check if shadowed property
+                # check if this attribute is shadowing a property
                 p = instance.template.propertyDefs.get(name)
                 if not p:
                     # same as EntityTemplate._create_properties()
                     p = Property(
                         name,
                         value,
                         dict(type="any"),
                         instance.template.toscaEntityTemplate.custom_def,
                     )
             if not p.schema.get("metadata", {}).get("internal"):
                 attrs.append(dict(name=p.name, value=attribute_value_to_json(p, value)))
     # add leftover attribute defs that have a default value
     for prop in attributeDefs.values():
         if prop.default is not None:
-            if always_export(prop):
-                # evaluate computed property now
-                attrs.append(
-                    dict(
-                        name=prop.name,
-                        value=attribute_value_to_json(
-                            prop, instance.attributes[prop.name]
-                        ),
-                    )
-                )
-            elif not is_computed(prop):
+            if not maybe_export_value(prop, instance, attrs) and not is_computed(prop):
                 attrs.append(
                     dict(
                         name=prop.name,
                         value=attribute_value_to_json(prop, prop.default),
                     )
                 )
     return attrs
 
 
-def add_computed_properties(instance):
+def add_computed_properties(instance: EntityInstance) -> List[Dict[str, Any]]:
     attrs = []
-    _attributes = instance._attributes or {}
+    if instance.shadow:
+        _attributes = instance.shadow._attributes
+    else:
+        _attributes = instance._attributes
     # instance._properties should already be serialized
     _properties = instance._properties or {}
     if _properties:
         for name, value in _properties.items():
             if name in _attributes:  # shadowed, don't include both
                 continue
             p = instance.template.propertyDefs.get(name)
@@ -1609,24 +1881,16 @@
                     value = p.value
                 else:
                     value = attribute_value_to_json(p, value)
                 attrs.append(dict(name=p.name, value=value))
 
     for prop in instance.template.propertyDefs.values():
         if prop.default is not None and prop.name not in instance._properties:
-            if always_export(prop) and prop.name not in instance.template.attributeDefs:
-                # evaluate computed property now
-                attrs.append(
-                    dict(
-                        name=prop.name,
-                        value=attribute_value_to_json(
-                            prop, instance.attributes[prop.name]
-                        ),
-                    )
-                )
+            if prop.name not in instance.template.attributeDefs:
+                maybe_export_value(prop, instance, attrs)
 
     return attrs
 
 
 def is_resource_real(instance):
     for resource_types in ["unfurl.nodes.CloudObject", "unfurl.nodes.K8sRawResource"]:
         if instance.template.is_compatible_type(resource_types):
@@ -1636,15 +1900,19 @@
         or "console_url" in instance.attributes
         or "url" in instance.attributes
     ):
         return True
     return False
 
 
-def to_graphql_resource(instance, manifest, db, relationships):
+def to_graphql_resource(
+    instance: EntityInstance,
+    db: GraphqlDB,
+    relationships: Dict[str, List[GraphqlObject]],
+) -> Optional[GraphqlObject]:
     """
     type Resource {
       name: String!
       title: String!
       url: String
       template: ResourceTemplate!
       status: Status
@@ -1659,31 +1927,32 @@
     # XXX url
     template = db["ResourceTemplate"].get(instance.template.name)
     pending = not instance.status or instance.status == Status.pending
     if not template:
         if pending or "virtual" in instance.template.directives:
             return None
         template = nodetemplate_to_json(
-            instance.template.toscaEntityTemplate,
-            manifest.tosca,
-            db["ResourceType"],
+            instance.template,
+            _get_types(db),
             True,
         )
         if template.get("visibility") == "omit":
             return None
         db["ResourceTemplate"][instance.template.name] = template
 
-    resource = dict(
-        name=instance.name,
-        title=template.get("title", instance.name),
-        template=instance.template.name,
-        state=instance.state,
-        status=instance.status,
-        __typename="Resource",
-        imported=instance.imported,
+    resource = GraphqlObject(
+        dict(
+            name=instance.nested_name,
+            title=template.get("title", instance.name),
+            template=instance.template.name,
+            state=instance.state,
+            status=instance.status,
+            __typename="Resource",
+            imported=instance.imported,
+        )
     )
 
     if "visibility" in template and template["visibility"] != "inherit":
         resource["visibility"] = template["visibility"]
     else:
         if instance.template.name in relationships:
             visibilities = set(
```

### Comparing `unfurl-0.6.2/unfurl/tosca_plugins/artifacts.yaml` & `unfurl-0.7.0/unfurl/tosca_plugins/artifacts.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/tosca_plugins/googlecloud.yaml` & `unfurl-0.7.0/unfurl/tosca_plugins/googlecloud.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/tosca_plugins/k8s.yaml` & `unfurl-0.7.0/unfurl/tosca_plugins/k8s.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -108,15 +108,22 @@
       name:
         type: string
         default:
           eval: .name
     attributes:
       namespace:
         type: string
-        default: { get_property: [HOST, name] }
+        default:
+          eval:
+            if:
+              is_function_defined: kubernetes_current_namespace
+            then:
+              kubernetes_current_namespace:
+            else:
+              get_property: [HOST, name]
 
   unfurl.nodes.K8sSecretResource:
     derived_from: unfurl.nodes.K8sResource
     properties:
       definition:
         metadata:
           # hide because this is computed from the "type" and "data" properties
```

### Comparing `unfurl-0.6.2/unfurl/tosca_plugins/localhost.yaml` & `unfurl-0.7.0/unfurl/tosca_plugins/localhost.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/tosca_plugins/tosca-ext.yaml` & `unfurl-0.7.0/unfurl/tosca_plugins/tosca-ext.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/unfurl-schema.json` & `unfurl-0.7.0/unfurl/unfurl-schema.json`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/util.py` & `unfurl-0.7.0/unfurl/util.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/sphinx-jsonschema/__init__.py` & `unfurl-0.7.0/unfurl/vendor/sphinx-jsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/sphinx-jsonschema/wide_format.py` & `unfurl-0.7.0/unfurl/vendor/sphinx-jsonschema/wide_format.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/__init__.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/__init__.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/activities.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/activities.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/artifacts.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/artifacts.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/capabilities.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/capabilities.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/common/exception.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/common/exception.py`

 * *Files 18% similar despite different names*

```diff
@@ -223,30 +223,42 @@
     @staticmethod
     def exceptionsCaught():
         return len(ExceptionCollector.exceptions) > 0
 
     @staticmethod
     def getTraceString(traceList):
         traceString = ''
-        for entry in traceList:
-            f, l, m, c = entry[0], entry[1], entry[2], entry[3]
-            traceString += (_('\t\tFile %(file)s, line %(line)s, in '
-                              '%(method)s\n\t\t\t%(call)s\n')
-                            % {'file': f, 'line': l, 'method': m, 'call': c})
+        if traceList:
+          for entry in traceList:
+              f, l, m, c = entry[0], entry[1], entry[2], entry[3]
+              traceString += (_('\t\tFile %(file)s, line %(line)s, in '
+                                '%(method)s\n\t\t\t%(call)s\n')
+                              % {'file': f, 'line': l, 'method': m, 'call': c})
         return traceString
 
     @staticmethod
     def getExceptionReportEntry(exception, full=True, extra=True):
         entry = exception.__class__.__name__ + ': ' + str(exception)
         if extra and getattr(exception, 'near', None):
-          entry += exception.near
+            entry += exception.near
+        if exception.__cause__:
+            entry += f"\nCaused by:{exception.__cause__.__class__.__name__}:{exception.__cause__}\n"
         if full:
             entry += '\n' + ExceptionCollector.getTraceString(exception.trace)
+            if exception.__cause__:
+                cause = exception.__cause__
+                if cause.__traceback__:
+                    cause.trace = traceback.extract_tb(cause.__traceback__)[:-1]
+                else:
+                    cause.trace = ()
+                entry += '\n' + ExceptionCollector.getExceptionReportEntry(cause, full, extra)
         return entry
 
+
+
     @staticmethod
     def getExceptions():
         return ExceptionCollector.exceptions
 
     @staticmethod
     def getExceptionsReport(full=True, extra=True):
         report = []
```

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/dataentity.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/dataentity.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_0.yaml` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_0.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_3.yaml` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/TOSCA_definition_1_3.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/artifacttype.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/artifacttype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/attribute_definition.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/attribute_definition.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/capabilitytype.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/capabilitytype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/constraints.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/constraints.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/datatype.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/datatype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/entity_type.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/entity_type.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/grouptype.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/grouptype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/interfaces.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,29 +263,31 @@
         else:
             operations[op] = baseDef
 
 
 def merge_interfacedefs(base, derived, _source):
     # merge the interfaces defined on the type with the template's interface definitions
     for iName, defs in derived.items():
+        if not isinstance(defs, dict):
+            continue
         # for each interface, see if base defines it too
         cls = getattr(defs, "mapCtor", defs.__class__)
         defs = cls(defs)
         inputs = defs.get('inputs') or cls()
         if 'operations' in defs:
             operations = defs['operations'] or cls()
         else:
             operations = defs
 
         baseDefs = base.get(iName)
         if baseDefs:
             # add in base's ops and merge interface-level inputs
             baseInputs = baseDefs.get('inputs')
             if baseInputs:  # merge shared inputs
-                inputs = dict(baseInputs, **inputs)
+                inputs = cls(baseInputs, **inputs)
                 defs['inputs'] = inputs
 
             # set shared implementation
             implementation = baseDefs.get('implementation')
             if implementation and 'implementation' not in defs:
                 defs['implementation'] = implementation
                 if isinstance(implementation, dict) and _source:
```

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/nodetype.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/nodetype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/policytype.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/policytype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/portspectype.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/portspectype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/property_definition.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/property_definition.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/relationshiptype.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/relationshiptype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/scalarunit.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/scalarunit.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/statefulentitytype.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/statefulentitytype.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
             ifaces = self.get_value(self.INTERFACES)
 
         if ifaces:
             for name, value in ifaces.items():
                 operation_names = None
                 if not isinstance(value, dict):
                     ExceptionCollector.appendException(TypeMismatchError(
-                                                       what=value,
+                                                       what=f"interface {name}",
                                                        type="dict"))
                     continue
                 if name == 'Mock':
                     error_source._common_validate_field(
                         value, INTERFACE_DEF_RESERVED_WORDS,
                         'interfaces')
                 elif name == 'defaults':
```

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/elements/tosca_type_validation.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/elements/tosca_type_validation.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/entity_template.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/entity_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,19 +247,25 @@
             properties = {}
         if not isinstance(properties, dict):
             ExceptionCollector.appendException(
               TypeMismatchError(
                   what='"properties" of template "%s"' % self.name,
                   type='dict'))
             return {}
-        if not self.entity_tpl.get(self.IMPORTED):
+        if self._should_validate_properties():
             # this is just a placeholder template for the imported one so it might not have properties
             self._common_validate_properties(self.type_definition, properties, self.additionalProperties)
         return properties
 
+    def _should_validate_properties(self):
+        return not self.entity_tpl.get(self.IMPORTED)
+
+    def revalidate_properties(self):
+        self._common_validate_properties(self.type_definition, self.get_properties(), self.additionalProperties)
+
     def _validate_capabilities(self):
         type_capabilities = self.type_definition.get_capabilities_def()
         allowed_caps = \
             type_capabilities.keys() if type_capabilities else []
         capabilities = self.type_definition.get_value(self.CAPABILITIES,
                                                       self.entity_tpl)
         if capabilities:
@@ -397,7 +403,10 @@
     def get_capability(self, name):
         """Provide named capability
 
         :param name: name of capability
         :return: capability object if found, None otherwise
         """
         return self.get_capabilities().get(name)
+
+    def __repr__(self):
+        return f"{self.__class__}({self.name})"
```

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/exttools.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/exttools.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml` & `unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml` & `unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml` & `unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/functions.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/functions.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/groups.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/groups.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/imports.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/prereq/csar.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,379 +6,385 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-import logging
-import os
+import os.path
+import requests
+import shutil
+import tempfile
+import yaml
+import zipfile
+
+from io import BytesIO
 
 from toscaparser.common.exception import ExceptionCollector
-from toscaparser.common.exception import InvalidPropertyValueError
-from toscaparser.common.exception import MissingRequiredFieldError
-from toscaparser.common.exception import UnknownFieldError
-from toscaparser.common.exception import ValidationError
 from toscaparser.common.exception import URLException
-from toscaparser.elements.tosca_type_validation import TypeValidation
+from toscaparser.common.exception import ValidationError
+from toscaparser.imports import ImportsLoader
 from toscaparser.utils.gettextutils import _
-import toscaparser.utils.urlutils
-import toscaparser.utils.yamlparser
-from six.moves.urllib.parse import urlparse
-from toscaparser.repositories import Repository
-
-
-YAML_LOADER = toscaparser.utils.yamlparser.load_yaml
-log = logging.getLogger("tosca")
-
-
-class ImportResolver(object):
-    def get_repository(self, name, tpl):
-        return Repository(name, tpl)
-
-    def get_repository_url(self, importsLoader, repository_name):
-        repo_def = importsLoader.repositories[repository_name]
-        url = repo_def["url"].strip()
-        if url.startswith("file:") and importsLoader:
-            url_path = url[5:]
-            # its relative so join with current location of import
-            if not os.path.isabs(url_path) and importsLoader.path:
-                if os.path.isdir(importsLoader.path):
-                    base_path = importsLoader.path
-                else:
-                    base_path = os.path.dirname(importsLoader.path)
-                return "file://" + os.path.join(base_path, url_path)
+from toscaparser.utils.urlutils import UrlUtils
+from toscaparser.utils import yamlparser
 
-        return url
 
-    def get_url(self, importsLoader, repository_name, file_name, isFile=None):
-        if repository_name:
-            full_url = self.get_repository_url(importsLoader, repository_name)
-            if file_name:
-                full_url = full_url.rstrip("/") + "/" + file_name
-        else:
-            full_url = file_name
-        if isFile:
-            return full_url, True, None
-
-        parsed = urlparse(full_url)
-        if parsed.scheme == "file":
-            path = parsed.path
-            if importsLoader.path:
-                if os.path.isdir(importsLoader.path):
-                    base_path = importsLoader.path
-                else:
-                    base_path = os.path.dirname(importsLoader.path)
-                path = os.path.join(base_path, path)
-            return path, True, parsed.fragment
-        if toscaparser.utils.urlutils.UrlUtils.validate_url(full_url):
-            return full_url, False, None
-        else:
-            return None
+TOSCA_META = 'TOSCA-Metadata/TOSCA.meta'
 
-    def load_yaml(self, importsLoader, path, isFile=True, fragment=None):
-        return YAML_LOADER(path, isFile, importsLoader, fragment)
+YAML_LOADER = yamlparser.load_yaml
 
-    def load_imports(self, importsLoader, importslist):
-        importsLoader.importslist = importslist
-        importsLoader._validate_and_load_imports()
-
-
-class ImportsLoader(object):
-
-    IMPORTS_SECTION = (FILE, REPOSITORY, NAMESPACE_URI, NAMESPACE_PREFIX, WHEN) = (
-        "file",
-        "repository",
-        "namespace_uri",
-        "namespace_prefix",
-        "when",
-    )
-
-    def __init__(
-        self, importslist, path, type_definition_list=None, repositories=None, resolver=None
-    ):
-        self.importslist = importslist
-        self.custom_defs = {}
-        self.nested_tosca_tpls = []
-        self.resolver = resolver or ImportResolver()
-        self.path = path
-        self.repositories = repositories or {}
-        # names of type definition sections
-        self.type_definition_list = type_definition_list or []
-        if importslist is not None:
-            if not path:
-                msg = _("Input tosca template is not provided.")
-                log.warning(msg)
-                ExceptionCollector.appendException(ValidationError(message=msg))
-            self._validate_and_load_imports()
-
-    def get_custom_defs(self):
-        return self.custom_defs
-
-    def get_nested_tosca_tpls(self):
-        return self.nested_tosca_tpls
-
-    def _validate_and_load_imports(self):
-        imports_names = set()
-
-        if not self.importslist:
-            msg = _('"imports" keyname is defined without including ' "templates.")
-            log.error(msg)
-            ExceptionCollector.appendException(ValidationError(message=msg))
-            return
 
-        for import_def in self.importslist:
-            if isinstance(import_def, dict):
-                if len(import_def) == 1 and "file" not in import_def:
-                    # old style {name: uri}
-                    import_name, import_uri = list(import_def.items())[0]
-                    if import_name in imports_names:
-                        msg = _('Duplicate import name "%s" was found.') % import_name
-                        log.error(msg)
-                        ExceptionCollector.appendException(ValidationError(message=msg))
-                    imports_names.add(import_name)
-                else:  # new style {"file": uri}
-                    import_name = None
-                    import_uri = import_def
-
-            else:  # import_def is just the uri string
-                import_name = None
-                import_uri = import_def
-
-            full_file_name, imported_tpl = self._load_import_template(
-                import_name, import_uri
-            )
-            if full_file_name is None:
-                return
-
-            namespace_prefix = None
-            if isinstance(import_uri, dict):
-                namespace_prefix = import_uri.get(self.NAMESPACE_PREFIX)
-            if imported_tpl:
-                TypeValidation(imported_tpl, import_def)
-                self._update_custom_def(imported_tpl, namespace_prefix, full_file_name)
-            # XXX should save prefix too
-            self._update_nested_tosca_tpls(full_file_name, imported_tpl)
-
-    def _update_custom_def(self, imported_tpl, namespace_prefix, path):
-        path = os.path.normpath(path)
-        for type_def_section in self.type_definition_list:
-            outer_custom_types = imported_tpl.get(type_def_section)
-            if outer_custom_types:
-                if type_def_section in [
-                    "node_types",
-                    "relationship_types",
-                    "artifact_types",
-                ]:
-                    for custom_def in outer_custom_types.values():
-                        custom_def["_source"] = path
-                if namespace_prefix:
-                    prefix_custom_types = {}
-                    for type_def_key in outer_custom_types:
-                        namespace_prefix_to_key = namespace_prefix + "." + type_def_key
-                        prefix_custom_types[
-                            namespace_prefix_to_key
-                        ] = outer_custom_types[type_def_key]
-                    self.custom_defs.update(prefix_custom_types)
-                else:
-                    self.custom_defs.update(outer_custom_types)
+class CSAR(object):
 
-    def _update_nested_tosca_tpls(self, full_file_name, custom_tpl):
-        if full_file_name and custom_tpl:
-            topo_tpl = {full_file_name: custom_tpl}
-            self.nested_tosca_tpls.append(topo_tpl)
-
-    def _validate_import_keys(self, import_name, import_uri_def):
-        if self.FILE not in import_uri_def.keys():
-            log.warning(
-                'Missing keyname "file" in import "%(name)s".' % {"name": import_name}
-            )
-            ExceptionCollector.appendException(
-                MissingRequiredFieldError(
-                    what='Import of template "%s"' % import_name, required=self.FILE
-                )
-            )
-        for key in import_uri_def.keys():
-            if key not in self.IMPORTS_SECTION:
-                log.warning(
-                    'Unknown keyname "%(key)s" error in '
-                    'imported definition "%(def)s".' % {"key": key, "def": import_name}
-                )
+    def __init__(self, csar_file, a_file=True):
+        self.path = csar_file
+        self.a_file = a_file
+        self.is_validated = False
+        self.csar = None
+        self.temp_dir = None
+        self.is_tosca_metadata = False
+        self.main_template_file_name = None
+        self.zfile = None
+
+    def validate(self):
+        """Validate the provided CSAR file."""
+
+        self.is_validated = True
+
+        # validate that the file or URL exists
+        missing_err_msg = (_('"%s" does not exist.') % self.path)
+        if self.a_file:
+            if not os.path.isfile(self.path):
                 ExceptionCollector.appendException(
-                    UnknownFieldError(
-                        what='Import of template "%s"' % import_name, field=key
-                    )
-                )
-
-    def _load_import_template(self, import_name, import_uri_def):
-        """Handle custom types defined in imported template files
-
-        This method loads the custom type definitions referenced in "imports"
-        section of the TOSCA YAML template by determining whether each import
-        is specified via a file reference (by relative or absolute path) or a
-        URL reference.
-
-        Possibilities:
-        +----------+--------+------------------------------+
-        | template | import | comment                      |
-        +----------+--------+------------------------------+
-        | file     | file   | OK                           |
-        | file     | URL    | OK                           |
-        | preparsed| file   | file must be a full path     |
-        | preparsed| URL    | OK                           |
-        | URL      | file   | file must be a relative path |
-        | URL      | URL    | OK                           |
-        +----------+--------+------------------------------+
-        """
-        path, a_file, fragment = self._resolve_import_template(
-            import_name, import_uri_def
-        )
-        if path is not None:
-            try:
-                doc = self.resolver.load_yaml(self, path, a_file, fragment)
-            except:
-                msg = _('Import "%s" is not valid.') % path
-                ExceptionCollector.appendException(URLException(what=msg))
-                return None, None
-            return getattr(doc, "path", path), doc
+                    ValidationError(message=missing_err_msg))
+                return False
+            else:
+                self.csar = self.path
+        else:  # a URL
+            if not UrlUtils.validate_url(self.path):
+                ExceptionCollector.appendException(
+                    ValidationError(message=missing_err_msg))
+                return False
+            else:
+                response = requests.get(self.path)
+                self.csar = BytesIO(response.content)
+
+        # validate that it is a valid zip file
+        if not zipfile.is_zipfile(self.csar):
+            err_msg = (_('"%s" is not a valid zip file.') % self.path)
+            ExceptionCollector.appendException(
+                ValidationError(message=err_msg))
+            return False
+
+        # validate that it contains the metadata file in the correct location
+        self.zfile = zipfile.ZipFile(self.csar, 'r')
+        filelist = self.zfile.namelist()
+        if TOSCA_META in filelist:
+            self.is_tosca_metadata = True
+            # validate that 'Entry-Definitions' property exists in TOSCA.meta
+            is_validated = self._validate_tosca_meta(filelist)
         else:
-            return None, None
+            self.is_tosca_metadata = False
+            is_validated = self._validate_root_level_yaml(filelist)
 
-    def _resolve_import_template(self, import_name, import_uri_def):
-        short_import_notation = False
-        if isinstance(import_uri_def, dict):
-            self._validate_import_keys(import_name, import_uri_def)
-            file_name = import_uri_def.get(self.FILE)
-            repository = import_uri_def.get(self.REPOSITORY)
-            repos = self.repositories.keys()
-            if repository is not None:
-                if repository not in repos:
-                    ExceptionCollector.appendException(
-                        ValidationError(
-                            message=_('Repository not found: "%s"') % repository
-                        )
-                    )
-                    return None, None, None
+        if is_validated:
+            # validate that external references and imports in the main
+            # template actually exist and are accessible
+            main_tpl = self._read_template_yaml(self.main_template_file_name)
+            self._validate_external_references(main_tpl)
+        return not ExceptionCollector.exceptionsCaught()
+
+    def get_metadata(self):
+        """Return the metadata dictionary."""
+
+        # validate the csar if not already validated
+        if not self.is_validated:
+            self.validate()
+
+        # return a copy to avoid changes overwrite the original
+        return dict(self.metadata) if self.metadata else None
+
+    def _get_metadata(self, key):
+        if not self.is_validated:
+            self.validate()
+        return self.metadata.get(key)
+
+    def get_author(self):
+        if self.is_tosca_metadata:
+            return self._get_metadata('Created-By')
         else:
-            file_name = import_uri_def
-            repository = None
-            short_import_notation = True
-
-        if file_name is None:
-            msg = _(
-                "A template file name is not provided with import "
-                'definition "%(import_name)s".'
-            ) % {"import_name": import_name}
-            log.error(msg)
-            ExceptionCollector.appendException(ValidationError(message=msg))
-            return None, None, None
-
-        if toscaparser.utils.urlutils.UrlUtils.validate_url(file_name):
-            # it's an absolute URL
-            return self.resolver.get_url(self, repository, file_name, False)
-
-        if not repository:
-            fragment = None
-            import_template = None
-            if self.path:
-                if toscaparser.utils.urlutils.UrlUtils.validate_url(self.path):
-                    if os.path.isabs(file_name):
-                        msg = _(
-                            'Absolute file name "%(name)s" cannot be '
-                            "used in a URL-based input template "
-                            '"%(template)s".'
-                        ) % {"name": file_name, "template": self.path}
-                        log.error(msg)
-                        ExceptionCollector.appendException(ImportError(msg))
-                        return None, None, None
-                    import_template = toscaparser.utils.urlutils.UrlUtils.join_url(
-                        self.path, file_name
-                    )
-                    assert import_template
-                    a_file = False
-                else:
-                    a_file = True
-                    main_a_file = os.path.isfile(self.path)
-                    if "#" in file_name:
-                        file_name, sep, fragment = file_name.rpartition("#")
-                    if os.path.isabs(file_name):
-                        import_template = file_name
-                    elif os.path.isdir(self.path):
-                        import_template = os.path.join(self.path, file_name)
-                    elif main_a_file:
-                        if os.path.isfile(file_name):
-                            import_template = file_name
-                        else:
-                            full_path = os.path.join(
-                                os.path.dirname(os.path.abspath(self.path)), file_name
-                            )
-                            if os.path.isfile(full_path):
-                                import_template = full_path
+            # In case CSAR zip doesn't contain TOSCA.Metadata directory,
+            # Created-By is defined by the template_author metadata
+            return self._get_metadata('template_author')
+
+    def get_version(self):
+        if self.is_tosca_metadata:
+            return self._get_metadata('CSAR-Version')
+        else:
+            # In case CSAR zip doesn't contain TOSCA.Metadata directory,
+            # CSAR-Version is defined by the template_version metadata
+            return self._get_metadata('template_version')
+
+    def get_main_template(self):
+        if not self.is_validated:
+            self.validate()
+        return self.main_template_file_name
+
+    def get_main_template_yaml(self):
+        main_template = self.get_main_template()
+        if main_template:
+            data = self.zfile.read(main_template)
+            invalid_tosca_yaml_err_msg = (
+                _('The file "%(template)s" in the CSAR "%(csar)s" does not '
+                  'contain valid TOSCA YAML content.') %
+                {'template': main_template, 'csar': self.path})
+            try:
+                tosca_yaml = yaml.safe_load(data)
+                if type(tosca_yaml) is not dict:
+                    ExceptionCollector.appendException(
+                        ValidationError(message=invalid_tosca_yaml_err_msg))
+                return tosca_yaml
+            except Exception:
+                ExceptionCollector.appendException(
+                    ValidationError(message=invalid_tosca_yaml_err_msg))
+
+    def get_description(self):
+        desc = self._get_metadata('Description')
+        if desc is not None:
+            return desc
+
+        self.metadata['Description'] = \
+            self.get_main_template_yaml().get('description')
+        return self.metadata['Description']
+
+    def decompress(self):
+        if not self.is_validated:
+            self.validate()
+        self.temp_dir = tempfile.NamedTemporaryFile().name
+        with zipfile.ZipFile(self.csar, "r") as zf:
+            zf.extractall(self.temp_dir)
+
+    def _validate_external_artifact_imports(self, main_tpl, tpl_filename):
+        """validate the imports and artifacts"""
+
+        self._validate_template(main_tpl, tpl_filename)
+
+        if main_tpl:
+            if 'imports' in main_tpl:
+                custom_service = ImportsLoader(
+                    main_tpl['imports'],
+                    os.path.join(self.temp_dir, tpl_filename))
+
+                # Get list of nested templates
+                nested_tosca_tpls = custom_service.get_nested_tosca_tpls()
+
+                # Validate external references of each nested template.
+                if nested_tosca_tpls:
+                    for tosca_tpl in nested_tosca_tpls:
+                        for filename, tpl in tosca_tpl.items():
+                            self._validate_external_artifact_imports(
+                                tpl,
+                                filename)
+
+    def _validate_external_references(self, main_tpl):
+        """Extracts files referenced in the main template
+
+        These references are currently supported:
+        * imports
+        * interface implementations
+        * artifacts
+        """
+        try:
+            self.decompress()
+            self._validate_external_artifact_imports(
+                main_tpl,
+                self.main_template_file_name)
+        finally:
+            if self.temp_dir:
+                shutil.rmtree(self.temp_dir)
+
+    def _validate_template(self, template_data, template):
+        if 'topology_template' in template_data:
+            topology_template = template_data['topology_template']
+
+            if 'node_templates' in topology_template:
+                node_templates = topology_template['node_templates']
+
+                for node_template_key in node_templates:
+                    node_template = node_templates[node_template_key]
+                    if 'artifacts' in node_template:
+                        artifacts = node_template['artifacts']
+                        for artifact_key in artifacts:
+                            artifact = artifacts[artifact_key]
+                            if isinstance(artifact, str):
+                                self._validate_external_reference(
+                                    node_templates,
+                                    template,
+                                    artifact)
+                            elif isinstance(artifact, dict):
+                                if 'file' in artifact:
+                                    self._validate_external_reference(
+                                        node_templates,
+                                        template,
+                                        artifact['file'])
                             else:
-                                file_path = file_name.rpartition(os.path.sep)
-                                dir_path = os.path.dirname(os.path.abspath(self.path))
-                                if file_path[0] != "" and dir_path.endswith(
-                                    file_path[0]
-                                ):
-                                    import_template = os.path.join(
-                                        dir_path, file_path[2]
-                                    )
-                                    if not os.path.isfile(import_template):
-                                        msg = _(
-                                            '"%(import_template)s" is'
-                                            "not a valid file"
-                                        ) % {"import_template": import_template}
-                                        log.error(msg)
-                                        ExceptionCollector.appendException
-                                        (ValueError(msg))
-                                else:
-                                    import_template = full_path  # try anyway
-
-            else:  # template is pre-parsed
-                if os.path.isabs(file_name) and os.path.isfile(file_name):
-                    a_file = True
-                    import_template = file_name
+                                ExceptionCollector.appendException(
+                                    ValueError(_('Unexpected artifact '
+                                                 'definition for "%s".')
+                                               % artifact_key))
+
+                    if 'interfaces' in node_template:
+                        interfaces = node_template['interfaces']
+                        for interface_key in interfaces:
+                            interface = interfaces[interface_key]
+                            for opertation_key in interface:
+                                operation = interface[opertation_key]
+                                if isinstance(operation, str):
+                                    self._validate_external_reference(
+                                        node_templates,
+                                        template,
+                                        operation,
+                                        False)
+                                elif isinstance(operation, dict):
+                                    if 'implementation' in operation:
+                                        self._validate_external_reference(
+                                            node_templates,
+                                            template,
+                                            operation['implementation'],
+                                            False)
+
+    def _validate_external_reference(self, node_templates, tpl_file,
+                                     resource_file, raise_exc=True):
+        """Verify that the external resource exists
+
+        If resource_file is a URL verify that the URL is valid.
+        If resource_file is a relative path verify that the path is valid
+        considering base folder (self.temp_dir) and tpl_file.
+        If resource_file is not a path verify that it is a valid
+        implementation name by matching the artifact name.
+        Note that in a CSAR resource_file cannot be an absolute path.
+        """
+        if UrlUtils.validate_url(resource_file):
+            msg = (_('The resource at "%s" cannot be accessed.') %
+                   resource_file)
+            try:
+                if UrlUtils.url_accessible(resource_file):
+                    return
                 else:
-                    msg = _(
-                        'Relative file name "%(name)s" cannot be used '
-                        "in a pre-parsed input template."
-                    ) % {"name": file_name}
-                    log.error(msg)
-                    ExceptionCollector.appendException(ImportError(msg))
-                    return None, None, None
-
-            if not import_template:
+                    ExceptionCollector.appendException(
+                        URLException(what=msg))
+            except Exception:
                 ExceptionCollector.appendException(
-                    ImportError(_('Import "%s" is not valid.') % import_uri_def)
-                )
-                return None, None, None
-
-            url_info = self.resolver.get_url(self, repository, import_template, a_file)
-            if not url_info:
-                log.error(_('Import "%s" is not valid.') % import_uri_def)
+                    URLException(what=msg))
+
+        if os.path.isfile(os.path.join(self.temp_dir,
+                                       os.path.dirname(tpl_file),
+                                       resource_file)):
+            return
+        elif self._validate_artifact_name(node_templates):
+            return
+        else:
+            raise_exc = True
+
+        if raise_exc:
+            ExceptionCollector.appendException(
+                ValueError(_('The resource "%s" does not exist.')
+                           % resource_file))
+
+    def _read_template_yaml(self, template):
+        data = self.zfile.read(template)
+        invalid_tosca_yaml_err_msg = (
+            _('The file "%(template)s" in the CSAR "%(csar)s" does not '
+              'contain valid YAML content.') %
+            {'template': template, 'csar': self.path})
+        try:
+            tosca_yaml = yaml.safe_load(data)
+            if type(tosca_yaml) is not dict:
                 ExceptionCollector.appendException(
-                    ImportError(_('Import "%s" is not valid.') % import_uri_def)
-                )
-                return None, None, None
-            return url_info[0], url_info[1], fragment
+                    ValidationError(message=invalid_tosca_yaml_err_msg))
+                return None
+            return tosca_yaml
+        except Exception:
+            ExceptionCollector.appendException(
+                ValidationError(message=invalid_tosca_yaml_err_msg))
+            return None
+
+    def _validate_tosca_meta(self, filelist):
+        tosca = self._read_template_yaml(TOSCA_META)
+        if tosca is None:
+            return False
+
+        self.metadata = tosca
+
+        if 'Entry-Definitions' not in self.metadata:
+            err_msg = (_('The CSAR "%s" is missing the required metadata '
+                         '"Entry-Definitions" in '
+                         '"TOSCA-Metadata/TOSCA.meta".')
+                       % self.path)
+            ExceptionCollector.appendException(
+                ValidationError(message=err_msg))
+            return False
 
-        if short_import_notation:
-            log.error('Import "%(name)s" is not valid.' % import_uri_def)
+        # validate that 'Entry-Definitions' metadata value points to an
+        # existing file in the CSAR
+        entry = self.metadata.get('Entry-Definitions')
+        if entry and entry not in filelist:
+            err_msg = (_('The "Entry-Definitions" file defined in the '
+                         'CSAR "%s" does not exist.') % self.path)
             ExceptionCollector.appendException(
-                ImportError(_('Import "%s" is not valid.') % import_uri_def)
-            )
-            return None, None, None
-
-        assert repository
-        return self._resolve_from_repository(repository, import_name, file_name)
-
-    def _resolve_from_repository(self, repository, import_name, file_name):
-        url_info = self.resolver.get_url(self, repository, file_name)
-        if not url_info:
-            msg = _(
-                'repository url "%(n_uri)s" is not valid in import '
-                'definition "%(tpl)s".'
-            ) % {"n_uri": self.repositories[repository]["url"], "tpl": import_name}
-            log.error(msg)
-            ExceptionCollector.appendException(ImportError(msg))
-            return None, None, None
-        return url_info
+                ValidationError(message=err_msg))
+            return False
+
+        self.main_template_file_name = entry
+        return True
+
+    def _validate_root_level_yaml(self, filelist):
+        root_files = []
+        for file in filelist:
+            if '/' not in file:
+                __, file_extension = os.path.splitext(file)
+                if file_extension in ['.yaml', '.yml']:
+                    root_files.append(file)
+
+        if not len(root_files) == 1:
+            err_msg = (_('CSAR file should contain only one root level yaml'
+                         ' file. Found "%d" yaml file(s).') % len(root_files))
+            ExceptionCollector.appendException(
+                ValidationError(message=err_msg))
+            return False
+
+        template_data = self._read_template_yaml(root_files[0])
+        if template_data is None:
+            return False
+
+        tosca_version = template_data.get('tosca_definitions_version')
+        if tosca_version == 'tosca_simple_yaml_1_0':
+            err_msg = (_('"%s" is not a valid CSAR as it does not contain'
+                         ' the required file "TOSCA.meta" in the'
+                         ' folder "TOSCA-Metadata".') % self.path)
+            ExceptionCollector.appendException(
+                ValidationError(message=err_msg))
+            return False
+
+        self.metadata = template_data.get('metadata')
+        self.main_template_file_name = root_files[0]
+        return True
+
+    def _validate_artifact_name(self, node_templates):
+        artifact_name = "none"
+        for node_template_key in node_templates:
+            node_template = node_templates[node_template_key]
+            if 'artifacts' in node_template:
+                artifacts = node_template['artifacts']
+                for artifact_key in artifacts:
+                    artifact_name = artifact_key
+
+            if 'interfaces' in node_template:
+                interfaces = node_template['interfaces']
+                for interface_key in interfaces:
+                    interface = interfaces[interface_key]
+                    for operation_key in interface:
+                        operation = interface[operation_key]
+                        if 'implementation' in operation:
+                            if artifact_name == operation['implementation']:
+                                return True
+        return False
```

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/nodetemplate.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/nodetemplate.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,30 +33,41 @@
 
 class NodeTemplate(EntityTemplate):
     '''Node template from a Tosca profile.'''
     def __init__(self, name, topology_template, custom_def=None,
                  available_rel_tpls=None):
         node_templates = topology_template._tpl_nodetemplates()
         ExceptionCollector.near = f' in node template "{name}"'
+        self.topology_template = topology_template
         super(NodeTemplate, self).__init__(name, node_templates[name],
                                            'node_type',
                                            custom_def)
-        self.topology_template = topology_template
         self.templates = node_templates
         self.custom_def = custom_def
         self.related = {}
         self.relationship_tpl = []
         self.available_rel_tpls = available_rel_tpls or []
         self._relationships = None
-        self.sub_mapping_tosca_template = None
+        self.substitution = None
         self._artifacts = None
         self._instance_keys = None
         self._all_requirements = None
         self._missing_requirements = None
 
+    def _should_validate_properties(self):
+        for name in ("select", "substitute"):
+            if name in self.directives:
+                return False
+        # if we're in a nested topology and we're the root node, defer validation till substitution
+        root_topology = self.topology_template.tosca_template and self.topology_template.tosca_template.topology_template
+        if root_topology and root_topology is not self.topology_template:
+            if self.name in ("_substitution_mapping", self.topology_template._tpl_substitution_mappings().get("node")):
+                return False
+        return super()._should_validate_properties()
+
     @property
     def all_requirements(self):
         """
         returns [{name: requires_tpl_dict}]
         """
         if self._all_requirements is None:
             self._all_requirements = []
@@ -86,25 +97,38 @@
             self._missing_requirements = {}
             if not self.type_definition:
                 return self._relationships
             # self.requirements is from the yaml
             requires = self.requirements
             type_requirements = self.type_definition.requirement_definitions
             names = []
+
+            if self.topology_template.substitution_mappings:
+                # if this node_template is substituted one, add or replace the outer node templates requirements
+                # (set in outer_reqs)
+                substituted = self.topology_template.substitution_mappings._update_requirements(self)
+            else:
+                substituted = []
+
             if requires and isinstance(requires, list):
                 for r in requires:
-                    name, value = next(iter(r.items())) # list only has one item
+                    name, value = next(iter(r.items()))  # list only has one item
+                    if name in substituted:
+                        continue
                     names.append(name)
                     reqDef, relTpl = self._get_explicit_relationship(name, value)
                     if relTpl:
                         self._relationships.append( (relTpl, r, reqDef) )
+                        if self.substitution:
+                            # this needs to be called before the substituted node.relationships is called
+                            self.substitution.add_relationship(name, value, relTpl)
 
             # add requirements on the type definition that were not defined by the template
             for name, req_on_type in type_requirements.items():
-                if name not in names:
+                if name not in names and name not in substituted:
                     node = req_on_type.get('node')
                     is_template = node and self.find_node_related_template(node)
                     if is_template:
                         relTpl = self._relationship_from_req(name, req_on_type)
                         if relTpl:
                             self._relationships.append( (relTpl, {name: req_on_type}, req_on_type) )
                     elif "occurrences" not in req_on_type or req_on_type["occurrences"][0]:
@@ -257,15 +281,15 @@
                             continue
                         elif "default" in related_node.directives:
                             related_node = found
                             related_capability = found_cap
                         else:
                             ExceptionCollector.appendException(
                           ValidationError(message=
-      'requirement "%s" of node ""%s" is ambiguous, targets more than one template: "%s" and "%s"' %
+      'requirement "%s" of node "%s" is ambiguous, targets more than one template: "%s" and "%s"' %
                                         (name, self.name, related_node.name, found.name)))
                             return None
                     else:
                         related_node = found
                         related_capability = found_cap
 
         if related_node:
@@ -432,19 +456,23 @@
                       ExceptionCollector.appendException(
                         ValidationError(message=compoundKeyMsg))
             elif not isinstance(key, str):
                 ExceptionCollector.appendException(
                     ValidationError(message=msg))
 
     def _validate_nodefilter_filter(self, node_filter, cap_label=''):
-        valid = True
         if cap_label:
             name = 'capability "%s" on nodefilter on template "%s"' % (cap_label, self.name)
         else:
             name = 'nodefilter on template "%s"' % self.name
+        return self.validate_filter(node_filter, name)
+
+    @staticmethod
+    def validate_filter(node_filter, name):
+        valid = True
         if not isinstance(node_filter, dict):
             ExceptionCollector.appendException(
                 TypeMismatchError(
                     what=name,
                     type='dict'))
             return False
         if 'properties' in node_filter:
```

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/parameters.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/parameters.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/policy.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/policy.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/properties.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/properties.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/relationship_template.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/relationship_template.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/repositories.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/repositories.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/reservation.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/reservation.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/shell.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/shell.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/steps.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/steps.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/substitution_mappings.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/substitution_mappings.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,236 +18,282 @@
 from toscaparser.common.exception import MissingRequiredFieldError
 from toscaparser.common.exception import MissingRequiredInputError
 from toscaparser.common.exception import UnknownFieldError
 from toscaparser.common.exception import UnknownOutputError
 from toscaparser.common.exception import ValidationError
 from toscaparser.elements.nodetype import NodeType
 from toscaparser.utils.gettextutils import _
+from toscaparser.nodetemplate import NodeTemplate
 
-log = logging.getLogger('tosca')
+log = logging.getLogger("tosca")
 
 
 class SubstitutionMappings(object):
-    '''SubstitutionMappings class declaration
+    """SubstitutionMappings class declaration
 
     SubstitutionMappings exports the topology template as an
     implementation of a Node type.
-    '''
+    """
 
-    SECTIONS = (NODE, NODE_TYPE, REQUIREMENTS, CAPABILITIES, PROPERTIES,
-                        SUBSTITUTION_FILTER, ATTRIBUTES, INTERFACES) = \
-               ('node', 'node_type', 'requirements', 'capabilities', 'properties',
-               'substitution_filter', 'attributes', 'interfaces')
+    # added in 1.3: substitution_filter, attributes, interfaces (and node is an extension)
+    SECTIONS = (
+        NODE,
+        NODE_TYPE,
+        REQUIREMENTS,
+        CAPABILITIES,
+        PROPERTIES,
+        SUBSTITUTION_FILTER,
+        ATTRIBUTES,
+        INTERFACES,
+    ) = (
+        "node",
+        "node_type",
+        "requirements",
+        "capabilities",
+        "properties",
+        "substitution_filter",
+        "attributes",
+        "interfaces",
+    )
 
-    # XXX added in 1.3: substitution_filter, attributes, interfaces,
-    # XXX currently only supports property name to input name mapping
+    OPTIONAL_OUTPUTS = ["tosca_id", "tosca_name", "state"]
 
-    OPTIONAL_OUTPUTS = ['tosca_id', 'tosca_name', 'state']
-
-    def __init__(self, sub_mapping_def, topology, inputs, outputs,
-                 sub_mapped_node_template, custom_defs):
+    def __init__(self, sub_mapping_def, topology):
         self.topology = topology
         self.sub_mapping_def = sub_mapping_def
-        self.inputs = {input.name : input for input in inputs} if inputs else {}
-        self.outputs = outputs or []
-        self.sub_mapped_node_template = sub_mapped_node_template
-        self.custom_defs = custom_defs or {}
-        self.node_definition = None
+        if topology:
+            self.inputs = {input.name: input for input in topology.inputs}
+            self.outputs = topology.outputs or []
+        else:
+            self.inputs = {}
+            self.outputs = []
+        self.sub_mapped_node_template = None
+        self.node_type = None
         self._capabilities = None
         self._requirements = None
         self._properties = None
+        self._node_template = None
+        self._outer_relationships = {}
         self._validate()
 
+    def match(self, nodetemplate):
+        if self.node_type and self.node_type.is_derived_from(nodetemplate.type):
+            if self.substitution_filter:
+                return nodetemplate.match_nodefilter(self.substitution_filter)
+            return True
+        return False
+
+    def _make_node(self):
+        if not self.node_type:
+            return None
+        tpl = dict(type=self.node_type.type, properties=self.properties)
+        # XXX capabilities, requirements, attributes
+        return self.topology.add_template("_substitution_mapping", tpl, False)
+
+    def substitute(self, nodetemplate, remaining_topologies):
+        if nodetemplate:
+            assert not self._outer_relationships
+            # each substituted node template should have its own topology
+            topology = self.topology.copy()
+            return topology.substitution_mappings._substitute(
+                nodetemplate, remaining_topologies
+            )
+        else:
+            return self._substitute(nodetemplate, remaining_topologies)
+
+    def _substitute(self, nodetemplate, remaining_topologies):
+        if not self._node_template:
+            self._node_template = self._make_node()
+        if not self._node_template:
+            return self
+
+        if nodetemplate:
+            # we only care about outputs matching attributes when we have a node to substitute
+            self._validate_outputs()
+
+            # update our node template with the substituted template's properties:
+            current_props = self._node_template.get_properties()
+            for p in nodetemplate.get_properties_objects():
+                if p.name in current_props:
+                    # XXX what if schema is incompatible?
+                    current_props[p.name].value = p.value
+                else:
+                    self._node_template._properties.append(p)
+            nodetemplate.substitution = self
+            self.sub_mapped_node_template = nodetemplate
+
+        self._node_template.revalidate_properties()
+        # topology might have to do its own substitutions:
+        if remaining_topologies:
+            self.topology._do_substitutions(remaining_topologies)
+        return self
+
     @property
     def type(self):
         if self.sub_mapping_def:
             return self.sub_mapping_def.get(self.NODE_TYPE)
 
     @property
-    def node_type(self):
-        return self.sub_mapping_def.get(self.NODE_TYPE)
-
-    @property
     def node(self):
         return self.sub_mapping_def.get(self.NODE)
 
     @property
     def capabilities(self):
         return self.sub_mapping_def.get(self.CAPABILITIES)
 
     @property
     def requirements(self):
         return self.sub_mapping_def.get(self.REQUIREMENTS)
 
     @property
+    def substitution_filter(self):
+        return self.sub_mapping_def.get(self.SUBSTITUTION_FILTER)
+
+    @property
     def properties(self):
+        # 3.8.8 Property mapping
         if self._properties is None:
             self._properties = {}
             mapping = self.sub_mapping_def.get(self.PROPERTIES)
-            if mapping:
-                self._map(mapping, self.inputs, self._properties)
+            if mapping is not None:
+                self._map(mapping, self._properties)
+            else:
+                # property mapping not defined, use all the inputs
+                inputs = self.topology.parsed_params or {}
+                for name, input in self.inputs.items():
+                    if name in inputs:
+                        value = inputs[name]
+                    else:
+                        value = input.default
+                    self._properties[name] = value
         return self._properties
 
-    def _map(self, mapping, source, dest):
+    def has_property_mapping(self):
+        return self.PROPERTIES in self.sub_mapping_def and not self.node
+
+    def get_declared_properties(self):
+        if self.node:
+            node = self.topology.node_templates.get(self.node)
+            if node:
+                return node._properties_tpl
+        else:
+            return self.properties
+        return {}
+
+    def get_declared_requirement_names(self):
+        if self.node:
+            node = self.topology.node_templates.get(self.node)
+            if node:
+                 # list only has one item
+                return [next(iter(r)) for r in node.requirements]
+        return []  # XXX extract from requirement mapping
+
+    def add_relationship(self, name, reqDef, rel):
+        # this is called in NodeTemplate.relationships by the outer node template
+        self._outer_relationships.setdefault(name, []).append((name, reqDef, rel))
+
+    def _update_requirements(self, node):
+        # traceback.print_stack()
+        # this is called in NodeTemplate.relationships by the inner node template
+        names = []
+        if node is self._node_template:
+            for rels in self._outer_relationships.values():
+                for name, reqDef, rel in rels:
+                    names.append(name)
+                    node._relationships.append((rel, {name: reqDef}, reqDef))
+        return names
+
+    def _map(self, mapping, dest):
+        inputs = self.topology.parsed_params or {}
         for propname, value in mapping.items():
             # map property from input
+            if isinstance(value, dict):
+                if "mapping" not in value:
+                    ExceptionCollector.appendException(
+                        UnknownFieldError(what="SubstitutionMappings", field=value)
+                    )
+                    continue
+                value = value["mapping"]
             if isinstance(value, list):
                 input = value[0]
             else:
                 input = value
-            dest[propname] = source[input]
+            if input in inputs:
+                dest[propname] = inputs[input]
+            elif input in self.inputs:
+                dest[propname] = self.inputs[input].default
+            else:
+                ExceptionCollector.appendException(
+                    MissingRequiredInputError(
+                        what=_("SubstitutionMappings with node_type ")
+                        + self.node_type.type,
+                        input_name=input,
+                    )
+                )
 
     def _validate(self):
         # Basic validation
         self._validate_keys()
         if not self._validate_type():
             return
 
-        # SubstitutionMapping class syntax validation
-        # XXX self._validate_inputs()
-        self._validate_capabilities()
-        self._validate_requirements()
-        self._validate_properties()
-        self._validate_outputs()
+        if self.node:
+            for key in [self.PROPERTIES, self.REQUIREMENTS, self.CAPABILITIES]:
+                if key in self.sub_mapping_def:
+                    ExceptionCollector.appendException(
+                        ValidationError(
+                            message=_(
+                                "substitution_mappings with explicit node declaration can not have a %s mapping declared"
+                            )
+                            % key
+                        )
+                    )
+        if self.substitution_filter:
+            NodeTemplate.validate_filter(
+                self.substitution_filter, "substitution_filter"
+            )
 
     def _validate_keys(self):
         """validate the keys of substitution mappings."""
         for key in self.sub_mapping_def.keys():
             if key not in self.SECTIONS:
                 ExceptionCollector.appendException(
-                    UnknownFieldError(what=_('SubstitutionMappings'),
-                                      field=key))
+                    UnknownFieldError(what=_("SubstitutionMappings"), field=key)
+                )
 
     def _validate_type(self):
         """validate the node_type of substitution mappings."""
         if self.node:
             node = self.topology.node_templates.get(self.node)
             if not node:
                 ExceptionCollector.appendException(
-                  ValidationError(message=_('Unknown node "%s" declared on substitution_mappings') % self.node)
+                    ValidationError(
+                        message=_('Unknown node "%s" declared on substitution_mappings')
+                        % self.node
+                    )
                 )
-            else:
-                self.node_definition = node.type_definition
-            return
-
-        node_type = self.sub_mapping_def.get(self.NODE_TYPE)
-        if not node_type:
-            ExceptionCollector.appendException(
-                MissingRequiredFieldError(
-                    what=_('SubstitutionMappings used in topology_template'),
-                    required=self.NODE_TYPE))
-            return False
-
-        node_type_def = self.custom_defs.get(node_type)
-        if not node_type_def:
-            ExceptionCollector.appendException(
-                InvalidNodeTypeError(what=node_type))
-            return False
-        self.node_definition = NodeType(self.node_type, self.custom_defs)
-        return True
-
-
-    def _validate_inputs(self):
-        """validate the inputs of substitution mappings.
-
-        The inputs defined by the topology template have to match the
-        properties of the node type or the substituted node. If there are
-        more inputs than the substituted node has properties, default values
-        must be defined for those inputs.
-        """
-        # reverse property name to input name mapping
-        reverse_property_mappings = {v : n for n,v in self.sub_mapping_def.get(self.PROPERTIES, {}).items()}
-        all_inputs = set([reverse_property_mappings.get(input, input) for input in self.inputs])
-        required_properties = set([p.name for p in
-                                   self.node_definition.
-                                   get_properties_def_objects()
-                                   if p.required and p.default is None])
-        # Must provide inputs for required properties of node type.
-        for property in required_properties:
-            # Check property which is 'required' and has no 'default' value
-            if property not in all_inputs:
-                ExceptionCollector.appendException(
-                    MissingRequiredInputError(
-                        what=_('SubstitutionMappings with node_type ')
-                        + self.node_type,
-                        input_name=property))
-
-        # If the optional properties of node type need to be customized by
-        # substituted node, it also is necessary to define inputs for them,
-        # otherwise they are not mandatory to be defined.
-        customized_parameters = set(self.sub_mapped_node_template
-                                    .get_properties().keys()
-                                    if self.sub_mapped_node_template else [])
-        all_properties = set(self.node_definition.get_properties_def())
-        for parameter in customized_parameters - all_inputs:
-            if parameter in all_properties:
-                ExceptionCollector.appendException(
-                    MissingRequiredInputError(
-                        what=_('SubstitutionMappings with node_type ')
-                        + self.node_type,
-                        input_name=parameter))
-
-        # Additional inputs are not in the properties of node type must
-        # provide default values. Currently the scenario may not happen
-        # because of parameters validation in nodetemplate, here is a
-        # guarantee.
-        for input in self.inputs.values():
-            if input.name in all_inputs - all_properties \
-               and input.default is None:
+                return False
+            self._node_template = node
+            self.node_type = node.type_definition
+        else:
+            node_type = self.sub_mapping_def.get(self.NODE_TYPE)
+            if not node_type:
                 ExceptionCollector.appendException(
-                    MissingDefaultValueError(
-                        what=_('SubstitutionMappings with node_type ')
-                        + self.node_type,
-                        input_name=input.name))
-
-    def _validate_capabilities(self):
-        """validate the capabilities of substitution mappings."""
-
-        # The capabilites must be in node template which be mapped.
-        tpls_capabilities = self.sub_mapping_def.get(self.CAPABILITIES)
-        node_capabilities = self.sub_mapped_node_template.get_capabilities() \
-            if self.sub_mapped_node_template else None
-        for cap in node_capabilities.keys() if node_capabilities else []:
-            if (tpls_capabilities and
-                    cap not in list(tpls_capabilities.keys())):
-                pass
-                # ExceptionCollector.appendException(
-                #    UnknownFieldError(what='SubstitutionMappings',
-                #                      field=cap))
-
-    def _validate_requirements(self):
-        """validate the requirements of substitution mappings."""
-
-        # The requirements must be in node template wchich be mapped.
-        tpls_requirements = self.sub_mapping_def.get(self.REQUIREMENTS)
-        node_requirements = self.sub_mapped_node_template.requirements \
-            if self.sub_mapped_node_template else None
-        for req in node_requirements if node_requirements else []:
-            if (tpls_requirements and
-                    req not in list(tpls_requirements.keys())):
-                pass
-                # ExceptionCollector.appendException(
-                #    UnknownFieldError(what='SubstitutionMappings',
-                #                      field=req))
-
-    def _validate_properties(self):
-        """validate the properties of substitution mappings."""
-        # The properties in the substitution_mappings must be present
-        # in the node template properties.
-        tpls_properties = self.sub_mapping_def.get(self.PROPERTIES)
-        node_properties = \
-            self.sub_mapped_node_template.get_properties_objects() \
-            if self.sub_mapped_node_template else None
-        for req in node_properties if node_properties else []:
-            if (tpls_properties and
-                    req not in list(tpls_properties.keys())):
-                pass
-                # ExceptionCollector.appendException(
-                #    UnknownFieldError(what='SubstitutionMappings',
-                #                      field=req))
+                    MissingRequiredFieldError(
+                        what=_("SubstitutionMappings used in topology_template"),
+                        required=self.NODE_TYPE,
+                    )
+                )
+                return False
+            node_type_def = self.topology.custom_defs.get(node_type)
+            if not node_type_def:
+                ExceptionCollector.appendException(InvalidNodeTypeError(what=node_type))
+                return False
+            self.node_type = NodeType(node_type, self.topology.custom_defs)
+        return True
 
     def _validate_outputs(self):
         """validate the outputs of substitution mappings.
 
         The outputs defined by the topology template have to match the
         attributes of the node type or the substituted node template,
         and the observable attributes of the substituted node template
@@ -256,13 +302,15 @@
         """
 
         # The outputs defined by the topology template have to match the
         # attributes of the node type according to the specification, but
         # it's reasonable that there are more inputs than the node type
         # has properties, the specification will be amended?
         for output in self.outputs:
-            if output.name not in self.node_definition.get_attributes_def():
+            if output.name not in self.node_type.get_attributes_def():
                 ExceptionCollector.appendException(
                     UnknownOutputError(
-                        where=_('SubstitutionMappings with node_type ')
-                        + self.node_type,
-                        output_name=output.name))
+                        where=_("SubstitutionMappings with node_type ")
+                        + self.node_type.type,
+                        output_name=output.name,
+                    )
+                )
```

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/topology_template.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/topology_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,35 +44,40 @@
     processIntrinsicFunctions = False
 
     '''Load the template data.'''
     def __init__(self, template, custom_defs,
                  parsed_params=None,
                  tosca_template=None):
         self.tpl = template
-        self.sub_mapped_node_template = None
         self.tosca_template = tosca_template
         if self.tpl:
             self.custom_defs = custom_defs or {}
             self.parsed_params = parsed_params
             self._validate_field()
             self.description = self._tpl_description()
             self.inputs = self._inputs()
             self.relationship_templates = self._relationship_templates()
             self.node_templates = self._nodetemplates()
             self.outputs = self._outputs()
             self.groups = self._groups()
             self.policies = self._policies()
             self.workflows = self._workflows()
             if not exception.ExceptionCollector.exceptionsCaught():
-              if self.processIntrinsicFunctions:
-                self._process_intrinsic_functions()
-              else:
-                self._validate_intrinsic_functions()
+                if self.processIntrinsicFunctions:
+                    self._process_intrinsic_functions()
+                else:
+                    self._validate_intrinsic_functions()
+
+            self.substitution_mappings = None
+            tpl_substitution_mapping = self._tpl_substitution_mappings()
+            if tpl_substitution_mapping:
+                self.substitution_mappings = SubstitutionMappings(tpl_substitution_mapping, self)
 
-            self.substitution_mappings = self._substitution_mappings()
+    def copy(self):
+        return TopologyTemplate(self.tpl, self.custom_defs, self.parsed_params, self.tosca_template)
 
     def _inputs(self):
         inputs = []
         parsed_params = self.parsed_params or {}
         for name, attrs in self._tpl_inputs().items():
             input = Input(name, attrs)
             if name in parsed_params:
@@ -111,29 +116,32 @@
                 #     (tpl.type in tpl.type_definition.TOSCA_DEF or
                 #      (tpl.type not in tpl.type_definition.TOSCA_DEF and
                 #       bool(tpl.custom_def)))):
                 tpl.validate(self)
                 nodetemplates[name] = tpl
         return nodetemplates
 
-    def add_template(self, name, tpl):
+    def add_template(self, name, tpl, get_relationships=True):
         # if name in self.node_templates:
         #     exception.ExceptionCollector.appendException(
         #           exception.ValidationError(message=
         #               'Node template already defined "%s"' % name))
         #     return None
 
         self.tpl.setdefault(NODE_TEMPLATES, {})[name] = tpl
         node = NodeTemplate(
             name,
             self,
             self.custom_defs,
             self.relationship_templates)
         node.validate(self)
-        node.relationships # this will update the relationship_tpl of the target node
+        if get_relationships:
+            # this will update the relationship_tpl of the target node
+            # call after topology is complete
+            node.relationships
         self.node_templates[name] = node
         return node
 
     def _relationship_templates(self):
         rel_templates = []
         tpls = self._tpl_relationship_templates()
         for name in tpls:
@@ -147,22 +155,34 @@
             output = Output(name, attrs)
             output.validate()
             outputs.append(output)
         return outputs
 
     def _substitution_mappings(self):
         tpl_substitution_mapping = self._tpl_substitution_mappings()
-        # if tpl_substitution_mapping and self.sub_mapped_node_template:
         if tpl_substitution_mapping:
-            return SubstitutionMappings(tpl_substitution_mapping,
-                                        self,
-                                        self.inputs,
-                                        self.outputs,
-                                        self.sub_mapped_node_template,
-                                        self.custom_defs)
+            return SubstitutionMappings(tpl_substitution_mapping, self)
+
+    def _do_substitutions(self, nested_topologies):
+        # if a node template should be substituted, set its substitution
+        remaining_topologies = [t for t in nested_topologies if t is not self]
+        for nodetemplate in self.nodetemplates:
+            if "substitute" not in nodetemplate.directives:
+                continue
+            for topology in remaining_topologies:
+                mappings = topology.substitution_mappings
+                if mappings.match(nodetemplate):
+                    # the node template's properties treated as inputs
+                    # create a new substitution mapping object for the mapped node
+                    nodetemplate.substitution = mappings.substitute(nodetemplate, remaining_topologies)
+                    break
+            else:
+                exception.ExceptionCollector.appendException(
+                      exception.ValidationError(message=
+                          'No substitute topology found for "%s"' % nodetemplate.name))
 
     def _policies(self):
         policies = []
         for policy in self._tpl_policies():
             for policy_name, policy_tpl in policy.items():
                 target_list = policy_tpl.get('targets')
                 target_objects = []
@@ -408,14 +428,15 @@
                                     self,
                                     node_template,
                                     prop.value)
 
         for output in self.outputs:
             ExceptionCollector.near = f' in output "{output.name}"'
             functions.get_function(self, self.outputs, output.value)
+        ExceptionCollector.near = ""
 
     def validate_relationships(self, strict):
         if not hasattr(self, 'nodetemplates'):
             return
         for node_template in self.nodetemplates:
             ExceptionCollector.near = f' in node template "{node_template.name}"'
             for rel_tpl, req, reqDef in node_template.relationships:
@@ -424,12 +445,15 @@
                     functions.get_function(self, req, prop.value)
                 for interface in rel_tpl.interfaces:
                     if interface.inputs:
                         for name, value in interface.inputs.items():
                             functions.get_function(self,
                                                    rel_tpl,
                                                    value)
-            if strict:
+
+            if node_template.substitution:
+                node_template.substitution.topology.validate_relationships(strict)
+            elif strict:
                 for name in node_template.missing_requirements:
                     msg = f'Required requirement "{name}" not defined'
                     ExceptionCollector.appendException(
                         ValidationError(message = msg))
```

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/tosca_template.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/tosca_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,14 +92,15 @@
             self.tpl = yaml_dict_tpl
 
         if not path and not yaml_dict_tpl:
             ExceptionCollector.appendException(
                 ValueError(_('No path or yaml_dict_tpl was provided. '
                              'There is nothing to parse.')))
 
+        self.topology_template = None
         if self.tpl:
             self.parsed_params = parsed_params
             self._validate_field()
             self.version = self._tpl_version()
             EntityType.reset_caches()
             self.description = self._tpl_description()
             custom_defs = self._get_all_custom_defs()
@@ -223,43 +224,27 @@
         # nested_tosca_tpls is list of {file_path : tpl} of the imported templates
         nested_tosca_tpls = imports_loader.get_nested_tosca_tpls()
         # custom defs are merged together (with possibly namespace prefix)
         custom_defs = imports_loader.get_custom_defs()
         return custom_defs, nested_tosca_tpls
 
     def _handle_nested_tosca_templates_with_topology(self, custom_types):
+        ExceptionCollector.near = ""
         for filename, tosca_tpl in self.nested_tosca_tpls.items():
             topology_tpl = tosca_tpl.get(TOPOLOGY_TEMPLATE)
             if topology_tpl:
                 custom_types = custom_types.copy()
-                custom_types.update(tosca_tpl.get('node_types', {})) # XXX isn't this redundant?
+                custom_types.update(tosca_tpl.get('node_types', {}))  # XXX isn't this redundant?
                 self.nested_topologies[filename] = TopologyTemplate(
                                 topology_tpl, custom_types, None, self)
-
-        # if a nodetemplate should be substituted, set its sub_mapping_tosca_template
-        for nodetemplate in self.nodetemplates:
-            if "substitute" not in nodetemplate.directives:
-                continue
-            for topology in self.nested_topologies.values():
-                if not topology.substitution_mappings:
-                    continue
-                if topology.substitution_mappings.type == nodetemplate.type:
-                    # the node template's properties treated as inputs
-                    inputs = self._get_params_for_nested_template(nodetemplate)
-                    # create a new substitution mapping object for the mapped node
-                    # XXX SubstitutionMappings is just a simple wrapper around the def dict, only performs validation
-                    # and sub_mapping_tosca_template is never unused!
-                    nodetemplate.sub_mapping_tosca_template = SubstitutionMappings(
-                        topology.substitution_mappings.sub_mapping_def,
-                        topology,
-                        inputs,
-                        topology.outputs,
-                        nodetemplate,
-                        topology.custom_defs)
-                    break
+        substitutable_topologies = [t for t in self.nested_topologies.values() if t.substitution_mappings]
+        self.topology_template._do_substitutions(substitutable_topologies)
+        if self.topology_template.substitution_mappings and not self.topology_template.substitution_mappings.node:
+            # create a node template for the root topology's substitution mapping
+            self.topology_template.substitution_mappings.substitute(None, None)
 
     def _validate_field(self):
         version = self._tpl_version()
         if not version:
             ExceptionCollector.appendException(
                 MissingRequiredFieldError(what='Template',
                                           required=DEFINITION_VERSION))
@@ -315,34 +300,7 @@
             if self.input_path:
                 msg = (_('The input "%(path)s" successfully passed '
                          'validation.') % {'path': self.input_path})
             else:
                 msg = _('The pre-parsed input successfully passed validation.')
 
             log.info(msg)
-
-    def _is_sub_mapped_node(self, nodetemplate, tosca_tpl):
-        """Return True if the nodetemple is substituted."""
-        # NOTE(ueha): Since condition "not nodetemplate.sub_mapping_tosca_\
-        #             template" was deleted as a fix for bug/1883220, there is
-        #             some possibility of breaking something on translator side
-        #             that current tests not coverd.
-        #             And this enhancement does not align with TOSCA standard
-        #             but needed for ETSI NFV-SOL 001.
-        if (nodetemplate and
-                self.get_sub_mapping_node_type(tosca_tpl) == nodetemplate.type
-                and len(nodetemplate.interfaces) < 1):
-            return True
-        else:
-            return False
-
-    def _get_params_for_nested_template(self, nodetemplate):
-        """Return total params for nested_template."""
-        parsed_params = {input.name : input for input in self.topology_template.inputs}
-        if nodetemplate:
-            parsed_params.update(nodetemplate.get_properties())
-        return list(parsed_params.values())
-
-    def _has_substitution_mappings(self):
-        """Return True if the template has valid substitution mappings."""
-        return self.topology_template is not None and \
-            self.topology_template.substitution_mappings is not None
```

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/tpl_relationship_graph.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/tpl_relationship_graph.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/triggers.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/triggers.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/unsupportedtype.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/unsupportedtype.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/utils/gettextutils.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/utils/gettextutils.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/utils/urlutils.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/utils/urlutils.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/utils/validateutils.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/utils/validateutils.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/utils/yamlparser.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/utils/yamlparser.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/vendor/toscaparser/workflow.py` & `unfurl-0.7.0/unfurl/vendor/toscaparser/workflow.py`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl/yamlloader.py` & `unfurl-0.7.0/unfurl/yamlloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 from .merge import (
     expand_doc,
     make_map_with_base,
     find_anchor,
     _cache_anchors,
     restore_includes,
 )
-from .repo import RepoView, GitRepo, is_url_or_git_path, split_git_url
+from .repo import Repo, RepoView, GitRepo, is_url_or_git_path, split_git_url
 from .packages import UnfurlPackageUpdateNeeded, resolve_package
 from .logs import getLogger
 from toscaparser.common.exception import URLException, ExceptionCollector
 from toscaparser.utils.gettextutils import _
 import toscaparser.imports
 from toscaparser.repositories import Repository
 
@@ -89,16 +89,23 @@
 
 
 def _use_clear_text(vault):
     clear_id = CLEARTEXT_VAULT.secrets[0][0]
     return vault.secrets and all(s[0] == clear_id for s in vault.secrets)
 
 
-def represent_undefined(self, data):
-    raise RepresenterError(f"cannot represent an object: <{data}> of type {type(data)}")
+from jinja2.runtime import DebugUndefined
+
+
+def represent_undefined(dumper, data):
+    msg = f"cannot represent an object: <{data}> of type {type(data)}"
+    if isinstance(data, DebugUndefined):
+        return dumper.represent_scalar("tag:yaml.org,2002:str", repr(msg))
+    else:
+        raise RepresenterError(msg)
 
 
 def _represent_sensitive(dumper, data, tag):
     if dumper.vault.secrets:
         b_ciphertext = dumper.vault.encrypt(data)
         return dumper.represent_scalar(tag, b_ciphertext.decode(), style="|")
     else:
@@ -239,14 +246,17 @@
 
 _refResolver = RefResolver("", None)
 
 GetURLType = Optional[Tuple[str, bool, Optional[str]]]
 
 
 class ImportResolver(toscaparser.imports.ImportResolver):
+    # get_repository() is called by the tosca template
+    # load_yaml() called by the ImportsLoader with the resolved path or url returned by resolve_file_reference()
+
     def __init__(
         self, manifest: "Manifest", ignoreFileNotFound=False, expand=False, config=None
     ):
         self.manifest = manifest
         self.readonly = bool(manifest.localEnv and manifest.localEnv.readonly)
         self.ignoreFileNotFound = ignoreFileNotFound
         self.yamlloader = manifest.loader
@@ -255,42 +265,47 @@
         self.repo_refs: Dict[str, GitRepo] = {}
 
     def __getstate__(self):
         state = self.__dict__.copy()
         state["yamlloader"] = None
         return state
 
-    def set_cache(self, url, val):
-        self.manifest.cache[url] = val
-
-    def get_cache(self, url):
-        return self.manifest.cache.get(url)
-
-    def load_imports(self, importsLoader, importslist):
+    def load_imports(
+        self,
+        importsLoader: toscaparser.imports.ImportsLoader,
+        importslist: List[Union[str, Dict]],
+    ):
         while True:
             try:
                 return super().load_imports(importsLoader, importslist)
             except UnfurlPackageUpdateNeeded:
                 pass  # reload
 
-    def get_repository(self, name: str, tpl: dict) -> Repository:
-        # don't create another Repository instance
-        if name in self.manifest.repositories:
-            return self.manifest.repositories[name].repository
+    def get_repository(self, name: str, tpl: dict, unique=False) -> Repository:
+        counter = 1
+        basename = name
+        while name in self.manifest.repositories:
+            if unique:
+                # create Repository instance with a unique name
+                name = basename + str(counter)
+                counter += 1
+            else:
+                # don't create another Repository instance
+                return self.manifest.repositories[name].repository
 
         if isinstance(tpl, dict) and "url" in tpl:
             url = tpl["url"]
             if (
                 "://" not in url and "@" in url
             ):  # scp style used by git: user@server:project.git
                 # convert to ssh://user@server/project.git
                 url = "ssh://" + url.replace(":", "/", 1)
             tpl["url"] = url
 
-        if tpl.get("credential"):
+        if tpl.get("credential") and not self.manifest.safe_mode:
             credential = tpl["credential"]
             # support expressions to resolve credential secrets
             if self.manifest.rootResource:
                 from .eval import map_value
 
                 tpl["credential"] = map_value(credential, self.manifest.rootResource)
             elif self.manifest.localEnv:
@@ -300,205 +315,321 @@
                 )
                 tpl["credential"] = self.manifest.localEnv.map_value(
                     credential, context.get("variables")
                 )
 
         return Repository(name, tpl)
 
-    def _get_bare_path(self, path, repo, filePath, revision, file_name, importsLoader):
-        # # XXX support empty filePath or when filePath is a directory -- need to checkout the tree
-        if not filePath:
-            raise UnfurlError(
-                f"local repository for '{path}' can not checkout revision '{revision}'"
-            )
-        elif repo.repo.rev_parse(revision + ":" + filePath).type != "blob":
-            raise UnfurlError(
-                f"can't retrieve '{filePath}' with revision '{revision}' from local repository for '{path}'"
-            )
-        url = "git-ref:" + repo.url
-        self.repo_refs[url] = repo
-        return f"{url}#{revision}:{filePath}"
+    confine_user_paths = True
 
-    def _get_repository_path(
-        self, importsLoader: toscaparser.imports.ImportsLoader, repository_name: str
-    ) -> Tuple[str, bool, Optional["RepoView"]]:
-        path = cast(str, self.get_repository_url(importsLoader, repository_name))
-        if path.startswith("file:"):
-            path = path[5:]
-            if path.startswith("//"):
-                path = path[2:]
-            return path, True, None
+    def _has_path_escaped(self, path, repository_name=None):
+        if not self.confine_user_paths:
+            return False
+        if repository_name:
+            if path.startswith("..") or os.path.isabs(path):
+                msg = f'Path not allowed outside of repository {repository_name}: "{path}"'
+                ExceptionCollector.appendException(ImportError(msg))
+                return True
+            else:
+                return False
+
+        # user supplied path can't be outside of the project or the home project
+        if self.manifest.localEnv and self.manifest.localEnv.project:
+            if os.path.abspath(path).startswith(
+                os.path.abspath(os.path.dirname(__file__))
+            ):
+                # special case for built-in "unfurl" repository
+                return False
+            if self.manifest.localEnv.project.get_relative_path(path).startswith(".."):
+                if (
+                    not self.manifest.localEnv.homeProject
+                    or self.manifest.localEnv.homeProject.get_relative_path(
+                        path
+                    ).startswith("..")
+                ):
+                    msg = f'Path "{os.path.abspath(path)}" not allowed outside of project: "{self.manifest.localEnv.project.projectRoot}"'
+                    ExceptionCollector.appendException(ImportError(msg))
+                    return True
+        return False
+
+    def _find_repoview(self, url: str) -> RepoView:
+        # if create, creates a new one
+        repo_view = None
+        git_url, path, revision = split_git_url(url)  # we only support git urls
+        assert self.manifest.localEnv
+        repoview_or_url = self.manifest.localEnv._find_git_repo(git_url, revision)
+        if isinstance(repoview_or_url, RepoView):
+            repo_view = repoview_or_url
         else:
-            repoview = self.manifest.repositories.get(repository_name)
-            if not repoview:
-                repository = self.get_repository(
-                    repository_name, importsLoader.repositories[repository_name]
-                )
-                repoview = self.manifest.add_repository(None, repository, "")
-            assert repoview
-            if repoview.package is None:
-                # need to resolve if its a package
-                # if repoview.repository references a package, set the repository's url
-                # and register this reference with the package
-                # might raise error if version conflict
-                resolve_package(
-                    repoview, self.manifest.packages, self.manifest.package_specs
-                )
-            return repoview.url, False, repoview
+            # repo wasn't not found, repoview_or_url is the git_url (with credentials possibly applied)
+            # create new RepoView for this url
+            name = Repo.get_path_for_git_repo(repoview_or_url, name_only=True)
+            repository = self.get_repository(name, dict(url=repoview_or_url), True)
+            repo_view = RepoView(repository, None)
+        return repo_view
 
-    def get_url(
+    def _resolve_repo_to_path(
         self,
-        importsLoader: toscaparser.imports.ImportsLoader,
-        repository_name: Optional[str],
+        repo_view: RepoView,
+        base: str,
         file_name: str,
-        isFile: Optional[bool] = None,
-    ) -> GetURLType:
-        # called by ImportsLoader when including or importing a file
-        # or resolving path to an artifact in a repository (see ToscaSpec.get_repository_path)
-        # returns url or path, isFile, fragment
-        fragment: Optional[str] = None
-        repo_view = None
-        if repository_name:
-            file_name, sep, fragment = file_name.partition("#")
-            path, isFile, repo_view = self._get_repository_path(
-                importsLoader, repository_name
+    ) -> str:
+        commit = repo_view.package.lock_to_commit if repo_view.package else ""
+        if not repo_view.repo:
+            repo, file_path, revision, bare = self.manifest.find_repo_from_git_url(
+                repo_view.as_git_url(), base
             )
-            # if not isFile path will be git url possibly including revision in fragment
-            if repo_view and repo_view.repo:
-                repo_view.add_file_ref(file_name)
-                return os.path.join(repo_view.working_dir, file_name), True, fragment
+            if repo:
+                repo_view.repo = repo
+            else:
+                raise UnfurlError(
+                    "Could not resolve git URL: " + repo_view.as_git_url(True)
+                )
         else:
-            url_info = cast(
-                GetURLType, super().get_url(importsLoader, None, file_name, isFile)
+            repo = repo_view.repo
+            file_path = repo_view.path
+            revision = repo.revision
+            bare = False  # XXX if commit
+
+        if bare:
+            path = self._get_bare_path(repo, file_path, revision)
+        else:
+            path = os.path.join(repo.working_dir, file_path, file_name or "").rstrip(
+                "/"
             )
-            if not url_info:
-                return url_info
-            path, isFile, fragment = url_info
-            file_name = ""  # was included in path
-
-        if not isFile or is_url_or_git_path(path):
-            # only support urls to git repos for now
-            # this may clone a remote git repo
-            repo, filePath, revision, bare = self.manifest.find_repo_from_git_url(
-                path, isFile, importsLoader
+        return path
+
+    def resolve_url(self, importsLoader, base, file_name, repository_name):
+        if repository_name:
+            if self._has_path_escaped(file_name, repository_name):
+                # can't be ".." or absolute path
+                return None, None
+            repo_view = self.manifest.repositories.get(repository_name)
+            if not repo_view:
+                repository = self.get_repository(
+                    repository_name, importsLoader.repositories[repository_name]
+                )
+                repo_view = self.manifest.add_repository(None, repository, "")
+        else:
+            # if file_name is relative, base will be set (to the importsLoader's path)
+            url = os.path.join(base, file_name)
+            if not toscaparser.imports.is_url(url):
+                # url is a local path
+                if self._has_path_escaped(url):
+                    return None, None
+                return url, (True, None, base, file_name)
+            repo_view = self._find_repoview(url)
+            assert repo_view
+
+        assert repo_view
+        if repo_view.package is None:
+            # need to resolve if its a package
+            # if repoview.repository references a package, set the repository's url
+            # and register this reference with the package
+            # might raise error if version conflict
+            resolve_package(
+                repo_view, self.manifest.packages, self.manifest.package_specs
             )
-            if not repo:
-                raise UnfurlError("Could not resolve git URL: " + path)
-            if bare:
-                path = self._get_bare_path(
-                    path, repo, filePath, revision, file_name, importsLoader
-                )
-                return path, False, fragment
-            else:
-                if repo_view:
-                    assert not repo_view.repo
-                    repo_view.set_repo_and_path(repo, filePath)
-                    repo_view.add_file_ref(file_name)
-                path = os.path.join(repo.working_dir, filePath, file_name or "").rstrip(
-                    "/"
+        repo_view.add_file_ref(file_name)
+        path = toscaparser.imports.normalize_path(repo_view.url)
+        is_file = not toscaparser.imports.is_url(path)
+        if is_file:
+            # repository is a local path
+            # so use the resolved base
+            path = os.path.join(base, file_name)
+            if self._has_path_escaped(path):
+                return None, None
+        return path, (is_file, repo_view, base, file_name)
+
+    def resolve_to_local_path(self, base_dir, file_name, repository_name):
+        if repository_name:
+            rv = self.manifest.repositories.get(repository_name)
+            if rv:
+                repository_tpl = rv.repository.tpl
+                repositories = {repository_name: repository_tpl}
+            else:
+                repositories = (
+                    self.manifest.tosca
+                    and self.manifest.tosca.template.tpl.get("repositories")
+                    or {}
                 )
-        elif file_name:
-            path = os.path.join(path, file_name)
+        else:
+            repositories = {}
+        loader = toscaparser.imports.ImportsLoader(
+            None, base_dir, repositories=repositories, resolver=self
+        )
+        tpl = dict(file=file_name, repository=repository_name)
+        url_info = loader.resolve_import(tpl)
+        if url_info:
+            url, fragment, ctx = url_info
+            is_file, repo_view, base, file_name = ctx
+            if is_file:
+                # already a path
+                return url, fragment
+            else:
+                # clone git repository if necessary
+                return self._resolve_repo_to_path(repo_view, base, file_name), fragment
+        return None, None
 
-        # always a local file path at this point
-        return path, True, fragment
+    def _get_bare_path(self, repo, filePath, revision):
+        # # XXX support empty filePath or when filePath is a directory -- need to checkout the tree
+        path = repo.working_dir
+        if not filePath:
+            raise UnfurlError(
+                f"local repository for '{path}' can not checkout revision '{revision}'"
+            )
+        elif repo.repo.rev_parse(revision + ":" + filePath).type != "blob":
+            raise UnfurlError(
+                f"can't retrieve '{filePath}' with revision '{revision}' from local repository for '{path}'"
+            )
+        url = "git-ref:" + repo.url
+        # self.repo_refs[url] = repo
+        return f"{url}#{revision}:{filePath}"
 
-    def _open(self, path: str, isFile: bool) -> Optional[TextIO]:
+    def _open(self, path: str, isFile: bool) -> Tuple[Optional[TextIO], bool]:
+        ok_to_show = True
         if path.startswith("git-ref:"):
-            url, filePath, revision = split_git_url(path)
-            return io.StringIO(self.repo_refs[url].show(filePath, revision))
+            # XXX we need both the commit and revision if we don't have the full git repo
+            url, filePath, revision = split_git_url(path[len("git-ref:") :])
+            repo_view = self._find_repoview(url)
+            if not repo_view.repo:
+                raise UnfurlError("Could not resolve " + path)
+            bdata = repo_view.repo.show(filePath, revision, stdout_as_string=False)
+            if self.yamlloader:
+                # ok_to_show if bdata was cleartext otherwise it was encrypted
+                bdata, ok_to_show = self.yamlloader._decrypt_if_vault_data(
+                    bdata, filePath
+                )
+            return io.StringIO(codecs.decode(bdata)), ok_to_show
         else:
             try:
                 if isFile:
                     ignoreFileNotFound = self.ignoreFileNotFound
                     if ignoreFileNotFound and not os.path.isfile(path):
-                        return None
+                        return None, ok_to_show
 
                     if self.yamlloader:
-                        # show == True if file was decrypted
-                        contents, show = self.yamlloader._get_file_contents(path)
+                        # ok_to_show if contents was cleartext otherwise it was encrypted
+                        contents, ok_to_show = self.yamlloader._get_file_contents(path)
                         f: TextIO = io.StringIO(codecs.decode(contents))
                     else:
                         f = codecs.open(path, encoding="utf-8", errors="strict")
                 else:
                     f = urlopen(path)
-                return f
+                return f, ok_to_show
             except urllib.error.URLError as e:
                 if hasattr(e, "reason"):
                     msg = _(
                         (
                             'Failed to reach server "%(path)s". Reason is: '
                             + "%(reason)s."
                         )
                     ) % {"path": path, "reason": e.reason}
                     ExceptionCollector.appendException(URLException(what=msg))
-                    return None
+                    return None, ok_to_show
                 elif hasattr(e, "code"):
                     msg = _(
                         (
                             'The server "%(path)s" couldn\'t fulfill the request. '
                             + 'Error code: "%(code)s".'
                         )
                     ) % {
                         "path": path,
                         "code": e.code,  # type: ignore
                     }
                     ExceptionCollector.appendException(URLException(what=msg))
-                    return None
+                    return None, ok_to_show
                 else:
                     raise
 
     def load_yaml(
         self,
-        importsLoader: toscaparser.imports.ImportsLoader,
+        importsLoader: Any,
+        path: str,
+        fragment: Optional[str],
+        ctx,
+    ) -> Tuple[Any, Any]:
+        is_file, repo_view, base, file_name = ctx
+        if not is_file:
+            # clone git repository if necessary
+            path = self._resolve_repo_to_path(repo_view, base, file_name)
+            is_file = True
+        return self._really_load_yaml(path, is_file, fragment)
+
+    def _really_load_yaml(
+        self,
         path: str,
-        isFile=True,
-        fragment=None,
-    ) -> Any:
+        isFile: bool,
+        fragment: Optional[str],
+    ) -> Tuple[Any, bool]:
+        originalPath = path
         try:
             logger.trace(
                 "attempting to load YAML %s: %s", "file" if isFile else "url", path
             )
-            originalPath = path
-            doc = self.get_cache(path)
-            if doc is not None:
-                if fragment and doc:
-                    return _refResolver.resolve_fragment(doc, fragment)
-                else:
-                    return doc
-
-            f = self._open(path, isFile)
+            f, cacheable = self._open(path, isFile)
             if f is None:
-                return None
+                return None, cacheable
 
             with f:
                 contents = f.read()
                 doc = load_yaml(yaml, contents, path, self.readonly)
                 yaml_dict = yaml_dict_type(self.readonly)
                 if isinstance(doc, yaml_dict):
                     if self.expand:
                         includes, doc = expand_doc(
                             doc,
                             cls=make_map_with_base(doc, get_base_dir(path), yaml_dict),
                         )
                         doc.includes = includes
                     doc.path = path
-            self.set_cache(path, doc)
             if fragment and doc:
-                return _refResolver.resolve_fragment(doc, fragment)
+                return _refResolver.resolve_fragment(doc, fragment), cacheable
             else:
-                return doc
+                return doc, cacheable
         except Exception:
             if path != originalPath:
                 msg = f'Could not load "{path}" (originally "{originalPath}")'
             else:
                 msg = f'Could not load "{path}"'
             raise UnfurlError(msg, True)
 
 
+class SimpleCacheResolver(ImportResolver):
+    def set_cache(self, path, val):
+        self.manifest.cache[path] = (val, 0)
+
+    def get_cache(self, doc_key):
+        if doc_key in self.manifest.cache:
+            val, count = self.manifest.cache[doc_key]
+            self.manifest.cache[doc_key] = (val, count + 1)
+            return val
+        return None
+
+    def load_yaml(
+        self,
+        importsLoader: toscaparser.imports.ImportsLoader,
+        path: str,
+        fragment,
+        ctx,
+    ) -> Tuple[Any, Any]:
+        is_file, repo_view, base, file_name = ctx
+        if not is_file:
+            # clone git repository if necessary
+            path = self._resolve_repo_to_path(repo_view, base, file_name)
+        doc = self.get_cache((path, fragment))
+        if doc is None:
+            doc, cacheable = self._really_load_yaml(path, True, fragment)
+            if cacheable:
+                self.set_cache((path, fragment), doc)
+        else:
+            cacheable = True
+        return doc, cacheable
+
+
 class LoadIncludeAction:
     def __init__(self, check_include=False, get_key=None):
         self.get_key = get_key
         self.check_include = check_include
 
 
 class YamlConfig:
@@ -582,15 +713,15 @@
         if url.scheme.startswith("http") and url.netloc:  # looks like an absolute url
             fragment = url.fragment
             logger.trace("attempting to load YAML url: %s", path)
             try:
                 f = urlopen(path)
             except urllib.error.URLError:
                 if warnWhenNotFound:
-                    logger.warning(f"document include {path} could not be retreived")
+                    logger.warning(f"document include {path} could not be retrieved")
                     return path, None
                 raise
         else:
             path, sep, fragment = path.partition("#")
             path = os.path.abspath(os.path.join(baseDir or self.get_base_dir(), path))
             if warnWhenNotFound and not os.path.isfile(path):
                 logger.warning(
@@ -755,27 +886,31 @@
             baseDir = self.baseDirs[-1]
             if self.loadHook:
                 path, template = self.loadHook(
                     self, templatePath, baseDir, warnWhenNotFound, expanded, None
                 )
             else:
                 path, template = self.load_yaml(key, baseDir, warnWhenNotFound)
-
-            if template is None:
-                return value, template, baseDir
-
-            if path.startswith("http"):  # its an url, don't change baseDir
-                newBaseDir = baseDir
-            else:
-                newBaseDir = os.path.dirname(path)
-            if isinstance(template, dict):
-                template.base_dir = newBaseDir  # type: ignore
-            _cache_anchors(self.config._anchorCache, template)
         except Exception:
-            raise UnfurlError(
-                f"unable to load document include: {templatePath} (base: {baseDir})",
-                True,
-            )
+            msg = f"unable to load document include: {templatePath} (base: {baseDir})"
+            if warnWhenNotFound:
+                logger.warning(msg, exc_info=True)
+                template = None  # type: ignore
+            else:
+                raise UnfurlError(
+                    msg,
+                    True,
+                )
+        if template is None:
+            return value, template, baseDir
+
+        if path.startswith("http"):  # its an url, don't change baseDir
+            newBaseDir = baseDir
+        else:
+            newBaseDir = os.path.dirname(path)
+        if isinstance(template, dict):
+            template.base_dir = newBaseDir  # type: ignore
+        _cache_anchors(self.config._anchorCache, template)
         self.baseDirs.append(newBaseDir)
 
         self._cachedDocIncludes[key] = (path, template)
         return value, template, newBaseDir
```

### Comparing `unfurl-0.6.2/unfurl/yamlmanifest.py` & `unfurl-0.7.0/unfurl/yamlmanifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from .merge import patch_dict, intersect_dict
 from .yamlloader import YamlConfig, make_yaml
 from .result import serialize_value
 from .support import ResourceChanges, Defaults, Status
 from .localenv import LocalEnv
 from .lock import Lock
 from .manifest import Manifest, relabel_dict, ChangeRecordRecord
-from .tosca import ArtifactSpec, find_env_vars
-from .runtime import TopologyInstance
+from .tosca import ArtifactSpec, NodeSpec, find_env_vars
+from .runtime import EntityInstance, NodeInstance, TopologyInstance
 from .eval import map_value
 from .planrequests import create_instance_from_spec
 from .logs import getLogger
 from ruamel.yaml.comments import CommentedMap
 from codecs import open
 from ansible.parsing.dataloader import DataLoader
 
@@ -101,15 +101,16 @@
         readyState["local"] = operational.local_status.name
     else:
         readyState["effective"] = operational.status.name
     if operational.state is not None:
         readyState["state"] = operational.state.name
     if operational.priority is not None:
         status["priority"] = operational.priority.name
-    status["readyState"] = readyState
+    if not status.get("imported"):
+        status["readyState"] = readyState
 
     if operational.last_state_change:
         status["lastStateChange"] = operational.last_state_change
     if operational.last_config_change:
         status["lastConfigChange"] = operational.last_config_change
 
     return status
@@ -179,42 +180,48 @@
     """Loads an ensemble from a manifest but doesn't instantiate the instance model."""
 
     def __init__(
         self,
         manifest=None,
         path: Optional[str] = None,
         validate=True,
-        localEnv=None,
+        localEnv: Optional[LocalEnv] = None,
         vault=None,
+        safe_mode: Optional[bool] = None,
     ):
-        path = path or localEnv and localEnv.manifestPath
+        path = path or (localEnv.manifestPath if localEnv else None)
         if path:
             path = os.path.abspath(path)
         super().__init__(path, localEnv)
+        readonly = bool(localEnv and localEnv.readonly)
+        self.safe_mode = bool(safe_mode)
         self.manifest = YamlConfig(
             manifest,
             self.path,
             validate,
             os.path.join(_basepath, "manifest-schema.json"),
             self.load_yaml_include,
             vault,
-            localEnv and localEnv.readonly,
+            readonly,
         )
         if self.manifest.path:
             logger.debug("loaded ensemble manifest at %s", self.manifest.path)
         manifest = self.manifest.expanded
         spec = manifest.get("spec", {})
         self.context = manifest.get("environment", CommentedMap())
         if localEnv:
             self.context = localEnv.get_context(self.context)
         inputs = spec.get("inputs") or {}
         context_inputs = self.context.get("inputs")
         if context_inputs:
             inputs.update(context_inputs)
         spec["inputs"] = inputs
+        lock = manifest.get("lock")
+        if lock:
+            Lock.apply_to_packages(lock, self.package_specs)
         # _update_repositories might not have been called while parsing
         # call it now to make sure we set up the built-in repositories
         self._update_repositories(manifest)
 
     @property
     def uris(self) -> List[str]:
         uris: List[str] = []
@@ -248,14 +255,17 @@
         return self.manifest.get_base_dir()
 
     def is_path_to_self(self, path):
         if self.path is None or path is None:
             return False
         return os.path.abspath(self.path) == os.path.abspath(path)
 
+    def get_saved_outputs(self):
+        return self.manifest.expanded.get("status", {}).get("outputs")
+
     # def addRepo(self, name, repo):
     #     self._getRepositories(self.manifest.config)[name] = repo
 
     def dump(self, out=sys.stdout):
         self.manifest.dump(out)
 
 
@@ -279,20 +289,21 @@
     lockfilepath = None
     lockfile = None
 
     def __init__(
         self,
         manifest=None,
         path=None,
-        validate=True,
+        validate=True,  # json schema validation
         localEnv=None,
         vault=None,
-        skip_validation=False,
+        skip_validation=False,  # tosca parser validation
+        safe_mode: Optional[bool] = None,
     ):
-        super().__init__(manifest, path, validate, localEnv, vault)
+        super().__init__(manifest, path, validate, localEnv, vault, safe_mode)
         self.validate = not skip_validation  # see AttributeManager.validate
         # instantiate the tosca template
         manifest = self.manifest.expanded
         if self.manifest.path:
             self.lockfilepath = self.manifest.path + ".lock"
         spec = manifest.get("spec", {})
         more_spec = self._load_context(self.context, localEnv)
@@ -435,31 +446,34 @@
                 root._environ["PATH"] = (
                     path + os.pathsep + root._environ.get("PATH", "")
                 )
                 logger.debug("PATH set to %s", root._environ["PATH"])
 
     def create_topology_instance(self, status: dict) -> TopologyInstance:
         """
-        If an instance of the toplogy is recorded in status, load it,
+        If an instance of the topology is recorded in status, load it,
         otherwise create a new resource using the the topology as its template
         """
         # XXX use the substitution_mapping (3.8.12) represent the resource
         operational = self.load_status(status)
-        root = TopologyInstance(self.tosca and self.tosca.topology, operational)
-        root.attributeManager = self
+        topology = self.tosca and self.tosca.topology
+        assert topology
+        root = TopologyInstance(topology, operational)
+        root.set_attribute_manager(self)
         if os.environ.get("UNFURL_WORKDIR"):
             root.set_base_dir(os.environ["UNFURL_WORKDIR"])
         elif not self.path:
             root.set_base_dir(root.tmp_dir)
         else:
             root.set_base_dir(self.get_base_dir())
 
         # need to set rootResource before createNodeInstance() is called
         self.rootResource = root
-        self._set_root_environ()
+        if not self.safe_mode:
+            self._set_root_environ()
 
         # self.load_external_ensemble("localhost", tpl) # declared in templates/home/unfurl.yaml.j2
         importsSpec = self.context.get("external", {})
         # note: external "localhost" is defined in UNFURL_HOME's context by convention
         for name, value in importsSpec.items():
             self.load_external_ensemble(name, value)
 
@@ -506,38 +520,44 @@
         if not location:
             raise UnfurlError(
                 f"Can not import external ensemble '{name}': no manifest specified"
             )
 
         if "project" in location:
             importedManifest = self.localEnv and self.localEnv.get_external_manifest(
-                location
+                location, skip_validation=not self.validate, safe_mode=self.safe_mode
             )
             if not importedManifest:
                 raise UnfurlError(
                     f"Can not import external ensemble '{name}': can't find project '{location['project']}'"
                 )
         else:
             # ensemble is in the same project
             baseDir = getattr(location, "base_dir", self.get_base_dir())
             artifact_tpl = dict(file=location["file"])
             if "repository" in location:
                 artifact_tpl = location["repository"]
-            artifact = ArtifactSpec(artifact_tpl, path=baseDir, spec=self.tosca)
+            artifact = ArtifactSpec(
+                artifact_tpl,
+                path=baseDir,
+                topology=self.tosca and self.tosca.topology or None,
+            )
             path = artifact.get_path()
             localEnv = LocalEnv(
                 path,
                 parent=self.localEnv,
                 override_context=location.get("environment", ""),
             )
             if self.is_path_to_self(localEnv.manifestPath):
                 # don't import self (might happen when context is shared)
                 return
             logger.verbose("loading external ensemble at %s", localEnv.manifestPath)
-            importedManifest = localEnv.get_manifest(skip_validation=not self.validate)
+            importedManifest = localEnv.get_manifest(
+                skip_validation=not self.validate, safe_mode=self.safe_mode
+            )
 
         uri = value.get("uri")
         if uri and not importedManifest.has_uri(uri):
             raise UnfurlError(
                 f"Error importing external ensemble at '{path}', uri mismatch for '{uri}'"
             )
         rname = value.get("instance", "root")
@@ -620,15 +640,15 @@
                         operationIndex[key] = change.changeId
             self._operationIndex = operationIndex
         changeId = self._operationIndex.get((target, operation))
         if changeId is not None and self.changeSets:
             return self.changeSets[changeId]
         return None
 
-    def save_entity_instance(self, resource) -> Tuple[str, Dict]:
+    def save_entity_instance(self, resource: EntityInstance) -> Tuple[str, Dict]:
         status = CommentedMap()
         status["template"] = resource.template.get_uri()
 
         # only save the attributes that were set by the instance, not spec properties or attribute defaults
         # particularly, because these will get loaded in later runs and mask any spec properties with the same name
         if resource._attributes:
             status["attributes"] = resource._attributes
@@ -668,31 +688,31 @@
                 and resource.local_status in [Status.unknown, Status.ok, Status.pending]
             )
         ):
             # no reason to serialize entities that haven't been instantiated
             return None
         return self.save_entity_instance(resource)
 
-    def save_resource(self, resource, discovered):
+    def save_resource(self, resource: NodeInstance, discovered):
         # XXX checkstatus break unit tests so skip mostly
         checkstatus = (
             resource.template.type == "unfurl.nodes.LocalRepository"
             or "default" in resource.template.directives
         )
         ret = self._save_entity_if_instantiated(resource, checkstatus)
         if not ret:
             return ret
         name, status = ret
 
         if (
             self.tosca
             and self.tosca.discovered
-            and resource.template.name in self.tosca.discovered
+            and resource.template.nested_name in self.tosca.discovered
         ):
-            discovered[resource.template.name] = self.tosca.discovered[
+            discovered[resource.template.nested_name] = self.tosca.discovered[
                 resource.template.name
             ]
 
         if resource._capabilities:
             capabilities = list(
                 filter(
                     None,
@@ -715,37 +735,44 @@
                 filter(
                     None, map(self._save_entity_if_instantiated, resource._artifacts)
                 )
             )
             if artifacts:
                 status["artifacts"] = CommentedMap(artifacts)
 
+        if cast(NodeSpec, resource.template).substitution and resource.shadow:
+            assert resource.shadow.root is not resource.root, (
+                resource is resource.shadow,
+                resource.root,
+            )
+            status["substitution"] = self.save_root_resource(
+                cast(TopologyInstance, resource.shadow.root), discovered
+            )
+
         if resource.instances:
             status["instances"] = CommentedMap(
                 filter(
                     None,
                     map(
-                        lambda r: self.save_resource(r, discovered), resource.instances
+                        lambda r: self.save_resource(r, discovered), resource.instances  # type: ignore
                     ),
                 )
             )
-
         return (name, status)
 
-    def save_root_resource(self, discovered):
-        resource = self.rootResource
+    def save_root_resource(self, root: TopologyInstance, discovered):
+        resource = root
         assert resource
         status = CommentedMap()
 
         # record the input and output values
         status["inputs"] = serialize_value(resource.attributes["inputs"])
         status["outputs"] = serialize_value(resource.attributes["outputs"])
 
         save_status(resource, status)
-        # getOperationalDependencies() skips inputs and outputs
         status["instances"] = CommentedMap(
             filter(
                 None,
                 map(
                     lambda r: self.save_resource(r, discovered),
                     resource.get_operational_dependencies(),
                 ),
@@ -788,15 +815,16 @@
         if self.currentCommitId:
             output["startCommit"] = self.currentCommitId
         output["specDigest"] = self.specDigest
         return save_status(job, output)
 
     def save_job(self, job):
         discovered = CommentedMap()
-        changed = self.save_root_resource(discovered)
+        assert self.rootResource
+        changed = self.save_root_resource(self.rootResource, discovered)
 
         # update changed with includes, this may change objects with references to these objects
         self.manifest.restore_includes(changed)
         # only saved discovered templates that are still referenced
         spec = self.manifest.config.setdefault("spec", {})
         spec.pop("discovered", None)
         if discovered:
@@ -886,23 +914,23 @@
             return "Commit by Unfurl"
 
     def get_repo_status(self, dirty=False) -> str:
         return "".join([r.get_repo_status(dirty) for r in self.repositories.values()])
 
     def add_all(self) -> None:
         for repository in self.repositories.values():
-            if not repository.readOnly and repository.is_dirty():
+            if not repository.read_only and repository.is_dirty():
                 repository.add_all()
 
     def commit(self, msg: str, add_all: bool = False) -> int:
         committed = 0
         for repository in self.repositories.values():
             if repository.repo == self.repo:
                 continue
-            if not repository.readOnly and repository.is_dirty():
+            if not repository.read_only and repository.is_dirty():
                 retVal = repository.commit(msg, add_all)
                 committed += 1
                 logger.info(
                     "committed %s to %s: %s", retVal, repository.working_dir, msg
                 )
         # if manifest was changed: # e.g. calling commit after a job was run
         #    if commits were made writeLock and save updated manifest??
```

### Comparing `unfurl-0.6.2/unfurl.egg-info/PKG-INFO` & `unfurl-0.7.0/unfurl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfurl
-Version: 0.6.2
+Version: 0.7.0
 Summary: use Git to record and deploy changes to your DevOps infrastructure
 Home-page: https://github.com/onecommons/unfurl
 Author: Adam Souzis
 Author-email: adam@onecommons.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: full
+Provides-Extra: server
 Provides-Extra: test
 License-File: LICENSE
 
 <p align="center">
   <img src="https://docs.unfurl.run/_images/unfurl_logo.svg" width="400px">
 </p>
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: unfurl Version: 0.6.2 Summary: use Git to record
+Metadata-Version: 2.1 Name: unfurl Version: 0.7.0 Summary: use Git to record
 and deploy changes to your DevOps infrastructure Home-page: https://github.com/
 onecommons/unfurl Author: Adam Souzis Author-email: adam@onecommons.org
 License: MIT Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-Provides-Extra: full Provides-Extra: test License-File: LICENSE
+Provides-Extra: full Provides-Extra: server Provides-Extra: test License-File:
+LICENSE
                [https://docs.unfurl.run/_images/unfurl_logo.svg]
                                 [PyPI_version]
 # Introduction Unfurl is a command line tool for managing your DevOps
 infrastructure. Unfurl lets you easily track configuration, secrets, software
 and code dependencies, and deployment history all in git. Unfurl can integrate
 with the DevOps tools you are already using -- like Terraform, Ansible, and
 Helm -- allowing you to encapsulate your DevOps processes into reusable
```

### Comparing `unfurl-0.6.2/unfurl.egg-info/SOURCES.txt` & `unfurl-0.7.0/unfurl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unfurl-0.6.2/unfurl.egg-info/requires.txt` & `unfurl-0.7.0/unfurl.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -45,14 +45,18 @@
 gunicorn==20.1.0
 octodns==0.9.14
 openshift
 python-gitlab<=3.4.0
 redis==4.3.5
 supervisor
 
+[server]
+gunicorn==20.1.0
+redis==4.3.5
+
 [test]
 boto3==1.21.46
 botocore==1.24.46
 coverage
 jinja2==3.1.2
 moto[server]==3.1.4
 mypy==0.950
```

