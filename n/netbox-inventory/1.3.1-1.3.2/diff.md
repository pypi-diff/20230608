# Comparing `tmp/netbox-inventory-1.3.1.tar.gz` & `tmp/netbox-inventory-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-inventory-1.3.1.tar", last modified: Fri May 26 18:19:55 2023, max compression
+gzip compressed data, was "netbox-inventory-1.3.2.tar", last modified: Thu Jun  8 13:24:25 2023, max compression
```

## Comparing `netbox-inventory-1.3.1.tar` & `netbox-inventory-1.3.2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.055877 netbox-inventory-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-26 18:19:55.055877 netbox-inventory-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.047877 netbox-inventory-1.3.1/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/analyzers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.047877 netbox-inventory-1.3.1/netbox_inventory/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.047877 netbox-inventory-1.3.1/netbox_inventory/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)    17795 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/bulk_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/forms/reassign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.047877 netbox-inventory-1.3.1/netbox_inventory/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/migrations/0001_initial_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/migrations/0002_alter_asset_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.043877 netbox-inventory-1.3.1/netbox_inventory/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset.html
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_assign.html
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_create.html
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_reassign.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/purchase.html
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/supplier.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/tests/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_views_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_views_reassign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_group/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_group/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_group/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_type/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_type/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/tests/purchase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/purchase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/purchase/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/purchase/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.051877 netbox-inventory-1.3.1/netbox_inventory/tests/supplier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/supplier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/supplier/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/supplier/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.055877 netbox-inventory-1.3.1/netbox_inventory/views/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/asset_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/asset_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/asset_reassign.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/inventoryitem_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/inventoryitem_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/purchase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/supplier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/netbox_inventory/views/tabs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:55.047877 netbox-inventory-1.3.1/netbox_inventory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-26 18:19:55.000000 netbox-inventory-1.3.1/netbox_inventory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-26 18:19:55.000000 netbox-inventory-1.3.1/netbox_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:19:55.000000 netbox-inventory-1.3.1/netbox_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:19:55.000000 netbox-inventory-1.3.1/netbox_inventory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 18:19:45.000000 netbox-inventory-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 18:19:55.055877 netbox-inventory-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.694632 netbox-inventory-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-06-08 13:24:25.694632 netbox-inventory-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.682631 netbox-inventory-1.3.2/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/analyzers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.686632 netbox-inventory-1.3.2/netbox_inventory/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.686632 netbox-inventory-1.3.2/netbox_inventory/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/forms/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17795 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/forms/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/forms/bulk_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/forms/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/forms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/forms/reassign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.686632 netbox-inventory-1.3.2/netbox_inventory/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/migrations/0001_initial_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/migrations/0002_alter_asset_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.682631 netbox-inventory-1.3.2/netbox_inventory/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.690631 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/asset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/asset_assign.html
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/asset_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/asset_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/asset_reassign.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.690631 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/purchase.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/supplier.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.690631 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.690631 netbox-inventory-1.3.2/netbox_inventory/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.690631 netbox-inventory-1.3.2/netbox_inventory/tests/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/asset/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/asset/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/asset/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/asset/test_views_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/asset/test_views_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.690631 netbox-inventory-1.3.2/netbox_inventory/tests/inventoryitem_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/inventoryitem_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/inventoryitem_group/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/inventoryitem_group/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.690631 netbox-inventory-1.3.2/netbox_inventory/tests/inventoryitem_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/inventoryitem_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/inventoryitem_type/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/inventoryitem_type/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.690631 netbox-inventory-1.3.2/netbox_inventory/tests/purchase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/purchase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/purchase/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/purchase/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.690631 netbox-inventory-1.3.2/netbox_inventory/tests/supplier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/supplier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/supplier/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/supplier/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.694632 netbox-inventory-1.3.2/netbox_inventory/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/views/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/views/asset_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/views/asset_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/views/asset_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/views/inventoryitem_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/views/inventoryitem_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/views/purchase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/views/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/netbox_inventory/views/tabs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:24:25.686632 netbox-inventory-1.3.2/netbox_inventory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-06-08 13:24:25.000000 netbox-inventory-1.3.2/netbox_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-08 13:24:25.000000 netbox-inventory-1.3.2/netbox_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:24:25.000000 netbox-inventory-1.3.2/netbox_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 13:24:25.000000 netbox-inventory-1.3.2/netbox_inventory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-08 13:24:16.000000 netbox-inventory-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:24:25.694632 netbox-inventory-1.3.2/setup.cfg
```

### Comparing `netbox-inventory-1.3.1/LICENSE` & `netbox-inventory-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/PKG-INFO` & `netbox-inventory-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.3.1
+Version: 1.3.2
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netbox-inventory-1.3.1/README.md` & `netbox-inventory-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/__init__.py` & `netbox-inventory-1.3.2/netbox_inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/analyzers.py` & `netbox-inventory-1.3.2/netbox_inventory/analyzers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/api/nested_serializers.py` & `netbox-inventory-1.3.2/netbox_inventory/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/api/serializers.py` & `netbox-inventory-1.3.2/netbox_inventory/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/api/urls.py` & `netbox-inventory-1.3.2/netbox_inventory/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/api/views.py` & `netbox-inventory-1.3.2/netbox_inventory/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/filtersets.py` & `netbox-inventory-1.3.2/netbox_inventory/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/forms/assign.py` & `netbox-inventory-1.3.2/netbox_inventory/forms/assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/forms/bulk.py` & `netbox-inventory-1.3.2/netbox_inventory/forms/bulk.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/forms/bulk_add.py` & `netbox-inventory-1.3.2/netbox_inventory/forms/bulk_add.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/forms/create.py` & `netbox-inventory-1.3.2/netbox_inventory/forms/create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/forms/filters.py` & `netbox-inventory-1.3.2/netbox_inventory/forms/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/forms/models.py` & `netbox-inventory-1.3.2/netbox_inventory/forms/models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/forms/reassign.py` & `netbox-inventory-1.3.2/netbox_inventory/forms/reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/migrations/0001_initial_prod.py` & `netbox-inventory-1.3.2/netbox_inventory/migrations/0001_initial_prod.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/migrations/0003_add_inventoryitemgroup.py` & `netbox-inventory-1.3.2/netbox_inventory/migrations/0003_add_inventoryitemgroup.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py` & `netbox-inventory-1.3.2/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/models.py` & `netbox-inventory-1.3.2/netbox_inventory/models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/navigation.py` & `netbox-inventory-1.3.2/netbox_inventory/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/search.py` & `netbox-inventory-1.3.2/netbox_inventory/search.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/signals.py` & `netbox-inventory-1.3.2/netbox_inventory/signals.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tables.py` & `netbox-inventory-1.3.2/netbox_inventory/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/template_content.py` & `netbox-inventory-1.3.2/netbox_inventory/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/asset.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 {% extends 'generic/object.html' %}
 {% load helpers %}
 {% load humanize %}
+{% load plugins %}
 
 {% block title %}{{ object.hardware_type.manufacturer }} {{ object }}{% endblock %}
 
 {% block breadcrumbs %}
   {{ block.super }}
   <li class="breadcrumb-item">
     <a href="{% url 'plugins:netbox_inventory:asset_list' %}?{{ object.kind }}_type_id={{ object.hardware_type.pk }}">{{ object.hardware_type.manufacturer }} {{ object.hardware_type }}</a>
@@ -137,14 +138,15 @@
               <th scope="row">Device</th>
               <td>{{ object.installed_device|linkify|placeholder }}</td>
             </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
+      {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Purchase</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
@@ -175,10 +177,16 @@
             </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
       {% include 'inc/panels/image_attachments.html' %}
+      {% plugin_right_page object %}
+    </div>
+  </div>
+  <div class="row mb-3">
+    <div class="col col-md-12">
+      {% plugin_full_width_page object %}
     </div>
   </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% load humanize %} {%
-block title %}{{ object.hardware_type.manufacturer }} {{ object }}{% endblock
-%} {% block breadcrumbs %} {{ block.super }}
+load plugins %} {% block title %}{{ object.hardware_type.manufacturer }} {
+{ object }}{% endblock %} {% block breadcrumbs %} {{ block.super }}
 {{_object.hardware_type.manufacturer_}}_{{_object.hardware_type_}}
 {% endblock %} {% block content %}
 ** Asset **
 Name                    {{ object.name|placeholder }}
 Asset Tag               {{ object.asset_tag|placeholder }}
 Serial Number           {{ object.serial|placeholder }}
 Status                  {% badge object.get_status_display
@@ -40,19 +40,21 @@
 Site     {{ object.installed_site|linkify|placeholder }}
          {% if object.installed_location %} {% for location in
 Location object.installed_location.get_ancestors %} {{ location|linkify }} / {%
          endfor %} {{ object.installed_location|linkify }} {% else %} {
          { ''|placeholder }} {% endif %}
 Rack     {{ object.installed_rack|linkify|placeholder }}
 Device   {{ object.installed_device|linkify|placeholder }}
-{% include 'inc/panels/custom_fields.html' %}
+{% include 'inc/panels/custom_fields.html' %} {% plugin_left_page object %}
 ** Purchase **
 Owner              {{ object.owner|linkify|placeholder }}
 Purchase           {{ object.purchase|linkify|placeholder }}
 Purchase date      {{ object.purchase.date|annotated_date|placeholder }}
 Warranty start     {{ object.warranty_start|annotated_date|placeholder }}
 Warranty end       {{ object.warranty_end|annotated_date|placeholder }}
 Warranty remaining {% include "netbox_inventory/inc/asset_warranty.html" with
                    asset=object %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
-{% include 'inc/panels/image_attachments.html' %}
+{% include 'inc/panels/image_attachments.html' %} {% plugin_right_page object
+%}
+{% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_edit.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/asset_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/asset_reassign.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/asset_reassign.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_info.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/inc/asset_info.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/inc/asset_warranty.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {% extends 'generic/object.html' %}
 {% load helpers %}
+{% load plugins %}
 {% load render_table from django_tables2 %}
 
 {% block breadcrumbs %}
   {{ block.super }}
   {% for group in object.get_ancestors %}
     <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_inventory:inventoryitemgroup' group.pk %}">{{ group }}</a></li>
   {% endfor %}
@@ -103,15 +104,15 @@
             {% empty %}
             <tr><td class="text-center text-muted" colspan="2">— No assets found —</td></tr>
             {% endfor %}
           </tbody>
           </table>
         </div>
       </div>
-  
+      {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">
           Child Groups
         </h5>
         <div class="card-body table-responsive">
@@ -123,21 +124,23 @@
               <span class="mdi mdi-plus-thick" aria-hidden="true"></span> Add Group
             </a>
           </div>
         {% endif %}
       </div>
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
+      {% plugin_right_page object %}
     </div>
   </div>
   <div class="row mb-3">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Assets</h5>
         <div class="card-body table-responsive">
           {% render_table asset_table 'inc/table.html' %}
           {% include 'inc/paginator.html' with paginator=asset_table.paginator page=asset_table.page %}
         </div>
       </div>
+      {% plugin_full_width_page object %}
     </div>
   </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-{% extends 'generic/object.html' %} {% load helpers %} {% load render_table
-from django_tables2 %} {% block breadcrumbs %} {{ block.super }} {% for group
-in object.get_ancestors %}
+{% extends 'generic/object.html' %} {% load helpers %} {% load plugins %} {%
+load render_table from django_tables2 %} {% block breadcrumbs %} {{ block.super
+}} {% for group in object.get_ancestors %}
 {{_group_}}
 {% endfor %} {% endblock %} {% block extra_controls %} {% if
 perms.netbox_inventory.add_inventoryitemtype %}
  Add_inventory_item_type
  {% endif %} {% endblock extra_controls %} {% block content %}
 ** Inventory Item Group **
 Name   {{ object.name }}
@@ -19,17 +19,20 @@
 Inventory Item Type                        Status - Count
 {                                          {% for status in tsc.status_list %}
 {                                          {%_badge_value=status.label|add:'_-
 tsc.inventoryitem_type__manufacturer__name '|add:status.count
 }}_{{_tsc.inventoryitem_type__model_}}     bg_color=status.color|add:'_w-100'
                                            %} {% endfor %}
 â No assets found â
+{% plugin_left_page object %}
 ** Child Groups **
 {% render_table child_groups_table 'inc/table.html' %}
 {% if perms.netbox_inventory.add_inventoryitemgroup %}
 _Add_Group
 {% endif %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
+{% plugin_right_page object %}
 ** Assets **
 {% render_table asset_table 'inc/table.html' %} {% include 'inc/paginator.html'
 with paginator=asset_table.paginator page=asset_table.page %}
+{% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% extends 'generic/object.html' %}
+{% load plugins %}
 
 {% block title %}{{ object.manufacturer }} {{ object.model }}{% endblock %}
 
 {% block breadcrumbs %}
   {{ block.super }}
   <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_inventory:inventoryitemtype_list' %}?manufacturer_id={{ object.manufacturer.pk }}">{{ object.manufacturer }}</a></li>
 {% endblock %}
@@ -42,15 +43,22 @@
               <th scope="row">Assets</th>
               <td><a href="{% url 'plugins:netbox_inventory:asset_list' %}?inventoryitem_type_id={{ object.pk }}">{{ asset_count }}</a></td>
             </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
+      {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
       {% include 'inc/panels/image_attachments.html' %}
+      {% plugin_right_page object %}
+    </div>
+  </div>
+  <div class="row mb-3">
+    <div class="col col-md-12">
+      {% plugin_full_width_page object %}
     </div>
   </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,17 +1,20 @@
-{% extends 'generic/object.html' %} {% block title %}{{ object.manufacturer }}
-{{ object.model }}{% endblock %} {% block breadcrumbs %} {{ block.super }}
+{% extends 'generic/object.html' %} {% load plugins %} {% block title %}{
+{ object.manufacturer }} {{ object.model }}{% endblock %} {% block breadcrumbs
+%} {{ block.super }}
 {{_object.manufacturer_}}
 {% endblock %} {% block extra_controls %} {% if
 perms.netbox_inventory.add_asset %}
  Add_asset
  {% endif %} {% endblock extra_controls %} {% block content %}
 ** Inventory Item Type **
 Manufacturer {{ object.manufacturer|linkify }}
 Model        {{ object.model }}
 Part number  {{ object.part_number }}
 Group        {{ object.inventoryitem_group|linkify|placeholder }}
 Assets       {{_asset_count_}}
-{% include 'inc/panels/custom_fields.html' %}
+{% include 'inc/panels/custom_fields.html' %} {% plugin_left_page object %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
-{% include 'inc/panels/image_attachments.html' %}
+{% include 'inc/panels/image_attachments.html' %} {% plugin_right_page object
+%}
+{% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/purchase.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/supplier.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,70 +1,67 @@
 {% extends 'generic/object.html' %}
-{% load helpers %}
+{% load plugins %}
 {% load render_table from django_tables2 %}
 
 {% block breadcrumbs %}
-  {{ block.super }}
-  <li class="breadcrumb-item">
-    <a href="{% url 'plugins:netbox_inventory:purchase_list' %}?supplier_id={{ object.supplier.pk }}">{{ object.supplier }}</a>
-  </li>
+  <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_inventory:supplier_list' %}">Suppliers</a></li>
 {% endblock %}
 
 {% block extra_controls %}
-  {% if perms.netbox_inventory.add_asset %}
-    <a href="{% url 'plugins:netbox_inventory:asset_add' %}?purchase={{ object.pk }}" class="btn btn-sm btn-primary">
-      <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add asset
+  {% if perms.netbox_inventory.add_purchase %}
+    <a href="{% url 'plugins:netbox_inventory:purchase_add' %}?supplier={{ object.pk }}" class="btn btn-sm btn-primary">
+      <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add purchase
     </a>
   {% endif %}
 {% endblock extra_controls %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
-        <h5 class="card-header">Purchase</h5>
+        <h5 class="card-header">Supplier</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Name</th>
               <td>{{ object.name }}</td>
             </tr>
             <tr>
-              <th scope="row">Supplier</th>
-              <td>{{ object.supplier|linkify }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Date</th>
-              <td>{{ object.date|annotated_date|placeholder }}</td>
+              <th scope="row">Description</th>
+              <td>{{ object.description }}</td>
             </tr>
             <tr>
-              <th scope="row">Description</th>
-              <td>{{ object.description|placeholder }}</td>
+              <th scope="row">Purchases</th>
+              <td>
+                <a href="{% url 'plugins:netbox_inventory:purchase_list' %}?supplier_id={{ object.pk }}">{{ purchase_count }}</a>
+              </td>
             </tr>
             <tr>
               <th scope="row">Assets</th>
               <td>
-                <a href="{% url 'plugins:netbox_inventory:asset_list' %}?purchase_id={{ object.pk }}">{{ asset_count }}</a>
+                <a href="{% url 'plugins:netbox_inventory:asset_list' %}?supplier_id={{ object.pk }}">{{ asset_count }}</a>
               </td>
             </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/tags.html' %}
+      {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/custom_fields.html' %}
       {% include 'inc/panels/comments.html' %}
+      {% plugin_right_page object %}
     </div>
   </div>
   <div class="row mb-3">
     <div class="col col-md-12">
       <div class="card">
-        <h5 class="card-header">Purchased Assets</h5>
+        <h5 class="card-header">Supplied Assets</h5>
         <div class="card-body table-responsive">
           {% render_table asset_table 'inc/table.html' %}
           {% include 'inc/paginator.html' with paginator=asset_table.paginator page=asset_table.page %}
         </div>
       </div>
+      {% plugin_full_width_page object %}
     </div>
-  </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-{% extends 'generic/object.html' %} {% load helpers %} {% load render_table
-from django_tables2 %} {% block breadcrumbs %} {{ block.super }}
-{{_object.supplier_}}
+{% extends 'generic/object.html' %} {% load plugins %} {% load render_table
+from django_tables2 %} {% block breadcrumbs %}
+Suppliers
 {% endblock %} {% block extra_controls %} {% if
-perms.netbox_inventory.add_asset %}
- Add_asset
+perms.netbox_inventory.add_purchase %}
+ Add_purchase
  {% endif %} {% endblock extra_controls %} {% block content %}
-** Purchase **
+** Supplier **
 Name        {{ object.name }}
-Supplier    {{ object.supplier|linkify }}
-Date        {{ object.date|annotated_date|placeholder }}
-Description {{ object.description|placeholder }}
+Description {{ object.description }}
+Purchases   {{_purchase_count_}}
 Assets      {{_asset_count_}}
-{% include 'inc/panels/tags.html' %}
+{% include 'inc/panels/tags.html' %} {% plugin_left_page object %}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/
-comments.html' %}
-** Purchased Assets **
+comments.html' %} {% plugin_right_page object %}
+** Supplied Assets **
 {% render_table asset_table 'inc/table.html' %} {% include 'inc/paginator.html'
 with paginator=asset_table.paginator page=asset_table.page %}
+{% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/supplier.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/purchase.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,74 @@
 {% extends 'generic/object.html' %}
+{% load helpers %}
+{% load plugins %}
 {% load render_table from django_tables2 %}
 
 {% block breadcrumbs %}
-  <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_inventory:supplier_list' %}">Suppliers</a></li>
+  {{ block.super }}
+  <li class="breadcrumb-item">
+    <a href="{% url 'plugins:netbox_inventory:purchase_list' %}?supplier_id={{ object.supplier.pk }}">{{ object.supplier }}</a>
+  </li>
 {% endblock %}
 
 {% block extra_controls %}
-  {% if perms.netbox_inventory.add_purchase %}
-    <a href="{% url 'plugins:netbox_inventory:purchase_add' %}?supplier={{ object.pk }}" class="btn btn-sm btn-primary">
-      <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add purchase
+  {% if perms.netbox_inventory.add_asset %}
+    <a href="{% url 'plugins:netbox_inventory:asset_add' %}?purchase={{ object.pk }}" class="btn btn-sm btn-primary">
+      <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add asset
     </a>
   {% endif %}
 {% endblock extra_controls %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
-        <h5 class="card-header">Supplier</h5>
+        <h5 class="card-header">Purchase</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Name</th>
               <td>{{ object.name }}</td>
             </tr>
             <tr>
-              <th scope="row">Description</th>
-              <td>{{ object.description }}</td>
+              <th scope="row">Supplier</th>
+              <td>{{ object.supplier|linkify }}</td>
             </tr>
             <tr>
-              <th scope="row">Purchases</th>
-              <td>
-                <a href="{% url 'plugins:netbox_inventory:purchase_list' %}?supplier_id={{ object.pk }}">{{ purchase_count }}</a>
-              </td>
+              <th scope="row">Date</th>
+              <td>{{ object.date|annotated_date|placeholder }}</td>
+            </tr>
+            <tr>
+              <th scope="row">Description</th>
+              <td>{{ object.description|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Assets</th>
               <td>
-                <a href="{% url 'plugins:netbox_inventory:asset_list' %}?supplier_id={{ object.pk }}">{{ asset_count }}</a>
+                <a href="{% url 'plugins:netbox_inventory:asset_list' %}?purchase_id={{ object.pk }}">{{ asset_count }}</a>
               </td>
             </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/tags.html' %}
+      {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/custom_fields.html' %}
       {% include 'inc/panels/comments.html' %}
+      {% plugin_right_page object %}
     </div>
   </div>
   <div class="row mb-3">
     <div class="col col-md-12">
       <div class="card">
-        <h5 class="card-header">Supplied Assets</h5>
+        <h5 class="card-header">Purchased Assets</h5>
         <div class="card-body table-responsive">
           {% render_table asset_table 'inc/table.html' %}
           {% include 'inc/paginator.html' with paginator=asset_table.paginator page=asset_table.page %}
         </div>
       </div>
+      {% plugin_full_width_page object %}
     </div>
+  </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,19 +1,22 @@
-{% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
-{% block breadcrumbs %}
-Suppliers
+{% extends 'generic/object.html' %} {% load helpers %} {% load plugins %} {%
+load render_table from django_tables2 %} {% block breadcrumbs %} {{ block.super
+}}
+{{_object.supplier_}}
 {% endblock %} {% block extra_controls %} {% if
-perms.netbox_inventory.add_purchase %}
- Add_purchase
+perms.netbox_inventory.add_asset %}
+ Add_asset
  {% endif %} {% endblock extra_controls %} {% block content %}
-** Supplier **
+** Purchase **
 Name        {{ object.name }}
-Description {{ object.description }}
-Purchases   {{_purchase_count_}}
+Supplier    {{ object.supplier|linkify }}
+Date        {{ object.date|annotated_date|placeholder }}
+Description {{ object.description|placeholder }}
 Assets      {{_asset_count_}}
-{% include 'inc/panels/tags.html' %}
+{% include 'inc/panels/tags.html' %} {% plugin_left_page object %}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/
-comments.html' %}
-** Supplied Assets **
+comments.html' %} {% plugin_right_page object %}
+** Purchased Assets **
 {% render_table asset_table 'inc/table.html' %} {% include 'inc/paginator.html'
 with paginator=asset_table.paginator page=asset_table.page %}
+{% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html` & `netbox-inventory-1.3.2/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_api.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/asset/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_models.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/asset/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_views.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/asset/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_views_create.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/asset/test_views_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/asset/test_views_reassign.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/asset/test_views_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/custom.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/custom.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_group/test_api.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/inventoryitem_group/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_group/test_views.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/inventoryitem_group/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_type/test_api.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/inventoryitem_type/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/inventoryitem_type/test_views.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/inventoryitem_type/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/purchase/test_api.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/purchase/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/purchase/test_views.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/purchase/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/settings.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/settings.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/supplier/test_api.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/supplier/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/supplier/test_views.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/supplier/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/tests/test_load.py` & `netbox-inventory-1.3.2/netbox_inventory/tests/test_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class NetboxDnsVersionTestCase(SimpleTestCase):
     """
     Test for netbox_inventory package
     """
 
     def test_version(self):
-        assert __version__ == "1.3.1"
+        assert __version__ == "1.3.2"
 
 
 class AppTest(APITestCase):
     """
     Test the availability of the plugin API root
     """
```

### Comparing `netbox-inventory-1.3.1/netbox_inventory/urls.py` & `netbox-inventory-1.3.2/netbox_inventory/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/utils.py` & `netbox-inventory-1.3.2/netbox_inventory/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/views/asset.py` & `netbox-inventory-1.3.2/netbox_inventory/views/asset.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/views/asset_assign.py` & `netbox-inventory-1.3.2/netbox_inventory/views/asset_assign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/views/asset_create.py` & `netbox-inventory-1.3.2/netbox_inventory/views/asset_create.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/views/asset_reassign.py` & `netbox-inventory-1.3.2/netbox_inventory/views/asset_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/views/inventoryitem_group.py` & `netbox-inventory-1.3.2/netbox_inventory/views/inventoryitem_group.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/views/inventoryitem_type.py` & `netbox-inventory-1.3.2/netbox_inventory/views/inventoryitem_type.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/views/purchase.py` & `netbox-inventory-1.3.2/netbox_inventory/views/purchase.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/views/supplier.py` & `netbox-inventory-1.3.2/netbox_inventory/views/supplier.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory/views/tabs.py` & `netbox-inventory-1.3.2/netbox_inventory/views/tabs.py`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/netbox_inventory.egg-info/PKG-INFO` & `netbox-inventory-1.3.2/netbox_inventory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.3.1
+Version: 1.3.2
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netbox-inventory-1.3.1/netbox_inventory.egg-info/SOURCES.txt` & `netbox-inventory-1.3.2/netbox_inventory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-inventory-1.3.1/pyproject.toml` & `netbox-inventory-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-inventory"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
   { name="Matej Vadnjal", email="matej.vadnjal@arnes.si" },
 ]
 description = "Inventory asset management in NetBox"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

