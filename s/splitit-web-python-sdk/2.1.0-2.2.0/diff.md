# Comparing `tmp/splitit-web-python-sdk-2.1.0.tar.gz` & `tmp/splitit_web_python_sdk-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/dylanhuang/Git/konfig-monorepo/customers/splitit/splitit-web-sdks/python/dist/.tmp-vb1jd08t/splitit-web-python-sdk-2.1.0", last modified: Tue Apr 25 03:35:48 2023, max compression
+gzip compressed data, was "splitit_web_python_sdk-2.2.0.tar", max compression
```

## Comparing `splitit-web-python-sdk-2.1.0.tar` & `splitit_web_python_sdk-2.2.0.tar`

### file list

```diff
@@ -1,220 +1,228 @@
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1081 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/LICENSE
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7565 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/PKG-INFO
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7205 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/README.md
--rw-r--r--   0 dylanhuang   (501) staff       (20)       69 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/setup.cfg
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1319 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/setup.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      725 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    64438 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/api_client.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      266 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/api_response.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      214 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3411 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/path_to_api.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      241 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      127 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      161 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_check_eligibility.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      144 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_initiate.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      169 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      185 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_cancel.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      185 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_refund.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      192 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_updateorder.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      208 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_verifyauthorization.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      137 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_search.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      147 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/paths/api_installmentplans_updateorder.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      371 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/tag_to_api.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/tags/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      328 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/tags/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1333 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/apis/tags/installment_plan_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      713 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/client.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    18376 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/configuration.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5627 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/exceptions.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2274 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/exceptions_base.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      348 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4871 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/address_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4894 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/address_data_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7418 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/authorization_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1752 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/card_brand.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5874 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/card_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1571 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/card_type.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3738 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/check_installments_eligibility_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3357 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/error.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5464 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/error_extended.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2898 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/failed_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1188 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/gw_authorization_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4856 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/identifier_contract.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     9111 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/initiate_plan_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3361 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/initiate_redirection_endpoints_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4303 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2499 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_cancel_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7348 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_create_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13350 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_create_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    14794 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_get_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6528 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_initiate_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3076 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_refund_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5607 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_refund_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3421 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_search_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4250 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_update_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4385 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_update_request_by_identifier.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4417 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_update_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1082 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installment_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3487 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/installments_eligibility_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4052 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/links_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3679 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/links_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3476 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/payment_method_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      962 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/payment_method_type.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5439 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/payment_plan_option_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    10239 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/plan_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     8734 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/plan_data_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4276 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/plan_error_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1345 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/plan_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1091 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/purchase_method.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4123 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/redirection_endpoints_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5623 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/refund_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1069 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/refund_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1485 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/refund_strategy.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4246 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/refund_summary.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    14808 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/search_installment_plan_response_item.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1075 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/shipping_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      958 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/shipping_status2.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3874 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/shopper_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1168 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/test_modes.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4386 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/three_ds_redirect_data_v3.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4223 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/update_order_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3409 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/ux_settings_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3864 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/model/verify_authorization_response.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/models/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4289 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/models/__init__.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1223 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/__init__.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      327 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    27024 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_check_eligibility/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      362 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_check_eligibility/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    25504 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_initiate/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      345 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_initiate/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    26975 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_initiate/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      375 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    16100 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      389 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    16154 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      389 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    28110 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      399 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    28130 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      415 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    16290 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_search/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      341 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_search/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    17890 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_search/get.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_updateorder/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      351 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_updateorder/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    25455 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_updateorder/put.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      639 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/request_after_hook.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      640 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/request_before_hook.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    10671 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/rest.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    95047 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/schemas.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3170 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/splitit_client/validation_metadata.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_web_python_sdk.egg-info/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7565 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_web_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dylanhuang   (501) staff       (20)     9561 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_web_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)        1 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_web_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)      139 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_web_python_sdk.egg-info/requires.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)       20 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/splitit_web_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2878 2023-04-25 03:29:08.000000 splitit-web-python-sdk-2.1.0/test/test_installment_plan_api_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_models/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      439 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_address_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      460 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_address_data_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      467 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_authorization_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      431 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_card_brand.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      427 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_card_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      427 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_card_type.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      537 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_check_installments_eligibility_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      414 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_error.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      447 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_error_extended.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      451 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_failed_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      480 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_gw_authorization_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      467 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_identifier_contract.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      476 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_initiate_plan_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      529 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_initiate_redirection_endpoints_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      438 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      513 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_cancel_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      509 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_create_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      513 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_create_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      501 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_get_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      517 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_initiate_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      509 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_refund_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      513 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_refund_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      513 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_search_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      509 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_update_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      559 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_update_request_by_identifier.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      513 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_update_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      463 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installment_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      520 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_installments_eligibility_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      431 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_links_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      435 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_links_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      468 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_payment_method_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      464 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_payment_method_type.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      485 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_payment_plan_option_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      427 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_plan_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      448 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_plan_data_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      464 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_plan_error_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      435 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_plan_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      451 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_purchase_method.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      496 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_redirection_endpoints_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      439 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_refund_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      443 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_refund_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      451 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_refund_strategy.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      447 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_refund_summary.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      530 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_search_installment_plan_response_item.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      451 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_shipping_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      455 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_shipping_status2.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      439 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_shopper_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      431 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_test_modes.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      482 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_three_ds_redirect_data_v3.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      468 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_update_order_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      456 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_ux_settings_model.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      504 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_models/test_verify_authorization_response.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1984 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/__init__.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      683 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_check_eligibility/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_check_eligibility/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      733 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_check_eligibility/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_initiate/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_initiate/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      708 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_initiate/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      740 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number/test_get.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_cancel/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_cancel/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      760 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_cancel/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_refund/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_refund/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      768 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_refund/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_updateorder/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_updateorder/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      782 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_updateorder/test_put.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_verifyauthorization/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_verifyauthorization/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      798 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_verifyauthorization/test_get.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_search/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_search/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      693 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_search/test_get.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:35:48.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_updateorder/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_updateorder/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      716 2023-04-25 03:28:00.000000 splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_updateorder/test_put.py
+-rw-r--r--   0        0        0     1081 2023-06-08 11:55:07.661154 splitit_web_python_sdk-2.2.0/LICENSE
+-rw-r--r--   0        0        0     8335 2023-06-08 11:55:07.728491 splitit_web_python_sdk-2.2.0/README.md
+-rw-r--r--   0        0        0      737 2023-06-08 11:55:07.608986 splitit_web_python_sdk-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      725 2023-06-08 11:55:07.609258 splitit_web_python_sdk-2.2.0/splitit_client/__init__.py
+-rw-r--r--   0        0        0    73578 2023-06-08 11:55:07.609403 splitit_web_python_sdk-2.2.0/splitit_client/api_client.py
+-rw-r--r--   0        0        0      663 2023-06-08 11:55:07.609506 splitit_web_python_sdk-2.2.0/splitit_client/api_response.py
+-rw-r--r--   0        0        0      214 2023-06-08 11:55:07.609599 splitit_web_python_sdk-2.2.0/splitit_client/apis/__init__.py
+-rw-r--r--   0        0        0     3411 2023-06-08 11:55:07.609690 splitit_web_python_sdk-2.2.0/splitit_client/apis/path_to_api.py
+-rw-r--r--   0        0        0      241 2023-06-08 11:55:07.609784 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/__init__.py
+-rw-r--r--   0        0        0      127 2023-06-08 11:55:07.609867 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans.py
+-rw-r--r--   0        0        0      161 2023-06-08 11:55:07.609966 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_check_eligibility.py
+-rw-r--r--   0        0        0      144 2023-06-08 11:55:07.610068 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_initiate.py
+-rw-r--r--   0        0        0      169 2023-06-08 11:55:07.610169 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number.py
+-rw-r--r--   0        0        0      185 2023-06-08 11:55:07.610276 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_cancel.py
+-rw-r--r--   0        0        0      185 2023-06-08 11:55:07.610372 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_refund.py
+-rw-r--r--   0        0        0      192 2023-06-08 11:55:07.610472 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_updateorder.py
+-rw-r--r--   0        0        0      208 2023-06-08 11:55:07.610580 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_installment_plan_number_verifyauthorization.py
+-rw-r--r--   0        0        0      137 2023-06-08 11:55:07.610666 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_search.py
+-rw-r--r--   0        0        0      147 2023-06-08 11:55:07.610751 splitit_web_python_sdk-2.2.0/splitit_client/apis/paths/api_installmentplans_updateorder.py
+-rw-r--r--   0        0        0      371 2023-06-08 11:55:07.610827 splitit_web_python_sdk-2.2.0/splitit_client/apis/tag_to_api.py
+-rw-r--r--   0        0        0      328 2023-06-08 11:55:07.610917 splitit_web_python_sdk-2.2.0/splitit_client/apis/tags/__init__.py
+-rw-r--r--   0        0        0     1333 2023-06-08 11:55:07.610998 splitit_web_python_sdk-2.2.0/splitit_client/apis/tags/installment_plan_api.py
+-rw-r--r--   0        0        0      989 2023-06-08 11:55:07.611082 splitit_web_python_sdk-2.2.0/splitit_client/client.py
+-rw-r--r--   0        0        0      989 2023-06-08 11:55:07.611166 splitit_web_python_sdk-2.2.0/splitit_client/client.pyi
+-rw-r--r--   0        0        0      669 2023-06-08 11:55:07.611270 splitit_web_python_sdk-2.2.0/splitit_client/client_custom.py
+-rw-r--r--   0        0        0    18575 2023-06-08 11:55:07.611375 splitit_web_python_sdk-2.2.0/splitit_client/configuration.py
+-rw-r--r--   0        0        0     7311 2023-06-08 11:55:07.611475 splitit_web_python_sdk-2.2.0/splitit_client/exceptions.py
+-rw-r--r--   0        0        0     2274 2023-06-08 11:55:07.611606 splitit_web_python_sdk-2.2.0/splitit_client/exceptions_base.py
+-rw-r--r--   0        0        0      348 2023-06-08 11:55:07.611770 splitit_web_python_sdk-2.2.0/splitit_client/model/__init__.py
+-rw-r--r--   0        0        0     4871 2023-06-08 11:55:07.611881 splitit_web_python_sdk-2.2.0/splitit_client/model/address_data.py
+-rw-r--r--   0        0        0     4871 2023-06-08 11:55:07.612011 splitit_web_python_sdk-2.2.0/splitit_client/model/address_data.pyi
+-rw-r--r--   0        0        0     4894 2023-06-08 11:55:07.612152 splitit_web_python_sdk-2.2.0/splitit_client/model/address_data_model.py
+-rw-r--r--   0        0        0     4894 2023-06-08 11:55:07.612282 splitit_web_python_sdk-2.2.0/splitit_client/model/address_data_model.pyi
+-rw-r--r--   0        0        0     7418 2023-06-08 11:55:07.612459 splitit_web_python_sdk-2.2.0/splitit_client/model/authorization_model.py
+-rw-r--r--   0        0        0     7418 2023-06-08 11:55:07.612659 splitit_web_python_sdk-2.2.0/splitit_client/model/authorization_model.pyi
+-rw-r--r--   0        0        0     1752 2023-06-08 11:55:07.612803 splitit_web_python_sdk-2.2.0/splitit_client/model/card_brand.py
+-rw-r--r--   0        0        0     1392 2023-06-08 11:55:07.613150 splitit_web_python_sdk-2.2.0/splitit_client/model/card_brand.pyi
+-rw-r--r--   0        0        0     5874 2023-06-08 11:55:07.614295 splitit_web_python_sdk-2.2.0/splitit_client/model/card_data.py
+-rw-r--r--   0        0        0     5874 2023-06-08 11:55:07.614545 splitit_web_python_sdk-2.2.0/splitit_client/model/card_data.pyi
+-rw-r--r--   0        0        0     1571 2023-06-08 11:55:07.614764 splitit_web_python_sdk-2.2.0/splitit_client/model/card_type.py
+-rw-r--r--   0        0        0     1251 2023-06-08 11:55:07.615025 splitit_web_python_sdk-2.2.0/splitit_client/model/card_type.pyi
+-rw-r--r--   0        0        0     3738 2023-06-08 11:55:07.615263 splitit_web_python_sdk-2.2.0/splitit_client/model/check_installments_eligibility_request.py
+-rw-r--r--   0        0        0     3738 2023-06-08 11:55:07.615455 splitit_web_python_sdk-2.2.0/splitit_client/model/check_installments_eligibility_request.pyi
+-rw-r--r--   0        0        0     3357 2023-06-08 11:55:07.615654 splitit_web_python_sdk-2.2.0/splitit_client/model/error.py
+-rw-r--r--   0        0        0     3357 2023-06-08 11:55:07.615875 splitit_web_python_sdk-2.2.0/splitit_client/model/error.pyi
+-rw-r--r--   0        0        0     5464 2023-06-08 11:55:07.616090 splitit_web_python_sdk-2.2.0/splitit_client/model/error_extended.py
+-rw-r--r--   0        0        0     5464 2023-06-08 11:55:07.616340 splitit_web_python_sdk-2.2.0/splitit_client/model/error_extended.pyi
+-rw-r--r--   0        0        0     2403 2023-06-08 11:55:07.616513 splitit_web_python_sdk-2.2.0/splitit_client/model/events_endpoints_model.py
+-rw-r--r--   0        0        0     2403 2023-06-08 11:55:07.616728 splitit_web_python_sdk-2.2.0/splitit_client/model/events_endpoints_model.pyi
+-rw-r--r--   0        0        0     2898 2023-06-08 11:55:07.616934 splitit_web_python_sdk-2.2.0/splitit_client/model/failed_response.py
+-rw-r--r--   0        0        0     2898 2023-06-08 11:55:07.617117 splitit_web_python_sdk-2.2.0/splitit_client/model/failed_response.pyi
+-rw-r--r--   0        0        0     1188 2023-06-08 11:55:07.617353 splitit_web_python_sdk-2.2.0/splitit_client/model/gw_authorization_status.py
+-rw-r--r--   0        0        0      991 2023-06-08 11:55:07.617536 splitit_web_python_sdk-2.2.0/splitit_client/model/gw_authorization_status.pyi
+-rw-r--r--   0        0        0     4856 2023-06-08 11:55:07.617737 splitit_web_python_sdk-2.2.0/splitit_client/model/identifier_contract.py
+-rw-r--r--   0        0        0     4856 2023-06-08 11:55:07.617931 splitit_web_python_sdk-2.2.0/splitit_client/model/identifier_contract.pyi
+-rw-r--r--   0        0        0     9111 2023-06-08 11:55:07.618119 splitit_web_python_sdk-2.2.0/splitit_client/model/initiate_plan_response.py
+-rw-r--r--   0        0        0     9111 2023-06-08 11:55:07.618407 splitit_web_python_sdk-2.2.0/splitit_client/model/initiate_plan_response.pyi
+-rw-r--r--   0        0        0     3361 2023-06-08 11:55:07.618623 splitit_web_python_sdk-2.2.0/splitit_client/model/initiate_redirection_endpoints_model.py
+-rw-r--r--   0        0        0     3361 2023-06-08 11:55:07.618837 splitit_web_python_sdk-2.2.0/splitit_client/model/initiate_redirection_endpoints_model.pyi
+-rw-r--r--   0        0        0     4303 2023-06-08 11:55:07.619012 splitit_web_python_sdk-2.2.0/splitit_client/model/installment.py
+-rw-r--r--   0        0        0     4303 2023-06-08 11:55:07.619174 splitit_web_python_sdk-2.2.0/splitit_client/model/installment.pyi
+-rw-r--r--   0        0        0     2499 2023-06-08 11:55:07.619339 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_cancel_response.py
+-rw-r--r--   0        0        0     2499 2023-06-08 11:55:07.619519 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_cancel_response.pyi
+-rw-r--r--   0        0        0     8108 2023-06-08 11:55:07.619690 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_create_request.py
+-rw-r--r--   0        0        0     8108 2023-06-08 11:55:07.619867 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_create_request.pyi
+-rw-r--r--   0        0        0    13350 2023-06-08 11:55:07.620058 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_create_response.py
+-rw-r--r--   0        0        0    13350 2023-06-08 11:55:07.620321 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_create_response.pyi
+-rw-r--r--   0        0        0    14794 2023-06-08 11:55:07.620550 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_get_response.py
+-rw-r--r--   0        0        0    14794 2023-06-08 11:55:07.620813 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_get_response.pyi
+-rw-r--r--   0        0        0     7288 2023-06-08 11:55:07.621012 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_initiate_request.py
+-rw-r--r--   0        0        0     7288 2023-06-08 11:55:07.621180 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_initiate_request.pyi
+-rw-r--r--   0        0        0     3076 2023-06-08 11:55:07.621340 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_refund_request.py
+-rw-r--r--   0        0        0     3076 2023-06-08 11:55:07.621495 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_refund_request.pyi
+-rw-r--r--   0        0        0     5607 2023-06-08 11:55:07.621648 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_refund_response.py
+-rw-r--r--   0        0        0     5607 2023-06-08 11:55:07.621798 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_refund_response.pyi
+-rw-r--r--   0        0        0     3421 2023-06-08 11:55:07.621975 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_search_response.py
+-rw-r--r--   0        0        0     3421 2023-06-08 11:55:07.622151 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_search_response.pyi
+-rw-r--r--   0        0        0     4250 2023-06-08 11:55:07.622311 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_request.py
+-rw-r--r--   0        0        0     4250 2023-06-08 11:55:07.622459 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_request.pyi
+-rw-r--r--   0        0        0     4385 2023-06-08 11:55:07.622625 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_request_by_identifier.py
+-rw-r--r--   0        0        0     4385 2023-06-08 11:55:07.622741 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_request_by_identifier.pyi
+-rw-r--r--   0        0        0     4417 2023-06-08 11:55:07.622851 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_response.py
+-rw-r--r--   0        0        0     4417 2023-06-08 11:55:07.623017 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_response.pyi
+-rw-r--r--   0        0        0     1082 2023-06-08 11:55:07.623194 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_status.py
+-rw-r--r--   0        0        0      911 2023-06-08 11:55:07.623364 splitit_web_python_sdk-2.2.0/splitit_client/model/installment_status.pyi
+-rw-r--r--   0        0        0     3487 2023-06-08 11:55:07.623535 splitit_web_python_sdk-2.2.0/splitit_client/model/installments_eligibility_response.py
+-rw-r--r--   0        0        0     3487 2023-06-08 11:55:07.623694 splitit_web_python_sdk-2.2.0/splitit_client/model/installments_eligibility_response.pyi
+-rw-r--r--   0        0        0     4052 2023-06-08 11:55:07.623836 splitit_web_python_sdk-2.2.0/splitit_client/model/links_data.py
+-rw-r--r--   0        0        0     4052 2023-06-08 11:55:07.623973 splitit_web_python_sdk-2.2.0/splitit_client/model/links_data.pyi
+-rw-r--r--   0        0        0     3679 2023-06-08 11:55:07.624168 splitit_web_python_sdk-2.2.0/splitit_client/model/links_model.py
+-rw-r--r--   0        0        0     3679 2023-06-08 11:55:07.624392 splitit_web_python_sdk-2.2.0/splitit_client/model/links_model.pyi
+-rw-r--r--   0        0        0     3476 2023-06-08 11:55:07.624544 splitit_web_python_sdk-2.2.0/splitit_client/model/payment_method_model.py
+-rw-r--r--   0        0        0     3476 2023-06-08 11:55:07.624699 splitit_web_python_sdk-2.2.0/splitit_client/model/payment_method_model.pyi
+-rw-r--r--   0        0        0      962 2023-06-08 11:55:07.624839 splitit_web_python_sdk-2.2.0/splitit_client/model/payment_method_type.py
+-rw-r--r--   0        0        0      826 2023-06-08 11:55:07.624967 splitit_web_python_sdk-2.2.0/splitit_client/model/payment_method_type.pyi
+-rw-r--r--   0        0        0     5439 2023-06-08 11:55:07.625086 splitit_web_python_sdk-2.2.0/splitit_client/model/payment_plan_option_model.py
+-rw-r--r--   0        0        0     5439 2023-06-08 11:55:07.625185 splitit_web_python_sdk-2.2.0/splitit_client/model/payment_plan_option_model.pyi
+-rw-r--r--   0        0        0    10239 2023-06-08 11:55:07.625299 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_data.py
+-rw-r--r--   0        0        0    10239 2023-06-08 11:55:07.625458 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_data.pyi
+-rw-r--r--   0        0        0     8734 2023-06-08 11:55:07.625663 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_data_model.py
+-rw-r--r--   0        0        0     8734 2023-06-08 11:55:07.625993 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_data_model.pyi
+-rw-r--r--   0        0        0     4276 2023-06-08 11:55:07.626176 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_error_response.py
+-rw-r--r--   0        0        0     4276 2023-06-08 11:55:07.626323 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_error_response.pyi
+-rw-r--r--   0        0        0     1345 2023-06-08 11:55:07.626538 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_status.py
+-rw-r--r--   0        0        0     1089 2023-06-08 11:55:07.626665 splitit_web_python_sdk-2.2.0/splitit_client/model/plan_status.pyi
+-rw-r--r--   0        0        0     1091 2023-06-08 11:55:07.626772 splitit_web_python_sdk-2.2.0/splitit_client/model/purchase_method.py
+-rw-r--r--   0        0        0      914 2023-06-08 11:55:07.626932 splitit_web_python_sdk-2.2.0/splitit_client/model/purchase_method.pyi
+-rw-r--r--   0        0        0     4123 2023-06-08 11:55:07.627130 splitit_web_python_sdk-2.2.0/splitit_client/model/redirection_endpoints_model.py
+-rw-r--r--   0        0        0     4123 2023-06-08 11:55:07.627292 splitit_web_python_sdk-2.2.0/splitit_client/model/redirection_endpoints_model.pyi
+-rw-r--r--   0        0        0     5623 2023-06-08 11:55:07.627437 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_model.py
+-rw-r--r--   0        0        0     5623 2023-06-08 11:55:07.627588 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_model.pyi
+-rw-r--r--   0        0        0     1069 2023-06-08 11:55:07.627728 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_status.py
+-rw-r--r--   0        0        0      902 2023-06-08 11:55:07.627871 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_status.pyi
+-rw-r--r--   0        0        0     1485 2023-06-08 11:55:07.628015 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_strategy.py
+-rw-r--r--   0        0        0     1136 2023-06-08 11:55:07.628156 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_strategy.pyi
+-rw-r--r--   0        0        0     4246 2023-06-08 11:55:07.628294 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_summary.py
+-rw-r--r--   0        0        0     4246 2023-06-08 11:55:07.628421 splitit_web_python_sdk-2.2.0/splitit_client/model/refund_summary.pyi
+-rw-r--r--   0        0        0    14808 2023-06-08 11:55:07.628600 splitit_web_python_sdk-2.2.0/splitit_client/model/search_installment_plan_response_item.py
+-rw-r--r--   0        0        0    14808 2023-06-08 11:55:07.628825 splitit_web_python_sdk-2.2.0/splitit_client/model/search_installment_plan_response_item.pyi
+-rw-r--r--   0        0        0     1075 2023-06-08 11:55:07.629036 splitit_web_python_sdk-2.2.0/splitit_client/model/shipping_status.py
+-rw-r--r--   0        0        0      906 2023-06-08 11:55:07.629183 splitit_web_python_sdk-2.2.0/splitit_client/model/shipping_status.pyi
+-rw-r--r--   0        0        0      958 2023-06-08 11:55:07.629328 splitit_web_python_sdk-2.2.0/splitit_client/model/shipping_status2.py
+-rw-r--r--   0        0        0      823 2023-06-08 11:55:07.629467 splitit_web_python_sdk-2.2.0/splitit_client/model/shipping_status2.pyi
+-rw-r--r--   0        0        0     3874 2023-06-08 11:55:07.629607 splitit_web_python_sdk-2.2.0/splitit_client/model/shopper_data.py
+-rw-r--r--   0        0        0     3874 2023-06-08 11:55:07.629749 splitit_web_python_sdk-2.2.0/splitit_client/model/shopper_data.pyi
+-rw-r--r--   0        0        0     1168 2023-06-08 11:55:07.629883 splitit_web_python_sdk-2.2.0/splitit_client/model/test_modes.py
+-rw-r--r--   0        0        0      975 2023-06-08 11:55:07.630028 splitit_web_python_sdk-2.2.0/splitit_client/model/test_modes.pyi
+-rw-r--r--   0        0        0     4386 2023-06-08 11:55:07.630166 splitit_web_python_sdk-2.2.0/splitit_client/model/three_ds_redirect_data_v3.py
+-rw-r--r--   0        0        0     4386 2023-06-08 11:55:07.630313 splitit_web_python_sdk-2.2.0/splitit_client/model/three_ds_redirect_data_v3.pyi
+-rw-r--r--   0        0        0     4223 2023-06-08 11:55:07.630452 splitit_web_python_sdk-2.2.0/splitit_client/model/update_order_request.py
+-rw-r--r--   0        0        0     4223 2023-06-08 11:55:07.630611 splitit_web_python_sdk-2.2.0/splitit_client/model/update_order_request.pyi
+-rw-r--r--   0        0        0     3409 2023-06-08 11:55:07.630805 splitit_web_python_sdk-2.2.0/splitit_client/model/ux_settings_model.py
+-rw-r--r--   0        0        0     3409 2023-06-08 11:55:07.630994 splitit_web_python_sdk-2.2.0/splitit_client/model/ux_settings_model.pyi
+-rw-r--r--   0        0        0     3864 2023-06-08 11:55:07.631158 splitit_web_python_sdk-2.2.0/splitit_client/model/verify_authorization_response.py
+-rw-r--r--   0        0        0     3864 2023-06-08 11:55:07.631312 splitit_web_python_sdk-2.2.0/splitit_client/model/verify_authorization_response.pyi
+-rw-r--r--   0        0        0     4366 2023-06-08 11:55:07.631475 splitit_web_python_sdk-2.2.0/splitit_client/models/__init__.py
+-rw-r--r--   0        0        0     1223 2023-06-08 11:55:07.631644 splitit_web_python_sdk-2.2.0/splitit_client/paths/__init__.py
+-rw-r--r--   0        0        0      327 2023-06-08 11:55:07.631809 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans/__init__.py
+-rw-r--r--   0        0        0    26616 2023-06-08 11:55:07.632095 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans/post.py
+-rw-r--r--   0        0        0    26167 2023-06-08 11:55:07.632436 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans/post.pyi
+-rw-r--r--   0        0        0      362 2023-06-08 11:55:07.632672 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_check_eligibility/__init__.py
+-rw-r--r--   0        0        0    20196 2023-06-08 11:55:07.632883 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py
+-rw-r--r--   0        0        0    19970 2023-06-08 11:55:07.633184 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_check_eligibility/post.pyi
+-rw-r--r--   0        0        0      345 2023-06-08 11:55:07.633396 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_initiate/__init__.py
+-rw-r--r--   0        0        0    25887 2023-06-08 11:55:07.633659 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_initiate/post.py
+-rw-r--r--   0        0        0    25438 2023-06-08 11:55:07.634029 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_initiate/post.pyi
+-rw-r--r--   0        0        0      375 2023-06-08 11:55:07.634244 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number/__init__.py
+-rw-r--r--   0        0        0    17857 2023-06-08 11:55:07.634480 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py
+-rw-r--r--   0        0        0    17631 2023-06-08 11:55:07.634734 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.pyi
+-rw-r--r--   0        0        0      389 2023-06-08 11:55:07.634943 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/__init__.py
+-rw-r--r--   0        0        0    17934 2023-06-08 11:55:07.635161 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.py
+-rw-r--r--   0        0        0    17708 2023-06-08 11:55:07.635429 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.pyi
+-rw-r--r--   0        0        0      389 2023-06-08 11:55:07.635636 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/__init__.py
+-rw-r--r--   0        0        0    21776 2023-06-08 11:55:07.635849 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.py
+-rw-r--r--   0        0        0    21550 2023-06-08 11:55:07.636089 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.pyi
+-rw-r--r--   0        0        0      399 2023-06-08 11:55:07.636318 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/__init__.py
+-rw-r--r--   0        0        0    22868 2023-06-08 11:55:07.636562 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.py
+-rw-r--r--   0        0        0    22642 2023-06-08 11:55:07.636861 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_updateorder/put.pyi
+-rw-r--r--   0        0        0      415 2023-06-08 11:55:07.637099 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/__init__.py
+-rw-r--r--   0        0        0    18102 2023-06-08 11:55:07.637281 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.py
+-rw-r--r--   0        0        0    17876 2023-06-08 11:55:07.637510 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.pyi
+-rw-r--r--   0        0        0      341 2023-06-08 11:55:07.637720 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_search/__init__.py
+-rw-r--r--   0        0        0    21271 2023-06-08 11:55:07.637986 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_search/get.py
+-rw-r--r--   0        0        0    21045 2023-06-08 11:55:07.638236 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_search/get.pyi
+-rw-r--r--   0        0        0      351 2023-06-08 11:55:07.638454 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_updateorder/__init__.py
+-rw-r--r--   0        0        0    21319 2023-06-08 11:55:07.638665 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_updateorder/put.py
+-rw-r--r--   0        0        0    21093 2023-06-08 11:55:07.638936 splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_updateorder/put.pyi
+-rw-r--r--   0        0        0      639 2023-06-08 11:55:07.639159 splitit_web_python_sdk-2.2.0/splitit_client/request_after_hook.py
+-rw-r--r--   0        0        0      640 2023-06-08 11:55:07.639383 splitit_web_python_sdk-2.2.0/splitit_client/request_before_hook.py
+-rw-r--r--   0        0        0    10957 2023-06-08 11:55:07.639589 splitit_web_python_sdk-2.2.0/splitit_client/rest.py
+-rw-r--r--   0        0        0    95571 2023-06-08 11:55:07.640105 splitit_web_python_sdk-2.2.0/splitit_client/schemas.py
+-rw-r--r--   0        0        0        0 2023-06-08 11:55:07.640275 splitit_web_python_sdk-2.2.0/splitit_client/type/__init__.py
+-rw-r--r--   0        0        0      561 2023-06-08 11:55:07.640426 splitit_web_python_sdk-2.2.0/splitit_client/type/address_data.py
+-rw-r--r--   0        0        0      587 2023-06-08 11:55:07.640581 splitit_web_python_sdk-2.2.0/splitit_client/type/address_data_model.py
+-rw-r--r--   0        0        0      887 2023-06-08 11:55:07.640741 splitit_web_python_sdk-2.2.0/splitit_client/type/authorization_model.py
+-rw-r--r--   0        0        0      398 2023-06-08 11:55:07.640895 splitit_web_python_sdk-2.2.0/splitit_client/type/card_brand.py
+-rw-r--r--   0        0        0      705 2023-06-08 11:55:07.641039 splitit_web_python_sdk-2.2.0/splitit_client/type/card_data.py
+-rw-r--r--   0        0        0      388 2023-06-08 11:55:07.641189 splitit_web_python_sdk-2.2.0/splitit_client/type/card_type.py
+-rw-r--r--   0        0        0      816 2023-06-08 11:55:07.641384 splitit_web_python_sdk-2.2.0/splitit_client/type/check_installments_eligibility_request.py
+-rw-r--r--   0        0        0      481 2023-06-08 11:55:07.641566 splitit_web_python_sdk-2.2.0/splitit_client/type/error.py
+-rw-r--r--   0        0        0      452 2023-06-08 11:55:07.641720 splitit_web_python_sdk-2.2.0/splitit_client/type/error_extended.py
+-rw-r--r--   0        0        0      524 2023-06-08 11:55:07.641893 splitit_web_python_sdk-2.2.0/splitit_client/type/events_endpoints_model.py
+-rw-r--r--   0        0        0      573 2023-06-08 11:55:07.642074 splitit_web_python_sdk-2.2.0/splitit_client/type/failed_response.py
+-rw-r--r--   0        0        0      359 2023-06-08 11:55:07.642249 splitit_web_python_sdk-2.2.0/splitit_client/type/gw_authorization_status.py
+-rw-r--r--   0        0        0      588 2023-06-08 11:55:07.642422 splitit_web_python_sdk-2.2.0/splitit_client/type/identifier_contract.py
+-rw-r--r--   0        0        0     1018 2023-06-08 11:55:07.642680 splitit_web_python_sdk-2.2.0/splitit_client/type/initiate_plan_response.py
+-rw-r--r--   0        0        0      617 2023-06-08 11:55:07.642907 splitit_web_python_sdk-2.2.0/splitit_client/type/initiate_redirection_endpoints_model.py
+-rw-r--r--   0        0        0      640 2023-06-08 11:55:07.643135 splitit_web_python_sdk-2.2.0/splitit_client/type/installment.py
+-rw-r--r--   0        0        0      575 2023-06-08 11:55:07.643349 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_cancel_response.py
+-rw-r--r--   0        0        0     1257 2023-06-08 11:55:07.643532 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_create_request.py
+-rw-r--r--   0        0        0     1510 2023-06-08 11:55:07.643757 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_create_response.py
+-rw-r--r--   0        0        0     1591 2023-06-08 11:55:07.643992 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_get_response.py
+-rw-r--r--   0        0        0     1242 2023-06-08 11:55:07.644256 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_initiate_request.py
+-rw-r--r--   0        0        0      665 2023-06-08 11:55:07.644461 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_refund_request.py
+-rw-r--r--   0        0        0      805 2023-06-08 11:55:07.644662 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_refund_response.py
+-rw-r--r--   0        0        0      709 2023-06-08 11:55:07.644855 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_search_response.py
+-rw-r--r--   0        0        0      709 2023-06-08 11:55:07.645105 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_update_request.py
+-rw-r--r--   0        0        0      622 2023-06-08 11:55:07.645504 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_update_request_by_identifier.py
+-rw-r--r--   0        0        0      768 2023-06-08 11:55:07.645696 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_update_response.py
+-rw-r--r--   0        0        0      348 2023-06-08 11:55:07.645868 splitit_web_python_sdk-2.2.0/splitit_client/type/installment_status.py
+-rw-r--r--   0        0        0      695 2023-06-08 11:55:07.646045 splitit_web_python_sdk-2.2.0/splitit_client/type/installments_eligibility_response.py
+-rw-r--r--   0        0        0      532 2023-06-08 11:55:07.646232 splitit_web_python_sdk-2.2.0/splitit_client/type/links_data.py
+-rw-r--r--   0        0        0      530 2023-06-08 11:55:07.646385 splitit_web_python_sdk-2.2.0/splitit_client/type/links_model.py
+-rw-r--r--   0        0        0      664 2023-06-08 11:55:07.646508 splitit_web_python_sdk-2.2.0/splitit_client/type/payment_method_model.py
+-rw-r--r--   0        0        0      336 2023-06-08 11:55:07.646617 splitit_web_python_sdk-2.2.0/splitit_client/type/payment_method_type.py
+-rw-r--r--   0        0        0      763 2023-06-08 11:55:07.646794 splitit_web_python_sdk-2.2.0/splitit_client/type/payment_plan_option_model.py
+-rw-r--r--   0        0        0      838 2023-06-08 11:55:07.646933 splitit_web_python_sdk-2.2.0/splitit_client/type/plan_data.py
+-rw-r--r--   0        0        0      824 2023-06-08 11:55:07.647027 splitit_web_python_sdk-2.2.0/splitit_client/type/plan_data_model.py
+-rw-r--r--   0        0        0      484 2023-06-08 11:55:07.647119 splitit_web_python_sdk-2.2.0/splitit_client/type/plan_error_response.py
+-rw-r--r--   0        0        0      371 2023-06-08 11:55:07.647218 splitit_web_python_sdk-2.2.0/splitit_client/type/plan_status.py
+-rw-r--r--   0        0        0      347 2023-06-08 11:55:07.647297 splitit_web_python_sdk-2.2.0/splitit_client/type/purchase_method.py
+-rw-r--r--   0        0        0      615 2023-06-08 11:55:07.647378 splitit_web_python_sdk-2.2.0/splitit_client/type/redirection_endpoints_model.py
+-rw-r--r--   0        0        0      719 2023-06-08 11:55:07.647461 splitit_web_python_sdk-2.2.0/splitit_client/type/refund_model.py
+-rw-r--r--   0        0        0      341 2023-06-08 11:55:07.647548 splitit_web_python_sdk-2.2.0/splitit_client/type/refund_status.py
+-rw-r--r--   0        0        0      423 2023-06-08 11:55:07.647634 splitit_web_python_sdk-2.2.0/splitit_client/type/refund_strategy.py
+-rw-r--r--   0        0        0      642 2023-06-08 11:55:07.647718 splitit_web_python_sdk-2.2.0/splitit_client/type/refund_summary.py
+-rw-r--r--   0        0        0     1626 2023-06-08 11:55:07.647802 splitit_web_python_sdk-2.2.0/splitit_client/type/search_installment_plan_response_item.py
+-rw-r--r--   0        0        0      344 2023-06-08 11:55:07.647884 splitit_web_python_sdk-2.2.0/splitit_client/type/shipping_status.py
+-rw-r--r--   0        0        0      334 2023-06-08 11:55:07.647983 splitit_web_python_sdk-2.2.0/splitit_client/type/shipping_status2.py
+-rw-r--r--   0        0        0      528 2023-06-08 11:55:07.648069 splitit_web_python_sdk-2.2.0/splitit_client/type/shopper_data.py
+-rw-r--r--   0        0        0      345 2023-06-08 11:55:07.648154 splitit_web_python_sdk-2.2.0/splitit_client/type/test_modes.py
+-rw-r--r--   0        0        0      567 2023-06-08 11:55:07.648240 splitit_web_python_sdk-2.2.0/splitit_client/type/three_ds_redirect_data_v3.py
+-rw-r--r--   0        0        0      656 2023-06-08 11:55:07.648338 splitit_web_python_sdk-2.2.0/splitit_client/type/update_order_request.py
+-rw-r--r--   0        0        0      524 2023-06-08 11:55:07.648430 splitit_web_python_sdk-2.2.0/splitit_client/type/ux_settings_model.py
+-rw-r--r--   0        0        0      708 2023-06-08 11:55:07.648516 splitit_web_python_sdk-2.2.0/splitit_client/type/verify_authorization_response.py
+-rw-r--r--   0        0        0      491 2023-06-08 11:55:07.648605 splitit_web_python_sdk-2.2.0/splitit_client/type_util.py
+-rw-r--r--   0        0        0     3170 2023-06-08 11:55:07.648691 splitit_web_python_sdk-2.2.0/splitit_client/validation_metadata.py
+-rw-r--r--   0        0        0     9244 1970-01-01 00:00:00.000000 splitit_web_python_sdk-2.2.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `splitit-web-python-sdk-2.1.0/LICENSE` & `splitit_web_python_sdk-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/PKG-INFO` & `splitit_web_python_sdk-2.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,39 @@
-Metadata-Version: 2.1
-Name: splitit-web-python-sdk
-Version: 2.1.0
-Summary: splitit-web-api-v3
-Home-page: https://github.com/konfig-dev/splitit-web-sdks/tree/main/python
-Author: Konfig
-Author-email: engineering@konfigthis.com
-License: MIT
-Keywords: Konfig,splitit-web-api-v3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# splitit-web-python-sdk
+# splitit-web-python-sdk@2.2.0
 Splitit's Web API
 
-- API version: 1.0.0
-- Package version: 2.1.0
 
-## Requirements.
+## Requirements
 
 Python >=3.7
 
-## Installation & Usage
-### pip install
-
-If the python package is hosted on a repository, you can install directly using:
+## Installing
 
 ```sh
-pip install splitit-web-python-sdk==2.1.0
+pip install splitit-web-python-sdk==2.2.0
 ```
-(you may need to run `pip` with root permission: `sudo pip install splitit-web-python-sdk==2.1.0`)
 
-Then import the package:
-```python
-import splitit_client
-```
 ## Getting Started
 
-Please follow the [installation procedure](#installation--usage) and then run the following:
-
 ```python
 from pprint import pprint
-from splitit_client import Splitit
+from splitit_client import Splitit, ApiException
 
 splitit = Splitit(
-    # Defining the host is optional and defaults to https://web-api-v3.sandbox.splitit.com
+    # Defining the host is optional and defaults to https://web-api-v3.production.splitit.com
     # See configuration.py for a list of all supported configuration parameters.
-    host = "https://web-api-v3.sandbox.splitit.com",
-
+    host="https://web-api-v3.production.splitit.com",
     # Configure OAuth2 access token for authorization: oauth
-    access_token = 'YOUR_ACCESS_TOKEN'
+    access_token="YOUR_ACCESS_TOKEN",
 )
 
 try:
     cancel_response = splitit.installment_plan.cancel(
-        path_params = {
-            'installmentPlanNumber': "installmentPlanNumber_example",
-        },
-        header_params = {
-            'X-Splitit-IdempotencyKey': "X-Splitit-IdempotencyKey_example",
-        },
+        installment_plan_number="installmentPlanNumber_example",  # required
+        x_splitit_idempotency_key="X-Splitit-IdempotencyKey_example",  # required
     )
     pprint(cancel_response.body)
     pprint(cancel_response.body["installment_plan_number"])
     pprint(cancel_response.headers)
     pprint(cancel_response.status)
     pprint(cancel_response.round_trip_time)
 except ApiException as e:
@@ -83,17 +53,71 @@
         pprint(e.body["error"])
     pprint(e.headers)
     pprint(e.status)
     pprint(e.reason)
     pprint(e.round_trip_time)
 ```
 
+## Async
+
+`async` support is available by prepending `a` to any method.
+
+```python
+import asyncio
+from pprint import pprint
+from splitit_client import Splitit, ApiException
+
+splitit = Splitit(
+    # Defining the host is optional and defaults to https://web-api-v3.production.splitit.com
+    # See configuration.py for a list of all supported configuration parameters.
+    host="https://web-api-v3.production.splitit.com",
+    # Configure OAuth2 access token for authorization: oauth
+    access_token="YOUR_ACCESS_TOKEN",
+)
+
+
+async def main():
+    try:
+        cancel_response = await splitit.installment_plan.acancel(
+            installment_plan_number="installmentPlanNumber_example",  # required
+            x_splitit_idempotency_key="X-Splitit-IdempotencyKey_example",  # required
+        )
+        pprint(cancel_response.body)
+        pprint(cancel_response.body["installment_plan_number"])
+        pprint(cancel_response.headers)
+        pprint(cancel_response.status)
+        pprint(cancel_response.round_trip_time)
+    except ApiException as e:
+        print("Exception when calling InstallmentPlanApi.cancel: %s\n" % e)
+        pprint(e.body)
+        if e.status == 401:
+            pprint(e.body["trace_id"])
+            pprint(e.body["error"])
+        if e.status == 500:
+            pprint(e.body["trace_id"])
+            pprint(e.body["error"])
+        if e.status == 403:
+            pprint(e.body["trace_id"])
+            pprint(e.body["error"])
+        if e.status == 404:
+            pprint(e.body["trace_id"])
+            pprint(e.body["error"])
+        pprint(e.headers)
+        pprint(e.status)
+        pprint(e.reason)
+        pprint(e.round_trip_time)
+
+
+asyncio.run(main())
+```
+
+
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://web-api-v3.sandbox.splitit.com*
+All URIs are relative to *https://web-api-v3.production.splitit.com*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *InstallmentPlanApi* | [**cancel**](docs/apis/tags/InstallmentPlanApi.md#cancel) | **post** /api/installmentplans/{installmentPlanNumber}/cancel | 
 *InstallmentPlanApi* | [**check_eligibility**](docs/apis/tags/InstallmentPlanApi.md#check_eligibility) | **post** /api/installmentplans/check-eligibility | 
 *InstallmentPlanApi* | [**get**](docs/apis/tags/InstallmentPlanApi.md#get) | **get** /api/installmentplans/{installmentPlanNumber} | 
 *InstallmentPlanApi* | [**post**](docs/apis/tags/InstallmentPlanApi.md#post) | **post** /api/installmentplans/initiate | 
@@ -111,14 +135,15 @@
  - [AuthorizationModel](docs/models/AuthorizationModel.md)
  - [CardBrand](docs/models/CardBrand.md)
  - [CardData](docs/models/CardData.md)
  - [CardType](docs/models/CardType.md)
  - [CheckInstallmentsEligibilityRequest](docs/models/CheckInstallmentsEligibilityRequest.md)
  - [Error](docs/models/Error.md)
  - [ErrorExtended](docs/models/ErrorExtended.md)
+ - [EventsEndpointsModel](docs/models/EventsEndpointsModel.md)
  - [FailedResponse](docs/models/FailedResponse.md)
  - [GwAuthorizationStatus](docs/models/GwAuthorizationStatus.md)
  - [IdentifierContract](docs/models/IdentifierContract.md)
  - [InitiatePlanResponse](docs/models/InitiatePlanResponse.md)
  - [InitiateRedirectionEndpointsModel](docs/models/InitiateRedirectionEndpointsModel.md)
  - [Installment](docs/models/Installment.md)
  - [InstallmentPlanCancelResponse](docs/models/InstallmentPlanCancelResponse.md)
@@ -155,22 +180,10 @@
  - [ShopperData](docs/models/ShopperData.md)
  - [TestModes](docs/models/TestModes.md)
  - [ThreeDsRedirectDataV3](docs/models/ThreeDsRedirectDataV3.md)
  - [UpdateOrderRequest](docs/models/UpdateOrderRequest.md)
  - [UxSettingsModel](docs/models/UxSettingsModel.md)
  - [VerifyAuthorizationResponse](docs/models/VerifyAuthorizationResponse.md)
 
-## Documentation For Authorization
-
- Authentication schemes defined for the API:
-## oauth
-
-- **Type**: OAuth
-- **Flow**: application
-- **Authorization URL**: 
-- **Scopes**: 
- - **api.v3**: 
-
-
 
 ## Author
 This Python package is automatically generated by [Konfig](https://konfigthis.com)
```

### Comparing `splitit-web-python-sdk-2.1.0/README.md` & `splitit_web_python_sdk-2.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,63 @@
-# splitit-web-python-sdk
+Metadata-Version: 2.1
+Name: splitit-web-python-sdk
+Version: 2.2.0
+Summary: Client for splitit-web-api-v3
+License: MIT
+Author: Konfig
+Author-email: engineering@konfigthis.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
+Requires-Dist: frozendict (>=2.3.4,<3.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
+Requires-Dist: urllib3 (>=1.26.7,<2.0.0)
+Requires-Dist: validators (>=0.20.0,<0.21.0)
+Description-Content-Type: text/markdown
+
+# splitit-web-python-sdk@2.2.0
 Splitit's Web API
 
-- API version: 1.0.0
-- Package version: 2.1.0
 
-## Requirements.
+## Requirements
 
 Python >=3.7
 
-## Installation & Usage
-### pip install
-
-If the python package is hosted on a repository, you can install directly using:
+## Installing
 
 ```sh
-pip install splitit-web-python-sdk==2.1.0
+pip install splitit-web-python-sdk==2.2.0
 ```
-(you may need to run `pip` with root permission: `sudo pip install splitit-web-python-sdk==2.1.0`)
 
-Then import the package:
-```python
-import splitit_client
-```
 ## Getting Started
 
-Please follow the [installation procedure](#installation--usage) and then run the following:
-
 ```python
 from pprint import pprint
-from splitit_client import Splitit
+from splitit_client import Splitit, ApiException
 
 splitit = Splitit(
-    # Defining the host is optional and defaults to https://web-api-v3.sandbox.splitit.com
+    # Defining the host is optional and defaults to https://web-api-v3.production.splitit.com
     # See configuration.py for a list of all supported configuration parameters.
-    host = "https://web-api-v3.sandbox.splitit.com",
-
+    host="https://web-api-v3.production.splitit.com",
     # Configure OAuth2 access token for authorization: oauth
-    access_token = 'YOUR_ACCESS_TOKEN'
+    access_token="YOUR_ACCESS_TOKEN",
 )
 
 try:
     cancel_response = splitit.installment_plan.cancel(
-        path_params = {
-            'installmentPlanNumber': "installmentPlanNumber_example",
-        },
-        header_params = {
-            'X-Splitit-IdempotencyKey': "X-Splitit-IdempotencyKey_example",
-        },
+        installment_plan_number="installmentPlanNumber_example",  # required
+        x_splitit_idempotency_key="X-Splitit-IdempotencyKey_example",  # required
     )
     pprint(cancel_response.body)
     pprint(cancel_response.body["installment_plan_number"])
     pprint(cancel_response.headers)
     pprint(cancel_response.status)
     pprint(cancel_response.round_trip_time)
 except ApiException as e:
@@ -70,17 +77,71 @@
         pprint(e.body["error"])
     pprint(e.headers)
     pprint(e.status)
     pprint(e.reason)
     pprint(e.round_trip_time)
 ```
 
+## Async
+
+`async` support is available by prepending `a` to any method.
+
+```python
+import asyncio
+from pprint import pprint
+from splitit_client import Splitit, ApiException
+
+splitit = Splitit(
+    # Defining the host is optional and defaults to https://web-api-v3.production.splitit.com
+    # See configuration.py for a list of all supported configuration parameters.
+    host="https://web-api-v3.production.splitit.com",
+    # Configure OAuth2 access token for authorization: oauth
+    access_token="YOUR_ACCESS_TOKEN",
+)
+
+
+async def main():
+    try:
+        cancel_response = await splitit.installment_plan.acancel(
+            installment_plan_number="installmentPlanNumber_example",  # required
+            x_splitit_idempotency_key="X-Splitit-IdempotencyKey_example",  # required
+        )
+        pprint(cancel_response.body)
+        pprint(cancel_response.body["installment_plan_number"])
+        pprint(cancel_response.headers)
+        pprint(cancel_response.status)
+        pprint(cancel_response.round_trip_time)
+    except ApiException as e:
+        print("Exception when calling InstallmentPlanApi.cancel: %s\n" % e)
+        pprint(e.body)
+        if e.status == 401:
+            pprint(e.body["trace_id"])
+            pprint(e.body["error"])
+        if e.status == 500:
+            pprint(e.body["trace_id"])
+            pprint(e.body["error"])
+        if e.status == 403:
+            pprint(e.body["trace_id"])
+            pprint(e.body["error"])
+        if e.status == 404:
+            pprint(e.body["trace_id"])
+            pprint(e.body["error"])
+        pprint(e.headers)
+        pprint(e.status)
+        pprint(e.reason)
+        pprint(e.round_trip_time)
+
+
+asyncio.run(main())
+```
+
+
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://web-api-v3.sandbox.splitit.com*
+All URIs are relative to *https://web-api-v3.production.splitit.com*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *InstallmentPlanApi* | [**cancel**](docs/apis/tags/InstallmentPlanApi.md#cancel) | **post** /api/installmentplans/{installmentPlanNumber}/cancel | 
 *InstallmentPlanApi* | [**check_eligibility**](docs/apis/tags/InstallmentPlanApi.md#check_eligibility) | **post** /api/installmentplans/check-eligibility | 
 *InstallmentPlanApi* | [**get**](docs/apis/tags/InstallmentPlanApi.md#get) | **get** /api/installmentplans/{installmentPlanNumber} | 
 *InstallmentPlanApi* | [**post**](docs/apis/tags/InstallmentPlanApi.md#post) | **post** /api/installmentplans/initiate | 
@@ -98,14 +159,15 @@
  - [AuthorizationModel](docs/models/AuthorizationModel.md)
  - [CardBrand](docs/models/CardBrand.md)
  - [CardData](docs/models/CardData.md)
  - [CardType](docs/models/CardType.md)
  - [CheckInstallmentsEligibilityRequest](docs/models/CheckInstallmentsEligibilityRequest.md)
  - [Error](docs/models/Error.md)
  - [ErrorExtended](docs/models/ErrorExtended.md)
+ - [EventsEndpointsModel](docs/models/EventsEndpointsModel.md)
  - [FailedResponse](docs/models/FailedResponse.md)
  - [GwAuthorizationStatus](docs/models/GwAuthorizationStatus.md)
  - [IdentifierContract](docs/models/IdentifierContract.md)
  - [InitiatePlanResponse](docs/models/InitiatePlanResponse.md)
  - [InitiateRedirectionEndpointsModel](docs/models/InitiateRedirectionEndpointsModel.md)
  - [Installment](docs/models/Installment.md)
  - [InstallmentPlanCancelResponse](docs/models/InstallmentPlanCancelResponse.md)
@@ -142,22 +204,11 @@
  - [ShopperData](docs/models/ShopperData.md)
  - [TestModes](docs/models/TestModes.md)
  - [ThreeDsRedirectDataV3](docs/models/ThreeDsRedirectDataV3.md)
  - [UpdateOrderRequest](docs/models/UpdateOrderRequest.md)
  - [UxSettingsModel](docs/models/UxSettingsModel.md)
  - [VerifyAuthorizationResponse](docs/models/VerifyAuthorizationResponse.md)
 
-## Documentation For Authorization
-
- Authentication schemes defined for the API:
-## oauth
-
-- **Type**: OAuth
-- **Flow**: application
-- **Authorization URL**: 
-- **Scopes**: 
- - **api.v3**: 
-
-
 
 ## Author
 This Python package is automatically generated by [Konfig](https://konfigthis.com)
+
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/__init__.py` & `splitit_web_python_sdk-2.2.0/splitit_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Splitit's Web API
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
-__version__ = "2.1.0"
+__version__ = "2.2.0"
 
 # import ApiClient
 from splitit_client.api_client import ApiClient
 
 # import Configuration
 from splitit_client.configuration import Configuration
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/api_client.py` & `splitit_web_python_sdk-2.2.0/splitit_client/api_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,4012 +17,4583 @@
 00000100: 6f6e 0a69 6d70 6f72 7420 6f73 0a69 6d70  on.import os.imp
 00000110: 6f72 7420 696f 0a69 6d70 6f72 7420 6174  ort io.import at
 00000120: 6578 6974 0a66 726f 6d20 6d75 6c74 6970  exit.from multip
 00000130: 726f 6365 7373 696e 672e 706f 6f6c 2069  rocessing.pool i
 00000140: 6d70 6f72 7420 5468 7265 6164 506f 6f6c  mport ThreadPool
 00000150: 0a69 6d70 6f72 7420 7265 0a69 6d70 6f72  .import re.impor
 00000160: 7420 7465 6d70 6669 6c65 0a69 6d70 6f72  t tempfile.impor
-00000170: 7420 7479 7069 6e67 0a69 6d70 6f72 7420  t typing.import 
-00000180: 7479 7069 6e67 5f65 7874 656e 7369 6f6e  typing_extension
-00000190: 730a 696d 706f 7274 2075 726c 6c69 6233  s.import urllib3
-000001a0: 0a66 726f 6d20 7572 6c6c 6962 332e 5f63  .from urllib3._c
-000001b0: 6f6c 6c65 6374 696f 6e73 2069 6d70 6f72  ollections impor
-000001c0: 7420 4854 5450 4865 6164 6572 4469 6374  t HTTPHeaderDict
-000001d0: 0a66 726f 6d20 7572 6c6c 6962 2e70 6172  .from urllib.par
-000001e0: 7365 2069 6d70 6f72 7420 7572 6c70 6172  se import urlpar
-000001f0: 7365 2c20 7175 6f74 650a 6672 6f6d 2075  se, quote.from u
-00000200: 726c 6c69 6233 2e66 6965 6c64 7320 696d  rllib3.fields im
-00000210: 706f 7274 2052 6571 7565 7374 4669 656c  port RequestFiel
-00000220: 6420 6173 2052 6571 7565 7374 4669 656c  d as RequestFiel
-00000230: 6442 6173 650a 6672 6f6d 2075 726c 6c69  dBase.from urlli
-00000240: 6233 2e66 6965 6c64 7320 696d 706f 7274  b3.fields import
-00000250: 2067 7565 7373 5f63 6f6e 7465 6e74 5f74   guess_content_t
-00000260: 7970 650a 0a69 6d70 6f72 7420 6672 6f7a  ype..import froz
-00000270: 656e 6469 6374 0a0a 6672 6f6d 2073 706c  endict..from spl
-00000280: 6974 6974 5f63 6c69 656e 7420 696d 706f  itit_client impo
-00000290: 7274 2072 6573 740a 6672 6f6d 2073 706c  rt rest.from spl
-000002a0: 6974 6974 5f63 6c69 656e 742e 6170 695f  itit_client.api_
-000002b0: 7265 7370 6f6e 7365 2069 6d70 6f72 7420  response import 
-000002c0: 4170 6952 6573 706f 6e73 650a 6672 6f6d  ApiResponse.from
-000002d0: 2073 706c 6974 6974 5f63 6c69 656e 742e   splitit_client.
-000002e0: 7265 7374 2069 6d70 6f72 7420 5265 7370  rest import Resp
-000002f0: 6f6e 7365 5772 6170 7065 720a 6672 6f6d  onseWrapper.from
-00000300: 2073 706c 6974 6974 5f63 6c69 656e 742e   splitit_client.
-00000310: 636f 6e66 6967 7572 6174 696f 6e20 696d  configuration im
-00000320: 706f 7274 2043 6f6e 6669 6775 7261 7469  port Configurati
-00000330: 6f6e 0a66 726f 6d20 7370 6c69 7469 745f  on.from splitit_
-00000340: 636c 6965 6e74 2e65 7863 6570 7469 6f6e  client.exception
-00000350: 7320 696d 706f 7274 2041 7069 5479 7065  s import ApiType
-00000360: 4572 726f 722c 2041 7069 5661 6c75 6545  Error, ApiValueE
-00000370: 7272 6f72 2c20 4d69 7373 696e 6752 6571  rror, MissingReq
-00000380: 7569 7265 6450 6172 616d 6574 6572 7345  uiredParametersE
-00000390: 7272 6f72 0a66 726f 6d20 7370 6c69 7469  rror.from spliti
-000003a0: 745f 636c 6965 6e74 2e72 6571 7565 7374  t_client.request
-000003b0: 5f61 6674 6572 5f68 6f6f 6b20 696d 706f  _after_hook impo
-000003c0: 7274 2072 6571 7565 7374 5f61 6674 6572  rt request_after
-000003d0: 5f68 6f6f 6b0a 6672 6f6d 2073 706c 6974  _hook.from split
-000003e0: 6974 5f63 6c69 656e 742e 7265 7175 6573  it_client.reques
-000003f0: 745f 6265 666f 7265 5f68 6f6f 6b20 696d  t_before_hook im
-00000400: 706f 7274 2072 6571 7565 7374 5f62 6566  port request_bef
-00000410: 6f72 655f 686f 6f6b 0a66 726f 6d20 7370  ore_hook.from sp
-00000420: 6c69 7469 745f 636c 6965 6e74 2e73 6368  litit_client.sch
-00000430: 656d 6173 2069 6d70 6f72 7420 280a 2020  emas import (.  
-00000440: 2020 4e6f 6e65 436c 6173 732c 0a20 2020    NoneClass,.   
-00000450: 2042 6f6f 6c43 6c61 7373 2c0a 2020 2020   BoolClass,.    
-00000460: 5363 6865 6d61 2c0a 2020 2020 4669 6c65  Schema,.    File
-00000470: 494f 2c0a 2020 2020 4269 6e61 7279 5363  IO,.    BinarySc
-00000480: 6865 6d61 2c0a 2020 2020 6461 7465 2c0a  hema,.    date,.
-00000490: 2020 2020 6461 7465 7469 6d65 2c0a 2020      datetime,.  
-000004a0: 2020 6e6f 6e65 5f74 7970 652c 0a20 2020    none_type,.   
-000004b0: 2055 6e73 6574 2c0a 2020 2020 756e 7365   Unset,.    unse
-000004c0: 742c 0a29 0a0a 0a63 6c61 7373 2052 6571  t,.)...class Req
-000004d0: 7565 7374 4669 656c 6428 5265 7175 6573  uestField(Reques
-000004e0: 7446 6965 6c64 4261 7365 293a 0a20 2020  tFieldBase):.   
-000004f0: 2064 6566 205f 5f65 715f 5f28 7365 6c66   def __eq__(self
-00000500: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-00000510: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-00000520: 6e63 6528 6f74 6865 722c 2052 6571 7565  nce(other, Reque
-00000530: 7374 4669 656c 6429 3a0a 2020 2020 2020  stField):.      
-00000540: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00000550: 7365 0a20 2020 2020 2020 2072 6574 7572  se.        retur
-00000560: 6e20 7365 6c66 2e5f 5f64 6963 745f 5f20  n self.__dict__ 
-00000570: 3d3d 206f 7468 6572 2e5f 5f64 6963 745f  == other.__dict_
-00000580: 5f0a 0a0a 636c 6173 7320 4a53 4f4e 456e  _...class JSONEn
-00000590: 636f 6465 7228 6a73 6f6e 2e4a 534f 4e45  coder(json.JSONE
-000005a0: 6e63 6f64 6572 293a 0a20 2020 2063 6f6d  ncoder):.    com
-000005b0: 7061 6374 5f73 6570 6172 6174 6f72 7320  pact_separators 
-000005c0: 3d20 2827 2c27 2c20 273a 2729 0a0a 2020  = (',', ':')..  
-000005d0: 2020 6465 6620 6465 6661 756c 7428 7365    def default(se
-000005e0: 6c66 2c20 6f62 6a29 3a0a 2020 2020 2020  lf, obj):.      
-000005f0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00000600: 6f62 6a2c 2073 7472 293a 0a20 2020 2020  obj, str):.     
-00000610: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
-00000620: 7228 6f62 6a29 0a20 2020 2020 2020 2065  r(obj).        e
-00000630: 6c69 6620 6973 696e 7374 616e 6365 286f  lif isinstance(o
-00000640: 626a 2c20 666c 6f61 7429 3a0a 2020 2020  bj, float):.    
-00000650: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00000660: 6c6f 6174 286f 626a 290a 2020 2020 2020  loat(obj).      
-00000670: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-00000680: 6528 6f62 6a2c 2069 6e74 293a 0a20 2020  e(obj, int):.   
-00000690: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000006a0: 696e 7428 6f62 6a29 0a20 2020 2020 2020  int(obj).       
-000006b0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
-000006c0: 286f 626a 2c20 4465 6369 6d61 6c29 3a0a  (obj, Decimal):.
-000006d0: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-000006e0: 626a 2e61 735f 7475 706c 6528 292e 6578  bj.as_tuple().ex
-000006f0: 706f 6e65 6e74 203e 3d20 303a 0a20 2020  ponent >= 0:.   
-00000700: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00000710: 7572 6e20 696e 7428 6f62 6a29 0a20 2020  urn int(obj).   
-00000720: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000730: 666c 6f61 7428 6f62 6a29 0a20 2020 2020  float(obj).     
-00000740: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-00000750: 6365 286f 626a 2c20 4e6f 6e65 436c 6173  ce(obj, NoneClas
-00000760: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00000770: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
-00000780: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-00000790: 6e63 6528 6f62 6a2c 2042 6f6f 6c43 6c61  nce(obj, BoolCla
-000007a0: 7373 293a 0a20 2020 2020 2020 2020 2020  ss):.           
-000007b0: 2072 6574 7572 6e20 626f 6f6c 286f 626a   return bool(obj
-000007c0: 290a 2020 2020 2020 2020 656c 6966 2069  ).        elif i
-000007d0: 7369 6e73 7461 6e63 6528 6f62 6a2c 2028  sinstance(obj, (
-000007e0: 6469 6374 2c20 6672 6f7a 656e 6469 6374  dict, frozendict
-000007f0: 2e66 726f 7a65 6e64 6963 7429 293a 0a20  .frozendict)):. 
-00000800: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00000810: 6e20 7b6b 6579 3a20 7365 6c66 2e64 6566  n {key: self.def
-00000820: 6175 6c74 2876 616c 2920 666f 7220 6b65  ault(val) for ke
-00000830: 792c 2076 616c 2069 6e20 6f62 6a2e 6974  y, val in obj.it
-00000840: 656d 7328 297d 0a20 2020 2020 2020 2065  ems()}.        e
-00000850: 6c69 6620 6973 696e 7374 616e 6365 286f  lif isinstance(o
-00000860: 626a 2c20 286c 6973 742c 2074 7570 6c65  bj, (list, tuple
-00000870: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-00000880: 7265 7475 726e 205b 7365 6c66 2e64 6566  return [self.def
-00000890: 6175 6c74 2869 7465 6d29 2066 6f72 2069  ault(item) for i
-000008a0: 7465 6d20 696e 206f 626a 5d0a 2020 2020  tem in obj].    
-000008b0: 2020 2020 7261 6973 6520 4170 6956 616c      raise ApiVal
-000008c0: 7565 4572 726f 7228 2755 6e61 626c 6520  ueError('Unable 
-000008d0: 746f 2070 7265 7061 7265 2074 7970 6520  to prepare type 
-000008e0: 7b7d 2066 6f72 2073 6572 6961 6c69 7a61  {} for serializa
-000008f0: 7469 6f6e 272e 666f 726d 6174 286f 626a  tion'.format(obj
-00000900: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
-00000910: 655f 5f29 290a 0a0a 636c 6173 7320 5061  e__))...class Pa
-00000920: 7261 6d65 7465 7249 6e54 7970 6528 656e  rameterInType(en
-00000930: 756d 2e45 6e75 6d29 3a0a 2020 2020 5155  um.Enum):.    QU
-00000940: 4552 5920 3d20 2771 7565 7279 270a 2020  ERY = 'query'.  
-00000950: 2020 4845 4144 4552 203d 2027 6865 6164    HEADER = 'head
-00000960: 6572 270a 2020 2020 5041 5448 203d 2027  er'.    PATH = '
-00000970: 7061 7468 270a 2020 2020 434f 4f4b 4945  path'.    COOKIE
-00000980: 203d 2027 636f 6f6b 6965 270a 0a0a 636c   = 'cookie'...cl
-00000990: 6173 7320 5061 7261 6d65 7465 7253 7479  ass ParameterSty
-000009a0: 6c65 2865 6e75 6d2e 456e 756d 293a 0a20  le(enum.Enum):. 
-000009b0: 2020 204d 4154 5249 5820 3d20 276d 6174     MATRIX = 'mat
-000009c0: 7269 7827 0a20 2020 204c 4142 454c 203d  rix'.    LABEL =
-000009d0: 2027 6c61 6265 6c27 0a20 2020 2046 4f52   'label'.    FOR
-000009e0: 4d20 3d20 2766 6f72 6d27 0a20 2020 2053  M = 'form'.    S
-000009f0: 494d 504c 4520 3d20 2773 696d 706c 6527  IMPLE = 'simple'
-00000a00: 0a20 2020 2053 5041 4345 5f44 454c 494d  .    SPACE_DELIM
-00000a10: 4954 4544 203d 2027 7370 6163 6544 656c  ITED = 'spaceDel
-00000a20: 696d 6974 6564 270a 2020 2020 5049 5045  imited'.    PIPE
-00000a30: 5f44 454c 494d 4954 4544 203d 2027 7069  _DELIMITED = 'pi
-00000a40: 7065 4465 6c69 6d69 7465 6427 0a20 2020  peDelimited'.   
-00000a50: 2044 4545 505f 4f42 4a45 4354 203d 2027   DEEP_OBJECT = '
-00000a60: 6465 6570 4f62 6a65 6374 270a 0a0a 636c  deepObject'...cl
-00000a70: 6173 7320 5072 6566 6978 5365 7061 7261  ass PrefixSepara
-00000a80: 746f 7249 7465 7261 746f 723a 0a20 2020  torIterator:.   
-00000a90: 2023 2041 2063 6c61 7373 2074 6f20 7374   # A class to st
-00000aa0: 6f72 6520 7072 6566 6978 6573 2061 6e64  ore prefixes and
-00000ab0: 2073 6570 6172 6174 6f72 7320 666f 7220   separators for 
-00000ac0: 7266 6336 3537 3020 6578 7061 6e73 696f  rfc6570 expansio
-00000ad0: 6e73 0a0a 2020 2020 6465 6620 5f5f 696e  ns..    def __in
-00000ae0: 6974 5f5f 2873 656c 662c 2070 7265 6669  it__(self, prefi
-00000af0: 783a 2073 7472 2c20 7365 7061 7261 746f  x: str, separato
-00000b00: 723a 2073 7472 293a 0a20 2020 2020 2020  r: str):.       
-00000b10: 2073 656c 662e 7072 6566 6978 203d 2070   self.prefix = p
-00000b20: 7265 6669 780a 2020 2020 2020 2020 7365  refix.        se
-00000b30: 6c66 2e73 6570 6172 6174 6f72 203d 2073  lf.separator = s
-00000b40: 6570 6172 6174 6f72 0a20 2020 2020 2020  eparator.       
-00000b50: 2073 656c 662e 6669 7273 7420 3d20 5472   self.first = Tr
-00000b60: 7565 0a20 2020 2020 2020 2069 6620 7365  ue.        if se
-00000b70: 7061 7261 746f 7220 696e 207b 272e 272c  parator in {'.',
-00000b80: 2027 7c27 2c20 2725 3230 277d 3a0a 2020   '|', '%20'}:.  
-00000b90: 2020 2020 2020 2020 2020 6974 656d 5f73            item_s
-00000ba0: 6570 6172 6174 6f72 203d 2073 6570 6172  eparator = separ
-00000bb0: 6174 6f72 0a20 2020 2020 2020 2065 6c73  ator.        els
-00000bc0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00000bd0: 7465 6d5f 7365 7061 7261 746f 7220 3d20  tem_separator = 
-00000be0: 272c 270a 2020 2020 2020 2020 7365 6c66  ','.        self
-00000bf0: 2e69 7465 6d5f 7365 7061 7261 746f 7220  .item_separator 
-00000c00: 3d20 6974 656d 5f73 6570 6172 6174 6f72  = item_separator
-00000c10: 0a0a 2020 2020 6465 6620 5f5f 6974 6572  ..    def __iter
-00000c20: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
-00000c30: 2020 7265 7475 726e 2073 656c 660a 0a20    return self.. 
-00000c40: 2020 2064 6566 205f 5f6e 6578 745f 5f28     def __next__(
-00000c50: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-00000c60: 6620 7365 6c66 2e66 6972 7374 3a0a 2020  f self.first:.  
-00000c70: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-00000c80: 6972 7374 203d 2046 616c 7365 0a20 2020  irst = False.   
-00000c90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000ca0: 7365 6c66 2e70 7265 6669 780a 2020 2020  self.prefix.    
-00000cb0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00000cc0: 7365 7061 7261 746f 720a 0a0a 636c 6173  separator...clas
-00000cd0: 7320 5061 7261 6d65 7465 7253 6572 6961  s ParameterSeria
-00000ce0: 6c69 7a65 7242 6173 653a 0a20 2020 2040  lizerBase:.    @
-00000cf0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
-00000d00: 6465 6620 5f67 6574 5f64 6566 6175 6c74  def _get_default
-00000d10: 5f65 7870 6c6f 6465 2863 6c73 2c20 7374  _explode(cls, st
-00000d20: 796c 653a 2050 6172 616d 6574 6572 5374  yle: ParameterSt
-00000d30: 796c 6529 202d 3e20 626f 6f6c 3a0a 2020  yle) -> bool:.  
-00000d40: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00000d50: 7365 0a0a 2020 2020 4073 7461 7469 636d  se..    @staticm
-00000d60: 6574 686f 640a 2020 2020 6465 6620 5f5f  ethod.    def __
-00000d70: 7265 6636 3537 305f 6974 656d 5f76 616c  ref6570_item_val
-00000d80: 7565 2869 6e5f 6461 7461 3a20 7479 7069  ue(in_data: typi
-00000d90: 6e67 2e41 6e79 2c20 7065 7263 656e 745f  ng.Any, percent_
-00000da0: 656e 636f 6465 3a20 626f 6f6c 293a 0a20  encode: bool):. 
-00000db0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00000dc0: 2020 2047 6574 2072 6570 7265 7365 6e74     Get represent
-00000dd0: 6174 696f 6e20 6966 2073 7472 2f66 6c6f  ation if str/flo
-00000de0: 6174 2f69 6e74 2f4e 6f6e 652f 6974 656d  at/int/None/item
-00000df0: 7320 696e 206c 6973 742f 2076 616c 7565  s in list/ value
-00000e00: 7320 696e 2064 6963 740a 2020 2020 2020  s in dict.      
-00000e10: 2020 4e6f 6e65 2069 7320 7265 7475 726e    None is return
-00000e20: 6564 2069 6620 616e 2069 7465 6d20 6973  ed if an item is
-00000e30: 2075 6e64 6566 696e 6564 2c20 7573 6520   undefined, use 
-00000e40: 6361 7365 7320 6172 6520 7661 6c75 653d  cases are value=
-00000e50: 0a20 2020 2020 2020 202d 204e 6f6e 650a  .        - None.
-00000e60: 2020 2020 2020 2020 2d20 5b5d 0a20 2020          - [].   
-00000e70: 2020 2020 202d 207b 7d0a 2020 2020 2020       - {}.      
-00000e80: 2020 2d20 5b4e 6f6e 652c 204e 6f6e 6520    - [None, None 
-00000e90: 4e6f 6e65 5d0a 2020 2020 2020 2020 2d20  None].        - 
-00000ea0: 7b27 6127 3a20 4e6f 6e65 2c20 2762 273a  {'a': None, 'b':
-00000eb0: 204e 6f6e 657d 0a20 2020 2020 2020 2022   None}.        "
-00000ec0: 2222 0a20 2020 2020 2020 2069 6620 7479  "".        if ty
-00000ed0: 7065 2869 6e5f 6461 7461 2920 696e 207b  pe(in_data) in {
-00000ee0: 7374 722c 2066 6c6f 6174 2c20 696e 747d  str, float, int}
-00000ef0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00000f00: 2070 6572 6365 6e74 5f65 6e63 6f64 653a   percent_encode:
-00000f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000f20: 2072 6574 7572 6e20 7175 6f74 6528 7374   return quote(st
-00000f30: 7228 696e 5f64 6174 6129 290a 2020 2020  r(in_data)).    
-00000f40: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00000f50: 7472 2869 6e5f 6461 7461 290a 2020 2020  tr(in_data).    
-00000f60: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-00000f70: 6e63 6528 696e 5f64 6174 612c 206e 6f6e  nce(in_data, non
-00000f80: 655f 7479 7065 293a 0a20 2020 2020 2020  e_type):.       
-00000f90: 2020 2020 2023 2069 676e 6f72 6564 2062       # ignored b
-00000fa0: 7920 7468 6520 6578 7061 6e73 696f 6e20  y the expansion 
-00000fb0: 7072 6f63 6573 7320 6874 7470 733a 2f2f  process https://
-00000fc0: 6461 7461 7472 6163 6b65 722e 6965 7466  datatracker.ietf
-00000fd0: 2e6f 7267 2f64 6f63 2f68 746d 6c2f 7266  .org/doc/html/rf
-00000fe0: 6336 3537 3023 7365 6374 696f 6e2d 332e  c6570#section-3.
-00000ff0: 322e 310a 2020 2020 2020 2020 2020 2020  2.1.            
-00001000: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
-00001010: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-00001020: 6e63 6528 696e 5f64 6174 612c 206c 6973  nce(in_data, lis
-00001030: 7429 2061 6e64 206e 6f74 2069 6e5f 6461  t) and not in_da
-00001040: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-00001050: 2320 6967 6e6f 7265 6420 6279 2074 6865  # ignored by the
-00001060: 2065 7870 616e 7369 6f6e 2070 726f 6365   expansion proce
-00001070: 7373 2068 7474 7073 3a2f 2f64 6174 6174  ss https://datat
-00001080: 7261 636b 6572 2e69 6574 662e 6f72 672f  racker.ietf.org/
-00001090: 646f 632f 6874 6d6c 2f72 6663 3635 3730  doc/html/rfc6570
-000010a0: 2373 6563 7469 6f6e 2d33 2e32 2e31 0a20  #section-3.2.1. 
-000010b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000010c0: 6e20 4e6f 6e65 0a20 2020 2020 2020 2065  n None.        e
-000010d0: 6c69 6620 6973 696e 7374 616e 6365 2869  lif isinstance(i
-000010e0: 6e5f 6461 7461 2c20 6469 6374 2920 616e  n_data, dict) an
-000010f0: 6420 6e6f 7420 696e 5f64 6174 613a 0a20  d not in_data:. 
-00001100: 2020 2020 2020 2020 2020 2023 2069 676e             # ign
-00001110: 6f72 6564 2062 7920 7468 6520 6578 7061  ored by the expa
-00001120: 6e73 696f 6e20 7072 6f63 6573 7320 6874  nsion process ht
-00001130: 7470 733a 2f2f 6461 7461 7472 6163 6b65  tps://datatracke
-00001140: 722e 6965 7466 2e6f 7267 2f64 6f63 2f68  r.ietf.org/doc/h
-00001150: 746d 6c2f 7266 6336 3537 3023 7365 6374  tml/rfc6570#sect
-00001160: 696f 6e2d 332e 322e 310a 2020 2020 2020  ion-3.2.1.      
-00001170: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00001180: 650a 2020 2020 2020 2020 7261 6973 6520  e.        raise 
-00001190: 4170 6956 616c 7565 4572 726f 7228 2755  ApiValueError('U
-000011a0: 6e61 626c 6520 746f 2067 656e 6572 6174  nable to generat
-000011b0: 6520 6120 7265 6636 3537 3020 6974 656d  e a ref6570 item
-000011c0: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-000011d0: 6f66 207b 7d27 2e66 6f72 6d61 7428 696e  of {}'.format(in
-000011e0: 5f64 6174 6129 290a 0a20 2020 2040 7374  _data))..    @st
-000011f0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-00001200: 6566 205f 746f 5f64 6963 7428 6e61 6d65  ef _to_dict(name
-00001210: 3a20 7374 722c 2076 616c 7565 3a20 7374  : str, value: st
-00001220: 7229 3a0a 2020 2020 2020 2020 7265 7475  r):.        retu
-00001230: 726e 207b 6e61 6d65 3a20 7661 6c75 657d  rn {name: value}
-00001240: 0a0a 2020 2020 2222 220a 2020 2020 7266  ..    """.    rf
-00001250: 6336 3537 3020 646f 6573 206e 6f74 2073  c6570 does not s
-00001260: 7065 6369 6679 2068 6f77 2062 6f6f 6c65  pecify how boole
-00001270: 616e 2076 616c 7565 7320 6172 6520 7365  an values are se
-00001280: 7269 616c 697a 6564 2073 6f20 7765 2075  rialized so we u
-00001290: 7365 206c 6f77 6572 6361 7365 2022 7472  se lowercase "tr
-000012a0: 7565 2220 616e 6420 2266 616c 7365 0a20  ue" and "false. 
-000012b0: 2020 2022 2222 0a20 2020 2040 636c 6173     """.    @clas
-000012c0: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-000012d0: 5f5f 6b6f 6e66 6967 5f62 6f6f 6c5f 6578  __konfig_bool_ex
-000012e0: 7061 6e73 696f 6e28 0a20 2020 2020 2020  pansion(.       
-000012f0: 2063 6c73 2c0a 2020 2020 2020 2020 696e   cls,.        in
-00001300: 5f64 6174 613a 2074 7970 696e 672e 416e  _data: typing.An
-00001310: 792c 0a20 2020 2020 2020 2070 7265 6669  y,.        prefi
-00001320: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-00001330: 6174 6f72 3a20 5072 6566 6978 5365 7061  ator: PrefixSepa
-00001340: 7261 746f 7249 7465 7261 746f 722c 0a20  ratorIterator,. 
-00001350: 2020 2020 2020 2076 6172 5f6e 616d 655f         var_name_
-00001360: 7069 6563 653a 2073 7472 2c0a 2020 2020  piece: str,.    
-00001370: 2020 2020 6e61 6d65 645f 7061 7261 6d65      named_parame
-00001380: 7465 725f 6578 7061 6e73 696f 6e3a 2062  ter_expansion: b
-00001390: 6f6f 6c0a 2020 2020 2920 2d3e 2073 7472  ool.    ) -> str
-000013a0: 3a0a 2020 2020 2020 2020 6974 656d 5f76  :.        item_v
-000013b0: 616c 7565 203d 2022 7472 7565 2220 6966  alue = "true" if
-000013c0: 2069 6e5f 6461 7461 2069 7320 5472 7565   in_data is True
-000013d0: 2065 6c73 6520 2266 616c 7365 220a 2020   else "false".  
-000013e0: 2020 2020 2020 6966 2069 7465 6d5f 7661        if item_va
-000013f0: 6c75 6520 6973 204e 6f6e 6520 6f72 2028  lue is None or (
-00001400: 6974 656d 5f76 616c 7565 203d 3d20 2727  item_value == ''
-00001410: 2061 6e64 2070 7265 6669 785f 7365 7061   and prefix_sepa
-00001420: 7261 746f 725f 6974 6572 6174 6f72 2e73  rator_iterator.s
-00001430: 6570 6172 6174 6f72 203d 3d20 273b 2729  eparator == ';')
-00001440: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00001450: 7475 726e 206e 6578 7428 7072 6566 6978  turn next(prefix
-00001460: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-00001470: 746f 7229 202b 2076 6172 5f6e 616d 655f  tor) + var_name_
-00001480: 7069 6563 650a 2020 2020 2020 2020 7661  piece.        va
-00001490: 6c75 655f 7061 6972 5f65 7175 616c 7320  lue_pair_equals 
-000014a0: 3d20 273d 2720 6966 206e 616d 6564 5f70  = '=' if named_p
-000014b0: 6172 616d 6574 6572 5f65 7870 616e 7369  arameter_expansi
-000014c0: 6f6e 2065 6c73 6520 2727 0a20 2020 2020  on else ''.     
-000014d0: 2020 2072 6574 7572 6e20 6e65 7874 2870     return next(p
-000014e0: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
-000014f0: 6974 6572 6174 6f72 2920 2b20 7661 725f  iterator) + var_
-00001500: 6e61 6d65 5f70 6965 6365 202b 2076 616c  name_piece + val
-00001510: 7565 5f70 6169 725f 6571 7561 6c73 202b  ue_pair_equals +
-00001520: 2069 7465 6d5f 7661 6c75 650a 0a20 2020   item_value..   
-00001530: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00001540: 2020 6465 6620 5f5f 7265 6636 3537 305f    def __ref6570_
-00001550: 7374 725f 666c 6f61 745f 696e 745f 6578  str_float_int_ex
-00001560: 7061 6e73 696f 6e28 0a20 2020 2020 2020  pansion(.       
-00001570: 2063 6c73 2c0a 2020 2020 2020 2020 7661   cls,.        va
-00001580: 7269 6162 6c65 5f6e 616d 653a 2073 7472  riable_name: str
-00001590: 2c0a 2020 2020 2020 2020 696e 5f64 6174  ,.        in_dat
-000015a0: 613a 2074 7970 696e 672e 416e 792c 0a20  a: typing.Any,. 
-000015b0: 2020 2020 2020 2065 7870 6c6f 6465 3a20         explode: 
-000015c0: 626f 6f6c 2c0a 2020 2020 2020 2020 7065  bool,.        pe
-000015d0: 7263 656e 745f 656e 636f 6465 3a20 626f  rcent_encode: bo
-000015e0: 6f6c 2c0a 2020 2020 2020 2020 7072 6566  ol,.        pref
-000015f0: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
-00001600: 7261 746f 723a 2050 7265 6669 7853 6570  rator: PrefixSep
-00001610: 6172 6174 6f72 4974 6572 6174 6f72 2c0a  aratorIterator,.
-00001620: 2020 2020 2020 2020 7661 725f 6e61 6d65          var_name
-00001630: 5f70 6965 6365 3a20 7374 722c 0a20 2020  _piece: str,.   
-00001640: 2020 2020 206e 616d 6564 5f70 6172 616d       named_param
-00001650: 6574 6572 5f65 7870 616e 7369 6f6e 3a20  eter_expansion: 
-00001660: 626f 6f6c 0a20 2020 2029 202d 3e20 7374  bool.    ) -> st
-00001670: 723a 0a20 2020 2020 2020 2069 7465 6d5f  r:.        item_
-00001680: 7661 6c75 6520 3d20 636c 732e 5f5f 7265  value = cls.__re
-00001690: 6636 3537 305f 6974 656d 5f76 616c 7565  f6570_item_value
-000016a0: 2869 6e5f 6461 7461 2c20 7065 7263 656e  (in_data, percen
-000016b0: 745f 656e 636f 6465 290a 2020 2020 2020  t_encode).      
-000016c0: 2020 6966 2069 7465 6d5f 7661 6c75 6520    if item_value 
-000016d0: 6973 204e 6f6e 6520 6f72 2028 6974 656d  is None or (item
-000016e0: 5f76 616c 7565 203d 3d20 2727 2061 6e64  _value == '' and
-000016f0: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
-00001700: 725f 6974 6572 6174 6f72 2e73 6570 6172  r_iterator.separ
-00001710: 6174 6f72 203d 3d20 273b 2729 3a0a 2020  ator == ';'):.  
-00001720: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00001730: 206e 6578 7428 7072 6566 6978 5f73 6570   next(prefix_sep
-00001740: 6172 6174 6f72 5f69 7465 7261 746f 7229  arator_iterator)
-00001750: 202b 2076 6172 5f6e 616d 655f 7069 6563   + var_name_piec
-00001760: 650a 2020 2020 2020 2020 7661 6c75 655f  e.        value_
-00001770: 7061 6972 5f65 7175 616c 7320 3d20 273d  pair_equals = '=
-00001780: 2720 6966 206e 616d 6564 5f70 6172 616d  ' if named_param
-00001790: 6574 6572 5f65 7870 616e 7369 6f6e 2065  eter_expansion e
-000017a0: 6c73 6520 2727 0a20 2020 2020 2020 2072  lse ''.        r
-000017b0: 6574 7572 6e20 6e65 7874 2870 7265 6669  eturn next(prefi
-000017c0: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-000017d0: 6174 6f72 2920 2b20 7661 725f 6e61 6d65  ator) + var_name
-000017e0: 5f70 6965 6365 202b 2076 616c 7565 5f70  _piece + value_p
-000017f0: 6169 725f 6571 7561 6c73 202b 2069 7465  air_equals + ite
-00001800: 6d5f 7661 6c75 650a 0a20 2020 2040 636c  m_value..    @cl
-00001810: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-00001820: 6620 5f5f 7265 6636 3537 305f 6c69 7374  f __ref6570_list
-00001830: 5f65 7870 616e 7369 6f6e 280a 2020 2020  _expansion(.    
-00001840: 2020 2020 636c 732c 0a20 2020 2020 2020      cls,.       
-00001850: 2076 6172 6961 626c 655f 6e61 6d65 3a20   variable_name: 
-00001860: 7374 722c 0a20 2020 2020 2020 2069 6e5f  str,.        in_
-00001870: 6461 7461 3a20 7479 7069 6e67 2e41 6e79  data: typing.Any
-00001880: 2c0a 2020 2020 2020 2020 6578 706c 6f64  ,.        explod
-00001890: 653a 2062 6f6f 6c2c 0a20 2020 2020 2020  e: bool,.       
-000018a0: 2070 6572 6365 6e74 5f65 6e63 6f64 653a   percent_encode:
-000018b0: 2062 6f6f 6c2c 0a20 2020 2020 2020 2070   bool,.        p
-000018c0: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
-000018d0: 6974 6572 6174 6f72 3a20 5072 6566 6978  iterator: Prefix
-000018e0: 5365 7061 7261 746f 7249 7465 7261 746f  SeparatorIterato
-000018f0: 722c 0a20 2020 2020 2020 2076 6172 5f6e  r,.        var_n
-00001900: 616d 655f 7069 6563 653a 2073 7472 2c0a  ame_piece: str,.
-00001910: 2020 2020 2020 2020 6e61 6d65 645f 7061          named_pa
-00001920: 7261 6d65 7465 725f 6578 7061 6e73 696f  rameter_expansio
-00001930: 6e3a 2062 6f6f 6c0a 2020 2020 2920 2d3e  n: bool.    ) ->
-00001940: 2073 7472 3a0a 2020 2020 2020 2020 6974   str:.        it
-00001950: 656d 5f76 616c 7565 7320 3d20 5b63 6c73  em_values = [cls
-00001960: 2e5f 5f72 6566 3635 3730 5f69 7465 6d5f  .__ref6570_item_
-00001970: 7661 6c75 6528 762c 2070 6572 6365 6e74  value(v, percent
-00001980: 5f65 6e63 6f64 6529 2066 6f72 2076 2069  _encode) for v i
-00001990: 6e20 696e 5f64 6174 615d 0a20 2020 2020  n in_data].     
-000019a0: 2020 2069 7465 6d5f 7661 6c75 6573 203d     item_values =
-000019b0: 205b 7620 666f 7220 7620 696e 2069 7465   [v for v in ite
-000019c0: 6d5f 7661 6c75 6573 2069 6620 7620 6973  m_values if v is
-000019d0: 206e 6f74 204e 6f6e 655d 0a20 2020 2020   not None].     
-000019e0: 2020 2069 6620 6e6f 7420 6974 656d 5f76     if not item_v
-000019f0: 616c 7565 733a 0a20 2020 2020 2020 2020  alues:.         
-00001a00: 2020 2023 2069 676e 6f72 6564 2062 7920     # ignored by 
-00001a10: 7468 6520 6578 7061 6e73 696f 6e20 7072  the expansion pr
-00001a20: 6f63 6573 7320 6874 7470 733a 2f2f 6461  ocess https://da
-00001a30: 7461 7472 6163 6b65 722e 6965 7466 2e6f  tatracker.ietf.o
-00001a40: 7267 2f64 6f63 2f68 746d 6c2f 7266 6336  rg/doc/html/rfc6
-00001a50: 3537 3023 7365 6374 696f 6e2d 332e 322e  570#section-3.2.
-00001a60: 310a 2020 2020 2020 2020 2020 2020 7265  1.            re
-00001a70: 7475 726e 2022 220a 2020 2020 2020 2020  turn "".        
-00001a80: 7661 6c75 655f 7061 6972 5f65 7175 616c  value_pair_equal
-00001a90: 7320 3d20 273d 2720 6966 206e 616d 6564  s = '=' if named
-00001aa0: 5f70 6172 616d 6574 6572 5f65 7870 616e  _parameter_expan
-00001ab0: 7369 6f6e 2065 6c73 6520 2727 0a20 2020  sion else ''.   
-00001ac0: 2020 2020 2069 6620 6e6f 7420 6578 706c       if not expl
-00001ad0: 6f64 653a 0a20 2020 2020 2020 2020 2020  ode:.           
-00001ae0: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
-00001af0: 2020 2020 2020 2020 2020 6e65 7874 2870            next(p
-00001b00: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
-00001b10: 6974 6572 6174 6f72 2920 2b0a 2020 2020  iterator) +.    
-00001b20: 2020 2020 2020 2020 2020 2020 7661 725f              var_
-00001b30: 6e61 6d65 5f70 6965 6365 202b 0a20 2020  name_piece +.   
-00001b40: 2020 2020 2020 2020 2020 2020 2076 616c               val
-00001b50: 7565 5f70 6169 725f 6571 7561 6c73 202b  ue_pair_equals +
-00001b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001b70: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
-00001b80: 725f 6974 6572 6174 6f72 2e69 7465 6d5f  r_iterator.item_
-00001b90: 7365 7061 7261 746f 722e 6a6f 696e 2869  separator.join(i
-00001ba0: 7465 6d5f 7661 6c75 6573 290a 2020 2020  tem_values).    
-00001bb0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00001bc0: 2020 2320 6578 706c 6f64 6564 0a20 2020    # exploded.   
-00001bd0: 2020 2020 2072 6574 7572 6e20 6e65 7874       return next
-00001be0: 2870 7265 6669 785f 7365 7061 7261 746f  (prefix_separato
-00001bf0: 725f 6974 6572 6174 6f72 2920 2b20 6e65  r_iterator) + ne
-00001c00: 7874 2870 7265 6669 785f 7365 7061 7261  xt(prefix_separa
-00001c10: 746f 725f 6974 6572 6174 6f72 292e 6a6f  tor_iterator).jo
-00001c20: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
-00001c30: 5b76 6172 5f6e 616d 655f 7069 6563 6520  [var_name_piece 
-00001c40: 2b20 7661 6c75 655f 7061 6972 5f65 7175  + value_pair_equ
-00001c50: 616c 7320 2b20 7661 6c20 666f 7220 7661  als + val for va
-00001c60: 6c20 696e 2069 7465 6d5f 7661 6c75 6573  l in item_values
-00001c70: 5d0a 2020 2020 2020 2020 290a 0a20 2020  ].        )..   
-00001c80: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00001c90: 2020 6465 6620 5f5f 7265 6636 3537 305f    def __ref6570_
-00001ca0: 6469 6374 5f65 7870 616e 7369 6f6e 280a  dict_expansion(.
-00001cb0: 2020 2020 2020 2020 636c 732c 0a20 2020          cls,.   
-00001cc0: 2020 2020 2076 6172 6961 626c 655f 6e61       variable_na
-00001cd0: 6d65 3a20 7374 722c 0a20 2020 2020 2020  me: str,.       
-00001ce0: 2069 6e5f 6461 7461 3a20 7479 7069 6e67   in_data: typing
-00001cf0: 2e41 6e79 2c0a 2020 2020 2020 2020 6578  .Any,.        ex
-00001d00: 706c 6f64 653a 2062 6f6f 6c2c 0a20 2020  plode: bool,.   
-00001d10: 2020 2020 2070 6572 6365 6e74 5f65 6e63       percent_enc
-00001d20: 6f64 653a 2062 6f6f 6c2c 0a20 2020 2020  ode: bool,.     
-00001d30: 2020 2070 7265 6669 785f 7365 7061 7261     prefix_separa
-00001d40: 746f 725f 6974 6572 6174 6f72 3a20 5072  tor_iterator: Pr
-00001d50: 6566 6978 5365 7061 7261 746f 7249 7465  efixSeparatorIte
-00001d60: 7261 746f 722c 0a20 2020 2020 2020 2076  rator,.        v
-00001d70: 6172 5f6e 616d 655f 7069 6563 653a 2073  ar_name_piece: s
-00001d80: 7472 2c0a 2020 2020 2020 2020 6e61 6d65  tr,.        name
-00001d90: 645f 7061 7261 6d65 7465 725f 6578 7061  d_parameter_expa
-00001da0: 6e73 696f 6e3a 2062 6f6f 6c0a 2020 2020  nsion: bool.    
-00001db0: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-00001dc0: 2020 696e 5f64 6174 615f 7472 616e 7366    in_data_transf
-00001dd0: 6f72 6d65 6420 3d20 7b6b 6579 3a20 636c  ormed = {key: cl
-00001de0: 732e 5f5f 7265 6636 3537 305f 6974 656d  s.__ref6570_item
-00001df0: 5f76 616c 7565 2876 616c 2c20 7065 7263  _value(val, perc
-00001e00: 656e 745f 656e 636f 6465 2920 666f 7220  ent_encode) for 
-00001e10: 6b65 792c 2076 616c 2069 6e20 696e 5f64  key, val in in_d
-00001e20: 6174 612e 6974 656d 7328 297d 0a20 2020  ata.items()}.   
-00001e30: 2020 2020 2069 6e5f 6461 7461 5f74 7261       in_data_tra
-00001e40: 6e73 666f 726d 6564 203d 207b 6b65 793a  nsformed = {key:
-00001e50: 2076 616c 2066 6f72 206b 6579 2c20 7661   val for key, va
-00001e60: 6c20 696e 2069 6e5f 6461 7461 5f74 7261  l in in_data_tra
-00001e70: 6e73 666f 726d 6564 2e69 7465 6d73 2829  nsformed.items()
-00001e80: 2069 6620 7661 6c20 6973 206e 6f74 204e   if val is not N
-00001e90: 6f6e 657d 0a20 2020 2020 2020 2069 6620  one}.        if 
-00001ea0: 6e6f 7420 696e 5f64 6174 615f 7472 616e  not in_data_tran
-00001eb0: 7366 6f72 6d65 643a 0a20 2020 2020 2020  sformed:.       
-00001ec0: 2020 2020 2023 2069 676e 6f72 6564 2062       # ignored b
-00001ed0: 7920 7468 6520 6578 7061 6e73 696f 6e20  y the expansion 
-00001ee0: 7072 6f63 6573 7320 6874 7470 733a 2f2f  process https://
-00001ef0: 6461 7461 7472 6163 6b65 722e 6965 7466  datatracker.ietf
-00001f00: 2e6f 7267 2f64 6f63 2f68 746d 6c2f 7266  .org/doc/html/rf
-00001f10: 6336 3537 3023 7365 6374 696f 6e2d 332e  c6570#section-3.
-00001f20: 322e 310a 2020 2020 2020 2020 2020 2020  2.1.            
-00001f30: 7265 7475 726e 2022 220a 2020 2020 2020  return "".      
-00001f40: 2020 7661 6c75 655f 7061 6972 5f65 7175    value_pair_equ
-00001f50: 616c 7320 3d20 273d 2720 6966 206e 616d  als = '=' if nam
-00001f60: 6564 5f70 6172 616d 6574 6572 5f65 7870  ed_parameter_exp
-00001f70: 616e 7369 6f6e 2065 6c73 6520 2727 0a20  ansion else ''. 
-00001f80: 2020 2020 2020 2069 6620 6e6f 7420 6578         if not ex
-00001f90: 706c 6f64 653a 0a20 2020 2020 2020 2020  plode:.         
-00001fa0: 2020 2072 6574 7572 6e20 280a 2020 2020     return (.    
-00001fb0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00001fc0: 2870 7265 6669 785f 7365 7061 7261 746f  (prefix_separato
-00001fd0: 725f 6974 6572 6174 6f72 2920 2b0a 2020  r_iterator) +.  
-00001fe0: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00001ff0: 725f 6e61 6d65 5f70 6965 6365 202b 2076  r_name_piece + v
-00002000: 616c 7565 5f70 6169 725f 6571 7561 6c73  alue_pair_equals
-00002010: 202b 0a20 2020 2020 2020 2020 2020 2020   +.             
-00002020: 2020 2070 7265 6669 785f 7365 7061 7261     prefix_separa
-00002030: 746f 725f 6974 6572 6174 6f72 2e69 7465  tor_iterator.ite
-00002040: 6d5f 7365 7061 7261 746f 722e 6a6f 696e  m_separator.join
-00002050: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00002060: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
-00002070: 6172 6174 6f72 5f69 7465 7261 746f 722e  arator_iterator.
-00002080: 6974 656d 5f73 6570 6172 6174 6f72 2e6a  item_separator.j
-00002090: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
-000020a0: 2020 2020 2020 2020 2020 2020 2069 7465               ite
-000020b0: 6d5f 7061 6972 0a20 2020 2020 2020 2020  m_pair.         
-000020c0: 2020 2020 2020 2020 2020 2029 2066 6f72             ) for
-000020d0: 2069 7465 6d5f 7061 6972 2069 6e20 696e   item_pair in in
-000020e0: 5f64 6174 615f 7472 616e 7366 6f72 6d65  _data_transforme
-000020f0: 642e 6974 656d 7328 290a 2020 2020 2020  d.items().      
-00002100: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00002110: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00002120: 2020 2320 6578 706c 6f64 6564 0a20 2020    # exploded.   
-00002130: 2020 2020 2072 6574 7572 6e20 6e65 7874       return next
-00002140: 2870 7265 6669 785f 7365 7061 7261 746f  (prefix_separato
-00002150: 725f 6974 6572 6174 6f72 2920 2b20 6e65  r_iterator) + ne
-00002160: 7874 2870 7265 6669 785f 7365 7061 7261  xt(prefix_separa
-00002170: 746f 725f 6974 6572 6174 6f72 292e 6a6f  tor_iterator).jo
-00002180: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
-00002190: 5b6b 6579 202b 2027 3d27 202b 2076 616c  [key + '=' + val
-000021a0: 2066 6f72 206b 6579 2c20 7661 6c20 696e   for key, val in
-000021b0: 2069 6e5f 6461 7461 5f74 7261 6e73 666f   in_data_transfo
-000021c0: 726d 6564 2e69 7465 6d73 2829 5d0a 2020  rmed.items()].  
-000021d0: 2020 2020 2020 290a 0a20 2020 2040 636c        )..    @cl
-000021e0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-000021f0: 6620 5f72 6566 3635 3730 5f65 7870 616e  f _ref6570_expan
-00002200: 7369 6f6e 280a 2020 2020 2020 2020 636c  sion(.        cl
-00002210: 732c 0a20 2020 2020 2020 2076 6172 6961  s,.        varia
-00002220: 626c 655f 6e61 6d65 3a20 7374 722c 0a20  ble_name: str,. 
-00002230: 2020 2020 2020 2069 6e5f 6461 7461 3a20         in_data: 
-00002240: 7479 7069 6e67 2e41 6e79 2c0a 2020 2020  typing.Any,.    
-00002250: 2020 2020 6578 706c 6f64 653a 2062 6f6f      explode: boo
-00002260: 6c2c 0a20 2020 2020 2020 2070 6572 6365  l,.        perce
-00002270: 6e74 5f65 6e63 6f64 653a 2062 6f6f 6c2c  nt_encode: bool,
-00002280: 0a20 2020 2020 2020 2070 7265 6669 785f  .        prefix_
-00002290: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
-000022a0: 6f72 3a20 5072 6566 6978 5365 7061 7261  or: PrefixSepara
-000022b0: 746f 7249 7465 7261 746f 720a 2020 2020  torIterator.    
-000022c0: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-000022d0: 2020 2222 220a 2020 2020 2020 2020 5365    """.        Se
-000022e0: 7061 7261 746f 7220 6973 2066 6f72 2073  parator is for s
-000022f0: 6570 6172 6174 6520 7661 7269 6162 6c65  eparate variable
-00002300: 7320 6c69 6b65 2064 6963 7420 7769 7468  s like dict with
-00002310: 2065 7870 6c6f 6465 2074 7275 652c 206e   explode true, n
-00002320: 6f74 2066 6f72 2061 7272 6179 2069 7465  ot for array ite
-00002330: 6d20 7365 7061 7261 7469 6f6e 0a20 2020  m separation.   
-00002340: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00002350: 206e 616d 6564 5f70 6172 616d 6574 6572   named_parameter
-00002360: 5f65 7870 616e 7369 6f6e 203d 2070 7265  _expansion = pre
-00002370: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
-00002380: 6572 6174 6f72 2e73 6570 6172 6174 6f72  erator.separator
-00002390: 2069 6e20 7b27 2627 2c20 273b 277d 0a20   in {'&', ';'}. 
-000023a0: 2020 2020 2020 2076 6172 5f6e 616d 655f         var_name_
-000023b0: 7069 6563 6520 3d20 7661 7269 6162 6c65  piece = variable
-000023c0: 5f6e 616d 6520 6966 206e 616d 6564 5f70  _name if named_p
-000023d0: 6172 616d 6574 6572 5f65 7870 616e 7369  arameter_expansi
-000023e0: 6f6e 2065 6c73 6520 2727 0a20 2020 2020  on else ''.     
-000023f0: 2020 2069 6620 7479 7065 2869 6e5f 6461     if type(in_da
-00002400: 7461 2920 696e 207b 7374 722c 2066 6c6f  ta) in {str, flo
-00002410: 6174 2c20 696e 747d 3a0a 2020 2020 2020  at, int}:.      
-00002420: 2020 2020 2020 7265 7475 726e 2063 6c73        return cls
-00002430: 2e5f 5f72 6566 3635 3730 5f73 7472 5f66  .__ref6570_str_f
-00002440: 6c6f 6174 5f69 6e74 5f65 7870 616e 7369  loat_int_expansi
-00002450: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00002460: 2020 2020 7661 7269 6162 6c65 5f6e 616d      variable_nam
-00002470: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00002480: 2020 2069 6e5f 6461 7461 2c0a 2020 2020     in_data,.    
-00002490: 2020 2020 2020 2020 2020 2020 6578 706c              expl
-000024a0: 6f64 652c 0a20 2020 2020 2020 2020 2020  ode,.           
-000024b0: 2020 2020 2070 6572 6365 6e74 5f65 6e63       percent_enc
-000024c0: 6f64 652c 0a20 2020 2020 2020 2020 2020  ode,.           
-000024d0: 2020 2020 2070 7265 6669 785f 7365 7061       prefix_sepa
-000024e0: 7261 746f 725f 6974 6572 6174 6f72 2c0a  rator_iterator,.
-000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002500: 7661 725f 6e61 6d65 5f70 6965 6365 2c0a  var_name_piece,.
-00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002520: 6e61 6d65 645f 7061 7261 6d65 7465 725f  named_parameter_
-00002530: 6578 7061 6e73 696f 6e0a 2020 2020 2020  expansion.      
-00002540: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00002550: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-00002560: 696e 5f64 6174 612c 206e 6f6e 655f 7479  in_data, none_ty
-00002570: 7065 293a 0a20 2020 2020 2020 2020 2020  pe):.           
-00002580: 2023 2069 676e 6f72 6564 2062 7920 7468   # ignored by th
-00002590: 6520 6578 7061 6e73 696f 6e20 7072 6f63  e expansion proc
-000025a0: 6573 7320 6874 7470 733a 2f2f 6461 7461  ess https://data
-000025b0: 7472 6163 6b65 722e 6965 7466 2e6f 7267  tracker.ietf.org
-000025c0: 2f64 6f63 2f68 746d 6c2f 7266 6336 3537  /doc/html/rfc657
-000025d0: 3023 7365 6374 696f 6e2d 332e 322e 310a  0#section-3.2.1.
-000025e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000025f0: 726e 2022 220a 2020 2020 2020 2020 656c  rn "".        el
-00002600: 6966 2069 7369 6e73 7461 6e63 6528 696e  if isinstance(in
-00002610: 5f64 6174 612c 206c 6973 7429 3a0a 2020  _data, list):.  
-00002620: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00002630: 2063 6c73 2e5f 5f72 6566 3635 3730 5f6c   cls.__ref6570_l
-00002640: 6973 745f 6578 7061 6e73 696f 6e28 0a20  ist_expansion(. 
-00002650: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00002660: 6172 6961 626c 655f 6e61 6d65 2c0a 2020  ariable_name,.  
-00002670: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00002680: 5f64 6174 612c 0a20 2020 2020 2020 2020  _data,.         
-00002690: 2020 2020 2020 2065 7870 6c6f 6465 2c0a         explode,.
-000026a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026b0: 7065 7263 656e 745f 656e 636f 6465 2c0a  percent_encode,.
-000026c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026d0: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
-000026e0: 5f69 7465 7261 746f 722c 0a20 2020 2020  _iterator,.     
-000026f0: 2020 2020 2020 2020 2020 2076 6172 5f6e             var_n
-00002700: 616d 655f 7069 6563 652c 0a20 2020 2020  ame_piece,.     
-00002710: 2020 2020 2020 2020 2020 206e 616d 6564             named
-00002720: 5f70 6172 616d 6574 6572 5f65 7870 616e  _parameter_expan
-00002730: 7369 6f6e 0a20 2020 2020 2020 2020 2020  sion.           
-00002740: 2029 0a20 2020 2020 2020 2065 6c69 6620   ).        elif 
-00002750: 6973 696e 7374 616e 6365 2869 6e5f 6461  isinstance(in_da
-00002760: 7461 2c20 6469 6374 293a 0a20 2020 2020  ta, dict):.     
-00002770: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
-00002780: 732e 5f5f 7265 6636 3537 305f 6469 6374  s.__ref6570_dict
-00002790: 5f65 7870 616e 7369 6f6e 280a 2020 2020  _expansion(.    
-000027a0: 2020 2020 2020 2020 2020 2020 7661 7269              vari
-000027b0: 6162 6c65 5f6e 616d 652c 0a20 2020 2020  able_name,.     
-000027c0: 2020 2020 2020 2020 2020 2069 6e5f 6461             in_da
-000027d0: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
-000027e0: 2020 2020 6578 706c 6f64 652c 0a20 2020      explode,.   
-000027f0: 2020 2020 2020 2020 2020 2020 2070 6572               per
-00002800: 6365 6e74 5f65 6e63 6f64 652c 0a20 2020  cent_encode,.   
-00002810: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-00002820: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
-00002830: 6572 6174 6f72 2c0a 2020 2020 2020 2020  erator,.        
-00002840: 2020 2020 2020 2020 7661 725f 6e61 6d65          var_name
-00002850: 5f70 6965 6365 2c0a 2020 2020 2020 2020  _piece,.        
-00002860: 2020 2020 2020 2020 6e61 6d65 645f 7061          named_pa
-00002870: 7261 6d65 7465 725f 6578 7061 6e73 696f  rameter_expansio
-00002880: 6e0a 2020 2020 2020 2020 2020 2020 290a  n.            ).
-00002890: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-000028a0: 6e73 7461 6e63 6528 696e 5f64 6174 612c  nstance(in_data,
-000028b0: 2062 6f6f 6c29 3a0a 2020 2020 2020 2020   bool):.        
-000028c0: 2020 2020 7265 7475 726e 2063 6c73 2e5f      return cls._
-000028d0: 5f6b 6f6e 6669 675f 626f 6f6c 5f65 7870  _konfig_bool_exp
-000028e0: 616e 7369 6f6e 280a 2020 2020 2020 2020  ansion(.        
-000028f0: 2020 2020 2020 2020 696e 5f64 6174 612c          in_data,
-00002900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002910: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
-00002920: 725f 6974 6572 6174 6f72 2c0a 2020 2020  r_iterator,.    
-00002930: 2020 2020 2020 2020 2020 2020 7661 725f              var_
-00002940: 6e61 6d65 5f70 6965 6365 2c0a 2020 2020  name_piece,.    
-00002950: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00002960: 645f 7061 7261 6d65 7465 725f 6578 7061  d_parameter_expa
-00002970: 6e73 696f 6e0a 2020 2020 2020 2020 2020  nsion.          
-00002980: 2020 290a 2020 2020 2020 2020 2320 6279    ).        # by
-00002990: 7465 732c 2065 7463 0a20 2020 2020 2020  tes, etc.       
-000029a0: 2072 6169 7365 2041 7069 5661 6c75 6545   raise ApiValueE
-000029b0: 7272 6f72 2827 556e 6162 6c65 2074 6f20  rror('Unable to 
-000029c0: 6765 6e65 7261 7465 2061 2072 6566 3635  generate a ref65
-000029d0: 3730 2072 6570 7265 7365 6e74 6174 696f  70 representatio
-000029e0: 6e20 6f66 207b 7d27 2e66 6f72 6d61 7428  n of {}'.format(
-000029f0: 696e 5f64 6174 6129 290a 0a0a 636c 6173  in_data))...clas
-00002a00: 7320 5374 796c 6546 6f72 6d53 6572 6961  s StyleFormSeria
-00002a10: 6c69 7a65 7228 5061 7261 6d65 7465 7253  lizer(ParameterS
-00002a20: 6572 6961 6c69 7a65 7242 6173 6529 3a0a  erializerBase):.
-00002a30: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-00002a40: 0a20 2020 2064 6566 205f 6765 745f 6465  .    def _get_de
-00002a50: 6661 756c 745f 6578 706c 6f64 6528 636c  fault_explode(cl
-00002a60: 732c 2073 7479 6c65 3a20 5061 7261 6d65  s, style: Parame
-00002a70: 7465 7253 7479 6c65 2920 2d3e 2062 6f6f  terStyle) -> boo
-00002a80: 6c3a 0a20 2020 2020 2020 2069 6620 7374  l:.        if st
-00002a90: 796c 6520 6973 2050 6172 616d 6574 6572  yle is Parameter
-00002aa0: 5374 796c 652e 464f 524d 3a0a 2020 2020  Style.FORM:.    
-00002ab0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00002ac0: 7275 650a 2020 2020 2020 2020 7265 7475  rue.        retu
-00002ad0: 726e 2073 7570 6572 2829 2e5f 6765 745f  rn super()._get_
-00002ae0: 6465 6661 756c 745f 6578 706c 6f64 6528  default_explode(
-00002af0: 7374 796c 6529 0a0a 2020 2020 6465 6620  style)..    def 
-00002b00: 5f73 6572 6961 6c69 7a65 5f66 6f72 6d28  _serialize_form(
-00002b10: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00002b20: 2020 2020 2020 2069 6e5f 6461 7461 3a20         in_data: 
-00002b30: 7479 7069 6e67 2e55 6e69 6f6e 5b4e 6f6e  typing.Union[Non
-00002b40: 652c 2069 6e74 2c20 666c 6f61 742c 2073  e, int, float, s
-00002b50: 7472 2c20 626f 6f6c 2c20 6469 6374 2c20  tr, bool, dict, 
-00002b60: 6c69 7374 5d2c 0a20 2020 2020 2020 206e  list],.        n
-00002b70: 616d 653a 2073 7472 2c0a 2020 2020 2020  ame: str,.      
-00002b80: 2020 6578 706c 6f64 653a 2062 6f6f 6c2c    explode: bool,
-00002b90: 0a20 2020 2020 2020 2070 6572 6365 6e74  .        percent
-00002ba0: 5f65 6e63 6f64 653a 2062 6f6f 6c2c 0a20  _encode: bool,. 
-00002bb0: 2020 2020 2020 2070 7265 6669 785f 7365         prefix_se
-00002bc0: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
-00002bd0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00002be0: 6c5b 5072 6566 6978 5365 7061 7261 746f  l[PrefixSeparato
-00002bf0: 7249 7465 7261 746f 725d 203d 204e 6f6e  rIterator] = Non
-00002c00: 650a 2020 2020 2920 2d3e 2073 7472 3a0a  e.    ) -> str:.
-00002c10: 2020 2020 2020 2020 6966 2070 7265 6669          if prefi
-00002c20: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-00002c30: 6174 6f72 2069 7320 4e6f 6e65 3a0a 2020  ator is None:.  
-00002c40: 2020 2020 2020 2020 2020 7072 6566 6978            prefix
-00002c50: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-00002c60: 746f 7220 3d20 5072 6566 6978 5365 7061  tor = PrefixSepa
-00002c70: 7261 746f 7249 7465 7261 746f 7228 2727  ratorIterator(''
-00002c80: 2c20 2726 2729 0a20 2020 2020 2020 2072  , '&').        r
-00002c90: 6574 7572 6e20 7365 6c66 2e5f 7265 6636  eturn self._ref6
-00002ca0: 3537 305f 6578 7061 6e73 696f 6e28 0a20  570_expansion(. 
-00002cb0: 2020 2020 2020 2020 2020 2076 6172 6961             varia
-00002cc0: 626c 655f 6e61 6d65 3d6e 616d 652c 0a20  ble_name=name,. 
-00002cd0: 2020 2020 2020 2020 2020 2069 6e5f 6461             in_da
-00002ce0: 7461 3d69 6e5f 6461 7461 2c0a 2020 2020  ta=in_data,.    
-00002cf0: 2020 2020 2020 2020 6578 706c 6f64 653d          explode=
-00002d00: 6578 706c 6f64 652c 0a20 2020 2020 2020  explode,.       
-00002d10: 2020 2020 2070 6572 6365 6e74 5f65 6e63       percent_enc
-00002d20: 6f64 653d 7065 7263 656e 745f 656e 636f  ode=percent_enco
-00002d30: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
-00002d40: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
-00002d50: 5f69 7465 7261 746f 723d 7072 6566 6978  _iterator=prefix
-00002d60: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-00002d70: 746f 720a 2020 2020 2020 2020 290a 0a0a  tor.        )...
-00002d80: 636c 6173 7320 5374 796c 6553 696d 706c  class StyleSimpl
-00002d90: 6553 6572 6961 6c69 7a65 7228 5061 7261  eSerializer(Para
-00002da0: 6d65 7465 7253 6572 6961 6c69 7a65 7242  meterSerializerB
-00002db0: 6173 6529 3a0a 0a20 2020 2064 6566 205f  ase):..    def _
-00002dc0: 7365 7269 616c 697a 655f 7369 6d70 6c65  serialize_simple
-00002dd0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00002de0: 2020 2020 2020 2020 696e 5f64 6174 613a          in_data:
-00002df0: 2074 7970 696e 672e 556e 696f 6e5b 4e6f   typing.Union[No
-00002e00: 6e65 2c20 696e 742c 2066 6c6f 6174 2c20  ne, int, float, 
-00002e10: 7374 722c 2062 6f6f 6c2c 2064 6963 742c  str, bool, dict,
-00002e20: 206c 6973 745d 2c0a 2020 2020 2020 2020   list],.        
-00002e30: 6e61 6d65 3a20 7374 722c 0a20 2020 2020  name: str,.     
-00002e40: 2020 2065 7870 6c6f 6465 3a20 626f 6f6c     explode: bool
-00002e50: 2c0a 2020 2020 2020 2020 7065 7263 656e  ,.        percen
-00002e60: 745f 656e 636f 6465 3a20 626f 6f6c 0a20  t_encode: bool. 
-00002e70: 2020 2029 202d 3e20 7374 723a 0a20 2020     ) -> str:.   
-00002e80: 2020 2020 2070 7265 6669 785f 7365 7061       prefix_sepa
-00002e90: 7261 746f 725f 6974 6572 6174 6f72 203d  rator_iterator =
-00002ea0: 2050 7265 6669 7853 6570 6172 6174 6f72   PrefixSeparator
-00002eb0: 4974 6572 6174 6f72 2827 272c 2027 2c27  Iterator('', ','
-00002ec0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00002ed0: 2073 656c 662e 5f72 6566 3635 3730 5f65   self._ref6570_e
-00002ee0: 7870 616e 7369 6f6e 280a 2020 2020 2020  xpansion(.      
-00002ef0: 2020 2020 2020 7661 7269 6162 6c65 5f6e        variable_n
-00002f00: 616d 653d 6e61 6d65 2c0a 2020 2020 2020  ame=name,.      
-00002f10: 2020 2020 2020 696e 5f64 6174 613d 696e        in_data=in
-00002f20: 5f64 6174 612c 0a20 2020 2020 2020 2020  _data,.         
-00002f30: 2020 2065 7870 6c6f 6465 3d65 7870 6c6f     explode=explo
-00002f40: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
-00002f50: 7065 7263 656e 745f 656e 636f 6465 3d70  percent_encode=p
-00002f60: 6572 6365 6e74 5f65 6e63 6f64 652c 0a20  ercent_encode,. 
-00002f70: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
-00002f80: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-00002f90: 6174 6f72 3d70 7265 6669 785f 7365 7061  ator=prefix_sepa
-00002fa0: 7261 746f 725f 6974 6572 6174 6f72 0a20  rator_iterator. 
-00002fb0: 2020 2020 2020 2029 0a0a 0a63 6c61 7373         )...class
-00002fc0: 204a 534f 4e44 6574 6563 746f 723a 0a20   JSONDetector:. 
-00002fd0: 2020 2022 2222 0a20 2020 2057 6f72 6b73     """.    Works
-00002fe0: 2066 6f72 3a0a 2020 2020 6170 706c 6963   for:.    applic
-00002ff0: 6174 696f 6e2f 6a73 6f6e 0a20 2020 2061  ation/json.    a
-00003000: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e3b  pplication/json;
-00003010: 2063 6861 7273 6574 3d55 5446 2d38 0a20   charset=UTF-8. 
-00003020: 2020 2061 7070 6c69 6361 7469 6f6e 2f6a     application/j
-00003030: 736f 6e2d 7061 7463 682b 6a73 6f6e 0a20  son-patch+json. 
-00003040: 2020 2061 7070 6c69 6361 7469 6f6e 2f67     application/g
-00003050: 656f 2b6a 736f 6e0a 2020 2020 2222 220a  eo+json.    """.
-00003060: 2020 2020 5f5f 6a73 6f6e 5f63 6f6e 7465      __json_conte
-00003070: 6e74 5f74 7970 655f 7061 7474 6572 6e20  nt_type_pattern 
-00003080: 3d20 7265 2e63 6f6d 7069 6c65 2822 6170  = re.compile("ap
-00003090: 706c 6963 6174 696f 6e2f 5b5e 2b5d 2a5b  plication/[^+]*[
-000030a0: 2b5d 3f28 6a73 6f6e 293b 3f2e 2a22 290a  +]?(json);?.*").
-000030b0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-000030c0: 640a 2020 2020 6465 6620 5f63 6f6e 7465  d.    def _conte
-000030d0: 6e74 5f74 7970 655f 6973 5f6a 736f 6e28  nt_type_is_json(
-000030e0: 636c 732c 2063 6f6e 7465 6e74 5f74 7970  cls, content_typ
-000030f0: 653a 2073 7472 2920 2d3e 2062 6f6f 6c3a  e: str) -> bool:
-00003100: 0a20 2020 2020 2020 2069 6620 636c 732e  .        if cls.
-00003110: 5f5f 6a73 6f6e 5f63 6f6e 7465 6e74 5f74  __json_content_t
-00003120: 7970 655f 7061 7474 6572 6e2e 6d61 7463  ype_pattern.matc
-00003130: 6828 636f 6e74 656e 745f 7479 7065 293a  h(content_type):
-00003140: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00003150: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
-00003160: 2072 6574 7572 6e20 4661 6c73 650a 0a0a   return False...
-00003170: 4064 6174 6163 6c61 7373 0a63 6c61 7373  @dataclass.class
-00003180: 2050 6172 616d 6574 6572 4261 7365 284a   ParameterBase(J
-00003190: 534f 4e44 6574 6563 746f 7229 3a0a 2020  SONDetector):.  
-000031a0: 2020 6e61 6d65 3a20 7374 720a 2020 2020    name: str.    
-000031b0: 696e 5f74 7970 653a 2050 6172 616d 6574  in_type: Paramet
-000031c0: 6572 496e 5479 7065 0a20 2020 2072 6571  erInType.    req
-000031d0: 7569 7265 643a 2062 6f6f 6c0a 2020 2020  uired: bool.    
-000031e0: 7374 796c 653a 2074 7970 696e 672e 4f70  style: typing.Op
-000031f0: 7469 6f6e 616c 5b50 6172 616d 6574 6572  tional[Parameter
-00003200: 5374 796c 655d 0a20 2020 2065 7870 6c6f  Style].    explo
-00003210: 6465 3a20 7479 7069 6e67 2e4f 7074 696f  de: typing.Optio
-00003220: 6e61 6c5b 626f 6f6c 5d0a 2020 2020 616c  nal[bool].    al
-00003230: 6c6f 775f 7265 7365 7276 6564 3a20 7479  low_reserved: ty
-00003240: 7069 6e67 2e4f 7074 696f 6e61 6c5b 626f  ping.Optional[bo
-00003250: 6f6c 5d0a 2020 2020 7363 6865 6d61 3a20  ol].    schema: 
-00003260: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00003270: 7479 7069 6e67 2e54 7970 655b 5363 6865  typing.Type[Sche
-00003280: 6d61 5d5d 0a20 2020 2063 6f6e 7465 6e74  ma]].    content
-00003290: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-000032a0: 6c5b 7479 7069 6e67 2e44 6963 745b 7374  l[typing.Dict[st
-000032b0: 722c 2074 7970 696e 672e 5479 7065 5b53  r, typing.Type[S
-000032c0: 6368 656d 615d 5d5d 0a0a 2020 2020 5f5f  chema]]]..    __
-000032d0: 7374 796c 655f 746f 5f69 6e5f 7479 7065  style_to_in_type
-000032e0: 203d 207b 0a20 2020 2020 2020 2050 6172   = {.        Par
-000032f0: 616d 6574 6572 5374 796c 652e 4d41 5452  ameterStyle.MATR
-00003300: 4958 3a20 7b50 6172 616d 6574 6572 496e  IX: {ParameterIn
-00003310: 5479 7065 2e50 4154 487d 2c0a 2020 2020  Type.PATH},.    
-00003320: 2020 2020 5061 7261 6d65 7465 7253 7479      ParameterSty
-00003330: 6c65 2e4c 4142 454c 3a20 7b50 6172 616d  le.LABEL: {Param
-00003340: 6574 6572 496e 5479 7065 2e50 4154 487d  eterInType.PATH}
-00003350: 2c0a 2020 2020 2020 2020 5061 7261 6d65  ,.        Parame
-00003360: 7465 7253 7479 6c65 2e46 4f52 4d3a 207b  terStyle.FORM: {
-00003370: 5061 7261 6d65 7465 7249 6e54 7970 652e  ParameterInType.
-00003380: 5155 4552 592c 2050 6172 616d 6574 6572  QUERY, Parameter
-00003390: 496e 5479 7065 2e43 4f4f 4b49 457d 2c0a  InType.COOKIE},.
-000033a0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-000033b0: 7253 7479 6c65 2e53 494d 504c 453a 207b  rStyle.SIMPLE: {
-000033c0: 5061 7261 6d65 7465 7249 6e54 7970 652e  ParameterInType.
-000033d0: 5041 5448 2c20 5061 7261 6d65 7465 7249  PATH, ParameterI
-000033e0: 6e54 7970 652e 4845 4144 4552 7d2c 0a20  nType.HEADER},. 
-000033f0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00003400: 5374 796c 652e 5350 4143 455f 4445 4c49  Style.SPACE_DELI
-00003410: 4d49 5445 443a 207b 5061 7261 6d65 7465  MITED: {Paramete
-00003420: 7249 6e54 7970 652e 5155 4552 597d 2c0a  rInType.QUERY},.
-00003430: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00003440: 7253 7479 6c65 2e50 4950 455f 4445 4c49  rStyle.PIPE_DELI
-00003450: 4d49 5445 443a 207b 5061 7261 6d65 7465  MITED: {Paramete
-00003460: 7249 6e54 7970 652e 5155 4552 597d 2c0a  rInType.QUERY},.
-00003470: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00003480: 7253 7479 6c65 2e44 4545 505f 4f42 4a45  rStyle.DEEP_OBJE
-00003490: 4354 3a20 7b50 6172 616d 6574 6572 496e  CT: {ParameterIn
-000034a0: 5479 7065 2e51 5545 5259 7d2c 0a20 2020  Type.QUERY},.   
-000034b0: 207d 0a20 2020 205f 5f69 6e5f 7479 7065   }.    __in_type
-000034c0: 5f74 6f5f 6465 6661 756c 745f 7374 796c  _to_default_styl
-000034d0: 6520 3d20 7b0a 2020 2020 2020 2020 5061  e = {.        Pa
-000034e0: 7261 6d65 7465 7249 6e54 7970 652e 5155  rameterInType.QU
-000034f0: 4552 593a 2050 6172 616d 6574 6572 5374  ERY: ParameterSt
-00003500: 796c 652e 464f 524d 2c0a 2020 2020 2020  yle.FORM,.      
-00003510: 2020 5061 7261 6d65 7465 7249 6e54 7970    ParameterInTyp
-00003520: 652e 5041 5448 3a20 5061 7261 6d65 7465  e.PATH: Paramete
-00003530: 7253 7479 6c65 2e53 494d 504c 452c 0a20  rStyle.SIMPLE,. 
-00003540: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00003550: 496e 5479 7065 2e48 4541 4445 523a 2050  InType.HEADER: P
-00003560: 6172 616d 6574 6572 5374 796c 652e 5349  arameterStyle.SI
-00003570: 4d50 4c45 2c0a 2020 2020 2020 2020 5061  MPLE,.        Pa
-00003580: 7261 6d65 7465 7249 6e54 7970 652e 434f  rameterInType.CO
-00003590: 4f4b 4945 3a20 5061 7261 6d65 7465 7253  OKIE: ParameterS
-000035a0: 7479 6c65 2e46 4f52 4d2c 0a20 2020 207d  tyle.FORM,.    }
-000035b0: 0a20 2020 205f 5f64 6973 616c 6c6f 7765  .    __disallowe
-000035c0: 645f 6865 6164 6572 5f6e 616d 6573 203d  d_header_names =
-000035d0: 207b 2741 6363 6570 7427 2c20 2743 6f6e   {'Accept', 'Con
-000035e0: 7465 6e74 2d54 7970 6527 2c20 2741 7574  tent-Type', 'Aut
-000035f0: 686f 7269 7a61 7469 6f6e 277d 0a20 2020  horization'}.   
-00003600: 205f 6a73 6f6e 5f65 6e63 6f64 6572 203d   _json_encoder =
-00003610: 204a 534f 4e45 6e63 6f64 6572 2829 0a0a   JSONEncoder()..
-00003620: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-00003630: 0a20 2020 2064 6566 205f 5f76 6572 6966  .    def __verif
-00003640: 795f 7374 796c 655f 746f 5f69 6e5f 7479  y_style_to_in_ty
-00003650: 7065 2863 6c73 2c20 7374 796c 653a 2074  pe(cls, style: t
-00003660: 7970 696e 672e 4f70 7469 6f6e 616c 5b50  yping.Optional[P
-00003670: 6172 616d 6574 6572 5374 796c 655d 2c20  arameterStyle], 
-00003680: 696e 5f74 7970 653a 2050 6172 616d 6574  in_type: Paramet
-00003690: 6572 496e 5479 7065 293a 0a20 2020 2020  erInType):.     
-000036a0: 2020 2069 6620 7374 796c 6520 6973 204e     if style is N
-000036b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000036c0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-000036d0: 696e 5f74 7970 655f 7365 7420 3d20 636c  in_type_set = cl
-000036e0: 732e 5f5f 7374 796c 655f 746f 5f69 6e5f  s.__style_to_in_
-000036f0: 7479 7065 5b73 7479 6c65 5d0a 2020 2020  type[style].    
-00003700: 2020 2020 6966 2069 6e5f 7479 7065 206e      if in_type n
-00003710: 6f74 2069 6e20 696e 5f74 7970 655f 7365  ot in in_type_se
-00003720: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
-00003730: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00003740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003750: 2027 496e 7661 6c69 6420 7374 796c 6520   'Invalid style 
-00003760: 616e 6420 696e 5f74 7970 6520 636f 6d62  and in_type comb
-00003770: 696e 6174 696f 6e2e 2046 6f72 2073 7479  ination. For sty
-00003780: 6c65 3d7b 7d20 6f6e 6c79 2069 6e5f 7479  le={} only in_ty
-00003790: 7065 3d7b 7d20 6172 6520 616c 6c6f 7765  pe={} are allowe
-000037a0: 6427 2e66 6f72 6d61 7428 0a20 2020 2020  d'.format(.     
-000037b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000037c0: 7479 6c65 2c20 696e 5f74 7970 655f 7365  tyle, in_type_se
-000037d0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-000037e0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-000037f0: 290a 0a20 2020 2064 6566 205f 5f69 6e69  )..    def __ini
-00003800: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00003810: 662c 0a20 2020 2020 2020 206e 616d 653a  f,.        name:
-00003820: 2073 7472 2c0a 2020 2020 2020 2020 696e   str,.        in
-00003830: 5f74 7970 653a 2050 6172 616d 6574 6572  _type: Parameter
-00003840: 496e 5479 7065 2c0a 2020 2020 2020 2020  InType,.        
-00003850: 7265 7175 6972 6564 3a20 626f 6f6c 203d  required: bool =
-00003860: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-00003870: 7374 796c 653a 2074 7970 696e 672e 4f70  style: typing.Op
-00003880: 7469 6f6e 616c 5b50 6172 616d 6574 6572  tional[Parameter
-00003890: 5374 796c 655d 203d 204e 6f6e 652c 0a20  Style] = None,. 
-000038a0: 2020 2020 2020 2065 7870 6c6f 6465 3a20         explode: 
-000038b0: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-000038c0: 2020 2020 2020 616c 6c6f 775f 7265 7365        allow_rese
-000038d0: 7276 6564 3a20 7479 7069 6e67 2e4f 7074  rved: typing.Opt
-000038e0: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
-000038f0: 6e65 2c0a 2020 2020 2020 2020 7363 6865  ne,.        sche
-00003900: 6d61 3a20 7479 7069 6e67 2e4f 7074 696f  ma: typing.Optio
-00003910: 6e61 6c5b 7479 7069 6e67 2e54 7970 655b  nal[typing.Type[
-00003920: 5363 6865 6d61 5d5d 203d 204e 6f6e 652c  Schema]] = None,
-00003930: 0a20 2020 2020 2020 2063 6f6e 7465 6e74  .        content
-00003940: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00003950: 6c5b 7479 7069 6e67 2e44 6963 745b 7374  l[typing.Dict[st
-00003960: 722c 2074 7970 696e 672e 5479 7065 5b53  r, typing.Type[S
-00003970: 6368 656d 615d 5d5d 203d 204e 6f6e 650a  chema]]] = None.
-00003980: 2020 2020 293a 0a20 2020 2020 2020 2069      ):.        i
-00003990: 6620 7363 6865 6d61 2069 7320 4e6f 6e65  f schema is None
-000039a0: 2061 6e64 2063 6f6e 7465 6e74 2069 7320   and content is 
-000039b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000039c0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-000039d0: 6f72 2827 5661 6c75 6520 6d69 7373 696e  or('Value missin
-000039e0: 673b 2050 6173 7320 696e 2065 6974 6865  g; Pass in eithe
-000039f0: 7220 7363 6865 6d61 206f 7220 636f 6e74  r schema or cont
-00003a00: 656e 7427 290a 2020 2020 2020 2020 6966  ent').        if
-00003a10: 2073 6368 656d 6120 616e 6420 636f 6e74   schema and cont
-00003a20: 656e 743a 0a20 2020 2020 2020 2020 2020  ent:.           
-00003a30: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00003a40: 7228 2754 6f6f 206d 616e 7920 7661 6c75  r('Too many valu
-00003a50: 6573 2070 726f 7669 6465 642e 2042 6f74  es provided. Bot
-00003a60: 6820 7363 6865 6d61 2061 6e64 2063 6f6e  h schema and con
-00003a70: 7465 6e74 2077 6572 6520 7072 6f76 6964  tent were provid
-00003a80: 6564 2e20 4f6e 6c79 206f 6e65 206d 6179  ed. Only one may
-00003a90: 2062 6520 696e 7075 7427 290a 2020 2020   be input').    
-00003aa0: 2020 2020 6966 206e 616d 6520 696e 2073      if name in s
-00003ab0: 656c 662e 5f5f 6469 7361 6c6c 6f77 6564  elf.__disallowed
-00003ac0: 5f68 6561 6465 725f 6e61 6d65 7320 616e  _header_names an
-00003ad0: 6420 696e 5f74 7970 6520 6973 2050 6172  d in_type is Par
-00003ae0: 616d 6574 6572 496e 5479 7065 2e48 4541  ameterInType.HEA
-00003af0: 4445 523a 0a20 2020 2020 2020 2020 2020  DER:.           
-00003b00: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00003b10: 7228 2749 6e76 616c 6964 206e 616d 652c  r('Invalid name,
-00003b20: 206e 616d 6520 6d61 7920 6e6f 7420 6265   name may not be
-00003b30: 206f 6e65 206f 6620 7b7d 272e 666f 726d   one of {}'.form
-00003b40: 6174 2873 656c 662e 5f5f 6469 7361 6c6c  at(self.__disall
-00003b50: 6f77 6564 5f68 6561 6465 725f 6e61 6d65  owed_header_name
-00003b60: 7329 290a 2020 2020 2020 2020 7365 6c66  s)).        self
-00003b70: 2e5f 5f76 6572 6966 795f 7374 796c 655f  .__verify_style_
-00003b80: 746f 5f69 6e5f 7479 7065 2873 7479 6c65  to_in_type(style
-00003b90: 2c20 696e 5f74 7970 6529 0a20 2020 2020  , in_type).     
-00003ba0: 2020 2069 6620 636f 6e74 656e 7420 6973     if content is
-00003bb0: 204e 6f6e 6520 616e 6420 7374 796c 6520   None and style 
-00003bc0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00003bd0: 2020 2020 2073 7479 6c65 203d 2073 656c       style = sel
-00003be0: 662e 5f5f 696e 5f74 7970 655f 746f 5f64  f.__in_type_to_d
-00003bf0: 6566 6175 6c74 5f73 7479 6c65 5b69 6e5f  efault_style[in_
-00003c00: 7479 7065 5d0a 2020 2020 2020 2020 6966  type].        if
-00003c10: 2063 6f6e 7465 6e74 2069 7320 6e6f 7420   content is not 
-00003c20: 4e6f 6e65 2061 6e64 2069 6e5f 7479 7065  None and in_type
-00003c30: 2069 6e20 7365 6c66 2e5f 5f69 6e5f 7479   in self.__in_ty
-00003c40: 7065 5f74 6f5f 6465 6661 756c 745f 7374  pe_to_default_st
-00003c50: 796c 6520 616e 6420 6c65 6e28 636f 6e74  yle and len(cont
-00003c60: 656e 7429 2021 3d20 313a 0a20 2020 2020  ent) != 1:.     
-00003c70: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00003c80: 7565 4572 726f 7228 2749 6e76 616c 6964  ueError('Invalid
-00003c90: 2063 6f6e 7465 6e74 206c 656e 6774 682c   content length,
-00003ca0: 2063 6f6e 7465 6e74 206c 656e 6774 6820   content length 
-00003cb0: 6d75 7374 2065 7175 616c 2031 2729 0a20  must equal 1'). 
-00003cc0: 2020 2020 2020 2073 656c 662e 696e 5f74         self.in_t
-00003cd0: 7970 6520 3d20 696e 5f74 7970 650a 2020  ype = in_type.  
-00003ce0: 2020 2020 2020 7365 6c66 2e6e 616d 6520        self.name 
-00003cf0: 3d20 6e61 6d65 0a20 2020 2020 2020 2073  = name.        s
-00003d00: 656c 662e 7265 7175 6972 6564 203d 2072  elf.required = r
-00003d10: 6571 7569 7265 640a 2020 2020 2020 2020  equired.        
-00003d20: 7365 6c66 2e73 7479 6c65 203d 2073 7479  self.style = sty
-00003d30: 6c65 0a20 2020 2020 2020 2073 656c 662e  le.        self.
-00003d40: 6578 706c 6f64 6520 3d20 6578 706c 6f64  explode = explod
-00003d50: 650a 2020 2020 2020 2020 7365 6c66 2e61  e.        self.a
-00003d60: 6c6c 6f77 5f72 6573 6572 7665 6420 3d20  llow_reserved = 
-00003d70: 616c 6c6f 775f 7265 7365 7276 6564 0a20  allow_reserved. 
-00003d80: 2020 2020 2020 2073 656c 662e 7363 6865         self.sche
-00003d90: 6d61 203d 2073 6368 656d 610a 2020 2020  ma = schema.    
-00003da0: 2020 2020 7365 6c66 2e63 6f6e 7465 6e74      self.content
-00003db0: 203d 2063 6f6e 7465 6e74 0a0a 2020 2020   = content..    
-00003dc0: 6465 6620 5f73 6572 6961 6c69 7a65 5f6a  def _serialize_j
-00003dd0: 736f 6e28 0a20 2020 2020 2020 2073 656c  son(.        sel
-00003de0: 662c 0a20 2020 2020 2020 2069 6e5f 6461  f,.        in_da
-00003df0: 7461 3a20 7479 7069 6e67 2e55 6e69 6f6e  ta: typing.Union
-00003e00: 5b4e 6f6e 652c 2069 6e74 2c20 666c 6f61  [None, int, floa
-00003e10: 742c 2073 7472 2c20 626f 6f6c 2c20 6469  t, str, bool, di
-00003e20: 6374 2c20 6c69 7374 5d2c 0a20 2020 2020  ct, list],.     
-00003e30: 2020 2065 6c69 6d69 6e61 7465 5f77 6869     eliminate_whi
-00003e40: 7465 7370 6163 653a 2062 6f6f 6c20 3d20  tespace: bool = 
-00003e50: 4661 6c73 650a 2020 2020 2920 2d3e 2073  False.    ) -> s
-00003e60: 7472 3a0a 2020 2020 2020 2020 6966 2065  tr:.        if e
-00003e70: 6c69 6d69 6e61 7465 5f77 6869 7465 7370  liminate_whitesp
-00003e80: 6163 653a 0a20 2020 2020 2020 2020 2020  ace:.           
-00003e90: 2072 6574 7572 6e20 6a73 6f6e 2e64 756d   return json.dum
-00003ea0: 7073 2869 6e5f 6461 7461 2c20 7365 7061  ps(in_data, sepa
-00003eb0: 7261 746f 7273 3d73 656c 662e 5f6a 736f  rators=self._jso
-00003ec0: 6e5f 656e 636f 6465 722e 636f 6d70 6163  n_encoder.compac
-00003ed0: 745f 7365 7061 7261 746f 7273 290a 2020  t_separators).  
-00003ee0: 2020 2020 2020 7265 7475 726e 206a 736f        return jso
-00003ef0: 6e2e 6475 6d70 7328 696e 5f64 6174 6129  n.dumps(in_data)
-00003f00: 0a0a 0a63 6c61 7373 2050 6174 6850 6172  ...class PathPar
-00003f10: 616d 6574 6572 2850 6172 616d 6574 6572  ameter(Parameter
-00003f20: 4261 7365 2c20 5374 796c 6553 696d 706c  Base, StyleSimpl
-00003f30: 6553 6572 6961 6c69 7a65 7229 3a0a 0a20  eSerializer):.. 
-00003f40: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00003f50: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00003f60: 2020 2020 2020 206e 616d 653a 2073 7472         name: str
-00003f70: 2c0a 2020 2020 2020 2020 7265 7175 6972  ,.        requir
-00003f80: 6564 3a20 626f 6f6c 203d 2046 616c 7365  ed: bool = False
-00003f90: 2c0a 2020 2020 2020 2020 7374 796c 653a  ,.        style:
-00003fa0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00003fb0: 5b50 6172 616d 6574 6572 5374 796c 655d  [ParameterStyle]
-00003fc0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00003fd0: 2065 7870 6c6f 6465 3a20 626f 6f6c 203d   explode: bool =
-00003fe0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-00003ff0: 616c 6c6f 775f 7265 7365 7276 6564 3a20  allow_reserved: 
-00004000: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00004010: 626f 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020  bool] = None,.  
-00004020: 2020 2020 2020 7363 6865 6d61 3a20 7479        schema: ty
-00004030: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-00004040: 7069 6e67 2e54 7970 655b 5363 6865 6d61  ping.Type[Schema
-00004050: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-00004060: 2020 2063 6f6e 7465 6e74 3a20 7479 7069     content: typi
-00004070: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-00004080: 6e67 2e44 6963 745b 7374 722c 2074 7970  ng.Dict[str, typ
-00004090: 696e 672e 5479 7065 5b53 6368 656d 615d  ing.Type[Schema]
-000040a0: 5d5d 203d 204e 6f6e 650a 2020 2020 293a  ]] = None.    ):
-000040b0: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-000040c0: 2e5f 5f69 6e69 745f 5f28 0a20 2020 2020  .__init__(.     
-000040d0: 2020 2020 2020 206e 616d 652c 0a20 2020         name,.   
-000040e0: 2020 2020 2020 2020 2069 6e5f 7479 7065           in_type
-000040f0: 3d50 6172 616d 6574 6572 496e 5479 7065  =ParameterInType
-00004100: 2e50 4154 482c 0a20 2020 2020 2020 2020  .PATH,.         
-00004110: 2020 2072 6571 7569 7265 643d 7265 7175     required=requ
-00004120: 6972 6564 2c0a 2020 2020 2020 2020 2020  ired,.          
-00004130: 2020 7374 796c 653d 7374 796c 652c 0a20    style=style,. 
-00004140: 2020 2020 2020 2020 2020 2065 7870 6c6f             explo
-00004150: 6465 3d65 7870 6c6f 6465 2c0a 2020 2020  de=explode,.    
-00004160: 2020 2020 2020 2020 616c 6c6f 775f 7265          allow_re
-00004170: 7365 7276 6564 3d61 6c6c 6f77 5f72 6573  served=allow_res
-00004180: 6572 7665 642c 0a20 2020 2020 2020 2020  erved,.         
-00004190: 2020 2073 6368 656d 613d 7363 6865 6d61     schema=schema
-000041a0: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
-000041b0: 6e74 656e 743d 636f 6e74 656e 740a 2020  ntent=content.  
-000041c0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-000041d0: 205f 5f73 6572 6961 6c69 7a65 5f6c 6162   __serialize_lab
-000041e0: 656c 280a 2020 2020 2020 2020 7365 6c66  el(.        self
-000041f0: 2c0a 2020 2020 2020 2020 696e 5f64 6174  ,.        in_dat
-00004200: 613a 2074 7970 696e 672e 556e 696f 6e5b  a: typing.Union[
-00004210: 4e6f 6e65 2c20 696e 742c 2066 6c6f 6174  None, int, float
-00004220: 2c20 7374 722c 2062 6f6f 6c2c 2064 6963  , str, bool, dic
-00004230: 742c 206c 6973 745d 0a20 2020 2029 202d  t, list].    ) -
-00004240: 3e20 7479 7069 6e67 2e44 6963 745b 7374  > typing.Dict[st
-00004250: 722c 2073 7472 5d3a 0a20 2020 2020 2020  r, str]:.       
-00004260: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
-00004270: 725f 6974 6572 6174 6f72 203d 2050 7265  r_iterator = Pre
-00004280: 6669 7853 6570 6172 6174 6f72 4974 6572  fixSeparatorIter
-00004290: 6174 6f72 2827 2e27 2c20 272e 2729 0a20  ator('.', '.'). 
-000042a0: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
-000042b0: 656c 662e 5f72 6566 3635 3730 5f65 7870  elf._ref6570_exp
-000042c0: 616e 7369 6f6e 280a 2020 2020 2020 2020  ansion(.        
-000042d0: 2020 2020 7661 7269 6162 6c65 5f6e 616d      variable_nam
-000042e0: 653d 7365 6c66 2e6e 616d 652c 0a20 2020  e=self.name,.   
-000042f0: 2020 2020 2020 2020 2069 6e5f 6461 7461           in_data
-00004300: 3d69 6e5f 6461 7461 2c0a 2020 2020 2020  =in_data,.      
-00004310: 2020 2020 2020 6578 706c 6f64 653d 7365        explode=se
-00004320: 6c66 2e65 7870 6c6f 6465 2c0a 2020 2020  lf.explode,.    
-00004330: 2020 2020 2020 2020 7065 7263 656e 745f          percent_
-00004340: 656e 636f 6465 3d54 7275 652c 0a20 2020  encode=True,.   
-00004350: 2020 2020 2020 2020 2070 7265 6669 785f           prefix_
-00004360: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
-00004370: 6f72 3d70 7265 6669 785f 7365 7061 7261  or=prefix_separa
-00004380: 746f 725f 6974 6572 6174 6f72 0a20 2020  tor_iterator.   
-00004390: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
-000043a0: 6574 7572 6e20 7365 6c66 2e5f 746f 5f64  eturn self._to_d
-000043b0: 6963 7428 7365 6c66 2e6e 616d 652c 2076  ict(self.name, v
-000043c0: 616c 7565 290a 0a20 2020 2064 6566 205f  alue)..    def _
-000043d0: 5f73 6572 6961 6c69 7a65 5f6d 6174 7269  _serialize_matri
-000043e0: 7828 0a20 2020 2020 2020 2073 656c 662c  x(.        self,
-000043f0: 0a20 2020 2020 2020 2069 6e5f 6461 7461  .        in_data
-00004400: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b4e  : typing.Union[N
-00004410: 6f6e 652c 2069 6e74 2c20 666c 6f61 742c  one, int, float,
-00004420: 2073 7472 2c20 626f 6f6c 2c20 6469 6374   str, bool, dict
-00004430: 2c20 6c69 7374 5d0a 2020 2020 2920 2d3e  , list].    ) ->
-00004440: 2074 7970 696e 672e 4469 6374 5b73 7472   typing.Dict[str
-00004450: 2c20 7374 725d 3a0a 2020 2020 2020 2020  , str]:.        
-00004460: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
-00004470: 5f69 7465 7261 746f 7220 3d20 5072 6566  _iterator = Pref
-00004480: 6978 5365 7061 7261 746f 7249 7465 7261  ixSeparatorItera
-00004490: 746f 7228 273b 272c 2027 3b27 290a 2020  tor(';', ';').  
-000044a0: 2020 2020 2020 7661 6c75 6520 3d20 7365        value = se
-000044b0: 6c66 2e5f 7265 6636 3537 305f 6578 7061  lf._ref6570_expa
-000044c0: 6e73 696f 6e28 0a20 2020 2020 2020 2020  nsion(.         
-000044d0: 2020 2076 6172 6961 626c 655f 6e61 6d65     variable_name
-000044e0: 3d73 656c 662e 6e61 6d65 2c0a 2020 2020  =self.name,.    
-000044f0: 2020 2020 2020 2020 696e 5f64 6174 613d          in_data=
-00004500: 696e 5f64 6174 612c 0a20 2020 2020 2020  in_data,.       
-00004510: 2020 2020 2065 7870 6c6f 6465 3d73 656c       explode=sel
-00004520: 662e 6578 706c 6f64 652c 0a20 2020 2020  f.explode,.     
-00004530: 2020 2020 2020 2070 6572 6365 6e74 5f65         percent_e
-00004540: 6e63 6f64 653d 5472 7565 2c0a 2020 2020  ncode=True,.    
-00004550: 2020 2020 2020 2020 7072 6566 6978 5f73          prefix_s
-00004560: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
-00004570: 723d 7072 6566 6978 5f73 6570 6172 6174  r=prefix_separat
-00004580: 6f72 5f69 7465 7261 746f 720a 2020 2020  or_iterator.    
-00004590: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
-000045a0: 7475 726e 2073 656c 662e 5f74 6f5f 6469  turn self._to_di
-000045b0: 6374 2873 656c 662e 6e61 6d65 2c20 7661  ct(self.name, va
-000045c0: 6c75 6529 0a0a 2020 2020 6465 6620 5f5f  lue)..    def __
-000045d0: 7365 7269 616c 697a 655f 7369 6d70 6c65  serialize_simple
-000045e0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000045f0: 2020 2020 2020 2020 696e 5f64 6174 613a          in_data:
-00004600: 2074 7970 696e 672e 556e 696f 6e5b 4e6f   typing.Union[No
-00004610: 6e65 2c20 696e 742c 2066 6c6f 6174 2c20  ne, int, float, 
-00004620: 7374 722c 2062 6f6f 6c2c 2064 6963 742c  str, bool, dict,
-00004630: 206c 6973 745d 2c0a 2020 2020 2920 2d3e   list],.    ) ->
-00004640: 2074 7970 696e 672e 4469 6374 5b73 7472   typing.Dict[str
-00004650: 2c20 7374 725d 3a0a 2020 2020 2020 2020  , str]:.        
-00004660: 7661 6c75 6520 3d20 7365 6c66 2e5f 7365  value = self._se
-00004670: 7269 616c 697a 655f 7369 6d70 6c65 280a  rialize_simple(.
-00004680: 2020 2020 2020 2020 2020 2020 696e 5f64              in_d
-00004690: 6174 613d 696e 5f64 6174 612c 0a20 2020  ata=in_data,.   
-000046a0: 2020 2020 2020 2020 206e 616d 653d 7365           name=se
-000046b0: 6c66 2e6e 616d 652c 0a20 2020 2020 2020  lf.name,.       
-000046c0: 2020 2020 2065 7870 6c6f 6465 3d73 656c       explode=sel
-000046d0: 662e 6578 706c 6f64 652c 0a20 2020 2020  f.explode,.     
-000046e0: 2020 2020 2020 2070 6572 6365 6e74 5f65         percent_e
-000046f0: 6e63 6f64 653d 5472 7565 0a20 2020 2020  ncode=True.     
-00004700: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
-00004710: 7572 6e20 7365 6c66 2e5f 746f 5f64 6963  urn self._to_dic
-00004720: 7428 7365 6c66 2e6e 616d 652c 2076 616c  t(self.name, val
-00004730: 7565 290a 0a20 2020 2064 6566 2073 6572  ue)..    def ser
-00004740: 6961 6c69 7a65 280a 2020 2020 2020 2020  ialize(.        
-00004750: 7365 6c66 2c0a 2020 2020 2020 2020 696e  self,.        in
-00004760: 5f64 6174 613a 2074 7970 696e 672e 556e  _data: typing.Un
-00004770: 696f 6e5b 0a20 2020 2020 2020 2020 2020  ion[.           
-00004780: 2053 6368 656d 612c 2044 6563 696d 616c   Schema, Decimal
-00004790: 2c20 696e 742c 2066 6c6f 6174 2c20 7374  , int, float, st
-000047a0: 722c 2064 6174 652c 2064 6174 6574 696d  r, date, datetim
-000047b0: 652c 204e 6f6e 652c 2062 6f6f 6c2c 206c  e, None, bool, l
-000047c0: 6973 742c 2074 7570 6c65 2c20 6469 6374  ist, tuple, dict
-000047d0: 2c20 6672 6f7a 656e 6469 6374 2e66 726f  , frozendict.fro
-000047e0: 7a65 6e64 6963 745d 0a20 2020 2029 202d  zendict].    ) -
-000047f0: 3e20 7479 7069 6e67 2e44 6963 745b 7374  > typing.Dict[st
-00004800: 722c 2073 7472 5d3a 0a20 2020 2020 2020  r, str]:.       
-00004810: 2069 6620 7365 6c66 2e73 6368 656d 613a   if self.schema:
-00004820: 0a20 2020 2020 2020 2020 2020 2063 6173  .            cas
-00004830: 745f 696e 5f64 6174 6120 3d20 7365 6c66  t_in_data = self
-00004840: 2e73 6368 656d 6128 696e 5f64 6174 6129  .schema(in_data)
-00004850: 0a20 2020 2020 2020 2020 2020 2063 6173  .            cas
-00004860: 745f 696e 5f64 6174 6120 3d20 7365 6c66  t_in_data = self
-00004870: 2e5f 6a73 6f6e 5f65 6e63 6f64 6572 2e64  ._json_encoder.d
-00004880: 6566 6175 6c74 2863 6173 745f 696e 5f64  efault(cast_in_d
-00004890: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
-000048a0: 2022 2222 0a20 2020 2020 2020 2020 2020   """.           
-000048b0: 2073 696d 706c 6520 2d3e 2070 6174 680a   simple -> path.
-000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048d0: 7061 7468 3a0a 2020 2020 2020 2020 2020  path:.          
-000048e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000048f0: 7320 7061 7468 5f70 6172 616d 733a 2064  s path_params: d
-00004900: 6963 740a 2020 2020 2020 2020 2020 2020  ict.            
-00004910: 6c61 6265 6c20 2d3e 2070 6174 680a 2020  label -> path.  
-00004920: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00004930: 7475 726e 7320 7061 7468 5f70 6172 616d  turns path_param
-00004940: 730a 2020 2020 2020 2020 2020 2020 6d61  s.            ma
-00004950: 7472 6978 202d 3e20 7061 7468 0a20 2020  trix -> path.   
-00004960: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00004970: 7572 6e73 2070 6174 685f 7061 7261 6d73  urns path_params
-00004980: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
-00004990: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000049a0: 7365 6c66 2e73 7479 6c65 3a0a 2020 2020  self.style:.    
-000049b0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000049c0: 656c 662e 7374 796c 6520 6973 2050 6172  elf.style is Par
-000049d0: 616d 6574 6572 5374 796c 652e 5349 4d50  ameterStyle.SIMP
-000049e0: 4c45 3a0a 2020 2020 2020 2020 2020 2020  LE:.            
-000049f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00004a00: 656c 662e 5f5f 7365 7269 616c 697a 655f  elf.__serialize_
-00004a10: 7369 6d70 6c65 2863 6173 745f 696e 5f64  simple(cast_in_d
-00004a20: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
-00004a30: 2020 2020 2065 6c69 6620 7365 6c66 2e73       elif self.s
-00004a40: 7479 6c65 2069 7320 5061 7261 6d65 7465  tyle is Paramete
-00004a50: 7253 7479 6c65 2e4c 4142 454c 3a0a 2020  rStyle.LABEL:.  
-00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a70: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
-00004a80: 7365 7269 616c 697a 655f 6c61 6265 6c28  serialize_label(
-00004a90: 6361 7374 5f69 6e5f 6461 7461 290a 2020  cast_in_data).  
-00004aa0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00004ab0: 6966 2073 656c 662e 7374 796c 6520 6973  if self.style is
-00004ac0: 2050 6172 616d 6574 6572 5374 796c 652e   ParameterStyle.
-00004ad0: 4d41 5452 4958 3a0a 2020 2020 2020 2020  MATRIX:.        
-00004ae0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00004af0: 726e 2073 656c 662e 5f5f 7365 7269 616c  rn self.__serial
-00004b00: 697a 655f 6d61 7472 6978 2863 6173 745f  ize_matrix(cast_
-00004b10: 696e 5f64 6174 6129 0a20 2020 2020 2020  in_data).       
-00004b20: 2023 2073 656c 662e 636f 6e74 656e 7420   # self.content 
-00004b30: 7769 6c6c 2062 6520 6c65 6e67 7468 206f  will be length o
-00004b40: 6e65 0a20 2020 2020 2020 2066 6f72 2063  ne.        for c
-00004b50: 6f6e 7465 6e74 5f74 7970 652c 2073 6368  ontent_type, sch
-00004b60: 656d 6120 696e 2073 656c 662e 636f 6e74  ema in self.cont
-00004b70: 656e 742e 6974 656d 7328 293a 0a20 2020  ent.items():.   
-00004b80: 2020 2020 2020 2020 2063 6173 745f 696e           cast_in
-00004b90: 5f64 6174 6120 3d20 7363 6865 6d61 2869  _data = schema(i
-00004ba0: 6e5f 6461 7461 290a 2020 2020 2020 2020  n_data).        
-00004bb0: 2020 2020 6361 7374 5f69 6e5f 6461 7461      cast_in_data
-00004bc0: 203d 2073 656c 662e 5f6a 736f 6e5f 656e   = self._json_en
-00004bd0: 636f 6465 722e 6465 6661 756c 7428 6361  coder.default(ca
-00004be0: 7374 5f69 6e5f 6461 7461 290a 2020 2020  st_in_data).    
-00004bf0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00004c00: 5f63 6f6e 7465 6e74 5f74 7970 655f 6973  _content_type_is
-00004c10: 5f6a 736f 6e28 636f 6e74 656e 745f 7479  _json(content_ty
-00004c20: 7065 293a 0a20 2020 2020 2020 2020 2020  pe):.           
-00004c30: 2020 2020 2076 616c 7565 203d 2073 656c       value = sel
-00004c40: 662e 5f73 6572 6961 6c69 7a65 5f6a 736f  f._serialize_jso
-00004c50: 6e28 6361 7374 5f69 6e5f 6461 7461 290a  n(cast_in_data).
-00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c70: 7265 7475 726e 2073 656c 662e 5f74 6f5f  return self._to_
-00004c80: 6469 6374 2873 656c 662e 6e61 6d65 2c20  dict(self.name, 
-00004c90: 7661 6c75 6529 0a20 2020 2020 2020 2020  value).         
-00004ca0: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
-00004cb0: 656d 656e 7465 6445 7272 6f72 2827 5365  ementedError('Se
-00004cc0: 7269 616c 697a 6174 696f 6e20 6f66 207b  rialization of {
-00004cd0: 7d20 6861 7320 6e6f 7420 7965 7420 6265  } has not yet be
-00004ce0: 656e 2069 6d70 6c65 6d65 6e74 6564 272e  en implemented'.
-00004cf0: 666f 726d 6174 2863 6f6e 7465 6e74 5f74  format(content_t
-00004d00: 7970 6529 290a 0a0a 636c 6173 7320 5175  ype))...class Qu
-00004d10: 6572 7950 6172 616d 6574 6572 2850 6172  eryParameter(Par
-00004d20: 616d 6574 6572 4261 7365 2c20 5374 796c  ameterBase, Styl
-00004d30: 6546 6f72 6d53 6572 6961 6c69 7a65 7229  eFormSerializer)
-00004d40: 3a0a 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
-00004d50: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00004d60: 662c 0a20 2020 2020 2020 206e 616d 653a  f,.        name:
-00004d70: 2073 7472 2c0a 2020 2020 2020 2020 7265   str,.        re
-00004d80: 7175 6972 6564 3a20 626f 6f6c 203d 2046  quired: bool = F
-00004d90: 616c 7365 2c0a 2020 2020 2020 2020 7374  alse,.        st
-00004da0: 796c 653a 2074 7970 696e 672e 4f70 7469  yle: typing.Opti
-00004db0: 6f6e 616c 5b50 6172 616d 6574 6572 5374  onal[ParameterSt
-00004dc0: 796c 655d 203d 204e 6f6e 652c 0a20 2020  yle] = None,.   
-00004dd0: 2020 2020 2065 7870 6c6f 6465 3a20 7479       explode: ty
-00004de0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 626f  ping.Optional[bo
-00004df0: 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ol] = None,.    
-00004e00: 2020 2020 616c 6c6f 775f 7265 7365 7276      allow_reserv
-00004e10: 6564 3a20 7479 7069 6e67 2e4f 7074 696f  ed: typing.Optio
-00004e20: 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65  nal[bool] = None
-00004e30: 2c0a 2020 2020 2020 2020 7363 6865 6d61  ,.        schema
-00004e40: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00004e50: 6c5b 7479 7069 6e67 2e54 7970 655b 5363  l[typing.Type[Sc
-00004e60: 6865 6d61 5d5d 203d 204e 6f6e 652c 0a20  hema]] = None,. 
-00004e70: 2020 2020 2020 2063 6f6e 7465 6e74 3a20         content: 
-00004e80: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00004e90: 7479 7069 6e67 2e44 6963 745b 7374 722c  typing.Dict[str,
-00004ea0: 2074 7970 696e 672e 5479 7065 5b53 6368   typing.Type[Sch
-00004eb0: 656d 615d 5d5d 203d 204e 6f6e 650a 2020  ema]]] = None.  
-00004ec0: 2020 293a 0a20 2020 2020 2020 2075 7365    ):.        use
-00004ed0: 645f 7374 796c 6520 3d20 5061 7261 6d65  d_style = Parame
-00004ee0: 7465 7253 7479 6c65 2e46 4f52 4d20 6966  terStyle.FORM if
-00004ef0: 2073 7479 6c65 2069 7320 4e6f 6e65 2065   style is None e
-00004f00: 6c73 6520 7374 796c 650a 2020 2020 2020  lse style.      
-00004f10: 2020 7573 6564 5f65 7870 6c6f 6465 203d    used_explode =
-00004f20: 2073 656c 662e 5f67 6574 5f64 6566 6175   self._get_defau
-00004f30: 6c74 5f65 7870 6c6f 6465 2875 7365 645f  lt_explode(used_
-00004f40: 7374 796c 6529 2069 6620 6578 706c 6f64  style) if explod
-00004f50: 6520 6973 204e 6f6e 6520 656c 7365 2065  e is None else e
-00004f60: 7870 6c6f 6465 0a0a 2020 2020 2020 2020  xplode..        
-00004f70: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-00004f80: 280a 2020 2020 2020 2020 2020 2020 6e61  (.            na
-00004f90: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-00004fa0: 696e 5f74 7970 653d 5061 7261 6d65 7465  in_type=Paramete
-00004fb0: 7249 6e54 7970 652e 5155 4552 592c 0a20  rInType.QUERY,. 
-00004fc0: 2020 2020 2020 2020 2020 2072 6571 7569             requi
-00004fd0: 7265 643d 7265 7175 6972 6564 2c0a 2020  red=required,.  
-00004fe0: 2020 2020 2020 2020 2020 7374 796c 653d            style=
-00004ff0: 7573 6564 5f73 7479 6c65 2c0a 2020 2020  used_style,.    
-00005000: 2020 2020 2020 2020 6578 706c 6f64 653d          explode=
-00005010: 7573 6564 5f65 7870 6c6f 6465 2c0a 2020  used_explode,.  
-00005020: 2020 2020 2020 2020 2020 616c 6c6f 775f            allow_
-00005030: 7265 7365 7276 6564 3d61 6c6c 6f77 5f72  reserved=allow_r
-00005040: 6573 6572 7665 642c 0a20 2020 2020 2020  eserved,.       
-00005050: 2020 2020 2073 6368 656d 613d 7363 6865       schema=sche
-00005060: 6d61 2c0a 2020 2020 2020 2020 2020 2020  ma,.            
-00005070: 636f 6e74 656e 743d 636f 6e74 656e 740a  content=content.
-00005080: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00005090: 6566 205f 5f73 6572 6961 6c69 7a65 5f73  ef __serialize_s
-000050a0: 7061 6365 5f64 656c 696d 6974 6564 280a  pace_delimited(.
-000050b0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000050c0: 2020 2020 2020 696e 5f64 6174 613a 2074        in_data: t
-000050d0: 7970 696e 672e 556e 696f 6e5b 4e6f 6e65  yping.Union[None
-000050e0: 2c20 696e 742c 2066 6c6f 6174 2c20 7374  , int, float, st
-000050f0: 722c 2062 6f6f 6c2c 2064 6963 742c 206c  r, bool, dict, l
-00005100: 6973 745d 2c0a 2020 2020 2020 2020 7072  ist],.        pr
-00005110: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
-00005120: 7465 7261 746f 723a 2074 7970 696e 672e  terator: typing.
-00005130: 4f70 7469 6f6e 616c 5b50 7265 6669 7853  Optional[PrefixS
-00005140: 6570 6172 6174 6f72 4974 6572 6174 6f72  eparatorIterator
-00005150: 5d0a 2020 2020 2920 2d3e 2074 7970 696e  ].    ) -> typin
-00005160: 672e 4469 6374 5b73 7472 2c20 7374 725d  g.Dict[str, str]
-00005170: 3a0a 2020 2020 2020 2020 6966 2070 7265  :.        if pre
-00005180: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
-00005190: 6572 6174 6f72 2069 7320 4e6f 6e65 3a0a  erator is None:.
-000051a0: 2020 2020 2020 2020 2020 2020 7072 6566              pref
-000051b0: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
-000051c0: 7261 746f 7220 3d20 7365 6c66 2e67 6574  rator = self.get
-000051d0: 5f70 7265 6669 785f 7365 7061 7261 746f  _prefix_separato
-000051e0: 725f 6974 6572 6174 6f72 2829 0a20 2020  r_iterator().   
-000051f0: 2020 2020 2076 616c 7565 203d 2073 656c       value = sel
-00005200: 662e 5f72 6566 3635 3730 5f65 7870 616e  f._ref6570_expan
-00005210: 7369 6f6e 280a 2020 2020 2020 2020 2020  sion(.          
-00005220: 2020 7661 7269 6162 6c65 5f6e 616d 653d    variable_name=
-00005230: 7365 6c66 2e6e 616d 652c 0a20 2020 2020  self.name,.     
-00005240: 2020 2020 2020 2069 6e5f 6461 7461 3d69         in_data=i
-00005250: 6e5f 6461 7461 2c0a 2020 2020 2020 2020  n_data,.        
-00005260: 2020 2020 6578 706c 6f64 653d 7365 6c66      explode=self
-00005270: 2e65 7870 6c6f 6465 2c0a 2020 2020 2020  .explode,.      
-00005280: 2020 2020 2020 7065 7263 656e 745f 656e        percent_en
-00005290: 636f 6465 3d54 7275 652c 0a20 2020 2020  code=True,.     
-000052a0: 2020 2020 2020 2070 7265 6669 785f 7365         prefix_se
-000052b0: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
-000052c0: 3d70 7265 6669 785f 7365 7061 7261 746f  =prefix_separato
-000052d0: 725f 6974 6572 6174 6f72 0a20 2020 2020  r_iterator.     
-000052e0: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
-000052f0: 7572 6e20 7365 6c66 2e5f 746f 5f64 6963  urn self._to_dic
-00005300: 7428 7365 6c66 2e6e 616d 652c 2076 616c  t(self.name, val
-00005310: 7565 290a 0a20 2020 2064 6566 205f 5f73  ue)..    def __s
-00005320: 6572 6961 6c69 7a65 5f70 6970 655f 6465  erialize_pipe_de
-00005330: 6c69 6d69 7465 6428 0a20 2020 2020 2020  limited(.       
-00005340: 2073 656c 662c 0a20 2020 2020 2020 2069   self,.        i
-00005350: 6e5f 6461 7461 3a20 7479 7069 6e67 2e55  n_data: typing.U
-00005360: 6e69 6f6e 5b4e 6f6e 652c 2069 6e74 2c20  nion[None, int, 
-00005370: 666c 6f61 742c 2073 7472 2c20 626f 6f6c  float, str, bool
-00005380: 2c20 6469 6374 2c20 6c69 7374 5d2c 0a20  , dict, list],. 
-00005390: 2020 2020 2020 2070 7265 6669 785f 7365         prefix_se
-000053a0: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
-000053b0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-000053c0: 6c5b 5072 6566 6978 5365 7061 7261 746f  l[PrefixSeparato
-000053d0: 7249 7465 7261 746f 725d 0a20 2020 2029  rIterator].    )
-000053e0: 202d 3e20 7479 7069 6e67 2e44 6963 745b   -> typing.Dict[
-000053f0: 7374 722c 2073 7472 5d3a 0a20 2020 2020  str, str]:.     
-00005400: 2020 2069 6620 7072 6566 6978 5f73 6570     if prefix_sep
-00005410: 6172 6174 6f72 5f69 7465 7261 746f 7220  arator_iterator 
-00005420: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00005430: 2020 2020 2070 7265 6669 785f 7365 7061       prefix_sepa
-00005440: 7261 746f 725f 6974 6572 6174 6f72 203d  rator_iterator =
-00005450: 2073 656c 662e 6765 745f 7072 6566 6978   self.get_prefix
-00005460: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-00005470: 746f 7228 290a 2020 2020 2020 2020 7661  tor().        va
-00005480: 6c75 6520 3d20 7365 6c66 2e5f 7265 6636  lue = self._ref6
-00005490: 3537 305f 6578 7061 6e73 696f 6e28 0a20  570_expansion(. 
-000054a0: 2020 2020 2020 2020 2020 2076 6172 6961             varia
-000054b0: 626c 655f 6e61 6d65 3d73 656c 662e 6e61  ble_name=self.na
-000054c0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-000054d0: 696e 5f64 6174 613d 696e 5f64 6174 612c  in_data=in_data,
-000054e0: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
-000054f0: 6c6f 6465 3d73 656c 662e 6578 706c 6f64  lode=self.explod
-00005500: 652c 0a20 2020 2020 2020 2020 2020 2070  e,.            p
-00005510: 6572 6365 6e74 5f65 6e63 6f64 653d 5472  ercent_encode=Tr
-00005520: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00005530: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
-00005540: 5f69 7465 7261 746f 723d 7072 6566 6978  _iterator=prefix
-00005550: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-00005560: 746f 720a 2020 2020 2020 2020 290a 2020  tor.        ).  
-00005570: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00005580: 662e 5f74 6f5f 6469 6374 2873 656c 662e  f._to_dict(self.
-00005590: 6e61 6d65 2c20 7661 6c75 6529 0a0a 2020  name, value)..  
-000055a0: 2020 6465 6620 5f5f 7365 7269 616c 697a    def __serializ
-000055b0: 655f 666f 726d 280a 2020 2020 2020 2020  e_form(.        
-000055c0: 7365 6c66 2c0a 2020 2020 2020 2020 696e  self,.        in
-000055d0: 5f64 6174 613a 2074 7970 696e 672e 556e  _data: typing.Un
-000055e0: 696f 6e5b 4e6f 6e65 2c20 696e 742c 2066  ion[None, int, f
-000055f0: 6c6f 6174 2c20 7374 722c 2062 6f6f 6c2c  loat, str, bool,
-00005600: 2064 6963 742c 206c 6973 745d 2c0a 2020   dict, list],.  
-00005610: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
-00005620: 6172 6174 6f72 5f69 7465 7261 746f 723a  arator_iterator:
-00005630: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00005640: 5b50 7265 6669 7853 6570 6172 6174 6f72  [PrefixSeparator
-00005650: 4974 6572 6174 6f72 5d0a 2020 2020 2920  Iterator].    ) 
-00005660: 2d3e 2074 7970 696e 672e 4469 6374 5b73  -> typing.Dict[s
-00005670: 7472 2c20 7374 725d 3a0a 2020 2020 2020  tr, str]:.      
-00005680: 2020 6966 2070 7265 6669 785f 7365 7061    if prefix_sepa
-00005690: 7261 746f 725f 6974 6572 6174 6f72 2069  rator_iterator i
-000056a0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-000056b0: 2020 2020 7072 6566 6978 5f73 6570 6172      prefix_separ
-000056c0: 6174 6f72 5f69 7465 7261 746f 7220 3d20  ator_iterator = 
-000056d0: 7365 6c66 2e67 6574 5f70 7265 6669 785f  self.get_prefix_
-000056e0: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
-000056f0: 6f72 2829 0a20 2020 2020 2020 2076 616c  or().        val
-00005700: 7565 203d 2073 656c 662e 5f73 6572 6961  ue = self._seria
-00005710: 6c69 7a65 5f66 6f72 6d28 0a20 2020 2020  lize_form(.     
-00005720: 2020 2020 2020 2069 6e5f 6461 7461 2c0a         in_data,.
-00005730: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00005740: 3d73 656c 662e 6e61 6d65 2c0a 2020 2020  =self.name,.    
-00005750: 2020 2020 2020 2020 6578 706c 6f64 653d          explode=
-00005760: 7365 6c66 2e65 7870 6c6f 6465 2c0a 2020  self.explode,.  
-00005770: 2020 2020 2020 2020 2020 7065 7263 656e            percen
-00005780: 745f 656e 636f 6465 3d54 7275 652c 0a20  t_encode=True,. 
-00005790: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
-000057a0: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-000057b0: 6174 6f72 3d70 7265 6669 785f 7365 7061  ator=prefix_sepa
-000057c0: 7261 746f 725f 6974 6572 6174 6f72 0a20  rator_iterator. 
-000057d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000057e0: 2072 6574 7572 6e20 7365 6c66 2e5f 746f   return self._to
-000057f0: 5f64 6963 7428 7365 6c66 2e6e 616d 652c  _dict(self.name,
-00005800: 2076 616c 7565 290a 0a20 2020 2064 6566   value)..    def
-00005810: 2067 6574 5f70 7265 6669 785f 7365 7061   get_prefix_sepa
-00005820: 7261 746f 725f 6974 6572 6174 6f72 2873  rator_iterator(s
-00005830: 656c 6629 202d 3e20 7479 7069 6e67 2e4f  elf) -> typing.O
-00005840: 7074 696f 6e61 6c5b 5072 6566 6978 5365  ptional[PrefixSe
-00005850: 7061 7261 746f 7249 7465 7261 746f 725d  paratorIterator]
-00005860: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00005870: 662e 7374 796c 6520 6973 2050 6172 616d  f.style is Param
-00005880: 6574 6572 5374 796c 652e 464f 524d 3a0a  eterStyle.FORM:.
-00005890: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000058a0: 726e 2050 7265 6669 7853 6570 6172 6174  rn PrefixSeparat
-000058b0: 6f72 4974 6572 6174 6f72 2827 3f27 2c20  orIterator('?', 
-000058c0: 2726 2729 0a20 2020 2020 2020 2065 6c69  '&').        eli
-000058d0: 6620 7365 6c66 2e73 7479 6c65 2069 7320  f self.style is 
-000058e0: 5061 7261 6d65 7465 7253 7479 6c65 2e53  ParameterStyle.S
-000058f0: 5041 4345 5f44 454c 494d 4954 4544 3a0a  PACE_DELIMITED:.
-00005900: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00005910: 726e 2050 7265 6669 7853 6570 6172 6174  rn PrefixSeparat
-00005920: 6f72 4974 6572 6174 6f72 2827 272c 2027  orIterator('', '
-00005930: 2532 3027 290a 2020 2020 2020 2020 656c  %20').        el
-00005940: 6966 2073 656c 662e 7374 796c 6520 6973  if self.style is
-00005950: 2050 6172 616d 6574 6572 5374 796c 652e   ParameterStyle.
-00005960: 5049 5045 5f44 454c 494d 4954 4544 3a0a  PIPE_DELIMITED:.
-00005970: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00005980: 726e 2050 7265 6669 7853 6570 6172 6174  rn PrefixSeparat
-00005990: 6f72 4974 6572 6174 6f72 2827 272c 2027  orIterator('', '
-000059a0: 7c27 290a 0a20 2020 2064 6566 2073 6572  |')..    def ser
-000059b0: 6961 6c69 7a65 280a 2020 2020 2020 2020  ialize(.        
-000059c0: 7365 6c66 2c0a 2020 2020 2020 2020 696e  self,.        in
-000059d0: 5f64 6174 613a 2074 7970 696e 672e 556e  _data: typing.Un
-000059e0: 696f 6e5b 0a20 2020 2020 2020 2020 2020  ion[.           
-000059f0: 2053 6368 656d 612c 2044 6563 696d 616c   Schema, Decimal
-00005a00: 2c20 696e 742c 2066 6c6f 6174 2c20 7374  , int, float, st
-00005a10: 722c 2064 6174 652c 2064 6174 6574 696d  r, date, datetim
-00005a20: 652c 204e 6f6e 652c 2062 6f6f 6c2c 206c  e, None, bool, l
-00005a30: 6973 742c 2074 7570 6c65 2c20 6469 6374  ist, tuple, dict
-00005a40: 2c20 6672 6f7a 656e 6469 6374 2e66 726f  , frozendict.fro
-00005a50: 7a65 6e64 6963 745d 2c0a 2020 2020 2020  zendict],.      
-00005a60: 2020 7072 6566 6978 5f73 6570 6172 6174    prefix_separat
-00005a70: 6f72 5f69 7465 7261 746f 723a 2074 7970  or_iterator: typ
-00005a80: 696e 672e 4f70 7469 6f6e 616c 5b50 7265  ing.Optional[Pre
-00005a90: 6669 7853 6570 6172 6174 6f72 4974 6572  fixSeparatorIter
-00005aa0: 6174 6f72 5d20 3d20 4e6f 6e65 0a20 2020  ator] = None.   
-00005ab0: 2029 202d 3e20 7479 7069 6e67 2e44 6963   ) -> typing.Dic
-00005ac0: 745b 7374 722c 2073 7472 5d3a 0a20 2020  t[str, str]:.   
-00005ad0: 2020 2020 2069 6620 7365 6c66 2e73 6368       if self.sch
-00005ae0: 656d 613a 0a20 2020 2020 2020 2020 2020  ema:.           
-00005af0: 2063 6173 745f 696e 5f64 6174 6120 3d20   cast_in_data = 
-00005b00: 7365 6c66 2e73 6368 656d 6128 696e 5f64  self.schema(in_d
-00005b10: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
-00005b20: 2063 6173 745f 696e 5f64 6174 6120 3d20   cast_in_data = 
-00005b30: 7365 6c66 2e5f 6a73 6f6e 5f65 6e63 6f64  self._json_encod
-00005b40: 6572 2e64 6566 6175 6c74 2863 6173 745f  er.default(cast_
-00005b50: 696e 5f64 6174 6129 0a20 2020 2020 2020  in_data).       
-00005b60: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00005b70: 2020 2020 2066 6f72 6d20 2d3e 2071 7565       form -> que
-00005b80: 7279 0a20 2020 2020 2020 2020 2020 2020  ry.             
-00005b90: 2020 2071 7565 7279 3a0a 2020 2020 2020     query:.      
-00005ba0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00005bb0: 4745 542f 4845 4144 2f44 454c 4554 453a  GET/HEAD/DELETE:
-00005bc0: 2063 6f75 6c64 2075 7365 2066 6965 6c64   could use field
-00005bd0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00005be0: 2020 2020 2020 2d20 5055 542f 504f 5354        - PUT/POST
-00005bf0: 3a20 6d75 7374 2075 7365 2075 726c 656e  : must use urlen
-00005c00: 636f 6465 2074 6f20 7365 6e64 2070 6172  code to send par
-00005c10: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00005c20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00005c30: 726e 7320 6669 656c 6473 3a20 7475 706c  rns fields: tupl
-00005c40: 650a 2020 2020 2020 2020 2020 2020 7370  e.            sp
-00005c50: 6163 6544 656c 696d 6974 6564 202d 3e20  aceDelimited -> 
-00005c60: 7175 6572 790a 2020 2020 2020 2020 2020  query.          
-00005c70: 2020 2020 2020 7265 7475 726e 7320 6669        returns fi
-00005c80: 656c 6473 0a20 2020 2020 2020 2020 2020  elds.           
-00005c90: 2070 6970 6544 656c 696d 6974 6564 202d   pipeDelimited -
-00005ca0: 3e20 7175 6572 790a 2020 2020 2020 2020  > query.        
-00005cb0: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
-00005cc0: 6669 656c 6473 0a20 2020 2020 2020 2020  fields.         
-00005cd0: 2020 2064 6565 704f 626a 6563 7420 2d3e     deepObject ->
-00005ce0: 2071 7565 7279 2c20 6874 7470 733a 2f2f   query, https://
-00005cf0: 6769 7468 7562 2e63 6f6d 2f4f 4149 2f4f  github.com/OAI/O
-00005d00: 7065 6e41 5049 2d53 7065 6369 6669 6361  penAPI-Specifica
-00005d10: 7469 6f6e 2f69 7373 7565 732f 3137 3036  tion/issues/1706
-00005d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005d30: 2072 6574 7572 6e73 2066 6965 6c64 730a   returns fields.
-00005d40: 2020 2020 2020 2020 2020 2020 2222 220a              """.
-00005d50: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00005d60: 656c 662e 7374 796c 653a 0a20 2020 2020  elf.style:.     
-00005d70: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
-00005d80: 4f20 7570 6461 7465 2071 7565 7279 206f  O update query o
-00005d90: 6e65 7320 746f 206f 6d69 7420 7365 7474  nes to omit sett
-00005da0: 696e 6720 7661 6c75 6573 2077 6865 6e20  ing values when 
-00005db0: 5b5d 207b 7d20 6f72 204e 6f6e 6520 6973  [] {} or None is
-00005dc0: 2069 6e70 7574 0a20 2020 2020 2020 2020   input.         
-00005dd0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00005de0: 7479 6c65 2069 7320 5061 7261 6d65 7465  tyle is Paramete
-00005df0: 7253 7479 6c65 2e46 4f52 4d3a 0a20 2020  rStyle.FORM:.   
-00005e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e10: 2072 6574 7572 6e20 7365 6c66 2e5f 5f73   return self.__s
-00005e20: 6572 6961 6c69 7a65 5f66 6f72 6d28 6361  erialize_form(ca
-00005e30: 7374 5f69 6e5f 6461 7461 2c20 7072 6566  st_in_data, pref
-00005e40: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
-00005e50: 7261 746f 7229 0a20 2020 2020 2020 2020  rator).         
-00005e60: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-00005e70: 2e73 7479 6c65 2069 7320 5061 7261 6d65  .style is Parame
-00005e80: 7465 7253 7479 6c65 2e53 5041 4345 5f44  terStyle.SPACE_D
-00005e90: 454c 494d 4954 4544 3a0a 2020 2020 2020  ELIMITED:.      
-00005ea0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00005eb0: 7475 726e 2073 656c 662e 5f5f 7365 7269  turn self.__seri
-00005ec0: 616c 697a 655f 7370 6163 655f 6465 6c69  alize_space_deli
-00005ed0: 6d69 7465 6428 6361 7374 5f69 6e5f 6461  mited(cast_in_da
-00005ee0: 7461 2c20 7072 6566 6978 5f73 6570 6172  ta, prefix_separ
-00005ef0: 6174 6f72 5f69 7465 7261 746f 7229 0a20  ator_iterator). 
-00005f00: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00005f10: 6c69 6620 7365 6c66 2e73 7479 6c65 2069  lif self.style i
-00005f20: 7320 5061 7261 6d65 7465 7253 7479 6c65  s ParameterStyle
-00005f30: 2e50 4950 455f 4445 4c49 4d49 5445 443a  .PIPE_DELIMITED:
-00005f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005f50: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00005f60: 2e5f 5f73 6572 6961 6c69 7a65 5f70 6970  .__serialize_pip
-00005f70: 655f 6465 6c69 6d69 7465 6428 6361 7374  e_delimited(cast
-00005f80: 5f69 6e5f 6461 7461 2c20 7072 6566 6978  _in_data, prefix
-00005f90: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-00005fa0: 746f 7229 0a20 2020 2020 2020 2023 2073  tor).        # s
-00005fb0: 656c 662e 636f 6e74 656e 7420 7769 6c6c  elf.content will
-00005fc0: 2062 6520 6c65 6e67 7468 206f 6e65 0a20   be length one. 
-00005fd0: 2020 2020 2020 2069 6620 7072 6566 6978         if prefix
-00005fe0: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-00005ff0: 746f 7220 6973 204e 6f6e 653a 0a20 2020  tor is None:.   
-00006000: 2020 2020 2020 2020 2070 7265 6669 785f           prefix_
-00006010: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
-00006020: 6f72 203d 2073 656c 662e 6765 745f 7072  or = self.get_pr
-00006030: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
-00006040: 7465 7261 746f 7228 290a 2020 2020 2020  terator().      
-00006050: 2020 666f 7220 636f 6e74 656e 745f 7479    for content_ty
-00006060: 7065 2c20 7363 6865 6d61 2069 6e20 7365  pe, schema in se
-00006070: 6c66 2e63 6f6e 7465 6e74 2e69 7465 6d73  lf.content.items
-00006080: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00006090: 6361 7374 5f69 6e5f 6461 7461 203d 2073  cast_in_data = s
-000060a0: 6368 656d 6128 696e 5f64 6174 6129 0a20  chema(in_data). 
-000060b0: 2020 2020 2020 2020 2020 2063 6173 745f             cast_
-000060c0: 696e 5f64 6174 6120 3d20 7365 6c66 2e5f  in_data = self._
-000060d0: 6a73 6f6e 5f65 6e63 6f64 6572 2e64 6566  json_encoder.def
-000060e0: 6175 6c74 2863 6173 745f 696e 5f64 6174  ault(cast_in_dat
-000060f0: 6129 0a20 2020 2020 2020 2020 2020 2069  a).            i
-00006100: 6620 7365 6c66 2e5f 636f 6e74 656e 745f  f self._content_
-00006110: 7479 7065 5f69 735f 6a73 6f6e 2863 6f6e  type_is_json(con
-00006120: 7465 6e74 5f74 7970 6529 3a0a 2020 2020  tent_type):.    
-00006130: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-00006140: 6520 3d20 7365 6c66 2e5f 7365 7269 616c  e = self._serial
-00006150: 697a 655f 6a73 6f6e 2863 6173 745f 696e  ize_json(cast_in
-00006160: 5f64 6174 612c 2065 6c69 6d69 6e61 7465  _data, eliminate
-00006170: 5f77 6869 7465 7370 6163 653d 5472 7565  _whitespace=True
-00006180: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00006190: 2020 7265 7475 726e 2073 656c 662e 5f74    return self._t
-000061a0: 6f5f 6469 6374 280a 2020 2020 2020 2020  o_dict(.        
-000061b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000061c0: 2e6e 616d 652c 0a20 2020 2020 2020 2020  .name,.         
-000061d0: 2020 2020 2020 2020 2020 206e 6578 7428             next(
-000061e0: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
-000061f0: 5f69 7465 7261 746f 7229 202b 2073 656c  _iterator) + sel
-00006200: 662e 6e61 6d65 202b 2027 3d27 202b 2071  f.name + '=' + q
-00006210: 756f 7465 2876 616c 7565 290a 2020 2020  uote(value).    
-00006220: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00006230: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00006240: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-00006250: 726f 7228 2753 6572 6961 6c69 7a61 7469  ror('Serializati
-00006260: 6f6e 206f 6620 7b7d 2068 6173 206e 6f74  on of {} has not
-00006270: 2079 6574 2062 6565 6e20 696d 706c 656d   yet been implem
-00006280: 656e 7465 6427 2e66 6f72 6d61 7428 636f  ented'.format(co
-00006290: 6e74 656e 745f 7479 7065 2929 0a0a 0a63  ntent_type))...c
-000062a0: 6c61 7373 2043 6f6f 6b69 6550 6172 616d  lass CookieParam
-000062b0: 6574 6572 2850 6172 616d 6574 6572 4261  eter(ParameterBa
-000062c0: 7365 2c20 5374 796c 6546 6f72 6d53 6572  se, StyleFormSer
-000062d0: 6961 6c69 7a65 7229 3a0a 0a20 2020 2064  ializer):..    d
-000062e0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-000062f0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00006300: 2020 206e 616d 653a 2073 7472 2c0a 2020     name: str,.  
-00006310: 2020 2020 2020 7265 7175 6972 6564 3a20        required: 
-00006320: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-00006330: 2020 2020 2020 7374 796c 653a 2074 7970        style: typ
-00006340: 696e 672e 4f70 7469 6f6e 616c 5b50 6172  ing.Optional[Par
-00006350: 616d 6574 6572 5374 796c 655d 203d 204e  ameterStyle] = N
-00006360: 6f6e 652c 0a20 2020 2020 2020 2065 7870  one,.        exp
-00006370: 6c6f 6465 3a20 7479 7069 6e67 2e4f 7074  lode: typing.Opt
-00006380: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
-00006390: 6e65 2c0a 2020 2020 2020 2020 616c 6c6f  ne,.        allo
-000063a0: 775f 7265 7365 7276 6564 3a20 7479 7069  w_reserved: typi
-000063b0: 6e67 2e4f 7074 696f 6e61 6c5b 626f 6f6c  ng.Optional[bool
-000063c0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-000063d0: 2020 7363 6865 6d61 3a20 7479 7069 6e67    schema: typing
-000063e0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-000063f0: 2e54 7970 655b 5363 6865 6d61 5d5d 203d  .Type[Schema]] =
-00006400: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
-00006410: 6f6e 7465 6e74 3a20 7479 7069 6e67 2e4f  ontent: typing.O
-00006420: 7074 696f 6e61 6c5b 7479 7069 6e67 2e44  ptional[typing.D
-00006430: 6963 745b 7374 722c 2074 7970 696e 672e  ict[str, typing.
-00006440: 5479 7065 5b53 6368 656d 615d 5d5d 203d  Type[Schema]]] =
-00006450: 204e 6f6e 650a 2020 2020 293a 0a20 2020   None.    ):.   
-00006460: 2020 2020 2075 7365 645f 7374 796c 6520       used_style 
-00006470: 3d20 5061 7261 6d65 7465 7253 7479 6c65  = ParameterStyle
-00006480: 2e46 4f52 4d20 6966 2073 7479 6c65 2069  .FORM if style i
-00006490: 7320 4e6f 6e65 2061 6e64 2063 6f6e 7465  s None and conte
-000064a0: 6e74 2069 7320 4e6f 6e65 2061 6e64 2073  nt is None and s
-000064b0: 6368 656d 6120 656c 7365 2073 7479 6c65  chema else style
-000064c0: 0a20 2020 2020 2020 2075 7365 645f 6578  .        used_ex
-000064d0: 706c 6f64 6520 3d20 7365 6c66 2e5f 6765  plode = self._ge
-000064e0: 745f 6465 6661 756c 745f 6578 706c 6f64  t_default_explod
-000064f0: 6528 7573 6564 5f73 7479 6c65 2920 6966  e(used_style) if
-00006500: 2065 7870 6c6f 6465 2069 7320 4e6f 6e65   explode is None
-00006510: 2065 6c73 6520 6578 706c 6f64 650a 0a20   else explode.. 
-00006520: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
-00006530: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00006540: 2020 2020 206e 616d 652c 0a20 2020 2020       name,.     
-00006550: 2020 2020 2020 2069 6e5f 7479 7065 3d50         in_type=P
-00006560: 6172 616d 6574 6572 496e 5479 7065 2e43  arameterInType.C
-00006570: 4f4f 4b49 452c 0a20 2020 2020 2020 2020  OOKIE,.         
-00006580: 2020 2072 6571 7569 7265 643d 7265 7175     required=requ
-00006590: 6972 6564 2c0a 2020 2020 2020 2020 2020  ired,.          
-000065a0: 2020 7374 796c 653d 7573 6564 5f73 7479    style=used_sty
-000065b0: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
-000065c0: 6578 706c 6f64 653d 7573 6564 5f65 7870  explode=used_exp
-000065d0: 6c6f 6465 2c0a 2020 2020 2020 2020 2020  lode,.          
-000065e0: 2020 616c 6c6f 775f 7265 7365 7276 6564    allow_reserved
-000065f0: 3d61 6c6c 6f77 5f72 6573 6572 7665 642c  =allow_reserved,
-00006600: 0a20 2020 2020 2020 2020 2020 2073 6368  .            sch
-00006610: 656d 613d 7363 6865 6d61 2c0a 2020 2020  ema=schema,.    
-00006620: 2020 2020 2020 2020 636f 6e74 656e 743d          content=
-00006630: 636f 6e74 656e 740a 2020 2020 2020 2020  content.        
-00006640: 290a 0a20 2020 2064 6566 2073 6572 6961  )..    def seria
-00006650: 6c69 7a65 280a 2020 2020 2020 2020 7365  lize(.        se
-00006660: 6c66 2c0a 2020 2020 2020 2020 696e 5f64  lf,.        in_d
-00006670: 6174 613a 2074 7970 696e 672e 556e 696f  ata: typing.Unio
-00006680: 6e5b 0a20 2020 2020 2020 2020 2020 2053  n[.            S
-00006690: 6368 656d 612c 2044 6563 696d 616c 2c20  chema, Decimal, 
-000066a0: 696e 742c 2066 6c6f 6174 2c20 7374 722c  int, float, str,
-000066b0: 2064 6174 652c 2064 6174 6574 696d 652c   date, datetime,
-000066c0: 204e 6f6e 652c 2062 6f6f 6c2c 206c 6973   None, bool, lis
-000066d0: 742c 2074 7570 6c65 2c20 6469 6374 2c20  t, tuple, dict, 
-000066e0: 6672 6f7a 656e 6469 6374 2e66 726f 7a65  frozendict.froze
-000066f0: 6e64 6963 745d 0a20 2020 2029 202d 3e20  ndict].    ) -> 
-00006700: 7479 7069 6e67 2e44 6963 745b 7374 722c  typing.Dict[str,
-00006710: 2073 7472 5d3a 0a20 2020 2020 2020 2069   str]:.        i
-00006720: 6620 7365 6c66 2e73 6368 656d 613a 0a20  f self.schema:. 
-00006730: 2020 2020 2020 2020 2020 2063 6173 745f             cast_
-00006740: 696e 5f64 6174 6120 3d20 7365 6c66 2e73  in_data = self.s
-00006750: 6368 656d 6128 696e 5f64 6174 6129 0a20  chema(in_data). 
-00006760: 2020 2020 2020 2020 2020 2063 6173 745f             cast_
-00006770: 696e 5f64 6174 6120 3d20 7365 6c66 2e5f  in_data = self._
-00006780: 6a73 6f6e 5f65 6e63 6f64 6572 2e64 6566  json_encoder.def
-00006790: 6175 6c74 2863 6173 745f 696e 5f64 6174  ault(cast_in_dat
-000067a0: 6129 0a20 2020 2020 2020 2020 2020 2022  a).            "
-000067b0: 2222 0a20 2020 2020 2020 2020 2020 2066  "".            f
-000067c0: 6f72 6d20 2d3e 2063 6f6f 6b69 650a 2020  orm -> cookie.  
-000067d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000067e0: 7475 726e 7320 6669 656c 6473 3a20 7475  turns fields: tu
-000067f0: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
-00006800: 2222 220a 2020 2020 2020 2020 2020 2020  """.            
-00006810: 6966 2073 656c 662e 7374 796c 653a 0a20  if self.style:. 
-00006820: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006830: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
-00006840: 2020 2054 4f44 4f20 6164 6420 6573 6361     TODO add esca
-00006850: 7069 6e67 206f 6620 636f 6d6d 612c 2073  ping of comma, s
-00006860: 7061 6365 2c20 6571 7561 6c73 0a20 2020  pace, equals.   
-00006870: 2020 2020 2020 2020 2020 2020 206f 7220               or 
-00006880: 7475 726e 2065 6e63 6f64 696e 6720 6f6e  turn encoding on
-00006890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000068a0: 2022 2222 0a20 2020 2020 2020 2020 2020   """.           
-000068b0: 2020 2020 2076 616c 7565 203d 2073 656c       value = sel
-000068c0: 662e 5f73 6572 6961 6c69 7a65 5f66 6f72  f._serialize_for
-000068d0: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
-000068e0: 2020 2020 2020 2063 6173 745f 696e 5f64         cast_in_d
-000068f0: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-00006900: 2020 2020 2020 2020 2065 7870 6c6f 6465           explode
-00006910: 3d73 656c 662e 6578 706c 6f64 652c 0a20  =self.explode,. 
-00006920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006930: 2020 206e 616d 653d 7365 6c66 2e6e 616d     name=self.nam
-00006940: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00006950: 2020 2020 2020 2070 6572 6365 6e74 5f65         percent_e
-00006960: 6e63 6f64 653d 4661 6c73 652c 0a20 2020  ncode=False,.   
-00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006980: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
-00006990: 725f 6974 6572 6174 6f72 3d50 7265 6669  r_iterator=Prefi
-000069a0: 7853 6570 6172 6174 6f72 4974 6572 6174  xSeparatorIterat
-000069b0: 6f72 2827 272c 2027 2627 290a 2020 2020  or('', '&').    
-000069c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000069d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000069e0: 7475 726e 2073 656c 662e 5f74 6f5f 6469  turn self._to_di
-000069f0: 6374 2873 656c 662e 6e61 6d65 2c20 7661  ct(self.name, va
-00006a00: 6c75 6529 0a20 2020 2020 2020 2023 2073  lue).        # s
-00006a10: 656c 662e 636f 6e74 656e 7420 7769 6c6c  elf.content will
-00006a20: 2062 6520 6c65 6e67 7468 206f 6e65 0a20   be length one. 
-00006a30: 2020 2020 2020 2066 6f72 2063 6f6e 7465         for conte
-00006a40: 6e74 5f74 7970 652c 2073 6368 656d 6120  nt_type, schema 
-00006a50: 696e 2073 656c 662e 636f 6e74 656e 742e  in self.content.
-00006a60: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
-00006a70: 2020 2020 2063 6173 745f 696e 5f64 6174       cast_in_dat
-00006a80: 6120 3d20 7363 6865 6d61 2869 6e5f 6461  a = schema(in_da
-00006a90: 7461 290a 2020 2020 2020 2020 2020 2020  ta).            
-00006aa0: 6361 7374 5f69 6e5f 6461 7461 203d 2073  cast_in_data = s
-00006ab0: 656c 662e 5f6a 736f 6e5f 656e 636f 6465  elf._json_encode
-00006ac0: 722e 6465 6661 756c 7428 6361 7374 5f69  r.default(cast_i
-00006ad0: 6e5f 6461 7461 290a 2020 2020 2020 2020  n_data).        
-00006ae0: 2020 2020 6966 2073 656c 662e 5f63 6f6e      if self._con
-00006af0: 7465 6e74 5f74 7970 655f 6973 5f6a 736f  tent_type_is_jso
-00006b00: 6e28 636f 6e74 656e 745f 7479 7065 293a  n(content_type):
-00006b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006b20: 2076 616c 7565 203d 2073 656c 662e 5f73   value = self._s
-00006b30: 6572 6961 6c69 7a65 5f6a 736f 6e28 6361  erialize_json(ca
-00006b40: 7374 5f69 6e5f 6461 7461 290a 2020 2020  st_in_data).    
-00006b50: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00006b60: 726e 2073 656c 662e 5f74 6f5f 6469 6374  rn self._to_dict
-00006b70: 2873 656c 662e 6e61 6d65 2c20 7661 6c75  (self.name, valu
-00006b80: 6529 0a20 2020 2020 2020 2020 2020 2072  e).            r
-00006b90: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
-00006ba0: 7465 6445 7272 6f72 2827 5365 7269 616c  tedError('Serial
-00006bb0: 697a 6174 696f 6e20 6f66 207b 7d20 6861  ization of {} ha
-00006bc0: 7320 6e6f 7420 7965 7420 6265 656e 2069  s not yet been i
-00006bd0: 6d70 6c65 6d65 6e74 6564 272e 666f 726d  mplemented'.form
-00006be0: 6174 2863 6f6e 7465 6e74 5f74 7970 6529  at(content_type)
-00006bf0: 290a 0a0a 636c 6173 7320 4865 6164 6572  )...class Header
-00006c00: 5061 7261 6d65 7465 7228 5061 7261 6d65  Parameter(Parame
-00006c10: 7465 7242 6173 652c 2053 7479 6c65 5369  terBase, StyleSi
-00006c20: 6d70 6c65 5365 7269 616c 697a 6572 293a  mpleSerializer):
-00006c30: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00006c40: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00006c50: 0a20 2020 2020 2020 206e 616d 653a 2073  .        name: s
-00006c60: 7472 2c0a 2020 2020 2020 2020 7265 7175  tr,.        requ
-00006c70: 6972 6564 3a20 626f 6f6c 203d 2046 616c  ired: bool = Fal
-00006c80: 7365 2c0a 2020 2020 2020 2020 7374 796c  se,.        styl
-00006c90: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
-00006ca0: 616c 5b50 6172 616d 6574 6572 5374 796c  al[ParameterStyl
-00006cb0: 655d 203d 204e 6f6e 652c 0a20 2020 2020  e] = None,.     
-00006cc0: 2020 2065 7870 6c6f 6465 3a20 626f 6f6c     explode: bool
-00006cd0: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-00006ce0: 2020 616c 6c6f 775f 7265 7365 7276 6564    allow_reserved
-00006cf0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00006d00: 6c5b 626f 6f6c 5d20 3d20 4e6f 6e65 2c0a  l[bool] = None,.
-00006d10: 2020 2020 2020 2020 7363 6865 6d61 3a20          schema: 
-00006d20: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00006d30: 7479 7069 6e67 2e54 7970 655b 5363 6865  typing.Type[Sche
-00006d40: 6d61 5d5d 203d 204e 6f6e 652c 0a20 2020  ma]] = None,.   
-00006d50: 2020 2020 2063 6f6e 7465 6e74 3a20 7479       content: ty
-00006d60: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-00006d70: 7069 6e67 2e44 6963 745b 7374 722c 2074  ping.Dict[str, t
-00006d80: 7970 696e 672e 5479 7065 5b53 6368 656d  yping.Type[Schem
-00006d90: 615d 5d5d 203d 204e 6f6e 650a 2020 2020  a]]] = None.    
-00006da0: 293a 0a20 2020 2020 2020 2073 7570 6572  ):.        super
-00006db0: 2829 2e5f 5f69 6e69 745f 5f28 0a20 2020  ().__init__(.   
-00006dc0: 2020 2020 2020 2020 206e 616d 652c 0a20           name,. 
-00006dd0: 2020 2020 2020 2020 2020 2069 6e5f 7479             in_ty
-00006de0: 7065 3d50 6172 616d 6574 6572 496e 5479  pe=ParameterInTy
-00006df0: 7065 2e48 4541 4445 522c 0a20 2020 2020  pe.HEADER,.     
-00006e00: 2020 2020 2020 2072 6571 7569 7265 643d         required=
-00006e10: 7265 7175 6972 6564 2c0a 2020 2020 2020  required,.      
-00006e20: 2020 2020 2020 7374 796c 653d 7374 796c        style=styl
-00006e30: 652c 0a20 2020 2020 2020 2020 2020 2065  e,.            e
-00006e40: 7870 6c6f 6465 3d65 7870 6c6f 6465 2c0a  xplode=explode,.
-00006e50: 2020 2020 2020 2020 2020 2020 616c 6c6f              allo
-00006e60: 775f 7265 7365 7276 6564 3d61 6c6c 6f77  w_reserved=allow
-00006e70: 5f72 6573 6572 7665 642c 0a20 2020 2020  _reserved,.     
-00006e80: 2020 2020 2020 2073 6368 656d 613d 7363         schema=sc
-00006e90: 6865 6d61 2c0a 2020 2020 2020 2020 2020  hema,.          
-00006ea0: 2020 636f 6e74 656e 743d 636f 6e74 656e    content=conten
-00006eb0: 740a 2020 2020 2020 2020 290a 0a20 2020  t.        )..   
-00006ec0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
-00006ed0: 2020 2064 6566 205f 5f74 6f5f 6865 6164     def __to_head
-00006ee0: 6572 7328 696e 5f64 6174 613a 2074 7970  ers(in_data: typ
-00006ef0: 696e 672e 5475 706c 655b 7479 7069 6e67  ing.Tuple[typing
-00006f00: 2e54 7570 6c65 5b73 7472 2c20 7374 725d  .Tuple[str, str]
-00006f10: 2c20 2e2e 2e5d 2920 2d3e 2048 5454 5048  , ...]) -> HTTPH
-00006f20: 6561 6465 7244 6963 743a 0a20 2020 2020  eaderDict:.     
-00006f30: 2020 2064 6174 6120 3d20 7475 706c 6528     data = tuple(
-00006f40: 7420 666f 7220 7420 696e 2069 6e5f 6461  t for t in in_da
-00006f50: 7461 2069 6620 7429 0a20 2020 2020 2020  ta if t).       
-00006f60: 2068 6561 6465 7273 203d 2048 5454 5048   headers = HTTPH
-00006f70: 6561 6465 7244 6963 7428 290a 2020 2020  eaderDict().    
-00006f80: 2020 2020 6966 206e 6f74 2064 6174 613a      if not data:
-00006f90: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00006fa0: 7572 6e20 6865 6164 6572 730a 2020 2020  urn headers.    
-00006fb0: 2020 2020 6865 6164 6572 732e 6578 7465      headers.exte
-00006fc0: 6e64 2864 6174 6129 0a20 2020 2020 2020  nd(data).       
-00006fd0: 2072 6574 7572 6e20 6865 6164 6572 730a   return headers.
-00006fe0: 0a20 2020 2064 6566 2073 6572 6961 6c69  .    def seriali
-00006ff0: 7a65 280a 2020 2020 2020 2020 7365 6c66  ze(.        self
-00007000: 2c0a 2020 2020 2020 2020 696e 5f64 6174  ,.        in_dat
-00007010: 613a 2074 7970 696e 672e 556e 696f 6e5b  a: typing.Union[
-00007020: 0a20 2020 2020 2020 2020 2020 2053 6368  .            Sch
-00007030: 656d 612c 2044 6563 696d 616c 2c20 696e  ema, Decimal, in
-00007040: 742c 2066 6c6f 6174 2c20 7374 722c 2064  t, float, str, d
-00007050: 6174 652c 2064 6174 6574 696d 652c 204e  ate, datetime, N
-00007060: 6f6e 652c 2062 6f6f 6c2c 206c 6973 742c  one, bool, list,
-00007070: 2074 7570 6c65 2c20 6469 6374 2c20 6672   tuple, dict, fr
-00007080: 6f7a 656e 6469 6374 2e66 726f 7a65 6e64  ozendict.frozend
-00007090: 6963 745d 0a20 2020 2029 202d 3e20 4854  ict].    ) -> HT
-000070a0: 5450 4865 6164 6572 4469 6374 3a0a 2020  TPHeaderDict:.  
-000070b0: 2020 2020 2020 6966 2073 656c 662e 7363        if self.sc
-000070c0: 6865 6d61 3a0a 2020 2020 2020 2020 2020  hema:.          
-000070d0: 2020 6361 7374 5f69 6e5f 6461 7461 203d    cast_in_data =
-000070e0: 2073 656c 662e 7363 6865 6d61 2869 6e5f   self.schema(in_
-000070f0: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
-00007100: 2020 6361 7374 5f69 6e5f 6461 7461 203d    cast_in_data =
-00007110: 2073 656c 662e 5f6a 736f 6e5f 656e 636f   self._json_enco
-00007120: 6465 722e 6465 6661 756c 7428 6361 7374  der.default(cast
-00007130: 5f69 6e5f 6461 7461 290a 2020 2020 2020  _in_data).      
-00007140: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00007150: 2020 2020 2020 7369 6d70 6c65 202d 3e20        simple -> 
-00007160: 6865 6164 6572 0a20 2020 2020 2020 2020  header.         
-00007170: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
-00007180: 506f 6f6c 4d61 6e61 6765 7220 6e65 6564  PoolManager need
-00007190: 7320 6120 6d61 7070 696e 672c 2074 7570  s a mapping, tup
-000071a0: 6c65 2069 7320 636c 6f73 650a 2020 2020  le is close.    
-000071b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071c0: 7265 7475 726e 7320 6865 6164 6572 733a  returns headers:
-000071d0: 2064 6963 740a 2020 2020 2020 2020 2020   dict.          
-000071e0: 2020 2222 220a 2020 2020 2020 2020 2020    """.          
-000071f0: 2020 6966 2073 656c 662e 7374 796c 653a    if self.style:
-00007200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007210: 2076 616c 7565 203d 2073 656c 662e 5f73   value = self._s
-00007220: 6572 6961 6c69 7a65 5f73 696d 706c 6528  erialize_simple(
-00007230: 6361 7374 5f69 6e5f 6461 7461 2c20 7365  cast_in_data, se
-00007240: 6c66 2e6e 616d 652c 2073 656c 662e 6578  lf.name, self.ex
-00007250: 706c 6f64 652c 2046 616c 7365 290a 2020  plode, False).  
-00007260: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00007270: 7475 726e 2073 656c 662e 5f5f 746f 5f68  turn self.__to_h
-00007280: 6561 6465 7273 2828 2873 656c 662e 6e61  eaders(((self.na
-00007290: 6d65 2c20 7661 6c75 6529 2c29 290a 2020  me, value),)).  
-000072a0: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
-000072b0: 7465 6e74 2077 696c 6c20 6265 206c 656e  tent will be len
-000072c0: 6774 6820 6f6e 650a 2020 2020 2020 2020  gth one.        
-000072d0: 666f 7220 636f 6e74 656e 745f 7479 7065  for content_type
-000072e0: 2c20 7363 6865 6d61 2069 6e20 7365 6c66  , schema in self
-000072f0: 2e63 6f6e 7465 6e74 2e69 7465 6d73 2829  .content.items()
-00007300: 3a0a 2020 2020 2020 2020 2020 2020 6361  :.            ca
-00007310: 7374 5f69 6e5f 6461 7461 203d 2073 6368  st_in_data = sch
-00007320: 656d 6128 696e 5f64 6174 6129 0a20 2020  ema(in_data).   
-00007330: 2020 2020 2020 2020 2063 6173 745f 696e           cast_in
-00007340: 5f64 6174 6120 3d20 7365 6c66 2e5f 6a73  _data = self._js
-00007350: 6f6e 5f65 6e63 6f64 6572 2e64 6566 6175  on_encoder.defau
-00007360: 6c74 2863 6173 745f 696e 5f64 6174 6129  lt(cast_in_data)
-00007370: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00007380: 7365 6c66 2e5f 636f 6e74 656e 745f 7479  self._content_ty
-00007390: 7065 5f69 735f 6a73 6f6e 2863 6f6e 7465  pe_is_json(conte
-000073a0: 6e74 5f74 7970 6529 3a0a 2020 2020 2020  nt_type):.      
-000073b0: 2020 2020 2020 2020 2020 7661 6c75 6520            value 
-000073c0: 3d20 7365 6c66 2e5f 7365 7269 616c 697a  = self._serializ
-000073d0: 655f 6a73 6f6e 2863 6173 745f 696e 5f64  e_json(cast_in_d
-000073e0: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
-000073f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00007400: 2e5f 5f74 6f5f 6865 6164 6572 7328 2828  .__to_headers(((
-00007410: 7365 6c66 2e6e 616d 652c 2076 616c 7565  self.name, value
-00007420: 292c 2929 0a20 2020 2020 2020 2020 2020  ),)).           
-00007430: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
-00007440: 656e 7465 6445 7272 6f72 2827 5365 7269  entedError('Seri
-00007450: 616c 697a 6174 696f 6e20 6f66 207b 7d20  alization of {} 
-00007460: 6861 7320 6e6f 7420 7965 7420 6265 656e  has not yet been
-00007470: 2069 6d70 6c65 6d65 6e74 6564 272e 666f   implemented'.fo
-00007480: 726d 6174 2863 6f6e 7465 6e74 5f74 7970  rmat(content_typ
-00007490: 6529 290a 0a0a 636c 6173 7320 456e 636f  e))...class Enco
-000074a0: 6469 6e67 3a0a 2020 2020 6465 6620 5f5f  ding:.    def __
-000074b0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-000074c0: 7365 6c66 2c0a 2020 2020 2020 2020 636f  self,.        co
-000074d0: 6e74 656e 745f 7479 7065 3a20 7374 722c  ntent_type: str,
-000074e0: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
-000074f0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00007500: 6c5b 7479 7069 6e67 2e44 6963 745b 7374  l[typing.Dict[st
-00007510: 722c 2048 6561 6465 7250 6172 616d 6574  r, HeaderParamet
-00007520: 6572 5d5d 203d 204e 6f6e 652c 0a20 2020  er]] = None,.   
-00007530: 2020 2020 2073 7479 6c65 3a20 7479 7069       style: typi
-00007540: 6e67 2e4f 7074 696f 6e61 6c5b 5061 7261  ng.Optional[Para
-00007550: 6d65 7465 7253 7479 6c65 5d20 3d20 4e6f  meterStyle] = No
-00007560: 6e65 2c0a 2020 2020 2020 2020 6578 706c  ne,.        expl
-00007570: 6f64 653a 2062 6f6f 6c20 3d20 4661 6c73  ode: bool = Fals
-00007580: 652c 0a20 2020 2020 2020 2061 6c6c 6f77  e,.        allow
-00007590: 5f72 6573 6572 7665 643a 2062 6f6f 6c20  _reserved: bool 
-000075a0: 3d20 4661 6c73 652c 0a20 2020 2029 3a0a  = False,.    ):.
-000075b0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000075c0: 7465 6e74 5f74 7970 6520 3d20 636f 6e74  tent_type = cont
-000075d0: 656e 745f 7479 7065 0a20 2020 2020 2020  ent_type.       
-000075e0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-000075f0: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-00007600: 7365 6c66 2e73 7479 6c65 203d 2073 7479  self.style = sty
-00007610: 6c65 0a20 2020 2020 2020 2073 656c 662e  le.        self.
-00007620: 6578 706c 6f64 6520 3d20 6578 706c 6f64  explode = explod
-00007630: 650a 2020 2020 2020 2020 7365 6c66 2e61  e.        self.a
-00007640: 6c6c 6f77 5f72 6573 6572 7665 6420 3d20  llow_reserved = 
-00007650: 616c 6c6f 775f 7265 7365 7276 6564 0a0a  allow_reserved..
-00007660: 0a40 6461 7461 636c 6173 730a 636c 6173  .@dataclass.clas
-00007670: 7320 4d65 6469 6154 7970 653a 0a20 2020  s MediaType:.   
-00007680: 2022 2222 0a20 2020 2055 7365 6420 746f   """.    Used to
-00007690: 2073 746f 7265 2072 6571 7565 7374 2061   store request a
-000076a0: 6e64 2072 6573 706f 6e73 6520 626f 6479  nd response body
-000076b0: 2073 6368 656d 6120 696e 666f 726d 6174   schema informat
-000076c0: 696f 6e0a 2020 2020 656e 636f 6469 6e67  ion.    encoding
-000076d0: 3a0a 2020 2020 2020 2020 4120 6d61 7020  :.        A map 
-000076e0: 6265 7477 6565 6e20 6120 7072 6f70 6572  between a proper
-000076f0: 7479 206e 616d 6520 616e 6420 6974 7320  ty name and its 
-00007700: 656e 636f 6469 6e67 2069 6e66 6f72 6d61  encoding informa
-00007710: 7469 6f6e 2e0a 2020 2020 2020 2020 5468  tion..        Th
-00007720: 6520 6b65 792c 2062 6569 6e67 2074 6865  e key, being the
-00007730: 2070 726f 7065 7274 7920 6e61 6d65 2c20   property name, 
-00007740: 4d55 5354 2065 7869 7374 2069 6e20 7468  MUST exist in th
-00007750: 6520 7363 6865 6d61 2061 7320 6120 7072  e schema as a pr
-00007760: 6f70 6572 7479 2e0a 2020 2020 2020 2020  operty..        
-00007770: 5468 6520 656e 636f 6469 6e67 206f 626a  The encoding obj
-00007780: 6563 7420 5348 414c 4c20 6f6e 6c79 2061  ect SHALL only a
-00007790: 7070 6c79 2074 6f20 7265 7175 6573 7442  pply to requestB
-000077a0: 6f64 7920 6f62 6a65 6374 7320 7768 656e  ody objects when
-000077b0: 2074 6865 206d 6564 6961 2074 7970 6520   the media type 
-000077c0: 6973 0a20 2020 2020 2020 206d 756c 7469  is.        multi
-000077d0: 7061 7274 206f 7220 6170 706c 6963 6174  part or applicat
-000077e0: 696f 6e2f 782d 7777 772d 666f 726d 2d75  ion/x-www-form-u
-000077f0: 726c 656e 636f 6465 642e 0a20 2020 2022  rlencoded..    "
-00007800: 2222 0a20 2020 2073 6368 656d 613a 2074  "".    schema: t
-00007810: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
-00007820: 7970 696e 672e 5479 7065 5b53 6368 656d  yping.Type[Schem
-00007830: 615d 5d20 3d20 4e6f 6e65 0a20 2020 2065  a]] = None.    e
-00007840: 6e63 6f64 696e 673a 2074 7970 696e 672e  ncoding: typing.
-00007850: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-00007860: 4469 6374 5b73 7472 2c20 456e 636f 6469  Dict[str, Encodi
-00007870: 6e67 5d5d 203d 204e 6f6e 650a 0a0a 4064  ng]] = None...@d
-00007880: 6174 6163 6c61 7373 0a63 6c61 7373 2041  ataclass.class A
-00007890: 7069 5265 7370 6f6e 7365 5769 7468 6f75  piResponseWithou
-000078a0: 7444 6573 6572 6961 6c69 7a61 7469 6f6e  tDeserialization
-000078b0: 2841 7069 5265 7370 6f6e 7365 293a 0a20  (ApiResponse):. 
-000078c0: 2020 2072 6573 706f 6e73 653a 2075 726c     response: url
-000078d0: 6c69 6233 2e48 5454 5052 6573 706f 6e73  lib3.HTTPRespons
-000078e0: 650a 2020 2020 626f 6479 3a20 7479 7069  e.    body: typi
-000078f0: 6e67 2e55 6e69 6f6e 5b55 6e73 6574 2c20  ng.Union[Unset, 
-00007900: 7479 7069 6e67 2e54 7970 655b 5363 6865  typing.Type[Sche
-00007910: 6d61 5d5d 203d 2075 6e73 6574 0a0a 0a63  ma]] = unset...c
-00007920: 6c61 7373 204f 7065 6e41 7069 5265 7370  lass OpenApiResp
-00007930: 6f6e 7365 284a 534f 4e44 6574 6563 746f  onse(JSONDetecto
-00007940: 7229 3a0a 2020 2020 5f5f 6669 6c65 6e61  r):.    __filena
-00007950: 6d65 5f63 6f6e 7465 6e74 5f64 6973 706f  me_content_dispo
-00007960: 7369 7469 6f6e 5f70 6174 7465 726e 203d  sition_pattern =
-00007970: 2072 652e 636f 6d70 696c 6528 2766 696c   re.compile('fil
-00007980: 656e 616d 653d 2228 2e2b 3f29 2227 290a  ename="(.+?)"').
-00007990: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000079a0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-000079b0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-000079c0: 655f 636c 733a 2074 7970 696e 672e 5479  e_cls: typing.Ty
-000079d0: 7065 5b41 7069 5265 7370 6f6e 7365 5d20  pe[ApiResponse] 
-000079e0: 3d20 4170 6952 6573 706f 6e73 652c 0a20  = ApiResponse,. 
-000079f0: 2020 2020 2020 2063 6f6e 7465 6e74 3a20         content: 
-00007a00: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00007a10: 7479 7069 6e67 2e44 6963 745b 7374 722c  typing.Dict[str,
-00007a20: 204d 6564 6961 5479 7065 5d5d 203d 204e   MediaType]] = N
-00007a30: 6f6e 652c 0a20 2020 2020 2020 2068 6561  one,.        hea
-00007a40: 6465 7273 3a20 7479 7069 6e67 2e4f 7074  ders: typing.Opt
-00007a50: 696f 6e61 6c5b 7479 7069 6e67 2e4c 6973  ional[typing.Lis
-00007a60: 745b 4865 6164 6572 5061 7261 6d65 7465  t[HeaderParamete
-00007a70: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
-00007a80: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00007a90: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-00007aa0: 730a 2020 2020 2020 2020 6966 2063 6f6e  s.        if con
-00007ab0: 7465 6e74 2069 7320 6e6f 7420 4e6f 6e65  tent is not None
-00007ac0: 2061 6e64 206c 656e 2863 6f6e 7465 6e74   and len(content
-00007ad0: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
-00007ae0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00007af0: 7272 6f72 2827 496e 7661 6c69 6420 7661  rror('Invalid va
-00007b00: 6c75 6520 666f 7220 636f 6e74 656e 742c  lue for content,
-00007b10: 2074 6865 2063 6f6e 7465 6e74 2064 6963   the content dic
-00007b20: 7420 6d75 7374 2068 6176 6520 3e3d 2031  t must have >= 1
-00007b30: 2065 6e74 7279 2729 0a20 2020 2020 2020   entry').       
-00007b40: 2073 656c 662e 636f 6e74 656e 7420 3d20   self.content = 
-00007b50: 636f 6e74 656e 740a 2020 2020 2020 2020  content.        
-00007b60: 7365 6c66 2e72 6573 706f 6e73 655f 636c  self.response_cl
-00007b70: 7320 3d20 7265 7370 6f6e 7365 5f63 6c73  s = response_cls
-00007b80: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-00007b90: 686f 640a 2020 2020 6465 6620 5f5f 6465  hod.    def __de
-00007ba0: 7365 7269 616c 697a 655f 6a73 6f6e 2872  serialize_json(r
-00007bb0: 6573 706f 6e73 653a 2075 726c 6c69 6233  esponse: urllib3
-00007bc0: 2e48 5454 5052 6573 706f 6e73 6529 202d  .HTTPResponse) -
-00007bd0: 3e20 7479 7069 6e67 2e41 6e79 3a0a 2020  > typing.Any:.  
-00007be0: 2020 2020 2020 2320 7079 7468 6f6e 206d        # python m
-00007bf0: 7573 7420 6265 203e 3d20 332e 3920 736f  ust be >= 3.9 so
-00007c00: 2077 6520 6361 6e20 7061 7373 2069 6e20   we can pass in 
-00007c10: 6279 7465 7320 696e 746f 206a 736f 6e2e  bytes into json.
-00007c20: 6c6f 6164 730a 2020 2020 2020 2020 7265  loads.        re
-00007c30: 7475 726e 206a 736f 6e2e 6c6f 6164 7328  turn json.loads(
-00007c40: 7265 7370 6f6e 7365 2e64 6174 6129 0a0a  response.data)..
-00007c50: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
-00007c60: 640a 2020 2020 6465 6620 5f5f 6669 6c65  d.    def __file
-00007c70: 5f6e 616d 655f 6672 6f6d 5f72 6573 706f  _name_from_respo
-00007c80: 6e73 655f 7572 6c28 7265 7370 6f6e 7365  nse_url(response
-00007c90: 5f75 726c 3a20 7479 7069 6e67 2e4f 7074  _url: typing.Opt
-00007ca0: 696f 6e61 6c5b 7374 725d 2920 2d3e 2074  ional[str]) -> t
-00007cb0: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-00007cc0: 7472 5d3a 0a20 2020 2020 2020 2069 6620  tr]:.        if 
-00007cd0: 7265 7370 6f6e 7365 5f75 726c 2069 7320  response_url is 
-00007ce0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00007cf0: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
-00007d00: 2020 2020 2020 7572 6c5f 7061 7468 203d        url_path =
-00007d10: 2075 726c 7061 7273 6528 7265 7370 6f6e   urlparse(respon
-00007d20: 7365 5f75 726c 292e 7061 7468 0a20 2020  se_url).path.   
-00007d30: 2020 2020 2069 6620 7572 6c5f 7061 7468       if url_path
-00007d40: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-00007d50: 7468 5f62 6173 656e 616d 6520 3d20 6f73  th_basename = os
-00007d60: 2e70 6174 682e 6261 7365 6e61 6d65 2875  .path.basename(u
-00007d70: 726c 5f70 6174 6829 0a20 2020 2020 2020  rl_path).       
-00007d80: 2020 2020 2069 6620 7061 7468 5f62 6173       if path_bas
-00007d90: 656e 616d 653a 0a20 2020 2020 2020 2020  ename:.         
-00007da0: 2020 2020 2020 205f 6669 6c65 6e61 6d65         _filename
-00007db0: 2c20 6578 7420 3d20 6f73 2e70 6174 682e  , ext = os.path.
-00007dc0: 7370 6c69 7465 7874 2870 6174 685f 6261  splitext(path_ba
-00007dd0: 7365 6e61 6d65 290a 2020 2020 2020 2020  sename).        
-00007de0: 2020 2020 2020 2020 6966 2065 7874 3a0a          if ext:.
-00007df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e00: 2020 2020 7265 7475 726e 2070 6174 685f      return path_
-00007e10: 6261 7365 6e61 6d65 0a20 2020 2020 2020  basename.       
-00007e20: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
-00007e30: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-00007e40: 2020 2064 6566 205f 5f66 696c 655f 6e61     def __file_na
-00007e50: 6d65 5f66 726f 6d5f 636f 6e74 656e 745f  me_from_content_
-00007e60: 6469 7370 6f73 6974 696f 6e28 636c 732c  disposition(cls,
-00007e70: 2063 6f6e 7465 6e74 5f64 6973 706f 7369   content_disposi
-00007e80: 7469 6f6e 3a20 7479 7069 6e67 2e4f 7074  tion: typing.Opt
-00007e90: 696f 6e61 6c5b 7374 725d 2920 2d3e 2074  ional[str]) -> t
-00007ea0: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-00007eb0: 7472 5d3a 0a20 2020 2020 2020 2069 6620  tr]:.        if 
-00007ec0: 636f 6e74 656e 745f 6469 7370 6f73 6974  content_disposit
-00007ed0: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
-00007ee0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00007ef0: 4e6f 6e65 0a20 2020 2020 2020 206d 6174  None.        mat
-00007f00: 6368 203d 2063 6c73 2e5f 5f66 696c 656e  ch = cls.__filen
-00007f10: 616d 655f 636f 6e74 656e 745f 6469 7370  ame_content_disp
-00007f20: 6f73 6974 696f 6e5f 7061 7474 6572 6e2e  osition_pattern.
-00007f30: 7365 6172 6368 2863 6f6e 7465 6e74 5f64  search(content_d
-00007f40: 6973 706f 7369 7469 6f6e 290a 2020 2020  isposition).    
-00007f50: 2020 2020 6966 206e 6f74 206d 6174 6368      if not match
-00007f60: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00007f70: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
-00007f80: 2020 7265 7475 726e 206d 6174 6368 2e67    return match.g
-00007f90: 726f 7570 2831 290a 0a20 2020 2064 6566  roup(1)..    def
-00007fa0: 205f 5f64 6573 6572 6961 6c69 7a65 5f61   __deserialize_a
-00007fb0: 7070 6c69 6361 7469 6f6e 5f6f 6374 6574  pplication_octet
-00007fc0: 5f73 7472 6561 6d28 0a20 2020 2020 2020  _stream(.       
-00007fd0: 2073 656c 662c 2072 6573 706f 6e73 653a   self, response:
-00007fe0: 2075 726c 6c69 6233 2e48 5454 5052 6573   urllib3.HTTPRes
-00007ff0: 706f 6e73 650a 2020 2020 2920 2d3e 2074  ponse.    ) -> t
-00008000: 7970 696e 672e 556e 696f 6e5b 6279 7465  yping.Union[byte
-00008010: 732c 2069 6f2e 4275 6666 6572 6564 5265  s, io.BufferedRe
-00008020: 6164 6572 5d3a 0a20 2020 2020 2020 2022  ader]:.        "
-00008030: 2222 0a20 2020 2020 2020 2075 726c 6c69  "".        urlli
-00008040: 6233 2075 7365 2063 6173 6573 3a0a 2020  b3 use cases:.  
-00008050: 2020 2020 2020 312e 2077 6865 6e20 7072        1. when pr
-00008060: 656c 6f61 645f 636f 6e74 656e 743d 5472  eload_content=Tr
-00008070: 7565 2028 7374 7265 616d 3d46 616c 7365  ue (stream=False
-00008080: 2920 7468 656e 2073 7570 706f 7274 735f  ) then supports_
-00008090: 6368 756e 6b65 645f 7265 6164 7320 6973  chunked_reads is
-000080a0: 2046 616c 7365 2061 6e64 2062 7974 6573   False and bytes
-000080b0: 2061 7265 2072 6574 7572 6e65 640a 2020   are returned.  
-000080c0: 2020 2020 2020 322e 2077 6865 6e20 7072        2. when pr
-000080d0: 656c 6f61 645f 636f 6e74 656e 743d 4661  eload_content=Fa
-000080e0: 6c73 6520 2873 7472 6561 6d3d 5472 7565  lse (stream=True
-000080f0: 2920 7468 656e 2073 7570 706f 7274 735f  ) then supports_
-00008100: 6368 756e 6b65 645f 7265 6164 7320 6973  chunked_reads is
-00008110: 2054 7275 6520 616e 640a 2020 2020 2020   True and.      
-00008120: 2020 2020 2020 6120 6669 6c65 2077 696c        a file wil
-00008130: 6c20 6265 2077 7269 7474 656e 2061 6e64  l be written and
-00008140: 2072 6574 7572 6e65 640a 2020 2020 2020   returned.      
-00008150: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00008160: 2072 6573 706f 6e73 652e 7375 7070 6f72   response.suppor
-00008170: 7473 5f63 6875 6e6b 6564 5f72 6561 6473  ts_chunked_reads
-00008180: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00008190: 6669 6c65 5f6e 616d 6520 3d20 280a 2020  file_name = (.  
-000081a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000081b0: 6c66 2e5f 5f66 696c 655f 6e61 6d65 5f66  lf.__file_name_f
-000081c0: 726f 6d5f 636f 6e74 656e 745f 6469 7370  rom_content_disp
-000081d0: 6f73 6974 696f 6e28 7265 7370 6f6e 7365  osition(response
-000081e0: 2e68 6561 6465 7273 2e67 6574 2827 636f  .headers.get('co
-000081f0: 6e74 656e 742d 6469 7370 6f73 6974 696f  ntent-dispositio
-00008200: 6e27 2929 0a20 2020 2020 2020 2020 2020  n')).           
-00008210: 2020 2020 206f 7220 7365 6c66 2e5f 5f66       or self.__f
-00008220: 696c 655f 6e61 6d65 5f66 726f 6d5f 7265  ile_name_from_re
-00008230: 7370 6f6e 7365 5f75 726c 2872 6573 706f  sponse_url(respo
-00008240: 6e73 652e 6765 7475 726c 2829 290a 2020  nse.geturl()).  
-00008250: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00008260: 2020 2020 2020 2020 2069 6620 6669 6c65           if file
-00008270: 5f6e 616d 6520 6973 204e 6f6e 653a 0a20  _name is None:. 
-00008280: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-00008290: 6664 2c20 7061 7468 203d 2074 656d 7066  fd, path = tempf
-000082a0: 696c 652e 6d6b 7374 656d 7028 290a 2020  ile.mkstemp().  
-000082b0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-000082c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082d0: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
-000082e0: 6f69 6e28 7465 6d70 6669 6c65 2e67 6574  oin(tempfile.get
-000082f0: 7465 6d70 6469 7228 292c 2066 696c 655f  tempdir(), file_
-00008300: 6e61 6d65 290a 0a20 2020 2020 2020 2020  name)..         
-00008310: 2020 2077 6974 6820 6f70 656e 2870 6174     with open(pat
-00008320: 682c 2027 7762 2729 2061 7320 6e65 775f  h, 'wb') as new_
-00008330: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
-00008340: 2020 2020 2020 6368 756e 6b5f 7369 7a65        chunk_size
-00008350: 203d 2031 3032 340a 2020 2020 2020 2020   = 1024.        
-00008360: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
-00008370: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
-00008380: 2020 2020 2020 2020 6461 7461 203d 2072          data = r
-00008390: 6573 706f 6e73 652e 7265 6164 2863 6875  esponse.read(chu
-000083a0: 6e6b 5f73 697a 6529 0a20 2020 2020 2020  nk_size).       
-000083b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000083c0: 6e6f 7420 6461 7461 3a0a 2020 2020 2020  not data:.      
-000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083e0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-000083f0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-00008400: 6669 6c65 2e77 7269 7465 2864 6174 6129  file.write(data)
-00008410: 0a20 2020 2020 2020 2020 2020 2023 2072  .            # r
-00008420: 656c 6561 7365 5f63 6f6e 6e20 6973 206e  elease_conn is n
-00008430: 6565 6465 6420 666f 7220 7374 7265 616d  eeded for stream
-00008440: 696e 6720 636f 6e6e 6563 7469 6f6e 7320  ing connections 
-00008450: 6f6e 6c79 0a20 2020 2020 2020 2020 2020  only.           
-00008460: 2072 6573 706f 6e73 652e 7265 6c65 6173   response.releas
-00008470: 655f 636f 6e6e 2829 0a20 2020 2020 2020  e_conn().       
-00008480: 2020 2020 206e 6577 5f66 696c 6520 3d20       new_file = 
-00008490: 6f70 656e 2870 6174 682c 2027 7262 2729  open(path, 'rb')
-000084a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000084b0: 7572 6e20 6e65 775f 6669 6c65 0a20 2020  urn new_file.   
-000084c0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000084d0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000084e0: 7370 6f6e 7365 2e64 6174 610a 0a20 2020  sponse.data..   
-000084f0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
-00008500: 2020 2064 6566 205f 5f64 6573 6572 6961     def __deseria
-00008510: 6c69 7a65 5f6d 756c 7469 7061 7274 5f66  lize_multipart_f
-00008520: 6f72 6d5f 6461 7461 280a 2020 2020 2020  orm_data(.      
-00008530: 2020 7265 7370 6f6e 7365 3a20 7572 6c6c    response: urll
-00008540: 6962 332e 4854 5450 5265 7370 6f6e 7365  ib3.HTTPResponse
-00008550: 0a20 2020 2029 202d 3e20 7479 7069 6e67  .    ) -> typing
-00008560: 2e44 6963 745b 7374 722c 2074 7970 696e  .Dict[str, typin
-00008570: 672e 416e 795d 3a0a 2020 2020 2020 2020  g.Any]:.        
-00008580: 6d73 6720 3d20 656d 6169 6c2e 6d65 7373  msg = email.mess
-00008590: 6167 655f 6672 6f6d 5f62 7974 6573 2872  age_from_bytes(r
-000085a0: 6573 706f 6e73 652e 6461 7461 290a 2020  esponse.data).  
-000085b0: 2020 2020 2020 7265 7475 726e 207b 0a20        return {. 
-000085c0: 2020 2020 2020 2020 2020 2070 6172 742e             part.
-000085d0: 6765 745f 7061 7261 6d28 226e 616d 6522  get_param("name"
-000085e0: 2c20 6865 6164 6572 3d22 436f 6e74 656e  , header="Conten
-000085f0: 742d 4469 7370 6f73 6974 696f 6e22 293a  t-Disposition"):
-00008600: 2070 6172 742e 6765 745f 7061 796c 6f61   part.get_payloa
-00008610: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
-00008620: 2020 2064 6563 6f64 653d 5472 7565 0a20     decode=True. 
-00008630: 2020 2020 2020 2020 2020 2029 2e64 6563             ).dec
-00008640: 6f64 6528 7061 7274 2e67 6574 5f63 6f6e  ode(part.get_con
-00008650: 7465 6e74 5f63 6861 7273 6574 2829 290a  tent_charset()).
-00008660: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-00008670: 6172 742e 6765 745f 636f 6e74 656e 745f  art.get_content_
-00008680: 6368 6172 7365 7428 290a 2020 2020 2020  charset().      
-00008690: 2020 2020 2020 656c 7365 2070 6172 742e        else part.
-000086a0: 6765 745f 7061 796c 6f61 6428 290a 2020  get_payload().  
-000086b0: 2020 2020 2020 2020 2020 666f 7220 7061            for pa
-000086c0: 7274 2069 6e20 6d73 672e 6765 745f 7061  rt in msg.get_pa
-000086d0: 796c 6f61 6428 290a 2020 2020 2020 2020  yload().        
-000086e0: 7d0a 0a20 2020 2064 6566 205f 5f67 6574  }..    def __get
-000086f0: 5f73 6368 656d 615f 666f 725f 636f 6e74  _schema_for_cont
-00008700: 656e 745f 7479 7065 280a 2020 2020 2020  ent_type(.      
-00008710: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00008720: 636f 6e74 656e 745f 7479 7065 0a20 2020  content_type.   
-00008730: 2029 202d 3e20 7479 7069 6e67 2e4f 7074   ) -> typing.Opt
-00008740: 696f 6e61 6c5b 7479 7069 6e67 2e54 7970  ional[typing.Typ
-00008750: 655b 5363 6865 6d61 5d5d 3a0a 2020 2020  e[Schema]]:.    
-00008760: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00008770: 4669 6e64 7320 7468 6520 636f 7272 6563  Finds the correc
-00008780: 7420 5363 6865 6d61 4f62 6a65 6374 2066  t SchemaObject f
-00008790: 6f72 2061 2070 6172 7469 6375 6c61 7220  or a particular 
-000087a0: 636f 6e74 656e 7420 7479 7065 2e20 4861  content type. Ha
-000087b0: 6e64 6c65 730a 2020 2020 2020 2020 7468  ndles.        th
-000087c0: 6520 6173 7465 7269 736b 2022 2a22 2063  e asterisk "*" c
-000087d0: 6861 7261 6374 6572 2074 6861 7420 6973  haracter that is
-000087e0: 2075 7365 6420 746f 2067 726f 7570 206d   used to group m
-000087f0: 6564 6961 2074 7970 6573 2069 6e74 6f20  edia types into 
-00008800: 7261 6e67 6573 0a20 2020 2020 2020 2028  ranges.        (
-00008810: 6874 7470 733a 2f2f 7777 772e 7266 632d  https://www.rfc-
-00008820: 6564 6974 6f72 2e6f 7267 2f72 6663 2f72  editor.org/rfc/r
-00008830: 6663 3732 3331 2373 6563 7469 6f6e 2d35  fc7231#section-5
-00008840: 2e33 2e32 292e 2041 6c73 6f20 6861 6e64  .3.2). Also hand
-00008850: 6c65 730a 2020 2020 2020 2020 7061 7261  les.        para
-00008860: 6d65 7465 7273 2069 6e20 7468 6520 666f  meters in the fo
-00008870: 726d 206f 6620 6e61 6d65 3d76 616c 7565  rm of name=value
-00008880: 2070 6169 7273 2e0a 2020 2020 2020 2020   pairs..        
-00008890: 2222 220a 2020 2020 2020 2020 6d65 6469  """.        medi
-000088a0: 615f 7479 7065 7320 3d20 7365 6c66 2e63  a_types = self.c
-000088b0: 6f6e 7465 6e74 2e6b 6579 7328 290a 2020  ontent.keys().  
-000088c0: 2020 2020 2020 6d61 7463 6865 645f 6d65        matched_me
-000088d0: 6469 615f 7479 7065 203d 204f 7065 6e41  dia_type = OpenA
-000088e0: 7069 5265 7370 6f6e 7365 2e6d 6174 6368  piResponse.match
-000088f0: 5f63 6f6e 7465 6e74 5f74 7970 6528 0a20  _content_type(. 
-00008900: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
-00008910: 6e74 5f74 7970 653d 636f 6e74 656e 745f  nt_type=content_
-00008920: 7479 7065 2c0a 2020 2020 2020 2020 2020  type,.          
-00008930: 2020 6d65 6469 615f 7479 7065 733d 6d65    media_types=me
-00008940: 6469 615f 7479 7065 730a 2020 2020 2020  dia_types.      
-00008950: 2020 290a 2020 2020 2020 2020 6966 206d    ).        if m
-00008960: 6174 6368 6564 5f6d 6564 6961 5f74 7970  atched_media_typ
-00008970: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
-00008980: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00008990: 6e65 0a20 2020 2020 2020 2072 6574 7572  ne.        retur
-000089a0: 6e20 7365 6c66 2e63 6f6e 7465 6e74 5b6d  n self.content[m
-000089b0: 6174 6368 6564 5f6d 6564 6961 5f74 7970  atched_media_typ
-000089c0: 655d 2e73 6368 656d 610a 0a20 2020 2040  e].schema..    @
-000089d0: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
-000089e0: 2064 6566 206d 6174 6368 5f63 6f6e 7465   def match_conte
-000089f0: 6e74 5f74 7970 6528 636f 6e74 656e 745f  nt_type(content_
-00008a00: 7479 7065 3a20 7374 722c 206d 6564 6961  type: str, media
-00008a10: 5f74 7970 6573 3a20 7479 7069 6e67 2e4c  _types: typing.L
-00008a20: 6973 745b 7374 725d 2920 2d3e 2074 7970  ist[str]) -> typ
-00008a30: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-00008a40: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
-00008a50: 2020 2020 2020 204d 6174 6368 6573 2061         Matches a
-00008a60: 2063 6f6e 7465 6e74 2074 7970 6520 746f   content type to
-00008a70: 2061 206d 6564 6961 2074 7970 6520 696e   a media type in
-00008a80: 2061 206c 6973 7420 6f66 206d 6564 6961   a list of media
-00008a90: 2074 7970 6573 2c20 6861 6e64 6c69 6e67   types, handling
-00008aa0: 206d 6564 6961 2074 7970 6520 7261 6e67   media type rang
-00008ab0: 6573 2061 7320 6465 6669 6e65 6420 696e  es as defined in
-00008ac0: 2052 4643 3732 3331 2e0a 0a20 2020 2020   RFC7231...     
-00008ad0: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
-00008ae0: 2020 2020 2020 2063 6f6e 7465 6e74 5f74         content_t
-00008af0: 7970 6520 2873 7472 293a 2054 6865 2063  ype (str): The c
-00008b00: 6f6e 7465 6e74 2074 7970 6520 746f 206d  ontent type to m
-00008b10: 6174 6368 2e0a 2020 2020 2020 2020 6d65  atch..        me
-00008b20: 6469 615f 7479 7065 7320 286c 6973 7429  dia_types (list)
-00008b30: 3a20 5468 6520 6c69 7374 206f 6620 6d65  : The list of me
-00008b40: 6469 6120 7479 7065 7320 746f 2073 6561  dia types to sea
-00008b50: 7263 682e 0a0a 2020 2020 2020 2020 5265  rch...        Re
-00008b60: 7475 726e 733a 0a20 2020 2020 2020 2073  turns:.        s
-00008b70: 7472 3a20 5468 6520 6669 7273 7420 6d65  tr: The first me
-00008b80: 6469 6120 7479 7065 2074 6861 7420 6d61  dia type that ma
-00008b90: 7463 6865 7320 7468 6520 636f 6e74 656e  tches the conten
-00008ba0: 7420 7479 7065 2c20 6f72 204e 6f6e 6520  t type, or None 
-00008bb0: 6966 206e 6f20 6d61 7463 6820 6973 2066  if no match is f
-00008bc0: 6f75 6e64 2e0a 2020 2020 2020 2020 2222  ound..        ""
-00008bd0: 220a 2020 2020 2020 2020 666f 7220 6d65  ".        for me
-00008be0: 6469 615f 7479 7065 2069 6e20 6d65 6469  dia_type in medi
-00008bf0: 615f 7479 7065 733a 0a20 2020 2020 2020  a_types:.       
-00008c00: 2020 2020 2069 6620 6d65 6469 615f 7479       if media_ty
-00008c10: 7065 203d 3d20 272a 2f2a 2720 6f72 206d  pe == '*/*' or m
-00008c20: 6564 6961 5f74 7970 6520 3d3d 2063 6f6e  edia_type == con
-00008c30: 7465 6e74 5f74 7970 653a 0a20 2020 2020  tent_type:.     
-00008c40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00008c50: 6e20 6d65 6469 615f 7479 7065 0a20 2020  n media_type.   
-00008c60: 2020 2020 2020 2020 2065 6c69 6620 272f           elif '/
-00008c70: 2720 696e 206d 6564 6961 5f74 7970 653a  ' in media_type:
-00008c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008c90: 2074 7970 655f 2c20 7375 6274 7970 6520   type_, subtype 
-00008ca0: 3d20 6d65 6469 615f 7479 7065 2e73 706c  = media_type.spl
-00008cb0: 6974 2827 2f27 290a 2020 2020 2020 2020  it('/').        
-00008cc0: 2020 2020 2020 2020 6966 2028 7479 7065          if (type
-00008cd0: 5f20 3d3d 2027 2a27 206f 7220 7479 7065  _ == '*' or type
-00008ce0: 5f20 3d3d 2063 6f6e 7465 6e74 5f74 7970  _ == content_typ
-00008cf0: 652e 7370 6c69 7428 272f 2729 5b30 5d29  e.split('/')[0])
-00008d00: 2061 6e64 205c 0a20 2020 2020 2020 2020   and \.         
-00008d10: 2020 2020 2020 2028 7375 6274 7970 6520         (subtype 
-00008d20: 3d3d 2027 2a27 206f 7220 7375 6274 7970  == '*' or subtyp
-00008d30: 6520 3d3d 2063 6f6e 7465 6e74 5f74 7970  e == content_typ
-00008d40: 652e 7370 6c69 7428 272f 2729 5b31 5d2e  e.split('/')[1].
-00008d50: 7370 6c69 7428 273b 2729 5b30 5d29 3a0a  split(';')[0]):.
-00008d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d70: 2020 2020 7265 7475 726e 206d 6564 6961      return media
-00008d80: 5f74 7970 650a 0a20 2020 2020 2020 2072  _type..        r
-00008d90: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-00008da0: 6465 6620 6465 7365 7269 616c 697a 6528  def deserialize(
-00008db0: 7365 6c66 2c20 7265 7370 6f6e 7365 3a20  self, response: 
-00008dc0: 5265 7370 6f6e 7365 5772 6170 7065 722c  ResponseWrapper,
-00008dd0: 2063 6f6e 6669 6775 7261 7469 6f6e 3a20   configuration: 
-00008de0: 436f 6e66 6967 7572 6174 696f 6e2c 2073  Configuration, s
-00008df0: 6b69 705f 6465 7365 7269 616c 697a 6174  kip_deserializat
-00008e00: 696f 6e20 3d20 4661 6c73 6529 202d 3e20  ion = False) -> 
-00008e10: 4170 6952 6573 706f 6e73 653a 0a20 2020  ApiResponse:.   
-00008e20: 2020 2020 2063 6f6e 7465 6e74 5f74 7970       content_typ
-00008e30: 6520 3d20 7265 7370 6f6e 7365 2e68 7474  e = response.htt
-00008e40: 705f 7265 7370 6f6e 7365 2e68 6561 6465  p_response.heade
-00008e50: 7273 2e67 6574 2827 636f 6e74 656e 742d  rs.get('content-
-00008e60: 7479 7065 2729 0a20 2020 2020 2020 2064  type').        d
-00008e70: 6573 6572 6961 6c69 7a65 645f 626f 6479  eserialized_body
-00008e80: 203d 2075 6e73 6574 0a20 2020 2020 2020   = unset.       
-00008e90: 2073 7472 6561 6d65 6420 3d20 7265 7370   streamed = resp
-00008ea0: 6f6e 7365 2e68 7474 705f 7265 7370 6f6e  onse.http_respon
-00008eb0: 7365 2e73 7570 706f 7274 735f 6368 756e  se.supports_chun
-00008ec0: 6b65 645f 7265 6164 7328 290a 0a20 2020  ked_reads()..   
-00008ed0: 2020 2020 2064 6573 6572 6961 6c69 7a65       deserialize
-00008ee0: 645f 6865 6164 6572 7320 3d20 756e 7365  d_headers = unse
-00008ef0: 740a 2020 2020 2020 2020 6966 2073 656c  t.        if sel
-00008f00: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-00008f10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00008f20: 2020 2023 2054 4f44 4f20 6164 6420 6865     # TODO add he
-00008f30: 6164 6572 2064 6573 6572 6961 6c69 6174  ader deserialiat
-00008f40: 696f 6e20 6865 7265 0a20 2020 2020 2020  ion here.       
-00008f50: 2020 2020 2070 6173 730a 0a20 2020 2020       pass..     
-00008f60: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
-00008f70: 6e74 2069 7320 6e6f 7420 4e6f 6e65 3a0a  nt is not None:.
-00008f80: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00008f90: 656e 2873 656c 662e 636f 6e74 656e 7429  en(self.content)
-00008fa0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-00008fb0: 2020 2020 2020 2023 2073 6f6d 6520 7370         # some sp
-00008fc0: 6563 7320 646f 206e 6f74 2064 6566 696e  ecs do not defin
-00008fd0: 6520 7265 7370 6f6e 7365 2063 6f6e 7465  e response conte
-00008fe0: 6e74 206d 6564 6961 2074 7970 6520 7363  nt media type sc
-00008ff0: 6865 6d61 730a 2020 2020 2020 2020 2020  hemas.          
-00009000: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00009010: 662e 7265 7370 6f6e 7365 5f63 6c73 280a  f.response_cls(.
-00009020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009030: 2020 2020 726f 756e 645f 7472 6970 5f74      round_trip_t
-00009040: 696d 653d 7265 7370 6f6e 7365 2e72 6f75  ime=response.rou
-00009050: 6e64 5f74 7269 705f 7469 6d65 2c0a 2020  nd_trip_time,.  
-00009060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009070: 2020 7265 7370 6f6e 7365 3d72 6573 706f    response=respo
-00009080: 6e73 652e 6874 7470 5f72 6573 706f 6e73  nse.http_respons
-00009090: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000090a0: 2020 2020 2020 2062 6f64 793d 756e 7365         body=unse
-000090b0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-000090c0: 2020 2020 2020 2068 6561 6465 7273 3d72         headers=r
-000090d0: 6573 706f 6e73 652e 6874 7470 5f72 6573  esponse.http_res
-000090e0: 706f 6e73 652e 6865 6164 6572 732c 0a20  ponse.headers,. 
-000090f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009100: 2020 2073 7461 7475 733d 7265 7370 6f6e     status=respon
-00009110: 7365 2e68 7474 705f 7265 7370 6f6e 7365  se.http_response
-00009120: 2e73 7461 7475 730a 2020 2020 2020 2020  .status.        
-00009130: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00009140: 2020 2020 2020 626f 6479 5f73 6368 656d        body_schem
-00009150: 6120 3d20 7365 6c66 2e5f 5f67 6574 5f73  a = self.__get_s
-00009160: 6368 656d 615f 666f 725f 636f 6e74 656e  chema_for_conten
-00009170: 745f 7479 7065 2863 6f6e 7465 6e74 5f74  t_type(content_t
-00009180: 7970 6529 0a20 2020 2020 2020 2020 2020  ype).           
-00009190: 2069 6620 626f 6479 5f73 6368 656d 6120   if body_schema 
-000091a0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-000091b0: 2020 2020 2020 2020 2072 6169 7365 2041           raise A
-000091c0: 7069 5661 6c75 6545 7272 6f72 280a 2020  piValueError(.  
-000091d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091e0: 2020 6622 496e 7661 6c69 6420 636f 6e74    f"Invalid cont
-000091f0: 656e 745f 7479 7065 2072 6574 7572 6e65  ent_type returne
-00009200: 642e 2043 6f6e 7465 6e74 5f74 7970 653d  d. Content_type=
-00009210: 277b 636f 6e74 656e 745f 7479 7065 7d27  '{content_type}'
-00009220: 2077 6173 2072 6574 7572 6e65 6420 220a   was returned ".
-00009230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009240: 2020 2020 6622 7768 656e 206f 6e6c 7920      f"when only 
-00009250: 7b73 7472 2873 6574 2873 656c 662e 636f  {str(set(self.co
-00009260: 6e74 656e 7429 297d 2061 7265 2064 6566  ntent))} are def
-00009270: 696e 6564 2066 6f72 2073 7461 7475 735f  ined for status_
-00009280: 636f 6465 3d7b 7374 7228 7265 7370 6f6e  code={str(respon
-00009290: 7365 2e68 7474 705f 7265 7370 6f6e 7365  se.http_response
-000092a0: 2e73 7461 7475 7329 7d22 0a20 2020 2020  .status)}".     
-000092b0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-000092c0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000092d0: 662e 5f63 6f6e 7465 6e74 5f74 7970 655f  f._content_type_
-000092e0: 6973 5f6a 736f 6e28 636f 6e74 656e 745f  is_json(content_
-000092f0: 7479 7065 293a 0a20 2020 2020 2020 2020  type):.         
-00009300: 2020 2020 2020 2062 6f64 795f 6461 7461         body_data
-00009310: 203d 2073 656c 662e 5f5f 6465 7365 7269   = self.__deseri
-00009320: 616c 697a 655f 6a73 6f6e 2872 6573 706f  alize_json(respo
-00009330: 6e73 652e 6874 7470 5f72 6573 706f 6e73  nse.http_respons
-00009340: 6529 0a20 2020 2020 2020 2020 2020 2065  e).            e
-00009350: 6c69 6620 636f 6e74 656e 745f 7479 7065  lif content_type
-00009360: 203d 3d20 2761 7070 6c69 6361 7469 6f6e   == 'application
-00009370: 2f6f 6374 6574 2d73 7472 6561 6d27 3a0a  /octet-stream':.
-00009380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009390: 626f 6479 5f64 6174 6120 3d20 7365 6c66  body_data = self
-000093a0: 2e5f 5f64 6573 6572 6961 6c69 7a65 5f61  .__deserialize_a
-000093b0: 7070 6c69 6361 7469 6f6e 5f6f 6374 6574  pplication_octet
-000093c0: 5f73 7472 6561 6d28 7265 7370 6f6e 7365  _stream(response
-000093d0: 2e68 7474 705f 7265 7370 6f6e 7365 290a  .http_response).
-000093e0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000093f0: 2063 6f6e 7465 6e74 5f74 7970 652e 7374   content_type.st
-00009400: 6172 7473 7769 7468 2827 6d75 6c74 6970  artswith('multip
-00009410: 6172 742f 666f 726d 2d64 6174 6127 293a  art/form-data'):
-00009420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009430: 2062 6f64 795f 6461 7461 203d 2073 656c   body_data = sel
-00009440: 662e 5f5f 6465 7365 7269 616c 697a 655f  f.__deserialize_
-00009450: 6d75 6c74 6970 6172 745f 666f 726d 5f64  multipart_form_d
-00009460: 6174 6128 7265 7370 6f6e 7365 2e68 7474  ata(response.htt
-00009470: 705f 7265 7370 6f6e 7365 290a 2020 2020  p_response).    
-00009480: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00009490: 656e 745f 7479 7065 203d 2027 6d75 6c74  ent_type = 'mult
-000094a0: 6970 6172 742f 666f 726d 2d64 6174 6127  ipart/form-data'
-000094b0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000094c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000094d0: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
-000094e0: 656d 656e 7465 6445 7272 6f72 2827 4465  ementedError('De
-000094f0: 7365 7269 616c 697a 6174 696f 6e20 6f66  serialization of
-00009500: 207b 7d20 6861 7320 6e6f 7420 7965 7420   {} has not yet 
-00009510: 6265 656e 2069 6d70 6c65 6d65 6e74 6564  been implemented
-00009520: 272e 666f 726d 6174 2863 6f6e 7465 6e74  '.format(content
-00009530: 5f74 7970 6529 290a 2020 2020 2020 2020  _type)).        
-00009540: 2020 2020 6966 2073 6b69 705f 6465 7365      if skip_dese
-00009550: 7269 616c 697a 6174 696f 6e3a 0a20 2020  rialization:.   
-00009560: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00009570: 7572 6e20 7365 6c66 2e72 6573 706f 6e73  urn self.respons
-00009580: 655f 636c 7328 0a20 2020 2020 2020 2020  e_cls(.         
-00009590: 2020 2020 2020 2020 2020 2072 6f75 6e64             round
-000095a0: 5f74 7269 705f 7469 6d65 3d72 6573 706f  _trip_time=respo
-000095b0: 6e73 652e 726f 756e 645f 7472 6970 5f74  nse.round_trip_t
-000095c0: 696d 652c 0a20 2020 2020 2020 2020 2020  ime,.           
-000095d0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-000095e0: 653d 7265 7370 6f6e 7365 2e68 7474 705f  e=response.http_
-000095f0: 7265 7370 6f6e 7365 2c0a 2020 2020 2020  response,.      
-00009600: 2020 2020 2020 2020 2020 2020 2020 626f                bo
-00009610: 6479 3d62 6f64 795f 6461 7461 2c0a 2020  dy=body_data,.  
-00009620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009630: 2020 6865 6164 6572 733d 7265 7370 6f6e    headers=respon
-00009640: 7365 2e68 7474 705f 7265 7370 6f6e 7365  se.http_response
-00009650: 2e68 6561 6465 7273 2c0a 2020 2020 2020  .headers,.      
-00009660: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00009670: 6174 7573 3d72 6573 706f 6e73 652e 6874  atus=response.ht
-00009680: 7470 5f72 6573 706f 6e73 652e 7374 6174  tp_response.stat
-00009690: 7573 0a20 2020 2020 2020 2020 2020 2020  us.             
-000096a0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-000096b0: 2020 2320 4578 6563 7574 6520 7661 6c69    # Execute vali
-000096c0: 6461 7469 6f6e 2061 6e64 2074 6872 6f77  dation and throw
-000096d0: 2061 7320 6120 7369 6465 2065 6666 6563   as a side effec
-000096e0: 7420 6966 2076 616c 6964 6174 696f 6e20  t if validation 
-000096f0: 6661 696c 730a 2020 2020 2020 2020 2020  fails.          
-00009700: 2020 626f 6479 5f73 6368 656d 612e 6672    body_schema.fr
-00009710: 6f6d 5f6f 7065 6e61 7069 5f64 6174 615f  om_openapi_data_
-00009720: 6f61 7067 280a 2020 2020 2020 2020 2020  oapg(.          
-00009730: 2020 2020 2020 626f 6479 5f64 6174 612c        body_data,
-00009740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009750: 205f 636f 6e66 6967 7572 6174 696f 6e3d   _configuration=
-00009760: 636f 6e66 6967 7572 6174 696f 6e0a 2020  configuration.  
-00009770: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00009780: 2020 2020 2020 2020 2320 5661 6c69 6461          # Valida
-00009790: 7469 6f6e 2070 6173 7365 642c 2073 6574  tion passed, set
-000097a0: 2064 6573 6572 6961 6c69 7a65 645f 626f   deserialized_bo
-000097b0: 6479 2074 6f20 706c 6169 6e20 6f6c 6420  dy to plain old 
-000097c0: 6465 7365 7269 616c 697a 6564 2064 6174  deserialized dat
-000097d0: 610a 2020 2020 2020 2020 2020 2020 6465  a.            de
-000097e0: 7365 7269 616c 697a 6564 5f62 6f64 7920  serialized_body 
-000097f0: 3d20 626f 6479 5f64 6174 610a 2020 2020  = body_data.    
-00009800: 2020 2020 656c 6966 2073 7472 6561 6d65      elif streame
-00009810: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
-00009820: 6573 706f 6e73 652e 6874 7470 5f72 6573  esponse.http_res
-00009830: 706f 6e73 652e 7265 6c65 6173 655f 636f  ponse.release_co
-00009840: 6e6e 2829 0a0a 2020 2020 2020 2020 7265  nn()..        re
-00009850: 7475 726e 2073 656c 662e 7265 7370 6f6e  turn self.respon
-00009860: 7365 5f63 6c73 280a 2020 2020 2020 2020  se_cls(.        
-00009870: 2020 2020 726f 756e 645f 7472 6970 5f74      round_trip_t
-00009880: 696d 653d 7265 7370 6f6e 7365 2e72 6f75  ime=response.rou
-00009890: 6e64 5f74 7269 705f 7469 6d65 2c0a 2020  nd_trip_time,.  
-000098a0: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
-000098b0: 7365 3d72 6573 706f 6e73 652e 6874 7470  se=response.http
-000098c0: 5f72 6573 706f 6e73 652c 0a20 2020 2020  _response,.     
-000098d0: 2020 2020 2020 2062 6f64 793d 6465 7365         body=dese
-000098e0: 7269 616c 697a 6564 5f62 6f64 792c 0a20  rialized_body,. 
-000098f0: 2020 2020 2020 2020 2020 2068 6561 6465             heade
-00009900: 7273 3d72 6573 706f 6e73 652e 6874 7470  rs=response.http
-00009910: 5f72 6573 706f 6e73 652e 6865 6164 6572  _response.header
-00009920: 732c 0a20 2020 2020 2020 2020 2020 2073  s,.            s
-00009930: 7461 7475 733d 7265 7370 6f6e 7365 2e68  tatus=response.h
-00009940: 7474 705f 7265 7370 6f6e 7365 2e73 7461  ttp_response.sta
-00009950: 7475 730a 2020 2020 2020 2020 290a 0a0a  tus.        )...
-00009960: 636c 6173 7320 4170 6943 6c69 656e 743a  class ApiClient:
-00009970: 0a20 2020 2022 2222 4765 6e65 7269 6320  .    """Generic 
-00009980: 4150 4920 636c 6965 6e74 2066 6f72 204f  API client for O
-00009990: 7065 6e41 5049 2063 6c69 656e 7420 6c69  penAPI client li
-000099a0: 6272 6172 7920 6275 696c 6473 2e0a 0a20  brary builds... 
-000099b0: 2020 204f 7065 6e41 5049 2067 656e 6572     OpenAPI gener
-000099c0: 6963 2041 5049 2063 6c69 656e 742e 2054  ic API client. T
-000099d0: 6869 7320 636c 6965 6e74 2068 616e 646c  his client handl
-000099e0: 6573 2074 6865 2063 6c69 656e 742d 0a20  es the client-. 
-000099f0: 2020 2073 6572 7665 7220 636f 6d6d 756e     server commun
-00009a00: 6963 6174 696f 6e2c 2061 6e64 2069 7320  ication, and is 
-00009a10: 696e 7661 7269 616e 7420 6163 726f 7373  invariant across
-00009a20: 2069 6d70 6c65 6d65 6e74 6174 696f 6e73   implementations
-00009a30: 2e20 5370 6563 6966 6963 7320 6f66 0a20  . Specifics of. 
-00009a40: 2020 2074 6865 206d 6574 686f 6473 2061     the methods a
-00009a50: 6e64 206d 6f64 656c 7320 666f 7220 6561  nd models for ea
-00009a60: 6368 2061 7070 6c69 6361 7469 6f6e 2061  ch application a
-00009a70: 7265 2067 656e 6572 6174 6564 2066 726f  re generated fro
-00009a80: 6d20 7468 6520 4f70 656e 4150 490a 2020  m the OpenAPI.  
-00009a90: 2020 7465 6d70 6c61 7465 732e 0a0a 2020    templates...  
-00009aa0: 2020 5468 6973 2063 6c61 7373 2069 7320    This class is 
-00009ab0: 6175 746f 2067 656e 6572 6174 6564 2062  auto generated b
-00009ac0: 7920 4b6f 6e66 6967 2028 6874 7470 733a  y Konfig (https:
-00009ad0: 2f2f 6b6f 6e66 6967 7468 6973 2e63 6f6d  //konfigthis.com
-00009ae0: 290a 0a20 2020 203a 7061 7261 6d20 636f  )..    :param co
-00009af0: 6e66 6967 7572 6174 696f 6e3a 202e 436f  nfiguration: .Co
-00009b00: 6e66 6967 7572 6174 696f 6e20 6f62 6a65  nfiguration obje
-00009b10: 6374 2066 6f72 2074 6869 7320 636c 6965  ct for this clie
-00009b20: 6e74 0a20 2020 203a 7061 7261 6d20 6865  nt.    :param he
-00009b30: 6164 6572 5f6e 616d 653a 2061 2068 6561  ader_name: a hea
-00009b40: 6465 7220 746f 2070 6173 7320 7768 656e  der to pass when
-00009b50: 206d 616b 696e 6720 6361 6c6c 7320 746f   making calls to
-00009b60: 2074 6865 2041 5049 2e0a 2020 2020 3a70   the API..    :p
-00009b70: 6172 616d 2068 6561 6465 725f 7661 6c75  aram header_valu
-00009b80: 653a 2061 2068 6561 6465 7220 7661 6c75  e: a header valu
-00009b90: 6520 746f 2070 6173 7320 7768 656e 206d  e to pass when m
-00009ba0: 616b 696e 6720 6361 6c6c 7320 746f 0a20  aking calls to. 
-00009bb0: 2020 2020 2020 2074 6865 2041 5049 2e0a         the API..
-00009bc0: 2020 2020 3a70 6172 616d 2063 6f6f 6b69      :param cooki
-00009bd0: 653a 2061 2063 6f6f 6b69 6520 746f 2069  e: a cookie to i
-00009be0: 6e63 6c75 6465 2069 6e20 7468 6520 6865  nclude in the he
-00009bf0: 6164 6572 2077 6865 6e20 6d61 6b69 6e67  ader when making
-00009c00: 2063 616c 6c73 0a20 2020 2020 2020 2074   calls.        t
-00009c10: 6f20 7468 6520 4150 490a 2020 2020 3a70  o the API.    :p
-00009c20: 6172 616d 2070 6f6f 6c5f 7468 7265 6164  aram pool_thread
-00009c30: 733a 2054 6865 206e 756d 6265 7220 6f66  s: The number of
-00009c40: 2074 6872 6561 6473 2074 6f20 7573 6520   threads to use 
-00009c50: 666f 7220 6173 796e 6320 7265 7175 6573  for async reques
-00009c60: 7473 0a20 2020 2020 2020 2074 6f20 7468  ts.        to th
-00009c70: 6520 4150 492e 204d 6f72 6520 7468 7265  e API. More thre
-00009c80: 6164 7320 6d65 616e 7320 6d6f 7265 2063  ads means more c
-00009c90: 6f6e 6375 7272 656e 7420 4150 4920 7265  oncurrent API re
-00009ca0: 7175 6573 7473 2e0a 2020 2020 2222 220a  quests..    """.
-00009cb0: 0a20 2020 205f 706f 6f6c 203d 204e 6f6e  .    _pool = Non
-00009cc0: 650a 0a20 2020 2064 6566 205f 5f69 6e69  e..    def __ini
-00009cd0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00009ce0: 662c 0a20 2020 2020 2020 2063 6f6e 6669  f,.        confi
-00009cf0: 6775 7261 7469 6f6e 3a20 7479 7069 6e67  guration: typing
-00009d00: 2e4f 7074 696f 6e61 6c5b 436f 6e66 6967  .Optional[Config
-00009d10: 7572 6174 696f 6e5d 203d 204e 6f6e 652c  uration] = None,
-00009d20: 0a20 2020 2020 2020 2068 6561 6465 725f  .        header_
-00009d30: 6e61 6d65 3a20 7479 7069 6e67 2e4f 7074  name: typing.Opt
-00009d40: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00009d50: 652c 0a20 2020 2020 2020 2068 6561 6465  e,.        heade
-00009d60: 725f 7661 6c75 653a 2074 7970 696e 672e  r_value: typing.
-00009d70: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00009d80: 4e6f 6e65 2c0a 2020 2020 2020 2020 636f  None,.        co
-00009d90: 6f6b 6965 3a20 7479 7069 6e67 2e4f 7074  okie: typing.Opt
-00009da0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00009db0: 652c 0a20 2020 2020 2020 2070 6f6f 6c5f  e,.        pool_
-00009dc0: 7468 7265 6164 733a 2069 6e74 203d 2031  threads: int = 1
-00009dd0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00009de0: 6966 2063 6f6e 6669 6775 7261 7469 6f6e  if configuration
-00009df0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00009e00: 2020 2020 2020 636f 6e66 6967 7572 6174        configurat
-00009e10: 696f 6e20 3d20 436f 6e66 6967 7572 6174  ion = Configurat
-00009e20: 696f 6e28 290a 2020 2020 2020 2020 7365  ion().        se
-00009e30: 6c66 2e63 6f6e 6669 6775 7261 7469 6f6e  lf.configuration
-00009e40: 203d 2063 6f6e 6669 6775 7261 7469 6f6e   = configuration
-00009e50: 0a20 2020 2020 2020 2073 656c 662e 706f  .        self.po
-00009e60: 6f6c 5f74 6872 6561 6473 203d 2070 6f6f  ol_threads = poo
-00009e70: 6c5f 7468 7265 6164 730a 0a20 2020 2020  l_threads..     
-00009e80: 2020 2073 656c 662e 7265 7374 5f63 6c69     self.rest_cli
-00009e90: 656e 7420 3d20 7265 7374 2e52 4553 5443  ent = rest.RESTC
-00009ea0: 6c69 656e 744f 626a 6563 7428 636f 6e66  lientObject(conf
-00009eb0: 6967 7572 6174 696f 6e29 0a20 2020 2020  iguration).     
-00009ec0: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
-00009ed0: 6865 6164 6572 7320 3d20 4854 5450 4865  headers = HTTPHe
-00009ee0: 6164 6572 4469 6374 2829 0a20 2020 2020  aderDict().     
-00009ef0: 2020 2069 6620 6865 6164 6572 5f6e 616d     if header_nam
-00009f00: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00009f10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009f20: 6465 6661 756c 745f 6865 6164 6572 735b  default_headers[
-00009f30: 6865 6164 6572 5f6e 616d 655d 203d 2068  header_name] = h
-00009f40: 6561 6465 725f 7661 6c75 650a 2020 2020  eader_value.    
-00009f50: 2020 2020 7365 6c66 2e63 6f6f 6b69 6520      self.cookie 
-00009f60: 3d20 636f 6f6b 6965 0a20 2020 2020 2020  = cookie.       
-00009f70: 2023 2053 6574 2064 6566 6175 6c74 2055   # Set default U
-00009f80: 7365 722d 4167 656e 742e 0a20 2020 2020  ser-Agent..     
-00009f90: 2020 2073 656c 662e 7573 6572 5f61 6765     self.user_age
-00009fa0: 6e74 203d 2027 4b6f 6e66 6967 2f32 2e31  nt = 'Konfig/2.1
-00009fb0: 2e30 2f70 7974 686f 6e27 0a0a 2020 2020  .0/python'..    
-00009fc0: 6465 6620 5f5f 656e 7465 725f 5f28 7365  def __enter__(se
-00009fd0: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-00009fe0: 7572 6e20 7365 6c66 0a0a 2020 2020 6465  urn self..    de
-00009ff0: 6620 5f5f 6578 6974 5f5f 2873 656c 662c  f __exit__(self,
-0000a000: 2065 7863 5f74 7970 652c 2065 7863 5f76   exc_type, exc_v
-0000a010: 616c 7565 2c20 7472 6163 6562 6163 6b29  alue, traceback)
-0000a020: 3a0a 2020 2020 2020 2020 7365 6c66 2e63  :.        self.c
-0000a030: 6c6f 7365 2829 0a0a 2020 2020 6465 6620  lose()..    def 
-0000a040: 636c 6f73 6528 7365 6c66 293a 0a20 2020  close(self):.   
-0000a050: 2020 2020 2069 6620 7365 6c66 2e5f 706f       if self._po
-0000a060: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
-0000a070: 7365 6c66 2e5f 706f 6f6c 2e63 6c6f 7365  self._pool.close
-0000a080: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-0000a090: 656c 662e 5f70 6f6f 6c2e 6a6f 696e 2829  elf._pool.join()
-0000a0a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000a0b0: 662e 5f70 6f6f 6c20 3d20 4e6f 6e65 0a20  f._pool = None. 
-0000a0c0: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
-0000a0d0: 7361 7474 7228 6174 6578 6974 2c20 2775  sattr(atexit, 'u
-0000a0e0: 6e72 6567 6973 7465 7227 293a 0a20 2020  nregister'):.   
-0000a0f0: 2020 2020 2020 2020 2020 2020 2061 7465               ate
-0000a100: 7869 742e 756e 7265 6769 7374 6572 2873  xit.unregister(s
-0000a110: 656c 662e 636c 6f73 6529 0a0a 2020 2020  elf.close)..    
-0000a120: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000a130: 6620 706f 6f6c 2873 656c 6629 3a0a 2020  f pool(self):.  
-0000a140: 2020 2020 2020 2222 2243 7265 6174 6520        """Create 
-0000a150: 7468 7265 6164 2070 6f6f 6c20 6f6e 2066  thread pool on f
-0000a160: 6972 7374 2072 6571 7565 7374 0a20 2020  irst request.   
-0000a170: 2020 2020 2020 6176 6f69 6473 2069 6e73        avoids ins
-0000a180: 7461 6e74 6961 7469 6e67 2075 6e75 7365  tantiating unuse
-0000a190: 6420 7468 7265 6164 706f 6f6c 2066 6f72  d threadpool for
-0000a1a0: 2062 6c6f 636b 696e 6720 636c 6965 6e74   blocking client
-0000a1b0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-0000a1c0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-0000a1d0: 706f 6f6c 2069 7320 4e6f 6e65 3a0a 2020  pool is None:.  
-0000a1e0: 2020 2020 2020 2020 2020 6174 6578 6974            atexit
-0000a1f0: 2e72 6567 6973 7465 7228 7365 6c66 2e63  .register(self.c
-0000a200: 6c6f 7365 290a 2020 2020 2020 2020 2020  lose).          
-0000a210: 2020 7365 6c66 2e5f 706f 6f6c 203d 2054    self._pool = T
-0000a220: 6872 6561 6450 6f6f 6c28 7365 6c66 2e70  hreadPool(self.p
-0000a230: 6f6f 6c5f 7468 7265 6164 7329 0a20 2020  ool_threads).   
-0000a240: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000a250: 2e5f 706f 6f6c 0a0a 2020 2020 4070 726f  ._pool..    @pro
-0000a260: 7065 7274 790a 2020 2020 6465 6620 7573  perty.    def us
-0000a270: 6572 5f61 6765 6e74 2873 656c 6629 3a0a  er_agent(self):.
-0000a280: 2020 2020 2020 2020 2222 2255 7365 7220          """User 
-0000a290: 6167 656e 7420 666f 7220 7468 6973 2041  agent for this A
-0000a2a0: 5049 2063 6c69 656e 7422 2222 0a20 2020  PI client""".   
-0000a2b0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000a2c0: 2e64 6566 6175 6c74 5f68 6561 6465 7273  .default_headers
-0000a2d0: 5b27 5573 6572 2d41 6765 6e74 275d 0a0a  ['User-Agent']..
-0000a2e0: 2020 2020 4075 7365 725f 6167 656e 742e      @user_agent.
-0000a2f0: 7365 7474 6572 0a20 2020 2064 6566 2075  setter.    def u
-0000a300: 7365 725f 6167 656e 7428 7365 6c66 2c20  ser_agent(self, 
-0000a310: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
-0000a320: 7365 6c66 2e64 6566 6175 6c74 5f68 6561  self.default_hea
-0000a330: 6465 7273 5b27 5573 6572 2d41 6765 6e74  ders['User-Agent
-0000a340: 275d 203d 2076 616c 7565 0a0a 2020 2020  '] = value..    
-0000a350: 6465 6620 7365 745f 6465 6661 756c 745f  def set_default_
-0000a360: 6865 6164 6572 2873 656c 662c 2068 6561  header(self, hea
-0000a370: 6465 725f 6e61 6d65 2c20 6865 6164 6572  der_name, header
-0000a380: 5f76 616c 7565 293a 0a20 2020 2020 2020  _value):.       
-0000a390: 2073 656c 662e 6465 6661 756c 745f 6865   self.default_he
-0000a3a0: 6164 6572 735b 6865 6164 6572 5f6e 616d  aders[header_nam
-0000a3b0: 655d 203d 2068 6561 6465 725f 7661 6c75  e] = header_valu
-0000a3c0: 650a 0a20 2020 2064 6566 205f 5f63 616c  e..    def __cal
-0000a3d0: 6c5f 6170 6928 0a20 2020 2020 2020 2073  l_api(.        s
-0000a3e0: 656c 662c 0a20 2020 2020 2020 2072 6573  elf,.        res
-0000a3f0: 6f75 7263 655f 7061 7468 3a20 7374 722c  ource_path: str,
-0000a400: 0a20 2020 2020 2020 206d 6574 686f 643a  .        method:
-0000a410: 2073 7472 2c0a 2020 2020 2020 2020 6865   str,.        he
-0000a420: 6164 6572 733a 2074 7970 696e 672e 4f70  aders: typing.Op
-0000a430: 7469 6f6e 616c 5b48 5454 5048 6561 6465  tional[HTTPHeade
-0000a440: 7244 6963 745d 203d 204e 6f6e 652c 0a20  rDict] = None,. 
-0000a450: 2020 2020 2020 2073 6572 6961 6c69 7a65         serialize
-0000a460: 645f 626f 6479 3a20 7479 7069 6e67 2e4f  d_body: typing.O
-0000a470: 7074 696f 6e61 6c5b 7479 7069 6e67 2e55  ptional[typing.U
-0000a480: 6e69 6f6e 5b73 7472 2c20 6279 7465 735d  nion[str, bytes]
-0000a490: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000a4a0: 2020 626f 6479 3a20 7479 7069 6e67 2e41    body: typing.A
-0000a4b0: 6e79 203d 204e 6f6e 652c 0a20 2020 2020  ny = None,.     
-0000a4c0: 2020 2066 6965 6c64 733a 2074 7970 696e     fields: typin
-0000a4d0: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-0000a4e0: 672e 5475 706c 655b 7479 7069 6e67 2e54  g.Tuple[typing.T
-0000a4f0: 7570 6c65 5b73 7472 2c20 7374 725d 2c20  uple[str, str], 
-0000a500: 2e2e 2e5d 5d20 3d20 4e6f 6e65 2c0a 2020  ...]] = None,.  
-0000a510: 2020 2020 2020 6175 7468 5f73 6574 7469        auth_setti
-0000a520: 6e67 733a 2074 7970 696e 672e 4f70 7469  ngs: typing.Opti
-0000a530: 6f6e 616c 5b74 7970 696e 672e 4c69 7374  onal[typing.List
-0000a540: 5b73 7472 5d5d 203d 204e 6f6e 652c 0a20  [str]] = None,. 
-0000a550: 2020 2020 2020 2073 7472 6561 6d3a 2062         stream: b
-0000a560: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-0000a570: 2020 2020 2074 696d 656f 7574 3a20 7479       timeout: ty
-0000a580: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-0000a590: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
-0000a5a0: 7479 7069 6e67 2e54 7570 6c65 5d5d 203d  typing.Tuple]] =
-0000a5b0: 204e 6f6e 652c 0a20 2020 2020 2020 2068   None,.        h
-0000a5c0: 6f73 743a 2074 7970 696e 672e 4f70 7469  ost: typing.Opti
-0000a5d0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-0000a5e0: 2c0a 2020 2020 2020 2020 7072 6566 6978  ,.        prefix
-0000a5f0: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-0000a600: 746f 723a 2050 7265 6669 7853 6570 6172  tor: PrefixSepar
-0000a610: 6174 6f72 4974 6572 6174 6f72 203d 204e  atorIterator = N
-0000a620: 6f6e 652c 0a20 2020 2020 2020 205f 7265  one,.        _re
-0000a630: 7472 795f 6f61 7574 6820 3d20 5472 7565  try_oauth = True
-0000a640: 2c0a 2020 2020 2920 2d3e 2052 6573 706f  ,.    ) -> Respo
-0000a650: 6e73 6557 7261 7070 6572 3a0a 0a20 2020  nseWrapper:..   
-0000a660: 2020 2020 2072 6571 7565 7374 5f62 6566       request_bef
-0000a670: 6f72 655f 686f 6f6b 280a 2020 2020 2020  ore_hook(.      
-0000a680: 2020 2020 2020 7265 736f 7572 6365 5f70        resource_p
-0000a690: 6174 683d 7265 736f 7572 6365 5f70 6174  ath=resource_pat
-0000a6a0: 682c 0a20 2020 2020 2020 2020 2020 206d  h,.            m
-0000a6b0: 6574 686f 643d 6d65 7468 6f64 2c0a 2020  ethod=method,.  
-0000a6c0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-0000a6d0: 7572 6174 696f 6e3d 7365 6c66 2e63 6f6e  uration=self.con
-0000a6e0: 6669 6775 7261 7469 6f6e 2c0a 2020 2020  figuration,.    
-0000a6f0: 2020 2020 2020 2020 626f 6479 3d62 6f64          body=bod
-0000a700: 792c 0a20 2020 2020 2020 2020 2020 2066  y,.            f
-0000a710: 6965 6c64 733d 6669 656c 6473 2c0a 2020  ields=fields,.  
-0000a720: 2020 2020 2020 2020 2020 6175 7468 5f73            auth_s
-0000a730: 6574 7469 6e67 733d 6175 7468 5f73 6574  ettings=auth_set
-0000a740: 7469 6e67 732c 0a20 2020 2020 2020 2020  tings,.         
-0000a750: 2020 2068 6561 6465 7273 3d68 6561 6465     headers=heade
-0000a760: 7273 2c0a 2020 2020 2020 2020 290a 0a20  rs,.        ).. 
-0000a770: 2020 2020 2020 2023 2068 6561 6465 7220         # header 
-0000a780: 7061 7261 6d65 7465 7273 0a20 2020 2020  parameters.     
-0000a790: 2020 2075 7365 645f 6865 6164 6572 7320     used_headers 
-0000a7a0: 3d20 4854 5450 4865 6164 6572 4469 6374  = HTTPHeaderDict
-0000a7b0: 2873 656c 662e 6465 6661 756c 745f 6865  (self.default_he
-0000a7c0: 6164 6572 7329 0a20 2020 2020 2020 2069  aders).        i
-0000a7d0: 6620 7365 6c66 2e63 6f6f 6b69 653a 0a20  f self.cookie:. 
-0000a7e0: 2020 2020 2020 2020 2020 2068 6561 6465             heade
-0000a7f0: 7273 5b27 436f 6f6b 6965 275d 203d 2073  rs['Cookie'] = s
-0000a800: 656c 662e 636f 6f6b 6965 0a0a 2020 2020  elf.cookie..    
-0000a810: 2020 2020 2320 6175 7468 2073 6574 7469      # auth setti
-0000a820: 6e67 0a20 2020 2020 2020 2072 6573 6f75  ng.        resou
-0000a830: 7263 655f 7061 7468 203d 2073 656c 662e  rce_path = self.
-0000a840: 7570 6461 7465 5f70 6172 616d 735f 666f  update_params_fo
-0000a850: 725f 6175 7468 280a 2020 2020 2020 2020  r_auth(.        
-0000a860: 2020 2020 7573 6564 5f68 6561 6465 7273      used_headers
-0000a870: 2c0a 2020 2020 2020 2020 2020 2020 6175  ,.            au
-0000a880: 7468 5f73 6574 7469 6e67 732c 0a20 2020  th_settings,.   
-0000a890: 2020 2020 2020 2020 2072 6573 6f75 7263           resourc
-0000a8a0: 655f 7061 7468 2c0a 2020 2020 2020 2020  e_path,.        
-0000a8b0: 2020 2020 6d65 7468 6f64 2c0a 2020 2020      method,.    
-0000a8c0: 2020 2020 2020 2020 626f 6479 2c0a 2020          body,.  
-0000a8d0: 2020 2020 2020 2020 2020 7072 6566 6978            prefix
-0000a8e0: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-0000a8f0: 746f 720a 2020 2020 2020 2020 290a 0a20  tor.        ).. 
-0000a900: 2020 2020 2020 2023 206d 7573 7420 6861         # must ha
-0000a910: 7070 656e 2061 6674 6572 2063 6f6f 6b69  ppen after cooki
-0000a920: 6520 7365 7474 696e 6720 616e 6420 6175  e setting and au
-0000a930: 7468 2073 6574 7469 6e67 2069 6e20 6361  th setting in ca
-0000a940: 7365 2075 7365 7220 6973 206f 7665 7272  se user is overr
-0000a950: 6964 696e 6720 7468 6f73 650a 2020 2020  iding those.    
-0000a960: 2020 2020 6966 2068 6561 6465 7273 3a0a      if headers:.
-0000a970: 2020 2020 2020 2020 2020 2020 7573 6564              used
-0000a980: 5f68 6561 6465 7273 2e75 7064 6174 6528  _headers.update(
-0000a990: 6865 6164 6572 7329 0a0a 2020 2020 2020  headers)..      
-0000a9a0: 2020 2320 7265 7175 6573 7420 7572 6c0a    # request url.
-0000a9b0: 2020 2020 2020 2020 6966 2068 6f73 7420          if host 
-0000a9c0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0000a9d0: 2020 2020 2075 726c 203d 2073 656c 662e       url = self.
-0000a9e0: 636f 6e66 6967 7572 6174 696f 6e2e 686f  configuration.ho
-0000a9f0: 7374 202b 2072 6573 6f75 7263 655f 7061  st + resource_pa
-0000aa00: 7468 0a20 2020 2020 2020 2065 6c73 653a  th.        else:
-0000aa10: 0a20 2020 2020 2020 2020 2020 2023 2075  .            # u
-0000aa20: 7365 2073 6572 7665 722f 686f 7374 2064  se server/host d
-0000aa30: 6566 696e 6564 2069 6e20 7061 7468 206f  efined in path o
-0000aa40: 7220 6f70 6572 6174 696f 6e20 696e 7374  r operation inst
-0000aa50: 6561 640a 2020 2020 2020 2020 2020 2020  ead.            
-0000aa60: 7572 6c20 3d20 686f 7374 202b 2072 6573  url = host + res
-0000aa70: 6f75 7263 655f 7061 7468 0a0a 2020 2020  ource_path..    
-0000aa80: 2020 2020 7265 7175 6573 745f 6166 7465      request_afte
-0000aa90: 725f 686f 6f6b 280a 2020 2020 2020 2020  r_hook(.        
-0000aaa0: 2020 2020 7265 736f 7572 6365 5f70 6174      resource_pat
-0000aab0: 683d 7265 736f 7572 6365 5f70 6174 682c  h=resource_path,
-0000aac0: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
-0000aad0: 686f 643d 6d65 7468 6f64 2c0a 2020 2020  hod=method,.    
-0000aae0: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
-0000aaf0: 6174 696f 6e3d 7365 6c66 2e63 6f6e 6669  ation=self.confi
-0000ab00: 6775 7261 7469 6f6e 2c0a 2020 2020 2020  guration,.      
-0000ab10: 2020 2020 2020 626f 6479 3d62 6f64 792c        body=body,
-0000ab20: 0a20 2020 2020 2020 2020 2020 2066 6965  .            fie
-0000ab30: 6c64 733d 6669 656c 6473 2c0a 2020 2020  lds=fields,.    
-0000ab40: 2020 2020 2020 2020 6175 7468 5f73 6574          auth_set
-0000ab50: 7469 6e67 733d 6175 7468 5f73 6574 7469  tings=auth_setti
-0000ab60: 6e67 732c 0a20 2020 2020 2020 2020 2020  ngs,.           
-0000ab70: 2068 6561 6465 7273 3d75 7365 645f 6865   headers=used_he
-0000ab80: 6164 6572 732c 0a20 2020 2020 2020 2029  aders,.        )
-0000ab90: 0a0a 2020 2020 2020 2020 2320 7065 7266  ..        # perf
-0000aba0: 6f72 6d20 7265 7175 6573 7420 616e 6420  orm request and 
-0000abb0: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
-0000abc0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-0000abd0: 203d 2073 656c 662e 7265 7175 6573 7428   = self.request(
-0000abe0: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
-0000abf0: 686f 642c 0a20 2020 2020 2020 2020 2020  hod,.           
-0000ac00: 2075 726c 2c0a 2020 2020 2020 2020 2020   url,.          
-0000ac10: 2020 6865 6164 6572 733d 7573 6564 5f68    headers=used_h
-0000ac20: 6561 6465 7273 2c0a 2020 2020 2020 2020  eaders,.        
-0000ac30: 2020 2020 6669 656c 6473 3d66 6965 6c64      fields=field
-0000ac40: 732c 0a20 2020 2020 2020 2020 2020 2062  s,.            b
-0000ac50: 6f64 793d 7365 7269 616c 697a 6564 5f62  ody=serialized_b
-0000ac60: 6f64 792c 0a20 2020 2020 2020 2020 2020  ody,.           
-0000ac70: 2073 7472 6561 6d3d 7374 7265 616d 2c0a   stream=stream,.
-0000ac80: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-0000ac90: 6f75 743d 7469 6d65 6f75 742c 0a20 2020  out=timeout,.   
-0000aca0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000acb0: 2320 4c69 6b65 6c79 2074 6861 7420 7374  # Likely that st
-0000acc0: 6174 7573 2063 6f64 6573 2034 3031 206f  atus codes 401 o
-0000acd0: 7220 3430 3320 696e 6469 6361 7465 2074  r 403 indicate t
-0000ace0: 6865 206e 6565 6420 746f 2072 6566 7265  he need to refre
-0000acf0: 7368 2061 6363 6573 7320 746f 6b65 6e20  sh access token 
-0000ad00: 666f 7220 4f41 7574 680a 2020 2020 2020  for OAuth.      
-0000ad10: 2020 6966 2072 6573 706f 6e73 652e 6874    if response.ht
-0000ad20: 7470 5f72 6573 706f 6e73 652e 7374 6174  tp_response.stat
-0000ad30: 7573 203d 3d20 3430 3120 6f72 2072 6573  us == 401 or res
-0000ad40: 706f 6e73 652e 6874 7470 5f72 6573 706f  ponse.http_respo
-0000ad50: 6e73 652e 7374 6174 7573 203d 3d20 3430  nse.status == 40
-0000ad60: 333a 0a20 2020 2020 2020 2020 2020 2069  3:.            i
-0000ad70: 6620 7365 6c66 2e63 6f6e 6669 6775 7261  f self.configura
-0000ad80: 7469 6f6e 2e6f 6175 7468 2069 7320 6e6f  tion.oauth is no
-0000ad90: 7420 4e6f 6e65 2061 6e64 205f 7265 7472  t None and _retr
-0000ada0: 795f 6f61 7574 683a 0a20 2020 2020 2020  y_oauth:.       
-0000adb0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-0000adc0: 6e66 6967 7572 6174 696f 6e2e 6f61 7574  nfiguration.oaut
-0000add0: 682e 7265 6672 6573 685f 6163 6365 7373  h.refresh_access
-0000ade0: 5f74 6f6b 656e 2829 0a20 2020 2020 2020  _token().       
-0000adf0: 2020 2020 2020 2020 2073 656c 662e 5f5f           self.__
-0000ae00: 6361 6c6c 5f61 7069 280a 2020 2020 2020  call_api(.      
-0000ae10: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000ae20: 736f 7572 6365 5f70 6174 683d 7265 736f  source_path=reso
-0000ae30: 7572 6365 5f70 6174 682c 0a20 2020 2020  urce_path,.     
-0000ae40: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000ae50: 6574 686f 643d 6d65 7468 6f64 2c0a 2020  ethod=method,.  
-0000ae60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae70: 2020 6865 6164 6572 733d 6865 6164 6572    headers=header
-0000ae80: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000ae90: 2020 2020 2020 2073 6572 6961 6c69 7a65         serialize
-0000aea0: 645f 626f 6479 3d73 6572 6961 6c69 7a65  d_body=serialize
-0000aeb0: 645f 626f 6479 2c0a 2020 2020 2020 2020  d_body,.        
-0000aec0: 2020 2020 2020 2020 2020 2020 626f 6479              body
-0000aed0: 3d62 6f64 792c 0a20 2020 2020 2020 2020  =body,.         
-0000aee0: 2020 2020 2020 2020 2020 2066 6965 6c64             field
-0000aef0: 733d 6669 656c 6473 2c0a 2020 2020 2020  s=fields,.      
-0000af00: 2020 2020 2020 2020 2020 2020 2020 6175                au
-0000af10: 7468 5f73 6574 7469 6e67 733d 6175 7468  th_settings=auth
-0000af20: 5f73 6574 7469 6e67 732c 0a20 2020 2020  _settings,.     
-0000af30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000af40: 7472 6561 6d3d 7374 7265 616d 2c0a 2020  tream=stream,.  
-0000af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af60: 2020 7469 6d65 6f75 743d 7469 6d65 6f75    timeout=timeou
-0000af70: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-0000af80: 2020 2020 2020 2068 6f73 743d 686f 7374         host=host
-0000af90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000afa0: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
-0000afb0: 6172 6174 6f72 5f69 7465 7261 746f 723d  arator_iterator=
-0000afc0: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
-0000afd0: 5f69 7465 7261 746f 722c 0a20 2020 2020  _iterator,.     
-0000afe0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-0000aff0: 7265 7472 795f 6f61 7574 683d 4661 6c73  retry_oauth=Fals
-0000b000: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000b010: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
-0000b020: 7475 726e 2072 6573 706f 6e73 650a 0a20  turn response.. 
-0000b030: 2020 2064 6566 2063 616c 6c5f 6170 6928     def call_api(
-0000b040: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0000b050: 2020 2020 2020 2072 6573 6f75 7263 655f         resource_
-0000b060: 7061 7468 3a20 7374 722c 0a20 2020 2020  path: str,.     
-0000b070: 2020 206d 6574 686f 643a 2073 7472 2c0a     method: str,.
-0000b080: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
-0000b090: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0000b0a0: 5b48 5454 5048 6561 6465 7244 6963 745d  [HTTPHeaderDict]
-0000b0b0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000b0c0: 2073 6572 6961 6c69 7a65 645f 626f 6479   serialized_body
-0000b0d0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0000b0e0: 6c5b 7479 7069 6e67 2e55 6e69 6f6e 5b73  l[typing.Union[s
-0000b0f0: 7472 2c20 6279 7465 735d 5d20 3d20 4e6f  tr, bytes]] = No
-0000b100: 6e65 2c0a 2020 2020 2020 2020 626f 6479  ne,.        body
-0000b110: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
-0000b120: 6f6e 652c 0a20 2020 2020 2020 2066 6965  one,.        fie
-0000b130: 6c64 733a 2074 7970 696e 672e 4f70 7469  lds: typing.Opti
-0000b140: 6f6e 616c 5b74 7970 696e 672e 5475 706c  onal[typing.Tupl
-0000b150: 655b 7479 7069 6e67 2e54 7570 6c65 5b73  e[typing.Tuple[s
-0000b160: 7472 2c20 7374 725d 2c20 2e2e 2e5d 5d20  tr, str], ...]] 
-0000b170: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000b180: 6175 7468 5f73 6574 7469 6e67 733a 2074  auth_settings: t
-0000b190: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
-0000b1a0: 7970 696e 672e 4c69 7374 5b73 7472 5d5d  yping.List[str]]
-0000b1b0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000b1c0: 2061 7379 6e63 5f72 6571 3a20 7479 7069   async_req: typi
-0000b1d0: 6e67 2e4f 7074 696f 6e61 6c5b 626f 6f6c  ng.Optional[bool
-0000b1e0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000b1f0: 2020 7374 7265 616d 3a20 626f 6f6c 203d    stream: bool =
-0000b200: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-0000b210: 7469 6d65 6f75 743a 2074 7970 696e 672e  timeout: typing.
-0000b220: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-0000b230: 556e 696f 6e5b 696e 742c 2074 7970 696e  Union[int, typin
-0000b240: 672e 5475 706c 655d 5d20 3d20 4e6f 6e65  g.Tuple]] = None
-0000b250: 2c0a 2020 2020 2020 2020 686f 7374 3a20  ,.        host: 
-0000b260: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-0000b270: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-0000b280: 2020 2020 2070 7265 6669 785f 7365 7061       prefix_sepa
-0000b290: 7261 746f 725f 6974 6572 6174 6f72 3a20  rator_iterator: 
-0000b2a0: 5072 6566 6978 5365 7061 7261 746f 7249  PrefixSeparatorI
-0000b2b0: 7465 7261 746f 7220 3d20 4e6f 6e65 2c0a  terator = None,.
-0000b2c0: 2020 2020 2920 2d3e 2052 6573 706f 6e73      ) -> Respons
-0000b2d0: 6557 7261 7070 6572 3a0a 2020 2020 2020  eWrapper:.      
-0000b2e0: 2020 2222 224d 616b 6573 2074 6865 2048    """Makes the H
-0000b2f0: 5454 5020 7265 7175 6573 7420 2873 796e  TTP request (syn
-0000b300: 6368 726f 6e6f 7573 2920 616e 6420 7265  chronous) and re
-0000b310: 7475 726e 7320 6465 7365 7269 616c 697a  turns deserializ
-0000b320: 6564 2064 6174 612e 0a0a 2020 2020 2020  ed data...      
-0000b330: 2020 546f 206d 616b 6520 616e 2061 7379    To make an asy
-0000b340: 6e63 5f72 6571 2072 6571 7565 7374 2c20  nc_req request, 
-0000b350: 7365 7420 7468 6520 6173 796e 635f 7265  set the async_re
-0000b360: 7120 7061 7261 6d65 7465 722e 0a0a 2020  q parameter...  
-0000b370: 2020 2020 2020 3a70 6172 616d 2072 6573        :param res
-0000b380: 6f75 7263 655f 7061 7468 3a20 5061 7468  ource_path: Path
-0000b390: 2074 6f20 6d65 7468 6f64 2065 6e64 706f   to method endpo
-0000b3a0: 696e 742e 0a20 2020 2020 2020 203a 7061  int..        :pa
-0000b3b0: 7261 6d20 6d65 7468 6f64 3a20 4d65 7468  ram method: Meth
-0000b3c0: 6f64 2074 6f20 6361 6c6c 2e0a 2020 2020  od to call..    
-0000b3d0: 2020 2020 3a70 6172 616d 2068 6561 6465      :param heade
-0000b3e0: 7273 3a20 4865 6164 6572 2070 6172 616d  rs: Header param
-0000b3f0: 6574 6572 7320 746f 2062 650a 2020 2020  eters to be.    
-0000b400: 2020 2020 2020 2020 706c 6163 6564 2069          placed i
-0000b410: 6e20 7468 6520 7265 7175 6573 7420 6865  n the request he
-0000b420: 6164 6572 2e0a 2020 2020 2020 2020 3a70  ader..        :p
-0000b430: 6172 616d 2062 6f64 793a 2052 6571 7565  aram body: Reque
-0000b440: 7374 2062 6f64 792e 0a20 2020 2020 2020  st body..       
-0000b450: 203a 7061 7261 6d20 6669 656c 6473 3a20   :param fields: 
-0000b460: 5265 7175 6573 7420 706f 7374 2066 6f72  Request post for
-0000b470: 6d20 7061 7261 6d65 7465 7273 2c0a 2020  m parameters,.  
-0000b480: 2020 2020 2020 2020 2020 666f 7220 6061            for `a
-0000b490: 7070 6c69 6361 7469 6f6e 2f78 2d77 7777  pplication/x-www
-0000b4a0: 2d66 6f72 6d2d 7572 6c65 6e63 6f64 6564  -form-urlencoded
-0000b4b0: 602c 2060 6d75 6c74 6970 6172 742f 666f  `, `multipart/fo
-0000b4c0: 726d 2d64 6174 6160 2e0a 2020 2020 2020  rm-data`..      
-0000b4d0: 2020 3a70 6172 616d 2061 7574 685f 7365    :param auth_se
-0000b4e0: 7474 696e 6773 3a20 4175 7468 2053 6574  ttings: Auth Set
-0000b4f0: 7469 6e67 7320 6e61 6d65 7320 666f 7220  tings names for 
-0000b500: 7468 6520 7265 7175 6573 742e 0a20 2020  the request..   
-0000b510: 2020 2020 203a 7061 7261 6d20 6173 796e       :param asyn
-0000b520: 635f 7265 713a 2065 7865 6375 7465 2072  c_req: execute r
-0000b530: 6571 7565 7374 2061 7379 6e63 6872 6f6e  equest asynchron
-0000b540: 6f75 736c 790a 2020 2020 2020 2020 3a74  ously.        :t
-0000b550: 7970 6520 6173 796e 635f 7265 713a 2062  ype async_req: b
-0000b560: 6f6f 6c2c 206f 7074 696f 6e61 6c20 544f  ool, optional TO
-0000b570: 444f 2072 656d 6f76 652c 2075 6e75 7365  DO remove, unuse
-0000b580: 640a 2020 2020 2020 2020 3a70 6172 616d  d.        :param
-0000b590: 2073 7472 6561 6d3a 2069 6620 5472 7565   stream: if True
-0000b5a0: 2c20 7468 6520 7572 6c6c 6962 332e 4854  , the urllib3.HT
-0000b5b0: 5450 5265 7370 6f6e 7365 206f 626a 6563  TPResponse objec
-0000b5c0: 7420 7769 6c6c 0a20 2020 2020 2020 2020  t will.         
-0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5e0: 2020 2020 2020 2020 6265 2072 6574 7572          be retur
-0000b5f0: 6e65 6420 7769 7468 6f75 7420 7265 6164  ned without read
-0000b600: 696e 672f 6465 636f 6469 6e67 2072 6573  ing/decoding res
-0000b610: 706f 6e73 650a 2020 2020 2020 2020 2020  ponse.          
-0000b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b630: 2020 2020 2020 2064 6174 612e 2041 6c73         data. Als
-0000b640: 6f20 7768 656e 2054 7275 652c 2069 6620  o when True, if 
-0000b650: 7468 6520 6f70 656e 6170 6920 7370 6563  the openapi spec
-0000b660: 2064 6573 6372 6962 6573 2061 2066 696c   describes a fil
-0000b670: 6520 646f 776e 6c6f 6164 2c0a 2020 2020  e download,.    
-0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b690: 2020 2020 2020 2020 2020 2020 2074 6865               the
-0000b6a0: 2064 6174 6120 7769 6c6c 2062 6520 7772   data will be wr
-0000b6b0: 6974 7465 6e20 746f 2061 206c 6f63 616c  itten to a local
-0000b6c0: 2066 696c 6573 7973 746d 6520 6669 6c65   filesystme file
-0000b6d0: 2061 6e64 2074 6865 2042 696e 6172 7953   and the BinaryS
-0000b6e0: 6368 656d 610a 2020 2020 2020 2020 2020  chema.          
-0000b6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b700: 2020 2020 2020 2069 6e73 7461 6e63 6520         instance 
-0000b710: 7769 6c6c 2061 6c73 6f20 696e 6865 7269  will also inheri
-0000b720: 7420 6672 6f6d 2046 696c 6553 6368 656d  t from FileSchem
-0000b730: 6120 616e 6420 4669 6c65 494f 0a20 2020  a and FileIO.   
-0000b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b750: 2020 2020 2020 2020 2020 2020 2020 4465                De
-0000b760: 6661 756c 7420 6973 2046 616c 7365 2e0a  fault is False..
-0000b770: 2020 2020 2020 2020 3a74 7970 6520 7374          :type st
-0000b780: 7265 616d 3a20 626f 6f6c 2c20 6f70 7469  ream: bool, opti
-0000b790: 6f6e 616c 0a20 2020 2020 2020 203a 7061  onal.        :pa
-0000b7a0: 7261 6d20 7469 6d65 6f75 743a 2074 696d  ram timeout: tim
-0000b7b0: 656f 7574 2073 6574 7469 6e67 2066 6f72  eout setting for
-0000b7c0: 2074 6869 7320 7265 7175 6573 742e 2049   this request. I
-0000b7d0: 6620 6f6e 650a 2020 2020 2020 2020 2020  f one.          
-0000b7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7f0: 2020 2020 2020 206e 756d 6265 7220 7072         number pr
-0000b800: 6f76 6964 6564 2c20 6974 2077 696c 6c20  ovided, it will 
-0000b810: 6265 2074 6f74 616c 2072 6571 7565 7374  be total request
-0000b820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b840: 2020 7469 6d65 6f75 742e 2049 7420 6361    timeout. It ca
-0000b850: 6e20 616c 736f 2062 6520 6120 7061 6972  n also be a pair
-0000b860: 2028 7475 706c 6529 206f 660a 2020 2020   (tuple) of.    
-0000b870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b880: 2020 2020 2020 2020 2020 2020 2028 636f               (co
-0000b890: 6e6e 6563 7469 6f6e 2c20 7265 6164 2920  nnection, read) 
-0000b8a0: 7469 6d65 6f75 7473 2e0a 2020 2020 2020  timeouts..      
-0000b8b0: 2020 3a70 6172 616d 2068 6f73 743a 2061    :param host: a
-0000b8c0: 7069 2065 6e64 706f 696e 7420 686f 7374  pi endpoint host
-0000b8d0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-0000b8e0: 3a0a 2020 2020 2020 2020 2020 2020 4966  :.            If
-0000b8f0: 2061 7379 6e63 5f72 6571 2070 6172 616d   async_req param
-0000b900: 6574 6572 2069 7320 5472 7565 2c0a 2020  eter is True,.  
-0000b910: 2020 2020 2020 2020 2020 7468 6520 7265            the re
-0000b920: 7175 6573 7420 7769 6c6c 2062 6520 6361  quest will be ca
-0000b930: 6c6c 6564 2061 7379 6e63 6872 6f6e 6f75  lled asynchronou
-0000b940: 736c 792e 0a20 2020 2020 2020 2020 2020  sly..           
-0000b950: 2054 6865 206d 6574 686f 6420 7769 6c6c   The method will
-0000b960: 2072 6574 7572 6e20 7468 6520 7265 7175   return the requ
-0000b970: 6573 7420 7468 7265 6164 2e0a 2020 2020  est thread..    
-0000b980: 2020 2020 2020 2020 4966 2070 6172 616d          If param
-0000b990: 6574 6572 2061 7379 6e63 5f72 6571 2069  eter async_req i
-0000b9a0: 7320 4661 6c73 6520 6f72 206d 6973 7369  s False or missi
-0000b9b0: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
-0000b9c0: 7468 656e 2074 6865 206d 6574 686f 6420  then the method 
-0000b9d0: 7769 6c6c 2072 6574 7572 6e20 7468 6520  will return the 
-0000b9e0: 7265 7370 6f6e 7365 2064 6972 6563 746c  response directl
-0000b9f0: 792e 0a20 2020 2020 2020 2022 2222 0a0a  y..        """..
-0000ba00: 2020 2020 2020 2020 6966 206e 6f74 2061          if not a
-0000ba10: 7379 6e63 5f72 6571 3a0a 2020 2020 2020  sync_req:.      
-0000ba20: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000ba30: 662e 5f5f 6361 6c6c 5f61 7069 280a 2020  f.__call_api(.  
-0000ba40: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000ba50: 736f 7572 6365 5f70 6174 682c 0a20 2020  source_path,.   
-0000ba60: 2020 2020 2020 2020 2020 2020 206d 6574               met
-0000ba70: 686f 642c 0a20 2020 2020 2020 2020 2020  hod,.           
-0000ba80: 2020 2020 2068 6561 6465 7273 2c0a 2020       headers,.  
-0000ba90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000baa0: 7269 616c 697a 6564 5f62 6f64 792c 0a20  rialized_body,. 
-0000bab0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0000bac0: 6f64 792c 0a20 2020 2020 2020 2020 2020  ody,.           
-0000bad0: 2020 2020 2066 6965 6c64 732c 0a20 2020       fields,.   
-0000bae0: 2020 2020 2020 2020 2020 2020 2061 7574               aut
-0000baf0: 685f 7365 7474 696e 6773 2c0a 2020 2020  h_settings,.    
-0000bb00: 2020 2020 2020 2020 2020 2020 7374 7265              stre
-0000bb10: 616d 2c0a 2020 2020 2020 2020 2020 2020  am,.            
-0000bb20: 2020 2020 7469 6d65 6f75 742c 0a20 2020      timeout,.   
-0000bb30: 2020 2020 2020 2020 2020 2020 2068 6f73               hos
-0000bb40: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-0000bb50: 2020 2070 7265 6669 785f 7365 7061 7261     prefix_separa
-0000bb60: 746f 725f 6974 6572 6174 6f72 2c0a 2020  tor_iterator,.  
-0000bb70: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-0000bb80: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000bb90: 2e70 6f6f 6c2e 6170 706c 795f 6173 796e  .pool.apply_asyn
-0000bba0: 6328 0a20 2020 2020 2020 2020 2020 2073  c(.            s
-0000bbb0: 656c 662e 5f5f 6361 6c6c 5f61 7069 2c0a  elf.__call_api,.
-0000bbc0: 2020 2020 2020 2020 2020 2020 280a 2020              (.  
-0000bbd0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000bbe0: 736f 7572 6365 5f70 6174 682c 0a20 2020  source_path,.   
-0000bbf0: 2020 2020 2020 2020 2020 2020 206d 6574               met
-0000bc00: 686f 642c 0a20 2020 2020 2020 2020 2020  hod,.           
-0000bc10: 2020 2020 2068 6561 6465 7273 2c0a 2020       headers,.  
-0000bc20: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000bc30: 7269 616c 697a 6564 5f62 6f64 792c 0a20  rialized_body,. 
-0000bc40: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0000bc50: 6f64 792c 0a20 2020 2020 2020 2020 2020  ody,.           
-0000bc60: 2020 2020 206a 736f 6e2c 0a20 2020 2020       json,.     
-0000bc70: 2020 2020 2020 2020 2020 2066 6965 6c64             field
-0000bc80: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000bc90: 2020 2061 7574 685f 7365 7474 696e 6773     auth_settings
-0000bca0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000bcb0: 2020 7374 7265 616d 2c0a 2020 2020 2020    stream,.      
-0000bcc0: 2020 2020 2020 2020 2020 7469 6d65 6f75            timeou
-0000bcd0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-0000bce0: 2020 2068 6f73 742c 0a20 2020 2020 2020     host,.       
-0000bcf0: 2020 2020 2020 2020 2070 7265 6669 785f           prefix_
-0000bd00: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
-0000bd10: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
-0000bd20: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
-0000bd30: 2064 6566 2072 6571 7565 7374 280a 2020   def request(.  
-0000bd40: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000bd50: 2020 2020 6d65 7468 6f64 3a20 7374 722c      method: str,
-0000bd60: 0a20 2020 2020 2020 2075 726c 3a20 7374  .        url: st
-0000bd70: 722c 0a20 2020 2020 2020 2068 6561 6465  r,.        heade
-0000bd80: 7273 3a20 7479 7069 6e67 2e4f 7074 696f  rs: typing.Optio
-0000bd90: 6e61 6c5b 4854 5450 4865 6164 6572 4469  nal[HTTPHeaderDi
-0000bda0: 6374 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ct] = None,.    
-0000bdb0: 2020 2020 6669 656c 6473 3a20 7479 7069      fields: typi
-0000bdc0: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-0000bdd0: 6e67 2e54 7570 6c65 5b74 7970 696e 672e  ng.Tuple[typing.
-0000bde0: 5475 706c 655b 7374 722c 2073 7472 5d2c  Tuple[str, str],
-0000bdf0: 202e 2e2e 5d5d 203d 204e 6f6e 652c 0a20   ...]] = None,. 
-0000be00: 2020 2020 2020 2062 6f64 793a 2074 7970         body: typ
-0000be10: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
-0000be20: 696e 672e 556e 696f 6e5b 7374 722c 2062  ing.Union[str, b
-0000be30: 7974 6573 5d5d 203d 204e 6f6e 652c 0a20  ytes]] = None,. 
-0000be40: 2020 2020 2020 2073 7472 6561 6d3a 2062         stream: b
-0000be50: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-0000be60: 2020 2020 2074 696d 656f 7574 3a20 7479       timeout: ty
-0000be70: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-0000be80: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
-0000be90: 7479 7069 6e67 2e54 7570 6c65 5d5d 203d  typing.Tuple]] =
-0000bea0: 204e 6f6e 652c 0a20 2020 2029 202d 3e20   None,.    ) -> 
-0000beb0: 5265 7370 6f6e 7365 5772 6170 7065 723a  ResponseWrapper:
-0000bec0: 0a20 2020 2020 2020 2022 2222 4d61 6b65  .        """Make
-0000bed0: 7320 7468 6520 4854 5450 2072 6571 7565  s the HTTP reque
-0000bee0: 7374 2075 7369 6e67 2052 4553 5443 6c69  st using RESTCli
-0000bef0: 656e 742e 2222 220a 2020 2020 2020 2020  ent.""".        
-0000bf00: 6966 206d 6574 686f 6420 3d3d 2022 4745  if method == "GE
-0000bf10: 5422 3a0a 2020 2020 2020 2020 2020 2020  T":.            
-0000bf20: 7265 7475 726e 2073 656c 662e 7265 7374  return self.rest
-0000bf30: 5f63 6c69 656e 742e 4745 5428 7572 6c2c  _client.GET(url,
-0000bf40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf60: 2020 2020 2020 2020 2073 7472 6561 6d3d           stream=
-0000bf70: 7374 7265 616d 2c0a 2020 2020 2020 2020  stream,.        
-0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfa0: 7469 6d65 6f75 743d 7469 6d65 6f75 742c  timeout=timeout,
-0000bfb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfd0: 2020 2020 2020 2020 2068 6561 6465 7273           headers
-0000bfe0: 3d68 6561 6465 7273 290a 2020 2020 2020  =headers).      
-0000bff0: 2020 656c 6966 206d 6574 686f 6420 3d3d    elif method ==
-0000c000: 2022 4845 4144 223a 0a20 2020 2020 2020   "HEAD":.       
-0000c010: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000c020: 2e72 6573 745f 636c 6965 6e74 2e48 4541  .rest_client.HEA
-0000c030: 4428 7572 6c2c 0a20 2020 2020 2020 2020  D(url,.         
-0000c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c060: 7374 7265 616d 3d73 7472 6561 6d2c 0a20  stream=stream,. 
-0000c070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c090: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
-0000c0a0: 7469 6d65 6f75 742c 0a20 2020 2020 2020  timeout,.       
-0000c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0d0: 2020 6865 6164 6572 733d 6865 6164 6572    headers=header
-0000c0e0: 7329 0a20 2020 2020 2020 2065 6c69 6620  s).        elif 
-0000c0f0: 6d65 7468 6f64 203d 3d20 224f 5054 494f  method == "OPTIO
-0000c100: 4e53 223a 0a20 2020 2020 2020 2020 2020  NS":.           
-0000c110: 2072 6574 7572 6e20 7365 6c66 2e72 6573   return self.res
-0000c120: 745f 636c 6965 6e74 2e4f 5054 494f 4e53  t_client.OPTIONS
-0000c130: 2875 726c 2c0a 2020 2020 2020 2020 2020  (url,.          
-0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c160: 2020 6865 6164 6572 733d 6865 6164 6572    headers=header
-0000c170: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c190: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000c1a0: 6965 6c64 733d 6669 656c 6473 2c0a 2020  ields=fields,.  
-0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1d0: 2020 2020 2020 2020 2020 7374 7265 616d            stream
-0000c1e0: 3d73 7472 6561 6d2c 0a20 2020 2020 2020  =stream,.       
-0000c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c210: 2020 2020 2074 696d 656f 7574 3d74 696d       timeout=tim
-0000c220: 656f 7574 2c0a 2020 2020 2020 2020 2020  eout,.          
-0000c230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c250: 2020 626f 6479 3d62 6f64 7929 0a20 2020    body=body).   
-0000c260: 2020 2020 2065 6c69 6620 6d65 7468 6f64       elif method
-0000c270: 203d 3d20 2250 4f53 5422 3a0a 2020 2020   == "POST":.    
-0000c280: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000c290: 656c 662e 7265 7374 5f63 6c69 656e 742e  elf.rest_client.
-0000c2a0: 504f 5354 2875 726c 2c0a 2020 2020 2020  POST(url,.      
-0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2d0: 2020 2068 6561 6465 7273 3d68 6561 6465     headers=heade
-0000c2e0: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
-0000c2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c300: 2020 2020 2020 2020 2020 2020 2066 6965               fie
-0000c310: 6c64 733d 6669 656c 6473 2c0a 2020 2020  lds=fields,.    
-0000c320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c340: 2020 2020 2073 7472 6561 6d3d 7374 7265       stream=stre
-0000c350: 616d 2c0a 2020 2020 2020 2020 2020 2020  am,.            
+00000170: 7420 7469 6d65 0a69 6d70 6f72 7420 7479  t time.import ty
+00000180: 7069 6e67 0a69 6d70 6f72 7420 7479 7069  ping.import typi
+00000190: 6e67 5f65 7874 656e 7369 6f6e 730a 696d  ng_extensions.im
+000001a0: 706f 7274 2061 696f 6874 7470 0a69 6d70  port aiohttp.imp
+000001b0: 6f72 7420 7572 6c6c 6962 330a 6672 6f6d  ort urllib3.from
+000001c0: 2075 726c 6c69 6233 2e5f 636f 6c6c 6563   urllib3._collec
+000001d0: 7469 6f6e 7320 696d 706f 7274 2048 5454  tions import HTT
+000001e0: 5048 6561 6465 7244 6963 740a 6672 6f6d  PHeaderDict.from
+000001f0: 2075 726c 6c69 622e 7061 7273 6520 696d   urllib.parse im
+00000200: 706f 7274 2075 726c 7061 7273 652c 2071  port urlparse, q
+00000210: 756f 7465 0a66 726f 6d20 7572 6c6c 6962  uote.from urllib
+00000220: 332e 6669 656c 6473 2069 6d70 6f72 7420  3.fields import 
+00000230: 5265 7175 6573 7446 6965 6c64 2061 7320  RequestField as 
+00000240: 5265 7175 6573 7446 6965 6c64 4261 7365  RequestFieldBase
+00000250: 0a66 726f 6d20 7572 6c6c 6962 332e 6669  .from urllib3.fi
+00000260: 656c 6473 2069 6d70 6f72 7420 6775 6573  elds import gues
+00000270: 735f 636f 6e74 656e 745f 7479 7065 0a0a  s_content_type..
+00000280: 696d 706f 7274 2066 726f 7a65 6e64 6963  import frozendic
+00000290: 740a 0a66 726f 6d20 7370 6c69 7469 745f  t..from splitit_
+000002a0: 636c 6965 6e74 2069 6d70 6f72 7420 7265  client import re
+000002b0: 7374 0a66 726f 6d20 7370 6c69 7469 745f  st.from splitit_
+000002c0: 636c 6965 6e74 2e61 7069 5f72 6573 706f  client.api_respo
+000002d0: 6e73 6520 696d 706f 7274 2041 7069 5265  nse import ApiRe
+000002e0: 7370 6f6e 7365 2c20 4173 796e 6341 7069  sponse, AsyncApi
+000002f0: 5265 7370 6f6e 7365 0a66 726f 6d20 7370  Response.from sp
+00000300: 6c69 7469 745f 636c 6965 6e74 2e72 6573  litit_client.res
+00000310: 7420 696d 706f 7274 2041 7379 6e63 5265  t import AsyncRe
+00000320: 7370 6f6e 7365 5772 6170 7065 722c 2052  sponseWrapper, R
+00000330: 6573 706f 6e73 6557 7261 7070 6572 0a66  esponseWrapper.f
+00000340: 726f 6d20 7370 6c69 7469 745f 636c 6965  rom splitit_clie
+00000350: 6e74 2e63 6f6e 6669 6775 7261 7469 6f6e  nt.configuration
+00000360: 2069 6d70 6f72 7420 436f 6e66 6967 7572   import Configur
+00000370: 6174 696f 6e0a 6672 6f6d 2073 706c 6974  ation.from split
+00000380: 6974 5f63 6c69 656e 742e 6578 6365 7074  it_client.except
+00000390: 696f 6e73 2069 6d70 6f72 7420 4170 6954  ions import ApiT
+000003a0: 7970 6545 7272 6f72 2c20 4170 6956 616c  ypeError, ApiVal
+000003b0: 7565 4572 726f 722c 204d 6973 7369 6e67  ueError, Missing
+000003c0: 5265 7175 6972 6564 5061 7261 6d65 7465  RequiredParamete
+000003d0: 7273 4572 726f 720a 6672 6f6d 2073 706c  rsError.from spl
+000003e0: 6974 6974 5f63 6c69 656e 742e 7265 7175  itit_client.requ
+000003f0: 6573 745f 6166 7465 725f 686f 6f6b 2069  est_after_hook i
+00000400: 6d70 6f72 7420 7265 7175 6573 745f 6166  mport request_af
+00000410: 7465 725f 686f 6f6b 0a66 726f 6d20 7370  ter_hook.from sp
+00000420: 6c69 7469 745f 636c 6965 6e74 2e72 6571  litit_client.req
+00000430: 7565 7374 5f62 6566 6f72 655f 686f 6f6b  uest_before_hook
+00000440: 2069 6d70 6f72 7420 7265 7175 6573 745f   import request_
+00000450: 6265 666f 7265 5f68 6f6f 6b0a 6672 6f6d  before_hook.from
+00000460: 2073 706c 6974 6974 5f63 6c69 656e 742e   splitit_client.
+00000470: 7363 6865 6d61 7320 696d 706f 7274 2028  schemas import (
+00000480: 0a20 2020 204e 6f6e 6543 6c61 7373 2c0a  .    NoneClass,.
+00000490: 2020 2020 426f 6f6c 436c 6173 732c 0a20      BoolClass,. 
+000004a0: 2020 2053 6368 656d 612c 0a20 2020 2046     Schema,.    F
+000004b0: 696c 6549 4f2c 0a20 2020 2042 696e 6172  ileIO,.    Binar
+000004c0: 7953 6368 656d 612c 0a20 2020 2064 6174  ySchema,.    dat
+000004d0: 652c 0a20 2020 2064 6174 6574 696d 652c  e,.    datetime,
+000004e0: 0a20 2020 206e 6f6e 655f 7479 7065 2c0a  .    none_type,.
+000004f0: 2020 2020 556e 7365 742c 0a20 2020 2075      Unset,.    u
+00000500: 6e73 6574 2c0a 290a 0a40 6461 7461 636c  nset,.)..@datacl
+00000510: 6173 730a 636c 6173 7320 4d61 7070 6564  ass.class Mapped
+00000520: 4172 6773 3a0a 2020 2020 626f 6479 3a20  Args:.    body: 
+00000530: 7479 7069 6e67 2e41 6e79 203d 204e 6f6e  typing.Any = Non
+00000540: 650a 2020 2020 7175 6572 793a 2074 7970  e.    query: typ
+00000550: 696e 672e 4f70 7469 6f6e 616c 5b64 6963  ing.Optional[dic
+00000560: 745d 203d 204e 6f6e 650a 2020 2020 7061  t] = None.    pa
+00000570: 7468 3a20 7479 7069 6e67 2e4f 7074 696f  th: typing.Optio
+00000580: 6e61 6c5b 6469 6374 5d20 3d20 4e6f 6e65  nal[dict] = None
+00000590: 0a20 2020 2068 6561 6465 723a 2074 7970  .    header: typ
+000005a0: 696e 672e 4f70 7469 6f6e 616c 5b64 6963  ing.Optional[dic
+000005b0: 745d 203d 204e 6f6e 650a 2020 2020 636f  t] = None.    co
+000005c0: 6f6b 6965 3a20 7479 7069 6e67 2e4f 7074  okie: typing.Opt
+000005d0: 696f 6e61 6c5b 6469 6374 5d20 3d20 4e6f  ional[dict] = No
+000005e0: 6e65 0a0a 636c 6173 7320 5265 7175 6573  ne..class Reques
+000005f0: 7446 6965 6c64 2852 6571 7565 7374 4669  tField(RequestFi
+00000600: 656c 6442 6173 6529 3a0a 2020 2020 6465  eldBase):.    de
+00000610: 6620 5f5f 6571 5f5f 2873 656c 662c 206f  f __eq__(self, o
+00000620: 7468 6572 293a 0a20 2020 2020 2020 2069  ther):.        i
+00000630: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+00000640: 286f 7468 6572 2c20 5265 7175 6573 7446  (other, RequestF
+00000650: 6965 6c64 293a 0a20 2020 2020 2020 2020  ield):.         
+00000660: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00000670: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00000680: 656c 662e 5f5f 6469 6374 5f5f 203d 3d20  elf.__dict__ == 
+00000690: 6f74 6865 722e 5f5f 6469 6374 5f5f 0a0a  other.__dict__..
+000006a0: 0a63 6c61 7373 204a 534f 4e45 6e63 6f64  .class JSONEncod
+000006b0: 6572 286a 736f 6e2e 4a53 4f4e 456e 636f  er(json.JSONEnco
+000006c0: 6465 7229 3a0a 2020 2020 636f 6d70 6163  der):.    compac
+000006d0: 745f 7365 7061 7261 746f 7273 203d 2028  t_separators = (
+000006e0: 272c 272c 2027 3a27 290a 0a20 2020 2064  ',', ':')..    d
+000006f0: 6566 2064 6566 6175 6c74 2873 656c 662c  ef default(self,
+00000700: 206f 626a 293a 0a20 2020 2020 2020 2069   obj):.        i
+00000710: 6620 6973 696e 7374 616e 6365 286f 626a  f isinstance(obj
+00000720: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
+00000730: 2020 2020 7265 7475 726e 2073 7472 286f      return str(o
+00000740: 626a 290a 2020 2020 2020 2020 656c 6966  bj).        elif
+00000750: 2069 7369 6e73 7461 6e63 6528 6f62 6a2c   isinstance(obj,
+00000760: 2066 6c6f 6174 293a 0a20 2020 2020 2020   float):.       
+00000770: 2020 2020 2072 6574 7572 6e20 666c 6f61       return floa
+00000780: 7428 6f62 6a29 0a20 2020 2020 2020 2065  t(obj).        e
+00000790: 6c69 6620 6973 696e 7374 616e 6365 286f  lif isinstance(o
+000007a0: 626a 2c20 696e 7429 3a0a 2020 2020 2020  bj, int):.      
+000007b0: 2020 2020 2020 7265 7475 726e 2069 6e74        return int
+000007c0: 286f 626a 290a 2020 2020 2020 2020 656c  (obj).        el
+000007d0: 6966 2069 7369 6e73 7461 6e63 6528 6f62  if isinstance(ob
+000007e0: 6a2c 2044 6563 696d 616c 293a 0a20 2020  j, Decimal):.   
+000007f0: 2020 2020 2020 2020 2069 6620 6f62 6a2e           if obj.
+00000800: 6173 5f74 7570 6c65 2829 2e65 7870 6f6e  as_tuple().expon
+00000810: 656e 7420 3e3d 2030 3a0a 2020 2020 2020  ent >= 0:.      
+00000820: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00000830: 2069 6e74 286f 626a 290a 2020 2020 2020   int(obj).      
+00000840: 2020 2020 2020 7265 7475 726e 2066 6c6f        return flo
+00000850: 6174 286f 626a 290a 2020 2020 2020 2020  at(obj).        
+00000860: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+00000870: 6f62 6a2c 204e 6f6e 6543 6c61 7373 293a  obj, NoneClass):
+00000880: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00000890: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
+000008a0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+000008b0: 286f 626a 2c20 426f 6f6c 436c 6173 7329  (obj, BoolClass)
+000008c0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000008d0: 7475 726e 2062 6f6f 6c28 6f62 6a29 0a20  turn bool(obj). 
+000008e0: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+000008f0: 7374 616e 6365 286f 626a 2c20 2864 6963  stance(obj, (dic
+00000900: 742c 2066 726f 7a65 6e64 6963 742e 6672  t, frozendict.fr
+00000910: 6f7a 656e 6469 6374 2929 3a0a 2020 2020  ozendict)):.    
+00000920: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+00000930: 6b65 793a 2073 656c 662e 6465 6661 756c  key: self.defaul
+00000940: 7428 7661 6c29 2066 6f72 206b 6579 2c20  t(val) for key, 
+00000950: 7661 6c20 696e 206f 626a 2e69 7465 6d73  val in obj.items
+00000960: 2829 7d0a 2020 2020 2020 2020 656c 6966  ()}.        elif
+00000970: 2069 7369 6e73 7461 6e63 6528 6f62 6a2c   isinstance(obj,
+00000980: 2028 6c69 7374 2c20 7475 706c 6529 293a   (list, tuple)):
+00000990: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000009a0: 7572 6e20 5b73 656c 662e 6465 6661 756c  urn [self.defaul
+000009b0: 7428 6974 656d 2920 666f 7220 6974 656d  t(item) for item
+000009c0: 2069 6e20 6f62 6a5d 0a20 2020 2020 2020   in obj].       
+000009d0: 2072 6169 7365 2041 7069 5661 6c75 6545   raise ApiValueE
+000009e0: 7272 6f72 2827 556e 6162 6c65 2074 6f20  rror('Unable to 
+000009f0: 7072 6570 6172 6520 7479 7065 207b 7d20  prepare type {} 
+00000a00: 666f 7220 7365 7269 616c 697a 6174 696f  for serializatio
+00000a10: 6e27 2e66 6f72 6d61 7428 6f62 6a2e 5f5f  n'.format(obj.__
+00000a20: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
+00000a30: 2929 0a0a 0a63 6c61 7373 2050 6172 616d  ))...class Param
+00000a40: 6574 6572 496e 5479 7065 2865 6e75 6d2e  eterInType(enum.
+00000a50: 456e 756d 293a 0a20 2020 2051 5545 5259  Enum):.    QUERY
+00000a60: 203d 2027 7175 6572 7927 0a20 2020 2048   = 'query'.    H
+00000a70: 4541 4445 5220 3d20 2768 6561 6465 7227  EADER = 'header'
+00000a80: 0a20 2020 2050 4154 4820 3d20 2770 6174  .    PATH = 'pat
+00000a90: 6827 0a20 2020 2043 4f4f 4b49 4520 3d20  h'.    COOKIE = 
+00000aa0: 2763 6f6f 6b69 6527 0a0a 0a63 6c61 7373  'cookie'...class
+00000ab0: 2050 6172 616d 6574 6572 5374 796c 6528   ParameterStyle(
+00000ac0: 656e 756d 2e45 6e75 6d29 3a0a 2020 2020  enum.Enum):.    
+00000ad0: 4d41 5452 4958 203d 2027 6d61 7472 6978  MATRIX = 'matrix
+00000ae0: 270a 2020 2020 4c41 4245 4c20 3d20 276c  '.    LABEL = 'l
+00000af0: 6162 656c 270a 2020 2020 464f 524d 203d  abel'.    FORM =
+00000b00: 2027 666f 726d 270a 2020 2020 5349 4d50   'form'.    SIMP
+00000b10: 4c45 203d 2027 7369 6d70 6c65 270a 2020  LE = 'simple'.  
+00000b20: 2020 5350 4143 455f 4445 4c49 4d49 5445    SPACE_DELIMITE
+00000b30: 4420 3d20 2773 7061 6365 4465 6c69 6d69  D = 'spaceDelimi
+00000b40: 7465 6427 0a20 2020 2050 4950 455f 4445  ted'.    PIPE_DE
+00000b50: 4c49 4d49 5445 4420 3d20 2770 6970 6544  LIMITED = 'pipeD
+00000b60: 656c 696d 6974 6564 270a 2020 2020 4445  elimited'.    DE
+00000b70: 4550 5f4f 424a 4543 5420 3d20 2764 6565  EP_OBJECT = 'dee
+00000b80: 704f 626a 6563 7427 0a0a 0a63 6c61 7373  pObject'...class
+00000b90: 2050 7265 6669 7853 6570 6172 6174 6f72   PrefixSeparator
+00000ba0: 4974 6572 6174 6f72 3a0a 2020 2020 2320  Iterator:.    # 
+00000bb0: 4120 636c 6173 7320 746f 2073 746f 7265  A class to store
+00000bc0: 2070 7265 6669 7865 7320 616e 6420 7365   prefixes and se
+00000bd0: 7061 7261 746f 7273 2066 6f72 2072 6663  parators for rfc
+00000be0: 3635 3730 2065 7870 616e 7369 6f6e 730a  6570 expansions.
+00000bf0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00000c00: 5f28 7365 6c66 2c20 7072 6566 6978 3a20  _(self, prefix: 
+00000c10: 7374 722c 2073 6570 6172 6174 6f72 3a20  str, separator: 
+00000c20: 7374 7229 3a0a 2020 2020 2020 2020 7365  str):.        se
+00000c30: 6c66 2e70 7265 6669 7820 3d20 7072 6566  lf.prefix = pref
+00000c40: 6978 0a20 2020 2020 2020 2073 656c 662e  ix.        self.
+00000c50: 7365 7061 7261 746f 7220 3d20 7365 7061  separator = sepa
+00000c60: 7261 746f 720a 2020 2020 2020 2020 7365  rator.        se
+00000c70: 6c66 2e66 6972 7374 203d 2054 7275 650a  lf.first = True.
+00000c80: 2020 2020 2020 2020 6966 2073 6570 6172          if separ
+00000c90: 6174 6f72 2069 6e20 7b27 2e27 2c20 277c  ator in {'.', '|
+00000ca0: 272c 2027 2532 3027 7d3a 0a20 2020 2020  ', '%20'}:.     
+00000cb0: 2020 2020 2020 2069 7465 6d5f 7365 7061         item_sepa
+00000cc0: 7261 746f 7220 3d20 7365 7061 7261 746f  rator = separato
+00000cd0: 720a 2020 2020 2020 2020 656c 7365 3a0a  r.        else:.
+00000ce0: 2020 2020 2020 2020 2020 2020 6974 656d              item
+00000cf0: 5f73 6570 6172 6174 6f72 203d 2027 2c27  _separator = ','
+00000d00: 0a20 2020 2020 2020 2073 656c 662e 6974  .        self.it
+00000d10: 656d 5f73 6570 6172 6174 6f72 203d 2069  em_separator = i
+00000d20: 7465 6d5f 7365 7061 7261 746f 720a 0a20  tem_separator.. 
+00000d30: 2020 2064 6566 205f 5f69 7465 725f 5f28     def __iter__(
+00000d40: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+00000d50: 6574 7572 6e20 7365 6c66 0a0a 2020 2020  eturn self..    
+00000d60: 6465 6620 5f5f 6e65 7874 5f5f 2873 656c  def __next__(sel
+00000d70: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
+00000d80: 656c 662e 6669 7273 743a 0a20 2020 2020  elf.first:.     
+00000d90: 2020 2020 2020 2073 656c 662e 6669 7273         self.firs
+00000da0: 7420 3d20 4661 6c73 650a 2020 2020 2020  t = False.      
+00000db0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00000dc0: 662e 7072 6566 6978 0a20 2020 2020 2020  f.prefix.       
+00000dd0: 2072 6574 7572 6e20 7365 6c66 2e73 6570   return self.sep
+00000de0: 6172 6174 6f72 0a0a 0a63 6c61 7373 2050  arator...class P
+00000df0: 6172 616d 6574 6572 5365 7269 616c 697a  arameterSerializ
+00000e00: 6572 4261 7365 3a0a 2020 2020 4063 6c61  erBase:.    @cla
+00000e10: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+00000e20: 205f 6765 745f 6465 6661 756c 745f 6578   _get_default_ex
+00000e30: 706c 6f64 6528 636c 732c 2073 7479 6c65  plode(cls, style
+00000e40: 3a20 5061 7261 6d65 7465 7253 7479 6c65  : ParameterStyle
+00000e50: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00000e60: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00000e70: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+00000e80: 6f64 0a20 2020 2064 6566 205f 5f72 6566  od.    def __ref
+00000e90: 3635 3730 5f69 7465 6d5f 7661 6c75 6528  6570_item_value(
+00000ea0: 696e 5f64 6174 613a 2074 7970 696e 672e  in_data: typing.
+00000eb0: 416e 792c 2070 6572 6365 6e74 5f65 6e63  Any, percent_enc
+00000ec0: 6f64 653a 2062 6f6f 6c29 3a0a 2020 2020  ode: bool):.    
+00000ed0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00000ee0: 4765 7420 7265 7072 6573 656e 7461 7469  Get representati
+00000ef0: 6f6e 2069 6620 7374 722f 666c 6f61 742f  on if str/float/
+00000f00: 696e 742f 4e6f 6e65 2f69 7465 6d73 2069  int/None/items i
+00000f10: 6e20 6c69 7374 2f20 7661 6c75 6573 2069  n list/ values i
+00000f20: 6e20 6469 6374 0a20 2020 2020 2020 204e  n dict.        N
+00000f30: 6f6e 6520 6973 2072 6574 7572 6e65 6420  one is returned 
+00000f40: 6966 2061 6e20 6974 656d 2069 7320 756e  if an item is un
+00000f50: 6465 6669 6e65 642c 2075 7365 2063 6173  defined, use cas
+00000f60: 6573 2061 7265 2076 616c 7565 3d0a 2020  es are value=.  
+00000f70: 2020 2020 2020 2d20 4e6f 6e65 0a20 2020        - None.   
+00000f80: 2020 2020 202d 205b 5d0a 2020 2020 2020       - [].      
+00000f90: 2020 2d20 7b7d 0a20 2020 2020 2020 202d    - {}.        -
+00000fa0: 205b 4e6f 6e65 2c20 4e6f 6e65 204e 6f6e   [None, None Non
+00000fb0: 655d 0a20 2020 2020 2020 202d 207b 2761  e].        - {'a
+00000fc0: 273a 204e 6f6e 652c 2027 6227 3a20 4e6f  ': None, 'b': No
+00000fd0: 6e65 7d0a 2020 2020 2020 2020 2222 220a  ne}.        """.
+00000fe0: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
+00000ff0: 696e 5f64 6174 6129 2069 6e20 7b73 7472  in_data) in {str
+00001000: 2c20 666c 6f61 742c 2069 6e74 7d3a 0a20  , float, int}:. 
+00001010: 2020 2020 2020 2020 2020 2069 6620 7065             if pe
+00001020: 7263 656e 745f 656e 636f 6465 3a0a 2020  rcent_encode:.  
+00001030: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00001040: 7475 726e 2071 756f 7465 2873 7472 2869  turn quote(str(i
+00001050: 6e5f 6461 7461 2929 0a20 2020 2020 2020  n_data)).       
+00001060: 2020 2020 2072 6574 7572 6e20 7374 7228       return str(
+00001070: 696e 5f64 6174 6129 0a20 2020 2020 2020  in_data).       
+00001080: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00001090: 2869 6e5f 6461 7461 2c20 6e6f 6e65 5f74  (in_data, none_t
+000010a0: 7970 6529 3a0a 2020 2020 2020 2020 2020  ype):.          
+000010b0: 2020 2320 6967 6e6f 7265 6420 6279 2074    # ignored by t
+000010c0: 6865 2065 7870 616e 7369 6f6e 2070 726f  he expansion pro
+000010d0: 6365 7373 2068 7474 7073 3a2f 2f64 6174  cess https://dat
+000010e0: 6174 7261 636b 6572 2e69 6574 662e 6f72  atracker.ietf.or
+000010f0: 672f 646f 632f 6874 6d6c 2f72 6663 3635  g/doc/html/rfc65
+00001100: 3730 2373 6563 7469 6f6e 2d33 2e32 2e31  70#section-3.2.1
+00001110: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00001120: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
+00001130: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00001140: 2869 6e5f 6461 7461 2c20 6c69 7374 2920  (in_data, list) 
+00001150: 616e 6420 6e6f 7420 696e 5f64 6174 613a  and not in_data:
+00001160: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
+00001170: 676e 6f72 6564 2062 7920 7468 6520 6578  gnored by the ex
+00001180: 7061 6e73 696f 6e20 7072 6f63 6573 7320  pansion process 
+00001190: 6874 7470 733a 2f2f 6461 7461 7472 6163  https://datatrac
+000011a0: 6b65 722e 6965 7466 2e6f 7267 2f64 6f63  ker.ietf.org/doc
+000011b0: 2f68 746d 6c2f 7266 6336 3537 3023 7365  /html/rfc6570#se
+000011c0: 6374 696f 6e2d 332e 322e 310a 2020 2020  ction-3.2.1.    
+000011d0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+000011e0: 6f6e 650a 2020 2020 2020 2020 656c 6966  one.        elif
+000011f0: 2069 7369 6e73 7461 6e63 6528 696e 5f64   isinstance(in_d
+00001200: 6174 612c 2064 6963 7429 2061 6e64 206e  ata, dict) and n
+00001210: 6f74 2069 6e5f 6461 7461 3a0a 2020 2020  ot in_data:.    
+00001220: 2020 2020 2020 2020 2320 6967 6e6f 7265          # ignore
+00001230: 6420 6279 2074 6865 2065 7870 616e 7369  d by the expansi
+00001240: 6f6e 2070 726f 6365 7373 2068 7474 7073  on process https
+00001250: 3a2f 2f64 6174 6174 7261 636b 6572 2e69  ://datatracker.i
+00001260: 6574 662e 6f72 672f 646f 632f 6874 6d6c  etf.org/doc/html
+00001270: 2f72 6663 3635 3730 2373 6563 7469 6f6e  /rfc6570#section
+00001280: 2d33 2e32 2e31 0a20 2020 2020 2020 2020  -3.2.1.         
+00001290: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+000012a0: 2020 2020 2020 2072 6169 7365 2041 7069         raise Api
+000012b0: 5661 6c75 6545 7272 6f72 2827 556e 6162  ValueError('Unab
+000012c0: 6c65 2074 6f20 6765 6e65 7261 7465 2061  le to generate a
+000012d0: 2072 6566 3635 3730 2069 7465 6d20 7265   ref6570 item re
+000012e0: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
+000012f0: 7b7d 272e 666f 726d 6174 2869 6e5f 6461  {}'.format(in_da
+00001300: 7461 2929 0a0a 2020 2020 4073 7461 7469  ta))..    @stati
+00001310: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
+00001320: 5f74 6f5f 6469 6374 286e 616d 653a 2073  _to_dict(name: s
+00001330: 7472 2c20 7661 6c75 653a 2073 7472 293a  tr, value: str):
+00001340: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001350: 7b6e 616d 653a 2076 616c 7565 7d0a 0a20  {name: value}.. 
+00001360: 2020 2022 2222 0a20 2020 2072 6663 3635     """.    rfc65
+00001370: 3730 2064 6f65 7320 6e6f 7420 7370 6563  70 does not spec
+00001380: 6966 7920 686f 7720 626f 6f6c 6561 6e20  ify how boolean 
+00001390: 7661 6c75 6573 2061 7265 2073 6572 6961  values are seria
+000013a0: 6c69 7a65 6420 736f 2077 6520 7573 6520  lized so we use 
+000013b0: 6c6f 7765 7263 6173 6520 2274 7275 6522  lowercase "true"
+000013c0: 2061 6e64 2022 6661 6c73 650a 2020 2020   and "false.    
+000013d0: 2222 220a 2020 2020 4063 6c61 7373 6d65  """.    @classme
+000013e0: 7468 6f64 0a20 2020 2064 6566 205f 5f6b  thod.    def __k
+000013f0: 6f6e 6669 675f 626f 6f6c 5f65 7870 616e  onfig_bool_expan
+00001400: 7369 6f6e 280a 2020 2020 2020 2020 636c  sion(.        cl
+00001410: 732c 0a20 2020 2020 2020 2069 6e5f 6461  s,.        in_da
+00001420: 7461 3a20 7479 7069 6e67 2e41 6e79 2c0a  ta: typing.Any,.
+00001430: 2020 2020 2020 2020 7072 6566 6978 5f73          prefix_s
+00001440: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+00001450: 723a 2050 7265 6669 7853 6570 6172 6174  r: PrefixSeparat
+00001460: 6f72 4974 6572 6174 6f72 2c0a 2020 2020  orIterator,.    
+00001470: 2020 2020 7661 725f 6e61 6d65 5f70 6965      var_name_pie
+00001480: 6365 3a20 7374 722c 0a20 2020 2020 2020  ce: str,.       
+00001490: 206e 616d 6564 5f70 6172 616d 6574 6572   named_parameter
+000014a0: 5f65 7870 616e 7369 6f6e 3a20 626f 6f6c  _expansion: bool
+000014b0: 0a20 2020 2029 202d 3e20 7374 723a 0a20  .    ) -> str:. 
+000014c0: 2020 2020 2020 2069 7465 6d5f 7661 6c75         item_valu
+000014d0: 6520 3d20 2274 7275 6522 2069 6620 696e  e = "true" if in
+000014e0: 5f64 6174 6120 6973 2054 7275 6520 656c  _data is True el
+000014f0: 7365 2022 6661 6c73 6522 0a20 2020 2020  se "false".     
+00001500: 2020 2069 6620 6974 656d 5f76 616c 7565     if item_value
+00001510: 2069 7320 4e6f 6e65 206f 7220 2869 7465   is None or (ite
+00001520: 6d5f 7661 6c75 6520 3d3d 2027 2720 616e  m_value == '' an
+00001530: 6420 7072 6566 6978 5f73 6570 6172 6174  d prefix_separat
+00001540: 6f72 5f69 7465 7261 746f 722e 7365 7061  or_iterator.sepa
+00001550: 7261 746f 7220 3d3d 2027 3b27 293a 0a20  rator == ';'):. 
+00001560: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001570: 6e20 6e65 7874 2870 7265 6669 785f 7365  n next(prefix_se
+00001580: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
+00001590: 2920 2b20 7661 725f 6e61 6d65 5f70 6965  ) + var_name_pie
+000015a0: 6365 0a20 2020 2020 2020 2076 616c 7565  ce.        value
+000015b0: 5f70 6169 725f 6571 7561 6c73 203d 2027  _pair_equals = '
+000015c0: 3d27 2069 6620 6e61 6d65 645f 7061 7261  =' if named_para
+000015d0: 6d65 7465 725f 6578 7061 6e73 696f 6e20  meter_expansion 
+000015e0: 656c 7365 2027 270a 2020 2020 2020 2020  else ''.        
+000015f0: 7265 7475 726e 206e 6578 7428 7072 6566  return next(pref
+00001600: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+00001610: 7261 746f 7229 202b 2076 6172 5f6e 616d  rator) + var_nam
+00001620: 655f 7069 6563 6520 2b20 7661 6c75 655f  e_piece + value_
+00001630: 7061 6972 5f65 7175 616c 7320 2b20 6974  pair_equals + it
+00001640: 656d 5f76 616c 7565 0a0a 2020 2020 4063  em_value..    @c
+00001650: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+00001660: 6566 205f 5f72 6566 3635 3730 5f73 7472  ef __ref6570_str
+00001670: 5f66 6c6f 6174 5f69 6e74 5f65 7870 616e  _float_int_expan
+00001680: 7369 6f6e 280a 2020 2020 2020 2020 636c  sion(.        cl
+00001690: 732c 0a20 2020 2020 2020 2076 6172 6961  s,.        varia
+000016a0: 626c 655f 6e61 6d65 3a20 7374 722c 0a20  ble_name: str,. 
+000016b0: 2020 2020 2020 2069 6e5f 6461 7461 3a20         in_data: 
+000016c0: 7479 7069 6e67 2e41 6e79 2c0a 2020 2020  typing.Any,.    
+000016d0: 2020 2020 6578 706c 6f64 653a 2062 6f6f      explode: boo
+000016e0: 6c2c 0a20 2020 2020 2020 2070 6572 6365  l,.        perce
+000016f0: 6e74 5f65 6e63 6f64 653a 2062 6f6f 6c2c  nt_encode: bool,
+00001700: 0a20 2020 2020 2020 2070 7265 6669 785f  .        prefix_
+00001710: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
+00001720: 6f72 3a20 5072 6566 6978 5365 7061 7261  or: PrefixSepara
+00001730: 746f 7249 7465 7261 746f 722c 0a20 2020  torIterator,.   
+00001740: 2020 2020 2076 6172 5f6e 616d 655f 7069       var_name_pi
+00001750: 6563 653a 2073 7472 2c0a 2020 2020 2020  ece: str,.      
+00001760: 2020 6e61 6d65 645f 7061 7261 6d65 7465    named_paramete
+00001770: 725f 6578 7061 6e73 696f 6e3a 2062 6f6f  r_expansion: boo
+00001780: 6c0a 2020 2020 2920 2d3e 2073 7472 3a0a  l.    ) -> str:.
+00001790: 2020 2020 2020 2020 6974 656d 5f76 616c          item_val
+000017a0: 7565 203d 2063 6c73 2e5f 5f72 6566 3635  ue = cls.__ref65
+000017b0: 3730 5f69 7465 6d5f 7661 6c75 6528 696e  70_item_value(in
+000017c0: 5f64 6174 612c 2070 6572 6365 6e74 5f65  _data, percent_e
+000017d0: 6e63 6f64 6529 0a20 2020 2020 2020 2069  ncode).        i
+000017e0: 6620 6974 656d 5f76 616c 7565 2069 7320  f item_value is 
+000017f0: 4e6f 6e65 206f 7220 2869 7465 6d5f 7661  None or (item_va
+00001800: 6c75 6520 3d3d 2027 2720 616e 6420 7072  lue == '' and pr
+00001810: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+00001820: 7465 7261 746f 722e 7365 7061 7261 746f  terator.separato
+00001830: 7220 3d3d 2027 3b27 293a 0a20 2020 2020  r == ';'):.     
+00001840: 2020 2020 2020 2072 6574 7572 6e20 6e65         return ne
+00001850: 7874 2870 7265 6669 785f 7365 7061 7261  xt(prefix_separa
+00001860: 746f 725f 6974 6572 6174 6f72 2920 2b20  tor_iterator) + 
+00001870: 7661 725f 6e61 6d65 5f70 6965 6365 0a20  var_name_piece. 
+00001880: 2020 2020 2020 2076 616c 7565 5f70 6169         value_pai
+00001890: 725f 6571 7561 6c73 203d 2027 3d27 2069  r_equals = '=' i
+000018a0: 6620 6e61 6d65 645f 7061 7261 6d65 7465  f named_paramete
+000018b0: 725f 6578 7061 6e73 696f 6e20 656c 7365  r_expansion else
+000018c0: 2027 270a 2020 2020 2020 2020 7265 7475   ''.        retu
+000018d0: 726e 206e 6578 7428 7072 6566 6978 5f73  rn next(prefix_s
+000018e0: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+000018f0: 7229 202b 2076 6172 5f6e 616d 655f 7069  r) + var_name_pi
+00001900: 6563 6520 2b20 7661 6c75 655f 7061 6972  ece + value_pair
+00001910: 5f65 7175 616c 7320 2b20 6974 656d 5f76  _equals + item_v
+00001920: 616c 7565 0a0a 2020 2020 4063 6c61 7373  alue..    @class
+00001930: 6d65 7468 6f64 0a20 2020 2064 6566 205f  method.    def _
+00001940: 5f72 6566 3635 3730 5f6c 6973 745f 6578  _ref6570_list_ex
+00001950: 7061 6e73 696f 6e28 0a20 2020 2020 2020  pansion(.       
+00001960: 2063 6c73 2c0a 2020 2020 2020 2020 7661   cls,.        va
+00001970: 7269 6162 6c65 5f6e 616d 653a 2073 7472  riable_name: str
+00001980: 2c0a 2020 2020 2020 2020 696e 5f64 6174  ,.        in_dat
+00001990: 613a 2074 7970 696e 672e 416e 792c 0a20  a: typing.Any,. 
+000019a0: 2020 2020 2020 2065 7870 6c6f 6465 3a20         explode: 
+000019b0: 626f 6f6c 2c0a 2020 2020 2020 2020 7065  bool,.        pe
+000019c0: 7263 656e 745f 656e 636f 6465 3a20 626f  rcent_encode: bo
+000019d0: 6f6c 2c0a 2020 2020 2020 2020 7072 6566  ol,.        pref
+000019e0: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+000019f0: 7261 746f 723a 2050 7265 6669 7853 6570  rator: PrefixSep
+00001a00: 6172 6174 6f72 4974 6572 6174 6f72 2c0a  aratorIterator,.
+00001a10: 2020 2020 2020 2020 7661 725f 6e61 6d65          var_name
+00001a20: 5f70 6965 6365 3a20 7374 722c 0a20 2020  _piece: str,.   
+00001a30: 2020 2020 206e 616d 6564 5f70 6172 616d       named_param
+00001a40: 6574 6572 5f65 7870 616e 7369 6f6e 3a20  eter_expansion: 
+00001a50: 626f 6f6c 0a20 2020 2029 202d 3e20 7374  bool.    ) -> st
+00001a60: 723a 0a20 2020 2020 2020 2069 7465 6d5f  r:.        item_
+00001a70: 7661 6c75 6573 203d 205b 636c 732e 5f5f  values = [cls.__
+00001a80: 7265 6636 3537 305f 6974 656d 5f76 616c  ref6570_item_val
+00001a90: 7565 2876 2c20 7065 7263 656e 745f 656e  ue(v, percent_en
+00001aa0: 636f 6465 2920 666f 7220 7620 696e 2069  code) for v in i
+00001ab0: 6e5f 6461 7461 5d0a 2020 2020 2020 2020  n_data].        
+00001ac0: 6974 656d 5f76 616c 7565 7320 3d20 5b76  item_values = [v
+00001ad0: 2066 6f72 2076 2069 6e20 6974 656d 5f76   for v in item_v
+00001ae0: 616c 7565 7320 6966 2076 2069 7320 6e6f  alues if v is no
+00001af0: 7420 4e6f 6e65 5d0a 2020 2020 2020 2020  t None].        
+00001b00: 6966 206e 6f74 2069 7465 6d5f 7661 6c75  if not item_valu
+00001b10: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00001b20: 2320 6967 6e6f 7265 6420 6279 2074 6865  # ignored by the
+00001b30: 2065 7870 616e 7369 6f6e 2070 726f 6365   expansion proce
+00001b40: 7373 2068 7474 7073 3a2f 2f64 6174 6174  ss https://datat
+00001b50: 7261 636b 6572 2e69 6574 662e 6f72 672f  racker.ietf.org/
+00001b60: 646f 632f 6874 6d6c 2f72 6663 3635 3730  doc/html/rfc6570
+00001b70: 2373 6563 7469 6f6e 2d33 2e32 2e31 0a20  #section-3.2.1. 
+00001b80: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001b90: 6e20 2222 0a20 2020 2020 2020 2076 616c  n "".        val
+00001ba0: 7565 5f70 6169 725f 6571 7561 6c73 203d  ue_pair_equals =
+00001bb0: 2027 3d27 2069 6620 6e61 6d65 645f 7061   '=' if named_pa
+00001bc0: 7261 6d65 7465 725f 6578 7061 6e73 696f  rameter_expansio
+00001bd0: 6e20 656c 7365 2027 270a 2020 2020 2020  n else ''.      
+00001be0: 2020 6966 206e 6f74 2065 7870 6c6f 6465    if not explode
+00001bf0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00001c00: 7475 726e 2028 0a20 2020 2020 2020 2020  turn (.         
+00001c10: 2020 2020 2020 206e 6578 7428 7072 6566         next(pref
+00001c20: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+00001c30: 7261 746f 7229 202b 0a20 2020 2020 2020  rator) +.       
+00001c40: 2020 2020 2020 2020 2076 6172 5f6e 616d           var_nam
+00001c50: 655f 7069 6563 6520 2b0a 2020 2020 2020  e_piece +.      
+00001c60: 2020 2020 2020 2020 2020 7661 6c75 655f            value_
+00001c70: 7061 6972 5f65 7175 616c 7320 2b0a 2020  pair_equals +.  
+00001c80: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001c90: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+00001ca0: 7465 7261 746f 722e 6974 656d 5f73 6570  terator.item_sep
+00001cb0: 6172 6174 6f72 2e6a 6f69 6e28 6974 656d  arator.join(item
+00001cc0: 5f76 616c 7565 7329 0a20 2020 2020 2020  _values).       
+00001cd0: 2020 2020 2029 0a20 2020 2020 2020 2023       ).        #
+00001ce0: 2065 7870 6c6f 6465 640a 2020 2020 2020   exploded.      
+00001cf0: 2020 7265 7475 726e 206e 6578 7428 7072    return next(pr
+00001d00: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+00001d10: 7465 7261 746f 7229 202b 206e 6578 7428  terator) + next(
+00001d20: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
+00001d30: 5f69 7465 7261 746f 7229 2e6a 6f69 6e28  _iterator).join(
+00001d40: 0a20 2020 2020 2020 2020 2020 205b 7661  .            [va
+00001d50: 725f 6e61 6d65 5f70 6965 6365 202b 2076  r_name_piece + v
+00001d60: 616c 7565 5f70 6169 725f 6571 7561 6c73  alue_pair_equals
+00001d70: 202b 2076 616c 2066 6f72 2076 616c 2069   + val for val i
+00001d80: 6e20 6974 656d 5f76 616c 7565 735d 0a20  n item_values]. 
+00001d90: 2020 2020 2020 2029 0a0a 2020 2020 4063         )..    @c
+00001da0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+00001db0: 6566 205f 5f72 6566 3635 3730 5f64 6963  ef __ref6570_dic
+00001dc0: 745f 6578 7061 6e73 696f 6e28 0a20 2020  t_expansion(.   
+00001dd0: 2020 2020 2063 6c73 2c0a 2020 2020 2020       cls,.      
+00001de0: 2020 7661 7269 6162 6c65 5f6e 616d 653a    variable_name:
+00001df0: 2073 7472 2c0a 2020 2020 2020 2020 696e   str,.        in
+00001e00: 5f64 6174 613a 2074 7970 696e 672e 416e  _data: typing.An
+00001e10: 792c 0a20 2020 2020 2020 2065 7870 6c6f  y,.        explo
+00001e20: 6465 3a20 626f 6f6c 2c0a 2020 2020 2020  de: bool,.      
+00001e30: 2020 7065 7263 656e 745f 656e 636f 6465    percent_encode
+00001e40: 3a20 626f 6f6c 2c0a 2020 2020 2020 2020  : bool,.        
+00001e50: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
+00001e60: 5f69 7465 7261 746f 723a 2050 7265 6669  _iterator: Prefi
+00001e70: 7853 6570 6172 6174 6f72 4974 6572 6174  xSeparatorIterat
+00001e80: 6f72 2c0a 2020 2020 2020 2020 7661 725f  or,.        var_
+00001e90: 6e61 6d65 5f70 6965 6365 3a20 7374 722c  name_piece: str,
+00001ea0: 0a20 2020 2020 2020 206e 616d 6564 5f70  .        named_p
+00001eb0: 6172 616d 6574 6572 5f65 7870 616e 7369  arameter_expansi
+00001ec0: 6f6e 3a20 626f 6f6c 0a20 2020 2029 202d  on: bool.    ) -
+00001ed0: 3e20 7374 723a 0a20 2020 2020 2020 2069  > str:.        i
+00001ee0: 6e5f 6461 7461 5f74 7261 6e73 666f 726d  n_data_transform
+00001ef0: 6564 203d 207b 6b65 793a 2063 6c73 2e5f  ed = {key: cls._
+00001f00: 5f72 6566 3635 3730 5f69 7465 6d5f 7661  _ref6570_item_va
+00001f10: 6c75 6528 7661 6c2c 2070 6572 6365 6e74  lue(val, percent
+00001f20: 5f65 6e63 6f64 6529 2066 6f72 206b 6579  _encode) for key
+00001f30: 2c20 7661 6c20 696e 2069 6e5f 6461 7461  , val in in_data
+00001f40: 2e69 7465 6d73 2829 7d0a 2020 2020 2020  .items()}.      
+00001f50: 2020 696e 5f64 6174 615f 7472 616e 7366    in_data_transf
+00001f60: 6f72 6d65 6420 3d20 7b6b 6579 3a20 7661  ormed = {key: va
+00001f70: 6c20 666f 7220 6b65 792c 2076 616c 2069  l for key, val i
+00001f80: 6e20 696e 5f64 6174 615f 7472 616e 7366  n in_data_transf
+00001f90: 6f72 6d65 642e 6974 656d 7328 2920 6966  ormed.items() if
+00001fa0: 2076 616c 2069 7320 6e6f 7420 4e6f 6e65   val is not None
+00001fb0: 7d0a 2020 2020 2020 2020 6966 206e 6f74  }.        if not
+00001fc0: 2069 6e5f 6461 7461 5f74 7261 6e73 666f   in_data_transfo
+00001fd0: 726d 6564 3a0a 2020 2020 2020 2020 2020  rmed:.          
+00001fe0: 2020 2320 6967 6e6f 7265 6420 6279 2074    # ignored by t
+00001ff0: 6865 2065 7870 616e 7369 6f6e 2070 726f  he expansion pro
+00002000: 6365 7373 2068 7474 7073 3a2f 2f64 6174  cess https://dat
+00002010: 6174 7261 636b 6572 2e69 6574 662e 6f72  atracker.ietf.or
+00002020: 672f 646f 632f 6874 6d6c 2f72 6663 3635  g/doc/html/rfc65
+00002030: 3730 2373 6563 7469 6f6e 2d33 2e32 2e31  70#section-3.2.1
+00002040: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00002050: 7572 6e20 2222 0a20 2020 2020 2020 2076  urn "".        v
+00002060: 616c 7565 5f70 6169 725f 6571 7561 6c73  alue_pair_equals
+00002070: 203d 2027 3d27 2069 6620 6e61 6d65 645f   = '=' if named_
+00002080: 7061 7261 6d65 7465 725f 6578 7061 6e73  parameter_expans
+00002090: 696f 6e20 656c 7365 2027 270a 2020 2020  ion else ''.    
+000020a0: 2020 2020 6966 206e 6f74 2065 7870 6c6f      if not explo
+000020b0: 6465 3a0a 2020 2020 2020 2020 2020 2020  de:.            
+000020c0: 7265 7475 726e 2028 0a20 2020 2020 2020  return (.       
+000020d0: 2020 2020 2020 2020 206e 6578 7428 7072           next(pr
+000020e0: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+000020f0: 7465 7261 746f 7229 202b 0a20 2020 2020  terator) +.     
+00002100: 2020 2020 2020 2020 2020 2076 6172 5f6e             var_n
+00002110: 616d 655f 7069 6563 6520 2b20 7661 6c75  ame_piece + valu
+00002120: 655f 7061 6972 5f65 7175 616c 7320 2b0a  e_pair_equals +.
+00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002140: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
+00002150: 5f69 7465 7261 746f 722e 6974 656d 5f73  _iterator.item_s
+00002160: 6570 6172 6174 6f72 2e6a 6f69 6e28 0a20  eparator.join(. 
+00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002180: 2020 2070 7265 6669 785f 7365 7061 7261     prefix_separa
+00002190: 746f 725f 6974 6572 6174 6f72 2e69 7465  tor_iterator.ite
+000021a0: 6d5f 7365 7061 7261 746f 722e 6a6f 696e  m_separator.join
+000021b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000021c0: 2020 2020 2020 2020 2020 6974 656d 5f70            item_p
+000021d0: 6169 720a 2020 2020 2020 2020 2020 2020  air.            
+000021e0: 2020 2020 2020 2020 2920 666f 7220 6974          ) for it
+000021f0: 656d 5f70 6169 7220 696e 2069 6e5f 6461  em_pair in in_da
+00002200: 7461 5f74 7261 6e73 666f 726d 6564 2e69  ta_transformed.i
+00002210: 7465 6d73 2829 0a20 2020 2020 2020 2020  tems().         
+00002220: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00002230: 2020 2020 2029 0a20 2020 2020 2020 2023       ).        #
+00002240: 2065 7870 6c6f 6465 640a 2020 2020 2020   exploded.      
+00002250: 2020 7265 7475 726e 206e 6578 7428 7072    return next(pr
+00002260: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+00002270: 7465 7261 746f 7229 202b 206e 6578 7428  terator) + next(
+00002280: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
+00002290: 5f69 7465 7261 746f 7229 2e6a 6f69 6e28  _iterator).join(
+000022a0: 0a20 2020 2020 2020 2020 2020 205b 6b65  .            [ke
+000022b0: 7920 2b20 273d 2720 2b20 7661 6c20 666f  y + '=' + val fo
+000022c0: 7220 6b65 792c 2076 616c 2069 6e20 696e  r key, val in in
+000022d0: 5f64 6174 615f 7472 616e 7366 6f72 6d65  _data_transforme
+000022e0: 642e 6974 656d 7328 295d 0a20 2020 2020  d.items()].     
+000022f0: 2020 2029 0a0a 2020 2020 4063 6c61 7373     )..    @class
+00002300: 6d65 7468 6f64 0a20 2020 2064 6566 205f  method.    def _
+00002310: 7265 6636 3537 305f 6578 7061 6e73 696f  ref6570_expansio
+00002320: 6e28 0a20 2020 2020 2020 2063 6c73 2c0a  n(.        cls,.
+00002330: 2020 2020 2020 2020 7661 7269 6162 6c65          variable
+00002340: 5f6e 616d 653a 2073 7472 2c0a 2020 2020  _name: str,.    
+00002350: 2020 2020 696e 5f64 6174 613a 2074 7970      in_data: typ
+00002360: 696e 672e 416e 792c 0a20 2020 2020 2020  ing.Any,.       
+00002370: 2065 7870 6c6f 6465 3a20 626f 6f6c 2c0a   explode: bool,.
+00002380: 2020 2020 2020 2020 7065 7263 656e 745f          percent_
+00002390: 656e 636f 6465 3a20 626f 6f6c 2c0a 2020  encode: bool,.  
+000023a0: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
+000023b0: 6172 6174 6f72 5f69 7465 7261 746f 723a  arator_iterator:
+000023c0: 2050 7265 6669 7853 6570 6172 6174 6f72   PrefixSeparator
+000023d0: 4974 6572 6174 6f72 0a20 2020 2029 202d  Iterator.    ) -
+000023e0: 3e20 7374 723a 0a20 2020 2020 2020 2022  > str:.        "
+000023f0: 2222 0a20 2020 2020 2020 2053 6570 6172  "".        Separ
+00002400: 6174 6f72 2069 7320 666f 7220 7365 7061  ator is for sepa
+00002410: 7261 7465 2076 6172 6961 626c 6573 206c  rate variables l
+00002420: 696b 6520 6469 6374 2077 6974 6820 6578  ike dict with ex
+00002430: 706c 6f64 6520 7472 7565 2c20 6e6f 7420  plode true, not 
+00002440: 666f 7220 6172 7261 7920 6974 656d 2073  for array item s
+00002450: 6570 6172 6174 696f 6e0a 2020 2020 2020  eparation.      
+00002460: 2020 2222 220a 2020 2020 2020 2020 6e61    """.        na
+00002470: 6d65 645f 7061 7261 6d65 7465 725f 6578  med_parameter_ex
+00002480: 7061 6e73 696f 6e20 3d20 7072 6566 6978  pansion = prefix
+00002490: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
+000024a0: 746f 722e 7365 7061 7261 746f 7220 696e  tor.separator in
+000024b0: 207b 2726 272c 2027 3b27 7d0a 2020 2020   {'&', ';'}.    
+000024c0: 2020 2020 7661 725f 6e61 6d65 5f70 6965      var_name_pie
+000024d0: 6365 203d 2076 6172 6961 626c 655f 6e61  ce = variable_na
+000024e0: 6d65 2069 6620 6e61 6d65 645f 7061 7261  me if named_para
+000024f0: 6d65 7465 725f 6578 7061 6e73 696f 6e20  meter_expansion 
+00002500: 656c 7365 2027 270a 2020 2020 2020 2020  else ''.        
+00002510: 6966 2074 7970 6528 696e 5f64 6174 6129  if type(in_data)
+00002520: 2069 6e20 7b73 7472 2c20 666c 6f61 742c   in {str, float,
+00002530: 2069 6e74 7d3a 0a20 2020 2020 2020 2020   int}:.         
+00002540: 2020 2072 6574 7572 6e20 636c 732e 5f5f     return cls.__
+00002550: 7265 6636 3537 305f 7374 725f 666c 6f61  ref6570_str_floa
+00002560: 745f 696e 745f 6578 7061 6e73 696f 6e28  t_int_expansion(
+00002570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002580: 2076 6172 6961 626c 655f 6e61 6d65 2c0a   variable_name,.
+00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025a0: 696e 5f64 6174 612c 0a20 2020 2020 2020  in_data,.       
+000025b0: 2020 2020 2020 2020 2065 7870 6c6f 6465           explode
+000025c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000025d0: 2020 7065 7263 656e 745f 656e 636f 6465    percent_encode
+000025e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000025f0: 2020 7072 6566 6978 5f73 6570 6172 6174    prefix_separat
+00002600: 6f72 5f69 7465 7261 746f 722c 0a20 2020  or_iterator,.   
+00002610: 2020 2020 2020 2020 2020 2020 2076 6172               var
+00002620: 5f6e 616d 655f 7069 6563 652c 0a20 2020  _name_piece,.   
+00002630: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+00002640: 6564 5f70 6172 616d 6574 6572 5f65 7870  ed_parameter_exp
+00002650: 616e 7369 6f6e 0a20 2020 2020 2020 2020  ansion.         
+00002660: 2020 2029 0a20 2020 2020 2020 2065 6c69     ).        eli
+00002670: 6620 6973 696e 7374 616e 6365 2869 6e5f  f isinstance(in_
+00002680: 6461 7461 2c20 6e6f 6e65 5f74 7970 6529  data, none_type)
+00002690: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+000026a0: 6967 6e6f 7265 6420 6279 2074 6865 2065  ignored by the e
+000026b0: 7870 616e 7369 6f6e 2070 726f 6365 7373  xpansion process
+000026c0: 2068 7474 7073 3a2f 2f64 6174 6174 7261   https://datatra
+000026d0: 636b 6572 2e69 6574 662e 6f72 672f 646f  cker.ietf.org/do
+000026e0: 632f 6874 6d6c 2f72 6663 3635 3730 2373  c/html/rfc6570#s
+000026f0: 6563 7469 6f6e 2d33 2e32 2e31 0a20 2020  ection-3.2.1.   
+00002700: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00002710: 2222 0a20 2020 2020 2020 2065 6c69 6620  "".        elif 
+00002720: 6973 696e 7374 616e 6365 2869 6e5f 6461  isinstance(in_da
+00002730: 7461 2c20 6c69 7374 293a 0a20 2020 2020  ta, list):.     
+00002740: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
+00002750: 732e 5f5f 7265 6636 3537 305f 6c69 7374  s.__ref6570_list
+00002760: 5f65 7870 616e 7369 6f6e 280a 2020 2020  _expansion(.    
+00002770: 2020 2020 2020 2020 2020 2020 7661 7269              vari
+00002780: 6162 6c65 5f6e 616d 652c 0a20 2020 2020  able_name,.     
+00002790: 2020 2020 2020 2020 2020 2069 6e5f 6461             in_da
+000027a0: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+000027b0: 2020 2020 6578 706c 6f64 652c 0a20 2020      explode,.   
+000027c0: 2020 2020 2020 2020 2020 2020 2070 6572               per
+000027d0: 6365 6e74 5f65 6e63 6f64 652c 0a20 2020  cent_encode,.   
+000027e0: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+000027f0: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
+00002800: 6572 6174 6f72 2c0a 2020 2020 2020 2020  erator,.        
+00002810: 2020 2020 2020 2020 7661 725f 6e61 6d65          var_name
+00002820: 5f70 6965 6365 2c0a 2020 2020 2020 2020  _piece,.        
+00002830: 2020 2020 2020 2020 6e61 6d65 645f 7061          named_pa
+00002840: 7261 6d65 7465 725f 6578 7061 6e73 696f  rameter_expansio
+00002850: 6e0a 2020 2020 2020 2020 2020 2020 290a  n.            ).
+00002860: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+00002870: 6e73 7461 6e63 6528 696e 5f64 6174 612c  nstance(in_data,
+00002880: 2064 6963 7429 3a0a 2020 2020 2020 2020   dict):.        
+00002890: 2020 2020 7265 7475 726e 2063 6c73 2e5f      return cls._
+000028a0: 5f72 6566 3635 3730 5f64 6963 745f 6578  _ref6570_dict_ex
+000028b0: 7061 6e73 696f 6e28 0a20 2020 2020 2020  pansion(.       
+000028c0: 2020 2020 2020 2020 2076 6172 6961 626c           variabl
+000028d0: 655f 6e61 6d65 2c0a 2020 2020 2020 2020  e_name,.        
+000028e0: 2020 2020 2020 2020 696e 5f64 6174 612c          in_data,
+000028f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002900: 2065 7870 6c6f 6465 2c0a 2020 2020 2020   explode,.      
+00002910: 2020 2020 2020 2020 2020 7065 7263 656e            percen
+00002920: 745f 656e 636f 6465 2c0a 2020 2020 2020  t_encode,.      
+00002930: 2020 2020 2020 2020 2020 7072 6566 6978            prefix
+00002940: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
+00002950: 746f 722c 0a20 2020 2020 2020 2020 2020  tor,.           
+00002960: 2020 2020 2076 6172 5f6e 616d 655f 7069       var_name_pi
+00002970: 6563 652c 0a20 2020 2020 2020 2020 2020  ece,.           
+00002980: 2020 2020 206e 616d 6564 5f70 6172 616d       named_param
+00002990: 6574 6572 5f65 7870 616e 7369 6f6e 0a20  eter_expansion. 
+000029a0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000029b0: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+000029c0: 616e 6365 2869 6e5f 6461 7461 2c20 626f  ance(in_data, bo
+000029d0: 6f6c 293a 0a20 2020 2020 2020 2020 2020  ol):.           
+000029e0: 2072 6574 7572 6e20 636c 732e 5f5f 6b6f   return cls.__ko
+000029f0: 6e66 6967 5f62 6f6f 6c5f 6578 7061 6e73  nfig_bool_expans
+00002a00: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+00002a10: 2020 2020 2069 6e5f 6461 7461 2c0a 2020       in_data,.  
+00002a20: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00002a30: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+00002a40: 7465 7261 746f 722c 0a20 2020 2020 2020  terator,.       
+00002a50: 2020 2020 2020 2020 2076 6172 5f6e 616d           var_nam
+00002a60: 655f 7069 6563 652c 0a20 2020 2020 2020  e_piece,.       
+00002a70: 2020 2020 2020 2020 206e 616d 6564 5f70           named_p
+00002a80: 6172 616d 6574 6572 5f65 7870 616e 7369  arameter_expansi
+00002a90: 6f6e 0a20 2020 2020 2020 2020 2020 2029  on.            )
+00002aa0: 0a20 2020 2020 2020 2023 2062 7974 6573  .        # bytes
+00002ab0: 2c20 6574 630a 2020 2020 2020 2020 7261  , etc.        ra
+00002ac0: 6973 6520 4170 6956 616c 7565 4572 726f  ise ApiValueErro
+00002ad0: 7228 2755 6e61 626c 6520 746f 2067 656e  r('Unable to gen
+00002ae0: 6572 6174 6520 6120 7265 6636 3537 3020  erate a ref6570 
+00002af0: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
+00002b00: 6620 7b7d 272e 666f 726d 6174 2869 6e5f  f {}'.format(in_
+00002b10: 6461 7461 2929 0a0a 0a63 6c61 7373 2053  data))...class S
+00002b20: 7479 6c65 466f 726d 5365 7269 616c 697a  tyleFormSerializ
+00002b30: 6572 2850 6172 616d 6574 6572 5365 7269  er(ParameterSeri
+00002b40: 616c 697a 6572 4261 7365 293a 0a20 2020  alizerBase):.   
+00002b50: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00002b60: 2020 6465 6620 5f67 6574 5f64 6566 6175    def _get_defau
+00002b70: 6c74 5f65 7870 6c6f 6465 2863 6c73 2c20  lt_explode(cls, 
+00002b80: 7374 796c 653a 2050 6172 616d 6574 6572  style: Parameter
+00002b90: 5374 796c 6529 202d 3e20 626f 6f6c 3a0a  Style) -> bool:.
+00002ba0: 2020 2020 2020 2020 6966 2073 7479 6c65          if style
+00002bb0: 2069 7320 5061 7261 6d65 7465 7253 7479   is ParameterSty
+00002bc0: 6c65 2e46 4f52 4d3a 0a20 2020 2020 2020  le.FORM:.       
+00002bd0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00002be0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002bf0: 7375 7065 7228 292e 5f67 6574 5f64 6566  super()._get_def
+00002c00: 6175 6c74 5f65 7870 6c6f 6465 2873 7479  ault_explode(sty
+00002c10: 6c65 290a 0a20 2020 2064 6566 205f 7365  le)..    def _se
+00002c20: 7269 616c 697a 655f 666f 726d 280a 2020  rialize_form(.  
+00002c30: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00002c40: 2020 2020 696e 5f64 6174 613a 2074 7970      in_data: typ
+00002c50: 696e 672e 556e 696f 6e5b 4e6f 6e65 2c20  ing.Union[None, 
+00002c60: 696e 742c 2066 6c6f 6174 2c20 7374 722c  int, float, str,
+00002c70: 2062 6f6f 6c2c 2064 6963 742c 206c 6973   bool, dict, lis
+00002c80: 745d 2c0a 2020 2020 2020 2020 6e61 6d65  t],.        name
+00002c90: 3a20 7374 722c 0a20 2020 2020 2020 2065  : str,.        e
+00002ca0: 7870 6c6f 6465 3a20 626f 6f6c 2c0a 2020  xplode: bool,.  
+00002cb0: 2020 2020 2020 7065 7263 656e 745f 656e        percent_en
+00002cc0: 636f 6465 3a20 626f 6f6c 2c0a 2020 2020  code: bool,.    
+00002cd0: 2020 2020 7072 6566 6978 5f73 6570 6172      prefix_separ
+00002ce0: 6174 6f72 5f69 7465 7261 746f 723a 2074  ator_iterator: t
+00002cf0: 7970 696e 672e 4f70 7469 6f6e 616c 5b50  yping.Optional[P
+00002d00: 7265 6669 7853 6570 6172 6174 6f72 4974  refixSeparatorIt
+00002d10: 6572 6174 6f72 5d20 3d20 4e6f 6e65 0a20  erator] = None. 
+00002d20: 2020 2029 202d 3e20 7374 723a 0a20 2020     ) -> str:.   
+00002d30: 2020 2020 2069 6620 7072 6566 6978 5f73       if prefix_s
+00002d40: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+00002d50: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
+00002d60: 2020 2020 2020 2070 7265 6669 785f 7365         prefix_se
+00002d70: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
+00002d80: 203d 2050 7265 6669 7853 6570 6172 6174   = PrefixSeparat
+00002d90: 6f72 4974 6572 6174 6f72 2827 272c 2027  orIterator('', '
+00002da0: 2627 290a 2020 2020 2020 2020 7265 7475  &').        retu
+00002db0: 726e 2073 656c 662e 5f72 6566 3635 3730  rn self._ref6570
+00002dc0: 5f65 7870 616e 7369 6f6e 280a 2020 2020  _expansion(.    
+00002dd0: 2020 2020 2020 2020 7661 7269 6162 6c65          variable
+00002de0: 5f6e 616d 653d 6e61 6d65 2c0a 2020 2020  _name=name,.    
+00002df0: 2020 2020 2020 2020 696e 5f64 6174 613d          in_data=
+00002e00: 696e 5f64 6174 612c 0a20 2020 2020 2020  in_data,.       
+00002e10: 2020 2020 2065 7870 6c6f 6465 3d65 7870       explode=exp
+00002e20: 6c6f 6465 2c0a 2020 2020 2020 2020 2020  lode,.          
+00002e30: 2020 7065 7263 656e 745f 656e 636f 6465    percent_encode
+00002e40: 3d70 6572 6365 6e74 5f65 6e63 6f64 652c  =percent_encode,
+00002e50: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
+00002e60: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
+00002e70: 6572 6174 6f72 3d70 7265 6669 785f 7365  erator=prefix_se
+00002e80: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
+00002e90: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
+00002ea0: 7373 2053 7479 6c65 5369 6d70 6c65 5365  ss StyleSimpleSe
+00002eb0: 7269 616c 697a 6572 2850 6172 616d 6574  rializer(Paramet
+00002ec0: 6572 5365 7269 616c 697a 6572 4261 7365  erSerializerBase
+00002ed0: 293a 0a0a 2020 2020 6465 6620 5f73 6572  ):..    def _ser
+00002ee0: 6961 6c69 7a65 5f73 696d 706c 6528 0a20  ialize_simple(. 
+00002ef0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00002f00: 2020 2020 2069 6e5f 6461 7461 3a20 7479       in_data: ty
+00002f10: 7069 6e67 2e55 6e69 6f6e 5b4e 6f6e 652c  ping.Union[None,
+00002f20: 2069 6e74 2c20 666c 6f61 742c 2073 7472   int, float, str
+00002f30: 2c20 626f 6f6c 2c20 6469 6374 2c20 6c69  , bool, dict, li
+00002f40: 7374 5d2c 0a20 2020 2020 2020 206e 616d  st],.        nam
+00002f50: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
+00002f60: 6578 706c 6f64 653a 2062 6f6f 6c2c 0a20  explode: bool,. 
+00002f70: 2020 2020 2020 2070 6572 6365 6e74 5f65         percent_e
+00002f80: 6e63 6f64 653a 2062 6f6f 6c0a 2020 2020  ncode: bool.    
+00002f90: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
+00002fa0: 2020 7072 6566 6978 5f73 6570 6172 6174    prefix_separat
+00002fb0: 6f72 5f69 7465 7261 746f 7220 3d20 5072  or_iterator = Pr
+00002fc0: 6566 6978 5365 7061 7261 746f 7249 7465  efixSeparatorIte
+00002fd0: 7261 746f 7228 2727 2c20 272c 2729 0a20  rator('', ','). 
+00002fe0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00002ff0: 6c66 2e5f 7265 6636 3537 305f 6578 7061  lf._ref6570_expa
+00003000: 6e73 696f 6e28 0a20 2020 2020 2020 2020  nsion(.         
+00003010: 2020 2076 6172 6961 626c 655f 6e61 6d65     variable_name
+00003020: 3d6e 616d 652c 0a20 2020 2020 2020 2020  =name,.         
+00003030: 2020 2069 6e5f 6461 7461 3d69 6e5f 6461     in_data=in_da
+00003040: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+00003050: 6578 706c 6f64 653d 6578 706c 6f64 652c  explode=explode,
+00003060: 0a20 2020 2020 2020 2020 2020 2070 6572  .            per
+00003070: 6365 6e74 5f65 6e63 6f64 653d 7065 7263  cent_encode=perc
+00003080: 656e 745f 656e 636f 6465 2c0a 2020 2020  ent_encode,.    
+00003090: 2020 2020 2020 2020 7072 6566 6978 5f73          prefix_s
+000030a0: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+000030b0: 723d 7072 6566 6978 5f73 6570 6172 6174  r=prefix_separat
+000030c0: 6f72 5f69 7465 7261 746f 720a 2020 2020  or_iterator.    
+000030d0: 2020 2020 290a 0a0a 636c 6173 7320 4a53      )...class JS
+000030e0: 4f4e 4465 7465 6374 6f72 3a0a 2020 2020  ONDetector:.    
+000030f0: 2222 220a 2020 2020 576f 726b 7320 666f  """.    Works fo
+00003100: 723a 0a20 2020 2061 7070 6c69 6361 7469  r:.    applicati
+00003110: 6f6e 2f6a 736f 6e0a 2020 2020 6170 706c  on/json.    appl
+00003120: 6963 6174 696f 6e2f 6a73 6f6e 3b20 6368  ication/json; ch
+00003130: 6172 7365 743d 5554 462d 380a 2020 2020  arset=UTF-8.    
+00003140: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+00003150: 2d70 6174 6368 2b6a 736f 6e0a 2020 2020  -patch+json.    
+00003160: 6170 706c 6963 6174 696f 6e2f 6765 6f2b  application/geo+
+00003170: 6a73 6f6e 0a20 2020 2022 2222 0a20 2020  json.    """.   
+00003180: 205f 5f6a 736f 6e5f 636f 6e74 656e 745f   __json_content_
+00003190: 7479 7065 5f70 6174 7465 726e 203d 2072  type_pattern = r
+000031a0: 652e 636f 6d70 696c 6528 2261 7070 6c69  e.compile("appli
+000031b0: 6361 7469 6f6e 2f5b 5e2b 5d2a 5b2b 5d3f  cation/[^+]*[+]?
+000031c0: 286a 736f 6e29 3b3f 2e2a 2229 0a0a 2020  (json);?.*")..  
+000031d0: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+000031e0: 2020 2064 6566 205f 636f 6e74 656e 745f     def _content_
+000031f0: 7479 7065 5f69 735f 6a73 6f6e 2863 6c73  type_is_json(cls
+00003200: 2c20 636f 6e74 656e 745f 7479 7065 3a20  , content_type: 
+00003210: 7374 7229 202d 3e20 626f 6f6c 3a0a 2020  str) -> bool:.  
+00003220: 2020 2020 2020 6966 2063 6c73 2e5f 5f6a        if cls.__j
+00003230: 736f 6e5f 636f 6e74 656e 745f 7479 7065  son_content_type
+00003240: 5f70 6174 7465 726e 2e6d 6174 6368 2863  _pattern.match(c
+00003250: 6f6e 7465 6e74 5f74 7970 6529 3a0a 2020  ontent_type):.  
+00003260: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00003270: 2054 7275 650a 2020 2020 2020 2020 7265   True.        re
+00003280: 7475 726e 2046 616c 7365 0a0a 0a40 6461  turn False...@da
+00003290: 7461 636c 6173 730a 636c 6173 7320 5061  taclass.class Pa
+000032a0: 7261 6d65 7465 7242 6173 6528 4a53 4f4e  rameterBase(JSON
+000032b0: 4465 7465 6374 6f72 293a 0a20 2020 206e  Detector):.    n
+000032c0: 616d 653a 2073 7472 0a20 2020 2069 6e5f  ame: str.    in_
+000032d0: 7479 7065 3a20 5061 7261 6d65 7465 7249  type: ParameterI
+000032e0: 6e54 7970 650a 2020 2020 7265 7175 6972  nType.    requir
+000032f0: 6564 3a20 626f 6f6c 0a20 2020 2073 7479  ed: bool.    sty
+00003300: 6c65 3a20 7479 7069 6e67 2e4f 7074 696f  le: typing.Optio
+00003310: 6e61 6c5b 5061 7261 6d65 7465 7253 7479  nal[ParameterSty
+00003320: 6c65 5d0a 2020 2020 6578 706c 6f64 653a  le].    explode:
+00003330: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00003340: 5b62 6f6f 6c5d 0a20 2020 2061 6c6c 6f77  [bool].    allow
+00003350: 5f72 6573 6572 7665 643a 2074 7970 696e  _reserved: typin
+00003360: 672e 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  g.Optional[bool]
+00003370: 0a20 2020 2073 6368 656d 613a 2074 7970  .    schema: typ
+00003380: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+00003390: 696e 672e 5479 7065 5b53 6368 656d 615d  ing.Type[Schema]
+000033a0: 5d0a 2020 2020 636f 6e74 656e 743a 2074  ].    content: t
+000033b0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+000033c0: 7970 696e 672e 4469 6374 5b73 7472 2c20  yping.Dict[str, 
+000033d0: 7479 7069 6e67 2e54 7970 655b 5363 6865  typing.Type[Sche
+000033e0: 6d61 5d5d 5d0a 0a20 2020 205f 5f73 7479  ma]]]..    __sty
+000033f0: 6c65 5f74 6f5f 696e 5f74 7970 6520 3d20  le_to_in_type = 
+00003400: 7b0a 2020 2020 2020 2020 5061 7261 6d65  {.        Parame
+00003410: 7465 7253 7479 6c65 2e4d 4154 5249 583a  terStyle.MATRIX:
+00003420: 207b 5061 7261 6d65 7465 7249 6e54 7970   {ParameterInTyp
+00003430: 652e 5041 5448 7d2c 0a20 2020 2020 2020  e.PATH},.       
+00003440: 2050 6172 616d 6574 6572 5374 796c 652e   ParameterStyle.
+00003450: 4c41 4245 4c3a 207b 5061 7261 6d65 7465  LABEL: {Paramete
+00003460: 7249 6e54 7970 652e 5041 5448 7d2c 0a20  rInType.PATH},. 
+00003470: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00003480: 5374 796c 652e 464f 524d 3a20 7b50 6172  Style.FORM: {Par
+00003490: 616d 6574 6572 496e 5479 7065 2e51 5545  ameterInType.QUE
+000034a0: 5259 2c20 5061 7261 6d65 7465 7249 6e54  RY, ParameterInT
+000034b0: 7970 652e 434f 4f4b 4945 7d2c 0a20 2020  ype.COOKIE},.   
+000034c0: 2020 2020 2050 6172 616d 6574 6572 5374       ParameterSt
+000034d0: 796c 652e 5349 4d50 4c45 3a20 7b50 6172  yle.SIMPLE: {Par
+000034e0: 616d 6574 6572 496e 5479 7065 2e50 4154  ameterInType.PAT
+000034f0: 482c 2050 6172 616d 6574 6572 496e 5479  H, ParameterInTy
+00003500: 7065 2e48 4541 4445 527d 2c0a 2020 2020  pe.HEADER},.    
+00003510: 2020 2020 5061 7261 6d65 7465 7253 7479      ParameterSty
+00003520: 6c65 2e53 5041 4345 5f44 454c 494d 4954  le.SPACE_DELIMIT
+00003530: 4544 3a20 7b50 6172 616d 6574 6572 496e  ED: {ParameterIn
+00003540: 5479 7065 2e51 5545 5259 7d2c 0a20 2020  Type.QUERY},.   
+00003550: 2020 2020 2050 6172 616d 6574 6572 5374       ParameterSt
+00003560: 796c 652e 5049 5045 5f44 454c 494d 4954  yle.PIPE_DELIMIT
+00003570: 4544 3a20 7b50 6172 616d 6574 6572 496e  ED: {ParameterIn
+00003580: 5479 7065 2e51 5545 5259 7d2c 0a20 2020  Type.QUERY},.   
+00003590: 2020 2020 2050 6172 616d 6574 6572 5374       ParameterSt
+000035a0: 796c 652e 4445 4550 5f4f 424a 4543 543a  yle.DEEP_OBJECT:
+000035b0: 207b 5061 7261 6d65 7465 7249 6e54 7970   {ParameterInTyp
+000035c0: 652e 5155 4552 597d 2c0a 2020 2020 7d0a  e.QUERY},.    }.
+000035d0: 2020 2020 5f5f 696e 5f74 7970 655f 746f      __in_type_to
+000035e0: 5f64 6566 6175 6c74 5f73 7479 6c65 203d  _default_style =
+000035f0: 207b 0a20 2020 2020 2020 2050 6172 616d   {.        Param
+00003600: 6574 6572 496e 5479 7065 2e51 5545 5259  eterInType.QUERY
+00003610: 3a20 5061 7261 6d65 7465 7253 7479 6c65  : ParameterStyle
+00003620: 2e46 4f52 4d2c 0a20 2020 2020 2020 2050  .FORM,.        P
+00003630: 6172 616d 6574 6572 496e 5479 7065 2e50  arameterInType.P
+00003640: 4154 483a 2050 6172 616d 6574 6572 5374  ATH: ParameterSt
+00003650: 796c 652e 5349 4d50 4c45 2c0a 2020 2020  yle.SIMPLE,.    
+00003660: 2020 2020 5061 7261 6d65 7465 7249 6e54      ParameterInT
+00003670: 7970 652e 4845 4144 4552 3a20 5061 7261  ype.HEADER: Para
+00003680: 6d65 7465 7253 7479 6c65 2e53 494d 504c  meterStyle.SIMPL
+00003690: 452c 0a20 2020 2020 2020 2050 6172 616d  E,.        Param
+000036a0: 6574 6572 496e 5479 7065 2e43 4f4f 4b49  eterInType.COOKI
+000036b0: 453a 2050 6172 616d 6574 6572 5374 796c  E: ParameterStyl
+000036c0: 652e 464f 524d 2c0a 2020 2020 7d0a 2020  e.FORM,.    }.  
+000036d0: 2020 5f5f 6469 7361 6c6c 6f77 6564 5f68    __disallowed_h
+000036e0: 6561 6465 725f 6e61 6d65 7320 3d20 7b27  eader_names = {'
+000036f0: 4163 6365 7074 272c 2027 436f 6e74 656e  Accept', 'Conten
+00003700: 742d 5479 7065 272c 2027 4175 7468 6f72  t-Type', 'Author
+00003710: 697a 6174 696f 6e27 7d0a 2020 2020 5f6a  ization'}.    _j
+00003720: 736f 6e5f 656e 636f 6465 7220 3d20 4a53  son_encoder = JS
+00003730: 4f4e 456e 636f 6465 7228 290a 0a20 2020  ONEncoder()..   
+00003740: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00003750: 2020 6465 6620 5f5f 7665 7269 6679 5f73    def __verify_s
+00003760: 7479 6c65 5f74 6f5f 696e 5f74 7970 6528  tyle_to_in_type(
+00003770: 636c 732c 2073 7479 6c65 3a20 7479 7069  cls, style: typi
+00003780: 6e67 2e4f 7074 696f 6e61 6c5b 5061 7261  ng.Optional[Para
+00003790: 6d65 7465 7253 7479 6c65 5d2c 2069 6e5f  meterStyle], in_
+000037a0: 7479 7065 3a20 5061 7261 6d65 7465 7249  type: ParameterI
+000037b0: 6e54 7970 6529 3a0a 2020 2020 2020 2020  nType):.        
+000037c0: 6966 2073 7479 6c65 2069 7320 4e6f 6e65  if style is None
+000037d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000037e0: 7475 726e 0a20 2020 2020 2020 2069 6e5f  turn.        in_
+000037f0: 7479 7065 5f73 6574 203d 2063 6c73 2e5f  type_set = cls._
+00003800: 5f73 7479 6c65 5f74 6f5f 696e 5f74 7970  _style_to_in_typ
+00003810: 655b 7374 796c 655d 0a20 2020 2020 2020  e[style].       
+00003820: 2069 6620 696e 5f74 7970 6520 6e6f 7420   if in_type not 
+00003830: 696e 2069 6e5f 7479 7065 5f73 6574 3a0a  in in_type_set:.
+00003840: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00003850: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+00003860: 2020 2020 2020 2020 2020 2020 2020 2749                'I
+00003870: 6e76 616c 6964 2073 7479 6c65 2061 6e64  nvalid style and
+00003880: 2069 6e5f 7479 7065 2063 6f6d 6269 6e61   in_type combina
+00003890: 7469 6f6e 2e20 466f 7220 7374 796c 653d  tion. For style=
+000038a0: 7b7d 206f 6e6c 7920 696e 5f74 7970 653d  {} only in_type=
+000038b0: 7b7d 2061 7265 2061 6c6c 6f77 6564 272e  {} are allowed'.
+000038c0: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+000038d0: 2020 2020 2020 2020 2020 2020 7374 796c              styl
+000038e0: 652c 2069 6e5f 7479 7065 5f73 6574 0a20  e, in_type_set. 
+000038f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00003900: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00003910: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00003920: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00003930: 2020 2020 2020 2020 6e61 6d65 3a20 7374          name: st
+00003940: 722c 0a20 2020 2020 2020 2069 6e5f 7479  r,.        in_ty
+00003950: 7065 3a20 5061 7261 6d65 7465 7249 6e54  pe: ParameterInT
+00003960: 7970 652c 0a20 2020 2020 2020 2072 6571  ype,.        req
+00003970: 7569 7265 643a 2062 6f6f 6c20 3d20 4661  uired: bool = Fa
+00003980: 6c73 652c 0a20 2020 2020 2020 2073 7479  lse,.        sty
+00003990: 6c65 3a20 7479 7069 6e67 2e4f 7074 696f  le: typing.Optio
+000039a0: 6e61 6c5b 5061 7261 6d65 7465 7253 7479  nal[ParameterSty
+000039b0: 6c65 5d20 3d20 4e6f 6e65 2c0a 2020 2020  le] = None,.    
+000039c0: 2020 2020 6578 706c 6f64 653a 2062 6f6f      explode: boo
+000039d0: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
+000039e0: 2020 2061 6c6c 6f77 5f72 6573 6572 7665     allow_reserve
+000039f0: 643a 2074 7970 696e 672e 4f70 7469 6f6e  d: typing.Option
+00003a00: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 652c  al[bool] = None,
+00003a10: 0a20 2020 2020 2020 2073 6368 656d 613a  .        schema:
+00003a20: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00003a30: 5b74 7970 696e 672e 5479 7065 5b53 6368  [typing.Type[Sch
+00003a40: 656d 615d 5d20 3d20 4e6f 6e65 2c0a 2020  ema]] = None,.  
+00003a50: 2020 2020 2020 636f 6e74 656e 743a 2074        content: t
+00003a60: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+00003a70: 7970 696e 672e 4469 6374 5b73 7472 2c20  yping.Dict[str, 
+00003a80: 7479 7069 6e67 2e54 7970 655b 5363 6865  typing.Type[Sche
+00003a90: 6d61 5d5d 5d20 3d20 4e6f 6e65 0a20 2020  ma]]] = None.   
+00003aa0: 2029 3a0a 2020 2020 2020 2020 6966 2073   ):.        if s
+00003ab0: 6368 656d 6120 6973 204e 6f6e 6520 616e  chema is None an
+00003ac0: 6420 636f 6e74 656e 7420 6973 204e 6f6e  d content is Non
+00003ad0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00003ae0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00003af0: 2756 616c 7565 206d 6973 7369 6e67 3b20  'Value missing; 
+00003b00: 5061 7373 2069 6e20 6569 7468 6572 2073  Pass in either s
+00003b10: 6368 656d 6120 6f72 2063 6f6e 7465 6e74  chema or content
+00003b20: 2729 0a20 2020 2020 2020 2069 6620 7363  ').        if sc
+00003b30: 6865 6d61 2061 6e64 2063 6f6e 7465 6e74  hema and content
+00003b40: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00003b50: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+00003b60: 546f 6f20 6d61 6e79 2076 616c 7565 7320  Too many values 
+00003b70: 7072 6f76 6964 6564 2e20 426f 7468 2073  provided. Both s
+00003b80: 6368 656d 6120 616e 6420 636f 6e74 656e  chema and conten
+00003b90: 7420 7765 7265 2070 726f 7669 6465 642e  t were provided.
+00003ba0: 204f 6e6c 7920 6f6e 6520 6d61 7920 6265   Only one may be
+00003bb0: 2069 6e70 7574 2729 0a20 2020 2020 2020   input').       
+00003bc0: 2069 6620 6e61 6d65 2069 6e20 7365 6c66   if name in self
+00003bd0: 2e5f 5f64 6973 616c 6c6f 7765 645f 6865  .__disallowed_he
+00003be0: 6164 6572 5f6e 616d 6573 2061 6e64 2069  ader_names and i
+00003bf0: 6e5f 7479 7065 2069 7320 5061 7261 6d65  n_type is Parame
+00003c00: 7465 7249 6e54 7970 652e 4845 4144 4552  terInType.HEADER
+00003c10: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00003c20: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+00003c30: 496e 7661 6c69 6420 6e61 6d65 2c20 6e61  Invalid name, na
+00003c40: 6d65 206d 6179 206e 6f74 2062 6520 6f6e  me may not be on
+00003c50: 6520 6f66 207b 7d27 2e66 6f72 6d61 7428  e of {}'.format(
+00003c60: 7365 6c66 2e5f 5f64 6973 616c 6c6f 7765  self.__disallowe
+00003c70: 645f 6865 6164 6572 5f6e 616d 6573 2929  d_header_names))
+00003c80: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
+00003c90: 7665 7269 6679 5f73 7479 6c65 5f74 6f5f  verify_style_to_
+00003ca0: 696e 5f74 7970 6528 7374 796c 652c 2069  in_type(style, i
+00003cb0: 6e5f 7479 7065 290a 2020 2020 2020 2020  n_type).        
+00003cc0: 6966 2063 6f6e 7465 6e74 2069 7320 4e6f  if content is No
+00003cd0: 6e65 2061 6e64 2073 7479 6c65 2069 7320  ne and style is 
+00003ce0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00003cf0: 2020 7374 796c 6520 3d20 7365 6c66 2e5f    style = self._
+00003d00: 5f69 6e5f 7479 7065 5f74 6f5f 6465 6661  _in_type_to_defa
+00003d10: 756c 745f 7374 796c 655b 696e 5f74 7970  ult_style[in_typ
+00003d20: 655d 0a20 2020 2020 2020 2069 6620 636f  e].        if co
+00003d30: 6e74 656e 7420 6973 206e 6f74 204e 6f6e  ntent is not Non
+00003d40: 6520 616e 6420 696e 5f74 7970 6520 696e  e and in_type in
+00003d50: 2073 656c 662e 5f5f 696e 5f74 7970 655f   self.__in_type_
+00003d60: 746f 5f64 6566 6175 6c74 5f73 7479 6c65  to_default_style
+00003d70: 2061 6e64 206c 656e 2863 6f6e 7465 6e74   and len(content
+00003d80: 2920 213d 2031 3a0a 2020 2020 2020 2020  ) != 1:.        
+00003d90: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00003da0: 7272 6f72 2827 496e 7661 6c69 6420 636f  rror('Invalid co
+00003db0: 6e74 656e 7420 6c65 6e67 7468 2c20 636f  ntent length, co
+00003dc0: 6e74 656e 7420 6c65 6e67 7468 206d 7573  ntent length mus
+00003dd0: 7420 6571 7561 6c20 3127 290a 2020 2020  t equal 1').    
+00003de0: 2020 2020 7365 6c66 2e69 6e5f 7479 7065      self.in_type
+00003df0: 203d 2069 6e5f 7479 7065 0a20 2020 2020   = in_type.     
+00003e00: 2020 2073 656c 662e 6e61 6d65 203d 206e     self.name = n
+00003e10: 616d 650a 2020 2020 2020 2020 7365 6c66  ame.        self
+00003e20: 2e72 6571 7569 7265 6420 3d20 7265 7175  .required = requ
+00003e30: 6972 6564 0a20 2020 2020 2020 2073 656c  ired.        sel
+00003e40: 662e 7374 796c 6520 3d20 7374 796c 650a  f.style = style.
+00003e50: 2020 2020 2020 2020 7365 6c66 2e65 7870          self.exp
+00003e60: 6c6f 6465 203d 2065 7870 6c6f 6465 0a20  lode = explode. 
+00003e70: 2020 2020 2020 2073 656c 662e 616c 6c6f         self.allo
+00003e80: 775f 7265 7365 7276 6564 203d 2061 6c6c  w_reserved = all
+00003e90: 6f77 5f72 6573 6572 7665 640a 2020 2020  ow_reserved.    
+00003ea0: 2020 2020 7365 6c66 2e73 6368 656d 6120      self.schema 
+00003eb0: 3d20 7363 6865 6d61 0a20 2020 2020 2020  = schema.       
+00003ec0: 2073 656c 662e 636f 6e74 656e 7420 3d20   self.content = 
+00003ed0: 636f 6e74 656e 740a 0a20 2020 2064 6566  content..    def
+00003ee0: 205f 7365 7269 616c 697a 655f 6a73 6f6e   _serialize_json
+00003ef0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00003f00: 2020 2020 2020 2020 696e 5f64 6174 613a          in_data:
+00003f10: 2074 7970 696e 672e 556e 696f 6e5b 4e6f   typing.Union[No
+00003f20: 6e65 2c20 696e 742c 2066 6c6f 6174 2c20  ne, int, float, 
+00003f30: 7374 722c 2062 6f6f 6c2c 2064 6963 742c  str, bool, dict,
+00003f40: 206c 6973 745d 2c0a 2020 2020 2020 2020   list],.        
+00003f50: 656c 696d 696e 6174 655f 7768 6974 6573  eliminate_whites
+00003f60: 7061 6365 3a20 626f 6f6c 203d 2046 616c  pace: bool = Fal
+00003f70: 7365 0a20 2020 2029 202d 3e20 7374 723a  se.    ) -> str:
+00003f80: 0a20 2020 2020 2020 2069 6620 656c 696d  .        if elim
+00003f90: 696e 6174 655f 7768 6974 6573 7061 6365  inate_whitespace
+00003fa0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00003fb0: 7475 726e 206a 736f 6e2e 6475 6d70 7328  turn json.dumps(
+00003fc0: 696e 5f64 6174 612c 2073 6570 6172 6174  in_data, separat
+00003fd0: 6f72 733d 7365 6c66 2e5f 6a73 6f6e 5f65  ors=self._json_e
+00003fe0: 6e63 6f64 6572 2e63 6f6d 7061 6374 5f73  ncoder.compact_s
+00003ff0: 6570 6172 6174 6f72 7329 0a20 2020 2020  eparators).     
+00004000: 2020 2072 6574 7572 6e20 6a73 6f6e 2e64     return json.d
+00004010: 756d 7073 2869 6e5f 6461 7461 290a 0a0a  umps(in_data)...
+00004020: 636c 6173 7320 5061 7468 5061 7261 6d65  class PathParame
+00004030: 7465 7228 5061 7261 6d65 7465 7242 6173  ter(ParameterBas
+00004040: 652c 2053 7479 6c65 5369 6d70 6c65 5365  e, StyleSimpleSe
+00004050: 7269 616c 697a 6572 293a 0a0a 2020 2020  rializer):..    
+00004060: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+00004070: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00004080: 2020 2020 6e61 6d65 3a20 7374 722c 0a20      name: str,. 
+00004090: 2020 2020 2020 2072 6571 7569 7265 643a         required:
+000040a0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+000040b0: 2020 2020 2020 2073 7479 6c65 3a20 7479         style: ty
+000040c0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 5061  ping.Optional[Pa
+000040d0: 7261 6d65 7465 7253 7479 6c65 5d20 3d20  rameterStyle] = 
+000040e0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6578  None,.        ex
+000040f0: 706c 6f64 653a 2062 6f6f 6c20 3d20 4661  plode: bool = Fa
+00004100: 6c73 652c 0a20 2020 2020 2020 2061 6c6c  lse,.        all
+00004110: 6f77 5f72 6573 6572 7665 643a 2074 7970  ow_reserved: typ
+00004120: 696e 672e 4f70 7469 6f6e 616c 5b62 6f6f  ing.Optional[boo
+00004130: 6c5d 203d 204e 6f6e 652c 0a20 2020 2020  l] = None,.     
+00004140: 2020 2073 6368 656d 613a 2074 7970 696e     schema: typin
+00004150: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+00004160: 672e 5479 7065 5b53 6368 656d 615d 5d20  g.Type[Schema]] 
+00004170: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00004180: 636f 6e74 656e 743a 2074 7970 696e 672e  content: typing.
+00004190: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+000041a0: 4469 6374 5b73 7472 2c20 7479 7069 6e67  Dict[str, typing
+000041b0: 2e54 7970 655b 5363 6865 6d61 5d5d 5d20  .Type[Schema]]] 
+000041c0: 3d20 4e6f 6e65 0a20 2020 2029 3a0a 2020  = None.    ):.  
+000041d0: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+000041e0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+000041f0: 2020 2020 6e61 6d65 2c0a 2020 2020 2020      name,.      
+00004200: 2020 2020 2020 696e 5f74 7970 653d 5061        in_type=Pa
+00004210: 7261 6d65 7465 7249 6e54 7970 652e 5041  rameterInType.PA
+00004220: 5448 2c0a 2020 2020 2020 2020 2020 2020  TH,.            
+00004230: 7265 7175 6972 6564 3d72 6571 7569 7265  required=require
+00004240: 642c 0a20 2020 2020 2020 2020 2020 2073  d,.            s
+00004250: 7479 6c65 3d73 7479 6c65 2c0a 2020 2020  tyle=style,.    
+00004260: 2020 2020 2020 2020 6578 706c 6f64 653d          explode=
+00004270: 6578 706c 6f64 652c 0a20 2020 2020 2020  explode,.       
+00004280: 2020 2020 2061 6c6c 6f77 5f72 6573 6572       allow_reser
+00004290: 7665 643d 616c 6c6f 775f 7265 7365 7276  ved=allow_reserv
+000042a0: 6564 2c0a 2020 2020 2020 2020 2020 2020  ed,.            
+000042b0: 7363 6865 6d61 3d73 6368 656d 612c 0a20  schema=schema,. 
+000042c0: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
+000042d0: 6e74 3d63 6f6e 7465 6e74 0a20 2020 2020  nt=content.     
+000042e0: 2020 2029 0a0a 2020 2020 6465 6620 5f5f     )..    def __
+000042f0: 7365 7269 616c 697a 655f 6c61 6265 6c28  serialize_label(
+00004300: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00004310: 2020 2020 2020 2069 6e5f 6461 7461 3a20         in_data: 
+00004320: 7479 7069 6e67 2e55 6e69 6f6e 5b4e 6f6e  typing.Union[Non
+00004330: 652c 2069 6e74 2c20 666c 6f61 742c 2073  e, int, float, s
+00004340: 7472 2c20 626f 6f6c 2c20 6469 6374 2c20  tr, bool, dict, 
+00004350: 6c69 7374 5d0a 2020 2020 2920 2d3e 2074  list].    ) -> t
+00004360: 7970 696e 672e 4469 6374 5b73 7472 2c20  yping.Dict[str, 
+00004370: 7374 725d 3a0a 2020 2020 2020 2020 7072  str]:.        pr
+00004380: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+00004390: 7465 7261 746f 7220 3d20 5072 6566 6978  terator = Prefix
+000043a0: 5365 7061 7261 746f 7249 7465 7261 746f  SeparatorIterato
+000043b0: 7228 272e 272c 2027 2e27 290a 2020 2020  r('.', '.').    
+000043c0: 2020 2020 7661 6c75 6520 3d20 7365 6c66      value = self
+000043d0: 2e5f 7265 6636 3537 305f 6578 7061 6e73  ._ref6570_expans
+000043e0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
+000043f0: 2076 6172 6961 626c 655f 6e61 6d65 3d73   variable_name=s
+00004400: 656c 662e 6e61 6d65 2c0a 2020 2020 2020  elf.name,.      
+00004410: 2020 2020 2020 696e 5f64 6174 613d 696e        in_data=in
+00004420: 5f64 6174 612c 0a20 2020 2020 2020 2020  _data,.         
+00004430: 2020 2065 7870 6c6f 6465 3d73 656c 662e     explode=self.
+00004440: 6578 706c 6f64 652c 0a20 2020 2020 2020  explode,.       
+00004450: 2020 2020 2070 6572 6365 6e74 5f65 6e63       percent_enc
+00004460: 6f64 653d 5472 7565 2c0a 2020 2020 2020  ode=True,.      
+00004470: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
+00004480: 6172 6174 6f72 5f69 7465 7261 746f 723d  arator_iterator=
+00004490: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
+000044a0: 5f69 7465 7261 746f 720a 2020 2020 2020  _iterator.      
+000044b0: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
+000044c0: 726e 2073 656c 662e 5f74 6f5f 6469 6374  rn self._to_dict
+000044d0: 2873 656c 662e 6e61 6d65 2c20 7661 6c75  (self.name, valu
+000044e0: 6529 0a0a 2020 2020 6465 6620 5f5f 7365  e)..    def __se
+000044f0: 7269 616c 697a 655f 6d61 7472 6978 280a  rialize_matrix(.
+00004500: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00004510: 2020 2020 2020 696e 5f64 6174 613a 2074        in_data: t
+00004520: 7970 696e 672e 556e 696f 6e5b 4e6f 6e65  yping.Union[None
+00004530: 2c20 696e 742c 2066 6c6f 6174 2c20 7374  , int, float, st
+00004540: 722c 2062 6f6f 6c2c 2064 6963 742c 206c  r, bool, dict, l
+00004550: 6973 745d 0a20 2020 2029 202d 3e20 7479  ist].    ) -> ty
+00004560: 7069 6e67 2e44 6963 745b 7374 722c 2073  ping.Dict[str, s
+00004570: 7472 5d3a 0a20 2020 2020 2020 2070 7265  tr]:.        pre
+00004580: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
+00004590: 6572 6174 6f72 203d 2050 7265 6669 7853  erator = PrefixS
+000045a0: 6570 6172 6174 6f72 4974 6572 6174 6f72  eparatorIterator
+000045b0: 2827 3b27 2c20 273b 2729 0a20 2020 2020  (';', ';').     
+000045c0: 2020 2076 616c 7565 203d 2073 656c 662e     value = self.
+000045d0: 5f72 6566 3635 3730 5f65 7870 616e 7369  _ref6570_expansi
+000045e0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+000045f0: 7661 7269 6162 6c65 5f6e 616d 653d 7365  variable_name=se
+00004600: 6c66 2e6e 616d 652c 0a20 2020 2020 2020  lf.name,.       
+00004610: 2020 2020 2069 6e5f 6461 7461 3d69 6e5f       in_data=in_
+00004620: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
+00004630: 2020 6578 706c 6f64 653d 7365 6c66 2e65    explode=self.e
+00004640: 7870 6c6f 6465 2c0a 2020 2020 2020 2020  xplode,.        
+00004650: 2020 2020 7065 7263 656e 745f 656e 636f      percent_enco
+00004660: 6465 3d54 7275 652c 0a20 2020 2020 2020  de=True,.       
+00004670: 2020 2020 2070 7265 6669 785f 7365 7061       prefix_sepa
+00004680: 7261 746f 725f 6974 6572 6174 6f72 3d70  rator_iterator=p
+00004690: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
+000046a0: 6974 6572 6174 6f72 0a20 2020 2020 2020  iterator.       
+000046b0: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
+000046c0: 6e20 7365 6c66 2e5f 746f 5f64 6963 7428  n self._to_dict(
+000046d0: 7365 6c66 2e6e 616d 652c 2076 616c 7565  self.name, value
+000046e0: 290a 0a20 2020 2064 6566 205f 5f73 6572  )..    def __ser
+000046f0: 6961 6c69 7a65 5f73 696d 706c 6528 0a20  ialize_simple(. 
+00004700: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00004710: 2020 2020 2069 6e5f 6461 7461 3a20 7479       in_data: ty
+00004720: 7069 6e67 2e55 6e69 6f6e 5b4e 6f6e 652c  ping.Union[None,
+00004730: 2069 6e74 2c20 666c 6f61 742c 2073 7472   int, float, str
+00004740: 2c20 626f 6f6c 2c20 6469 6374 2c20 6c69  , bool, dict, li
+00004750: 7374 5d2c 0a20 2020 2029 202d 3e20 7479  st],.    ) -> ty
+00004760: 7069 6e67 2e44 6963 745b 7374 722c 2073  ping.Dict[str, s
+00004770: 7472 5d3a 0a20 2020 2020 2020 2076 616c  tr]:.        val
+00004780: 7565 203d 2073 656c 662e 5f73 6572 6961  ue = self._seria
+00004790: 6c69 7a65 5f73 696d 706c 6528 0a20 2020  lize_simple(.   
+000047a0: 2020 2020 2020 2020 2069 6e5f 6461 7461           in_data
+000047b0: 3d69 6e5f 6461 7461 2c0a 2020 2020 2020  =in_data,.      
+000047c0: 2020 2020 2020 6e61 6d65 3d73 656c 662e        name=self.
+000047d0: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+000047e0: 2020 6578 706c 6f64 653d 7365 6c66 2e65    explode=self.e
+000047f0: 7870 6c6f 6465 2c0a 2020 2020 2020 2020  xplode,.        
+00004800: 2020 2020 7065 7263 656e 745f 656e 636f      percent_enco
+00004810: 6465 3d54 7275 650a 2020 2020 2020 2020  de=True.        
+00004820: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00004830: 2073 656c 662e 5f74 6f5f 6469 6374 2873   self._to_dict(s
+00004840: 656c 662e 6e61 6d65 2c20 7661 6c75 6529  elf.name, value)
+00004850: 0a0a 2020 2020 6465 6620 7365 7269 616c  ..    def serial
+00004860: 697a 6528 0a20 2020 2020 2020 2073 656c  ize(.        sel
+00004870: 662c 0a20 2020 2020 2020 2069 6e5f 6461  f,.        in_da
+00004880: 7461 3a20 7479 7069 6e67 2e55 6e69 6f6e  ta: typing.Union
+00004890: 5b0a 2020 2020 2020 2020 2020 2020 5363  [.            Sc
+000048a0: 6865 6d61 2c20 4465 6369 6d61 6c2c 2069  hema, Decimal, i
+000048b0: 6e74 2c20 666c 6f61 742c 2073 7472 2c20  nt, float, str, 
+000048c0: 6461 7465 2c20 6461 7465 7469 6d65 2c20  date, datetime, 
+000048d0: 4e6f 6e65 2c20 626f 6f6c 2c20 6c69 7374  None, bool, list
+000048e0: 2c20 7475 706c 652c 2064 6963 742c 2066  , tuple, dict, f
+000048f0: 726f 7a65 6e64 6963 742e 6672 6f7a 656e  rozendict.frozen
+00004900: 6469 6374 5d0a 2020 2020 2920 2d3e 2074  dict].    ) -> t
+00004910: 7970 696e 672e 4469 6374 5b73 7472 2c20  yping.Dict[str, 
+00004920: 7374 725d 3a0a 2020 2020 2020 2020 6966  str]:.        if
+00004930: 2073 656c 662e 7363 6865 6d61 3a0a 2020   self.schema:.  
+00004940: 2020 2020 2020 2020 2020 6361 7374 5f69            cast_i
+00004950: 6e5f 6461 7461 203d 2073 656c 662e 7363  n_data = self.sc
+00004960: 6865 6d61 2869 6e5f 6461 7461 290a 2020  hema(in_data).  
+00004970: 2020 2020 2020 2020 2020 6361 7374 5f69            cast_i
+00004980: 6e5f 6461 7461 203d 2073 656c 662e 5f6a  n_data = self._j
+00004990: 736f 6e5f 656e 636f 6465 722e 6465 6661  son_encoder.defa
+000049a0: 756c 7428 6361 7374 5f69 6e5f 6461 7461  ult(cast_in_data
+000049b0: 290a 2020 2020 2020 2020 2020 2020 2222  ).            ""
+000049c0: 220a 2020 2020 2020 2020 2020 2020 7369  ".            si
+000049d0: 6d70 6c65 202d 3e20 7061 7468 0a20 2020  mple -> path.   
+000049e0: 2020 2020 2020 2020 2020 2020 2070 6174               pat
+000049f0: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
+00004a00: 2020 2020 2020 2072 6574 7572 6e73 2070         returns p
+00004a10: 6174 685f 7061 7261 6d73 3a20 6469 6374  ath_params: dict
+00004a20: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
+00004a30: 656c 202d 3e20 7061 7468 0a20 2020 2020  el -> path.     
+00004a40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00004a50: 6e73 2070 6174 685f 7061 7261 6d73 0a20  ns path_params. 
+00004a60: 2020 2020 2020 2020 2020 206d 6174 7269             matri
+00004a70: 7820 2d3e 2070 6174 680a 2020 2020 2020  x -> path.      
+00004a80: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00004a90: 7320 7061 7468 5f70 6172 616d 730a 2020  s path_params.  
+00004aa0: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
+00004ab0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00004ac0: 662e 7374 796c 653a 0a20 2020 2020 2020  f.style:.       
+00004ad0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00004ae0: 2e73 7479 6c65 2069 7320 5061 7261 6d65  .style is Parame
+00004af0: 7465 7253 7479 6c65 2e53 494d 504c 453a  terStyle.SIMPLE:
+00004b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004b10: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00004b20: 2e5f 5f73 6572 6961 6c69 7a65 5f73 696d  .__serialize_sim
+00004b30: 706c 6528 6361 7374 5f69 6e5f 6461 7461  ple(cast_in_data
+00004b40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00004b50: 2020 656c 6966 2073 656c 662e 7374 796c    elif self.styl
+00004b60: 6520 6973 2050 6172 616d 6574 6572 5374  e is ParameterSt
+00004b70: 796c 652e 4c41 4245 4c3a 0a20 2020 2020  yle.LABEL:.     
+00004b80: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004b90: 6574 7572 6e20 7365 6c66 2e5f 5f73 6572  eturn self.__ser
+00004ba0: 6961 6c69 7a65 5f6c 6162 656c 2863 6173  ialize_label(cas
+00004bb0: 745f 696e 5f64 6174 6129 0a20 2020 2020  t_in_data).     
+00004bc0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00004bd0: 7365 6c66 2e73 7479 6c65 2069 7320 5061  self.style is Pa
+00004be0: 7261 6d65 7465 7253 7479 6c65 2e4d 4154  rameterStyle.MAT
+00004bf0: 5249 583a 0a20 2020 2020 2020 2020 2020  RIX:.           
+00004c00: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00004c10: 7365 6c66 2e5f 5f73 6572 6961 6c69 7a65  self.__serialize
+00004c20: 5f6d 6174 7269 7828 6361 7374 5f69 6e5f  _matrix(cast_in_
+00004c30: 6461 7461 290a 2020 2020 2020 2020 2320  data).        # 
+00004c40: 7365 6c66 2e63 6f6e 7465 6e74 2077 696c  self.content wil
+00004c50: 6c20 6265 206c 656e 6774 6820 6f6e 650a  l be length one.
+00004c60: 2020 2020 2020 2020 666f 7220 636f 6e74          for cont
+00004c70: 656e 745f 7479 7065 2c20 7363 6865 6d61  ent_type, schema
+00004c80: 2069 6e20 7365 6c66 2e63 6f6e 7465 6e74   in self.content
+00004c90: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+00004ca0: 2020 2020 2020 6361 7374 5f69 6e5f 6461        cast_in_da
+00004cb0: 7461 203d 2073 6368 656d 6128 696e 5f64  ta = schema(in_d
+00004cc0: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
+00004cd0: 2063 6173 745f 696e 5f64 6174 6120 3d20   cast_in_data = 
+00004ce0: 7365 6c66 2e5f 6a73 6f6e 5f65 6e63 6f64  self._json_encod
+00004cf0: 6572 2e64 6566 6175 6c74 2863 6173 745f  er.default(cast_
+00004d00: 696e 5f64 6174 6129 0a20 2020 2020 2020  in_data).       
+00004d10: 2020 2020 2069 6620 7365 6c66 2e5f 636f       if self._co
+00004d20: 6e74 656e 745f 7479 7065 5f69 735f 6a73  ntent_type_is_js
+00004d30: 6f6e 2863 6f6e 7465 6e74 5f74 7970 6529  on(content_type)
+00004d40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004d50: 2020 7661 6c75 6520 3d20 7365 6c66 2e5f    value = self._
+00004d60: 7365 7269 616c 697a 655f 6a73 6f6e 2863  serialize_json(c
+00004d70: 6173 745f 696e 5f64 6174 6129 0a20 2020  ast_in_data).   
+00004d80: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00004d90: 7572 6e20 7365 6c66 2e5f 746f 5f64 6963  urn self._to_dic
+00004da0: 7428 7365 6c66 2e6e 616d 652c 2076 616c  t(self.name, val
+00004db0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00004dc0: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
+00004dd0: 6e74 6564 4572 726f 7228 2753 6572 6961  ntedError('Seria
+00004de0: 6c69 7a61 7469 6f6e 206f 6620 7b7d 2068  lization of {} h
+00004df0: 6173 206e 6f74 2079 6574 2062 6565 6e20  as not yet been 
+00004e00: 696d 706c 656d 656e 7465 6427 2e66 6f72  implemented'.for
+00004e10: 6d61 7428 636f 6e74 656e 745f 7479 7065  mat(content_type
+00004e20: 2929 0a0a 0a63 6c61 7373 2051 7565 7279  ))...class Query
+00004e30: 5061 7261 6d65 7465 7228 5061 7261 6d65  Parameter(Parame
+00004e40: 7465 7242 6173 652c 2053 7479 6c65 466f  terBase, StyleFo
+00004e50: 726d 5365 7269 616c 697a 6572 293a 0a0a  rmSerializer):..
+00004e60: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00004e70: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00004e80: 2020 2020 2020 2020 6e61 6d65 3a20 7374          name: st
+00004e90: 722c 0a20 2020 2020 2020 2072 6571 7569  r,.        requi
+00004ea0: 7265 643a 2062 6f6f 6c20 3d20 4661 6c73  red: bool = Fals
+00004eb0: 652c 0a20 2020 2020 2020 2073 7479 6c65  e,.        style
+00004ec0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00004ed0: 6c5b 5061 7261 6d65 7465 7253 7479 6c65  l[ParameterStyle
+00004ee0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00004ef0: 2020 6578 706c 6f64 653a 2074 7970 696e    explode: typin
+00004f00: 672e 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  g.Optional[bool]
+00004f10: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00004f20: 2061 6c6c 6f77 5f72 6573 6572 7665 643a   allow_reserved:
+00004f30: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00004f40: 5b62 6f6f 6c5d 203d 204e 6f6e 652c 0a20  [bool] = None,. 
+00004f50: 2020 2020 2020 2073 6368 656d 613a 2074         schema: t
+00004f60: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+00004f70: 7970 696e 672e 5479 7065 5b53 6368 656d  yping.Type[Schem
+00004f80: 615d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  a]] = None,.    
+00004f90: 2020 2020 636f 6e74 656e 743a 2074 7970      content: typ
+00004fa0: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+00004fb0: 696e 672e 4469 6374 5b73 7472 2c20 7479  ing.Dict[str, ty
+00004fc0: 7069 6e67 2e54 7970 655b 5363 6865 6d61  ping.Type[Schema
+00004fd0: 5d5d 5d20 3d20 4e6f 6e65 0a20 2020 2029  ]]] = None.    )
+00004fe0: 3a0a 2020 2020 2020 2020 7573 6564 5f73  :.        used_s
+00004ff0: 7479 6c65 203d 2050 6172 616d 6574 6572  tyle = Parameter
+00005000: 5374 796c 652e 464f 524d 2069 6620 7374  Style.FORM if st
+00005010: 796c 6520 6973 204e 6f6e 6520 656c 7365  yle is None else
+00005020: 2073 7479 6c65 0a20 2020 2020 2020 2075   style.        u
+00005030: 7365 645f 6578 706c 6f64 6520 3d20 7365  sed_explode = se
+00005040: 6c66 2e5f 6765 745f 6465 6661 756c 745f  lf._get_default_
+00005050: 6578 706c 6f64 6528 7573 6564 5f73 7479  explode(used_sty
+00005060: 6c65 2920 6966 2065 7870 6c6f 6465 2069  le) if explode i
+00005070: 7320 4e6f 6e65 2065 6c73 6520 6578 706c  s None else expl
+00005080: 6f64 650a 0a20 2020 2020 2020 2073 7570  ode..        sup
+00005090: 6572 2829 2e5f 5f69 6e69 745f 5f28 0a20  er().__init__(. 
+000050a0: 2020 2020 2020 2020 2020 206e 616d 652c             name,
+000050b0: 0a20 2020 2020 2020 2020 2020 2069 6e5f  .            in_
+000050c0: 7479 7065 3d50 6172 616d 6574 6572 496e  type=ParameterIn
+000050d0: 5479 7065 2e51 5545 5259 2c0a 2020 2020  Type.QUERY,.    
+000050e0: 2020 2020 2020 2020 7265 7175 6972 6564          required
+000050f0: 3d72 6571 7569 7265 642c 0a20 2020 2020  =required,.     
+00005100: 2020 2020 2020 2073 7479 6c65 3d75 7365         style=use
+00005110: 645f 7374 796c 652c 0a20 2020 2020 2020  d_style,.       
+00005120: 2020 2020 2065 7870 6c6f 6465 3d75 7365       explode=use
+00005130: 645f 6578 706c 6f64 652c 0a20 2020 2020  d_explode,.     
+00005140: 2020 2020 2020 2061 6c6c 6f77 5f72 6573         allow_res
+00005150: 6572 7665 643d 616c 6c6f 775f 7265 7365  erved=allow_rese
+00005160: 7276 6564 2c0a 2020 2020 2020 2020 2020  rved,.          
+00005170: 2020 7363 6865 6d61 3d73 6368 656d 612c    schema=schema,
+00005180: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00005190: 7465 6e74 3d63 6f6e 7465 6e74 0a20 2020  tent=content.   
+000051a0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+000051b0: 5f5f 7365 7269 616c 697a 655f 7370 6163  __serialize_spac
+000051c0: 655f 6465 6c69 6d69 7465 6428 0a20 2020  e_delimited(.   
+000051d0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000051e0: 2020 2069 6e5f 6461 7461 3a20 7479 7069     in_data: typi
+000051f0: 6e67 2e55 6e69 6f6e 5b4e 6f6e 652c 2069  ng.Union[None, i
+00005200: 6e74 2c20 666c 6f61 742c 2073 7472 2c20  nt, float, str, 
+00005210: 626f 6f6c 2c20 6469 6374 2c20 6c69 7374  bool, dict, list
+00005220: 5d2c 0a20 2020 2020 2020 2070 7265 6669  ],.        prefi
+00005230: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
+00005240: 6174 6f72 3a20 7479 7069 6e67 2e4f 7074  ator: typing.Opt
+00005250: 696f 6e61 6c5b 5072 6566 6978 5365 7061  ional[PrefixSepa
+00005260: 7261 746f 7249 7465 7261 746f 725d 0a20  ratorIterator]. 
+00005270: 2020 2029 202d 3e20 7479 7069 6e67 2e44     ) -> typing.D
+00005280: 6963 745b 7374 722c 2073 7472 5d3a 0a20  ict[str, str]:. 
+00005290: 2020 2020 2020 2069 6620 7072 6566 6978         if prefix
+000052a0: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
+000052b0: 746f 7220 6973 204e 6f6e 653a 0a20 2020  tor is None:.   
+000052c0: 2020 2020 2020 2020 2070 7265 6669 785f           prefix_
+000052d0: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
+000052e0: 6f72 203d 2073 656c 662e 6765 745f 7072  or = self.get_pr
+000052f0: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+00005300: 7465 7261 746f 7228 290a 2020 2020 2020  terator().      
+00005310: 2020 7661 6c75 6520 3d20 7365 6c66 2e5f    value = self._
+00005320: 7265 6636 3537 305f 6578 7061 6e73 696f  ref6570_expansio
+00005330: 6e28 0a20 2020 2020 2020 2020 2020 2076  n(.            v
+00005340: 6172 6961 626c 655f 6e61 6d65 3d73 656c  ariable_name=sel
+00005350: 662e 6e61 6d65 2c0a 2020 2020 2020 2020  f.name,.        
+00005360: 2020 2020 696e 5f64 6174 613d 696e 5f64      in_data=in_d
+00005370: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+00005380: 2065 7870 6c6f 6465 3d73 656c 662e 6578   explode=self.ex
+00005390: 706c 6f64 652c 0a20 2020 2020 2020 2020  plode,.         
+000053a0: 2020 2070 6572 6365 6e74 5f65 6e63 6f64     percent_encod
+000053b0: 653d 5472 7565 2c0a 2020 2020 2020 2020  e=True,.        
+000053c0: 2020 2020 7072 6566 6978 5f73 6570 6172      prefix_separ
+000053d0: 6174 6f72 5f69 7465 7261 746f 723d 7072  ator_iterator=pr
+000053e0: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+000053f0: 7465 7261 746f 720a 2020 2020 2020 2020  terator.        
+00005400: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00005410: 2073 656c 662e 5f74 6f5f 6469 6374 2873   self._to_dict(s
+00005420: 656c 662e 6e61 6d65 2c20 7661 6c75 6529  elf.name, value)
+00005430: 0a0a 2020 2020 6465 6620 5f5f 7365 7269  ..    def __seri
+00005440: 616c 697a 655f 7069 7065 5f64 656c 696d  alize_pipe_delim
+00005450: 6974 6564 280a 2020 2020 2020 2020 7365  ited(.        se
+00005460: 6c66 2c0a 2020 2020 2020 2020 696e 5f64  lf,.        in_d
+00005470: 6174 613a 2074 7970 696e 672e 556e 696f  ata: typing.Unio
+00005480: 6e5b 4e6f 6e65 2c20 696e 742c 2066 6c6f  n[None, int, flo
+00005490: 6174 2c20 7374 722c 2062 6f6f 6c2c 2064  at, str, bool, d
+000054a0: 6963 742c 206c 6973 745d 2c0a 2020 2020  ict, list],.    
+000054b0: 2020 2020 7072 6566 6978 5f73 6570 6172      prefix_separ
+000054c0: 6174 6f72 5f69 7465 7261 746f 723a 2074  ator_iterator: t
+000054d0: 7970 696e 672e 4f70 7469 6f6e 616c 5b50  yping.Optional[P
+000054e0: 7265 6669 7853 6570 6172 6174 6f72 4974  refixSeparatorIt
+000054f0: 6572 6174 6f72 5d0a 2020 2020 2920 2d3e  erator].    ) ->
+00005500: 2074 7970 696e 672e 4469 6374 5b73 7472   typing.Dict[str
+00005510: 2c20 7374 725d 3a0a 2020 2020 2020 2020  , str]:.        
+00005520: 6966 2070 7265 6669 785f 7365 7061 7261  if prefix_separa
+00005530: 746f 725f 6974 6572 6174 6f72 2069 7320  tor_iterator is 
+00005540: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00005550: 2020 7072 6566 6978 5f73 6570 6172 6174    prefix_separat
+00005560: 6f72 5f69 7465 7261 746f 7220 3d20 7365  or_iterator = se
+00005570: 6c66 2e67 6574 5f70 7265 6669 785f 7365  lf.get_prefix_se
+00005580: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
+00005590: 2829 0a20 2020 2020 2020 2076 616c 7565  ().        value
+000055a0: 203d 2073 656c 662e 5f72 6566 3635 3730   = self._ref6570
+000055b0: 5f65 7870 616e 7369 6f6e 280a 2020 2020  _expansion(.    
+000055c0: 2020 2020 2020 2020 7661 7269 6162 6c65          variable
+000055d0: 5f6e 616d 653d 7365 6c66 2e6e 616d 652c  _name=self.name,
+000055e0: 0a20 2020 2020 2020 2020 2020 2069 6e5f  .            in_
+000055f0: 6461 7461 3d69 6e5f 6461 7461 2c0a 2020  data=in_data,.  
+00005600: 2020 2020 2020 2020 2020 6578 706c 6f64            explod
+00005610: 653d 7365 6c66 2e65 7870 6c6f 6465 2c0a  e=self.explode,.
+00005620: 2020 2020 2020 2020 2020 2020 7065 7263              perc
+00005630: 656e 745f 656e 636f 6465 3d54 7275 652c  ent_encode=True,
+00005640: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
+00005650: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
+00005660: 6572 6174 6f72 3d70 7265 6669 785f 7365  erator=prefix_se
+00005670: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
+00005680: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00005690: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+000056a0: 746f 5f64 6963 7428 7365 6c66 2e6e 616d  to_dict(self.nam
+000056b0: 652c 2076 616c 7565 290a 0a20 2020 2064  e, value)..    d
+000056c0: 6566 205f 5f73 6572 6961 6c69 7a65 5f66  ef __serialize_f
+000056d0: 6f72 6d28 0a20 2020 2020 2020 2073 656c  orm(.        sel
+000056e0: 662c 0a20 2020 2020 2020 2069 6e5f 6461  f,.        in_da
+000056f0: 7461 3a20 7479 7069 6e67 2e55 6e69 6f6e  ta: typing.Union
+00005700: 5b4e 6f6e 652c 2069 6e74 2c20 666c 6f61  [None, int, floa
+00005710: 742c 2073 7472 2c20 626f 6f6c 2c20 6469  t, str, bool, di
+00005720: 6374 2c20 6c69 7374 5d2c 0a20 2020 2020  ct, list],.     
+00005730: 2020 2070 7265 6669 785f 7365 7061 7261     prefix_separa
+00005740: 746f 725f 6974 6572 6174 6f72 3a20 7479  tor_iterator: ty
+00005750: 7069 6e67 2e4f 7074 696f 6e61 6c5b 5072  ping.Optional[Pr
+00005760: 6566 6978 5365 7061 7261 746f 7249 7465  efixSeparatorIte
+00005770: 7261 746f 725d 0a20 2020 2029 202d 3e20  rator].    ) -> 
+00005780: 7479 7069 6e67 2e44 6963 745b 7374 722c  typing.Dict[str,
+00005790: 2073 7472 5d3a 0a20 2020 2020 2020 2069   str]:.        i
+000057a0: 6620 7072 6566 6978 5f73 6570 6172 6174  f prefix_separat
+000057b0: 6f72 5f69 7465 7261 746f 7220 6973 204e  or_iterator is N
+000057c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000057d0: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
+000057e0: 725f 6974 6572 6174 6f72 203d 2073 656c  r_iterator = sel
+000057f0: 662e 6765 745f 7072 6566 6978 5f73 6570  f.get_prefix_sep
+00005800: 6172 6174 6f72 5f69 7465 7261 746f 7228  arator_iterator(
+00005810: 290a 2020 2020 2020 2020 7661 6c75 6520  ).        value 
+00005820: 3d20 7365 6c66 2e5f 7365 7269 616c 697a  = self._serializ
+00005830: 655f 666f 726d 280a 2020 2020 2020 2020  e_form(.        
+00005840: 2020 2020 696e 5f64 6174 612c 0a20 2020      in_data,.   
+00005850: 2020 2020 2020 2020 206e 616d 653d 7365           name=se
+00005860: 6c66 2e6e 616d 652c 0a20 2020 2020 2020  lf.name,.       
+00005870: 2020 2020 2065 7870 6c6f 6465 3d73 656c       explode=sel
+00005880: 662e 6578 706c 6f64 652c 0a20 2020 2020  f.explode,.     
+00005890: 2020 2020 2020 2070 6572 6365 6e74 5f65         percent_e
+000058a0: 6e63 6f64 653d 5472 7565 2c0a 2020 2020  ncode=True,.    
+000058b0: 2020 2020 2020 2020 7072 6566 6978 5f73          prefix_s
+000058c0: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+000058d0: 723d 7072 6566 6978 5f73 6570 6172 6174  r=prefix_separat
+000058e0: 6f72 5f69 7465 7261 746f 720a 2020 2020  or_iterator.    
+000058f0: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
+00005900: 7475 726e 2073 656c 662e 5f74 6f5f 6469  turn self._to_di
+00005910: 6374 2873 656c 662e 6e61 6d65 2c20 7661  ct(self.name, va
+00005920: 6c75 6529 0a0a 2020 2020 6465 6620 6765  lue)..    def ge
+00005930: 745f 7072 6566 6978 5f73 6570 6172 6174  t_prefix_separat
+00005940: 6f72 5f69 7465 7261 746f 7228 7365 6c66  or_iterator(self
+00005950: 2920 2d3e 2074 7970 696e 672e 4f70 7469  ) -> typing.Opti
+00005960: 6f6e 616c 5b50 7265 6669 7853 6570 6172  onal[PrefixSepar
+00005970: 6174 6f72 4974 6572 6174 6f72 5d3a 0a20  atorIterator]:. 
+00005980: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00005990: 7479 6c65 2069 7320 5061 7261 6d65 7465  tyle is Paramete
+000059a0: 7253 7479 6c65 2e46 4f52 4d3a 0a20 2020  rStyle.FORM:.   
+000059b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000059c0: 5072 6566 6978 5365 7061 7261 746f 7249  PrefixSeparatorI
+000059d0: 7465 7261 746f 7228 273f 272c 2027 2627  terator('?', '&'
+000059e0: 290a 2020 2020 2020 2020 656c 6966 2073  ).        elif s
+000059f0: 656c 662e 7374 796c 6520 6973 2050 6172  elf.style is Par
+00005a00: 616d 6574 6572 5374 796c 652e 5350 4143  ameterStyle.SPAC
+00005a10: 455f 4445 4c49 4d49 5445 443a 0a20 2020  E_DELIMITED:.   
+00005a20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00005a30: 5072 6566 6978 5365 7061 7261 746f 7249  PrefixSeparatorI
+00005a40: 7465 7261 746f 7228 2727 2c20 2725 3230  terator('', '%20
+00005a50: 2729 0a20 2020 2020 2020 2065 6c69 6620  ').        elif 
+00005a60: 7365 6c66 2e73 7479 6c65 2069 7320 5061  self.style is Pa
+00005a70: 7261 6d65 7465 7253 7479 6c65 2e50 4950  rameterStyle.PIP
+00005a80: 455f 4445 4c49 4d49 5445 443a 0a20 2020  E_DELIMITED:.   
+00005a90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00005aa0: 5072 6566 6978 5365 7061 7261 746f 7249  PrefixSeparatorI
+00005ab0: 7465 7261 746f 7228 2727 2c20 277c 2729  terator('', '|')
+00005ac0: 0a0a 2020 2020 6465 6620 7365 7269 616c  ..    def serial
+00005ad0: 697a 6528 0a20 2020 2020 2020 2073 656c  ize(.        sel
+00005ae0: 662c 0a20 2020 2020 2020 2069 6e5f 6461  f,.        in_da
+00005af0: 7461 3a20 7479 7069 6e67 2e55 6e69 6f6e  ta: typing.Union
+00005b00: 5b0a 2020 2020 2020 2020 2020 2020 5363  [.            Sc
+00005b10: 6865 6d61 2c20 4465 6369 6d61 6c2c 2069  hema, Decimal, i
+00005b20: 6e74 2c20 666c 6f61 742c 2073 7472 2c20  nt, float, str, 
+00005b30: 6461 7465 2c20 6461 7465 7469 6d65 2c20  date, datetime, 
+00005b40: 4e6f 6e65 2c20 626f 6f6c 2c20 6c69 7374  None, bool, list
+00005b50: 2c20 7475 706c 652c 2064 6963 742c 2066  , tuple, dict, f
+00005b60: 726f 7a65 6e64 6963 742e 6672 6f7a 656e  rozendict.frozen
+00005b70: 6469 6374 5d2c 0a20 2020 2020 2020 2070  dict],.        p
+00005b80: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
+00005b90: 6974 6572 6174 6f72 3a20 7479 7069 6e67  iterator: typing
+00005ba0: 2e4f 7074 696f 6e61 6c5b 5072 6566 6978  .Optional[Prefix
+00005bb0: 5365 7061 7261 746f 7249 7465 7261 746f  SeparatorIterato
+00005bc0: 725d 203d 204e 6f6e 650a 2020 2020 2920  r] = None.    ) 
+00005bd0: 2d3e 2074 7970 696e 672e 4469 6374 5b73  -> typing.Dict[s
+00005be0: 7472 2c20 7374 725d 3a0a 2020 2020 2020  tr, str]:.      
+00005bf0: 2020 6966 2073 656c 662e 7363 6865 6d61    if self.schema
+00005c00: 3a0a 2020 2020 2020 2020 2020 2020 6361  :.            ca
+00005c10: 7374 5f69 6e5f 6461 7461 203d 2073 656c  st_in_data = sel
+00005c20: 662e 7363 6865 6d61 2869 6e5f 6461 7461  f.schema(in_data
+00005c30: 290a 2020 2020 2020 2020 2020 2020 6361  ).            ca
+00005c40: 7374 5f69 6e5f 6461 7461 203d 2073 656c  st_in_data = sel
+00005c50: 662e 5f6a 736f 6e5f 656e 636f 6465 722e  f._json_encoder.
+00005c60: 6465 6661 756c 7428 6361 7374 5f69 6e5f  default(cast_in_
+00005c70: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
+00005c80: 2020 2222 220a 2020 2020 2020 2020 2020    """.          
+00005c90: 2020 666f 726d 202d 3e20 7175 6572 790a    form -> query.
+00005ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cb0: 7175 6572 793a 0a20 2020 2020 2020 2020  query:.         
+00005cc0: 2020 2020 2020 2020 2020 202d 2047 4554             - GET
+00005cd0: 2f48 4541 442f 4445 4c45 5445 3a20 636f  /HEAD/DELETE: co
+00005ce0: 756c 6420 7573 6520 6669 656c 6473 0a20  uld use fields. 
+00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d00: 2020 202d 2050 5554 2f50 4f53 543a 206d     - PUT/POST: m
+00005d10: 7573 7420 7573 6520 7572 6c65 6e63 6f64  ust use urlencod
+00005d20: 6520 746f 2073 656e 6420 7061 7261 6d65  e to send parame
+00005d30: 7465 7273 0a20 2020 2020 2020 2020 2020  ters.           
+00005d40: 2020 2020 2020 2020 2072 6574 7572 6e73           returns
+00005d50: 2066 6965 6c64 733a 2074 7570 6c65 0a20   fields: tuple. 
+00005d60: 2020 2020 2020 2020 2020 2073 7061 6365             space
+00005d70: 4465 6c69 6d69 7465 6420 2d3e 2071 7565  Delimited -> que
+00005d80: 7279 0a20 2020 2020 2020 2020 2020 2020  ry.             
+00005d90: 2020 2072 6574 7572 6e73 2066 6965 6c64     returns field
+00005da0: 730a 2020 2020 2020 2020 2020 2020 7069  s.            pi
+00005db0: 7065 4465 6c69 6d69 7465 6420 2d3e 2071  peDelimited -> q
+00005dc0: 7565 7279 0a20 2020 2020 2020 2020 2020  uery.           
+00005dd0: 2020 2020 2072 6574 7572 6e73 2066 6965       returns fie
+00005de0: 6c64 730a 2020 2020 2020 2020 2020 2020  lds.            
+00005df0: 6465 6570 4f62 6a65 6374 202d 3e20 7175  deepObject -> qu
+00005e00: 6572 792c 2068 7474 7073 3a2f 2f67 6974  ery, https://git
+00005e10: 6875 622e 636f 6d2f 4f41 492f 4f70 656e  hub.com/OAI/Open
+00005e20: 4150 492d 5370 6563 6966 6963 6174 696f  API-Specificatio
+00005e30: 6e2f 6973 7375 6573 2f31 3730 360a 2020  n/issues/1706.  
+00005e40: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00005e50: 7475 726e 7320 6669 656c 6473 0a20 2020  turns fields.   
+00005e60: 2020 2020 2020 2020 2022 2222 0a20 2020           """.   
+00005e70: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00005e80: 2e73 7479 6c65 3a0a 2020 2020 2020 2020  .style:.        
+00005e90: 2020 2020 2020 2020 2320 544f 444f 2075          # TODO u
+00005ea0: 7064 6174 6520 7175 6572 7920 6f6e 6573  pdate query ones
+00005eb0: 2074 6f20 6f6d 6974 2073 6574 7469 6e67   to omit setting
+00005ec0: 2076 616c 7565 7320 7768 656e 205b 5d20   values when [] 
+00005ed0: 7b7d 206f 7220 4e6f 6e65 2069 7320 696e  {} or None is in
+00005ee0: 7075 740a 2020 2020 2020 2020 2020 2020  put.            
+00005ef0: 2020 2020 6966 2073 656c 662e 7374 796c      if self.styl
+00005f00: 6520 6973 2050 6172 616d 6574 6572 5374  e is ParameterSt
+00005f10: 796c 652e 464f 524d 3a0a 2020 2020 2020  yle.FORM:.      
+00005f20: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00005f30: 7475 726e 2073 656c 662e 5f5f 7365 7269  turn self.__seri
+00005f40: 616c 697a 655f 666f 726d 2863 6173 745f  alize_form(cast_
+00005f50: 696e 5f64 6174 612c 2070 7265 6669 785f  in_data, prefix_
+00005f60: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
+00005f70: 6f72 290a 2020 2020 2020 2020 2020 2020  or).            
+00005f80: 2020 2020 656c 6966 2073 656c 662e 7374      elif self.st
+00005f90: 796c 6520 6973 2050 6172 616d 6574 6572  yle is Parameter
+00005fa0: 5374 796c 652e 5350 4143 455f 4445 4c49  Style.SPACE_DELI
+00005fb0: 4d49 5445 443a 0a20 2020 2020 2020 2020  MITED:.         
+00005fc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00005fd0: 6e20 7365 6c66 2e5f 5f73 6572 6961 6c69  n self.__seriali
+00005fe0: 7a65 5f73 7061 6365 5f64 656c 696d 6974  ze_space_delimit
+00005ff0: 6564 2863 6173 745f 696e 5f64 6174 612c  ed(cast_in_data,
+00006000: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
+00006010: 725f 6974 6572 6174 6f72 290a 2020 2020  r_iterator).    
+00006020: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00006030: 2073 656c 662e 7374 796c 6520 6973 2050   self.style is P
+00006040: 6172 616d 6574 6572 5374 796c 652e 5049  arameterStyle.PI
+00006050: 5045 5f44 454c 494d 4954 4544 3a0a 2020  PE_DELIMITED:.  
+00006060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006070: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
+00006080: 7365 7269 616c 697a 655f 7069 7065 5f64  serialize_pipe_d
+00006090: 656c 696d 6974 6564 2863 6173 745f 696e  elimited(cast_in
+000060a0: 5f64 6174 612c 2070 7265 6669 785f 7365  _data, prefix_se
+000060b0: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
+000060c0: 290a 2020 2020 2020 2020 2320 7365 6c66  ).        # self
+000060d0: 2e63 6f6e 7465 6e74 2077 696c 6c20 6265  .content will be
+000060e0: 206c 656e 6774 6820 6f6e 650a 2020 2020   length one.    
+000060f0: 2020 2020 6966 2070 7265 6669 785f 7365      if prefix_se
+00006100: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
+00006110: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00006120: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
+00006130: 6172 6174 6f72 5f69 7465 7261 746f 7220  arator_iterator 
+00006140: 3d20 7365 6c66 2e67 6574 5f70 7265 6669  = self.get_prefi
+00006150: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
+00006160: 6174 6f72 2829 0a20 2020 2020 2020 2066  ator().        f
+00006170: 6f72 2063 6f6e 7465 6e74 5f74 7970 652c  or content_type,
+00006180: 2073 6368 656d 6120 696e 2073 656c 662e   schema in self.
+00006190: 636f 6e74 656e 742e 6974 656d 7328 293a  content.items():
+000061a0: 0a20 2020 2020 2020 2020 2020 2063 6173  .            cas
+000061b0: 745f 696e 5f64 6174 6120 3d20 7363 6865  t_in_data = sche
+000061c0: 6d61 2869 6e5f 6461 7461 290a 2020 2020  ma(in_data).    
+000061d0: 2020 2020 2020 2020 6361 7374 5f69 6e5f          cast_in_
+000061e0: 6461 7461 203d 2073 656c 662e 5f6a 736f  data = self._jso
+000061f0: 6e5f 656e 636f 6465 722e 6465 6661 756c  n_encoder.defaul
+00006200: 7428 6361 7374 5f69 6e5f 6461 7461 290a  t(cast_in_data).
+00006210: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00006220: 656c 662e 5f63 6f6e 7465 6e74 5f74 7970  elf._content_typ
+00006230: 655f 6973 5f6a 736f 6e28 636f 6e74 656e  e_is_json(conten
+00006240: 745f 7479 7065 293a 0a20 2020 2020 2020  t_type):.       
+00006250: 2020 2020 2020 2020 2076 616c 7565 203d           value =
+00006260: 2073 656c 662e 5f73 6572 6961 6c69 7a65   self._serialize
+00006270: 5f6a 736f 6e28 6361 7374 5f69 6e5f 6461  _json(cast_in_da
+00006280: 7461 2c20 656c 696d 696e 6174 655f 7768  ta, eliminate_wh
+00006290: 6974 6573 7061 6365 3d54 7275 6529 0a20  itespace=True). 
+000062a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000062b0: 6574 7572 6e20 7365 6c66 2e5f 746f 5f64  eturn self._to_d
+000062c0: 6963 7428 0a20 2020 2020 2020 2020 2020  ict(.           
+000062d0: 2020 2020 2020 2020 2073 656c 662e 6e61           self.na
+000062e0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+000062f0: 2020 2020 2020 2020 6e65 7874 2870 7265          next(pre
+00006300: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
+00006310: 6572 6174 6f72 2920 2b20 7365 6c66 2e6e  erator) + self.n
+00006320: 616d 6520 2b20 273d 2720 2b20 7175 6f74  ame + '=' + quot
+00006330: 6528 7661 6c75 6529 0a20 2020 2020 2020  e(value).       
+00006340: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00006350: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+00006360: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00006370: 2827 5365 7269 616c 697a 6174 696f 6e20  ('Serialization 
+00006380: 6f66 207b 7d20 6861 7320 6e6f 7420 7965  of {} has not ye
+00006390: 7420 6265 656e 2069 6d70 6c65 6d65 6e74  t been implement
+000063a0: 6564 272e 666f 726d 6174 2863 6f6e 7465  ed'.format(conte
+000063b0: 6e74 5f74 7970 6529 290a 0a0a 636c 6173  nt_type))...clas
+000063c0: 7320 436f 6f6b 6965 5061 7261 6d65 7465  s CookieParamete
+000063d0: 7228 5061 7261 6d65 7465 7242 6173 652c  r(ParameterBase,
+000063e0: 2053 7479 6c65 466f 726d 5365 7269 616c   StyleFormSerial
+000063f0: 697a 6572 293a 0a0a 2020 2020 6465 6620  izer):..    def 
+00006400: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+00006410: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00006420: 6e61 6d65 3a20 7374 722c 0a20 2020 2020  name: str,.     
+00006430: 2020 2072 6571 7569 7265 643a 2062 6f6f     required: boo
+00006440: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
+00006450: 2020 2073 7479 6c65 3a20 7479 7069 6e67     style: typing
+00006460: 2e4f 7074 696f 6e61 6c5b 5061 7261 6d65  .Optional[Parame
+00006470: 7465 7253 7479 6c65 5d20 3d20 4e6f 6e65  terStyle] = None
+00006480: 2c0a 2020 2020 2020 2020 6578 706c 6f64  ,.        explod
+00006490: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
+000064a0: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 652c  al[bool] = None,
+000064b0: 0a20 2020 2020 2020 2061 6c6c 6f77 5f72  .        allow_r
+000064c0: 6573 6572 7665 643a 2074 7970 696e 672e  eserved: typing.
+000064d0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+000064e0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+000064f0: 6368 656d 613a 2074 7970 696e 672e 4f70  chema: typing.Op
+00006500: 7469 6f6e 616c 5b74 7970 696e 672e 5479  tional[typing.Ty
+00006510: 7065 5b53 6368 656d 615d 5d20 3d20 4e6f  pe[Schema]] = No
+00006520: 6e65 2c0a 2020 2020 2020 2020 636f 6e74  ne,.        cont
+00006530: 656e 743a 2074 7970 696e 672e 4f70 7469  ent: typing.Opti
+00006540: 6f6e 616c 5b74 7970 696e 672e 4469 6374  onal[typing.Dict
+00006550: 5b73 7472 2c20 7479 7069 6e67 2e54 7970  [str, typing.Typ
+00006560: 655b 5363 6865 6d61 5d5d 5d20 3d20 4e6f  e[Schema]]] = No
+00006570: 6e65 0a20 2020 2029 3a0a 2020 2020 2020  ne.    ):.      
+00006580: 2020 7573 6564 5f73 7479 6c65 203d 2050    used_style = P
+00006590: 6172 616d 6574 6572 5374 796c 652e 464f  arameterStyle.FO
+000065a0: 524d 2069 6620 7374 796c 6520 6973 204e  RM if style is N
+000065b0: 6f6e 6520 616e 6420 636f 6e74 656e 7420  one and content 
+000065c0: 6973 204e 6f6e 6520 616e 6420 7363 6865  is None and sche
+000065d0: 6d61 2065 6c73 6520 7374 796c 650a 2020  ma else style.  
+000065e0: 2020 2020 2020 7573 6564 5f65 7870 6c6f        used_explo
+000065f0: 6465 203d 2073 656c 662e 5f67 6574 5f64  de = self._get_d
+00006600: 6566 6175 6c74 5f65 7870 6c6f 6465 2875  efault_explode(u
+00006610: 7365 645f 7374 796c 6529 2069 6620 6578  sed_style) if ex
+00006620: 706c 6f64 6520 6973 204e 6f6e 6520 656c  plode is None el
+00006630: 7365 2065 7870 6c6f 6465 0a0a 2020 2020  se explode..    
+00006640: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+00006650: 6974 5f5f 280a 2020 2020 2020 2020 2020  it__(.          
+00006660: 2020 6e61 6d65 2c0a 2020 2020 2020 2020    name,.        
+00006670: 2020 2020 696e 5f74 7970 653d 5061 7261      in_type=Para
+00006680: 6d65 7465 7249 6e54 7970 652e 434f 4f4b  meterInType.COOK
+00006690: 4945 2c0a 2020 2020 2020 2020 2020 2020  IE,.            
+000066a0: 7265 7175 6972 6564 3d72 6571 7569 7265  required=require
+000066b0: 642c 0a20 2020 2020 2020 2020 2020 2073  d,.            s
+000066c0: 7479 6c65 3d75 7365 645f 7374 796c 652c  tyle=used_style,
+000066d0: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
+000066e0: 6c6f 6465 3d75 7365 645f 6578 706c 6f64  lode=used_explod
+000066f0: 652c 0a20 2020 2020 2020 2020 2020 2061  e,.            a
+00006700: 6c6c 6f77 5f72 6573 6572 7665 643d 616c  llow_reserved=al
+00006710: 6c6f 775f 7265 7365 7276 6564 2c0a 2020  low_reserved,.  
+00006720: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
+00006730: 3d73 6368 656d 612c 0a20 2020 2020 2020  =schema,.       
+00006740: 2020 2020 2063 6f6e 7465 6e74 3d63 6f6e       content=con
+00006750: 7465 6e74 0a20 2020 2020 2020 2029 0a0a  tent.        )..
+00006760: 2020 2020 6465 6620 7365 7269 616c 697a      def serializ
+00006770: 6528 0a20 2020 2020 2020 2073 656c 662c  e(.        self,
+00006780: 0a20 2020 2020 2020 2069 6e5f 6461 7461  .        in_data
+00006790: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b0a  : typing.Union[.
+000067a0: 2020 2020 2020 2020 2020 2020 5363 6865              Sche
+000067b0: 6d61 2c20 4465 6369 6d61 6c2c 2069 6e74  ma, Decimal, int
+000067c0: 2c20 666c 6f61 742c 2073 7472 2c20 6461  , float, str, da
+000067d0: 7465 2c20 6461 7465 7469 6d65 2c20 4e6f  te, datetime, No
+000067e0: 6e65 2c20 626f 6f6c 2c20 6c69 7374 2c20  ne, bool, list, 
+000067f0: 7475 706c 652c 2064 6963 742c 2066 726f  tuple, dict, fro
+00006800: 7a65 6e64 6963 742e 6672 6f7a 656e 6469  zendict.frozendi
+00006810: 6374 5d0a 2020 2020 2920 2d3e 2074 7970  ct].    ) -> typ
+00006820: 696e 672e 4469 6374 5b73 7472 2c20 7374  ing.Dict[str, st
+00006830: 725d 3a0a 2020 2020 2020 2020 6966 2073  r]:.        if s
+00006840: 656c 662e 7363 6865 6d61 3a0a 2020 2020  elf.schema:.    
+00006850: 2020 2020 2020 2020 6361 7374 5f69 6e5f          cast_in_
+00006860: 6461 7461 203d 2073 656c 662e 7363 6865  data = self.sche
+00006870: 6d61 2869 6e5f 6461 7461 290a 2020 2020  ma(in_data).    
+00006880: 2020 2020 2020 2020 6361 7374 5f69 6e5f          cast_in_
+00006890: 6461 7461 203d 2073 656c 662e 5f6a 736f  data = self._jso
+000068a0: 6e5f 656e 636f 6465 722e 6465 6661 756c  n_encoder.defaul
+000068b0: 7428 6361 7374 5f69 6e5f 6461 7461 290a  t(cast_in_data).
+000068c0: 2020 2020 2020 2020 2020 2020 2222 220a              """.
+000068d0: 2020 2020 2020 2020 2020 2020 666f 726d              form
+000068e0: 202d 3e20 636f 6f6b 6965 0a20 2020 2020   -> cookie.     
+000068f0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00006900: 6e73 2066 6965 6c64 733a 2074 7570 6c65  ns fields: tuple
+00006910: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
+00006920: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00006930: 7365 6c66 2e73 7479 6c65 3a0a 2020 2020  self.style:.    
+00006940: 2020 2020 2020 2020 2020 2020 2222 220a              """.
+00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006960: 544f 444f 2061 6464 2065 7363 6170 696e  TODO add escapin
+00006970: 6720 6f66 2063 6f6d 6d61 2c20 7370 6163  g of comma, spac
+00006980: 652c 2065 7175 616c 730a 2020 2020 2020  e, equals.      
+00006990: 2020 2020 2020 2020 2020 6f72 2074 7572            or tur
+000069a0: 6e20 656e 636f 6469 6e67 206f 6e0a 2020  n encoding on.  
+000069b0: 2020 2020 2020 2020 2020 2020 2020 2222                ""
+000069c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000069d0: 2020 7661 6c75 6520 3d20 7365 6c66 2e5f    value = self._
+000069e0: 7365 7269 616c 697a 655f 666f 726d 280a  serialize_form(.
+000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a00: 2020 2020 6361 7374 5f69 6e5f 6461 7461      cast_in_data
+00006a10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006a20: 2020 2020 2020 6578 706c 6f64 653d 7365        explode=se
+00006a30: 6c66 2e65 7870 6c6f 6465 2c0a 2020 2020  lf.explode,.    
+00006a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a50: 6e61 6d65 3d73 656c 662e 6e61 6d65 2c0a  name=self.name,.
+00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a70: 2020 2020 7065 7263 656e 745f 656e 636f      percent_enco
+00006a80: 6465 3d46 616c 7365 2c0a 2020 2020 2020  de=False,.      
+00006a90: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00006aa0: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+00006ab0: 7465 7261 746f 723d 5072 6566 6978 5365  terator=PrefixSe
+00006ac0: 7061 7261 746f 7249 7465 7261 746f 7228  paratorIterator(
+00006ad0: 2727 2c20 2726 2729 0a20 2020 2020 2020  '', '&').       
+00006ae0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00006af0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00006b00: 6e20 7365 6c66 2e5f 746f 5f64 6963 7428  n self._to_dict(
+00006b10: 7365 6c66 2e6e 616d 652c 2076 616c 7565  self.name, value
+00006b20: 290a 2020 2020 2020 2020 2320 7365 6c66  ).        # self
+00006b30: 2e63 6f6e 7465 6e74 2077 696c 6c20 6265  .content will be
+00006b40: 206c 656e 6774 6820 6f6e 650a 2020 2020   length one.    
+00006b50: 2020 2020 666f 7220 636f 6e74 656e 745f      for content_
+00006b60: 7479 7065 2c20 7363 6865 6d61 2069 6e20  type, schema in 
+00006b70: 7365 6c66 2e63 6f6e 7465 6e74 2e69 7465  self.content.ite
+00006b80: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+00006b90: 2020 6361 7374 5f69 6e5f 6461 7461 203d    cast_in_data =
+00006ba0: 2073 6368 656d 6128 696e 5f64 6174 6129   schema(in_data)
+00006bb0: 0a20 2020 2020 2020 2020 2020 2063 6173  .            cas
+00006bc0: 745f 696e 5f64 6174 6120 3d20 7365 6c66  t_in_data = self
+00006bd0: 2e5f 6a73 6f6e 5f65 6e63 6f64 6572 2e64  ._json_encoder.d
+00006be0: 6566 6175 6c74 2863 6173 745f 696e 5f64  efault(cast_in_d
+00006bf0: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
+00006c00: 2069 6620 7365 6c66 2e5f 636f 6e74 656e   if self._conten
+00006c10: 745f 7479 7065 5f69 735f 6a73 6f6e 2863  t_type_is_json(c
+00006c20: 6f6e 7465 6e74 5f74 7970 6529 3a0a 2020  ontent_type):.  
+00006c30: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00006c40: 6c75 6520 3d20 7365 6c66 2e5f 7365 7269  lue = self._seri
+00006c50: 616c 697a 655f 6a73 6f6e 2863 6173 745f  alize_json(cast_
+00006c60: 696e 5f64 6174 6129 0a20 2020 2020 2020  in_data).       
+00006c70: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00006c80: 7365 6c66 2e5f 746f 5f64 6963 7428 7365  self._to_dict(se
+00006c90: 6c66 2e6e 616d 652c 2076 616c 7565 290a  lf.name, value).
+00006ca0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00006cb0: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
+00006cc0: 4572 726f 7228 2753 6572 6961 6c69 7a61  Error('Serializa
+00006cd0: 7469 6f6e 206f 6620 7b7d 2068 6173 206e  tion of {} has n
+00006ce0: 6f74 2079 6574 2062 6565 6e20 696d 706c  ot yet been impl
+00006cf0: 656d 656e 7465 6427 2e66 6f72 6d61 7428  emented'.format(
+00006d00: 636f 6e74 656e 745f 7479 7065 2929 0a0a  content_type))..
+00006d10: 0a63 6c61 7373 2048 6561 6465 7250 6172  .class HeaderPar
+00006d20: 616d 6574 6572 2850 6172 616d 6574 6572  ameter(Parameter
+00006d30: 4261 7365 2c20 5374 796c 6553 696d 706c  Base, StyleSimpl
+00006d40: 6553 6572 6961 6c69 7a65 7229 3a0a 2020  eSerializer):.  
+00006d50: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00006d60: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00006d70: 2020 2020 2020 6e61 6d65 3a20 7374 722c        name: str,
+00006d80: 0a20 2020 2020 2020 2072 6571 7569 7265  .        require
+00006d90: 643a 2062 6f6f 6c20 3d20 4661 6c73 652c  d: bool = False,
+00006da0: 0a20 2020 2020 2020 2073 7479 6c65 3a20  .        style: 
+00006db0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00006dc0: 5061 7261 6d65 7465 7253 7479 6c65 5d20  ParameterStyle] 
+00006dd0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00006de0: 6578 706c 6f64 653a 2062 6f6f 6c20 3d20  explode: bool = 
+00006df0: 4661 6c73 652c 0a20 2020 2020 2020 2061  False,.        a
+00006e00: 6c6c 6f77 5f72 6573 6572 7665 643a 2074  llow_reserved: t
+00006e10: 7970 696e 672e 4f70 7469 6f6e 616c 5b62  yping.Optional[b
+00006e20: 6f6f 6c5d 203d 204e 6f6e 652c 0a20 2020  ool] = None,.   
+00006e30: 2020 2020 2073 6368 656d 613a 2074 7970       schema: typ
+00006e40: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+00006e50: 696e 672e 5479 7065 5b53 6368 656d 615d  ing.Type[Schema]
+00006e60: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00006e70: 2020 636f 6e74 656e 743a 2074 7970 696e    content: typin
+00006e80: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+00006e90: 672e 4469 6374 5b73 7472 2c20 7479 7069  g.Dict[str, typi
+00006ea0: 6e67 2e54 7970 655b 5363 6865 6d61 5d5d  ng.Type[Schema]]
+00006eb0: 5d20 3d20 4e6f 6e65 0a20 2020 2029 3a0a  ] = None.    ):.
+00006ec0: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+00006ed0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+00006ee0: 2020 2020 2020 6e61 6d65 2c0a 2020 2020        name,.    
+00006ef0: 2020 2020 2020 2020 696e 5f74 7970 653d          in_type=
+00006f00: 5061 7261 6d65 7465 7249 6e54 7970 652e  ParameterInType.
+00006f10: 4845 4144 4552 2c0a 2020 2020 2020 2020  HEADER,.        
+00006f20: 2020 2020 7265 7175 6972 6564 3d72 6571      required=req
+00006f30: 7569 7265 642c 0a20 2020 2020 2020 2020  uired,.         
+00006f40: 2020 2073 7479 6c65 3d73 7479 6c65 2c0a     style=style,.
+00006f50: 2020 2020 2020 2020 2020 2020 6578 706c              expl
+00006f60: 6f64 653d 6578 706c 6f64 652c 0a20 2020  ode=explode,.   
+00006f70: 2020 2020 2020 2020 2061 6c6c 6f77 5f72           allow_r
+00006f80: 6573 6572 7665 643d 616c 6c6f 775f 7265  eserved=allow_re
+00006f90: 7365 7276 6564 2c0a 2020 2020 2020 2020  served,.        
+00006fa0: 2020 2020 7363 6865 6d61 3d73 6368 656d      schema=schem
+00006fb0: 612c 0a20 2020 2020 2020 2020 2020 2063  a,.            c
+00006fc0: 6f6e 7465 6e74 3d63 6f6e 7465 6e74 0a20  ontent=content. 
+00006fd0: 2020 2020 2020 2029 0a0a 2020 2020 4073         )..    @s
+00006fe0: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+00006ff0: 6465 6620 5f5f 746f 5f68 6561 6465 7273  def __to_headers
+00007000: 2869 6e5f 6461 7461 3a20 7479 7069 6e67  (in_data: typing
+00007010: 2e54 7570 6c65 5b74 7970 696e 672e 5475  .Tuple[typing.Tu
+00007020: 706c 655b 7374 722c 2073 7472 5d2c 202e  ple[str, str], .
+00007030: 2e2e 5d29 202d 3e20 4854 5450 4865 6164  ..]) -> HTTPHead
+00007040: 6572 4469 6374 3a0a 2020 2020 2020 2020  erDict:.        
+00007050: 6461 7461 203d 2074 7570 6c65 2874 2066  data = tuple(t f
+00007060: 6f72 2074 2069 6e20 696e 5f64 6174 6120  or t in in_data 
+00007070: 6966 2074 290a 2020 2020 2020 2020 6865  if t).        he
+00007080: 6164 6572 7320 3d20 4854 5450 4865 6164  aders = HTTPHead
+00007090: 6572 4469 6374 2829 0a20 2020 2020 2020  erDict().       
+000070a0: 2069 6620 6e6f 7420 6461 7461 3a0a 2020   if not data:.  
+000070b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000070c0: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
+000070d0: 2068 6561 6465 7273 2e65 7874 656e 6428   headers.extend(
+000070e0: 6461 7461 290a 2020 2020 2020 2020 7265  data).        re
+000070f0: 7475 726e 2068 6561 6465 7273 0a0a 2020  turn headers..  
+00007100: 2020 6465 6620 7365 7269 616c 697a 6528    def serialize(
+00007110: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00007120: 2020 2020 2020 2069 6e5f 6461 7461 3a20         in_data: 
+00007130: 7479 7069 6e67 2e55 6e69 6f6e 5b0a 2020  typing.Union[.  
+00007140: 2020 2020 2020 2020 2020 5363 6865 6d61            Schema
+00007150: 2c20 4465 6369 6d61 6c2c 2069 6e74 2c20  , Decimal, int, 
+00007160: 666c 6f61 742c 2073 7472 2c20 6461 7465  float, str, date
+00007170: 2c20 6461 7465 7469 6d65 2c20 4e6f 6e65  , datetime, None
+00007180: 2c20 626f 6f6c 2c20 6c69 7374 2c20 7475  , bool, list, tu
+00007190: 706c 652c 2064 6963 742c 2066 726f 7a65  ple, dict, froze
+000071a0: 6e64 6963 742e 6672 6f7a 656e 6469 6374  ndict.frozendict
+000071b0: 5d0a 2020 2020 2920 2d3e 2048 5454 5048  ].    ) -> HTTPH
+000071c0: 6561 6465 7244 6963 743a 0a20 2020 2020  eaderDict:.     
+000071d0: 2020 2069 6620 7365 6c66 2e73 6368 656d     if self.schem
+000071e0: 613a 0a20 2020 2020 2020 2020 2020 2063  a:.            c
+000071f0: 6173 745f 696e 5f64 6174 6120 3d20 7365  ast_in_data = se
+00007200: 6c66 2e73 6368 656d 6128 696e 5f64 6174  lf.schema(in_dat
+00007210: 6129 0a20 2020 2020 2020 2020 2020 2063  a).            c
+00007220: 6173 745f 696e 5f64 6174 6120 3d20 7365  ast_in_data = se
+00007230: 6c66 2e5f 6a73 6f6e 5f65 6e63 6f64 6572  lf._json_encoder
+00007240: 2e64 6566 6175 6c74 2863 6173 745f 696e  .default(cast_in
+00007250: 5f64 6174 6129 0a20 2020 2020 2020 2020  _data).         
+00007260: 2020 2022 2222 0a20 2020 2020 2020 2020     """.         
+00007270: 2020 2073 696d 706c 6520 2d3e 2068 6561     simple -> hea
+00007280: 6465 720a 2020 2020 2020 2020 2020 2020  der.            
+00007290: 2020 2020 6865 6164 6572 733a 2050 6f6f      headers: Poo
+000072a0: 6c4d 616e 6167 6572 206e 6565 6473 2061  lManager needs a
+000072b0: 206d 6170 7069 6e67 2c20 7475 706c 6520   mapping, tuple 
+000072c0: 6973 2063 6c6f 7365 0a20 2020 2020 2020  is close.       
+000072d0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000072e0: 7572 6e73 2068 6561 6465 7273 3a20 6469  urns headers: di
+000072f0: 6374 0a20 2020 2020 2020 2020 2020 2022  ct.            "
+00007300: 2222 0a20 2020 2020 2020 2020 2020 2069  "".            i
+00007310: 6620 7365 6c66 2e73 7479 6c65 3a0a 2020  f self.style:.  
+00007320: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00007330: 6c75 6520 3d20 7365 6c66 2e5f 7365 7269  lue = self._seri
+00007340: 616c 697a 655f 7369 6d70 6c65 2863 6173  alize_simple(cas
+00007350: 745f 696e 5f64 6174 612c 2073 656c 662e  t_in_data, self.
+00007360: 6e61 6d65 2c20 7365 6c66 2e65 7870 6c6f  name, self.explo
+00007370: 6465 2c20 4661 6c73 6529 0a20 2020 2020  de, False).     
+00007380: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00007390: 6e20 7365 6c66 2e5f 5f74 6f5f 6865 6164  n self.__to_head
+000073a0: 6572 7328 2828 7365 6c66 2e6e 616d 652c  ers(((self.name,
+000073b0: 2076 616c 7565 292c 2929 0a20 2020 2020   value),)).     
+000073c0: 2020 2023 2073 656c 662e 636f 6e74 656e     # self.conten
+000073d0: 7420 7769 6c6c 2062 6520 6c65 6e67 7468  t will be length
+000073e0: 206f 6e65 0a20 2020 2020 2020 2066 6f72   one.        for
+000073f0: 2063 6f6e 7465 6e74 5f74 7970 652c 2073   content_type, s
+00007400: 6368 656d 6120 696e 2073 656c 662e 636f  chema in self.co
+00007410: 6e74 656e 742e 6974 656d 7328 293a 0a20  ntent.items():. 
+00007420: 2020 2020 2020 2020 2020 2063 6173 745f             cast_
+00007430: 696e 5f64 6174 6120 3d20 7363 6865 6d61  in_data = schema
+00007440: 2869 6e5f 6461 7461 290a 2020 2020 2020  (in_data).      
+00007450: 2020 2020 2020 6361 7374 5f69 6e5f 6461        cast_in_da
+00007460: 7461 203d 2073 656c 662e 5f6a 736f 6e5f  ta = self._json_
+00007470: 656e 636f 6465 722e 6465 6661 756c 7428  encoder.default(
+00007480: 6361 7374 5f69 6e5f 6461 7461 290a 2020  cast_in_data).  
+00007490: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+000074a0: 662e 5f63 6f6e 7465 6e74 5f74 7970 655f  f._content_type_
+000074b0: 6973 5f6a 736f 6e28 636f 6e74 656e 745f  is_json(content_
+000074c0: 7479 7065 293a 0a20 2020 2020 2020 2020  type):.         
+000074d0: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
+000074e0: 656c 662e 5f73 6572 6961 6c69 7a65 5f6a  elf._serialize_j
+000074f0: 736f 6e28 6361 7374 5f69 6e5f 6461 7461  son(cast_in_data
+00007500: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00007510: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
+00007520: 746f 5f68 6561 6465 7273 2828 2873 656c  to_headers(((sel
+00007530: 662e 6e61 6d65 2c20 7661 6c75 6529 2c29  f.name, value),)
+00007540: 290a 2020 2020 2020 2020 2020 2020 7261  ).            ra
+00007550: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
+00007560: 6564 4572 726f 7228 2753 6572 6961 6c69  edError('Seriali
+00007570: 7a61 7469 6f6e 206f 6620 7b7d 2068 6173  zation of {} has
+00007580: 206e 6f74 2079 6574 2062 6565 6e20 696d   not yet been im
+00007590: 706c 656d 656e 7465 6427 2e66 6f72 6d61  plemented'.forma
+000075a0: 7428 636f 6e74 656e 745f 7479 7065 2929  t(content_type))
+000075b0: 0a0a 0a63 6c61 7373 2045 6e63 6f64 696e  ...class Encodin
+000075c0: 673a 0a20 2020 2064 6566 205f 5f69 6e69  g:.    def __ini
+000075d0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+000075e0: 662c 0a20 2020 2020 2020 2063 6f6e 7465  f,.        conte
+000075f0: 6e74 5f74 7970 653a 2073 7472 2c0a 2020  nt_type: str,.  
+00007600: 2020 2020 2020 6865 6164 6572 733a 2074        headers: t
+00007610: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+00007620: 7970 696e 672e 4469 6374 5b73 7472 2c20  yping.Dict[str, 
+00007630: 4865 6164 6572 5061 7261 6d65 7465 725d  HeaderParameter]
+00007640: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00007650: 2020 7374 796c 653a 2074 7970 696e 672e    style: typing.
+00007660: 4f70 7469 6f6e 616c 5b50 6172 616d 6574  Optional[Paramet
+00007670: 6572 5374 796c 655d 203d 204e 6f6e 652c  erStyle] = None,
+00007680: 0a20 2020 2020 2020 2065 7870 6c6f 6465  .        explode
+00007690: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+000076a0: 2020 2020 2020 2020 616c 6c6f 775f 7265          allow_re
+000076b0: 7365 7276 6564 3a20 626f 6f6c 203d 2046  served: bool = F
+000076c0: 616c 7365 2c0a 2020 2020 293a 0a20 2020  alse,.    ):.   
+000076d0: 2020 2020 2073 656c 662e 636f 6e74 656e       self.conten
+000076e0: 745f 7479 7065 203d 2063 6f6e 7465 6e74  t_type = content
+000076f0: 5f74 7970 650a 2020 2020 2020 2020 7365  _type.        se
+00007700: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
+00007710: 6465 7273 0a20 2020 2020 2020 2073 656c  ders.        sel
+00007720: 662e 7374 796c 6520 3d20 7374 796c 650a  f.style = style.
+00007730: 2020 2020 2020 2020 7365 6c66 2e65 7870          self.exp
+00007740: 6c6f 6465 203d 2065 7870 6c6f 6465 0a20  lode = explode. 
+00007750: 2020 2020 2020 2073 656c 662e 616c 6c6f         self.allo
+00007760: 775f 7265 7365 7276 6564 203d 2061 6c6c  w_reserved = all
+00007770: 6f77 5f72 6573 6572 7665 640a 0a0a 4064  ow_reserved...@d
+00007780: 6174 6163 6c61 7373 0a63 6c61 7373 204d  ataclass.class M
+00007790: 6564 6961 5479 7065 3a0a 2020 2020 2222  ediaType:.    ""
+000077a0: 220a 2020 2020 5573 6564 2074 6f20 7374  ".    Used to st
+000077b0: 6f72 6520 7265 7175 6573 7420 616e 6420  ore request and 
+000077c0: 7265 7370 6f6e 7365 2062 6f64 7920 7363  response body sc
+000077d0: 6865 6d61 2069 6e66 6f72 6d61 7469 6f6e  hema information
+000077e0: 0a20 2020 2065 6e63 6f64 696e 673a 0a20  .    encoding:. 
+000077f0: 2020 2020 2020 2041 206d 6170 2062 6574         A map bet
+00007800: 7765 656e 2061 2070 726f 7065 7274 7920  ween a property 
+00007810: 6e61 6d65 2061 6e64 2069 7473 2065 6e63  name and its enc
+00007820: 6f64 696e 6720 696e 666f 726d 6174 696f  oding informatio
+00007830: 6e2e 0a20 2020 2020 2020 2054 6865 206b  n..        The k
+00007840: 6579 2c20 6265 696e 6720 7468 6520 7072  ey, being the pr
+00007850: 6f70 6572 7479 206e 616d 652c 204d 5553  operty name, MUS
+00007860: 5420 6578 6973 7420 696e 2074 6865 2073  T exist in the s
+00007870: 6368 656d 6120 6173 2061 2070 726f 7065  chema as a prope
+00007880: 7274 792e 0a20 2020 2020 2020 2054 6865  rty..        The
+00007890: 2065 6e63 6f64 696e 6720 6f62 6a65 6374   encoding object
+000078a0: 2053 4841 4c4c 206f 6e6c 7920 6170 706c   SHALL only appl
+000078b0: 7920 746f 2072 6571 7565 7374 426f 6479  y to requestBody
+000078c0: 206f 626a 6563 7473 2077 6865 6e20 7468   objects when th
+000078d0: 6520 6d65 6469 6120 7479 7065 2069 730a  e media type is.
+000078e0: 2020 2020 2020 2020 6d75 6c74 6970 6172          multipar
+000078f0: 7420 6f72 2061 7070 6c69 6361 7469 6f6e  t or application
+00007900: 2f78 2d77 7777 2d66 6f72 6d2d 7572 6c65  /x-www-form-urle
+00007910: 6e63 6f64 6564 2e0a 2020 2020 2222 220a  ncoded..    """.
+00007920: 2020 2020 7363 6865 6d61 3a20 7479 7069      schema: typi
+00007930: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
+00007940: 6e67 2e54 7970 655b 5363 6865 6d61 5d5d  ng.Type[Schema]]
+00007950: 203d 204e 6f6e 650a 2020 2020 656e 636f   = None.    enco
+00007960: 6469 6e67 3a20 7479 7069 6e67 2e4f 7074  ding: typing.Opt
+00007970: 696f 6e61 6c5b 7479 7069 6e67 2e44 6963  ional[typing.Dic
+00007980: 745b 7374 722c 2045 6e63 6f64 696e 675d  t[str, Encoding]
+00007990: 5d20 3d20 4e6f 6e65 0a0a 0a40 6461 7461  ] = None...@data
+000079a0: 636c 6173 730a 636c 6173 7320 4170 6952  class.class ApiR
+000079b0: 6573 706f 6e73 6557 6974 686f 7574 4465  esponseWithoutDe
+000079c0: 7365 7269 616c 697a 6174 696f 6e28 4170  serialization(Ap
+000079d0: 6952 6573 706f 6e73 6529 3a0a 2020 2020  iResponse):.    
+000079e0: 7061 7373 0a0a 4064 6174 6163 6c61 7373  pass..@dataclass
+000079f0: 0a63 6c61 7373 2041 7069 5265 7370 6f6e  .class ApiRespon
+00007a00: 7365 5769 7468 6f75 7444 6573 6572 6961  seWithoutDeseria
+00007a10: 6c69 7a61 7469 6f6e 4173 796e 6328 4173  lizationAsync(As
+00007a20: 796e 6341 7069 5265 7370 6f6e 7365 293a  yncApiResponse):
+00007a30: 0a20 2020 2070 6173 730a 0a0a 636c 6173  .    pass...clas
+00007a40: 7320 4f70 656e 4170 6952 6573 706f 6e73  s OpenApiRespons
+00007a50: 6528 4a53 4f4e 4465 7465 6374 6f72 293a  e(JSONDetector):
+00007a60: 0a20 2020 205f 5f66 696c 656e 616d 655f  .    __filename_
+00007a70: 636f 6e74 656e 745f 6469 7370 6f73 6974  content_disposit
+00007a80: 696f 6e5f 7061 7474 6572 6e20 3d20 7265  ion_pattern = re
+00007a90: 2e63 6f6d 7069 6c65 2827 6669 6c65 6e61  .compile('filena
+00007aa0: 6d65 3d22 282e 2b3f 2922 2729 0a0a 2020  me="(.+?)"')..  
+00007ab0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00007ac0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00007ad0: 2020 2020 2020 7265 7370 6f6e 7365 5f63        response_c
+00007ae0: 6c73 3a20 7479 7069 6e67 2e54 7970 655b  ls: typing.Type[
+00007af0: 4170 6952 6573 706f 6e73 655d 203d 2041  ApiResponse] = A
+00007b00: 7069 5265 7370 6f6e 7365 2c0a 2020 2020  piResponse,.    
+00007b10: 2020 2020 7265 7370 6f6e 7365 5f63 6c73      response_cls
+00007b20: 5f61 7379 6e63 3a20 7479 7069 6e67 2e54  _async: typing.T
+00007b30: 7970 655b 4173 796e 6341 7069 5265 7370  ype[AsyncApiResp
+00007b40: 6f6e 7365 5d20 3d20 4173 796e 6341 7069  onse] = AsyncApi
+00007b50: 5265 7370 6f6e 7365 2c0a 2020 2020 2020  Response,.      
+00007b60: 2020 636f 6e74 656e 743a 2074 7970 696e    content: typin
+00007b70: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+00007b80: 672e 4469 6374 5b73 7472 2c20 4d65 6469  g.Dict[str, Medi
+00007b90: 6154 7970 655d 5d20 3d20 4e6f 6e65 2c0a  aType]] = None,.
+00007ba0: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
+00007bb0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00007bc0: 5b74 7970 696e 672e 4c69 7374 5b48 6561  [typing.List[Hea
+00007bd0: 6465 7250 6172 616d 6574 6572 5d5d 203d  derParameter]] =
+00007be0: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+00007bf0: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+00007c00: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
+00007c10: 2020 2020 2069 6620 636f 6e74 656e 7420       if content 
+00007c20: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00007c30: 6c65 6e28 636f 6e74 656e 7429 203d 3d20  len(content) == 
+00007c40: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+00007c50: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00007c60: 2749 6e76 616c 6964 2076 616c 7565 2066  'Invalid value f
+00007c70: 6f72 2063 6f6e 7465 6e74 2c20 7468 6520  or content, the 
+00007c80: 636f 6e74 656e 7420 6469 6374 206d 7573  content dict mus
+00007c90: 7420 6861 7665 203e 3d20 3120 656e 7472  t have >= 1 entr
+00007ca0: 7927 290a 2020 2020 2020 2020 7365 6c66  y').        self
+00007cb0: 2e63 6f6e 7465 6e74 203d 2063 6f6e 7465  .content = conte
+00007cc0: 6e74 0a20 2020 2020 2020 2073 656c 662e  nt.        self.
+00007cd0: 7265 7370 6f6e 7365 5f63 6c73 203d 2072  response_cls = r
+00007ce0: 6573 706f 6e73 655f 636c 730a 2020 2020  esponse_cls.    
+00007cf0: 2020 2020 7365 6c66 2e72 6573 706f 6e73      self.respons
+00007d00: 655f 636c 735f 6173 796e 6320 3d20 7265  e_cls_async = re
+00007d10: 7370 6f6e 7365 5f63 6c73 5f61 7379 6e63  sponse_cls_async
+00007d20: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+00007d30: 686f 640a 2020 2020 6465 6620 5f5f 6465  hod.    def __de
+00007d40: 7365 7269 616c 697a 655f 6a73 6f6e 2872  serialize_json(r
+00007d50: 6573 706f 6e73 653a 2062 7974 6573 2920  esponse: bytes) 
+00007d60: 2d3e 2074 7970 696e 672e 416e 793a 0a20  -> typing.Any:. 
+00007d70: 2020 2020 2020 2023 2070 7974 686f 6e20         # python 
+00007d80: 6d75 7374 2062 6520 3e3d 2033 2e39 2073  must be >= 3.9 s
+00007d90: 6f20 7765 2063 616e 2070 6173 7320 696e  o we can pass in
+00007da0: 2062 7974 6573 2069 6e74 6f20 6a73 6f6e   bytes into json
+00007db0: 2e6c 6f61 6473 0a20 2020 2020 2020 2072  .loads.        r
+00007dc0: 6574 7572 6e20 6a73 6f6e 2e6c 6f61 6473  eturn json.loads
+00007dd0: 2872 6573 706f 6e73 6529 0a0a 2020 2020  (response)..    
+00007de0: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+00007df0: 2020 6465 6620 5f5f 6669 6c65 5f6e 616d    def __file_nam
+00007e00: 655f 6672 6f6d 5f72 6573 706f 6e73 655f  e_from_response_
+00007e10: 7572 6c28 7265 7370 6f6e 7365 5f75 726c  url(response_url
+00007e20: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00007e30: 6c5b 7374 725d 2920 2d3e 2074 7970 696e  l[str]) -> typin
+00007e40: 672e 4f70 7469 6f6e 616c 5b73 7472 5d3a  g.Optional[str]:
+00007e50: 0a20 2020 2020 2020 2069 6620 7265 7370  .        if resp
+00007e60: 6f6e 7365 5f75 726c 2069 7320 4e6f 6e65  onse_url is None
+00007e70: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00007e80: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
+00007e90: 2020 7572 6c5f 7061 7468 203d 2075 726c    url_path = url
+00007ea0: 7061 7273 6528 7265 7370 6f6e 7365 5f75  parse(response_u
+00007eb0: 726c 292e 7061 7468 0a20 2020 2020 2020  rl).path.       
+00007ec0: 2069 6620 7572 6c5f 7061 7468 3a0a 2020   if url_path:.  
+00007ed0: 2020 2020 2020 2020 2020 7061 7468 5f62            path_b
+00007ee0: 6173 656e 616d 6520 3d20 6f73 2e70 6174  asename = os.pat
+00007ef0: 682e 6261 7365 6e61 6d65 2875 726c 5f70  h.basename(url_p
+00007f00: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
+00007f10: 2069 6620 7061 7468 5f62 6173 656e 616d   if path_basenam
+00007f20: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00007f30: 2020 205f 6669 6c65 6e61 6d65 2c20 6578     _filename, ex
+00007f40: 7420 3d20 6f73 2e70 6174 682e 7370 6c69  t = os.path.spli
+00007f50: 7465 7874 2870 6174 685f 6261 7365 6e61  text(path_basena
+00007f60: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+00007f70: 2020 2020 6966 2065 7874 3a0a 2020 2020      if ext:.    
+00007f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f90: 7265 7475 726e 2070 6174 685f 6261 7365  return path_base
+00007fa0: 6e61 6d65 0a20 2020 2020 2020 2072 6574  name.        ret
+00007fb0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 4063  urn None..    @c
+00007fc0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+00007fd0: 6566 205f 5f66 696c 655f 6e61 6d65 5f66  ef __file_name_f
+00007fe0: 726f 6d5f 636f 6e74 656e 745f 6469 7370  rom_content_disp
+00007ff0: 6f73 6974 696f 6e28 636c 732c 2063 6f6e  osition(cls, con
+00008000: 7465 6e74 5f64 6973 706f 7369 7469 6f6e  tent_disposition
+00008010: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00008020: 6c5b 7374 725d 2920 2d3e 2074 7970 696e  l[str]) -> typin
+00008030: 672e 4f70 7469 6f6e 616c 5b73 7472 5d3a  g.Optional[str]:
+00008040: 0a20 2020 2020 2020 2069 6620 636f 6e74  .        if cont
+00008050: 656e 745f 6469 7370 6f73 6974 696f 6e20  ent_disposition 
+00008060: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00008070: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00008080: 0a20 2020 2020 2020 206d 6174 6368 203d  .        match =
+00008090: 2063 6c73 2e5f 5f66 696c 656e 616d 655f   cls.__filename_
+000080a0: 636f 6e74 656e 745f 6469 7370 6f73 6974  content_disposit
+000080b0: 696f 6e5f 7061 7474 6572 6e2e 7365 6172  ion_pattern.sear
+000080c0: 6368 2863 6f6e 7465 6e74 5f64 6973 706f  ch(content_dispo
+000080d0: 7369 7469 6f6e 290a 2020 2020 2020 2020  sition).        
+000080e0: 6966 206e 6f74 206d 6174 6368 3a0a 2020  if not match:.  
+000080f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00008100: 204e 6f6e 650a 2020 2020 2020 2020 7265   None.        re
+00008110: 7475 726e 206d 6174 6368 2e67 726f 7570  turn match.group
+00008120: 2831 290a 0a20 2020 2064 6566 205f 5f64  (1)..    def __d
+00008130: 6573 6572 6961 6c69 7a65 5f61 7070 6c69  eserialize_appli
+00008140: 6361 7469 6f6e 5f6f 6374 6574 5f73 7472  cation_octet_str
+00008150: 6561 6d28 0a20 2020 2020 2020 2073 656c  eam(.        sel
+00008160: 662c 2072 6573 706f 6e73 653a 2075 726c  f, response: url
+00008170: 6c69 6233 2e48 5454 5052 6573 706f 6e73  lib3.HTTPRespons
+00008180: 650a 2020 2020 2920 2d3e 2074 7970 696e  e.    ) -> typin
+00008190: 672e 556e 696f 6e5b 6279 7465 732c 2069  g.Union[bytes, i
+000081a0: 6f2e 4275 6666 6572 6564 5265 6164 6572  o.BufferedReader
+000081b0: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
+000081c0: 2020 2020 2020 2075 726c 6c69 6233 2075         urllib3 u
+000081d0: 7365 2063 6173 6573 3a0a 2020 2020 2020  se cases:.      
+000081e0: 2020 312e 2077 6865 6e20 7072 656c 6f61    1. when preloa
+000081f0: 645f 636f 6e74 656e 743d 5472 7565 2028  d_content=True (
+00008200: 7374 7265 616d 3d46 616c 7365 2920 7468  stream=False) th
+00008210: 656e 2073 7570 706f 7274 735f 6368 756e  en supports_chun
+00008220: 6b65 645f 7265 6164 7320 6973 2046 616c  ked_reads is Fal
+00008230: 7365 2061 6e64 2062 7974 6573 2061 7265  se and bytes are
+00008240: 2072 6574 7572 6e65 640a 2020 2020 2020   returned.      
+00008250: 2020 322e 2077 6865 6e20 7072 656c 6f61    2. when preloa
+00008260: 645f 636f 6e74 656e 743d 4661 6c73 6520  d_content=False 
+00008270: 2873 7472 6561 6d3d 5472 7565 2920 7468  (stream=True) th
+00008280: 656e 2073 7570 706f 7274 735f 6368 756e  en supports_chun
+00008290: 6b65 645f 7265 6164 7320 6973 2054 7275  ked_reads is Tru
+000082a0: 6520 616e 640a 2020 2020 2020 2020 2020  e and.          
+000082b0: 2020 6120 6669 6c65 2077 696c 6c20 6265    a file will be
+000082c0: 2077 7269 7474 656e 2061 6e64 2072 6574   written and ret
+000082d0: 7572 6e65 640a 2020 2020 2020 2020 2222  urned.        ""
+000082e0: 220a 2020 2020 2020 2020 6966 2072 6573  ".        if res
+000082f0: 706f 6e73 652e 7375 7070 6f72 7473 5f63  ponse.supports_c
+00008300: 6875 6e6b 6564 5f72 6561 6473 2829 3a0a  hunked_reads():.
+00008310: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00008320: 5f6e 616d 6520 3d20 280a 2020 2020 2020  _name = (.      
+00008330: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00008340: 5f66 696c 655f 6e61 6d65 5f66 726f 6d5f  _file_name_from_
+00008350: 636f 6e74 656e 745f 6469 7370 6f73 6974  content_disposit
+00008360: 696f 6e28 7265 7370 6f6e 7365 2e68 6561  ion(response.hea
+00008370: 6465 7273 2e67 6574 2827 636f 6e74 656e  ders.get('conten
+00008380: 742d 6469 7370 6f73 6974 696f 6e27 2929  t-disposition'))
+00008390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000083a0: 206f 7220 7365 6c66 2e5f 5f66 696c 655f   or self.__file_
+000083b0: 6e61 6d65 5f66 726f 6d5f 7265 7370 6f6e  name_from_respon
+000083c0: 7365 5f75 726c 2872 6573 706f 6e73 652e  se_url(response.
+000083d0: 6765 7475 726c 2829 290a 2020 2020 2020  geturl()).      
+000083e0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+000083f0: 2020 2020 2069 6620 6669 6c65 5f6e 616d       if file_nam
+00008400: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+00008410: 2020 2020 2020 2020 2020 205f 6664 2c20             _fd, 
+00008420: 7061 7468 203d 2074 656d 7066 696c 652e  path = tempfile.
+00008430: 6d6b 7374 656d 7028 290a 2020 2020 2020  mkstemp().      
+00008440: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00008450: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00008460: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00008470: 7465 6d70 6669 6c65 2e67 6574 7465 6d70  tempfile.gettemp
+00008480: 6469 7228 292c 2066 696c 655f 6e61 6d65  dir(), file_name
+00008490: 290a 0a20 2020 2020 2020 2020 2020 2077  )..            w
+000084a0: 6974 6820 6f70 656e 2870 6174 682c 2027  ith open(path, '
+000084b0: 7762 2729 2061 7320 6e65 775f 6669 6c65  wb') as new_file
+000084c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000084d0: 2020 6368 756e 6b5f 7369 7a65 203d 2031    chunk_size = 1
+000084e0: 3032 340a 2020 2020 2020 2020 2020 2020  024.            
+000084f0: 2020 2020 7768 696c 6520 5472 7565 3a0a      while True:.
+00008500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008510: 2020 2020 6461 7461 203d 2072 6573 706f      data = respo
+00008520: 6e73 652e 7265 6164 2863 6875 6e6b 5f73  nse.read(chunk_s
+00008530: 697a 6529 0a20 2020 2020 2020 2020 2020  ize).           
+00008540: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00008550: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
+00008560: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00008570: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
+00008580: 2020 2020 2020 2020 6e65 775f 6669 6c65          new_file
+00008590: 2e77 7269 7465 2864 6174 6129 0a20 2020  .write(data).   
+000085a0: 2020 2020 2020 2020 2023 2072 656c 6561           # relea
+000085b0: 7365 5f63 6f6e 6e20 6973 206e 6565 6465  se_conn is neede
+000085c0: 6420 666f 7220 7374 7265 616d 696e 6720  d for streaming 
+000085d0: 636f 6e6e 6563 7469 6f6e 7320 6f6e 6c79  connections only
+000085e0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000085f0: 706f 6e73 652e 7265 6c65 6173 655f 636f  ponse.release_co
+00008600: 6e6e 2829 0a20 2020 2020 2020 2020 2020  nn().           
+00008610: 206e 6577 5f66 696c 6520 3d20 6f70 656e   new_file = open
+00008620: 2870 6174 682c 2027 7262 2729 0a20 2020  (path, 'rb').   
+00008630: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008640: 6e65 775f 6669 6c65 0a20 2020 2020 2020  new_file.       
+00008650: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00008660: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
+00008670: 7365 2e64 6174 610a 0a20 2020 2040 7374  se.data..    @st
+00008680: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+00008690: 6566 205f 5f64 6573 6572 6961 6c69 7a65  ef __deserialize
+000086a0: 5f6d 756c 7469 7061 7274 5f66 6f72 6d5f  _multipart_form_
+000086b0: 6461 7461 280a 2020 2020 2020 2020 7265  data(.        re
+000086c0: 7370 6f6e 7365 3a20 6279 7465 730a 2020  sponse: bytes.  
+000086d0: 2020 2920 2d3e 2074 7970 696e 672e 4469    ) -> typing.Di
+000086e0: 6374 5b73 7472 2c20 7479 7069 6e67 2e41  ct[str, typing.A
+000086f0: 6e79 5d3a 0a20 2020 2020 2020 206d 7367  ny]:.        msg
+00008700: 203d 2065 6d61 696c 2e6d 6573 7361 6765   = email.message
+00008710: 5f66 726f 6d5f 6279 7465 7328 7265 7370  _from_bytes(resp
+00008720: 6f6e 7365 290a 2020 2020 2020 2020 7265  onse).        re
+00008730: 7475 726e 207b 0a20 2020 2020 2020 2020  turn {.         
+00008740: 2020 2070 6172 742e 6765 745f 7061 7261     part.get_para
+00008750: 6d28 226e 616d 6522 2c20 6865 6164 6572  m("name", header
+00008760: 3d22 436f 6e74 656e 742d 4469 7370 6f73  ="Content-Dispos
+00008770: 6974 696f 6e22 293a 2070 6172 742e 6765  ition"): part.ge
+00008780: 745f 7061 796c 6f61 6428 0a20 2020 2020  t_payload(.     
+00008790: 2020 2020 2020 2020 2020 2064 6563 6f64             decod
+000087a0: 653d 5472 7565 0a20 2020 2020 2020 2020  e=True.         
+000087b0: 2020 2029 2e64 6563 6f64 6528 7061 7274     ).decode(part
+000087c0: 2e67 6574 5f63 6f6e 7465 6e74 5f63 6861  .get_content_cha
+000087d0: 7273 6574 2829 290a 2020 2020 2020 2020  rset()).        
+000087e0: 2020 2020 6966 2070 6172 742e 6765 745f      if part.get_
+000087f0: 636f 6e74 656e 745f 6368 6172 7365 7428  content_charset(
+00008800: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00008810: 7365 2070 6172 742e 6765 745f 7061 796c  se part.get_payl
+00008820: 6f61 6428 290a 2020 2020 2020 2020 2020  oad().          
+00008830: 2020 666f 7220 7061 7274 2069 6e20 6d73    for part in ms
+00008840: 672e 6765 745f 7061 796c 6f61 6428 290a  g.get_payload().
+00008850: 2020 2020 2020 2020 7d0a 0a20 2020 2064          }..    d
+00008860: 6566 205f 5f67 6574 5f73 6368 656d 615f  ef __get_schema_
+00008870: 666f 725f 636f 6e74 656e 745f 7479 7065  for_content_type
+00008880: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00008890: 2020 2020 2020 2020 636f 6e74 656e 745f          content_
+000088a0: 7479 7065 0a20 2020 2029 202d 3e20 7479  type.    ) -> ty
+000088b0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+000088c0: 7069 6e67 2e54 7970 655b 5363 6865 6d61  ping.Type[Schema
+000088d0: 5d5d 3a0a 2020 2020 2020 2020 2222 220a  ]]:.        """.
+000088e0: 2020 2020 2020 2020 4669 6e64 7320 7468          Finds th
+000088f0: 6520 636f 7272 6563 7420 5363 6865 6d61  e correct Schema
+00008900: 4f62 6a65 6374 2066 6f72 2061 2070 6172  Object for a par
+00008910: 7469 6375 6c61 7220 636f 6e74 656e 7420  ticular content 
+00008920: 7479 7065 2e20 4861 6e64 6c65 730a 2020  type. Handles.  
+00008930: 2020 2020 2020 7468 6520 6173 7465 7269        the asteri
+00008940: 736b 2022 2a22 2063 6861 7261 6374 6572  sk "*" character
+00008950: 2074 6861 7420 6973 2075 7365 6420 746f   that is used to
+00008960: 2067 726f 7570 206d 6564 6961 2074 7970   group media typ
+00008970: 6573 2069 6e74 6f20 7261 6e67 6573 0a20  es into ranges. 
+00008980: 2020 2020 2020 2028 6874 7470 733a 2f2f         (https://
+00008990: 7777 772e 7266 632d 6564 6974 6f72 2e6f  www.rfc-editor.o
+000089a0: 7267 2f72 6663 2f72 6663 3732 3331 2373  rg/rfc/rfc7231#s
+000089b0: 6563 7469 6f6e 2d35 2e33 2e32 292e 2041  ection-5.3.2). A
+000089c0: 6c73 6f20 6861 6e64 6c65 730a 2020 2020  lso handles.    
+000089d0: 2020 2020 7061 7261 6d65 7465 7273 2069      parameters i
+000089e0: 6e20 7468 6520 666f 726d 206f 6620 6e61  n the form of na
+000089f0: 6d65 3d76 616c 7565 2070 6169 7273 2e0a  me=value pairs..
+00008a00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00008a10: 2020 2020 6d65 6469 615f 7479 7065 7320      media_types 
+00008a20: 3d20 7365 6c66 2e63 6f6e 7465 6e74 2e6b  = self.content.k
+00008a30: 6579 7328 290a 2020 2020 2020 2020 6d61  eys().        ma
+00008a40: 7463 6865 645f 6d65 6469 615f 7479 7065  tched_media_type
+00008a50: 203d 204f 7065 6e41 7069 5265 7370 6f6e   = OpenApiRespon
+00008a60: 7365 2e6d 6174 6368 5f63 6f6e 7465 6e74  se.match_content
+00008a70: 5f74 7970 6528 0a20 2020 2020 2020 2020  _type(.         
+00008a80: 2020 2063 6f6e 7465 6e74 5f74 7970 653d     content_type=
+00008a90: 636f 6e74 656e 745f 7479 7065 2c0a 2020  content_type,.  
+00008aa0: 2020 2020 2020 2020 2020 6d65 6469 615f            media_
+00008ab0: 7479 7065 733d 6d65 6469 615f 7479 7065  types=media_type
+00008ac0: 730a 2020 2020 2020 2020 290a 2020 2020  s.        ).    
+00008ad0: 2020 2020 6966 206d 6174 6368 6564 5f6d      if matched_m
+00008ae0: 6564 6961 5f74 7970 6520 6973 204e 6f6e  edia_type is Non
+00008af0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00008b00: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
+00008b10: 2020 2072 6574 7572 6e20 7365 6c66 2e63     return self.c
+00008b20: 6f6e 7465 6e74 5b6d 6174 6368 6564 5f6d  ontent[matched_m
+00008b30: 6564 6961 5f74 7970 655d 2e73 6368 656d  edia_type].schem
+00008b40: 610a 0a20 2020 2040 7374 6174 6963 6d65  a..    @staticme
+00008b50: 7468 6f64 0a20 2020 2064 6566 206d 6174  thod.    def mat
+00008b60: 6368 5f63 6f6e 7465 6e74 5f74 7970 6528  ch_content_type(
+00008b70: 636f 6e74 656e 745f 7479 7065 3a20 7374  content_type: st
+00008b80: 722c 206d 6564 6961 5f74 7970 6573 3a20  r, media_types: 
+00008b90: 7479 7069 6e67 2e4c 6973 745b 7374 725d  typing.List[str]
+00008ba0: 2920 2d3e 2074 7970 696e 672e 4f70 7469  ) -> typing.Opti
+00008bb0: 6f6e 616c 5b73 7472 5d3a 0a20 2020 2020  onal[str]:.     
+00008bc0: 2020 2022 2222 0a20 2020 2020 2020 204d     """.        M
+00008bd0: 6174 6368 6573 2061 2063 6f6e 7465 6e74  atches a content
+00008be0: 2074 7970 6520 746f 2061 206d 6564 6961   type to a media
+00008bf0: 2074 7970 6520 696e 2061 206c 6973 7420   type in a list 
+00008c00: 6f66 206d 6564 6961 2074 7970 6573 2c20  of media types, 
+00008c10: 6861 6e64 6c69 6e67 206d 6564 6961 2074  handling media t
+00008c20: 7970 6520 7261 6e67 6573 2061 7320 6465  ype ranges as de
+00008c30: 6669 6e65 6420 696e 2052 4643 3732 3331  fined in RFC7231
+00008c40: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00008c50: 6574 6572 733a 0a20 2020 2020 2020 2063  eters:.        c
+00008c60: 6f6e 7465 6e74 5f74 7970 6520 2873 7472  ontent_type (str
+00008c70: 293a 2054 6865 2063 6f6e 7465 6e74 2074  ): The content t
+00008c80: 7970 6520 746f 206d 6174 6368 2e0a 2020  ype to match..  
+00008c90: 2020 2020 2020 6d65 6469 615f 7479 7065        media_type
+00008ca0: 7320 286c 6973 7429 3a20 5468 6520 6c69  s (list): The li
+00008cb0: 7374 206f 6620 6d65 6469 6120 7479 7065  st of media type
+00008cc0: 7320 746f 2073 6561 7263 682e 0a0a 2020  s to search...  
+00008cd0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00008ce0: 2020 2020 2020 2073 7472 3a20 5468 6520         str: The 
+00008cf0: 6669 7273 7420 6d65 6469 6120 7479 7065  first media type
+00008d00: 2074 6861 7420 6d61 7463 6865 7320 7468   that matches th
+00008d10: 6520 636f 6e74 656e 7420 7479 7065 2c20  e content type, 
+00008d20: 6f72 204e 6f6e 6520 6966 206e 6f20 6d61  or None if no ma
+00008d30: 7463 6820 6973 2066 6f75 6e64 2e0a 2020  tch is found..  
+00008d40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00008d50: 2020 666f 7220 6d65 6469 615f 7479 7065    for media_type
+00008d60: 2069 6e20 6d65 6469 615f 7479 7065 733a   in media_types:
+00008d70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00008d80: 6d65 6469 615f 7479 7065 203d 3d20 272a  media_type == '*
+00008d90: 2f2a 2720 6f72 206d 6564 6961 5f74 7970  /*' or media_typ
+00008da0: 6520 3d3d 2063 6f6e 7465 6e74 5f74 7970  e == content_typ
+00008db0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00008dc0: 2020 2072 6574 7572 6e20 6d65 6469 615f     return media_
+00008dd0: 7479 7065 0a20 2020 2020 2020 2020 2020  type.           
+00008de0: 2065 6c69 6620 272f 2720 696e 206d 6564   elif '/' in med
+00008df0: 6961 5f74 7970 653a 0a20 2020 2020 2020  ia_type:.       
+00008e00: 2020 2020 2020 2020 2074 7970 655f 2c20           type_, 
+00008e10: 7375 6274 7970 6520 3d20 6d65 6469 615f  subtype = media_
+00008e20: 7479 7065 2e73 706c 6974 2827 2f27 290a  type.split('/').
+00008e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e40: 6966 2028 7479 7065 5f20 3d3d 2027 2a27  if (type_ == '*'
+00008e50: 206f 7220 7479 7065 5f20 3d3d 2063 6f6e   or type_ == con
+00008e60: 7465 6e74 5f74 7970 652e 7370 6c69 7428  tent_type.split(
+00008e70: 272f 2729 5b30 5d29 2061 6e64 205c 0a20  '/')[0]) and \. 
+00008e80: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00008e90: 7375 6274 7970 6520 3d3d 2027 2a27 206f  subtype == '*' o
+00008ea0: 7220 7375 6274 7970 6520 3d3d 2063 6f6e  r subtype == con
+00008eb0: 7465 6e74 5f74 7970 652e 7370 6c69 7428  tent_type.split(
+00008ec0: 272f 2729 5b31 5d2e 7370 6c69 7428 273b  '/')[1].split(';
+00008ed0: 2729 5b30 5d29 3a0a 2020 2020 2020 2020  ')[0]):.        
+00008ee0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00008ef0: 726e 206d 6564 6961 5f74 7970 650a 0a20  rn media_type.. 
+00008f00: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00008f10: 6e65 0a0a 2020 2020 6173 796e 6320 6465  ne..    async de
+00008f20: 6620 6465 7365 7269 616c 697a 655f 6173  f deserialize_as
+00008f30: 796e 6328 7365 6c66 2c20 7265 7370 6f6e  ync(self, respon
+00008f40: 7365 3a20 4173 796e 6352 6573 706f 6e73  se: AsyncRespons
+00008f50: 6557 7261 7070 6572 2c20 636f 6e66 6967  eWrapper, config
+00008f60: 7572 6174 696f 6e3a 2043 6f6e 6669 6775  uration: Configu
+00008f70: 7261 7469 6f6e 2c20 736b 6970 5f64 6573  ration, skip_des
+00008f80: 6572 6961 6c69 7a61 7469 6f6e 203d 2046  erialization = F
+00008f90: 616c 7365 2920 2d3e 2041 7379 6e63 4170  alse) -> AsyncAp
+00008fa0: 6952 6573 706f 6e73 653a 0a20 2020 2020  iResponse:.     
+00008fb0: 2020 2022 2222 0a20 2020 2020 2020 2044     """.        D
+00008fc0: 6573 6572 6961 6c69 7a65 7320 616e 2048  eserializes an H
+00008fd0: 5454 5020 7265 7370 6f6e 7365 2062 6f64  TTP response bod
+00008fe0: 7920 696e 746f 2061 6e20 6f62 6a65 6374  y into an object
+00008ff0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00009000: 2020 2020 2020 636f 6e74 656e 745f 7479        content_ty
+00009010: 7065 203d 2072 6573 706f 6e73 652e 6874  pe = response.ht
+00009020: 7470 5f72 6573 706f 6e73 652e 636f 6e74  tp_response.cont
+00009030: 656e 745f 7479 7065 0a20 2020 2020 2020  ent_type.       
+00009040: 2064 6573 6572 6961 6c69 7a65 645f 626f   deserialized_bo
+00009050: 6479 203d 2075 6e73 6574 0a20 2020 2020  dy = unset.     
+00009060: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
+00009070: 6e74 2069 7320 6e6f 7420 4e6f 6e65 3a0a  nt is not None:.
+00009080: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00009090: 656e 2873 656c 662e 636f 6e74 656e 7429  en(self.content)
+000090a0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+000090b0: 2020 2020 2020 2023 2073 6f6d 6520 7370         # some sp
+000090c0: 6563 7320 646f 206e 6f74 2064 6566 696e  ecs do not defin
+000090d0: 6520 7265 7370 6f6e 7365 2063 6f6e 7465  e response conte
+000090e0: 6e74 206d 6564 6961 2074 7970 6520 7363  nt media type sc
+000090f0: 6865 6d61 730a 2020 2020 2020 2020 2020  hemas.          
+00009100: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00009110: 662e 7265 7370 6f6e 7365 5f63 6c73 5f61  f.response_cls_a
+00009120: 7379 6e63 280a 2020 2020 2020 2020 2020  sync(.          
+00009130: 2020 2020 2020 2020 2020 726f 756e 645f            round_
+00009140: 7472 6970 5f74 696d 653d 7265 7370 6f6e  trip_time=respon
+00009150: 7365 2e72 6f75 6e64 5f74 7269 705f 7469  se.round_trip_ti
+00009160: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00009170: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00009180: 3d72 6573 706f 6e73 652e 6874 7470 5f72  =response.http_r
+00009190: 6573 706f 6e73 652c 0a20 2020 2020 2020  esponse,.       
+000091a0: 2020 2020 2020 2020 2020 2020 2062 6f64               bod
+000091b0: 793d 756e 7365 742c 0a20 2020 2020 2020  y=unset,.       
+000091c0: 2020 2020 2020 2020 2020 2020 2068 6561               hea
+000091d0: 6465 7273 3d72 6573 706f 6e73 652e 6874  ders=response.ht
+000091e0: 7470 5f72 6573 706f 6e73 652e 6865 6164  tp_response.head
+000091f0: 6572 732c 0a20 2020 2020 2020 2020 2020  ers,.           
+00009200: 2020 2020 2020 2020 2073 7461 7475 733d           status=
+00009210: 7265 7370 6f6e 7365 2e68 7474 705f 7265  response.http_re
+00009220: 7370 6f6e 7365 2e73 7461 7475 730a 2020  sponse.status.  
+00009230: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00009240: 2020 2020 2020 2020 2020 2020 626f 6479              body
+00009250: 5f73 6368 656d 6120 3d20 7365 6c66 2e5f  _schema = self._
+00009260: 5f67 6574 5f73 6368 656d 615f 666f 725f  _get_schema_for_
+00009270: 636f 6e74 656e 745f 7479 7065 2863 6f6e  content_type(con
+00009280: 7465 6e74 5f74 7970 6529 0a20 2020 2020  tent_type).     
+00009290: 2020 2020 2020 2069 6620 626f 6479 5f73         if body_s
+000092a0: 6368 656d 6120 6973 204e 6f6e 653a 0a20  chema is None:. 
+000092b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000092c0: 6169 7365 2041 7069 5661 6c75 6545 7272  aise ApiValueErr
+000092d0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+000092e0: 2020 2020 2020 2020 6622 496e 7661 6c69          f"Invali
+000092f0: 6420 636f 6e74 656e 745f 7479 7065 2072  d content_type r
+00009300: 6574 7572 6e65 642e 2043 6f6e 7465 6e74  eturned. Content
+00009310: 5f74 7970 653d 277b 636f 6e74 656e 745f  _type='{content_
+00009320: 7479 7065 7d27 2077 6173 2072 6574 7572  type}' was retur
+00009330: 6e65 6420 220a 2020 2020 2020 2020 2020  ned ".          
+00009340: 2020 2020 2020 2020 2020 6622 7768 656e            f"when
+00009350: 206f 6e6c 7920 7b73 7472 2873 6574 2873   only {str(set(s
+00009360: 656c 662e 636f 6e74 656e 7429 297d 2061  elf.content))} a
+00009370: 7265 2064 6566 696e 6564 2066 6f72 2073  re defined for s
+00009380: 7461 7475 735f 636f 6465 3d7b 7374 7228  tatus_code={str(
+00009390: 7265 7370 6f6e 7365 2e68 7474 705f 7265  response.http_re
+000093a0: 7370 6f6e 7365 2e73 7461 7475 7329 7d22  sponse.status)}"
+000093b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000093c0: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
+000093d0: 6620 7365 6c66 2e5f 636f 6e74 656e 745f  f self._content_
+000093e0: 7479 7065 5f69 735f 6a73 6f6e 2863 6f6e  type_is_json(con
+000093f0: 7465 6e74 5f74 7970 6529 3a0a 2020 2020  tent_type):.    
+00009400: 2020 2020 2020 2020 2020 2020 626f 6479              body
+00009410: 5f64 6174 6120 3d20 7365 6c66 2e5f 5f64  _data = self.__d
+00009420: 6573 6572 6961 6c69 7a65 5f6a 736f 6e28  eserialize_json(
+00009430: 6177 6169 7420 7265 7370 6f6e 7365 2e68  await response.h
+00009440: 7474 705f 7265 7370 6f6e 7365 2e72 6561  ttp_response.rea
+00009450: 6428 2929 0a20 2020 2020 2020 2020 2020  d()).           
+00009460: 2065 6c69 6620 636f 6e74 656e 745f 7479   elif content_ty
+00009470: 7065 2e73 7461 7274 7377 6974 6828 276d  pe.startswith('m
+00009480: 756c 7469 7061 7274 2f66 6f72 6d2d 6461  ultipart/form-da
+00009490: 7461 2729 3a0a 2020 2020 2020 2020 2020  ta'):.          
+000094a0: 2020 2020 2020 626f 6479 5f64 6174 6120        body_data 
+000094b0: 3d20 7365 6c66 2e5f 5f64 6573 6572 6961  = self.__deseria
+000094c0: 6c69 7a65 5f6d 756c 7469 7061 7274 5f66  lize_multipart_f
+000094d0: 6f72 6d5f 6461 7461 2861 7761 6974 2072  orm_data(await r
+000094e0: 6573 706f 6e73 652e 6874 7470 5f72 6573  esponse.http_res
+000094f0: 706f 6e73 652e 7265 6164 2829 290a 2020  ponse.read()).  
+00009500: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00009510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009520: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
+00009530: 6e74 6564 4572 726f 7228 2744 6573 6572  ntedError('Deser
+00009540: 6961 6c69 7a61 7469 6f6e 206f 6620 7b7d  ialization of {}
+00009550: 2068 6173 206e 6f74 2079 6574 2062 6565   has not yet bee
+00009560: 6e20 696d 706c 656d 656e 7465 6427 2e66  n implemented'.f
+00009570: 6f72 6d61 7428 636f 6e74 656e 745f 7479  ormat(content_ty
+00009580: 7065 2929 0a20 2020 2020 2020 2020 2020  pe)).           
+00009590: 2069 6620 736b 6970 5f64 6573 6572 6961   if skip_deseria
+000095a0: 6c69 7a61 7469 6f6e 3a0a 2020 2020 2020  lization:.      
+000095b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000095c0: 2073 656c 662e 7265 7370 6f6e 7365 5f63   self.response_c
+000095d0: 6c73 5f61 7379 6e63 280a 2020 2020 2020  ls_async(.      
+000095e0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
+000095f0: 756e 645f 7472 6970 5f74 696d 653d 7265  und_trip_time=re
+00009600: 7370 6f6e 7365 2e72 6f75 6e64 5f74 7269  sponse.round_tri
+00009610: 705f 7469 6d65 2c0a 2020 2020 2020 2020  p_time,.        
+00009620: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+00009630: 6f6e 7365 3d72 6573 706f 6e73 652e 6874  onse=response.ht
+00009640: 7470 5f72 6573 706f 6e73 652c 0a20 2020  tp_response,.   
+00009650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009660: 2062 6f64 793d 626f 6479 5f64 6174 612c   body=body_data,
+00009670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009680: 2020 2020 2068 6561 6465 7273 3d72 6573       headers=res
+00009690: 706f 6e73 652e 6874 7470 5f72 6573 706f  ponse.http_respo
+000096a0: 6e73 652e 6865 6164 6572 732c 0a20 2020  nse.headers,.   
+000096b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096c0: 2073 7461 7475 733d 7265 7370 6f6e 7365   status=response
+000096d0: 2e68 7474 705f 7265 7370 6f6e 7365 2e73  .http_response.s
+000096e0: 7461 7475 730a 2020 2020 2020 2020 2020  tatus.          
+000096f0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00009700: 2020 2020 2320 4578 6563 7574 6520 7661      # Execute va
+00009710: 6c69 6461 7469 6f6e 2061 6e64 2074 6872  lidation and thr
+00009720: 6f77 2061 7320 6120 7369 6465 2065 6666  ow as a side eff
+00009730: 6563 7420 6966 2076 616c 6964 6174 696f  ect if validatio
+00009740: 6e20 6661 696c 730a 2020 2020 2020 2020  n fails.        
+00009750: 2020 2020 626f 6479 5f73 6368 656d 612e      body_schema.
+00009760: 6672 6f6d 5f6f 7065 6e61 7069 5f64 6174  from_openapi_dat
+00009770: 615f 6f61 7067 280a 2020 2020 2020 2020  a_oapg(.        
+00009780: 2020 2020 2020 2020 626f 6479 5f64 6174          body_dat
+00009790: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+000097a0: 2020 205f 636f 6e66 6967 7572 6174 696f     _configuratio
+000097b0: 6e3d 636f 6e66 6967 7572 6174 696f 6e0a  n=configuration.
+000097c0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000097d0: 2020 2020 2020 2020 2020 2320 5661 6c69            # Vali
+000097e0: 6461 7469 6f6e 2070 6173 7365 642c 2073  dation passed, s
+000097f0: 6574 2064 6573 6572 6961 6c69 7a65 645f  et deserialized_
+00009800: 626f 6479 2074 6f20 706c 6169 6e20 6f6c  body to plain ol
+00009810: 6420 6465 7365 7269 616c 697a 6564 2064  d deserialized d
+00009820: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
+00009830: 6465 7365 7269 616c 697a 6564 5f62 6f64  deserialized_bod
+00009840: 7920 3d20 626f 6479 5f64 6174 610a 0a20  y = body_data.. 
+00009850: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00009860: 6c66 2e72 6573 706f 6e73 655f 636c 735f  lf.response_cls_
+00009870: 6173 796e 6328 0a20 2020 2020 2020 2020  async(.         
+00009880: 2020 2072 6f75 6e64 5f74 7269 705f 7469     round_trip_ti
+00009890: 6d65 3d72 6573 706f 6e73 652e 726f 756e  me=response.roun
+000098a0: 645f 7472 6970 5f74 696d 652c 0a20 2020  d_trip_time,.   
+000098b0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+000098c0: 653d 7265 7370 6f6e 7365 2e68 7474 705f  e=response.http_
+000098d0: 7265 7370 6f6e 7365 2c0a 2020 2020 2020  response,.      
+000098e0: 2020 2020 2020 626f 6479 3d64 6573 6572        body=deser
+000098f0: 6961 6c69 7a65 645f 626f 6479 2c0a 2020  ialized_body,.  
+00009900: 2020 2020 2020 2020 2020 6865 6164 6572            header
+00009910: 733d 7265 7370 6f6e 7365 2e68 7474 705f  s=response.http_
+00009920: 7265 7370 6f6e 7365 2e68 6561 6465 7273  response.headers
+00009930: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
+00009940: 6174 7573 3d72 6573 706f 6e73 652e 6874  atus=response.ht
+00009950: 7470 5f72 6573 706f 6e73 652e 7374 6174  tp_response.stat
+00009960: 7573 0a20 2020 2020 2020 2029 0a0a 0a20  us.        )... 
+00009970: 2020 2064 6566 2064 6573 6572 6961 6c69     def deseriali
+00009980: 7a65 2873 656c 662c 2072 6573 706f 6e73  ze(self, respons
+00009990: 653a 2052 6573 706f 6e73 6557 7261 7070  e: ResponseWrapp
+000099a0: 6572 2c20 636f 6e66 6967 7572 6174 696f  er, configuratio
+000099b0: 6e3a 2043 6f6e 6669 6775 7261 7469 6f6e  n: Configuration
+000099c0: 2c20 736b 6970 5f64 6573 6572 6961 6c69  , skip_deseriali
+000099d0: 7a61 7469 6f6e 203d 2046 616c 7365 2920  zation = False) 
+000099e0: 2d3e 2041 7069 5265 7370 6f6e 7365 3a0a  -> ApiResponse:.
+000099f0: 2020 2020 2020 2020 636f 6e74 656e 745f          content_
+00009a00: 7479 7065 203d 2072 6573 706f 6e73 652e  type = response.
+00009a10: 6874 7470 5f72 6573 706f 6e73 652e 6865  http_response.he
+00009a20: 6164 6572 732e 6765 7428 2763 6f6e 7465  aders.get('conte
+00009a30: 6e74 2d74 7970 6527 290a 2020 2020 2020  nt-type').      
+00009a40: 2020 6465 7365 7269 616c 697a 6564 5f62    deserialized_b
+00009a50: 6f64 7920 3d20 756e 7365 740a 2020 2020  ody = unset.    
+00009a60: 2020 2020 7374 7265 616d 6564 203d 2072      streamed = r
+00009a70: 6573 706f 6e73 652e 6874 7470 5f72 6573  esponse.http_res
+00009a80: 706f 6e73 652e 7375 7070 6f72 7473 5f63  ponse.supports_c
+00009a90: 6875 6e6b 6564 5f72 6561 6473 2829 0a0a  hunked_reads()..
+00009aa0: 2020 2020 2020 2020 6465 7365 7269 616c          deserial
+00009ab0: 697a 6564 5f68 6561 6465 7273 203d 2075  ized_headers = u
+00009ac0: 6e73 6574 0a20 2020 2020 2020 2069 6620  nset.        if 
+00009ad0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
+00009ae0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00009af0: 2020 2020 2020 2320 544f 444f 2061 6464        # TODO add
+00009b00: 2068 6561 6465 7220 6465 7365 7269 616c   header deserial
+00009b10: 6961 7469 6f6e 2068 6572 650a 2020 2020  iation here.    
+00009b20: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00009b30: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+00009b40: 6e74 656e 7420 6973 206e 6f74 204e 6f6e  ntent is not Non
+00009b50: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+00009b60: 6620 6c65 6e28 7365 6c66 2e63 6f6e 7465  f len(self.conte
+00009b70: 6e74 2920 3d3d 2030 3a0a 2020 2020 2020  nt) == 0:.      
+00009b80: 2020 2020 2020 2020 2020 2320 736f 6d65            # some
+00009b90: 2073 7065 6373 2064 6f20 6e6f 7420 6465   specs do not de
+00009ba0: 6669 6e65 2072 6573 706f 6e73 6520 636f  fine response co
+00009bb0: 6e74 656e 7420 6d65 6469 6120 7479 7065  ntent media type
+00009bc0: 2073 6368 656d 6173 0a20 2020 2020 2020   schemas.       
+00009bd0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00009be0: 7365 6c66 2e72 6573 706f 6e73 655f 636c  self.response_cl
+00009bf0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+00009c00: 2020 2020 2020 2072 6f75 6e64 5f74 7269         round_tri
+00009c10: 705f 7469 6d65 3d72 6573 706f 6e73 652e  p_time=response.
+00009c20: 726f 756e 645f 7472 6970 5f74 696d 652c  round_trip_time,
+00009c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009c40: 2020 2020 2072 6573 706f 6e73 653d 7265       response=re
+00009c50: 7370 6f6e 7365 2e68 7474 705f 7265 7370  sponse.http_resp
+00009c60: 6f6e 7365 2c0a 2020 2020 2020 2020 2020  onse,.          
+00009c70: 2020 2020 2020 2020 2020 626f 6479 3d75            body=u
+00009c80: 6e73 6574 2c0a 2020 2020 2020 2020 2020  nset,.          
+00009c90: 2020 2020 2020 2020 2020 6865 6164 6572            header
+00009ca0: 733d 7265 7370 6f6e 7365 2e68 7474 705f  s=response.http_
+00009cb0: 7265 7370 6f6e 7365 2e68 6561 6465 7273  response.headers
+00009cc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009cd0: 2020 2020 2020 7374 6174 7573 3d72 6573        status=res
+00009ce0: 706f 6e73 652e 6874 7470 5f72 6573 706f  ponse.http_respo
+00009cf0: 6e73 652e 7374 6174 7573 0a20 2020 2020  nse.status.     
+00009d00: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00009d10: 2020 2020 2020 2020 2062 6f64 795f 7363           body_sc
+00009d20: 6865 6d61 203d 2073 656c 662e 5f5f 6765  hema = self.__ge
+00009d30: 745f 7363 6865 6d61 5f66 6f72 5f63 6f6e  t_schema_for_con
+00009d40: 7465 6e74 5f74 7970 6528 636f 6e74 656e  tent_type(conten
+00009d50: 745f 7479 7065 290a 2020 2020 2020 2020  t_type).        
+00009d60: 2020 2020 6966 2062 6f64 795f 7363 6865      if body_sche
+00009d70: 6d61 2069 7320 4e6f 6e65 3a0a 2020 2020  ma is None:.    
+00009d80: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00009d90: 6520 4170 6956 616c 7565 4572 726f 7228  e ApiValueError(
+00009da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009db0: 2020 2020 2066 2249 6e76 616c 6964 2063       f"Invalid c
+00009dc0: 6f6e 7465 6e74 5f74 7970 6520 7265 7475  ontent_type retu
+00009dd0: 726e 6564 2e20 436f 6e74 656e 745f 7479  rned. Content_ty
+00009de0: 7065 3d27 7b63 6f6e 7465 6e74 5f74 7970  pe='{content_typ
+00009df0: 657d 2720 7761 7320 7265 7475 726e 6564  e}' was returned
+00009e00: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00009e10: 2020 2020 2020 2066 2277 6865 6e20 6f6e         f"when on
+00009e20: 6c79 207b 7374 7228 7365 7428 7365 6c66  ly {str(set(self
+00009e30: 2e63 6f6e 7465 6e74 2929 7d20 6172 6520  .content))} are 
+00009e40: 6465 6669 6e65 6420 666f 7220 7374 6174  defined for stat
+00009e50: 7573 5f63 6f64 653d 7b73 7472 2872 6573  us_code={str(res
+00009e60: 706f 6e73 652e 6874 7470 5f72 6573 706f  ponse.http_respo
+00009e70: 6e73 652e 7374 6174 7573 297d 220a 2020  nse.status)}".  
+00009e80: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00009e90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00009ea0: 7365 6c66 2e5f 636f 6e74 656e 745f 7479  self._content_ty
+00009eb0: 7065 5f69 735f 6a73 6f6e 2863 6f6e 7465  pe_is_json(conte
+00009ec0: 6e74 5f74 7970 6529 3a0a 2020 2020 2020  nt_type):.      
+00009ed0: 2020 2020 2020 2020 2020 626f 6479 5f64            body_d
+00009ee0: 6174 6120 3d20 7365 6c66 2e5f 5f64 6573  ata = self.__des
+00009ef0: 6572 6961 6c69 7a65 5f6a 736f 6e28 7265  erialize_json(re
+00009f00: 7370 6f6e 7365 2e68 7474 705f 7265 7370  sponse.http_resp
+00009f10: 6f6e 7365 2e64 6174 6129 0a20 2020 2020  onse.data).     
+00009f20: 2020 2020 2020 2065 6c69 6620 636f 6e74         elif cont
+00009f30: 656e 745f 7479 7065 203d 3d20 2761 7070  ent_type == 'app
+00009f40: 6c69 6361 7469 6f6e 2f6f 6374 6574 2d73  lication/octet-s
+00009f50: 7472 6561 6d27 3a0a 2020 2020 2020 2020  tream':.        
+00009f60: 2020 2020 2020 2020 626f 6479 5f64 6174          body_dat
+00009f70: 6120 3d20 7365 6c66 2e5f 5f64 6573 6572  a = self.__deser
+00009f80: 6961 6c69 7a65 5f61 7070 6c69 6361 7469  ialize_applicati
+00009f90: 6f6e 5f6f 6374 6574 5f73 7472 6561 6d28  on_octet_stream(
+00009fa0: 7265 7370 6f6e 7365 2e68 7474 705f 7265  response.http_re
+00009fb0: 7370 6f6e 7365 290a 2020 2020 2020 2020  sponse).        
+00009fc0: 2020 2020 656c 6966 2063 6f6e 7465 6e74      elif content
+00009fd0: 5f74 7970 652e 7374 6172 7473 7769 7468  _type.startswith
+00009fe0: 2827 6d75 6c74 6970 6172 742f 666f 726d  ('multipart/form
+00009ff0: 2d64 6174 6127 293a 0a20 2020 2020 2020  -data'):.       
+0000a000: 2020 2020 2020 2020 2062 6f64 795f 6461           body_da
+0000a010: 7461 203d 2073 656c 662e 5f5f 6465 7365  ta = self.__dese
+0000a020: 7269 616c 697a 655f 6d75 6c74 6970 6172  rialize_multipar
+0000a030: 745f 666f 726d 5f64 6174 6128 7265 7370  t_form_data(resp
+0000a040: 6f6e 7365 2e68 7474 705f 7265 7370 6f6e  onse.http_respon
+0000a050: 7365 2e64 6174 6129 0a20 2020 2020 2020  se.data).       
+0000a060: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
+0000a070: 5f74 7970 6520 3d20 276d 756c 7469 7061  _type = 'multipa
+0000a080: 7274 2f66 6f72 6d2d 6461 7461 270a 2020  rt/form-data'.  
+0000a090: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000a0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0b0: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
+0000a0c0: 6e74 6564 4572 726f 7228 2744 6573 6572  ntedError('Deser
+0000a0d0: 6961 6c69 7a61 7469 6f6e 206f 6620 7b7d  ialization of {}
+0000a0e0: 2068 6173 206e 6f74 2079 6574 2062 6565   has not yet bee
+0000a0f0: 6e20 696d 706c 656d 656e 7465 6427 2e66  n implemented'.f
+0000a100: 6f72 6d61 7428 636f 6e74 656e 745f 7479  ormat(content_ty
+0000a110: 7065 2929 0a20 2020 2020 2020 2020 2020  pe)).           
+0000a120: 2069 6620 736b 6970 5f64 6573 6572 6961   if skip_deseria
+0000a130: 6c69 7a61 7469 6f6e 3a0a 2020 2020 2020  lization:.      
+0000a140: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000a150: 2073 656c 662e 7265 7370 6f6e 7365 5f63   self.response_c
+0000a160: 6c73 280a 2020 2020 2020 2020 2020 2020  ls(.            
+0000a170: 2020 2020 2020 2020 726f 756e 645f 7472          round_tr
+0000a180: 6970 5f74 696d 653d 7265 7370 6f6e 7365  ip_time=response
+0000a190: 2e72 6f75 6e64 5f74 7269 705f 7469 6d65  .round_trip_time
+0000a1a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a1b0: 2020 2020 2020 7265 7370 6f6e 7365 3d72        response=r
+0000a1c0: 6573 706f 6e73 652e 6874 7470 5f72 6573  esponse.http_res
+0000a1d0: 706f 6e73 652c 0a20 2020 2020 2020 2020  ponse,.         
+0000a1e0: 2020 2020 2020 2020 2020 2062 6f64 793d             body=
+0000a1f0: 626f 6479 5f64 6174 612c 0a20 2020 2020  body_data,.     
+0000a200: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+0000a210: 6561 6465 7273 3d72 6573 706f 6e73 652e  eaders=response.
+0000a220: 6874 7470 5f72 6573 706f 6e73 652e 6865  http_response.he
+0000a230: 6164 6572 732c 0a20 2020 2020 2020 2020  aders,.         
+0000a240: 2020 2020 2020 2020 2020 2073 7461 7475             statu
+0000a250: 733d 7265 7370 6f6e 7365 2e68 7474 705f  s=response.http_
+0000a260: 7265 7370 6f6e 7365 2e73 7461 7475 730a  response.status.
+0000a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a280: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+0000a290: 2045 7865 6375 7465 2076 616c 6964 6174   Execute validat
+0000a2a0: 696f 6e20 616e 6420 7468 726f 7720 6173  ion and throw as
+0000a2b0: 2061 2073 6964 6520 6566 6665 6374 2069   a side effect i
+0000a2c0: 6620 7661 6c69 6461 7469 6f6e 2066 6169  f validation fai
+0000a2d0: 6c73 0a20 2020 2020 2020 2020 2020 2062  ls.            b
+0000a2e0: 6f64 795f 7363 6865 6d61 2e66 726f 6d5f  ody_schema.from_
+0000a2f0: 6f70 656e 6170 695f 6461 7461 5f6f 6170  openapi_data_oap
+0000a300: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
+0000a310: 2020 2062 6f64 795f 6461 7461 2c0a 2020     body_data,.  
+0000a320: 2020 2020 2020 2020 2020 2020 2020 5f63                _c
+0000a330: 6f6e 6669 6775 7261 7469 6f6e 3d63 6f6e  onfiguration=con
+0000a340: 6669 6775 7261 7469 6f6e 0a20 2020 2020  figuration.     
+0000a350: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000a360: 2020 2020 2023 2056 616c 6964 6174 696f       # Validatio
+0000a370: 6e20 7061 7373 6564 2c20 7365 7420 6465  n passed, set de
+0000a380: 7365 7269 616c 697a 6564 5f62 6f64 7920  serialized_body 
+0000a390: 746f 2070 6c61 696e 206f 6c64 2064 6573  to plain old des
+0000a3a0: 6572 6961 6c69 7a65 6420 6461 7461 0a20  erialized data. 
+0000a3b0: 2020 2020 2020 2020 2020 2064 6573 6572             deser
+0000a3c0: 6961 6c69 7a65 645f 626f 6479 203d 2062  ialized_body = b
+0000a3d0: 6f64 795f 6461 7461 0a20 2020 2020 2020  ody_data.       
+0000a3e0: 2065 6c69 6620 7374 7265 616d 6564 3a0a   elif streamed:.
+0000a3f0: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+0000a400: 6f6e 7365 2e68 7474 705f 7265 7370 6f6e  onse.http_respon
+0000a410: 7365 2e72 656c 6561 7365 5f63 6f6e 6e28  se.release_conn(
+0000a420: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+0000a430: 6e20 7365 6c66 2e72 6573 706f 6e73 655f  n self.response_
+0000a440: 636c 7328 0a20 2020 2020 2020 2020 2020  cls(.           
+0000a450: 2072 6f75 6e64 5f74 7269 705f 7469 6d65   round_trip_time
+0000a460: 3d72 6573 706f 6e73 652e 726f 756e 645f  =response.round_
+0000a470: 7472 6970 5f74 696d 652c 0a20 2020 2020  trip_time,.     
+0000a480: 2020 2020 2020 2072 6573 706f 6e73 653d         response=
+0000a490: 7265 7370 6f6e 7365 2e68 7474 705f 7265  response.http_re
+0000a4a0: 7370 6f6e 7365 2c0a 2020 2020 2020 2020  sponse,.        
+0000a4b0: 2020 2020 626f 6479 3d64 6573 6572 6961      body=deseria
+0000a4c0: 6c69 7a65 645f 626f 6479 2c0a 2020 2020  lized_body,.    
+0000a4d0: 2020 2020 2020 2020 6865 6164 6572 733d          headers=
+0000a4e0: 7265 7370 6f6e 7365 2e68 7474 705f 7265  response.http_re
+0000a4f0: 7370 6f6e 7365 2e68 6561 6465 7273 2c0a  sponse.headers,.
+0000a500: 2020 2020 2020 2020 2020 2020 7374 6174              stat
+0000a510: 7573 3d72 6573 706f 6e73 652e 6874 7470  us=response.http
+0000a520: 5f72 6573 706f 6e73 652e 7374 6174 7573  _response.status
+0000a530: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
+0000a540: 7373 2041 7069 436c 6965 6e74 3a0a 2020  ss ApiClient:.  
+0000a550: 2020 2222 2247 656e 6572 6963 2041 5049    """Generic API
+0000a560: 2063 6c69 656e 7420 666f 7220 4f70 656e   client for Open
+0000a570: 4150 4920 636c 6965 6e74 206c 6962 7261  API client libra
+0000a580: 7279 2062 7569 6c64 732e 0a0a 2020 2020  ry builds...    
+0000a590: 4f70 656e 4150 4920 6765 6e65 7269 6320  OpenAPI generic 
+0000a5a0: 4150 4920 636c 6965 6e74 2e20 5468 6973  API client. This
+0000a5b0: 2063 6c69 656e 7420 6861 6e64 6c65 7320   client handles 
+0000a5c0: 7468 6520 636c 6965 6e74 2d0a 2020 2020  the client-.    
+0000a5d0: 7365 7276 6572 2063 6f6d 6d75 6e69 6361  server communica
+0000a5e0: 7469 6f6e 2c20 616e 6420 6973 2069 6e76  tion, and is inv
+0000a5f0: 6172 6961 6e74 2061 6372 6f73 7320 696d  ariant across im
+0000a600: 706c 656d 656e 7461 7469 6f6e 732e 2053  plementations. S
+0000a610: 7065 6369 6669 6373 206f 660a 2020 2020  pecifics of.    
+0000a620: 7468 6520 6d65 7468 6f64 7320 616e 6420  the methods and 
+0000a630: 6d6f 6465 6c73 2066 6f72 2065 6163 6820  models for each 
+0000a640: 6170 706c 6963 6174 696f 6e20 6172 6520  application are 
+0000a650: 6765 6e65 7261 7465 6420 6672 6f6d 2074  generated from t
+0000a660: 6865 204f 7065 6e41 5049 0a20 2020 2074  he OpenAPI.    t
+0000a670: 656d 706c 6174 6573 2e0a 0a20 2020 2054  emplates...    T
+0000a680: 6869 7320 636c 6173 7320 6973 2061 7574  his class is aut
+0000a690: 6f20 6765 6e65 7261 7465 6420 6279 204b  o generated by K
+0000a6a0: 6f6e 6669 6720 2868 7474 7073 3a2f 2f6b  onfig (https://k
+0000a6b0: 6f6e 6669 6774 6869 732e 636f 6d29 0a0a  onfigthis.com)..
+0000a6c0: 2020 2020 3a70 6172 616d 2063 6f6e 6669      :param confi
+0000a6d0: 6775 7261 7469 6f6e 3a20 2e43 6f6e 6669  guration: .Confi
+0000a6e0: 6775 7261 7469 6f6e 206f 626a 6563 7420  guration object 
+0000a6f0: 666f 7220 7468 6973 2063 6c69 656e 740a  for this client.
+0000a700: 2020 2020 3a70 6172 616d 2068 6561 6465      :param heade
+0000a710: 725f 6e61 6d65 3a20 6120 6865 6164 6572  r_name: a header
+0000a720: 2074 6f20 7061 7373 2077 6865 6e20 6d61   to pass when ma
+0000a730: 6b69 6e67 2063 616c 6c73 2074 6f20 7468  king calls to th
+0000a740: 6520 4150 492e 0a20 2020 203a 7061 7261  e API..    :para
+0000a750: 6d20 6865 6164 6572 5f76 616c 7565 3a20  m header_value: 
+0000a760: 6120 6865 6164 6572 2076 616c 7565 2074  a header value t
+0000a770: 6f20 7061 7373 2077 6865 6e20 6d61 6b69  o pass when maki
+0000a780: 6e67 2063 616c 6c73 2074 6f0a 2020 2020  ng calls to.    
+0000a790: 2020 2020 7468 6520 4150 492e 0a20 2020      the API..   
+0000a7a0: 203a 7061 7261 6d20 636f 6f6b 6965 3a20   :param cookie: 
+0000a7b0: 6120 636f 6f6b 6965 2074 6f20 696e 636c  a cookie to incl
+0000a7c0: 7564 6520 696e 2074 6865 2068 6561 6465  ude in the heade
+0000a7d0: 7220 7768 656e 206d 616b 696e 6720 6361  r when making ca
+0000a7e0: 6c6c 730a 2020 2020 2020 2020 746f 2074  lls.        to t
+0000a7f0: 6865 2041 5049 0a20 2020 203a 7061 7261  he API.    :para
+0000a800: 6d20 706f 6f6c 5f74 6872 6561 6473 3a20  m pool_threads: 
+0000a810: 5468 6520 6e75 6d62 6572 206f 6620 7468  The number of th
+0000a820: 7265 6164 7320 746f 2075 7365 2066 6f72  reads to use for
+0000a830: 2061 7379 6e63 2072 6571 7565 7374 730a   async requests.
+0000a840: 2020 2020 2020 2020 746f 2074 6865 2041          to the A
+0000a850: 5049 2e20 4d6f 7265 2074 6872 6561 6473  PI. More threads
+0000a860: 206d 6561 6e73 206d 6f72 6520 636f 6e63   means more conc
+0000a870: 7572 7265 6e74 2041 5049 2072 6571 7565  urrent API reque
+0000a880: 7374 732e 0a20 2020 2022 2222 0a0a 2020  sts..    """..  
+0000a890: 2020 5f70 6f6f 6c20 3d20 4e6f 6e65 0a0a    _pool = None..
+0000a8a0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0000a8b0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000a8c0: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
+0000a8d0: 6174 696f 6e3a 2074 7970 696e 672e 4f70  ation: typing.Op
+0000a8e0: 7469 6f6e 616c 5b43 6f6e 6669 6775 7261  tional[Configura
+0000a8f0: 7469 6f6e 5d20 3d20 4e6f 6e65 2c0a 2020  tion] = None,.  
+0000a900: 2020 2020 2020 6865 6164 6572 5f6e 616d        header_nam
+0000a910: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
+0000a920: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+0000a930: 2020 2020 2020 2020 6865 6164 6572 5f76          header_v
+0000a940: 616c 7565 3a20 7479 7069 6e67 2e4f 7074  alue: typing.Opt
+0000a950: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000a960: 652c 0a20 2020 2020 2020 2063 6f6f 6b69  e,.        cooki
+0000a970: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
+0000a980: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+0000a990: 2020 2020 2020 2020 706f 6f6c 5f74 6872          pool_thr
+0000a9a0: 6561 6473 3a20 696e 7420 3d20 310a 2020  eads: int = 1.  
+0000a9b0: 2020 293a 0a20 2020 2020 2020 2069 6620    ):.        if 
+0000a9c0: 636f 6e66 6967 7572 6174 696f 6e20 6973  configuration is
+0000a9d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000a9e0: 2020 2063 6f6e 6669 6775 7261 7469 6f6e     configuration
+0000a9f0: 203d 2043 6f6e 6669 6775 7261 7469 6f6e   = Configuration
+0000aa00: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000aa10: 636f 6e66 6967 7572 6174 696f 6e20 3d20  configuration = 
+0000aa20: 636f 6e66 6967 7572 6174 696f 6e0a 2020  configuration.  
+0000aa30: 2020 2020 2020 7365 6c66 2e70 6f6f 6c5f        self.pool_
+0000aa40: 7468 7265 6164 7320 3d20 706f 6f6c 5f74  threads = pool_t
+0000aa50: 6872 6561 6473 0a0a 2020 2020 2020 2020  hreads..        
+0000aa60: 7365 6c66 2e72 6573 745f 636c 6965 6e74  self.rest_client
+0000aa70: 203d 2072 6573 742e 5245 5354 436c 6965   = rest.RESTClie
+0000aa80: 6e74 4f62 6a65 6374 2863 6f6e 6669 6775  ntObject(configu
+0000aa90: 7261 7469 6f6e 290a 2020 2020 2020 2020  ration).        
+0000aaa0: 7365 6c66 2e64 6566 6175 6c74 5f68 6561  self.default_hea
+0000aab0: 6465 7273 203d 2048 5454 5048 6561 6465  ders = HTTPHeade
+0000aac0: 7244 6963 7428 290a 2020 2020 2020 2020  rDict().        
+0000aad0: 6966 2068 6561 6465 725f 6e61 6d65 2069  if header_name i
+0000aae0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000aaf0: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
+0000ab00: 6175 6c74 5f68 6561 6465 7273 5b68 6561  ault_headers[hea
+0000ab10: 6465 725f 6e61 6d65 5d20 3d20 6865 6164  der_name] = head
+0000ab20: 6572 5f76 616c 7565 0a20 2020 2020 2020  er_value.       
+0000ab30: 2073 656c 662e 636f 6f6b 6965 203d 2063   self.cookie = c
+0000ab40: 6f6f 6b69 650a 2020 2020 2020 2020 2320  ookie.        # 
+0000ab50: 5365 7420 6465 6661 756c 7420 5573 6572  Set default User
+0000ab60: 2d41 6765 6e74 2e0a 2020 2020 2020 2020  -Agent..        
+0000ab70: 7365 6c66 2e75 7365 725f 6167 656e 7420  self.user_agent 
+0000ab80: 3d20 274b 6f6e 6669 672f 322e 322e 302f  = 'Konfig/2.2.0/
+0000ab90: 7079 7468 6f6e 270a 0a20 2020 2064 6566  python'..    def
+0000aba0: 205f 5f65 6e74 6572 5f5f 2873 656c 6629   __enter__(self)
+0000abb0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0000abc0: 2073 656c 660a 0a20 2020 2064 6566 205f   self..    def _
+0000abd0: 5f65 7869 745f 5f28 7365 6c66 2c20 6578  _exit__(self, ex
+0000abe0: 635f 7479 7065 2c20 6578 635f 7661 6c75  c_type, exc_valu
+0000abf0: 652c 2074 7261 6365 6261 636b 293a 0a20  e, traceback):. 
+0000ac00: 2020 2020 2020 2073 656c 662e 636c 6f73         self.clos
+0000ac10: 6528 290a 0a20 2020 2064 6566 2063 6c6f  e()..    def clo
+0000ac20: 7365 2873 656c 6629 3a0a 2020 2020 2020  se(self):.      
+0000ac30: 2020 6966 2073 656c 662e 5f70 6f6f 6c3a    if self._pool:
+0000ac40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000ac50: 662e 5f70 6f6f 6c2e 636c 6f73 6528 290a  f._pool.close().
+0000ac60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ac70: 2e5f 706f 6f6c 2e6a 6f69 6e28 290a 2020  ._pool.join().  
+0000ac80: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000ac90: 706f 6f6c 203d 204e 6f6e 650a 2020 2020  pool = None.    
+0000aca0: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
+0000acb0: 7472 2861 7465 7869 742c 2027 756e 7265  tr(atexit, 'unre
+0000acc0: 6769 7374 6572 2729 3a0a 2020 2020 2020  gister'):.      
+0000acd0: 2020 2020 2020 2020 2020 6174 6578 6974            atexit
+0000ace0: 2e75 6e72 6567 6973 7465 7228 7365 6c66  .unregister(self
+0000acf0: 2e63 6c6f 7365 290a 0a20 2020 2040 7072  .close)..    @pr
+0000ad00: 6f70 6572 7479 0a20 2020 2064 6566 2070  operty.    def p
+0000ad10: 6f6f 6c28 7365 6c66 293a 0a20 2020 2020  ool(self):.     
+0000ad20: 2020 2022 2222 4372 6561 7465 2074 6872     """Create thr
+0000ad30: 6561 6420 706f 6f6c 206f 6e20 6669 7273  ead pool on firs
+0000ad40: 7420 7265 7175 6573 740a 2020 2020 2020  t request.      
+0000ad50: 2020 2061 766f 6964 7320 696e 7374 616e     avoids instan
+0000ad60: 7469 6174 696e 6720 756e 7573 6564 2074  tiating unused t
+0000ad70: 6872 6561 6470 6f6f 6c20 666f 7220 626c  hreadpool for bl
+0000ad80: 6f63 6b69 6e67 2063 6c69 656e 7473 2e0a  ocking clients..
+0000ad90: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000ada0: 2020 2020 6966 2073 656c 662e 5f70 6f6f      if self._poo
+0000adb0: 6c20 6973 204e 6f6e 653a 0a20 2020 2020  l is None:.     
+0000adc0: 2020 2020 2020 2061 7465 7869 742e 7265         atexit.re
+0000add0: 6769 7374 6572 2873 656c 662e 636c 6f73  gister(self.clos
+0000ade0: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
+0000adf0: 656c 662e 5f70 6f6f 6c20 3d20 5468 7265  elf._pool = Thre
+0000ae00: 6164 506f 6f6c 2873 656c 662e 706f 6f6c  adPool(self.pool
+0000ae10: 5f74 6872 6561 6473 290a 2020 2020 2020  _threads).      
+0000ae20: 2020 7265 7475 726e 2073 656c 662e 5f70    return self._p
+0000ae30: 6f6f 6c0a 0a20 2020 2040 7072 6f70 6572  ool..    @proper
+0000ae40: 7479 0a20 2020 2064 6566 2075 7365 725f  ty.    def user_
+0000ae50: 6167 656e 7428 7365 6c66 293a 0a20 2020  agent(self):.   
+0000ae60: 2020 2020 2022 2222 5573 6572 2061 6765       """User age
+0000ae70: 6e74 2066 6f72 2074 6869 7320 4150 4920  nt for this API 
+0000ae80: 636c 6965 6e74 2222 220a 2020 2020 2020  client""".      
+0000ae90: 2020 7265 7475 726e 2073 656c 662e 6465    return self.de
+0000aea0: 6661 756c 745f 6865 6164 6572 735b 2755  fault_headers['U
+0000aeb0: 7365 722d 4167 656e 7427 5d0a 0a20 2020  ser-Agent']..   
+0000aec0: 2040 7573 6572 5f61 6765 6e74 2e73 6574   @user_agent.set
+0000aed0: 7465 720a 2020 2020 6465 6620 7573 6572  ter.    def user
+0000aee0: 5f61 6765 6e74 2873 656c 662c 2076 616c  _agent(self, val
+0000aef0: 7565 293a 0a20 2020 2020 2020 2073 656c  ue):.        sel
+0000af00: 662e 6465 6661 756c 745f 6865 6164 6572  f.default_header
+0000af10: 735b 2755 7365 722d 4167 656e 7427 5d20  s['User-Agent'] 
+0000af20: 3d20 7661 6c75 650a 0a20 2020 2064 6566  = value..    def
+0000af30: 2073 6574 5f64 6566 6175 6c74 5f68 6561   set_default_hea
+0000af40: 6465 7228 7365 6c66 2c20 6865 6164 6572  der(self, header
+0000af50: 5f6e 616d 652c 2068 6561 6465 725f 7661  _name, header_va
+0000af60: 6c75 6529 3a0a 2020 2020 2020 2020 7365  lue):.        se
+0000af70: 6c66 2e64 6566 6175 6c74 5f68 6561 6465  lf.default_heade
+0000af80: 7273 5b68 6561 6465 725f 6e61 6d65 5d20  rs[header_name] 
+0000af90: 3d20 6865 6164 6572 5f76 616c 7565 0a0a  = header_value..
+0000afa0: 2020 2020 6173 796e 6320 6465 6620 5f5f      async def __
+0000afb0: 6173 796e 635f 6361 6c6c 5f61 7069 280a  async_call_api(.
+0000afc0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000afd0: 2020 2020 2020 7265 736f 7572 6365 5f70        resource_p
+0000afe0: 6174 683a 2073 7472 2c0a 2020 2020 2020  ath: str,.      
+0000aff0: 2020 6d65 7468 6f64 3a20 7374 722c 0a20    method: str,. 
+0000b000: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
+0000b010: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+0000b020: 4854 5450 4865 6164 6572 4469 6374 5d20  HTTPHeaderDict] 
+0000b030: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000b040: 7365 7269 616c 697a 6564 5f62 6f64 793a  serialized_body:
+0000b050: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0000b060: 5b74 7970 696e 672e 556e 696f 6e5b 7374  [typing.Union[st
+0000b070: 722c 2062 7974 6573 5d5d 203d 204e 6f6e  r, bytes]] = Non
+0000b080: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
+0000b090: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
+0000b0a0: 6e65 2c0a 2020 2020 2020 2020 6669 656c  ne,.        fiel
+0000b0b0: 6473 3a20 7479 7069 6e67 2e4f 7074 696f  ds: typing.Optio
+0000b0c0: 6e61 6c5b 7479 7069 6e67 2e54 7570 6c65  nal[typing.Tuple
+0000b0d0: 5b74 7970 696e 672e 5475 706c 655b 7374  [typing.Tuple[st
+0000b0e0: 722c 2073 7472 5d2c 202e 2e2e 5d5d 203d  r, str], ...]] =
+0000b0f0: 204e 6f6e 652c 0a20 2020 2020 2020 2061   None,.        a
+0000b100: 7574 685f 7365 7474 696e 6773 3a20 7479  uth_settings: ty
+0000b110: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+0000b120: 7069 6e67 2e4c 6973 745b 7374 725d 5d20  ping.List[str]] 
+0000b130: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000b140: 7374 7265 616d 3a20 626f 6f6c 203d 2046  stream: bool = F
+0000b150: 616c 7365 2c0a 2020 2020 2020 2020 7469  alse,.        ti
+0000b160: 6d65 6f75 743a 2074 7970 696e 672e 4f70  meout: typing.Op
+0000b170: 7469 6f6e 616c 5b74 7970 696e 672e 556e  tional[typing.Un
+0000b180: 696f 6e5b 696e 742c 2074 7970 696e 672e  ion[int, typing.
+0000b190: 5475 706c 655d 5d20 3d20 4e6f 6e65 2c0a  Tuple]] = None,.
+0000b1a0: 2020 2020 2020 2020 686f 7374 3a20 7479          host: ty
+0000b1b0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
+0000b1c0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0000b1d0: 2020 2070 7265 6669 785f 7365 7061 7261     prefix_separa
+0000b1e0: 746f 725f 6974 6572 6174 6f72 3a20 5072  tor_iterator: Pr
+0000b1f0: 6566 6978 5365 7061 7261 746f 7249 7465  efixSeparatorIte
+0000b200: 7261 746f 7220 3d20 4e6f 6e65 2c0a 2020  rator = None,.  
+0000b210: 2020 2920 2d3e 2041 7379 6e63 5265 7370    ) -> AsyncResp
+0000b220: 6f6e 7365 5772 6170 7065 723a 0a0a 2020  onseWrapper:..  
+0000b230: 2020 2020 2020 7265 7175 6573 745f 6265        request_be
+0000b240: 666f 7265 5f68 6f6f 6b28 0a20 2020 2020  fore_hook(.     
+0000b250: 2020 2020 2020 2072 6573 6f75 7263 655f         resource_
+0000b260: 7061 7468 3d72 6573 6f75 7263 655f 7061  path=resource_pa
+0000b270: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+0000b280: 6d65 7468 6f64 3d6d 6574 686f 642c 0a20  method=method,. 
+0000b290: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+0000b2a0: 6775 7261 7469 6f6e 3d73 656c 662e 636f  guration=self.co
+0000b2b0: 6e66 6967 7572 6174 696f 6e2c 0a20 2020  nfiguration,.   
+0000b2c0: 2020 2020 2020 2020 2062 6f64 793d 626f           body=bo
+0000b2d0: 6479 2c0a 2020 2020 2020 2020 2020 2020  dy,.            
+0000b2e0: 6669 656c 6473 3d66 6965 6c64 732c 0a20  fields=fields,. 
+0000b2f0: 2020 2020 2020 2020 2020 2061 7574 685f             auth_
+0000b300: 7365 7474 696e 6773 3d61 7574 685f 7365  settings=auth_se
+0000b310: 7474 696e 6773 2c0a 2020 2020 2020 2020  ttings,.        
+0000b320: 2020 2020 6865 6164 6572 733d 6865 6164      headers=head
+0000b330: 6572 732c 0a20 2020 2020 2020 2029 0a0a  ers,.        )..
+0000b340: 2020 2020 2020 2020 2320 6865 6164 6572          # header
+0000b350: 2070 6172 616d 6574 6572 730a 2020 2020   parameters.    
+0000b360: 2020 2020 7573 6564 5f68 6561 6465 7273      used_headers
+0000b370: 203d 2048 5454 5048 6561 6465 7244 6963   = HTTPHeaderDic
+0000b380: 7428 7365 6c66 2e64 6566 6175 6c74 5f68  t(self.default_h
+0000b390: 6561 6465 7273 290a 2020 2020 2020 2020  eaders).        
+0000b3a0: 6966 2073 656c 662e 636f 6f6b 6965 3a0a  if self.cookie:.
+0000b3b0: 2020 2020 2020 2020 2020 2020 6865 6164              head
+0000b3c0: 6572 735b 2743 6f6f 6b69 6527 5d20 3d20  ers['Cookie'] = 
+0000b3d0: 7365 6c66 2e63 6f6f 6b69 650a 0a20 2020  self.cookie..   
+0000b3e0: 2020 2020 2023 2061 7574 6820 7365 7474       # auth sett
+0000b3f0: 696e 670a 2020 2020 2020 2020 7265 736f  ing.        reso
+0000b400: 7572 6365 5f70 6174 6820 3d20 7365 6c66  urce_path = self
+0000b410: 2e75 7064 6174 655f 7061 7261 6d73 5f66  .update_params_f
+0000b420: 6f72 5f61 7574 6828 0a20 2020 2020 2020  or_auth(.       
+0000b430: 2020 2020 2075 7365 645f 6865 6164 6572       used_header
+0000b440: 732c 0a20 2020 2020 2020 2020 2020 2061  s,.            a
+0000b450: 7574 685f 7365 7474 696e 6773 2c0a 2020  uth_settings,.  
+0000b460: 2020 2020 2020 2020 2020 7265 736f 7572            resour
+0000b470: 6365 5f70 6174 682c 0a20 2020 2020 2020  ce_path,.       
+0000b480: 2020 2020 206d 6574 686f 642c 0a20 2020       method,.   
+0000b490: 2020 2020 2020 2020 2062 6f64 792c 0a20           body,. 
+0000b4a0: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
+0000b4b0: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
+0000b4c0: 6174 6f72 0a20 2020 2020 2020 2029 0a0a  ator.        )..
+0000b4d0: 2020 2020 2020 2020 2320 6d75 7374 2068          # must h
+0000b4e0: 6170 7065 6e20 6166 7465 7220 636f 6f6b  appen after cook
+0000b4f0: 6965 2073 6574 7469 6e67 2061 6e64 2061  ie setting and a
+0000b500: 7574 6820 7365 7474 696e 6720 696e 2063  uth setting in c
+0000b510: 6173 6520 7573 6572 2069 7320 6f76 6572  ase user is over
+0000b520: 7269 6469 6e67 2074 686f 7365 0a20 2020  riding those.   
+0000b530: 2020 2020 2069 6620 6865 6164 6572 733a       if headers:
+0000b540: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+0000b550: 645f 6865 6164 6572 732e 7570 6461 7465  d_headers.update
+0000b560: 2868 6561 6465 7273 290a 0a20 2020 2020  (headers)..     
+0000b570: 2020 2023 2072 6571 7565 7374 2075 726c     # request url
+0000b580: 0a20 2020 2020 2020 2069 6620 686f 7374  .        if host
+0000b590: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000b5a0: 2020 2020 2020 7572 6c20 3d20 7365 6c66        url = self
+0000b5b0: 2e63 6f6e 6669 6775 7261 7469 6f6e 2e68  .configuration.h
+0000b5c0: 6f73 7420 2b20 7265 736f 7572 6365 5f70  ost + resource_p
+0000b5d0: 6174 680a 2020 2020 2020 2020 656c 7365  ath.        else
+0000b5e0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000b5f0: 7573 6520 7365 7276 6572 2f68 6f73 7420  use server/host 
+0000b600: 6465 6669 6e65 6420 696e 2070 6174 6820  defined in path 
+0000b610: 6f72 206f 7065 7261 7469 6f6e 2069 6e73  or operation ins
+0000b620: 7465 6164 0a20 2020 2020 2020 2020 2020  tead.           
+0000b630: 2075 726c 203d 2068 6f73 7420 2b20 7265   url = host + re
+0000b640: 736f 7572 6365 5f70 6174 680a 0a20 2020  source_path..   
+0000b650: 2020 2020 2072 6571 7565 7374 5f61 6674       request_aft
+0000b660: 6572 5f68 6f6f 6b28 0a20 2020 2020 2020  er_hook(.       
+0000b670: 2020 2020 2072 6573 6f75 7263 655f 7061       resource_pa
+0000b680: 7468 3d72 6573 6f75 7263 655f 7061 7468  th=resource_path
+0000b690: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
+0000b6a0: 7468 6f64 3d6d 6574 686f 642c 0a20 2020  thod=method,.   
+0000b6b0: 2020 2020 2020 2020 2063 6f6e 6669 6775           configu
+0000b6c0: 7261 7469 6f6e 3d73 656c 662e 636f 6e66  ration=self.conf
+0000b6d0: 6967 7572 6174 696f 6e2c 0a20 2020 2020  iguration,.     
+0000b6e0: 2020 2020 2020 2062 6f64 793d 626f 6479         body=body
+0000b6f0: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
+0000b700: 656c 6473 3d66 6965 6c64 732c 0a20 2020  elds=fields,.   
+0000b710: 2020 2020 2020 2020 2061 7574 685f 7365           auth_se
+0000b720: 7474 696e 6773 3d61 7574 685f 7365 7474  ttings=auth_sett
+0000b730: 696e 6773 2c0a 2020 2020 2020 2020 2020  ings,.          
+0000b740: 2020 6865 6164 6572 733d 7573 6564 5f68    headers=used_h
+0000b750: 6561 6465 7273 2c0a 2020 2020 2020 2020  eaders,.        
+0000b760: 290a 0a20 2020 2020 2020 2023 2070 6572  )..        # per
+0000b770: 666f 726d 2072 6571 7565 7374 2061 6e64  form request and
+0000b780: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
+0000b790: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+0000b7a0: 6520 3d20 6177 6169 7420 7365 6c66 2e61  e = await self.a
+0000b7b0: 7379 6e63 5f72 6571 7565 7374 280a 2020  sync_request(.  
+0000b7c0: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
+0000b7d0: 2c0a 2020 2020 2020 2020 2020 2020 7572  ,.            ur
+0000b7e0: 6c2c 0a20 2020 2020 2020 2020 2020 2068  l,.            h
+0000b7f0: 6561 6465 7273 3d75 7365 645f 6865 6164  eaders=used_head
+0000b800: 6572 732c 0a20 2020 2020 2020 2020 2020  ers,.           
+0000b810: 2066 6965 6c64 733d 6669 656c 6473 2c0a   fields=fields,.
+0000b820: 2020 2020 2020 2020 2020 2020 626f 6479              body
+0000b830: 3d73 6572 6961 6c69 7a65 645f 626f 6479  =serialized_body
+0000b840: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
+0000b850: 7265 616d 3d73 7472 6561 6d2c 0a20 2020  ream=stream,.   
+0000b860: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
+0000b870: 3d74 696d 656f 7574 2c0a 2020 2020 2020  =timeout,.      
+0000b880: 2020 290a 0a0a 2020 2020 2020 2020 7265    )...        re
+0000b890: 7475 726e 2072 6573 706f 6e73 650a 0a20  turn response.. 
+0000b8a0: 2020 2064 6566 205f 5f63 616c 6c5f 6170     def __call_ap
+0000b8b0: 6928 0a20 2020 2020 2020 2073 656c 662c  i(.        self,
+0000b8c0: 0a20 2020 2020 2020 2072 6573 6f75 7263  .        resourc
+0000b8d0: 655f 7061 7468 3a20 7374 722c 0a20 2020  e_path: str,.   
+0000b8e0: 2020 2020 206d 6574 686f 643a 2073 7472       method: str
+0000b8f0: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+0000b900: 733a 2074 7970 696e 672e 4f70 7469 6f6e  s: typing.Option
+0000b910: 616c 5b48 5454 5048 6561 6465 7244 6963  al[HTTPHeaderDic
+0000b920: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+0000b930: 2020 2073 6572 6961 6c69 7a65 645f 626f     serialized_bo
+0000b940: 6479 3a20 7479 7069 6e67 2e4f 7074 696f  dy: typing.Optio
+0000b950: 6e61 6c5b 7479 7069 6e67 2e55 6e69 6f6e  nal[typing.Union
+0000b960: 5b73 7472 2c20 6279 7465 735d 5d20 3d20  [str, bytes]] = 
+0000b970: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
+0000b980: 6479 3a20 7479 7069 6e67 2e41 6e79 203d  dy: typing.Any =
+0000b990: 204e 6f6e 652c 0a20 2020 2020 2020 2066   None,.        f
+0000b9a0: 6965 6c64 733a 2074 7970 696e 672e 4f70  ields: typing.Op
+0000b9b0: 7469 6f6e 616c 5b74 7970 696e 672e 5475  tional[typing.Tu
+0000b9c0: 706c 655b 7479 7069 6e67 2e54 7570 6c65  ple[typing.Tuple
+0000b9d0: 5b73 7472 2c20 7374 725d 2c20 2e2e 2e5d  [str, str], ...]
+0000b9e0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000b9f0: 2020 6175 7468 5f73 6574 7469 6e67 733a    auth_settings:
+0000ba00: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0000ba10: 5b74 7970 696e 672e 4c69 7374 5b73 7472  [typing.List[str
+0000ba20: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+0000ba30: 2020 2073 7472 6561 6d3a 2062 6f6f 6c20     stream: bool 
+0000ba40: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
+0000ba50: 2074 696d 656f 7574 3a20 7479 7069 6e67   timeout: typing
+0000ba60: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+0000ba70: 2e55 6e69 6f6e 5b69 6e74 2c20 7479 7069  .Union[int, typi
+0000ba80: 6e67 2e54 7570 6c65 5d5d 203d 204e 6f6e  ng.Tuple]] = Non
+0000ba90: 652c 0a20 2020 2020 2020 2068 6f73 743a  e,.        host:
+0000baa0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0000bab0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0000bac0: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
+0000bad0: 6172 6174 6f72 5f69 7465 7261 746f 723a  arator_iterator:
+0000bae0: 2050 7265 6669 7853 6570 6172 6174 6f72   PrefixSeparator
+0000baf0: 4974 6572 6174 6f72 203d 204e 6f6e 652c  Iterator = None,
+0000bb00: 0a20 2020 2020 2020 205f 7265 7472 795f  .        _retry_
+0000bb10: 6f61 7574 6820 3d20 5472 7565 2c0a 2020  oauth = True,.  
+0000bb20: 2020 2920 2d3e 2052 6573 706f 6e73 6557    ) -> ResponseW
+0000bb30: 7261 7070 6572 3a0a 0a20 2020 2020 2020  rapper:..       
+0000bb40: 2072 6571 7565 7374 5f62 6566 6f72 655f   request_before_
+0000bb50: 686f 6f6b 280a 2020 2020 2020 2020 2020  hook(.          
+0000bb60: 2020 7265 736f 7572 6365 5f70 6174 683d    resource_path=
+0000bb70: 7265 736f 7572 6365 5f70 6174 682c 0a20  resource_path,. 
+0000bb80: 2020 2020 2020 2020 2020 206d 6574 686f             metho
+0000bb90: 643d 6d65 7468 6f64 2c0a 2020 2020 2020  d=method,.      
+0000bba0: 2020 2020 2020 636f 6e66 6967 7572 6174        configurat
+0000bbb0: 696f 6e3d 7365 6c66 2e63 6f6e 6669 6775  ion=self.configu
+0000bbc0: 7261 7469 6f6e 2c0a 2020 2020 2020 2020  ration,.        
+0000bbd0: 2020 2020 626f 6479 3d62 6f64 792c 0a20      body=body,. 
+0000bbe0: 2020 2020 2020 2020 2020 2066 6965 6c64             field
+0000bbf0: 733d 6669 656c 6473 2c0a 2020 2020 2020  s=fields,.      
+0000bc00: 2020 2020 2020 6175 7468 5f73 6574 7469        auth_setti
+0000bc10: 6e67 733d 6175 7468 5f73 6574 7469 6e67  ngs=auth_setting
+0000bc20: 732c 0a20 2020 2020 2020 2020 2020 2068  s,.            h
+0000bc30: 6561 6465 7273 3d68 6561 6465 7273 2c0a  eaders=headers,.
+0000bc40: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000bc50: 2020 2023 2068 6561 6465 7220 7061 7261     # header para
+0000bc60: 6d65 7465 7273 0a20 2020 2020 2020 2075  meters.        u
+0000bc70: 7365 645f 6865 6164 6572 7320 3d20 4854  sed_headers = HT
+0000bc80: 5450 4865 6164 6572 4469 6374 2873 656c  TPHeaderDict(sel
+0000bc90: 662e 6465 6661 756c 745f 6865 6164 6572  f.default_header
+0000bca0: 7329 0a20 2020 2020 2020 2069 6620 7365  s).        if se
+0000bcb0: 6c66 2e63 6f6f 6b69 653a 0a20 2020 2020  lf.cookie:.     
+0000bcc0: 2020 2020 2020 2068 6561 6465 7273 5b27         headers['
+0000bcd0: 436f 6f6b 6965 275d 203d 2073 656c 662e  Cookie'] = self.
+0000bce0: 636f 6f6b 6965 0a0a 2020 2020 2020 2020  cookie..        
+0000bcf0: 2320 6175 7468 2073 6574 7469 6e67 0a20  # auth setting. 
+0000bd00: 2020 2020 2020 2072 6573 6f75 7263 655f         resource_
+0000bd10: 7061 7468 203d 2073 656c 662e 7570 6461  path = self.upda
+0000bd20: 7465 5f70 6172 616d 735f 666f 725f 6175  te_params_for_au
+0000bd30: 7468 280a 2020 2020 2020 2020 2020 2020  th(.            
+0000bd40: 7573 6564 5f68 6561 6465 7273 2c0a 2020  used_headers,.  
+0000bd50: 2020 2020 2020 2020 2020 6175 7468 5f73            auth_s
+0000bd60: 6574 7469 6e67 732c 0a20 2020 2020 2020  ettings,.       
+0000bd70: 2020 2020 2072 6573 6f75 7263 655f 7061       resource_pa
+0000bd80: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+0000bd90: 6d65 7468 6f64 2c0a 2020 2020 2020 2020  method,.        
+0000bda0: 2020 2020 626f 6479 2c0a 2020 2020 2020      body,.      
+0000bdb0: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
+0000bdc0: 6172 6174 6f72 5f69 7465 7261 746f 720a  arator_iterator.
+0000bdd0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000bde0: 2020 2023 206d 7573 7420 6861 7070 656e     # must happen
+0000bdf0: 2061 6674 6572 2063 6f6f 6b69 6520 7365   after cookie se
+0000be00: 7474 696e 6720 616e 6420 6175 7468 2073  tting and auth s
+0000be10: 6574 7469 6e67 2069 6e20 6361 7365 2075  etting in case u
+0000be20: 7365 7220 6973 206f 7665 7272 6964 696e  ser is overridin
+0000be30: 6720 7468 6f73 650a 2020 2020 2020 2020  g those.        
+0000be40: 6966 2068 6561 6465 7273 3a0a 2020 2020  if headers:.    
+0000be50: 2020 2020 2020 2020 7573 6564 5f68 6561          used_hea
+0000be60: 6465 7273 2e75 7064 6174 6528 6865 6164  ders.update(head
+0000be70: 6572 7329 0a0a 2020 2020 2020 2020 2320  ers)..        # 
+0000be80: 7265 7175 6573 7420 7572 6c0a 2020 2020  request url.    
+0000be90: 2020 2020 6966 2068 6f73 7420 6973 204e      if host is N
+0000bea0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000beb0: 2075 726c 203d 2073 656c 662e 636f 6e66   url = self.conf
+0000bec0: 6967 7572 6174 696f 6e2e 686f 7374 202b  iguration.host +
+0000bed0: 2072 6573 6f75 7263 655f 7061 7468 0a20   resource_path. 
+0000bee0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000bef0: 2020 2020 2020 2020 2023 2075 7365 2073           # use s
+0000bf00: 6572 7665 722f 686f 7374 2064 6566 696e  erver/host defin
+0000bf10: 6564 2069 6e20 7061 7468 206f 7220 6f70  ed in path or op
+0000bf20: 6572 6174 696f 6e20 696e 7374 6561 640a  eration instead.
+0000bf30: 2020 2020 2020 2020 2020 2020 7572 6c20              url 
+0000bf40: 3d20 686f 7374 202b 2072 6573 6f75 7263  = host + resourc
+0000bf50: 655f 7061 7468 0a0a 2020 2020 2020 2020  e_path..        
+0000bf60: 7265 7175 6573 745f 6166 7465 725f 686f  request_after_ho
+0000bf70: 6f6b 280a 2020 2020 2020 2020 2020 2020  ok(.            
+0000bf80: 7265 736f 7572 6365 5f70 6174 683d 7265  resource_path=re
+0000bf90: 736f 7572 6365 5f70 6174 682c 0a20 2020  source_path,.   
+0000bfa0: 2020 2020 2020 2020 206d 6574 686f 643d           method=
+0000bfb0: 6d65 7468 6f64 2c0a 2020 2020 2020 2020  method,.        
+0000bfc0: 2020 2020 636f 6e66 6967 7572 6174 696f      configuratio
+0000bfd0: 6e3d 7365 6c66 2e63 6f6e 6669 6775 7261  n=self.configura
+0000bfe0: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+0000bff0: 2020 626f 6479 3d62 6f64 792c 0a20 2020    body=body,.   
+0000c000: 2020 2020 2020 2020 2066 6965 6c64 733d           fields=
+0000c010: 6669 656c 6473 2c0a 2020 2020 2020 2020  fields,.        
+0000c020: 2020 2020 6175 7468 5f73 6574 7469 6e67      auth_setting
+0000c030: 733d 6175 7468 5f73 6574 7469 6e67 732c  s=auth_settings,
+0000c040: 0a20 2020 2020 2020 2020 2020 2068 6561  .            hea
+0000c050: 6465 7273 3d75 7365 645f 6865 6164 6572  ders=used_header
+0000c060: 732c 0a20 2020 2020 2020 2029 0a0a 2020  s,.        )..  
+0000c070: 2020 2020 2020 2320 7065 7266 6f72 6d20        # perform 
+0000c080: 7265 7175 6573 7420 616e 6420 7265 7475  request and retu
+0000c090: 726e 2072 6573 706f 6e73 650a 2020 2020  rn response.    
+0000c0a0: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
+0000c0b0: 656c 662e 7265 7175 6573 7428 0a20 2020  elf.request(.   
+0000c0c0: 2020 2020 2020 2020 206d 6574 686f 642c           method,
+0000c0d0: 0a20 2020 2020 2020 2020 2020 2075 726c  .            url
+0000c0e0: 2c0a 2020 2020 2020 2020 2020 2020 6865  ,.            he
+0000c0f0: 6164 6572 733d 7573 6564 5f68 6561 6465  aders=used_heade
+0000c100: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
+0000c110: 6669 656c 6473 3d66 6965 6c64 732c 0a20  fields=fields,. 
+0000c120: 2020 2020 2020 2020 2020 2062 6f64 793d             body=
+0000c130: 7365 7269 616c 697a 6564 5f62 6f64 792c  serialized_body,
+0000c140: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+0000c150: 6561 6d3d 7374 7265 616d 2c0a 2020 2020  eam=stream,.    
+0000c160: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
+0000c170: 7469 6d65 6f75 742c 0a20 2020 2020 2020  timeout,.       
+0000c180: 2029 0a0a 2020 2020 2020 2020 2320 4c69   )..        # Li
+0000c190: 6b65 6c79 2074 6861 7420 7374 6174 7573  kely that status
+0000c1a0: 2063 6f64 6573 2034 3031 206f 7220 3430   codes 401 or 40
+0000c1b0: 3320 696e 6469 6361 7465 2074 6865 206e  3 indicate the n
+0000c1c0: 6565 6420 746f 2072 6566 7265 7368 2061  eed to refresh a
+0000c1d0: 6363 6573 7320 746f 6b65 6e20 666f 7220  ccess token for 
+0000c1e0: 4f41 7574 680a 2020 2020 2020 2020 6966  OAuth.        if
+0000c1f0: 2072 6573 706f 6e73 652e 6874 7470 5f72   response.http_r
+0000c200: 6573 706f 6e73 652e 7374 6174 7573 203d  esponse.status =
+0000c210: 3d20 3430 3120 6f72 2072 6573 706f 6e73  = 401 or respons
+0000c220: 652e 6874 7470 5f72 6573 706f 6e73 652e  e.http_response.
+0000c230: 7374 6174 7573 203d 3d20 3430 333a 0a20  status == 403:. 
+0000c240: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000c250: 6c66 2e63 6f6e 6669 6775 7261 7469 6f6e  lf.configuration
+0000c260: 2e6f 6175 7468 2069 7320 6e6f 7420 4e6f  .oauth is not No
+0000c270: 6e65 2061 6e64 205f 7265 7472 795f 6f61  ne and _retry_oa
+0000c280: 7574 683a 0a20 2020 2020 2020 2020 2020  uth:.           
+0000c290: 2020 2020 2073 656c 662e 636f 6e66 6967       self.config
+0000c2a0: 7572 6174 696f 6e2e 6f61 7574 682e 7265  uration.oauth.re
+0000c2b0: 6672 6573 685f 6163 6365 7373 5f74 6f6b  fresh_access_tok
+0000c2c0: 656e 2829 0a20 2020 2020 2020 2020 2020  en().           
+0000c2d0: 2020 2020 2073 656c 662e 5f5f 6361 6c6c       self.__call
+0000c2e0: 5f61 7069 280a 2020 2020 2020 2020 2020  _api(.          
+0000c2f0: 2020 2020 2020 2020 2020 7265 736f 7572            resour
+0000c300: 6365 5f70 6174 683d 7265 736f 7572 6365  ce_path=resource
+0000c310: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
+0000c320: 2020 2020 2020 2020 2020 206d 6574 686f             metho
+0000c330: 643d 6d65 7468 6f64 2c0a 2020 2020 2020  d=method,.      
+0000c340: 2020 2020 2020 2020 2020 2020 2020 6865                he
+0000c350: 6164 6572 733d 6865 6164 6572 732c 0a20  aders=headers,. 
 0000c360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c370: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-0000c380: 656f 7574 3d74 696d 656f 7574 2c0a 2020  eout=timeout,.  
-0000c390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3b0: 2020 2020 2020 2062 6f64 793d 626f 6479         body=body
-0000c3c0: 290a 2020 2020 2020 2020 656c 6966 206d  ).        elif m
-0000c3d0: 6574 686f 6420 3d3d 2022 5055 5422 3a0a  ethod == "PUT":.
-0000c3e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c3f0: 726e 2073 656c 662e 7265 7374 5f63 6c69  rn self.rest_cli
-0000c400: 656e 742e 5055 5428 7572 6c2c 0a20 2020  ent.PUT(url,.   
-0000c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c430: 2020 2020 2068 6561 6465 7273 3d68 6561       headers=hea
-0000c440: 6465 7273 2c0a 2020 2020 2020 2020 2020  ders,.          
+0000c370: 2020 2073 6572 6961 6c69 7a65 645f 626f     serialized_bo
+0000c380: 6479 3d73 6572 6961 6c69 7a65 645f 626f  dy=serialized_bo
+0000c390: 6479 2c0a 2020 2020 2020 2020 2020 2020  dy,.            
+0000c3a0: 2020 2020 2020 2020 626f 6479 3d62 6f64          body=bod
+0000c3b0: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
+0000c3c0: 2020 2020 2020 2066 6965 6c64 733d 6669         fields=fi
+0000c3d0: 656c 6473 2c0a 2020 2020 2020 2020 2020  elds,.          
+0000c3e0: 2020 2020 2020 2020 2020 6175 7468 5f73            auth_s
+0000c3f0: 6574 7469 6e67 733d 6175 7468 5f73 6574  ettings=auth_set
+0000c400: 7469 6e67 732c 0a20 2020 2020 2020 2020  tings,.         
+0000c410: 2020 2020 2020 2020 2020 2073 7472 6561             strea
+0000c420: 6d3d 7374 7265 616d 2c0a 2020 2020 2020  m=stream,.      
+0000c430: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+0000c440: 6d65 6f75 743d 7469 6d65 6f75 742c 0a20  meout=timeout,. 
 0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c460: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-0000c470: 656c 6473 3d66 6965 6c64 732c 0a20 2020  elds=fields,.   
-0000c480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4a0: 2020 2020 2073 7472 6561 6d3d 7374 7265       stream=stre
-0000c4b0: 616d 2c0a 2020 2020 2020 2020 2020 2020  am,.            
-0000c4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4d0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-0000c4e0: 6f75 743d 7469 6d65 6f75 742c 0a20 2020  out=timeout,.   
-0000c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c510: 2020 2020 2062 6f64 793d 626f 6479 290a       body=body).
-0000c520: 2020 2020 2020 2020 656c 6966 206d 6574          elif met
-0000c530: 686f 6420 3d3d 2022 5041 5443 4822 3a0a  hod == "PATCH":.
-0000c540: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c550: 726e 2073 656c 662e 7265 7374 5f63 6c69  rn self.rest_cli
-0000c560: 656e 742e 5041 5443 4828 7572 6c2c 0a20  ent.PATCH(url,. 
-0000c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c590: 2020 2020 2020 2020 2068 6561 6465 7273           headers
-0000c5a0: 3d68 6561 6465 7273 2c0a 2020 2020 2020  =headers,.      
-0000c5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5d0: 2020 2020 6669 656c 6473 3d66 6965 6c64      fields=field
-0000c5e0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000c5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c600: 2020 2020 2020 2020 2020 2020 2073 7472               str
-0000c610: 6561 6d3d 7374 7265 616d 2c0a 2020 2020  eam=stream,.    
-0000c620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c640: 2020 2020 2020 7469 6d65 6f75 743d 7469        timeout=ti
-0000c650: 6d65 6f75 742c 0a20 2020 2020 2020 2020  meout,.         
-0000c660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c680: 2062 6f64 793d 626f 6479 290a 2020 2020   body=body).    
-0000c690: 2020 2020 656c 6966 206d 6574 686f 6420      elif method 
-0000c6a0: 3d3d 2022 4445 4c45 5445 223a 0a20 2020  == "DELETE":.   
-0000c6b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000c6c0: 7365 6c66 2e72 6573 745f 636c 6965 6e74  self.rest_client
-0000c6d0: 2e44 454c 4554 4528 7572 6c2c 0a20 2020  .DELETE(url,.   
-0000c6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c700: 2020 2020 2020 2020 6865 6164 6572 733d          headers=
-0000c710: 6865 6164 6572 732c 0a20 2020 2020 2020  headers,.       
-0000c720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c740: 2020 2020 7374 7265 616d 3d73 7472 6561      stream=strea
-0000c750: 6d2c 0a20 2020 2020 2020 2020 2020 2020  m,.             
-0000c760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c770: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-0000c780: 6d65 6f75 743d 7469 6d65 6f75 742c 0a20  meout=timeout,. 
-0000c790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7b0: 2020 2020 2020 2020 2020 626f 6479 3d62            body=b
-0000c7c0: 6f64 7929 0a20 2020 2020 2020 2065 6c73  ody).        els
-0000c7d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000c7e0: 6169 7365 2041 7069 5661 6c75 6545 7272  aise ApiValueErr
-0000c7f0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-0000c800: 2020 2020 2268 7474 7020 6d65 7468 6f64      "http method
-0000c810: 206d 7573 7420 6265 2060 4745 5460 2c20   must be `GET`, 
-0000c820: 6048 4541 4460 2c20 604f 5054 494f 4e53  `HEAD`, `OPTIONS
-0000c830: 602c 220a 2020 2020 2020 2020 2020 2020  `,".            
-0000c840: 2020 2020 2220 6050 4f53 5460 2c20 6050      " `POST`, `P
-0000c850: 4154 4348 602c 2060 5055 5460 206f 7220  ATCH`, `PUT` or 
-0000c860: 6044 454c 4554 4560 2e22 0a20 2020 2020  `DELETE`.".     
-0000c870: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-0000c880: 6620 7570 6461 7465 5f70 6172 616d 735f  f update_params_
-0000c890: 666f 725f 6175 7468 280a 2020 2020 2020  for_auth(.      
-0000c8a0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000c8b0: 2020 2020 2020 2020 6865 6164 6572 732c          headers,
-0000c8c0: 0a20 2020 2020 2020 2020 2020 2061 7574  .            aut
-0000c8d0: 685f 7365 7474 696e 6773 2c0a 2020 2020  h_settings,.    
-0000c8e0: 2020 2020 2020 2020 7265 736f 7572 6365          resource
-0000c8f0: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
-0000c900: 2020 206d 6574 686f 642c 0a20 2020 2020     method,.     
-0000c910: 2020 2020 2020 2062 6f64 792c 0a20 2020         body,.   
-0000c920: 2020 2020 2020 2020 2070 7265 6669 785f           prefix_
-0000c930: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
-0000c940: 6f72 3a20 5072 6566 6978 5365 7061 7261  or: PrefixSepara
-0000c950: 746f 7249 7465 7261 746f 7220 3d20 4e6f  torIterator = No
-0000c960: 6e65 0a20 2020 2020 2020 2029 202d 3e20  ne.        ) -> 
-0000c970: 7374 723a 0a20 2020 2020 2020 2022 2222  str:.        """
-0000c980: 5570 6461 7465 7320 6865 6164 6572 2061  Updates header a
-0000c990: 6e64 2071 7565 7279 2070 6172 616d 7320  nd query params 
-0000c9a0: 6261 7365 6420 6f6e 2061 7574 6865 6e74  based on authent
-0000c9b0: 6963 6174 696f 6e20 7365 7474 696e 672e  ication setting.
-0000c9c0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0000c9d0: 2068 6561 6465 7273 3a20 4865 6164 6572   headers: Header
-0000c9e0: 2070 6172 616d 6574 6572 7320 6469 6374   parameters dict
-0000c9f0: 2074 6f20 6265 2075 7064 6174 6564 2e0a   to be updated..
-0000ca00: 2020 2020 2020 2020 3a70 6172 616d 2061          :param a
-0000ca10: 7574 685f 7365 7474 696e 6773 3a20 4175  uth_settings: Au
-0000ca20: 7468 656e 7469 6361 7469 6f6e 2073 6574  thentication set
-0000ca30: 7469 6e67 2069 6465 6e74 6966 6965 7273  ting identifiers
-0000ca40: 206c 6973 742e 0a20 2020 2020 2020 203a   list..        :
-0000ca50: 7061 7261 6d20 7265 736f 7572 6365 5f70  param resource_p
-0000ca60: 6174 683a 2041 2073 7472 696e 6720 7265  ath: A string re
-0000ca70: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
-0000ca80: 7468 6520 4854 5450 2072 6571 7565 7374  the HTTP request
-0000ca90: 2072 6573 6f75 7263 6520 7061 7468 2e0a   resource path..
-0000caa0: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
-0000cab0: 6574 686f 643a 2041 2073 7472 696e 6720  ethod: A string 
-0000cac0: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
-0000cad0: 6620 7468 6520 4854 5450 2072 6571 7565  f the HTTP reque
-0000cae0: 7374 206d 6574 686f 642e 0a20 2020 2020  st method..     
-0000caf0: 2020 203a 7061 7261 6d20 626f 6479 3a20     :param body: 
-0000cb00: 4120 6f62 6a65 6374 2072 6570 7265 7365  A object represe
-0000cb10: 6e74 696e 6720 7468 6520 626f 6479 206f  nting the body o
-0000cb20: 6620 7468 6520 4854 5450 2072 6571 7565  f the HTTP reque
-0000cb30: 7374 2e0a 2020 2020 2020 2020 2020 2020  st..            
-0000cb40: 5468 6520 6f62 6a65 6374 2074 7970 6520  The object type 
-0000cb50: 6973 2074 6865 2072 6574 7572 6e20 7661  is the return va
-0000cb60: 6c75 6520 6f66 205f 656e 636f 6465 722e  lue of _encoder.
-0000cb70: 6465 6661 756c 7428 292e 0a20 2020 2020  default()..     
-0000cb80: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-0000cb90: 6620 6e6f 7420 6175 7468 5f73 6574 7469  f not auth_setti
-0000cba0: 6e67 733a 0a20 2020 2020 2020 2020 2020  ngs:.           
-0000cbb0: 2072 6574 7572 6e20 7265 736f 7572 6365   return resource
-0000cbc0: 5f70 6174 680a 2020 2020 2020 2020 6966  _path.        if
-0000cbd0: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
-0000cbe0: 725f 6974 6572 6174 6f72 2069 7320 4e6f  r_iterator is No
-0000cbf0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000cc00: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
-0000cc10: 5f69 7465 7261 746f 7220 3d20 5072 6566  _iterator = Pref
-0000cc20: 6978 5365 7061 7261 746f 7249 7465 7261  ixSeparatorItera
-0000cc30: 746f 7228 223f 222c 2022 2622 290a 0a20  tor("?", "&").. 
-0000cc40: 2020 2020 2020 2066 6f72 2061 7574 6820         for auth 
-0000cc50: 696e 2061 7574 685f 7365 7474 696e 6773  in auth_settings
-0000cc60: 3a0a 2020 2020 2020 2020 2020 2020 6175  :.            au
-0000cc70: 7468 5f73 6574 7469 6e67 203d 2073 656c  th_setting = sel
-0000cc80: 662e 636f 6e66 6967 7572 6174 696f 6e2e  f.configuration.
-0000cc90: 6175 7468 5f73 6574 7469 6e67 7328 292e  auth_settings().
-0000cca0: 6765 7428 6175 7468 290a 2020 2020 2020  get(auth).      
-0000ccb0: 2020 2020 2020 6966 206e 6f74 2061 7574        if not aut
-0000ccc0: 685f 7365 7474 696e 673a 0a20 2020 2020  h_setting:.     
-0000ccd0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-0000cce0: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
-0000ccf0: 6966 2061 7574 685f 7365 7474 696e 675b  if auth_setting[
-0000cd00: 2769 6e27 5d20 3d3d 2027 636f 6f6b 6965  'in'] == 'cookie
-0000cd10: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-0000cd20: 2020 2068 6561 6465 7273 2e61 6464 2827     headers.add('
-0000cd30: 436f 6f6b 6965 272c 2061 7574 685f 7365  Cookie', auth_se
-0000cd40: 7474 696e 675b 2776 616c 7565 275d 290a  tting['value']).
-0000cd50: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0000cd60: 2061 7574 685f 7365 7474 696e 675b 2769   auth_setting['i
-0000cd70: 6e27 5d20 3d3d 2027 6865 6164 6572 273a  n'] == 'header':
-0000cd80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cd90: 2069 6620 6175 7468 5f73 6574 7469 6e67   if auth_setting
-0000cda0: 5b27 7479 7065 275d 2021 3d20 2768 7474  ['type'] != 'htt
-0000cdb0: 702d 7369 676e 6174 7572 6527 3a0a 2020  p-signature':.  
-0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdd0: 2020 6865 6164 6572 732e 6164 6428 6175    headers.add(au
-0000cde0: 7468 5f73 6574 7469 6e67 5b27 6b65 7927  th_setting['key'
-0000cdf0: 5d2c 2061 7574 685f 7365 7474 696e 675b  ], auth_setting[
-0000ce00: 2776 616c 7565 275d 290a 2020 2020 2020  'value']).      
-0000ce10: 2020 2020 2020 656c 6966 2061 7574 685f        elif auth_
-0000ce20: 7365 7474 696e 675b 2769 6e27 5d20 3d3d  setting['in'] ==
-0000ce30: 2027 7175 6572 7927 3a0a 2020 2020 2020   'query':.      
-0000ce40: 2020 2020 2020 2020 2020 2222 2220 544f            """ TO
-0000ce50: 444f 2069 6d70 6c65 6d65 6e74 2061 7574  DO implement aut
-0000ce60: 6820 696e 2071 7565 7279 0a20 2020 2020  h in query.     
-0000ce70: 2020 2020 2020 2020 2020 206e 6565 6420             need 
-0000ce80: 746f 2070 6173 7320 696e 2070 7265 6669  to pass in prefi
-0000ce90: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-0000cea0: 6174 6f72 0a20 2020 2020 2020 2020 2020  ator.           
-0000ceb0: 2020 2020 2061 6e64 206e 6565 6420 746f       and need to
-0000cec0: 206f 7574 7075 7420 7265 736f 7572 6365   output resource
-0000ced0: 5f70 6174 6820 7769 7468 2071 7565 7279  _path with query
-0000cee0: 2070 6172 616d 7320 6164 6465 640a 2020   params added.  
-0000cef0: 2020 2020 2020 2020 2020 2020 2020 2222                ""
-0000cf00: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000cf10: 2020 7265 736f 7572 6365 5f70 6174 6820    resource_path 
-0000cf20: 2b3d 2050 6172 616d 6574 6572 5365 7269  += ParameterSeri
-0000cf30: 616c 697a 6572 4261 7365 2e5f 7265 6636  alizerBase._ref6
-0000cf40: 3537 305f 6578 7061 6e73 696f 6e28 0a20  570_expansion(. 
-0000cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf60: 2020 2076 6172 6961 626c 655f 6e61 6d65     variable_name
-0000cf70: 3d61 7574 685f 7365 7474 696e 675b 276b  =auth_setting['k
-0000cf80: 6579 275d 2c0a 2020 2020 2020 2020 2020  ey'],.          
-0000cf90: 2020 2020 2020 2020 2020 696e 5f64 6174            in_dat
-0000cfa0: 613d 6175 7468 5f73 6574 7469 6e67 5b27  a=auth_setting['
-0000cfb0: 7661 6c75 6527 5d2c 0a20 2020 2020 2020  value'],.       
-0000cfc0: 2020 2020 2020 2020 2020 2020 2065 7870               exp
-0000cfd0: 6c6f 6465 3d46 616c 7365 2c0a 2020 2020  lode=False,.    
-0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cff0: 7065 7263 656e 745f 656e 636f 6465 3d46  percent_encode=F
-0000d000: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-0000d010: 2020 2020 2020 2020 2020 7072 6566 6978            prefix
-0000d020: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-0000d030: 746f 723d 7072 6566 6978 5f73 6570 6172  tor=prefix_separ
-0000d040: 6174 6f72 5f69 7465 7261 746f 720a 2020  ator_iterator.  
-0000d050: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000d060: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000d070: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d080: 2020 7261 6973 6520 4170 6956 616c 7565    raise ApiValue
-0000d090: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-0000d0a0: 2020 2020 2020 2020 2020 2027 4175 7468             'Auth
-0000d0b0: 656e 7469 6361 7469 6f6e 2074 6f6b 656e  entication token
-0000d0c0: 206d 7573 7420 6265 2069 6e20 6071 7565   must be in `que
-0000d0d0: 7279 6020 6f72 2060 6865 6164 6572 6027  ry` or `header`'
-0000d0e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d0f0: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-0000d100: 6e20 7265 736f 7572 6365 5f70 6174 680a  n resource_path.
-0000d110: 0a0a 636c 6173 7320 4170 693a 0a20 2020  ..class Api:.   
-0000d120: 2022 2222 4e4f 5445 3a0a 2020 2020 5468   """NOTE:.    Th
-0000d130: 6973 2063 6c61 7373 2069 7320 6175 746f  is class is auto
-0000d140: 2067 656e 6572 6174 6564 2062 7920 4b6f   generated by Ko
-0000d150: 6e66 6967 2028 6874 7470 733a 2f2f 6b6f  nfig (https://ko
-0000d160: 6e66 6967 7468 6973 2e63 6f6d 290a 2020  nfigthis.com).  
-0000d170: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
-0000d180: 5f69 6e69 745f 5f28 7365 6c66 2c20 6170  _init__(self, ap
-0000d190: 695f 636c 6965 6e74 3a20 7479 7069 6e67  i_client: typing
-0000d1a0: 2e4f 7074 696f 6e61 6c5b 4170 6943 6c69  .Optional[ApiCli
-0000d1b0: 656e 745d 203d 204e 6f6e 6529 3a0a 2020  ent] = None):.  
-0000d1c0: 2020 2020 2020 6966 2061 7069 5f63 6c69        if api_cli
-0000d1d0: 656e 7420 6973 204e 6f6e 653a 0a20 2020  ent is None:.   
-0000d1e0: 2020 2020 2020 2020 2061 7069 5f63 6c69           api_cli
-0000d1f0: 656e 7420 3d20 4170 6943 6c69 656e 7428  ent = ApiClient(
-0000d200: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0000d210: 7069 5f63 6c69 656e 7420 3d20 6170 695f  pi_client = api_
-0000d220: 636c 6965 6e74 0a0a 2020 2020 4073 7461  client..    @sta
-0000d230: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
-0000d240: 6620 5f76 6572 6966 795f 7479 7065 645f  f _verify_typed_
-0000d250: 6469 6374 5f69 6e70 7574 735f 6f61 7067  dict_inputs_oapg
-0000d260: 2863 6c73 3a20 7479 7069 6e67 2e54 7970  (cls: typing.Typ
-0000d270: 655b 7479 7069 6e67 5f65 7874 656e 7369  e[typing_extensi
-0000d280: 6f6e 732e 5479 7065 6444 6963 745d 2c20  ons.TypedDict], 
-0000d290: 6461 7461 3a20 7479 7069 6e67 2e44 6963  data: typing.Dic
-0000d2a0: 745b 7374 722c 2074 7970 696e 672e 416e  t[str, typing.An
-0000d2b0: 795d 293a 0a20 2020 2020 2020 2022 2222  y]):.        """
-0000d2c0: 0a20 2020 2020 2020 2045 6e73 7572 6573  .        Ensures
-0000d2d0: 2074 6861 743a 0a20 2020 2020 2020 202d   that:.        -
-0000d2e0: 2072 6571 7569 7265 6420 6b65 7973 2061   required keys a
-0000d2f0: 7265 2070 7265 7365 6e74 0a20 2020 2020  re present.     
-0000d300: 2020 202d 2061 6464 6974 696f 6e61 6c20     - additional 
-0000d310: 7072 6f70 6572 7469 6573 2061 7265 206e  properties are n
-0000d320: 6f74 2069 6e70 7574 0a20 2020 2020 2020  ot input.       
-0000d330: 202d 2076 616c 7565 2073 746f 7265 6420   - value stored 
-0000d340: 756e 6465 7220 7265 7175 6972 6564 206b  under required k
-0000d350: 6579 7320 646f 206e 6f74 2068 6176 6520  eys do not have 
-0000d360: 7468 6520 7661 6c75 6520 756e 7365 740a  the value unset.
-0000d370: 2020 2020 2020 2020 4e6f 7465 3a20 6465          Note: de
-0000d380: 7461 696c 6564 2076 616c 7565 2063 6865  tailed value che
-0000d390: 636b 696e 6720 6973 2064 6f6e 6520 696e  cking is done in
-0000d3a0: 2073 6368 656d 6120 636c 6173 7365 730a   schema classes.
-0000d3b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000d3c0: 2020 2020 6d69 7373 696e 675f 7265 7175      missing_requ
-0000d3d0: 6972 6564 5f6b 6579 7320 3d20 5b5d 0a20  ired_keys = []. 
-0000d3e0: 2020 2020 2020 2072 6571 7569 7265 645f         required_
-0000d3f0: 6b65 7973 5f77 6974 685f 756e 7365 745f  keys_with_unset_
-0000d400: 7661 6c75 6573 203d 205b 5d0a 2020 2020  values = [].    
-0000d410: 2020 2020 666f 7220 7265 7175 6972 6564      for required
-0000d420: 5f6b 6579 2069 6e20 636c 732e 5f5f 7265  _key in cls.__re
-0000d430: 7175 6972 6564 5f6b 6579 735f 5f3a 0a20  quired_keys__:. 
-0000d440: 2020 2020 2020 2020 2020 2069 6620 7265             if re
-0000d450: 7175 6972 6564 5f6b 6579 206e 6f74 2069  quired_key not i
-0000d460: 6e20 6461 7461 3a0a 2020 2020 2020 2020  n data:.        
-0000d470: 2020 2020 2020 2020 6d69 7373 696e 675f          missing_
-0000d480: 7265 7175 6972 6564 5f6b 6579 732e 6170  required_keys.ap
-0000d490: 7065 6e64 2872 6571 7569 7265 645f 6b65  pend(required_ke
-0000d4a0: 7929 0a20 2020 2020 2020 2020 2020 2020  y).             
-0000d4b0: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-0000d4c0: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-0000d4d0: 6461 7461 5b72 6571 7569 7265 645f 6b65  data[required_ke
-0000d4e0: 795d 0a20 2020 2020 2020 2020 2020 2069  y].            i
-0000d4f0: 6620 7661 6c75 6520 6973 2075 6e73 6574  f value is unset
-0000d500: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d510: 2020 7265 7175 6972 6564 5f6b 6579 735f    required_keys_
-0000d520: 7769 7468 5f75 6e73 6574 5f76 616c 7565  with_unset_value
-0000d530: 732e 6170 7065 6e64 2872 6571 7569 7265  s.append(require
-0000d540: 645f 6b65 7929 0a20 2020 2020 2020 2069  d_key).        i
-0000d550: 6620 6d69 7373 696e 675f 7265 7175 6972  f missing_requir
-0000d560: 6564 5f6b 6579 733a 0a20 2020 2020 2020  ed_keys:.       
-0000d570: 2020 2020 2072 6169 7365 2041 7069 5479       raise ApiTy
-0000d580: 7065 4572 726f 7228 0a20 2020 2020 2020  peError(.       
-0000d590: 2020 2020 2020 2020 2027 7b7d 206d 6973           '{} mis
-0000d5a0: 7369 6e67 207b 7d20 7265 7175 6972 6564  sing {} required
-0000d5b0: 2061 7267 756d 656e 7473 3a20 7b7d 272e   arguments: {}'.
-0000d5c0: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-0000d5d0: 2020 2020 2020 2020 2020 2020 636c 732e              cls.
-0000d5e0: 5f5f 6e61 6d65 5f5f 2c20 6c65 6e28 6d69  __name__, len(mi
-0000d5f0: 7373 696e 675f 7265 7175 6972 6564 5f6b  ssing_required_k
-0000d600: 6579 7329 2c20 6d69 7373 696e 675f 7265  eys), missing_re
-0000d610: 7175 6972 6564 5f6b 6579 730a 2020 2020  quired_keys.    
-0000d620: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000d630: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000d640: 2020 2020 2020 6966 2072 6571 7569 7265        if require
-0000d650: 645f 6b65 7973 5f77 6974 685f 756e 7365  d_keys_with_unse
-0000d660: 745f 7661 6c75 6573 3a0a 2020 2020 2020  t_values:.      
-0000d670: 2020 2020 2020 7261 6973 6520 4170 6956        raise ApiV
-0000d680: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
-0000d690: 2020 2020 2020 2020 2020 2027 7b7d 2063             '{} c
-0000d6a0: 6f6e 7461 696e 7320 696e 7661 6c69 6420  ontains invalid 
-0000d6b0: 756e 7365 7420 7661 6c75 6573 2066 6f72  unset values for
-0000d6c0: 207b 7d20 7265 7175 6972 6564 206b 6579   {} required key
-0000d6d0: 733a 207b 7d27 2e66 6f72 6d61 7428 0a20  s: {}'.format(. 
-0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6f0: 2020 2063 6c73 2e5f 5f6e 616d 655f 5f2c     cls.__name__,
-0000d700: 206c 656e 2872 6571 7569 7265 645f 6b65   len(required_ke
-0000d710: 7973 5f77 6974 685f 756e 7365 745f 7661  ys_with_unset_va
-0000d720: 6c75 6573 292c 2072 6571 7569 7265 645f  lues), required_
-0000d730: 6b65 7973 5f77 6974 685f 756e 7365 745f  keys_with_unset_
-0000d740: 7661 6c75 6573 0a20 2020 2020 2020 2020  values.         
-0000d750: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000d760: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000d770: 6469 7361 6c6c 6f77 6564 5f61 6464 6974  disallowed_addit
-0000d780: 696f 6e61 6c5f 6b65 7973 203d 205b 5d0a  ional_keys = [].
-0000d790: 2020 2020 2020 2020 666f 7220 6b65 7920          for key 
-0000d7a0: 696e 2064 6174 613a 0a20 2020 2020 2020  in data:.       
-0000d7b0: 2020 2020 2069 6620 6b65 7920 696e 2063       if key in c
-0000d7c0: 6c73 2e5f 5f72 6571 7569 7265 645f 6b65  ls.__required_ke
-0000d7d0: 7973 5f5f 206f 7220 6b65 7920 696e 2063  ys__ or key in c
-0000d7e0: 6c73 2e5f 5f6f 7074 696f 6e61 6c5f 6b65  ls.__optional_ke
-0000d7f0: 7973 5f5f 3a0a 2020 2020 2020 2020 2020  ys__:.          
-0000d800: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-0000d810: 2020 2020 2020 2020 2020 2064 6973 616c             disal
-0000d820: 6c6f 7765 645f 6164 6469 7469 6f6e 616c  lowed_additional
-0000d830: 5f6b 6579 732e 6170 7065 6e64 286b 6579  _keys.append(key
-0000d840: 290a 2020 2020 2020 2020 6966 2064 6973  ).        if dis
-0000d850: 616c 6c6f 7765 645f 6164 6469 7469 6f6e  allowed_addition
-0000d860: 616c 5f6b 6579 733a 0a20 2020 2020 2020  al_keys:.       
-0000d870: 2020 2020 2072 6169 7365 2041 7069 5479       raise ApiTy
-0000d880: 7065 4572 726f 7228 0a20 2020 2020 2020  peError(.       
-0000d890: 2020 2020 2020 2020 2027 7b7d 2067 6f74           '{} got
-0000d8a0: 207b 7d20 756e 6578 7065 6374 6564 206b   {} unexpected k
-0000d8b0: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
-0000d8c0: 3a20 7b7d 272e 666f 726d 6174 280a 2020  : {}'.format(.  
-0000d8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8e0: 2020 636c 732e 5f5f 6e61 6d65 5f5f 2c20    cls.__name__, 
-0000d8f0: 6c65 6e28 6469 7361 6c6c 6f77 6564 5f61  len(disallowed_a
-0000d900: 6464 6974 696f 6e61 6c5f 6b65 7973 292c  dditional_keys),
-0000d910: 2064 6973 616c 6c6f 7765 645f 6164 6469   disallowed_addi
-0000d920: 7469 6f6e 616c 5f6b 6579 730a 2020 2020  tional_keys.    
-0000d930: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000d940: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-0000d950: 2064 6566 205f 6765 745f 686f 7374 5f6f   def _get_host_o
-0000d960: 6170 6728 0a20 2020 2020 2020 2073 656c  apg(.        sel
-0000d970: 662c 0a20 2020 2020 2020 206f 7065 7261  f,.        opera
-0000d980: 7469 6f6e 5f69 643a 2073 7472 2c0a 2020  tion_id: str,.  
-0000d990: 2020 2020 2020 7365 7276 6572 733a 2074        servers: t
-0000d9a0: 7970 696e 672e 5475 706c 655b 7479 7069  yping.Tuple[typi
-0000d9b0: 6e67 2e44 6963 745b 7374 722c 2073 7472  ng.Dict[str, str
-0000d9c0: 5d2c 202e 2e2e 5d20 3d20 7475 706c 6528  ], ...] = tuple(
-0000d9d0: 292c 0a20 2020 2020 2020 2068 6f73 745f  ),.        host_
-0000d9e0: 696e 6465 783a 2074 7970 696e 672e 4f70  index: typing.Op
-0000d9f0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-0000da00: 6e65 0a20 2020 2029 202d 3e20 7479 7069  ne.    ) -> typi
-0000da10: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
-0000da20: 3a0a 2020 2020 2020 2020 636f 6e66 6967  :.        config
-0000da30: 7572 6174 696f 6e20 3d20 7365 6c66 2e61  uration = self.a
-0000da40: 7069 5f63 6c69 656e 742e 636f 6e66 6967  pi_client.config
-0000da50: 7572 6174 696f 6e0a 2020 2020 2020 2020  uration.        
-0000da60: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0000da70: 2069 6620 686f 7374 5f69 6e64 6578 2069   if host_index i
-0000da80: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000da90: 2020 2020 2020 2020 696e 6465 7820 3d20          index = 
-0000daa0: 636f 6e66 6967 7572 6174 696f 6e2e 7365  configuration.se
-0000dab0: 7276 6572 5f6f 7065 7261 7469 6f6e 5f69  rver_operation_i
-0000dac0: 6e64 6578 2e67 6574 280a 2020 2020 2020  ndex.get(.      
-0000dad0: 2020 2020 2020 2020 2020 2020 2020 6f70                op
-0000dae0: 6572 6174 696f 6e5f 6964 2c20 636f 6e66  eration_id, conf
-0000daf0: 6967 7572 6174 696f 6e2e 7365 7276 6572  iguration.server
-0000db00: 5f69 6e64 6578 0a20 2020 2020 2020 2020  _index.         
-0000db10: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000db20: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000db30: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-0000db40: 203d 2068 6f73 745f 696e 6465 780a 2020   = host_index.  
-0000db50: 2020 2020 2020 2020 2020 7365 7276 6572            server
-0000db60: 5f76 6172 6961 626c 6573 203d 2063 6f6e  _variables = con
-0000db70: 6669 6775 7261 7469 6f6e 2e73 6572 7665  figuration.serve
-0000db80: 725f 6f70 6572 6174 696f 6e5f 7661 7269  r_operation_vari
-0000db90: 6162 6c65 732e 6765 7428 0a20 2020 2020  ables.get(.     
-0000dba0: 2020 2020 2020 2020 2020 206f 7065 7261             opera
-0000dbb0: 7469 6f6e 5f69 642c 2063 6f6e 6669 6775  tion_id, configu
-0000dbc0: 7261 7469 6f6e 2e73 6572 7665 725f 7661  ration.server_va
-0000dbd0: 7269 6162 6c65 730a 2020 2020 2020 2020  riables.        
-0000dbe0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000dbf0: 2020 686f 7374 203d 2063 6f6e 6669 6775    host = configu
-0000dc00: 7261 7469 6f6e 2e67 6574 5f68 6f73 745f  ration.get_host_
-0000dc10: 6672 6f6d 5f73 6574 7469 6e67 7328 0a20  from_settings(. 
-0000dc20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000dc30: 6e64 6578 2c20 7661 7269 6162 6c65 733d  ndex, variables=
-0000dc40: 7365 7276 6572 5f76 6172 6961 626c 6573  server_variables
-0000dc50: 2c20 7365 7276 6572 733d 7365 7276 6572  , servers=server
-0000dc60: 730a 2020 2020 2020 2020 2020 2020 290a  s.            ).
-0000dc70: 2020 2020 2020 2020 6578 6365 7074 2049          except I
-0000dc80: 6e64 6578 4572 726f 723a 0a20 2020 2020  ndexError:.     
-0000dc90: 2020 2020 2020 2069 6620 7365 7276 6572         if server
-0000dca0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000dcb0: 2020 2072 6169 7365 2041 7069 5661 6c75     raise ApiValu
-0000dcc0: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-0000dcd0: 2020 2020 2020 2020 2020 2020 2249 6e76              "Inv
-0000dce0: 616c 6964 2068 6f73 7420 696e 6465 782e  alid host index.
-0000dcf0: 204d 7573 7420 6265 2030 203c 3d20 696e   Must be 0 <= in
-0000dd00: 6465 7820 3c20 2573 2220 250a 2020 2020  dex < %s" %.    
-0000dd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd20: 6c65 6e28 7365 7276 6572 7329 0a20 2020  len(servers).   
-0000dd30: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000dd40: 2020 2020 2020 2020 2020 2068 6f73 7420             host 
-0000dd50: 3d20 4e6f 6e65 0a20 2020 2020 2020 2072  = None.        r
-0000dd60: 6574 7572 6e20 686f 7374 0a0a 0a63 6c61  eturn host...cla
-0000dd70: 7373 2053 6572 6961 6c69 7a65 6452 6571  ss SerializedReq
-0000dd80: 7565 7374 426f 6479 2874 7970 696e 675f  uestBody(typing_
-0000dd90: 6578 7465 6e73 696f 6e73 2e54 7970 6564  extensions.Typed
-0000dda0: 4469 6374 2c20 746f 7461 6c3d 4661 6c73  Dict, total=Fals
-0000ddb0: 6529 3a0a 2020 2020 626f 6479 3a20 7479  e):.    body: ty
-0000ddc0: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
-0000ddd0: 6279 7465 735d 0a20 2020 2066 6965 6c64  bytes].    field
-0000dde0: 733a 2074 7970 696e 672e 5475 706c 655b  s: typing.Tuple[
-0000ddf0: 7479 7069 6e67 2e55 6e69 6f6e 5b52 6571  typing.Union[Req
-0000de00: 7565 7374 4669 656c 642c 2074 7970 696e  uestField, typin
-0000de10: 672e 5475 706c 655b 7374 722c 2073 7472  g.Tuple[str, str
-0000de20: 5d5d 2c20 2e2e 2e5d 0a0a 0a63 6c61 7373  ]], ...]...class
-0000de30: 2052 6571 7565 7374 426f 6479 2853 7479   RequestBody(Sty
-0000de40: 6c65 466f 726d 5365 7269 616c 697a 6572  leFormSerializer
-0000de50: 2c20 4a53 4f4e 4465 7465 6374 6f72 293a  , JSONDetector):
-0000de60: 0a20 2020 2022 2222 0a20 2020 2041 2072  .    """.    A r
-0000de70: 6571 7565 7374 2062 6f64 7920 7061 7261  equest body para
-0000de80: 6d65 7465 720a 2020 2020 636f 6e74 656e  meter.    conten
-0000de90: 743a 2063 6f6e 7465 6e74 5f74 7970 6520  t: content_type 
-0000dea0: 746f 204d 6564 6961 5479 7065 2053 6368  to MediaType Sch
-0000deb0: 656d 6120 696e 666f 0a20 2020 2022 2222  ema info.    """
-0000dec0: 0a20 2020 205f 5f6a 736f 6e5f 656e 636f  .    __json_enco
-0000ded0: 6465 7220 3d20 4a53 4f4e 456e 636f 6465  der = JSONEncode
-0000dee0: 7228 290a 0a20 2020 2064 6566 205f 5f69  r()..    def __i
-0000def0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-0000df00: 656c 662c 0a20 2020 2020 2020 2063 6f6e  elf,.        con
-0000df10: 7465 6e74 3a20 7479 7069 6e67 2e44 6963  tent: typing.Dic
-0000df20: 745b 7374 722c 204d 6564 6961 5479 7065  t[str, MediaType
-0000df30: 5d2c 0a20 2020 2020 2020 2072 6571 7569  ],.        requi
-0000df40: 7265 643a 2062 6f6f 6c20 3d20 4661 6c73  red: bool = Fals
-0000df50: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-0000df60: 2020 7365 6c66 2e72 6571 7569 7265 6420    self.required 
-0000df70: 3d20 7265 7175 6972 6564 0a20 2020 2020  = required.     
-0000df80: 2020 2069 6620 6c65 6e28 636f 6e74 656e     if len(conten
-0000df90: 7429 203d 3d20 303a 0a20 2020 2020 2020  t) == 0:.       
-0000dfa0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0000dfb0: 4572 726f 7228 2749 6e76 616c 6964 2076  Error('Invalid v
-0000dfc0: 616c 7565 2066 6f72 2063 6f6e 7465 6e74  alue for content
-0000dfd0: 2c20 7468 6520 636f 6e74 656e 7420 6469  , the content di
-0000dfe0: 6374 206d 7573 7420 6861 7665 203e 3d20  ct must have >= 
-0000dff0: 3120 656e 7472 7927 290a 2020 2020 2020  1 entry').      
-0000e000: 2020 7365 6c66 2e63 6f6e 7465 6e74 203d    self.content =
-0000e010: 2063 6f6e 7465 6e74 0a0a 2020 2020 6465   content..    de
-0000e020: 6620 5f5f 7365 7269 616c 697a 655f 6a73  f __serialize_js
-0000e030: 6f6e 280a 2020 2020 2020 2020 7365 6c66  on(.        self
-0000e040: 2c0a 2020 2020 2020 2020 696e 5f64 6174  ,.        in_dat
-0000e050: 613a 2074 7970 696e 672e 416e 790a 2020  a: typing.Any.  
-0000e060: 2020 2920 2d3e 2074 7970 696e 672e 4469    ) -> typing.Di
-0000e070: 6374 5b73 7472 2c20 6279 7465 735d 3a0a  ct[str, bytes]:.
-0000e080: 2020 2020 2020 2020 696e 5f64 6174 6120          in_data 
-0000e090: 3d20 7365 6c66 2e5f 5f6a 736f 6e5f 656e  = self.__json_en
-0000e0a0: 636f 6465 722e 6465 6661 756c 7428 696e  coder.default(in
-0000e0b0: 5f64 6174 6129 0a20 2020 2020 2020 206a  _data).        j
-0000e0c0: 736f 6e5f 7374 7220 3d20 6a73 6f6e 2e64  son_str = json.d
-0000e0d0: 756d 7073 2869 6e5f 6461 7461 2c20 7365  umps(in_data, se
-0000e0e0: 7061 7261 746f 7273 3d28 222c 222c 2022  parators=(",", "
-0000e0f0: 3a22 292c 2065 6e73 7572 655f 6173 6369  :"), ensure_asci
-0000e100: 693d 4661 6c73 6529 2e65 6e63 6f64 6528  i=False).encode(
-0000e110: 0a20 2020 2020 2020 2020 2020 2022 7574  .            "ut
-0000e120: 662d 3822 0a20 2020 2020 2020 2029 0a20  f-8".        ). 
-0000e130: 2020 2020 2020 2072 6574 7572 6e20 6469         return di
-0000e140: 6374 2862 6f64 793d 6a73 6f6e 5f73 7472  ct(body=json_str
-0000e150: 290a 0a20 2020 2040 7374 6174 6963 6d65  )..    @staticme
-0000e160: 7468 6f64 0a20 2020 2064 6566 205f 5f73  thod.    def __s
-0000e170: 6572 6961 6c69 7a65 5f74 6578 745f 706c  erialize_text_pl
-0000e180: 6169 6e28 696e 5f64 6174 613a 2074 7970  ain(in_data: typ
-0000e190: 696e 672e 416e 7929 202d 3e20 7479 7069  ing.Any) -> typi
-0000e1a0: 6e67 2e44 6963 745b 7374 722c 2073 7472  ng.Dict[str, str
-0000e1b0: 5d3a 0a20 2020 2020 2020 2069 6620 6973  ]:.        if is
-0000e1c0: 696e 7374 616e 6365 2869 6e5f 6461 7461  instance(in_data
-0000e1d0: 2c20 6672 6f7a 656e 6469 6374 2e66 726f  , frozendict.fro
-0000e1e0: 7a65 6e64 6963 7429 3a0a 2020 2020 2020  zendict):.      
-0000e1f0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0000e200: 6545 7272 6f72 2827 556e 6162 6c65 2074  eError('Unable t
-0000e210: 6f20 7365 7269 616c 697a 6520 7479 7065  o serialize type
-0000e220: 2066 726f 7a65 6e64 6963 742e 6672 6f7a   frozendict.froz
-0000e230: 656e 6469 6374 2074 6f20 7465 7874 2f70  endict to text/p
-0000e240: 6c61 696e 2729 0a20 2020 2020 2020 2065  lain').        e
-0000e250: 6c69 6620 6973 696e 7374 616e 6365 2869  lif isinstance(i
-0000e260: 6e5f 6461 7461 2c20 7475 706c 6529 3a0a  n_data, tuple):.
-0000e270: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000e280: 6520 5661 6c75 6545 7272 6f72 2827 556e  e ValueError('Un
-0000e290: 6162 6c65 2074 6f20 7365 7269 616c 697a  able to serializ
-0000e2a0: 6520 7479 7065 2074 7570 6c65 2074 6f20  e type tuple to 
-0000e2b0: 7465 7874 2f70 6c61 696e 2729 0a20 2020  text/plain').   
-0000e2c0: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-0000e2d0: 616e 6365 2869 6e5f 6461 7461 2c20 4e6f  ance(in_data, No
-0000e2e0: 6e65 436c 6173 7329 3a0a 2020 2020 2020  neClass):.      
-0000e2f0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0000e300: 6545 7272 6f72 2827 556e 6162 6c65 2074  eError('Unable t
-0000e310: 6f20 7365 7269 616c 697a 6520 7479 7065  o serialize type
-0000e320: 204e 6f6e 6543 6c61 7373 2074 6f20 7465   NoneClass to te
-0000e330: 7874 2f70 6c61 696e 2729 0a20 2020 2020  xt/plain').     
-0000e340: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-0000e350: 6365 2869 6e5f 6461 7461 2c20 426f 6f6c  ce(in_data, Bool
-0000e360: 436c 6173 7329 3a0a 2020 2020 2020 2020  Class):.        
-0000e370: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000e380: 7272 6f72 2827 556e 6162 6c65 2074 6f20  rror('Unable to 
-0000e390: 7365 7269 616c 697a 6520 7479 7065 2042  serialize type B
-0000e3a0: 6f6f 6c43 6c61 7373 2074 6f20 7465 7874  oolClass to text
-0000e3b0: 2f70 6c61 696e 2729 0a20 2020 2020 2020  /plain').       
-0000e3c0: 2072 6574 7572 6e20 6469 6374 2862 6f64   return dict(bod
-0000e3d0: 793d 7374 7228 696e 5f64 6174 6129 290a  y=str(in_data)).
-0000e3e0: 0a20 2020 2064 6566 205f 5f6d 756c 7469  .    def __multi
-0000e3f0: 7061 7274 5f6a 736f 6e5f 6974 656d 2873  part_json_item(s
-0000e400: 656c 662c 206b 6579 3a20 7374 722c 2076  elf, key: str, v
-0000e410: 616c 7565 3a20 5363 6865 6d61 2920 2d3e  alue: Schema) ->
-0000e420: 2052 6571 7565 7374 4669 656c 643a 0a20   RequestField:. 
-0000e430: 2020 2020 2020 206a 736f 6e5f 7661 6c75         json_valu
-0000e440: 6520 3d20 7365 6c66 2e5f 5f6a 736f 6e5f  e = self.__json_
-0000e450: 656e 636f 6465 722e 6465 6661 756c 7428  encoder.default(
-0000e460: 7661 6c75 6529 0a20 2020 2020 2020 2072  value).        r
-0000e470: 6574 7572 6e20 5265 7175 6573 7446 6965  eturn RequestFie
-0000e480: 6c64 286e 616d 653d 6b65 792c 2064 6174  ld(name=key, dat
-0000e490: 613d 6a73 6f6e 2e64 756d 7073 286a 736f  a=json.dumps(jso
-0000e4a0: 6e5f 7661 6c75 6529 2c20 6865 6164 6572  n_value), header
-0000e4b0: 733d 7b27 436f 6e74 656e 742d 5479 7065  s={'Content-Type
-0000e4c0: 273a 2027 6170 706c 6963 6174 696f 6e2f  ': 'application/
-0000e4d0: 6a73 6f6e 277d 290a 0a20 2020 2064 6566  json'})..    def
-0000e4e0: 205f 5f6d 756c 7469 7061 7274 5f66 6f72   __multipart_for
-0000e4f0: 6d5f 6974 656d 2873 656c 662c 206b 6579  m_item(self, key
-0000e500: 3a20 7374 722c 2076 616c 7565 3a20 5363  : str, value: Sc
-0000e510: 6865 6d61 2920 2d3e 2052 6571 7565 7374  hema) -> Request
-0000e520: 4669 656c 643a 0a20 2020 2020 2020 2069  Field:.        i
-0000e530: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
-0000e540: 7565 2c20 7374 7229 3a0a 2020 2020 2020  ue, str):.      
-0000e550: 2020 2020 2020 7265 7475 726e 2052 6571        return Req
-0000e560: 7565 7374 4669 656c 6428 6e61 6d65 3d6b  uestField(name=k
-0000e570: 6579 2c20 6461 7461 3d73 7472 2876 616c  ey, data=str(val
-0000e580: 7565 292c 2068 6561 6465 7273 3d7b 2743  ue), headers={'C
-0000e590: 6f6e 7465 6e74 2d54 7970 6527 3a20 2774  ontent-Type': 't
-0000e5a0: 6578 742f 706c 6169 6e27 7d29 0a20 2020  ext/plain'}).   
-0000e5b0: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-0000e5c0: 616e 6365 2876 616c 7565 2c20 6279 7465  ance(value, byte
-0000e5d0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0000e5e0: 7265 7475 726e 2052 6571 7565 7374 4669  return RequestFi
-0000e5f0: 656c 6428 6e61 6d65 3d6b 6579 2c20 6461  eld(name=key, da
-0000e600: 7461 3d76 616c 7565 2c20 6865 6164 6572  ta=value, header
-0000e610: 733d 7b27 436f 6e74 656e 742d 5479 7065  s={'Content-Type
-0000e620: 273a 2027 6170 706c 6963 6174 696f 6e2f  ': 'application/
-0000e630: 6f63 7465 742d 7374 7265 616d 277d 290a  octet-stream'}).
-0000e640: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-0000e650: 6e73 7461 6e63 6528 7661 6c75 652c 2046  nstance(value, F
-0000e660: 696c 6549 4f29 3a0a 2020 2020 2020 2020  ileIO):.        
-0000e670: 2020 2020 6669 6c65 6e61 6d65 203d 206f      filename = o
-0000e680: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
-0000e690: 7661 6c75 652e 6e61 6d65 290a 2020 2020  value.name).    
-0000e6a0: 2020 2020 2020 2020 7265 7175 6573 745f          request_
-0000e6b0: 6669 656c 6420 3d20 5265 7175 6573 7446  field = RequestF
-0000e6c0: 6965 6c64 280a 2020 2020 2020 2020 2020  ield(.          
-0000e6d0: 2020 2020 2020 6e61 6d65 3d6b 6579 2c0a        name=key,.
+0000c460: 2020 2068 6f73 743d 686f 7374 2c0a 2020     host=host,.  
+0000c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c480: 2020 7072 6566 6978 5f73 6570 6172 6174    prefix_separat
+0000c490: 6f72 5f69 7465 7261 746f 723d 7072 6566  or_iterator=pref
+0000c4a0: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+0000c4b0: 7261 746f 722c 0a20 2020 2020 2020 2020  rator,.         
+0000c4c0: 2020 2020 2020 2020 2020 205f 7265 7472             _retr
+0000c4d0: 795f 6f61 7574 683d 4661 6c73 652c 0a20  y_oauth=False,. 
+0000c4e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000c4f0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000c500: 2072 6573 706f 6e73 650a 0a20 2020 2061   response..    a
+0000c510: 7379 6e63 2064 6566 2061 7379 6e63 5f63  sync def async_c
+0000c520: 616c 6c5f 6170 6928 0a20 2020 2020 2020  all_api(.       
+0000c530: 2073 656c 662c 0a20 2020 2020 2020 2072   self,.        r
+0000c540: 6573 6f75 7263 655f 7061 7468 3a20 7374  esource_path: st
+0000c550: 722c 0a20 2020 2020 2020 206d 6574 686f  r,.        metho
+0000c560: 643a 2073 7472 2c0a 2020 2020 2020 2020  d: str,.        
+0000c570: 6865 6164 6572 733a 2074 7970 696e 672e  headers: typing.
+0000c580: 4f70 7469 6f6e 616c 5b48 5454 5048 6561  Optional[HTTPHea
+0000c590: 6465 7244 6963 745d 203d 204e 6f6e 652c  derDict] = None,
+0000c5a0: 0a20 2020 2020 2020 2073 6572 6961 6c69  .        seriali
+0000c5b0: 7a65 645f 626f 6479 3a20 7479 7069 6e67  zed_body: typing
+0000c5c0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+0000c5d0: 2e55 6e69 6f6e 5b73 7472 2c20 6279 7465  .Union[str, byte
+0000c5e0: 735d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  s]] = None,.    
+0000c5f0: 2020 2020 626f 6479 3a20 7479 7069 6e67      body: typing
+0000c600: 2e41 6e79 203d 204e 6f6e 652c 0a20 2020  .Any = None,.   
+0000c610: 2020 2020 2066 6965 6c64 733a 2074 7970       fields: typ
+0000c620: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+0000c630: 696e 672e 5475 706c 655b 7479 7069 6e67  ing.Tuple[typing
+0000c640: 2e54 7570 6c65 5b73 7472 2c20 7374 725d  .Tuple[str, str]
+0000c650: 2c20 2e2e 2e5d 5d20 3d20 4e6f 6e65 2c0a  , ...]] = None,.
+0000c660: 2020 2020 2020 2020 6175 7468 5f73 6574          auth_set
+0000c670: 7469 6e67 733a 2074 7970 696e 672e 4f70  tings: typing.Op
+0000c680: 7469 6f6e 616c 5b74 7970 696e 672e 4c69  tional[typing.Li
+0000c690: 7374 5b73 7472 5d5d 203d 204e 6f6e 652c  st[str]] = None,
+0000c6a0: 0a20 2020 2020 2020 2073 7472 6561 6d3a  .        stream:
+0000c6b0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+0000c6c0: 2020 2020 2020 2074 696d 656f 7574 3a20         timeout: 
+0000c6d0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+0000c6e0: 7479 7069 6e67 2e55 6e69 6f6e 5b69 6e74  typing.Union[int
+0000c6f0: 2c20 7479 7069 6e67 2e54 7570 6c65 5d5d  , typing.Tuple]]
+0000c700: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000c710: 2068 6f73 743a 2074 7970 696e 672e 4f70   host: typing.Op
+0000c720: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0000c730: 6e65 2c0a 2020 2020 2020 2020 7072 6566  ne,.        pref
+0000c740: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+0000c750: 7261 746f 723a 2050 7265 6669 7853 6570  rator: PrefixSep
+0000c760: 6172 6174 6f72 4974 6572 6174 6f72 203d  aratorIterator =
+0000c770: 204e 6f6e 652c 0a20 2020 2029 202d 3e20   None,.    ) -> 
+0000c780: 4173 796e 6352 6573 706f 6e73 6557 7261  AsyncResponseWra
+0000c790: 7070 6572 3a0a 2020 2020 2020 2020 2222  pper:.        ""
+0000c7a0: 224d 616b 6573 2074 6865 2048 5454 5020  "Makes the HTTP 
+0000c7b0: 7265 7175 6573 7420 2873 796e 6368 726f  request (synchro
+0000c7c0: 6e6f 7573 2920 616e 6420 7265 7475 726e  nous) and return
+0000c7d0: 7320 6465 7365 7269 616c 697a 6564 2064  s deserialized d
+0000c7e0: 6174 612e 0a0a 2020 2020 2020 2020 3a70  ata...        :p
+0000c7f0: 6172 616d 2072 6573 6f75 7263 655f 7061  aram resource_pa
+0000c800: 7468 3a20 5061 7468 2074 6f20 6d65 7468  th: Path to meth
+0000c810: 6f64 2065 6e64 706f 696e 742e 0a20 2020  od endpoint..   
+0000c820: 2020 2020 203a 7061 7261 6d20 6d65 7468       :param meth
+0000c830: 6f64 3a20 4d65 7468 6f64 2074 6f20 6361  od: Method to ca
+0000c840: 6c6c 2e0a 2020 2020 2020 2020 3a70 6172  ll..        :par
+0000c850: 616d 2068 6561 6465 7273 3a20 4865 6164  am headers: Head
+0000c860: 6572 2070 6172 616d 6574 6572 7320 746f  er parameters to
+0000c870: 2062 650a 2020 2020 2020 2020 2020 2020   be.            
+0000c880: 706c 6163 6564 2069 6e20 7468 6520 7265  placed in the re
+0000c890: 7175 6573 7420 6865 6164 6572 2e0a 2020  quest header..  
+0000c8a0: 2020 2020 2020 3a70 6172 616d 2062 6f64        :param bod
+0000c8b0: 793a 2052 6571 7565 7374 2062 6f64 792e  y: Request body.
+0000c8c0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000c8d0: 6669 656c 6473 3a20 5265 7175 6573 7420  fields: Request 
+0000c8e0: 706f 7374 2066 6f72 6d20 7061 7261 6d65  post form parame
+0000c8f0: 7465 7273 2c0a 2020 2020 2020 2020 2020  ters,.          
+0000c900: 2020 666f 7220 6061 7070 6c69 6361 7469    for `applicati
+0000c910: 6f6e 2f78 2d77 7777 2d66 6f72 6d2d 7572  on/x-www-form-ur
+0000c920: 6c65 6e63 6f64 6564 602c 2060 6d75 6c74  lencoded`, `mult
+0000c930: 6970 6172 742f 666f 726d 2d64 6174 6160  ipart/form-data`
+0000c940: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+0000c950: 2061 7574 685f 7365 7474 696e 6773 3a20   auth_settings: 
+0000c960: 4175 7468 2053 6574 7469 6e67 7320 6e61  Auth Settings na
+0000c970: 6d65 7320 666f 7220 7468 6520 7265 7175  mes for the requ
+0000c980: 6573 742e 0a20 2020 2020 2020 203a 7061  est..        :pa
+0000c990: 7261 6d20 7374 7265 616d 3a20 6966 2054  ram stream: if T
+0000c9a0: 7275 652c 2074 6865 2075 726c 6c69 6233  rue, the urllib3
+0000c9b0: 2e48 5454 5052 6573 706f 6e73 6520 6f62  .HTTPResponse ob
+0000c9c0: 6a65 6374 2077 696c 6c0a 2020 2020 2020  ject will.      
+0000c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9e0: 2020 2020 2020 2020 2020 2062 6520 7265             be re
+0000c9f0: 7475 726e 6564 2077 6974 686f 7574 2072  turned without r
+0000ca00: 6561 6469 6e67 2f64 6563 6f64 696e 6720  eading/decoding 
+0000ca10: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
+0000ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca30: 2020 2020 2020 2020 2020 6461 7461 2e20            data. 
+0000ca40: 416c 736f 2077 6865 6e20 5472 7565 2c20  Also when True, 
+0000ca50: 6966 2074 6865 206f 7065 6e61 7069 2073  if the openapi s
+0000ca60: 7065 6320 6465 7363 7269 6265 7320 6120  pec describes a 
+0000ca70: 6669 6c65 2064 6f77 6e6c 6f61 642c 0a20  file download,. 
+0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000caa0: 7468 6520 6461 7461 2077 696c 6c20 6265  the data will be
+0000cab0: 2077 7269 7474 656e 2074 6f20 6120 6c6f   written to a lo
+0000cac0: 6361 6c20 6669 6c65 7379 7374 6d65 2066  cal filesystme f
+0000cad0: 696c 6520 616e 6420 7468 6520 4269 6e61  ile and the Bina
+0000cae0: 7279 5363 6865 6d61 0a20 2020 2020 2020  rySchema.       
+0000caf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb00: 2020 2020 2020 2020 2020 696e 7374 616e            instan
+0000cb10: 6365 2077 696c 6c20 616c 736f 2069 6e68  ce will also inh
+0000cb20: 6572 6974 2066 726f 6d20 4669 6c65 5363  erit from FileSc
+0000cb30: 6865 6d61 2061 6e64 2046 696c 6549 4f0a  hema and FileIO.
+0000cb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb60: 2044 6566 6175 6c74 2069 7320 4661 6c73   Default is Fals
+0000cb70: 652e 0a20 2020 2020 2020 203a 7479 7065  e..        :type
+0000cb80: 2073 7472 6561 6d3a 2062 6f6f 6c2c 206f   stream: bool, o
+0000cb90: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0000cba0: 3a70 6172 616d 2074 696d 656f 7574 3a20  :param timeout: 
+0000cbb0: 7469 6d65 6f75 7420 7365 7474 696e 6720  timeout setting 
+0000cbc0: 666f 7220 7468 6973 2072 6571 7565 7374  for this request
+0000cbd0: 2e20 4966 206f 6e65 0a20 2020 2020 2020  . If one.       
+0000cbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbf0: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
+0000cc00: 2070 726f 7669 6465 642c 2069 7420 7769   provided, it wi
+0000cc10: 6c6c 2062 6520 746f 7461 6c20 7265 7175  ll be total requ
+0000cc20: 6573 740a 2020 2020 2020 2020 2020 2020  est.            
+0000cc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc40: 2020 2020 2074 696d 656f 7574 2e20 4974       timeout. It
+0000cc50: 2063 616e 2061 6c73 6f20 6265 2061 2070   can also be a p
+0000cc60: 6169 7220 2874 7570 6c65 2920 6f66 0a20  air (tuple) of. 
+0000cc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc90: 2863 6f6e 6e65 6374 696f 6e2c 2072 6561  (connection, rea
+0000cca0: 6429 2074 696d 656f 7574 732e 0a20 2020  d) timeouts..   
+0000ccb0: 2020 2020 203a 7061 7261 6d20 686f 7374       :param host
+0000ccc0: 3a20 6170 6920 656e 6470 6f69 6e74 2068  : api endpoint h
+0000ccd0: 6f73 740a 2020 2020 2020 2020 3a72 6574  ost.        :ret
+0000cce0: 7572 6e3a 2072 6573 706f 6e73 650a 2020  urn: response.  
+0000ccf0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000cd00: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
+0000cd10: 656c 662e 5f5f 6173 796e 635f 6361 6c6c  elf.__async_call
+0000cd20: 5f61 7069 280a 2020 2020 2020 2020 2020  _api(.          
+0000cd30: 2020 7265 736f 7572 6365 5f70 6174 682c    resource_path,
+0000cd40: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+0000cd50: 686f 642c 0a20 2020 2020 2020 2020 2020  hod,.           
+0000cd60: 2068 6561 6465 7273 2c0a 2020 2020 2020   headers,.      
+0000cd70: 2020 2020 2020 7365 7269 616c 697a 6564        serialized
+0000cd80: 5f62 6f64 792c 0a20 2020 2020 2020 2020  _body,.         
+0000cd90: 2020 2062 6f64 792c 0a20 2020 2020 2020     body,.       
+0000cda0: 2020 2020 2066 6965 6c64 732c 0a20 2020       fields,.   
+0000cdb0: 2020 2020 2020 2020 2061 7574 685f 7365           auth_se
+0000cdc0: 7474 696e 6773 2c0a 2020 2020 2020 2020  ttings,.        
+0000cdd0: 2020 2020 7374 7265 616d 2c0a 2020 2020      stream,.    
+0000cde0: 2020 2020 2020 2020 7469 6d65 6f75 742c          timeout,
+0000cdf0: 0a20 2020 2020 2020 2020 2020 2068 6f73  .            hos
+0000ce00: 742c 0a20 2020 2020 2020 2020 2020 2070  t,.            p
+0000ce10: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
+0000ce20: 6974 6572 6174 6f72 2c0a 2020 2020 2020  iterator,.      
+0000ce30: 2020 290a 0a20 2020 2064 6566 2063 616c    )..    def cal
+0000ce40: 6c5f 6170 6928 0a20 2020 2020 2020 2073  l_api(.        s
+0000ce50: 656c 662c 0a20 2020 2020 2020 2072 6573  elf,.        res
+0000ce60: 6f75 7263 655f 7061 7468 3a20 7374 722c  ource_path: str,
+0000ce70: 0a20 2020 2020 2020 206d 6574 686f 643a  .        method:
+0000ce80: 2073 7472 2c0a 2020 2020 2020 2020 6865   str,.        he
+0000ce90: 6164 6572 733a 2074 7970 696e 672e 4f70  aders: typing.Op
+0000cea0: 7469 6f6e 616c 5b48 5454 5048 6561 6465  tional[HTTPHeade
+0000ceb0: 7244 6963 745d 203d 204e 6f6e 652c 0a20  rDict] = None,. 
+0000cec0: 2020 2020 2020 2073 6572 6961 6c69 7a65         serialize
+0000ced0: 645f 626f 6479 3a20 7479 7069 6e67 2e4f  d_body: typing.O
+0000cee0: 7074 696f 6e61 6c5b 7479 7069 6e67 2e55  ptional[typing.U
+0000cef0: 6e69 6f6e 5b73 7472 2c20 6279 7465 735d  nion[str, bytes]
+0000cf00: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000cf10: 2020 626f 6479 3a20 7479 7069 6e67 2e41    body: typing.A
+0000cf20: 6e79 203d 204e 6f6e 652c 0a20 2020 2020  ny = None,.     
+0000cf30: 2020 2066 6965 6c64 733a 2074 7970 696e     fields: typin
+0000cf40: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+0000cf50: 672e 5475 706c 655b 7479 7069 6e67 2e54  g.Tuple[typing.T
+0000cf60: 7570 6c65 5b73 7472 2c20 7374 725d 2c20  uple[str, str], 
+0000cf70: 2e2e 2e5d 5d20 3d20 4e6f 6e65 2c0a 2020  ...]] = None,.  
+0000cf80: 2020 2020 2020 6175 7468 5f73 6574 7469        auth_setti
+0000cf90: 6e67 733a 2074 7970 696e 672e 4f70 7469  ngs: typing.Opti
+0000cfa0: 6f6e 616c 5b74 7970 696e 672e 4c69 7374  onal[typing.List
+0000cfb0: 5b73 7472 5d5d 203d 204e 6f6e 652c 0a20  [str]] = None,. 
+0000cfc0: 2020 2020 2020 2073 7472 6561 6d3a 2062         stream: b
+0000cfd0: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+0000cfe0: 2020 2020 2074 696d 656f 7574 3a20 7479       timeout: ty
+0000cff0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+0000d000: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
+0000d010: 7479 7069 6e67 2e54 7570 6c65 5d5d 203d  typing.Tuple]] =
+0000d020: 204e 6f6e 652c 0a20 2020 2020 2020 2068   None,.        h
+0000d030: 6f73 743a 2074 7970 696e 672e 4f70 7469  ost: typing.Opti
+0000d040: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0000d050: 2c0a 2020 2020 2020 2020 7072 6566 6978  ,.        prefix
+0000d060: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
+0000d070: 746f 723a 2050 7265 6669 7853 6570 6172  tor: PrefixSepar
+0000d080: 6174 6f72 4974 6572 6174 6f72 203d 204e  atorIterator = N
+0000d090: 6f6e 652c 0a20 2020 2029 202d 3e20 5265  one,.    ) -> Re
+0000d0a0: 7370 6f6e 7365 5772 6170 7065 723a 0a20  sponseWrapper:. 
+0000d0b0: 2020 2020 2020 2022 2222 4d61 6b65 7320         """Makes 
+0000d0c0: 7468 6520 4854 5450 2072 6571 7565 7374  the HTTP request
+0000d0d0: 2028 7379 6e63 6872 6f6e 6f75 7329 2061   (synchronous) a
+0000d0e0: 6e64 2072 6574 7572 6e73 2064 6573 6572  nd returns deser
+0000d0f0: 6961 6c69 7a65 6420 6461 7461 2e0a 0a20  ialized data... 
+0000d100: 2020 2020 2020 203a 7061 7261 6d20 7265         :param re
+0000d110: 736f 7572 6365 5f70 6174 683a 2050 6174  source_path: Pat
+0000d120: 6820 746f 206d 6574 686f 6420 656e 6470  h to method endp
+0000d130: 6f69 6e74 2e0a 2020 2020 2020 2020 3a70  oint..        :p
+0000d140: 6172 616d 206d 6574 686f 643a 204d 6574  aram method: Met
+0000d150: 686f 6420 746f 2063 616c 6c2e 0a20 2020  hod to call..   
+0000d160: 2020 2020 203a 7061 7261 6d20 6865 6164       :param head
+0000d170: 6572 733a 2048 6561 6465 7220 7061 7261  ers: Header para
+0000d180: 6d65 7465 7273 2074 6f20 6265 0a20 2020  meters to be.   
+0000d190: 2020 2020 2020 2020 2070 6c61 6365 6420           placed 
+0000d1a0: 696e 2074 6865 2072 6571 7565 7374 2068  in the request h
+0000d1b0: 6561 6465 722e 0a20 2020 2020 2020 203a  eader..        :
+0000d1c0: 7061 7261 6d20 626f 6479 3a20 5265 7175  param body: Requ
+0000d1d0: 6573 7420 626f 6479 2e0a 2020 2020 2020  est body..      
+0000d1e0: 2020 3a70 6172 616d 2066 6965 6c64 733a    :param fields:
+0000d1f0: 2052 6571 7565 7374 2070 6f73 7420 666f   Request post fo
+0000d200: 726d 2070 6172 616d 6574 6572 732c 0a20  rm parameters,. 
+0000d210: 2020 2020 2020 2020 2020 2066 6f72 2060             for `
+0000d220: 6170 706c 6963 6174 696f 6e2f 782d 7777  application/x-ww
+0000d230: 772d 666f 726d 2d75 726c 656e 636f 6465  w-form-urlencode
+0000d240: 6460 2c20 606d 756c 7469 7061 7274 2f66  d`, `multipart/f
+0000d250: 6f72 6d2d 6461 7461 602e 0a20 2020 2020  orm-data`..     
+0000d260: 2020 203a 7061 7261 6d20 6175 7468 5f73     :param auth_s
+0000d270: 6574 7469 6e67 733a 2041 7574 6820 5365  ettings: Auth Se
+0000d280: 7474 696e 6773 206e 616d 6573 2066 6f72  ttings names for
+0000d290: 2074 6865 2072 6571 7565 7374 2e0a 2020   the request..  
+0000d2a0: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
+0000d2b0: 6561 6d3a 2069 6620 5472 7565 2c20 7468  eam: if True, th
+0000d2c0: 6520 7572 6c6c 6962 332e 4854 5450 5265  e urllib3.HTTPRe
+0000d2d0: 7370 6f6e 7365 206f 626a 6563 7420 7769  sponse object wi
+0000d2e0: 6c6c 0a20 2020 2020 2020 2020 2020 2020  ll.             
+0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d300: 2020 2020 6265 2072 6574 7572 6e65 6420      be returned 
+0000d310: 7769 7468 6f75 7420 7265 6164 696e 672f  without reading/
+0000d320: 6465 636f 6469 6e67 2072 6573 706f 6e73  decoding respons
+0000d330: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d350: 2020 2064 6174 612e 2041 6c73 6f20 7768     data. Also wh
+0000d360: 656e 2054 7275 652c 2069 6620 7468 6520  en True, if the 
+0000d370: 6f70 656e 6170 6920 7370 6563 2064 6573  openapi spec des
+0000d380: 6372 6962 6573 2061 2066 696c 6520 646f  cribes a file do
+0000d390: 776e 6c6f 6164 2c0a 2020 2020 2020 2020  wnload,.        
+0000d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3b0: 2020 2020 2020 2020 2074 6865 2064 6174           the dat
+0000d3c0: 6120 7769 6c6c 2062 6520 7772 6974 7465  a will be writte
+0000d3d0: 6e20 746f 2061 206c 6f63 616c 2066 696c  n to a local fil
+0000d3e0: 6573 7973 746d 6520 6669 6c65 2061 6e64  esystme file and
+0000d3f0: 2074 6865 2042 696e 6172 7953 6368 656d   the BinarySchem
+0000d400: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+0000d410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d420: 2020 2069 6e73 7461 6e63 6520 7769 6c6c     instance will
+0000d430: 2061 6c73 6f20 696e 6865 7269 7420 6672   also inherit fr
+0000d440: 6f6d 2046 696c 6553 6368 656d 6120 616e  om FileSchema an
+0000d450: 6420 4669 6c65 494f 0a20 2020 2020 2020  d FileIO.       
+0000d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d470: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+0000d480: 7420 6973 2046 616c 7365 2e0a 2020 2020  t is False..    
+0000d490: 2020 2020 3a74 7970 6520 7374 7265 616d      :type stream
+0000d4a0: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+0000d4b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000d4c0: 7469 6d65 6f75 743a 2074 696d 656f 7574  timeout: timeout
+0000d4d0: 2073 6574 7469 6e67 2066 6f72 2074 6869   setting for thi
+0000d4e0: 7320 7265 7175 6573 742e 2049 6620 6f6e  s request. If on
+0000d4f0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d510: 2020 206e 756d 6265 7220 7072 6f76 6964     number provid
+0000d520: 6564 2c20 6974 2077 696c 6c20 6265 2074  ed, it will be t
+0000d530: 6f74 616c 2072 6571 7565 7374 0a20 2020  otal request.   
+0000d540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d550: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+0000d560: 6d65 6f75 742e 2049 7420 6361 6e20 616c  meout. It can al
+0000d570: 736f 2062 6520 6120 7061 6972 2028 7475  so be a pair (tu
+0000d580: 706c 6529 206f 660a 2020 2020 2020 2020  ple) of.        
+0000d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5a0: 2020 2020 2020 2020 2028 636f 6e6e 6563           (connec
+0000d5b0: 7469 6f6e 2c20 7265 6164 2920 7469 6d65  tion, read) time
+0000d5c0: 6f75 7473 2e0a 2020 2020 2020 2020 3a70  outs..        :p
+0000d5d0: 6172 616d 2068 6f73 743a 2061 7069 2065  aram host: api e
+0000d5e0: 6e64 706f 696e 7420 686f 7374 0a20 2020  ndpoint host.   
+0000d5f0: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
+0000d600: 7370 6f6e 7365 0a20 2020 2020 2020 2022  sponse.        "
+0000d610: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0000d620: 6e20 7365 6c66 2e5f 5f63 616c 6c5f 6170  n self.__call_ap
+0000d630: 6928 0a20 2020 2020 2020 2020 2020 2072  i(.            r
+0000d640: 6573 6f75 7263 655f 7061 7468 2c0a 2020  esource_path,.  
+0000d650: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
+0000d660: 2c0a 2020 2020 2020 2020 2020 2020 6865  ,.            he
+0000d670: 6164 6572 732c 0a20 2020 2020 2020 2020  aders,.         
+0000d680: 2020 2073 6572 6961 6c69 7a65 645f 626f     serialized_bo
+0000d690: 6479 2c0a 2020 2020 2020 2020 2020 2020  dy,.            
+0000d6a0: 626f 6479 2c0a 2020 2020 2020 2020 2020  body,.          
+0000d6b0: 2020 6669 656c 6473 2c0a 2020 2020 2020    fields,.      
+0000d6c0: 2020 2020 2020 6175 7468 5f73 6574 7469        auth_setti
+0000d6d0: 6e67 732c 0a20 2020 2020 2020 2020 2020  ngs,.           
+0000d6e0: 2073 7472 6561 6d2c 0a20 2020 2020 2020   stream,.       
+0000d6f0: 2020 2020 2074 696d 656f 7574 2c0a 2020       timeout,.  
+0000d700: 2020 2020 2020 2020 2020 686f 7374 2c0a            host,.
+0000d710: 2020 2020 2020 2020 2020 2020 7072 6566              pref
+0000d720: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+0000d730: 7261 746f 722c 0a20 2020 2020 2020 2029  rator,.        )
+0000d740: 0a0a 2020 2020 6465 6620 6669 656c 6473  ..    def fields
+0000d750: 5f74 6f5f 6469 6374 2873 656c 662c 2066  _to_dict(self, f
+0000d760: 6965 6c64 733a 2074 7970 696e 672e 4f70  ields: typing.Op
+0000d770: 7469 6f6e 616c 5b74 7970 696e 672e 5475  tional[typing.Tu
+0000d780: 706c 655b 7479 7069 6e67 2e54 7570 6c65  ple[typing.Tuple
+0000d790: 5b73 7472 2c20 7374 725d 2c20 2e2e 2e5d  [str, str], ...]
+0000d7a0: 5d29 3a0a 2020 2020 2020 2020 2222 2243  ]):.        """C
+0000d7b0: 6f6e 7665 7274 7320 6669 656c 6473 2074  onverts fields t
+0000d7c0: 6f20 6469 6374 2e0a 0a20 2020 2020 2020  o dict...       
+0000d7d0: 203a 7061 7261 6d20 6669 656c 6473 3a20   :param fields: 
+0000d7e0: 6669 656c 6473 0a20 2020 2020 2020 203a  fields.        :
+0000d7f0: 7265 7475 726e 3a20 6469 6374 0a20 2020  return: dict.   
+0000d800: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000d810: 2069 6620 6669 656c 6473 2069 7320 4e6f   if fields is No
+0000d820: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000d830: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
+0000d840: 2020 2020 7265 7475 726e 207b 6b3a 2076      return {k: v
+0000d850: 2066 6f72 206b 2c20 7620 696e 2066 6965   for k, v in fie
+0000d860: 6c64 737d 0a0a 2020 2020 6173 796e 6320  lds}..    async 
+0000d870: 6465 6620 6173 796e 635f 7265 7175 6573  def async_reques
+0000d880: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
+0000d890: 0a20 2020 2020 2020 206d 6574 686f 643a  .        method:
+0000d8a0: 2073 7472 2c0a 2020 2020 2020 2020 7572   str,.        ur
+0000d8b0: 6c3a 2073 7472 2c0a 2020 2020 2020 2020  l: str,.        
+0000d8c0: 6865 6164 6572 733a 2074 7970 696e 672e  headers: typing.
+0000d8d0: 4f70 7469 6f6e 616c 5b48 5454 5048 6561  Optional[HTTPHea
+0000d8e0: 6465 7244 6963 745d 203d 204e 6f6e 652c  derDict] = None,
+0000d8f0: 0a20 2020 2020 2020 2066 6965 6c64 733a  .        fields:
+0000d900: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0000d910: 5b74 7970 696e 672e 5475 706c 655b 7479  [typing.Tuple[ty
+0000d920: 7069 6e67 2e54 7570 6c65 5b73 7472 2c20  ping.Tuple[str, 
+0000d930: 7374 725d 2c20 2e2e 2e5d 5d20 3d20 4e6f  str], ...]] = No
+0000d940: 6e65 2c0a 2020 2020 2020 2020 626f 6479  ne,.        body
+0000d950: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+0000d960: 6c5b 7479 7069 6e67 2e55 6e69 6f6e 5b73  l[typing.Union[s
+0000d970: 7472 2c20 6279 7465 735d 5d20 3d20 4e6f  tr, bytes]] = No
+0000d980: 6e65 2c0a 2020 2020 2020 2020 7374 7265  ne,.        stre
+0000d990: 616d 3a20 626f 6f6c 203d 2046 616c 7365  am: bool = False
+0000d9a0: 2c0a 2020 2020 2020 2020 7469 6d65 6f75  ,.        timeou
+0000d9b0: 743a 2074 7970 696e 672e 4f70 7469 6f6e  t: typing.Option
+0000d9c0: 616c 5b74 7970 696e 672e 556e 696f 6e5b  al[typing.Union[
+0000d9d0: 696e 742c 2074 7970 696e 672e 5475 706c  int, typing.Tupl
+0000d9e0: 655d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  e]] = None,.    
+0000d9f0: 2920 2d3e 2041 7379 6e63 5265 7370 6f6e  ) -> AsyncRespon
+0000da00: 7365 5772 6170 7065 723a 0a20 2020 2020  seWrapper:.     
+0000da10: 2020 2069 6620 626f 6479 2061 6e64 2066     if body and f
+0000da20: 6965 6c64 733a 0a20 2020 2020 2020 2020  ields:.         
+0000da30: 2020 2072 6169 7365 2041 7069 5661 6c75     raise ApiValu
+0000da40: 6545 7272 6f72 2822 626f 6479 2070 6172  eError("body par
+0000da50: 616d 6574 6572 2063 616e 6e6f 7420 6265  ameter cannot be
+0000da60: 2075 7365 6420 7769 7468 2066 6965 6c64   used with field
+0000da70: 7320 7061 7261 6d65 7465 7222 290a 2020  s parameter").  
+0000da80: 2020 2020 2020 6461 7461 203d 204e 6f6e        data = Non
+0000da90: 650a 2020 2020 2020 2020 6966 2062 6f64  e.        if bod
+0000daa0: 793a 0a20 2020 2020 2020 2020 2020 2064  y:.            d
+0000dab0: 6174 613d 626f 6479 0a20 2020 2020 2020  ata=body.       
+0000dac0: 2069 6620 6669 656c 6473 3a0a 2020 2020   if fields:.    
+0000dad0: 2020 2020 2020 2020 6461 7461 3d73 656c          data=sel
+0000dae0: 662e 6669 656c 6473 5f74 6f5f 6469 6374  f.fields_to_dict
+0000daf0: 2866 6965 6c64 7329 0a20 2020 2020 2020  (fields).       
+0000db00: 2073 6573 7369 6f6e 203d 2061 696f 6874   session = aioht
+0000db10: 7470 2e43 6c69 656e 7453 6573 7369 6f6e  tp.ClientSession
+0000db20: 2829 0a20 2020 2020 2020 2074 3120 3d20  ().        t1 = 
+0000db30: 7469 6d65 2e74 696d 6528 290a 2020 2020  time.time().    
+0000db40: 2020 2020 6966 206d 6574 686f 6420 3d3d      if method ==
+0000db50: 2022 4745 5422 3a0a 2020 2020 2020 2020   "GET":.        
+0000db60: 2020 2020 7365 7373 696f 6e2e 6765 7428      session.get(
+0000db70: 7572 6c29 0a20 2020 2020 2020 2020 2020  url).           
+0000db80: 2072 6573 706f 6e73 6520 3d20 6177 6169   response = awai
+0000db90: 7420 7365 7373 696f 6e2e 6765 7428 7572  t session.get(ur
+0000dba0: 6c2c 2068 6561 6465 7273 3d68 6561 6465  l, headers=heade
+0000dbb0: 7273 290a 2020 2020 2020 2020 2020 2020  rs).            
+0000dbc0: 7265 7475 726e 2041 7379 6e63 5265 7370  return AsyncResp
+0000dbd0: 6f6e 7365 5772 6170 7065 7228 7265 7370  onseWrapper(resp
+0000dbe0: 6f6e 7365 2c20 7469 6d65 2e74 696d 6528  onse, time.time(
+0000dbf0: 2920 2d20 7431 2c20 7365 7373 696f 6e29  ) - t1, session)
+0000dc00: 0a20 2020 2020 2020 2065 6c69 6620 6d65  .        elif me
+0000dc10: 7468 6f64 203d 3d20 2248 4541 4422 3a0a  thod == "HEAD":.
+0000dc20: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+0000dc30: 6f6e 7365 203d 2061 7761 6974 2073 6573  onse = await ses
+0000dc40: 7369 6f6e 2e68 6561 6428 7572 6c2c 2068  sion.head(url, h
+0000dc50: 6561 6465 7273 3d68 6561 6465 7273 290a  eaders=headers).
+0000dc60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000dc70: 726e 2041 7379 6e63 5265 7370 6f6e 7365  rn AsyncResponse
+0000dc80: 5772 6170 7065 7228 7265 7370 6f6e 7365  Wrapper(response
+0000dc90: 2c20 7469 6d65 2e74 696d 6528 2920 2d20  , time.time() - 
+0000dca0: 7431 2c20 7365 7373 696f 6e29 0a20 2020  t1, session).   
+0000dcb0: 2020 2020 2065 6c69 6620 6d65 7468 6f64       elif method
+0000dcc0: 203d 3d20 224f 5054 494f 4e53 223a 0a20   == "OPTIONS":. 
+0000dcd0: 2020 2020 2020 2020 2020 2072 6573 706f             respo
+0000dce0: 6e73 6520 3d20 6177 6169 7420 7365 7373  nse = await sess
+0000dcf0: 696f 6e2e 6f70 7469 6f6e 7328 7572 6c2c  ion.options(url,
+0000dd00: 2064 6174 613d 6461 7461 2c20 6865 6164   data=data, head
+0000dd10: 6572 733d 6865 6164 6572 7329 0a20 2020  ers=headers).   
+0000dd20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000dd30: 4173 796e 6352 6573 706f 6e73 6557 7261  AsyncResponseWra
+0000dd40: 7070 6572 2872 6573 706f 6e73 652c 2074  pper(response, t
+0000dd50: 696d 652e 7469 6d65 2829 202d 2074 312c  ime.time() - t1,
+0000dd60: 2073 6573 7369 6f6e 290a 2020 2020 2020   session).      
+0000dd70: 2020 656c 6966 206d 6574 686f 6420 3d3d    elif method ==
+0000dd80: 2022 504f 5354 223a 0a20 2020 2020 2020   "POST":.       
+0000dd90: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+0000dda0: 6177 6169 7420 7365 7373 696f 6e2e 706f  await session.po
+0000ddb0: 7374 2875 726c 2c20 6461 7461 3d64 6174  st(url, data=dat
+0000ddc0: 612c 2068 6561 6465 7273 3d68 6561 6465  a, headers=heade
+0000ddd0: 7273 290a 2020 2020 2020 2020 2020 2020  rs).            
+0000dde0: 7265 7475 726e 2041 7379 6e63 5265 7370  return AsyncResp
+0000ddf0: 6f6e 7365 5772 6170 7065 7228 7265 7370  onseWrapper(resp
+0000de00: 6f6e 7365 2c20 7469 6d65 2e74 696d 6528  onse, time.time(
+0000de10: 2920 2d20 7431 2c20 7365 7373 696f 6e29  ) - t1, session)
+0000de20: 0a20 2020 2020 2020 2065 6c69 6620 6d65  .        elif me
+0000de30: 7468 6f64 203d 3d20 2250 5554 223a 0a20  thod == "PUT":. 
+0000de40: 2020 2020 2020 2020 2020 2072 6573 706f             respo
+0000de50: 6e73 6520 3d20 6177 6169 7420 7365 7373  nse = await sess
+0000de60: 696f 6e2e 7075 7428 7572 6c2c 2064 6174  ion.put(url, dat
+0000de70: 613d 6461 7461 2c20 6865 6164 6572 733d  a=data, headers=
+0000de80: 6865 6164 6572 7329 0a20 2020 2020 2020  headers).       
+0000de90: 2020 2020 2072 6574 7572 6e20 4173 796e       return Asyn
+0000dea0: 6352 6573 706f 6e73 6557 7261 7070 6572  cResponseWrapper
+0000deb0: 2872 6573 706f 6e73 652c 2074 696d 652e  (response, time.
+0000dec0: 7469 6d65 2829 202d 2074 312c 2073 6573  time() - t1, ses
+0000ded0: 7369 6f6e 290a 2020 2020 2020 2020 656c  sion).        el
+0000dee0: 6966 206d 6574 686f 6420 3d3d 2022 5041  if method == "PA
+0000def0: 5443 4822 3a0a 2020 2020 2020 2020 2020  TCH":.          
+0000df00: 2020 7265 7370 6f6e 7365 203d 2061 7761    response = awa
+0000df10: 6974 2073 6573 7369 6f6e 2e70 6174 6368  it session.patch
+0000df20: 2875 726c 2c20 6461 7461 3d64 6174 612c  (url, data=data,
+0000df30: 2068 6561 6465 7273 3d68 6561 6465 7273   headers=headers
+0000df40: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0000df50: 7475 726e 2041 7379 6e63 5265 7370 6f6e  turn AsyncRespon
+0000df60: 7365 5772 6170 7065 7228 7265 7370 6f6e  seWrapper(respon
+0000df70: 7365 2c20 7469 6d65 2e74 696d 6528 2920  se, time.time() 
+0000df80: 2d20 7431 2c20 7365 7373 696f 6e29 0a20  - t1, session). 
+0000df90: 2020 2020 2020 2065 6c69 6620 6d65 7468         elif meth
+0000dfa0: 6f64 203d 3d20 2244 454c 4554 4522 3a0a  od == "DELETE":.
+0000dfb0: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+0000dfc0: 6f6e 7365 203d 2061 7761 6974 2073 6573  onse = await ses
+0000dfd0: 7369 6f6e 2e64 656c 6574 6528 7572 6c2c  sion.delete(url,
+0000dfe0: 2064 6174 613d 6461 7461 2c20 6865 6164   data=data, head
+0000dff0: 6572 733d 6865 6164 6572 7329 0a20 2020  ers=headers).   
+0000e000: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000e010: 4173 796e 6352 6573 706f 6e73 6557 7261  AsyncResponseWra
+0000e020: 7070 6572 2872 6573 706f 6e73 652c 2074  pper(response, t
+0000e030: 696d 652e 7469 6d65 2829 202d 2074 312c  ime.time() - t1,
+0000e040: 2073 6573 7369 6f6e 290a 2020 2020 2020   session).      
+0000e050: 2020 7261 6973 6520 4170 6956 616c 7565    raise ApiValue
+0000e060: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+0000e070: 2020 2022 6874 7470 206d 6574 686f 6420     "http method 
+0000e080: 6d75 7374 2062 6520 6047 4554 602c 2060  must be `GET`, `
+0000e090: 4845 4144 602c 2060 4f50 5449 4f4e 5360  HEAD`, `OPTIONS`
+0000e0a0: 2c22 0a20 2020 2020 2020 2020 2020 2022  ,".            "
+0000e0b0: 2060 504f 5354 602c 2060 5041 5443 4860   `POST`, `PATCH`
+0000e0c0: 2c20 6050 5554 6020 6f72 2060 4445 4c45  , `PUT` or `DELE
+0000e0d0: 5445 602e 220a 2020 2020 2020 2020 290a  TE`.".        ).
+0000e0e0: 0a20 2020 2064 6566 2072 6571 7565 7374  .    def request
+0000e0f0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000e100: 2020 2020 2020 2020 6d65 7468 6f64 3a20          method: 
+0000e110: 7374 722c 0a20 2020 2020 2020 2075 726c  str,.        url
+0000e120: 3a20 7374 722c 0a20 2020 2020 2020 2068  : str,.        h
+0000e130: 6561 6465 7273 3a20 7479 7069 6e67 2e4f  eaders: typing.O
+0000e140: 7074 696f 6e61 6c5b 4854 5450 4865 6164  ptional[HTTPHead
+0000e150: 6572 4469 6374 5d20 3d20 4e6f 6e65 2c0a  erDict] = None,.
+0000e160: 2020 2020 2020 2020 6669 656c 6473 3a20          fields: 
+0000e170: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+0000e180: 7479 7069 6e67 2e54 7570 6c65 5b74 7970  typing.Tuple[typ
+0000e190: 696e 672e 5475 706c 655b 7374 722c 2073  ing.Tuple[str, s
+0000e1a0: 7472 5d2c 202e 2e2e 5d5d 203d 204e 6f6e  tr], ...]] = Non
+0000e1b0: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
+0000e1c0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0000e1d0: 5b74 7970 696e 672e 556e 696f 6e5b 7374  [typing.Union[st
+0000e1e0: 722c 2062 7974 6573 5d5d 203d 204e 6f6e  r, bytes]] = Non
+0000e1f0: 652c 0a20 2020 2020 2020 2073 7472 6561  e,.        strea
+0000e200: 6d3a 2062 6f6f 6c20 3d20 4661 6c73 652c  m: bool = False,
+0000e210: 0a20 2020 2020 2020 2074 696d 656f 7574  .        timeout
+0000e220: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+0000e230: 6c5b 7479 7069 6e67 2e55 6e69 6f6e 5b69  l[typing.Union[i
+0000e240: 6e74 2c20 7479 7069 6e67 2e54 7570 6c65  nt, typing.Tuple
+0000e250: 5d5d 203d 204e 6f6e 652c 0a20 2020 2029  ]] = None,.    )
+0000e260: 202d 3e20 5265 7370 6f6e 7365 5772 6170   -> ResponseWrap
+0000e270: 7065 723a 0a20 2020 2020 2020 2022 2222  per:.        """
+0000e280: 4d61 6b65 7320 7468 6520 4854 5450 2072  Makes the HTTP r
+0000e290: 6571 7565 7374 2075 7369 6e67 2052 4553  equest using RES
+0000e2a0: 5443 6c69 656e 742e 2222 220a 2020 2020  TClient.""".    
+0000e2b0: 2020 2020 6966 206d 6574 686f 6420 3d3d      if method ==
+0000e2c0: 2022 4745 5422 3a0a 2020 2020 2020 2020   "GET":.        
+0000e2d0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000e2e0: 7265 7374 5f63 6c69 656e 742e 4745 5428  rest_client.GET(
+0000e2f0: 7572 6c2c 0a20 2020 2020 2020 2020 2020  url,.           
+0000e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e310: 2020 2020 2020 2020 2020 2020 2073 7472               str
+0000e320: 6561 6d3d 7374 7265 616d 2c0a 2020 2020  eam=stream,.    
+0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e350: 2020 2020 7469 6d65 6f75 743d 7469 6d65      timeout=time
+0000e360: 6f75 742c 0a20 2020 2020 2020 2020 2020  out,.           
+0000e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e380: 2020 2020 2020 2020 2020 2020 2068 6561               hea
+0000e390: 6465 7273 3d68 6561 6465 7273 290a 2020  ders=headers).  
+0000e3a0: 2020 2020 2020 656c 6966 206d 6574 686f        elif metho
+0000e3b0: 6420 3d3d 2022 4845 4144 223a 0a20 2020  d == "HEAD":.   
+0000e3c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000e3d0: 7365 6c66 2e72 6573 745f 636c 6965 6e74  self.rest_client
+0000e3e0: 2e48 4541 4428 7572 6c2c 0a20 2020 2020  .HEAD(url,.     
+0000e3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e410: 2020 2020 7374 7265 616d 3d73 7472 6561      stream=strea
+0000e420: 6d2c 0a20 2020 2020 2020 2020 2020 2020  m,.             
+0000e430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e440: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0000e450: 6f75 743d 7469 6d65 6f75 742c 0a20 2020  out=timeout,.   
+0000e460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e480: 2020 2020 2020 6865 6164 6572 733d 6865        headers=he
+0000e490: 6164 6572 7329 0a20 2020 2020 2020 2065  aders).        e
+0000e4a0: 6c69 6620 6d65 7468 6f64 203d 3d20 224f  lif method == "O
+0000e4b0: 5054 494f 4e53 223a 0a20 2020 2020 2020  PTIONS":.       
+0000e4c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000e4d0: 2e72 6573 745f 636c 6965 6e74 2e4f 5054  .rest_client.OPT
+0000e4e0: 494f 4e53 2875 726c 2c0a 2020 2020 2020  IONS(url,.      
+0000e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e510: 2020 2020 2020 6865 6164 6572 733d 6865        headers=he
+0000e520: 6164 6572 732c 0a20 2020 2020 2020 2020  aders,.         
+0000e530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e550: 2020 2066 6965 6c64 733d 6669 656c 6473     fields=fields
+0000e560: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e580: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000e590: 7265 616d 3d73 7472 6561 6d2c 0a20 2020  ream=stream,.   
+0000e5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5c0: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
+0000e5d0: 3d74 696d 656f 7574 2c0a 2020 2020 2020  =timeout,.      
+0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e600: 2020 2020 2020 626f 6479 3d62 6f64 7929        body=body)
+0000e610: 0a20 2020 2020 2020 2065 6c69 6620 6d65  .        elif me
+0000e620: 7468 6f64 203d 3d20 2250 4f53 5422 3a0a  thod == "POST":.
+0000e630: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000e640: 726e 2073 656c 662e 7265 7374 5f63 6c69  rn self.rest_cli
+0000e650: 656e 742e 504f 5354 2875 726c 2c0a 2020  ent.POST(url,.  
+0000e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e680: 2020 2020 2020 2068 6561 6465 7273 3d68         headers=h
+0000e690: 6561 6465 7273 2c0a 2020 2020 2020 2020  eaders,.        
+0000e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6c0: 2066 6965 6c64 733d 6669 656c 6473 2c0a   fields=fields,.
+0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6f0: 6461 7461 3d76 616c 7565 2e72 6561 6428  data=value.read(
-0000e700: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000e710: 2020 2066 696c 656e 616d 653d 6669 6c65     filename=file
-0000e720: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-0000e730: 2020 2020 2020 6865 6164 6572 733d 7b27        headers={'
-0000e740: 436f 6e74 656e 742d 5479 7065 273a 2067  Content-Type': g
-0000e750: 7565 7373 5f63 6f6e 7465 6e74 5f74 7970  uess_content_typ
-0000e760: 6528 6669 6c65 6e61 6d65 297d 0a20 2020  e(filename)}.   
-0000e770: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000e780: 2020 2020 2020 2076 616c 7565 2e63 6c6f         value.clo
-0000e790: 7365 2829 0a20 2020 2020 2020 2020 2020  se().           
-0000e7a0: 2072 6574 7572 6e20 7265 7175 6573 745f   return request_
-0000e7b0: 6669 656c 640a 2020 2020 2020 2020 656c  field.        el
-0000e7c0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000e7d0: 7265 7475 726e 2073 656c 662e 5f5f 6d75  return self.__mu
-0000e7e0: 6c74 6970 6172 745f 6a73 6f6e 5f69 7465  ltipart_json_ite
-0000e7f0: 6d28 6b65 793d 6b65 792c 2076 616c 7565  m(key=key, value
-0000e800: 3d76 616c 7565 290a 0a20 2020 2064 6566  =value)..    def
-0000e810: 205f 5f73 6572 6961 6c69 7a65 5f6d 756c   __serialize_mul
-0000e820: 7469 7061 7274 5f66 6f72 6d5f 6461 7461  tipart_form_data
-0000e830: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-0000e840: 696e 5f64 6174 613a 2053 6368 656d 610a  in_data: Schema.
-0000e850: 2020 2020 2920 2d3e 2074 7970 696e 672e      ) -> typing.
-0000e860: 4469 6374 5b73 7472 2c20 7479 7069 6e67  Dict[str, typing
-0000e870: 2e54 7570 6c65 5b52 6571 7565 7374 4669  .Tuple[RequestFi
-0000e880: 656c 642c 202e 2e2e 5d5d 3a0a 2020 2020  eld, ...]]:.    
-0000e890: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-0000e8a0: 7461 6e63 6528 696e 5f64 6174 612c 2066  tance(in_data, f
-0000e8b0: 726f 7a65 6e64 6963 742e 6672 6f7a 656e  rozendict.frozen
-0000e8c0: 6469 6374 293a 0a20 2020 2020 2020 2020  dict):.         
-0000e8d0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0000e8e0: 726f 7228 6627 556e 6162 6c65 2074 6f20  ror(f'Unable to 
-0000e8f0: 7365 7269 616c 697a 6520 7b69 6e5f 6461  serialize {in_da
-0000e900: 7461 7d20 746f 206d 756c 7469 7061 7274  ta} to multipart
-0000e910: 2f66 6f72 6d2d 6461 7461 2062 6563 6175  /form-data becau
-0000e920: 7365 2069 7420 6973 206e 6f74 2061 2064  se it is not a d
-0000e930: 6963 7420 6f66 2064 6174 6127 290a 2020  ict of data').  
-0000e940: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000e950: 2020 496e 2061 206d 756c 7469 7061 7274    In a multipart
-0000e960: 2f66 6f72 6d2d 6461 7461 2072 6571 7565  /form-data reque
-0000e970: 7374 2062 6f64 792c 2065 6163 6820 7363  st body, each sc
-0000e980: 6865 6d61 2070 726f 7065 7274 792c 206f  hema property, o
-0000e990: 7220 6561 6368 2065 6c65 6d65 6e74 206f  r each element o
-0000e9a0: 6620 6120 7363 6865 6d61 2061 7272 6179  f a schema array
-0000e9b0: 2070 726f 7065 7274 792c 0a20 2020 2020   property,.     
-0000e9c0: 2020 2074 616b 6573 2061 2073 6563 7469     takes a secti
-0000e9d0: 6f6e 2069 6e20 7468 6520 7061 796c 6f61  on in the payloa
-0000e9e0: 6420 7769 7468 2061 6e20 696e 7465 726e  d with an intern
-0000e9f0: 616c 2068 6561 6465 7220 6173 2064 6566  al header as def
-0000ea00: 696e 6564 2062 7920 5246 4337 3537 382e  ined by RFC7578.
-0000ea10: 2054 6865 2073 6572 6961 6c69 7a61 7469   The serializati
-0000ea20: 6f6e 2073 7472 6174 6567 790a 2020 2020  on strategy.    
-0000ea30: 2020 2020 666f 7220 6561 6368 2070 726f      for each pro
-0000ea40: 7065 7274 7920 6f66 2061 206d 756c 7469  perty of a multi
-0000ea50: 7061 7274 2f66 6f72 6d2d 6461 7461 2072  part/form-data r
-0000ea60: 6571 7565 7374 2062 6f64 7920 6361 6e20  equest body can 
-0000ea70: 6265 2073 7065 6369 6669 6564 2069 6e20  be specified in 
-0000ea80: 616e 2061 7373 6f63 6961 7465 6420 456e  an associated En
-0000ea90: 636f 6469 6e67 204f 626a 6563 742e 0a0a  coding Object...
-0000eaa0: 2020 2020 2020 2020 5768 656e 2070 6173          When pas
-0000eab0: 7369 6e67 2069 6e20 6d75 6c74 6970 6172  sing in multipar
-0000eac0: 7420 7479 7065 732c 2062 6f75 6e64 6172  t types, boundar
-0000ead0: 6965 7320 4d41 5920 6265 2075 7365 6420  ies MAY be used 
-0000eae0: 746f 2073 6570 6172 6174 6520 7365 6374  to separate sect
-0000eaf0: 696f 6e73 206f 6620 7468 6520 636f 6e74  ions of the cont
-0000eb00: 656e 7420 6265 696e 670a 2020 2020 2020  ent being.      
-0000eb10: 2020 7472 616e 7366 6572 7265 6420 e280    transferred ..
-0000eb20: 9320 7468 7573 2c20 7468 6520 666f 6c6c  . thus, the foll
-0000eb30: 6f77 696e 6720 6465 6661 756c 7420 436f  owing default Co
-0000eb40: 6e74 656e 742d 5479 7065 7320 6172 6520  ntent-Types are 
-0000eb50: 6465 6669 6e65 6420 666f 7220 6d75 6c74  defined for mult
-0000eb60: 6970 6172 743a 0a0a 2020 2020 2020 2020  ipart:..        
-0000eb70: 4966 2074 6865 2028 6f62 6a65 6374 2920  If the (object) 
-0000eb80: 7072 6f70 6572 7479 2069 7320 6120 7072  property is a pr
-0000eb90: 696d 6974 6976 652c 206f 7220 616e 2061  imitive, or an a
-0000eba0: 7272 6179 206f 6620 7072 696d 6974 6976  rray of primitiv
-0000ebb0: 6520 7661 6c75 6573 2c20 7468 6520 6465  e values, the de
-0000ebc0: 6661 756c 7420 436f 6e74 656e 742d 5479  fault Content-Ty
-0000ebd0: 7065 2069 7320 7465 7874 2f70 6c61 696e  pe is text/plain
-0000ebe0: 0a20 2020 2020 2020 2049 6620 7468 6520  .        If the 
-0000ebf0: 7072 6f70 6572 7479 2069 7320 636f 6d70  property is comp
-0000ec00: 6c65 782c 206f 7220 616e 2061 7272 6179  lex, or an array
-0000ec10: 206f 6620 636f 6d70 6c65 7820 7661 6c75   of complex valu
-0000ec20: 6573 2c20 7468 6520 6465 6661 756c 7420  es, the default 
-0000ec30: 436f 6e74 656e 742d 5479 7065 2069 7320  Content-Type is 
-0000ec40: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-0000ec50: 0a20 2020 2020 2020 2020 2020 2051 7565  .            Que
-0000ec60: 7374 696f 6e3a 2068 6f77 2069 7320 7468  stion: how is th
-0000ec70: 6520 6172 7261 7920 6f66 2070 7269 6d69  e array of primi
-0000ec80: 7469 7665 7320 656e 636f 6465 643f 0a20  tives encoded?. 
-0000ec90: 2020 2020 2020 2049 6620 7468 6520 7072         If the pr
-0000eca0: 6f70 6572 7479 2069 7320 6120 7479 7065  operty is a type
-0000ecb0: 3a20 7374 7269 6e67 2077 6974 6820 6120  : string with a 
-0000ecc0: 636f 6e74 656e 7445 6e63 6f64 696e 672c  contentEncoding,
-0000ecd0: 2074 6865 2064 6566 6175 6c74 2043 6f6e   the default Con
-0000ece0: 7465 6e74 2d54 7970 6520 6973 2061 7070  tent-Type is app
-0000ecf0: 6c69 6361 7469 6f6e 2f6f 6374 6574 2d73  lication/octet-s
-0000ed00: 7472 6561 6d0a 2020 2020 2020 2020 2222  tream.        ""
-0000ed10: 220a 2020 2020 2020 2020 6669 656c 6473  ".        fields
-0000ed20: 3a20 7479 7069 6e67 2e4c 6973 745b 5265  : typing.List[Re
-0000ed30: 7175 6573 7446 6965 6c64 5d20 3d20 5b5d  questField] = []
-0000ed40: 0a20 2020 2020 2020 2066 6f72 206b 6579  .        for key
-0000ed50: 2c20 7661 6c75 6520 696e 2069 6e5f 6461  , value in in_da
-0000ed60: 7461 2e69 7465 6d73 2829 3a0a 2020 2020  ta.items():.    
-0000ed70: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0000ed80: 7461 6e63 6528 7661 6c75 652c 2074 7570  tance(value, tup
-0000ed90: 6c65 293a 0a20 2020 2020 2020 2020 2020  le):.           
-0000eda0: 2020 2020 2069 6620 7661 6c75 653a 0a20       if value:. 
-0000edb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000edc0: 2020 2023 2076 616c 7565 7320 7573 6520     # values use 
-0000edd0: 6578 706c 6f64 6520 3d20 5472 7565 2c20  explode = True, 
-0000ede0: 736f 2074 6865 2063 6f64 6520 6d61 6b65  so the code make
-0000edf0: 7320 6120 5265 7175 6573 7446 6965 6c64  s a RequestField
-0000ee00: 2066 6f72 2065 6163 6820 6974 656d 2077   for each item w
-0000ee10: 6974 6820 6e61 6d65 3d6b 6579 0a20 2020  ith name=key.   
-0000ee20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee30: 2066 6f72 2069 7465 6d20 696e 2076 616c   for item in val
-0000ee40: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
-0000ee50: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-0000ee60: 6573 745f 6669 656c 6420 3d20 7365 6c66  est_field = self
-0000ee70: 2e5f 5f6d 756c 7469 7061 7274 5f66 6f72  .__multipart_for
-0000ee80: 6d5f 6974 656d 286b 6579 3d6b 6579 2c20  m_item(key=key, 
-0000ee90: 7661 6c75 653d 6974 656d 290a 2020 2020  value=item).    
-0000eea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eeb0: 2020 2020 6669 656c 6473 2e61 7070 656e      fields.appen
-0000eec0: 6428 7265 7175 6573 745f 6669 656c 6429  d(request_field)
-0000eed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eee0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000eef0: 2020 2020 2020 2020 2020 2023 2073 656e             # sen
-0000ef00: 6420 616e 2065 6d70 7479 2061 7272 6179  d an empty array
-0000ef10: 2061 7320 6a73 6f6e 2062 6563 6175 7365   as json because
-0000ef20: 2065 7870 6c6f 6469 6e67 2077 696c 6c20   exploding will 
-0000ef30: 6e6f 7420 7365 6e64 2069 740a 2020 2020  not send it.    
-0000ef40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef50: 7265 7175 6573 745f 6669 656c 6420 3d20  request_field = 
-0000ef60: 7365 6c66 2e5f 5f6d 756c 7469 7061 7274  self.__multipart
-0000ef70: 5f6a 736f 6e5f 6974 656d 286b 6579 3d6b  _json_item(key=k
-0000ef80: 6579 2c20 7661 6c75 653d 7661 6c75 6529  ey, value=value)
-0000ef90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000efa0: 2020 2020 2066 6965 6c64 732e 6170 7065       fields.appe
-0000efb0: 6e64 2872 6571 7565 7374 5f66 6965 6c64  nd(request_field
-0000efc0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-0000efd0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000efe0: 2020 2020 7265 7175 6573 745f 6669 656c      request_fiel
-0000eff0: 6420 3d20 7365 6c66 2e5f 5f6d 756c 7469  d = self.__multi
-0000f000: 7061 7274 5f66 6f72 6d5f 6974 656d 286b  part_form_item(k
-0000f010: 6579 3d6b 6579 2c20 7661 6c75 653d 7661  ey=key, value=va
-0000f020: 6c75 6529 0a20 2020 2020 2020 2020 2020  lue).           
-0000f030: 2020 2020 2066 6965 6c64 732e 6170 7065       fields.appe
-0000f040: 6e64 2872 6571 7565 7374 5f66 6965 6c64  nd(request_field
-0000f050: 290a 0a20 2020 2020 2020 2023 2054 6869  )..        # Thi
-0000f060: 7320 6973 206e 6563 6573 7361 7279 2074  s is necessary t
-0000f070: 6f20 6669 6c6c 2074 6865 2022 436f 6e74  o fill the "Cont
-0000f080: 656e 742d 4469 7370 6f73 6974 696f 6e22  ent-Disposition"
-0000f090: 2068 6561 6465 7220 6e65 6564 6564 2066   header needed f
-0000f0a0: 6f72 206e 616d 696e 6720 6669 656c 6473  or naming fields
-0000f0b0: 2069 6e20 6d75 6c74 6970 6172 740a 2020   in multipart.  
-0000f0c0: 2020 2020 2020 666f 7220 6669 656c 6420        for field 
-0000f0d0: 696e 2066 6965 6c64 733a 0a20 2020 2020  in fields:.     
-0000f0e0: 2020 2020 2020 2066 6965 6c64 2e6d 616b         field.mak
-0000f0f0: 655f 6d75 6c74 6970 6172 7428 636f 6e74  e_multipart(cont
-0000f100: 656e 745f 7479 7065 3d66 6965 6c64 2e68  ent_type=field.h
-0000f110: 6561 6465 7273 5b22 436f 6e74 656e 742d  eaders["Content-
-0000f120: 5479 7065 225d 290a 2020 2020 2020 2020  Type"]).        
-0000f130: 7265 7475 726e 2064 6963 7428 6669 656c  return dict(fiel
-0000f140: 6473 3d74 7570 6c65 2866 6965 6c64 7329  ds=tuple(fields)
-0000f150: 290a 0a20 2020 2064 6566 205f 5f73 6572  )..    def __ser
-0000f160: 6961 6c69 7a65 5f61 7070 6c69 6361 7469  ialize_applicati
-0000f170: 6f6e 5f6f 6374 6574 5f73 7472 6561 6d28  on_octet_stream(
-0000f180: 7365 6c66 2c20 696e 5f64 6174 613a 2042  self, in_data: B
-0000f190: 696e 6172 7953 6368 656d 6129 202d 3e20  inarySchema) -> 
-0000f1a0: 7479 7069 6e67 2e44 6963 745b 7374 722c  typing.Dict[str,
-0000f1b0: 2062 7974 6573 5d3a 0a20 2020 2020 2020   bytes]:.       
-0000f1c0: 2069 6620 6973 696e 7374 616e 6365 2869   if isinstance(i
-0000f1d0: 6e5f 6461 7461 2c20 6279 7465 7329 3a0a  n_data, bytes):.
-0000f1e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000f1f0: 726e 2064 6963 7428 626f 6479 3d69 6e5f  rn dict(body=in_
-0000f200: 6461 7461 290a 2020 2020 2020 2020 2320  data).        # 
-0000f210: 4669 6c65 494f 2074 7970 650a 2020 2020  FileIO type.    
-0000f220: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-0000f230: 7428 626f 6479 3d69 6e5f 6461 7461 2e72  t(body=in_data.r
-0000f240: 6561 6428 2929 0a20 2020 2020 2020 2069  ead()).        i
-0000f250: 6e5f 6461 7461 2e63 6c6f 7365 2829 0a20  n_data.close(). 
-0000f260: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0000f270: 7375 6c74 0a0a 2020 2020 6465 6620 5f5f  sult..    def __
-0000f280: 7365 7269 616c 697a 655f 6170 706c 6963  serialize_applic
-0000f290: 6174 696f 6e5f 785f 7777 775f 666f 726d  ation_x_www_form
-0000f2a0: 5f64 6174 6128 0a20 2020 2020 2020 2073  _data(.        s
-0000f2b0: 656c 662c 2069 6e5f 6461 7461 3a20 7479  elf, in_data: ty
-0000f2c0: 7069 6e67 2e41 6e79 0a20 2020 2029 202d  ping.Any.    ) -
-0000f2d0: 3e20 5365 7269 616c 697a 6564 5265 7175  > SerializedRequ
-0000f2e0: 6573 7442 6f64 793a 0a20 2020 2020 2020  estBody:.       
-0000f2f0: 2022 2222 0a20 2020 2020 2020 2050 4f53   """.        POS
-0000f300: 5420 7375 626d 6973 7369 6f6e 206f 6620  T submission of 
-0000f310: 666f 726d 2064 6174 6120 696e 2062 6f64  form data in bod
-0000f320: 790a 2020 2020 2020 2020 2222 220a 2020  y.        """.  
-0000f330: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
-0000f340: 6e73 7461 6e63 6528 696e 5f64 6174 612c  nstance(in_data,
-0000f350: 2066 726f 7a65 6e64 6963 742e 6672 6f7a   frozendict.froz
-0000f360: 656e 6469 6374 293a 0a20 2020 2020 2020  endict):.       
-0000f370: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0000f380: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-0000f390: 2020 2020 2020 2066 2755 6e61 626c 6520         f'Unable 
-0000f3a0: 746f 2073 6572 6961 6c69 7a65 207b 696e  to serialize {in
-0000f3b0: 5f64 6174 617d 2074 6f20 6170 706c 6963  _data} to applic
-0000f3c0: 6174 696f 6e2f 782d 7777 772d 666f 726d  ation/x-www-form
-0000f3d0: 2d75 726c 656e 636f 6465 6420 6265 6361  -urlencoded beca
-0000f3e0: 7573 6520 6974 2069 7320 6e6f 7420 6120  use it is not a 
-0000f3f0: 6469 6374 206f 6620 6461 7461 2729 0a20  dict of data'). 
-0000f400: 2020 2020 2020 2063 6173 745f 696e 5f64         cast_in_d
-0000f410: 6174 6120 3d20 7365 6c66 2e5f 5f6a 736f  ata = self.__jso
-0000f420: 6e5f 656e 636f 6465 722e 6465 6661 756c  n_encoder.defaul
-0000f430: 7428 696e 5f64 6174 6129 0a20 2020 2020  t(in_data).     
-0000f440: 2020 2076 616c 7565 203d 2073 656c 662e     value = self.
-0000f450: 5f73 6572 6961 6c69 7a65 5f66 6f72 6d28  _serialize_form(
-0000f460: 6361 7374 5f69 6e5f 6461 7461 2c20 6e61  cast_in_data, na
-0000f470: 6d65 3d27 272c 2065 7870 6c6f 6465 3d54  me='', explode=T
-0000f480: 7275 652c 2070 6572 6365 6e74 5f65 6e63  rue, percent_enc
-0000f490: 6f64 653d 5472 7565 290a 2020 2020 2020  ode=True).      
-0000f4a0: 2020 7265 7475 726e 2064 6963 7428 626f    return dict(bo
-0000f4b0: 6479 3d76 616c 7565 290a 0a20 2020 2064  dy=value)..    d
-0000f4c0: 6566 2073 6572 6961 6c69 7a65 280a 2020  ef serialize(.  
-0000f4d0: 2020 2020 2020 7365 6c66 2c20 696e 5f64        self, in_d
-0000f4e0: 6174 613a 2074 7970 696e 672e 416e 792c  ata: typing.Any,
-0000f4f0: 2063 6f6e 7465 6e74 5f74 7970 653a 2073   content_type: s
-0000f500: 7472 0a20 2020 2029 202d 3e20 5365 7269  tr.    ) -> Seri
-0000f510: 616c 697a 6564 5265 7175 6573 7442 6f64  alizedRequestBod
-0000f520: 793a 0a20 2020 2020 2020 2022 2222 0a20  y:.        """. 
-0000f530: 2020 2020 2020 2049 6620 6120 7374 7220         If a str 
-0000f540: 6973 2072 6574 7572 6e65 6420 7468 656e  is returned then
-0000f550: 2074 6865 2072 6573 756c 7420 7769 6c6c   the result will
-0000f560: 2062 6520 6173 7369 676e 6564 2074 6f20   be assigned to 
-0000f570: 6461 7461 2077 6865 6e20 6d61 6b69 6e67  data when making
-0000f580: 2074 6865 2072 6571 7565 7374 0a20 2020   the request.   
-0000f590: 2020 2020 2049 6620 6120 7475 706c 6520       If a tuple 
-0000f5a0: 6973 2072 6574 7572 6e65 6420 7468 656e  is returned then
-0000f5b0: 2074 6865 2072 6573 756c 7420 7769 6c6c   the result will
-0000f5c0: 2062 6520 7573 6564 2061 7320 6669 656c   be used as fiel
-0000f5d0: 6473 2069 6e70 7574 2069 6e20 656e 636f  ds input in enco
-0000f5e0: 6465 5f6d 756c 7469 7061 7274 5f66 6f72  de_multipart_for
-0000f5f0: 6d64 6174 610a 2020 2020 2020 2020 5265  mdata.        Re
-0000f600: 7475 726e 2061 2074 7570 6c65 206f 660a  turn a tuple of.
-0000f610: 0a20 2020 2020 2020 2054 6865 206b 6579  .        The key
-0000f620: 206f 6620 7468 6520 7265 7475 726e 2064   of the return d
-0000f630: 6963 7420 6973 0a20 2020 2020 2020 202d  ict is.        -
-0000f640: 2062 6f64 7920 666f 7220 6170 706c 6963   body for applic
-0000f650: 6174 696f 6e2f 6a73 6f6e 0a20 2020 2020  ation/json.     
-0000f660: 2020 202d 2065 6e63 6f64 655f 6d75 6c74     - encode_mult
-0000f670: 6970 6172 7420 616e 6420 6669 656c 6473  ipart and fields
-0000f680: 2066 6f72 206d 756c 7469 7061 7274 2f66   for multipart/f
-0000f690: 6f72 6d2d 6461 7461 0a20 2020 2020 2020  orm-data.       
-0000f6a0: 2022 2222 0a20 2020 2020 2020 206d 6564   """.        med
-0000f6b0: 6961 5f74 7970 6520 3d20 7365 6c66 2e63  ia_type = self.c
-0000f6c0: 6f6e 7465 6e74 5b63 6f6e 7465 6e74 5f74  ontent[content_t
-0000f6d0: 7970 655d 0a20 2020 2020 2020 2069 6620  ype].        if 
-0000f6e0: 6973 696e 7374 616e 6365 2869 6e5f 6461  isinstance(in_da
-0000f6f0: 7461 2c20 6d65 6469 615f 7479 7065 2e73  ta, media_type.s
-0000f700: 6368 656d 6129 3a0a 2020 2020 2020 2020  chema):.        
-0000f710: 2020 2020 6361 7374 5f69 6e5f 6461 7461      cast_in_data
-0000f720: 203d 2069 6e5f 6461 7461 0a20 2020 2020   = in_data.     
-0000f730: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-0000f740: 6365 2869 6e5f 6461 7461 2c20 2864 6963  ce(in_data, (dic
-0000f750: 742c 2066 726f 7a65 6e64 6963 742e 6672  t, frozendict.fr
-0000f760: 6f7a 656e 6469 6374 2929 2061 6e64 2069  ozendict)) and i
-0000f770: 6e5f 6461 7461 3a0a 2020 2020 2020 2020  n_data:.        
-0000f780: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0000f790: 2020 2020 2020 2020 2063 6173 745f 696e           cast_in
-0000f7a0: 5f64 6174 6120 3d20 6d65 6469 615f 7479  _data = media_ty
-0000f7b0: 7065 2e73 6368 656d 6128 2a2a 696e 5f64  pe.schema(**in_d
-0000f7c0: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
-0000f7d0: 2065 7863 6570 7420 5479 7065 4572 726f   except TypeErro
-0000f7e0: 7220 6173 2065 3a0a 2020 2020 2020 2020  r as e:.        
-0000f7f0: 2020 2020 2020 2020 7261 6973 6520 4d69          raise Mi
-0000f800: 7373 696e 6752 6571 7569 7265 6450 6172  ssingRequiredPar
-0000f810: 616d 6574 6572 7345 7272 6f72 2865 290a  ametersError(e).
-0000f820: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000f830: 2020 2020 2020 2020 2020 6361 7374 5f69            cast_i
-0000f840: 6e5f 6461 7461 203d 206d 6564 6961 5f74  n_data = media_t
-0000f850: 7970 652e 7363 6865 6d61 2869 6e5f 6461  ype.schema(in_da
-0000f860: 7461 290a 2020 2020 2020 2020 2320 544f  ta).        # TO
-0000f870: 444f 2063 6865 636b 2066 6f72 2061 6e64  DO check for and
-0000f880: 2075 7365 2065 6e63 6f64 696e 6720 6966   use encoding if
-0000f890: 2069 7420 6578 6973 7473 0a20 2020 2020   it exists.     
-0000f8a0: 2020 2023 2061 6e64 2063 6f6e 7465 6e74     # and content
-0000f8b0: 5f74 7970 6520 6973 206d 756c 7469 7061  _type is multipa
-0000f8c0: 7274 206f 7220 6170 706c 6963 6174 696f  rt or applicatio
-0000f8d0: 6e2f 782d 7777 772d 666f 726d 2d75 726c  n/x-www-form-url
-0000f8e0: 656e 636f 6465 640a 2020 2020 2020 2020  encoded.        
-0000f8f0: 6966 2073 656c 662e 5f63 6f6e 7465 6e74  if self._content
-0000f900: 5f74 7970 655f 6973 5f6a 736f 6e28 636f  _type_is_json(co
-0000f910: 6e74 656e 745f 7479 7065 293a 0a20 2020  ntent_type):.   
-0000f920: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000f930: 7365 6c66 2e5f 5f73 6572 6961 6c69 7a65  self.__serialize
-0000f940: 5f6a 736f 6e28 6361 7374 5f69 6e5f 6461  _json(cast_in_da
-0000f950: 7461 290a 2020 2020 2020 2020 656c 6966  ta).        elif
-0000f960: 2063 6f6e 7465 6e74 5f74 7970 6520 3d3d   content_type ==
-0000f970: 2027 7465 7874 2f70 6c61 696e 273a 0a20   'text/plain':. 
-0000f980: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000f990: 6e20 7365 6c66 2e5f 5f73 6572 6961 6c69  n self.__seriali
-0000f9a0: 7a65 5f74 6578 745f 706c 6169 6e28 6361  ze_text_plain(ca
-0000f9b0: 7374 5f69 6e5f 6461 7461 290a 2020 2020  st_in_data).    
-0000f9c0: 2020 2020 656c 6966 2063 6f6e 7465 6e74      elif content
-0000f9d0: 5f74 7970 6520 3d3d 2027 6d75 6c74 6970  _type == 'multip
-0000f9e0: 6172 742f 666f 726d 2d64 6174 6127 3a0a  art/form-data':.
-0000f9f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000fa00: 726e 2073 656c 662e 5f5f 7365 7269 616c  rn self.__serial
-0000fa10: 697a 655f 6d75 6c74 6970 6172 745f 666f  ize_multipart_fo
-0000fa20: 726d 5f64 6174 6128 6361 7374 5f69 6e5f  rm_data(cast_in_
-0000fa30: 6461 7461 290a 2020 2020 2020 2020 656c  data).        el
-0000fa40: 6966 2063 6f6e 7465 6e74 5f74 7970 6520  if content_type 
-0000fa50: 3d3d 2027 6170 706c 6963 6174 696f 6e2f  == 'application/
-0000fa60: 782d 7777 772d 666f 726d 2d75 726c 656e  x-www-form-urlen
-0000fa70: 636f 6465 6427 3a0a 2020 2020 2020 2020  coded':.        
-0000fa80: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000fa90: 5f5f 7365 7269 616c 697a 655f 6170 706c  __serialize_appl
-0000faa0: 6963 6174 696f 6e5f 785f 7777 775f 666f  ication_x_www_fo
-0000fab0: 726d 5f64 6174 6128 6361 7374 5f69 6e5f  rm_data(cast_in_
-0000fac0: 6461 7461 290a 2020 2020 2020 2020 656c  data).        el
-0000fad0: 6966 2063 6f6e 7465 6e74 5f74 7970 6520  if content_type 
-0000fae0: 3d3d 2027 6170 706c 6963 6174 696f 6e2f  == 'application/
-0000faf0: 6f63 7465 742d 7374 7265 616d 273a 0a20  octet-stream':. 
-0000fb00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000fb10: 6e20 7365 6c66 2e5f 5f73 6572 6961 6c69  n self.__seriali
-0000fb20: 7a65 5f61 7070 6c69 6361 7469 6f6e 5f6f  ze_application_o
-0000fb30: 6374 6574 5f73 7472 6561 6d28 6361 7374  ctet_stream(cast
-0000fb40: 5f69 6e5f 6461 7461 290a 2020 2020 2020  _in_data).      
-0000fb50: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
-0000fb60: 6d65 6e74 6564 4572 726f 7228 2753 6572  mentedError('Ser
-0000fb70: 6961 6c69 7a61 7469 6f6e 2068 6173 206e  ialization has n
-0000fb80: 6f74 2079 6574 2062 6565 6e20 696d 706c  ot yet been impl
-0000fb90: 656d 656e 7465 6420 666f 7220 7b7d 272e  emented for {}'.
-0000fba0: 666f 726d 6174 2863 6f6e 7465 6e74 5f74  format(content_t
-0000fbb0: 7970 6529 290a                           ype)).
+0000e6f0: 2020 2020 2020 2020 2073 7472 6561 6d3d           stream=
+0000e700: 7374 7265 616d 2c0a 2020 2020 2020 2020  stream,.        
+0000e710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e730: 2074 696d 656f 7574 3d74 696d 656f 7574   timeout=timeout
+0000e740: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e760: 2020 2020 2020 2020 2020 2062 6f64 793d             body=
+0000e770: 626f 6479 290a 2020 2020 2020 2020 656c  body).        el
+0000e780: 6966 206d 6574 686f 6420 3d3d 2022 5055  if method == "PU
+0000e790: 5422 3a0a 2020 2020 2020 2020 2020 2020  T":.            
+0000e7a0: 7265 7475 726e 2073 656c 662e 7265 7374  return self.rest
+0000e7b0: 5f63 6c69 656e 742e 5055 5428 7572 6c2c  _client.PUT(url,
+0000e7c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7e0: 2020 2020 2020 2020 2068 6561 6465 7273           headers
+0000e7f0: 3d68 6561 6465 7273 2c0a 2020 2020 2020  =headers,.      
+0000e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e820: 2020 6669 656c 6473 3d66 6965 6c64 732c    fields=fields,
+0000e830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e850: 2020 2020 2020 2020 2073 7472 6561 6d3d           stream=
+0000e860: 7374 7265 616d 2c0a 2020 2020 2020 2020  stream,.        
+0000e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e890: 7469 6d65 6f75 743d 7469 6d65 6f75 742c  timeout=timeout,
+0000e8a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8c0: 2020 2020 2020 2020 2062 6f64 793d 626f           body=bo
+0000e8d0: 6479 290a 2020 2020 2020 2020 656c 6966  dy).        elif
+0000e8e0: 206d 6574 686f 6420 3d3d 2022 5041 5443   method == "PATC
+0000e8f0: 4822 3a0a 2020 2020 2020 2020 2020 2020  H":.            
+0000e900: 7265 7475 726e 2073 656c 662e 7265 7374  return self.rest
+0000e910: 5f63 6c69 656e 742e 5041 5443 4828 7572  _client.PATCH(ur
+0000e920: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
+0000e930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e940: 2020 2020 2020 2020 2020 2020 2068 6561               hea
+0000e950: 6465 7273 3d68 6561 6465 7273 2c0a 2020  ders=headers,.  
+0000e960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e980: 2020 2020 2020 2020 6669 656c 6473 3d66          fields=f
+0000e990: 6965 6c64 732c 0a20 2020 2020 2020 2020  ields,.         
+0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9c0: 2073 7472 6561 6d3d 7374 7265 616d 2c0a   stream=stream,.
+0000e9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9f0: 2020 2020 2020 2020 2020 7469 6d65 6f75            timeou
+0000ea00: 743d 7469 6d65 6f75 742c 0a20 2020 2020  t=timeout,.     
+0000ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea30: 2020 2020 2062 6f64 793d 626f 6479 290a       body=body).
+0000ea40: 2020 2020 2020 2020 656c 6966 206d 6574          elif met
+0000ea50: 686f 6420 3d3d 2022 4445 4c45 5445 223a  hod == "DELETE":
+0000ea60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000ea70: 7572 6e20 7365 6c66 2e72 6573 745f 636c  urn self.rest_cl
+0000ea80: 6965 6e74 2e44 454c 4554 4528 7572 6c2c  ient.DELETE(url,
+0000ea90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eab0: 2020 2020 2020 2020 2020 2020 6865 6164              head
+0000eac0: 6572 733d 6865 6164 6572 732c 0a20 2020  ers=headers,.   
+0000ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eaf0: 2020 2020 2020 2020 7374 7265 616d 3d73          stream=s
+0000eb00: 7472 6561 6d2c 0a20 2020 2020 2020 2020  tream,.         
+0000eb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb30: 2020 7469 6d65 6f75 743d 7469 6d65 6f75    timeout=timeou
+0000eb40: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+0000eb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb60: 2020 2020 2020 2020 2020 2020 2020 626f                bo
+0000eb70: 6479 3d62 6f64 7929 0a20 2020 2020 2020  dy=body).       
+0000eb80: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000eb90: 2020 2072 6169 7365 2041 7069 5661 6c75     raise ApiValu
+0000eba0: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+0000ebb0: 2020 2020 2020 2020 2268 7474 7020 6d65          "http me
+0000ebc0: 7468 6f64 206d 7573 7420 6265 2060 4745  thod must be `GE
+0000ebd0: 5460 2c20 6048 4541 4460 2c20 604f 5054  T`, `HEAD`, `OPT
+0000ebe0: 494f 4e53 602c 220a 2020 2020 2020 2020  IONS`,".        
+0000ebf0: 2020 2020 2020 2020 2220 6050 4f53 5460          " `POST`
+0000ec00: 2c20 6050 4154 4348 602c 2060 5055 5460  , `PATCH`, `PUT`
+0000ec10: 206f 7220 6044 454c 4554 4560 2e22 0a20   or `DELETE`.". 
+0000ec20: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0000ec30: 2020 6465 6620 7570 6461 7465 5f70 6172    def update_par
+0000ec40: 616d 735f 666f 725f 6175 7468 280a 2020  ams_for_auth(.  
+0000ec50: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
+0000ec60: 2020 2020 2020 2020 2020 2020 6865 6164              head
+0000ec70: 6572 732c 0a20 2020 2020 2020 2020 2020  ers,.           
+0000ec80: 2061 7574 685f 7365 7474 696e 6773 2c0a   auth_settings,.
+0000ec90: 2020 2020 2020 2020 2020 2020 7265 736f              reso
+0000eca0: 7572 6365 5f70 6174 682c 0a20 2020 2020  urce_path,.     
+0000ecb0: 2020 2020 2020 206d 6574 686f 642c 0a20         method,. 
+0000ecc0: 2020 2020 2020 2020 2020 2062 6f64 792c             body,
+0000ecd0: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
+0000ece0: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
+0000ecf0: 6572 6174 6f72 3a20 5072 6566 6978 5365  erator: PrefixSe
+0000ed00: 7061 7261 746f 7249 7465 7261 746f 7220  paratorIterator 
+0000ed10: 3d20 4e6f 6e65 0a20 2020 2020 2020 2029  = None.        )
+0000ed20: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+0000ed30: 2022 2222 5570 6461 7465 7320 6865 6164   """Updates head
+0000ed40: 6572 2061 6e64 2071 7565 7279 2070 6172  er and query par
+0000ed50: 616d 7320 6261 7365 6420 6f6e 2061 7574  ams based on aut
+0000ed60: 6865 6e74 6963 6174 696f 6e20 7365 7474  hentication sett
+0000ed70: 696e 672e 0a0a 2020 2020 2020 2020 3a70  ing...        :p
+0000ed80: 6172 616d 2068 6561 6465 7273 3a20 4865  aram headers: He
+0000ed90: 6164 6572 2070 6172 616d 6574 6572 7320  ader parameters 
+0000eda0: 6469 6374 2074 6f20 6265 2075 7064 6174  dict to be updat
+0000edb0: 6564 2e0a 2020 2020 2020 2020 3a70 6172  ed..        :par
+0000edc0: 616d 2061 7574 685f 7365 7474 696e 6773  am auth_settings
+0000edd0: 3a20 4175 7468 656e 7469 6361 7469 6f6e  : Authentication
+0000ede0: 2073 6574 7469 6e67 2069 6465 6e74 6966   setting identif
+0000edf0: 6965 7273 206c 6973 742e 0a20 2020 2020  iers list..     
+0000ee00: 2020 203a 7061 7261 6d20 7265 736f 7572     :param resour
+0000ee10: 6365 5f70 6174 683a 2041 2073 7472 696e  ce_path: A strin
+0000ee20: 6720 7265 7072 6573 656e 7461 7469 6f6e  g representation
+0000ee30: 206f 6620 7468 6520 4854 5450 2072 6571   of the HTTP req
+0000ee40: 7565 7374 2072 6573 6f75 7263 6520 7061  uest resource pa
+0000ee50: 7468 2e0a 2020 2020 2020 2020 3a70 6172  th..        :par
+0000ee60: 616d 206d 6574 686f 643a 2041 2073 7472  am method: A str
+0000ee70: 696e 6720 7265 7072 6573 656e 7461 7469  ing representati
+0000ee80: 6f6e 206f 6620 7468 6520 4854 5450 2072  on of the HTTP r
+0000ee90: 6571 7565 7374 206d 6574 686f 642e 0a20  equest method.. 
+0000eea0: 2020 2020 2020 203a 7061 7261 6d20 626f         :param bo
+0000eeb0: 6479 3a20 4120 6f62 6a65 6374 2072 6570  dy: A object rep
+0000eec0: 7265 7365 6e74 696e 6720 7468 6520 626f  resenting the bo
+0000eed0: 6479 206f 6620 7468 6520 4854 5450 2072  dy of the HTTP r
+0000eee0: 6571 7565 7374 2e0a 2020 2020 2020 2020  equest..        
+0000eef0: 2020 2020 5468 6520 6f62 6a65 6374 2074      The object t
+0000ef00: 7970 6520 6973 2074 6865 2072 6574 7572  ype is the retur
+0000ef10: 6e20 7661 6c75 6520 6f66 205f 656e 636f  n value of _enco
+0000ef20: 6465 722e 6465 6661 756c 7428 292e 0a20  der.default().. 
+0000ef30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000ef40: 2020 2069 6620 6e6f 7420 6175 7468 5f73     if not auth_s
+0000ef50: 6574 7469 6e67 733a 0a20 2020 2020 2020  ettings:.       
+0000ef60: 2020 2020 2072 6574 7572 6e20 7265 736f       return reso
+0000ef70: 7572 6365 5f70 6174 680a 2020 2020 2020  urce_path.      
+0000ef80: 2020 6966 2070 7265 6669 785f 7365 7061    if prefix_sepa
+0000ef90: 7261 746f 725f 6974 6572 6174 6f72 2069  rator_iterator i
+0000efa0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0000efb0: 2020 2020 7072 6566 6978 5f73 6570 6172      prefix_separ
+0000efc0: 6174 6f72 5f69 7465 7261 746f 7220 3d20  ator_iterator = 
+0000efd0: 5072 6566 6978 5365 7061 7261 746f 7249  PrefixSeparatorI
+0000efe0: 7465 7261 746f 7228 223f 222c 2022 2622  terator("?", "&"
+0000eff0: 290a 0a20 2020 2020 2020 2066 6f72 2061  )..        for a
+0000f000: 7574 6820 696e 2061 7574 685f 7365 7474  uth in auth_sett
+0000f010: 696e 6773 3a0a 2020 2020 2020 2020 2020  ings:.          
+0000f020: 2020 6175 7468 5f73 6574 7469 6e67 203d    auth_setting =
+0000f030: 2073 656c 662e 636f 6e66 6967 7572 6174   self.configurat
+0000f040: 696f 6e2e 6175 7468 5f73 6574 7469 6e67  ion.auth_setting
+0000f050: 7328 292e 6765 7428 6175 7468 290a 2020  s().get(auth).  
+0000f060: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0000f070: 2061 7574 685f 7365 7474 696e 673a 0a20   auth_setting:. 
+0000f080: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000f090: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+0000f0a0: 2020 2020 6966 2061 7574 685f 7365 7474      if auth_sett
+0000f0b0: 696e 675b 2769 6e27 5d20 3d3d 2027 636f  ing['in'] == 'co
+0000f0c0: 6f6b 6965 273a 0a20 2020 2020 2020 2020  okie':.         
+0000f0d0: 2020 2020 2020 2068 6561 6465 7273 2e61         headers.a
+0000f0e0: 6464 2827 436f 6f6b 6965 272c 2061 7574  dd('Cookie', aut
+0000f0f0: 685f 7365 7474 696e 675b 2776 616c 7565  h_setting['value
+0000f100: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
+0000f110: 656c 6966 2061 7574 685f 7365 7474 696e  elif auth_settin
+0000f120: 675b 2769 6e27 5d20 3d3d 2027 6865 6164  g['in'] == 'head
+0000f130: 6572 273a 0a20 2020 2020 2020 2020 2020  er':.           
+0000f140: 2020 2020 2069 6620 6175 7468 5f73 6574       if auth_set
+0000f150: 7469 6e67 5b27 7479 7065 275d 2021 3d20  ting['type'] != 
+0000f160: 2768 7474 702d 7369 676e 6174 7572 6527  'http-signature'
+0000f170: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f180: 2020 2020 2020 6865 6164 6572 732e 6164        headers.ad
+0000f190: 6428 6175 7468 5f73 6574 7469 6e67 5b27  d(auth_setting['
+0000f1a0: 6b65 7927 5d2c 2061 7574 685f 7365 7474  key'], auth_sett
+0000f1b0: 696e 675b 2776 616c 7565 275d 290a 2020  ing['value']).  
+0000f1c0: 2020 2020 2020 2020 2020 656c 6966 2061            elif a
+0000f1d0: 7574 685f 7365 7474 696e 675b 2769 6e27  uth_setting['in'
+0000f1e0: 5d20 3d3d 2027 7175 6572 7927 3a0a 2020  ] == 'query':.  
+0000f1f0: 2020 2020 2020 2020 2020 2020 2020 2222                ""
+0000f200: 2220 544f 444f 2069 6d70 6c65 6d65 6e74  " TODO implement
+0000f210: 2061 7574 6820 696e 2071 7565 7279 0a20   auth in query. 
+0000f220: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000f230: 6565 6420 746f 2070 6173 7320 696e 2070  eed to pass in p
+0000f240: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
+0000f250: 6974 6572 6174 6f72 0a20 2020 2020 2020  iterator.       
+0000f260: 2020 2020 2020 2020 2061 6e64 206e 6565           and nee
+0000f270: 6420 746f 206f 7574 7075 7420 7265 736f  d to output reso
+0000f280: 7572 6365 5f70 6174 6820 7769 7468 2071  urce_path with q
+0000f290: 7565 7279 2070 6172 616d 7320 6164 6465  uery params adde
+0000f2a0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+0000f2b0: 2020 2222 220a 2020 2020 2020 2020 2020    """.          
+0000f2c0: 2020 2020 2020 7265 736f 7572 6365 5f70        resource_p
+0000f2d0: 6174 6820 2b3d 2050 6172 616d 6574 6572  ath += Parameter
+0000f2e0: 5365 7269 616c 697a 6572 4261 7365 2e5f  SerializerBase._
+0000f2f0: 7265 6636 3537 305f 6578 7061 6e73 696f  ref6570_expansio
+0000f300: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+0000f310: 2020 2020 2020 2076 6172 6961 626c 655f         variable_
+0000f320: 6e61 6d65 3d61 7574 685f 7365 7474 696e  name=auth_settin
+0000f330: 675b 276b 6579 275d 2c0a 2020 2020 2020  g['key'],.      
+0000f340: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000f350: 5f64 6174 613d 6175 7468 5f73 6574 7469  _data=auth_setti
+0000f360: 6e67 5b27 7661 6c75 6527 5d2c 0a20 2020  ng['value'],.   
+0000f370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f380: 2065 7870 6c6f 6465 3d46 616c 7365 2c0a   explode=False,.
+0000f390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3a0: 2020 2020 7065 7263 656e 745f 656e 636f      percent_enco
+0000f3b0: 6465 3d46 616c 7365 2c0a 2020 2020 2020  de=False,.      
+0000f3c0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000f3d0: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+0000f3e0: 7465 7261 746f 723d 7072 6566 6978 5f73  terator=prefix_s
+0000f3f0: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+0000f400: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+0000f410: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000f420: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000f430: 2020 2020 2020 7261 6973 6520 4170 6956        raise ApiV
+0000f440: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
+0000f450: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000f460: 4175 7468 656e 7469 6361 7469 6f6e 2074  Authentication t
+0000f470: 6f6b 656e 206d 7573 7420 6265 2069 6e20  oken must be in 
+0000f480: 6071 7565 7279 6020 6f72 2060 6865 6164  `query` or `head
+0000f490: 6572 6027 0a20 2020 2020 2020 2020 2020  er`'.           
+0000f4a0: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
+0000f4b0: 6574 7572 6e20 7265 736f 7572 6365 5f70  eturn resource_p
+0000f4c0: 6174 680a 0a0a 636c 6173 7320 4170 693a  ath...class Api:
+0000f4d0: 0a20 2020 2022 2222 4e4f 5445 3a0a 2020  .    """NOTE:.  
+0000f4e0: 2020 5468 6973 2063 6c61 7373 2069 7320    This class is 
+0000f4f0: 6175 746f 2067 656e 6572 6174 6564 2062  auto generated b
+0000f500: 7920 4b6f 6e66 6967 2028 6874 7470 733a  y Konfig (https:
+0000f510: 2f2f 6b6f 6e66 6967 7468 6973 2e63 6f6d  //konfigthis.com
+0000f520: 290a 2020 2020 2222 220a 0a20 2020 2064  ).    """..    d
+0000f530: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+0000f540: 2c20 6170 695f 636c 6965 6e74 3a20 7479  , api_client: ty
+0000f550: 7069 6e67 2e4f 7074 696f 6e61 6c5b 4170  ping.Optional[Ap
+0000f560: 6943 6c69 656e 745d 203d 204e 6f6e 6529  iClient] = None)
+0000f570: 3a0a 2020 2020 2020 2020 6966 2061 7069  :.        if api
+0000f580: 5f63 6c69 656e 7420 6973 204e 6f6e 653a  _client is None:
+0000f590: 0a20 2020 2020 2020 2020 2020 2061 7069  .            api
+0000f5a0: 5f63 6c69 656e 7420 3d20 4170 6943 6c69  _client = ApiCli
+0000f5b0: 656e 7428 290a 2020 2020 2020 2020 7365  ent().        se
+0000f5c0: 6c66 2e61 7069 5f63 6c69 656e 7420 3d20  lf.api_client = 
+0000f5d0: 6170 695f 636c 6965 6e74 0a0a 2020 2020  api_client..    
+0000f5e0: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+0000f5f0: 2020 6465 6620 5f76 6572 6966 795f 7479    def _verify_ty
+0000f600: 7065 645f 6469 6374 5f69 6e70 7574 735f  ped_dict_inputs_
+0000f610: 6f61 7067 2863 6c73 3a20 7479 7069 6e67  oapg(cls: typing
+0000f620: 2e54 7970 655b 7479 7069 6e67 5f65 7874  .Type[typing_ext
+0000f630: 656e 7369 6f6e 732e 5479 7065 6444 6963  ensions.TypedDic
+0000f640: 745d 2c20 6461 7461 3a20 7479 7069 6e67  t], data: typing
+0000f650: 2e44 6963 745b 7374 722c 2074 7970 696e  .Dict[str, typin
+0000f660: 672e 416e 795d 293a 0a20 2020 2020 2020  g.Any]):.       
+0000f670: 2022 2222 0a20 2020 2020 2020 2045 6e73   """.        Ens
+0000f680: 7572 6573 2074 6861 743a 0a20 2020 2020  ures that:.     
+0000f690: 2020 202d 2072 6571 7569 7265 6420 6b65     - required ke
+0000f6a0: 7973 2061 7265 2070 7265 7365 6e74 0a20  ys are present. 
+0000f6b0: 2020 2020 2020 202d 2061 6464 6974 696f         - additio
+0000f6c0: 6e61 6c20 7072 6f70 6572 7469 6573 2061  nal properties a
+0000f6d0: 7265 206e 6f74 2069 6e70 7574 0a20 2020  re not input.   
+0000f6e0: 2020 2020 202d 2076 616c 7565 2073 746f       - value sto
+0000f6f0: 7265 6420 756e 6465 7220 7265 7175 6972  red under requir
+0000f700: 6564 206b 6579 7320 646f 206e 6f74 2068  ed keys do not h
+0000f710: 6176 6520 7468 6520 7661 6c75 6520 756e  ave the value un
+0000f720: 7365 740a 2020 2020 2020 2020 4e6f 7465  set.        Note
+0000f730: 3a20 6465 7461 696c 6564 2076 616c 7565  : detailed value
+0000f740: 2063 6865 636b 696e 6720 6973 2064 6f6e   checking is don
+0000f750: 6520 696e 2073 6368 656d 6120 636c 6173  e in schema clas
+0000f760: 7365 730a 2020 2020 2020 2020 2222 220a  ses.        """.
+0000f770: 2020 2020 2020 2020 6d69 7373 696e 675f          missing_
+0000f780: 7265 7175 6972 6564 5f6b 6579 7320 3d20  required_keys = 
+0000f790: 5b5d 0a20 2020 2020 2020 2072 6571 7569  [].        requi
+0000f7a0: 7265 645f 6b65 7973 5f77 6974 685f 756e  red_keys_with_un
+0000f7b0: 7365 745f 7661 6c75 6573 203d 205b 5d0a  set_values = [].
+0000f7c0: 2020 2020 2020 2020 666f 7220 7265 7175          for requ
+0000f7d0: 6972 6564 5f6b 6579 2069 6e20 636c 732e  ired_key in cls.
+0000f7e0: 5f5f 7265 7175 6972 6564 5f6b 6579 735f  __required_keys_
+0000f7f0: 5f3a 0a20 2020 2020 2020 2020 2020 2069  _:.            i
+0000f800: 6620 7265 7175 6972 6564 5f6b 6579 206e  f required_key n
+0000f810: 6f74 2069 6e20 6461 7461 3a0a 2020 2020  ot in data:.    
+0000f820: 2020 2020 2020 2020 2020 2020 6d69 7373              miss
+0000f830: 696e 675f 7265 7175 6972 6564 5f6b 6579  ing_required_key
+0000f840: 732e 6170 7065 6e64 2872 6571 7569 7265  s.append(require
+0000f850: 645f 6b65 7929 0a20 2020 2020 2020 2020  d_key).         
+0000f860: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+0000f870: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+0000f880: 6520 3d20 6461 7461 5b72 6571 7569 7265  e = data[require
+0000f890: 645f 6b65 795d 0a20 2020 2020 2020 2020  d_key].         
+0000f8a0: 2020 2069 6620 7661 6c75 6520 6973 2075     if value is u
+0000f8b0: 6e73 6574 3a0a 2020 2020 2020 2020 2020  nset:.          
+0000f8c0: 2020 2020 2020 7265 7175 6972 6564 5f6b        required_k
+0000f8d0: 6579 735f 7769 7468 5f75 6e73 6574 5f76  eys_with_unset_v
+0000f8e0: 616c 7565 732e 6170 7065 6e64 2872 6571  alues.append(req
+0000f8f0: 7569 7265 645f 6b65 7929 0a20 2020 2020  uired_key).     
+0000f900: 2020 2069 6620 6d69 7373 696e 675f 7265     if missing_re
+0000f910: 7175 6972 6564 5f6b 6579 733a 0a20 2020  quired_keys:.   
+0000f920: 2020 2020 2020 2020 2072 6169 7365 2041           raise A
+0000f930: 7069 5479 7065 4572 726f 7228 0a20 2020  piTypeError(.   
+0000f940: 2020 2020 2020 2020 2020 2020 2027 7b7d               '{}
+0000f950: 206d 6973 7369 6e67 207b 7d20 7265 7175   missing {} requ
+0000f960: 6972 6564 2061 7267 756d 656e 7473 3a20  ired arguments: 
+0000f970: 7b7d 272e 666f 726d 6174 280a 2020 2020  {}'.format(.    
+0000f980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f990: 636c 732e 5f5f 6e61 6d65 5f5f 2c20 6c65  cls.__name__, le
+0000f9a0: 6e28 6d69 7373 696e 675f 7265 7175 6972  n(missing_requir
+0000f9b0: 6564 5f6b 6579 7329 2c20 6d69 7373 696e  ed_keys), missin
+0000f9c0: 675f 7265 7175 6972 6564 5f6b 6579 730a  g_required_keys.
+0000f9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9e0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000f9f0: 290a 2020 2020 2020 2020 6966 2072 6571  ).        if req
+0000fa00: 7569 7265 645f 6b65 7973 5f77 6974 685f  uired_keys_with_
+0000fa10: 756e 7365 745f 7661 6c75 6573 3a0a 2020  unset_values:.  
+0000fa20: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000fa30: 4170 6956 616c 7565 4572 726f 7228 0a20  ApiValueError(. 
+0000fa40: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000fa50: 7b7d 2063 6f6e 7461 696e 7320 696e 7661  {} contains inva
+0000fa60: 6c69 6420 756e 7365 7420 7661 6c75 6573  lid unset values
+0000fa70: 2066 6f72 207b 7d20 7265 7175 6972 6564   for {} required
+0000fa80: 206b 6579 733a 207b 7d27 2e66 6f72 6d61   keys: {}'.forma
+0000fa90: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+0000faa0: 2020 2020 2020 2063 6c73 2e5f 5f6e 616d         cls.__nam
+0000fab0: 655f 5f2c 206c 656e 2872 6571 7569 7265  e__, len(require
+0000fac0: 645f 6b65 7973 5f77 6974 685f 756e 7365  d_keys_with_unse
+0000fad0: 745f 7661 6c75 6573 292c 2072 6571 7569  t_values), requi
+0000fae0: 7265 645f 6b65 7973 5f77 6974 685f 756e  red_keys_with_un
+0000faf0: 7365 745f 7661 6c75 6573 0a20 2020 2020  set_values.     
+0000fb00: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000fb10: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000fb20: 2020 2020 6469 7361 6c6c 6f77 6564 5f61      disallowed_a
+0000fb30: 6464 6974 696f 6e61 6c5f 6b65 7973 203d  dditional_keys =
+0000fb40: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
+0000fb50: 6b65 7920 696e 2064 6174 613a 0a20 2020  key in data:.   
+0000fb60: 2020 2020 2020 2020 2069 6620 6b65 7920           if key 
+0000fb70: 696e 2063 6c73 2e5f 5f72 6571 7569 7265  in cls.__require
+0000fb80: 645f 6b65 7973 5f5f 206f 7220 6b65 7920  d_keys__ or key 
+0000fb90: 696e 2063 6c73 2e5f 5f6f 7074 696f 6e61  in cls.__optiona
+0000fba0: 6c5f 6b65 7973 5f5f 3a0a 2020 2020 2020  l_keys__:.      
+0000fbb0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+0000fbc0: 7565 0a20 2020 2020 2020 2020 2020 2064  ue.            d
+0000fbd0: 6973 616c 6c6f 7765 645f 6164 6469 7469  isallowed_additi
+0000fbe0: 6f6e 616c 5f6b 6579 732e 6170 7065 6e64  onal_keys.append
+0000fbf0: 286b 6579 290a 2020 2020 2020 2020 6966  (key).        if
+0000fc00: 2064 6973 616c 6c6f 7765 645f 6164 6469   disallowed_addi
+0000fc10: 7469 6f6e 616c 5f6b 6579 733a 0a20 2020  tional_keys:.   
+0000fc20: 2020 2020 2020 2020 2072 6169 7365 2041           raise A
+0000fc30: 7069 5479 7065 4572 726f 7228 0a20 2020  piTypeError(.   
+0000fc40: 2020 2020 2020 2020 2020 2020 2027 7b7d               '{}
+0000fc50: 2067 6f74 207b 7d20 756e 6578 7065 6374   got {} unexpect
+0000fc60: 6564 206b 6579 776f 7264 2061 7267 756d  ed keyword argum
+0000fc70: 656e 7473 3a20 7b7d 272e 666f 726d 6174  ents: {}'.format
+0000fc80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000fc90: 2020 2020 2020 636c 732e 5f5f 6e61 6d65        cls.__name
+0000fca0: 5f5f 2c20 6c65 6e28 6469 7361 6c6c 6f77  __, len(disallow
+0000fcb0: 6564 5f61 6464 6974 696f 6e61 6c5f 6b65  ed_additional_ke
+0000fcc0: 7973 292c 2064 6973 616c 6c6f 7765 645f  ys), disallowed_
+0000fcd0: 6164 6469 7469 6f6e 616c 5f6b 6579 730a  additional_keys.
+0000fce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcf0: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+0000fd00: 0a20 2020 2064 6566 205f 6765 745f 686f  .    def _get_ho
+0000fd10: 7374 5f6f 6170 6728 0a20 2020 2020 2020  st_oapg(.       
+0000fd20: 2073 656c 662c 0a20 2020 2020 2020 206f   self,.        o
+0000fd30: 7065 7261 7469 6f6e 5f69 643a 2073 7472  peration_id: str
+0000fd40: 2c0a 2020 2020 2020 2020 7365 7276 6572  ,.        server
+0000fd50: 733a 2074 7970 696e 672e 5475 706c 655b  s: typing.Tuple[
+0000fd60: 7479 7069 6e67 2e44 6963 745b 7374 722c  typing.Dict[str,
+0000fd70: 2073 7472 5d2c 202e 2e2e 5d20 3d20 7475   str], ...] = tu
+0000fd80: 706c 6528 292c 0a20 2020 2020 2020 2068  ple(),.        h
+0000fd90: 6f73 745f 696e 6465 783a 2074 7970 696e  ost_index: typin
+0000fda0: 672e 4f70 7469 6f6e 616c 5b69 6e74 5d20  g.Optional[int] 
+0000fdb0: 3d20 4e6f 6e65 0a20 2020 2029 202d 3e20  = None.    ) -> 
+0000fdc0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+0000fdd0: 7374 725d 3a0a 2020 2020 2020 2020 636f  str]:.        co
+0000fde0: 6e66 6967 7572 6174 696f 6e20 3d20 7365  nfiguration = se
+0000fdf0: 6c66 2e61 7069 5f63 6c69 656e 742e 636f  lf.api_client.co
+0000fe00: 6e66 6967 7572 6174 696f 6e0a 2020 2020  nfiguration.    
+0000fe10: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000fe20: 2020 2020 2069 6620 686f 7374 5f69 6e64       if host_ind
+0000fe30: 6578 2069 7320 4e6f 6e65 3a0a 2020 2020  ex is None:.    
+0000fe40: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+0000fe50: 7820 3d20 636f 6e66 6967 7572 6174 696f  x = configuratio
+0000fe60: 6e2e 7365 7276 6572 5f6f 7065 7261 7469  n.server_operati
+0000fe70: 6f6e 5f69 6e64 6578 2e67 6574 280a 2020  on_index.get(.  
+0000fe80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe90: 2020 6f70 6572 6174 696f 6e5f 6964 2c20    operation_id, 
+0000fea0: 636f 6e66 6967 7572 6174 696f 6e2e 7365  configuration.se
+0000feb0: 7276 6572 5f69 6e64 6578 0a20 2020 2020  rver_index.     
+0000fec0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000fed0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000fee0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000fef0: 6e64 6578 203d 2068 6f73 745f 696e 6465  ndex = host_inde
+0000ff00: 780a 2020 2020 2020 2020 2020 2020 7365  x.            se
+0000ff10: 7276 6572 5f76 6172 6961 626c 6573 203d  rver_variables =
+0000ff20: 2063 6f6e 6669 6775 7261 7469 6f6e 2e73   configuration.s
+0000ff30: 6572 7665 725f 6f70 6572 6174 696f 6e5f  erver_operation_
+0000ff40: 7661 7269 6162 6c65 732e 6765 7428 0a20  variables.get(. 
+0000ff50: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000ff60: 7065 7261 7469 6f6e 5f69 642c 2063 6f6e  peration_id, con
+0000ff70: 6669 6775 7261 7469 6f6e 2e73 6572 7665  figuration.serve
+0000ff80: 725f 7661 7269 6162 6c65 730a 2020 2020  r_variables.    
+0000ff90: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000ffa0: 2020 2020 2020 686f 7374 203d 2063 6f6e        host = con
+0000ffb0: 6669 6775 7261 7469 6f6e 2e67 6574 5f68  figuration.get_h
+0000ffc0: 6f73 745f 6672 6f6d 5f73 6574 7469 6e67  ost_from_setting
+0000ffd0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+0000ffe0: 2020 2069 6e64 6578 2c20 7661 7269 6162     index, variab
+0000fff0: 6c65 733d 7365 7276 6572 5f76 6172 6961  les=server_varia
+00010000: 626c 6573 2c20 7365 7276 6572 733d 7365  bles, servers=se
+00010010: 7276 6572 730a 2020 2020 2020 2020 2020  rvers.          
+00010020: 2020 290a 2020 2020 2020 2020 6578 6365    ).        exce
+00010030: 7074 2049 6e64 6578 4572 726f 723a 0a20  pt IndexError:. 
+00010040: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00010050: 7276 6572 733a 0a20 2020 2020 2020 2020  rvers:.         
+00010060: 2020 2020 2020 2072 6169 7365 2041 7069         raise Api
+00010070: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
+00010080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010090: 2249 6e76 616c 6964 2068 6f73 7420 696e  "Invalid host in
+000100a0: 6465 782e 204d 7573 7420 6265 2030 203c  dex. Must be 0 <
+000100b0: 3d20 696e 6465 7820 3c20 2573 2220 250a  = index < %s" %.
+000100c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100d0: 2020 2020 6c65 6e28 7365 7276 6572 7329      len(servers)
+000100e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000100f0: 2029 0a20 2020 2020 2020 2020 2020 2068   ).            h
+00010100: 6f73 7420 3d20 4e6f 6e65 0a20 2020 2020  ost = None.     
+00010110: 2020 2072 6574 7572 6e20 686f 7374 0a0a     return host..
+00010120: 0a63 6c61 7373 2053 6572 6961 6c69 7a65  .class Serialize
+00010130: 6452 6571 7565 7374 426f 6479 2874 7970  dRequestBody(typ
+00010140: 696e 675f 6578 7465 6e73 696f 6e73 2e54  ing_extensions.T
+00010150: 7970 6564 4469 6374 2c20 746f 7461 6c3d  ypedDict, total=
+00010160: 4661 6c73 6529 3a0a 2020 2020 626f 6479  False):.    body
+00010170: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b73  : typing.Union[s
+00010180: 7472 2c20 6279 7465 735d 0a20 2020 2066  tr, bytes].    f
+00010190: 6965 6c64 733a 2074 7970 696e 672e 5475  ields: typing.Tu
+000101a0: 706c 655b 7479 7069 6e67 2e55 6e69 6f6e  ple[typing.Union
+000101b0: 5b52 6571 7565 7374 4669 656c 642c 2074  [RequestField, t
+000101c0: 7970 696e 672e 5475 706c 655b 7374 722c  yping.Tuple[str,
+000101d0: 2073 7472 5d5d 2c20 2e2e 2e5d 0a0a 0a63   str]], ...]...c
+000101e0: 6c61 7373 2052 6571 7565 7374 426f 6479  lass RequestBody
+000101f0: 2853 7479 6c65 466f 726d 5365 7269 616c  (StyleFormSerial
+00010200: 697a 6572 2c20 4a53 4f4e 4465 7465 6374  izer, JSONDetect
+00010210: 6f72 293a 0a20 2020 2022 2222 0a20 2020  or):.    """.   
+00010220: 2041 2072 6571 7565 7374 2062 6f64 7920   A request body 
+00010230: 7061 7261 6d65 7465 720a 2020 2020 636f  parameter.    co
+00010240: 6e74 656e 743a 2063 6f6e 7465 6e74 5f74  ntent: content_t
+00010250: 7970 6520 746f 204d 6564 6961 5479 7065  ype to MediaType
+00010260: 2053 6368 656d 6120 696e 666f 0a20 2020   Schema info.   
+00010270: 2022 2222 0a20 2020 205f 5f6a 736f 6e5f   """.    __json_
+00010280: 656e 636f 6465 7220 3d20 4a53 4f4e 456e  encoder = JSONEn
+00010290: 636f 6465 7228 290a 0a20 2020 2064 6566  coder()..    def
+000102a0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+000102b0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+000102c0: 2063 6f6e 7465 6e74 3a20 7479 7069 6e67   content: typing
+000102d0: 2e44 6963 745b 7374 722c 204d 6564 6961  .Dict[str, Media
+000102e0: 5479 7065 5d2c 0a20 2020 2020 2020 2072  Type],.        r
+000102f0: 6571 7569 7265 643a 2062 6f6f 6c20 3d20  equired: bool = 
+00010300: 4661 6c73 652c 0a20 2020 2029 3a0a 2020  False,.    ):.  
+00010310: 2020 2020 2020 7365 6c66 2e72 6571 7569        self.requi
+00010320: 7265 6420 3d20 7265 7175 6972 6564 0a20  red = required. 
+00010330: 2020 2020 2020 2069 6620 6c65 6e28 636f         if len(co
+00010340: 6e74 656e 7429 203d 3d20 303a 0a20 2020  ntent) == 0:.   
+00010350: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00010360: 616c 7565 4572 726f 7228 2749 6e76 616c  alueError('Inval
+00010370: 6964 2076 616c 7565 2066 6f72 2063 6f6e  id value for con
+00010380: 7465 6e74 2c20 7468 6520 636f 6e74 656e  tent, the conten
+00010390: 7420 6469 6374 206d 7573 7420 6861 7665  t dict must have
+000103a0: 203e 3d20 3120 656e 7472 7927 290a 2020   >= 1 entry').  
+000103b0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
+000103c0: 6e74 203d 2063 6f6e 7465 6e74 0a0a 2020  nt = content..  
+000103d0: 2020 6465 6620 5f5f 7365 7269 616c 697a    def __serializ
+000103e0: 655f 6a73 6f6e 280a 2020 2020 2020 2020  e_json(.        
+000103f0: 7365 6c66 2c0a 2020 2020 2020 2020 696e  self,.        in
+00010400: 5f64 6174 613a 2074 7970 696e 672e 416e  _data: typing.An
+00010410: 790a 2020 2020 2920 2d3e 2074 7970 696e  y.    ) -> typin
+00010420: 672e 4469 6374 5b73 7472 2c20 6279 7465  g.Dict[str, byte
+00010430: 735d 3a0a 2020 2020 2020 2020 696e 5f64  s]:.        in_d
+00010440: 6174 6120 3d20 7365 6c66 2e5f 5f6a 736f  ata = self.__jso
+00010450: 6e5f 656e 636f 6465 722e 6465 6661 756c  n_encoder.defaul
+00010460: 7428 696e 5f64 6174 6129 0a20 2020 2020  t(in_data).     
+00010470: 2020 206a 736f 6e5f 7374 7220 3d20 6a73     json_str = js
+00010480: 6f6e 2e64 756d 7073 2869 6e5f 6461 7461  on.dumps(in_data
+00010490: 2c20 7365 7061 7261 746f 7273 3d28 222c  , separators=(",
+000104a0: 222c 2022 3a22 292c 2065 6e73 7572 655f  ", ":"), ensure_
+000104b0: 6173 6369 693d 4661 6c73 6529 2e65 6e63  ascii=False).enc
+000104c0: 6f64 6528 0a20 2020 2020 2020 2020 2020  ode(.           
+000104d0: 2022 7574 662d 3822 0a20 2020 2020 2020   "utf-8".       
+000104e0: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
+000104f0: 6e20 6469 6374 2862 6f64 793d 6a73 6f6e  n dict(body=json
+00010500: 5f73 7472 290a 0a20 2020 2040 7374 6174  _str)..    @stat
+00010510: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+00010520: 205f 5f73 6572 6961 6c69 7a65 5f74 6578   __serialize_tex
+00010530: 745f 706c 6169 6e28 696e 5f64 6174 613a  t_plain(in_data:
+00010540: 2074 7970 696e 672e 416e 7929 202d 3e20   typing.Any) -> 
+00010550: 7479 7069 6e67 2e44 6963 745b 7374 722c  typing.Dict[str,
+00010560: 2073 7472 5d3a 0a20 2020 2020 2020 2069   str]:.        i
+00010570: 6620 6973 696e 7374 616e 6365 2869 6e5f  f isinstance(in_
+00010580: 6461 7461 2c20 6672 6f7a 656e 6469 6374  data, frozendict
+00010590: 2e66 726f 7a65 6e64 6963 7429 3a0a 2020  .frozendict):.  
+000105a0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000105b0: 5661 6c75 6545 7272 6f72 2827 556e 6162  ValueError('Unab
+000105c0: 6c65 2074 6f20 7365 7269 616c 697a 6520  le to serialize 
+000105d0: 7479 7065 2066 726f 7a65 6e64 6963 742e  type frozendict.
+000105e0: 6672 6f7a 656e 6469 6374 2074 6f20 7465  frozendict to te
+000105f0: 7874 2f70 6c61 696e 2729 0a20 2020 2020  xt/plain').     
+00010600: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+00010610: 6365 2869 6e5f 6461 7461 2c20 7475 706c  ce(in_data, tupl
+00010620: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00010630: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00010640: 2827 556e 6162 6c65 2074 6f20 7365 7269  ('Unable to seri
+00010650: 616c 697a 6520 7479 7065 2074 7570 6c65  alize type tuple
+00010660: 2074 6f20 7465 7874 2f70 6c61 696e 2729   to text/plain')
+00010670: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
+00010680: 696e 7374 616e 6365 2869 6e5f 6461 7461  instance(in_data
+00010690: 2c20 4e6f 6e65 436c 6173 7329 3a0a 2020  , NoneClass):.  
+000106a0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000106b0: 5661 6c75 6545 7272 6f72 2827 556e 6162  ValueError('Unab
+000106c0: 6c65 2074 6f20 7365 7269 616c 697a 6520  le to serialize 
+000106d0: 7479 7065 204e 6f6e 6543 6c61 7373 2074  type NoneClass t
+000106e0: 6f20 7465 7874 2f70 6c61 696e 2729 0a20  o text/plain'). 
+000106f0: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+00010700: 7374 616e 6365 2869 6e5f 6461 7461 2c20  stance(in_data, 
+00010710: 426f 6f6c 436c 6173 7329 3a0a 2020 2020  BoolClass):.    
+00010720: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00010730: 6c75 6545 7272 6f72 2827 556e 6162 6c65  lueError('Unable
+00010740: 2074 6f20 7365 7269 616c 697a 6520 7479   to serialize ty
+00010750: 7065 2042 6f6f 6c43 6c61 7373 2074 6f20  pe BoolClass to 
+00010760: 7465 7874 2f70 6c61 696e 2729 0a20 2020  text/plain').   
+00010770: 2020 2020 2072 6574 7572 6e20 6469 6374       return dict
+00010780: 2862 6f64 793d 7374 7228 696e 5f64 6174  (body=str(in_dat
+00010790: 6129 290a 0a20 2020 2064 6566 205f 5f6d  a))..    def __m
+000107a0: 756c 7469 7061 7274 5f6a 736f 6e5f 6974  ultipart_json_it
+000107b0: 656d 2873 656c 662c 206b 6579 3a20 7374  em(self, key: st
+000107c0: 722c 2076 616c 7565 3a20 5363 6865 6d61  r, value: Schema
+000107d0: 2920 2d3e 2052 6571 7565 7374 4669 656c  ) -> RequestFiel
+000107e0: 643a 0a20 2020 2020 2020 206a 736f 6e5f  d:.        json_
+000107f0: 7661 6c75 6520 3d20 7365 6c66 2e5f 5f6a  value = self.__j
+00010800: 736f 6e5f 656e 636f 6465 722e 6465 6661  son_encoder.defa
+00010810: 756c 7428 7661 6c75 6529 0a20 2020 2020  ult(value).     
+00010820: 2020 2072 6574 7572 6e20 5265 7175 6573     return Reques
+00010830: 7446 6965 6c64 286e 616d 653d 6b65 792c  tField(name=key,
+00010840: 2064 6174 613d 6a73 6f6e 2e64 756d 7073   data=json.dumps
+00010850: 286a 736f 6e5f 7661 6c75 6529 2c20 6865  (json_value), he
+00010860: 6164 6572 733d 7b27 436f 6e74 656e 742d  aders={'Content-
+00010870: 5479 7065 273a 2027 6170 706c 6963 6174  Type': 'applicat
+00010880: 696f 6e2f 6a73 6f6e 277d 290a 0a20 2020  ion/json'})..   
+00010890: 2064 6566 205f 5f6d 756c 7469 7061 7274   def __multipart
+000108a0: 5f66 6f72 6d5f 6974 656d 2873 656c 662c  _form_item(self,
+000108b0: 206b 6579 3a20 7374 722c 2076 616c 7565   key: str, value
+000108c0: 3a20 5363 6865 6d61 2920 2d3e 2052 6571  : Schema) -> Req
+000108d0: 7565 7374 4669 656c 643a 0a20 2020 2020  uestField:.     
+000108e0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+000108f0: 2876 616c 7565 2c20 7374 7229 3a0a 2020  (value, str):.  
+00010900: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00010910: 2052 6571 7565 7374 4669 656c 6428 6e61   RequestField(na
+00010920: 6d65 3d6b 6579 2c20 6461 7461 3d73 7472  me=key, data=str
+00010930: 2876 616c 7565 292c 2068 6561 6465 7273  (value), headers
+00010940: 3d7b 2743 6f6e 7465 6e74 2d54 7970 6527  ={'Content-Type'
+00010950: 3a20 2774 6578 742f 706c 6169 6e27 7d29  : 'text/plain'})
+00010960: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
+00010970: 696e 7374 616e 6365 2876 616c 7565 2c20  instance(value, 
+00010980: 6279 7465 7329 3a0a 2020 2020 2020 2020  bytes):.        
+00010990: 2020 2020 7265 7475 726e 2052 6571 7565      return Reque
+000109a0: 7374 4669 656c 6428 6e61 6d65 3d6b 6579  stField(name=key
+000109b0: 2c20 6461 7461 3d76 616c 7565 2c20 6865  , data=value, he
+000109c0: 6164 6572 733d 7b27 436f 6e74 656e 742d  aders={'Content-
+000109d0: 5479 7065 273a 2027 6170 706c 6963 6174  Type': 'applicat
+000109e0: 696f 6e2f 6f63 7465 742d 7374 7265 616d  ion/octet-stream
+000109f0: 277d 290a 2020 2020 2020 2020 656c 6966  '}).        elif
+00010a00: 2069 7369 6e73 7461 6e63 6528 7661 6c75   isinstance(valu
+00010a10: 652c 2046 696c 6549 4f29 3a0a 2020 2020  e, FileIO):.    
+00010a20: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
+00010a30: 203d 206f 732e 7061 7468 2e62 6173 656e   = os.path.basen
+00010a40: 616d 6528 7661 6c75 652e 6e61 6d65 290a  ame(value.name).
+00010a50: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+00010a60: 6573 745f 6669 656c 6420 3d20 5265 7175  est_field = Requ
+00010a70: 6573 7446 6965 6c64 280a 2020 2020 2020  estField(.      
+00010a80: 2020 2020 2020 2020 2020 6e61 6d65 3d6b            name=k
+00010a90: 6579 2c0a 2020 2020 2020 2020 2020 2020  ey,.            
+00010aa0: 2020 2020 6461 7461 3d76 616c 7565 2e72      data=value.r
+00010ab0: 6561 6428 292c 0a20 2020 2020 2020 2020  ead(),.         
+00010ac0: 2020 2020 2020 2066 696c 656e 616d 653d         filename=
+00010ad0: 6669 6c65 6e61 6d65 2c0a 2020 2020 2020  filename,.      
+00010ae0: 2020 2020 2020 2020 2020 6865 6164 6572            header
+00010af0: 733d 7b27 436f 6e74 656e 742d 5479 7065  s={'Content-Type
+00010b00: 273a 2067 7565 7373 5f63 6f6e 7465 6e74  ': guess_content
+00010b10: 5f74 7970 6528 6669 6c65 6e61 6d65 297d  _type(filename)}
+00010b20: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00010b30: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00010b40: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
+00010b50: 2020 2020 2072 6574 7572 6e20 7265 7175       return requ
+00010b60: 6573 745f 6669 656c 640a 2020 2020 2020  est_field.      
+00010b70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00010b80: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00010b90: 5f5f 6d75 6c74 6970 6172 745f 6a73 6f6e  __multipart_json
+00010ba0: 5f69 7465 6d28 6b65 793d 6b65 792c 2076  _item(key=key, v
+00010bb0: 616c 7565 3d76 616c 7565 290a 0a20 2020  alue=value)..   
+00010bc0: 2064 6566 205f 5f73 6572 6961 6c69 7a65   def __serialize
+00010bd0: 5f6d 756c 7469 7061 7274 5f66 6f72 6d5f  _multipart_form_
+00010be0: 6461 7461 280a 2020 2020 2020 2020 7365  data(.        se
+00010bf0: 6c66 2c20 696e 5f64 6174 613a 2053 6368  lf, in_data: Sch
+00010c00: 656d 610a 2020 2020 2920 2d3e 2074 7970  ema.    ) -> typ
+00010c10: 696e 672e 4469 6374 5b73 7472 2c20 7479  ing.Dict[str, ty
+00010c20: 7069 6e67 2e54 7570 6c65 5b52 6571 7565  ping.Tuple[Reque
+00010c30: 7374 4669 656c 642c 202e 2e2e 5d5d 3a0a  stField, ...]]:.
+00010c40: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+00010c50: 7369 6e73 7461 6e63 6528 696e 5f64 6174  sinstance(in_dat
+00010c60: 612c 2066 726f 7a65 6e64 6963 742e 6672  a, frozendict.fr
+00010c70: 6f7a 656e 6469 6374 293a 0a20 2020 2020  ozendict):.     
+00010c80: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00010c90: 7565 4572 726f 7228 6627 556e 6162 6c65  ueError(f'Unable
+00010ca0: 2074 6f20 7365 7269 616c 697a 6520 7b69   to serialize {i
+00010cb0: 6e5f 6461 7461 7d20 746f 206d 756c 7469  n_data} to multi
+00010cc0: 7061 7274 2f66 6f72 6d2d 6461 7461 2062  part/form-data b
+00010cd0: 6563 6175 7365 2069 7420 6973 206e 6f74  ecause it is not
+00010ce0: 2061 2064 6963 7420 6f66 2064 6174 6127   a dict of data'
+00010cf0: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
+00010d00: 2020 2020 2020 496e 2061 206d 756c 7469        In a multi
+00010d10: 7061 7274 2f66 6f72 6d2d 6461 7461 2072  part/form-data r
+00010d20: 6571 7565 7374 2062 6f64 792c 2065 6163  equest body, eac
+00010d30: 6820 7363 6865 6d61 2070 726f 7065 7274  h schema propert
+00010d40: 792c 206f 7220 6561 6368 2065 6c65 6d65  y, or each eleme
+00010d50: 6e74 206f 6620 6120 7363 6865 6d61 2061  nt of a schema a
+00010d60: 7272 6179 2070 726f 7065 7274 792c 0a20  rray property,. 
+00010d70: 2020 2020 2020 2074 616b 6573 2061 2073         takes a s
+00010d80: 6563 7469 6f6e 2069 6e20 7468 6520 7061  ection in the pa
+00010d90: 796c 6f61 6420 7769 7468 2061 6e20 696e  yload with an in
+00010da0: 7465 726e 616c 2068 6561 6465 7220 6173  ternal header as
+00010db0: 2064 6566 696e 6564 2062 7920 5246 4337   defined by RFC7
+00010dc0: 3537 382e 2054 6865 2073 6572 6961 6c69  578. The seriali
+00010dd0: 7a61 7469 6f6e 2073 7472 6174 6567 790a  zation strategy.
+00010de0: 2020 2020 2020 2020 666f 7220 6561 6368          for each
+00010df0: 2070 726f 7065 7274 7920 6f66 2061 206d   property of a m
+00010e00: 756c 7469 7061 7274 2f66 6f72 6d2d 6461  ultipart/form-da
+00010e10: 7461 2072 6571 7565 7374 2062 6f64 7920  ta request body 
+00010e20: 6361 6e20 6265 2073 7065 6369 6669 6564  can be specified
+00010e30: 2069 6e20 616e 2061 7373 6f63 6961 7465   in an associate
+00010e40: 6420 456e 636f 6469 6e67 204f 626a 6563  d Encoding Objec
+00010e50: 742e 0a0a 2020 2020 2020 2020 5768 656e  t...        When
+00010e60: 2070 6173 7369 6e67 2069 6e20 6d75 6c74   passing in mult
+00010e70: 6970 6172 7420 7479 7065 732c 2062 6f75  ipart types, bou
+00010e80: 6e64 6172 6965 7320 4d41 5920 6265 2075  ndaries MAY be u
+00010e90: 7365 6420 746f 2073 6570 6172 6174 6520  sed to separate 
+00010ea0: 7365 6374 696f 6e73 206f 6620 7468 6520  sections of the 
+00010eb0: 636f 6e74 656e 7420 6265 696e 670a 2020  content being.  
+00010ec0: 2020 2020 2020 7472 616e 7366 6572 7265        transferre
+00010ed0: 6420 e280 9320 7468 7573 2c20 7468 6520  d ... thus, the 
+00010ee0: 666f 6c6c 6f77 696e 6720 6465 6661 756c  following defaul
+00010ef0: 7420 436f 6e74 656e 742d 5479 7065 7320  t Content-Types 
+00010f00: 6172 6520 6465 6669 6e65 6420 666f 7220  are defined for 
+00010f10: 6d75 6c74 6970 6172 743a 0a0a 2020 2020  multipart:..    
+00010f20: 2020 2020 4966 2074 6865 2028 6f62 6a65      If the (obje
+00010f30: 6374 2920 7072 6f70 6572 7479 2069 7320  ct) property is 
+00010f40: 6120 7072 696d 6974 6976 652c 206f 7220  a primitive, or 
+00010f50: 616e 2061 7272 6179 206f 6620 7072 696d  an array of prim
+00010f60: 6974 6976 6520 7661 6c75 6573 2c20 7468  itive values, th
+00010f70: 6520 6465 6661 756c 7420 436f 6e74 656e  e default Conten
+00010f80: 742d 5479 7065 2069 7320 7465 7874 2f70  t-Type is text/p
+00010f90: 6c61 696e 0a20 2020 2020 2020 2049 6620  lain.        If 
+00010fa0: 7468 6520 7072 6f70 6572 7479 2069 7320  the property is 
+00010fb0: 636f 6d70 6c65 782c 206f 7220 616e 2061  complex, or an a
+00010fc0: 7272 6179 206f 6620 636f 6d70 6c65 7820  rray of complex 
+00010fd0: 7661 6c75 6573 2c20 7468 6520 6465 6661  values, the defa
+00010fe0: 756c 7420 436f 6e74 656e 742d 5479 7065  ult Content-Type
+00010ff0: 2069 7320 6170 706c 6963 6174 696f 6e2f   is application/
+00011000: 6a73 6f6e 0a20 2020 2020 2020 2020 2020  json.           
+00011010: 2051 7565 7374 696f 6e3a 2068 6f77 2069   Question: how i
+00011020: 7320 7468 6520 6172 7261 7920 6f66 2070  s the array of p
+00011030: 7269 6d69 7469 7665 7320 656e 636f 6465  rimitives encode
+00011040: 643f 0a20 2020 2020 2020 2049 6620 7468  d?.        If th
+00011050: 6520 7072 6f70 6572 7479 2069 7320 6120  e property is a 
+00011060: 7479 7065 3a20 7374 7269 6e67 2077 6974  type: string wit
+00011070: 6820 6120 636f 6e74 656e 7445 6e63 6f64  h a contentEncod
+00011080: 696e 672c 2074 6865 2064 6566 6175 6c74  ing, the default
+00011090: 2043 6f6e 7465 6e74 2d54 7970 6520 6973   Content-Type is
+000110a0: 2061 7070 6c69 6361 7469 6f6e 2f6f 6374   application/oct
+000110b0: 6574 2d73 7472 6561 6d0a 2020 2020 2020  et-stream.      
+000110c0: 2020 2222 220a 2020 2020 2020 2020 6669    """.        fi
+000110d0: 656c 6473 3a20 7479 7069 6e67 2e4c 6973  elds: typing.Lis
+000110e0: 745b 5265 7175 6573 7446 6965 6c64 5d20  t[RequestField] 
+000110f0: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
+00011100: 206b 6579 2c20 7661 6c75 6520 696e 2069   key, value in i
+00011110: 6e5f 6461 7461 2e69 7465 6d73 2829 3a0a  n_data.items():.
+00011120: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00011130: 7369 6e73 7461 6e63 6528 7661 6c75 652c  sinstance(value,
+00011140: 2074 7570 6c65 293a 0a20 2020 2020 2020   tuple):.       
+00011150: 2020 2020 2020 2020 2069 6620 7661 6c75           if valu
+00011160: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00011170: 2020 2020 2020 2023 2076 616c 7565 7320         # values 
+00011180: 7573 6520 6578 706c 6f64 6520 3d20 5472  use explode = Tr
+00011190: 7565 2c20 736f 2074 6865 2063 6f64 6520  ue, so the code 
+000111a0: 6d61 6b65 7320 6120 5265 7175 6573 7446  makes a RequestF
+000111b0: 6965 6c64 2066 6f72 2065 6163 6820 6974  ield for each it
+000111c0: 656d 2077 6974 6820 6e61 6d65 3d6b 6579  em with name=key
+000111d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000111e0: 2020 2020 2066 6f72 2069 7465 6d20 696e       for item in
+000111f0: 2076 616c 7565 3a0a 2020 2020 2020 2020   value:.        
+00011200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011210: 7265 7175 6573 745f 6669 656c 6420 3d20  request_field = 
+00011220: 7365 6c66 2e5f 5f6d 756c 7469 7061 7274  self.__multipart
+00011230: 5f66 6f72 6d5f 6974 656d 286b 6579 3d6b  _form_item(key=k
+00011240: 6579 2c20 7661 6c75 653d 6974 656d 290a  ey, value=item).
+00011250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011260: 2020 2020 2020 2020 6669 656c 6473 2e61          fields.a
+00011270: 7070 656e 6428 7265 7175 6573 745f 6669  ppend(request_fi
+00011280: 656c 6429 0a20 2020 2020 2020 2020 2020  eld).           
+00011290: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000112a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000112b0: 2073 656e 6420 616e 2065 6d70 7479 2061   send an empty a
+000112c0: 7272 6179 2061 7320 6a73 6f6e 2062 6563  rray as json bec
+000112d0: 6175 7365 2065 7870 6c6f 6469 6e67 2077  ause exploding w
+000112e0: 696c 6c20 6e6f 7420 7365 6e64 2069 740a  ill not send it.
+000112f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011300: 2020 2020 7265 7175 6573 745f 6669 656c      request_fiel
+00011310: 6420 3d20 7365 6c66 2e5f 5f6d 756c 7469  d = self.__multi
+00011320: 7061 7274 5f6a 736f 6e5f 6974 656d 286b  part_json_item(k
+00011330: 6579 3d6b 6579 2c20 7661 6c75 653d 7661  ey=key, value=va
+00011340: 6c75 6529 0a20 2020 2020 2020 2020 2020  lue).           
+00011350: 2020 2020 2020 2020 2066 6965 6c64 732e           fields.
+00011360: 6170 7065 6e64 2872 6571 7565 7374 5f66  append(request_f
+00011370: 6965 6c64 290a 2020 2020 2020 2020 2020  ield).          
+00011380: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00011390: 2020 2020 2020 2020 7265 7175 6573 745f          request_
+000113a0: 6669 656c 6420 3d20 7365 6c66 2e5f 5f6d  field = self.__m
+000113b0: 756c 7469 7061 7274 5f66 6f72 6d5f 6974  ultipart_form_it
+000113c0: 656d 286b 6579 3d6b 6579 2c20 7661 6c75  em(key=key, valu
+000113d0: 653d 7661 6c75 6529 0a20 2020 2020 2020  e=value).       
+000113e0: 2020 2020 2020 2020 2066 6965 6c64 732e           fields.
+000113f0: 6170 7065 6e64 2872 6571 7565 7374 5f66  append(request_f
+00011400: 6965 6c64 290a 0a20 2020 2020 2020 2023  ield)..        #
+00011410: 2054 6869 7320 6973 206e 6563 6573 7361   This is necessa
+00011420: 7279 2074 6f20 6669 6c6c 2074 6865 2022  ry to fill the "
+00011430: 436f 6e74 656e 742d 4469 7370 6f73 6974  Content-Disposit
+00011440: 696f 6e22 2068 6561 6465 7220 6e65 6564  ion" header need
+00011450: 6564 2066 6f72 206e 616d 696e 6720 6669  ed for naming fi
+00011460: 656c 6473 2069 6e20 6d75 6c74 6970 6172  elds in multipar
+00011470: 740a 2020 2020 2020 2020 666f 7220 6669  t.        for fi
+00011480: 656c 6420 696e 2066 6965 6c64 733a 0a20  eld in fields:. 
+00011490: 2020 2020 2020 2020 2020 2066 6965 6c64             field
+000114a0: 2e6d 616b 655f 6d75 6c74 6970 6172 7428  .make_multipart(
+000114b0: 636f 6e74 656e 745f 7479 7065 3d66 6965  content_type=fie
+000114c0: 6c64 2e68 6561 6465 7273 5b22 436f 6e74  ld.headers["Cont
+000114d0: 656e 742d 5479 7065 225d 290a 2020 2020  ent-Type"]).    
+000114e0: 2020 2020 7265 7475 726e 2064 6963 7428      return dict(
+000114f0: 6669 656c 6473 3d74 7570 6c65 2866 6965  fields=tuple(fie
+00011500: 6c64 7329 290a 0a20 2020 2064 6566 205f  lds))..    def _
+00011510: 5f73 6572 6961 6c69 7a65 5f61 7070 6c69  _serialize_appli
+00011520: 6361 7469 6f6e 5f6f 6374 6574 5f73 7472  cation_octet_str
+00011530: 6561 6d28 7365 6c66 2c20 696e 5f64 6174  eam(self, in_dat
+00011540: 613a 2042 696e 6172 7953 6368 656d 6129  a: BinarySchema)
+00011550: 202d 3e20 7479 7069 6e67 2e44 6963 745b   -> typing.Dict[
+00011560: 7374 722c 2062 7974 6573 5d3a 0a20 2020  str, bytes]:.   
+00011570: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00011580: 6365 2869 6e5f 6461 7461 2c20 6279 7465  ce(in_data, byte
+00011590: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+000115a0: 7265 7475 726e 2064 6963 7428 626f 6479  return dict(body
+000115b0: 3d69 6e5f 6461 7461 290a 2020 2020 2020  =in_data).      
+000115c0: 2020 2320 4669 6c65 494f 2074 7970 650a    # FileIO type.
+000115d0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+000115e0: 2064 6963 7428 626f 6479 3d69 6e5f 6461   dict(body=in_da
+000115f0: 7461 2e72 6561 6428 2929 0a20 2020 2020  ta.read()).     
+00011600: 2020 2069 6e5f 6461 7461 2e63 6c6f 7365     in_data.close
+00011610: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+00011620: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00011630: 6620 5f5f 7365 7269 616c 697a 655f 6170  f __serialize_ap
+00011640: 706c 6963 6174 696f 6e5f 785f 7777 775f  plication_x_www_
+00011650: 666f 726d 5f64 6174 6128 0a20 2020 2020  form_data(.     
+00011660: 2020 2073 656c 662c 2069 6e5f 6461 7461     self, in_data
+00011670: 3a20 7479 7069 6e67 2e41 6e79 0a20 2020  : typing.Any.   
+00011680: 2029 202d 3e20 5365 7269 616c 697a 6564   ) -> Serialized
+00011690: 5265 7175 6573 7442 6f64 793a 0a20 2020  RequestBody:.   
+000116a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000116b0: 2050 4f53 5420 7375 626d 6973 7369 6f6e   POST submission
+000116c0: 206f 6620 666f 726d 2064 6174 6120 696e   of form data in
+000116d0: 2062 6f64 790a 2020 2020 2020 2020 2222   body.        ""
+000116e0: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
+000116f0: 2069 7369 6e73 7461 6e63 6528 696e 5f64   isinstance(in_d
+00011700: 6174 612c 2066 726f 7a65 6e64 6963 742e  ata, frozendict.
+00011710: 6672 6f7a 656e 6469 6374 293a 0a20 2020  frozendict):.   
+00011720: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00011730: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
+00011740: 2020 2020 2020 2020 2020 2066 2755 6e61             f'Una
+00011750: 626c 6520 746f 2073 6572 6961 6c69 7a65  ble to serialize
+00011760: 207b 696e 5f64 6174 617d 2074 6f20 6170   {in_data} to ap
+00011770: 706c 6963 6174 696f 6e2f 782d 7777 772d  plication/x-www-
+00011780: 666f 726d 2d75 726c 656e 636f 6465 6420  form-urlencoded 
+00011790: 6265 6361 7573 6520 6974 2069 7320 6e6f  because it is no
+000117a0: 7420 6120 6469 6374 206f 6620 6461 7461  t a dict of data
+000117b0: 2729 0a20 2020 2020 2020 2063 6173 745f  ').        cast_
+000117c0: 696e 5f64 6174 6120 3d20 7365 6c66 2e5f  in_data = self._
+000117d0: 5f6a 736f 6e5f 656e 636f 6465 722e 6465  _json_encoder.de
+000117e0: 6661 756c 7428 696e 5f64 6174 6129 0a20  fault(in_data). 
+000117f0: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
+00011800: 656c 662e 5f73 6572 6961 6c69 7a65 5f66  elf._serialize_f
+00011810: 6f72 6d28 6361 7374 5f69 6e5f 6461 7461  orm(cast_in_data
+00011820: 2c20 6e61 6d65 3d27 272c 2065 7870 6c6f  , name='', explo
+00011830: 6465 3d54 7275 652c 2070 6572 6365 6e74  de=True, percent
+00011840: 5f65 6e63 6f64 653d 5472 7565 290a 2020  _encode=True).  
+00011850: 2020 2020 2020 7265 7475 726e 2064 6963        return dic
+00011860: 7428 626f 6479 3d76 616c 7565 290a 0a20  t(body=value).. 
+00011870: 2020 2064 6566 2073 6572 6961 6c69 7a65     def serialize
+00011880: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+00011890: 696e 5f64 6174 613a 2074 7970 696e 672e  in_data: typing.
+000118a0: 416e 792c 2063 6f6e 7465 6e74 5f74 7970  Any, content_typ
+000118b0: 653a 2073 7472 0a20 2020 2029 202d 3e20  e: str.    ) -> 
+000118c0: 5365 7269 616c 697a 6564 5265 7175 6573  SerializedReques
+000118d0: 7442 6f64 793a 0a20 2020 2020 2020 2022  tBody:.        "
+000118e0: 2222 0a20 2020 2020 2020 2049 6620 6120  "".        If a 
+000118f0: 7374 7220 6973 2072 6574 7572 6e65 6420  str is returned 
+00011900: 7468 656e 2074 6865 2072 6573 756c 7420  then the result 
+00011910: 7769 6c6c 2062 6520 6173 7369 676e 6564  will be assigned
+00011920: 2074 6f20 6461 7461 2077 6865 6e20 6d61   to data when ma
+00011930: 6b69 6e67 2074 6865 2072 6571 7565 7374  king the request
+00011940: 0a20 2020 2020 2020 2049 6620 6120 7475  .        If a tu
+00011950: 706c 6520 6973 2072 6574 7572 6e65 6420  ple is returned 
+00011960: 7468 656e 2074 6865 2072 6573 756c 7420  then the result 
+00011970: 7769 6c6c 2062 6520 7573 6564 2061 7320  will be used as 
+00011980: 6669 656c 6473 2069 6e70 7574 2069 6e20  fields input in 
+00011990: 656e 636f 6465 5f6d 756c 7469 7061 7274  encode_multipart
+000119a0: 5f66 6f72 6d64 6174 610a 2020 2020 2020  _formdata.      
+000119b0: 2020 5265 7475 726e 2061 2074 7570 6c65    Return a tuple
+000119c0: 206f 660a 0a20 2020 2020 2020 2054 6865   of..        The
+000119d0: 206b 6579 206f 6620 7468 6520 7265 7475   key of the retu
+000119e0: 726e 2064 6963 7420 6973 0a20 2020 2020  rn dict is.     
+000119f0: 2020 202d 2062 6f64 7920 666f 7220 6170     - body for ap
+00011a00: 706c 6963 6174 696f 6e2f 6a73 6f6e 0a20  plication/json. 
+00011a10: 2020 2020 2020 202d 2065 6e63 6f64 655f         - encode_
+00011a20: 6d75 6c74 6970 6172 7420 616e 6420 6669  multipart and fi
+00011a30: 656c 6473 2066 6f72 206d 756c 7469 7061  elds for multipa
+00011a40: 7274 2f66 6f72 6d2d 6461 7461 0a20 2020  rt/form-data.   
+00011a50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00011a60: 206d 6564 6961 5f74 7970 6520 3d20 7365   media_type = se
+00011a70: 6c66 2e63 6f6e 7465 6e74 5b63 6f6e 7465  lf.content[conte
+00011a80: 6e74 5f74 7970 655d 0a20 2020 2020 2020  nt_type].       
+00011a90: 2069 6620 6973 696e 7374 616e 6365 2869   if isinstance(i
+00011aa0: 6e5f 6461 7461 2c20 6d65 6469 615f 7479  n_data, media_ty
+00011ab0: 7065 2e73 6368 656d 6129 3a0a 2020 2020  pe.schema):.    
+00011ac0: 2020 2020 2020 2020 6361 7374 5f69 6e5f          cast_in_
+00011ad0: 6461 7461 203d 2069 6e5f 6461 7461 0a20  data = in_data. 
+00011ae0: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+00011af0: 7374 616e 6365 2869 6e5f 6461 7461 2c20  stance(in_data, 
+00011b00: 2864 6963 742c 2066 726f 7a65 6e64 6963  (dict, frozendic
+00011b10: 742e 6672 6f7a 656e 6469 6374 2929 2061  t.frozendict)) a
+00011b20: 6e64 2069 6e5f 6461 7461 3a0a 2020 2020  nd in_data:.    
+00011b30: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00011b40: 2020 2020 2020 2020 2020 2020 2063 6173               cas
+00011b50: 745f 696e 5f64 6174 6120 3d20 6d65 6469  t_in_data = medi
+00011b60: 615f 7479 7065 2e73 6368 656d 6128 2a2a  a_type.schema(**
+00011b70: 696e 5f64 6174 6129 0a20 2020 2020 2020  in_data).       
+00011b80: 2020 2020 2065 7863 6570 7420 5479 7065       except Type
+00011b90: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
+00011ba0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00011bb0: 6520 4d69 7373 696e 6752 6571 7569 7265  e MissingRequire
+00011bc0: 6450 6172 616d 6574 6572 7345 7272 6f72  dParametersError
+00011bd0: 2865 290a 2020 2020 2020 2020 656c 7365  (e).        else
+00011be0: 3a0a 2020 2020 2020 2020 2020 2020 6361  :.            ca
+00011bf0: 7374 5f69 6e5f 6461 7461 203d 206d 6564  st_in_data = med
+00011c00: 6961 5f74 7970 652e 7363 6865 6d61 2869  ia_type.schema(i
+00011c10: 6e5f 6461 7461 290a 2020 2020 2020 2020  n_data).        
+00011c20: 2320 544f 444f 2063 6865 636b 2066 6f72  # TODO check for
+00011c30: 2061 6e64 2075 7365 2065 6e63 6f64 696e   and use encodin
+00011c40: 6720 6966 2069 7420 6578 6973 7473 0a20  g if it exists. 
+00011c50: 2020 2020 2020 2023 2061 6e64 2063 6f6e         # and con
+00011c60: 7465 6e74 5f74 7970 6520 6973 206d 756c  tent_type is mul
+00011c70: 7469 7061 7274 206f 7220 6170 706c 6963  tipart or applic
+00011c80: 6174 696f 6e2f 782d 7777 772d 666f 726d  ation/x-www-form
+00011c90: 2d75 726c 656e 636f 6465 640a 2020 2020  -urlencoded.    
+00011ca0: 2020 2020 6966 2073 656c 662e 5f63 6f6e      if self._con
+00011cb0: 7465 6e74 5f74 7970 655f 6973 5f6a 736f  tent_type_is_jso
+00011cc0: 6e28 636f 6e74 656e 745f 7479 7065 293a  n(content_type):
+00011cd0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00011ce0: 7572 6e20 7365 6c66 2e5f 5f73 6572 6961  urn self.__seria
+00011cf0: 6c69 7a65 5f6a 736f 6e28 6361 7374 5f69  lize_json(cast_i
+00011d00: 6e5f 6461 7461 290a 2020 2020 2020 2020  n_data).        
+00011d10: 656c 6966 2063 6f6e 7465 6e74 5f74 7970  elif content_typ
+00011d20: 6520 3d3d 2027 7465 7874 2f70 6c61 696e  e == 'text/plain
+00011d30: 273a 0a20 2020 2020 2020 2020 2020 2072  ':.            r
+00011d40: 6574 7572 6e20 7365 6c66 2e5f 5f73 6572  eturn self.__ser
+00011d50: 6961 6c69 7a65 5f74 6578 745f 706c 6169  ialize_text_plai
+00011d60: 6e28 6361 7374 5f69 6e5f 6461 7461 290a  n(cast_in_data).
+00011d70: 2020 2020 2020 2020 656c 6966 2063 6f6e          elif con
+00011d80: 7465 6e74 5f74 7970 6520 3d3d 2027 6d75  tent_type == 'mu
+00011d90: 6c74 6970 6172 742f 666f 726d 2d64 6174  ltipart/form-dat
+00011da0: 6127 3a0a 2020 2020 2020 2020 2020 2020  a':.            
+00011db0: 7265 7475 726e 2073 656c 662e 5f5f 7365  return self.__se
+00011dc0: 7269 616c 697a 655f 6d75 6c74 6970 6172  rialize_multipar
+00011dd0: 745f 666f 726d 5f64 6174 6128 6361 7374  t_form_data(cast
+00011de0: 5f69 6e5f 6461 7461 290a 2020 2020 2020  _in_data).      
+00011df0: 2020 656c 6966 2063 6f6e 7465 6e74 5f74    elif content_t
+00011e00: 7970 6520 3d3d 2027 6170 706c 6963 6174  ype == 'applicat
+00011e10: 696f 6e2f 782d 7777 772d 666f 726d 2d75  ion/x-www-form-u
+00011e20: 726c 656e 636f 6465 6427 3a0a 2020 2020  rlencoded':.    
+00011e30: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00011e40: 656c 662e 5f5f 7365 7269 616c 697a 655f  elf.__serialize_
+00011e50: 6170 706c 6963 6174 696f 6e5f 785f 7777  application_x_ww
+00011e60: 775f 666f 726d 5f64 6174 6128 6361 7374  w_form_data(cast
+00011e70: 5f69 6e5f 6461 7461 290a 2020 2020 2020  _in_data).      
+00011e80: 2020 656c 6966 2063 6f6e 7465 6e74 5f74    elif content_t
+00011e90: 7970 6520 3d3d 2027 6170 706c 6963 6174  ype == 'applicat
+00011ea0: 696f 6e2f 6f63 7465 742d 7374 7265 616d  ion/octet-stream
+00011eb0: 273a 0a20 2020 2020 2020 2020 2020 2072  ':.            r
+00011ec0: 6574 7572 6e20 7365 6c66 2e5f 5f73 6572  eturn self.__ser
+00011ed0: 6961 6c69 7a65 5f61 7070 6c69 6361 7469  ialize_applicati
+00011ee0: 6f6e 5f6f 6374 6574 5f73 7472 6561 6d28  on_octet_stream(
+00011ef0: 6361 7374 5f69 6e5f 6461 7461 290a 2020  cast_in_data).  
+00011f00: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
+00011f10: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
+00011f20: 2753 6572 6961 6c69 7a61 7469 6f6e 2068  'Serialization h
+00011f30: 6173 206e 6f74 2079 6574 2062 6565 6e20  as not yet been 
+00011f40: 696d 706c 656d 656e 7465 6420 666f 7220  implemented for 
+00011f50: 7b7d 272e 666f 726d 6174 2863 6f6e 7465  {}'.format(conte
+00011f60: 6e74 5f74 7970 6529 290a                 nt_type)).
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/apis/path_to_api.py` & `splitit_web_python_sdk-2.2.0/splitit_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/apis/tags/installment_plan_api.py` & `splitit_web_python_sdk-2.2.0/splitit_client/apis/tags/installment_plan_api.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/configuration.py` & `splitit_web_python_sdk-2.2.0/splitit_client/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,32 +86,34 @@
     :Example:
     """
 
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
-                 client_id=None, client_secret=None,
+                 client_id=None, client_secret=None, token_url: typing.Optional[str] = None,
                  username=None, password=None,
                  discard_unknown_keys=False,
                  disabled_client_side_validations="",
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ):
         """Constructor
         """
-        self.host = "https://web-api-v3.sandbox.splitit.com" if host is None else host
+        self.host = "https://web-api-v3.production.splitit.com" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
         if client_id is not None and client_secret is not None:
             self.oauth = OAuth(client_id=client_id, client_secret=client_secret)
+        if token_url is not None and self.oauth is not None:
+            self.oauth.token_url = token_url
         """OAuth2 Client Credentials
         """
         self.server_variables = server_variables or {}
         self.server_operation_variables = server_operation_variables or {}
         """Default server variables
         """
         self.temp_folder_path = None
@@ -396,25 +398,25 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 2.1.0".\
+               "SDK Package Version: 2.2.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "https://web-api-v3.sandbox.splitit.com",
+                'url': "https://web-api-v3.production.splitit.com",
                 'description': "No description provided",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
@@ -460,40 +462,41 @@
         return self.get_host_from_settings(self.server_index, variables=self.server_variables)
 
     @host.setter
     def host(self, value):
         """Fix base path."""
         self._base_path = check_url(value)
         self.server_index = None
-        
+
 def check_url(url: str):
     parsed = urlparse(url)
-    if parsed.query is not '':
+    if parsed.query != '':
         raise InvalidHostConfigurationError(url, "query string is not allowed")
-    if parsed.fragment is not '':
+    if parsed.fragment != '':
         raise InvalidHostConfigurationError(url, "fragment is not allowed")
     if parsed.scheme not in ["http", "https"]:
         raise InvalidHostConfigurationError(url, 'scheme must be "http" or "https"'.format(parsed.scheme))
     if not validators.url(url):
         raise InvalidHostConfigurationError(url, "invalid url")
     if (url.endswith("/")):
         return url[:-1]
     return url
 
 class OAuth:
-    def __init__(self, client_id: typing.AnyStr, client_secret: typing.AnyStr) -> None:
+    def __init__(self, client_id: typing.AnyStr, client_secret: typing.AnyStr, token_url: str = "https://id.production.splitit.com/connect/token") -> None:
         self._client_id = client_id
         self._client_secret = client_secret
+        self.token_url = token_url
         self.access_token = None
-    
+
     def refresh_access_token(self) -> None:
         self.access_token = self.retrieve_access_token()
-    
+
     def retrieve_access_token(self) -> typing.AnyStr:
-        request = urllib.request.Request("https://id.sandbox.splitit.com/connect/token")
+        request = urllib.request.Request(self.token_url)
         request.add_header("Content-Type", "application/x-www-form-urlencoded")
         params = {
                 "grant_type": "client_credentials",
                 "client_id": self._client_id,
                 "client_secret": self._client_secret
         }
         data = urllib.parse.urlencode(params).encode("utf-8")
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/exceptions.py` & `splitit_web_python_sdk-2.2.0/splitit_client/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
 
 import typing
-from splitit_client.api_response import ApiResponse
+from splitit_client.api_response import ApiResponse, AsyncApiResponse
 from splitit_client.exceptions_base import OpenApiException, ApiTypeError, ApiValueError, render_path
 
 class ClientConfigurationError(OpenApiException):
     def __init__(self, msg):
         super(ClientConfigurationError, self).__init__(msg)
 
 
@@ -53,20 +53,20 @@
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
 class ApiException(OpenApiException):
 
-    def __init__(self, status=None, reason=None, api_response: ApiResponse = None):
+    def __init__(self, status=None, reason=None, api_response: typing.Optional[typing.Union[ApiResponse, AsyncApiResponse]] = None):
         if api_response:
             self.status = api_response.status
             self.reason = api_response.response.reason
             self.body = api_response.body
-            self.headers = api_response.response.getheaders()
+            self.headers = api_response.response.headers
             self.round_trip_time = api_response.round_trip_time
         else:
             self.status = status
             self.reason = reason
             self.body = None
             self.headers = None
             self.round_trip_time = None
@@ -81,22 +81,45 @@
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
 
+class AnyOfValidationError(OpenApiException):
+    def __init__(self, error_list: typing.List[typing.Union[ApiTypeError, ApiValueError]]):
+        self.error_list = error_list
+        sub_msgs: typing.List[str] = []
+        for type_error in error_list:
+            sub_msgs.append(str(type_error))
+        num_validation_errors = len(self.error_list)
+        if num_validation_errors == 1:
+            super().__init__(sub_msgs[0])
+        else:
+            # create a string that says how many validation errors there were and
+            # prints each sub_msg out using a bulleted list of messages
+            msg = "{} validation error{} detected: \n".format(num_validation_errors, "s" if num_validation_errors > 1 else "")
+            for i, sub_msg in enumerate(sub_msgs):
+                msg += " {}. {}\n".format(i+1, sub_msg)
+            super().__init__(msg)
+
+
 class InvalidHostConfigurationError(ClientConfigurationError):
     def __init__(self, host: str, reason: str):
         self.host = host
         self.reason = reason
         super().__init__('Invalid host: "{}", {}'.format(self.host, self.reason))
 
 
-class MissingRequiredParametersError(TypeError):
+class MissingRequiredPropertiesError(ApiTypeError):
+    def __init__(self, msg: str):
+        super().__init__(msg)
+
+
+class MissingRequiredParametersError(ApiTypeError):
     def __init__(self, error: TypeError):
         self.error = error
         error_str = str(error)
         self.msg = error_str
         if "__new__()" in error_str:
             # parse error to reformat
             missing_parameters = error_str.split(":")[1].strip()
@@ -122,26 +145,35 @@
                              True if it is a key in a dict
                              False if our item is an item in a list
                              None if unset
         """
         self.validation_errors = validation_errors
         self.type_errors: typing.List[ApiTypeError] = []
         self.value_errors: typing.List[ApiValueError] = []
+        self.missing_required_properties_errors: typing.List[MissingRequiredPropertiesError] = []
         for error in validation_errors:
             if isinstance(error, ApiTypeError):
                 self.type_errors.append(error)
             elif isinstance(error, ApiValueError):
                 self.value_errors.append(error)
+            elif isinstance(error, MissingRequiredPropertiesError):
+                self.missing_required_properties_errors.append(error)
         sub_msgs: typing.List[str] = []
+        if len(self.missing_required_properties_errors) > 0:
+            for error in self.missing_required_properties_errors:
+                sub_msgs.append(str(error))
         if len(self.type_errors) > 0:
             for type_error in self.type_errors:
-                classes = ", ".join([cls.__name__ for cls in type_error.valid_classes])
-                msg = 'Got {}({}) for required type {} at {}'.format(
-                    type(type_error.invalid_value).__name__, type_error.invalid_value, classes, render_path(type_error.path_to_item))
-                sub_msgs.append(msg)
+                if isinstance(type_error, MissingRequiredPropertiesError) or isinstance(type_error, MissingRequiredParametersError):
+                    sub_msgs.append(str(type_error))
+                else:
+                    classes = ", ".join([cls.__name__ for cls in type_error.valid_classes])
+                    msg = 'Got {}({}) for required type {} at {}'.format(
+                        type(type_error.invalid_value).__name__, type_error.invalid_value, classes, render_path(type_error.path_to_item))
+                    sub_msgs.append(msg)
         if len(self.value_errors) > 0:
             for value_error in self.value_errors:
                 sub_msgs.append(value_error.full_msg)
         sub_msg = ". ".join(sub_msgs)
         num_validation_errors = len(self.validation_errors)
         self.msg = "{} invalid argument{}. {}".format(num_validation_errors, "s" if num_validation_errors > 1 else "", sub_msg)
         super().__init__(self.msg)
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/exceptions_base.py` & `splitit_web_python_sdk-2.2.0/splitit_client/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/address_data.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/address_data.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/address_data_model.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/address_data_model.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/authorization_model.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/authorization_model.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/card_brand.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/card_brand.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/card_data.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/card_data.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/card_type.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/card_type.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/check_installments_eligibility_request.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/check_installments_eligibility_request.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/error.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/error.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/error_extended.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/error_extended.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/failed_response.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/failed_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/gw_authorization_status.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/gw_authorization_status.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/identifier_contract.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/identifier_contract.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/initiate_plan_response.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/initiate_plan_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/initiate_redirection_endpoints_model.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/initiate_redirection_endpoints_model.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/installment.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/installment.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_cancel_response.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_cancel_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_create_request.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_create_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,23 +57,28 @@
             @staticmethod
             def PaymentMethod() -> typing.Type['PaymentMethodModel']:
                 return PaymentMethodModel
         
             @staticmethod
             def RedirectUrls() -> typing.Type['RedirectionEndpointsModel']:
                 return RedirectionEndpointsModel
+        
+            @staticmethod
+            def EventsEndpoints() -> typing.Type['EventsEndpointsModel']:
+                return EventsEndpointsModel
             __annotations__ = {
                 "AutoCapture": AutoCapture,
                 "TermsAndConditionsAccepted": TermsAndConditionsAccepted,
                 "Attempt3dSecure": Attempt3dSecure,
                 "Shopper": Shopper,
                 "PlanData": PlanData,
                 "BillingAddress": BillingAddress,
                 "PaymentMethod": PaymentMethod,
                 "RedirectUrls": RedirectUrls,
+                "EventsEndpoints": EventsEndpoints,
             }
     
     TermsAndConditionsAccepted: MetaOapg.properties.TermsAndConditionsAccepted
     AutoCapture: MetaOapg.properties.AutoCapture
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["AutoCapture"]) -> MetaOapg.properties.AutoCapture: ...
@@ -96,17 +101,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["PaymentMethod"]) -> 'PaymentMethodModel': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["RedirectUrls"]) -> 'RedirectionEndpointsModel': ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["EventsEndpoints"]) -> 'EventsEndpointsModel': ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "TermsAndConditionsAccepted", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "PaymentMethod", "RedirectUrls", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "TermsAndConditionsAccepted", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "PaymentMethod", "RedirectUrls", "EventsEndpoints", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["AutoCapture"]) -> MetaOapg.properties.AutoCapture: ...
     
@@ -128,47 +136,53 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["PaymentMethod"]) -> typing.Union['PaymentMethodModel', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["RedirectUrls"]) -> typing.Union['RedirectionEndpointsModel', schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["EventsEndpoints"]) -> typing.Union['EventsEndpointsModel', schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "TermsAndConditionsAccepted", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "PaymentMethod", "RedirectUrls", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "TermsAndConditionsAccepted", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "PaymentMethod", "RedirectUrls", "EventsEndpoints", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         TermsAndConditionsAccepted: typing.Union[MetaOapg.properties.TermsAndConditionsAccepted, bool, ],
         AutoCapture: typing.Union[MetaOapg.properties.AutoCapture, bool, ],
         Attempt3dSecure: typing.Union[MetaOapg.properties.Attempt3dSecure, bool, schemas.Unset] = schemas.unset,
         Shopper: typing.Union['ShopperData', schemas.Unset] = schemas.unset,
         PlanData: typing.Union['PlanDataModel', schemas.Unset] = schemas.unset,
         BillingAddress: typing.Union['AddressDataModel', schemas.Unset] = schemas.unset,
         PaymentMethod: typing.Union['PaymentMethodModel', schemas.Unset] = schemas.unset,
         RedirectUrls: typing.Union['RedirectionEndpointsModel', schemas.Unset] = schemas.unset,
+        EventsEndpoints: typing.Union['EventsEndpointsModel', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'InstallmentPlanCreateRequest':
         return super().__new__(
             cls,
             *args,
             TermsAndConditionsAccepted=TermsAndConditionsAccepted,
             AutoCapture=AutoCapture,
             Attempt3dSecure=Attempt3dSecure,
             Shopper=Shopper,
             PlanData=PlanData,
             BillingAddress=BillingAddress,
             PaymentMethod=PaymentMethod,
             RedirectUrls=RedirectUrls,
+            EventsEndpoints=EventsEndpoints,
             _configuration=_configuration,
             **kwargs,
         )
 
 from splitit_client.model.address_data_model import AddressDataModel
+from splitit_client.model.events_endpoints_model import EventsEndpointsModel
 from splitit_client.model.payment_method_model import PaymentMethodModel
 from splitit_client.model.plan_data_model import PlanDataModel
 from splitit_client.model.redirection_endpoints_model import RedirectionEndpointsModel
 from splitit_client.model.shopper_data import ShopperData
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_create_response.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_create_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_get_response.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_get_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_initiate_request.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_initiate_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,22 +55,27 @@
             @staticmethod
             def RedirectUrls() -> typing.Type['InitiateRedirectionEndpointsModel']:
                 return InitiateRedirectionEndpointsModel
         
             @staticmethod
             def UxSettings() -> typing.Type['UxSettingsModel']:
                 return UxSettingsModel
+        
+            @staticmethod
+            def EventsEndpoints() -> typing.Type['EventsEndpointsModel']:
+                return EventsEndpointsModel
             __annotations__ = {
                 "AutoCapture": AutoCapture,
                 "Attempt3dSecure": Attempt3dSecure,
                 "Shopper": Shopper,
                 "PlanData": PlanData,
                 "BillingAddress": BillingAddress,
                 "RedirectUrls": RedirectUrls,
                 "UxSettings": UxSettings,
+                "EventsEndpoints": EventsEndpoints,
             }
     
     AutoCapture: MetaOapg.properties.AutoCapture
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["AutoCapture"]) -> MetaOapg.properties.AutoCapture: ...
     
@@ -89,17 +94,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["RedirectUrls"]) -> 'InitiateRedirectionEndpointsModel': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["UxSettings"]) -> 'UxSettingsModel': ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["EventsEndpoints"]) -> 'EventsEndpointsModel': ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", "UxSettings", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", "UxSettings", "EventsEndpoints", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["AutoCapture"]) -> MetaOapg.properties.AutoCapture: ...
     
@@ -118,45 +126,51 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["RedirectUrls"]) -> typing.Union['InitiateRedirectionEndpointsModel', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["UxSettings"]) -> typing.Union['UxSettingsModel', schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["EventsEndpoints"]) -> typing.Union['EventsEndpointsModel', schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", "UxSettings", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["AutoCapture", "Attempt3dSecure", "Shopper", "PlanData", "BillingAddress", "RedirectUrls", "UxSettings", "EventsEndpoints", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         AutoCapture: typing.Union[MetaOapg.properties.AutoCapture, bool, ],
         Attempt3dSecure: typing.Union[MetaOapg.properties.Attempt3dSecure, bool, schemas.Unset] = schemas.unset,
         Shopper: typing.Union['ShopperData', schemas.Unset] = schemas.unset,
         PlanData: typing.Union['PlanDataModel', schemas.Unset] = schemas.unset,
         BillingAddress: typing.Union['AddressDataModel', schemas.Unset] = schemas.unset,
         RedirectUrls: typing.Union['InitiateRedirectionEndpointsModel', schemas.Unset] = schemas.unset,
         UxSettings: typing.Union['UxSettingsModel', schemas.Unset] = schemas.unset,
+        EventsEndpoints: typing.Union['EventsEndpointsModel', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'InstallmentPlanInitiateRequest':
         return super().__new__(
             cls,
             *args,
             AutoCapture=AutoCapture,
             Attempt3dSecure=Attempt3dSecure,
             Shopper=Shopper,
             PlanData=PlanData,
             BillingAddress=BillingAddress,
             RedirectUrls=RedirectUrls,
             UxSettings=UxSettings,
+            EventsEndpoints=EventsEndpoints,
             _configuration=_configuration,
             **kwargs,
         )
 
 from splitit_client.model.address_data_model import AddressDataModel
+from splitit_client.model.events_endpoints_model import EventsEndpointsModel
 from splitit_client.model.initiate_redirection_endpoints_model import InitiateRedirectionEndpointsModel
 from splitit_client.model.plan_data_model import PlanDataModel
 from splitit_client.model.shopper_data import ShopperData
 from splitit_client.model.ux_settings_model import UxSettingsModel
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_refund_request.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_refund_request.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_refund_response.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_refund_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_search_response.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_search_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_update_request.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_request.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_update_request_by_identifier.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_request_by_identifier.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_plan_update_response.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_plan_update_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/installment_status.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/installment_status.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/installments_eligibility_response.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/installments_eligibility_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/links_data.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/links_data.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/links_model.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/links_model.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/payment_method_model.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/payment_method_model.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/payment_method_type.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/payment_plan_option_model.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/payment_plan_option_model.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/plan_data.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/plan_data.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/plan_data_model.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/plan_data_model.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/plan_error_response.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/plan_error_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/plan_status.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/plan_status.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/purchase_method.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/purchase_method.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/redirection_endpoints_model.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/redirection_endpoints_model.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/refund_model.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/refund_model.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/refund_status.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/refund_status.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/refund_strategy.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/refund_strategy.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/refund_summary.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/refund_summary.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/search_installment_plan_response_item.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/search_installment_plan_response_item.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/shipping_status.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/shipping_status.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/shipping_status2.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/shipping_status2.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/shopper_data.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/shopper_data.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/test_modes.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/test_modes.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/three_ds_redirect_data_v3.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/three_ds_redirect_data_v3.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/update_order_request.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/update_order_request.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/ux_settings_model.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/ux_settings_model.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/model/verify_authorization_response.py` & `splitit_web_python_sdk-2.2.0/splitit_client/model/verify_authorization_response.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/models/__init__.py` & `splitit_web_python_sdk-2.2.0/splitit_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from splitit_client.model.authorization_model import AuthorizationModel
 from splitit_client.model.card_brand import CardBrand
 from splitit_client.model.card_data import CardData
 from splitit_client.model.card_type import CardType
 from splitit_client.model.check_installments_eligibility_request import CheckInstallmentsEligibilityRequest
 from splitit_client.model.error import Error
 from splitit_client.model.error_extended import ErrorExtended
+from splitit_client.model.events_endpoints_model import EventsEndpointsModel
 from splitit_client.model.failed_response import FailedResponse
 from splitit_client.model.gw_authorization_status import GwAuthorizationStatus
 from splitit_client.model.identifier_contract import IdentifierContract
 from splitit_client.model.initiate_plan_response import InitiatePlanResponse
 from splitit_client.model.initiate_redirection_endpoints_model import InitiateRedirectionEndpointsModel
 from splitit_client.model.installment import Installment
 from splitit_client.model.installment_plan_cancel_response import InstallmentPlanCancelResponse
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/paths/__init__.py` & `splitit_web_python_sdk-2.2.0/splitit_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans/post.py` & `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,106 +11,101 @@
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
 import json
 from urllib3._collections import HTTPHeaderDict
 
+from splitit_client.api_response import AsyncGeneratorResponse
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
-from splitit_client.model.installment_plan_create_request import InstallmentPlanCreateRequest
-from splitit_client.model.failed_response import FailedResponse
-from splitit_client.model.plan_error_response import PlanErrorResponse
-from splitit_client.model.installment_plan_create_response import InstallmentPlanCreateResponse
+from splitit_client.model.failed_response import FailedResponse as FailedResponseSchema
+from splitit_client.model.refund_strategy import RefundStrategy as RefundStrategySchema
+from splitit_client.model.installment_plan_refund_response import InstallmentPlanRefundResponse as InstallmentPlanRefundResponseSchema
+from splitit_client.model.installment_plan_refund_request import InstallmentPlanRefundRequest as InstallmentPlanRefundRequestSchema
+
+from splitit_client.type.failed_response import FailedResponse
+from splitit_client.type.installment_plan_refund_response import InstallmentPlanRefundResponse
+from splitit_client.type.refund_strategy import RefundStrategy
+from splitit_client.type.installment_plan_refund_request import InstallmentPlanRefundRequest
 
 from . import path
 
 # Header params
-
-
-class XSplititTestModeSchema(
-    schemas.EnumBase,
-    schemas.StrSchema
-):
-
-
-    class MetaOapg:
-        enum_value_to_name = {
-            "None": "NONE",
-            "Regular": "REGULAR",
-            "Fast": "FAST",
-            "Automation": "AUTOMATION",
-        }
-    
-    @schemas.classproperty
-    def NONE(cls):
-        return cls("None")
-    
-    @schemas.classproperty
-    def REGULAR(cls):
-        return cls("Regular")
-    
-    @schemas.classproperty
-    def FAST(cls):
-        return cls("Fast")
-    
-    @schemas.classproperty
-    def AUTOMATION(cls):
-        return cls("Automation")
 XSplititIdempotencyKeySchema = schemas.StrSchema
 RequestRequiredHeaderParams = typing_extensions.TypedDict(
     'RequestRequiredHeaderParams',
     {
         'X-Splitit-IdempotencyKey': typing.Union[XSplititIdempotencyKeySchema, str, ],
     }
 )
 RequestOptionalHeaderParams = typing_extensions.TypedDict(
     'RequestOptionalHeaderParams',
     {
-        'X-Splitit-TestMode': typing.Union[XSplititTestModeSchema, str, ],
     },
     total=False
 )
 
 
 class RequestHeaderParams(RequestRequiredHeaderParams, RequestOptionalHeaderParams):
     pass
 
 
-request_header_x_splitit_test_mode = api_client.HeaderParameter(
-    name="X-Splitit-TestMode",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XSplititTestModeSchema,
-)
 request_header_x_splitit_idempotency_key = api_client.HeaderParameter(
     name="X-Splitit-IdempotencyKey",
     style=api_client.ParameterStyle.SIMPLE,
     schema=XSplititIdempotencyKeySchema,
     required=True,
 )
+# Path params
+InstallmentPlanNumberSchema = schemas.StrSchema
+RequestRequiredPathParams = typing_extensions.TypedDict(
+    'RequestRequiredPathParams',
+    {
+        'installmentPlanNumber': typing.Union[InstallmentPlanNumberSchema, str, ],
+    }
+)
+RequestOptionalPathParams = typing_extensions.TypedDict(
+    'RequestOptionalPathParams',
+    {
+    },
+    total=False
+)
+
+
+class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
+    pass
+
+
+request_path_installment_plan_number = api_client.PathParameter(
+    name="installmentPlanNumber",
+    style=api_client.ParameterStyle.SIMPLE,
+    schema=InstallmentPlanNumberSchema,
+    required=True,
+)
 # body param
-SchemaForRequestBodyApplicationJsonPatchjson = InstallmentPlanCreateRequest
-SchemaForRequestBodyApplicationJson = InstallmentPlanCreateRequest
-SchemaForRequestBodyTextJson = InstallmentPlanCreateRequest
-SchemaForRequestBodyApplicationJson = InstallmentPlanCreateRequest
+SchemaForRequestBodyApplicationJsonPatchjson = InstallmentPlanRefundRequestSchema
+SchemaForRequestBodyApplicationJson = InstallmentPlanRefundRequestSchema
+SchemaForRequestBodyTextJson = InstallmentPlanRefundRequestSchema
+SchemaForRequestBodyApplicationJson = InstallmentPlanRefundRequestSchema
 
 
-request_body_installment_plan_create_request = api_client.RequestBody(
+request_body_installment_plan_refund_request = api_client.RequestBody(
     content={
         'application/json-patch+json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJsonPatchjson),
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaForRequestBodyTextJson),
@@ -118,595 +113,491 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'oauth',
 ]
-SchemaFor200ResponseBodyTextPlain = InstallmentPlanCreateResponse
-SchemaFor200ResponseBodyApplicationJson = InstallmentPlanCreateResponse
-SchemaFor200ResponseBodyTextJson = InstallmentPlanCreateResponse
+SchemaFor200ResponseBodyTextPlain = InstallmentPlanRefundResponseSchema
+SchemaFor200ResponseBodyApplicationJson = InstallmentPlanRefundResponseSchema
+SchemaFor200ResponseBodyTextJson = InstallmentPlanRefundResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor200ResponseBodyTextPlain,
-        SchemaFor200ResponseBodyApplicationJson,
-        SchemaFor200ResponseBodyTextJson,
-    ]
+    body: InstallmentPlanRefundResponse
+
+
+@dataclass
+class ApiResponseFor200Async(api_client.AsyncApiResponse):
+    body: InstallmentPlanRefundResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
+    response_cls_async=ApiResponseFor200Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor200ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyTextJson),
     },
 )
-SchemaFor400ResponseBodyTextPlain = PlanErrorResponse
-SchemaFor400ResponseBodyApplicationJson = PlanErrorResponse
-SchemaFor400ResponseBodyTextJson = PlanErrorResponse
+SchemaFor401ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor401ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor401ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor400ResponseBodyTextPlain,
-        SchemaFor400ResponseBodyApplicationJson,
-        SchemaFor400ResponseBodyTextJson,
-    ]
-
-
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
-    content={
-        'text/plain': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyTextPlain),
-        'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
-        'text/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyTextJson),
-    },
-)
-SchemaFor401ResponseBodyTextPlain = FailedResponse
-SchemaFor401ResponseBodyApplicationJson = FailedResponse
-SchemaFor401ResponseBodyTextJson = FailedResponse
+class ApiResponseFor401(api_client.ApiResponse):
+    body: FailedResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor401ResponseBodyTextPlain,
-        SchemaFor401ResponseBodyApplicationJson,
-        SchemaFor401ResponseBodyTextJson,
-    ]
+class ApiResponseFor401Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
+    response_cls_async=ApiResponseFor401Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor401ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyTextJson),
     },
 )
-SchemaFor403ResponseBodyTextPlain = FailedResponse
-SchemaFor403ResponseBodyApplicationJson = FailedResponse
-SchemaFor403ResponseBodyTextJson = FailedResponse
+SchemaFor403ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor403ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor403ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor403ResponseBodyTextPlain,
-        SchemaFor403ResponseBodyApplicationJson,
-        SchemaFor403ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor403Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
+    response_cls_async=ApiResponseFor403Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor403ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyTextJson),
     },
 )
-SchemaFor404ResponseBodyTextPlain = FailedResponse
-SchemaFor404ResponseBodyApplicationJson = FailedResponse
-SchemaFor404ResponseBodyTextJson = FailedResponse
+SchemaFor404ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor404ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor404ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor404ResponseBodyTextPlain,
-        SchemaFor404ResponseBodyApplicationJson,
-        SchemaFor404ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor404Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
+    response_cls_async=ApiResponseFor404Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor404ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyTextJson),
     },
 )
-SchemaFor500ResponseBodyTextPlain = FailedResponse
-SchemaFor500ResponseBodyApplicationJson = FailedResponse
-SchemaFor500ResponseBodyTextJson = FailedResponse
+SchemaFor500ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor500ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor500ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor500(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor500ResponseBodyTextPlain,
-        SchemaFor500ResponseBodyApplicationJson,
-        SchemaFor500ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor500Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_500 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor500,
+    response_cls_async=ApiResponseFor500Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
-    '400': _response_for_400,
     '401': _response_for_401,
     '403': _response_for_403,
     '404': _response_for_404,
     '500': _response_for_500,
 }
 _all_accept_content_types = (
     'text/plain',
     'application/json',
     'text/json',
 )
 
 
 class BaseApi(api_client.Api):
-    @typing.overload
-    def _post2_oapg(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,],
-        content_type: typing_extensions.Literal["application/json-patch+json"] = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def _post2_oapg(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def _post2_oapg(
-        self,
-        body: typing.Union[SchemaForRequestBodyTextJson,],
-        content_type: typing_extensions.Literal["text/json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
 
-    @typing.overload
-    def _post2_oapg(
+    def _refund_mapped_args(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/*+json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
+        amount: typing.Union[int, float],
+        installment_plan_number: str,
+        x_splitit_idempotency_key: str,
+        refund_strategy: typing.Optional[RefundStrategy] = None,
+    ) -> api_client.MappedArgs:
+        args: api_client.MappedArgs = api_client.MappedArgs()
+        _header_params = {}
+        _path_params = {}
+        _body = {}
+        if amount is not None:
+            _body["Amount"] = amount
+        if refund_strategy is not None:
+            _body["RefundStrategy"] = refund_strategy
+        args.body = _body
+        if x_splitit_idempotency_key is not None:
+            _header_params["X-Splitit-IdempotencyKey"] = x_splitit_idempotency_key
+        if installment_plan_number is not None:
+            _path_params["installmentPlanNumber"] = installment_plan_number
+        args.header = _header_params
+        args.path = _path_params
+        return args
+
+    async def _arefund_oapg(
+        self,
+        body: typing.Any = None,
+            header_params: typing.Optional[dict] = {},
+            path_params: typing.Optional[dict] = {},
+        skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def _post2_oapg(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'application/json-patch+json',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        """
+        :param skip_deserialization: If true then api_response.response will be set but
+            api_response.body and api_response.headers will not be deserialized into schema
+            class instances
+        """
+        self._verify_typed_dict_inputs_oapg(RequestHeaderParams, header_params)
+        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
+        used_path = path.value
+    
+        _path_params = {}
+        for parameter in (
+            request_path_installment_plan_number,
+        ):
+            parameter_data = path_params.get(parameter.name, schemas.unset)
+            if parameter_data is schemas.unset:
+                continue
+            serialized_data = parameter.serialize(parameter_data)
+            _path_params.update(serialized_data)
+    
+        for k, v in _path_params.items():
+            used_path = used_path.replace('{%s}' % k, v)
+    
+        _headers = HTTPHeaderDict()
+        for parameter in (
+            request_header_x_splitit_idempotency_key,
+        ):
+            parameter_data = header_params.get(parameter.name, schemas.unset)
+            if parameter_data is schemas.unset:
+                continue
+            serialized_data = parameter.serialize(parameter_data)
+            _headers.extend(serialized_data)
+        # TODO add cookie handling
+        if accept_content_types:
+            for accept_content_type in accept_content_types:
+                _headers.add('Accept', accept_content_type)
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_installment_plan_refund_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
+        response = await self.api_client.async_call_api(
+            resource_path=used_path,
+            method='post'.upper(),
+            headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
+            auth_settings=_auth,
+            timeout=timeout,
+        )
+        
+        if stream:
+            async def stream_iterator():
+                """
+                iterates over response.http_response.content and closes connection once iteration has finished
+                """
+                async for line in response.http_response.content:
+                    if line == b'\r\n':
+                        continue
+                    yield line
+                response.http_response.close()
+                await response.session.close()
+            return AsyncGeneratorResponse(
+                content=stream_iterator(),
+                headers=response.http_response.headers,
+                status=response.http_response.status,
+                response=response.http_response
+            )
+    
+        response_for_status = _status_code_to_response.get(str(response.http_response.status))
+        if response_for_status:
+            api_response = await response_for_status.deserialize_async(
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
+        else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
+            api_response = api_client.ApiResponseWithoutDeserializationAsync(
+                body=await response.http_response.json() if is_json else await response.http_response.text(),
+                response=response.http_response,
+                round_trip_time=response.round_trip_time,
+                status=response.http_response.status,
+                headers=response.http_response.headers,
+            )
+    
+        if not 200 <= api_response.status <= 299:
+            raise exceptions.ApiException(api_response=api_response)
+    
+        # cleanup session / response
+        response.http_response.close()
+        await response.session.close()
+    
+        return api_response
 
-    @typing.overload
-    def _post2_oapg(
+    def _refund_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
+        body: typing.Any = None,
+            header_params: typing.Optional[dict] = {},
+            path_params: typing.Optional[dict] = {},
+        skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def _post2_oapg(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'application/json-patch+json',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def _post2_oapg(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = 'application/json-patch+json',
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
+    ]:
         """
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestHeaderParams, header_params)
+        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
-
+    
+        _path_params = {}
+        for parameter in (
+            request_path_installment_plan_number,
+        ):
+            parameter_data = path_params.get(parameter.name, schemas.unset)
+            if parameter_data is schemas.unset:
+                continue
+            serialized_data = parameter.serialize(parameter_data)
+            _path_params.update(serialized_data)
+    
+        for k, v in _path_params.items():
+            used_path = used_path.replace('{%s}' % k, v)
+    
         _headers = HTTPHeaderDict()
         for parameter in (
-            request_header_x_splitit_test_mode,
             request_header_x_splitit_idempotency_key,
         ):
             parameter_data = header_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _headers.extend(serialized_data)
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-
+    
         if body is schemas.unset:
             raise exceptions.ApiValueError(
                 'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        serialized_data = request_body_installment_plan_create_request.serialize(body, content_type)
+        serialized_data = request_body_installment_plan_refund_request.serialize(body, content_type)
         _headers.add('Content-Type', content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
-            _body = serialized_data['body']
+            _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
             method='post'.upper(),
             headers=_headers,
             fields=_fields,
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
-            stream=stream,
             timeout=timeout,
         )
-
+    
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
-                                                   response,
-                                                   self.api_client.configuration,
-                                                   skip_deserialization=skip_deserialization
-                                               )
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
         else:
             # If response data is JSON then deserialize for SDK consumer convenience
             is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
                 body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
-
+    
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
-
+    
         return api_response
 
-
-class Post2(BaseApi):
+class Refund(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    @typing.overload
-    def post2(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,],
-        content_type: typing_extensions.Literal["application/json-patch+json"] = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post2(
+    async def arefund(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post2(
-        self,
-        body: typing.Union[SchemaForRequestBodyTextJson,],
-        content_type: typing_extensions.Literal["text/json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post2(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/*+json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post2(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def post2(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def post2(
+        amount: typing.Union[int, float],
+        installment_plan_number: str,
+        x_splitit_idempotency_key: str,
+        refund_strategy: typing.Optional[RefundStrategy] = None,
+    ) -> typing.Union[
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._refund_mapped_args(
+            amount=amount,
+            installment_plan_number=installment_plan_number,
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            refund_strategy=refund_strategy,
+        )
+        return await self._arefund_oapg(
+            body=args.body,
+            header_params=args.header,
+            path_params=args.path,
+        )
+    
+    def refund(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        amount: typing.Union[int, float],
+        installment_plan_number: str,
+        x_splitit_idempotency_key: str,
+        refund_strategy: typing.Optional[RefundStrategy] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def post2(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = 'application/json-patch+json',
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._post2_oapg(
-            body=body,
-            header_params=header_params,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+    ]:
+        args = self._refund_mapped_args(
+            amount=amount,
+            installment_plan_number=installment_plan_number,
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            refund_strategy=refund_strategy,
+        )
+        return self._refund_oapg(
+            body=args.body,
+            header_params=args.header,
+            path_params=args.path,
         )
-
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    @typing.overload
-    def post(
+    async def apost(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,],
-        content_type: typing_extensions.Literal["application/json-patch+json"] = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyTextJson,],
-        content_type: typing_extensions.Literal["text/json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/*+json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
+        amount: typing.Union[int, float],
+        installment_plan_number: str,
+        x_splitit_idempotency_key: str,
+        refund_strategy: typing.Optional[RefundStrategy] = None,
+    ) -> typing.Union[
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._refund_mapped_args(
+            amount=amount,
+            installment_plan_number=installment_plan_number,
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            refund_strategy=refund_strategy,
+        )
+        return await self._arefund_oapg(
+            body=args.body,
+            header_params=args.header,
+            path_params=args.path,
+        )
+    
     def post(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        amount: typing.Union[int, float],
+        installment_plan_number: str,
+        x_splitit_idempotency_key: str,
+        refund_strategy: typing.Optional[RefundStrategy] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = 'application/json-patch+json',
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._post2_oapg(
-            body=body,
-            header_params=header_params,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+    ]:
+        args = self._refund_mapped_args(
+            amount=amount,
+            installment_plan_number=installment_plan_number,
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            refund_strategy=refund_strategy,
+        )
+        return self._refund_oapg(
+            body=args.body,
+            header_params=args.header,
+            path_params=args.path,
         )
-
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py` & `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number_refund/post.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -11,33 +11,38 @@
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
 import json
 from urllib3._collections import HTTPHeaderDict
 
+from splitit_client.api_response import AsyncGeneratorResponse
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
-from splitit_client.model.check_installments_eligibility_request import CheckInstallmentsEligibilityRequest
-from splitit_client.model.installments_eligibility_response import InstallmentsEligibilityResponse
-from splitit_client.model.failed_response import FailedResponse
-
-from . import path
+from splitit_client.model.failed_response import FailedResponse as FailedResponseSchema
+from splitit_client.model.refund_strategy import RefundStrategy as RefundStrategySchema
+from splitit_client.model.installment_plan_refund_response import InstallmentPlanRefundResponse as InstallmentPlanRefundResponseSchema
+from splitit_client.model.installment_plan_refund_request import InstallmentPlanRefundRequest as InstallmentPlanRefundRequestSchema
+
+from splitit_client.type.failed_response import FailedResponse
+from splitit_client.type.installment_plan_refund_response import InstallmentPlanRefundResponse
+from splitit_client.type.refund_strategy import RefundStrategy
+from splitit_client.type.installment_plan_refund_request import InstallmentPlanRefundRequest
 
 # Header params
 XSplititIdempotencyKeySchema = schemas.StrSchema
 RequestRequiredHeaderParams = typing_extensions.TypedDict(
     'RequestRequiredHeaderParams',
     {
         'X-Splitit-IdempotencyKey': typing.Union[XSplititIdempotencyKeySchema, str, ],
@@ -57,591 +62,530 @@
 
 request_header_x_splitit_idempotency_key = api_client.HeaderParameter(
     name="X-Splitit-IdempotencyKey",
     style=api_client.ParameterStyle.SIMPLE,
     schema=XSplititIdempotencyKeySchema,
     required=True,
 )
+# Path params
+InstallmentPlanNumberSchema = schemas.StrSchema
+RequestRequiredPathParams = typing_extensions.TypedDict(
+    'RequestRequiredPathParams',
+    {
+        'installmentPlanNumber': typing.Union[InstallmentPlanNumberSchema, str, ],
+    }
+)
+RequestOptionalPathParams = typing_extensions.TypedDict(
+    'RequestOptionalPathParams',
+    {
+    },
+    total=False
+)
+
+
+class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
+    pass
+
+
+request_path_installment_plan_number = api_client.PathParameter(
+    name="installmentPlanNumber",
+    style=api_client.ParameterStyle.SIMPLE,
+    schema=InstallmentPlanNumberSchema,
+    required=True,
+)
 # body param
-SchemaForRequestBodyApplicationJsonPatchjson = CheckInstallmentsEligibilityRequest
-SchemaForRequestBodyApplicationJson = CheckInstallmentsEligibilityRequest
-SchemaForRequestBodyTextJson = CheckInstallmentsEligibilityRequest
-SchemaForRequestBodyApplicationJson = CheckInstallmentsEligibilityRequest
+SchemaForRequestBodyApplicationJsonPatchjson = InstallmentPlanRefundRequestSchema
+SchemaForRequestBodyApplicationJson = InstallmentPlanRefundRequestSchema
+SchemaForRequestBodyTextJson = InstallmentPlanRefundRequestSchema
+SchemaForRequestBodyApplicationJson = InstallmentPlanRefundRequestSchema
 
 
-request_body_check_installments_eligibility_request = api_client.RequestBody(
+request_body_installment_plan_refund_request = api_client.RequestBody(
     content={
         'application/json-patch+json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJsonPatchjson),
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaForRequestBodyTextJson),
         'application/*+json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-_auth = [
-    'oauth',
-]
-SchemaFor200ResponseBodyTextPlain = InstallmentsEligibilityResponse
-SchemaFor200ResponseBodyApplicationJson = InstallmentsEligibilityResponse
-SchemaFor200ResponseBodyTextJson = InstallmentsEligibilityResponse
+SchemaFor200ResponseBodyTextPlain = InstallmentPlanRefundResponseSchema
+SchemaFor200ResponseBodyApplicationJson = InstallmentPlanRefundResponseSchema
+SchemaFor200ResponseBodyTextJson = InstallmentPlanRefundResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor200ResponseBodyTextPlain,
-        SchemaFor200ResponseBodyApplicationJson,
-        SchemaFor200ResponseBodyTextJson,
-    ]
+    body: InstallmentPlanRefundResponse
+
+
+@dataclass
+class ApiResponseFor200Async(api_client.AsyncApiResponse):
+    body: InstallmentPlanRefundResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
+    response_cls_async=ApiResponseFor200Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor200ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyTextJson),
     },
 )
-SchemaFor401ResponseBodyTextPlain = FailedResponse
-SchemaFor401ResponseBodyApplicationJson = FailedResponse
-SchemaFor401ResponseBodyTextJson = FailedResponse
+SchemaFor401ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor401ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor401ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor401ResponseBodyTextPlain,
-        SchemaFor401ResponseBodyApplicationJson,
-        SchemaFor401ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor401Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
+    response_cls_async=ApiResponseFor401Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor401ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyTextJson),
     },
 )
-SchemaFor403ResponseBodyTextPlain = FailedResponse
-SchemaFor403ResponseBodyApplicationJson = FailedResponse
-SchemaFor403ResponseBodyTextJson = FailedResponse
+SchemaFor403ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor403ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor403ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor403ResponseBodyTextPlain,
-        SchemaFor403ResponseBodyApplicationJson,
-        SchemaFor403ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor403Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
+    response_cls_async=ApiResponseFor403Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor403ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyTextJson),
     },
 )
-SchemaFor404ResponseBodyTextPlain = FailedResponse
-SchemaFor404ResponseBodyApplicationJson = FailedResponse
-SchemaFor404ResponseBodyTextJson = FailedResponse
+SchemaFor404ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor404ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor404ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor404ResponseBodyTextPlain,
-        SchemaFor404ResponseBodyApplicationJson,
-        SchemaFor404ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor404Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
+    response_cls_async=ApiResponseFor404Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor404ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyTextJson),
     },
 )
-SchemaFor500ResponseBodyTextPlain = FailedResponse
-SchemaFor500ResponseBodyApplicationJson = FailedResponse
-SchemaFor500ResponseBodyTextJson = FailedResponse
+SchemaFor500ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor500ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor500ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor500(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor500ResponseBodyTextPlain,
-        SchemaFor500ResponseBodyApplicationJson,
-        SchemaFor500ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor500Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_500 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor500,
+    response_cls_async=ApiResponseFor500Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '401': _response_for_401,
-    '403': _response_for_403,
-    '404': _response_for_404,
-    '500': _response_for_500,
-}
 _all_accept_content_types = (
     'text/plain',
     'application/json',
     'text/json',
 )
 
 
 class BaseApi(api_client.Api):
-    @typing.overload
-    def _check_eligibility_oapg(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,],
-        content_type: typing_extensions.Literal["application/json-patch+json"] = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def _check_eligibility_oapg(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def _check_eligibility_oapg(
-        self,
-        body: typing.Union[SchemaForRequestBodyTextJson,],
-        content_type: typing_extensions.Literal["text/json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
 
-    @typing.overload
-    def _check_eligibility_oapg(
+    def _refund_mapped_args(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/*+json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
+        amount: typing.Union[int, float],
+        installment_plan_number: str,
+        x_splitit_idempotency_key: str,
+        refund_strategy: typing.Optional[RefundStrategy] = None,
+    ) -> api_client.MappedArgs:
+        args: api_client.MappedArgs = api_client.MappedArgs()
+        _header_params = {}
+        _path_params = {}
+        _body = {}
+        if amount is not None:
+            _body["Amount"] = amount
+        if refund_strategy is not None:
+            _body["RefundStrategy"] = refund_strategy
+        args.body = _body
+        if x_splitit_idempotency_key is not None:
+            _header_params["X-Splitit-IdempotencyKey"] = x_splitit_idempotency_key
+        if installment_plan_number is not None:
+            _path_params["installmentPlanNumber"] = installment_plan_number
+        args.header = _header_params
+        args.path = _path_params
+        return args
+
+    async def _arefund_oapg(
+        self,
+        body: typing.Any = None,
+            header_params: typing.Optional[dict] = {},
+            path_params: typing.Optional[dict] = {},
+        skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def _check_eligibility_oapg(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'application/json-patch+json',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        """
+        :param skip_deserialization: If true then api_response.response will be set but
+            api_response.body and api_response.headers will not be deserialized into schema
+            class instances
+        """
+        self._verify_typed_dict_inputs_oapg(RequestHeaderParams, header_params)
+        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
+        used_path = path.value
+    
+        _path_params = {}
+        for parameter in (
+            request_path_installment_plan_number,
+        ):
+            parameter_data = path_params.get(parameter.name, schemas.unset)
+            if parameter_data is schemas.unset:
+                continue
+            serialized_data = parameter.serialize(parameter_data)
+            _path_params.update(serialized_data)
+    
+        for k, v in _path_params.items():
+            used_path = used_path.replace('{%s}' % k, v)
+    
+        _headers = HTTPHeaderDict()
+        for parameter in (
+            request_header_x_splitit_idempotency_key,
+        ):
+            parameter_data = header_params.get(parameter.name, schemas.unset)
+            if parameter_data is schemas.unset:
+                continue
+            serialized_data = parameter.serialize(parameter_data)
+            _headers.extend(serialized_data)
+        # TODO add cookie handling
+        if accept_content_types:
+            for accept_content_type in accept_content_types:
+                _headers.add('Accept', accept_content_type)
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_installment_plan_refund_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
+        response = await self.api_client.async_call_api(
+            resource_path=used_path,
+            method='post'.upper(),
+            headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
+            auth_settings=_auth,
+            timeout=timeout,
+        )
+        
+        if stream:
+            async def stream_iterator():
+                """
+                iterates over response.http_response.content and closes connection once iteration has finished
+                """
+                async for line in response.http_response.content:
+                    if line == b'\r\n':
+                        continue
+                    yield line
+                response.http_response.close()
+                await response.session.close()
+            return AsyncGeneratorResponse(
+                content=stream_iterator(),
+                headers=response.http_response.headers,
+                status=response.http_response.status,
+                response=response.http_response
+            )
+    
+        response_for_status = _status_code_to_response.get(str(response.http_response.status))
+        if response_for_status:
+            api_response = await response_for_status.deserialize_async(
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
+        else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
+            api_response = api_client.ApiResponseWithoutDeserializationAsync(
+                body=await response.http_response.json() if is_json else await response.http_response.text(),
+                response=response.http_response,
+                round_trip_time=response.round_trip_time,
+                status=response.http_response.status,
+                headers=response.http_response.headers,
+            )
+    
+        if not 200 <= api_response.status <= 299:
+            raise exceptions.ApiException(api_response=api_response)
+    
+        # cleanup session / response
+        response.http_response.close()
+        await response.session.close()
+    
+        return api_response
 
-    @typing.overload
-    def _check_eligibility_oapg(
+    def _refund_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
+        body: typing.Any = None,
+            header_params: typing.Optional[dict] = {},
+            path_params: typing.Optional[dict] = {},
+        skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def _check_eligibility_oapg(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'application/json-patch+json',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def _check_eligibility_oapg(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = 'application/json-patch+json',
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
+    ]:
         """
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestHeaderParams, header_params)
+        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
-
+    
+        _path_params = {}
+        for parameter in (
+            request_path_installment_plan_number,
+        ):
+            parameter_data = path_params.get(parameter.name, schemas.unset)
+            if parameter_data is schemas.unset:
+                continue
+            serialized_data = parameter.serialize(parameter_data)
+            _path_params.update(serialized_data)
+    
+        for k, v in _path_params.items():
+            used_path = used_path.replace('{%s}' % k, v)
+    
         _headers = HTTPHeaderDict()
         for parameter in (
             request_header_x_splitit_idempotency_key,
         ):
             parameter_data = header_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _headers.extend(serialized_data)
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-
+    
         if body is schemas.unset:
             raise exceptions.ApiValueError(
                 'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        serialized_data = request_body_check_installments_eligibility_request.serialize(body, content_type)
+        serialized_data = request_body_installment_plan_refund_request.serialize(body, content_type)
         _headers.add('Content-Type', content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
-            _body = serialized_data['body']
+            _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
             method='post'.upper(),
             headers=_headers,
             fields=_fields,
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
-            stream=stream,
             timeout=timeout,
         )
-
+    
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
-                                                   response,
-                                                   self.api_client.configuration,
-                                                   skip_deserialization=skip_deserialization
-                                               )
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
         else:
             # If response data is JSON then deserialize for SDK consumer convenience
             is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
                 body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
-
+    
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
-
+    
         return api_response
 
-
-class CheckEligibility(BaseApi):
+class Refund(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    @typing.overload
-    def check_eligibility(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,],
-        content_type: typing_extensions.Literal["application/json-patch+json"] = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def check_eligibility(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def check_eligibility(
-        self,
-        body: typing.Union[SchemaForRequestBodyTextJson,],
-        content_type: typing_extensions.Literal["text/json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def check_eligibility(
+    async def arefund(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/*+json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def check_eligibility(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def check_eligibility(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def check_eligibility(
+        amount: typing.Union[int, float],
+        installment_plan_number: str,
+        x_splitit_idempotency_key: str,
+        refund_strategy: typing.Optional[RefundStrategy] = None,
+    ) -> typing.Union[
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._refund_mapped_args(
+            amount=amount,
+            installment_plan_number=installment_plan_number,
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            refund_strategy=refund_strategy,
+        )
+        return await self._arefund_oapg(
+            body=args.body,
+            header_params=args.header,
+            path_params=args.path,
+        )
+    
+    def refund(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        amount: typing.Union[int, float],
+        installment_plan_number: str,
+        x_splitit_idempotency_key: str,
+        refund_strategy: typing.Optional[RefundStrategy] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def check_eligibility(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = 'application/json-patch+json',
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._check_eligibility_oapg(
-            body=body,
-            header_params=header_params,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+    ]:
+        args = self._refund_mapped_args(
+            amount=amount,
+            installment_plan_number=installment_plan_number,
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            refund_strategy=refund_strategy,
+        )
+        return self._refund_oapg(
+            body=args.body,
+            header_params=args.header,
+            path_params=args.path,
         )
-
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    @typing.overload
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,],
-        content_type: typing_extensions.Literal["application/json-patch+json"] = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyTextJson,],
-        content_type: typing_extensions.Literal["text/json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/*+json"],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post(
+    async def apost(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
+        amount: typing.Union[int, float],
+        installment_plan_number: str,
+        x_splitit_idempotency_key: str,
+        refund_strategy: typing.Optional[RefundStrategy] = None,
+    ) -> typing.Union[
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._refund_mapped_args(
+            amount=amount,
+            installment_plan_number=installment_plan_number,
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            refund_strategy=refund_strategy,
+        )
+        return await self._arefund_oapg(
+            body=args.body,
+            header_params=args.header,
+            path_params=args.path,
+        )
+    
     def post(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        amount: typing.Union[int, float],
+        installment_plan_number: str,
+        x_splitit_idempotency_key: str,
+        refund_strategy: typing.Optional[RefundStrategy] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJsonPatchjson,SchemaForRequestBodyApplicationJson,SchemaForRequestBodyTextJson,SchemaForRequestBodyApplicationJson,],
-        content_type: str = 'application/json-patch+json',
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._check_eligibility_oapg(
-            body=body,
-            header_params=header_params,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+    ]:
+        args = self._refund_mapped_args(
+            amount=amount,
+            installment_plan_number=installment_plan_number,
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            refund_strategy=refund_strategy,
+        )
+        return self._refund_oapg(
+            body=args.body,
+            header_params=args.header,
+            path_params=args.path,
         )
-
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py` & `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_search/get.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -11,457 +11,569 @@
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
 import json
 from urllib3._collections import HTTPHeaderDict
 
+from splitit_client.api_response import AsyncGeneratorResponse
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
-from splitit_client.model.failed_response import FailedResponse
-from splitit_client.model.installment_plan_get_response import InstallmentPlanGetResponse
+from splitit_client.model.failed_response import FailedResponse as FailedResponseSchema
+from splitit_client.model.installment_plan_search_response import InstallmentPlanSearchResponse as InstallmentPlanSearchResponseSchema
 
-from . import path
+from splitit_client.type.failed_response import FailedResponse
+from splitit_client.type.installment_plan_search_response import InstallmentPlanSearchResponse
 
-# Header params
-XSplititIdempotencyKeySchema = schemas.StrSchema
-RequestRequiredHeaderParams = typing_extensions.TypedDict(
-    'RequestRequiredHeaderParams',
+# Query params
+InstallmentPlanNumberSchema = schemas.StrSchema
+RefOrderNumberSchema = schemas.StrSchema
+
+
+class ExtendedParamsSchema(
+    schemas.DictSchema
+):
+
+
+    class MetaOapg:
+        additional_properties = schemas.StrSchema
+    
+    def __getitem__(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+    
+    def get_item_oapg(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
+        return super().get_item_oapg(name)
+
+    def __new__(
+        cls,
+        *args: typing.Union[dict, frozendict.frozendict, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[MetaOapg.additional_properties, str, ],
+    ) -> 'ExtendedParamsSchema':
+        return super().__new__(
+            cls,
+            *args,
+            _configuration=_configuration,
+            **kwargs,
+        )
+RequestRequiredQueryParams = typing_extensions.TypedDict(
+    'RequestRequiredQueryParams',
     {
-        'X-Splitit-IdempotencyKey': typing.Union[XSplititIdempotencyKeySchema, str, ],
     }
 )
-RequestOptionalHeaderParams = typing_extensions.TypedDict(
-    'RequestOptionalHeaderParams',
+RequestOptionalQueryParams = typing_extensions.TypedDict(
+    'RequestOptionalQueryParams',
     {
+        'installmentPlanNumber': typing.Union[InstallmentPlanNumberSchema, str, ],
+        'refOrderNumber': typing.Union[RefOrderNumberSchema, str, ],
+        'extendedParams': typing.Union[ExtendedParamsSchema, dict, frozendict.frozendict, ],
     },
     total=False
 )
 
 
-class RequestHeaderParams(RequestRequiredHeaderParams, RequestOptionalHeaderParams):
+class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
-request_header_x_splitit_idempotency_key = api_client.HeaderParameter(
-    name="X-Splitit-IdempotencyKey",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XSplititIdempotencyKeySchema,
-    required=True,
+request_query_installment_plan_number = api_client.QueryParameter(
+    name="installmentPlanNumber",
+    style=api_client.ParameterStyle.FORM,
+    schema=InstallmentPlanNumberSchema,
+    explode=True,
 )
-# Path params
-InstallmentPlanNumberSchema = schemas.StrSchema
-RequestRequiredPathParams = typing_extensions.TypedDict(
-    'RequestRequiredPathParams',
+request_query_ref_order_number = api_client.QueryParameter(
+    name="refOrderNumber",
+    style=api_client.ParameterStyle.FORM,
+    schema=RefOrderNumberSchema,
+    explode=True,
+)
+request_query_extended_params = api_client.QueryParameter(
+    name="extendedParams",
+    style=api_client.ParameterStyle.FORM,
+    schema=ExtendedParamsSchema,
+    explode=True,
+)
+# Header params
+XSplititIdempotencyKeySchema = schemas.StrSchema
+RequestRequiredHeaderParams = typing_extensions.TypedDict(
+    'RequestRequiredHeaderParams',
     {
-        'installmentPlanNumber': typing.Union[InstallmentPlanNumberSchema, str, ],
+        'X-Splitit-IdempotencyKey': typing.Union[XSplititIdempotencyKeySchema, str, ],
     }
 )
-RequestOptionalPathParams = typing_extensions.TypedDict(
-    'RequestOptionalPathParams',
+RequestOptionalHeaderParams = typing_extensions.TypedDict(
+    'RequestOptionalHeaderParams',
     {
     },
     total=False
 )
 
 
-class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
+class RequestHeaderParams(RequestRequiredHeaderParams, RequestOptionalHeaderParams):
     pass
 
 
-request_path_installment_plan_number = api_client.PathParameter(
-    name="installmentPlanNumber",
+request_header_x_splitit_idempotency_key = api_client.HeaderParameter(
+    name="X-Splitit-IdempotencyKey",
     style=api_client.ParameterStyle.SIMPLE,
-    schema=InstallmentPlanNumberSchema,
+    schema=XSplititIdempotencyKeySchema,
     required=True,
 )
-_auth = [
-    'oauth',
-]
-SchemaFor200ResponseBodyTextPlain = InstallmentPlanGetResponse
-SchemaFor200ResponseBodyApplicationJson = InstallmentPlanGetResponse
-SchemaFor200ResponseBodyTextJson = InstallmentPlanGetResponse
+SchemaFor200ResponseBodyTextPlain = InstallmentPlanSearchResponseSchema
+SchemaFor200ResponseBodyApplicationJson = InstallmentPlanSearchResponseSchema
+SchemaFor200ResponseBodyTextJson = InstallmentPlanSearchResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor200ResponseBodyTextPlain,
-        SchemaFor200ResponseBodyApplicationJson,
-        SchemaFor200ResponseBodyTextJson,
-    ]
+    body: InstallmentPlanSearchResponse
+
+
+@dataclass
+class ApiResponseFor200Async(api_client.AsyncApiResponse):
+    body: InstallmentPlanSearchResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
+    response_cls_async=ApiResponseFor200Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor200ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyTextJson),
     },
 )
-SchemaFor401ResponseBodyTextPlain = FailedResponse
-SchemaFor401ResponseBodyApplicationJson = FailedResponse
-SchemaFor401ResponseBodyTextJson = FailedResponse
+SchemaFor401ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor401ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor401ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor401ResponseBodyTextPlain,
-        SchemaFor401ResponseBodyApplicationJson,
-        SchemaFor401ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor401Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
+    response_cls_async=ApiResponseFor401Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor401ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyTextJson),
     },
 )
-SchemaFor403ResponseBodyTextPlain = FailedResponse
-SchemaFor403ResponseBodyApplicationJson = FailedResponse
-SchemaFor403ResponseBodyTextJson = FailedResponse
+SchemaFor403ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor403ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor403ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor403ResponseBodyTextPlain,
-        SchemaFor403ResponseBodyApplicationJson,
-        SchemaFor403ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor403Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
+    response_cls_async=ApiResponseFor403Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor403ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyTextJson),
     },
 )
-SchemaFor404ResponseBodyTextPlain = FailedResponse
-SchemaFor404ResponseBodyApplicationJson = FailedResponse
-SchemaFor404ResponseBodyTextJson = FailedResponse
+SchemaFor404ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor404ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor404ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor404ResponseBodyTextPlain,
-        SchemaFor404ResponseBodyApplicationJson,
-        SchemaFor404ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor404Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
+    response_cls_async=ApiResponseFor404Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor404ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyTextJson),
     },
 )
-SchemaFor500ResponseBodyTextPlain = FailedResponse
-SchemaFor500ResponseBodyApplicationJson = FailedResponse
-SchemaFor500ResponseBodyTextJson = FailedResponse
+SchemaFor500ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor500ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor500ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor500(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor500ResponseBodyTextPlain,
-        SchemaFor500ResponseBodyApplicationJson,
-        SchemaFor500ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor500Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_500 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor500,
+    response_cls_async=ApiResponseFor500Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '401': _response_for_401,
-    '403': _response_for_403,
-    '404': _response_for_404,
-    '500': _response_for_500,
-}
 _all_accept_content_types = (
     'text/plain',
     'application/json',
     'text/json',
 )
 
 
 class BaseApi(api_client.Api):
-    @typing.overload
-    def _get_oapg(
+
+    def _search_mapped_args(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+        x_splitit_idempotency_key: str,
+        installment_plan_number: typing.Optional[str] = None,
+        ref_order_number: typing.Optional[str] = None,
+        extended_params: typing.Optional[typing.Dict[str, str]] = None,
+    ) -> api_client.MappedArgs:
+        args: api_client.MappedArgs = api_client.MappedArgs()
+        _query_params = {}
+        _header_params = {}
+        if installment_plan_number is not None:
+            _query_params["installmentPlanNumber"] = installment_plan_number
+        if ref_order_number is not None:
+            _query_params["refOrderNumber"] = ref_order_number
+        if extended_params is not None:
+            _query_params["extendedParams"] = extended_params
+        if x_splitit_idempotency_key is not None:
+            _header_params["X-Splitit-IdempotencyKey"] = x_splitit_idempotency_key
+        args.query = _query_params
+        args.header = _header_params
+        return args
 
-    @typing.overload
-    def _get_oapg(
+    async def _asearch_oapg(
         self,
-        skip_deserialization: typing_extensions.Literal[True],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
+            query_params: typing.Optional[dict] = {},
+            header_params: typing.Optional[dict] = {},
+        skip_deserialization: bool = True,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
+    ) -> typing.Union[
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        """
+        :param skip_deserialization: If true then api_response.response will be set but
+            api_response.body and api_response.headers will not be deserialized into schema
+            class instances
+        """
+        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
+        self._verify_typed_dict_inputs_oapg(RequestHeaderParams, header_params)
+        used_path = path.value
+    
+        prefix_separator_iterator = None
+        for parameter in (
+            request_query_installment_plan_number,
+            request_query_ref_order_number,
+            request_query_extended_params,
+        ):
+            parameter_data = query_params.get(parameter.name, schemas.unset)
+            if parameter_data is schemas.unset:
+                continue
+            if prefix_separator_iterator is None:
+                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
+            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
+            for serialized_value in serialized_data.values():
+                used_path += serialized_value
+    
+        _headers = HTTPHeaderDict()
+        for parameter in (
+            request_header_x_splitit_idempotency_key,
+        ):
+            parameter_data = header_params.get(parameter.name, schemas.unset)
+            if parameter_data is schemas.unset:
+                continue
+            serialized_data = parameter.serialize(parameter_data)
+            _headers.extend(serialized_data)
+        # TODO add cookie handling
+        if accept_content_types:
+            for accept_content_type in accept_content_types:
+                _headers.add('Accept', accept_content_type)
+    
+        response = await self.api_client.async_call_api(
+            resource_path=used_path,
+            method='get'.upper(),
+            headers=_headers,
+            auth_settings=_auth,
+            prefix_separator_iterator=prefix_separator_iterator,
+            timeout=timeout,
+        )
+        
+        if stream:
+            async def stream_iterator():
+                """
+                iterates over response.http_response.content and closes connection once iteration has finished
+                """
+                async for line in response.http_response.content:
+                    if line == b'\r\n':
+                        continue
+                    yield line
+                response.http_response.close()
+                await response.session.close()
+            return AsyncGeneratorResponse(
+                content=stream_iterator(),
+                headers=response.http_response.headers,
+                status=response.http_response.status,
+                response=response.http_response
+            )
+    
+        response_for_status = _status_code_to_response.get(str(response.http_response.status))
+        if response_for_status:
+            api_response = await response_for_status.deserialize_async(
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
+        else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
+            api_response = api_client.ApiResponseWithoutDeserializationAsync(
+                body=await response.http_response.json() if is_json else await response.http_response.text(),
+                response=response.http_response,
+                round_trip_time=response.round_trip_time,
+                status=response.http_response.status,
+                headers=response.http_response.headers,
+            )
+    
+        if not 200 <= api_response.status <= 299:
+            raise exceptions.ApiException(api_response=api_response)
+    
+        # cleanup session / response
+        response.http_response.close()
+        await response.session.close()
+    
+        return api_response
 
-    @typing.overload
-    def _get_oapg(
+    def _search_oapg(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
+            query_params: typing.Optional[dict] = {},
+            header_params: typing.Optional[dict] = {},
+        skip_deserialization: bool = True,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def _get_oapg(
-        self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
+    ]:
         """
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
+        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestHeaderParams, header_params)
-        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
-
-        _path_params = {}
+    
+        prefix_separator_iterator = None
         for parameter in (
-            request_path_installment_plan_number,
+            request_query_installment_plan_number,
+            request_query_ref_order_number,
+            request_query_extended_params,
         ):
-            parameter_data = path_params.get(parameter.name, schemas.unset)
+            parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
-            serialized_data = parameter.serialize(parameter_data)
-            _path_params.update(serialized_data)
-
-        for k, v in _path_params.items():
-            used_path = used_path.replace('{%s}' % k, v)
-
+            if prefix_separator_iterator is None:
+                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
+            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
+            for serialized_value in serialized_data.values():
+                used_path += serialized_value
+    
         _headers = HTTPHeaderDict()
         for parameter in (
             request_header_x_splitit_idempotency_key,
         ):
             parameter_data = header_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _headers.extend(serialized_data)
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-
+    
         response = self.api_client.call_api(
             resource_path=used_path,
             method='get'.upper(),
             headers=_headers,
             auth_settings=_auth,
-            stream=stream,
+            prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
-
+    
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
-                                                   response,
-                                                   self.api_client.configuration,
-                                                   skip_deserialization=skip_deserialization
-                                               )
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
         else:
             # If response data is JSON then deserialize for SDK consumer convenience
             is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
                 body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
-
+    
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
-
+    
         return api_response
 
-
-class Get(BaseApi):
+class Search(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    @typing.overload
-    def get(
+    async def asearch(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        x_splitit_idempotency_key: str,
+        installment_plan_number: typing.Optional[str] = None,
+        ref_order_number: typing.Optional[str] = None,
+        extended_params: typing.Optional[typing.Dict[str, str]] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def get(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def get(
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._search_mapped_args(
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            installment_plan_number=installment_plan_number,
+            ref_order_number=ref_order_number,
+            extended_params=extended_params,
+        )
+        return await self._asearch_oapg(
+            query_params=args.query,
+            header_params=args.header,
+        )
+    
+    def search(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        x_splitit_idempotency_key: str,
+        installment_plan_number: typing.Optional[str] = None,
+        ref_order_number: typing.Optional[str] = None,
+        extended_params: typing.Optional[typing.Dict[str, str]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def get(
-        self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._get_oapg(
-            header_params=header_params,
-            path_params=path_params,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+    ]:
+        args = self._search_mapped_args(
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            installment_plan_number=installment_plan_number,
+            ref_order_number=ref_order_number,
+            extended_params=extended_params,
+        )
+        return self._search_oapg(
+            query_params=args.query,
+            header_params=args.header,
         )
-
 
 class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    @typing.overload
-    def get(
+    async def aget(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        x_splitit_idempotency_key: str,
+        installment_plan_number: typing.Optional[str] = None,
+        ref_order_number: typing.Optional[str] = None,
+        extended_params: typing.Optional[typing.Dict[str, str]] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def get(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._search_mapped_args(
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            installment_plan_number=installment_plan_number,
+            ref_order_number=ref_order_number,
+            extended_params=extended_params,
+        )
+        return await self._asearch_oapg(
+            query_params=args.query,
+            header_params=args.header,
+        )
+    
     def get(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        x_splitit_idempotency_key: str,
+        installment_plan_number: typing.Optional[str] = None,
+        ref_order_number: typing.Optional[str] = None,
+        extended_params: typing.Optional[typing.Dict[str, str]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def get(
-        self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._get_oapg(
-            header_params=header_params,
-            path_params=path_params,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+    ]:
+        args = self._search_mapped_args(
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            installment_plan_number=installment_plan_number,
+            ref_order_number=ref_order_number,
+            extended_params=extended_params,
+        )
+        return self._search_oapg(
+            query_params=args.query,
+            header_params=args.header,
         )
-
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_cancel/post.py` & `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_search/get.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,204 +11,262 @@
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
 import json
 from urllib3._collections import HTTPHeaderDict
 
+from splitit_client.api_response import AsyncGeneratorResponse
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
-from splitit_client.model.failed_response import FailedResponse
-from splitit_client.model.installment_plan_cancel_response import InstallmentPlanCancelResponse
+from splitit_client.model.failed_response import FailedResponse as FailedResponseSchema
+from splitit_client.model.installment_plan_search_response import InstallmentPlanSearchResponse as InstallmentPlanSearchResponseSchema
+
+from splitit_client.type.failed_response import FailedResponse
+from splitit_client.type.installment_plan_search_response import InstallmentPlanSearchResponse
 
 from . import path
 
-# Header params
-XSplititIdempotencyKeySchema = schemas.StrSchema
-RequestRequiredHeaderParams = typing_extensions.TypedDict(
-    'RequestRequiredHeaderParams',
+# Query params
+InstallmentPlanNumberSchema = schemas.StrSchema
+RefOrderNumberSchema = schemas.StrSchema
+
+
+class ExtendedParamsSchema(
+    schemas.DictSchema
+):
+
+
+    class MetaOapg:
+        additional_properties = schemas.StrSchema
+    
+    def __getitem__(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+    
+    def get_item_oapg(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
+        return super().get_item_oapg(name)
+
+    def __new__(
+        cls,
+        *args: typing.Union[dict, frozendict.frozendict, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[MetaOapg.additional_properties, str, ],
+    ) -> 'ExtendedParamsSchema':
+        return super().__new__(
+            cls,
+            *args,
+            _configuration=_configuration,
+            **kwargs,
+        )
+RequestRequiredQueryParams = typing_extensions.TypedDict(
+    'RequestRequiredQueryParams',
     {
-        'X-Splitit-IdempotencyKey': typing.Union[XSplititIdempotencyKeySchema, str, ],
     }
 )
-RequestOptionalHeaderParams = typing_extensions.TypedDict(
-    'RequestOptionalHeaderParams',
+RequestOptionalQueryParams = typing_extensions.TypedDict(
+    'RequestOptionalQueryParams',
     {
+        'installmentPlanNumber': typing.Union[InstallmentPlanNumberSchema, str, ],
+        'refOrderNumber': typing.Union[RefOrderNumberSchema, str, ],
+        'extendedParams': typing.Union[ExtendedParamsSchema, dict, frozendict.frozendict, ],
     },
     total=False
 )
 
 
-class RequestHeaderParams(RequestRequiredHeaderParams, RequestOptionalHeaderParams):
+class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
-request_header_x_splitit_idempotency_key = api_client.HeaderParameter(
-    name="X-Splitit-IdempotencyKey",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XSplititIdempotencyKeySchema,
-    required=True,
+request_query_installment_plan_number = api_client.QueryParameter(
+    name="installmentPlanNumber",
+    style=api_client.ParameterStyle.FORM,
+    schema=InstallmentPlanNumberSchema,
+    explode=True,
 )
-# Path params
-InstallmentPlanNumberSchema = schemas.StrSchema
-RequestRequiredPathParams = typing_extensions.TypedDict(
-    'RequestRequiredPathParams',
+request_query_ref_order_number = api_client.QueryParameter(
+    name="refOrderNumber",
+    style=api_client.ParameterStyle.FORM,
+    schema=RefOrderNumberSchema,
+    explode=True,
+)
+request_query_extended_params = api_client.QueryParameter(
+    name="extendedParams",
+    style=api_client.ParameterStyle.FORM,
+    schema=ExtendedParamsSchema,
+    explode=True,
+)
+# Header params
+XSplititIdempotencyKeySchema = schemas.StrSchema
+RequestRequiredHeaderParams = typing_extensions.TypedDict(
+    'RequestRequiredHeaderParams',
     {
-        'installmentPlanNumber': typing.Union[InstallmentPlanNumberSchema, str, ],
+        'X-Splitit-IdempotencyKey': typing.Union[XSplititIdempotencyKeySchema, str, ],
     }
 )
-RequestOptionalPathParams = typing_extensions.TypedDict(
-    'RequestOptionalPathParams',
+RequestOptionalHeaderParams = typing_extensions.TypedDict(
+    'RequestOptionalHeaderParams',
     {
     },
     total=False
 )
 
 
-class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
+class RequestHeaderParams(RequestRequiredHeaderParams, RequestOptionalHeaderParams):
     pass
 
 
-request_path_installment_plan_number = api_client.PathParameter(
-    name="installmentPlanNumber",
+request_header_x_splitit_idempotency_key = api_client.HeaderParameter(
+    name="X-Splitit-IdempotencyKey",
     style=api_client.ParameterStyle.SIMPLE,
-    schema=InstallmentPlanNumberSchema,
+    schema=XSplititIdempotencyKeySchema,
     required=True,
 )
 _auth = [
     'oauth',
 ]
-SchemaFor200ResponseBodyTextPlain = InstallmentPlanCancelResponse
-SchemaFor200ResponseBodyApplicationJson = InstallmentPlanCancelResponse
-SchemaFor200ResponseBodyTextJson = InstallmentPlanCancelResponse
+SchemaFor200ResponseBodyTextPlain = InstallmentPlanSearchResponseSchema
+SchemaFor200ResponseBodyApplicationJson = InstallmentPlanSearchResponseSchema
+SchemaFor200ResponseBodyTextJson = InstallmentPlanSearchResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor200ResponseBodyTextPlain,
-        SchemaFor200ResponseBodyApplicationJson,
-        SchemaFor200ResponseBodyTextJson,
-    ]
+    body: InstallmentPlanSearchResponse
+
+
+@dataclass
+class ApiResponseFor200Async(api_client.AsyncApiResponse):
+    body: InstallmentPlanSearchResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
+    response_cls_async=ApiResponseFor200Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor200ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyTextJson),
     },
 )
-SchemaFor401ResponseBodyTextPlain = FailedResponse
-SchemaFor401ResponseBodyApplicationJson = FailedResponse
-SchemaFor401ResponseBodyTextJson = FailedResponse
+SchemaFor401ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor401ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor401ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor401ResponseBodyTextPlain,
-        SchemaFor401ResponseBodyApplicationJson,
-        SchemaFor401ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor401Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
+    response_cls_async=ApiResponseFor401Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor401ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyTextJson),
     },
 )
-SchemaFor403ResponseBodyTextPlain = FailedResponse
-SchemaFor403ResponseBodyApplicationJson = FailedResponse
-SchemaFor403ResponseBodyTextJson = FailedResponse
+SchemaFor403ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor403ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor403ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor403ResponseBodyTextPlain,
-        SchemaFor403ResponseBodyApplicationJson,
-        SchemaFor403ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor403Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
+    response_cls_async=ApiResponseFor403Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor403ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyTextJson),
     },
 )
-SchemaFor404ResponseBodyTextPlain = FailedResponse
-SchemaFor404ResponseBodyApplicationJson = FailedResponse
-SchemaFor404ResponseBodyTextJson = FailedResponse
+SchemaFor404ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor404ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor404ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor404ResponseBodyTextPlain,
-        SchemaFor404ResponseBodyApplicationJson,
-        SchemaFor404ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor404Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
+    response_cls_async=ApiResponseFor404Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor404ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyTextJson),
     },
 )
-SchemaFor500ResponseBodyTextPlain = FailedResponse
-SchemaFor500ResponseBodyApplicationJson = FailedResponse
-SchemaFor500ResponseBodyTextJson = FailedResponse
+SchemaFor500ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor500ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor500ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor500(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor500ResponseBodyTextPlain,
-        SchemaFor500ResponseBodyApplicationJson,
-        SchemaFor500ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor500Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_500 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor500,
+    response_cls_async=ApiResponseFor500Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextJson),
@@ -225,243 +283,309 @@
     'text/plain',
     'application/json',
     'text/json',
 )
 
 
 class BaseApi(api_client.Api):
-    @typing.overload
-    def _cancel_oapg(
+
+    def _search_mapped_args(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+        x_splitit_idempotency_key: str,
+        installment_plan_number: typing.Optional[str] = None,
+        ref_order_number: typing.Optional[str] = None,
+        extended_params: typing.Optional[typing.Dict[str, str]] = None,
+    ) -> api_client.MappedArgs:
+        args: api_client.MappedArgs = api_client.MappedArgs()
+        _query_params = {}
+        _header_params = {}
+        if installment_plan_number is not None:
+            _query_params["installmentPlanNumber"] = installment_plan_number
+        if ref_order_number is not None:
+            _query_params["refOrderNumber"] = ref_order_number
+        if extended_params is not None:
+            _query_params["extendedParams"] = extended_params
+        if x_splitit_idempotency_key is not None:
+            _header_params["X-Splitit-IdempotencyKey"] = x_splitit_idempotency_key
+        args.query = _query_params
+        args.header = _header_params
+        return args
 
-    @typing.overload
-    def _cancel_oapg(
+    async def _asearch_oapg(
         self,
-        skip_deserialization: typing_extensions.Literal[True],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
+            query_params: typing.Optional[dict] = {},
+            header_params: typing.Optional[dict] = {},
+        skip_deserialization: bool = True,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
+    ) -> typing.Union[
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        """
+        :param skip_deserialization: If true then api_response.response will be set but
+            api_response.body and api_response.headers will not be deserialized into schema
+            class instances
+        """
+        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
+        self._verify_typed_dict_inputs_oapg(RequestHeaderParams, header_params)
+        used_path = path.value
+    
+        prefix_separator_iterator = None
+        for parameter in (
+            request_query_installment_plan_number,
+            request_query_ref_order_number,
+            request_query_extended_params,
+        ):
+            parameter_data = query_params.get(parameter.name, schemas.unset)
+            if parameter_data is schemas.unset:
+                continue
+            if prefix_separator_iterator is None:
+                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
+            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
+            for serialized_value in serialized_data.values():
+                used_path += serialized_value
+    
+        _headers = HTTPHeaderDict()
+        for parameter in (
+            request_header_x_splitit_idempotency_key,
+        ):
+            parameter_data = header_params.get(parameter.name, schemas.unset)
+            if parameter_data is schemas.unset:
+                continue
+            serialized_data = parameter.serialize(parameter_data)
+            _headers.extend(serialized_data)
+        # TODO add cookie handling
+        if accept_content_types:
+            for accept_content_type in accept_content_types:
+                _headers.add('Accept', accept_content_type)
+    
+        response = await self.api_client.async_call_api(
+            resource_path=used_path,
+            method='get'.upper(),
+            headers=_headers,
+            auth_settings=_auth,
+            prefix_separator_iterator=prefix_separator_iterator,
+            timeout=timeout,
+        )
+        
+        if stream:
+            async def stream_iterator():
+                """
+                iterates over response.http_response.content and closes connection once iteration has finished
+                """
+                async for line in response.http_response.content:
+                    if line == b'\r\n':
+                        continue
+                    yield line
+                response.http_response.close()
+                await response.session.close()
+            return AsyncGeneratorResponse(
+                content=stream_iterator(),
+                headers=response.http_response.headers,
+                status=response.http_response.status,
+                response=response.http_response
+            )
+    
+        response_for_status = _status_code_to_response.get(str(response.http_response.status))
+        if response_for_status:
+            api_response = await response_for_status.deserialize_async(
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
+        else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
+            api_response = api_client.ApiResponseWithoutDeserializationAsync(
+                body=await response.http_response.json() if is_json else await response.http_response.text(),
+                response=response.http_response,
+                round_trip_time=response.round_trip_time,
+                status=response.http_response.status,
+                headers=response.http_response.headers,
+            )
+    
+        if not 200 <= api_response.status <= 299:
+            raise exceptions.ApiException(api_response=api_response)
+    
+        # cleanup session / response
+        response.http_response.close()
+        await response.session.close()
+    
+        return api_response
 
-    @typing.overload
-    def _cancel_oapg(
+    def _search_oapg(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
+            query_params: typing.Optional[dict] = {},
+            header_params: typing.Optional[dict] = {},
+        skip_deserialization: bool = True,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def _cancel_oapg(
-        self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
+    ]:
         """
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
+        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestHeaderParams, header_params)
-        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
-
-        _path_params = {}
+    
+        prefix_separator_iterator = None
         for parameter in (
-            request_path_installment_plan_number,
+            request_query_installment_plan_number,
+            request_query_ref_order_number,
+            request_query_extended_params,
         ):
-            parameter_data = path_params.get(parameter.name, schemas.unset)
+            parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
-            serialized_data = parameter.serialize(parameter_data)
-            _path_params.update(serialized_data)
-
-        for k, v in _path_params.items():
-            used_path = used_path.replace('{%s}' % k, v)
-
+            if prefix_separator_iterator is None:
+                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
+            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
+            for serialized_value in serialized_data.values():
+                used_path += serialized_value
+    
         _headers = HTTPHeaderDict()
         for parameter in (
             request_header_x_splitit_idempotency_key,
         ):
             parameter_data = header_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _headers.extend(serialized_data)
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-
+    
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='post'.upper(),
+            method='get'.upper(),
             headers=_headers,
             auth_settings=_auth,
-            stream=stream,
+            prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
-
+    
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
-                                                   response,
-                                                   self.api_client.configuration,
-                                                   skip_deserialization=skip_deserialization
-                                               )
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
         else:
             # If response data is JSON then deserialize for SDK consumer convenience
             is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
                 body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
-
+    
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
-
+    
         return api_response
 
-
-class Cancel(BaseApi):
+class Search(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    @typing.overload
-    def cancel(
+    async def asearch(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        x_splitit_idempotency_key: str,
+        installment_plan_number: typing.Optional[str] = None,
+        ref_order_number: typing.Optional[str] = None,
+        extended_params: typing.Optional[typing.Dict[str, str]] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def cancel(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def cancel(
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._search_mapped_args(
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            installment_plan_number=installment_plan_number,
+            ref_order_number=ref_order_number,
+            extended_params=extended_params,
+        )
+        return await self._asearch_oapg(
+            query_params=args.query,
+            header_params=args.header,
+        )
+    
+    def search(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        x_splitit_idempotency_key: str,
+        installment_plan_number: typing.Optional[str] = None,
+        ref_order_number: typing.Optional[str] = None,
+        extended_params: typing.Optional[typing.Dict[str, str]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def cancel(
-        self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._cancel_oapg(
-            header_params=header_params,
-            path_params=path_params,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+    ]:
+        args = self._search_mapped_args(
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            installment_plan_number=installment_plan_number,
+            ref_order_number=ref_order_number,
+            extended_params=extended_params,
+        )
+        return self._search_oapg(
+            query_params=args.query,
+            header_params=args.header,
         )
 
-
-class ApiForpost(BaseApi):
+class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    @typing.overload
-    def post(
+    async def aget(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        x_splitit_idempotency_key: str,
+        installment_plan_number: typing.Optional[str] = None,
+        ref_order_number: typing.Optional[str] = None,
+        extended_params: typing.Optional[typing.Dict[str, str]] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def post(
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._search_mapped_args(
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            installment_plan_number=installment_plan_number,
+            ref_order_number=ref_order_number,
+            extended_params=extended_params,
+        )
+        return await self._asearch_oapg(
+            query_params=args.query,
+            header_params=args.header,
+        )
+    
+    def get(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        x_splitit_idempotency_key: str,
+        installment_plan_number: typing.Optional[str] = None,
+        ref_order_number: typing.Optional[str] = None,
+        extended_params: typing.Optional[typing.Dict[str, str]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def post(
-        self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._cancel_oapg(
-            header_params=header_params,
-            path_params=path_params,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+    ]:
+        args = self._search_mapped_args(
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            installment_plan_number=installment_plan_number,
+            ref_order_number=ref_order_number,
+            extended_params=extended_params,
+        )
+        return self._search_oapg(
+            query_params=args.query,
+            header_params=args.header,
         )
-
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_installment_plan_number_verifyauthorization/get.py` & `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_installment_plan_number/get.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,30 +11,34 @@
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
 import json
 from urllib3._collections import HTTPHeaderDict
 
+from splitit_client.api_response import AsyncGeneratorResponse
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
-from splitit_client.model.verify_authorization_response import VerifyAuthorizationResponse
-from splitit_client.model.failed_response import FailedResponse
+from splitit_client.model.failed_response import FailedResponse as FailedResponseSchema
+from splitit_client.model.installment_plan_get_response import InstallmentPlanGetResponse as InstallmentPlanGetResponseSchema
+
+from splitit_client.type.failed_response import FailedResponse
+from splitit_client.type.installment_plan_get_response import InstallmentPlanGetResponse
 
 from . import path
 
 # Header params
 XSplititIdempotencyKeySchema = schemas.StrSchema
 RequestRequiredHeaderParams = typing_extensions.TypedDict(
     'RequestRequiredHeaderParams',
@@ -85,130 +89,140 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=InstallmentPlanNumberSchema,
     required=True,
 )
 _auth = [
     'oauth',
 ]
-SchemaFor200ResponseBodyTextPlain = VerifyAuthorizationResponse
-SchemaFor200ResponseBodyApplicationJson = VerifyAuthorizationResponse
-SchemaFor200ResponseBodyTextJson = VerifyAuthorizationResponse
+SchemaFor200ResponseBodyTextPlain = InstallmentPlanGetResponseSchema
+SchemaFor200ResponseBodyApplicationJson = InstallmentPlanGetResponseSchema
+SchemaFor200ResponseBodyTextJson = InstallmentPlanGetResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor200ResponseBodyTextPlain,
-        SchemaFor200ResponseBodyApplicationJson,
-        SchemaFor200ResponseBodyTextJson,
-    ]
+    body: InstallmentPlanGetResponse
+
+
+@dataclass
+class ApiResponseFor200Async(api_client.AsyncApiResponse):
+    body: InstallmentPlanGetResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
+    response_cls_async=ApiResponseFor200Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor200ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyTextJson),
     },
 )
-SchemaFor401ResponseBodyTextPlain = FailedResponse
-SchemaFor401ResponseBodyApplicationJson = FailedResponse
-SchemaFor401ResponseBodyTextJson = FailedResponse
+SchemaFor401ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor401ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor401ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor401ResponseBodyTextPlain,
-        SchemaFor401ResponseBodyApplicationJson,
-        SchemaFor401ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor401Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
+    response_cls_async=ApiResponseFor401Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor401ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyTextJson),
     },
 )
-SchemaFor403ResponseBodyTextPlain = FailedResponse
-SchemaFor403ResponseBodyApplicationJson = FailedResponse
-SchemaFor403ResponseBodyTextJson = FailedResponse
+SchemaFor403ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor403ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor403ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor403ResponseBodyTextPlain,
-        SchemaFor403ResponseBodyApplicationJson,
-        SchemaFor403ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor403Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
+    response_cls_async=ApiResponseFor403Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor403ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyTextJson),
     },
 )
-SchemaFor404ResponseBodyTextPlain = FailedResponse
-SchemaFor404ResponseBodyApplicationJson = FailedResponse
-SchemaFor404ResponseBodyTextJson = FailedResponse
+SchemaFor404ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor404ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor404ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor404ResponseBodyTextPlain,
-        SchemaFor404ResponseBodyApplicationJson,
-        SchemaFor404ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor404Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
+    response_cls_async=ApiResponseFor404Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor404ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyTextJson),
     },
 )
-SchemaFor500ResponseBodyTextPlain = FailedResponse
-SchemaFor500ResponseBodyApplicationJson = FailedResponse
-SchemaFor500ResponseBodyTextJson = FailedResponse
+SchemaFor500ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor500ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor500ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor500(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor500ResponseBodyTextPlain,
-        SchemaFor500ResponseBodyApplicationJson,
-        SchemaFor500ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor500Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_500 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor500,
+    response_cls_async=ApiResponseFor500Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextJson),
@@ -225,243 +239,281 @@
     'text/plain',
     'application/json',
     'text/json',
 )
 
 
 class BaseApi(api_client.Api):
-    @typing.overload
-    def _verify_authorization_oapg(
+
+    def _get_mapped_args(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+        installment_plan_number: str,
+        x_splitit_idempotency_key: str,
+    ) -> api_client.MappedArgs:
+        args: api_client.MappedArgs = api_client.MappedArgs()
+        _header_params = {}
+        _path_params = {}
+        if x_splitit_idempotency_key is not None:
+            _header_params["X-Splitit-IdempotencyKey"] = x_splitit_idempotency_key
+        if installment_plan_number is not None:
+            _path_params["installmentPlanNumber"] = installment_plan_number
+        args.header = _header_params
+        args.path = _path_params
+        return args
 
-    @typing.overload
-    def _verify_authorization_oapg(
+    async def _aget_oapg(
         self,
-        skip_deserialization: typing_extensions.Literal[True],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
+            header_params: typing.Optional[dict] = {},
+            path_params: typing.Optional[dict] = {},
+        skip_deserialization: bool = True,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
+    ) -> typing.Union[
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        """
+        :param skip_deserialization: If true then api_response.response will be set but
+            api_response.body and api_response.headers will not be deserialized into schema
+            class instances
+        """
+        self._verify_typed_dict_inputs_oapg(RequestHeaderParams, header_params)
+        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
+        used_path = path.value
+    
+        _path_params = {}
+        for parameter in (
+            request_path_installment_plan_number,
+        ):
+            parameter_data = path_params.get(parameter.name, schemas.unset)
+            if parameter_data is schemas.unset:
+                continue
+            serialized_data = parameter.serialize(parameter_data)
+            _path_params.update(serialized_data)
+    
+        for k, v in _path_params.items():
+            used_path = used_path.replace('{%s}' % k, v)
+    
+        _headers = HTTPHeaderDict()
+        for parameter in (
+            request_header_x_splitit_idempotency_key,
+        ):
+            parameter_data = header_params.get(parameter.name, schemas.unset)
+            if parameter_data is schemas.unset:
+                continue
+            serialized_data = parameter.serialize(parameter_data)
+            _headers.extend(serialized_data)
+        # TODO add cookie handling
+        if accept_content_types:
+            for accept_content_type in accept_content_types:
+                _headers.add('Accept', accept_content_type)
+    
+        response = await self.api_client.async_call_api(
+            resource_path=used_path,
+            method='get'.upper(),
+            headers=_headers,
+            auth_settings=_auth,
+            timeout=timeout,
+        )
+        
+        if stream:
+            async def stream_iterator():
+                """
+                iterates over response.http_response.content and closes connection once iteration has finished
+                """
+                async for line in response.http_response.content:
+                    if line == b'\r\n':
+                        continue
+                    yield line
+                response.http_response.close()
+                await response.session.close()
+            return AsyncGeneratorResponse(
+                content=stream_iterator(),
+                headers=response.http_response.headers,
+                status=response.http_response.status,
+                response=response.http_response
+            )
+    
+        response_for_status = _status_code_to_response.get(str(response.http_response.status))
+        if response_for_status:
+            api_response = await response_for_status.deserialize_async(
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
+        else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
+            api_response = api_client.ApiResponseWithoutDeserializationAsync(
+                body=await response.http_response.json() if is_json else await response.http_response.text(),
+                response=response.http_response,
+                round_trip_time=response.round_trip_time,
+                status=response.http_response.status,
+                headers=response.http_response.headers,
+            )
+    
+        if not 200 <= api_response.status <= 299:
+            raise exceptions.ApiException(api_response=api_response)
+    
+        # cleanup session / response
+        response.http_response.close()
+        await response.session.close()
+    
+        return api_response
 
-    @typing.overload
-    def _verify_authorization_oapg(
+    def _get_oapg(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
+            header_params: typing.Optional[dict] = {},
+            path_params: typing.Optional[dict] = {},
+        skip_deserialization: bool = True,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def _verify_authorization_oapg(
-        self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
+    ]:
         """
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestHeaderParams, header_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
-
+    
         _path_params = {}
         for parameter in (
             request_path_installment_plan_number,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
-
+    
         for k, v in _path_params.items():
             used_path = used_path.replace('{%s}' % k, v)
-
+    
         _headers = HTTPHeaderDict()
         for parameter in (
             request_header_x_splitit_idempotency_key,
         ):
             parameter_data = header_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _headers.extend(serialized_data)
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-
+    
         response = self.api_client.call_api(
             resource_path=used_path,
             method='get'.upper(),
             headers=_headers,
             auth_settings=_auth,
-            stream=stream,
             timeout=timeout,
         )
-
+    
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
-                                                   response,
-                                                   self.api_client.configuration,
-                                                   skip_deserialization=skip_deserialization
-                                               )
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
         else:
             # If response data is JSON then deserialize for SDK consumer convenience
             is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
                 body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
-
+    
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
-
+    
         return api_response
 
-
-class VerifyAuthorization(BaseApi):
+class Get(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    @typing.overload
-    def verify_authorization(
+    async def aget(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        installment_plan_number: str,
+        x_splitit_idempotency_key: str,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def verify_authorization(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def verify_authorization(
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._get_mapped_args(
+            installment_plan_number=installment_plan_number,
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+        )
+        return await self._aget_oapg(
+            header_params=args.header,
+            path_params=args.path,
+        )
+    
+    def get(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        installment_plan_number: str,
+        x_splitit_idempotency_key: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def verify_authorization(
-        self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._verify_authorization_oapg(
-            header_params=header_params,
-            path_params=path_params,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+    ]:
+        args = self._get_mapped_args(
+            installment_plan_number=installment_plan_number,
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+        )
+        return self._get_oapg(
+            header_params=args.header,
+            path_params=args.path,
         )
-
 
 class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    @typing.overload
-    def get(
+    async def aget(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        installment_plan_number: str,
+        x_splitit_idempotency_key: str,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def get(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._get_mapped_args(
+            installment_plan_number=installment_plan_number,
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+        )
+        return await self._aget_oapg(
+            header_params=args.header,
+            path_params=args.path,
+        )
+    
     def get(
         self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        installment_plan_number: str,
+        x_splitit_idempotency_key: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def get(
-        self,
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._verify_authorization_oapg(
-            header_params=header_params,
-            path_params=path_params,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+    ]:
+        args = self._get_mapped_args(
+            installment_plan_number=installment_plan_number,
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+        )
+        return self._get_oapg(
+            header_params=args.header,
+            path_params=args.path,
         )
-
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/paths/api_installmentplans_search/get.py` & `splitit_web_python_sdk-2.2.0/splitit_client/paths/api_installmentplans_check_eligibility/post.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,103 +11,45 @@
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
 import json
 from urllib3._collections import HTTPHeaderDict
 
+from splitit_client.api_response import AsyncGeneratorResponse
 from splitit_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from splitit_client import schemas  # noqa: F401
 
-from splitit_client.model.failed_response import FailedResponse
-from splitit_client.model.installment_plan_search_response import InstallmentPlanSearchResponse
+from splitit_client.model.plan_data import PlanData as PlanDataSchema
+from splitit_client.model.failed_response import FailedResponse as FailedResponseSchema
+from splitit_client.model.card_data import CardData as CardDataSchema
+from splitit_client.model.address_data import AddressData as AddressDataSchema
+from splitit_client.model.check_installments_eligibility_request import CheckInstallmentsEligibilityRequest as CheckInstallmentsEligibilityRequestSchema
+from splitit_client.model.installments_eligibility_response import InstallmentsEligibilityResponse as InstallmentsEligibilityResponseSchema
+
+from splitit_client.type.failed_response import FailedResponse
+from splitit_client.type.address_data import AddressData
+from splitit_client.type.installments_eligibility_response import InstallmentsEligibilityResponse
+from splitit_client.type.card_data import CardData
+from splitit_client.type.plan_data import PlanData
+from splitit_client.type.check_installments_eligibility_request import CheckInstallmentsEligibilityRequest
 
 from . import path
 
-# Query params
-InstallmentPlanNumberSchema = schemas.StrSchema
-RefOrderNumberSchema = schemas.StrSchema
-
-
-class ExtendedParamsSchema(
-    schemas.DictSchema
-):
-
-
-    class MetaOapg:
-        additional_properties = schemas.StrSchema
-    
-    def __getitem__(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    def get_item_oapg(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
-        return super().get_item_oapg(name)
-
-    def __new__(
-        cls,
-        *args: typing.Union[dict, frozendict.frozendict, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[MetaOapg.additional_properties, str, ],
-    ) -> 'ExtendedParamsSchema':
-        return super().__new__(
-            cls,
-            *args,
-            _configuration=_configuration,
-            **kwargs,
-        )
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
-    {
-    }
-)
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
-    {
-        'installmentPlanNumber': typing.Union[InstallmentPlanNumberSchema, str, ],
-        'refOrderNumber': typing.Union[RefOrderNumberSchema, str, ],
-        'extendedParams': typing.Union[ExtendedParamsSchema, dict, frozendict.frozendict, ],
-    },
-    total=False
-)
-
-
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
-    pass
-
-
-request_query_installment_plan_number = api_client.QueryParameter(
-    name="installmentPlanNumber",
-    style=api_client.ParameterStyle.FORM,
-    schema=InstallmentPlanNumberSchema,
-    explode=True,
-)
-request_query_ref_order_number = api_client.QueryParameter(
-    name="refOrderNumber",
-    style=api_client.ParameterStyle.FORM,
-    schema=RefOrderNumberSchema,
-    explode=True,
-)
-request_query_extended_params = api_client.QueryParameter(
-    name="extendedParams",
-    style=api_client.ParameterStyle.FORM,
-    schema=ExtendedParamsSchema,
-    explode=True,
-)
 # Header params
 XSplititIdempotencyKeySchema = schemas.StrSchema
 RequestRequiredHeaderParams = typing_extensions.TypedDict(
     'RequestRequiredHeaderParams',
     {
         'X-Splitit-IdempotencyKey': typing.Union[XSplititIdempotencyKeySchema, str, ],
     }
@@ -126,133 +68,163 @@
 
 request_header_x_splitit_idempotency_key = api_client.HeaderParameter(
     name="X-Splitit-IdempotencyKey",
     style=api_client.ParameterStyle.SIMPLE,
     schema=XSplititIdempotencyKeySchema,
     required=True,
 )
+# body param
+SchemaForRequestBodyApplicationJsonPatchjson = CheckInstallmentsEligibilityRequestSchema
+SchemaForRequestBodyApplicationJson = CheckInstallmentsEligibilityRequestSchema
+SchemaForRequestBodyTextJson = CheckInstallmentsEligibilityRequestSchema
+SchemaForRequestBodyApplicationJson = CheckInstallmentsEligibilityRequestSchema
+
+
+request_body_check_installments_eligibility_request = api_client.RequestBody(
+    content={
+        'application/json-patch+json': api_client.MediaType(
+            schema=SchemaForRequestBodyApplicationJsonPatchjson),
+        'application/json': api_client.MediaType(
+            schema=SchemaForRequestBodyApplicationJson),
+        'text/json': api_client.MediaType(
+            schema=SchemaForRequestBodyTextJson),
+        'application/*+json': api_client.MediaType(
+            schema=SchemaForRequestBodyApplicationJson),
+    },
+    required=True,
+)
 _auth = [
     'oauth',
 ]
-SchemaFor200ResponseBodyTextPlain = InstallmentPlanSearchResponse
-SchemaFor200ResponseBodyApplicationJson = InstallmentPlanSearchResponse
-SchemaFor200ResponseBodyTextJson = InstallmentPlanSearchResponse
+SchemaFor200ResponseBodyTextPlain = InstallmentsEligibilityResponseSchema
+SchemaFor200ResponseBodyApplicationJson = InstallmentsEligibilityResponseSchema
+SchemaFor200ResponseBodyTextJson = InstallmentsEligibilityResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor200ResponseBodyTextPlain,
-        SchemaFor200ResponseBodyApplicationJson,
-        SchemaFor200ResponseBodyTextJson,
-    ]
+    body: InstallmentsEligibilityResponse
+
+
+@dataclass
+class ApiResponseFor200Async(api_client.AsyncApiResponse):
+    body: InstallmentsEligibilityResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
+    response_cls_async=ApiResponseFor200Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor200ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyTextJson),
     },
 )
-SchemaFor401ResponseBodyTextPlain = FailedResponse
-SchemaFor401ResponseBodyApplicationJson = FailedResponse
-SchemaFor401ResponseBodyTextJson = FailedResponse
+SchemaFor401ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor401ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor401ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor401ResponseBodyTextPlain,
-        SchemaFor401ResponseBodyApplicationJson,
-        SchemaFor401ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor401Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
+    response_cls_async=ApiResponseFor401Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor401ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyTextJson),
     },
 )
-SchemaFor403ResponseBodyTextPlain = FailedResponse
-SchemaFor403ResponseBodyApplicationJson = FailedResponse
-SchemaFor403ResponseBodyTextJson = FailedResponse
+SchemaFor403ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor403ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor403ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor403ResponseBodyTextPlain,
-        SchemaFor403ResponseBodyApplicationJson,
-        SchemaFor403ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor403Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
+    response_cls_async=ApiResponseFor403Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor403ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyTextJson),
     },
 )
-SchemaFor404ResponseBodyTextPlain = FailedResponse
-SchemaFor404ResponseBodyApplicationJson = FailedResponse
-SchemaFor404ResponseBodyTextJson = FailedResponse
+SchemaFor404ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor404ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor404ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor404ResponseBodyTextPlain,
-        SchemaFor404ResponseBodyApplicationJson,
-        SchemaFor404ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor404Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
+    response_cls_async=ApiResponseFor404Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor404ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyTextJson),
     },
 )
-SchemaFor500ResponseBodyTextPlain = FailedResponse
-SchemaFor500ResponseBodyApplicationJson = FailedResponse
-SchemaFor500ResponseBodyTextJson = FailedResponse
+SchemaFor500ResponseBodyTextPlain = FailedResponseSchema
+SchemaFor500ResponseBodyApplicationJson = FailedResponseSchema
+SchemaFor500ResponseBodyTextJson = FailedResponseSchema
 
 
 @dataclass
 class ApiResponseFor500(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor500ResponseBodyTextPlain,
-        SchemaFor500ResponseBodyApplicationJson,
-        SchemaFor500ResponseBodyTextJson,
-    ]
+    body: FailedResponse
+
+
+@dataclass
+class ApiResponseFor500Async(api_client.AsyncApiResponse):
+    body: FailedResponse
 
 
 _response_for_500 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor500,
+    response_cls_async=ApiResponseFor500Async,
     content={
         'text/plain': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextPlain),
         'application/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyApplicationJson),
         'text/json': api_client.MediaType(
             schema=SchemaFor500ResponseBodyTextJson),
@@ -269,246 +241,305 @@
     'text/plain',
     'application/json',
     'text/json',
 )
 
 
 class BaseApi(api_client.Api):
-    @typing.overload
-    def _search_oapg(
-        self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
 
-    @typing.overload
-    def _search_oapg(
+    def _check_eligibility_mapped_args(
         self,
-        skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
+        x_splitit_idempotency_key: str,
+        plan_data: typing.Optional[PlanData] = None,
+        card_details: typing.Optional[CardData] = None,
+        billing_address: typing.Optional[AddressData] = None,
+    ) -> api_client.MappedArgs:
+        args: api_client.MappedArgs = api_client.MappedArgs()
+        _header_params = {}
+        _body = {}
+        if plan_data is not None:
+            _body["PlanData"] = plan_data
+        if card_details is not None:
+            _body["CardDetails"] = card_details
+        if billing_address is not None:
+            _body["BillingAddress"] = billing_address
+        args.body = _body
+        if x_splitit_idempotency_key is not None:
+            _header_params["X-Splitit-IdempotencyKey"] = x_splitit_idempotency_key
+        args.header = _header_params
+        return args
 
-    @typing.overload
-    def _search_oapg(
+    async def _acheck_eligibility_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
+        body: typing.Any = None,
+            header_params: typing.Optional[dict] = {},
+        skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-        api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def _search_oapg(
-        self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
-        header_params: RequestHeaderParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'application/json-patch+json',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
+    ) -> typing.Union[
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
         """
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestHeaderParams, header_params)
         used_path = path.value
-
-        prefix_separator_iterator = None
+    
+        _headers = HTTPHeaderDict()
         for parameter in (
-            request_query_installment_plan_number,
-            request_query_ref_order_number,
-            request_query_extended_params,
+            request_header_x_splitit_idempotency_key,
         ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
+            parameter_data = header_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
+            serialized_data = parameter.serialize(parameter_data)
+            _headers.extend(serialized_data)
+        # TODO add cookie handling
+        if accept_content_types:
+            for accept_content_type in accept_content_types:
+                _headers.add('Accept', accept_content_type)
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_check_installments_eligibility_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
+        response = await self.api_client.async_call_api(
+            resource_path=used_path,
+            method='post'.upper(),
+            headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
+            auth_settings=_auth,
+            timeout=timeout,
+        )
+        
+        if stream:
+            async def stream_iterator():
+                """
+                iterates over response.http_response.content and closes connection once iteration has finished
+                """
+                async for line in response.http_response.content:
+                    if line == b'\r\n':
+                        continue
+                    yield line
+                response.http_response.close()
+                await response.session.close()
+            return AsyncGeneratorResponse(
+                content=stream_iterator(),
+                headers=response.http_response.headers,
+                status=response.http_response.status,
+                response=response.http_response
+            )
+    
+        response_for_status = _status_code_to_response.get(str(response.http_response.status))
+        if response_for_status:
+            api_response = await response_for_status.deserialize_async(
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
+        else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
+            api_response = api_client.ApiResponseWithoutDeserializationAsync(
+                body=await response.http_response.json() if is_json else await response.http_response.text(),
+                response=response.http_response,
+                round_trip_time=response.round_trip_time,
+                status=response.http_response.status,
+                headers=response.http_response.headers,
+            )
+    
+        if not 200 <= api_response.status <= 299:
+            raise exceptions.ApiException(api_response=api_response)
+    
+        # cleanup session / response
+        response.http_response.close()
+        await response.session.close()
+    
+        return api_response
 
+    def _check_eligibility_oapg(
+        self,
+        body: typing.Any = None,
+            header_params: typing.Optional[dict] = {},
+        skip_deserialization: bool = True,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'application/json-patch+json',
+        stream: bool = False,
+    ) -> typing.Union[
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]:
+        """
+        :param skip_deserialization: If true then api_response.response will be set but
+            api_response.body and api_response.headers will not be deserialized into schema
+            class instances
+        """
+        self._verify_typed_dict_inputs_oapg(RequestHeaderParams, header_params)
+        used_path = path.value
+    
         _headers = HTTPHeaderDict()
         for parameter in (
             request_header_x_splitit_idempotency_key,
         ):
             parameter_data = header_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _headers.extend(serialized_data)
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_check_installments_eligibility_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='post'.upper(),
             headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
             auth_settings=_auth,
-            prefix_separator_iterator=prefix_separator_iterator,
-            stream=stream,
             timeout=timeout,
         )
-
+    
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
-                                                   response,
-                                                   self.api_client.configuration,
-                                                   skip_deserialization=skip_deserialization
-                                               )
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
         else:
             # If response data is JSON then deserialize for SDK consumer convenience
             is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
                 body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
-
+    
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
-
+    
         return api_response
 
-
-class Search(BaseApi):
+class CheckEligibility(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    @typing.overload
-    def search(
+    async def acheck_eligibility(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        x_splitit_idempotency_key: str,
+        plan_data: typing.Optional[PlanData] = None,
+        card_details: typing.Optional[CardData] = None,
+        billing_address: typing.Optional[AddressData] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def search(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def search(
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._check_eligibility_mapped_args(
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            plan_data=plan_data,
+            card_details=card_details,
+            billing_address=billing_address,
+        )
+        return await self._acheck_eligibility_oapg(
+            body=args.body,
+            header_params=args.header,
+        )
+    
+    def check_eligibility(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        x_splitit_idempotency_key: str,
+        plan_data: typing.Optional[PlanData] = None,
+        card_details: typing.Optional[CardData] = None,
+        billing_address: typing.Optional[AddressData] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def search(
-        self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._search_oapg(
-            query_params=query_params,
-            header_params=header_params,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+    ]:
+        args = self._check_eligibility_mapped_args(
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            plan_data=plan_data,
+            card_details=card_details,
+            billing_address=billing_address,
+        )
+        return self._check_eligibility_oapg(
+            body=args.body,
+            header_params=args.header,
         )
 
-
-class ApiForget(BaseApi):
+class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    @typing.overload
-    def get(
+    async def apost(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        x_splitit_idempotency_key: str,
+        plan_data: typing.Optional[PlanData] = None,
+        card_details: typing.Optional[CardData] = None,
+        billing_address: typing.Optional[AddressData] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def get(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def get(
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._check_eligibility_mapped_args(
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            plan_data=plan_data,
+            card_details=card_details,
+            billing_address=billing_address,
+        )
+        return await self._acheck_eligibility_oapg(
+            body=args.body,
+            header_params=args.header,
+        )
+    
+    def post(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        x_splitit_idempotency_key: str,
+        plan_data: typing.Optional[PlanData] = None,
+        card_details: typing.Optional[CardData] = None,
+        billing_address: typing.Optional[AddressData] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def get(
-        self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
-        header_params: RequestHeaderParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._search_oapg(
-            query_params=query_params,
-            header_params=header_params,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+    ]:
+        args = self._check_eligibility_mapped_args(
+            x_splitit_idempotency_key=x_splitit_idempotency_key,
+            plan_data=plan_data,
+            card_details=card_details,
+            billing_address=billing_address,
+        )
+        return self._check_eligibility_oapg(
+            body=args.body,
+            header_params=args.header,
         )
-
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/request_after_hook.py` & `splitit_web_python_sdk-2.2.0/splitit_client/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/request_before_hook.py` & `splitit_web_python_sdk-2.2.0/splitit_client/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/rest.py` & `splitit_web_python_sdk-2.2.0/splitit_client/rest.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,30 +10,37 @@
 """
 
 
 import logging
 import ssl
 from urllib.parse import urlencode
 import typing
+import aiohttp
 
 import certifi
 import urllib3
 import time
 from urllib3._collections import HTTPHeaderDict
 
 from splitit_client.exceptions import ApiException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 class ResponseWrapper:
-    def __init__(self, http_response: urllib3.HTTPResponse, round_trip_time: int):
+    def __init__(self, http_response: urllib3.HTTPResponse, round_trip_time: float):
         self.http_response = http_response
         self.round_trip_time = round_trip_time
 
+class AsyncResponseWrapper:
+    def __init__(self, http_response: aiohttp.ClientResponse, round_trip_time: float, session: aiohttp.ClientSession):
+        self.http_response = http_response
+        self.round_trip_time = round_trip_time
+        self.session = session
+
 class RESTClientObject(object):
 
     def __init__(self, configuration, pools_size=4, maxsize=None):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680
         # maxsize is the number of requests to host that are allowed in parallel
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/schemas.py` & `splitit_web_python_sdk-2.2.0/splitit_client/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from datetime import date, datetime, timedelta  # noqa: F401
 import functools
 import decimal
 import io
 import re
 import types
 import typing
+import typing_extensions
 import uuid
 
 from dateutil.parser.isoparser import isoparser, _takes_ascii
 import frozendict
 
 from splitit_client.exceptions_base import (
     ApiTypeError,
@@ -28,15 +29,18 @@
 )
 from splitit_client.configuration import (
     Configuration,
 )
 from splitit_client.exceptions import SchemaValidationError
 from splitit_client.exceptions import render_path
 from splitit_client.validation_metadata import ValidationMetadata
+from splitit_client.exceptions import AnyOfValidationError
+from splitit_client.exceptions import MissingRequiredPropertiesError
 
+Primitive: typing_extensions.TypeAlias = typing.Union[int, float, bool, str]
 
 class Unset(object):
     """
     An instance of this class is set as the default value for object type(dict) properties that are optional
     When a property has an unset value, that property will not be assigned in the dict
     """
     pass
@@ -169,17 +173,17 @@
     class properties:
         # to hold object properties
         pass
 
     additional_properties: typing.Optional[typing.Type['Schema']]
     max_properties: int
     min_properties: int
-    all_of: typing.List[typing.Type['Schema']]
-    one_of: typing.List[typing.Type['Schema']]
-    any_of: typing.List[typing.Type['Schema']]
+    all_of: typing.Callable[[], typing.List[typing.Type['Schema']]]
+    one_of: typing.Callable[[], typing.List[typing.Type['Schema']]]
+    any_of: typing.Callable[[], typing.List[typing.Type['Schema']]]
     not_schema: typing.Type['Schema']
     max_length: int
     min_length: int
     items: typing.Type['Schema']
 
 
 class Schema:
@@ -446,35 +450,35 @@
             kwargs (str, int/float/decimal.Decimal/str/list/tuple/dict/frozendict.frozendict/bool/None): dict values
             _configuration: contains the Configuration that enables json schema validation keywords
                 like minItems, minLength etc
 
         Note: double underscores are used here because pycharm thinks that these variables
         are instance properties if they are named normally :(
         """
-        __kwargs = cls.__remove_unsets(kwargs)
-        if not args and not __kwargs:
+        _kwargs = cls.__remove_unsets(kwargs)
+        if not args and not _kwargs:
             raise TypeError(
                 'No input given. args or kwargs must be given.'
             )
-        if not __kwargs and args and not isinstance(args[0], dict):
-            __arg = args[0]
+        if not _kwargs and args and not isinstance(args[0], dict):
+            _arg = args[0]
         else:
-            __arg = cls.__get_input_dict(*args, **__kwargs)
-        __from_server = False
-        __validated_path_to_schemas = {}
-        __arg = cast_to_allowed_types(
-            __arg, __from_server, __validated_path_to_schemas, schema=cls)
-        __validation_metadata = ValidationMetadata(
-            configuration=_configuration, from_server=__from_server, validated_path_to_schemas=__validated_path_to_schemas)
-        __path_to_schemas = cls.__get_new_cls(__arg, __validation_metadata)
-        __new_cls = __path_to_schemas[__validation_metadata.path_to_item]
-        return __new_cls._get_new_instance_without_conversion_oapg(
-            __arg,
-            __validation_metadata.path_to_item,
-            __path_to_schemas
+            _arg = cls.__get_input_dict(*args, **_kwargs)
+        _from_server = False
+        _validated_path_to_schemas = {}
+        _arg = cast_to_allowed_types(
+            _arg, _from_server, _validated_path_to_schemas, schema=cls)
+        _validation_metadata = ValidationMetadata(
+            configuration=_configuration, from_server=_from_server, validated_path_to_schemas=_validated_path_to_schemas)
+        _path_to_schemas = cls.__get_new_cls(_arg, _validation_metadata)
+        _new_cls = _path_to_schemas[_validation_metadata.path_to_item]
+        return _new_cls._get_new_instance_without_conversion_oapg(
+            _arg,
+            _validation_metadata.path_to_item,
+            _path_to_schemas
         )
 
     def __init__(
         self,
         *args: typing.Union[
             dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, 'Schema'],
         _configuration: typing.Optional[Configuration] = None,
@@ -1438,15 +1442,15 @@
                     return discriminated_cls
         return None
 
 
 class DictBase(Discriminable, ValidatorBase):
 
     @classmethod
-    def __validate_arg_presence(cls, arg):
+    def __validate_arg_presence(cls, arg, validation_metadata: ValidationMetadata):
         """
         Ensures that:
         - all required arguments are passed in
         - the input variable names are valid
             - present in properties or
             - accepted because additionalProperties exists
         Exceptions will be raised if:
@@ -1475,19 +1479,20 @@
             elif additional_properties is not NotAnyTypeSchema:
                 continue
             else:
                 invalid_arguments.append(property_name)
         missing_required_arguments = list(required_property_names - seen_required_properties)
         if missing_required_arguments:
             missing_required_arguments.sort()
-            raise ApiTypeError(
-                "{} is missing {} required argument{}: {}".format(
+            raise MissingRequiredPropertiesError(
+                "{} is missing {} required propert{}{}: {}".format(
                     cls.__name__,
                     len(missing_required_arguments),
-                    "s" if len(missing_required_arguments) > 1 else "",
+                    "ies" if len(missing_required_arguments) > 1 else "y",
+                    " at '{}'".format('.'.join([str(i) for i in validation_metadata.path_to_item[1:]])) if len(validation_metadata.path_to_item) > 1 else "",
                     missing_required_arguments
                 )
             )
         if invalid_arguments:
             invalid_arguments.sort()
             raise ApiTypeError(
                 "{} was passed {} invalid argument{}: {}".format(
@@ -1543,15 +1548,15 @@
                 validated_path_to_schemas=validation_metadata.validated_path_to_schemas
             )
             if arg_validation_metadata.validation_ran_earlier(schema):
                 continue
             try:
                 other_path_to_schemas = schema._validate_oapg(value, validation_metadata=arg_validation_metadata)
                 update(path_to_schemas, other_path_to_schemas)
-            except (ApiTypeError, ApiValueError) as e:
+            except (ApiTypeError, ApiValueError, MissingRequiredPropertiesError) as e:
                 validation_errors.append(e)
         if len(validation_errors) > 0:
             raise SchemaValidationError(validation_errors)
         return path_to_schemas
 
     @classmethod
     def __check_dict_validations(
@@ -1603,15 +1608,15 @@
             ApiTypeError: when the input type is not in the list of allowed spec types
         """
         if isinstance(arg, frozendict.frozendict):
             cls.__check_dict_validations(arg, validation_metadata)
         _path_to_schemas = super()._validate_oapg(arg, validation_metadata=validation_metadata)
         if not isinstance(arg, frozendict.frozendict):
             return _path_to_schemas
-        cls.__validate_arg_presence(arg)
+        cls.__validate_arg_presence(arg, validation_metadata)
         other_path_to_schemas = cls.__validate_args(arg, validation_metadata=validation_metadata)
         update(_path_to_schemas, other_path_to_schemas)
         try:
             discriminator = cls.MetaOapg.discriminator()
         except AttributeError:
             return _path_to_schemas
         # discriminator exists
@@ -1851,33 +1856,32 @@
     def __get_anyof_classes(
         cls,
         arg,
         discriminated_cls,
         validation_metadata: ValidationMetadata
     ):
         anyof_classes = []
+        exceptions: typing.List[typing.Union[ApiTypeError, ApiValueError]] = []
         path_to_schemas = defaultdict(set)
         for anyof_cls in cls.MetaOapg.any_of():
             if validation_metadata.validation_ran_earlier(anyof_cls):
                 anyof_classes.append(anyof_cls)
                 continue
 
             try:
                 other_path_to_schemas = anyof_cls._validate_oapg(arg, validation_metadata=validation_metadata)
             except (ApiValueError, ApiTypeError) as ex:
                 if discriminated_cls is not None and anyof_cls is discriminated_cls:
                     raise ex
+                exceptions.append(ex)
                 continue
             anyof_classes.append(anyof_cls)
             update(path_to_schemas, other_path_to_schemas)
         if not anyof_classes:
-            raise ApiValueError(
-                "Invalid inputs given to generate an instance of {}. None "
-                "of the anyOf schemas matched the input data.".format(cls)
-            )
+            raise AnyOfValidationError(error_list=exceptions)
         return path_to_schemas
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
```

### Comparing `splitit-web-python-sdk-2.1.0/splitit_client/validation_metadata.py` & `splitit_web_python_sdk-2.2.0/splitit_client/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `splitit-web-python-sdk-2.1.0/test/test_models/test_installment_plan_refund_response.py` & `splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_refund_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,21 +5,32 @@
 
     Splitit's Web API
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
-import unittest
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import splitit_client
-from splitit_client.model.installment_plan_refund_response import InstallmentPlanRefundResponse
-from splitit_client import configuration
+from splitit_client.type.refund_summary import RefundSummary
 
-
-class TestInstallmentPlanRefundResponse(unittest.TestCase):
-    """InstallmentPlanRefundResponse unit test stubs"""
+class RequiredInstallmentPlanRefundResponse(TypedDict):
     pass
 
+class OptionalInstallmentPlanRefundResponse(TypedDict, total=False):
+    RefundId: str
+
+    InstallmentPlanNumber: str
+
+    Currency: str
+
+    NonCreditRefundAmount: typing.Union[int, float]
 
-if __name__ == '__main__':
-    unittest.main()
+    CreditRefundAmount: typing.Union[int, float]
+
+    Summary: RefundSummary
+
+class InstallmentPlanRefundResponse(RequiredInstallmentPlanRefundResponse, OptionalInstallmentPlanRefundResponse):
+    pass
```

### Comparing `splitit-web-python-sdk-2.1.0/test/test_paths/test_api_installmentplans_installment_plan_number_cancel/test_post.py` & `splitit_web_python_sdk-2.2.0/splitit_client/type/installment_plan_update_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,41 +5,27 @@
 
     Splitit's Web API
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
-import unittest
-from unittest.mock import patch
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import urllib3
+from splitit_client.type.plan_status import PlanStatus
+from splitit_client.type.shipping_status import ShippingStatus
 
-import splitit_client
-from splitit_client.paths.api_installmentplans_installment_plan_number_cancel import post
-from splitit_client import configuration, schemas, api_client
+class RequiredInstallmentPlanUpdateResponse(TypedDict):
+    Status: PlanStatus
 
-from .. import ApiTestMixin
+    ShippingStatus: ShippingStatus
 
+class OptionalInstallmentPlanUpdateResponse(TypedDict, total=False):
+    RefOrderNumber: str
 
-class TestApiInstallmentplansInstallmentPlanNumberCancel(ApiTestMixin, unittest.TestCase):
-    """
-    ApiInstallmentplansInstallmentPlanNumberCancel unit test stubs
-    """
+    InstallmentPlanNumber: str
 
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    response_status = 200
-
-
-
-
-
-
-
-
-if __name__ == '__main__':
-    unittest.main()
+class InstallmentPlanUpdateResponse(RequiredInstallmentPlanUpdateResponse, OptionalInstallmentPlanUpdateResponse):
+    pass
```

