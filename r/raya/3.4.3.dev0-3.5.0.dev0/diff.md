# Comparing `tmp/raya-3.4.3.dev0.tar.gz` & `tmp/raya-3.5.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raya-3.4.3.dev0.tar", last modified: Wed Jun  7 02:53:20 2023, max compression
+gzip compressed data, was "raya-3.5.0.dev0.tar", last modified: Thu Jun  8 01:58:14 2023, max compression
```

## Comparing `raya-3.4.3.dev0.tar` & `raya-3.5.0.dev0.tar`

### file list

```diff
@@ -1,75 +1,85 @@
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.686632 raya-3.4.3.dev0/
--rw-rw-r--   0 prod      (1001) prod      (1001)      568 2023-06-07 02:53:20.686632 raya-3.4.3.dev0/PKG-INFO
--rw-rw-r--   0 prod      (1001) prod      (1001)      150 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/README.md
--rw-rw-r--   0 prod      (1001) prod      (1001)      103 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/pyproject.toml
--rw-rw-r--   0 prod      (1001) prod      (1001)       38 2023-06-07 02:53:20.686632 raya-3.4.3.dev0/setup.cfg
--rw-rw-r--   0 prod      (1001) prod      (1001)     2752 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/setup.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.682632 raya-3.4.3.dev0/src/
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.682632 raya-3.4.3.dev0/src/raya/
--rw-rw-r--   0 prod      (1001) prod      (1001)       38 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/src/raya/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       25 2023-06-07 02:53:11.000000 raya-3.4.3.dev0/src/raya/_version.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     3183 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/application_base.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      664 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/constants.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.682632 raya-3.4.3.dev0/src/raya/controllers/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/src/raya/controllers/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      260 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/analytics_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)    17485 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/arms_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      620 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/base_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       90 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/base_pseudo_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1222 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/cameras_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      425 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/controllers/communication_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2838 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/controllers/cv_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1387 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/fleet_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      523 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/grasping_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      924 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/controllers/interactions_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1298 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/leds_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1171 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/lidar_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     3127 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/manipulation_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2042 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/controllers/motion_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     7148 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/navigation_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1367 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/sensors_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      808 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/skills_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2590 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/controllers/sound_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     8614 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya/controllers/ui_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       59 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/entry_point.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     4681 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/enumerations.py
--rw-rw-r--   0 prod      (1001) prod      (1001)    13099 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/exceptions.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     6272 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/exceptions_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.682632 raya-3.4.3.dev0/src/raya/handlers/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/src/raya/handlers/__init__.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.686632 raya-3.4.3.dev0/src/raya/handlers/cv/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/src/raya/handlers/cv/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      877 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/classifier_handler_base.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      844 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/detector_handler_base.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      743 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/estimator_handler_base.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      302 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/faces_detector_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      831 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/faces_recognizer_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      305 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/hand_estimator_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      183 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/model_base.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      790 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/objects_classifier_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      782 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/objects_detector_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      794 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/objects_segmentator_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      783 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/planes_segmentator_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      862 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/recognizer_handler_base.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      871 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/segmentator_handler_base.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      703 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/cv/tags_detector_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.686632 raya-3.4.3.dev0/src/raya/handlers/general/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/src/raya/handlers/general/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      330 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/handlers/general/callback_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.686632 raya-3.4.3.dev0/src/raya/listeners/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/src/raya/listeners/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       77 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/listeners/lidar_listeners.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      160 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/listeners/sensors_listeners.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      352 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/logger.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2055 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/raya_interface.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      257 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/standalone_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.686632 raya-3.4.3.dev0/src/raya/tools/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.4.3.dev0/src/raya/tools/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      399 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/tools/filesystem.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      984 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/tools/fsm.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      152 2023-06-07 02:53:19.000000 raya-3.4.3.dev0/src/raya/tools/image.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-07 02:53:20.682632 raya-3.4.3.dev0/src/raya.egg-info/
--rw-rw-r--   0 prod      (1001) prod      (1001)      568 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya.egg-info/PKG-INFO
--rw-rw-r--   0 prod      (1001) prod      (1001)     2306 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya.egg-info/SOURCES.txt
--rw-rw-r--   0 prod      (1001) prod      (1001)        1 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya.egg-info/dependency_links.txt
--rw-rw-r--   0 prod      (1001) prod      (1001)        5 2023-06-07 02:53:20.000000 raya-3.4.3.dev0/src/raya.egg-info/top_level.txt
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.440130 raya-3.5.0.dev0/
+-rw-rw-r--   0 prod      (1001) prod      (1001)      568 2023-06-08 01:58:14.440130 raya-3.5.0.dev0/PKG-INFO
+-rw-rw-r--   0 prod      (1001) prod      (1001)      150 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/README.md
+-rw-rw-r--   0 prod      (1001) prod      (1001)      103 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/pyproject.toml
+-rw-rw-r--   0 prod      (1001) prod      (1001)       38 2023-06-08 01:58:14.440130 raya-3.5.0.dev0/setup.cfg
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2752 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/setup.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/
+-rw-rw-r--   0 prod      (1001) prod      (1001)       38 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/src/raya/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       25 2023-06-08 01:58:04.000000 raya-3.5.0.dev0/src/raya/_version.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     3183 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/application_base.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      664 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/constants.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/controllers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/src/raya/controllers/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      260 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya/controllers/analytics_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)    25655 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya/controllers/arms_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      952 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/base_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       90 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/base_pseudo_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1289 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/cameras_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      425 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/communication_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2934 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/cv_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1387 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/fleet_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      523 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/grasping_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      924 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/interactions_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1298 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/leds_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1171 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/lidar_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     3127 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/manipulation_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2436 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/motion_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     7148 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/navigation_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1367 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/sensors_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      808 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya/controllers/skills_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2590 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/controllers/sound_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     8614 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya/controllers/ui_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       59 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/entry_point.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     4876 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/enumerations.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)    14002 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/exceptions.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     6639 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/exceptions_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/src/raya/handlers/__init__.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/cv/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/src/raya/handlers/cv/__init__.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/cv/classifiers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.0.dev0/src/raya/handlers/cv/classifiers/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1211 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/classifiers/classifier_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      802 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/classifiers/objects_classifier_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/cv/detectors/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.0.dev0/src/raya/handlers/cv/detectors/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1168 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/detectors/detector_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      312 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/detectors/faces_detector_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      792 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/detectors/objects_detector_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      713 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/detectors/tags_detector_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/cv/estimators/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.0.dev0/src/raya/handlers/cv/estimators/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1069 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/estimators/estimator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      316 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/estimators/hand_estimator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      197 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/model_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/cv/recognizers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.0.dev0/src/raya/handlers/cv/recognizers/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      843 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/recognizers/faces_recognizer_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1190 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/recognizers/recognizer_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/cv/segmentators/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.0.dev0/src/raya/handlers/cv/segmentators/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      807 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/segmentators/objects_segmentator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      796 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/segmentators/planes_segmentator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1201 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/cv/segmentators/segmentator_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/handlers/general/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/src/raya/handlers/general/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      330 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/handlers/general/callback_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/listeners/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/src/raya/listeners/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       77 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/listeners/lidar_listeners.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      160 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/listeners/sensors_listeners.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      408 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/logger.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2055 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/raya_interface.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      257 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/standalone_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya/tools/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.0.dev0/src/raya/tools/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      399 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/tools/filesystem.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      984 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/tools/fsm.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      294 2023-06-08 01:58:13.000000 raya-3.5.0.dev0/src/raya/tools/image.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-08 01:58:14.436130 raya-3.5.0.dev0/src/raya.egg-info/
+-rw-rw-r--   0 prod      (1001) prod      (1001)      568 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya.egg-info/PKG-INFO
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2656 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya.egg-info/SOURCES.txt
+-rw-rw-r--   0 prod      (1001) prod      (1001)        1 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya.egg-info/dependency_links.txt
+-rw-rw-r--   0 prod      (1001) prod      (1001)        5 2023-06-08 01:58:14.000000 raya-3.5.0.dev0/src/raya.egg-info/top_level.txt
```

### Comparing `raya-3.4.3.dev0/PKG-INFO` & `raya-3.5.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raya
-Version: 3.4.3.dev0
+Version: 3.5.0.dev0
 Summary: Unlimited Robotics - Ra-Ya Python Library
 Home-page: https://documentation.unlimited-robotics.com/
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: UNKNOWN
```

### Comparing `raya-3.4.3.dev0/setup.py` & `raya-3.5.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya/application_base.py` & `raya-3.5.0.dev0/src/raya/application_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya/constants.py` & `raya-3.5.0.dev0/src/raya/constants.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya/controllers/arms_controller.py` & `raya-3.5.0.dev0/src/raya/controllers/arms_controller.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,169 +1,317 @@
 from rclpy.node import Node
 import typing
 from raya.controllers.base_controller import BaseController
+from raya.logger import DEPRECATION_NEW_METHOD
 from raya.enumerations import ANG_UNIT, MANAGE_ACTIONS
 
 
 class ArmsController(BaseController):
 
     def __init__(self, name: str, node: Node, app, extra_info={}):
         pass
 
+    def get_arms_list(self):
+        return
+
+    @DEPRECATION_NEW_METHOD('get_arms_list')
     def get_list_of_arms(self):
+        pass
+
+    def get_groups_list(self):
         return
 
+    @DEPRECATION_NEW_METHOD('get_groups_list')
     def get_list_of_groups(self):
-        return
+        pass
 
-    def get_state_of_arm(self, arm: str):
+    def get_joints_list(self, arm: str):
         return
 
+    @DEPRECATION_NEW_METHOD('get_joints_list')
     def get_list_of_joints(self, arm: str):
+        pass
+
+    def get_joint_type(self, arm: str, joint: str):
+        pass
+
+    async def get_predefined_poses_list(self, arm: str):
         return
 
-    def get_limits_of_joints(self, arm: str, units: ANG_UNIT = ANG_UNIT.DEG):
+    @DEPRECATION_NEW_METHOD('get_predefined_poses_list')
+    async def get_list_predefined_poses(self, arm: str):
+        pass
+
+    async def get_predefined_trajectories_list(self):
         return
 
-    async def is_any_arm_in_execution(self):
+    @DEPRECATION_NEW_METHOD('get_predefined_trajectories_list')
+    async def get_list_predefined_trajectories(self):
+        pass
+
+    def get_joints_limits(self, arm: str, units: ANG_UNIT = ANG_UNIT.DEG):
         return
 
-    def are_checkings_in_progress(self):
+    @DEPRECATION_NEW_METHOD('get_joints_limits')
+    def get_limits_of_joints(self, arm: str, units: ANG_UNIT = ANG_UNIT.DEG):
+        pass
+
+    def get_arm_state(self, arm: str):
         return
 
-    async def cancel_execution(self):
+    @DEPRECATION_NEW_METHOD('get_arm_state')
+    def get_state_of_arm(self, arm: str):
         pass
 
-    async def gripper_cmd(self,
-                          arm: str,
-                          desired_position: float,
-                          desired_pressure: float = 0.8,
-                          timeout: float = 10.0,
-                          callback_finish: typing.Callable = None,
-                          callback_finish_async: typing.Callable = None,
-                          callback_feedback: typing.Callable = None,
-                          callback_feedback_async: typing.Callable = None,
-                          wait: bool = False):
+    async def get_current_joints_position(self,
+                                          arm: str,
+                                          units: ANG_UNIT = ANG_UNIT.DEG,
+                                          as_dict: bool = False):
+        pass
+
+    @DEPRECATION_NEW_METHOD('get_current_joints_position')
+    async def get_current_joint_values(self,
+                                       arm: str,
+                                       units: ANG_UNIT = ANG_UNIT.DEG,
+                                       as_dict: bool = False):
+        pass
+
+    async def get_current_joint_position(self,
+                                         arm: str,
+                                         joint: str,
+                                         units: ANG_UNIT = ANG_UNIT.DEG):
         return
 
-    async def execute_joint_values_array(
+    async def get_current_pose(self, arm: str, units: ANG_UNIT = ANG_UNIT.DEG):
+        return
+
+    async def is_pose_valid(self,
+                            arm: str,
+                            x: float,
+                            y: float,
+                            z: float,
+                            roll: float,
+                            pitch: float,
+                            yaw: float,
+                            start_x: float = 0.0,
+                            start_y: float = 0.0,
+                            start_z: float = 0.0,
+                            start_roll: float = 0.0,
+                            start_pitch: float = 0.0,
+                            start_yaw: float = 0.0,
+                            start_joints: list = [],
+                            name_start_joints: list = [],
+                            use_start_pose: bool = False,
+                            use_start_joints: bool = False,
+                            cartesian_path: bool = False,
+                            tilt_constraint: bool = False,
+                            units: ANG_UNIT = ANG_UNIT.DEG,
+                            use_obstacles: bool = False,
+                            cameras: list = [],
+                            update_obstacles: bool = False,
+                            min_bbox_clear_obstacles: list = [],
+                            max_bbox_clear_obstacles: list = [],
+                            save_trajectory: bool = False,
+                            name_trajectory: str = '',
+                            velocity_scaling: float = 0.0,
+                            acceleration_scaling: float = 0.0,
+                            callback_finish: typing.Callable = None,
+                            callback_finish_async: typing.Callable = None,
+                            wait: bool = False):
+        return
+
+    async def is_pose_valid_q(self,
+                              arm: str,
+                              x: float,
+                              y: float,
+                              z: float,
+                              qx: float,
+                              qy: float,
+                              qz: float,
+                              qw: float,
+                              start_x: float = 0.0,
+                              start_y: float = 0.0,
+                              start_z: float = 0.0,
+                              start_qx: float = 0.0,
+                              start_qy: float = 0.0,
+                              start_qz: float = 0.0,
+                              start_qw: float = 0.0,
+                              start_joints: list = [],
+                              name_start_joints: list = [],
+                              use_start_pose: bool = False,
+                              use_start_joints: bool = False,
+                              units: ANG_UNIT = ANG_UNIT.DEG,
+                              cartesian_path: bool = False,
+                              tilt_constraint: bool = False,
+                              use_obstacles: bool = False,
+                              cameras: list = [],
+                              update_obstacles: bool = False,
+                              min_bbox_clear_obstacles: list = [],
+                              max_bbox_clear_obstacles: list = [],
+                              save_trajectory: bool = False,
+                              name_trajectory: str = '',
+                              velocity_scaling: float = 0.0,
+                              acceleration_scaling: float = 0.0,
+                              wait: bool = False,
+                              callback_finish: typing.Callable = None,
+                              callback_finish_async: typing.Callable = None):
+        return
+
+    def is_rotational_joint(self, arm: str, joint: str):
+        return
+
+    def is_linear_joint(self, arm: str, joint: str):
+        return
+
+    async def is_joints_position_valid(
             self,
             arm: str,
-            joint_values: list,
+            name_joints: list,
+            angle_joints: list,
             units: ANG_UNIT = ANG_UNIT.DEG,
+            start_joints: list = [],
+            name_start_joints: list = [],
+            use_start_joints: bool = False,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
+            min_bbox_clear_obstacles: list = [],
+            max_bbox_clear_obstacles: list = [],
             save_trajectory: bool = False,
             name_trajectory: str = '',
             velocity_scaling: float = 0.0,
             acceleration_scaling: float = 0.0,
-            min_bbox_clear_obstacles: list = [],
-            max_bbox_clear_obstacles: list = [],
-            callback_feedback: typing.Callable = None,
-            callback_feedback_async: typing.Callable = None,
             callback_finish: typing.Callable = None,
             callback_finish_async: typing.Callable = None,
-            wait=False):
+            wait: bool = False):
         return
 
-    async def execute_pose_array(
+    @DEPRECATION_NEW_METHOD('is_joints_position_valid')
+    async def are_joints_position_valid(
             self,
             arm: str,
-            poses: list,
+            name_joints: list,
+            angle_joints: list,
             units: ANG_UNIT = ANG_UNIT.DEG,
-            cartesian_path: bool = False,
+            start_joints: list = [],
+            name_start_joints: list = [],
+            use_start_joints: bool = False,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
+            min_bbox_clear_obstacles: list = [],
+            max_bbox_clear_obstacles: list = [],
             save_trajectory: bool = False,
             name_trajectory: str = '',
             velocity_scaling: float = 0.0,
             acceleration_scaling: float = 0.0,
-            min_bbox_clear_obstacles: list = [],
-            max_bbox_clear_obstacles: list = [],
-            callback_feedback: typing.Callable = None,
-            callback_feedback_async: typing.Callable = None,
             callback_finish: typing.Callable = None,
             callback_finish_async: typing.Callable = None,
-            wait=False):
+            wait: bool = False):
         pass
 
-    async def execute_pose_array_q(
+    async def is_any_arm_in_execution(self):
+        return
+
+    def are_checkings_in_progress(self):
+        return
+
+    async def manage_predefined_pose(
             self,
             arm: str,
-            poses: list,
-            cartesian_path: bool = False,
+            name: str,
+            position: list = [],
+            action: MANAGE_ACTIONS = MANAGE_ACTIONS.CREATE,
+            units: ANG_UNIT = ANG_UNIT.DEG):
+        pass
+
+    async def manage_predefined_trajectory(
+            self,
+            name: str,
+            action: MANAGE_ACTIONS = MANAGE_ACTIONS.GET_INFORMATION):
+        pass
+
+    async def set_predefined_pose(
+            self,
+            arm: str,
+            predefined_pose: str,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
             min_bbox_clear_obstacles: list = [],
             max_bbox_clear_obstacles: list = [],
             save_trajectory: bool = False,
             name_trajectory: str = '',
             velocity_scaling: float = 0.0,
             acceleration_scaling: float = 0.0,
             callback_feedback: typing.Callable = None,
             callback_feedback_async: typing.Callable = None,
             callback_finish: typing.Callable = None,
             callback_finish_async: typing.Callable = None,
-            wait=False):
+            wait: bool = False):
         return
 
-    async def execute_predefined_pose_array(
+    async def set_joints_position(
             self,
             arm: str,
-            predefined_poses: list,
+            name_joints: list,
+            angle_joints: list,
+            units: ANG_UNIT = ANG_UNIT.DEG,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
             min_bbox_clear_obstacles: list = [],
             max_bbox_clear_obstacles: list = [],
             save_trajectory: bool = False,
             name_trajectory: str = '',
             velocity_scaling: float = 0.0,
             acceleration_scaling: float = 0.0,
             callback_feedback: typing.Callable = None,
             callback_feedback_async: typing.Callable = None,
             callback_finish: typing.Callable = None,
             callback_finish_async: typing.Callable = None,
-            wait=False):
+            wait: bool = False):
         return
 
-    async def execute_predefined_trajectory(
+    async def set_joint_position(
             self,
-            predefined_trajectory: str,
-            reverse_execution: bool = False,
+            arm: str,
+            joint: list,
+            position: list,
+            units: ANG_UNIT = ANG_UNIT.DEG,
+            tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
             min_bbox_clear_obstacles: list = [],
             max_bbox_clear_obstacles: list = [],
-            additional_options: dict = {},
+            save_trajectory: bool = False,
+            name_trajectory: str = '',
             velocity_scaling: float = 0.0,
             acceleration_scaling: float = 0.0,
-            wait: bool = False,
             callback_feedback: typing.Callable = None,
             callback_feedback_async: typing.Callable = None,
             callback_finish: typing.Callable = None,
-            callback_finish_async: typing.Callable = None):
+            callback_finish_async: typing.Callable = None,
+            wait: bool = False):
         return
 
     async def set_pose(self,
                        arm: str,
-                       x: float,
-                       y: float,
-                       z: float,
-                       roll: float,
-                       pitch: float,
-                       yaw: float,
+                       x: float = None,
+                       y: float = None,
+                       z: float = None,
+                       roll: float = None,
+                       pitch: float = None,
+                       yaw: float = None,
+                       pose_dict: dict = None,
                        units: ANG_UNIT = ANG_UNIT.DEG,
                        cartesian_path: bool = False,
                        tilt_constraint: bool = False,
                        use_obstacles: bool = False,
                        cameras: list = [],
                        update_obstacles: bool = False,
                        min_bbox_clear_obstacles: list = [],
@@ -202,237 +350,307 @@
                          callback_feedback: typing.Callable = None,
                          callback_feedback_async: typing.Callable = None,
                          callback_finish: typing.Callable = None,
                          callback_finish_async: typing.Callable = None,
                          wait: bool = False):
         return
 
-    async def set_multi_arms_pose(
+    async def execute_predefined_trajectory(
             self,
-            group: str,
-            arms: list,
-            goal_poses: list,
-            cartesian_path: bool = False,
+            predefined_trajectory: str,
+            reverse_execution: bool = False,
+            use_obstacles: bool = False,
+            cameras: list = [],
+            update_obstacles: bool = False,
+            min_bbox_clear_obstacles: list = [],
+            max_bbox_clear_obstacles: list = [],
+            additional_options: dict = {},
+            velocity_scaling: float = 0.0,
+            acceleration_scaling: float = 0.0,
+            wait: bool = False,
+            callback_feedback: typing.Callable = None,
+            callback_feedback_async: typing.Callable = None,
+            callback_finish: typing.Callable = None,
+            callback_finish_async: typing.Callable = None):
+        return
+
+    async def execute_predefined_poses_array(
+            self,
+            arm: str,
+            predefined_poses: list,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
             min_bbox_clear_obstacles: list = [],
             max_bbox_clear_obstacles: list = [],
             save_trajectory: bool = False,
             name_trajectory: str = '',
             velocity_scaling: float = 0.0,
             acceleration_scaling: float = 0.0,
-            units: ANG_UNIT = ANG_UNIT.DEG,
             callback_feedback: typing.Callable = None,
             callback_feedback_async: typing.Callable = None,
             callback_finish: typing.Callable = None,
             callback_finish_async: typing.Callable = None,
-            wait: bool = False):
+            wait=False):
         return
 
-    async def set_predefined_pose(
+    @DEPRECATION_NEW_METHOD('execute_predefined_poses_array')
+    async def execute_predefined_pose_array(
             self,
             arm: str,
-            predefined_pose: str,
+            predefined_poses: list,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
             min_bbox_clear_obstacles: list = [],
             max_bbox_clear_obstacles: list = [],
             save_trajectory: bool = False,
             name_trajectory: str = '',
             velocity_scaling: float = 0.0,
             acceleration_scaling: float = 0.0,
             callback_feedback: typing.Callable = None,
             callback_feedback_async: typing.Callable = None,
             callback_finish: typing.Callable = None,
             callback_finish_async: typing.Callable = None,
-            wait: bool = False):
-        return
+            wait=False):
+        pass
 
-    async def set_joints_position(
+    async def execute_joints_positions_array(
             self,
             arm: str,
-            name_joints: list,
-            angle_joints: list,
+            joint_values: list,
             units: ANG_UNIT = ANG_UNIT.DEG,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
-            min_bbox_clear_obstacles: list = [],
-            max_bbox_clear_obstacles: list = [],
             save_trajectory: bool = False,
             name_trajectory: str = '',
             velocity_scaling: float = 0.0,
             acceleration_scaling: float = 0.0,
+            min_bbox_clear_obstacles: list = [],
+            max_bbox_clear_obstacles: list = [],
             callback_feedback: typing.Callable = None,
             callback_feedback_async: typing.Callable = None,
             callback_finish: typing.Callable = None,
             callback_finish_async: typing.Callable = None,
-            wait: bool = False):
+            wait=False):
         return
 
-    def convert_orientation(self,
-                            orientation: dict,
-                            units: ANG_UNIT = ANG_UNIT.DEG):
-        pass
-
-    async def add_collision_object(self,
-                                   id: str,
-                                   types: list,
-                                   dimensions: list,
-                                   shapes_poses: list,
-                                   units: ANG_UNIT = ANG_UNIT.DEG):
-        pass
-
-    async def add_constraints(self,
-                              arm: str,
-                              joint_constraints: list = [],
-                              orientation_constraints: list = [],
-                              position_constraints: list = [],
-                              units: ANG_UNIT = ANG_UNIT.DEG):
-        pass
-
-    async def remove_collision_object(self,
-                                      id: str = '',
-                                      remove_all_objects: bool = True):
-        pass
-
-    async def remove_constraints(self, arm: str = ''):
-        pass
-
-    async def add_attached_object(self, arm: str, id: str, types: list,
-                                  dimensions: list, shapes_poses: list):
+    @DEPRECATION_NEW_METHOD('execute_joints_positions_array')
+    async def execute_joint_values_array(
+            self,
+            arm: str,
+            joint_values: list,
+            units: ANG_UNIT = ANG_UNIT.DEG,
+            tilt_constraint: bool = False,
+            use_obstacles: bool = False,
+            cameras: list = [],
+            update_obstacles: bool = False,
+            save_trajectory: bool = False,
+            name_trajectory: str = '',
+            velocity_scaling: float = 0.0,
+            acceleration_scaling: float = 0.0,
+            min_bbox_clear_obstacles: list = [],
+            max_bbox_clear_obstacles: list = [],
+            callback_feedback: typing.Callable = None,
+            callback_feedback_async: typing.Callable = None,
+            callback_finish: typing.Callable = None,
+            callback_finish_async: typing.Callable = None,
+            wait=False):
         pass
 
-    async def remove_attached_object(self,
-                                     id: str = '',
-                                     remove_all_objects: bool = True):
+    async def execute_poses_array(
+            self,
+            arm: str,
+            poses: list,
+            units: ANG_UNIT = ANG_UNIT.DEG,
+            cartesian_path: bool = False,
+            tilt_constraint: bool = False,
+            use_obstacles: bool = False,
+            cameras: list = [],
+            update_obstacles: bool = False,
+            save_trajectory: bool = False,
+            name_trajectory: str = '',
+            velocity_scaling: float = 0.0,
+            acceleration_scaling: float = 0.0,
+            min_bbox_clear_obstacles: list = [],
+            max_bbox_clear_obstacles: list = [],
+            callback_feedback: typing.Callable = None,
+            callback_feedback_async: typing.Callable = None,
+            callback_finish: typing.Callable = None,
+            callback_finish_async: typing.Callable = None,
+            wait=False):
         pass
 
-    async def manage_predefined_pose(
+    @DEPRECATION_NEW_METHOD('execute_poses_array')
+    async def execute_pose_array(
             self,
             arm: str,
-            name: str,
-            position: list = [],
-            action: MANAGE_ACTIONS = MANAGE_ACTIONS.CREATE,
-            units: ANG_UNIT = ANG_UNIT.DEG):
+            poses: list,
+            units: ANG_UNIT = ANG_UNIT.DEG,
+            cartesian_path: bool = False,
+            tilt_constraint: bool = False,
+            use_obstacles: bool = False,
+            cameras: list = [],
+            update_obstacles: bool = False,
+            save_trajectory: bool = False,
+            name_trajectory: str = '',
+            velocity_scaling: float = 0.0,
+            acceleration_scaling: float = 0.0,
+            min_bbox_clear_obstacles: list = [],
+            max_bbox_clear_obstacles: list = [],
+            callback_feedback: typing.Callable = None,
+            callback_feedback_async: typing.Callable = None,
+            callback_finish: typing.Callable = None,
+            callback_finish_async: typing.Callable = None,
+            wait=False):
         pass
 
-    async def get_current_pose(self, arm: str, units: ANG_UNIT = ANG_UNIT.DEG):
-        return
-
-    async def get_current_joint_values(self,
-                                       arm: str,
-                                       units: ANG_UNIT = ANG_UNIT.DEG):
-        return
-
-    async def get_list_predefined_poses(self, arm: str):
-        return
-
-    async def get_list_predefined_trajectories(self):
+    async def execute_poses_array_q(
+            self,
+            arm: str,
+            poses: list,
+            cartesian_path: bool = False,
+            tilt_constraint: bool = False,
+            use_obstacles: bool = False,
+            cameras: list = [],
+            update_obstacles: bool = False,
+            min_bbox_clear_obstacles: list = [],
+            max_bbox_clear_obstacles: list = [],
+            save_trajectory: bool = False,
+            name_trajectory: str = '',
+            velocity_scaling: float = 0.0,
+            acceleration_scaling: float = 0.0,
+            callback_feedback: typing.Callable = None,
+            callback_feedback_async: typing.Callable = None,
+            callback_finish: typing.Callable = None,
+            callback_finish_async: typing.Callable = None,
+            wait=False):
         return
 
-    async def manage_predefined_trajectory(
+    @DEPRECATION_NEW_METHOD('execute_poses_array_q')
+    async def execute_pose_array_q(
             self,
-            name: str,
-            action: MANAGE_ACTIONS = MANAGE_ACTIONS.GET_INFORMATION):
+            arm: str,
+            poses: list,
+            cartesian_path: bool = False,
+            tilt_constraint: bool = False,
+            use_obstacles: bool = False,
+            cameras: list = [],
+            update_obstacles: bool = False,
+            min_bbox_clear_obstacles: list = [],
+            max_bbox_clear_obstacles: list = [],
+            save_trajectory: bool = False,
+            name_trajectory: str = '',
+            velocity_scaling: float = 0.0,
+            acceleration_scaling: float = 0.0,
+            callback_feedback: typing.Callable = None,
+            callback_feedback_async: typing.Callable = None,
+            callback_finish: typing.Callable = None,
+            callback_finish_async: typing.Callable = None,
+            wait=False):
         pass
 
-    async def is_pose_valid(self,
-                            arm: str,
-                            x: float,
-                            y: float,
-                            z: float,
-                            roll: float,
-                            pitch: float,
-                            yaw: float,
-                            start_x: float = 0.0,
-                            start_y: float = 0.0,
-                            start_z: float = 0.0,
-                            start_roll: float = 0.0,
-                            start_pitch: float = 0.0,
-                            start_yaw: float = 0.0,
-                            start_joints: list = [],
-                            name_start_joints: list = [],
-                            use_start_pose: bool = False,
-                            use_start_joints: bool = False,
-                            cartesian_path: bool = False,
-                            tilt_constraint: bool = False,
-                            units: ANG_UNIT = ANG_UNIT.DEG,
-                            use_obstacles: bool = False,
-                            cameras: list = [],
-                            update_obstacles: bool = False,
-                            min_bbox_clear_obstacles: list = [],
-                            max_bbox_clear_obstacles: list = [],
-                            save_trajectory: bool = False,
-                            name_trajectory: str = '',
-                            velocity_scaling: float = 0.0,
-                            acceleration_scaling: float = 0.0,
-                            callback_finish: typing.Callable = None,
-                            callback_finish_async: typing.Callable = None,
-                            wait: bool = False):
-        return
-
-    async def is_pose_valid_q(self,
-                              arm: str,
-                              x: float,
-                              y: float,
-                              z: float,
-                              qx: float,
-                              qy: float,
-                              qz: float,
-                              qw: float,
-                              start_x: float = 0.0,
-                              start_y: float = 0.0,
-                              start_z: float = 0.0,
-                              start_qx: float = 0.0,
-                              start_qy: float = 0.0,
-                              start_qz: float = 0.0,
-                              start_qw: float = 0.0,
-                              start_joints: list = [],
-                              name_start_joints: list = [],
-                              use_start_pose: bool = False,
-                              use_start_joints: bool = False,
-                              units: ANG_UNIT = ANG_UNIT.DEG,
-                              cartesian_path: bool = False,
-                              tilt_constraint: bool = False,
-                              use_obstacles: bool = False,
-                              cameras: list = [],
-                              update_obstacles: bool = False,
-                              min_bbox_clear_obstacles: list = [],
-                              max_bbox_clear_obstacles: list = [],
-                              save_trajectory: bool = False,
-                              name_trajectory: str = '',
-                              velocity_scaling: float = 0.0,
-                              acceleration_scaling: float = 0.0,
-                              wait: bool = False,
-                              callback_finish: typing.Callable = None,
-                              callback_finish_async: typing.Callable = None):
+    async def set_multi_arm_pose(
+            self,
+            group: str,
+            arms: list,
+            goal_poses: list,
+            cartesian_path: bool = False,
+            tilt_constraint: bool = False,
+            use_obstacles: bool = False,
+            cameras: list = [],
+            update_obstacles: bool = False,
+            min_bbox_clear_obstacles: list = [],
+            max_bbox_clear_obstacles: list = [],
+            save_trajectory: bool = False,
+            name_trajectory: str = '',
+            velocity_scaling: float = 0.0,
+            acceleration_scaling: float = 0.0,
+            units: ANG_UNIT = ANG_UNIT.DEG,
+            callback_feedback: typing.Callable = None,
+            callback_feedback_async: typing.Callable = None,
+            callback_finish: typing.Callable = None,
+            callback_finish_async: typing.Callable = None,
+            wait: bool = False):
         return
 
-    async def are_joints_position_valid(
+    @DEPRECATION_NEW_METHOD('set_multi_arm_pose')
+    async def set_multi_arms_pose(
             self,
-            arm: str,
-            name_joints: list,
-            angle_joints: list,
-            units: ANG_UNIT = ANG_UNIT.DEG,
-            start_joints: list = [],
-            name_start_joints: list = [],
-            use_start_joints: bool = False,
+            group: str,
+            arms: list,
+            goal_poses: list,
+            cartesian_path: bool = False,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
             min_bbox_clear_obstacles: list = [],
             max_bbox_clear_obstacles: list = [],
             save_trajectory: bool = False,
             name_trajectory: str = '',
             velocity_scaling: float = 0.0,
             acceleration_scaling: float = 0.0,
+            units: ANG_UNIT = ANG_UNIT.DEG,
+            callback_feedback: typing.Callable = None,
+            callback_feedback_async: typing.Callable = None,
             callback_finish: typing.Callable = None,
             callback_finish_async: typing.Callable = None,
             wait: bool = False):
+        pass
+
+    async def gripper_cmd(self,
+                          arm: str,
+                          desired_position: float,
+                          desired_pressure: float = 0.8,
+                          timeout: float = 10.0,
+                          callback_finish: typing.Callable = None,
+                          callback_finish_async: typing.Callable = None,
+                          callback_feedback: typing.Callable = None,
+                          callback_feedback_async: typing.Callable = None,
+                          wait: bool = False):
         return
+
+    async def cancel_execution(self):
+        pass
+
+    async def add_attached_object(self, arm: str, id: str, types: list,
+                                  dimensions: list, shapes_poses: list):
+        pass
+
+    async def remove_attached_object(self,
+                                     id: str = '',
+                                     remove_all_objects: bool = True):
+        pass
+
+    async def add_collision_object(self,
+                                   id: str,
+                                   types: list,
+                                   dimensions: list,
+                                   shapes_poses: list,
+                                   units: ANG_UNIT = ANG_UNIT.DEG):
+        pass
+
+    async def remove_collision_object(self,
+                                      id: str = '',
+                                      remove_all_objects: bool = True):
+        pass
+
+    async def add_constraints(self,
+                              arm: str,
+                              joint_constraints: list = [],
+                              orientation_constraints: list = [],
+                              position_constraints: list = [],
+                              units: ANG_UNIT = ANG_UNIT.DEG):
+        pass
+
+    async def remove_constraints(self, arm: str = ''):
+        pass
+
+    def convert_orientation(self,
+                            orientation: dict,
+                            units: ANG_UNIT = ANG_UNIT.DEG):
+        pass
```

### Comparing `raya-3.4.3.dev0/src/raya/controllers/cameras_controller.py` & `raya-3.5.0.dev0/src/raya/controllers/cameras_controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 
 class CamerasController(BaseController):
 
     def __init__(self, name: str, node: Node, app, extra_info: dict):
         pass
 
+    def is_camera_enabled(self, camera_name: str):
+        return
+
     def available_color_cameras(self):
         return
 
     async def enable_color_camera(self, camera_name: str):
         pass
 
     async def disable_color_camera(self, camera_name: str):
```

### Comparing `raya-3.4.3.dev0/src/raya/controllers/cv_controller.py` & `raya-3.5.0.dev0/src/raya/controllers/cv_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from rclpy.node import Node
 from raya.controllers.base_controller import BaseController
-from raya.handlers.cv.model_base import CVModelBase
-from raya.handlers.cv.objects_detector_handler import ObjectsDetectorHandler
-from raya.handlers.cv.tags_detector_handler import TagsDetectorHandler
-from raya.handlers.cv.faces_detector_handler import FacesDetectorHandler
-from raya.handlers.cv.faces_recognizer_handler import FacesRecognizerHandler
-from raya.handlers.cv.hand_estimator_handler import HandEstimatorHandler
-from raya.handlers.cv.objects_classifier_handler import ObjectsClassifierHandler
-from raya.handlers.cv.objects_segmentator_handler import ObjectsSegmentatorHandler
-from raya.handlers.cv.planes_segmentator_handler import PlanesSegmentatorHandler
+from raya.handlers.cv.model_handler import ModelHandler
+from raya.handlers.cv.detectors.objects_detector_handler import ObjectsDetectorHandler
+from raya.handlers.cv.detectors.tags_detector_handler import TagsDetectorHandler
+from raya.handlers.cv.detectors.faces_detector_handler import FacesDetectorHandler
+from raya.handlers.cv.recognizers.faces_recognizer_handler import FacesRecognizerHandler
+from raya.handlers.cv.estimators.hand_estimator_handler import HandEstimatorHandler
+from raya.handlers.cv.classifiers.objects_classifier_handler import ObjectsClassifierHandler
+from raya.handlers.cv.segmentators.objects_segmentator_handler import ObjectsSegmentatorHandler
+from raya.handlers.cv.segmentators.planes_segmentator_handler import PlanesSegmentatorHandler
 
 HANDLERS_CLASSES = {
     'detector': {
         'object': ObjectsDetectorHandler,
         'tag': TagsDetectorHandler,
         'face': FacesDetectorHandler
     },
@@ -49,15 +49,15 @@
                            continues_msg: bool = True,
                            model_params: dict = {}):
         return
 
     async def disable_model(self,
                             model: str = None,
                             type: str = None,
-                            model_obj: CVModelBase = None):
+                            model_obj: ModelHandler = None):
         pass
 
     async def disable_all_models(self):
         return
 
     async def train_model_folder_path(self,
                                       model_name: str,
```

### Comparing `raya-3.4.3.dev0/src/raya/controllers/fleet_controller.py` & `raya-3.5.0.dev0/src/raya/controllers/fleet_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya/controllers/grasping_controller.py` & `raya-3.5.0.dev0/src/raya/controllers/grasping_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya/controllers/interactions_controller.py` & `raya-3.5.0.dev0/src/raya/controllers/interactions_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya/controllers/leds_controller.py` & `raya-3.5.0.dev0/src/raya/controllers/leds_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya/controllers/lidar_controller.py` & `raya-3.5.0.dev0/src/raya/controllers/lidar_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya/controllers/manipulation_controller.py` & `raya-3.5.0.dev0/src/raya/controllers/manipulation_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya/controllers/motion_controller.py` & `raya-3.5.0.dev0/src/raya/controllers/motion_controller.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,26 +5,35 @@
 
 
 class MotionController(BaseController):
 
     def __init__(self, name: str, node: Node, app, extra_info={}):
         pass
 
+    async def update_set_velocity(self,
+                                  x_velocity: float,
+                                  y_velocity: float,
+                                  angular_velocity: float,
+                                  duration: float,
+                                  enable_obstacles: bool = True):
+        return
+
     async def set_velocity(self,
                            x_velocity: float,
                            y_velocity: float,
                            angular_velocity: float,
                            duration: float,
+                           enable_obstacles: bool = True,
                            ang_unit: ANG_UNIT = ANG_UNIT.DEG,
                            callback_feedback: typing.Callable = None,
                            callback_feedback_async: typing.Callable = None,
                            callback_finish: typing.Callable = None,
                            callback_finish_async: typing.Callable = None,
                            wait: bool = False):
-        return
+        pass
 
     async def move_linear(self,
                           distance: float,
                           x_velocity: float,
                           y_velocity: float = 0.0,
                           callback_feedback: typing.Callable = None,
                           callback_feedback_async: typing.Callable = None,
```

### Comparing `raya-3.4.3.dev0/src/raya/controllers/navigation_controller.py` & `raya-3.5.0.dev0/src/raya/controllers/navigation_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya/controllers/sensors_controller.py` & `raya-3.5.0.dev0/src/raya/controllers/sensors_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya/controllers/skills_controller.py` & `raya-3.5.0.dev0/src/raya/controllers/skills_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya/controllers/sound_controller.py` & `raya-3.5.0.dev0/src/raya/controllers/sound_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya/controllers/ui_controller.py` & `raya-3.5.0.dev0/src/raya/controllers/ui_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya/enumerations.py` & `raya-3.5.0.dev0/src/raya/enumerations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,27 @@
 from enum import IntEnum, Enum
 
 
-class INPUT_TYPE(Enum):
-    '\n    Enumeration to set input type\n    INPUT_TYPE.TEXT: user can only input a-z or A-Z\n    INPUT_TYPE.NUMERIC: user can only input numbers\n    '
-    TEXT = 'text'
-    NUMERIC = 'numeric'
-
-
-class THEME_TYPE(Enum):
-    '\n    Enumeration to set the UI theme type\n    THEME_TYPE.DARK : will specify to set background to dark\n    THEME_TYPE.WHITE : will specify to set background to white\n    '
-    DARK = 'DARK'
-    WHITE = 'WHITE'
-
-
-class MODAL_TYPE(Enum):
-    '\n    Enumeration to set the UI modal type\n    UI_TYPES.INFO : specify that this is an informative componant, No callback\n    UI_TYPES.SUCCESS : showing a messege that the opration was seccessful\n    UI_TYPES.ERROR : showing a messege that will alert of a bad precedere\n    '
-    INFO = 'info'
-    SUCCESS = 'success'
-    ERROR = 'error'
-
-
 class POS_UNIT(IntEnum):
     '\n    Enumeration to set the unit of the coordinates in a map.\n    POS_UNIT.PIXEL : Based on the pixel of the image map.\n    POS_UNIT.METERS : Meters\n    '
     PIXEL = 0
     METERS = 1
 
 
 class ANG_UNIT(IntEnum):
     '\n    Enumeration to set the angles unit.\n    ANG_UNIT.DEG : Degrees\n    ANG_UNIT.RAD : Radians\n    '
     DEG = 0
     RAD = 1
 
 
-class TITLE_SIZE(Enum):
-    '\n    Enumeration to set the title size.\n    TITLE_SIZE.SMALL : Small size\n    TITLE_SIZE.MEDIUM : Medium size\n    TITLE_SIZE.LARGE : Large size\n    '
-    SMALL = 'small'
-    MEDIUM = 'medium'
-    LARGE = 'large'
+class JOINT_TYPE(IntEnum):
+    '\n    Enumeration to define the type of arm joint\n    JOINT_TYPE.ROTATIONAL\n    JOINT_TYPE.LINEAR\n    '
+    NOT_DEFINED = 0
+    LINEAR = 1
+    ROTATIONAL = 2
 
 
 class TYPE_SHAPES(IntEnum):
     '\n    Enumeration to define the type of shape for obstacles.\n    TYPE_SHAPES.BOX : Box\n    TYPE_SHAPES.SPHERE : Sphere\n    TYPE_SHAPES.CYLINDER : Cylinder\n    TYPE_SHAPES.CONE : Cone\n    '
     BOX = 1
     SPHERE = 2
     CYLINDER = 3
@@ -55,14 +36,49 @@
     SPHERE_RADIUS = 0
     CYLINDER_HEIGHT = 0
     CYLINDER_RADIUS = 1
     CONE_HEIGHT = 0
     CONE_RADIUS = 1
 
 
+class MANAGE_ACTIONS(Enum):
+    '\n    Enumeration to set the action to take when the user wants to manage predefined data.\n    '
+    GET = 'get'
+    EDIT = 'edit'
+    REMOVE = 'remove'
+    GET_INFORMATION = 'get_info'
+    CREATE = 'create'
+
+
+class INPUT_TYPE(Enum):
+    '\n    Enumeration to set input type\n    INPUT_TYPE.TEXT: user can only input a-z or A-Z\n    INPUT_TYPE.NUMERIC: user can only input numbers\n    '
+    TEXT = 'text'
+    NUMERIC = 'numeric'
+
+
+class THEME_TYPE(Enum):
+    '\n    Enumeration to set the UI theme type\n    THEME_TYPE.DARK : will specify to set background to dark\n    THEME_TYPE.WHITE : will specify to set background to white\n    '
+    DARK = 'DARK'
+    WHITE = 'WHITE'
+
+
+class MODAL_TYPE(Enum):
+    '\n    Enumeration to set the UI modal type\n    UI_TYPES.INFO : specify that this is an informative componant, No callback\n    UI_TYPES.SUCCESS : showing a messege that the opration was seccessful\n    UI_TYPES.ERROR : showing a messege that will alert of a bad precedere\n    '
+    INFO = 'info'
+    SUCCESS = 'success'
+    ERROR = 'error'
+
+
+class TITLE_SIZE(Enum):
+    '\n    Enumeration to set the title size.\n    TITLE_SIZE.SMALL : Small size\n    TITLE_SIZE.MEDIUM : Medium size\n    TITLE_SIZE.LARGE : Large size\n    '
+    SMALL = 'small'
+    MEDIUM = 'medium'
+    LARGE = 'large'
+
+
 class ANIMATION_TYPE(Enum):
     '\n    ANIMATION_TYPE.LOTTIE : Lottie format\n    Enumeration to set the animation format.\n    ANIMATION_TYPE.PNG : PNG format\n    ANIMATION_TYPE.JPEG : JPEG format\n    ANIMATION_TYPE.GIF : GIF format\n    ANIMATION_TYPE.URL : URL format\n    '
     LOTTIE = 'LOTTIE'
     PNG = 'BASE64'
     JPEG = 'BASE64'
     GIF = 'BASE64'
     URL = 'URL'
@@ -71,23 +87,14 @@
 class EXECUTION_CONTROL(IntEnum):
     '\n    Enumeration to set the animation to be overriden.\n    EXECUTION_CONTROL.OVERRIDE : Overide current animation.\n    EXECUTION_CONTROL.ADD_TO_QUEUE : Insert animation to serial queue.\n    EXECUTION_CONTROL.AFTER_CURRENT : Run animation at the end of current animation.\n    '
     OVERRIDE = 0
     ADD_TO_QUEUE = 1
     AFTER_CURRENT = 2
 
 
-class MANAGE_ACTIONS(Enum):
-    '\n    Enumeration to set the action to take when the user wants to manage predefined data.\n    '
-    GET = 'get'
-    EDIT = 'edit'
-    REMOVE = 'remove'
-    GET_INFORMATION = 'get_info'
-    CREATE = 'create'
-
-
 class FINISH_STATUS(Enum):
     '\n    Enumeration to set indicate whether the app finished successfully or not.\n    FINISH_STATUS.SUCCESS : The app finished successfully.\n    FINISH_STATUS.FAILED : The app finished with errors or did not finish as expected.\n    '
     SUCCESS = 'Done'
     FAILED = 'Failed'
 
 
 class SPLIT_TYPE(Enum):
```

### Comparing `raya-3.4.3.dev0/src/raya/exceptions.py` & `raya-3.5.0.dev0/src/raya/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,26 @@
     pass
 
 
 class RayaOutsideSetup(RayaApplicationException):
     pass
 
 
+class RayaCustomCommandNotAvailable(RayaApplicationException):
+    pass
+
+
+class RayaCustomMissingRequiredParameter(RayaApplicationException):
+    pass
+
+
+class RayaCustomErrorParsingParameter(RayaApplicationException):
+    pass
+
+
 class RayaFileSystemException(RayaApplicationException):
     pass
 
 
 class RayaNotValidPath(RayaFileSystemException):
     pass
 
@@ -308,22 +320,30 @@
     pass
 
 
 class RayaCVNeedCallback(RayaCVException):
     pass
 
 
+class RayaCVNeedController(RayaCVException):
+    pass
+
+
 class RayaCVAlreadyEnabled(RayaCVException):
     pass
 
 
 class RayaCVNotCameraInterface(RayaCVException):
     pass
 
 
+class RayaCVNotCameraEnabled(RayaCVException):
+    pass
+
+
 class RayaCVTopicNotPublishig(RayaCVException):
     pass
 
 
 class RayaCVGPUNotAvailable(RayaCVException):
     pass
 
@@ -468,14 +488,34 @@
     pass
 
 
 class RayaNotValidMotionCommand(RayaMotionException):
     pass
 
 
+class RayaObstacleDetected(RayaMotionException):
+    pass
+
+
+class RayaInvalidMinDistance(RayaMotionException):
+    pass
+
+
+class RayaMotionTimeout(RayaMotionException):
+    pass
+
+
+class RayaRobotNotMoving(RayaMotionException):
+    pass
+
+
+class RayaUnableToEnableCamera(RayaMotionException):
+    pass
+
+
 class RayaInteractionsException(RayaControllerException):
     pass
 
 
 class RayaInteractionsAlreadyRunning(RayaInteractionsException):
     pass
 
@@ -708,14 +748,18 @@
     pass
 
 
 class RayaNavMappingDisabled(RayaNavException):
     pass
 
 
+class RayaNavUnableToEnableCamera(RayaNavException):
+    pass
+
+
 class RayaNavFileNotFound(RayaNavException):
     pass
 
 
 class RayaNavWrongFileFormat(RayaNavException):
     pass
 
@@ -764,14 +808,22 @@
     pass
 
 
 class RayaArmsInvalidGroupName(RayaArmsException):
     pass
 
 
+class RayaArmsInvalidArmOrGroupName(RayaArmsException):
+    pass
+
+
+class RayaArmsInvalidJointName(RayaArmsException):
+    pass
+
+
 class RayaArmsNotPoseArmDataAvailable(RayaArmsException):
     pass
 
 
 class RayaArmsNotPredefinedPoseAvailable(RayaArmsException):
     pass
 
@@ -804,14 +856,18 @@
     pass
 
 
 class RayaArmsErrorParsingPredefinedTrajectory(RayaArmsException):
     pass
 
 
+class RayaArmsInvalidCustomCommand(RayaArmsException):
+    pass
+
+
 class RayaUIException(RayaException):
     pass
 
 
 class RayaUIMissingValue(RayaUIException):
     pass
```

### Comparing `raya-3.4.3.dev0/src/raya/exceptions_handler.py` & `raya-3.5.0.dev0/src/raya/exceptions_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,20 @@
     128: (RayaSoundErrorRecording, ''),
     129: (RayaSoundErrorPlayingAudio, ''),
     130: (RayaSoundBufferNotFound, '')
 }
 EXCEPTIONS_MAP_MOTION = {
     **EXCEPTIONS_MAP_GENERAL, 20: (RayaAlreadyMoving, ''),
     21: (RayaNotValidMotionCommand, ''),
-    22: (RayaNotValidMotionCommand, '')
+    22: (RayaNotValidMotionCommand, ''),
+    23: (RayaObstacleDetected, ''),
+    24: (RayaInvalidMinDistance, ''),
+    25: (RayaMotionTimeout, ''),
+    26: (RayaRobotNotMoving, ''),
+    136: (RayaUnableToEnableCamera, '')
 }
 EXCEPTIONS_MAP_NAV = {
     **EXCEPTIONS_MAP_GENERAL, 20: (RayaNavAlreadyNavigating, ''),
     22: (RayaNavNotMapping, ''),
     23: (RayaNavLocationAlreadyExist, ''),
     24: (RayaNavErrorReadingYaml, ''),
     25: (RayaNavErrorWritingYaml, ''),
@@ -84,14 +89,15 @@
     124: (RayaNavInvalidGoal, ''),
     125: (RayaUnableToFollowPath, ''),
     126: (RayaNoPathToGoal, ''),
     127: (RayaNavIncompletePath, ''),
     128: (RayaNavIncorrectPath, ''),
     129: (RayaNavBadImageSize, ''),
     130: (RayaNavMappingDisabled, ''),
+    136: (RayaNavUnableToEnableCamera, ''),
     140: (RayaNavFileNotFound, ''),
     141: (RayaNavWrongFileFormat, '')
 }
 EXCEPTIONS_MAP_CV = {
     **EXCEPTIONS_MAP_GENERAL, 20: (RayaCVAlreadyEnabled, ''),
     21: (RayaCVNotCameraInterface, ''),
     22: (RayaCVTopicNotPublishig, ''),
@@ -118,14 +124,17 @@
     25: (RayaArmsOutOfLimits, ''),
     26: (RayaArmsPredefinedPoseEmptyName, ''),
     27: (RayaArmsPredefinedPoseNameAlreadyExist, ''),
     28: (RayaArmsPredefinedPoseNameNotExist, ''),
     29: (RayaArmsPredefinedTrajectoryNameAlreadyExist, ''),
     30: (RayaArmsPredefinedTrajectoryNameNotExist, ''),
     31: (RayaArmsErrorParsingPredefinedTrajectory, ''),
+    33: (RayaArmsInvalidCustomCommand, ''),
+    38: (RayaCustomMissingRequiredParameter, ''),
+    39: (RayaCustomErrorParsingParameter, ''),
     121: (RayaArmsExternalException, ''),
     122: (RayaArmsExternalException, ''),
     123: (RayaArmsExternalException, ''),
     124: (RayaArmsExternalException, ''),
     125: (RayaArmsExternalException, ''),
     126: (RayaArmsExternalException, ''),
     127: (RayaArmsExternalException, ''),
```

### Comparing `raya-3.4.3.dev0/src/raya/handlers/cv/classifier_handler_base.py` & `raya-3.5.0.dev0/src/raya/handlers/cv/recognizers/recognizer_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import typing
 from rclpy.node import Node
-from raya.handlers.cv.model_base import CVModelBase
+from raya.handlers.cv.model_handler import ModelHandler
 
 
-class ClassifierHandlerBase(CVModelBase):
+class RecognizerHandler(ModelHandler):
 
-    def __init__(self, node: Node, topic: str, model_id: int, model_info: dict,
-                 continues_msg: bool, cli_cmd, cmd_call):
+    def __init__(self, node: Node, topic: str, source: str, model_id: int,
+                 model_info: dict, continues_msg: bool, cli_cmd, cmd_call):
         self.cli_cmd = cli_cmd
 
-    async def get_classifications_once(self,
-                                       as_dict=False,
-                                       get_timestamp=False):
+    async def get_recognitions_once(self, as_dict=False, get_timestamp=False):
         pass
 
-    def get_current_classifications(self, as_dict=False, get_timestamp=False):
+    def get_current_recognitions(self, as_dict=False, get_timestamp=False):
         pass
 
-    def set_classifications_callback(
+    def set_recognitions_callback(self,
+                                  callback: typing.Callable = None,
+                                  callback_async: typing.Callable = None,
+                                  as_dict: bool = False,
+                                  call_without_recognitions: bool = False):
+        pass
+
+    def set_img_recognitions_callback(
             self,
             callback: typing.Callable = None,
             callback_async: typing.Callable = None,
             as_dict: bool = False,
-            call_without_classifications: bool = False):
+            call_without_recognitions: bool = False,
+            cameras_controller: typing.Callable = None):
         pass
 
     def cancel_finds(self):
         pass
```

### Comparing `raya-3.4.3.dev0/src/raya/handlers/cv/estimator_handler_base.py` & `raya-3.5.0.dev0/src/raya/handlers/cv/classifiers/objects_classifier_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import typing
 from rclpy.node import Node
-from raya.handlers.cv.model_base import CVModelBase
+from raya.handlers.cv.classifiers.classifier_handler import ClassifierHandler
 
 
-class EstimatorHandlerBase(CVModelBase):
+class ObjectsClassifierHandler(ClassifierHandler):
 
-    def __init__(self, node: Node, topic: str, model_id: int, model_info: dict,
-                 continues_msg: bool, cli_cmd, cmd_call):
+    def __init__(self, node: Node, topic: str, source: str, model_id: int,
+                 model_info: dict, continues_msg: bool, cli_cmd, cmd_call):
         pass
 
-    def get_current_estimations(self, as_dict=False, get_timestamp=False):
-        pass
+    async def find_objects(self,
+                           objects: list,
+                           callback: typing.Callable = None,
+                           callback_async: typing.Callable = None,
+                           wait: bool = False,
+                           timeout: float = 0.0,
+                           as_dict: bool = False):
+        return
 
-    def set_estimations_callback(self,
-                                 callback: typing.Callable = None,
-                                 callback_async: typing.Callable = None,
-                                 as_dict: bool = False,
-                                 call_without_estimations: bool = False):
+    def cancel_find_objects(self):
         pass
 
-    def cancel_finds(self):
-        pass
+    def get_objects_names(self):
+        return
```

### Comparing `raya-3.4.3.dev0/src/raya/handlers/cv/faces_recognizer_handler.py` & `raya-3.5.0.dev0/src/raya/handlers/cv/recognizers/faces_recognizer_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import typing
 from rclpy.node import Node
-from raya.handlers.cv.recognizer_handler_base import RecognizerHandlerBase
+from raya.handlers.cv.recognizers.recognizer_handler import RecognizerHandler
 
 
-class FacesRecognizerHandler(RecognizerHandlerBase):
+class FacesRecognizerHandler(RecognizerHandler):
 
-    def __init__(self, node: Node, topic: str, model_id: int, model_info: dict,
-                 continues_msg: bool, cli_cmd, cmd_call):
+    def __init__(self, node: Node, topic: str, source: str, model_id: int,
+                 model_info: dict, continues_msg: bool, cli_cmd, cmd_call):
         pass
 
     async def find_recognition(self,
                                recognitions: list,
                                callback: typing.Callable = None,
                                callback_async: typing.Callable = None,
                                wait: bool = False,
```

### Comparing `raya-3.4.3.dev0/src/raya/handlers/cv/objects_detector_handler.py` & `raya-3.5.0.dev0/src/raya/handlers/cv/detectors/objects_detector_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import typing
 from rclpy.node import Node
-from raya.handlers.cv.detector_handler_base import DetectorHandlerBase
+from raya.handlers.cv.detectors.detector_handler import DetectorHandler
 
 
-class ObjectsDetectorHandler(DetectorHandlerBase):
+class ObjectsDetectorHandler(DetectorHandler):
 
-    def __init__(self, node: Node, topic: str, model_id: int, model_info: dict,
-                 continues_msg: bool, cli_cmd, cmd_call):
+    def __init__(self, node: Node, topic: str, source: str, model_id: int,
+                 model_info: dict, continues_msg: bool, cli_cmd, cmd_call):
         pass
 
     async def find_objects(self,
                            objects: list,
                            callback: typing.Callable = None,
                            callback_async: typing.Callable = None,
                            wait: bool = False,
```

### Comparing `raya-3.4.3.dev0/src/raya/handlers/cv/objects_segmentator_handler.py` & `raya-3.5.0.dev0/src/raya/handlers/cv/segmentators/planes_segmentator_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import typing
 from rclpy.node import Node
-from raya.handlers.cv.segmentator_handler_base import SegmentatorHandlerBase
+from raya.handlers.cv.segmentators.segmentator_handler import SegmentatorHandler
 
 
-class ObjectsSegmentatorHandler(SegmentatorHandlerBase):
+class PlanesSegmentatorHandler(SegmentatorHandler):
 
-    def __init__(self, node: Node, topic: str, model_id: int, model_info: dict,
-                 continues_msg: bool, cli_cmd, cmd_call):
+    def __init__(self, node: Node, topic: str, source: str, model_id: int,
+                 model_info: dict, continues_msg: bool, cli_cmd, cmd_call):
         pass
 
-    async def find_objects(self,
-                           objects: list,
-                           callback: typing.Callable = None,
-                           callback_async: typing.Callable = None,
-                           wait: bool = False,
-                           timeout: float = 0.0,
-                           as_dict: bool = False):
+    async def find_planes(self,
+                          planes: list,
+                          callback: typing.Callable = None,
+                          callback_async: typing.Callable = None,
+                          wait: bool = False,
+                          timeout: float = 0.0,
+                          as_dict: bool = False):
         return
 
-    def cancel_find_objects(self):
+    def cancel_find_planes(self):
         pass
 
-    def get_objects_names(self):
+    def get_planes_names(self):
         return
```

### Comparing `raya-3.4.3.dev0/src/raya/handlers/cv/planes_segmentator_handler.py` & `raya-3.5.0.dev0/src/raya/handlers/cv/detectors/tags_detector_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import typing
 from rclpy.node import Node
-from raya.handlers.cv.segmentator_handler_base import SegmentatorHandlerBase
+from raya.handlers.cv.detectors.detector_handler import DetectorHandler
 
 
-class PlanesSegmentatorHandler(SegmentatorHandlerBase):
+class TagsDetectorHandler(DetectorHandler):
 
-    def __init__(self, node: Node, topic: str, model_id: int, model_info: dict,
-                 continues_msg: bool, cli_cmd, cmd_call):
+    def __init__(self, node: Node, topic: str, source: str, model_id: int,
+                 model_info: dict, continues_msg: bool, cli_cmd, cmd_call):
         pass
 
-    async def find_planes(self,
-                          planes: list,
-                          callback: typing.Callable = None,
-                          callback_async: typing.Callable = None,
-                          wait: bool = False,
-                          timeout: float = 0.0,
-                          as_dict: bool = False):
+    async def find_tags(self,
+                        tags: dict,
+                        callback: typing.Callable = None,
+                        callback_async: typing.Callable = None,
+                        wait: bool = False,
+                        timeout: float = 0.0,
+                        as_dict: bool = False):
         return
 
-    def cancel_find_planes(self):
+    def cancel_find_tags(self):
         pass
-
-    def get_planes_names(self):
-        return
```

### Comparing `raya-3.4.3.dev0/src/raya/handlers/cv/recognizer_handler_base.py` & `raya-3.5.0.dev0/src/raya/handlers/cv/detectors/detector_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 import typing
 from rclpy.node import Node
-from raya.handlers.cv.model_base import CVModelBase
+from raya.handlers.cv.model_handler import ModelHandler
 
 
-class RecognizerHandlerBase(CVModelBase):
+class DetectorHandler(ModelHandler):
 
-    def __init__(self, node: Node, topic: str, model_id: int, model_info: dict,
-                 continues_msg: bool, cli_cmd, cmd_call):
+    def __init__(self, node: Node, topic: str, source: str, model_id: int,
+                 model_info: dict, continues_msg: bool, cli_cmd, cmd_call):
         self.cli_cmd = cli_cmd
 
-    async def get_recognitions_once(self, as_dict=False, get_timestamp=False):
+    async def get_detections_once(self, as_dict=False, get_timestamp=False):
         pass
 
-    def get_current_recognitions(self, as_dict=False, get_timestamp=False):
+    def get_current_detections(self, as_dict=False, get_timestamp=False):
         pass
 
-    def set_recognitions_callback(self,
-                                  callback: typing.Callable = None,
-                                  callback_async: typing.Callable = None,
-                                  as_dict: bool = False,
-                                  call_without_recognitions: bool = False):
+    def set_detections_callback(self,
+                                callback: typing.Callable = None,
+                                callback_async: typing.Callable = None,
+                                as_dict: bool = False,
+                                call_without_detections: bool = False):
+        pass
+
+    def set_img_detections_callback(
+            self,
+            callback: typing.Callable = None,
+            callback_async: typing.Callable = None,
+            as_dict: bool = False,
+            call_without_detections: bool = False,
+            cameras_controller: typing.Callable = None):
         pass
 
     def cancel_finds(self):
         pass
```

### Comparing `raya-3.4.3.dev0/src/raya/raya_interface.py` & `raya-3.5.0.dev0/src/raya/raya_interface.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya/tools/fsm.py` & `raya-3.5.0.dev0/src/raya/tools/fsm.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.3.dev0/src/raya.egg-info/PKG-INFO` & `raya-3.5.0.dev0/src/raya.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raya
-Version: 3.4.3.dev0
+Version: 3.5.0.dev0
 Summary: Unlimited Robotics - Ra-Ya Python Library
 Home-page: https://documentation.unlimited-robotics.com/
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: UNKNOWN
```

### Comparing `raya-3.4.3.dev0/src/raya.egg-info/SOURCES.txt` & `raya-3.5.0.dev0/src/raya.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -34,28 +34,33 @@
 src/raya/controllers/navigation_controller.py
 src/raya/controllers/sensors_controller.py
 src/raya/controllers/skills_controller.py
 src/raya/controllers/sound_controller.py
 src/raya/controllers/ui_controller.py
 src/raya/handlers/__init__.py
 src/raya/handlers/cv/__init__.py
-src/raya/handlers/cv/classifier_handler_base.py
-src/raya/handlers/cv/detector_handler_base.py
-src/raya/handlers/cv/estimator_handler_base.py
-src/raya/handlers/cv/faces_detector_handler.py
-src/raya/handlers/cv/faces_recognizer_handler.py
-src/raya/handlers/cv/hand_estimator_handler.py
-src/raya/handlers/cv/model_base.py
-src/raya/handlers/cv/objects_classifier_handler.py
-src/raya/handlers/cv/objects_detector_handler.py
-src/raya/handlers/cv/objects_segmentator_handler.py
-src/raya/handlers/cv/planes_segmentator_handler.py
-src/raya/handlers/cv/recognizer_handler_base.py
-src/raya/handlers/cv/segmentator_handler_base.py
-src/raya/handlers/cv/tags_detector_handler.py
+src/raya/handlers/cv/model_handler.py
+src/raya/handlers/cv/classifiers/__init__.py
+src/raya/handlers/cv/classifiers/classifier_handler.py
+src/raya/handlers/cv/classifiers/objects_classifier_handler.py
+src/raya/handlers/cv/detectors/__init__.py
+src/raya/handlers/cv/detectors/detector_handler.py
+src/raya/handlers/cv/detectors/faces_detector_handler.py
+src/raya/handlers/cv/detectors/objects_detector_handler.py
+src/raya/handlers/cv/detectors/tags_detector_handler.py
+src/raya/handlers/cv/estimators/__init__.py
+src/raya/handlers/cv/estimators/estimator_handler.py
+src/raya/handlers/cv/estimators/hand_estimator_handler.py
+src/raya/handlers/cv/recognizers/__init__.py
+src/raya/handlers/cv/recognizers/faces_recognizer_handler.py
+src/raya/handlers/cv/recognizers/recognizer_handler.py
+src/raya/handlers/cv/segmentators/__init__.py
+src/raya/handlers/cv/segmentators/objects_segmentator_handler.py
+src/raya/handlers/cv/segmentators/planes_segmentator_handler.py
+src/raya/handlers/cv/segmentators/segmentator_handler.py
 src/raya/handlers/general/__init__.py
 src/raya/handlers/general/callback_handler.py
 src/raya/listeners/__init__.py
 src/raya/listeners/lidar_listeners.py
 src/raya/listeners/sensors_listeners.py
 src/raya/tools/__init__.py
 src/raya/tools/filesystem.py
```

