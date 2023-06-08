# Comparing `tmp/scinode-0.3.0.tar.gz` & `tmp/scinode-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scinode-0.3.0.tar", last modified: Sun May  7 14:24:54 2023, max compression
+gzip compressed data, was "scinode-0.3.1.tar", last modified: Thu Jun  8 03:16:10 2023, max compression
```

## Comparing `scinode-0.3.0.tar` & `scinode-0.3.1.tar`

### file list

```diff
@@ -1,221 +1,226 @@
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.639503 scinode-0.3.0/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1064 2022-12-06 13:50:07.000000 scinode-0.3.0/LICENSE
--rw-rw-r--   0 xing      (1000) xing      (1000)      444 2023-05-02 12:47:10.000000 scinode-0.3.0/MANIFEST.in
--rw-rw-r--   0 xing      (1000) xing      (1000)     1871 2023-05-07 14:24:54.639503 scinode-0.3.0/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)     1537 2023-05-02 12:47:10.000000 scinode-0.3.0/README.md
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.623503 scinode-0.3.0/scinode/
--rw-rw-r--   0 xing      (1000) xing      (1000)      392 2023-04-17 08:55:44.000000 scinode-0.3.0/scinode/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.623503 scinode-0.3.0/scinode/app/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3661 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/app.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.623503 scinode-0.3.0/scinode/app/blueprints/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/blueprints/component/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/component/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     6676 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/component/component.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/blueprints/component/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)     7092 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/component/templates/component_editor.html
--rw-rw-r--   0 xing      (1000) xing      (1000)      594 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/component/templates/component_exporter.html
--rw-rw-r--   0 xing      (1000) xing      (1000)      359 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/component/templates/component_importer.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     1613 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/component/templates/component_table.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     1474 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/component/utils.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/blueprints/config/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/config/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2644 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/config/config.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/blueprints/config/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)     4703 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/config/templates/config.html
--rw-rw-r--   0 xing      (1000) xing      (1000)      739 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/config/templates/daemon_logfile.html
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/blueprints/data/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/data/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2331 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/data/data.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/blueprints/data/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)      800 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/data/templates/data_table.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     1265 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/data/templates/data_viewer.html
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/blueprints/node/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/node/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3505 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/node/node.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/blueprints/node/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1717 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/node/templates/node_table.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     2715 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/node/templates/node_viewer.html
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/blueprints/nodetree/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/nodetree/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     7747 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/nodetree/nodetree.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/blueprints/nodetree/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)     3823 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/nodetree/templates/nodetree_editor.html
--rw-rw-r--   0 xing      (1000) xing      (1000)      605 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/nodetree/templates/nodetree_exporter.html
--rw-rw-r--   0 xing      (1000) xing      (1000)      359 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/nodetree/templates/nodetree_importer.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     2079 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/nodetree/templates/nodetree_table.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     2930 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/nodetree/templates/nodetree_viewer.html
--rw-rw-r--   0 xing      (1000) xing      (1000)      249 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/nodetree/templates/tab-description.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     6594 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/nodetree/templates/tab-graph-sidebar.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     1545 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/nodetree/templates/tab-graph.html
--rw-rw-r--   0 xing      (1000) xing      (1000)      789 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/nodetree/templates/tab-table.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     1036 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/nodetree/templates/tab.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     1816 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/nodetree/utils.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/blueprints/scheduler/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/scheduler/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      657 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/scheduler/scheduler.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/blueprints/scheduler/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/scheduler/templates/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/blueprints/template/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/template/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2361 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/template/template.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/blueprints/template/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1757 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/blueprints/template/templates/template_table.html
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/cli/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/cli/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.627503 scinode-0.3.0/scinode/app/cli/commands/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/cli/commands/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1451 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/cli/commands/plugin.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      532 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/cli/commands/web.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     8299 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/db.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      432 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/init_data.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.631503 scinode-0.3.0/scinode/app/static/
--rw-rw-r--   0 xing      (1000) xing      (1000)      345 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/static/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.631503 scinode-0.3.0/scinode/app/static/__pycache__/
--rw-rw-r--   0 xing      (1000) xing      (1000)      555 2023-05-05 04:32:32.000000 scinode-0.3.0/scinode/app/static/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 xing      (1000) xing      (1000)    14636 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/static/component_editor.js
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.631503 scinode-0.3.0/scinode/app/static/components/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/static/components/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.631503 scinode-0.3.0/scinode/app/static/components/__pycache__/
--rw-rw-r--   0 xing      (1000) xing      (1000)      170 2023-05-01 07:20:25.000000 scinode-0.3.0/scinode/app/static/components/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 xing      (1000) xing      (1000)    21043 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/static/components/app_components.js
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.631503 scinode-0.3.0/scinode/app/static/controls/
--rw-rw-r--   0 xing      (1000) xing      (1000)    21092 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/static/controls/app_controls.js
--rw-rw-r--   0 xing      (1000) xing      (1000)      950 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/static/init_editor.js
--rw-rw-r--   0 xing      (1000) xing      (1000)     5620 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/static/json_components.js
--rw-rw-r--   0 xing      (1000) xing      (1000)    22329 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/static/logo.png
--rw-rw-r--   0 xing      (1000) xing      (1000)    10686 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/static/nodetree_editor.js
--rw-rw-r--   0 xing      (1000) xing      (1000)     1572 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/static/nodetree_node_table.js
--rw-rw-r--   0 xing      (1000) xing      (1000)     7589 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/static/scinode_components.js
--rw-rw-r--   0 xing      (1000) xing      (1000)     2067 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/static/scinode_editor.js
--rw-rw-r--   0 xing      (1000) xing      (1000)      759 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/static/sidebar.js
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.631503 scinode-0.3.0/scinode/app/static/sockets/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1276 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/static/sockets/app_sockets.js
--rw-rw-r--   0 xing      (1000) xing      (1000)     3501 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/static/styles.css
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.631503 scinode-0.3.0/scinode/app/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)     3713 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/templates/base.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     2371 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/templates/base_editor.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     2065 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/templates/index.html
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.631503 scinode-0.3.0/scinode/app/utils/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1020 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/utils/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     6640 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/app/utils/rete_adapter.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.631503 scinode-0.3.0/scinode/cli/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.0/scinode/cli/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.631503 scinode-0.3.0/scinode/cli/commands/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.0/scinode/cli/commands/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1756 2023-04-17 08:55:44.000000 scinode-0.3.0/scinode/cli/commands/data.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      665 2023-04-18 11:52:21.000000 scinode-0.3.0/scinode/cli/commands/mq.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    12342 2023-04-17 08:55:44.000000 scinode-0.3.0/scinode/cli/commands/node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     8278 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/cli/commands/nodetree.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2738 2023-04-03 03:09:25.000000 scinode-0.3.0/scinode/cli/commands/profile.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3478 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/cli/commands/scheduler.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1309 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/cli/commands/shell.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     8638 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/cli/commands/worker.py
--rwxrwxr-x   0 xing      (1000) xing      (1000)     5084 2023-05-07 13:38:33.000000 scinode-0.3.0/scinode/cli/main.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.631503 scinode-0.3.0/scinode/core/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-03-20 09:18:35.000000 scinode-0.3.0/scinode/core/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    10601 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/core/collection.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1381 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/core/executor.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3596 2023-04-17 08:55:44.000000 scinode-0.3.0/scinode/core/link.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    22169 2023-05-07 13:38:33.000000 scinode-0.3.0/scinode/core/node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3207 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/core/property.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4454 2023-04-17 08:55:44.000000 scinode-0.3.0/scinode/core/socket.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.631503 scinode-0.3.0/scinode/daemon/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.0/scinode/daemon/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4635 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/daemon/daemon.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1681 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/daemon/scheduler.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      440 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/daemon/scheduler_config.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     5472 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/daemon/worker.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2836 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/daemon/worker_config.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.635503 scinode-0.3.0/scinode/database/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.0/scinode/database/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      531 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/database/client.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2102 2023-04-17 08:55:44.000000 scinode-0.3.0/scinode/database/data.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1519 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/database/db.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3657 2023-04-21 14:26:57.000000 scinode-0.3.0/scinode/database/node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     8208 2023-04-17 08:55:44.000000 scinode-0.3.0/scinode/database/nodetree.py
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.0/scinode/database/utils.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4203 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/database/worker.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.635503 scinode-0.3.0/scinode/engine/
--rw-rw-r--   0 xing      (1000) xing      (1000)       99 2023-03-20 09:18:35.000000 scinode-0.3.0/scinode/engine/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.635503 scinode-0.3.0/scinode/engine/celery/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-03-01 08:01:27.000000 scinode-0.3.0/scinode/engine/celery/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      154 2023-03-01 08:01:27.000000 scinode-0.3.0/scinode/engine/celery/app.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      708 2023-03-01 08:01:27.000000 scinode-0.3.0/scinode/engine/celery/base.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      297 2023-03-01 08:01:27.000000 scinode-0.3.0/scinode/engine/celery/celery_config.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     5694 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/engine/celery/tasks.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2251 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/engine/celery/worker.py
--rw-rw-r--   0 xing      (1000) xing      (1000)       32 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/engine/config.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4228 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/engine/mq.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     9769 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/engine/node_engine.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    16275 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/engine/nodetree_engine.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    12224 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/engine/nodetree_launch.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    12484 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/engine/scheduler.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1703 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/engine/send_to_queue.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     6482 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/engine/worker.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.635503 scinode-0.3.0/scinode/executors/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.0/scinode/executors/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     5044 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/executors/built_in.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.635503 scinode-0.3.0/scinode/executors/controls/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.0/scinode/executors/controls/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4558 2023-04-17 08:55:44.000000 scinode-0.3.0/scinode/executors/controls/scatter_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1414 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/executors/controls/switch_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1900 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/executors/controls/update_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1125 2023-03-20 09:18:35.000000 scinode-0.3.0/scinode/executors/python.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1980 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/executors/test.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.635503 scinode-0.3.0/scinode/nodes/
--rw-rw-r--   0 xing      (1000) xing      (1000)      122 2022-12-23 08:17:58.000000 scinode-0.3.0/scinode/nodes/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      907 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/nodes/bash_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     5623 2023-02-14 21:05:04.000000 scinode-0.3.0/scinode/nodes/build_node_from_database.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1044 2023-04-23 12:13:12.000000 scinode-0.3.0/scinode/nodes/built_in.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1954 2023-04-17 08:55:44.000000 scinode-0.3.0/scinode/nodes/control.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1289 2023-02-14 20:38:16.000000 scinode-0.3.0/scinode/nodes/node_from_database.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    23457 2023-04-03 03:09:25.000000 scinode-0.3.0/scinode/nodes/numpy_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     7557 2023-04-03 03:09:25.000000 scinode-0.3.0/scinode/nodes/python_builtin.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     8752 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/nodes/test.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2024 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/nodes/test_node_group.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    14631 2023-05-07 13:38:33.000000 scinode-0.3.0/scinode/nodetree.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.635503 scinode-0.3.0/scinode/orm/
--rw-rw-r--   0 xing      (1000) xing      (1000)     5758 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/orm/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      648 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/orm/data.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     8774 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/orm/db_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    11826 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/orm/db_nodetree.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1658 2023-03-20 09:18:35.000000 scinode-0.3.0/scinode/orm/db_property.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2178 2023-03-20 09:18:35.000000 scinode-0.3.0/scinode/orm/db_socket.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4765 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/orm/node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2527 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/orm/nodetree.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.635503 scinode-0.3.0/scinode/profile/
--rw-rw-r--   0 xing      (1000) xing      (1000)       51 2023-01-14 05:41:38.000000 scinode-0.3.0/scinode/profile/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3073 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/profile/base_config.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     5076 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/profile/profile.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.635503 scinode-0.3.0/scinode/properties/
--rw-rw-r--   0 xing      (1000) xing      (1000)      140 2022-12-23 08:17:58.000000 scinode-0.3.0/scinode/properties/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    11696 2023-04-03 03:09:25.000000 scinode-0.3.0/scinode/properties/built_in.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.635503 scinode-0.3.0/scinode/serialization/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-02-10 18:56:33.000000 scinode-0.3.0/scinode/serialization/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1595 2023-03-20 09:18:35.000000 scinode-0.3.0/scinode/serialization/built_in.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.635503 scinode-0.3.0/scinode/sockets/
--rw-rw-r--   0 xing      (1000) xing      (1000)      128 2022-12-23 08:17:58.000000 scinode-0.3.0/scinode/sockets/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2502 2023-04-17 08:55:44.000000 scinode-0.3.0/scinode/sockets/built_in.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.639503 scinode-0.3.0/scinode/utils/
--rw-rw-r--   0 xing      (1000) xing      (1000)     2151 2023-04-24 08:58:03.000000 scinode-0.3.0/scinode/utils/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      935 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/utils/daemon.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2415 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/utils/db.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     6226 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/utils/decorator.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1089 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/utils/emoji.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      565 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/utils/formater.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    15344 2023-04-28 02:27:11.000000 scinode-0.3.0/scinode/utils/node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     7641 2023-04-21 13:20:34.000000 scinode-0.3.0/scinode/utils/nodetree.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     9864 2023-04-17 08:55:44.000000 scinode-0.3.0/scinode/utils/nt_analysis.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      977 2023-05-02 12:47:10.000000 scinode-0.3.0/scinode/utils/process.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      103 2022-12-06 13:50:07.000000 scinode-0.3.0/scinode/version.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-05-07 14:24:54.623503 scinode-0.3.0/scinode.egg-info/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1871 2023-05-07 14:24:54.000000 scinode-0.3.0/scinode.egg-info/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)     5999 2023-05-07 14:24:54.000000 scinode-0.3.0/scinode.egg-info/SOURCES.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)        1 2023-05-07 14:24:54.000000 scinode-0.3.0/scinode.egg-info/dependency_links.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)     1032 2023-05-07 14:24:54.000000 scinode-0.3.0/scinode.egg-info/entry_points.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)      133 2023-05-07 14:24:54.000000 scinode-0.3.0/scinode.egg-info/requires.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)        8 2023-05-07 14:24:54.000000 scinode-0.3.0/scinode.egg-info/top_level.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       38 2023-05-07 14:24:54.639503 scinode-0.3.0/setup.cfg
--rw-rw-r--   0 xing      (1000) xing      (1000)     2714 2023-05-07 13:59:07.000000 scinode-0.3.0/setup.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.656987 scinode-0.3.1/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1064 2022-12-06 13:50:07.000000 scinode-0.3.1/LICENSE
+-rw-rw-r--   0 xing      (1000) xing      (1000)      444 2023-05-02 12:47:10.000000 scinode-0.3.1/MANIFEST.in
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1871 2023-06-08 03:16:10.656987 scinode-0.3.1/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1537 2023-05-02 12:47:10.000000 scinode-0.3.1/README.md
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.636987 scinode-0.3.1/scinode/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      392 2023-04-17 08:55:44.000000 scinode-0.3.1/scinode/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.636987 scinode-0.3.1/scinode/app/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3661 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/app.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.636987 scinode-0.3.1/scinode/app/blueprints/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.636987 scinode-0.3.1/scinode/app/blueprints/component/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/component/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6676 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/component/component.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.636987 scinode-0.3.1/scinode/app/blueprints/component/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     7092 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/component/templates/component_editor.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)      594 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/component/templates/component_exporter.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)      359 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/component/templates/component_importer.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1613 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/component/templates/component_table.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1474 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/component/utils.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.636987 scinode-0.3.1/scinode/app/blueprints/config/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/config/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2644 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/config/config.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.636987 scinode-0.3.1/scinode/app/blueprints/config/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4703 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/config/templates/config.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)      739 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/config/templates/daemon_logfile.html
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.636987 scinode-0.3.1/scinode/app/blueprints/data/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/data/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2343 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/app/blueprints/data/data.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.636987 scinode-0.3.1/scinode/app/blueprints/data/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      800 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/data/templates/data_table.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1265 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/data/templates/data_viewer.html
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.640987 scinode-0.3.1/scinode/app/blueprints/node/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/node/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3505 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/node/node.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.640987 scinode-0.3.1/scinode/app/blueprints/node/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1717 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/node/templates/node_table.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2715 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/node/templates/node_viewer.html
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.640987 scinode-0.3.1/scinode/app/blueprints/nodetree/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/nodetree/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     7747 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/nodetree/nodetree.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.640987 scinode-0.3.1/scinode/app/blueprints/nodetree/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4081 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/app/blueprints/nodetree/templates/nodetree_editor.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)      605 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/nodetree/templates/nodetree_exporter.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)      359 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/nodetree/templates/nodetree_importer.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2079 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/nodetree/templates/nodetree_table.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2930 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/nodetree/templates/nodetree_viewer.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)      249 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/nodetree/templates/tab-description.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6594 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/nodetree/templates/tab-graph-sidebar.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1545 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/nodetree/templates/tab-graph.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)      789 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/nodetree/templates/tab-table.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1036 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/nodetree/templates/tab.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1816 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/nodetree/utils.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.640987 scinode-0.3.1/scinode/app/blueprints/scheduler/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/scheduler/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      657 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/scheduler/scheduler.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.640987 scinode-0.3.1/scinode/app/blueprints/scheduler/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/scheduler/templates/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.640987 scinode-0.3.1/scinode/app/blueprints/template/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/template/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2361 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/template/template.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.640987 scinode-0.3.1/scinode/app/blueprints/template/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1757 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/blueprints/template/templates/template_table.html
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.640987 scinode-0.3.1/scinode/app/cli/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/cli/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.640987 scinode-0.3.1/scinode/app/cli/commands/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/cli/commands/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1451 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/cli/commands/plugin.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      532 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/cli/commands/web.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     8299 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/db.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      432 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/init_data.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.644987 scinode-0.3.1/scinode/app/static/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      345 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/static/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.644987 scinode-0.3.1/scinode/app/static/__pycache__/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      555 2023-05-05 04:32:32.000000 scinode-0.3.1/scinode/app/static/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 xing      (1000) xing      (1000)    14636 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/static/component_editor.js
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.644987 scinode-0.3.1/scinode/app/static/components/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/static/components/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.644987 scinode-0.3.1/scinode/app/static/components/__pycache__/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      170 2023-05-01 07:20:25.000000 scinode-0.3.1/scinode/app/static/components/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 xing      (1000) xing      (1000)    21066 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/app/static/components/app_components.js
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.644987 scinode-0.3.1/scinode/app/static/controls/
+-rw-rw-r--   0 xing      (1000) xing      (1000)    21092 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/static/controls/app_controls.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)      950 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/static/init_editor.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5620 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/static/json_components.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)    22329 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/static/logo.png
+-rw-rw-r--   0 xing      (1000) xing      (1000)    10689 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/app/static/nodetree_editor.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1572 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/static/nodetree_node_table.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)     7589 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/static/scinode_components.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2067 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/static/scinode_editor.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)      759 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/static/sidebar.js
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.644987 scinode-0.3.1/scinode/app/static/sockets/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1276 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/static/sockets/app_sockets.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3501 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/static/styles.css
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.644987 scinode-0.3.1/scinode/app/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3713 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/templates/base.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2371 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/templates/base_editor.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2065 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/templates/index.html
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.644987 scinode-0.3.1/scinode/app/utils/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1020 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/utils/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6640 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/app/utils/rete_adapter.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.644987 scinode-0.3.1/scinode/cli/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.1/scinode/cli/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.648987 scinode-0.3.1/scinode/cli/commands/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.1/scinode/cli/commands/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1756 2023-04-17 08:55:44.000000 scinode-0.3.1/scinode/cli/commands/data.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      665 2023-04-18 11:52:21.000000 scinode-0.3.1/scinode/cli/commands/mq.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    12475 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/cli/commands/node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     8278 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/cli/commands/nodetree.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2738 2023-04-03 03:09:25.000000 scinode-0.3.1/scinode/cli/commands/profile.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3478 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/cli/commands/scheduler.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1309 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/cli/commands/shell.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     8638 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/cli/commands/worker.py
+-rwxrwxr-x   0 xing      (1000) xing      (1000)     5084 2023-05-07 13:38:33.000000 scinode-0.3.1/scinode/cli/main.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.648987 scinode-0.3.1/scinode/core/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-03-20 09:18:35.000000 scinode-0.3.1/scinode/core/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    10601 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/core/collection.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1737 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/core/executor.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3656 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/core/link.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    23429 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/core/node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3207 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/core/property.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4454 2023-04-17 08:55:44.000000 scinode-0.3.1/scinode/core/socket.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.648987 scinode-0.3.1/scinode/daemon/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.1/scinode/daemon/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4635 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/daemon/daemon.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1681 2023-04-28 02:27:11.000000 scinode-0.3.1/scinode/daemon/scheduler.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      440 2023-04-28 02:27:11.000000 scinode-0.3.1/scinode/daemon/scheduler_config.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5542 2023-06-08 03:12:34.000000 scinode-0.3.1/scinode/daemon/worker.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2836 2023-04-28 02:27:11.000000 scinode-0.3.1/scinode/daemon/worker_config.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.648987 scinode-0.3.1/scinode/database/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.1/scinode/database/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      531 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/database/client.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2102 2023-04-17 08:55:44.000000 scinode-0.3.1/scinode/database/data.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1519 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/database/db.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3657 2023-04-21 14:26:57.000000 scinode-0.3.1/scinode/database/node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     8208 2023-04-17 08:55:44.000000 scinode-0.3.1/scinode/database/nodetree.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.1/scinode/database/utils.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4203 2023-04-28 02:27:11.000000 scinode-0.3.1/scinode/database/worker.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.648987 scinode-0.3.1/scinode/engine/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       99 2023-03-20 09:18:35.000000 scinode-0.3.1/scinode/engine/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.648987 scinode-0.3.1/scinode/engine/celery/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-03-01 08:01:27.000000 scinode-0.3.1/scinode/engine/celery/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      154 2023-03-01 08:01:27.000000 scinode-0.3.1/scinode/engine/celery/app.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      708 2023-03-01 08:01:27.000000 scinode-0.3.1/scinode/engine/celery/base.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      297 2023-03-01 08:01:27.000000 scinode-0.3.1/scinode/engine/celery/celery_config.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5694 2023-04-28 02:27:11.000000 scinode-0.3.1/scinode/engine/celery/tasks.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2251 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/engine/celery/worker.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)       32 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/engine/config.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4228 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/engine/mq.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     9769 2023-04-28 02:27:11.000000 scinode-0.3.1/scinode/engine/node_engine.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    30819 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/engine/nodetree_engine.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    11992 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/engine/nodetree_launch.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3801 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/engine/scheduler.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1703 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/engine/send_to_queue.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6484 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/engine/worker.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.652987 scinode-0.3.1/scinode/executors/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.1/scinode/executors/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5050 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/executors/built_in.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.652987 scinode-0.3.1/scinode/executors/controls/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.1/scinode/executors/controls/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1471 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/executors/controls/for_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1695 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/executors/controls/if_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4585 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/executors/controls/scatter_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1401 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/executors/controls/switch_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1825 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/executors/controls/update_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3320 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/executors/list.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1865 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/executors/python.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1980 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/executors/test.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      133 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/executors/utils.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.652987 scinode-0.3.1/scinode/nodes/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      122 2022-12-23 08:17:58.000000 scinode-0.3.1/scinode/nodes/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      907 2023-04-28 02:27:11.000000 scinode-0.3.1/scinode/nodes/bash_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5623 2023-02-14 21:05:04.000000 scinode-0.3.1/scinode/nodes/build_node_from_database.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1044 2023-04-23 12:13:12.000000 scinode-0.3.1/scinode/nodes/built_in.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4112 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/nodes/control.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1289 2023-02-14 20:38:16.000000 scinode-0.3.1/scinode/nodes/node_from_database.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    23457 2023-06-05 19:35:04.000000 scinode-0.3.1/scinode/nodes/numpy_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    10719 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/nodes/python_builtin.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     8751 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/nodes/test.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2024 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/nodes/test_node_group.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      773 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/nodes/utils.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    15203 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/nodetree.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.652987 scinode-0.3.1/scinode/orm/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5758 2023-04-28 02:27:11.000000 scinode-0.3.1/scinode/orm/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      648 2023-04-28 02:27:11.000000 scinode-0.3.1/scinode/orm/data.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     8774 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/orm/db_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    12053 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/orm/db_nodetree.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1658 2023-03-20 09:18:35.000000 scinode-0.3.1/scinode/orm/db_property.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2184 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/orm/db_socket.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4929 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/orm/node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2932 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/orm/nodetree.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.652987 scinode-0.3.1/scinode/profile/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       51 2023-01-14 05:41:38.000000 scinode-0.3.1/scinode/profile/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3073 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/profile/base_config.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5076 2023-04-28 02:27:11.000000 scinode-0.3.1/scinode/profile/profile.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.652987 scinode-0.3.1/scinode/properties/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      140 2022-12-23 08:17:58.000000 scinode-0.3.1/scinode/properties/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    11696 2023-04-03 03:09:25.000000 scinode-0.3.1/scinode/properties/built_in.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.652987 scinode-0.3.1/scinode/serialization/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-02-10 18:56:33.000000 scinode-0.3.1/scinode/serialization/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1595 2023-03-20 09:18:35.000000 scinode-0.3.1/scinode/serialization/built_in.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.652987 scinode-0.3.1/scinode/sockets/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      128 2022-12-23 08:17:58.000000 scinode-0.3.1/scinode/sockets/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2502 2023-04-17 08:55:44.000000 scinode-0.3.1/scinode/sockets/built_in.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.656987 scinode-0.3.1/scinode/utils/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2151 2023-04-24 08:58:03.000000 scinode-0.3.1/scinode/utils/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      935 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/utils/daemon.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2415 2023-04-28 02:27:11.000000 scinode-0.3.1/scinode/utils/db.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6568 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/utils/decorator.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1089 2023-04-28 02:27:11.000000 scinode-0.3.1/scinode/utils/emoji.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      565 2023-04-21 13:20:34.000000 scinode-0.3.1/scinode/utils/formater.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    15124 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/utils/node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     7693 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/utils/nodetree.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    13329 2023-06-08 03:15:13.000000 scinode-0.3.1/scinode/utils/nt_analysis.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      977 2023-05-02 12:47:10.000000 scinode-0.3.1/scinode/utils/process.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      103 2022-12-06 13:50:07.000000 scinode-0.3.1/scinode/version.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-06-08 03:16:10.636987 scinode-0.3.1/scinode.egg-info/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1871 2023-06-08 03:16:10.000000 scinode-0.3.1/scinode.egg-info/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6152 2023-06-08 03:16:10.000000 scinode-0.3.1/scinode.egg-info/SOURCES.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)        1 2023-06-08 03:16:10.000000 scinode-0.3.1/scinode.egg-info/dependency_links.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1021 2023-06-08 03:16:10.000000 scinode-0.3.1/scinode.egg-info/entry_points.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)      133 2023-06-08 03:16:10.000000 scinode-0.3.1/scinode.egg-info/requires.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)        8 2023-06-08 03:16:10.000000 scinode-0.3.1/scinode.egg-info/top_level.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       38 2023-06-08 03:16:10.656987 scinode-0.3.1/setup.cfg
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2682 2023-06-08 03:15:55.000000 scinode-0.3.1/setup.py
```

### Comparing `scinode-0.3.0/LICENSE` & `scinode-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/PKG-INFO` & `scinode-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinode
-Version: 0.3.0
+Version: 0.3.1
 Summary: Design computational workflow using nodes.
 Home-page: https://github.com/scinode/scinode
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `scinode-0.3.0/README.md` & `scinode-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/app.py` & `scinode-0.3.1/scinode/app/app.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/component/component.py` & `scinode-0.3.1/scinode/app/blueprints/component/component.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/component/templates/component_editor.html` & `scinode-0.3.1/scinode/app/blueprints/component/templates/component_editor.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/component/templates/component_exporter.html` & `scinode-0.3.1/scinode/app/blueprints/component/templates/component_exporter.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/component/templates/component_table.html` & `scinode-0.3.1/scinode/app/blueprints/component/templates/component_table.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/component/utils.py` & `scinode-0.3.1/scinode/app/blueprints/component/utils.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/config/config.py` & `scinode-0.3.1/scinode/app/blueprints/config/config.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/config/templates/config.html` & `scinode-0.3.1/scinode/app/blueprints/config/templates/config.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/config/templates/daemon_logfile.html` & `scinode-0.3.1/scinode/app/blueprints/config/templates/daemon_logfile.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/data/data.py` & `scinode-0.3.1/scinode/app/blueprints/data/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,33 +42,33 @@
 
     Args:
         uuid (str): uuid of the node
 
     Returns:
         _type_: _description_
     """
-    from scinode.utils.node import get_result
+    from scinode.utils.node import get_data
 
-    result = get_result(uuid)
+    result = get_data({"uuid": uuid})
     # change to string for display
     if result["identifier"] in ["General"]:
         result["value"] = str(result["value"])
     print("result: ", result)
     return render_template("data_viewer.html", title="Data", socket_data=result)
 
 
 @data_bp.route("/<uuid>.cif")
 def download_file(uuid):
     # Generate your text file (replace with your own logic)
-    from scinode.utils.node import get_result
+    from scinode.utils.node import get_data
     from ase.io.cif import write_cif_image
     from io import StringIO
 
     s = StringIO()
-    results = get_result(uuid)
+    results = get_data({"uuid": uuid})
     atoms = results["value"]
     atoms.pbc = True
     print("atoms: ", atoms)
     write_cif_image("", atoms, s, wrap=True, labels=None, loop_keys={})
     # Create a response object with the file data
     text = s.getvalue()
     # print("cif text: ", text)
```

### Comparing `scinode-0.3.0/scinode/app/blueprints/data/templates/data_table.html` & `scinode-0.3.1/scinode/app/blueprints/data/templates/data_table.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/data/templates/data_viewer.html` & `scinode-0.3.1/scinode/app/blueprints/data/templates/data_viewer.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/node/node.py` & `scinode-0.3.1/scinode/app/blueprints/node/node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/node/templates/node_table.html` & `scinode-0.3.1/scinode/app/blueprints/node/templates/node_table.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/node/templates/node_viewer.html` & `scinode-0.3.1/scinode/app/blueprints/node/templates/node_viewer.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/nodetree/nodetree.py` & `scinode-0.3.1/scinode/app/blueprints/nodetree/nodetree.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/nodetree/templates/nodetree_editor.html` & `scinode-0.3.1/scinode/app/blueprints/nodetree/templates/nodetree_editor.html`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,18 @@
 <script src="{{ url_for('static', filename='scinode_editor.js')}}"></script>
 
 
 
 <script src="{{ url_for('static', filename='json_components.js')}}"></script>
 <script src="{{ url_for('static', filename='init_editor.js')}}"></script>
 
+<script src="{{ url_for('static', filename="sockets/app_sockets.js") }}"></script>
+<script src="{{ url_for('static', filename="controls/app_controls.js") }}"></script>
+<script src="{{ url_for('static', filename="components/app_components.js") }}"></script>
+
 {% for socket in sockets %}
 <script src="{{ url_for('static', filename="sockets/"+socket) }}"></script>
 {% endfor %}
 {% for control in controls %}
 <script src="{{ url_for('static', filename="controls/"+control) }}"></script>
 {% endfor %}
 {% for component in components %}
```

### Comparing `scinode-0.3.0/scinode/app/blueprints/nodetree/templates/nodetree_exporter.html` & `scinode-0.3.1/scinode/app/blueprints/nodetree/templates/nodetree_exporter.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/nodetree/templates/nodetree_table.html` & `scinode-0.3.1/scinode/app/blueprints/nodetree/templates/nodetree_table.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/nodetree/templates/nodetree_viewer.html` & `scinode-0.3.1/scinode/app/blueprints/nodetree/templates/nodetree_viewer.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/nodetree/templates/tab-graph-sidebar.html` & `scinode-0.3.1/scinode/app/blueprints/nodetree/templates/tab-graph-sidebar.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/nodetree/templates/tab-graph.html` & `scinode-0.3.1/scinode/app/blueprints/nodetree/templates/tab-graph.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/nodetree/templates/tab-table.html` & `scinode-0.3.1/scinode/app/blueprints/nodetree/templates/tab-table.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/nodetree/templates/tab.html` & `scinode-0.3.1/scinode/app/blueprints/nodetree/templates/tab.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/nodetree/utils.py` & `scinode-0.3.1/scinode/app/blueprints/nodetree/utils.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/scheduler/scheduler.py` & `scinode-0.3.1/scinode/app/blueprints/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/template/template.py` & `scinode-0.3.1/scinode/app/blueprints/template/template.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/blueprints/template/templates/template_table.html` & `scinode-0.3.1/scinode/app/blueprints/template/templates/template_table.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/cli/commands/plugin.py` & `scinode-0.3.1/scinode/app/cli/commands/plugin.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/cli/commands/web.py` & `scinode-0.3.1/scinode/app/cli/commands/web.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/db.py` & `scinode-0.3.1/scinode/app/db.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/static/__pycache__/__init__.cpython-310.pyc` & `scinode-0.3.1/scinode/app/static/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/static/component_editor.js` & `scinode-0.3.1/scinode/app/static/component_editor.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/static/components/app_components.js` & `scinode-0.3.1/scinode/app/static/components/app_components.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -519,15 +519,16 @@
     ]
 });
 UpdateComponent = createScinodeComponent({
     "name": "Update",
     "catalog": "Control",
     "controls": [],
     "inputs": [
-        ["General", "Input"]
+        ["General", "Input"],
+        ["General", "Update"]
     ],
     "outputs": [
         ["General", "Result"]
     ]
 });
```

### Comparing `scinode-0.3.0/scinode/app/static/controls/app_controls.js` & `scinode-0.3.1/scinode/app/static/controls/app_controls.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/static/init_editor.js` & `scinode-0.3.1/scinode/app/static/init_editor.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/static/json_components.js` & `scinode-0.3.1/scinode/app/static/json_components.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/static/logo.png` & `scinode-0.3.1/scinode/app/static/logo.png`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/static/nodetree_editor.js` & `scinode-0.3.1/scinode/app/static/nodetree_editor.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -272,15 +272,15 @@
     });
 }
 
 async function nodetree_push_message(data) {
     // post nodetree message to app
     console.log("Nodetree push message: ", data);
     console.log("Nodetree uuid: ", editor.uuid);
-    const response = await fetch("/broker/", {
+    const response = await fetch("/scheduler/", {
         method: "POST",
         headers: {
             Accept: "application/json",
             "Content-Type": "application/json",
         },
         body: JSON.stringify(data),
     });
```

### Comparing `scinode-0.3.0/scinode/app/static/nodetree_node_table.js` & `scinode-0.3.1/scinode/app/static/nodetree_node_table.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/static/scinode_components.js` & `scinode-0.3.1/scinode/app/static/scinode_components.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/static/scinode_editor.js` & `scinode-0.3.1/scinode/app/static/scinode_editor.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/static/sidebar.js` & `scinode-0.3.1/scinode/app/static/sidebar.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/static/sockets/app_sockets.js` & `scinode-0.3.1/scinode/app/static/sockets/app_sockets.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/static/styles.css` & `scinode-0.3.1/scinode/app/static/styles.css`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/templates/base.html` & `scinode-0.3.1/scinode/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/templates/base_editor.html` & `scinode-0.3.1/scinode/app/templates/base_editor.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/templates/index.html` & `scinode-0.3.1/scinode/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/utils/__init__.py` & `scinode-0.3.1/scinode/app/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/app/utils/rete_adapter.py` & `scinode-0.3.1/scinode/app/utils/rete_adapter.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/cli/commands/data.py` & `scinode-0.3.1/scinode/cli/commands/data.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/cli/commands/mq.py` & `scinode-0.3.1/scinode/cli/commands/mq.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/cli/commands/node.py` & `scinode-0.3.1/scinode/cli/commands/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
         query["state"] = state
     if action:
         query["action"] = action
     items = scinodedb["node"].find(
         query, {"_id": 0, "name": 1, "uuid": 1, "metadata.nodetree_uuid": 1}
     )
     for item in items:
-        msg = f"{item['metadata']['nodetree_uuid']},node,{item['name']}:action:LAUNCH"
+        msg = f"{item['metadata']['nodetree_uuid']},node,{item['name']}:action:CHECK"
         send_message_to_queue(broker_queue_name, msg)
-        click.secho(f'Launch node: {item["name"]} successfully!', fg="green")
+        click.secho(f'Try to launch node: {item["name"]}!', fg="green")
 
 
 @node.command(help="Reset node and its branch in the database.")
 @click.option("--name", help="Name of the node.")
 @click.option("--index", help="Index of the node.", type=int)
 @click.option("--state", help="State of the node.")
 @click.option("--uuid", help="uuid of the node.")
@@ -201,14 +201,16 @@
         query["action"] = action
     items = scinodedb["node"].find(query, {"_id": 0, "name": 1, "metadata": 1})
     if items is None:
         return
     for item in items:
         msg = f"{item['metadata']['nodetree_uuid']},node,{item['name']}:state:CREATED"
         send_message_to_queue(broker_queue_name, msg)
+        msg = f"{item['metadata']['nodetree_uuid']},node,{item['name']}:action:CHECK"
+        send_message_to_queue(broker_queue_name, msg)
         click.secho(
             f'Send the message to play node: {item["name"]} successfully!', fg="green"
         )
 
 
 @node.command(help="Cancel nodes. Warning: cancel won't stop running tasks.")
 @click.option("-n", "--name", help="Name of the item.")
```

### Comparing `scinode-0.3.0/scinode/cli/commands/nodetree.py` & `scinode-0.3.1/scinode/cli/commands/nodetree.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/cli/commands/profile.py` & `scinode-0.3.1/scinode/cli/commands/profile.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/cli/commands/scheduler.py` & `scinode-0.3.1/scinode/cli/commands/scheduler.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/cli/commands/shell.py` & `scinode-0.3.1/scinode/cli/commands/shell.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/cli/commands/worker.py` & `scinode-0.3.1/scinode/cli/commands/worker.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/cli/main.py` & `scinode-0.3.1/scinode/cli/main.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/core/collection.py` & `scinode-0.3.1/scinode/core/collection.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/core/executor.py` & `scinode-0.3.1/scinode/core/executor.py`

 * *Files 19% similar despite different names*

```diff
@@ -49,7 +49,20 @@
     def run(self):
         """Run the job."""
         pass
 
     def cancel(self):
         """callback for cancellation."""
         pass
+
+    def update_counter(self):
+        """Update the counter of the node.
+
+        Args:
+            counter (int): counter of the node.
+        """
+        from scinode.database.client import scinodedb
+
+        scinodedb["nodetree"].update_many(
+            {"uuid": self.nodetree_uuid},
+            {"$inc": {f"nodes.{self.name}.counter": 1}},
+        )
```

### Comparing `scinode-0.3.0/scinode/core/link.py` & `scinode-0.3.1/scinode/core/link.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
             from_socket (scinode.core.Socket): _description_
             to_socket (scinode.core.Socket): _description_
         """
         self.from_socket = from_socket
         self.from_node = from_socket.node
         self.to_socket = to_socket
         self.to_node = to_socket.node
+        self.state = False
         self.name = "{}.{} -> {}.{}".format(
             self.from_node.name,
             self.from_socket.name,
             self.to_node.name,
             self.to_socket.name,
         )
         self.check_socket_match()
@@ -88,14 +89,15 @@
         # logger.debug("save socket to db: {}".format(self.name))
         dbdata = {
             "from_socket": self.from_socket.name,
             "from_node": self.from_node.name,
             "from_socket_uuid": self.from_socket.uuid,
             "to_socket": self.to_socket.name,
             "to_node": self.to_node.name,
+            "state": self.state,
         }
         return dbdata
 
     def copy(self):
         """We can not simply copy the link, because the link is related to the node."""
         pass
```

### Comparing `scinode-0.3.0/scinode/core/node.py` & `scinode-0.3.1/scinode/core/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,23 +96,26 @@
         self.scattered_label = scattered_label
         self.scatter_node = scatter_node
         self.ref_uuid = ""
         self.copy_uuid = ""
         self.properties = PropertyCollection(self)
         self.inputs = InputSocketCollection(self)
         self.outputs = OutputSocketCollection(self)
+        self.ctrl_inputs = InputSocketCollection(self)
+        self.ctrl_outputs = OutputSocketCollection(self)
         self.executor = None
         self.state = "CREATED"
         self.action = "NONE"
         self.position = [30 * self.inner_id, 30 * self.inner_id]
         self.description = ""
         self.log = ""
         self.ng = self.get_node_group() if self.node_type.upper() == "GROUP" else None
         self.create_properties()
         self.create_sockets()
+        self.create_ctrl_sockets()
         # logger.debug("Create {}: {}".format(self.node_type, self.name))
 
     def create_properties(self):
         """Create properties for this node.
         If this node is a group node, create properties based on the exposed properties.
         """
         self.properties.clear()
@@ -139,14 +142,23 @@
         If this node is a group node, create sockets based on group inputs and outputs.
         """
         self.inputs.clear()
         self.outputs.clear()
         if self.node_type.upper() == "GROUP":
             self.create_group_sockets()
 
+    def create_ctrl_sockets(self):
+        """Create control input and output sockets for this node."""
+        self.ctrl_inputs.clear()
+        self.ctrl_outputs.clear()
+        socket = self.ctrl_inputs.new("General", "Entry")
+        socket.link_limit = 1000
+        socket = self.ctrl_outputs.new("General", "Exit")
+        socket.link_limit = 1000
+
     def create_group_sockets(self):
         """Create input and output sockets based on group inputs
         and outputs.
 
         group_inputs = [
             ["add1", "x", "x"],
             ["add1", "y", "y"]]
@@ -268,27 +280,31 @@
                 "register_path": self.register_path,
             }
         else:
             metadata = self.get_metadata()
             properties = self.properties_to_dict()
             input_sockets = self.input_sockets_to_dict()
             output_sockets = self.output_sockets_to_dict()
+            ctrl_input_sockets = self.ctrl_input_sockets_to_dict()
+            ctrl_output_sockets = self.ctrl_output_sockets_to_dict()
             executor = self.executor_to_dict()
             data = {
                 "version": "scinode@{}".format(__version__),
                 "uuid": self.uuid,
                 "name": self.name,
                 "inner_id": self.inner_id,
                 "state": self.state,
                 "action": self.action,
                 "error": "",
                 "metadata": metadata,
                 "properties": properties,
                 "inputs": input_sockets,
                 "outputs": output_sockets,
+                "ctrl_inputs": ctrl_input_sockets,
+                "ctrl_outputs": ctrl_output_sockets,
                 "executor": executor,
                 "position": self.position,
                 "description": self.description,
                 "log": self.log,
                 "hash": "",
             }
             # calculate the hash of metadata
@@ -361,14 +377,30 @@
         """Export output sockets to a dictionary."""
         # save all relations using links
         outputs = []
         for socket in self.outputs:
             outputs.append(socket.to_dict())
         return outputs
 
+    def ctrl_input_sockets_to_dict(self):
+        """Export ctrl_input sockets to a dictionary."""
+        # save all relations using links
+        ctrl_inputs = []
+        for socket in self.ctrl_inputs:
+            ctrl_inputs.append(socket.to_dict())
+        return ctrl_inputs
+
+    def ctrl_output_sockets_to_dict(self):
+        """Export ctrl_output sockets to a dictionary."""
+        # save all relations using links
+        ctrl_outputs = []
+        for socket in self.ctrl_outputs:
+            ctrl_outputs.append(socket.to_dict())
+        return ctrl_outputs
+
     def executor_to_dict(self):
         """Export executor dictionary to a dictionary.
         Three kinds of executor:
         - Python built-in function. e.g. getattr
         - User defined function
         - User defined class.
         """
@@ -550,15 +582,14 @@
         """Update node."""
         from scinode.database.client import scinodedb
 
         query = {"uuid": self.uuid}
         data = scinodedb["node"].find_one(
             query, {"state": 1, "action": 1, "results": 1, "metadata.counter": 1}
         )
-        self.counter = data["metadata"]["counter"]
         self.results = self.get_results()
 
     def ref_to(self, uuid):
         """Set reference node."""
         from scinode.database.client import scinodedb
 
         self.node_type = "REF"
```

### Comparing `scinode-0.3.0/scinode/core/property.py` & `scinode-0.3.1/scinode/core/property.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/core/socket.py` & `scinode-0.3.1/scinode/core/socket.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/daemon/daemon.py` & `scinode-0.3.1/scinode/daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/daemon/scheduler.py` & `scinode-0.3.1/scinode/daemon/scheduler.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/daemon/worker.py` & `scinode-0.3.1/scinode/daemon/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,16 @@
             )
         )
         print("Reset: ")
         for ntdata in ntdatas:
             nt = DBNodeTree(uuid=ntdata["uuid"])  # , self.worker_name)
             for name, node in ntdata["nodes"].items():
                 if node["state"] == "RUNNING":
-                    nt.reset_node(name, launch=True)
+                    print("  nodetree: {}, node: {}".format(ntdata["name"], name))
+                    nt.reset_node(name)
             nt.launch()
 
     def showlog(self, limit=100):
         with open(self.logfile) as f:
             lines = f.readlines()
             for line in lines[-limit:]:
                 print(line.strip())
```

### Comparing `scinode-0.3.0/scinode/daemon/worker_config.py` & `scinode-0.3.1/scinode/daemon/worker_config.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/database/client.py` & `scinode-0.3.1/scinode/database/client.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/database/data.py` & `scinode-0.3.1/scinode/database/data.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/database/db.py` & `scinode-0.3.1/scinode/database/db.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/database/node.py` & `scinode-0.3.1/scinode/database/node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/database/nodetree.py` & `scinode-0.3.1/scinode/database/nodetree.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/database/worker.py` & `scinode-0.3.1/scinode/database/worker.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/engine/celery/base.py` & `scinode-0.3.1/scinode/engine/celery/base.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/engine/celery/tasks.py` & `scinode-0.3.1/scinode/engine/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/engine/celery/worker.py` & `scinode-0.3.1/scinode/engine/celery/worker.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/engine/mq.py` & `scinode-0.3.1/scinode/engine/mq.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/engine/node_engine.py` & `scinode-0.3.1/scinode/engine/node_engine.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/engine/nodetree_launch.py` & `scinode-0.3.1/scinode/engine/nodetree_launch.py`

 * *Files 5% similar despite different names*

```diff
@@ -327,22 +327,15 @@
         """Analyze the connectivity of nodetree and save it into dict."""
         from scinode.utils.nt_analysis import ConnectivityAnalysis
 
         if ntdata is None:
             ntdata = self.ntdata
         logger.debug("Calculate child nodes...")
         nc = ConnectivityAnalysis(ntdata)
-        child_node, control_node = nc.build_children()
-        inputs = nc.get_input_output()
-        connectivity = {
-            "child_node": child_node,
-            "control_node": control_node,
-            "input_node": inputs,
-        }
-        self.ntdata["connectivity"] = connectivity
+        self.ntdata["connectivity"] = nc.build_connectivity()
 
 
 if __name__ == "__main__":
     from scinode.nodetree import NodeTree
 
     nt = NodeTree(name="test_debug_math")
     float1 = nt.nodes.new("TestFloat", "float1")
```

### Comparing `scinode-0.3.0/scinode/engine/send_to_queue.py` & `scinode-0.3.1/scinode/engine/send_to_queue.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/engine/worker.py` & `scinode-0.3.1/scinode/engine/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         elif action == "LAUNCH":
             self.launch_node(uuid, name)
         elif action == "EXPOSE_OUTPUTS":
             self.expose_outputs(uuid, name)
         else:
             print("Unknown action: ", action)
         # print("apply_node_action: ", self.record["nodes"])
-        logger.debug("apply_node_action, time: {}".format(time.time() - tstart))
+        # logger.debug("apply_node_action, time: {}".format(time.time() - tstart))
 
     def launch_node(self, uuid, name):
         """Launch node"""
         print(f"\nLaunch node: {name}, {uuid}")
         ntdata = scinodedb["nodetree"].find_one(
             {"uuid": uuid}, {"_id": 0, f"nodes.{name}": 1}
         )
```

### Comparing `scinode-0.3.0/scinode/executors/built_in.py` & `scinode-0.3.1/scinode/executors/built_in.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,21 +36,21 @@
     for x in args:
         results += (x,)
     return results
 
 
 def data_node(uuid="", Input=None):
     """Out the data node result as sockets."""
-    from scinode.utils.node import get_result
+    from scinode.utils.node import get_data
 
     results = ()
     if uuid == "" or uuid is None:
         results = (Input,)
     else:
-        results = (get_result(uuid),)
+        results = (get_data({"uuid": uuid}),)
     return results
 
 
 class NodeGroup(Executor):
     """Out the properties as sockets."""
 
     def run(self):
```

### Comparing `scinode-0.3.0/scinode/executors/controls/scatter_node.py` & `scinode-0.3.1/scinode/executors/controls/scatter_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 class ScinodeScatter(Executor):
     """Scatter nodes executor"""
 
     def run(self):
         """
         0) Find all subtrees created by this node, and delete them
-        1) Find all children nodes after the scatter node
+        1) Find all nodes controled by the scatter node
         2) Create a new nodetree nt1
         3) build all children node inside new nodetree nt1
         4) use REF node
         5) launch the nodetree
         """
         print("Run for scatter {}".format(self.name))
         self.prepare()
         self.new_nodetree()
-        self.set_gather_state()
+        self.set_scattered_state()
 
     def prepare(self):
         from scinode.nodetree import NodeTree
 
         self.delete_sub_nodetree()
         if isinstance(self.kwargs["Input"], dict):
             labels = self.kwargs["Input"].keys()
@@ -30,15 +30,15 @@
         self.labels = labels
         print("  Scatter labels: {}".format(self.labels))
         # nodetree data
         self.nt = NodeTree.load(self.dbdata["metadata"]["nodetree_uuid"])
         connectivity = scinodedb["nodetree"].find_one(
             {"uuid": self.dbdata["metadata"]["nodetree_uuid"]}, {"connectivity": 1}
         )["connectivity"]
-        self.copy_nodes = connectivity["child_node"][self.name]
+        self.copy_nodes = connectivity["control_node"][self.name].get("Scatter", [])
         print("copy_nodes: ", self.copy_nodes)
 
     def delete_sub_nodetree(self):
         """Delete nodetrees which are scattered from this node."""
         from scinode.database.nodetree import NodetreeClient
 
         # Find all subtrees created by this node, and delete them
@@ -89,22 +89,22 @@
                 data_node.outputs["Result"],
                 nt.nodes[link["to_node"]].inputs[link["to_socket"]],
             )
         # data_node.state = "FINISHED"
         # data_node.scattered_from = self.uuid
         # data_node.scattered_label = str(label)
 
-    def set_gather_state(self):
+    def set_scattered_state(self):
         from scinode.engine.send_to_queue import send_message_to_queue
         from scinode.engine.config import broker_queue_name
 
         scatter = {}
         for label in self.labels:
             scatter[str(label)] = "CREATED"
-        # all the children nodes should not run, instead the action should be gather.
+        # all the children nodes should not run, instead the state should be scattered.
         for name in self.copy_nodes:
             print(f"    Set Node {name} state to SCATTERED.")
             msg = f"{self.nodetree_uuid},node,{name}:state:SCATTERED"
             send_message_to_queue(broker_queue_name, msg)
             #
             print(f"    Add new key: scatter for Node {name}.")
             newvalues = {"$set": {f"nodes.{name}.scatter": scatter}}
```

### Comparing `scinode-0.3.0/scinode/executors/controls/switch_node.py` & `scinode-0.3.1/scinode/executors/controls/switch_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,14 @@
         # print(data)
         replace_one(serialize_item(data), scinodedb["data"])
         # set node state to be finished to avoid deadblock
         # find all children nodes of the "switch" node
         if self.kwargs["Switch"]:
             # reset all nodes and launch
             print("reset node")
-            nt.reset_node(dbdata["name"], launch=True)
+            nt.reset_node(dbdata["name"])
         else:
             # skip all nodes
             print("skip node")
             nt.skip_node(dbdata["name"])
         this_results = (self.kwargs["Input"],)
         return this_results
```

### Comparing `scinode-0.3.0/scinode/executors/controls/update_node.py` & `scinode-0.3.1/scinode/executors/controls/update_node.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,23 +31,21 @@
         inputs = dbdata["inputs"]
         non_from_nodes = []
         for link in inputs[1]["links"]:
             non_from_nodes.append(link["from_node"])
         # because we skip the worker to set the state
         # we have to update the result manully here
         data = self.dbdata["outputs"][0]
-        print("   Counter: {}".format(dbdata["metadata"]["counter"]))
-        if dbdata["metadata"]["counter"] > 0:
+        print("   Counter: {}".format(nt.record["nodes"][self.name]["counter"]))
+        if nt.record["nodes"][self.name]["counter"] > 0:
             # reset all nodes and launch
-            nt.reset_node(dbdata["name"], launch=True)
+            nt.reset_node(dbdata["name"])
             data["value"] = self.kwargs["Update"]
             # print("    results: ", results)
             this_results = (self.kwargs["Update"],)
         else:
             data["value"] = self.kwargs["Input"]
             this_results = (self.kwargs["Input"],)
         # print("  Save results: ", results)
         replace_one(serialize_item(data), scinodedb["data"])
-        update_node.update_db_keys(
-            {"metadata.counter": dbdata["metadata"]["counter"] + 1}
-        )
+        self.update_counter()
         return this_results
```

### Comparing `scinode-0.3.0/scinode/executors/test.py` & `scinode-0.3.1/scinode/executors/test.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/nodes/bash_node.py` & `scinode-0.3.1/scinode/nodes/bash_node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/nodes/build_node_from_database.py` & `scinode-0.3.1/scinode/nodes/build_node_from_database.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/nodes/built_in.py` & `scinode-0.3.1/scinode/nodes/built_in.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/nodes/node_from_database.py` & `scinode-0.3.1/scinode/nodes/node_from_database.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/nodes/numpy_node.py` & `scinode-0.3.1/scinode/nodes/numpy_node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/nodes/python_builtin.py` & `scinode-0.3.1/scinode/nodes/python_builtin.py`

 * *Files 18% similar despite different names*

```diff
@@ -89,14 +89,35 @@
         return {
             "path": "builtins",
             "name": "str",
             "type": "function",
         }
 
 
+class DictNode(Node):
+    """Output an empty Dict value."""
+
+    identifier = "Dict"
+    name = "Dict"
+    catalog = "Input"
+
+    def create_properties(self):
+        pass
+
+    def create_sockets(self):
+        self.outputs.new("BaseDict", "Dict")
+
+    def get_executor(self):
+        return {
+            "path": "builtins",
+            "name": "dict",
+            "type": "function",
+        }
+
+
 class Getattr(Node):
     """The Getattr node sets the value of the attribute of an object.
 
     Executor:
         Python builtin function: getattr()
 
     Results:
@@ -264,55 +285,154 @@
         return {
             "path": "scinode.executors.python",
             "name": "setitem",
             "type": "function",
         }
 
 
-class Index(Node):
-    """To find index of the first occurrence of an element
-    in a given Python List or numpy array.
+list_func_items = [
+    ["List", "List", "List"],
+    ["Append", "Append", "Append"],
+    ["Extend", "Extend", "Extend"],
+    ["Remove", "Remove", "Remove"],
+    ["Index", "Index", "Index"],
+    ["Count", "Count", "Count"],
+    ["Insert", "Insert", "Insert"],
+    ["Pop", "Pop", "Pop"],
+    ["Reverse", "Reverse", "Reverse"],
+]
+
+
+class List(Node):
+    """Append a value to a list.
 
     Executor:
-        Python builtin function: list.index(), numpy.where()
+        Python builtin function: list.append()
 
     Results:
-        Index.
+        List.
 
     Example:
 
     """
 
-    identifier: str = "Index"
+    identifier: str = "List"
     node_type: str = "Normal"
     catalog = "Builtin"
 
     def create_properties(self):
-        pass
+        self.properties.new(
+            "Enum",
+            "function",
+            data={
+                "default": "List",
+                "options": list_func_items,
+                "update": self.create_sockets,
+            },
+        )
 
     def create_sockets(self):
         self.inputs.clear()
         self.outputs.clear()
-        self.inputs.new("General", "Source")
-        self.inputs.new("General", "Value")
-        self.outputs.new("General", "Index")
-        self.args = ["Source", "Value"]
+        if self.properties["function"].value in ["List"]:
+            self.inputs.new("General", "Input")
+            self.kwargs = ["Input"]
+        elif self.properties["function"].value in [
+            "Append",
+            "Extend",
+            "Remove",
+            "Index",
+            "Count",
+        ]:
+            self.inputs.new("BaseList", "List")
+            self.inputs.new("General", "Value")
+            self.kwargs = ["List", "Value"]
+        elif self.properties["function"].value in ["Insert"]:
+            self.inputs.new("BaseList", "List")
+            self.inputs.new("Int", "Index")
+            self.inputs.new("General", "Value")
+            self.kwargs = ["List", "Index", "Value"]
+        elif self.properties["function"].value in ["Pop"]:
+            self.inputs.new("BaseList", "List")
+            self.inputs.new("Int", "Index")
+            self.kwargs = ["List", "Index"]
+        elif self.properties["function"].value in ["Reverse"]:
+            self.inputs.new("BaseList", "List")
+            self.kwargs = ["List"]
+        else:
+            self.inputs.new("BaseList", "List")
+            self.kwargs = ["List"]
+        self.outputs.new("General", "Result")
+
+    def get_executor(self):
+        return {
+            "path": "scinode.executors.list",
+            "name": self.properties["function"].value,
+            "type": "class",
+        }
+
+
+operator_items = [
+    ["+", "+", "+"],
+    ["-", "-", "-"],
+    ["*", "*", "*"],
+    ["/", "/", "/"],
+    ["%", "%", "%"],
+    ["**", "**", "**"],
+    ["//", "//", "//"],
+    ["==", "==", "=="],
+    ["!=", "!=", "!="],
+    [">", ">", ">"],
+    ["<", "<", "<"],
+    [">=", ">=", ">="],
+    ["<=", "<=", "<="],
+]
+
+
+class Operator(Node):
+    """Operators are used to perform operations on variables and values."""
+
+    identifier: str = "Operator"
+    node_type: str = "Normal"
+    catalog = "Builtin"
+
+    def create_properties(self):
+        self.properties.new(
+            "Enum",
+            "operator",
+            data={
+                "default": "==",
+                "options": operator_items,
+                "update": self.create_sockets,
+            },
+        )
+
+    def create_sockets(self):
+        self.inputs.clear()
+        self.outputs.clear()
+        self.inputs.new("General", "x")
+        self.inputs.new("General", "y")
+        self.outputs.new("General", "Result")
+        self.args = ["x", "y"]
+        self.kwargs = ["operator"]
 
     def get_executor(self):
         return {
             "path": "scinode.executors.python",
-            "name": "index",
-            "type": "function",
+            "name": "operator",
+            "type": "fucntion",
         }
 
 
 node_list = [
     IntNode,
     FloatNode,
     BoolNode,
     StrNode,
+    DictNode,
     Getattr,
     Setattr,
     Getitem,
     Setitem,
-    Index,
+    List,
+    Operator,
 ]
```

### Comparing `scinode-0.3.0/scinode/nodes/test.py` & `scinode-0.3.1/scinode/nodes/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         self.properties.new("Int", "t", data={"default": 1})
 
     def create_sockets(self):
         self.inputs.clear()
         self.outputs.clear()
         self.inputs.new("Float", "x")
         self.inputs.new("Float", "y")
-        self.outputs.new("Float", "Result")
+        self.outputs.new("Bool", "Result")
 
     def get_executor(self):
         return {
             "path": "scinode.executors.test",
             "name": "test_greater",
         }
```

### Comparing `scinode-0.3.0/scinode/nodes/test_node_group.py` & `scinode-0.3.1/scinode/nodes/test_node_group.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/nodetree.py` & `scinode-0.3.1/scinode/nodetree.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         self.parent = parent
         self.parent_node = parent_node
         self.scatter_node = scatter_node
         self.scattered_label = scattered_label
         self.nodetrees = NodeTreeCollection(self)
         self.nodes = NodeCollection(self)
         self.links = LinkCollection(self)
+        self.ctrl_links = LinkCollection(self)
         self.state = "CREATED"
         self.action = "NONE"
         self.description = ""
         self.log = ""
         logger.info("Create NodeTree: {}".format(self.name))
 
     def launch(self, worker_name=None):
@@ -133,24 +134,26 @@
             dict: nodetree data
         """
         from scinode.version import __version__
 
         metadata = self.get_metadata()
         nodes = self.nodes_to_dict(short=short)
         links = self.links_to_dict()
+        ctrl_links = self.ctrl_links_to_dict()
         data = {
             "version": "scinode@{}".format(__version__),
             "uuid": self.uuid,
             "name": self.name,
             "state": self.state,
             "action": self.action,
             "error": "",
             "metadata": metadata,
             "nodes": nodes,
             "links": links,
+            "ctrl_links": ctrl_links,
             "description": self.description,
             "log": self.log,
         }
         return data
 
     def get_metadata(self):
         """metadata to dict"""
@@ -184,14 +187,23 @@
         # save all relations using links
         links = []
         for link in self.links:
             links.append(link.to_dict())
         # logger.debug("Done")
         return links
 
+    def ctrl_links_to_dict(self):
+        """ctrl_links to dict"""
+        # save all relations using ctrl_links
+        ctrl_links = []
+        for link in self.ctrl_links:
+            ctrl_links.append(link.to_dict())
+        # logger.debug("Done")
+        return ctrl_links
+
     def to_yaml(self):
         """Export to a yaml format data.
         Results of the nodes are not exported."""
         import yaml
 
         data = self.to_dict()
         for name, node in data["nodes"].items():
@@ -216,14 +228,15 @@
         self.state = data["state"]
         self.action = data["action"]
         self.update_nodes(data["nodes"])
 
     def update_nodes(self, data):
         for node in self.nodes:
             node.state = data[node.name]["state"]
+            node.counter = data[node.name]["counter"]
             node.action = data[node.name]["action"]
             node.update()
 
     @skip_ref_node
     def reset_node(self, name):
         """Reset node.
 
@@ -251,14 +264,16 @@
 
         Args:
             name (str): name of the node to be played
         """
 
         msg = f"{self.uuid},node,{name}:state:CREATED"
         send_message_to_queue(broker_queue_name, msg)
+        msg = f"{self.uuid},node,{name}:action:CHECK"
+        send_message_to_queue(broker_queue_name, msg)
 
     @classmethod
     def from_dict(cls, ntdata):
         """Rebuild nodetree from dict ntdata.
 
         Args:
             ntdata (dict): data of the nodetree.
```

### Comparing `scinode-0.3.0/scinode/orm/__init__.py` & `scinode-0.3.1/scinode/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/orm/data.py` & `scinode-0.3.1/scinode/orm/data.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/orm/db_node.py` & `scinode-0.3.1/scinode/orm/db_node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/orm/db_nodetree.py` & `scinode-0.3.1/scinode/orm/db_nodetree.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,14 +284,21 @@
         dbdata_nodes = self.dbdata_nodes
         nodes = {}
         for name, dbdata in dbdata_nodes.items():
             node = DBNode(uuid=dbdata["uuid"])  # , self.worker_name)
             nodes[node.name] = node
         return nodes
 
+    def set_node_state(self, names, state):
+        """Set node state."""
+        for name in names:
+            send_message_to_queue(
+                broker_queue_name, f"{self.uuid},node,{name}:state:{state}"
+            )
+
     @skip_ref_node
     def pause_node(self, name):
         """Pause node.
 
         Args:
             name (str): name of the node to be paused
         """
```

### Comparing `scinode-0.3.0/scinode/orm/db_property.py` & `scinode-0.3.1/scinode/orm/db_property.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/orm/db_socket.py` & `scinode-0.3.1/scinode/orm/db_socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,16 @@
         Input: input value.
         Output: result."""
         if self.type == "inputs":
             from scinode.utils.node import get_input_socket_value
 
             value = get_input_socket_value(self.dbdata)
         else:
-            from scinode.utils.node import get_result
+            from scinode.utils.node import get_data
 
-            value = get_result(self.uuid)
+            value = get_data({"uuid": self.uuid})
         return value["value"]
 
     def __repr__(self) -> str:
         s = ""
         s += 'NodeSocekt(name="{}")'.format(self.name)
         return s
```

### Comparing `scinode-0.3.0/scinode/orm/node.py` & `scinode-0.3.1/scinode/orm/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from mongoengine import (
     Document,
     EmbeddedDocument,
     StringField,
     FloatField,
     IntField,
+    BooleanField,
     DateTimeField,
     ListField,
     MapField,
     ObjectIdField,
     EmbeddedDocumentField,
     signals,
 )
@@ -50,14 +51,15 @@
 class Link(EmbeddedDocument):
     from_node = StringField(max_length=50)
     from_socket = StringField(max_length=50)
     from_socket_uuid = StringField(max_length=50)
     to_node = StringField(max_length=50)
     to_socket = StringField(max_length=50)
     to_socket_uuid = StringField(max_length=50)
+    state = BooleanField()
 
 
 class Socket(EmbeddedDocument):
     name = StringField(max_length=50)
     type = StringField(max_length=50)
     node_uuid = StringField(max_length=50)
     identifier = StringField(max_length=50)
@@ -99,14 +101,16 @@
     error = StringField()
     index = IntField()
     inner_id = IntField(primary_key=True)
     metadata = EmbeddedDocumentField(Meta)
     executor = EmbeddedDocumentField(Executor)
     inputs = ListField(EmbeddedDocumentField(Socket))
     outputs = ListField(EmbeddedDocumentField(Socket))
+    ctrl_inputs = ListField(EmbeddedDocumentField(Socket))
+    ctrl_outputs = ListField(EmbeddedDocumentField(Socket))
     properties = MapField(EmbeddedDocumentField(Property))
     position = ListField()
     hash = StringField(max_length=100)
 
     def _init__(self, uuid, name):
         self.uuid = (uuid,)
         self.name = name
```

### Comparing `scinode-0.3.0/scinode/profile/base_config.py` & `scinode-0.3.1/scinode/profile/base_config.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/profile/profile.py` & `scinode-0.3.1/scinode/profile/profile.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/properties/built_in.py` & `scinode-0.3.1/scinode/properties/built_in.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/serialization/built_in.py` & `scinode-0.3.1/scinode/serialization/built_in.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/sockets/built_in.py` & `scinode-0.3.1/scinode/sockets/built_in.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/utils/__init__.py` & `scinode-0.3.1/scinode/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/utils/daemon.py` & `scinode-0.3.1/scinode/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/utils/db.py` & `scinode-0.3.1/scinode/utils/db.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/utils/decorator.py` & `scinode-0.3.1/scinode/utils/decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         _type_: _description_
     """
     from scinode.core.node import Node
 
     # print("ndata: ", ndata)
     class MyNode(Node):
         identifier: str = ndata["identifier"]
+        node_type: str = ndata["node_type"]
         args = ndata.get("args", [])
         kwargs = ndata.get("kwargs", [])
         catalog = ndata.get("catalog", "Others")
         register_path = ndata.get("register_path", "")
 
         def create_properties(self):
             for prop in ndata.get("properties", []):
@@ -70,28 +71,30 @@
             return ngdata["nt"]
 
     return MyNodeGroup
 
 
 def register_node(
     identifier,
+    node_type="Normal",
     args={},
     kwargs={},
     properties=[],
     inputs=[],
     outputs=[],
     executor={},
     register_path="",
     catalog="Others",
 ):
     from scinode.utils import register
     from scinode.nodes import node_pool
 
     ndata = {
         "identifier": identifier,
+        "node_type": node_type,
         "catalog": catalog,
         "args": args,
         "kwargs": kwargs,
         "properties": properties,
         "inputs": inputs,
         "outputs": outputs,
         "executor": executor,
@@ -124,20 +127,22 @@
         return None
     return node
 
 
 # decorator with arguments indentifier, args, kwargs, properties, inputs, outputs, executor
 def decorator_node(
     identifier,
+    node_type="Normal",
     args={},
     kwargs={},
     properties=[],
     inputs=[],
     outputs=[],
     catalog="Others",
+    executor_path=None,
 ):
     """Generate a decorator that register a function as a SciNode node.
 
     Attributes:
         indentifier (str): node identifier
         catalog (str): node catalog
         args (list): node args
@@ -147,24 +152,28 @@
         outputs (list): node outputs
     """
 
     def decorator(func):
         import inspect
         from pathlib import Path
 
-        path = Path(inspect.getfile(func))
+        if executor_path is None:
+            path = Path(inspect.getfile(func)).name.split(".")[0]
+        else:
+            path = executor_path
         name = func.__name__
         executor = {
-            "path": path.name.split(".")[0],
+            "path": path,
             "name": name,
             "type": "function",
         }
-        register_path = f'{path.name.split(".")[0]}.{name}'
+        register_path = f"{path}.{name}"
         register_node(
             identifier,
+            node_type,
             args,
             kwargs,
             properties,
             inputs,
             outputs,
             executor,
             register_path=register_path,
@@ -173,28 +182,31 @@
         func.identifier = identifier
         return func
 
     return decorator
 
 
 # decorator with arguments indentifier, args, kwargs, properties, inputs, outputs, executor
-def decorator_node_group(identifier, catalog="Others"):
+def decorator_node_group(identifier, catalog="Others", executor_path=None):
     """Generate a decorator that register a function as a SciNode node.
 
     Attributes:
         indentifier (str): node identifier
     """
 
     def decorator(func):
         from pathlib import Path
         import inspect
 
-        path = Path(inspect.getfile(func))
+        if executor_path is None:
+            path = Path(inspect.getfile(func)).name.split(".")[0]
+        else:
+            path = executor_path
         name = func.__name__
-        register_path = f'{path.name.split(".")[0]}.{name}'
+        register_path = f"{path}.{name}"
         nt = func()
         node = register_node_group(
             identifier, nt, register_path=register_path, catalog=catalog
         )
         return node
 
     return decorator
```

### Comparing `scinode-0.3.0/scinode/utils/emoji.py` & `scinode-0.3.1/scinode/utils/emoji.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/utils/formater.py` & `scinode-0.3.1/scinode/utils/formater.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode/utils/node.py` & `scinode-0.3.1/scinode/utils/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -259,32 +259,21 @@
     children = scinodedb["node"].find(
         {"metadata.scattered_from": ndata["uuid"]},
         {"uuid": 1},
     )
     for child in children:
         child_results = get_results(child["uuid"])
         for i in range(no):
+            if child_results[i] is None:
+                continue
             value = child_results[i]["value"]
             outputs[i]["value"].append(value)
     return outputs
 
 
-def get_result(uuid):
-    from scinode.database.client import scinodedb
-    from scinode.utils.node import deserialize_item
-
-    query = {"uuid": uuid}
-    data = scinodedb["data"].find_one(query, {"_id": 0})
-    if data:
-        result = deserialize_item(data)
-    else:
-        result = data
-    return result
-
-
 def get_results(uuid):
     """Get node results.
 
     If the node is scattered, gather the results.
     """
     from scinode.database.client import scinodedb
 
@@ -296,23 +285,23 @@
     )
     # check node is scattered or not
     if "scatter" in ntdata["nodes"][ndata["name"]]:
         results = gather_node_results(ndata)
     else:
         results = []
         for output in ndata["outputs"]:
-            result = get_result(output["uuid"])
+            result = get_data({"uuid": output["uuid"]})
             results += [result]
     return results
 
 
 def get_data(query):
     from scinode.database.db import scinodedb
 
-    data = scinodedb["data"].find_one(query)
+    data = scinodedb["data"].find_one(query, {"_id": 0})
     # print("get_data: ", data)
     if data is None:
         return data
     data = deserialize_item(data)
     # print("get_data: ", data)
     return data
 
@@ -423,15 +412,15 @@
     from scinode.engine.config import broker_queue_name
 
     outputs = ndata["outputs"]
     no = len(outputs)
     # expose outputs
     for i in range(no):
         # find the output of the node in the nodetree
-        result = get_result(cache_node["outputs"][i]["uuid"])
+        result = get_data({"uuid": cache_node["outputs"][i]["uuid"]})
         if result is None:
             return 1
         outputs[i]["value"] = result["value"]
         save_socket_data(outputs[i])
     log = f"Node: {ndata['name']} reuse cache node {cache_node['name']} with uuid: {cache_node['uuid']}.\n"
     log += "Results: {}".format(outputs)
     #
```

### Comparing `scinode-0.3.0/scinode/utils/nodetree.py` & `scinode-0.3.1/scinode/utils/nodetree.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
             "identifier": node["metadata"]["identifier"],
             "node_type": node["metadata"]["node_type"],
             "register_path": node["metadata"]["register_path"],
             "uuid": node["uuid"],
             "state": node["state"],
             "action": node["action"],
             "worker": node["metadata"]["worker_name"],
+            "counter": node["metadata"]["counter"],
         }
     return ntdata_short
 
 
 def nt_export_py(ntdata):
     from scinode.utils.node import deserialize
```

### Comparing `scinode-0.3.0/scinode/utils/process.py` & `scinode-0.3.1/scinode/utils/process.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.0/scinode.egg-info/PKG-INFO` & `scinode-0.3.1/scinode.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinode
-Version: 0.3.0
+Version: 0.3.1
 Summary: Design computational workflow using nodes.
 Home-page: https://github.com/scinode/scinode
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `scinode-0.3.0/scinode.egg-info/SOURCES.txt` & `scinode-0.3.1/scinode.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -125,30 +125,35 @@
 scinode/engine/celery/app.py
 scinode/engine/celery/base.py
 scinode/engine/celery/celery_config.py
 scinode/engine/celery/tasks.py
 scinode/engine/celery/worker.py
 scinode/executors/__init__.py
 scinode/executors/built_in.py
+scinode/executors/list.py
 scinode/executors/python.py
 scinode/executors/test.py
+scinode/executors/utils.py
 scinode/executors/controls/__init__.py
+scinode/executors/controls/for_node.py
+scinode/executors/controls/if_node.py
 scinode/executors/controls/scatter_node.py
 scinode/executors/controls/switch_node.py
 scinode/executors/controls/update_node.py
 scinode/nodes/__init__.py
 scinode/nodes/bash_node.py
 scinode/nodes/build_node_from_database.py
 scinode/nodes/built_in.py
 scinode/nodes/control.py
 scinode/nodes/node_from_database.py
 scinode/nodes/numpy_node.py
 scinode/nodes/python_builtin.py
 scinode/nodes/test.py
 scinode/nodes/test_node_group.py
+scinode/nodes/utils.py
 scinode/orm/__init__.py
 scinode/orm/data.py
 scinode/orm/db_node.py
 scinode/orm/db_nodetree.py
 scinode/orm/db_property.py
 scinode/orm/db_socket.py
 scinode/orm/node.py
```

### Comparing `scinode-0.3.0/scinode.egg-info/entry_points.txt` & `scinode-0.3.1/scinode.egg-info/entry_points.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 bash_node = scinode.nodes.bash_node:node_list
 built_in = scinode.nodes.built_in:node_list
 control = scinode.nodes.control:node_list
 numpy_node = scinode.nodes.numpy_node:node_list
 python_builtin = scinode.nodes.python_builtin:node_list
 test = scinode.nodes.test:node_list
 test_node_group = scinode.nodes.test_node_group:node_list
+utils = scinode.nodes.utils:node_list
 
 [scinode_property]
 built_in = scinode.properties.built_in:property_list
 
 [scinode_socket]
 built_in = scinode.sockets.built_in:socket_list
-
-[scinode_static]
-main = scinode.app.static:main
```

### Comparing `scinode-0.3.0/setup.py` & `scinode-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="scinode",
-    version="0.3.0",
+    version="0.3.1",
     description="Design computational workflow using nodes.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/scinode/scinode",
     author="Xing Wang",
     author_email="xingwang1991@gmail.com",
     license="MIT License",
@@ -45,25 +45,23 @@
         "scinode_node": [
             "built_in = scinode.nodes.built_in:node_list",
             "bash_node = scinode.nodes.bash_node:node_list",
             "control = scinode.nodes.control:node_list",
             "python_builtin = scinode.nodes.python_builtin:node_list",
             "numpy_node = scinode.nodes.numpy_node:node_list",
             "test = scinode.nodes.test:node_list",
+            "utils = scinode.nodes.utils:node_list",
             "test_node_group = scinode.nodes.test_node_group:node_list",
         ],
         "scinode_socket": [
             "built_in = scinode.sockets.built_in:socket_list",
         ],
         "scinode_property": [
             "built_in = scinode.properties.built_in:property_list",
         ],
-        "scinode_static": [
-            "main = scinode.app.static:main",
-        ],
     },
     install_requires=[
         "psutil",
         "numpy",
         "scipy",
         "click",
         "dnspython",
```

