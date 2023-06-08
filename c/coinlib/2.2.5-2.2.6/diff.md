# Comparing `tmp/coinlib-2.2.5.tar.gz` & `tmp/coinlib-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coinlib-2.2.5.tar", last modified: Mon May 29 19:12:28 2023, max compression
+gzip compressed data, was "dist/coinlib-2.2.6.tar", last modified: Thu Jun  8 10:25:35 2023, max compression
```

## Comparing `coinlib-2.2.5.tar` & `coinlib-2.2.6.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.591048 coinlib-2.2.5/
--rw-r--r--   0 root         (0) root         (0)      642 2023-05-29 19:12:28.591048 coinlib-2.2.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.569049 coinlib-2.2.5/coinlib/
--rw-rw-rw-   0 root         (0) root         (0)    27933 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/BasicJob.py
--rw-rw-rw-   0 root         (0) root         (0)     7817 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/BasicJobSessionStorage.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/ChartsFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     9523 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/ChartsIndicatorJob.py
--rw-rw-rw-   0 root         (0) root         (0)     9404 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/ChartsWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/CoinlibCrypto.py
--rw-rw-rw-   0 root         (0) root         (0)     3625 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/CoinlibDataInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     8338 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/CoinlibWorkspace.py
--rw-rw-rw-   0 root         (0) root         (0)    26721 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/DataWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     5777 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/Functions.py
--rw-rw-rw-   0 root         (0) root         (0)     3018 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/InfluxDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     3985 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/PluginLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     6388 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/PluginsWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     5960 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/Registrar.py
--rw-rw-rw-   0 root         (0) root         (0)    17647 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/Simulator.py
--rw-rw-rw-   0 root         (0) root         (0)    13006 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/WorkerJobProcess.py
--rw-rw-rw-   0 root         (0) root         (0)     5812 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.572049 coinlib-2.2.5/coinlib/broker/
--rw-rw-rw-   0 root         (0) root         (0)     7229 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/Broker.py
--rw-rw-rw-   0 root         (0) root         (0)     4411 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/BrokerDTO.py
--rw-rw-rw-   0 root         (0) root         (0)    11295 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/CoinlibBroker.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/CoinlibBrokerFuture.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/CoinlibBrokerMargin.py
--rw-rw-rw-   0 root         (0) root         (0)     1160 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/CoinlibBrokerSpot.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/CoinlibSessionManager.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/broker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.574049 coinlib-2.2.5/coinlib/brokerWorker/
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/brokerWorker/BrokerFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     7841 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/brokerWorker/BrokerSession.py
--rw-rw-rw-   0 root         (0) root         (0)     2930 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/brokerWorker/BrokerSessionWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     5984 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/brokerWorker/BrokerWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/brokerWorker/TestProtocolResult.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/brokerWorker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3017 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/coinlibFactory.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.574049 coinlib-2.2.5/coinlib/data/
--rw-rw-rw-   0 root         (0) root         (0)     2467 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/data/CollectionInterface.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/data/DataTable.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    78694 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/dataWorker_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)   164353 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/dataWorker_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.575049 coinlib-2.2.5/coinlib/drawable/
--rw-rw-rw-   0 root         (0) root         (0)     3528 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/drawable/CoinlibDrawable.py
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/drawable/DrawableComponent.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/drawable/WindowGrid.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/drawable/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.576048 coinlib-2.2.5/coinlib/event/
--rw-rw-rw-   0 root         (0) root         (0)     2820 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/event/EventConsumer.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/event/EventInterface.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/event/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.578049 coinlib-2.2.5/coinlib/feature/
--rw-rw-rw-   0 root         (0) root         (0)    17646 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/CoinlibFeature.py
--rw-rw-rw-   0 root         (0) root         (0)     1220 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/CoinlibFeatureFetcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2256 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/CoinlibFeatureLake.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/CoinlibFeatureProcessor.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/FeatureDTO.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/FeatureFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     9545 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/FeatureWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     6088 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/Features.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/feature/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13456 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/helper.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/index.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.583048 coinlib-2.2.5/coinlib/logics/
--rw-rw-rw-   0 root         (0) root         (0)    13495 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/Logic.py
--rw-rw-rw-   0 root         (0) root         (0)     8794 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicBasicWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicDTo.py
--rw-rw-rw-   0 root         (0) root         (0)     7477 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicJob.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicLoader.py
--rw-rw-rw-   0 root         (0) root         (0)      520 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOfflineJob.py
--rw-rw-rw-   0 root         (0) root         (0)    10021 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOfflineWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOfflineWorkerData.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOfflineWorkerScreener.py
--rw-rw-rw-   0 root         (0) root         (0)     1992 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOfflineWorkerTrader.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOnlineDataWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOnlineJob.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOnlineScreenerWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOnlineTraderWorker.py
--rw-rw-rw-   0 root         (0) root         (0)    14919 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOnlineWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicOptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8512 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicRegistrationInstance.py
--rw-rw-rw-   0 root         (0) root         (0)    16758 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/LogicTestBrokerWorker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.583048 coinlib-2.2.5/coinlib/logics/broker/
--rw-rw-rw-   0 root         (0) root         (0)     3107 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/broker/LogicBrokerInterface.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/broker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.584048 coinlib-2.2.5/coinlib/logics/manager/
--rw-rw-rw-   0 root         (0) root         (0)     7098 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/manager/LogicJobBroker.py
--rw-rw-rw-   0 root         (0) root         (0)     8814 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/manager/LogicManager.py
--rw-rw-rw-   0 root         (0) root         (0)     4375 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/manager/PortfolioModel.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/manager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.585048 coinlib-2.2.5/coinlib/logics/offlineManager/
--rw-rw-rw-   0 root         (0) root         (0)    20273 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py
--rw-rw-rw-   0 root         (0) root         (0)    11492 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py
--rw-rw-rw-   0 root         (0) root         (0)     3298 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/offlineManager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.586048 coinlib-2.2.5/coinlib/logics/onlineManager/
--rw-rw-rw-   0 root         (0) root         (0)     6706 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/onlineManager/LogicOnlineJobBroker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/logics/onlineManager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.587048 coinlib-2.2.5/coinlib/notification/
--rw-rw-rw-   0 root         (0) root         (0)     3908 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/notification/Notification.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/notification/NotificationFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     5781 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/notification/NotificationWorker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/notification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.589048 coinlib-2.2.5/coinlib/statistics/
--rw-rw-rw-   0 root         (0) root         (0)      730 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/StatisticMethodJob.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/StatisticRuleJob.py
--rw-rw-rw-   0 root         (0) root         (0)     6228 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/Statistics.py
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/StatisticsMethodFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     5277 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/StatisticsMethodWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/StatisticsRuleFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     6204 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/StatisticsRuleWorker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/statistics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.590048 coinlib-2.2.5/coinlib/symbols/
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/symbols/SymbolFactory.py
--rw-rw-rw-   0 root         (0) root         (0)    14991 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/symbols/SymbolWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     3584 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/symbols/Symbols.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 19:12:15.000000 coinlib-2.2.5/coinlib/symbols/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.570049 coinlib-2.2.5/coinlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      642 2023-05-29 19:12:28.000000 coinlib-2.2.5/coinlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3789 2023-05-29 19:12:28.000000 coinlib-2.2.5/coinlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 19:12:28.000000 coinlib-2.2.5/coinlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-29 19:12:28.000000 coinlib-2.2.5/coinlib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-29 19:12:28.000000 coinlib-2.2.5/coinlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-29 19:12:28.000000 coinlib-2.2.5/coinlib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 19:12:28.591048 coinlib-2.2.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-05-29 19:12:15.000000 coinlib-2.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:12:28.590048 coinlib-2.2.5/test/
--rw-rw-rw-   0 root         (0) root         (0)     4048 2023-05-29 19:12:15.000000 coinlib-2.2.5/test/testchartworker.py
--rw-rw-rw-   0 root         (0) root         (0)    10860 2023-05-29 19:12:15.000000 coinlib-2.2.5/test/testcross.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2023-05-29 19:12:15.000000 coinlib-2.2.5/test/testplot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.676814 coinlib-2.2.6/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-06-08 10:25:35.676814 coinlib-2.2.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.655814 coinlib-2.2.6/coinlib/
+-rw-rw-rw-   0 root         (0) root         (0)    28406 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/BasicJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     7820 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/BasicJobSessionStorage.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/ChartsFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     9523 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/ChartsIndicatorJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     9404 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/ChartsWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/CoinlibCrypto.py
+-rw-rw-rw-   0 root         (0) root         (0)     3625 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/CoinlibDataInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     8338 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/CoinlibWorkspace.py
+-rw-rw-rw-   0 root         (0) root         (0)    26721 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/DataWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5777 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/Functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3018 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/InfluxDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     3985 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/PluginLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     6388 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/PluginsWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5960 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/Registrar.py
+-rw-rw-rw-   0 root         (0) root         (0)    17647 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/Simulator.py
+-rw-rw-rw-   0 root         (0) root         (0)    13006 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/WorkerJobProcess.py
+-rw-rw-rw-   0 root         (0) root         (0)     5812 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.659814 coinlib-2.2.6/coinlib/broker/
+-rw-rw-rw-   0 root         (0) root         (0)     7229 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/Broker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4411 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/BrokerDTO.py
+-rw-rw-rw-   0 root         (0) root         (0)    11295 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/CoinlibBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/CoinlibBrokerFuture.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/CoinlibBrokerMargin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/CoinlibBrokerSpot.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/CoinlibSessionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/broker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.660814 coinlib-2.2.6/coinlib/brokerWorker/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/brokerWorker/BrokerFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     7841 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/brokerWorker/BrokerSession.py
+-rw-rw-rw-   0 root         (0) root         (0)     2930 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/brokerWorker/BrokerSessionWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5984 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/brokerWorker/BrokerWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/brokerWorker/TestProtocolResult.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/brokerWorker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/coinlibFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.661814 coinlib-2.2.6/coinlib/data/
+-rw-rw-rw-   0 root         (0) root         (0)     2467 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/data/CollectionInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)    11600 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/data/DataTable.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    78694 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/dataWorker_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)   164353 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/dataWorker_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.662814 coinlib-2.2.6/coinlib/drawable/
+-rw-rw-rw-   0 root         (0) root         (0)     3528 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/drawable/CoinlibDrawable.py
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/drawable/DrawableComponent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/drawable/WindowGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/drawable/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.662814 coinlib-2.2.6/coinlib/event/
+-rw-rw-rw-   0 root         (0) root         (0)     2820 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/event/EventConsumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/event/EventInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/event/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.664814 coinlib-2.2.6/coinlib/feature/
+-rw-rw-rw-   0 root         (0) root         (0)    17646 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/CoinlibFeature.py
+-rw-rw-rw-   0 root         (0) root         (0)     1220 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/CoinlibFeatureFetcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/CoinlibFeatureLake.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/CoinlibFeatureProcessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/FeatureDTO.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/FeatureFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     9545 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/FeatureWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     6088 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/Features.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/feature/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13456 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.669814 coinlib-2.2.6/coinlib/logics/
+-rw-rw-rw-   0 root         (0) root         (0)    13495 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/Logic.py
+-rw-rw-rw-   0 root         (0) root         (0)     8794 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicBasicWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicDTo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7564 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)      520 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOfflineJob.py
+-rw-rw-rw-   0 root         (0) root         (0)    10121 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOfflineWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOfflineWorkerData.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOfflineWorkerScreener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOfflineWorkerTrader.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOnlineDataWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOnlineJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOnlineScreenerWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOnlineTraderWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)    14919 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOnlineWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicOptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8512 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicRegistrationInstance.py
+-rw-rw-rw-   0 root         (0) root         (0)    16758 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/LogicTestBrokerWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.669814 coinlib-2.2.6/coinlib/logics/broker/
+-rw-rw-rw-   0 root         (0) root         (0)     3107 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/broker/LogicBrokerInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/broker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.670814 coinlib-2.2.6/coinlib/logics/manager/
+-rw-rw-rw-   0 root         (0) root         (0)     7098 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/manager/LogicJobBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)     9156 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/manager/LogicManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4375 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/manager/PortfolioModel.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/manager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.671814 coinlib-2.2.6/coinlib/logics/offlineManager/
+-rw-rw-rw-   0 root         (0) root         (0)    20273 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)    11492 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/offlineManager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.671814 coinlib-2.2.6/coinlib/logics/onlineManager/
+-rw-rw-rw-   0 root         (0) root         (0)     6706 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/onlineManager/LogicOnlineJobBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/logics/onlineManager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.672814 coinlib-2.2.6/coinlib/notification/
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/notification/Notification.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/notification/NotificationFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5781 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/notification/NotificationWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/notification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.674814 coinlib-2.2.6/coinlib/statistics/
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/StatisticMethodJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/StatisticRuleJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     6228 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/Statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/StatisticsMethodFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5277 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/StatisticsMethodWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/StatisticsRuleFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     6204 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/StatisticsRuleWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/statistics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.675814 coinlib-2.2.6/coinlib/symbols/
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/symbols/SymbolFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)    14991 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/symbols/SymbolWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/symbols/Symbols.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 10:25:22.000000 coinlib-2.2.6/coinlib/symbols/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.657814 coinlib-2.2.6/coinlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-06-08 10:25:35.000000 coinlib-2.2.6/coinlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-06-08 10:25:35.000000 coinlib-2.2.6/coinlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 10:25:35.000000 coinlib-2.2.6/coinlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-08 10:25:35.000000 coinlib-2.2.6/coinlib.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      256 2023-06-08 10:25:35.000000 coinlib-2.2.6/coinlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 10:25:35.000000 coinlib-2.2.6/coinlib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 10:25:35.676814 coinlib-2.2.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-06-08 10:25:22.000000 coinlib-2.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:25:35.676814 coinlib-2.2.6/test/
+-rw-rw-rw-   0 root         (0) root         (0)     4048 2023-06-08 10:25:22.000000 coinlib-2.2.6/test/testchartworker.py
+-rw-rw-rw-   0 root         (0) root         (0)    10860 2023-06-08 10:25:22.000000 coinlib-2.2.6/test/testcross.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2023-06-08 10:25:22.000000 coinlib-2.2.6/test/testplot.py
```

### Comparing `coinlib-2.2.5/PKG-INFO` & `coinlib-2.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinlib
-Version: 2.2.5
+Version: 2.2.6
 Summary: Develop new code for your coindeck environment
 Home-page: https://gitlab.com/coindeck/coinlib
 Author: coindeck
 Author-email: donnercody86@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `coinlib-2.2.5/coinlib/BasicJob.py` & `coinlib-2.2.6/coinlib/BasicJob.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,14 +261,26 @@
                     return True
             if mode == CrossMode.both or mode == CrossMode.down:
                 if currentline[-1] < y:
                     return True
 
         return False
 
+    def isDateGreater(self, date, time=None):
+        if time is not None:
+            date = date +" "+ time
+
+        curdate = self.date(index=-1)
+        testdate = parser.parse(date)
+        if testdate is None:
+            raise(Exception("The date u gave can not be parsed to a date."))
+
+        if curdate > testdate:
+            return True
+        return False
 
     def isDate(self, date, time=None):
         if time is not None:
             date = date +" "+ time
 
         curdate = self.date(index=-1)
         lastdate = self.date(index=-3)
@@ -677,15 +689,15 @@
 
         if data is not None:
             return data
 
         return data
 
     def getNow_date(self):
-        dt = self.table.getLast("datetime")
+        dt = self.table.index[-1]
         return dt
 
     def current(self, name):
         return self.get(name, index=-1)
 
     def statistic(self, name="r_master"):
 
@@ -736,14 +748,19 @@
 
     def time(self):
         if len(self.table.index) > 0:
             date = pd.to_datetime(self.table.index[-1])
             return date
         return None
 
+
+    def varInfo(self, name, logicId=None):
+        d = self.getLastData(logicId+".var."+name)
+        return d
+
     ## This method adds a signal
     def var(self, name, data=None, logicId=None):
 
         if data is not None:
             return self._storageManager.setVar(logicId if logicId is not None else self.getUniqueName(), name, data)
 
         return self._storageManager.getVar(logicId if logicId is not None else self.getUniqueName(), name)
```

### Comparing `coinlib-2.2.5/coinlib/BasicJobSessionStorage.py` & `coinlib-2.2.6/coinlib/BasicJobSessionStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     def getLastData(self, key, maxSecondsDistance=None) -> LastSignalValue:
         last = LastSignalValue()
         last.found = False
         last.value = None
         if key in self._lastStorage:
             nv = self._lastStorage[key]
             lastTime = datetime.datetime.strptime(nv.time, "%Y-%m-%d-%H:%M:%S") if isinstance(nv.time, str) else nv.time
-            currentTime = datetime.datetime.strptime(self._lastIndex, "%Y-%m-%d-%H:%M:%S")
+            currentTime = datetime.datetime.strptime(self._currentIndex, "%Y-%m-%d-%H:%M:%S")
             ticks = self._currentTicks - nv.ticks if self._currentTicks > 0 else nv.ticks
             distance = (currentTime - lastTime).total_seconds()
             if maxSecondsDistance is not None:
                 if distance > maxSecondsDistance:
                     return last
 
             last.time = nv.time
```

### Comparing `coinlib-2.2.5/coinlib/ChartsIndicatorJob.py` & `coinlib-2.2.6/coinlib/ChartsIndicatorJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/ChartsWorker.py` & `coinlib-2.2.6/coinlib/ChartsWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/CoinlibCrypto.py` & `coinlib-2.2.6/coinlib/CoinlibCrypto.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/CoinlibDataInterface.py` & `coinlib-2.2.6/coinlib/CoinlibDataInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/CoinlibWorkspace.py` & `coinlib-2.2.6/coinlib/CoinlibWorkspace.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/DataWorker.py` & `coinlib-2.2.6/coinlib/DataWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/Functions.py` & `coinlib-2.2.6/coinlib/Functions.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/InfluxDatabase.py` & `coinlib-2.2.6/coinlib/InfluxDatabase.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/PluginLoader.py` & `coinlib-2.2.6/coinlib/PluginLoader.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/PluginsWorker.py` & `coinlib-2.2.6/coinlib/PluginsWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/Registrar.py` & `coinlib-2.2.6/coinlib/Registrar.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/Simulator.py` & `coinlib-2.2.6/coinlib/Simulator.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/WorkerJobProcess.py` & `coinlib-2.2.6/coinlib/WorkerJobProcess.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/__init__.py` & `coinlib-2.2.6/coinlib/__init__.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/broker/Broker.py` & `coinlib-2.2.6/coinlib/broker/Broker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/broker/BrokerDTO.py` & `coinlib-2.2.6/coinlib/broker/BrokerDTO.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/broker/CoinlibBroker.py` & `coinlib-2.2.6/coinlib/broker/CoinlibBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/broker/CoinlibBrokerFuture.py` & `coinlib-2.2.6/coinlib/broker/CoinlibBrokerFuture.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/broker/CoinlibBrokerMargin.py` & `coinlib-2.2.6/coinlib/broker/CoinlibBrokerMargin.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/broker/CoinlibBrokerSpot.py` & `coinlib-2.2.6/coinlib/broker/CoinlibBrokerSpot.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/brokerWorker/BrokerSession.py` & `coinlib-2.2.6/coinlib/brokerWorker/BrokerSession.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/brokerWorker/BrokerSessionWorker.py` & `coinlib-2.2.6/coinlib/brokerWorker/BrokerSessionWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/brokerWorker/BrokerWorker.py` & `coinlib-2.2.6/coinlib/brokerWorker/BrokerWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/brokerWorker/TestProtocolResult.py` & `coinlib-2.2.6/coinlib/brokerWorker/TestProtocolResult.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/coinlibFactory.py` & `coinlib-2.2.6/coinlib/coinlibFactory.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/config.py` & `coinlib-2.2.6/coinlib/config.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/data/CollectionInterface.py` & `coinlib-2.2.6/coinlib/data/CollectionInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/data/DataTable.py` & `coinlib-2.2.6/coinlib/data/DataTable.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,37 +37,44 @@
     def from_df(self, df: pd.DataFrame):
         self._df = df
         self.convertDataFrame(df)
 
     def get_cleared_np_from_df(self, chart):
 
         targetColumn = self._np[self.col[chart+".main:close"],:]
-        indexes = pd.isna(targetColumn)
 
-        new_numpy_transposed = None
-        for d in self.col_chart[chart]:
-            index = self.col_chart[chart][d]
-            new_data = np.delete(self._np[self.col[d]], indexes)
-            if new_numpy_transposed is None:
-                new_numpy_transposed = np.empty([len(self.col_chart[chart]), len(new_data)], dtype=object)
-            new_numpy_transposed[index,:] = new_data
-        index = np.delete(self.index, indexes)
-
-        i = 0
-        index_reference = np.zeros(len(self.index))
-        intern_index = -1
-        for d in indexes:
-            index_reference[i] = intern_index
-            if d == False:
-                intern_index = intern_index + 1
-            i = i + 1
+        new_numpy_transposed = []
+        index = []
+        index_reference = []
+        nextIndex = 0
+
+        # we fill the self._np with the last value when there is a gap
+        for i in range(0, len(targetColumn)):
+            index_reference.append(nextIndex)
+            if targetColumn[i] is None or np.isnan(targetColumn[i]):
+                # all values within the self._np get the last value of the column
+                # but only for all columsn of the same chart
+                for c in self.col_chart[chart]:
+                    if c != "datetime":
+                        self._np[self.col[c], i] = self._np[self.col[c], i-1]
+            else:
+                # we have a valid value
+                # we add the index to the index list
+                index.append(self.index[i])
+                # we add the row to the new numpy array transposed
+                # but only for all columsn of the same chart
+                row = []
+                for c in self.col_chart[chart]:
+                    row.append(self._np[self.col[c], i])
+                new_numpy_transposed.append(row)
+                nextIndex = nextIndex + 1
 
 
         return {
-            "data": new_numpy_transposed,
+            "data": np.array(new_numpy_transposed),
             "index": index,
             "index_reference": index_reference
         }
 
     def convertDataFrame(self, df):
         try:
             self._df = df
@@ -96,14 +103,16 @@
                     data = self.get_cleared_np_from_df(chart)
                     self._np_by_chart[chart] = data["data"]
                     self._index_by_chart[chart] = data["index"]
                     self._index_reference_by_chart[chart] = data["index_reference"]
                 except Exception as e:
                     print("error in generating the speedup datatbles")
 
+            pass
+
         except Exception as e:
             print("Error while converting dataframe ", e)
 
     def rows(self):
         return self._np.transpose()
 
     def asArray(self):
@@ -112,36 +121,35 @@
     def subTable(self, index=0, length=None, columns=None):
         sub = DataTable()
         sub._df = self._df
         sub.columns = self.columns
         sub.col = self.col
         if length is None:
             length = len(self.index)
-        sub.index = self.index[index:index + length]
+        sub.index = self.index[index:index+index]
         #copy_np = self._np.copy()
         try:
             if columns is not None:
                 sub.columns = columns
                 list = []
-                index = 0
+                i = 0
                 cols = {}
                 for c in columns:
-                    list.append(self._np[self.col[c], 0: length].copy())
-                    cols[c] = index
-                    index = index + 1
+                    list.append(self._np[self.col[c], index: index+length].copy())
+                    cols[c] = i
+                    i = i + 1
                 sub._np = np.array(list)
                 sub.col = cols
             else:
-                sub._np = self._np[:, 0: length].copy()
+                sub._np = self._np[:, index: index+length].copy()
                 sub.col_chart = self.col_chart
                 for chart in self.col_chart:
-                    convertedIndex = int(self._index_reference_by_chart[chart][index + length])
+                    convertedIndex = int(self._index_reference_by_chart[chart][index+length])
                     sub._index_by_chart = self._index_reference_by_chart
-                    sub._np_by_chart[chart] = self._np_by_chart[chart][:, (
-                                                                              convertedIndex - length if convertedIndex - length > 0 else 0):convertedIndex]
+                    sub._np_by_chart[chart] = self._np_by_chart[chart][:, convertedIndex: convertedIndex+length].copy()
         except Exception as e:
             print("Error while subtable ", e)
 
         return sub
 
     def setColumn(self, name, data, index=None, pad=True, type=float):
         ## padding needed maybe
@@ -282,18 +290,15 @@
                   clear_nan=True, to_date=None, from_date=None):
         data = None
         datetimes = None
         if name not in self.col:
             return False
 
         chart = name.split(".")[0]
-        if chart in self.col_chart and name in self.col_chart[chart]:
-            targetColumn = self._np_by_chart[chart][self.col_chart[chart][name]]
-        else:
-            targetColumn = self._np[self.col[name]]
+        targetColumn = self._np[self.col[name]]
         indexColumn = self.index
 
         if to_date and not from_date:
             indexColumn = [date for date in indexColumn if date <= to_date]
             targetColumn = targetColumn[0:len(indexColumn)]
 
         if from_date and not to_date:
```

### Comparing `coinlib-2.2.5/coinlib/dataWorker_pb2.py` & `coinlib-2.2.6/coinlib/dataWorker_pb2.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/dataWorker_pb2_grpc.py` & `coinlib-2.2.6/coinlib/dataWorker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/drawable/CoinlibDrawable.py` & `coinlib-2.2.6/coinlib/drawable/CoinlibDrawable.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/drawable/WindowGrid.py` & `coinlib-2.2.6/coinlib/drawable/WindowGrid.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/event/EventConsumer.py` & `coinlib-2.2.6/coinlib/event/EventConsumer.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/event/EventInterface.py` & `coinlib-2.2.6/coinlib/event/EventInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/feature/CoinlibFeature.py` & `coinlib-2.2.6/coinlib/feature/CoinlibFeature.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/feature/CoinlibFeatureFetcher.py` & `coinlib-2.2.6/coinlib/feature/CoinlibFeatureFetcher.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/feature/CoinlibFeatureLake.py` & `coinlib-2.2.6/coinlib/feature/CoinlibFeatureLake.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/feature/FeatureDTO.py` & `coinlib-2.2.6/coinlib/feature/FeatureDTO.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/feature/FeatureWorker.py` & `coinlib-2.2.6/coinlib/feature/FeatureWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/feature/Features.py` & `coinlib-2.2.6/coinlib/feature/Features.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/helper.py` & `coinlib-2.2.6/coinlib/helper.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logger.py` & `coinlib-2.2.6/coinlib/logger.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/Logic.py` & `coinlib-2.2.6/coinlib/logics/Logic.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/LogicBasicWorker.py` & `coinlib-2.2.6/coinlib/logics/LogicBasicWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/LogicJob.py` & `coinlib-2.2.6/coinlib/logics/LogicJob.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,16 @@
         return self.manager.isBacktrader()
 
     #### Symbol Blocks
 
     ##### Trader Blocks
 
     ## reachable through .broker / .trader
+    def time_running_seconds(self):
+        return self.manager.time_running_seconds()
 
     #### Alert blocks
 
     def notification(self, text, notificationModule, images=[], parameters={}, auth={}):
 
         self.manager.saveInfo("notification", "notification",
                               {"text": text, "module": notificationModule, "parameters": parameters})
```

### Comparing `coinlib-2.2.5/coinlib/logics/LogicLoader.py` & `coinlib-2.2.6/coinlib/logics/LogicLoader.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/LogicOfflineJob.py` & `coinlib-2.2.6/coinlib/logics/LogicOfflineJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/LogicOfflineWorker.py` & `coinlib-2.2.6/coinlib/logics/LogicOfflineWorker.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,14 +190,15 @@
 
                     lastindex = index-minimumPeriod if index-minimumPeriod > 0 else 0
 
 
                     subTable = table.subTable(lastindex, minimumPeriod)
 
                     fakeManager.setTable(subTable)
+                    fakeManager.setTimeRunningInSec(index_date.timestamp() - startDate.timestamp())
                     self.onNextSubTableReceived(fakeManager, subTable)
                     fakeManager.updateCurrentIndexToLast()
                     fakeManager.resetChanges()
 
                     self.onBeforeSingleStepRunng(fakeManager, subTable)
 
                     self.runLogicComponents(subTable, fakeManager)
```

### Comparing `coinlib-2.2.5/coinlib/logics/LogicOfflineWorkerTrader.py` & `coinlib-2.2.6/coinlib/logics/LogicOfflineWorkerTrader.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/LogicOnlineJob.py` & `coinlib-2.2.6/coinlib/logics/LogicOnlineJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/LogicOnlineWorker.py` & `coinlib-2.2.6/coinlib/logics/LogicOnlineWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/LogicRegistrationInstance.py` & `coinlib-2.2.6/coinlib/logics/LogicRegistrationInstance.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/LogicTestBrokerWorker.py` & `coinlib-2.2.6/coinlib/logics/LogicTestBrokerWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/broker/LogicBrokerInterface.py` & `coinlib-2.2.6/coinlib/logics/broker/LogicBrokerInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/manager/LogicJobBroker.py` & `coinlib-2.2.6/coinlib/logics/manager/LogicJobBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/manager/LogicManager.py` & `coinlib-2.2.6/coinlib/logics/manager/LogicManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,21 +23,23 @@
 
 class LogicCommandPortfolioDTO:
     assets: List[AssetInfo]
     currentCalculatedMoney: CurrentMoneyInfo
 
 class LogicCommandParams:
     traderName: str
+    timeRunningInSec: int
     portfolio: LogicCommandPortfolioDTO
 
 class LogicManager(BasicJobSessionStorage):
     logicConfig: statsModel.LogicRunnerLogic
     brokerAccount: statsModel.BrokerAccountModel
     _portfolio: PortfolioModel
     _params: LogicCommandParams
+    _time_running_in_sec: int
 
     def __init__(self, name, logicConfig: statsModel.LogicRunnerLogic,
                  brokerAccount: statsModel.BrokerAccountModel=statsModel.BrokerAccountModel(),
                  portfolio: PortfolioModel = None, infoStorage = None, options: LogicOptions = None,
                  advancedInfo = None):
         super(LogicManager, self).__init__(infoStorage)
         self.table: DataTable = DataTable()
@@ -50,23 +52,27 @@
         self.loop = asyncio.new_event_loop()
         self.appWorkerId = logicConfig.app_worker_id
         self.appWorkerRunnerId = logicConfig.app_worker_runner_id
         self.advancedInfo = advancedInfo
         if portfolio is None:
             portfolio = PortfolioModel()
         self._portfolio = portfolio
+        self._time_running_in_sec = 0
         self.brokerAccount = brokerAccount
         self.name = name
         self.logicConfig = logicConfig
 
         pass
 
     def getOptions(self):
         return self.logicOptions
 
+    def time_running_seconds(self):
+        return self._time_running_in_sec
+
     def send_worker_data_to_queue_sync(self, force=False):
         newLoop = asyncio.new_event_loop()
         timeDistanceInSeconds = time.time() - self._lastTimeLogQueueWasRunning
         if force or (not self._sendLogQueueRunning and timeDistanceInSeconds > 5):
             self._lastTimeLogQueueWasRunning = time.time()
 
             newLoop.run_until_complete(self.send_worker_data_to_queue(loop=newLoop))
@@ -143,14 +149,15 @@
         return self.appWorkerId
 
     def getAppWorkerActivityIdentifier(self):
         return self.appWorkerRunnerId
 
     def setLogicParams(self, params: LogicCommandParams):
         self._params = params
+        self._timeRunningInSec = params.timeRunningInSec
         return True
 
     def updatePortfolio(self, newPortfolio: PortfolioModel):
         #print("update portfolio with: "+str(self._portfolio.currentMoney.summary))
         self._portfolio = newPortfolio
 
     def getSymbolForChart(self, chartId=None):
@@ -264,7 +271,10 @@
         return self._portfolio
 
     def getFreePortfolioQuoteMoney(self):
         return self._portfolio.currentMoney.free
 
     def getPortfolioQuoteMoney(self):
         return self._portfolio.currentMoney.summary
+
+    def setTimeRunningInSec(self, time_running_in_sec):
+        self._time_running_in_sec = time_running_in_sec
```

### Comparing `coinlib-2.2.5/coinlib/logics/manager/PortfolioModel.py` & `coinlib-2.2.6/coinlib/logics/manager/PortfolioModel.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py` & `coinlib-2.2.6/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py` & `coinlib-2.2.6/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py` & `coinlib-2.2.6/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/logics/onlineManager/LogicOnlineJobBroker.py` & `coinlib-2.2.6/coinlib/logics/onlineManager/LogicOnlineJobBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/notification/Notification.py` & `coinlib-2.2.6/coinlib/notification/Notification.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/notification/NotificationWorker.py` & `coinlib-2.2.6/coinlib/notification/NotificationWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/statistics/StatisticMethodJob.py` & `coinlib-2.2.6/coinlib/statistics/StatisticMethodJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/statistics/StatisticRuleJob.py` & `coinlib-2.2.6/coinlib/statistics/StatisticRuleJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/statistics/Statistics.py` & `coinlib-2.2.6/coinlib/statistics/Statistics.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/statistics/StatisticsMethodWorker.py` & `coinlib-2.2.6/coinlib/statistics/StatisticsMethodWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/statistics/StatisticsRuleWorker.py` & `coinlib-2.2.6/coinlib/statistics/StatisticsRuleWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/symbols/SymbolWorker.py` & `coinlib-2.2.6/coinlib/symbols/SymbolWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib/symbols/Symbols.py` & `coinlib-2.2.6/coinlib/symbols/Symbols.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/coinlib.egg-info/PKG-INFO` & `coinlib-2.2.6/coinlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinlib
-Version: 2.2.5
+Version: 2.2.6
 Summary: Develop new code for your coindeck environment
 Home-page: https://gitlab.com/coindeck/coinlib
 Author: coindeck
 Author-email: donnercody86@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `coinlib-2.2.5/coinlib.egg-info/SOURCES.txt` & `coinlib-2.2.6/coinlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/setup.py` & `coinlib-2.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README_pip.md")) as fid:
     README = fid.read()
 
 # This call to setup() does all the work
 setup(
     name="coinlib",
-    version="2.2.5",
+    version="2.2.6",
     description="Develop new code for your coindeck environment",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/coindeck/coinlib",
     author="coindeck",
     author_email="donnercody86@gmail.com",
     license="MIT",
```

### Comparing `coinlib-2.2.5/test/testchartworker.py` & `coinlib-2.2.6/test/testchartworker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/test/testcross.py` & `coinlib-2.2.6/test/testcross.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.5/test/testplot.py` & `coinlib-2.2.6/test/testplot.py`

 * *Files identical despite different names*

