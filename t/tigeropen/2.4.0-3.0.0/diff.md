# Comparing `tmp/tigeropen-2.4.0.tar.gz` & `tmp/tigeropen-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigeropen-2.4.0.tar", last modified: Wed Jun  7 11:40:27 2023, max compression
+gzip compressed data, was "tigeropen-3.0.0.tar", last modified: Thu Jun  8 06:17:55 2023, max compression
```

## Comparing `tigeropen-2.4.0.tar` & `tigeropen-3.0.0.tar`

### file list

```diff
@@ -1,208 +1,208 @@
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.870142 tigeropen-2.4.0/
--rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-2.4.0/MANIFEST.in
--rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-07 11:40:27.869956 tigeropen-2.4.0/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-2.4.0/README.md
--rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-2.4.0/requirements.txt
--rw-r--r--   0 sukai      (501) staff       (20)       38 2023-06-07 11:40:27.870186 tigeropen-2.4.0/setup.cfg
--rw-r--r--   0 sukai      (501) staff       (20)     1358 2023-04-18 08:29:36.000000 tigeropen-2.4.0/setup.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.837015 tigeropen-2.4.0/tigeropen/
--rw-r--r--   0 sukai      (501) staff       (20)       91 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.839369 tigeropen-2.4.0/tigeropen/common/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/common/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.842044 tigeropen-2.4.0/tigeropen/common/consts/
--rw-r--r--   0 sukai      (501) staff       (20)     4706 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/common/consts/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    19190 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/common/consts/filter_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/common/consts/fundamental_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-2.4.0/tigeropen/common/consts/params.py
--rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/common/consts/push_destinations.py
--rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/common/consts/push_subscriptions.py
--rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/common/consts/push_types.py
--rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-2.4.0/tigeropen/common/consts/quote_keys.py
--rw-r--r--   0 sukai      (501) staff       (20)     2989 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/common/consts/service_types.py
--rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/common/consts/tick_constants.py
--rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/common/exceptions.py
--rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/common/model.py
--rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/common/request.py
--rw-r--r--   0 sukai      (501) staff       (20)      654 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/common/response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.844159 tigeropen-2.4.0/tigeropen/common/util/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/common/util/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/common/util/account_util.py
--rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/common/util/common_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-05-08 03:14:32.000000 tigeropen-2.4.0/tigeropen/common/util/contract_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     7461 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/common/util/order_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/common/util/price_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-2.4.0/tigeropen/common/util/signature_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/common/util/string_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-2.4.0/tigeropen/common/util/tick_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-04-11 08:55:54.000000 tigeropen-2.4.0/tigeropen/common/util/web_utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.845626 tigeropen-2.4.0/tigeropen/examples/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/examples/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/examples/client_config.py
--rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/examples/nasdaq100.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.845926 tigeropen-2.4.0/tigeropen/examples/option_helpers/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/examples/option_helpers/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/examples/option_helpers/helpers.py
--rw-r--r--   0 sukai      (501) staff       (20)    10346 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/examples/push_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-04-11 08:55:54.000000 tigeropen-2.4.0/tigeropen/examples/push_client_stomp_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/examples/quote_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)     8386 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/examples/trade_client_demo.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.846105 tigeropen-2.4.0/tigeropen/fundamental/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.4.0/tigeropen/fundamental/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.846287 tigeropen-2.4.0/tigeropen/fundamental/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.4.0/tigeropen/fundamental/domain/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.846666 tigeropen-2.4.0/tigeropen/fundamental/request/
--rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-2.4.0/tigeropen/fundamental/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/fundamental/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.848520 tigeropen-2.4.0/tigeropen/fundamental/response/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.4.0/tigeropen/fundamental/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-2.4.0/tigeropen/fundamental/response/corporate_dividend_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-2.4.0/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-2.4.0/tigeropen/fundamental/response/corporate_split_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/fundamental/response/financial_daily_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/fundamental/response/financial_report_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/fundamental/response/industry_response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.849638 tigeropen-2.4.0/tigeropen/push/
--rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/push/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.851287 tigeropen-2.4.0/tigeropen/push/network/
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/network/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/network/connect.py
--rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/network/exception.py
--rw-r--r--   0 sukai      (501) staff       (20)     7566 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/network/listener.py
--rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/network/protocal.py
--rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-06-01 06:23:56.000000 tigeropen-2.4.0/tigeropen/push/network/transport.py
--rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/network/utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.858275 tigeropen-2.4.0/tigeropen/push/pb/
--rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/AssetData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/AssetData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/AssetData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1969 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/pb/OrderStatusData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2534 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/pb/OrderStatusData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4388 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/pb/OrderStatusData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/OrderTransactionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/OrderTransactionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/OrderTransactionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1117 2023-04-18 08:29:36.000000 tigeropen-2.4.0/tigeropen/push/pb/PositionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1824 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/PositionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2418 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/PositionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      826 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/PushData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3277 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/PushData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2985 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/PushData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteBBOData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteBBOData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteBBOData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteBasicData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteBasicData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteBasicData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     2303 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteDepthData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteDepthData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/QuoteDepthData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/Request.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/Request_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/Request_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/Response.proto
--rw-r--r--   0 sukai      (501) staff       (20)     4204 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/Response_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1717 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/Response_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      726 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/SocketCommon.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2049 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/SocketCommon_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/SocketCommon_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/TradeTickData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/TradeTickData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-06-01 02:58:45.000000 tigeropen-2.4.0/tigeropen/push/pb/TradeTickData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-2.4.0/tigeropen/push/pb/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/pb/readme.md
--rw-r--r--   0 sukai      (501) staff       (20)      661 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/pb/trade_tick.py
--rw-r--r--   0 sukai      (501) staff       (20)     8948 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/pb/util.py
--rw-r--r--   0 sukai      (501) staff       (20)    15009 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/push/protobuf_push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)     8097 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    27606 2023-03-03 09:45:38.000000 tigeropen-2.4.0/tigeropen/push/stomp_push_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.858605 tigeropen-2.4.0/tigeropen/quote/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/quote/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.860314 tigeropen-2.4.0/tigeropen/quote/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/quote/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/domain/bar.py
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/quote/domain/capital_distribution.py
--rw-r--r--   0 sukai      (501) staff       (20)     9623 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/domain/filter.py
--rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/domain/market_status.py
--rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/domain/quote_brief.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/quote/domain/stock_broker.py
--rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/domain/tick.py
--rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/domain/timeline.py
--rw-r--r--   0 sukai      (501) staff       (20)    77148 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/quote_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.860585 tigeropen-2.4.0/tigeropen/quote/request/
--rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/quote/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    33696 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.865913 tigeropen-2.4.0/tigeropen/quote/response/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/quote/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/quote/response/capital_distribution_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/quote/response/capital_flow_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-2.4.0/tigeropen/quote/response/future_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-2.4.0/tigeropen/quote/response/future_contract_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/future_exchange_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1746 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/response/future_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/quote/response/future_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-2.4.0/tigeropen/quote/response/future_trading_times_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1805 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/response/market_scanner_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/market_status_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/option_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-2.4.0/tigeropen/quote/response/option_chains_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/option_expirations_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/option_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/option_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1599 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2469 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_brief_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_delay_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_depth_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_grab_permission_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2730 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_hour_trading_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2410 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_timeline_history_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-2.4.0/tigeropen/quote/response/quote_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-2.4.0/tigeropen/quote/response/stock_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-2.4.0/tigeropen/quote/response/stock_broker_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4898 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/quote/response/stock_details_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/stock_short_interest_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/stock_trade_meta_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/symbol_names_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-2.4.0/tigeropen/quote/response/symbols_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/quote/response/trading_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      802 2023-04-11 09:03:52.000000 tigeropen-2.4.0/tigeropen/quote/response/warrant_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      979 2023-04-11 09:03:52.000000 tigeropen-2.4.0/tigeropen/quote/response/warrant_filter_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    11281 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/tiger_open_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-06-01 02:40:59.000000 tigeropen-2.4.0/tigeropen/tiger_open_config.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.866190 tigeropen-2.4.0/tigeropen/trade/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/trade/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.867453 tigeropen-2.4.0/tigeropen/trade/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/trade/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-04-11 08:55:54.000000 tigeropen-2.4.0/tigeropen/trade/domain/account.py
--rw-r--r--   0 sukai      (501) staff       (20)     6154 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/domain/contract.py
--rw-r--r--   0 sukai      (501) staff       (20)    10103 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/domain/order.py
--rw-r--r--   0 sukai      (501) staff       (20)     2257 2023-04-18 08:29:36.000000 tigeropen-2.4.0/tigeropen/trade/domain/position.py
--rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-2.4.0/tigeropen/trade/domain/prime_account.py
--rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/trade/domain/profile.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.867832 tigeropen-2.4.0/tigeropen/trade/request/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.4.0/tigeropen/trade/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    32808 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.869669 tigeropen-2.4.0/tigeropen/trade/response/
--rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-2.4.0/tigeropen/trade/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1120 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/account_profile_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      949 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/analytics_asset_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4426 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1528 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/contracts_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-04-11 08:55:54.000000 tigeropen-2.4.0/tigeropen/trade/response/forex_order_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1166 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/order_id_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1278 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/order_preview_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     7277 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/orders_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4759 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/positions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-2.4.0/tigeropen/trade/response/prime_assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-04-11 08:55:54.000000 tigeropen-2.4.0/tigeropen/trade/response/segment_fund_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1413 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/response/transactions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    40527 2023-06-07 11:40:19.000000 tigeropen-2.4.0/tigeropen/trade/trade_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-07 11:40:27.838100 tigeropen-2.4.0/tigeropen.egg-info/
--rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-07 11:40:27.000000 tigeropen-2.4.0/tigeropen.egg-info/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     7392 2023-06-07 11:40:27.000000 tigeropen-2.4.0/tigeropen.egg-info/SOURCES.txt
--rw-r--r--   0 sukai      (501) staff       (20)        1 2023-06-07 11:40:27.000000 tigeropen-2.4.0/tigeropen.egg-info/dependency_links.txt
--rw-r--r--   0 sukai      (501) staff       (20)      130 2023-06-07 11:40:27.000000 tigeropen-2.4.0/tigeropen.egg-info/requires.txt
--rw-r--r--   0 sukai      (501) staff       (20)       10 2023-06-07 11:40:27.000000 tigeropen-2.4.0/tigeropen.egg-info/top_level.txt
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.028241 tigeropen-3.0.0/
+-rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-3.0.0/MANIFEST.in
+-rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-08 06:17:55.028116 tigeropen-3.0.0/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-3.0.0/README.md
+-rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-3.0.0/requirements.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       38 2023-06-08 06:17:55.028282 tigeropen-3.0.0/setup.cfg
+-rw-r--r--   0 sukai      (501) staff       (20)     1358 2023-04-18 08:29:36.000000 tigeropen-3.0.0/setup.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:54.998125 tigeropen-3.0.0/tigeropen/
+-rw-r--r--   0 sukai      (501) staff       (20)       91 2023-06-08 06:17:42.000000 tigeropen-3.0.0/tigeropen/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.000279 tigeropen-3.0.0/tigeropen/common/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/common/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.002478 tigeropen-3.0.0/tigeropen/common/consts/
+-rw-r--r--   0 sukai      (501) staff       (20)     4706 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/common/consts/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    19190 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/common/consts/filter_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/common/consts/fundamental_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-3.0.0/tigeropen/common/consts/params.py
+-rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/common/consts/push_destinations.py
+-rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/common/consts/push_subscriptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/common/consts/push_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-3.0.0/tigeropen/common/consts/quote_keys.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2989 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/common/consts/service_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/common/consts/tick_constants.py
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/common/exceptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/common/model.py
+-rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/common/request.py
+-rw-r--r--   0 sukai      (501) staff       (20)      654 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/common/response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.004207 tigeropen-3.0.0/tigeropen/common/util/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/common/util/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/common/util/account_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/common/util/common_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-05-08 03:14:32.000000 tigeropen-3.0.0/tigeropen/common/util/contract_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7461 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/common/util/order_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/common/util/price_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-3.0.0/tigeropen/common/util/signature_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/common/util/string_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-3.0.0/tigeropen/common/util/tick_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-04-11 08:55:54.000000 tigeropen-3.0.0/tigeropen/common/util/web_utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.005147 tigeropen-3.0.0/tigeropen/examples/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/examples/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/examples/client_config.py
+-rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/examples/nasdaq100.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.005406 tigeropen-3.0.0/tigeropen/examples/option_helpers/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/examples/option_helpers/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/examples/option_helpers/helpers.py
+-rw-r--r--   0 sukai      (501) staff       (20)    10346 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/examples/push_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-04-11 08:55:54.000000 tigeropen-3.0.0/tigeropen/examples/push_client_stomp_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/examples/quote_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8386 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/examples/trade_client_demo.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.005535 tigeropen-3.0.0/tigeropen/fundamental/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.0.0/tigeropen/fundamental/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.005663 tigeropen-3.0.0/tigeropen/fundamental/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.0.0/tigeropen/fundamental/domain/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.005927 tigeropen-3.0.0/tigeropen/fundamental/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-3.0.0/tigeropen/fundamental/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/fundamental/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.006843 tigeropen-3.0.0/tigeropen/fundamental/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.0.0/tigeropen/fundamental/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-3.0.0/tigeropen/fundamental/response/corporate_dividend_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-3.0.0/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-3.0.0/tigeropen/fundamental/response/corporate_split_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/fundamental/response/financial_daily_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/fundamental/response/financial_report_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/fundamental/response/industry_response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.007446 tigeropen-3.0.0/tigeropen/push/
+-rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/push/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.008769 tigeropen-3.0.0/tigeropen/push/network/
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/network/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/network/connect.py
+-rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/network/exception.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7566 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/network/listener.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/network/protocal.py
+-rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-06-01 06:23:56.000000 tigeropen-3.0.0/tigeropen/push/network/transport.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/network/utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.015342 tigeropen-3.0.0/tigeropen/push/pb/
+-rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/AssetData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/AssetData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/AssetData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1969 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/pb/OrderStatusData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2534 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/pb/OrderStatusData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4388 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/pb/OrderStatusData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/OrderTransactionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/OrderTransactionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/OrderTransactionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1117 2023-04-18 08:29:36.000000 tigeropen-3.0.0/tigeropen/push/pb/PositionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1824 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/PositionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2418 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/PositionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      826 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/PushData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3277 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/PushData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2985 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/PushData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteBBOData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteBBOData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteBBOData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteBasicData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteBasicData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteBasicData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     2303 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteDepthData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteDepthData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/QuoteDepthData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/Request.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/Request_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/Request_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/Response.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     4204 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/Response_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1717 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/Response_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      726 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/SocketCommon.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2049 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/SocketCommon_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/SocketCommon_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/TradeTickData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/TradeTickData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-06-01 02:58:45.000000 tigeropen-3.0.0/tigeropen/push/pb/TradeTickData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-3.0.0/tigeropen/push/pb/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/pb/readme.md
+-rw-r--r--   0 sukai      (501) staff       (20)      661 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/pb/trade_tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8948 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/pb/util.py
+-rw-r--r--   0 sukai      (501) staff       (20)    15009 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/push/protobuf_push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8077 2023-06-08 06:17:42.000000 tigeropen-3.0.0/tigeropen/push/push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    27606 2023-03-03 09:45:38.000000 tigeropen-3.0.0/tigeropen/push/stomp_push_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.015596 tigeropen-3.0.0/tigeropen/quote/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/quote/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.017521 tigeropen-3.0.0/tigeropen/quote/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/quote/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/domain/bar.py
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/quote/domain/capital_distribution.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9623 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/domain/filter.py
+-rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/domain/market_status.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/domain/quote_brief.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/quote/domain/stock_broker.py
+-rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/domain/tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/domain/timeline.py
+-rw-r--r--   0 sukai      (501) staff       (20)    77148 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/quote_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.017770 tigeropen-3.0.0/tigeropen/quote/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/quote/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    33696 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.023294 tigeropen-3.0.0/tigeropen/quote/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/quote/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/quote/response/capital_distribution_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/quote/response/capital_flow_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-3.0.0/tigeropen/quote/response/future_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-3.0.0/tigeropen/quote/response/future_contract_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/future_exchange_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1746 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/response/future_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/quote/response/future_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-3.0.0/tigeropen/quote/response/future_trading_times_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1805 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/response/market_scanner_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/market_status_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/option_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-3.0.0/tigeropen/quote/response/option_chains_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/option_expirations_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/option_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/option_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1599 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2469 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_brief_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_delay_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_depth_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_grab_permission_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2730 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_hour_trading_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2410 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_timeline_history_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-3.0.0/tigeropen/quote/response/quote_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-3.0.0/tigeropen/quote/response/stock_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-3.0.0/tigeropen/quote/response/stock_broker_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4898 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/quote/response/stock_details_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/stock_short_interest_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/stock_trade_meta_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/symbol_names_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-3.0.0/tigeropen/quote/response/symbols_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/quote/response/trading_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      802 2023-04-11 09:03:52.000000 tigeropen-3.0.0/tigeropen/quote/response/warrant_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      979 2023-04-11 09:03:52.000000 tigeropen-3.0.0/tigeropen/quote/response/warrant_filter_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11281 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/tiger_open_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-06-01 02:40:59.000000 tigeropen-3.0.0/tigeropen/tiger_open_config.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.023583 tigeropen-3.0.0/tigeropen/trade/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/trade/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.025094 tigeropen-3.0.0/tigeropen/trade/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/trade/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-04-11 08:55:54.000000 tigeropen-3.0.0/tigeropen/trade/domain/account.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6154 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/domain/contract.py
+-rw-r--r--   0 sukai      (501) staff       (20)    10103 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/domain/order.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2257 2023-04-18 08:29:36.000000 tigeropen-3.0.0/tigeropen/trade/domain/position.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-3.0.0/tigeropen/trade/domain/prime_account.py
+-rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/trade/domain/profile.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.025531 tigeropen-3.0.0/tigeropen/trade/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.0/tigeropen/trade/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    32808 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:55.027877 tigeropen-3.0.0/tigeropen/trade/response/
+-rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-3.0.0/tigeropen/trade/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1120 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/account_profile_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      949 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/analytics_asset_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4426 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1528 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/contracts_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-04-11 08:55:54.000000 tigeropen-3.0.0/tigeropen/trade/response/forex_order_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1166 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/order_id_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1278 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/order_preview_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7277 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/orders_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4759 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/positions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-3.0.0/tigeropen/trade/response/prime_assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-04-11 08:55:54.000000 tigeropen-3.0.0/tigeropen/trade/response/segment_fund_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1413 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/response/transactions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    40527 2023-06-07 11:40:19.000000 tigeropen-3.0.0/tigeropen/trade/trade_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-08 06:17:54.999044 tigeropen-3.0.0/tigeropen.egg-info/
+-rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-08 06:17:54.000000 tigeropen-3.0.0/tigeropen.egg-info/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     7392 2023-06-08 06:17:54.000000 tigeropen-3.0.0/tigeropen.egg-info/SOURCES.txt
+-rw-r--r--   0 sukai      (501) staff       (20)        1 2023-06-08 06:17:54.000000 tigeropen-3.0.0/tigeropen.egg-info/dependency_links.txt
+-rw-r--r--   0 sukai      (501) staff       (20)      130 2023-06-08 06:17:54.000000 tigeropen-3.0.0/tigeropen.egg-info/requires.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       10 2023-06-08 06:17:54.000000 tigeropen-3.0.0/tigeropen.egg-info/top_level.txt
```

### Comparing `tigeropen-2.4.0/PKG-INFO` & `tigeropen-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 2.4.0
+Version: 3.0.0
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-2.4.0/README.md` & `tigeropen-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/setup.py` & `tigeropen-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/consts/__init__.py` & `tigeropen-3.0.0/tigeropen/common/consts/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/consts/filter_fields.py` & `tigeropen-3.0.0/tigeropen/common/consts/filter_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/consts/fundamental_fields.py` & `tigeropen-3.0.0/tigeropen/common/consts/fundamental_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/consts/params.py` & `tigeropen-3.0.0/tigeropen/common/consts/params.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/consts/push_types.py` & `tigeropen-3.0.0/tigeropen/common/consts/push_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/consts/quote_keys.py` & `tigeropen-3.0.0/tigeropen/common/consts/quote_keys.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/consts/service_types.py` & `tigeropen-3.0.0/tigeropen/common/consts/service_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/consts/tick_constants.py` & `tigeropen-3.0.0/tigeropen/common/consts/tick_constants.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/model.py` & `tigeropen-3.0.0/tigeropen/common/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/request.py` & `tigeropen-3.0.0/tigeropen/common/request.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/response.py` & `tigeropen-3.0.0/tigeropen/common/response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/util/common_utils.py` & `tigeropen-3.0.0/tigeropen/common/util/common_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/util/contract_utils.py` & `tigeropen-3.0.0/tigeropen/common/util/contract_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/util/order_utils.py` & `tigeropen-3.0.0/tigeropen/common/util/order_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/util/price_util.py` & `tigeropen-3.0.0/tigeropen/common/util/price_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/util/signature_utils.py` & `tigeropen-3.0.0/tigeropen/common/util/signature_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/util/string_utils.py` & `tigeropen-3.0.0/tigeropen/common/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/util/tick_util.py` & `tigeropen-3.0.0/tigeropen/common/util/tick_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/common/util/web_utils.py` & `tigeropen-3.0.0/tigeropen/common/util/web_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/examples/client_config.py` & `tigeropen-3.0.0/tigeropen/examples/client_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/examples/nasdaq100.py` & `tigeropen-3.0.0/tigeropen/examples/nasdaq100.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/examples/option_helpers/helpers.py` & `tigeropen-3.0.0/tigeropen/examples/option_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/examples/push_client_demo.py` & `tigeropen-3.0.0/tigeropen/examples/push_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/examples/push_client_stomp_demo.py` & `tigeropen-3.0.0/tigeropen/examples/push_client_stomp_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/examples/quote_client_demo.py` & `tigeropen-3.0.0/tigeropen/examples/quote_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/examples/trade_client_demo.py` & `tigeropen-3.0.0/tigeropen/examples/trade_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/fundamental/request/model.py` & `tigeropen-3.0.0/tigeropen/fundamental/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/fundamental/response/corporate_dividend_response.py` & `tigeropen-3.0.0/tigeropen/fundamental/response/corporate_dividend_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/fundamental/response/corporate_earnings_calendar_response.py` & `tigeropen-3.0.0/tigeropen/fundamental/response/corporate_earnings_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/fundamental/response/corporate_split_response.py` & `tigeropen-3.0.0/tigeropen/fundamental/response/corporate_split_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/fundamental/response/financial_daily_response.py` & `tigeropen-3.0.0/tigeropen/fundamental/response/financial_daily_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/fundamental/response/financial_report_response.py` & `tigeropen-3.0.0/tigeropen/fundamental/response/financial_report_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/fundamental/response/industry_response.py` & `tigeropen-3.0.0/tigeropen/fundamental/response/industry_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/__init__.py` & `tigeropen-3.0.0/tigeropen/push/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/network/connect.py` & `tigeropen-3.0.0/tigeropen/push/network/connect.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/network/exception.py` & `tigeropen-3.0.0/tigeropen/push/network/exception.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/network/listener.py` & `tigeropen-3.0.0/tigeropen/push/network/listener.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/network/protocal.py` & `tigeropen-3.0.0/tigeropen/push/network/protocal.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/network/transport.py` & `tigeropen-3.0.0/tigeropen/push/network/transport.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/network/utils.py` & `tigeropen-3.0.0/tigeropen/push/network/utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/AssetData.proto` & `tigeropen-3.0.0/tigeropen/push/pb/AssetData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/AssetData_pb2.py` & `tigeropen-3.0.0/tigeropen/push/pb/AssetData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/AssetData_pb2.pyi` & `tigeropen-3.0.0/tigeropen/push/pb/AssetData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/OrderStatusData.proto` & `tigeropen-3.0.0/tigeropen/push/pb/OrderStatusData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/OrderStatusData_pb2.py` & `tigeropen-3.0.0/tigeropen/push/pb/OrderStatusData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/OrderStatusData_pb2.pyi` & `tigeropen-3.0.0/tigeropen/push/pb/OrderStatusData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/OrderTransactionData.proto` & `tigeropen-3.0.0/tigeropen/push/pb/OrderTransactionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/OrderTransactionData_pb2.py` & `tigeropen-3.0.0/tigeropen/push/pb/OrderTransactionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/OrderTransactionData_pb2.pyi` & `tigeropen-3.0.0/tigeropen/push/pb/OrderTransactionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/PositionData.proto` & `tigeropen-3.0.0/tigeropen/push/pb/PositionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/PositionData_pb2.py` & `tigeropen-3.0.0/tigeropen/push/pb/PositionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/PositionData_pb2.pyi` & `tigeropen-3.0.0/tigeropen/push/pb/PositionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/PushData.proto` & `tigeropen-3.0.0/tigeropen/push/pb/PushData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/PushData_pb2.py` & `tigeropen-3.0.0/tigeropen/push/pb/PushData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/PushData_pb2.pyi` & `tigeropen-3.0.0/tigeropen/push/pb/PushData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/QuoteBBOData_pb2.py` & `tigeropen-3.0.0/tigeropen/push/pb/QuoteBBOData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/QuoteBBOData_pb2.pyi` & `tigeropen-3.0.0/tigeropen/push/pb/QuoteBBOData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/QuoteBasicData.proto` & `tigeropen-3.0.0/tigeropen/push/pb/QuoteBasicData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/QuoteBasicData_pb2.py` & `tigeropen-3.0.0/tigeropen/push/pb/QuoteBasicData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/QuoteBasicData_pb2.pyi` & `tigeropen-3.0.0/tigeropen/push/pb/QuoteBasicData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/QuoteData.proto` & `tigeropen-3.0.0/tigeropen/push/pb/QuoteData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/QuoteData_pb2.py` & `tigeropen-3.0.0/tigeropen/push/pb/QuoteData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/QuoteData_pb2.pyi` & `tigeropen-3.0.0/tigeropen/push/pb/QuoteData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/QuoteDepthData_pb2.py` & `tigeropen-3.0.0/tigeropen/push/pb/QuoteDepthData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/QuoteDepthData_pb2.pyi` & `tigeropen-3.0.0/tigeropen/push/pb/QuoteDepthData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/Request.proto` & `tigeropen-3.0.0/tigeropen/push/pb/Request.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/Request_pb2.py` & `tigeropen-3.0.0/tigeropen/push/pb/Request_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/Request_pb2.pyi` & `tigeropen-3.0.0/tigeropen/push/pb/Request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/Response_pb2.py` & `tigeropen-3.0.0/tigeropen/push/pb/Response_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/Response_pb2.pyi` & `tigeropen-3.0.0/tigeropen/push/pb/Response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/SocketCommon.proto` & `tigeropen-3.0.0/tigeropen/push/pb/SocketCommon.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/SocketCommon_pb2.py` & `tigeropen-3.0.0/tigeropen/push/pb/SocketCommon_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/SocketCommon_pb2.pyi` & `tigeropen-3.0.0/tigeropen/push/pb/SocketCommon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/TradeTickData.proto` & `tigeropen-3.0.0/tigeropen/push/pb/TradeTickData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/TradeTickData_pb2.py` & `tigeropen-3.0.0/tigeropen/push/pb/TradeTickData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/TradeTickData_pb2.pyi` & `tigeropen-3.0.0/tigeropen/push/pb/TradeTickData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/trade_tick.py` & `tigeropen-3.0.0/tigeropen/push/pb/trade_tick.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/pb/util.py` & `tigeropen-3.0.0/tigeropen/push/pb/util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/protobuf_push_client.py` & `tigeropen-3.0.0/tigeropen/push/protobuf_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/push/push_client.py` & `tigeropen-3.0.0/tigeropen/push/push_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 
 @author: gaoan
 """
 
 from tigeropen.push.protobuf_push_client import ProtobufPushClient
 from tigeropen.push.stomp_push_client import StompPushClient
 
-USE_STOMP = False
-
 
 class PushClient:
     def __init__(self, host, port, use_ssl=True, connection_timeout=120, heartbeats=(30 * 1000, 30 * 1000),
-                 use_protobuf=False):
+                 use_protobuf=True):
         """
         :param host:
         :param port:
         :param use_ssl:
         :param connection_timeout: unit: second. The timeout value should be greater the heartbeats interval
         :param heartbeats: tuple of millisecond
         :param use_protobuf: use stomp protocol or protobuf
```

### Comparing `tigeropen-2.4.0/tigeropen/push/stomp_push_client.py` & `tigeropen-3.0.0/tigeropen/push/stomp_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/domain/filter.py` & `tigeropen-3.0.0/tigeropen/quote/domain/filter.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/domain/quote_brief.py` & `tigeropen-3.0.0/tigeropen/quote/domain/quote_brief.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/domain/stock_broker.py` & `tigeropen-3.0.0/tigeropen/quote/domain/stock_broker.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/quote_client.py` & `tigeropen-3.0.0/tigeropen/quote/quote_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/request/model.py` & `tigeropen-3.0.0/tigeropen/quote/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/capital_distribution_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/capital_distribution_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/capital_flow_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/capital_flow_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/future_briefs_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/future_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/future_contract_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/future_contract_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/future_exchange_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/future_exchange_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/future_quote_bar_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/future_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/future_quote_ticks_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/future_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/future_trading_times_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/future_trading_times_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/market_scanner_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/market_scanner_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/market_status_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/market_status_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/option_briefs_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/option_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/option_chains_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/option_chains_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/option_expirations_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/option_expirations_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/option_quote_bar_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/option_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/option_quote_ticks_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/option_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/quote_bar_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/quote_brief_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/quote_brief_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/quote_delay_briefs_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/quote_delay_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/quote_depth_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/quote_depth_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/quote_grab_permission_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/quote_grab_permission_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/quote_hour_trading_timeline_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/quote_hour_trading_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/quote_ticks_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/quote_timeline_history_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/quote_timeline_history_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/quote_timeline_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/quote_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/stock_briefs_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/stock_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/stock_broker_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/stock_broker_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/stock_details_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/stock_details_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/stock_short_interest_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/stock_short_interest_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/stock_trade_meta_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/stock_trade_meta_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/symbol_names_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/symbol_names_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/symbols_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/symbols_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/trading_calendar_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/trading_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/warrant_briefs_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/warrant_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/quote/response/warrant_filter_response.py` & `tigeropen-3.0.0/tigeropen/quote/response/warrant_filter_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/tiger_open_client.py` & `tigeropen-3.0.0/tigeropen/tiger_open_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/tiger_open_config.py` & `tigeropen-3.0.0/tigeropen/tiger_open_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/domain/account.py` & `tigeropen-3.0.0/tigeropen/trade/domain/account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/domain/contract.py` & `tigeropen-3.0.0/tigeropen/trade/domain/contract.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/domain/order.py` & `tigeropen-3.0.0/tigeropen/trade/domain/order.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/domain/position.py` & `tigeropen-3.0.0/tigeropen/trade/domain/position.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/domain/prime_account.py` & `tigeropen-3.0.0/tigeropen/trade/domain/prime_account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/request/model.py` & `tigeropen-3.0.0/tigeropen/trade/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/response/__init__.py` & `tigeropen-3.0.0/tigeropen/trade/response/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/response/account_profile_response.py` & `tigeropen-3.0.0/tigeropen/trade/response/account_profile_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/response/analytics_asset_response.py` & `tigeropen-3.0.0/tigeropen/trade/response/analytics_asset_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/response/assets_response.py` & `tigeropen-3.0.0/tigeropen/trade/response/assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/response/contracts_response.py` & `tigeropen-3.0.0/tigeropen/trade/response/contracts_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/response/forex_order_response.py` & `tigeropen-3.0.0/tigeropen/trade/response/forex_order_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/response/order_id_response.py` & `tigeropen-3.0.0/tigeropen/trade/response/order_id_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/response/order_preview_response.py` & `tigeropen-3.0.0/tigeropen/trade/response/order_preview_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/response/orders_response.py` & `tigeropen-3.0.0/tigeropen/trade/response/orders_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/response/positions_response.py` & `tigeropen-3.0.0/tigeropen/trade/response/positions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/response/prime_assets_response.py` & `tigeropen-3.0.0/tigeropen/trade/response/prime_assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/response/segment_fund_response.py` & `tigeropen-3.0.0/tigeropen/trade/response/segment_fund_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/response/transactions_response.py` & `tigeropen-3.0.0/tigeropen/trade/response/transactions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen/trade/trade_client.py` & `tigeropen-3.0.0/tigeropen/trade/trade_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.4.0/tigeropen.egg-info/PKG-INFO` & `tigeropen-3.0.0/tigeropen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 2.4.0
+Version: 3.0.0
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-2.4.0/tigeropen.egg-info/SOURCES.txt` & `tigeropen-3.0.0/tigeropen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

