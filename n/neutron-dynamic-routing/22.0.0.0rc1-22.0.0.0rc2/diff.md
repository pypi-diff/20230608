# Comparing `tmp/neutron-dynamic-routing-22.0.0.0rc1.tar.gz` & `tmp/neutron-dynamic-routing-22.0.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutron-dynamic-routing-22.0.0.0rc1.tar", last modified: Wed Mar  1 09:37:14 2023, max compression
+gzip compressed data, was "neutron-dynamic-routing-22.0.0.0rc2.tar", last modified: Thu Mar 16 20:26:31 2023, max compression
```

## Comparing `neutron-dynamic-routing-22.0.0.0rc1.tar` & `neutron-dynamic-routing-22.0.0.0rc2.tar`

### file list

```diff
@@ -1,245 +1,246 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.638467 neutron-dynamic-routing-22.0.0.0rc1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3469 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/.pylintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1649 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8664 2023-03-01 09:37:14.000000 neutron-dynamic-routing-22.0.0.0rc1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30059 2023-03-01 09:37:14.000000 neutron-dynamic-routing-22.0.0.0rc1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2021 2023-03-01 09:37:14.638467 neutron-dynamic-routing-22.0.0.0rc1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/TESTING.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.610466 neutron-dynamic-routing-22.0.0.0rc1/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/devstack/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.610466 neutron-dynamic-routing-22.0.0.0rc1/devstack/lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2962 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/devstack/lib/dr
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      608 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2439 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.610466 neutron-dynamic-routing-22.0.0.0rc1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.610466 neutron-dynamic-routing-22.0.0.0rc1/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.610466 neutron-dynamic-routing-22.0.0.0rc1/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.614467 neutron-dynamic-routing-22.0.0.0rc1/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5925 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/admin/agent-scheduler.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7645 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/admin/bgp-speaker.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5523 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/admin/route-advertisement.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5770 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/admin/system-design.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.614467 neutron-dynamic-routing-22.0.0.0rc1/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4507 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/cli/bgp-peer.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6831 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/cli/bgp-speaker.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3336 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/cli/dynamic-routing-agent.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4174 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.614467 neutron-dynamic-routing-22.0.0.0rc1/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/configuration/bgp_dragent.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/configuration/policy-sample.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/configuration/policy.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.614467 neutron-dynamic-routing-22.0.0.0rc1/doc/source/configuration/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/configuration/samples/bgp_dragent.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.614467 neutron-dynamic-routing-22.0.0.0rc1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1003 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4697 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/contributor/dragent-drivers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1591 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30631 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/contributor/testing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1585 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.614467 neutron-dynamic-routing-22.0.0.0rc1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1164 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.614467 neutron-dynamic-routing-22.0.0.0rc1/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.614467 neutron-dynamic-routing-22.0.0.0rc1/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/etc/README.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.614467 neutron-dynamic-routing-22.0.0.0rc1/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/etc/oslo-config-generator/bgp_dragent.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.614467 neutron-dynamic-routing-22.0.0.0rc1/etc/oslo-policy-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/etc/oslo-policy-generator/policy.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.618466 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1371 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/_i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.618466 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.618466 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/rpc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/rpc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.618466 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/rpc/agentnotifiers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/rpc/agentnotifiers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5074 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/rpc/agentnotifiers/bgp_dr_rpc_agent_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.618466 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/rpc/callbacks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/rpc/callbacks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      601 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/rpc/callbacks/resources.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.618466 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/rpc/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/rpc/handlers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2485 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/rpc/handlers/bgp_speaker_rpc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.618466 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/cmd/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.618466 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/cmd/eventlet/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/cmd/eventlet/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.618466 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/cmd/eventlet/agents/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/cmd/eventlet/agents/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/cmd/eventlet/agents/bgp_dragent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.622467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    62247 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/bgp_db.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12495 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/bgp_dragentscheduler_db.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.622467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.622467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2560 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.622467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/CONTRACT_HEAD
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/EXPAND_HEAD
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.602466 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.622467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/contract/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3316 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/contract/4cf8bc3edb66_rename_tenant_to_project.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      977 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/contract/61cc795e43e8_initial.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.622467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/expand/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/expand/f399fa0f5f25_initial.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.602466 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/queens/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.622467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/queens/contract/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1198 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/queens/contract/a589fdb5724c_change_size_of_as_number.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/start_neutron_dynamic_routing.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.622467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/models/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/models/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/models/head.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.622467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2869 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/extensions/bgp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/extensions/bgp_4byte_asn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5448 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/extensions/bgp_dragentscheduler.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.626467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      723 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1983 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/policies/bgp_dragent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1788 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/policies/bgp_peer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3312 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/policies/bgp_speaker.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.626467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.626467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.626467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31901 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/bgp_dragent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.626467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/driver/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/driver/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6093 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/driver/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2070 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/driver/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.626467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/driver/os_ken/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/driver/os_ken/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9653 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/driver/os_ken/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3159 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/driver/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1839 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/entry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21042 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/bgp_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.626467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      993 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/common/opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.626467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/scheduler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/scheduler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9659 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/scheduler/bgp_dragent_scheduler.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.626467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.630467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/common/helpers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.630467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.630467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/functional/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/functional/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.630467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/functional/services/bgp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/functional/services/bgp/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.630467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/functional/services/bgp/scheduler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/functional/services/bgp/scheduler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8261 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/functional/services/bgp/scheduler/test_bgp_dragent_scheduler.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.630467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.630467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.630467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/api/rpc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/api/rpc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.630467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/api/rpc/agentnotifiers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/api/rpc/agentnotifiers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3886 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/api/rpc/agentnotifiers/test_bgp_dr_rpc_agent_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.630467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/api/rpc/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/api/rpc/handlers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1742 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/api/rpc/handlers/test_bgp_speaker_rpc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.630467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    81810 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/db/test_bgp_db.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8827 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/db/test_bgp_dragentscheduler_db.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.630467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.630467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.630467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/agent/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34173 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/agent/test_bgp_dragent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.634467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/driver/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/driver/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.634467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/driver/os_ken/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/driver/os_ken/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15204 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/driver/os_ken/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7770 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/driver/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.634467 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/scheduler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/scheduler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14946 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/scheduler/test_bgp_dragent_scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6611 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/test_bgp_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.618466 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2021 2023-03-01 09:37:14.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8120 2023-03-01 09:37:14.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-01 09:37:14.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2023-03-01 09:37:14.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-01 09:37:14.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-01 09:37:14.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-03-01 09:37:14.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2023-03-01 09:37:14.000000 neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.606466 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.634467 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/notes/add-static-scheduler-a3b0f54b964ae306.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/notes/drop-py27-support-795303ca12cccd34.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/notes/drop-python-3-6-and-3-7-efc3424202bf3f90.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/notes/dvr-aware-announcements-24bfcb8fee87161d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/notes/mp-bgp-support-d408e8569e94d07f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/notes/rehome-dynamic-routing-apidef-d656e3273baac4e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/notes/rpc-workers-4941f3b9136418df.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/notes/sqlalchemy-20-abaa3d2895131ab4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/notes/static-scheduler-2288b8173f9357a6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/notes/support-4byte-asn-d89d7100c0890ebf.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.638467 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.638467 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.638467 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9140 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1445 2023-03-01 09:37:14.638467 neutron-dynamic-routing-22.0.0.0rc1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      647 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-01 09:37:14.638467 neutron-dynamic-routing-22.0.0.0rc1/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1616 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/tools/check_unit_test_structure.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      196 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/tools/clean.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      800 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/tools/generate_config_file_samples.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4048 2023-03-01 09:36:49.000000 neutron-dynamic-routing-22.0.0.0rc1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.064034 neutron-dynamic-routing-22.0.0.0rc2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3469 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1649 2023-03-16 20:26:04.000000 neutron-dynamic-routing-22.0.0.0rc2/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8664 2023-03-16 20:26:30.000000 neutron-dynamic-routing-22.0.0.0rc2/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30226 2023-03-16 20:26:30.000000 neutron-dynamic-routing-22.0.0.0rc2/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2021 2023-03-16 20:26:31.068035 neutron-dynamic-routing-22.0.0.0rc2/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/TESTING.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.028025 neutron-dynamic-routing-22.0.0.0rc2/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/devstack/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.028025 neutron-dynamic-routing-22.0.0.0rc2/devstack/lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2962 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/devstack/lib/dr
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      608 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2439 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.032026 neutron-dynamic-routing-22.0.0.0rc2/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.032026 neutron-dynamic-routing-22.0.0.0rc2/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.032026 neutron-dynamic-routing-22.0.0.0rc2/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.032026 neutron-dynamic-routing-22.0.0.0rc2/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5925 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/admin/agent-scheduler.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7645 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/admin/bgp-speaker.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5523 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/admin/route-advertisement.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5770 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/admin/system-design.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.032026 neutron-dynamic-routing-22.0.0.0rc2/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4507 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/cli/bgp-peer.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6831 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/cli/bgp-speaker.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3336 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/cli/dynamic-routing-agent.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4174 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.032026 neutron-dynamic-routing-22.0.0.0rc2/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/configuration/bgp_dragent.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/configuration/policy-sample.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/configuration/policy.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.036027 neutron-dynamic-routing-22.0.0.0rc2/doc/source/configuration/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/configuration/samples/bgp_dragent.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.036027 neutron-dynamic-routing-22.0.0.0rc2/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1003 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4697 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/contributor/dragent-drivers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1591 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30631 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/contributor/testing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1585 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.036027 neutron-dynamic-routing-22.0.0.0rc2/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1164 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.036027 neutron-dynamic-routing-22.0.0.0rc2/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.036027 neutron-dynamic-routing-22.0.0.0rc2/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/etc/README.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.036027 neutron-dynamic-routing-22.0.0.0rc2/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/etc/oslo-config-generator/bgp_dragent.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.036027 neutron-dynamic-routing-22.0.0.0rc2/etc/oslo-policy-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/etc/oslo-policy-generator/policy.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.036027 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1371 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.040028 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.040028 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/rpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/rpc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.040028 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/rpc/agentnotifiers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/rpc/agentnotifiers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5074 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/rpc/agentnotifiers/bgp_dr_rpc_agent_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.040028 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/rpc/callbacks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/rpc/callbacks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      601 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/rpc/callbacks/resources.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.040028 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/rpc/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/rpc/handlers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2485 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/rpc/handlers/bgp_speaker_rpc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.040028 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/cmd/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.040028 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/cmd/eventlet/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/cmd/eventlet/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.040028 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/cmd/eventlet/agents/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/cmd/eventlet/agents/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/cmd/eventlet/agents/bgp_dragent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.044029 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    62247 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/bgp_db.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12495 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/bgp_dragentscheduler_db.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.044029 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.044029 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2560 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.044029 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/CONTRACT_HEAD
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/EXPAND_HEAD
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.020023 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.044029 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/contract/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3316 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/contract/4cf8bc3edb66_rename_tenant_to_project.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      977 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/contract/61cc795e43e8_initial.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.044029 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/expand/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/expand/f399fa0f5f25_initial.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.020023 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/queens/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.044029 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/queens/contract/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1198 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/queens/contract/a589fdb5724c_change_size_of_as_number.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/start_neutron_dynamic_routing.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.044029 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/models/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/models/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/models/head.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.048030 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2869 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/extensions/bgp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/extensions/bgp_4byte_asn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5448 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/extensions/bgp_dragentscheduler.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.048030 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      723 2023-03-16 20:26:04.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1983 2023-03-16 20:26:04.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/policies/bgp_dragent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1788 2023-03-16 20:26:04.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/policies/bgp_peer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3312 2023-03-16 20:26:04.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/policies/bgp_speaker.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.048030 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.048030 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.048030 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31901 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/bgp_dragent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.052031 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/driver/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/driver/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6093 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/driver/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2070 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/driver/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.052031 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/driver/os_ken/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/driver/os_ken/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9653 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/driver/os_ken/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3159 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/driver/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1839 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/entry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21042 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/bgp_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.052031 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      993 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/common/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.052031 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/scheduler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/scheduler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9659 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/scheduler/bgp_dragent_scheduler.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.052031 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.052031 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/common/helpers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.052031 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.052031 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/functional/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/functional/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.052031 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/functional/services/bgp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/functional/services/bgp/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.052031 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/functional/services/bgp/scheduler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/functional/services/bgp/scheduler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8261 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/functional/services/bgp/scheduler/test_bgp_dragent_scheduler.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.052031 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.056032 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.056032 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/api/rpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/api/rpc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.056032 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/api/rpc/agentnotifiers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/api/rpc/agentnotifiers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3886 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/api/rpc/agentnotifiers/test_bgp_dr_rpc_agent_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.056032 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/api/rpc/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/api/rpc/handlers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1742 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/api/rpc/handlers/test_bgp_speaker_rpc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.056032 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    81810 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/db/test_bgp_db.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8827 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/db/test_bgp_dragentscheduler_db.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.056032 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.056032 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.056032 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/agent/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34173 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/agent/test_bgp_dragent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.056032 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/driver/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/driver/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.060033 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/driver/os_ken/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/driver/os_ken/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15204 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/driver/os_ken/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7770 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/driver/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.060033 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/scheduler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/scheduler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14946 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/scheduler/test_bgp_dragent_scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6611 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/test_bgp_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.040028 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2021 2023-03-16 20:26:30.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8191 2023-03-16 20:26:31.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-16 20:26:30.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2023-03-16 20:26:30.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-16 20:26:30.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-16 20:26:30.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-03-16 20:26:30.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2023-03-16 20:26:30.000000 neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.024024 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.060033 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/notes/add-static-scheduler-a3b0f54b964ae306.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/notes/drop-py27-support-795303ca12cccd34.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/notes/drop-python-3-6-and-3-7-efc3424202bf3f90.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/notes/dvr-aware-announcements-24bfcb8fee87161d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/notes/fix-address-scope-calculation-c8ac84662a6547bd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/notes/mp-bgp-support-d408e8569e94d07f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/notes/rehome-dynamic-routing-apidef-d656e3273baac4e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/notes/rpc-workers-4941f3b9136418df.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/notes/sqlalchemy-20-abaa3d2895131ab4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/notes/static-scheduler-2288b8173f9357a6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/notes/support-4byte-asn-d89d7100c0890ebf.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.064034 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.064034 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.064034 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9140 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-03-16 20:26:04.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1445 2023-03-16 20:26:31.068035 neutron-dynamic-routing-22.0.0.0rc2/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      647 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-16 20:26:31.064034 neutron-dynamic-routing-22.0.0.0rc2/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1616 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/tools/check_unit_test_structure.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      196 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/tools/clean.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      800 2023-03-16 20:26:03.000000 neutron-dynamic-routing-22.0.0.0rc2/tools/generate_config_file_samples.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4048 2023-03-16 20:26:04.000000 neutron-dynamic-routing-22.0.0.0rc2/tox.ini
```

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/.pylintrc` & `neutron-dynamic-routing-22.0.0.0rc2/.pylintrc`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/.zuul.yaml` & `neutron-dynamic-routing-22.0.0.0rc2/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/AUTHORS` & `neutron-dynamic-routing-22.0.0.0rc2/AUTHORS`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/ChangeLog` & `neutron-dynamic-routing-22.0.0.0rc2/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+22.0.0.0rc2
+-----------
+
+* Add a reno for the fixed address scope calculation
+* Update TOX\_CONSTRAINTS\_FILE for stable/2023.1
+* Update .gitreview for stable/2023.1
+
 22.0.0.0rc1
 -----------
 
 * Use SLQAlchemy ORM "relationship" instead of "relation"
 * Delete empty reno branches
 * Add oslo.log to config generator
 * Fix for tox4.0
```

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/LICENSE` & `neutron-dynamic-routing-22.0.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/PKG-INFO` & `neutron-dynamic-routing-22.0.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: neutron-dynamic-routing
-Version: 22.0.0.0rc1
+Version: 22.0.0.0rc2
 Summary: Neutron Dynamic Routing
 Home-page: https://docs.openstack.org/neutron-dynamic-routing/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Team and repository tags
         ========================
```

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/README.rst` & `neutron-dynamic-routing-22.0.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/devstack/README.rst` & `neutron-dynamic-routing-22.0.0.0rc2/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/devstack/lib/dr` & `neutron-dynamic-routing-22.0.0.0rc2/devstack/lib/dr`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/devstack/plugin.sh` & `neutron-dynamic-routing-22.0.0.0rc2/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/devstack/settings` & `neutron-dynamic-routing-22.0.0.0rc2/devstack/settings`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/admin/agent-scheduler.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/admin/agent-scheduler.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/admin/bgp-speaker.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/admin/bgp-speaker.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/admin/index.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/admin/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/admin/route-advertisement.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/admin/route-advertisement.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/admin/system-design.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/admin/system-design.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/cli/bgp-peer.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/cli/bgp-peer.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/cli/bgp-speaker.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/cli/bgp-speaker.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/cli/dynamic-routing-agent.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/cli/dynamic-routing-agent.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/cli/index.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/cli/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/conf.py` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/configuration/index.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/configuration/policy-sample.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/configuration/policy-sample.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/contributor/contributing.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/contributor/dragent-drivers.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/contributor/dragent-drivers.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/contributor/index.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/contributor/testing.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/contributor/testing.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/index.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/install/index.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/doc/source/reference/index.rst` & `neutron-dynamic-routing-22.0.0.0rc2/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/__init__.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/__init__.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/_i18n.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/_i18n.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/rpc/agentnotifiers/bgp_dr_rpc_agent_api.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/rpc/agentnotifiers/bgp_dr_rpc_agent_api.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/rpc/callbacks/resources.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/rpc/callbacks/resources.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/api/rpc/handlers/bgp_speaker_rpc.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/api/rpc/handlers/bgp_speaker_rpc.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/cmd/eventlet/__init__.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/cmd/eventlet/__init__.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/cmd/eventlet/agents/bgp_dragent.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/cmd/eventlet/agents/bgp_dragent.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/bgp_db.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/bgp_db.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/bgp_dragentscheduler_db.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/bgp_dragentscheduler_db.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/env.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/env.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/script.py.mako` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/contract/4cf8bc3edb66_rename_tenant_to_project.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/contract/4cf8bc3edb66_rename_tenant_to_project.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/contract/61cc795e43e8_initial.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/contract/61cc795e43e8_initial.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/expand/f399fa0f5f25_initial.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/newton/expand/f399fa0f5f25_initial.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/queens/contract/a589fdb5724c_change_size_of_as_number.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/queens/contract/a589fdb5724c_change_size_of_as_number.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/alembic_migrations/versions/start_neutron_dynamic_routing.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/alembic_migrations/versions/start_neutron_dynamic_routing.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/db/migration/models/head.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/db/migration/models/head.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/extensions/bgp.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/extensions/bgp.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/extensions/bgp_4byte_asn.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/extensions/bgp_4byte_asn.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/extensions/bgp_dragentscheduler.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/extensions/bgp_dragentscheduler.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/policies/__init__.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/policies/base.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/policies/base.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/policies/bgp_dragent.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/policies/bgp_dragent.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/policies/bgp_peer.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/policies/bgp_peer.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/policies/bgp_speaker.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/policies/bgp_speaker.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/bgp_dragent.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/bgp_dragent.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/config.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/config.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/driver/base.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/driver/base.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/driver/exceptions.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/driver/exceptions.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/driver/os_ken/driver.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/driver/os_ken/driver.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/driver/utils.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/driver/utils.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/agent/entry.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/agent/entry.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/bgp_plugin.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/bgp_plugin.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/common/constants.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/common/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/common/opts.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/common/opts.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/services/bgp/scheduler/bgp_dragent_scheduler.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/services/bgp/scheduler/bgp_dragent_scheduler.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/common/helpers.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/common/helpers.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/functional/services/bgp/scheduler/test_bgp_dragent_scheduler.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/functional/services/bgp/scheduler/test_bgp_dragent_scheduler.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/api/rpc/agentnotifiers/test_bgp_dr_rpc_agent_api.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/api/rpc/agentnotifiers/test_bgp_dr_rpc_agent_api.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/api/rpc/handlers/test_bgp_speaker_rpc.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/api/rpc/handlers/test_bgp_speaker_rpc.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/db/test_bgp_db.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/db/test_bgp_db.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/db/test_bgp_dragentscheduler_db.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/db/test_bgp_dragentscheduler_db.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/agent/test_bgp_dragent.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/agent/test_bgp_dragent.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/driver/os_ken/test_driver.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/driver/os_ken/test_driver.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/driver/test_utils.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/driver/test_utils.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/scheduler/test_bgp_dragent_scheduler.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/scheduler/test_bgp_dragent_scheduler.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/tests/unit/services/bgp/test_bgp_plugin.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/tests/unit/services/bgp/test_bgp_plugin.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing/version.py` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing/version.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing.egg-info/PKG-INFO` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: neutron-dynamic-routing
-Version: 22.0.0.0rc1
+Version: 22.0.0.0rc2
 Summary: Neutron Dynamic Routing
 Home-page: https://docs.openstack.org/neutron-dynamic-routing/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Team and repository tags
         ========================
```

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing.egg-info/SOURCES.txt` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,15 @@
 neutron_dynamic_routing/tests/unit/services/bgp/scheduler/__init__.py
 neutron_dynamic_routing/tests/unit/services/bgp/scheduler/test_bgp_dragent_scheduler.py
 releasenotes/notes/.placeholder
 releasenotes/notes/add-static-scheduler-a3b0f54b964ae306.yaml
 releasenotes/notes/drop-py27-support-795303ca12cccd34.yaml
 releasenotes/notes/drop-python-3-6-and-3-7-efc3424202bf3f90.yaml
 releasenotes/notes/dvr-aware-announcements-24bfcb8fee87161d.yaml
+releasenotes/notes/fix-address-scope-calculation-c8ac84662a6547bd.yaml
 releasenotes/notes/mp-bgp-support-d408e8569e94d07f.yaml
 releasenotes/notes/rehome-dynamic-routing-apidef-d656e3273baac4e8.yaml
 releasenotes/notes/rpc-workers-4941f3b9136418df.yaml
 releasenotes/notes/sqlalchemy-20-abaa3d2895131ab4.yaml
 releasenotes/notes/static-scheduler-2288b8173f9357a6.yaml
 releasenotes/notes/support-4byte-asn-d89d7100c0890ebf.yaml
 releasenotes/source/README.rst
```

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/neutron_dynamic_routing.egg-info/entry_points.txt` & `neutron-dynamic-routing-22.0.0.0rc2/neutron_dynamic_routing.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/README.rst` & `neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/releasenotes/source/conf.py` & `neutron-dynamic-routing-22.0.0.0rc2/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/requirements.txt` & `neutron-dynamic-routing-22.0.0.0rc2/requirements.txt`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/setup.cfg` & `neutron-dynamic-routing-22.0.0.0rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/setup.py` & `neutron-dynamic-routing-22.0.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/test-requirements.txt` & `neutron-dynamic-routing-22.0.0.0rc2/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/tools/check_unit_test_structure.sh` & `neutron-dynamic-routing-22.0.0.0rc2/tools/check_unit_test_structure.sh`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/tools/generate_config_file_samples.sh` & `neutron-dynamic-routing-22.0.0.0rc2/tools/generate_config_file_samples.sh`

 * *Files identical despite different names*

### Comparing `neutron-dynamic-routing-22.0.0.0rc1/tox.ini` & `neutron-dynamic-routing-22.0.0.0rc2/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [testenv]
 setenv = VIRTUAL_ENV={envdir}
          OS_LOG_CAPTURE={env:OS_LOG_CAPTURE:true}
          OS_STDOUT_CAPTURE={env:OS_STDOUT_CAPTURE:true}
          OS_STDERR_CAPTURE={env:OS_STDERR_CAPTURE:true}
          PYTHONWARNINGS=default::DeprecationWarning
 usedevelop = True
-deps = -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+deps = -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.1}
        -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
 allowlist_externals =
   find
   bash
 commands =
   find . -type f -name "*.py[c|o]" -delete
@@ -50,15 +50,15 @@
   coverage html -d cover
   coverage xml -o cover/coverage.xml
 
 [testenv:venv]
 commands = {posargs}
 
 [testenv:docs]
-deps = -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+deps = -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2023.1}
        -r{toxinidir}/doc/requirements.txt
 commands =
   sphinx-build -W -b html doc/source doc/build/html
 
 [testenv:pdf-docs]
 envdir = {toxworkdir}/docs
 deps = {[testenv:docs]deps}
```

