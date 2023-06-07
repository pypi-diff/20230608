# Comparing `tmp/ovos-skill-homescreen-0.0.3a1.tar.gz` & `tmp/ovos-skill-homescreen-0.0.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-skill-homescreen-0.0.3a1.tar", last modified: Wed Jun  7 20:03:20 2023, max compression
+gzip compressed data, was "ovos-skill-homescreen-0.0.3a3.tar", last modified: Wed Jun  7 22:04:57 2023, max compression
```

## Comparing `ovos-skill-homescreen-0.0.3a1.tar` & `ovos-skill-homescreen-0.0.3a3.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.200258 ovos-skill-homescreen-0.0.3a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-07 20:03:20.200258 ovos-skill-homescreen-0.0.3a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    26307 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/initialcards.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.168258 ovos-skill-homescreen-0.0.3a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.168258 ovos-skill-homescreen-0.0.3a1/locale/de-de/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/locale/de-de/change.wallpaper.intent
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/locale/de-de/take.screenshot.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.168258 ovos-skill-homescreen-0.0.3a1/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/locale/en-us/change.wallpaper.intent
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/locale/en-us/take.screenshot.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.168258 ovos-skill-homescreen-0.0.3a1/locale/es-es/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/locale/es-es/change.wallpaper.intent
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/locale/es-es/take.screenshot.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.172258 ovos-skill-homescreen-0.0.3a1/locale/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/locale/fr-fr/change.wallpaper.intent
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/locale/fr-fr/take.screenshot.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.172258 ovos-skill-homescreen-0.0.3a1/locale/it-it/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/locale/it-it/change.wallpaper.intent
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/locale/it-it/take.screenshot.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.172258 ovos-skill-homescreen-0.0.3a1/locale/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/locale/nl-nl/change.wallpaper.intent
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/locale/nl-nl/take.screenshot.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.172258 ovos-skill-homescreen-0.0.3a1/locale/pt-pt/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/locale/pt-pt/change.wallpaper.intent
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/locale/pt-pt/take.screenshot.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.172258 ovos-skill-homescreen-0.0.3a1/ovos_skill_homescreen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-07 20:03:20.000000 ovos-skill-homescreen-0.0.3a1/ovos_skill_homescreen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-07 20:03:20.000000 ovos-skill-homescreen-0.0.3a1/ovos_skill_homescreen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:03:20.000000 ovos-skill-homescreen-0.0.3a1/ovos_skill_homescreen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-07 20:03:20.000000 ovos-skill-homescreen-0.0.3a1/ovos_skill_homescreen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-07 20:03:20.000000 ovos-skill-homescreen-0.0.3a1/ovos_skill_homescreen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 20:03:20.000000 ovos-skill-homescreen-0.0.3a1/ovos_skill_homescreen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.168258 ovos-skill-homescreen-0.0.3a1/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.172258 ovos-skill-homescreen-0.0.3a1/res/desktop/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/res/desktop/skill.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:03:20.200258 ovos-skill-homescreen-0.0.3a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.172258 ovos-skill-homescreen-0.0.3a1/skill/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/skill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/skill/cardGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/skill/dashboardHandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.176258 ovos-skill-homescreen-0.0.3a1/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/AddCardOverlay.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/AppEntry.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/AppsBar.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/BottomWidgetsArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/BoxesPage.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/DayMonthDisplay.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/ExamplesDisplay.qml
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/GridBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/HorizontalDisplayLayout.qml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/HorizontalTopArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/MainPage.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/MediaWidgetButton.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/MediaWidgetDisplay.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/NightTimePage.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/NotificationDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/SwipeArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/TimeDisplay.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/VerticalDisplayLayout.qml
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/VerticalTopArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/WeatherArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/WidgetsArea.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.176258 ovos-skill-homescreen-0.0.3a1/ui/boxes/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/boxes/PlayRelaxingMusic.qml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/boxes/PlayTheNews.qml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/boxes/SetAlarmBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/boxes/TakeNoteBox.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.176258 ovos-skill-homescreen-0.0.3a1/ui/code/
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/code/dashmodel.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.176258 ovos-skill-homescreen-0.0.3a1/ui/delegates/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/delegates/BoxAbstractDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/delegates/BoxSimpleDelegate.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.180258 ovos-skill-homescreen-0.0.3a1/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/alarmicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/cam.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/clear.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/clouds.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/delete.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/dialog-close.svg
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/fog.svg
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/high_temperature.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/humidity.svg
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/low_temperature.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/mic-min.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/mic-start.svg
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/mic.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/moon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25294 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/no-internet.svg
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/notification-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/notificationicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/offline_layer_one.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/offline_layer_two.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/partial_clouds.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/partial_clouds_day.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/partial_clouds_night.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/rain.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/snow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/storm.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/sun.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/sunrise.svg
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/sunset.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/timericon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/icons/wind.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/idle.qml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/qmldir
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.180258 ovos-skill-homescreen-0.0.3a1/ui/sounds/
--rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/sounds/clicked.wav
--rw-r--r--   0 runner    (1001) docker     (123)    67090 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/sounds/start-listening.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.180258 ovos-skill-homescreen-0.0.3a1/ui/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/templates/CardTemplate.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.188258 ovos-skill-homescreen-0.0.3a1/ui/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/AddCardOverlay_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/AddCardOverlay_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/AddCardOverlay_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/AddCardOverlay_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/AddCardOverlay_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/AddCardOverlay_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/BoxesPage_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/BoxesPage_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/BoxesPage_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/BoxesPage_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/BoxesPage_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/BoxesPage_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/ExamplesDisplay_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/ExamplesDisplay_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/ExamplesDisplay_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/ExamplesDisplay_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/ExamplesDisplay_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/ExamplesDisplay_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/GridBox_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/GridBox_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/GridBox_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/GridBox_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/GridBox_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/GridBox_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/idle_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/idle_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/idle_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/idle_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/idle_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/idle_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/skill-ovos-homescreen.openvoiceos_de.qm
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/skill-ovos-homescreen.openvoiceos_es.qm
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/skill-ovos-homescreen.openvoiceos_fr.qm
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/skill-ovos-homescreen.openvoiceos_it.qm
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/skill-ovos-homescreen.openvoiceos_nl.qm
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/translations/skill-ovos-homescreen.openvoiceos_pt.qm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:03:20.196258 ovos-skill-homescreen-0.0.3a1/ui/wallpapers/
--rw-r--r--   0 runner    (1001) docker     (123)   756810 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/wallpapers/background-01.png
--rw-r--r--   0 runner    (1001) docker     (123)  2011692 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/wallpapers/background-02.png
--rw-r--r--   0 runner    (1001) docker     (123)  1137893 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/wallpapers/background-03.png
--rw-r--r--   0 runner    (1001) docker     (123)  2125851 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/wallpapers/background-04.png
--rw-r--r--   0 runner    (1001) docker     (123)  1595246 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/wallpapers/background-05.png
--rw-r--r--   0 runner    (1001) docker     (123)  1711853 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/ui/wallpapers/default.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-07 20:03:19.000000 ovos-skill-homescreen-0.0.3a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.692313 ovos-skill-homescreen-0.0.3a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-07 22:04:57.692313 ovos-skill-homescreen-0.0.3a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26250 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/initialcards.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.656311 ovos-skill-homescreen-0.0.3a3/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.656311 ovos-skill-homescreen-0.0.3a3/locale/de-de/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/locale/de-de/change.wallpaper.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/locale/de-de/take.screenshot.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.660311 ovos-skill-homescreen-0.0.3a3/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/locale/en-us/change.wallpaper.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/locale/en-us/take.screenshot.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.660311 ovos-skill-homescreen-0.0.3a3/locale/es-es/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/locale/es-es/change.wallpaper.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/locale/es-es/take.screenshot.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.660311 ovos-skill-homescreen-0.0.3a3/locale/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/locale/fr-fr/change.wallpaper.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/locale/fr-fr/take.screenshot.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.660311 ovos-skill-homescreen-0.0.3a3/locale/it-it/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/locale/it-it/change.wallpaper.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/locale/it-it/take.screenshot.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.660311 ovos-skill-homescreen-0.0.3a3/locale/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/locale/nl-nl/change.wallpaper.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/locale/nl-nl/take.screenshot.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.660311 ovos-skill-homescreen-0.0.3a3/locale/pt-pt/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/locale/pt-pt/change.wallpaper.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/locale/pt-pt/take.screenshot.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.660311 ovos-skill-homescreen-0.0.3a3/ovos_skill_homescreen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ovos_skill_homescreen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ovos_skill_homescreen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ovos_skill_homescreen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ovos_skill_homescreen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ovos_skill_homescreen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ovos_skill_homescreen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.656311 ovos-skill-homescreen-0.0.3a3/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.660311 ovos-skill-homescreen-0.0.3a3/res/desktop/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/res/desktop/skill.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 22:04:57.692313 ovos-skill-homescreen-0.0.3a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3229 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.660311 ovos-skill-homescreen-0.0.3a3/skill/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/skill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/skill/cardGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/skill/dashboardHandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.664311 ovos-skill-homescreen-0.0.3a3/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/AddCardOverlay.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/AppEntry.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/AppsBar.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/BottomWidgetsArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/BoxesPage.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/DayMonthDisplay.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/ExamplesDisplay.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/GridBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/HorizontalDisplayLayout.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/HorizontalTopArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/MainPage.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/MediaWidgetButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/MediaWidgetDisplay.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/NightTimePage.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/NotificationDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/SwipeArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/TimeDisplay.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/VerticalDisplayLayout.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/VerticalTopArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/WeatherArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/WidgetsArea.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.668311 ovos-skill-homescreen-0.0.3a3/ui/boxes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/boxes/PlayRelaxingMusic.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/boxes/PlayTheNews.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/boxes/SetAlarmBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/boxes/TakeNoteBox.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.668311 ovos-skill-homescreen-0.0.3a3/ui/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/code/dashmodel.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.668311 ovos-skill-homescreen-0.0.3a3/ui/delegates/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/delegates/BoxAbstractDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/delegates/BoxSimpleDelegate.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.672312 ovos-skill-homescreen-0.0.3a3/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/alarmicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/cam.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/clear.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/clouds.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/dialog-close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/fog.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/high_temperature.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/humidity.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/low_temperature.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/mic-min.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/mic-start.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/mic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/moon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25294 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/no-internet.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/notification-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/notificationicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/offline_layer_one.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/offline_layer_two.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/partial_clouds.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/partial_clouds_day.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/partial_clouds_night.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/rain.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/snow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/storm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/sun.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/sunrise.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/sunset.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/timericon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/icons/wind.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/idle.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/qmldir
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.672312 ovos-skill-homescreen-0.0.3a3/ui/sounds/
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/sounds/clicked.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    67090 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/sounds/start-listening.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.672312 ovos-skill-homescreen-0.0.3a3/ui/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/templates/CardTemplate.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.680312 ovos-skill-homescreen-0.0.3a3/ui/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/AddCardOverlay_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/AddCardOverlay_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/AddCardOverlay_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/AddCardOverlay_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/AddCardOverlay_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/AddCardOverlay_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/BoxesPage_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/BoxesPage_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/BoxesPage_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/BoxesPage_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/BoxesPage_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/BoxesPage_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/ExamplesDisplay_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/ExamplesDisplay_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/ExamplesDisplay_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/ExamplesDisplay_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/ExamplesDisplay_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/ExamplesDisplay_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/GridBox_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/GridBox_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/GridBox_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/GridBox_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/GridBox_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/GridBox_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/idle_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/idle_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/idle_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/idle_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/idle_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/idle_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/skill-ovos-homescreen.openvoiceos_de.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/skill-ovos-homescreen.openvoiceos_es.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/skill-ovos-homescreen.openvoiceos_fr.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/skill-ovos-homescreen.openvoiceos_it.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/skill-ovos-homescreen.openvoiceos_nl.qm
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/translations/skill-ovos-homescreen.openvoiceos_pt.qm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:04:57.688312 ovos-skill-homescreen-0.0.3a3/ui/wallpapers/
+-rw-r--r--   0 runner    (1001) docker     (123)   756810 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/wallpapers/background-01.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2011692 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/wallpapers/background-02.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1137893 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/wallpapers/background-03.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2125851 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/wallpapers/background-04.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1595246 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/wallpapers/background-05.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1711853 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/ui/wallpapers/default.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-07 22:04:57.000000 ovos-skill-homescreen-0.0.3a3/version.py
```

### Comparing `ovos-skill-homescreen-0.0.3a1/LICENSE` & `ovos-skill-homescreen-0.0.3a3/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/__init__.py` & `ovos-skill-homescreen-0.0.3a3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,16 +212,15 @@
         if self.skill_info_api:
             self.gui['skill_examples'] = {"examples": self.skill_info_api.skill_info_examples()}
         else:
             skill_examples = get_skills_examples(randomize=self.settings.get("randomize_examples", True))
             self.gui['skill_examples'] = {"examples": skill_examples}
 
         self.gui['skill_info_enabled'] = self.examples_enabled
-        self.gui['skill_info_prefix'] = self.settings.get("examples_prefix",
-                                                          True)
+        self.gui['skill_info_prefix'] = self.settings.get("examples_prefix", False)
 
     def update_dt(self):
         """
         Loads or updates date/time via the datetime_api.
         """
         if not self.datetime_api and self.datetime_skill_id:
             LOG.debug("Requested update before datetime API loaded")
```

### Comparing `ovos-skill-homescreen-0.0.3a1/initialcards.json` & `ovos-skill-homescreen-0.0.3a3/initialcards.json`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ovos_skill_homescreen.egg-info/SOURCES.txt` & `ovos-skill-homescreen-0.0.3a3/ovos_skill_homescreen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/res/desktop/skill.json` & `ovos-skill-homescreen-0.0.3a3/res/desktop/skill.json`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/setup.py` & `ovos-skill-homescreen-0.0.3a3/setup.py`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/skill/__init__.py` & `ovos-skill-homescreen-0.0.3a3/skill/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/skill/cardGenerator.py` & `ovos-skill-homescreen-0.0.3a3/skill/cardGenerator.py`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/skill/dashboardHandler.py` & `ovos-skill-homescreen-0.0.3a3/skill/dashboardHandler.py`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/AddCardOverlay.qml` & `ovos-skill-homescreen-0.0.3a3/ui/AddCardOverlay.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/AppEntry.qml` & `ovos-skill-homescreen-0.0.3a3/ui/AppEntry.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/AppsBar.qml` & `ovos-skill-homescreen-0.0.3a3/ui/AppsBar.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/BottomWidgetsArea.qml` & `ovos-skill-homescreen-0.0.3a3/ui/BottomWidgetsArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/BoxesPage.qml` & `ovos-skill-homescreen-0.0.3a3/ui/BoxesPage.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/DayMonthDisplay.qml` & `ovos-skill-homescreen-0.0.3a3/ui/DayMonthDisplay.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/ExamplesDisplay.qml` & `ovos-skill-homescreen-0.0.3a3/ui/ExamplesDisplay.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/GridBox.qml` & `ovos-skill-homescreen-0.0.3a3/ui/GridBox.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/HorizontalDisplayLayout.qml` & `ovos-skill-homescreen-0.0.3a3/ui/HorizontalDisplayLayout.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/HorizontalTopArea.qml` & `ovos-skill-homescreen-0.0.3a3/ui/HorizontalTopArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/MainPage.qml` & `ovos-skill-homescreen-0.0.3a3/ui/MainPage.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/MediaWidgetButton.qml` & `ovos-skill-homescreen-0.0.3a3/ui/MediaWidgetButton.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/MediaWidgetDisplay.qml` & `ovos-skill-homescreen-0.0.3a3/ui/MediaWidgetDisplay.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/NightTimePage.qml` & `ovos-skill-homescreen-0.0.3a3/ui/NightTimePage.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/NotificationDelegate.qml` & `ovos-skill-homescreen-0.0.3a3/ui/NotificationDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/SwipeArea.qml` & `ovos-skill-homescreen-0.0.3a3/ui/SwipeArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/TimeDisplay.qml` & `ovos-skill-homescreen-0.0.3a3/ui/TimeDisplay.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/VerticalDisplayLayout.qml` & `ovos-skill-homescreen-0.0.3a3/ui/VerticalDisplayLayout.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/VerticalTopArea.qml` & `ovos-skill-homescreen-0.0.3a3/ui/VerticalTopArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/WeatherArea.qml` & `ovos-skill-homescreen-0.0.3a3/ui/WeatherArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/WidgetsArea.qml` & `ovos-skill-homescreen-0.0.3a3/ui/WidgetsArea.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/boxes/PlayRelaxingMusic.qml` & `ovos-skill-homescreen-0.0.3a3/ui/boxes/PlayRelaxingMusic.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/code/dashmodel.js` & `ovos-skill-homescreen-0.0.3a3/ui/code/dashmodel.js`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/delegates/BoxAbstractDelegate.qml` & `ovos-skill-homescreen-0.0.3a3/ui/delegates/BoxAbstractDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/delegates/BoxSimpleDelegate.qml` & `ovos-skill-homescreen-0.0.3a3/ui/delegates/BoxSimpleDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/alarmicon.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/alarmicon.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/clear.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/clear.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/close.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/close.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/clouds.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/clouds.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/delete.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/delete.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/dialog-close.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/dialog-close.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/fog.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/fog.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/high_temperature.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/high_temperature.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/humidity.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/humidity.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/low_temperature.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/low_temperature.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/mic-min.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/mic-min.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/mic-start.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/mic-start.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/mic.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/mic.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/no-internet.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/no-internet.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/notificationicon.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/notificationicon.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/offline_layer_one.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/offline_layer_one.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/offline_layer_two.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/offline_layer_two.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/partial_clouds.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/partial_clouds.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/partial_clouds_day.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/partial_clouds_day.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/partial_clouds_night.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/partial_clouds_night.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/rain.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/rain.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/snow.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/snow.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/storm.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/storm.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/sun.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/sun.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/sunrise.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/sunrise.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/sunset.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/sunset.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/timericon.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/timericon.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/icons/wind.svg` & `ovos-skill-homescreen-0.0.3a3/ui/icons/wind.svg`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/idle.qml` & `ovos-skill-homescreen-0.0.3a3/ui/idle.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/qmldir` & `ovos-skill-homescreen-0.0.3a3/ui/qmldir`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/sounds/clicked.wav` & `ovos-skill-homescreen-0.0.3a3/ui/sounds/clicked.wav`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/sounds/start-listening.wav` & `ovos-skill-homescreen-0.0.3a3/ui/sounds/start-listening.wav`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/templates/CardTemplate.qml` & `ovos-skill-homescreen-0.0.3a3/ui/templates/CardTemplate.qml`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/AddCardOverlay_de.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/AddCardOverlay_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/AddCardOverlay_es.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/AddCardOverlay_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/AddCardOverlay_fr.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/AddCardOverlay_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/AddCardOverlay_it.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/AddCardOverlay_pt.ts`

 * *Files 11% similar despite different names*

#### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/AddCardOverlay_it.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/AddCardOverlay_pt.ts`

```diff
@@ -1,57 +1,57 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS language="it_IT" version="2.1">
+<TS language="pt_BR" version="2.1">
   <context>
     <name>AddCardOverlay</name>
     <message>
       <location filename="../AddCardOverlay.qml" line="63"/>
       <source>Add Card</source>
-      <translation>Aggiungi carta</translation>
+      <translation>Adicionar cartão</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="106"/>
       <source>Header</source>
-      <translation>Intestazione</translation>
+      <translation>Cabeçalho</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="127"/>
       <source>Card Header Text</source>
-      <translation>Testo dell'intestazione della carta</translation>
+      <translation>Texto do cabeçalho do cartão</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="147"/>
       <source>Description</source>
-      <translation>Descrizione</translation>
+      <translation>Descrição</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="168"/>
       <source>Card Description Text</source>
-      <translation>Testo di descrizione della carta</translation>
+      <translation>Texto de descrição do cartão</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="189"/>
       <source>Utterance</source>
-      <translation>Espressione</translation>
+      <translation>Enunciado</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="211"/>
       <source>Card Action Text</source>
-      <translation>Testo dell'azione della carta</translation>
+      <translation>Texto da ação do cartão</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="232"/>
       <source>Icon</source>
-      <translation>Icona</translation>
+      <translation>Ícone</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="302"/>
       <source>Add</source>
-      <translation>Aggiungere</translation>
+      <translation>Adicionar</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="326"/>
       <source>Cancel</source>
-      <translation>Annulla</translation>
+      <translation>Cancelar</translation>
     </message>
   </context>
 </TS>
```

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/AddCardOverlay_nl.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/AddCardOverlay_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/AddCardOverlay_pt.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/AddCardOverlay_it.ts`

 * *Files 22% similar despite different names*

#### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/AddCardOverlay_pt.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/AddCardOverlay_it.ts`

```diff
@@ -1,57 +1,57 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS language="pt_BR" version="2.1">
+<TS language="it_IT" version="2.1">
   <context>
     <name>AddCardOverlay</name>
     <message>
       <location filename="../AddCardOverlay.qml" line="63"/>
       <source>Add Card</source>
-      <translation>Adicionar cartão</translation>
+      <translation>Aggiungi blocco</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="106"/>
       <source>Header</source>
-      <translation>Cabeçalho</translation>
+      <translation>Intestazione</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="127"/>
       <source>Card Header Text</source>
-      <translation>Texto do cabeçalho do cartão</translation>
+      <translation>Testo dell'intestazione del blocco</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="147"/>
       <source>Description</source>
-      <translation>Descrição</translation>
+      <translation>Descrizione</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="168"/>
       <source>Card Description Text</source>
-      <translation>Texto de descrição do cartão</translation>
+      <translation>Descrizione del blocco</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="189"/>
       <source>Utterance</source>
-      <translation>Enunciado</translation>
+      <translation>Espressione</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="211"/>
       <source>Card Action Text</source>
-      <translation>Texto da ação do cartão</translation>
+      <translation>Funzione del blocco</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="232"/>
       <source>Icon</source>
-      <translation>Ícone</translation>
+      <translation>Icona</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="302"/>
       <source>Add</source>
-      <translation>Adicionar</translation>
+      <translation>Aggiungere</translation>
     </message>
     <message>
       <location filename="../AddCardOverlay.qml" line="326"/>
       <source>Cancel</source>
-      <translation>Cancelar</translation>
+      <translation>Annulla</translation>
     </message>
   </context>
 </TS>
```

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/BoxesPage_de.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/BoxesPage_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/BoxesPage_es.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/BoxesPage_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/BoxesPage_fr.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/BoxesPage_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/BoxesPage_it.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/BoxesPage_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/BoxesPage_nl.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/BoxesPage_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/BoxesPage_pt.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/BoxesPage_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/GridBox_de.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/GridBox_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/GridBox_es.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/GridBox_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/GridBox_fr.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/GridBox_fr.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/GridBox_it.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/GridBox_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/GridBox_nl.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/GridBox_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/GridBox_pt.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/GridBox_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/idle_de.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/idle_de.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/idle_es.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/idle_es.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/idle_it.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/idle_it.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/idle_nl.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/idle_nl.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/idle_pt.ts` & `ovos-skill-homescreen-0.0.3a3/ui/translations/idle_pt.ts`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/skill-ovos-homescreen.openvoiceos_de.qm` & `ovos-skill-homescreen-0.0.3a3/ui/translations/skill-ovos-homescreen.openvoiceos_de.qm`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/skill-ovos-homescreen.openvoiceos_es.qm` & `ovos-skill-homescreen-0.0.3a3/ui/translations/skill-ovos-homescreen.openvoiceos_es.qm`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/skill-ovos-homescreen.openvoiceos_fr.qm` & `ovos-skill-homescreen-0.0.3a3/ui/translations/skill-ovos-homescreen.openvoiceos_fr.qm`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/skill-ovos-homescreen.openvoiceos_it.qm` & `ovos-skill-homescreen-0.0.3a3/ui/translations/skill-ovos-homescreen.openvoiceos_it.qm`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/skill-ovos-homescreen.openvoiceos_nl.qm` & `ovos-skill-homescreen-0.0.3a3/ui/translations/skill-ovos-homescreen.openvoiceos_nl.qm`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/translations/skill-ovos-homescreen.openvoiceos_pt.qm` & `ovos-skill-homescreen-0.0.3a3/ui/translations/skill-ovos-homescreen.openvoiceos_pt.qm`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/wallpapers/background-01.png` & `ovos-skill-homescreen-0.0.3a3/ui/wallpapers/background-01.png`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/wallpapers/background-02.png` & `ovos-skill-homescreen-0.0.3a3/ui/wallpapers/background-02.png`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/wallpapers/background-03.png` & `ovos-skill-homescreen-0.0.3a3/ui/wallpapers/background-03.png`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/wallpapers/background-04.png` & `ovos-skill-homescreen-0.0.3a3/ui/wallpapers/background-04.png`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/wallpapers/background-05.png` & `ovos-skill-homescreen-0.0.3a3/ui/wallpapers/background-05.png`

 * *Files identical despite different names*

### Comparing `ovos-skill-homescreen-0.0.3a1/ui/wallpapers/default.jpg` & `ovos-skill-homescreen-0.0.3a3/ui/wallpapers/default.jpg`

 * *Files identical despite different names*

