# Comparing `tmp/channel_app-0.0.98.tar.gz` & `tmp/channel_app-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/channel_app-0.0.98.tar", last modified: Mon Jun 13 08:44:03 2022, max compression
+gzip compressed data, was "dist/channel_app-0.0.99.tar", last modified: Fri Jun 17 08:02:27 2022, max compression
```

## Comparing `channel_app-0.0.98.tar` & `channel_app-0.0.99.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      339 2022-06-13 08:44:03.000000 channel_app-0.0.98/PKG-INFO
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/README.md
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/__init__.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/app/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/app/__init__.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/app/order/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/app/order/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     9384 2022-06-13 08:43:34.000000 channel_app-0.0.98/channel_app/app/order/service.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/app/product/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/app/product/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    10272 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/app/product/service.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/app/product_image/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/app/product_image/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     5527 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/app/product_image/service.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/app/product_price/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/app/product_price/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    11038 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/app/product_price/service.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/app/product_stock/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/app/product_stock/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    10891 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/app/product_stock/service.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/app/setup/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/app/setup/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2727 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/app/setup/service.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/channel/__init__.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel/commands/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/channel/commands/__init__.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel/commands/orders/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/channel/commands/orders/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    11068 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/channel/commands/orders/orders.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       52 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/channel/commands/product_categories.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     4855 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/channel/commands/product_images.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     4855 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/channel/commands/product_prices.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     8157 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/channel/commands/product_stocks.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     5257 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/channel/commands/products.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    33882 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/channel/commands/setup.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3444 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/channel/integration.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel_app/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/__init__.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel_app/app/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/app/__init__.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel_app/app/order/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/app/order/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     8841 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/app/order/service.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel_app/app/product/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/app/product/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     9883 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/app/product/service.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel_app/app/product_price/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/app/product_price/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    11038 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/app/product_price/service.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel_app/app/product_stock/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/app/product_stock/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    10891 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/app/product_stock/service.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel_app/app/setup/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/app/setup/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2727 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/app/setup/service.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel_app/channel/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/channel/__init__.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel_app/channel/commands/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/channel/commands/__init__.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel_app/channel/commands/orders/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/channel/commands/orders/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    11068 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/channel/commands/orders/orders.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       52 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/channel/commands/product_categories.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       41 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/channel/commands/product_images.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     4855 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/channel/commands/product_prices.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     8157 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/channel/commands/product_stocks.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     5257 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/channel/commands/products.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    33882 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/channel/commands/setup.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3694 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/channel/integration.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel_app/core/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/core/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      491 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/core/clients.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    13976 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/core/commands.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     5601 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/core/data.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2817 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/core/integration.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2092 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/core/products.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     1212 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/core/settings.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3081 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/core/utilities.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3345 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/batch_request.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    11498 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/batch_requests.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2942 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/error_reports.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     7338 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/integration_actions.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/orders/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/orders/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    10846 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/orders/addresses.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     1308 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/orders/cargo_companies.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3409 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/orders/customers.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    18202 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/orders/orders.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       43 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/product_categories.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       32 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/product_images.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     7629 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/product_prices.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     8897 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/product_stocks.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    28205 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/products.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    35153 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/commands/setup.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2718 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/constants.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      928 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/exceptions.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     8322 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/channel_app/omnitron/integration.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/core/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/core/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      491 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/core/clients.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    13976 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/core/commands.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     5670 2022-06-13 08:43:34.000000 channel_app-0.0.98/channel_app/core/data.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2817 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/core/integration.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2092 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/core/products.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     1212 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/core/settings.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3081 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/core/utilities.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/omnitron/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3345 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/batch_request.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/omnitron/commands/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/commands/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    11498 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/commands/batch_requests.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2942 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/commands/error_reports.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     7338 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/commands/integration_actions.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app/omnitron/commands/orders/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/commands/orders/__init__.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    10968 2022-06-13 08:43:34.000000 channel_app-0.0.98/channel_app/omnitron/commands/orders/addresses.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     1308 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/commands/orders/cargo_companies.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3409 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/commands/orders/customers.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    19029 2022-06-13 08:43:34.000000 channel_app-0.0.98/channel_app/omnitron/commands/orders/orders.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       43 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/commands/product_categories.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     5497 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/commands/product_images.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     7518 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/commands/product_prices.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     8785 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/commands/product_stocks.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    28201 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/commands/products.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    35153 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/commands/setup.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2718 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/constants.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      928 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/exceptions.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     8650 2022-06-13 08:37:13.000000 channel_app-0.0.98/channel_app/omnitron/integration.py
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      669 2022-06-01 12:03:38.000000 channel_app-0.0.98/channel_app/setup.py
-drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-13 08:44:03.000000 channel_app-0.0.98/channel_app.egg-info/
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      339 2022-06-13 08:44:02.000000 channel_app-0.0.98/channel_app.egg-info/PKG-INFO
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     4952 2022-06-13 08:44:02.000000 channel_app-0.0.98/channel_app.egg-info/SOURCES.txt
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        1 2022-06-13 08:44:02.000000 channel_app-0.0.98/channel_app.egg-info/dependency_links.txt
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        9 2022-06-13 08:44:02.000000 channel_app-0.0.98/channel_app.egg-info/requires.txt
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       12 2022-06-13 08:44:02.000000 channel_app-0.0.98/channel_app.egg-info/top_level.txt
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       38 2022-06-13 08:44:03.000000 channel_app-0.0.98/setup.cfg
--rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      628 2022-06-13 08:43:34.000000 channel_app-0.0.98/setup.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      339 2022-06-17 08:02:27.000000 channel_app-0.0.99/PKG-INFO
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/README.md
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/__init__.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/app/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/app/__init__.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/app/order/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/app/order/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     9384 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/app/order/service.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/app/product/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/app/product/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    10272 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/app/product/service.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/app/product_image/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/app/product_image/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     5527 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/app/product_image/service.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/app/product_price/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/app/product_price/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    11038 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/app/product_price/service.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/app/product_stock/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/app/product_stock/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    10891 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/app/product_stock/service.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/app/setup/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/app/setup/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2811 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/app/setup/service.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/channel/__init__.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel/commands/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/channel/commands/__init__.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel/commands/orders/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/channel/commands/orders/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    11068 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/channel/commands/orders/orders.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       52 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/channel/commands/product_categories.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     4855 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/channel/commands/product_images.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     4855 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/channel/commands/product_prices.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     8157 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/channel/commands/product_stocks.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     5257 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/channel/commands/products.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    33882 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/channel/commands/setup.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3444 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/channel/integration.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel_app/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/__init__.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel_app/app/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/app/__init__.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel_app/app/order/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/app/order/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     8841 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/app/order/service.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel_app/app/product/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/app/product/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     9883 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/app/product/service.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel_app/app/product_price/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/app/product_price/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    11038 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/app/product_price/service.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel_app/app/product_stock/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/app/product_stock/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    10891 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/app/product_stock/service.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel_app/app/setup/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/app/setup/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2727 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/app/setup/service.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel_app/channel/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/channel/__init__.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel_app/channel/commands/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/channel/commands/__init__.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel_app/channel/commands/orders/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/channel/commands/orders/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    11068 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/channel/commands/orders/orders.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       52 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/channel/commands/product_categories.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       41 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/channel/commands/product_images.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     4855 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/channel/commands/product_prices.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     8157 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/channel/commands/product_stocks.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     5257 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/channel/commands/products.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    33882 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/channel/commands/setup.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3694 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/channel/integration.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel_app/core/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/core/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      491 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/core/clients.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    13976 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/core/commands.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     5601 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/core/data.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2817 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/core/integration.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2092 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/core/products.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     1212 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/core/settings.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3081 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/core/utilities.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3345 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/batch_request.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    11498 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/batch_requests.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2942 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/error_reports.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     7338 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/integration_actions.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/orders/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/orders/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    10846 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/orders/addresses.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     1308 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/orders/cargo_companies.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3409 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/orders/customers.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    18202 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/orders/orders.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       43 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/product_categories.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       32 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/product_images.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     7629 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/product_prices.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     8897 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/product_stocks.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    28205 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/products.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    35153 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/commands/setup.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2718 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/constants.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      928 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/exceptions.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     8322 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/channel_app/omnitron/integration.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/core/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/core/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      491 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/core/clients.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    13976 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/core/commands.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     5670 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/core/data.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2817 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/core/integration.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2092 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/core/products.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     1212 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/core/settings.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3081 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/core/utilities.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/omnitron/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3550 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/batch_request.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/omnitron/commands/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/commands/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    11498 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/commands/batch_requests.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2942 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/commands/error_reports.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     7338 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/commands/integration_actions.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app/omnitron/commands/orders/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/commands/orders/__init__.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    10968 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/commands/orders/addresses.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     1308 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/commands/orders/cargo_companies.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     3409 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/commands/orders/customers.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    19029 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/commands/orders/orders.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       43 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/commands/product_categories.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     5497 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/commands/product_images.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     7518 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/commands/product_prices.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     8785 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/commands/product_stocks.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    28201 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/commands/products.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)    35153 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/commands/setup.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     2718 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/constants.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      928 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/exceptions.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     8650 2022-06-17 08:00:34.000000 channel_app-0.0.99/channel_app/omnitron/integration.py
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      669 2022-06-01 12:03:38.000000 channel_app-0.0.99/channel_app/setup.py
+drwxrwxr-x   0 eyupt     (1000) eyupt     (1000)        0 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app.egg-info/
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      339 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app.egg-info/PKG-INFO
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)     4952 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app.egg-info/SOURCES.txt
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        1 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app.egg-info/dependency_links.txt
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)        9 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app.egg-info/requires.txt
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       12 2022-06-17 08:02:27.000000 channel_app-0.0.99/channel_app.egg-info/top_level.txt
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)       38 2022-06-17 08:02:27.000000 channel_app-0.0.99/setup.cfg
+-rw-rw-r--   0 eyupt     (1000) eyupt     (1000)      628 2022-06-17 08:00:34.000000 channel_app-0.0.99/setup.py
```

### Comparing `channel_app-0.0.98/channel_app/app/order/service.py` & `channel_app-0.0.99/channel_app/app/order/service.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/app/product/service.py` & `channel_app-0.0.99/channel_app/app/product/service.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/app/product_image/service.py` & `channel_app-0.0.99/channel_app/app/product_image/service.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/app/product_price/service.py` & `channel_app-0.0.99/channel_app/app/product_price/service.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/app/product_stock/service.py` & `channel_app-0.0.99/channel_app/app/product_stock/service.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/app/setup/service.py` & `channel_app-0.0.99/channel_app/channel_app/app/setup/service.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel/commands/orders/orders.py` & `channel_app-0.0.99/channel_app/channel/commands/orders/orders.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel/commands/product_images.py` & `channel_app-0.0.99/channel_app/channel/commands/product_images.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel/commands/product_prices.py` & `channel_app-0.0.99/channel_app/channel/commands/product_prices.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel/commands/product_stocks.py` & `channel_app-0.0.99/channel_app/channel/commands/product_stocks.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel/commands/products.py` & `channel_app-0.0.99/channel_app/channel/commands/products.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel/commands/setup.py` & `channel_app-0.0.99/channel_app/channel/commands/setup.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel/integration.py` & `channel_app-0.0.99/channel_app/channel/integration.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/app/order/service.py` & `channel_app-0.0.99/channel_app/channel_app/app/order/service.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/app/product/service.py` & `channel_app-0.0.99/channel_app/channel_app/app/product/service.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/app/product_price/service.py` & `channel_app-0.0.99/channel_app/channel_app/app/product_price/service.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/app/product_stock/service.py` & `channel_app-0.0.99/channel_app/channel_app/app/product_stock/service.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/app/setup/service.py` & `channel_app-0.0.99/channel_app/app/setup/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,17 +41,18 @@
                     batch_request=omnitron_integration.batch_request
                 )
                 if report and (is_success_log or not report.is_ok):
                     omnitron_integration.do_action(
                         key='create_error_report',
                         objects=report)
 
+                category = category if category.attributes else None
                 omnitron_integration.do_action(
                     key='create_or_update_category_attributes',
-                    objects=category)
+                    objects=(category_ia, category))
 
     def update_channel_conf_schema(self):
         with OmnitronIntegration(
                 content_type=ContentType.channel.value) as omnitron_integration:
             channel_integration = ChannelIntegration()
             schema, _, _ = channel_integration.do_action(
                 key='get_channel_conf_schema',
```

### Comparing `channel_app-0.0.98/channel_app/channel_app/channel/commands/orders/orders.py` & `channel_app-0.0.99/channel_app/channel_app/channel/commands/orders/orders.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/channel/commands/product_prices.py` & `channel_app-0.0.99/channel_app/channel_app/channel/commands/product_prices.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/channel/commands/product_stocks.py` & `channel_app-0.0.99/channel_app/channel_app/channel/commands/product_stocks.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/channel/commands/products.py` & `channel_app-0.0.99/channel_app/channel_app/channel/commands/products.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/channel/commands/setup.py` & `channel_app-0.0.99/channel_app/channel_app/channel/commands/setup.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/channel/integration.py` & `channel_app-0.0.99/channel_app/channel_app/channel/integration.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/core/commands.py` & `channel_app-0.0.99/channel_app/channel_app/core/commands.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/core/data.py` & `channel_app-0.0.99/channel_app/channel_app/core/data.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/core/integration.py` & `channel_app-0.0.99/channel_app/channel_app/core/integration.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/core/products.py` & `channel_app-0.0.99/channel_app/channel_app/core/products.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/core/settings.py` & `channel_app-0.0.99/channel_app/channel_app/core/settings.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/core/utilities.py` & `channel_app-0.0.99/channel_app/channel_app/core/utilities.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/omnitron/batch_request.py` & `channel_app-0.0.99/channel_app/channel_app/omnitron/batch_request.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/omnitron/commands/batch_requests.py` & `channel_app-0.0.99/channel_app/channel_app/omnitron/commands/batch_requests.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/omnitron/commands/error_reports.py` & `channel_app-0.0.99/channel_app/channel_app/omnitron/commands/error_reports.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/omnitron/commands/integration_actions.py` & `channel_app-0.0.99/channel_app/channel_app/omnitron/commands/integration_actions.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/omnitron/commands/orders/addresses.py` & `channel_app-0.0.99/channel_app/channel_app/omnitron/commands/orders/addresses.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/omnitron/commands/orders/cargo_companies.py` & `channel_app-0.0.99/channel_app/channel_app/omnitron/commands/orders/cargo_companies.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/omnitron/commands/orders/customers.py` & `channel_app-0.0.99/channel_app/channel_app/omnitron/commands/orders/customers.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/omnitron/commands/orders/orders.py` & `channel_app-0.0.99/channel_app/channel_app/omnitron/commands/orders/orders.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/omnitron/commands/product_prices.py` & `channel_app-0.0.99/channel_app/channel_app/omnitron/commands/product_prices.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/omnitron/commands/product_stocks.py` & `channel_app-0.0.99/channel_app/channel_app/omnitron/commands/product_stocks.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/omnitron/commands/products.py` & `channel_app-0.0.99/channel_app/channel_app/omnitron/commands/products.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/omnitron/commands/setup.py` & `channel_app-0.0.99/channel_app/channel_app/omnitron/commands/setup.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/omnitron/constants.py` & `channel_app-0.0.99/channel_app/channel_app/omnitron/constants.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/omnitron/exceptions.py` & `channel_app-0.0.99/channel_app/channel_app/omnitron/exceptions.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/channel_app/omnitron/integration.py` & `channel_app-0.0.99/channel_app/channel_app/omnitron/integration.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/core/commands.py` & `channel_app-0.0.99/channel_app/core/commands.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/core/data.py` & `channel_app-0.0.99/channel_app/core/data.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/core/integration.py` & `channel_app-0.0.99/channel_app/core/integration.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/core/products.py` & `channel_app-0.0.99/channel_app/core/products.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/core/settings.py` & `channel_app-0.0.99/channel_app/core/settings.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/core/utilities.py` & `channel_app-0.0.99/channel_app/core/utilities.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/omnitron/batch_request.py` & `channel_app-0.0.99/channel_app/omnitron/batch_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,59 +24,64 @@
         :param batch_request:
         :return:
         """
         br = BatchRequest(channel=self.channel_id)
         br.objects = batch_request.objects
         br.status = BatchRequestStatus.commit.value
         br.content_type = batch_request.content_type
+        batch_request.status = br.status
         return self.endpoint(channel_id=self.channel_id).update(id=batch_request.pk, item=br)
 
     def to_sent_to_remote(self, batch_request: BatchRequest) -> BatchRequest:
         """
         If objects are sent to channel, state must be updated to sent_to_remote
         and channel batch id is stored if it sent one.
         :param batch_request:
         :return:
         """
         br = BatchRequest(channel=self.channel_id)
         br.remote_batch_id = batch_request.remote_batch_id
         br.status = BatchRequestStatus.sent_to_remote.value
+        batch_request.status = br.status
         return self.endpoint(channel_id=self.channel_id).update(
             id=batch_request.pk, item=br)
 
     def to_ongoing(self, batch_request: BatchRequest) -> BatchRequest:
         """
         If channel has not finished the batch yet, once we query for it after an interval, we
         update the state to ongoing.
         :param batch_request:
         :return:
         """
         br = BatchRequest(channel=self.channel_id)
         br.status = BatchRequestStatus.ongoing.value
+        batch_request.status = br.status
         return self.endpoint(channel_id=self.channel_id).update(
             id=batch_request.pk, item=br)
 
     def to_fail(self, batch_request: BatchRequest) -> BatchRequest:
         """
         If channel fails completing the batch, batch request is finalized with fail state.
         :param batch_request:
         :return:
         """
         br = BatchRequest(channel=self.channel_id)
         br.objects = batch_request.objects
         br.status = BatchRequestStatus.fail.value
+        batch_request.status = br.status
         return self.endpoint(channel_id=self.channel_id).update(
             id=batch_request.pk, item=br)
 
     def to_done(self, batch_request: BatchRequest) -> BatchRequest:
         """
         If all objects are processed disregarding the fact that they succeeded or failed,
         batch request is finalized with done.
         :param batch_request:
         :return:
         """
         br = BatchRequest(channel=self.channel_id)
         br.objects = batch_request.objects
         br.status = BatchRequestStatus.done.value
+        batch_request.status = br.status
         return self.endpoint(channel_id=self.channel_id).update(
             id=batch_request.pk, item=br)
```

### Comparing `channel_app-0.0.98/channel_app/omnitron/commands/batch_requests.py` & `channel_app-0.0.99/channel_app/omnitron/commands/batch_requests.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/omnitron/commands/error_reports.py` & `channel_app-0.0.99/channel_app/omnitron/commands/error_reports.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/omnitron/commands/integration_actions.py` & `channel_app-0.0.99/channel_app/omnitron/commands/integration_actions.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/omnitron/commands/orders/addresses.py` & `channel_app-0.0.99/channel_app/omnitron/commands/orders/addresses.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/omnitron/commands/orders/cargo_companies.py` & `channel_app-0.0.99/channel_app/omnitron/commands/orders/cargo_companies.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/omnitron/commands/orders/customers.py` & `channel_app-0.0.99/channel_app/omnitron/commands/orders/customers.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/omnitron/commands/orders/orders.py` & `channel_app-0.0.99/channel_app/omnitron/commands/orders/orders.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/omnitron/commands/product_images.py` & `channel_app-0.0.99/channel_app/omnitron/commands/product_images.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/omnitron/commands/product_prices.py` & `channel_app-0.0.99/channel_app/omnitron/commands/product_prices.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/omnitron/commands/product_stocks.py` & `channel_app-0.0.99/channel_app/omnitron/commands/product_stocks.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/omnitron/commands/products.py` & `channel_app-0.0.99/channel_app/omnitron/commands/products.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/omnitron/commands/setup.py` & `channel_app-0.0.99/channel_app/omnitron/commands/setup.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/omnitron/constants.py` & `channel_app-0.0.99/channel_app/omnitron/constants.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/omnitron/exceptions.py` & `channel_app-0.0.99/channel_app/omnitron/exceptions.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/omnitron/integration.py` & `channel_app-0.0.99/channel_app/omnitron/integration.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app/setup.py` & `channel_app-0.0.99/channel_app/setup.py`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/channel_app.egg-info/SOURCES.txt` & `channel_app-0.0.99/channel_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `channel_app-0.0.98/setup.py` & `channel_app-0.0.99/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="channel_app",
-    version="0.0.98",
+    version="0.0.99",
     packages=find_packages(),
     url="https://github.com/akinon/channel_app",
     description="Channel app for Sales Channels",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="akinonteam",
     python_requires=">=3.5",
```

