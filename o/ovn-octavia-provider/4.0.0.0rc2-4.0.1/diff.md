# Comparing `tmp/ovn-octavia-provider-4.0.0.0rc2.tar.gz` & `tmp/ovn-octavia-provider-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovn-octavia-provider-4.0.0.0rc2.tar", last modified: Fri Mar 17 15:42:18 2023, max compression
+gzip compressed data, was "ovn-octavia-provider-4.0.1.tar", last modified: Thu Jun  8 14:41:09 2023, max compression
```

## Comparing `ovn-octavia-provider-4.0.0.0rc2.tar` & `ovn-octavia-provider-4.0.1.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.871280 ovn-octavia-provider-4.0.0.0rc2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3092 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/.pylintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7990 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2023-03-17 15:42:18.871280 ovn-octavia-provider-4.0.0.0rc2/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.847280 ovn-octavia-provider-4.0.0.0rc2/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4164 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/devstack/local.conf.sample
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1980 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.847280 ovn-octavia-provider-4.0.0.0rc2/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.847280 ovn-octavia-provider-4.0.0.0rc2/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12963 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/admin/driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2788 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/configuration/config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13845 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/contributor/loadbalancer.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/doc/source/pdf-index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.843280 ovn-octavia-provider-4.0.0.0rc2/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/etc/octavia/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/etc/octavia/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/etc/octavia/conf.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/etc/octavia/conf.d/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/etc/oslo-config-generator/ovn.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.851280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2374 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.855280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4271 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6277 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4219 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2773 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26138 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3198 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/event.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.855280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6906 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   136426 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      771 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.855280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/ovsdb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9761 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/ovsdb/impl_idl_ovn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3710 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/ovsdb/ovsdb_monitor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.855280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.855280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51550 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10201 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/test_agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21679 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7050 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/test_integration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.859280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2455 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.859280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3499 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/common/test_clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2155 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/common/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9964 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.859280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11807 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/hacking/test_checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.859280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/ovsdb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/ovsdb/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6410 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/ovsdb/test_impl_idl_ovn.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.859280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/schemas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25838 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/schemas/ovn-nb.ovsschema
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26568 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/schemas/ovn-sb.ovsschema
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1159 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52034 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_hacking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   218326 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_helper.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.855280 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4168 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2023-03-17 15:42:18.000000 ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.859280 ovn-octavia-provider-4.0.0.0rc2/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/playbooks/configure_functional_job.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/playbooks/post_functional_job.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/playbooks/run_functional_job.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.843280 ovn-octavia-provider-4.0.0.0rc2/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.863280 ovn-octavia-provider-4.0.0.0rc2/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/notes/add-hm-support-2c6729d8816125a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/notes/add-sctp-support-bedfed905e1f5a58.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/notes/drop-python-3-6-and-3-7-e890961ed94c146e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/notes/new-repository-for-ovn-octavia-provider-driver-dd81c4414c529c4e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/notes/ovn-octavia-provider-driver-multiple-protocols-4a93e184b8f374c7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/notes/support-member-create-without-subnetid-0b4e3aa6ac453f28.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.863280 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1472 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.863280 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.863280 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8629 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.843280 ovn-octavia-provider-4.0.0.0rc2/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.863280 ovn-octavia-provider-4.0.0.0rc2/roles/configure_functional_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/configure_functional_tests/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/configure_functional_tests/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/configure_functional_tests/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/configure_functional_tests/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/configure_functional_tests/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/fetch_journal_log/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/fetch_journal_log/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/fetch_journal_log/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/fetch_journal_log/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/fetch_journal_log/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/fetch_journal_log/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/setup_logdir/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/setup_logdir/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/setup_logdir/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/setup_logdir/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/roles/setup_logdir/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/roles/setup_logdir/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2023-03-17 15:42:18.871280 ovn-octavia-provider-4.0.0.0rc2/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1737 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/tools/check_unit_test_structure.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1587 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/tools/coding-checks.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      792 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/tools/generate_config_file_samples.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      658 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/tools/pip_install_src_modules.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5584 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-17 15:42:18.867280 ovn-octavia-provider-4.0.0.0rc2/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6677 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/zuul.d/base.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2023-03-17 15:41:49.000000 ovn-octavia-provider-4.0.0.0rc2/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.932103 ovn-octavia-provider-4.0.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3092 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2023-06-08 14:41:09.000000 ovn-octavia-provider-4.0.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8279 2023-06-08 14:41:09.000000 ovn-octavia-provider-4.0.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2030 2023-06-08 14:41:09.936103 ovn-octavia-provider-4.0.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.912103 ovn-octavia-provider-4.0.1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4164 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/devstack/local.conf.sample
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1980 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.912103 ovn-octavia-provider-4.0.1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.912103 ovn-octavia-provider-4.0.1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.912103 ovn-octavia-provider-4.0.1/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/doc/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.912103 ovn-octavia-provider-4.0.1/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12963 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/doc/source/admin/driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2788 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.912103 ovn-octavia-provider-4.0.1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/doc/source/configuration/config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.912103 ovn-octavia-provider-4.0.1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13845 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/doc/source/contributor/loadbalancer.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/doc/source/pdf-index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.904103 ovn-octavia-provider-4.0.1/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.912103 ovn-octavia-provider-4.0.1/etc/octavia/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/etc/octavia/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.912103 ovn-octavia-provider-4.0.1/etc/octavia/conf.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/etc/octavia/conf.d/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.912103 ovn-octavia-provider-4.0.1/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/etc/oslo-config-generator/ovn.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.916103 ovn-octavia-provider-4.0.1/ovn_octavia_provider/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2374 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.920103 ovn-octavia-provider-4.0.1/ovn_octavia_provider/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4271 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/common/clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6277 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4219 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/common/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2773 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25019 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3198 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/event.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.920103 ovn-octavia-provider-4.0.1/ovn_octavia_provider/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6906 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   138567 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      771 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.920103 ovn-octavia-provider-4.0.1/ovn_octavia_provider/ovsdb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11652 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/ovsdb/impl_idl_ovn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3710 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/ovsdb/ovsdb_monitor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.920103 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.920103 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52244 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/functional/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/functional/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10201 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/functional/test_agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22591 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/functional/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7050 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/functional/test_integration.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.924103 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2455 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.924103 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3499 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/common/test_clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2155 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/common/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9964 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.924103 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11807 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/hacking/test_checks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.924103 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/ovsdb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/ovsdb/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6410 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/ovsdb/test_impl_idl_ovn.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.924103 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/schemas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25838 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/schemas/ovn-nb.ovsschema
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26568 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/schemas/ovn-sb.ovsschema
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1159 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/test_agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52877 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/test_hacking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   224393 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/test_helper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.916103 ovn-octavia-provider-4.0.1/ovn_octavia_provider.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2030 2023-06-08 14:41:09.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4168 2023-06-08 14:41:09.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-08 14:41:09.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-06-08 14:41:09.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-08 14:41:09.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-06-08 14:41:09.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-06-08 14:41:09.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2023-06-08 14:41:09.000000 ovn-octavia-provider-4.0.1/ovn_octavia_provider.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.928103 ovn-octavia-provider-4.0.1/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/playbooks/configure_functional_job.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/playbooks/post_functional_job.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/playbooks/run_functional_job.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.904103 ovn-octavia-provider-4.0.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.928103 ovn-octavia-provider-4.0.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/notes/add-hm-support-2c6729d8816125a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/notes/add-sctp-support-bedfed905e1f5a58.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/notes/drop-python-3-6-and-3-7-e890961ed94c146e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/notes/new-repository-for-ovn-octavia-provider-driver-dd81c4414c529c4e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/notes/ovn-octavia-provider-driver-multiple-protocols-4a93e184b8f374c7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/notes/support-member-create-without-subnetid-0b4e3aa6ac453f28.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.928103 ovn-octavia-provider-4.0.1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1472 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/source/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.932103 ovn-octavia-provider-4.0.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.932103 ovn-octavia-provider-4.0.1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8629 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.908103 ovn-octavia-provider-4.0.1/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.932103 ovn-octavia-provider-4.0.1/roles/configure_functional_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/roles/configure_functional_tests/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.932103 ovn-octavia-provider-4.0.1/roles/configure_functional_tests/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/roles/configure_functional_tests/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.932103 ovn-octavia-provider-4.0.1/roles/configure_functional_tests/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/roles/configure_functional_tests/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.932103 ovn-octavia-provider-4.0.1/roles/fetch_journal_log/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/roles/fetch_journal_log/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.932103 ovn-octavia-provider-4.0.1/roles/fetch_journal_log/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/roles/fetch_journal_log/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.932103 ovn-octavia-provider-4.0.1/roles/fetch_journal_log/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/roles/fetch_journal_log/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.932103 ovn-octavia-provider-4.0.1/roles/setup_logdir/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/roles/setup_logdir/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.932103 ovn-octavia-provider-4.0.1/roles/setup_logdir/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/roles/setup_logdir/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.932103 ovn-octavia-provider-4.0.1/roles/setup_logdir/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/roles/setup_logdir/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2023-06-08 14:41:09.936103 ovn-octavia-provider-4.0.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.932103 ovn-octavia-provider-4.0.1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1737 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/tools/check_unit_test_structure.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1587 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/tools/coding-checks.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      792 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/tools/generate_config_file_samples.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      658 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/tools/pip_install_src_modules.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5584 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-08 14:41:09.932103 ovn-octavia-provider-4.0.1/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6067 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/zuul.d/base.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-06-08 14:40:41.000000 ovn-octavia-provider-4.0.1/zuul.d/project.yaml
```

### Comparing `ovn-octavia-provider-4.0.0.0rc2/.pylintrc` & `ovn-octavia-provider-4.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/AUTHORS` & `ovn-octavia-provider-4.0.1/AUTHORS`

 * *Files 19% similar despite different names*

```diff
@@ -18,7 +18,8 @@
 Miguel Lavalle <mlavalle@redhat.com>
 OpenStack Release Bot <infra-root@openstack.org>
 Rodolfo Alonso Hernandez <ralonsoh@redhat.com>
 Sean McGinnis <sean.mcginnis@gmail.com>
 Slawek Kaplonski <skaplons@redhat.com>
 Terry Wilson <twilson@redhat.com>
 shanyunfan33 <shanyunfan@inspur.com>
+yatinkarel <ykarel@redhat.com>
```

### Comparing `ovn-octavia-provider-4.0.0.0rc2/CONTRIBUTING.rst` & `ovn-octavia-provider-4.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ChangeLog` & `ovn-octavia-provider-4.0.1/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 CHANGES
 =======
 
-4.0.0.0rc2
-----------
+4.0.1
+-----
+
+* Discard batch-update-members not valid request
+* Apply admin\_state\_up on a new member creation
+* Add retry on case of sqlite3.InterfaceError on FT
+* Fix update member action
+* Use ovsdbapp commands to add/del backends to ip\_port\_mappings
+* [stable/2023.1 only] Drop -master jobs
+
+4.0.0
+-----
 
 * Add new FTs for health monitoring basic operations
 * Remove HM uuiid from LB external\_ids when the HM's pool is deleted
 * Fix broken pep8 jobs due to bandit 1.7.5 updated version
 * Update TOX\_CONSTRAINTS\_FILE for stable/2023.1
 * Update .gitreview for stable/2023.1
```

### Comparing `ovn-octavia-provider-4.0.0.0rc2/HACKING.rst` & `ovn-octavia-provider-4.0.1/HACKING.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/LICENSE` & `ovn-octavia-provider-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/PKG-INFO` & `ovn-octavia-provider-4.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ovn-octavia-provider
-Version: 4.0.0.0rc2
+Version: 4.0.1
 Summary: OpenStack Octavia integration with OVN
 Home-page: https://docs.openstack.org/ovn-octavia-provider/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===================================================================
         ovn-octavia-provider - OVN Provider driver for Octavia LoadBalancer
```

### Comparing `ovn-octavia-provider-4.0.0.0rc2/README.rst` & `ovn-octavia-provider-4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/devstack/local.conf.sample` & `ovn-octavia-provider-4.0.1/devstack/local.conf.sample`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/devstack/plugin.sh` & `ovn-octavia-provider-4.0.1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/doc/source/admin/driver.rst` & `ovn-octavia-provider-4.0.1/doc/source/admin/driver.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/doc/source/conf.py` & `ovn-octavia-provider-4.0.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/doc/source/contributor/loadbalancer.rst` & `ovn-octavia-provider-4.0.1/doc/source/contributor/loadbalancer.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/doc/source/index.rst` & `ovn-octavia-provider-4.0.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/doc/source/pdf-index.rst` & `ovn-octavia-provider-4.0.1/doc/source/pdf-index.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/agent.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/agent.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/clients.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/common/clients.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/config.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/common/config.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/constants.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/common/constants.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/exceptions.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/common/utils.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/common/utils.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/driver.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -325,63 +325,48 @@
                         'subnet_id': subnet_id,
                         'action': ovn_const.REQ_INFO_MEMBER_DELETED}
         request = {'type': ovn_const.REQ_TYPE_HANDLE_MEMBER_DVR,
                    'info': request_info}
         self._ovn_helper.add_request(request)
 
     def member_update(self, old_member, new_member):
-        # NOTE(froyo): OVN provider allow to create member without param
-        # subnet_id, in that case the driver search it according to the
-        # pool_id, but it is not propagated to Octavia. In this case, if
-        # the member is updated, Octavia send the object without subnet_id.
-        subnet_id = old_member.subnet_id
-        if (isinstance(subnet_id, o_datamodels.UnsetType) or not subnet_id):
-            subnet_id, subnet_cidr = self._ovn_helper._get_subnet_from_pool(
-                old_member.pool_id)
-            if not (subnet_id and
-                    self._ovn_helper._check_ip_in_subnet(new_member.address,
-                                                         subnet_cidr)):
-                msg = _('Subnet is required, or Loadbalancer associated with '
-                        'Pool must have a subnet, for Member update '
-                        'with OVN Provider Driver if it is not the same as '
-                        'LB VIP subnet')
-                raise driver_exceptions.UnsupportedOptionError(
-                    user_fault_string=msg,
-                    operator_fault_string=msg)
-
         # Validate monitoring options if present
         self._check_member_monitor_options(new_member)
         if new_member.address and self._ip_version_differs(new_member):
             raise ovn_exc.IPVersionsMixingNotSupportedError()
         request_info = {'id': new_member.member_id,
                         'address': old_member.address,
                         'protocol_port': old_member.protocol_port,
                         'pool_id': old_member.pool_id,
-                        'subnet_id': subnet_id,
                         'old_admin_state_up': old_member.admin_state_up}
         if not isinstance(new_member.admin_state_up, o_datamodels.UnsetType):
             request_info['admin_state_up'] = new_member.admin_state_up
         request = {'type': ovn_const.REQ_TYPE_MEMBER_UPDATE,
                    'info': request_info}
         self._ovn_helper.add_request(request)
 
     def member_batch_update(self, pool_id, members):
         request_list = []
-        skipped_members = []
         pool_key, ovn_lb = self._ovn_helper._find_ovn_lb_by_pool_id(pool_id)
         external_ids = copy.deepcopy(ovn_lb.external_ids)
         pool = external_ids[pool_key]
         existing_members = pool.split(',') if pool else []
         members_to_delete = copy.copy(existing_members)
         pool_subnet_id = None
         for member in members:
-            if (self._check_monitor_options(member) or
-                    member.address and self._ip_version_differs(member)):
-                skipped_members.append(member.member_id)
-                continue
+            # NOTE(froyo): in order to keep sync with Octavia DB, we raise
+            # not supporting exceptions as soon as posible, considering the
+            # full request as not valid
+            if (self._check_monitor_options(member)):
+                msg = 'OVN provider does not support monitor options'
+                raise driver_exceptions.UnsupportedOptionError(
+                    user_fault_string=msg,
+                    operator_fault_string=msg)
+            if (member.address and self._ip_version_differs(member)):
+                raise ovn_exc.IPVersionsMixingNotSupportedError()
             # NOTE(froyo): if subnet_id not provided, lets try to get it
             # from the member pool_id
             subnet_id = member.subnet_id
             if (isinstance(subnet_id, o_datamodels.UnsetType) or
                     not subnet_id):
                 if not pool_subnet_id:
                     pool_subnet_id, pool_subnet_cidr = (
@@ -421,34 +406,28 @@
                             'admin_state_up': admin_state_up}
             request = {'type': req_type,
                        'info': request_info}
             request_list.append(request)
 
         for member in members_to_delete:
             member_info = member.split('_')
-            member_ip, member_port, subnet_id = (
+            member_ip, member_port, subnet_id, member_id = (
                 self._ovn_helper._extract_member_info(member)[0])
             request_info = {'id': member_info[1],
                             'address': member_ip,
                             'protocol_port': member_port,
                             'pool_id': pool_id}
             if len(member_info) == 4:
                 request_info['subnet_id'] = subnet_id
             request = {'type': ovn_const.REQ_TYPE_MEMBER_DELETE,
                        'info': request_info}
             request_list.append(request)
 
         for request in request_list:
             self._ovn_helper.add_request(request)
-        if skipped_members:
-            msg = (_('OVN provider does not support monitor options, '
-                     'so following members skipped: %s') % skipped_members)
-            raise driver_exceptions.UnsupportedOptionError(
-                user_fault_string=msg,
-                operator_fault_string=msg)
 
     def create_vip_port(self, lb_id, project_id, vip_dict,
                         additional_vip_dicts=None):
         """Create the VIP port of a load balancer
 
         :param lb_id: The ID of the load balancer
         :param project_id: The ID of the project that owns the load balancer
```

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/event.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/event.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/hacking/checks.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/helper.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -838,18 +838,19 @@
         return pool_key
 
     def _extract_member_info(self, member):
         mem_info = []
         if member:
             for mem in member.split(','):
                 mem_split = mem.split('_')
+                mem_id = mem_split[1]
                 mem_ip_port = mem_split[2]
                 mem_ip, mem_port = mem_ip_port.rsplit(':', 1)
                 mem_subnet = mem_split[3]
-                mem_info.append((mem_ip, mem_port, mem_subnet))
+                mem_info.append((mem_ip, mem_port, mem_subnet, mem_id))
         return mem_info
 
     def _get_member_info(self, member):
         member_info = ''
         if isinstance(member, dict):
             subnet_id = member.get(constants.SUBNET_ID, '')
             member_info = (
@@ -896,15 +897,18 @@
             if ovn_const.LB_EXT_IDS_LISTENER_PREFIX not in k:
                 continue
             vip_port, p_key = self._extract_listener_key_value(v)
             if pool_key == p_key:
                 return vip_port
         return None
 
-    def _frame_vip_ips(self, lb_external_ids):
+    def _is_member_offline(self, ovn_lb, member_id):
+        return constants.OFFLINE == self._find_member_status(ovn_lb, member_id)
+
+    def _frame_vip_ips(self, ovn_lb, lb_external_ids):
         vip_ips = {}
         # If load balancer is disabled, return
         if lb_external_ids.get('enabled') == 'False':
             return vip_ips
 
         lb_vip = lb_external_ids[ovn_const.LB_EXT_IDS_VIP_KEY]
         vip_fip = lb_external_ids.get(ovn_const.LB_EXT_IDS_VIP_FIP_KEY)
@@ -918,37 +922,39 @@
             if not vip_port or not pool_id:
                 continue
 
             if pool_id not in lb_external_ids or not lb_external_ids[pool_id]:
                 continue
 
             ips = []
-            for member_ip, member_port, subnet in self._extract_member_info(
+            for mb_ip, mb_port, mb_subnet, mb_id in self._extract_member_info(
                     lb_external_ids[pool_id]):
-                if netaddr.IPNetwork(member_ip).version == 6:
-                    ips.append(f'[{member_ip}]:{member_port}')
-                else:
-                    ips.append(f'{member_ip}:{member_port}')
+                if not self._is_member_offline(ovn_lb, mb_id):
+                    if netaddr.IPNetwork(mb_ip).version == 6:
+                        ips.append(f'[{mb_ip}]:{mb_port}')
+                    else:
+                        ips.append(f'{mb_ip}:{mb_port}')
 
-            if netaddr.IPNetwork(lb_vip).version == 6:
-                lb_vip = f'[{lb_vip}]'
-            vip_ips[lb_vip + ':' + vip_port] = ','.join(ips)
-
-            if vip_fip:
-                if netaddr.IPNetwork(vip_fip).version == 6:
-                    vip_fip = f'[{vip_fip}]'
-                vip_ips[vip_fip + ':' + vip_port] = ','.join(ips)
+            if ips:
+                if netaddr.IPNetwork(lb_vip).version == 6:
+                    lb_vip = f'[{lb_vip}]'
+                vip_ips[lb_vip + ':' + vip_port] = ','.join(ips)
+
+                if vip_fip:
+                    if netaddr.IPNetwork(vip_fip).version == 6:
+                        vip_fip = f'[{vip_fip}]'
+                    vip_ips[vip_fip + ':' + vip_port] = ','.join(ips)
 
         return vip_ips
 
-    def _refresh_lb_vips(self, ovn_lb_uuid, lb_external_ids):
-        vip_ips = self._frame_vip_ips(lb_external_ids)
-        return [self.ovn_nbdb_api.db_clear('Load_Balancer', ovn_lb_uuid,
+    def _refresh_lb_vips(self, ovn_lb, lb_external_ids):
+        vip_ips = self._frame_vip_ips(ovn_lb, lb_external_ids)
+        return [self.ovn_nbdb_api.db_clear('Load_Balancer', ovn_lb.uuid,
                                            'vips'),
-                self.ovn_nbdb_api.db_set('Load_Balancer', ovn_lb_uuid,
+                self.ovn_nbdb_api.db_set('Load_Balancer', ovn_lb.uuid,
                                          ('vips', vip_ips))]
 
     def _is_listener_in_lb(self, lb):
         for key in list(lb.external_ids):
             if key.startswith(ovn_const.LB_EXT_IDS_LISTENER_PREFIX):
                 return True
         return False
@@ -1311,15 +1317,15 @@
                     enable_info = {'enabled': str(lb_enabled)}
                     ovn_lb.external_ids['enabled'] = str(lb_enabled)
                     commands.append(
                         self.ovn_nbdb_api.db_set('Load_Balancer', ovn_lb.uuid,
                                                  ('external_ids', enable_info))
                     )
                     commands.extend(
-                        self._refresh_lb_vips(ovn_lb.uuid,
+                        self._refresh_lb_vips(ovn_lb,
                                               ovn_lb.external_ids))
                     self._execute_commands(commands)
                 if lb_enabled:
                     operating_status = constants.ONLINE
                 else:
                     operating_status = constants.OFFLINE
                 lb_status[constants.OPERATING_STATUS] = operating_status
@@ -1360,15 +1366,15 @@
                                          ('external_ids', listener_info)))
             if not self._is_listener_in_lb(ovn_lb):
                 commands.append(
                     self.ovn_nbdb_api.db_set(
                         'Load_Balancer', ovn_lb.uuid,
                         ('protocol',
                          str(listener[constants.PROTOCOL]).lower())))
-            commands.extend(self._refresh_lb_vips(ovn_lb.uuid, external_ids))
+            commands.extend(self._refresh_lb_vips(ovn_lb, external_ids))
             self._execute_commands(commands)
         except Exception:
             LOG.exception(ovn_const.EXCEPTION_MSG, "creation of listener")
             status = {
                 constants.LISTENERS: [
                     {constants.ID: listener[constants.ID],
                      constants.PROVISIONING_STATUS: constants.ERROR,
@@ -1431,15 +1437,15 @@
                 cmds, lb_to_delete = self._clean_lb_if_empty(
                     ovn_lb, listener[constants.LOADBALANCER_ID], external_ids)
                 commands.extend(cmds)
                 # Do not refresh vips if OVN LB for given protocol
                 # has pending delete operation.
                 if not lb_to_delete:
                     commands.extend(
-                        self._refresh_lb_vips(ovn_lb.uuid, external_ids))
+                        self._refresh_lb_vips(ovn_lb, external_ids))
                 self._execute_commands(commands)
             except Exception:
                 LOG.exception(ovn_const.EXCEPTION_MSG, "deletion of listener")
                 status = {
                     constants.LISTENERS: [
                         {constants.ID: listener[constants.ID],
                          constants.PROVISIONING_STATUS: constants.ERROR,
@@ -1537,15 +1543,15 @@
             if l_key_to_add:
                 commands.append(
                     self.ovn_nbdb_api.db_set(
                         'Load_Balancer', ovn_lb.uuid,
                         ('external_ids', l_key_to_add)))
 
             commands.extend(
-                self._refresh_lb_vips(ovn_lb.uuid, external_ids))
+                self._refresh_lb_vips(ovn_lb, external_ids))
             self._execute_commands(commands)
         except Exception:
             LOG.exception(ovn_const.EXCEPTION_MSG, "update of listener")
             status = {
                 constants.LISTENERS: [
                     {constants.ID: listener[constants.ID],
                      constants.PROVISIONING_STATUS: constants.ERROR}],
@@ -1637,15 +1643,15 @@
             pool_listeners = self._get_pool_listeners(ovn_lb, pool_key)
             if pool_key in ovn_lb.external_ids:
                 commands.append(
                     self.ovn_nbdb_api.db_remove('Load_Balancer', ovn_lb.uuid,
                                                 'external_ids', (pool_key)))
                 del external_ids[pool_key]
                 commands.extend(
-                    self._refresh_lb_vips(ovn_lb.uuid, external_ids))
+                    self._refresh_lb_vips(ovn_lb, external_ids))
             # Remove Pool from Listener if it is associated
             for key, value in ovn_lb.external_ids.items():
                 if (key.startswith(ovn_const.LB_EXT_IDS_LISTENER_PREFIX) and
                         pool_key in value):
                     external_ids[key] = value.split(':')[0] + ':'
                     commands.append(
                         self.ovn_nbdb_api.db_set(
@@ -1738,15 +1744,15 @@
 
                 commands.append(
                     self.ovn_nbdb_api.db_set(
                         'Load_Balancer', ovn_lb.uuid,
                         ('external_ids', p_key_to_add)))
 
                 commands.extend(
-                    self._refresh_lb_vips(ovn_lb.uuid, external_ids))
+                    self._refresh_lb_vips(ovn_lb, external_ids))
                 self._execute_commands(commands)
             if pool[constants.ADMIN_STATE_UP]:
                 operating_status = constants.ONLINE
             else:
                 operating_status = constants.OFFLINE
             pool_status[constants.OPERATING_STATUS] = operating_status
 
@@ -1854,15 +1860,19 @@
 
         commands = []
         commands.append(
             self.ovn_nbdb_api.db_set('Load_Balancer', ovn_lb.uuid,
                                      ('external_ids', pool_data)))
 
         external_ids[pool_key] = pool_data[pool_key]
-        commands.extend(self._refresh_lb_vips(ovn_lb.uuid, external_ids))
+
+        # NOTE(froyo): Add the member to the vips if it is enabled
+        if member.get(constants.ADMIN_STATE_UP, False):
+            commands.extend(self._refresh_lb_vips(ovn_lb, external_ids))
+
         # Note (froyo): commands are now splitted to separate atomic process,
         # leaving outside the not mandatory ones to allow add_member
         # finish correctly
         self._execute_commands(commands)
 
         subnet_id = member[constants.SUBNET_ID]
         self._update_lb_to_ls_association(
@@ -1904,21 +1914,16 @@
             pool_key, ovn_lb = self._find_ovn_lb_by_pool_id(
                 member[constants.POOL_ID])
             pool_listeners = self._get_pool_listeners(ovn_lb, pool_key)
             new_member = self._add_member(member, ovn_lb, pool_key)
             pool = {constants.ID: member[constants.POOL_ID],
                     constants.PROVISIONING_STATUS: constants.ACTIVE,
                     constants.OPERATING_STATUS: constants.ONLINE}
-            member_status = {constants.ID: member[constants.ID],
-                             constants.PROVISIONING_STATUS: constants.ACTIVE}
-            if not member[constants.ADMIN_STATE_UP]:
-                member_status[constants.OPERATING_STATUS] = constants.OFFLINE
             status = {
                 constants.POOLS: [pool],
-                constants.MEMBERS: [member_status],
                 constants.LOADBALANCERS: [
                     {constants.ID: ovn_lb.name,
                      constants.PROVISIONING_STATUS: constants.ACTIVE}]}
         except Exception:
             LOG.exception(ovn_const.EXCEPTION_MSG, "creation of member")
             status = {
                 constants.POOLS: [
@@ -1935,46 +1940,61 @@
         for listener in pool_listeners:
             listener_status.append(
                 {constants.ID: listener,
                  constants.PROVISIONING_STATUS: constants.ACTIVE})
         status[constants.LISTENERS] = listener_status
 
         operating_status = constants.NO_MONITOR
-        if new_member and ovn_lb.health_check:
+        if not member[constants.ADMIN_STATE_UP]:
+            operating_status = constants.OFFLINE
+        elif (new_member and operating_status == constants.NO_MONITOR and
+                ovn_lb.health_check):
             operating_status = constants.ONLINE
-            if not self._update_hm_members(ovn_lb, pool_key):
+            mb_ip, mb_port, mb_subnet, mb_id = self._extract_member_info(
+                new_member)[0]
+            if not self._update_hm_member(ovn_lb, pool_key, mb_ip):
                 operating_status = constants.ERROR
-            member_status[constants.OPERATING_STATUS] = operating_status
+        member_status = {constants.ID: member[constants.ID],
+                         constants.PROVISIONING_STATUS: constants.ACTIVE,
+                         constants.OPERATING_STATUS: operating_status}
+        status[constants.MEMBERS] = [member_status]
 
         self._update_external_ids_member_status(
             ovn_lb,
             member[constants.ID],
             operating_status)
 
         return status
 
     def _remove_member(self, member, ovn_lb, pool_key):
         external_ids = copy.deepcopy(ovn_lb.external_ids)
         existing_members = external_ids[pool_key].split(",")
         member_info = self._get_member_info(member)
         if member_info in existing_members:
+
+            if ovn_lb.health_check:
+                self._update_hm_member(ovn_lb,
+                                       pool_key,
+                                       member.get(constants.ADDRESS),
+                                       delete=True)
+
             commands = []
             existing_members.remove(member_info)
 
             if not existing_members:
                 pool_status = constants.OFFLINE
             else:
                 pool_status = constants.ONLINE
             pool_data = {pool_key: ",".join(existing_members)}
             commands.append(
                 self.ovn_nbdb_api.db_set('Load_Balancer', ovn_lb.uuid,
                                          ('external_ids', pool_data)))
             external_ids[pool_key] = ",".join(existing_members)
             commands.extend(
-                self._refresh_lb_vips(ovn_lb.uuid, external_ids))
+                self._refresh_lb_vips(ovn_lb, external_ids))
             self._execute_commands(commands)
             self._update_lb_to_ls_association(
                 ovn_lb, subnet_id=member.get(constants.SUBNET_ID),
                 associate=False, update_ls_ref=True)
             return pool_status
         else:
             msg = f"Member {member[constants.ID]} not found in the pool"
@@ -1988,22 +2008,21 @@
             pool_key, ovn_lb = self._find_ovn_lb_by_pool_id(
                 member[constants.POOL_ID])
             pool_listeners = self._get_pool_listeners(ovn_lb, pool_key)
             pool_status = self._remove_member(member, ovn_lb, pool_key)
             pool = {constants.ID: member[constants.POOL_ID],
                     constants.PROVISIONING_STATUS: constants.ACTIVE,
                     constants.OPERATING_STATUS: pool_status}
-            if ovn_lb.health_check:
-                self._update_hm_members(ovn_lb, pool_key)
+            if ovn_lb.health_check and pool_status == constants.OFFLINE:
                 # NOTE(froyo): if the pool status is OFFLINE there are no more
                 # members. So we should ensure the hm-port is deleted if no
                 # more LB are using it. We need to do this call after the
                 # cleaning of the ip_port_mappings for the ovn LB.
-                if pool_status == constants.OFFLINE:
-                    self._clean_up_hm_port(member['subnet_id'])
+                self._clean_up_hm_port(member[constants.SUBNET_ID])
+
             status = {
                 constants.POOLS: [pool],
                 constants.MEMBERS: [
                     {constants.ID: member[constants.ID],
                      constants.PROVISIONING_STATUS: constants.DELETED}],
                 constants.LOADBALANCERS: [
                     {constants.ID: ovn_lb.name,
@@ -2029,33 +2048,14 @@
             listener_status.append(
                 {constants.ID: listener,
                  constants.PROVISIONING_STATUS: constants.ACTIVE})
         status[constants.LISTENERS] = listener_status
 
         return status
 
-    def _update_member(self, member, ovn_lb, pool_key):
-        commands = []
-        external_ids = copy.deepcopy(ovn_lb.external_ids)
-        existing_members = external_ids[pool_key].split(",")
-        member_info = self._get_member_info(member)
-        for mem in existing_members:
-            if (member_info.split('_')[1] == mem.split('_')[1] and
-                    mem != member_info):
-                existing_members.remove(mem)
-                existing_members.append(member_info)
-                pool_data = {pool_key: ",".join(existing_members)}
-                commands.append(
-                    self.ovn_nbdb_api.db_set('Load_Balancer', ovn_lb.uuid,
-                                             ('external_ids', pool_data)))
-                external_ids[pool_key] = ",".join(existing_members)
-                commands.extend(
-                    self._refresh_lb_vips(ovn_lb.uuid, external_ids))
-                self._execute_commands(commands)
-
     def member_update(self, member):
         pool_listeners = []
         try:
             pool_key, ovn_lb = self._find_ovn_lb_by_pool_id(
                 member[constants.POOL_ID])
             member_status = {constants.ID: member[constants.ID],
                              constants.PROVISIONING_STATUS: constants.ACTIVE}
@@ -2064,49 +2064,65 @@
                     {constants.ID: member[constants.POOL_ID],
                      constants.PROVISIONING_STATUS: constants.ACTIVE}],
                 constants.MEMBERS: [member_status],
                 constants.LOADBALANCERS: [
                     {constants.ID: ovn_lb.name,
                      constants.PROVISIONING_STATUS: constants.ACTIVE}]}
             pool_listeners = self._get_pool_listeners(ovn_lb, pool_key)
-            self._update_member(member, ovn_lb, pool_key)
+            last_status = self._find_member_status(
+                ovn_lb, member[constants.ID])
             if constants.ADMIN_STATE_UP in member:
                 if member[constants.ADMIN_STATE_UP]:
                     # if HM exists trust on neutron:member_status
                     # as the last status valid for the member
                     if ovn_lb.health_check:
                         # search status of member_uuid
-                        last_status = self._find_member_status(
-                            ovn_lb, member[constants.ID])
                         member_status[constants.OPERATING_STATUS] = last_status
                     else:
                         member_status[constants.OPERATING_STATUS] = (
                             constants.NO_MONITOR)
                 else:
                     member_status[constants.OPERATING_STATUS] = (
                         constants.OFFLINE)
+
+                if constants.OPERATING_STATUS in member_status:
+                    self._update_external_ids_member_status(
+                        ovn_lb,
+                        member[constants.ID],
+                        member_status[constants.OPERATING_STATUS])
+
+                # NOTE(froyo): If we are toggling from/to OFFLINE due to an
+                # admin_state_up change, in that case we should update vips
+                if (
+                    last_status != constants.OFFLINE and
+                    member_status[constants.OPERATING_STATUS] ==
+                    constants.OFFLINE
+                ) or (
+                    last_status == constants.OFFLINE and
+                    member_status[constants.OPERATING_STATUS] !=
+                    constants.OFFLINE
+                ):
+                    commands = []
+                    commands.extend(self._refresh_lb_vips(ovn_lb,
+                                                          ovn_lb.external_ids))
+                    self._execute_commands(commands)
+
         except Exception:
             LOG.exception(ovn_const.EXCEPTION_MSG, "update of member")
             status = {
                 constants.POOLS: [
                     {constants.ID: member[constants.POOL_ID],
                      constants.PROVISIONING_STATUS: constants.ACTIVE}],
                 constants.MEMBERS: [
                     {constants.ID: member[constants.ID],
                      constants.PROVISIONING_STATUS: constants.ERROR}],
                 constants.LOADBALANCERS: [
                     {constants.ID: ovn_lb.name,
                      constants.PROVISIONING_STATUS: constants.ACTIVE}]}
 
-        if constants.OPERATING_STATUS in member_status:
-            self._update_external_ids_member_status(
-                ovn_lb,
-                member[constants.ID],
-                member_status[constants.OPERATING_STATUS])
-
         listener_status = []
         for listener in pool_listeners:
             listener_status.append(
                 {constants.ID: listener,
                  constants.PROVISIONING_STATUS: constants.ACTIVE})
         status[constants.LISTENERS] = listener_status
         return status
@@ -2233,15 +2249,15 @@
                                                     ovn_lb.uuid,
                                                     'health_check',
                                                     lbhc.uuid))
                     commands.append(self.ovn_nbdb_api.db_destroy(
                         'Load_Balancer_Health_Check', lbhc.uuid))
                     break
 
-        commands.extend(self._refresh_lb_vips(ovn_lb.uuid, external_ids))
+        commands.extend(self._refresh_lb_vips(ovn_lb, external_ids))
         self._execute_commands(commands)
 
     def handle_member_dvr(self, info):
         pool_key, ovn_lb = self._find_ovn_lb_by_pool_id(info['pool_id'])
         if not ovn_lb.external_ids.get(ovn_const.LB_EXT_IDS_VIP_FIP_KEY):
             LOG.debug("LB %(lb)s has no FIP on VIP configured. "
                       "There is no need to centralize member %(member)s "
@@ -2488,94 +2504,122 @@
                 commands.append(
                     self.ovn_nbdb_api.db_set(
                         'Load_Balancer_Health_Check',
                         ovn_lb.health_check[1].uuid, ('vip', fip)))
         self._execute_commands(commands)
         return True
 
-    def _update_hm_members(self, ovn_lb, pool_key):
-        mappings = {}
-        # For each member, set it's HM
-        for member_ip, member_port, member_subnet in self._extract_member_info(
-                ovn_lb.external_ids[pool_key]):
-            member_lsp = self._get_member_lsp(member_ip, member_subnet)
-            if not member_lsp:
-                # NOTE(froyo): In order to continue evaluating the rest of
-                # the members, we just warn about the member issue,
-                # assuming that it will be in OFFLINE status as soon as the
-                # HM does the first evaluation.
-                LOG.error("Member %(member)s Logical_Switch_Port not found, "
-                          "when creating a Health Monitor for pool %(pool)s.",
-                          {'member': member_ip, 'pool': pool_key})
-                continue
+    def _update_ip_port_mappings(self, ovn_lb, backend_ip, port_name, src_ip,
+                                 delete=False):
 
-            network_id = member_lsp.external_ids.get(
-                ovn_const.OVN_NETWORK_NAME_EXT_ID_KEY).split('neutron-')[1]
-            project_id = member_lsp.external_ids.get(
-                ovn_const.OVN_PROJECT_EXT_ID_KEY)
-            hm_port = self._ensure_hm_ovn_port(
-                network_id, member_subnet, project_id)
-            if not hm_port:
-                LOG.error("No port on network %(network)s available for "
-                          "health monitoring. Cannot create a Health Monitor "
-                          "for pool %(pool)s.",
-                          {'network': network_id,
-                           'pool': pool_key})
-                return False
-            hm_source_ip = None
-            for fixed_ip in hm_port['fixed_ips']:
-                if fixed_ip['subnet_id'] == member_subnet:
-                    hm_source_ip = fixed_ip['ip_address']
-                    break
-            if not hm_source_ip:
-                LOG.error("No port on subnet %(subnet)s available for "
-                          "health monitoring member IP %(member)s. Cannot "
-                          "create a Health Monitor for pool %(pool)s.",
-                          {'subnet': member_subnet,
-                           'member': member_ip,
-                           'pool': pool_key})
-                return False
-            # ovn-nbctl set load_balancer ${OVN_LB_ID}
-            #   ip_port_mappings:${MEMBER_IP}=${LSP_NAME_MEMBER}:${HEALTH_SRC}
-            # where:
-            #  OVN_LB_ID: id of LB
-            #  MEMBER_IP: IP of member_lsp
-            #  HEALTH_SRC: source IP of hm_port
-
-            # need output like this
-            # vips: {"172.24.4.246:80"="10.0.0.10:80"}
-            # ip_port_mappings: {"10.0.0.10"="ID:10.0.0.2"}
-            # ip_port_mappings: {"MEMBER_IP"="LSP_NAME_MEMBER:HEALTH_SRC"}
-            # OVN does not support IPv6 Health Checks, but we check anyways
-            member_src = f'{member_lsp.name}:'
-            if netaddr.IPNetwork(hm_source_ip).version == 6:
-                member_src += f'[{hm_source_ip}]'
-            else:
-                member_src += f'{hm_source_ip}'
+        # ip_port_mappings:${MEMBER_IP}=${LSP_NAME_MEMBER}:${HEALTH_SRC}
+        # where:
+        #  MEMBER_IP: IP of member_lsp
+        #  LSP_NAME_MEMBER: Logical switch port
+        #  HEALTH_SRC: source IP of hm_port
 
-            if netaddr.IPNetwork(member_ip).version == 6:
-                member_ip = f'[{member_ip}]'
-            mappings[member_ip] = member_src
+        if delete:
+            self.ovn_nbdb_api.lb_del_ip_port_mapping(ovn_lb.uuid,
+                                                     backend_ip).execute()
+        else:
+            self.ovn_nbdb_api.lb_add_ip_port_mapping(ovn_lb.uuid,
+                                                     backend_ip,
+                                                     port_name,
+                                                     src_ip).execute()
 
-        commands = []
-        # NOTE(froyo): This db_clear over field ip_port_mappings is needed just
-        # to clean the old values (including the removed member) and the
-        # following db_set will update the using the mappings calculated some
-        # lines above with reemaining members only.
-        # TODO(froyo): use the ovsdbapp commands to add/del members to
-        # ip_port_mappings field
-        commands.append(
+    def _clean_ip_port_mappings(self, ovn_lb, pool_key=None):
+        if not pool_key:
             self.ovn_nbdb_api.db_clear('Load_Balancer', ovn_lb.uuid,
-                                       'ip_port_mappings'))
-        if mappings:
-            commands.append(
-                self.ovn_nbdb_api.db_set(
-                    'Load_Balancer', ovn_lb.uuid,
-                    ('ip_port_mappings', mappings)))
-        self._execute_commands(commands)
+                                       'ip_port_mappings').execute()
+        else:
+            # NOTE(froyo): before removing a member from the ip_port_mappings
+            # list, we need to ensure that the member is not being monitored by
+            # any other existing HM. To prevent accidentally removing the
+            # member we can use the neutron:member_status to search for any
+            # other members with the same address
+            members_try_remove = self._extract_member_info(
+                ovn_lb.external_ids[pool_key])
+            other_members = []
+            for k, v in ovn_lb.external_ids.items():
+                if ovn_const.LB_EXT_IDS_POOL_PREFIX in k and k != pool_key:
+                    other_members.extend(self._extract_member_info(
+                        ovn_lb.external_ids[k]))
+
+            member_statuses = ovn_lb.external_ids.get(
+                ovn_const.OVN_MEMBER_STATUS_KEY)
+
+            try:
+                member_statuses = jsonutils.loads(member_statuses)
+            except TypeError:
+                LOG.debug("no member status on external_ids: %s",
+                          str(member_statuses))
+                member_statuses = {}
+
+            for (mb_ip, mb_port, mb_subnet, mb_id) in members_try_remove:
+                delete = True
+                for member_id in [item[3] for item in other_members
+                                  if item[0] == mb_ip]:
+                    if member_statuses.get(
+                            member_id, '') != constants.NO_MONITOR:
+                        # same address being monitorized by another HM
+                        delete = False
+
+                if delete:
+                    self.ovn_nbdb_api.lb_del_ip_port_mapping(
+                        ovn_lb.uuid, mb_ip).execute()
+
+    def _update_hm_member(self, ovn_lb, pool_key, backend_ip, delete=False):
+        # Update just the backend_ip member
+        for mb_ip, mb_port, mb_subnet, mb_id in self._extract_member_info(
+                ovn_lb.external_ids[pool_key]):
+            member_lsp = self._get_member_lsp(mb_ip, mb_subnet)
+            if mb_ip == backend_ip:
+                if not member_lsp:
+                    # NOTE(froyo): In order to continue evaluating the rest of
+                    # the members, we just warn about the member issue,
+                    # assuming that it will be in OFFLINE status as soon as the
+                    # HM does the first evaluation.
+                    LOG.error("Member %(member)s Logical_Switch_Port not "
+                              "found, when creating a Health Monitor for "
+                              "pool %(pool)s.",
+                              {'member': mb_ip, 'pool': pool_key})
+                    break
+
+                network_id = member_lsp.external_ids.get(
+                    ovn_const.OVN_NETWORK_NAME_EXT_ID_KEY).split('neutron-')[1]
+                project_id = member_lsp.external_ids.get(
+                    ovn_const.OVN_PROJECT_EXT_ID_KEY)
+                hm_port = self._ensure_hm_ovn_port(
+                    network_id, mb_subnet, project_id)
+                if not hm_port:
+                    LOG.error("No port on network %(network)s available for "
+                              "health monitoring. Cannot find a Health "
+                              "Monitor for pool %(pool)s.",
+                              {'network': network_id, 'pool': pool_key})
+                    return False
+                hm_source_ip = None
+                for fixed_ip in hm_port['fixed_ips']:
+                    if fixed_ip['subnet_id'] == mb_subnet:
+                        hm_source_ip = fixed_ip['ip_address']
+                        break
+                if not hm_source_ip:
+                    LOG.error("No port on subnet %(subnet)s available for "
+                              "health monitoring member IP %(member)s. Cannot "
+                              "find a Health Monitor for pool %(pool)s.",
+                              {'subnet': mb_subnet,
+                               'member': mb_ip,
+                               'pool': pool_key})
+                    return False
+                self._update_ip_port_mappings(ovn_lb, backend_ip,
+                                              member_lsp.name, hm_source_ip,
+                                              delete)
+                return True
+
+        # NOTE(froyo): If the backend is not located or just one member but not
+        # found the lsp
         return True
 
     def _lookup_lbhcs_by_hm_id(self, hm_id):
         lbhc_rows = self.ovn_nbdb_api.db_list_rows(
             'Load_Balancer_Health_Check').execute(check_error=True)
         lbhcs = []
         for lbhc in lbhc_rows:
@@ -2654,17 +2698,21 @@
         # ovn-nbctl --wait=sb -- --id=@hc create Load_Balancer_Health_Check
         #   vip="${LB_VIP_ADDR}\:${MONITOR_PRT}" -- add Load_Balancer
         #   ${OVN_LB_ID} health_check @hc
         # options here are interval, timeout, failure_count and success_count
         # from info object passed-in
         hm_status = self._add_lbhc(ovn_lb, pool_key, info)
         if hm_status[constants.PROVISIONING_STATUS] == constants.ACTIVE:
-            if not self._update_hm_members(ovn_lb, pool_key):
-                hm_status[constants.PROVISIONING_STATUS] = constants.ERROR
-                hm_status[constants.OPERATING_STATUS] = constants.ERROR
+            for mb_ip, mb_port, mb_subnet, mb_id in self._extract_member_info(
+                    ovn_lb.external_ids[pool_key]):
+                if not self._update_hm_member(ovn_lb, pool_key, mb_ip):
+                    hm_status[constants.PROVISIONING_STATUS] = constants.ERROR
+                    hm_status[constants.OPERATING_STATUS] = constants.ERROR
+                    self._clean_ip_port_mappings(ovn_lb, pool_key)
+                    break
         status[constants.HEALTHMONITORS] = [hm_status]
         return status
 
     def hm_update(self, info):
         status = {
             constants.HEALTHMONITORS: [
                 {constants.ID: info[constants.ID],
@@ -2744,15 +2792,16 @@
         pool_id = None
         pool_listeners = []
         member_subnets = []
         for k, v in ovn_lb.external_ids.items():
             if ovn_const.LB_EXT_IDS_POOL_PREFIX in k:
                 members = self._extract_member_info(ovn_lb.external_ids[k])
                 member_subnets = list(
-                    set([mem_subnet for (_, _, mem_subnet) in members])
+                    set([mb_subnet
+                         for (mb_ip, mb_port, mb_subnet, mb_id) in members])
                 )
                 pool_id = k.split('_')[1]
                 pool_listeners = self._get_pool_listeners(
                     ovn_lb, self._get_pool_key(pool_id))
                 break
 
         # ovn-nbctl clear load_balancer ${OVN_LB_ID} ip_port_mappings
@@ -2765,18 +2814,19 @@
                                                      constants.ACTIVE,
                                                      constants.NO_MONITOR)
 
         if hms_key:
             hms_key = jsonutils.loads(hms_key)
             if hm_id in hms_key:
                 hms_key.remove(hm_id)
+
+        self._clean_ip_port_mappings(ovn_lb, ovn_const.LB_EXT_IDS_POOL_PREFIX +
+                                     str(pool_id_related))
+
         commands = []
-        commands.append(
-            self.ovn_nbdb_api.db_clear('Load_Balancer', ovn_lb.uuid,
-                                       'ip_port_mappings'))
         for lbhc in lbhcs:
             commands.append(
                 self.ovn_nbdb_api.db_remove('Load_Balancer', ovn_lb.uuid,
                                             'health_check', lbhc.uuid))
             commands.append(
                 self.ovn_nbdb_api.db_destroy('Load_Balancer_Health_Check',
                                              lbhc.uuid))
@@ -3001,25 +3051,23 @@
         for ovn_lb in ovn_lbs:
             # Lookup member
             member_id = None
             for k, v in ovn_lb.external_ids.items():
                 if ovn_const.LB_EXT_IDS_POOL_PREFIX not in k:
                     continue
                 for (
-                    member_ip,
-                    member_port,
-                    subnet,
+                    mb_ip, mb_port, mb_subnet, mb_id,
                 ) in self._extract_member_info(v):
-                    if info['ip'] != member_ip:
+                    if info['ip'] != mb_ip:
                         continue
-                    if info['port'] != member_port:
+                    if info['port'] != mb_port:
                         continue
                     # match
                     member_id = [mb.split('_')[1] for mb in v.split(',')
-                                 if member_ip in mb and member_port in mb][0]
+                                 if mb_ip in mb and mb_port in mb][0]
                     break
 
                 # found it in inner loop
                 if member_id:
                     break
 
             if not member_id:
```

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/i18n.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/i18n.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/ovsdb/impl_idl_ovn.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/ovsdb/impl_idl_ovn.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import atexit
 import contextlib
 
+import netaddr
+
 from neutron_lib import exceptions as n_exc
 from oslo_log import log
 from ovsdbapp.backend import ovs_idl
 from ovsdbapp.backend.ovs_idl import command
 from ovsdbapp.backend.ovs_idl import connection
 from ovsdbapp.backend.ovs_idl import idlutils
 from ovsdbapp.backend.ovs_idl import rowview
@@ -133,14 +135,43 @@
 class GetLrsCommand(command.ReadOnlyCommand):
     def run_idl(self, txn):
         self.result = [
             rowview.RowView(item) for item in
             self.api.tables['Logical_Router'].rows.values()]
 
 
+class LbAddIpPortMappingCommand(command.BaseCommand):
+    table = 'Load_Balancer'
+
+    def __init__(self, api, lb, endpoint_ip, port_name, source_ip):
+        super().__init__(api)
+        self.lb = lb
+        self.endpoint_ip = str(netaddr.IPAddress(endpoint_ip))
+        self.port_name = port_name
+        self.source_ip = str(netaddr.IPAddress(source_ip))
+
+    def run_idl(self, txn):
+        lb = self.api.lookup(self.table, self.lb)
+        lb.setkey('ip_port_mappings', self.endpoint_ip,
+                  '%s:%s' % (self.port_name, self.source_ip))
+
+
+class LbDelIpPortMappingCommand(command.BaseCommand):
+    table = 'Load_Balancer'
+
+    def __init__(self, api, lb, endpoint_ip):
+        super().__init__(api)
+        self.lb = lb
+        self.endpoint_ip = str(netaddr.IPAddress(endpoint_ip))
+
+    def run_idl(self, txn):
+        lb = self.api.lookup(self.table, self.lb)
+        lb.delkey('ip_port_mappings', self.endpoint_ip)
+
+
 class OvsdbNbOvnIdl(nb_impl_idl.OvnNbApiIdlImpl, Backend):
     def __init__(self, connection):
         super().__init__(connection)
         self.idl._session.reconnect.set_probe_interval(
             config.get_ovn_ovsdb_probe_interval())
 
     @property
@@ -168,14 +199,29 @@
 
     def find_lb_in_table(self, lb, table):
         return FindLbInTableCommand(self, lb, table)
 
     def get_lrs(self):
         return GetLrsCommand(self)
 
+    # FIXME (froyo): Remove this method once the ovsdbapp version is upgraded
+    # to a version higher than 2.1.0, it will be possible to remove this method
+    # This is done due to some conflict on bumping the noted version. Also
+    # class LbDelIpPortMappingCommand shall be removed at the same time.
+    def lb_del_ip_port_mapping(self, lb, endpoint_ip):
+        return LbDelIpPortMappingCommand(self, lb, endpoint_ip)
+
+    # FIXME (froyo): Remove this method once the ovsdbapp version is upgraded
+    # to a version higher than 2.1.0, it will be possible to remove this method
+    # This is done due to some conflict on bumping the noted version. Also
+    # class LbAddIpPortMappingCommand shall be removed at the same time.
+    def lb_add_ip_port_mapping(self, lb, endpoint_ip, port_name, source_ip):
+        return LbAddIpPortMappingCommand(self, lb, endpoint_ip, port_name,
+                                         source_ip)
+
 
 class OvsdbSbOvnIdl(sb_impl_idl.OvnSbApiIdlImpl, Backend):
     def __init__(self, connection):
         super().__init__(connection)
         self.idl._session.reconnect.set_probe_interval(
             config.get_ovn_ovsdb_probe_interval())
```

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/ovsdb/ovsdb_monitor.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/ovsdb/ovsdb_monitor.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/base.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/functional/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,22 @@
 from unittest import mock
 
 from neutron.common import utils as n_utils
 from neutron_lib.plugins import directory
 from octavia_lib.api.drivers import data_models as octavia_data_model
 from octavia_lib.api.drivers import driver_lib
 from octavia_lib.common import constants as o_constants
+from oslo_db import exception as odb_exc
 from oslo_serialization import jsonutils
 from oslo_utils import uuidutils
 from ovsdbapp.schema.ovn_northbound import impl_idl as nb_idl_ovn
 from ovsdbapp.schema.ovn_southbound import impl_idl as sb_idl_ovn
 
+import tenacity
+
 # NOTE(mjozefcz): We need base neutron functionals because we need
 # mechanism driver and l3 plugin.
 from neutron.tests.functional import base
 from ovn_octavia_provider.common import clients
 from ovn_octavia_provider.common import constants as ovn_const
 from ovn_octavia_provider import driver as ovn_driver
 
@@ -250,24 +253,34 @@
         lb_uuid = self._get_loadbalancer_id(lb_name)
         for ls in self.nb_api.tables[table].rows.values():
             if ls.name == ls_name:
                 ls_lbs = [lb.uuid for lb in ls.load_balancer]
                 return lb_uuid in ls_lbs
         return False
 
+    @tenacity.retry(
+        retry=tenacity.retry_if_exception_type(odb_exc.DBError),
+        wait=tenacity.wait_exponential(),
+        stop=tenacity.stop_after_attempt(3),
+        reraise=True)
     def _create_router(self, name, gw_info=None):
         router = {'router':
                   {'name': name,
                    'admin_state_up': True,
                    'tenant_id': self._tenant_id}}
         if gw_info:
             router['router']['external_gateway_info'] = gw_info
         router = self.l3_plugin.create_router(self.context, router)
         return router['id']
 
+    @tenacity.retry(
+        retry=tenacity.retry_if_exception_type(odb_exc.DBError),
+        wait=tenacity.wait_exponential(),
+        stop=tenacity.stop_after_attempt(3),
+        reraise=True)
     def _create_net(self, name, cidr, router_id=None):
         n1 = self._make_network(self.fmt, name, True)
         res = self._create_subnet(self.fmt, n1['network']['id'],
                                   cidr)
         subnet = self.deserialize(self.fmt, res)['subnet']
         self._local_net_cache[subnet['id']] = n1['network']['id']
         self._local_cidr_cache[subnet['id']] = subnet['cidr']
@@ -599,16 +612,14 @@
         for p in lb_data.get('pools', []):
             member_status = {}
             external_ids = _get_lb_field_by_protocol(
                 p.protocol.lower(),
                 field='external_ids')
             p_members = ""
             for m in p.members:
-                if not m.admin_state_up:
-                    continue
                 m_info = 'member_' + m.member_id + '_' + m.address
                 m_info += ":" + str(m.protocol_port)
                 m_info += "_" + str(m.subnet_id)
                 if p_members:
                     p_members += "," + m_info
                 else:
                     p_members = m_info
@@ -625,15 +636,18 @@
                                 ex['neutron-%s' % port['network_id']] = act + 1
                                 break
                 if p.healthmonitor:
                     member_status[m.member_id] = o_constants.ONLINE
                     external_ids[ovn_const.LB_EXT_IDS_HMS_KEY] = \
                         jsonutils.dumps([p.healthmonitor.healthmonitor_id])
                 else:
-                    member_status[m.member_id] = o_constants.NO_MONITOR
+                    if m.admin_state_up:
+                        member_status[m.member_id] = o_constants.NO_MONITOR
+                    else:
+                        member_status[m.member_id] = o_constants.OFFLINE
             pool_key = 'pool_' + p.pool_id
             if not p.admin_state_up:
                 pool_key += ':D'
             external_ids[pool_key] = p_members
             pool_info[p.pool_id] = p_members
             if member_status:
                 external_ids[ovn_const.OVN_MEMBER_STATUS_KEY] = member_status
@@ -843,34 +857,36 @@
         expected_listener_status = [
             {'id': listener.listener_id, 'provisioning_status': 'ACTIVE'}
             for listener in pool_listeners]
 
         expected_status = {
             'pools': [pool_status],
             'members': [{"id": m_member.member_id,
-                         "provisioning_status": "ACTIVE"}],
+                         "provisioning_status": "ACTIVE",
+                         "operating_status": o_constants.NO_MONITOR}],
             'loadbalancers': [{'id': pool.loadbalancer_id,
                                'provisioning_status': 'ACTIVE'}],
             'listeners': expected_listener_status
         }
         self._wait_for_status_and_validate(lb_data, [expected_status])
 
     def _get_pool_member(self, pool, member_address):
         for m in pool.members:
             if m.address == member_address:
                 return m
 
     def _update_member_and_validate(self, lb_data, pool_id, member_address,
-                                    remove_subnet_id=False):
+                                    remove_subnet_id=False,
+                                    admin_state_up=True):
         pool = self._get_pool_from_lb_data(lb_data, pool_id=pool_id)
 
         member = self._get_pool_member(pool, member_address)
         self._o_driver_lib.update_loadbalancer_status.reset_mock()
         old_member = copy.deepcopy(member)
-
+        member.admin_state_up = admin_state_up
         # NOTE(froyo): In order to test update of member without passing the
         # subnet_id parameter of the member, just to cover the case when a new
         # member has been created without passing that argument
         if remove_subnet_id:
             old_member.subnet_id = None
 
         self.ovn_driver.member_update(old_member, member)
```

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/test_agent.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/functional/test_agent.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/test_driver.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/functional/test_driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,32 +103,38 @@
         pool_SCTP_id = lb_data['pools'][2].pool_id
 
         # Members for TCP Pool
         self._create_member_and_validate(
             lb_data, pool_TCP_id, lb_data['vip_net_info'][1],
             lb_data['vip_net_info'][0], '10.0.0.10')
         self._update_member_and_validate(lb_data, pool_TCP_id, "10.0.0.10")
+        self._update_member_and_validate(lb_data, pool_TCP_id, "10.0.0.10",
+                                         admin_state_up=False)
         self._create_member_and_validate(
             lb_data, pool_TCP_id, lb_data['vip_net_info'][1],
             lb_data['vip_net_info'][0], '10.0.0.11')
 
         # Members for UDP Pool
         self._create_member_and_validate(
             lb_data, pool_UDP_id, lb_data['vip_net_info'][1],
             lb_data['vip_net_info'][0], '10.0.0.10')
         self._update_member_and_validate(lb_data, pool_UDP_id, "10.0.0.10")
+        self._update_member_and_validate(lb_data, pool_UDP_id, "10.0.0.10",
+                                         admin_state_up=False)
         self._create_member_and_validate(
             lb_data, pool_UDP_id, lb_data['vip_net_info'][1],
             lb_data['vip_net_info'][0], '10.0.0.11')
 
         # Members for SCTP Pool
         self._create_member_and_validate(
             lb_data, pool_SCTP_id, lb_data['vip_net_info'][1],
             lb_data['vip_net_info'][0], '10.0.0.10')
         self._update_member_and_validate(lb_data, pool_SCTP_id, "10.0.0.10")
+        self._update_member_and_validate(lb_data, pool_SCTP_id, "10.0.0.10",
+                                         admin_state_up=False)
         self._create_member_and_validate(
             lb_data, pool_SCTP_id, lb_data['vip_net_info'][1],
             lb_data['vip_net_info'][0], '10.0.0.11')
 
         # Disable loadbalancer
         self._update_load_balancer_and_validate(lb_data,
                                                 admin_state_up=False)
@@ -454,8 +460,18 @@
         lb_data['pools'][0].members.append(m_member)
         # Add a new member to the LB
         members = [m_member] + [lb_data['pools'][0].members[0]]
         self._update_members_in_batch_and_validate(lb_data, pool_id, members)
         # Deleting one member, while keeping the other member available
         self._update_members_in_batch_and_validate(lb_data, pool_id,
                                                    [m_member])
+        # Create Member-3 with monitor options
+        m_member = self._create_member_model(pool_id,
+                                             lb_data['vip_net_info'][1],
+                                             '10.0.0.12')
+        m_member.monitor_port = 8080
+        members = [m_member]
+        self.assertRaises(o_exceptions.UnsupportedOptionError,
+                          self.ovn_driver.member_batch_update,
+                          pool_id,
+                          members)
         self._delete_load_balancer_and_validate(lb_data)
```

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/functional/test_integration.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/functional/test_integration.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/base.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/common/test_clients.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/common/test_clients.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/common/test_utils.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/fakes.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/fakes.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/hacking/test_checks.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/hacking/test_checks.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/ovsdb/test_impl_idl_ovn.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/ovsdb/test_impl_idl_ovn.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/schemas/ovn-nb.ovsschema` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/schemas/ovn-nb.ovsschema`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/schemas/ovn-sb.ovsschema` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/schemas/ovn-sb.ovsschema`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_agent.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/test_agent.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_driver.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/test_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,31 +362,29 @@
 
     def test_member_update(self):
         info = {'id': self.update_member.member_id,
                 'address': self.ref_member.address,
                 'protocol_port': self.ref_member.protocol_port,
                 'pool_id': self.ref_member.pool_id,
                 'admin_state_up': self.update_member.admin_state_up,
-                'old_admin_state_up': self.ref_member.admin_state_up,
-                'subnet_id': self.ref_member.subnet_id}
+                'old_admin_state_up': self.ref_member.admin_state_up}
         expected_dict = {'type': ovn_const.REQ_TYPE_MEMBER_UPDATE,
                          'info': info}
         self.driver.member_update(self.ref_member, self.update_member)
         self.mock_add_request.assert_called_once_with(expected_dict)
 
     def test_member_update_missing_subnet_id(self):
         self.driver._ovn_helper._get_subnet_from_pool.return_value = (
             self.ref_member.subnet_id, '198.52.100.0/24')
         info = {'id': self.update_member.member_id,
                 'address': self.ref_member.address,
                 'protocol_port': self.ref_member.protocol_port,
                 'pool_id': self.ref_member.pool_id,
                 'admin_state_up': self.update_member.admin_state_up,
-                'old_admin_state_up': self.ref_member.admin_state_up,
-                'subnet_id': self.ref_member.subnet_id}
+                'old_admin_state_up': self.ref_member.admin_state_up}
         expected_dict = {'type': ovn_const.REQ_TYPE_MEMBER_UPDATE,
                          'info': info}
         member = copy.copy(self.ref_member)
         member.subnet_id = data_models.UnsetType()
         self.driver.member_update(member, self.update_member)
         self.mock_add_request.assert_called_once_with(expected_dict)
 
@@ -394,43 +392,49 @@
         self.driver._ovn_helper._get_subnet_from_pool.return_value = (
             self.ref_member.subnet_id, '198.52.100.0/24')
         self.update_member.admin_state_up = data_models.UnsetType()
         info = {'id': self.update_member.member_id,
                 'address': self.ref_member.address,
                 'protocol_port': self.ref_member.protocol_port,
                 'pool_id': self.ref_member.pool_id,
-                'old_admin_state_up': self.ref_member.admin_state_up,
-                'subnet_id': self.ref_member.subnet_id}
+                'old_admin_state_up': self.ref_member.admin_state_up}
         expected_dict = {'type': ovn_const.REQ_TYPE_MEMBER_UPDATE,
                          'info': info}
         member = copy.copy(self.ref_member)
         member.subnet_id = data_models.UnsetType()
         self.driver.member_update(member, self.update_member)
         self.mock_add_request.assert_called_once_with(expected_dict)
 
-    def test_member_update_missing_subnet_id_differs_from_lb_vip(self):
-        self.driver._ovn_helper._get_subnet_from_pool.return_value = (
-            self.ref_member.subnet_id, '198.52.100.0/24')
-        self.driver._ovn_helper._check_ip_in_subnet.return_value = False
-        self.ref_member.subnet_id = data_models.UnsetType()
-        self.assertRaises(exceptions.UnsupportedOptionError,
-                          self.driver.member_update, self.ref_member,
-                          self.update_member)
-
     @mock.patch.object(ovn_driver.OvnProviderDriver, '_ip_version_differs')
     def test_member_update_no_ip_addr(self, mock_ip_differs):
         self.update_member.address = None
         self.driver.member_update(self.ref_member, self.update_member)
         mock_ip_differs.assert_not_called()
 
     def test_member_batch_update(self):
         self.driver.member_batch_update(self.pool_id,
                                         [self.ref_member, self.update_member])
         self.assertEqual(self.mock_add_request.call_count, 3)
 
+    def test_member_batch_update_member_delete(self):
+        info_md = {
+            'id': self.ref_member.member_id,
+            'address': mock.ANY,
+            'protocol_port': mock.ANY,
+            'pool_id': self.ref_member.pool_id,
+            'subnet_id': self.ref_member.subnet_id}
+        expected_dict_md = {
+            'type': ovn_const.REQ_TYPE_MEMBER_DELETE,
+            'info': info_md}
+        expected = [
+            mock.call(expected_dict_md)]
+        self.driver.member_batch_update(self.pool_id, [])
+        self.assertEqual(self.mock_add_request.call_count, 1)
+        self.mock_add_request.assert_has_calls(expected)
+
     def test_member_batch_update_no_members(self):
         pool_key = 'pool_%s' % self.pool_id
         ovn_lb = copy.copy(self.ovn_lb)
         ovn_lb.external_ids[pool_key] = []
         self.mock_find_lb_pool_key.return_value = ovn_lb
         self.driver.member_batch_update(self.pool_id,
                                         [self.ref_member, self.update_member])
@@ -451,14 +455,34 @@
                           [self.ref_member])
 
     def test_member_batch_update_unset_admin_state_up(self):
         self.ref_member.admin_state_up = data_models.UnsetType()
         self.driver.member_batch_update(self.pool_id, [self.ref_member])
         self.assertEqual(self.mock_add_request.call_count, 2)
 
+    def test_member_batch_update_toggle_admin_state_up(self):
+        info_mu = {
+            'id': self.ref_member.member_id,
+            'address': self.member_address,
+            'protocol_port': self.member_port,
+            'pool_id': self.ref_member.pool_id,
+            'subnet_id': self.ref_member.subnet_id,
+            'admin_state_up': False}
+        expected_dict_mu = {
+            'type': ovn_const.REQ_TYPE_MEMBER_UPDATE,
+            'info': info_mu}
+        expected = [
+            mock.call(expected_dict_mu)]
+        self.ref_member.admin_state_up = False
+        self.ref_member.address = self.member_address
+        self.ref_member.protocol_port = self.member_port
+        self.driver.member_batch_update(self.pool_id, [self.ref_member])
+        self.assertEqual(self.mock_add_request.call_count, 1)
+        self.mock_add_request.assert_has_calls(expected)
+
     def test_member_batch_update_missing_subnet_id(self):
         self.ref_member.subnet_id = None
         self.assertRaises(exceptions.UnsupportedOptionError,
                           self.driver.member_batch_update,
                           self.pool_id, [self.ref_member])
 
     def test_member_batch_update_missing_subnet_id_get_from_pool(self):
```

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_hacking.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/test_hacking.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider/tests/unit/test_helper.py` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider/tests/unit/test_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,136 @@
         self.mock_get_nw = mock.patch.object(
             self.helper, '_get_nw_router_info_on_interface_event',
             return_value=(self.router, self.network))
         self.mock_get_nw.start()
         (self.helper.ovn_nbdb_api.ls_get.return_value.
             execute.return_value) = self.network
 
+    def test__update_hm_member_no_members(self):
+        pool_key = 'pool_%s' % self.pool_id
+        self.ovn_lb.external_ids[pool_key] = ''
+        self.assertTrue(
+            self.helper._update_hm_member(self.ovn_lb,
+                                          pool_key,
+                                          '10.0.0.4'))
+
+    def test__update_hm_member_backend_ip_not_match(self):
+        pool_key = 'pool_%s' % self.pool_id
+        self.ovn_lb.external_ids[pool_key] = self.member_line
+        with mock.patch.object(ovn_helper.OvnProviderHelper,
+                               '_get_member_lsp'):
+            self.assertTrue(
+                self.helper._update_hm_member(self.ovn_lb,
+                                              pool_key,
+                                              '10.0.0.4'))
+
+    @mock.patch.object(ovn_helper.OvnProviderHelper, '_ensure_hm_ovn_port')
+    def test__update_hm_member_hm_port_multiple_ip(self, ensure_hm_port):
+        hm_port = {
+            'fixed_ips': [{
+                'subnet_id': 'ipv6_foo',
+                'ip_address': '2001:db8::199'}, {
+                'subnet_id': self.member_subnet_id,
+                'ip_address': '10.0.0.4'}]}
+        ensure_hm_port.return_value = hm_port
+        pool_key = 'pool_%s' % self.pool_id
+        with mock.patch.object(ovn_helper.OvnProviderHelper,
+                               '_get_member_lsp'):
+            self.assertTrue(
+                self.helper._update_hm_member(self.ovn_lb,
+                                              pool_key,
+                                              self.member_address))
+
+    @mock.patch.object(ovn_helper.OvnProviderHelper, '_ensure_hm_ovn_port')
+    def test__update_hm_member_hm_port_not_found(self, ensure_hm_port):
+        ensure_hm_port.return_value = None
+        pool_key = 'pool_%s' % self.pool_id
+        with mock.patch.object(ovn_helper.OvnProviderHelper,
+                               '_get_member_lsp'):
+            self.assertFalse(
+                self.helper._update_hm_member(self.ovn_lb,
+                                              pool_key,
+                                              self.member_address))
+
+    def test__clean_ip_port_mappings(self):
+        self.helper._clean_ip_port_mappings(self.ovn_hm_lb)
+        self.helper.ovn_nbdb_api.db_clear.assert_called_once_with(
+            'Load_Balancer', self.ovn_hm_lb.uuid, 'ip_port_mappings')
+
+    def test__clean_ip_port_mappings_two_hm_pools_sharing_members(self):
+        self.member_line_pool1 = 'member_uuid1_address1:port1_subnet1, \
+            member_uuid2_address2:port2_subnet1'
+        self.member_line_pool2 = 'member_uuid3_address1:port3_subnet1, \
+            member_uuid4_address4:port4_subnet1'
+        self.ovn_hm_lb.external_ids['pool_1'] = self.member_line_pool1
+        self.ovn_hm_lb.external_ids['pool_2'] = self.member_line_pool2
+        self.ovn_hm_lb.external_ids[ovn_const.OVN_MEMBER_STATUS_KEY] = \
+            '{"uuid1":  "ONLINE", "uuid2":  "ONLINE", \
+              "uuid3":  "ONLINE", "uuid4":  "ONLINE"}'
+        self.helper._clean_ip_port_mappings(self.ovn_hm_lb, 'pool_1')
+        self.helper.ovn_nbdb_api.db_clear.assert_not_called()
+        self.helper.ovn_nbdb_api.lb_del_ip_port_mapping.\
+            assert_called_once_with(self.ovn_hm_lb.uuid, 'address2')
+
+    def test__clean_ip_port_mappings_one_hm_pools_sharing_members(self):
+        self.member_line_pool1 = 'member_uuid1_address1:port1_subnet1, \
+            member_uuid2_address2:port2_subnet1'
+        self.member_line_pool2 = 'member_uuid3_address1:port3_subnet1, \
+            member_uuid4_address2:port4_subnet1'
+        self.ovn_hm_lb.external_ids['pool_1'] = self.member_line_pool1
+        self.ovn_hm_lb.external_ids['pool_2'] = self.member_line_pool2
+        self.ovn_hm_lb.external_ids[ovn_const.OVN_MEMBER_STATUS_KEY] = \
+            '{"uuid1":  "ONLINE", "uuid2":  "ONLINE", \
+              "uuid3":  "NO_MONITOR", "uuid4":  "NO_MONITOR"}'
+        self.helper._clean_ip_port_mappings(self.ovn_hm_lb, 'pool_1')
+        self.helper.ovn_nbdb_api.db_clear.assert_not_called()
+        self.helper.ovn_nbdb_api.lb_del_ip_port_mapping.\
+            assert_has_calls([mock.call(self.ovn_hm_lb.uuid, 'address1'),
+                              mock.ANY,
+                              mock.call(self.ovn_hm_lb.uuid, 'address2'),
+                              mock.ANY])
+
+    def test__clean_ip_port_mappings_two_hm_pools_not_sharing_members(self):
+        self.member_line_pool1 = 'member_uuid1_address1:port1_subnet1, \
+            member_uuid2_address2:port2_subnet1'
+        self.member_line_pool2 = 'member_uuid3_address3:port3_subnet1, \
+            member_uuid4_address4:port4_subnet1'
+        self.ovn_hm_lb.external_ids['pool_1'] = self.member_line_pool1
+        self.ovn_hm_lb.external_ids['pool_2'] = self.member_line_pool2
+        self.ovn_hm_lb.external_ids[ovn_const.OVN_MEMBER_STATUS_KEY] = \
+            '{"uuid1":  "ONLINE", "uuid2":  "ONLINE", \
+              "uuid3":  "ONLINE", "uuid4":  "ONLINE"}'
+        self.helper._clean_ip_port_mappings(self.ovn_hm_lb, 'pool_1')
+        self.helper.ovn_nbdb_api.db_clear.assert_not_called()
+        self.helper.ovn_nbdb_api.lb_del_ip_port_mapping.\
+            assert_has_calls([mock.call(self.ovn_hm_lb.uuid, 'address1'),
+                              mock.ANY,
+                              mock.call(self.ovn_hm_lb.uuid, 'address2'),
+                              mock.ANY])
+
+    def test__update_ip_port_mappings(self):
+        src_ip = '10.22.33.4'
+        fakes.FakeOvsdbRow.create_one_ovsdb_row(
+            attrs={'ip': self.member_address,
+                   'logical_port': 'a-logical-port',
+                   'src_ip': src_ip,
+                   'port': self.member_port,
+                   'protocol': self.ovn_hm_lb.protocol,
+                   'status': ovn_const.HM_EVENT_MEMBER_PORT_ONLINE})
+        self.helper._update_ip_port_mappings(
+            self.ovn_lb, self.member_address, 'a-logical-port', src_ip)
+        self.helper.ovn_nbdb_api.lb_add_ip_port_mapping.\
+            assert_called_once_with(self.ovn_lb.uuid, self.member_address,
+                                    'a-logical-port', src_ip)
+        self.helper._update_ip_port_mappings(
+            self.ovn_lb, self.member_address, 'a-logical-port', src_ip,
+            delete=True)
+        self.helper.ovn_nbdb_api.lb_del_ip_port_mapping.\
+            assert_called_once_with(self.ovn_lb.uuid, self.member_address)
+
     def test__update_external_ids_member_status(self):
         self.helper._update_external_ids_member_status(
             self.ovn_lb, self.member_id, constants.NO_MONITOR)
         member_status = {
             ovn_const.OVN_MEMBER_STATUS_KEY: '{"%s": "%s"}'
             % (self.member_id, constants.NO_MONITOR)}
         self.helper.ovn_nbdb_api.db_set.assert_called_once_with(
@@ -898,15 +1020,15 @@
         self.lb['admin_state_up'] = False
         status = self.helper.lb_update(self.lb)
         self.assertEqual(status['loadbalancers'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['loadbalancers'][0]['operating_status'],
                          constants.OFFLINE)
         refresh_vips.assert_called_once_with(
-            self.ovn_lb.uuid, self.ovn_lb.external_ids)
+            self.ovn_lb, self.ovn_lb.external_ids)
         self.helper.ovn_nbdb_api.db_set.assert_called_once_with(
             'Load_Balancer', self.ovn_lb.uuid,
             ('external_ids', {'enabled': 'False'}))
 
     @mock.patch.object(ovn_helper.OvnProviderHelper, '_refresh_lb_vips')
     def test_lb_update_enabled(self, refresh_vips):
         # Change the mock, its enabled by default.
@@ -914,28 +1036,28 @@
         self.lb['admin_state_up'] = True
         status = self.helper.lb_update(self.lb)
         self.assertEqual(status['loadbalancers'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['loadbalancers'][0]['operating_status'],
                          constants.ONLINE)
         refresh_vips.assert_called_once_with(
-            self.ovn_lb.uuid, self.ovn_lb.external_ids)
+            self.ovn_lb, self.ovn_lb.external_ids)
         self.helper.ovn_nbdb_api.db_set.assert_called_once_with(
             'Load_Balancer', self.ovn_lb.uuid,
             ('external_ids', {'enabled': 'True'}))
         # update to re-enable
         self.ovn_lb.external_ids.update({'enabled': True})
         self.lb['admin_state_up'] = True
         status = self.helper.lb_update(self.lb)
         self.assertEqual(status['loadbalancers'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['loadbalancers'][0]['operating_status'],
                          constants.ONLINE)
         refresh_vips.assert_called_once_with(
-            self.ovn_lb.uuid, self.ovn_lb.external_ids)
+            self.ovn_lb, self.ovn_lb.external_ids)
         self.helper.ovn_nbdb_api.db_set.assert_called_once_with(
             'Load_Balancer', self.ovn_lb.uuid,
             ('external_ids', {'enabled': 'True'}))
 
     @mock.patch.object(ovn_helper.OvnProviderHelper, '_refresh_lb_vips')
     def test_lb_update_enabled_multiple_protocols(self, refresh_vips):
         self.mock_find_ovn_lbs.stop()
@@ -948,18 +1070,18 @@
         self.lb['admin_state_up'] = True
         status = self.helper.lb_update(self.lb)
         self.assertEqual(status['loadbalancers'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['loadbalancers'][0]['operating_status'],
                          constants.ONLINE)
         refresh_vips.assert_has_calls([
-            mock.call(self.ovn_lb.uuid, self.ovn_lb.external_ids),
+            mock.call(self.ovn_lb, self.ovn_lb.external_ids),
             mock.ANY,
             mock.ANY,
-            mock.call(udp_lb.uuid, udp_lb.external_ids)],
+            mock.call(udp_lb, udp_lb.external_ids)],
             any_order=False)
         self.helper.ovn_nbdb_api.db_set.assert_has_calls([
             mock.call('Load_Balancer', self.ovn_lb.uuid,
                       ('external_ids', {'enabled': 'True'})),
             mock.call('Load_Balancer', udp_lb.uuid,
                       ('external_ids', {'enabled': 'True'}))])
 
@@ -982,15 +1104,15 @@
     def test_listener_create_disabled(self, refresh_vips):
         self.ovn_lb.external_ids.pop('listener_%s' % self.listener_id)
         status = self.helper.listener_create(self.listener)
         # Set expected as disabled
         self.ovn_lb.external_ids.update({
             'listener_%s:D' % self.listener_id: '80:pool_%s' % self.pool_id})
         refresh_vips.assert_called_once_with(
-            self.ovn_lb.uuid, self.ovn_lb.external_ids)
+            self.ovn_lb, self.ovn_lb.external_ids)
         expected_calls = [
             mock.call(
                 'Load_Balancer', self.ovn_lb.uuid,
                 ('external_ids', {
                     'listener_%s:D' % self.listener_id:
                         '80:pool_%s' % self.pool_id})),
             mock.call('Load_Balancer', self.ovn_lb.uuid, ('protocol', 'tcp'))]
@@ -1006,15 +1128,15 @@
                          constants.OFFLINE)
 
     @mock.patch.object(ovn_helper.OvnProviderHelper, '_refresh_lb_vips')
     def test_listener_create_enabled(self, refresh_vips):
         self.listener['admin_state_up'] = True
         status = self.helper.listener_create(self.listener)
         refresh_vips.assert_called_once_with(
-            self.ovn_lb.uuid, self.ovn_lb.external_ids)
+            self.ovn_lb, self.ovn_lb.external_ids)
         expected_calls = [
             mock.call(
                 'Load_Balancer', self.ovn_lb.uuid,
                 ('external_ids', {
                     'listener_%s' % self.listener_id:
                         '80:pool_%s' % self.pool_id}))]
         self.helper.ovn_nbdb_api.db_set.assert_has_calls(expected_calls)
@@ -1112,15 +1234,15 @@
                 'listener_%s' % self.listener_id:
                 '123:pool_%s' % self.pool_id}))
         # Update expected listener, because it was updated.
         self.ovn_lb.external_ids.pop('listener_%s' % self.listener_id)
         self.ovn_lb.external_ids.update(
             {'listener_%s' % self.listener_id: '123:pool_%s' % self.pool_id})
         refresh_vips.assert_called_once_with(
-            self.ovn_lb.uuid, self.ovn_lb.external_ids)
+            self.ovn_lb, self.ovn_lb.external_ids)
 
     @mock.patch.object(ovn_helper.OvnProviderHelper, '_refresh_lb_vips')
     def test_listener_update_listener_disabled(self, refresh_vips):
         self.listener['admin_state_up'] = False
         status = self.helper.listener_update(self.listener)
         self.assertEqual(status['loadbalancers'][0]['provisioning_status'],
                          constants.ACTIVE)
@@ -1134,15 +1256,15 @@
             'Load_Balancer', self.ovn_lb.uuid, 'external_ids',
             'listener_%s' % self.listener_id)
         # It gets disabled, so update the key
         self.ovn_lb.external_ids.pop('listener_%s' % self.listener_id)
         self.ovn_lb.external_ids.update(
             {'listener_%s:D' % self.listener_id: '80:pool_%s' % self.pool_id})
         refresh_vips.assert_called_once_with(
-            self.ovn_lb.uuid, self.ovn_lb.external_ids)
+            self.ovn_lb, self.ovn_lb.external_ids)
         # As it is marked disabled, a second call should not try and remove it
         self.helper.ovn_nbdb_api.db_remove.reset_mock()
         status = self.helper.listener_update(self.listener)
         self.assertEqual(status['listeners'][0]['operating_status'],
                          constants.OFFLINE)
         self.helper.ovn_nbdb_api.db_remove.assert_not_called()
 
@@ -1154,15 +1276,15 @@
                          constants.ACTIVE)
         self.assertEqual(status['listeners'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['pools'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.helper.ovn_nbdb_api.db_remove.assert_not_called()
         refresh_vips.assert_called_once_with(
-            self.ovn_lb.uuid, self.ovn_lb.external_ids)
+            self.ovn_lb, self.ovn_lb.external_ids)
 
     @mock.patch.object(ovn_helper.OvnProviderHelper, '_refresh_lb_vips')
     def test_listener_update_no_admin_state_up_or_default_pool_id(
             self, refresh_vips):
         self.listener.pop('admin_state_up')
         self.listener.pop('default_pool_id')
         status = self.helper.listener_update(self.listener)
@@ -1214,15 +1336,15 @@
         self.assertEqual(status['listeners'][0]['operating_status'],
                          constants.OFFLINE)
         self.helper.ovn_nbdb_api.db_remove.assert_called_once_with(
             'Load_Balancer', self.ovn_lb.uuid,
             'external_ids', 'listener_%s' % self.listener_id)
         self.ovn_lb.external_ids.pop('listener_%s' % self.listener_id)
         refresh_vips.assert_called_once_with(
-            self.ovn_lb.uuid, self.ovn_lb.external_ids)
+            self.ovn_lb, self.ovn_lb.external_ids)
 
     @mock.patch.object(ovn_helper.OvnProviderHelper, '_is_lb_empty')
     def test_listener_delete_ovn_lb_not_empty(self, lb_empty):
         lb_empty.return_value = False
         self.helper.listener_delete(self.listener)
         self.helper.ovn_nbdb_api.db_remove.assert_called_once_with(
             'Load_Balancer', self.ovn_lb.uuid,
@@ -1550,34 +1672,45 @@
             'Load_Balancer', self.ovn_lb.uuid,
             'external_ids', 'pool_%s' % self.pool_id)
         self.helper.ovn_nbdb_api.lb_del.assert_called_once_with(
             self.ovn_lb.uuid)
 
     @mock.patch('ovn_octavia_provider.common.clients.get_neutron_client')
     def test_member_create(self, net_cli):
-        net_cli.return_value.show_subnet.side_effect = [
-            idlutils.RowNotFound, idlutils.RowNotFound]
+        net_cli.return_value.show_subnet.side_effect = [idlutils.RowNotFound]
         self.ovn_lb.external_ids = mock.MagicMock()
         status = self.helper.member_create(self.member)
         self.assertEqual(status['loadbalancers'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['pools'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['members'][0]['provisioning_status'],
                          constants.ACTIVE)
+        self.assertEqual(status['members'][0]['operating_status'],
+                         constants.NO_MONITOR)
+        calls = [
+            mock.call.db_clear('Load_Balancer', self.ovn_lb.uuid, 'vips'),
+            mock.call.db_set('Load_Balancer', self.ovn_lb.uuid, ('vips', {}))]
+        self.helper.ovn_nbdb_api.assert_has_calls(calls)
+
+    @mock.patch('ovn_octavia_provider.common.clients.get_neutron_client')
+    def test_member_create_disabled(self, net_cli):
+        net_cli.return_value.show_subnet.side_effect = [idlutils.RowNotFound]
+        self.ovn_lb.external_ids = mock.MagicMock()
         self.member['admin_state_up'] = False
         status = self.helper.member_create(self.member)
         self.assertEqual(status['loadbalancers'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['pools'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['members'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['members'][0]['operating_status'],
                          constants.OFFLINE)
+        self.helper.ovn_nbdb_api.db_clear.assert_not_called()
 
     @mock.patch.object(ovn_helper.OvnProviderHelper, '_find_ovn_lb_by_pool_id')
     @mock.patch.object(ovn_helper.OvnProviderHelper, '_find_lr_of_ls')
     @mock.patch('ovn_octavia_provider.common.clients.get_neutron_client')
     def test_member_create_lb_add_from_lr(self, net_cli, f_lr, folbpi):
         fake_subnet = fakes.FakeSubnet.create_one_subnet()
         net_cli.return_value.show_subnet.return_value = {'subnet': fake_subnet}
@@ -1784,62 +1917,21 @@
         self.helper._get_pool_listeners.return_value = ['listener1']
         status = self.helper.member_update(self.member)
         self.assertEqual(status['listeners'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['listeners'][0]['id'],
                          'listener1')
 
-    @mock.patch.object(ovn_helper.OvnProviderHelper, '_update_member')
-    def test_member_update_exception(self, mock_update_member):
-        mock_update_member.side_effect = [RuntimeError]
+    @mock.patch.object(ovn_helper.OvnProviderHelper, '_find_member_status')
+    def test_member_update_exception(self, mock_find_member_status):
+        mock_find_member_status.side_effect = [TypeError]
         status = self.helper.member_update(self.member)
         self.assertEqual(status['pools'][0]['provisioning_status'],
                          constants.ACTIVE)
 
-    def test_member_update_new_member_line(self):
-        old_member_line = (
-            'member_%s_%s:%s' %
-            (self.member_id, self.member_address,
-             self.member_port))
-        new_member_line = (
-            'member_%s_%s:%s_%s' %
-            (self.member_id, self.member_address,
-             self.member_port, self.member_subnet_id))
-        self.ovn_lb.external_ids.update(
-            {'pool_%s' % self.pool_id: old_member_line})
-        self.helper.member_update(self.member)
-        expected_calls = [
-            mock.call('Load_Balancer', self.ovn_lb.uuid,
-                      ('external_ids', {
-                          'pool_%s' % self.pool_id: new_member_line}))]
-        self.helper.ovn_nbdb_api.db_set.assert_has_calls(
-            expected_calls)
-
-    def test_member_update_new_port(self):
-        new_port = 11
-        member_line = ('member_%s_%s:%s_%s' %
-                       (self.member_id, self.member_address,
-                        new_port, self.member_subnet_id))
-        self.ovn_lb.external_ids.update(
-            {'pool_%s' % self.pool_id: member_line})
-        self.helper.member_update(self.member)
-        new_member_line = (
-            'member_%s_%s:%s_%s' %
-            (self.member_id, self.member_address,
-             self.member_port, self.member_subnet_id))
-        expected_calls = [
-            mock.call('Load_Balancer', self.ovn_lb.uuid,
-                      ('external_ids', {
-                          'pool_%s' % self.pool_id: new_member_line})),
-            mock.call('Load_Balancer', self.ovn_lb.uuid, ('vips', {
-                '10.22.33.4:80': '192.168.2.149:1010',
-                '123.123.123.123:80': '192.168.2.149:1010'}))]
-        self.helper.ovn_nbdb_api.db_set.assert_has_calls(
-            expected_calls)
-
     @mock.patch('ovn_octavia_provider.helper.OvnProviderHelper.'
                 '_refresh_lb_vips')
     def test_member_delete(self, mock_vip_command):
         status = self.helper.member_delete(self.member)
         self.assertEqual(status['loadbalancers'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['pools'][0]['provisioning_status'],
@@ -1861,14 +1953,28 @@
             'pool_' + self.pool_id: member_line})
         status = self.helper.member_delete(self.member)
         self.assertEqual(status['members'][0]['provisioning_status'],
                          constants.DELETED)
         self.assertEqual(status['pools'][0]['provisioning_status'],
                          constants.ACTIVE)
 
+    @mock.patch.object(ovn_helper.OvnProviderHelper, '_find_ovn_lb_by_pool_id')
+    @mock.patch.object(ovn_helper.OvnProviderHelper, '_update_hm_member')
+    def test_member_delete_hm(self, uhm, folbpi):
+        pool_key = 'pool_%s' % self.pool_id
+        self.ovn_hm_lb.external_ids[pool_key] = self.member_line
+        self.ovn_hm_lb.external_ids[ovn_const.OVN_MEMBER_STATUS_KEY] = \
+            '{"%s": "%s"}' % (self.member_id, constants.ONLINE)
+        folbpi.return_value = (pool_key, self.ovn_hm_lb)
+        self.helper.member_delete(self.member)
+        uhm.assert_called_once_with(self.ovn_hm_lb,
+                                    pool_key,
+                                    self.member_address,
+                                    delete=True)
+
     def test_member_delete_none(self):
         self.ovn_lb.external_ids.update({'pool_' + self.pool_id: ''})
         status = self.helper.member_delete(self.member)
         self.assertEqual(status['members'][0]['provisioning_status'],
                          constants.ERROR)
         self.assertEqual(status['pools'][0]['provisioning_status'],
                          constants.ACTIVE)
@@ -3430,42 +3536,49 @@
     def test__get_existing_pool_members_exception(self, folbpi):
         folbpi.return_value = (None, None)
         self.assertRaises(exceptions.DriverError,
                           self.helper._get_existing_pool_members,
                           self.pool_id)
 
     def test__frame_lb_vips(self):
-        ret = self.helper._frame_vip_ips(self.ovn_lb.external_ids)
+        ret = self.helper._frame_vip_ips(self.ovn_lb, self.ovn_lb.external_ids)
         expected = {'10.22.33.4:80': '192.168.2.149:1010',
                     '123.123.123.123:80': '192.168.2.149:1010'}
         self.assertEqual(expected, ret)
 
+    def test__frame_lb_vips_member_offline(self):
+        self.ovn_lb.external_ids[ovn_const.OVN_MEMBER_STATUS_KEY] = \
+            '{"%s": "%s"}' % (self.member_id, constants.OFFLINE)
+        ret = self.helper._frame_vip_ips(self.ovn_lb, self.ovn_lb.external_ids)
+        expected = {}
+        self.assertEqual(expected, ret)
+
     def test__frame_lb_vips_no_vip_fip(self):
         self.ovn_lb.external_ids.pop(ovn_const.LB_EXT_IDS_VIP_FIP_KEY)
-        ret = self.helper._frame_vip_ips(self.ovn_lb.external_ids)
+        ret = self.helper._frame_vip_ips(self.ovn_lb, self.ovn_lb.external_ids)
         expected = {'10.22.33.4:80': '192.168.2.149:1010'}
         self.assertEqual(expected, ret)
 
     def test__frame_lb_vips_disabled(self):
         self.ovn_lb.external_ids['enabled'] = 'False'
-        ret = self.helper._frame_vip_ips(self.ovn_lb.external_ids)
+        ret = self.helper._frame_vip_ips(self.ovn_lb, self.ovn_lb.external_ids)
         self.assertEqual({}, ret)
 
     def test__frame_lb_vips_ipv6(self):
         self.member_address = '2001:db8::1'
         self.member_line = (
             'member_%s_%s:%s_%s' %
             (self.member_id, self.member_address,
              self.member_port, self.member_subnet_id))
         self.ovn_lb.external_ids = {
             ovn_const.LB_EXT_IDS_VIP_KEY: 'fc00::',
             ovn_const.LB_EXT_IDS_VIP_FIP_KEY: '2002::',
             'pool_%s' % self.pool_id: self.member_line,
             'listener_%s' % self.listener_id: '80:pool_%s' % self.pool_id}
-        ret = self.helper._frame_vip_ips(self.ovn_lb.external_ids)
+        ret = self.helper._frame_vip_ips(self.ovn_lb, self.ovn_lb.external_ids)
         expected = {'[2002::]:80': '[2001:db8::1]:1010',
                     '[fc00::]:80': '[2001:db8::1]:1010'}
         self.assertEqual(expected, ret)
 
     def test_check_lb_protocol(self):
         self.ovn_lb.protocol = ['tcp']
         ret = self.helper.check_lb_protocol(self.listener_id, 'udp')
@@ -3492,15 +3605,15 @@
                 '_find_ovn_lbs')
     def test_check_lb_protocol_no_lb(self, fol):
         fol.return_value = None
         ret = self.helper.check_lb_protocol(self.listener_id, 'TCP')
         self.assertFalse(ret)
 
     @mock.patch('ovn_octavia_provider.common.clients.get_neutron_client')
-    @mock.patch.object(ovn_helper.OvnProviderHelper, '_update_hm_members')
+    @mock.patch.object(ovn_helper.OvnProviderHelper, '_update_hm_member')
     @mock.patch.object(ovn_helper.OvnProviderHelper, '_find_ovn_lb_by_pool_id')
     def _test_hm_create(self, protocol, members, fip, folbpi, uhm,
                         net_cli):
         self._get_pool_listeners.stop()
         fake_subnet = fakes.FakeSubnet.create_one_subnet()
         pool_key = 'pool_%s' % self.pool_id
         self.ovn_hm_lb.protocol = [protocol]
@@ -3909,27 +4022,22 @@
                          constants.NO_MONITOR)
         self.assertEqual(status['loadbalancers'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['pools'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['listeners'][0]['provisioning_status'],
                          constants.ACTIVE)
-        expected_clear_calls = [
-            mock.call('Load_Balancer', self.ovn_hm_lb.uuid,
-                      'ip_port_mappings')]
         expected_remove_calls = [
             mock.call('Load_Balancer', self.ovn_hm_lb.uuid, 'health_check',
                       self.ovn_hm.uuid),
             mock.call('Load_Balancer', self.ovn_hm_lb.uuid,
                       'external_ids', ovn_const.LB_EXT_IDS_HMS_KEY)]
         expected_destroy_calls = [
             mock.call('Load_Balancer_Health_Check', self.ovn_hm.uuid)]
         del_hm_port.assert_called_once_with(self.member_subnet_id)
-        self.helper.ovn_nbdb_api.db_clear.assert_has_calls(
-            expected_clear_calls)
         self.helper.ovn_nbdb_api.db_remove.assert_has_calls(
             expected_remove_calls)
         self.helper.ovn_nbdb_api.db_destroy.assert_has_calls(
             expected_destroy_calls)
 
     @mock.patch.object(ovn_helper.OvnProviderHelper, '_clean_up_hm_port')
     def test_hm_delete_without_members_in_pool(self, del_hm_port):
@@ -3945,25 +4053,22 @@
                          constants.NO_MONITOR)
         self.assertEqual(status['loadbalancers'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['pools'][0]['provisioning_status'],
                          constants.ACTIVE)
         self.assertEqual(status['listeners'][0]['provisioning_status'],
                          constants.ACTIVE)
-        expected_clear_calls = [
-            mock.call('Load_Balancer', self.ovn_hm_lb.uuid,
-                      'ip_port_mappings')]
         expected_remove_calls = [
             mock.call('Load_Balancer', self.ovn_hm_lb.uuid, 'health_check',
-                      self.ovn_hm.uuid)]
+                      self.ovn_hm.uuid),
+            mock.call('Load_Balancer', self.ovn_hm_lb.uuid,
+                      'external_ids', ovn_const.LB_EXT_IDS_HMS_KEY)]
         expected_destroy_calls = [
             mock.call('Load_Balancer_Health_Check', self.ovn_hm.uuid)]
         del_hm_port.assert_not_called()
-        self.helper.ovn_nbdb_api.db_clear.assert_has_calls(
-            expected_clear_calls)
         self.helper.ovn_nbdb_api.db_remove.assert_has_calls(
             expected_remove_calls)
         self.helper.ovn_nbdb_api.db_destroy.assert_has_calls(
             expected_destroy_calls)
 
     def test_hm_delete_row_not_found(self):
         self.helper.ovn_nbdb_api.db_list_rows.return_value.\
```

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/PKG-INFO` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ovn-octavia-provider
-Version: 4.0.0.0rc2
+Version: 4.0.1
 Summary: OpenStack Octavia integration with OVN
 Home-page: https://docs.openstack.org/ovn-octavia-provider/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===================================================================
         ovn-octavia-provider - OVN Provider driver for Octavia LoadBalancer
```

### Comparing `ovn-octavia-provider-4.0.0.0rc2/ovn_octavia_provider.egg-info/SOURCES.txt` & `ovn-octavia-provider-4.0.1/ovn_octavia_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/README.rst` & `ovn-octavia-provider-4.0.1/releasenotes/source/README.rst`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/releasenotes/source/conf.py` & `ovn-octavia-provider-4.0.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/requirements.txt` & `ovn-octavia-provider-4.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/roles/configure_functional_tests/tasks/main.yaml` & `ovn-octavia-provider-4.0.1/roles/configure_functional_tests/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/roles/fetch_journal_log/tasks/main.yaml` & `ovn-octavia-provider-4.0.1/roles/fetch_journal_log/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/setup.cfg` & `ovn-octavia-provider-4.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/setup.py` & `ovn-octavia-provider-4.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/test-requirements.txt` & `ovn-octavia-provider-4.0.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/tools/check_unit_test_structure.sh` & `ovn-octavia-provider-4.0.1/tools/check_unit_test_structure.sh`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/tools/coding-checks.sh` & `ovn-octavia-provider-4.0.1/tools/coding-checks.sh`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/tools/generate_config_file_samples.sh` & `ovn-octavia-provider-4.0.1/tools/generate_config_file_samples.sh`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/tools/pip_install_src_modules.sh` & `ovn-octavia-provider-4.0.1/tools/pip_install_src_modules.sh`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/tox.ini` & `ovn-octavia-provider-4.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `ovn-octavia-provider-4.0.0.0rc2/zuul.d/base.yaml` & `ovn-octavia-provider-4.0.1/zuul.d/base.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -39,25 +39,14 @@
       OVN_BUILD_FROM_SOURCE: True
       Q_BUILD_OVS_FROM_GIT: True
       INSTALL_OVN: True
       OVN_BRANCH: v21.06.0
       OVS_BRANCH: "a4b04276ab5934d087669ff2d191a23931335c87"
 
 - job:
-    name: ovn-octavia-provider-functional-master
-    parent: ovn-octavia-provider-functional-base
-    description: Run OVN Octavia provider functional tests - OVN master
-    vars:
-      OVN_BUILD_FROM_SOURCE: True
-      Q_BUILD_OVS_FROM_GIT: True
-      INSTALL_OVN: True
-      OVN_BRANCH: main
-      OVS_BRANCH: master
-
-- job:
     name: ovn-octavia-provider-tempest-base
     parent: devstack-tempest
     abstract: true
     timeout: 7800
     required-projects:
       - openstack/neutron
       - openstack/octavia
@@ -169,18 +158,7 @@
     vars:
       devstack_localrc:
         OVN_BUILD_FROM_SOURCE: True
         Q_BUILD_OVS_FROM_GIT: True
         INSTALL_OVN: True
         OVN_BRANCH: v21.06.0
         OVS_BRANCH: "a4b04276ab5934d087669ff2d191a23931335c87"
-
-- job:
-    name: ovn-octavia-provider-tempest-master
-    parent: ovn-octavia-provider-tempest-base
-    vars:
-      devstack_localrc:
-        OVN_BUILD_FROM_SOURCE: True
-        Q_BUILD_OVS_FROM_GIT: True
-        INSTALL_OVN: True
-        OVN_BRANCH: main
-        OVS_BRANCH: master
```

### Comparing `ovn-octavia-provider-4.0.0.0rc2/zuul.d/project.yaml` & `ovn-octavia-provider-4.0.1/zuul.d/project.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -7,19 +7,15 @@
       - openstack-python3-jobs-neutron
     check:
       jobs:
         - openstack-tox-cover:
             required-projects:
               - openstack/neutron
         - ovn-octavia-provider-functional-release
-        - ovn-octavia-provider-functional-master
         - ovn-octavia-provider-tempest-release
-        - ovn-octavia-provider-tempest-master:
-            voting: false
         - kuryr-kubernetes-tempest-ovn-provider-ovn:
             voting: false
     gate:
       fail-fast: true
       jobs:
         - ovn-octavia-provider-functional-release
-        - ovn-octavia-provider-functional-master
         - ovn-octavia-provider-tempest-release
```

