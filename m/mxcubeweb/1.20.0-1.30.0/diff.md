# Comparing `tmp/mxcubeweb-1.20.0.tar.gz` & `tmp/mxcubeweb-1.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxcubeweb-1.20.0.tar", max compression
+gzip compressed data, was "mxcubeweb-1.30.0.tar", max compression
```

## Comparing `mxcubeweb-1.20.0.tar` & `mxcubeweb-1.30.0.tar`

### file list

```diff
@@ -1,78 +1,67 @@
--rw-r--r--   0        0        0     7652 2022-06-24 08:47:25.414449 mxcubeweb-1.20.0/LICENSE
--rw-r--r--   0        0        0     3522 2022-11-29 15:24:36.217460 mxcubeweb-1.20.0/README.md
--rw-r--r--   0        0        0     3584 2023-05-26 04:23:36.809782 mxcubeweb-1.20.0/mxcube3/__init__.py
--rw-r--r--   0        0        0     3778 2023-03-20 10:13:15.238458 mxcubeweb-1.20.0/mxcube3/__init__.py.orig
--rw-r--r--   0        0        0    17723 2023-06-08 06:21:07.999553 mxcubeweb-1.20.0/mxcube3/app.py
--rw-r--r--   0        0        0    17361 2023-01-05 13:58:02.312280 mxcubeweb-1.20.0/mxcube3/app.py.orig
--rw-r--r--   0        0        0     1409 2023-01-18 08:28:39.601143 mxcubeweb-1.20.0/mxcube3/config.py
--rw-r--r--   0        0        0        0 2022-06-24 08:47:25.414449 mxcubeweb-1.20.0/mxcube3/core/__init__.py
--rw-r--r--   0        0        0        0 2023-01-18 08:28:39.601143 mxcubeweb-1.20.0/mxcube3/core/adapter/__init__.py
--rw-r--r--   0        0        0     2408 2023-01-18 08:28:39.601143 mxcubeweb-1.20.0/mxcube3/core/adapter/actuator_adapter.py
--rw-r--r--   0        0        0    13582 2023-06-08 06:18:31.787733 mxcubeweb-1.20.0/mxcube3/core/adapter/adapter_base.py
--rw-r--r--   0        0        0     1846 2023-01-18 08:28:39.601143 mxcubeweb-1.20.0/mxcube3/core/adapter/beam_adapter.py
--rw-r--r--   0        0        0     1642 2023-01-18 08:28:39.601143 mxcubeweb-1.20.0/mxcube3/core/adapter/beamline_action_adapter.py
--rw-r--r--   0        0        0     2689 2023-06-08 06:21:08.003553 mxcubeweb-1.20.0/mxcube3/core/adapter/beamline_adapter.py
--rw-r--r--   0        0        0     1586 2023-05-26 04:23:36.809782 mxcubeweb-1.20.0/mxcube3/core/adapter/data_publisher_adapter.py
--rw-r--r--   0        0        0      494 2023-05-26 04:23:36.809782 mxcubeweb-1.20.0/mxcube3/core/adapter/detector_adapter.py
--rw-r--r--   0        0        0      988 2023-06-08 06:21:08.003553 mxcubeweb-1.20.0/mxcube3/core/adapter/diffractometer_adapter.py
--rw-r--r--   0        0        0     1420 2023-02-16 14:09:06.824261 mxcubeweb-1.20.0/mxcube3/core/adapter/diffractometer_adapter.py.orig
--rw-r--r--   0        0        0      591 2022-10-19 14:19:09.327226 mxcubeweb-1.20.0/mxcube3/core/adapter/energy_adapter.py
--rw-r--r--   0        0        0     1384 2023-01-18 08:28:39.601143 mxcubeweb-1.20.0/mxcube3/core/adapter/flux_adapter.py
--rw-r--r--   0        0        0     2111 2023-01-18 08:28:39.601143 mxcubeweb-1.20.0/mxcube3/core/adapter/machine_info_adapter.py
--rw-r--r--   0        0        0     2218 2023-06-08 06:18:31.787733 mxcubeweb-1.20.0/mxcube3/core/adapter/motor_adapter.py
--rw-r--r--   0        0        0     1763 2023-01-18 08:28:39.601143 mxcubeweb-1.20.0/mxcube3/core/adapter/nstate_adapter.py
--rw-r--r--   0        0        0     2905 2023-01-18 08:28:39.601143 mxcubeweb-1.20.0/mxcube3/core/adapter/wavelength_adapter.py
--rw-r--r--   0        0        0    12293 2023-05-26 04:23:36.809782 mxcubeweb-1.20.0/mxcube3/core/components/beamline.py
--rw-r--r--   0        0        0     1384 2023-01-18 08:28:39.605143 mxcubeweb-1.20.0/mxcube3/core/components/chat.py
--rw-r--r--   0        0        0      630 2022-10-19 14:19:09.327226 mxcubeweb-1.20.0/mxcube3/core/components/component_base.py
--rw-r--r--   0        0        0    16902 2023-06-08 06:21:08.003553 mxcubeweb-1.20.0/mxcube3/core/components/lims.py
--rw-r--r--   0        0        0    90181 2023-06-08 06:21:08.003553 mxcubeweb-1.20.0/mxcube3/core/components/queue.py
--rw-r--r--   0        0        0    94121 2023-01-05 13:58:02.312280 mxcubeweb-1.20.0/mxcube3/core/components/queue.py.orig
--rw-r--r--   0        0        0    18590 2023-06-08 06:21:08.003553 mxcubeweb-1.20.0/mxcube3/core/components/samplechanger.py
--rw-r--r--   0        0        0    22573 2023-06-08 06:18:31.787733 mxcubeweb-1.20.0/mxcube3/core/components/sampleview.py
--rw-r--r--   0        0        0     1896 2023-01-18 08:28:39.605143 mxcubeweb-1.20.0/mxcube3/core/components/user/database.py
--rw-r--r--   0        0        0      418 2022-10-19 14:19:09.327226 mxcubeweb-1.20.0/mxcube3/core/components/user/dummyusermanager.py
--rw-r--r--   0        0        0    15081 2023-06-08 06:18:31.787733 mxcubeweb-1.20.0/mxcube3/core/components/user/usermanager.py
--rw-r--r--   0        0        0    14383 2023-03-20 10:14:56.850147 mxcubeweb-1.20.0/mxcube3/core/components/user/usermanager.py.orig
--rw-r--r--   0        0        0     1986 2022-10-19 14:19:09.327226 mxcubeweb-1.20.0/mxcube3/core/components/workflow.py
--rw-r--r--   0        0        0     2344 2023-01-18 08:28:39.605143 mxcubeweb-1.20.0/mxcube3/core/models/adaptermodels.py
--rw-r--r--   0        0        0     2689 2023-05-26 04:23:36.809782 mxcubeweb-1.20.0/mxcube3/core/models/configmodels.py
--rw-r--r--   0        0        0      254 2023-01-18 08:28:39.605143 mxcubeweb-1.20.0/mxcube3/core/models/generic.py
--rw-r--r--   0        0        0      299 2023-01-05 13:57:32.808278 mxcubeweb-1.20.0/mxcube3/core/models/generic.py.orig
--rw-r--r--   0        0        0     3359 2023-05-26 04:23:36.813782 mxcubeweb-1.20.0/mxcube3/core/models/usermodels.py
--rw-r--r--   0        0        0     2344 2023-05-26 04:23:36.813782 mxcubeweb-1.20.0/mxcube3/core/util/adapterutils.py
--rw-r--r--   0        0        0     1630 2022-10-19 14:19:09.327226 mxcubeweb-1.20.0/mxcube3/core/util/convertutils.py
--rw-r--r--   0        0        0      523 2022-10-19 14:19:09.327226 mxcubeweb-1.20.0/mxcube3/core/util/fsutils.py
--rw-r--r--   0        0        0     4507 2022-11-25 09:06:04.564685 mxcubeweb-1.20.0/mxcube3/core/util/networkutils.py
--rw-r--r--   0        0        0     1188 2023-01-18 08:28:39.605143 mxcubeweb-1.20.0/mxcube3/logging_handler.py
--rw-r--r--   0        0        0        0 2023-01-18 08:28:39.605143 mxcubeweb-1.20.0/mxcube3/routes/__init__.py
--rw-r--r--   0        0        0     8128 2023-03-20 10:15:28.554050 mxcubeweb-1.20.0/mxcube3/routes/beamline.py
--rw-r--r--   0        0        0      859 2023-05-26 04:23:36.813782 mxcubeweb-1.20.0/mxcube3/routes/detector.py
--rw-r--r--   0        0        0     4033 2022-10-19 14:19:09.327226 mxcubeweb-1.20.0/mxcube3/routes/diffractometer.py
--rw-r--r--   0        0        0     5165 2023-01-18 08:28:39.605143 mxcubeweb-1.20.0/mxcube3/routes/lims.py
--rw-r--r--   0        0        0      563 2022-10-19 14:19:09.327226 mxcubeweb-1.20.0/mxcube3/routes/log.py
--rw-r--r--   0        0        0     3235 2023-06-08 06:18:31.787733 mxcubeweb-1.20.0/mxcube3/routes/login.py
--rw-r--r--   0        0        0     3294 2023-04-26 06:02:22.777096 mxcubeweb-1.20.0/mxcube3/routes/login.py.orig
--rw-r--r--   0        0        0     2613 2023-05-26 04:23:36.813782 mxcubeweb-1.20.0/mxcube3/routes/main.py
--rw-r--r--   0        0        0     3355 2023-03-29 06:09:47.528078 mxcubeweb-1.20.0/mxcube3/routes/main.py.orig
--rw-r--r--   0        0        0     4291 2023-05-26 04:23:36.813782 mxcubeweb-1.20.0/mxcube3/routes/mockups.py
--rw-r--r--   0        0        0    10369 2023-06-08 06:21:08.003553 mxcubeweb-1.20.0/mxcube3/routes/queue.py
--rw-r--r--   0        0        0     6224 2023-05-26 04:23:36.813782 mxcubeweb-1.20.0/mxcube3/routes/ra.py
--rw-r--r--   0        0        0    13766 2023-06-08 06:18:31.787733 mxcubeweb-1.20.0/mxcube3/routes/samplecentring.py
--rw-r--r--   0        0        0     4671 2023-01-18 08:28:39.609143 mxcubeweb-1.20.0/mxcube3/routes/samplechanger.py
--rw-r--r--   0        0        0    20592 2023-06-08 06:18:28.263737 mxcubeweb-1.20.0/mxcube3/routes/signals.py
--rw-r--r--   0        0        0     1125 2022-10-19 14:19:09.331226 mxcubeweb-1.20.0/mxcube3/routes/workflow.py
--rw-r--r--   0        0        0     6709 2023-05-26 04:23:36.813782 mxcubeweb-1.20.0/mxcube3/server.py
--rw-r--r--   0        0        0     7025 2022-11-07 07:54:22.889232 mxcubeweb-1.20.0/mxcube3/server.py.orig
--rw-r--r--   0        0        0     1396 2023-03-29 06:08:13.484073 mxcubeweb-1.20.0/mxcube3/state_storage.py
--rw-r--r--   0        0        0      771 2022-06-24 08:47:25.418449 mxcubeweb-1.20.0/mxcube3/templates/characterisation-results.js
--rw-r--r--   0        0        0     3610 2022-06-24 08:47:25.418449 mxcubeweb-1.20.0/mxcube3/templates/data-collection-results.html
--rw-r--r--   0        0        0   329138 2022-11-21 09:20:51.834118 mxcubeweb-1.20.0/mxcube3/templates/precompiled.templates.min.js
--rw-r--r--   0        0        0      721 2022-06-24 08:47:25.422448 mxcubeweb-1.20.0/mxcube3/templates/workflow-results.js
--rw-r--r--   0        0        0     1316 2022-11-25 08:58:39.005902 mxcubeweb-1.20.0/mxcube3/timing_logger.py
--rw-r--r--   0        0        0       22 2022-10-19 14:19:09.331226 mxcubeweb-1.20.0/mxcube3/version.py
--rw-r--r--   0        0        0        0 2022-06-24 08:47:25.422448 mxcubeweb-1.20.0/mxcube3/video/__init__.py
--rw-r--r--   0        0        0     2647 2022-06-24 08:47:25.422448 mxcubeweb-1.20.0/mxcube3/video/websocket-relay.js
--rw-r--r--   0        0        0     1785 2023-06-08 07:10:40.796134 mxcubeweb-1.20.0/pyproject.toml
--rw-r--r--   0        0        0     5158 1970-01-01 00:00:00.000000 mxcubeweb-1.20.0/setup.py
--rw-r--r--   0        0        0     5368 1970-01-01 00:00:00.000000 mxcubeweb-1.20.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/LICENSE
+-rw-r--r--   0        0        0     3522 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/README.md
+-rw-r--r--   0        0        0     3584 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/__init__.py
+-rw-r--r--   0        0        0    17723 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/app.py
+-rw-r--r--   0        0        0     1409 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/config.py
+-rw-r--r--   0        0        0        0 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/core/adapter/__init__.py
+-rw-r--r--   0        0        0     2408 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/core/adapter/actuator_adapter.py
+-rw-r--r--   0        0        0    13582 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/core/adapter/adapter_base.py
+-rw-r--r--   0        0        0     1846 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/core/adapter/beam_adapter.py
+-rw-r--r--   0        0        0     1642 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/core/adapter/beamline_action_adapter.py
+-rw-r--r--   0        0        0     2689 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/core/adapter/beamline_adapter.py
+-rw-r--r--   0        0        0     1586 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/core/adapter/data_publisher_adapter.py
+-rw-r--r--   0        0        0      494 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/core/adapter/detector_adapter.py
+-rw-r--r--   0        0        0      988 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/core/adapter/diffractometer_adapter.py
+-rw-r--r--   0        0        0      591 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/core/adapter/energy_adapter.py
+-rw-r--r--   0        0        0     1384 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/core/adapter/flux_adapter.py
+-rw-r--r--   0        0        0     2111 2023-06-08 12:15:33.626231 mxcubeweb-1.30.0/mxcube3/core/adapter/machine_info_adapter.py
+-rw-r--r--   0        0        0     2218 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/adapter/motor_adapter.py
+-rw-r--r--   0        0        0     1763 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/adapter/nstate_adapter.py
+-rw-r--r--   0        0        0     2905 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/adapter/wavelength_adapter.py
+-rw-r--r--   0        0        0    12293 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/components/beamline.py
+-rw-r--r--   0        0        0     1384 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/components/chat.py
+-rw-r--r--   0        0        0      630 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/components/component_base.py
+-rw-r--r--   0        0        0    16902 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/components/lims.py
+-rw-r--r--   0        0        0    90181 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/components/queue.py
+-rw-r--r--   0        0        0    18591 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/components/samplechanger.py
+-rw-r--r--   0        0        0    22573 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/components/sampleview.py
+-rw-r--r--   0        0        0     1896 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/components/user/database.py
+-rw-r--r--   0        0        0      418 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/components/user/dummyusermanager.py
+-rw-r--r--   0        0        0    15081 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/components/user/usermanager.py
+-rw-r--r--   0        0        0     1986 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/components/workflow.py
+-rw-r--r--   0        0        0     2344 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/models/adaptermodels.py
+-rw-r--r--   0        0        0     2689 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/models/configmodels.py
+-rw-r--r--   0        0        0      254 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/models/generic.py
+-rw-r--r--   0        0        0     3359 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/models/usermodels.py
+-rw-r--r--   0        0        0     2344 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/util/adapterutils.py
+-rw-r--r--   0        0        0     1630 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/util/convertutils.py
+-rw-r--r--   0        0        0      523 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/util/fsutils.py
+-rw-r--r--   0        0        0     4507 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/core/util/networkutils.py
+-rw-r--r--   0        0        0     1188 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/logging_handler.py
+-rw-r--r--   0        0        0        0 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/routes/__init__.py
+-rw-r--r--   0        0        0     8128 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/routes/beamline.py
+-rw-r--r--   0        0        0      859 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/routes/detector.py
+-rw-r--r--   0        0        0     4033 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/routes/diffractometer.py
+-rw-r--r--   0        0        0     5165 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/routes/lims.py
+-rw-r--r--   0        0        0      563 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/routes/log.py
+-rw-r--r--   0        0        0     3235 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/routes/login.py
+-rw-r--r--   0        0        0     2613 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/routes/main.py
+-rw-r--r--   0        0        0     4291 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/routes/mockups.py
+-rw-r--r--   0        0        0    10369 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/routes/queue.py
+-rw-r--r--   0        0        0     6224 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/routes/ra.py
+-rw-r--r--   0        0        0    13766 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/routes/samplecentring.py
+-rw-r--r--   0        0        0     4671 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/routes/samplechanger.py
+-rw-r--r--   0        0        0    20592 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/routes/signals.py
+-rw-r--r--   0        0        0     1125 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/routes/workflow.py
+-rw-r--r--   0        0        0     6709 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/server.py
+-rw-r--r--   0        0        0     1396 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/state_storage.py
+-rw-r--r--   0        0        0      771 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/templates/characterisation-results.js
+-rw-r--r--   0        0        0     3610 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/templates/data-collection-results.html
+-rw-r--r--   0        0        0   329138 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/templates/precompiled.templates.min.js
+-rw-r--r--   0        0        0      721 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/templates/workflow-results.js
+-rw-r--r--   0        0        0       22 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/version.py
+-rw-r--r--   0        0        0        0 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/video/__init__.py
+-rw-r--r--   0        0        0     2647 2023-06-08 12:15:33.630231 mxcubeweb-1.30.0/mxcube3/video/websocket-relay.js
+-rw-r--r--   0        0        0     1785 2023-06-08 12:15:50.906349 mxcubeweb-1.30.0/pyproject.toml
+-rw-r--r--   0        0        0     5368 1970-01-01 00:00:00.000000 mxcubeweb-1.30.0/PKG-INFO
```

### Comparing `mxcubeweb-1.20.0/LICENSE` & `mxcubeweb-1.30.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/README.md` & `mxcubeweb-1.30.0/README.md`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/__init__.py` & `mxcubeweb-1.30.0/mxcube3/__init__.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/app.py` & `mxcubeweb-1.30.0/mxcube3/app.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/config.py` & `mxcubeweb-1.30.0/mxcube3/config.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/adapter/actuator_adapter.py` & `mxcubeweb-1.30.0/mxcube3/core/adapter/actuator_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/adapter/adapter_base.py` & `mxcubeweb-1.30.0/mxcube3/core/adapter/adapter_base.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/adapter/beam_adapter.py` & `mxcubeweb-1.30.0/mxcube3/core/adapter/beam_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/adapter/beamline_action_adapter.py` & `mxcubeweb-1.30.0/mxcube3/core/adapter/beamline_action_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/adapter/beamline_adapter.py` & `mxcubeweb-1.30.0/mxcube3/core/adapter/beamline_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/adapter/data_publisher_adapter.py` & `mxcubeweb-1.30.0/mxcube3/core/adapter/data_publisher_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/adapter/diffractometer_adapter.py` & `mxcubeweb-1.30.0/mxcube3/core/adapter/diffractometer_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/adapter/energy_adapter.py` & `mxcubeweb-1.30.0/mxcube3/core/adapter/energy_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/adapter/flux_adapter.py` & `mxcubeweb-1.30.0/mxcube3/core/adapter/flux_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/adapter/machine_info_adapter.py` & `mxcubeweb-1.30.0/mxcube3/core/adapter/machine_info_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/adapter/motor_adapter.py` & `mxcubeweb-1.30.0/mxcube3/core/adapter/motor_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/adapter/nstate_adapter.py` & `mxcubeweb-1.30.0/mxcube3/core/adapter/nstate_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/adapter/wavelength_adapter.py` & `mxcubeweb-1.30.0/mxcube3/core/adapter/wavelength_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/components/beamline.py` & `mxcubeweb-1.30.0/mxcube3/core/components/beamline.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/components/chat.py` & `mxcubeweb-1.30.0/mxcube3/core/components/chat.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/components/component_base.py` & `mxcubeweb-1.30.0/mxcube3/core/components/component_base.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/components/lims.py` & `mxcubeweb-1.30.0/mxcube3/core/components/lims.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/components/queue.py` & `mxcubeweb-1.30.0/mxcube3/core/components/queue.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/components/samplechanger.py` & `mxcubeweb-1.30.0/mxcube3/core/components/samplechanger.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                 if res is None:
                     res = True
                 if (
                     res
                     and self.app.CENTRING_METHOD == queue_entry.CENTRING_METHOD.LOOP
                     and not HWR.beamline.diffractometer.in_plate_mode()
                 ):
-                    HWR.beamline.diffractometer.rejectCentring()
+                    HWR.beamline.diffractometer.reject_centring()
                     msg = "Starting autoloop centring ..."
                     logging.getLogger("MX3.HWR").info(msg)
                     C3D_MODE = HWR.beamline.diffractometer.C3D_MODE
                     HWR.beamline.diffractometer.start_centring_method(C3D_MODE)
 
             else:
                 msg = "Mounting sample: %s" % sample["sampleName"]
```

### Comparing `mxcubeweb-1.20.0/mxcube3/core/components/sampleview.py` & `mxcubeweb-1.30.0/mxcube3/core/components/sampleview.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/components/user/database.py` & `mxcubeweb-1.30.0/mxcube3/core/components/user/database.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/components/user/usermanager.py` & `mxcubeweb-1.30.0/mxcube3/core/components/user/usermanager.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/components/workflow.py` & `mxcubeweb-1.30.0/mxcube3/core/components/workflow.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/models/adaptermodels.py` & `mxcubeweb-1.30.0/mxcube3/core/models/adaptermodels.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/models/configmodels.py` & `mxcubeweb-1.30.0/mxcube3/core/models/configmodels.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/models/usermodels.py` & `mxcubeweb-1.30.0/mxcube3/core/models/usermodels.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/util/adapterutils.py` & `mxcubeweb-1.30.0/mxcube3/core/util/adapterutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/util/convertutils.py` & `mxcubeweb-1.30.0/mxcube3/core/util/convertutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/util/fsutils.py` & `mxcubeweb-1.30.0/mxcube3/core/util/fsutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/core/util/networkutils.py` & `mxcubeweb-1.30.0/mxcube3/core/util/networkutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/logging_handler.py` & `mxcubeweb-1.30.0/mxcube3/logging_handler.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/routes/beamline.py` & `mxcubeweb-1.30.0/mxcube3/routes/beamline.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/routes/detector.py` & `mxcubeweb-1.30.0/mxcube3/routes/detector.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/routes/diffractometer.py` & `mxcubeweb-1.30.0/mxcube3/routes/diffractometer.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/routes/lims.py` & `mxcubeweb-1.30.0/mxcube3/routes/lims.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/routes/log.py` & `mxcubeweb-1.30.0/mxcube3/routes/log.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/routes/login.py` & `mxcubeweb-1.30.0/mxcube3/routes/login.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/routes/main.py` & `mxcubeweb-1.30.0/mxcube3/routes/main.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/routes/mockups.py` & `mxcubeweb-1.30.0/mxcube3/routes/mockups.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/routes/queue.py` & `mxcubeweb-1.30.0/mxcube3/routes/queue.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/routes/ra.py` & `mxcubeweb-1.30.0/mxcube3/routes/ra.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/routes/samplecentring.py` & `mxcubeweb-1.30.0/mxcube3/routes/samplecentring.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/routes/samplechanger.py` & `mxcubeweb-1.30.0/mxcube3/routes/samplechanger.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/routes/signals.py` & `mxcubeweb-1.30.0/mxcube3/routes/signals.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/routes/workflow.py` & `mxcubeweb-1.30.0/mxcube3/routes/workflow.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/server.py` & `mxcubeweb-1.30.0/mxcube3/server.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/state_storage.py` & `mxcubeweb-1.30.0/mxcube3/state_storage.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/templates/characterisation-results.js` & `mxcubeweb-1.30.0/mxcube3/templates/characterisation-results.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/templates/data-collection-results.html` & `mxcubeweb-1.30.0/mxcube3/templates/data-collection-results.html`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/templates/precompiled.templates.min.js` & `mxcubeweb-1.30.0/mxcube3/templates/precompiled.templates.min.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/templates/workflow-results.js` & `mxcubeweb-1.30.0/mxcube3/templates/workflow-results.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/mxcube3/video/websocket-relay.js` & `mxcubeweb-1.30.0/mxcube3/video/websocket-relay.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.20.0/pyproject.toml` & `mxcubeweb-1.30.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mxcubeweb"
-version = "1.20.0"
+version = "1.30.0"
 license = "LGPL-3.0-or-later"
 description = "MXCuBE Web user interface"
 authors = ["The MXCuBE collaboration <mxcube@esrf.fr>"]
 maintainers = [
     "MXCuBE collaboration <mxcube@esrf.fr>",
 ]
 readme = "README.md"
```

### Comparing `mxcubeweb-1.20.0/PKG-INFO` & `mxcubeweb-1.30.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxcubeweb
-Version: 1.20.0
+Version: 1.30.0
 Summary: MXCuBE Web user interface
 Home-page: http://github.com/mxcube/mxcubeweb
 License: LGPL-3.0-or-later
 Keywords: mxcube,mxcube3,mxcubeweb
 Author: The MXCuBE collaboration
 Author-email: mxcube@esrf.fr
 Maintainer: MXCuBE collaboration
```

