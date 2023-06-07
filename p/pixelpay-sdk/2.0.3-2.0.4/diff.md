# Comparing `tmp/pixelpay-sdk-2.0.3.tar.gz` & `tmp/pixelpay-sdk-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelpay-sdk-2.0.3.tar", last modified: Thu Jan 26 21:36:58 2023, max compression
+gzip compressed data, was "pixelpay-sdk-2.0.4.tar", last modified: Wed Jun  7 22:53:40 2023, max compression
```

## Comparing `pixelpay-sdk-2.0.3.tar` & `pixelpay-sdk-2.0.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-01-26 21:36:58.958286 pixelpay-sdk-2.0.3/
--rw-r--r--   0 javiercano   (501) staff       (20)     1088 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/LICENSE.md
--rw-r--r--   0 javiercano   (501) staff       (20)     1498 2023-01-26 21:36:58.957654 pixelpay-sdk-2.0.3/PKG-INFO
--rw-r--r--   0 javiercano   (501) staff       (20)      996 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/README.md
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-01-26 21:36:58.932178 pixelpay-sdk-2.0.3/pixelpay_sdk.egg-info/
--rw-r--r--   0 javiercano   (501) staff       (20)     1498 2023-01-26 21:36:58.000000 pixelpay-sdk-2.0.3/pixelpay_sdk.egg-info/PKG-INFO
--rw-r--r--   0 javiercano   (501) staff       (20)     2026 2023-01-26 21:36:58.000000 pixelpay-sdk-2.0.3/pixelpay_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 javiercano   (501) staff       (20)        1 2023-01-26 21:36:58.000000 pixelpay-sdk-2.0.3/pixelpay_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 javiercano   (501) staff       (20)       16 2023-01-26 21:36:58.000000 pixelpay-sdk-2.0.3/pixelpay_sdk.egg-info/requires.txt
--rw-r--r--   0 javiercano   (501) staff       (20)        9 2023-01-26 21:36:58.000000 pixelpay-sdk-2.0.3/pixelpay_sdk.egg-info/top_level.txt
--rw-r--r--   0 javiercano   (501) staff       (20)       85 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/pyproject.toml
--rw-r--r--   0 javiercano   (501) staff       (20)       38 2023-01-26 21:36:58.958326 pixelpay-sdk-2.0.3/setup.cfg
--rw-r--r--   0 javiercano   (501) staff       (20)     1380 2022-09-21 22:49:24.000000 pixelpay-sdk-2.0.3/setup.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-01-26 21:36:58.924945 pixelpay-sdk-2.0.3/src/
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-01-26 21:36:58.932457 pixelpay-sdk-2.0.3/src/pixelpay/
--rw-r--r--   0 javiercano   (501) staff       (20)      365 2023-01-26 21:28:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-01-26 21:36:58.934162 pixelpay-sdk-2.0.3/src/pixelpay/assets/
--rw-r--r--   0 javiercano   (501) staff       (20)     5438 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/assets/countries.json
--rw-r--r--   0 javiercano   (501) staff       (20)    18333 2023-01-26 21:25:46.000000 pixelpay-sdk-2.0.3/src/pixelpay/assets/formats.json
--rw-r--r--   0 javiercano   (501) staff       (20)    88971 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/assets/states.json
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-01-26 21:36:58.936615 pixelpay-sdk-2.0.3/src/pixelpay/base/
--rw-r--r--   0 javiercano   (501) staff       (20)     2036 2022-09-21 22:53:20.000000 pixelpay-sdk-2.0.3/src/pixelpay/base/Helpers.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1300 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/base/RequestBehaviour.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1804 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/base/Response.py
--rw-r--r--   0 javiercano   (501) staff       (20)     6898 2022-09-21 22:43:53.000000 pixelpay-sdk-2.0.3/src/pixelpay/base/ServiceBehaviour.py
--rw-r--r--   0 javiercano   (501) staff       (20)      248 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/base/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-01-26 21:36:58.938092 pixelpay-sdk-2.0.3/src/pixelpay/entities/
--rw-r--r--   0 javiercano   (501) staff       (20)     1812 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/entities/CardResult.py
--rw-r--r--   0 javiercano   (501) staff       (20)     3028 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/entities/TransactionResult.py
--rw-r--r--   0 javiercano   (501) staff       (20)      142 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/entities/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-01-26 21:36:58.940322 pixelpay-sdk-2.0.3/src/pixelpay/exceptions/
--rw-r--r--   0 javiercano   (501) staff       (20)       55 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/exceptions/InvalidCredentialsException.py
--rw-r--r--   0 javiercano   (501) staff       (20)       59 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/exceptions/InvalidTransactionTypeException.py
--rw-r--r--   0 javiercano   (501) staff       (20)      235 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/exceptions/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-01-26 21:36:58.946045 pixelpay-sdk-2.0.3/src/pixelpay/models/
--rw-r--r--   0 javiercano   (501) staff       (20)      512 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/models/Billing.py
--rw-r--r--   0 javiercano   (501) staff       (20)      656 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/models/Card.py
--rw-r--r--   0 javiercano   (501) staff       (20)      653 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/models/Item.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1873 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/models/Order.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1841 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/models/Settings.py
--rw-r--r--   0 javiercano   (501) staff       (20)      214 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/models/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-01-26 21:36:58.949058 pixelpay-sdk-2.0.3/src/pixelpay/requests/
--rw-r--r--   0 javiercano   (501) staff       (20)      105 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/requests/AuthTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      358 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/requests/CaptureTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)     2170 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/requests/CardTokenization.py
--rw-r--r--   0 javiercano   (501) staff       (20)     4336 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/requests/PaymentTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)       96 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/requests/SaleTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      198 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/requests/StatusTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      274 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/requests/VoidTransaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      518 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/requests/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-01-26 21:36:58.950021 pixelpay-sdk-2.0.3/src/pixelpay/resources/
--rw-r--r--   0 javiercano   (501) staff       (20)      123 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/resources/Environment.py
--rw-r--r--   0 javiercano   (501) staff       (20)     1657 2023-01-26 21:27:02.000000 pixelpay-sdk-2.0.3/src/pixelpay/resources/Locations.py
--rw-r--r--   0 javiercano   (501) staff       (20)      121 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/resources/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-01-26 21:36:58.956571 pixelpay-sdk-2.0.3/src/pixelpay/responses/
--rw-r--r--   0 javiercano   (501) staff       (20)       70 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/responses/ErrorResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/responses/FailureResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       75 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/responses/InputErrorResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/responses/NetworkFailureResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/responses/NoAccessResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/responses/NotFoundResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/responses/PayloadResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       80 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/responses/PaymentDeclinedResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/responses/PreconditionalResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/responses/SuccessResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/responses/TimeoutResponse.py
--rw-r--r--   0 javiercano   (501) staff       (20)      838 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/responses/__init__.py
-drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-01-26 21:36:58.957359 pixelpay-sdk-2.0.3/src/pixelpay/services/
--rw-r--r--   0 javiercano   (501) staff       (20)     2081 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/services/Tokenization.py
--rw-r--r--   0 javiercano   (501) staff       (20)     2471 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/services/Transaction.py
--rw-r--r--   0 javiercano   (501) staff       (20)      130 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.3/src/pixelpay/services/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-06-07 22:53:40.641168 pixelpay-sdk-2.0.4/
+-rw-r--r--   0 javiercano   (501) staff       (20)     1088 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/LICENSE.md
+-rw-r--r--   0 javiercano   (501) staff       (20)      957 2023-06-07 22:53:40.641003 pixelpay-sdk-2.0.4/PKG-INFO
+-rw-r--r--   0 javiercano   (501) staff       (20)      455 2023-06-07 22:52:21.000000 pixelpay-sdk-2.0.4/README.md
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-06-07 22:53:40.620975 pixelpay-sdk-2.0.4/pixelpay_sdk.egg-info/
+-rw-r--r--   0 javiercano   (501) staff       (20)      957 2023-06-07 22:53:40.000000 pixelpay-sdk-2.0.4/pixelpay_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 javiercano   (501) staff       (20)     2026 2023-06-07 22:53:40.000000 pixelpay-sdk-2.0.4/pixelpay_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)        1 2023-06-07 22:53:40.000000 pixelpay-sdk-2.0.4/pixelpay_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)       16 2023-06-07 22:53:40.000000 pixelpay-sdk-2.0.4/pixelpay_sdk.egg-info/requires.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)        9 2023-06-07 22:53:40.000000 pixelpay-sdk-2.0.4/pixelpay_sdk.egg-info/top_level.txt
+-rw-r--r--   0 javiercano   (501) staff       (20)       85 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/pyproject.toml
+-rw-r--r--   0 javiercano   (501) staff       (20)       38 2023-06-07 22:53:40.641206 pixelpay-sdk-2.0.4/setup.cfg
+-rw-r--r--   0 javiercano   (501) staff       (20)     1380 2022-09-21 22:49:24.000000 pixelpay-sdk-2.0.4/setup.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-06-07 22:53:40.610257 pixelpay-sdk-2.0.4/src/
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-06-07 22:53:40.621216 pixelpay-sdk-2.0.4/src/pixelpay/
+-rw-r--r--   0 javiercano   (501) staff       (20)      365 2023-06-07 22:45:09.000000 pixelpay-sdk-2.0.4/src/pixelpay/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-06-07 22:53:40.622488 pixelpay-sdk-2.0.4/src/pixelpay/assets/
+-rw-r--r--   0 javiercano   (501) staff       (20)     5438 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/assets/countries.json
+-rw-r--r--   0 javiercano   (501) staff       (20)    18333 2023-01-26 21:25:46.000000 pixelpay-sdk-2.0.4/src/pixelpay/assets/formats.json
+-rw-r--r--   0 javiercano   (501) staff       (20)    88971 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/assets/states.json
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-06-07 22:53:40.624424 pixelpay-sdk-2.0.4/src/pixelpay/base/
+-rw-r--r--   0 javiercano   (501) staff       (20)     2036 2022-09-21 22:53:20.000000 pixelpay-sdk-2.0.4/src/pixelpay/base/Helpers.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1300 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/base/RequestBehaviour.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1804 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/base/Response.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     6898 2022-09-21 22:43:53.000000 pixelpay-sdk-2.0.4/src/pixelpay/base/ServiceBehaviour.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      248 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/base/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-06-07 22:53:40.625295 pixelpay-sdk-2.0.4/src/pixelpay/entities/
+-rw-r--r--   0 javiercano   (501) staff       (20)     1812 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/entities/CardResult.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     3028 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/entities/TransactionResult.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      142 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/entities/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-06-07 22:53:40.626455 pixelpay-sdk-2.0.4/src/pixelpay/exceptions/
+-rw-r--r--   0 javiercano   (501) staff       (20)       55 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/exceptions/InvalidCredentialsException.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       59 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/exceptions/InvalidTransactionTypeException.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      235 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/exceptions/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-06-07 22:53:40.628793 pixelpay-sdk-2.0.4/src/pixelpay/models/
+-rw-r--r--   0 javiercano   (501) staff       (20)      512 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/models/Billing.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      656 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/models/Card.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      653 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/models/Item.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1873 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/models/Order.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1841 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/models/Settings.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      214 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/models/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-06-07 22:53:40.633312 pixelpay-sdk-2.0.4/src/pixelpay/requests/
+-rw-r--r--   0 javiercano   (501) staff       (20)      105 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/requests/AuthTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      358 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/requests/CaptureTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     2170 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/requests/CardTokenization.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     4336 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/requests/PaymentTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1020 2023-06-07 22:41:02.000000 pixelpay-sdk-2.0.4/src/pixelpay/requests/SaleTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      198 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/requests/StatusTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      372 2023-06-07 22:21:17.000000 pixelpay-sdk-2.0.4/src/pixelpay/requests/VoidTransaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      518 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/requests/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-06-07 22:53:40.634967 pixelpay-sdk-2.0.4/src/pixelpay/resources/
+-rw-r--r--   0 javiercano   (501) staff       (20)      123 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/resources/Environment.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     1657 2023-01-26 21:27:02.000000 pixelpay-sdk-2.0.4/src/pixelpay/resources/Locations.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      121 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/resources/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-06-07 22:53:40.639249 pixelpay-sdk-2.0.4/src/pixelpay/responses/
+-rw-r--r--   0 javiercano   (501) staff       (20)       70 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/responses/ErrorResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/responses/FailureResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       75 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/responses/InputErrorResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/responses/NetworkFailureResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/responses/NoAccessResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       73 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/responses/NotFoundResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/responses/PayloadResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       80 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/responses/PaymentDeclinedResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       79 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/responses/PreconditionalResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/responses/SuccessResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)       72 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/responses/TimeoutResponse.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      838 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/responses/__init__.py
+drwxr-xr-x   0 javiercano   (501) staff       (20)        0 2023-06-07 22:53:40.640736 pixelpay-sdk-2.0.4/src/pixelpay/services/
+-rw-r--r--   0 javiercano   (501) staff       (20)     2081 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/services/Tokenization.py
+-rw-r--r--   0 javiercano   (501) staff       (20)     2471 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/services/Transaction.py
+-rw-r--r--   0 javiercano   (501) staff       (20)      130 2022-09-21 22:36:22.000000 pixelpay-sdk-2.0.4/src/pixelpay/services/__init__.py
```

### Comparing `pixelpay-sdk-2.0.3/LICENSE.md` & `pixelpay-sdk-2.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/pixelpay_sdk.egg-info/SOURCES.txt` & `pixelpay-sdk-2.0.4/pixelpay_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/setup.py` & `pixelpay-sdk-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/assets/countries.json` & `pixelpay-sdk-2.0.4/src/pixelpay/assets/countries.json`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/assets/formats.json` & `pixelpay-sdk-2.0.4/src/pixelpay/assets/formats.json`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/assets/states.json` & `pixelpay-sdk-2.0.4/src/pixelpay/assets/states.json`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/base/Helpers.py` & `pixelpay-sdk-2.0.4/src/pixelpay/base/Helpers.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/base/RequestBehaviour.py` & `pixelpay-sdk-2.0.4/src/pixelpay/base/RequestBehaviour.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/base/Response.py` & `pixelpay-sdk-2.0.4/src/pixelpay/base/Response.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/base/ServiceBehaviour.py` & `pixelpay-sdk-2.0.4/src/pixelpay/base/ServiceBehaviour.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/entities/CardResult.py` & `pixelpay-sdk-2.0.4/src/pixelpay/entities/CardResult.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/entities/TransactionResult.py` & `pixelpay-sdk-2.0.4/src/pixelpay/entities/TransactionResult.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/models/Billing.py` & `pixelpay-sdk-2.0.4/src/pixelpay/models/Billing.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/models/Card.py` & `pixelpay-sdk-2.0.4/src/pixelpay/models/Card.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/models/Item.py` & `pixelpay-sdk-2.0.4/src/pixelpay/models/Item.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/models/Order.py` & `pixelpay-sdk-2.0.4/src/pixelpay/models/Order.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/models/Settings.py` & `pixelpay-sdk-2.0.4/src/pixelpay/models/Settings.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/requests/CardTokenization.py` & `pixelpay-sdk-2.0.4/src/pixelpay/requests/CardTokenization.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/requests/PaymentTransaction.py` & `pixelpay-sdk-2.0.4/src/pixelpay/requests/PaymentTransaction.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/requests/__init__.py` & `pixelpay-sdk-2.0.4/src/pixelpay/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/resources/Locations.py` & `pixelpay-sdk-2.0.4/src/pixelpay/resources/Locations.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/responses/__init__.py` & `pixelpay-sdk-2.0.4/src/pixelpay/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/services/Tokenization.py` & `pixelpay-sdk-2.0.4/src/pixelpay/services/Tokenization.py`

 * *Files identical despite different names*

### Comparing `pixelpay-sdk-2.0.3/src/pixelpay/services/Transaction.py` & `pixelpay-sdk-2.0.4/src/pixelpay/services/Transaction.py`

 * *Files identical despite different names*

