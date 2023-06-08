# Comparing `tmp/BasicLibrary.PY-0.5.4.tar.gz` & `tmp/BasicLibrary.PY-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BasicLibrary.PY-0.5.4.tar", last modified: Wed Jun  7 14:06:45 2023, max compression
+gzip compressed data, was "BasicLibrary.PY-0.5.5.tar", last modified: Thu Jun  8 02:47:46 2023, max compression
```

## Comparing `BasicLibrary.PY-0.5.4.tar` & `BasicLibrary.PY-0.5.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 14:06:45.256817 BasicLibrary.PY-0.5.4/
-drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.196821 BasicLibrary.PY-0.5.4/BasicLibrary/
--rw-rw-rw-   0        0        0      883 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/__init__.py
--rw-rw-rw-   0        0        0      560 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.4/BasicLibrary/__projectHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.339817 BasicLibrary.PY-0.5.4/BasicLibrary/biz/
--rw-rw-rw-   0        0        0      172 2021-11-07 07:17:04.000000 BasicLibrary.PY-0.5.4/BasicLibrary/biz/__init__.py
--rw-rw-rw-   0        0        0     2559 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.4/BasicLibrary/biz/stockHelper.py
--rw-rw-rw-   0        0        0      226 2021-12-25 06:01:03.000000 BasicLibrary.PY-0.5.4/BasicLibrary/biz/tencentHelper.py
--rw-rw-rw-   0        0        0     3242 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.4/BasicLibrary/configHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.628822 BasicLibrary.PY-0.5.4/BasicLibrary/data/
--rw-rw-rw-   0        0        0      174 2022-03-10 00:57:41.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/__init__.py
--rw-rw-rw-   0        0        0     1771 2022-04-20 12:57:51.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/collectionHelper.py
--rw-rw-rw-   0        0        0     4891 2022-04-20 11:14:53.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/dateTimeHelper.py
--rw-rw-rw-   0        0        0     1704 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/dictHelper.py
--rw-rw-rw-   0        0        0        0 2021-04-24 11:00:12.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/htmlHelper.py
--rw-rw-rw-   0        0        0     4373 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/listHelper.py
--rw-rw-rw-   0        0        0     1280 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/numberHelper.py
--rw-rw-rw-   0        0        0     2645 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/objectHelper.py
--rw-rw-rw-   0        0        0     3610 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/pandasHelper.py
--rw-rw-rw-   0        0        0     1221 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/randomHelper.py
--rw-rw-rw-   0        0        0      771 2022-04-20 11:16:27.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/reflectHelper.py
--rw-rw-rw-   0        0        0     1621 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/regexHelper.py
--rw-rw-rw-   0        0        0        2 2021-03-21 10:02:22.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/setHelper.py
--rw-rw-rw-   0        0        0     6499 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/data/stringHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.745815 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/
-drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.822815 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:17:08.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/__init__.py
--rw-rw-rw-   0        0        0     1501 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/ddl.py
--rw-rw-rw-   0        0        0     2829 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/helper.py
--rw-rw-rw-   0        0        0    10551 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/mate.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.881820 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:18:12.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/__init__.py
--rw-rw-rw-   0        0        0     4642 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/ddl.py
--rw-rw-rw-   0        0        0    12613 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/mate.py
--rw-rw-rw-   0        0        0     3368 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/pool.py
--rw-rw-rw-   0        0        0      218 2022-04-20 11:22:18.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/__init__.py
--rw-rw-rw-   0        0        0     4785 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseClient.py
--rw-rw-rw-   0        0        0     2187 2022-04-20 11:23:22.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseDDL.py
--rw-rw-rw-   0        0        0      345 2022-04-20 11:23:51.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseEnum.py
--rw-rw-rw-   0        0        0     6446 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseHelper.py
--rw-rw-rw-   0        0        0     5468 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseMate.py
--rw-rw-rw-   0        0        0     1144 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseUnitTest.py
--rw-rw-rw-   0        0        0      510 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.4/BasicLibrary/enums.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.937821 BasicLibrary.PY-0.5.4/BasicLibrary/environment/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.4/BasicLibrary/environment/__init__.py
--rw-rw-rw-   0        0        0     1265 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.4/BasicLibrary/environment/consoleHelper.py
--rw-rw-rw-   0        0        0     1059 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/environment/envHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:06:45.039818 BasicLibrary.PY-0.5.4/BasicLibrary/io/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.4/BasicLibrary/io/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/io/dirHelper.py
--rw-rw-rw-   0        0        0     5979 2023-06-07 07:54:07.000000 BasicLibrary.PY-0.5.4/BasicLibrary/io/fileHelper.py
--rw-rw-rw-   0        0        0     1435 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.4/BasicLibrary/io/ioHelper.py
--rw-rw-rw-   0        0        0     1942 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.4/BasicLibrary/io/pathHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:06:45.125815 BasicLibrary.PY-0.5.4/BasicLibrary/model/
--rw-rw-rw-   0        0        0      186 2022-04-20 11:26:05.000000 BasicLibrary.PY-0.5.4/BasicLibrary/model/__init__.py
--rw-rw-rw-   0        0        0     1326 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.4/BasicLibrary/model/container.py
--rw-rw-rw-   0        0        0     2185 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.4/BasicLibrary/model/dataCompare.py
--rw-rw-rw-   0        0        0     1099 2022-04-20 11:26:29.000000 BasicLibrary.PY-0.5.4/BasicLibrary/model/kvPair.py
--rw-rw-rw-   0        0        0      342 2022-04-20 11:26:30.000000 BasicLibrary.PY-0.5.4/BasicLibrary/model/stopWatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:06:45.174818 BasicLibrary.PY-0.5.4/BasicLibrary/office/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:26:38.000000 BasicLibrary.PY-0.5.4/BasicLibrary/office/__init__.py
--rw-rw-rw-   0        0        0     6634 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.4/BasicLibrary/office/excelBookMate.py
--rw-rw-rw-   0        0        0     2458 2023-06-07 11:39:53.000000 BasicLibrary.PY-0.5.4/BasicLibrary/office/excelHelper.py
--rw-rw-rw-   0        0        0     3375 2023-06-07 11:44:09.000000 BasicLibrary.PY-0.5.4/BasicLibrary/office/excelMisc.py
--rw-rw-rw-   0        0        0    11164 2023-06-07 14:03:03.000000 BasicLibrary.PY-0.5.4/BasicLibrary/office/excelSheetMate.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:06:45.187821 BasicLibrary.PY-0.5.4/BasicLibrary/pattern/
--rw-rw-rw-   0        0        0      163 2022-04-20 11:27:42.000000 BasicLibrary.PY-0.5.4/BasicLibrary/pattern/__init__.py
--rw-rw-rw-   0        0        0      470 2022-04-20 11:28:04.000000 BasicLibrary.PY-0.5.4/BasicLibrary/pattern/singleton.py
--rw-rw-rw-   0        0        0      374 2022-04-20 11:31:03.000000 BasicLibrary.PY-0.5.4/BasicLibrary/projectHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:06:45.201821 BasicLibrary.PY-0.5.4/BasicLibrary/syntax/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:28:12.000000 BasicLibrary.PY-0.5.4/BasicLibrary/syntax/__init__.py
--rw-rw-rw-   0        0        0     1664 2022-04-20 11:28:39.000000 BasicLibrary.PY-0.5.4/BasicLibrary/syntax/switch.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:06:45.242815 BasicLibrary.PY-0.5.4/BasicLibrary/web/
--rw-rw-rw-   0        0        0      164 2022-04-20 11:28:40.000000 BasicLibrary.PY-0.5.4/BasicLibrary/web/__init__.py
--rw-rw-rw-   0        0        0     7972 2021-11-09 12:40:32.000000 BasicLibrary.PY-0.5.4/BasicLibrary/web/beautifulSoupHelper.py
--rw-rw-rw-   0        0        0     1790 2022-04-20 11:28:54.000000 BasicLibrary.PY-0.5.4/BasicLibrary/web/requestHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:06:44.253819 BasicLibrary.PY-0.5.4/BasicLibrary.PY.egg-info/
--rw-rw-rw-   0        0        0     2896 2023-06-07 14:06:42.000000 BasicLibrary.PY-0.5.4/BasicLibrary.PY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2290 2023-06-07 14:06:43.000000 BasicLibrary.PY-0.5.4/BasicLibrary.PY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 14:06:43.000000 BasicLibrary.PY-0.5.4/BasicLibrary.PY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-07 14:06:43.000000 BasicLibrary.PY-0.5.4/BasicLibrary.PY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      119 2022-04-20 11:32:35.000000 BasicLibrary.PY-0.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2896 2023-06-07 14:06:45.253816 BasicLibrary.PY-0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2023-06-06 10:08:46.000000 BasicLibrary.PY-0.5.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 14:06:45.256817 BasicLibrary.PY-0.5.4/setup.cfg
--rw-rw-rw-   0        0        0     4280 2023-06-07 14:06:11.000000 BasicLibrary.PY-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:47:46.028277 BasicLibrary.PY-0.5.5/
+drwxrwxrwx   0        0        0        0 2023-06-08 02:47:41.182212 BasicLibrary.PY-0.5.5/BasicLibrary/
+-rw-rw-rw-   0        0        0      883 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.5/BasicLibrary/__init__.py
+-rw-rw-rw-   0        0        0      560 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.5/BasicLibrary/__projectHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:47:41.393208 BasicLibrary.PY-0.5.5/BasicLibrary/biz/
+-rw-rw-rw-   0        0        0      172 2021-11-07 07:17:04.000000 BasicLibrary.PY-0.5.5/BasicLibrary/biz/__init__.py
+-rw-rw-rw-   0        0        0     2559 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.5/BasicLibrary/biz/stockHelper.py
+-rw-rw-rw-   0        0        0      226 2021-12-25 06:01:03.000000 BasicLibrary.PY-0.5.5/BasicLibrary/biz/tencentHelper.py
+-rw-rw-rw-   0        0        0     3242 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.5/BasicLibrary/configHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:47:41.759115 BasicLibrary.PY-0.5.5/BasicLibrary/data/
+-rw-rw-rw-   0        0        0      174 2022-03-10 00:57:41.000000 BasicLibrary.PY-0.5.5/BasicLibrary/data/__init__.py
+-rw-rw-rw-   0        0        0     1771 2022-04-20 12:57:51.000000 BasicLibrary.PY-0.5.5/BasicLibrary/data/collectionHelper.py
+-rw-rw-rw-   0        0        0     5753 2023-06-08 02:21:21.000000 BasicLibrary.PY-0.5.5/BasicLibrary/data/dateTimeHelper.py
+-rw-rw-rw-   0        0        0     1704 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.5/BasicLibrary/data/dictHelper.py
+-rw-rw-rw-   0        0        0        0 2021-04-24 11:00:12.000000 BasicLibrary.PY-0.5.5/BasicLibrary/data/htmlHelper.py
+-rw-rw-rw-   0        0        0     4373 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.5/BasicLibrary/data/listHelper.py
+-rw-rw-rw-   0        0        0     1280 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.5/BasicLibrary/data/numberHelper.py
+-rw-rw-rw-   0        0        0     2728 2023-06-08 02:17:54.000000 BasicLibrary.PY-0.5.5/BasicLibrary/data/objectHelper.py
+-rw-rw-rw-   0        0        0     3610 2022-04-20 11:16:24.000000 BasicLibrary.PY-0.5.5/BasicLibrary/data/pandasHelper.py
+-rw-rw-rw-   0        0        0     1221 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.5/BasicLibrary/data/randomHelper.py
+-rw-rw-rw-   0        0        0      771 2022-04-20 11:16:27.000000 BasicLibrary.PY-0.5.5/BasicLibrary/data/reflectHelper.py
+-rw-rw-rw-   0        0        0     1621 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.5/BasicLibrary/data/regexHelper.py
+-rw-rw-rw-   0        0        0        2 2021-03-21 10:02:22.000000 BasicLibrary.PY-0.5.5/BasicLibrary/data/setHelper.py
+-rw-rw-rw-   0        0        0     6499 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.5/BasicLibrary/data/stringHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:47:41.928113 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/
+drwxrwxrwx   0        0        0        0 2023-06-08 02:47:41.998115 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MongoDB/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:17:08.000000 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MongoDB/__init__.py
+-rw-rw-rw-   0        0        0     1501 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MongoDB/ddl.py
+-rw-rw-rw-   0        0        0     2829 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MongoDB/helper.py
+-rw-rw-rw-   0        0        0    10551 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MongoDB/mate.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:47:42.071115 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MySql/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:18:12.000000 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MySql/__init__.py
+-rw-rw-rw-   0        0        0     4642 2023-06-06 09:46:32.000000 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MySql/ddl.py
+-rw-rw-rw-   0        0        0    12613 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MySql/mate.py
+-rw-rw-rw-   0        0        0     3368 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MySql/pool.py
+-rw-rw-rw-   0        0        0      218 2022-04-20 11:22:18.000000 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/__init__.py
+-rw-rw-rw-   0        0        0     4785 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/databaseClient.py
+-rw-rw-rw-   0        0        0     2187 2022-04-20 11:23:22.000000 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/databaseDDL.py
+-rw-rw-rw-   0        0        0      345 2022-04-20 11:23:51.000000 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/databaseEnum.py
+-rw-rw-rw-   0        0        0     6446 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/databaseHelper.py
+-rw-rw-rw-   0        0        0     5468 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/databaseMate.py
+-rw-rw-rw-   0        0        0     1144 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/databaseUnitTest.py
+-rw-rw-rw-   0        0        0      510 2022-04-20 11:30:48.000000 BasicLibrary.PY-0.5.5/BasicLibrary/enums.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:47:42.177113 BasicLibrary.PY-0.5.5/BasicLibrary/environment/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.5/BasicLibrary/environment/__init__.py
+-rw-rw-rw-   0        0        0     1265 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.5/BasicLibrary/environment/consoleHelper.py
+-rw-rw-rw-   0        0        0     1059 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.5/BasicLibrary/environment/envHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:47:42.767358 BasicLibrary.PY-0.5.5/BasicLibrary/io/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:24:39.000000 BasicLibrary.PY-0.5.5/BasicLibrary/io/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.5/BasicLibrary/io/dirHelper.py
+-rw-rw-rw-   0        0        0     5979 2023-06-07 07:54:07.000000 BasicLibrary.PY-0.5.5/BasicLibrary/io/fileHelper.py
+-rw-rw-rw-   0        0        0     1435 2023-06-06 09:46:33.000000 BasicLibrary.PY-0.5.5/BasicLibrary/io/ioHelper.py
+-rw-rw-rw-   0        0        0     1942 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.5/BasicLibrary/io/pathHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:47:44.798273 BasicLibrary.PY-0.5.5/BasicLibrary/model/
+-rw-rw-rw-   0        0        0      186 2022-04-20 11:26:05.000000 BasicLibrary.PY-0.5.5/BasicLibrary/model/__init__.py
+-rw-rw-rw-   0        0        0     1326 2023-06-06 09:46:34.000000 BasicLibrary.PY-0.5.5/BasicLibrary/model/container.py
+-rw-rw-rw-   0        0        0     2185 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.5/BasicLibrary/model/dataCompare.py
+-rw-rw-rw-   0        0        0     1099 2022-04-20 11:26:29.000000 BasicLibrary.PY-0.5.5/BasicLibrary/model/kvPair.py
+-rw-rw-rw-   0        0        0      342 2022-04-20 11:26:30.000000 BasicLibrary.PY-0.5.5/BasicLibrary/model/stopWatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:47:45.361277 BasicLibrary.PY-0.5.5/BasicLibrary/office/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:26:38.000000 BasicLibrary.PY-0.5.5/BasicLibrary/office/__init__.py
+-rw-rw-rw-   0        0        0     6634 2023-06-06 09:46:31.000000 BasicLibrary.PY-0.5.5/BasicLibrary/office/excelBookMate.py
+-rw-rw-rw-   0        0        0     2458 2023-06-07 11:39:53.000000 BasicLibrary.PY-0.5.5/BasicLibrary/office/excelHelper.py
+-rw-rw-rw-   0        0        0     3375 2023-06-07 11:44:09.000000 BasicLibrary.PY-0.5.5/BasicLibrary/office/excelMisc.py
+-rw-rw-rw-   0        0        0    11164 2023-06-07 14:03:03.000000 BasicLibrary.PY-0.5.5/BasicLibrary/office/excelSheetMate.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:47:45.453276 BasicLibrary.PY-0.5.5/BasicLibrary/pattern/
+-rw-rw-rw-   0        0        0      163 2022-04-20 11:27:42.000000 BasicLibrary.PY-0.5.5/BasicLibrary/pattern/__init__.py
+-rw-rw-rw-   0        0        0      470 2022-04-20 11:28:04.000000 BasicLibrary.PY-0.5.5/BasicLibrary/pattern/singleton.py
+-rw-rw-rw-   0        0        0      374 2022-04-20 11:31:03.000000 BasicLibrary.PY-0.5.5/BasicLibrary/projectHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:47:45.560279 BasicLibrary.PY-0.5.5/BasicLibrary/syntax/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:28:12.000000 BasicLibrary.PY-0.5.5/BasicLibrary/syntax/__init__.py
+-rw-rw-rw-   0        0        0     1664 2022-04-20 11:28:39.000000 BasicLibrary.PY-0.5.5/BasicLibrary/syntax/switch.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:47:46.004281 BasicLibrary.PY-0.5.5/BasicLibrary/web/
+-rw-rw-rw-   0        0        0      164 2022-04-20 11:28:40.000000 BasicLibrary.PY-0.5.5/BasicLibrary/web/__init__.py
+-rw-rw-rw-   0        0        0     7972 2021-11-09 12:40:32.000000 BasicLibrary.PY-0.5.5/BasicLibrary/web/beautifulSoupHelper.py
+-rw-rw-rw-   0        0        0     1790 2022-04-20 11:28:54.000000 BasicLibrary.PY-0.5.5/BasicLibrary/web/requestHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:47:41.340212 BasicLibrary.PY-0.5.5/BasicLibrary.PY.egg-info/
+-rw-rw-rw-   0        0        0     2896 2023-06-08 02:47:39.000000 BasicLibrary.PY-0.5.5/BasicLibrary.PY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2290 2023-06-08 02:47:40.000000 BasicLibrary.PY-0.5.5/BasicLibrary.PY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 02:47:39.000000 BasicLibrary.PY-0.5.5/BasicLibrary.PY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-08 02:47:40.000000 BasicLibrary.PY-0.5.5/BasicLibrary.PY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      119 2022-04-20 11:32:35.000000 BasicLibrary.PY-0.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2896 2023-06-08 02:47:46.023277 BasicLibrary.PY-0.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-06-06 10:08:46.000000 BasicLibrary.PY-0.5.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-08 02:47:46.029276 BasicLibrary.PY-0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     4280 2023-06-08 02:46:06.000000 BasicLibrary.PY-0.5.5/setup.py
```

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/__init__.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/__projectHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/__projectHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/biz/stockHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/biz/stockHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/configHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/configHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/data/collectionHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/data/collectionHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/data/dateTimeHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/data/dateTimeHelper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re
 from datetime import datetime, timedelta, date
 
+from BasicLibrary import ObjectHelper
+
 
 # +--------------------------------------------------------------------------
 # |::说明：| Python内置两个方法的说明
 # |·······|     strptime()方法,里面的p是parse的意思，就是把字符串解析成日期时间类型
 # |·······|     strftime()方法,里面的f是format的意思，就是把日期时间类型格式化为某种格式的字符串
 # +--------------------------------------------------------------------------
 
@@ -37,20 +39,40 @@
         :return:
         """
         return DateTimeHelper.convert_from_string(date_time_string, "%Y%m%d")
 
     @staticmethod
     def get_compact_string(date_time_value=None):
         """
-        获取“20210221”这种类型的日期字符串（在股市交易中常用）
+        获取“20210221”这种类型的日期字符串（在股市交易中常用）;跟get_compact_date_string功能一样
         :param date_time_value:
         :return:
         """
         return DateTimeHelper.get_string(date_time_value, "%Y%m%d")
 
+    @classmethod
+    def get_compact_date_string(cls, date_time_value=None):
+        """
+        获取“20210221”这种类型的日期字符串（在股市交易中常用）;get_compact_string的别名
+        :param date_time_value:
+        :return:
+        """
+        return cls.get_compact_string(date_time_value)
+        pass
+
+    @classmethod
+    def get_compact_date_time_string(cls, date_time_value=None):
+        """
+        获取“20210221030526”这种类型的日期时间字符串
+        :param date_time_value:
+        :return:
+        """
+        return DateTimeHelper.get_string(date_time_value, "%Y%m%d%H%M%S")
+        pass
+
     @staticmethod
     def get_short_string(date_time_value=None, formatter="%Y-%m-%d"):
         """
         获取“2021-02-21”这种短类型格式的日期字符串
         :param date_time_value:
         :param formatter:
         :return:
@@ -62,25 +84,28 @@
         """
         获取给定时间的标准格式日期字符串表示形式(类似2021-10-11 03:34:25)
         :param date_time_value:
         :return:
         """
         return DateTimeHelper.get_string(date_time_value, "%Y-%m-%d %H:%M:%S")
 
-    @staticmethod
-    def get_string(date_time_value=None, formatter="%Y-%m-%d %H:%M:%S"):
+    @classmethod
+    def get_string(cls, date_time_value=None, formatter="%Y-%m-%d %H:%M:%S"):
         """
         获取给定时间的字符串表示形式（默认情况下返回当前的时间数据）
         :param formatter:
         :param date_time_value: 需要展示的日期时间数据，默认不传递此参数则返回当前时间数据
         :return: 给定时间的字符串表示形式
         """
         if date_time_value is None:
             date_time_value = datetime.now()
 
+        if ObjectHelper.get_type(date_time_value) is str:
+            date_time_value = cls.convert_from_string(date_time_value)
+
         result = date_time_value.strftime(formatter)
         return result
 
     @staticmethod
     def add_days(original_date=None, delta=1, original_date_formatter="%Y%m%d"):
         """
```

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/data/dictHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/data/dictHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/data/listHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/data/listHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/data/numberHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/data/numberHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/data/objectHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/data/objectHelper.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 
         return False
 
     @staticmethod
     def get_type(data):
         """
         获取目标对象的数据类型
+        使用方法：`if ObjectHelper.get_type(entity_dict_or_list) is dict:`等
         :param data:
         :return:
         """
         return type(data)
 
     @staticmethod
     def get_length(data):
```

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/data/pandasHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/data/pandasHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/data/randomHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/data/randomHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/data/reflectHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/data/reflectHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/data/regexHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/data/regexHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/data/stringHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/data/stringHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/ddl.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MongoDB/ddl.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/helper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MongoDB/helper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MongoDB/mate.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MongoDB/mate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/ddl.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MySql/ddl.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/mate.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MySql/mate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/MySql/pool.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/MySql/pool.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseClient.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/databaseClient.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseDDL.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/databaseDDL.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/databaseHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseMate.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/databaseMate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/dataBase/databaseUnitTest.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/dataBase/databaseUnitTest.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/environment/consoleHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/environment/consoleHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/environment/envHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/environment/envHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/io/dirHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/io/dirHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/io/fileHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/io/fileHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/io/ioHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/io/ioHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/io/pathHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/io/pathHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/model/container.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/model/container.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/model/dataCompare.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/model/dataCompare.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/model/kvPair.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/model/kvPair.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/office/excelBookMate.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/office/excelBookMate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/office/excelHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/office/excelHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/office/excelMisc.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/office/excelMisc.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/office/excelSheetMate.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/office/excelSheetMate.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/syntax/switch.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/syntax/switch.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/web/beautifulSoupHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/web/beautifulSoupHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary/web/requestHelper.py` & `BasicLibrary.PY-0.5.5/BasicLibrary/web/requestHelper.py`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary.PY.egg-info/PKG-INFO` & `BasicLibrary.PY-0.5.5/BasicLibrary.PY.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BasicLibrary.PY
-Version: 0.5.4
+Version: 0.5.5
 Summary: 企业级的 PYTHON 库
 Home-page: https://github.com/notinmood/BasicLibrary.PY
 Author: xiedali
 Author-email: 9727005@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `BasicLibrary.PY-0.5.4/BasicLibrary.PY.egg-info/SOURCES.txt` & `BasicLibrary.PY-0.5.5/BasicLibrary.PY.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/PKG-INFO` & `BasicLibrary.PY-0.5.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BasicLibrary.PY
-Version: 0.5.4
+Version: 0.5.5
 Summary: 企业级的 PYTHON 库
 Home-page: https://github.com/notinmood/BasicLibrary.PY
 Author: xiedali
 Author-email: 9727005@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `BasicLibrary.PY-0.5.4/README.md` & `BasicLibrary.PY-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `BasicLibrary.PY-0.5.4/setup.py` & `BasicLibrary.PY-0.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 NAME = 'BasicLibrary.PY'
 DESCRIPTION = '企业级的 PYTHON 库'
 URL = 'https://github.com/notinmood/BasicLibrary.PY'
 EMAIL = '9727005@qq.com'
 AUTHOR = 'xiedali'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.5.4'
+VERSION = '0.5.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

