# Comparing `tmp/mote-gtest-gui-0.8.1.tar.gz` & `tmp/mote-gtest-gui-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mote-gtest-gui-0.8.1.tar", last modified: Mon Apr 24 19:08:38 2023, max compression
+gzip compressed data, was "mote-gtest-gui-0.9.0.tar", last modified: Thu Jun  8 19:35:59 2023, max compression
```

## Comparing `mote-gtest-gui-0.8.1.tar` & `mote-gtest-gui-0.9.0.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-04-24 19:08:38.035321 mote-gtest-gui-0.8.1/
--rw-r--r--   0 tom      (31978) tom       (2000)    35149 2023-03-12 12:42:14.000000 mote-gtest-gui-0.8.1/LICENSE
--rw-r--r--   0 tom      (31978) tom       (2000)      110 2023-04-23 09:14:13.000000 mote-gtest-gui-0.8.1/MANIFEST.in
--rw-r--r--   0 tom      (31978) tom       (2000)    28541 2023-04-24 19:08:38.035321 mote-gtest-gui-0.8.1/PKG-INFO
--rw-r--r--   0 tom      (31978) tom       (2000)     4976 2023-04-24 19:03:19.000000 mote-gtest-gui-0.8.1/README.md
--rw-r--r--   0 tom      (31978) tom       (2000)     2901 2023-04-24 18:58:13.000000 mote-gtest-gui-0.8.1/TODO.txt
-drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-04-24 19:08:38.031321 mote-gtest-gui-0.8.1/bin/
--rwxr-xr-x   0 tom      (31978) tom       (2000)     1280 2023-04-23 09:14:13.000000 mote-gtest-gui-0.8.1/bin/gtest_gui
-drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-04-24 19:08:38.035321 mote-gtest-gui-0.8.1/gtest_gui/
--rw-r--r--   0 tom      (31978) tom       (2000)       22 2023-03-21 18:15:59.000000 mote-gtest-gui-0.8.1/gtest_gui/__init__.py
--rw-r--r--   0 tom      (31978) tom       (2000)       31 2023-03-21 18:15:59.000000 mote-gtest-gui-0.8.1/gtest_gui/__main__.py
--rw-r--r--   0 tom      (31978) tom       (2000)      670 2023-03-21 18:15:59.000000 mote-gtest-gui-0.8.1/gtest_gui/bisect.py
--rwxr-xr-x   0 tom      (31978) tom       (2000)    14215 2023-04-24 07:48:51.000000 mote-gtest-gui-0.8.1/gtest_gui/config_db.py
--rw-r--r--   0 tom      (31978) tom       (2000)    12432 2023-04-24 18:49:48.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_browser.py
--rw-r--r--   0 tom      (31978) tom       (2000)    10132 2023-04-18 11:26:41.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_config.py
--rw-r--r--   0 tom      (31978) tom       (2000)     8073 2023-04-02 17:01:27.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_debug.py
--rw-r--r--   0 tom      (31978) tom       (2000)     7488 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_font_sel.py
--rwxr-xr-x   0 tom      (31978) tom       (2000)    10929 2023-04-16 18:15:48.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_help.py
--rw-r--r--   0 tom      (31978) tom       (2000)     9212 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_job_list.py
--rw-r--r--   0 tom      (31978) tom       (2000)    17290 2023-04-24 18:51:42.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_main.py
--rw-r--r--   0 tom      (31978) tom       (2000)    20826 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.1/gtest_gui/dlg_tc_list.py
--rw-r--r--   0 tom      (31978) tom       (2000)     1637 2023-03-21 18:15:59.000000 mote-gtest-gui-0.8.1/gtest_gui/fcntl.py
--rw-r--r--   0 tom      (31978) tom       (2000)    10319 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.1/gtest_gui/filter_expr.py
--rw-r--r--   0 tom      (31978) tom       (2000)    37727 2023-04-24 18:22:59.000000 mote-gtest-gui-0.8.1/gtest_gui/gtest.py
--rw-r--r--   0 tom      (31978) tom       (2000)    33151 2023-04-24 19:00:42.000000 mote-gtest-gui-0.8.1/gtest_gui/help_db.py
--rw-r--r--   0 tom      (31978) tom       (2000)     4120 2023-04-24 07:48:51.000000 mote-gtest-gui-0.8.1/gtest_gui/main.py
--rw-r--r--   0 tom      (31978) tom       (2000)     5357 2023-04-22 05:49:45.000000 mote-gtest-gui-0.8.1/gtest_gui/test_db.py
--rw-r--r--   0 tom      (31978) tom       (2000)     8434 2023-04-22 05:44:31.000000 mote-gtest-gui-0.8.1/gtest_gui/tk_utils.py
--rw-r--r--   0 tom      (31978) tom       (2000)    13123 2023-04-23 09:13:02.000000 mote-gtest-gui-0.8.1/gtest_gui/tool_tip_db.py
--rw-r--r--   0 tom      (31978) tom       (2000)     3594 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.1/gtest_gui/wid_status_line.py
--rw-r--r--   0 tom      (31978) tom       (2000)    35236 2023-04-24 18:30:17.000000 mote-gtest-gui-0.8.1/gtest_gui/wid_test_ctrl.py
--rw-r--r--   0 tom      (31978) tom       (2000)    31652 2023-04-24 18:50:48.000000 mote-gtest-gui-0.8.1/gtest_gui/wid_test_log.py
--rw-r--r--   0 tom      (31978) tom       (2000)    21045 2023-03-22 18:17:17.000000 mote-gtest-gui-0.8.1/gtest_gui/wid_text_sel.py
--rw-r--r--   0 tom      (31978) tom       (2000)     6032 2023-04-16 09:19:33.000000 mote-gtest-gui-0.8.1/gtest_gui/wid_tool_tip.py
-drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-04-24 19:08:38.035321 mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/
--rw-r--r--   0 tom      (31978) tom       (2000)    28541 2023-04-24 19:08:37.000000 mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/PKG-INFO
--rw-r--r--   0 tom      (31978) tom       (2000)      834 2023-04-24 19:08:37.000000 mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/SOURCES.txt
--rw-r--r--   0 tom      (31978) tom       (2000)        1 2023-04-24 19:08:37.000000 mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/dependency_links.txt
--rw-r--r--   0 tom      (31978) tom       (2000)        8 2023-04-24 19:08:37.000000 mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/requires.txt
--rw-r--r--   0 tom      (31978) tom       (2000)       10 2023-04-24 19:08:37.000000 mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/top_level.txt
--rw-r--r--   0 tom      (31978) tom       (2000)       38 2023-04-24 19:08:38.035321 mote-gtest-gui-0.8.1/setup.cfg
--rwxr-xr-x   0 tom      (31978) tom       (2000)     1538 2023-04-24 18:51:56.000000 mote-gtest-gui-0.8.1/setup.py
+drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-06-08 19:35:59.686571 mote-gtest-gui-0.9.0/
+-rw-r--r--   0 tom      (31978) tom       (2000)    35149 2023-03-12 12:42:14.000000 mote-gtest-gui-0.9.0/LICENSE
+-rw-r--r--   0 tom      (31978) tom       (2000)      110 2023-04-23 09:14:13.000000 mote-gtest-gui-0.9.0/MANIFEST.in
+-rw-r--r--   0 tom      (31978) tom       (2000)    39132 2023-06-08 19:35:59.686571 mote-gtest-gui-0.9.0/PKG-INFO
+-rw-r--r--   0 tom      (31978) tom       (2000)     5004 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/README.md
+-rw-r--r--   0 tom      (31978) tom       (2000)     3263 2023-06-01 03:46:57.000000 mote-gtest-gui-0.9.0/TODO.txt
+drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-06-08 19:35:59.678571 mote-gtest-gui-0.9.0/bin/
+-rwxr-xr-x   0 tom      (31978) tom       (2000)     1280 2023-04-23 09:14:13.000000 mote-gtest-gui-0.9.0/bin/gtest_gui
+drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-06-08 19:35:59.682571 mote-gtest-gui-0.9.0/gtest_gui/
+-rw-r--r--   0 tom      (31978) tom       (2000)       22 2023-03-21 18:15:59.000000 mote-gtest-gui-0.9.0/gtest_gui/__init__.py
+-rw-r--r--   0 tom      (31978) tom       (2000)       80 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/__main__.py
+-rw-r--r--   0 tom      (31978) tom       (2000)      724 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/bisect.py
+-rwxr-xr-x   0 tom      (31978) tom       (2000)    14525 2023-06-01 04:35:53.000000 mote-gtest-gui-0.9.0/gtest_gui/config_db.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    15329 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/dlg_browser.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    11284 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/dlg_config.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     9194 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/dlg_debug.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     8614 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/dlg_font_sel.py
+-rwxr-xr-x   0 tom      (31978) tom       (2000)    11836 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/dlg_help.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    10196 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/dlg_job_list.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    18361 2023-06-08 15:59:51.000000 mote-gtest-gui-0.9.0/gtest_gui/dlg_main.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    21839 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/dlg_tc_list.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     2684 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/fcntl.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    15218 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/filter_expr.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    30448 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/gtest_ctrl.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     3159 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/gtest_list_tests.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     7241 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/gtest_sharding.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    45586 2023-06-01 03:43:58.000000 mote-gtest-gui-0.9.0/gtest_gui/help_db.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     4858 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/main.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     8247 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/test_db.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    12404 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/tk_utils.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    15336 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/tool_tip_db.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    10562 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/trace_db.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     4787 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/wid_status_line.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    38569 2023-06-01 03:45:55.000000 mote-gtest-gui-0.9.0/gtest_gui/wid_test_ctrl.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    37415 2023-06-01 02:49:48.000000 mote-gtest-gui-0.9.0/gtest_gui/wid_test_log.py
+-rw-r--r--   0 tom      (31978) tom       (2000)    22455 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/wid_text_sel.py
+-rw-r--r--   0 tom      (31978) tom       (2000)     9707 2023-06-01 00:21:49.000000 mote-gtest-gui-0.9.0/gtest_gui/wid_tool_tip.py
+drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-06-08 19:35:59.686571 mote-gtest-gui-0.9.0/mote_gtest_gui.egg-info/
+-rw-r--r--   0 tom      (31978) tom       (2000)    39132 2023-06-08 19:35:59.000000 mote-gtest-gui-0.9.0/mote_gtest_gui.egg-info/PKG-INFO
+-rw-r--r--   0 tom      (31978) tom       (2000)      919 2023-06-08 19:35:59.000000 mote-gtest-gui-0.9.0/mote_gtest_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 tom      (31978) tom       (2000)        1 2023-06-08 19:35:59.000000 mote-gtest-gui-0.9.0/mote_gtest_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 tom      (31978) tom       (2000)       49 2023-06-08 19:35:59.000000 mote-gtest-gui-0.9.0/mote_gtest_gui.egg-info/requires.txt
+-rw-r--r--   0 tom      (31978) tom       (2000)       10 2023-06-08 19:35:59.000000 mote-gtest-gui-0.9.0/mote_gtest_gui.egg-info/top_level.txt
+-rw-r--r--   0 tom      (31978) tom       (2000)       38 2023-06-08 19:35:59.686571 mote-gtest-gui-0.9.0/setup.cfg
+-rwxr-xr-x   0 tom      (31978) tom       (2000)     1600 2023-06-08 15:59:51.000000 mote-gtest-gui-0.9.0/setup.py
```

### Comparing `mote-gtest-gui-0.8.1/LICENSE` & `mote-gtest-gui-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.1/PKG-INFO` & `mote-gtest-gui-0.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mote-gtest-gui
-Version: 0.8.1
+Version: 0.9.0
 Summary: Module tester's Gtest GUI is a full-featured graphical user-interface to C++ test applications using the GoogleTest framework.
 Home-page: https://github.com/tomzox/gtest_gui
 Author: T. Zoerner
 Author-email: tomzox@gmail.com
 License: UNKNOWN
 Keywords: google-test,gtest,testing-tools,test-runners,tkinter,GUI
 Platform: posix
@@ -23,40 +23,53 @@
 
 Module-Tester's Gtest GUI
 =========================
 
 Description
 -----------
 
-**Module-tester's GtestGui** is a full-featured graphical user-interface to C++ test applications using the GoogleTest framework.
+**Module-tester's GtestGui** is a test-runner with graphical user-interface for C++ test applications using the GoogleTest framework.
 
-The tool will work with any application with Gtest command line interface, however it is designed especially for C++ developers using test-driven design based on module testing and integration testing. These differ from unit-testing by longer execution times and usually not fully predictable results, which in turn require multiple repetitions of each test case. To support this well, GtestGui offers firstly easily accessible ways for test case filtering and concurrent scheduling across multiple CPUs; Secondly, there are multiple features for tracking progress and managing results via sorting and filtering, which are fully usable already while a test campaign still is in progress.
+GtestGui will work with any application that implements the Gtest command line interface, however it is designed especially for C++ developers using test-driven design based on module testing and integration testing. These differ from unit-testing by longer execution times and usually not fully predictable results (i.e. "flakiness"), which in turn require multiple repetitions of each test case. To support this well, GtestGui offers firstly easily accessible ways for test case filtering and concurrent scheduling across multiple CPUs; Secondly, there are multiple features for tracking progress and managing results via sorting and filtering, which are fully usable already while a test campaign still is in progress.
 
 GtestGui typically is started with the path of an executable on the command line which is built using the gtest library. Using the "Run" button in the GUI, this executable can then be started and its progress be monitored live in the result log frame of the main window. Additional controls allow specifying options such as test case filter string and repetition count, which are forwarded to the executable via the respective "\ ``--gtest_*``" command line arguments.
 
 While tests are running, test verdicts can be monitored live in the result log. Traces of passed or failed tests can already be analyzed simply by double-clicking on an entry in the result log, which will open the trace of that particular test case run. For this purpose GtestGui comes bundled with *Trowser*, which is a graphical browser for large line-oriented text files. Trowser in principle is just a text browser with syntax highlighting and search, but its search capabilities are designed especially to facilitate analysis of complex debug logs, essentially by allowing to build a condensed (filtered) view of the trace file in the search result window via incremental searches and manual manipulations. By default, GtestGui is configured to user *trowser.py*, but there is also a more modern-looking Qt5 variant. GtestGui can also be configured to use any other GUI application for opening traces.
 
 Test control
 ------------
 
 The application main window consists of a menu bar, a frame containing test controls, a frame containing the test result log, and a text frame for trace preview. This chapter describes the top-most frame with the test controls.
 
+Executable selection
+~~~~~~~~~~~~~~~~~~~~
+
+Before tests can be started or a test filter be defined, a target executable has to be selected. If the executable file was not already specified on the command line, then this is done via *Select executable file...* in the *Control* menu. Either select a file via the file selector dialog, or choose one from the list of previously used executables. (Note when hovering the mouse over enries in this list, the full path and timestamp of the file is displayed as tool-tip. The entry is grayed out if the file no longer exists.)
+
+Upon selecting an executable file, the test case list is read automatocally by running it with the "\ ``--gtest_list_tests``" command line option. If that fails with an error, or if the list is empty, executable selection is aborted.
+
+Whenever starting a new test campaign, GtestGui will automatically check if a new executable version is available by checking the file timestamp. If a change is detected, the test case list is read again. The *Refresh test case list* command in the menu allows performing the same steps independently. That command is useful if you want to specify newly added test case names in the test case filter string before starting a new test campaign (maybe to only run the new test cases.)
+
+Results of the previous executable are kept in the result log window, but the log entries are updated to include the executable name. Repeating test cases of other executables via the *Repeat* button is not possible; You have to manually switch back to the respective executable to allow that.
+
+The executable cannot be "refreshed" or switched while a test campaign is running.
+
 Test campaign control buttons
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Most prominent in the test control frame are the green buttons, which directly control execution of the configured executable file:
+Most prominent in the test control frame are the green buttons, which directly control execution of the configured executable file. The same commands are also in the "Control" menu:
 
 *Run*:
   Starts the text executable in a separate process, with its output redirected into a pipe which is read by GtestGui for progress monitoring. The output is also saved into a file.
 
-  Note when the timestamp of the executable file on disk has changed, GtestGui automatically reads the test case list to check for changes. An error will be reported if the current test case filter contains pattern that no longer match any test case. Note after adding a new test case, use the *Refresh test case list* command in the *Control* menu to read the test case list, for allowing to use the new test case name in a filter pattern.
+  Note when the timestamp of the executable file on disk has changed, GtestGui automatically reads the test case list to check for changes. An error will be reported if the current test case filter contains pattern that no longer match any test case. If the timestamp has not changed, the age of the file is shown in a status message below the buttons, to warn you about this in case you forget to build the executable after making changes.
 
   Multiple processes are started if the *CPUs* value is larger than 1. Most of the time, GtestGui will use gtest's "sharding" feature, which assigns a static sub-set of tests to each process. However, if repetition count is larger than one and the number of configured CPUs is larger than the number of test cases, or if the remainder of division of test cases by CPUs is large, GtestGui may instead or additionally partition by repetitions.
 
-  Note when a test process crashes, it is currently not restarted. That is because gtest's static sharding does not allow disabling the instable test case without influencing test case partitioning.
+  Note when a test process crashes during a campaign, it is currently not restarted. That is because gtest's static sharding does not allow disabling the instable test case without influencing test case partitioning.
 
 *Stop*:
   Sends a TERM signal to the test processes and waits for them to finish. When termination takes a long time (possibly because the executable is hung) and the button is clicked a second time, a KILL signal is sent.
 
 *Resume*:
   Restarts test case execution using the same test case filter setting and executable version as previously used, without resetting the test result statistics. Other options, such as repetition or CPU count may be modified. This operation is useful when a long test run has to be paused temporarily as the CPUs are needed otherwise, or for changing options such as the number of used CPUs.
 
@@ -72,14 +85,16 @@
 
 The entry field at the top of the test control frame allows specifying a test case filter, so that only a matching sub-set of test cases is run. The filter can be entered manually using the same syntax as the "\ ``--gtest-filter``" command line option: The format of a filter expression is a ":"-separated list of test case names of wildcard patterns (positive patterns), optionally followed by a "-" and another ":"-separated pattern list (negative patterns). A test matches the filter if and only if it matches any of the positive patterns, but none of the negative ones. Wildcard characters are "*" (matching any sub-string) and "?" (matching any single character). As a special case, when no positive pattern is specified, all test cases are considered matching.
 
 Alternatively, the test case filter can be modified via the drop-down menu below the entry field (which can be opened by the Cursor-Down key or a click on the drop-down button next to the entry field). The menu has entries for selecting and deselecting entries test suites as well as individual test cases. When modifying the filter this way, GtestGui will update the entry field with the shortest filter expression it can find using trailing wild card and negative patterns.
 
 Yet another alternative for modifying test case filters is the test case list dialog, either via its context menu or the "Return" and "Delete" key bindings. Finally note any modification to the test case filter can be undone using "Control-Z" key binding in the entry field, or redone using "Control-Y" key binding.
 
+After renaming a test case or adding a new test case, use the *Refresh test case list* command in the *Control* menu to read the test case list from the executable file. Afterward the new test case names can be used in the filter string.
+
 Test control options
 ~~~~~~~~~~~~~~~~~~~~
 
 *Repetitions*:
   If a value larger than 1 is entered here, it is passed via the "\ ``--gtest_repeat=NNN``" option on the executable's command line. This causes each test case to be repeated the given number of times.
 
 *CPUs*:
@@ -118,14 +133,34 @@
   When enabled, "\ ``--gtest_catch_exceptions=0``" option is set via the executable's command line. This will disable catching of exceptions by the Gtest framework, which means any exception not caught by the test case itself causes the test process to crash due to an unhandled exception.
 
   When core dumps are enabled in the kernel, the core will be saved by GtestGui and can be analyzed via the *Extract stack trace from core dump* command in the result log's context menu. When core dumps are not enabled, this option is probably not useful.
 
 *Valgrind* and *Valgrind - 2nd option set*:
   The two valgrind options serve to run each execution of the test executable under valgrind using the configured command line. Notably, valgrind checks are performed across the complete lifetime of the test process, thus spanning all test cases or test repetitions. Therefore, if for example a memory leak is reported at the end, it cannot be determined which test case caused it (or it may even be caused by interaction of the test sequence.) Therefore valgrind errors are reported with a special entry in the result log. Some kind of errors such as invalid memory accesses can be mapped to test cases based on the position of the error report in the output stream. Note however that the position may not exactly reflect the timing of occurrence due to possible buffering in output streams within the test executable.) See `Result log`_ and `Configuration`_ for more details.
 
+Status and progress monitoring
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The lower left part of the test control frame shows the status of the latest test campaign. The left box with label "Status" shows three numbers with the following meaning:
+
+*Running*:
+  Shows the number of test processes currently executing test cases. (See `Caveats`_ for an explanation why this number may be lower than the number of requested "CPUs".)
+
+*Passed*:
+  Shows the number of test cases that were passed or skipped.
+
+*Failed*:
+  Shows the number of test cases that failed or crashed. The number also includes a possible additional fail verdict by valgrind at the end of a test process.
+
+The left box with label "Progress" shows the completion ratio in form of a progress bar. The ratio is calculated as the number of received results (i.e. passed, skipped, failed, or crashed) divided by the number of expected results. The number of expected results is the number of test cases selected by the test case filter, multiplied with the repetition count.
+
+In case the *Ignore filter* option in `Test control options`_ is set to a non-zero value, completion ratio of the respective test jobs is disregarded for the progress display, as these jobs are terminated automatically once the regular test jobs have completed. Note the "Status" frame however does include results received from these jobs, so that the numbers shown there may exceed the configured repetition count for tests matching the test case filter.
+
+When hovering the mouse over the progress bar, a tool-tip text shows additional details about the progress, namely the ratio of completed test cases and repetitions and estimated remaining run time.
+
 Result log
 ----------
 
 The result log frame is located in the middle of the main window. When started for the first time, the log is usually empty. However, results can also be imported via the command line, for example from a file that contains output from a test executable that was redirected into a file. The result log may also show results from a previous run of GtestGui, if auto-import is enabled in `Configuration`_.
 
 The result log contains one line for each ``[ OK ]``, ``[ SKIPPED ]`` and ``[ FAILED ]`` line in the test application's gtest-generated output. The test executable's output stream is redirected to a pipe that is read continuously by GtestGui for this purpose. GtestGui also stores this output to a file, so that the trace output between ``[ RUN ]`` and verdict text line can be opened in a trace browser.
 
@@ -147,19 +182,66 @@
 
 -   In case of failure, source code file and line where of the first "Failure" was reported in trace output.
 
 -   Timestamp or name of executable that generated the test output, in case the executable has changed since running the test.
 
 When selecting an entry by clicking on it, the corresponding trace output is shown in the trace preview frame below the result log. In case of a test case failure, the view is centered on the first line containing "Failure" and the text is marked by light red background.
 
-When clicking on an entry with the right mouse button, a context menu opens that allow opening the trace file, adding or removing the selected test case from the filter option, scheduling a test for repetition, excluding a result from the log display, or removing results.
+Double-clicking on an entry opens the trace of that entry in an external application, which can be selected via the Configuration dialog. Default application is "trace browser", a text browser with syntax highlighting and search and filtering capabilities especially tailored for trace analysis. As GTest writes trace output of all test cases into a single file, only the portion between "\ ``[ RUN ]``" and "\ ``[ OK ]``" or "\ ``[ FAILED ]``" respectively of the selected test case is extracted and passed to the application.
+
+When clicking on an entry with the right mouse button, a context menu opens that allow opening the trace file, adding or removing the selected test case from the filter option, scheduling a test for repetition, excluding a result from the log display, or removing results. The context menu also has an entry for sending the complete trace file to the external trace browser application; This may be needed in rare cases when behavior of a test case depends on the sequence of preceding tests.
+
+Additional commands are offered in the "Result log" drop-down of the main window menu. The commands allow sorting and filtering the result log by various criteria. By default, log entries are sorted by the time they were created at. When running a test campaign, it's recommended to enabled the *Show only failed* filter, so that it's easy to track which test cases failed.
+
+While a test campaign is running, new result entries are added at the bottom (when in default sort order) and the view is scrolled automatically to keep the added entry visible. This auto-scrolling can be stopped by selecting any entry in the list. To return to auto-scrolling, deselect the last entry either by clicking on it while holding the *Control* key, or by clicking in the empty line at the end of the list.
+
+Result entries can be deleted using the context menu or by pressing the *Delete* key. To delete all entries, press *Control-A* (i.e. select complete list) and then *Delete*. Note actual trace files are removed from disk only if all test case results stored in it have been deleted from the log.
 
-Additional commands are offered in the "Result log" drop-down of the main window menu. The commands allow sorting and filtering the result log by various criteria.
+Post-mortem core dump analysis
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-On UNIX platform, the context menu additionally supports extracting a thread overview and stack-trace (backtrace) of each thread from a core dump in case of a crash during execution of a test case. To allow this, ``/proc/sys/kernel/core_pattern`` needs to be configured as "\ ``core.%p``", or alternatively as "\ ``core``", when additionally ``/proc/sys/kernel/core_uses_pid`` is set to "1". If GtestGui thus finds a file named "core.PID" with PID matching that of the test executable process after a process crashed, it will automatically preserve that core file for analysis by renaming it and moving it into the directory where trace text output files are stored. It will also preserve the executable file version by keeping a hard link to the same executable.
+POSIX platforms only: When selecting the result of a test case that caused a crash of the test process, the context menu has an entry that allows analyzing the generated core dump file. The Analysis consists of a thread overview and stack-trace (backtrace) of each thread. This allows finding quickly at which test step the crash occurred.
+
+To allow this, ``/proc/sys/kernel/core_pattern`` needs to be configured as "\ ``core.%p``", or alternatively as "\ ``core``", when additionally ``/proc/sys/kernel/core_uses_pid`` is set to "1". This way, a file named "\ ``core.PID``" will be created by the operating system in the directory where GtestGui was started.
+
+If GtestGui thus finds a core file with a matching process ID after a process crashed, it will automatically preserve that core file for analysis by moving it into the directory where trace text output files are stored and renaming it to the same name of the corresponding trace file with prefix "core". It will also preserve the executable file version by keeping a hard link to the same executable in the trace directory for as long as the core file exists.
+
+Test case list dialog
+---------------------
+
+A dialog showing the list of test cases read from the selected executable file can be opened via the control menu.
+
+For each test case, the list shows in the first column if the test case is currently enabled for execution, the test case name, the number of times it has passed and failed in the current campaign and its accumulated execution time.
+
+By default, test cases in the list are in the order as received. The list can be sorted in different ways using the context menu: The list can be sorted alpabetically, by execution or failure count within the current test campaign, or by test case execution duration.
+
+By default, all test cases defined in the executable are listed. You can filter the list via the context menu to show only test cases enabled via test case filter in the main window, or only test cases that failed in the current test campaign, or only test cases whose name or test suite namedoesn't start with "\ ``DISABLED_``".
+
+The "Run" column is updated to reflect changes in the "Test filter" entry field in the main window. Updates occur when you press the "Return" key, or when keyboard focus is moved out of the entry field. When the "Show only tests enabled to run" filter is active in the test case list dialog, the test case sub-set shown in the list is also updated to match the current filter string. This feature can be used for testing the manually entered filter string against the list, as you'll see exactly which test cases it selects.
+
+Inversely, you can use the list for modifying the test case filter in the main window: This can be done via the *Add/Remove selected test case* and *Add/Remove selected test suite* commands in the list's context menu. The latter works on all test cases in the test suite of the selected test case. The same can be achive via key bindings: *Return* adds selected test cases and *Del* removes selected test cases. Note for selecting multiple lines in the list via keyboard, hold the *Shift* button while moving the cursor via the Up/Down keys.
+
+Test cases named "\ ``DISABLED_``" can only be enabled via the test case list commands when option *Run disabled tests* in the main window is checked.
+
+Note while the filter string is empty, all test cases are considered as enabled.  Nevertheless, the context menu will offer adding selected test cases. If you do so, then implictly all test cases except for the one added by the command get disabled.
+
+After making changes to the test case filter via the dialog, the filter string in the main window is updated automatically to reflect the selection. The filter uses wildcards to minimize the filter string length.
+
+Job list dialog
+---------------
+
+A dialog window showing the status of test processes in a currently ongoing test campaign can be opened via the *Open job list* command in the control menu. If no test campaign is active, it will only show a message informing that currently no processes are running.
+
+During an ongoing test campaign, the list shows for each process its ID assigned by the operating system ("PID"), if it is a background job ("BgJob"), the number of bytes of trace output received from it ("Traced"), the number of test case results found in received trace ("Results"), the percentage of completed results from expected results ("Done"), and finally the name of the current test case reported via "\ ``[ RUN ]``" in received trace.
+
+Note a "background job" is one for which the test case filter is ignored as per *Ignore filter* option in `Test control options`_. These jobs are special as they are terminated automatically when the last regular job is completed. For this reason their completion ratio (i.e. "Done" column) is disregarded for progress display in the main window.
+
+The dialog is useful in case you suspect that a test campaign may be hung (for example when a test case ran into a deadlock or busy loop.) You could notice that firstly by the number of results not increasing and if that's the case, by the number of received bytes received as trace output not increasing. (The latter will however not if your test cases generate few or no trace output.)
+
+The context menu allows sending an *ABORT* signal to the process, which will terminate it and cause a core image to be dumped on UNIX. The test case will be reported as crashed in the result log. This can be used for debugging a hung process: You can find where it was hung by using the *Extract stack trace from core dump* command in context menu of the result log entry. Alternatively, you could use the PID for attaching a debugger to the live process (e.g. "\ ``gdb -p PID exe_file``").
 
 Configuration
 -------------
 
 User-interface options
 ~~~~~~~~~~~~~~~~~~~~~~
 
@@ -176,14 +258,16 @@
 
 *Show tool-tip popups*:
   The option can be unchecked to disable display of "tool-tip" popup windows when hovering with the mouse on labels or check-buttons in the main window and dialogs which have such built-in help. Changes of the option are stored in the configuration file, so that it is persistent. This may be useful once you are sufficiently familiar with the tool.
 
 Test management options
 ~~~~~~~~~~~~~~~~~~~~~~~
 
+The following configuration options are available in the *Options* dialog window that can be opened via the *Configure* menu:
+
 *Trace browser*
   This entry field selects the external application used for displaying trace files and trace snippets, when double-clicking on an entry in the result log. By default, trace browser *trowser.py* is used. You can either specify just the application file name, or its full path if it is not found via ``PATH`` configured in environment. The path of the trace file to be displayed will be appended to the given command line.
 
   Currently the application path name or parameters cannot contain space characters, as these are assumed to be separators.
 
   Note for the Windows platform: When using the default of ``trowser.py``, you may need to insert the Python interpreter in front of "trowser.py", depending on your Python installation. In that case you need to add the full path to where ``trowser.py`` is installed.
 
@@ -218,19 +302,19 @@
 
 Caveats
 -------
 
 This chapter lists notable limitations that are not easy to overcome due to design choices.
 
 Concurrent scheduling
-  Concurrent scheduling requested via option *CPUs* is based on the "sharding" feature provided by Gtest framework. Unfortunately, Gtest only supports static case test partitioning, which means for example when using two CPUs, the set of test cases is split in two parts, of which the first is executed in one test process and the second in the second process.
+  Concurrent scheduling requested via option *CPUs* is based on the "sharding" feature provided by Gtest framework. Unfortunately, Gtest only supports static case test partitioning, which means for example when using two CPUs, the set of test cases is split in two parts, of which the first is executed in one test process and the second in the other process.
 
-  One problem arises when the number of test cases is smaller than the number of CPUs. This typically occurs, when trying to run a single test case many times. Sharding would then only use a single CPU, as it does not consider repetitions in its "sharding" algorithm. GtestGui works around that by calculating if it is more efficient to partition test cases by repetition than by sharding, or if a combination of both is even better. In the mentioned example, it would not use sharding, but instead run half the number of repetitions in one process, and the second half in the second. For more complex configurations such as 10 repetitions of 9 test cases on 8 CPUs, a combination of both methods will be used.
+  One problem arises when the number of test cases is smaller than the number of requested CPUs. This typically occurs when trying to run a single test case many times.  Sharding would then only use a single CPU, as it does not consider repetitions in its "sharding" algorithm. GtestGui works around that by calculating if it is more efficient to partition test cases by repetition than by sharding, or if a combination of both is even better. In the mentioned example, it would not use sharding, but instead run half the number of repetitions in one process, and the second half in the second. For more complex configurations such as 10 repetitions of 9 test cases on 8 CPUs, a combination of both methods will be used.
 
-  A second problem that GtestGui cannot work around occurs when test cases have non-uniform execution time. As the "sharding" algorithm uses static partitioning solely based on the number of test cases per process, differences in execution times are not considered. For example, when two tests are scheduled for 100 times and test case A takes 1 second, but test case B only 1 millisecond, Gtest will still schedule all runs of A in the first process and all runs of B in the second process. Thus, the second process will sit idle for 99.9% of the total test execution time.
+  A second problem, that GtestGui cannot work around, occurs when test cases have non-uniform execution time. As the "sharding" algorithm uses static partitioning solely based on the number of test cases per process, differences in execution times are not considered. For example, when two tests are scheduled for 100 times and test case A takes 1 second, but test case B only 1 millisecond, Gtest will still schedule all runs of A in the first process and all runs of B in the second process. Thus, the second process will sit idle for 99.9% of the total test execution time.
 
 Test case crashes
   In a well-behaved test application, failures are normally reported via Gtest macros or exceptions. Thus, the failure is recorded and the next test case is executed. Sometimes however, a test case may have a bug that leads to a crash of the complete process. In this case all following test cases or test case repetitions are no longer executed.
 
   Currently GtestGui will not attempt to restart tests after a crash, because it expects that the same test case will crash again and thus keep blocking following tests. It is not possible to disable the instable test, as this would interfere with partitioning by Gtest "sharding", i.e. the set of test cases run by that test case would be altered. The only way around is for the use to manually disable the instable test case and then restart the test campaign.
 
 Overload of GUI by concurrent unit-testing
```

### Comparing `mote-gtest-gui-0.8.1/README.md` & `mote-gtest-gui-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 # GtestGui
 
-GtestGui is a full-featured graphical user-interface to test applications using
-the [GoogleTest framework](https://google.github.io/googletest/).
+GtestGui is a test-runner with graphical user-interface for test applications
+using the [GoogleTest framework](https://google.github.io/googletest/).
 
 GtestGui was created mainly for removing the need for fiddling with Gtest
 command line options, for tracking the status of long-running test campaigns
 and for extracting individual test cases' traces from large trace output
 files.
 
 The GoogleTest framework is widely known for its C++ Unit-Testing support
 via the [GMock](https://google.github.io/googletest/reference/mocking.html)
 feature. But one can also use just the
 [test framework](https://google.github.io/googletest/reference/testing.html)
-for defining test cases, scheduling test executions, and collecting verdicts
-and thus encapsulate any kind of test cases. This saves some implementation
-effort, but more importantly also has the advantage of presenting a well-known
-common interface to developers.
+for defining test cases, scheduling test executions, and collecting verdicts.
+Even using only the framework saves some implementation effort, but more
+importantly also has the advantage of presenting a well-known common interface
+to developers.
 
 GtestGui is designed especially for component tests, integration tests and
 other higher-level testing, where the number of tests is smaller compared to
 unit-testing, but individual test cases run longer and tests may have to be run
 repeatedly (e.g. when test scenarios are not fully reproducible due to timing
-between threads.)
-
-GtestGui supports this by allowing to schedule test cases across multiple CPUs.
-For very long-running campaigns, the "clean traces of passed tests" option
-allows storing only traces of failed tests to disk. Status of ongoing tests is
-presented in form of a top-level pass/fail summary and progress bar, as well as
-a running log of test case verdicts, which can be filtered and sorted (e.g. to
-show only failed test cases.) Traces of individual test cases are accessible
-while the test campaign is still running either in a small preview window below
-the test log, or via double-click which exports them to an external trace
-browser. ([Trowser](https://github.com/tomzox/trowser) is recommended for this
-purpose.)
+between threads.) But it can also be used for unit-tests with "flakiness" (as
+the [gtest-parallel](https://github.com/google/gtest-parallel) command line
+tool calls it) which show sporadic failures and thus require high repetition
+count for proving stability.
+
+GtestGui supports this by allowing to schedule test cases concurrently across
+multiple CPUs.  For very long-running campaigns, the "clean traces of passed
+tests" option allows storing only traces of failed tests to disk. Status of
+ongoing tests is presented in form of a top-level pass/fail summary and
+progress bar, as well as a running log of test case verdicts, which can be
+filtered and sorted (e.g. to show only failed test cases.) Traces of individual
+test cases are accessible while the test campaign is still running either in a
+small preview window below the test log, or via double-click which exports them
+to an external trace browser. ([Trowser](https://github.com/tomzox/trowser) is
+recommended for this purpose.)
 
 GtestGui provides access to Gtest command line options directly from the main
 window. Most importantly, test case filters can be entered manually, or via
 drop-down menu listing all test cases, or the test case list dialog. Other
 supported options are the test repetition count, failure limit, shuffling
 execution order, running disabled tests and breaking on failure or exceptions.
 The latter will on POSIX systems produce a core dump that can be pre-analyzed
@@ -45,24 +48,21 @@
 that were found for the result log.
 
 GtestGui can also be used for analyzing pre-existing trace output files
 by adding the trace file names on the command line when starting.
 
 <IMG ALIGN="center" SRC="images/screenshot_main.png" ALT="screenshot of main window" BORDER="10" WIDTH="400" />
 
-I developed GtestGui for my daily work as a C++ software engineer. (Actually,
-it is a re-implementation of a GUI I had designed in C and Tcl/Tk for a
-self-written C test framework that predated GoogleTest, which is why I consider
-the tool mature despite the apparent young age of this most recent
-incarnation.) GtestGui supports me in initial development phases using
-test-driven development where I need to run the same sub-set of test cases over
-and over again. It supports getting a quick overview of stability across the
-complete set of tests and which kind of failures occur.  And it supports final
-quality checking in long-running, high-repetition test campaigns, optionally
-using valgrind or sanitizer builds.
+GtestGui has a mature feature set that can support C++ development in all
+development phases: During initial code construction with test-driven design,
+it supports running the same sub-set of test cases over and over again. After
+code completion, it supports getting a quick overview of stability across the
+complete set of test cases and which kind of failures occur. And it supports
+final quality checking in long-running, high-repetition test campaigns,
+optionally using valgrind or sanitizer builds.
 
 ## Installation
 
 GtestGui is available as package "mote-gtest-gui" ("Module tester's Gtest GUI")
 on [PyPi](https://pypi.org/project/mote-gtest-gui/). It can be installed using
 pip3:
 ```console
```

### Comparing `mote-gtest-gui-0.8.1/TODO.txt` & `mote-gtest-gui-0.9.0/TODO.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 General:
-- code comments
-- test suite at least for filter_expr & gtest parser
+- extend code comments
+- refactor according to remaining pylint warnings
+- test suite at least for filter_expr & gtest sharding & gtest parser
 
 gtest:
+- clean-up at shutdown: delete traces from file that were deleted from result log
 - import of trace with core: executable not linked & not cleaned upon trace removal
-- import of trace: executable file & ts is unknown:
+- import of trace: executable file & timestamp is unknown:
   Add "info" file to directory, or encode name in sub-directory path (hash);
   prerequisite: allow only one exe per directory even if timestamp equal
-- handle I/O error in trace writing
 - after crash: check if core dump is enabled, add warning to trace file
 - if /proc/sys/kernel/core_pattern pipes to apport: copy core from /var/lib/apport/coredump/
 - unit-test on many CPUs: GUI is overloaded => throttle updates of result log
 - optimize TC allocation per CPU: consider actual duration
 - restart test job after crash of a test case (problem: cannot change filter
   without affecting gtest's "sharding", i.e. CPU partitioning)
 - Repeat with the actual SEED value (not supported by gtest)
@@ -21,27 +22,29 @@
 - add menu cmd for trace import from file
 - support gtest input via socket
 - hide test_ctrl: switch status_line to wid_test_log
 
 wid_test_ctrl:
 - enhance popup_test_list for case that there's single test suite
 - option to make tc filter-string case-independent? (problem: gtest compatibility)
-- win32: hide core & valgrind options
+- remote control for campaign start/stop for use in IDE build
 
 wid_test_log:
 - menu for result mgmt: remove selected, all old passed, all filtered;
 - when removing traces: rewrite trace files to actually remove text?
+  problem: cannot be done while test campaign is running for that file
   OR: new command for "compressing" trace files
 - add key binding for toggling repetition mark on selected test cases
 - allow adding bookmark / attaching note to result log entries
 
 dlg_browser:
 - trowser command argv: use shell if cmd contains space or special chars; check if escape needed
   or add config option
 - export trace files in other archive formats, or uncompressed to directory
+- make gdb command used for core dump analysis configurable
 
 dlg_config:
 - extend option for cleaning trace upon exit: Radiobutton all/failed-only/ask
 - add option: Save test control settings when quitting?
 - add option: Reg.exp. for extracting failure line
   requires to parse all traces after changing expression to update file/line of exception
 - upon window close: ask for saving pending changes
@@ -56,13 +59,14 @@
 - add footer containing sums: #test cases, total pass/fail, exec time, #enabled
 - folding: show test suite names only (possibly controllable individually?)
 - add column showing skip count
 - enable sort via click in column head / via ctx menu
 - entry field for filtering by name
 
 dlg_job_list:
+- keep completed processes during the active campaign to see if done or crashed
 - use mclistbox (multi-column listbox, available in Tcl/Tk)
 - allow sending KILL signal to job
 - show %CPU read via /proc (Linux only)
 
 dlg_help:
 - text search
```

### Comparing `mote-gtest-gui-0.8.1/bin/gtest_gui` & `mote-gtest-gui-0.9.0/bin/gtest_gui`

 * *Files identical despite different names*

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/config_db.py` & `mote-gtest-gui-0.9.0/gtest_gui/config_db.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,78 +13,162 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
+"""
+Database and persistent storage for configuration parameters. Parameters are
+read from a file into memory once during start-up. Various modules access the
+database when needed using getters. Updates are done via setters and
+automatically trigger an update of the configuration file after a short delay
+timer (for combining multiple consecutive changes), or at latest upon shutdown.
+The module does not provide notifications about configuration parameter changes.
+"""
+
 import errno
 from datetime import datetime
 import json
 import os
 import re
 import sys
 import tempfile
+import tkinter as tk
 from tkinter import messagebox as tk_messagebox
 
 import gtest_gui.tk_utils as tk_utils
 
-# Options set via configuration menu
+# Module "appdirs" is required on Windows to learn the directory where to store
+# application configuration files. Install the module via "pip3 install appdirs"
+# if the import fails. (Alternatively, you could replace the one function call
+# into the module with a hard-coded path.)
+if sys.platform == "win32":
+    import appdirs
+
+#
+# Database of configuration options and other persistent state to be written to
+# the configuration file. Default values assigned here are overridden when
+# loading the configuration file. Therefore they are only used when a user starts
+# the application for the first time after installation.
+#
 options = {
-    "browser": "trowser.py",
+    # Options set via configuration menu
+    "log_browser": "trowser.py",
     "browser_stdin": True,
     "seed_regexp": "",
     "trace_dir": "",
     "exit_clean_trace": True,
     "startup_import_trace": True,
     "copy_executable": True,
-    "valgrind1": "valgrind --leak-check=full --show-leak-kinds=definite,possible,indirect --show-reachable=yes --num-callers=50",
-    "valgrind2": "valgrind --leak-check=full --show-leak-kinds=definite,possible,indirect --expensive-definedness-checks=yes --show-reachable=yes --num-callers=50 --track-origins=yes",
+    "cmd_valgrind1": "valgrind --leak-check=full "
+                     "--show-leak-kinds=definite,possible,indirect "
+                     "--show-reachable=yes --num-callers=50",
+    "cmd_valgrind2": "valgrind --leak-check=full "
+                     "--show-leak-kinds=definite,possible,indirect "
+                     "--show-reachable=yes --num-callers=50 "
+                     "--track-origins=yes --expensive-definedness-checks=yes",
     "valgrind_exit": True,
     "enable_tool_tips": True,
-}
 
-# Parameters of main window
-prev_exe_file_list = []
-
-# Parameters of wid_test_log
-log_pane_height = 0
-log_pane_solo_height = 0
-trace_pane_height = 0
-trace_pane_solo_height = 0
-
-# Parameters of misc. dialogs
-tc_list_geometry = ""
-job_list_geometry = ""
-help_win_geometry = ""
+    # Parameters of class TextLogWidget
+    "log_pane_height": 0,
+    "log_pane_solo_height": 0,
+    "trace_pane_height": 0,
+    "trace_pane_solo_height": 0,
+
+    # Parameters of misc. dialog classes
+    "tc_list_geometry": "",
+    "job_list_geometry": "",
+    "help_win_geometry": "",
 
+    # Parameters of class MainWindow
+    "prev_exe_file_list": [],
+}
 
 # internal state
 tid_update_rc_sec = None
 tid_update_rc_min = None
 
 # "compat" := oldest version of gtest_gui that can parse this file
-rcfile_compat = 0x01000000
-rcfile_version = 0x01000003
-rcfile_error = 0
+RCFILE_COMPAT = 0x01000000
+RCFILE_VERSION = 0x01000003
+rcfile_name_appendix = ""
+rcfile_error = False
+
+
+def get_opt(name):
+    """ Return the configured value for the named option. """
+    return options[name]
+
+
+def set_opt(name, value):
+    """
+    Update the configuration value for the named option in memory and RC file.
+    File update is delayed a few seconds for bundling updates after consecutive
+    configuration changes.
+    """
+    if options[name] != value:
+        options[name] = value
+        __rc_file_update_after_idle()
 
 
 def update_prev_exe_file_list(path):
-    global prev_exe_file_list
-
+    """
+    Add the given path to the list of previously used executable files, or move
+    it to the front of the list if already in it. Afterwards update the
+    RC file to store the new list value.
+    """
     path = os.path.abspath(path)
-    if not prev_exe_file_list or prev_exe_file_list[-1] != path:
-        prev_exe_file_list = [x for x in prev_exe_file_list if x != path]
-        prev_exe_file_list.append(path)
+    prev_list = options["prev_exe_file_list"]
+    if not prev_list or prev_list[-1] != path:
+        prev_list = [x for x in prev_list if x != path]
+        prev_list.append(path)
+        options["prev_exe_file_list"] = prev_list
+
+        __rc_file_update_after_idle()
+
+
+def update_fonts():
+    """
+    Trigger update of the RC file after a font configuration change. The font
+    options are retrieved dynamically during the update.
+    """
+    __rc_file_update_after_idle()
+
+
+def __load_rc_value(var, val, font_opts):
+    result = True
+
+    if var in options:
+        options[var] = val
+
+    elif var == "font_content":
+        font_opts[0] = val
+    elif var == "font_trace":
+        font_opts[1] = val
+
+    else:
+        result = False
+
+    return result
 
-        rc_file_update_after_idle()
 
+def __write_rc_values(rcfile):
+    # dump configuration options
+    for var in options:
+        print(var + "=" + json.dumps(options[var]), file=rcfile)
 
-def get_rc_file_path():
-    if (os.name == "posix"):
+    # dump font selection
+    print("font_content=", json.dumps(tk_utils.font_content.configure()), file=rcfile)
+    print("font_trace=", json.dumps(tk_utils.font_trace.configure()), file=rcfile)
+
+
+def __get_rc_file_path():
+    if os.name == "posix":
         xdg_config_home = os.environ.get("XDG_CONFIG_HOME")
         home = os.path.expanduser("~")
 
         if xdg_config_home is not None and os.path.exists(xdg_config_home):
             rc_file = os.path.join(xdg_config_home, "gtest_gui", "gtest_gui.rc")
 
         elif home is not None and os.path.exists(home):
@@ -93,234 +177,210 @@
                 rc_file = os.path.join(home, ".config", "gtest_gui", "gtest_gui.rc")
             else:
                 rc_file = os.path.join(home, ".gtest_gui.rc")
 
         else:
             rc_file = "gtest_gui.rc"
 
+        rc_file += rcfile_name_appendix
+
         os.makedirs(os.path.dirname(rc_file), exist_ok=True)
 
     else:
-        # TODO
-        rc_file = "gtest_gui.ini"
+        # Query system library for the common path for application configuration.
+        # e.g. on Win10: C:\Users\USERNAME\AppData\Local\GtestGui (hidden directory)
+        config_dir = appdirs.user_config_dir(appname="GtestGui", appauthor=False)
+        os.makedirs(config_dir, exist_ok=True)
+
+        rc_file = os.path.join(config_dir, "gtest_gui.rc")
 
     return rc_file
 
 
 def rc_file_load():
-    global rcfile_version
-    global log_pane_height, log_pane_solo_height
-    global trace_pane_height, trace_pane_solo_height
-    global tc_list_geometry, job_list_geometry, help_win_geometry
-    global options
-    global prev_exe_file_list
-
-    font_content_opt = None
-    font_trace_opt = None
-
+    """ Parse the configuration file and load option values into memory. """
+    font_opts = [None, None]
     error = False
-    ver_check = False
-    rc_compat_version = None
     line_no = 0
-    rc_path = get_rc_file_path()
+    rc_path = __get_rc_file_path()
+    file_version = 0
 
     try:
         with open(rc_path, "r") as rcfile:
             for line in rcfile:
                 line_no += 1
                 if re.match(r"^\s*(?:#.*)?$", line):
                     continue
 
                 match = re.match(r"^([a-z][a-z0-9_\:]*)=(.+)$", line)
                 if match:
                     var = match.group(1)
                     try:
                         val = json.loads(match.group(2))
 
-                        if   (var == "log_browser"):            options["browser"] = val
-                        elif (var == "browser_stdin"):          options["browser_stdin"] = val
-                        elif (var == "cmd_valgrind1"):          options["valgrind1"] = val
-                        elif (var == "cmd_valgrind2"):          options["valgrind2"] = val
-                        elif (var == "valgrind_exit"):          options["valgrind_exit"] = val
-                        elif (var == "seed_regexp"):            options["seed_regexp"] = val
-                        elif (var == "trace_dir"):              options["trace_dir"] = val
-                        elif (var == "exit_clean_trace"):       options["exit_clean_trace"] = val
-                        elif (var == "startup_import_trace"):   options["startup_import_trace"] = val
-                        elif (var == "copy_executable"):        options["copy_executable"] = val
-                        elif (var == "enable_tool_tips"):       options["enable_tool_tips"] = val
-
-                        elif (var == "font_content"):           font_content_opt = val
-                        elif (var == "font_trace"):             font_trace_opt = val
-                        elif (var == "prev_exe_file_list"):     prev_exe_file_list = val
-
-                        elif (var == "log_pane_height"):        log_pane_height = val
-                        elif (var == "log_pane_solo_height"):   log_pane_solo_height = val
-                        elif (var == "trace_pane_height"):      trace_pane_height = val
-                        elif (var == "trace_pane_solo_height"): trace_pane_solo_height = val
-                        elif (var == "tc_list_geometry"):       tc_list_geometry = val
-                        elif (var == "job_list_geometry"):      job_list_geometry = val
-                        elif (var == "help_win_geometry"):      help_win_geometry = val
-
-                        elif (var == "rcfile_version"):         rcfile_version = val
-                        elif (var == "rc_compat_version"):      rc_compat_version = val
-                        elif (var == "rc_timestamp"):           pass
-                        else:
-                            print("Warning: ignoring unknown keyword in rcfile line %d:" % line_no, var, file=sys.stderr)
+                        if var == "rc_compat_version":
+                            # check if the given rc file is from a newer version
+                            if val > RCFILE_VERSION:
+                                msg = "RC file '%s' is from an incompatible, " \
+                                      "newer version (%s) of this software (version %s) " \
+                                      "and cannot be loaded." \
+                                      % (rc_path, file_version if file_version > val else val,
+                                         RCFILE_VERSION)
+                                tk_messagebox.showerror(parent=tk_utils.tk_top, message=msg)
+
+                                # change name of rc file so that the newer one isn't overwritten
+                                global rcfile_name_appendix
+                                rcfile_name_appendix = "." + val
+                                # abort loading further data (would overwrite valid defaults)
+                                return
+                        elif var == "rcfile_version":
+                            file_version = val
+                        elif var == "rc_timestamp":
+                            pass
+                        elif not __load_rc_value(var, val, font_opts):
+                            print("Warning: ignoring unknown keyword in rcfile line %d:"
+                                  % line_no, var, file=sys.stderr)
 
                     except json.decoder.JSONDecodeError:
-                        tk_messagebox.showerror(parent=tk_utils.tk_top, message="Syntax error decoding rcfile line %d: %s" % (line_no, line[:40]))
+                        tk_messagebox.showerror(parent=tk_utils.tk_top,
+                                                message="Syntax error decoding rcfile line %d: %s"
+                                                % (line_no, line[:40]))
                         error = True
 
                 elif not error:
-                    tk_messagebox.showerror(parent=tk_utils.tk_top, message="Syntax error in rc file, line #%d: %s" % (line_no, line[:40]))
+                    tk_messagebox.showerror(parent=tk_utils.tk_top,
+                                            message="Syntax error in rc file, line #%d: %s"
+                                            % (line_no, line[:40]))
                     error = True
 
-                elif not ver_check:
-                    # check if the given rc file is from a newer version
-                    if rc_compat_version is not None:
-                        if rc_compat_version > rcfile_version:
-                            tk_messagebox.showerror(parent=tk_utils.tk_top,
-                                                    message="rc file '%s' is from an incompatible, "
-                                                    "newer version (%s) of this softare and cannot be loaded."
-                                                    % (rc_path, rcfile_version))
-
-                            # change name of rc file so that the newer one isn't overwritten
-                            rc_path = rc_path + "." + rcfile_version
-                            # abort loading further data (would overwrite valid defaults)
-                            return
-
-                        ver_check = True
-
-        if font_content_opt:
+        if font_opts[0]:
             try:
-                tk_utils.init_font_content(font_content_opt)
-            except Exception as e:
-                print("Error configuring content font:", str(e), file=sys.stderr)
+                tk_utils.init_font_content(font_opts[0])
+            except tk.TclError as exc:
+                print("Error configuring content font:", str(exc), file=sys.stderr)
 
-        if font_trace_opt:
+        if font_opts[1]:
             try:
-                tk_utils.init_font_trace(font_trace_opt)
-            except Exception as e:
-                print("Error configuring trace font:", str(e), file=sys.stderr)
-
-    except OSError as e:
-        if e.errno != errno.ENOENT:
-            print("Failed to load config file " + rc_path + ":", str(e), file=sys.stderr)
-
-
-def rc_file_update():
-    global rcfile_error, rcfile_compat, rcfile_version
-    global options, tid_update_rc_sec, tid_update_rc_min
-    global log_pane_height, log_pane_solo_height
-    global trace_pane_height, trace_pane_solo_height
-    global tc_list_geometry, job_list_geometry, help_win_geometry
-    global prev_exe_file_list
-
-    if tid_update_rc_sec: tk_utils.tk_top.after_cancel(tid_update_rc_sec)
-    if tid_update_rc_min: tk_utils.tk_top.after_cancel(tid_update_rc_min)
-    tid_update_rc_sec = None
-    tid_update_rc_min = None
+                tk_utils.init_font_trace(font_opts[1])
+            except tk.TclError as exc:
+                print("Error configuring trace font:", str(exc), file=sys.stderr)
+
+    except OSError as exc:
+        if exc.errno != errno.ENOENT:
+            print("Failed to load config file " + rc_path + ":", str(exc), file=sys.stderr)
 
-    rc_path = get_rc_file_path()
+
+def __rc_file_update():
+    global rcfile_error
+    global tid_update_rc_sec, tid_update_rc_min
+
+    if tid_update_rc_sec:
+        tk_utils.tk_top.after_cancel(tid_update_rc_sec)
+        tid_update_rc_sec = None
+    if tid_update_rc_min:
+        tk_utils.tk_top.after_cancel(tid_update_rc_min)
+        tid_update_rc_min = None
+
+    rc_path = __get_rc_file_path()
+    tmp_file_path = None
     try:
         with tempfile.NamedTemporaryFile(mode="w", delete=False, suffix=".tmp",
                                          dir=os.path.dirname(rc_path),
                                          prefix=os.path.basename(rc_path)) as rcfile:
+            tmp_file_path = rcfile.name
             timestamp = str(datetime.now())
             print("#\n"
                   "# gtest_gui configuration file\n"
                   "#\n"
                   "# This file is automatically generated - do not edit\n"
                   "# Written at: %s\n"
                   "#\n" % timestamp, file=rcfile, end="")
 
             # dump software version
-            print("rcfile_version=", json.dumps(rcfile_version), file=rcfile)
-            print("rc_compat_version=", json.dumps(rcfile_compat), file=rcfile)
+            print("rcfile_version=", json.dumps(RCFILE_VERSION), file=rcfile)
+            print("rc_compat_version=", json.dumps(RCFILE_COMPAT), file=rcfile)
             print("rc_timestamp=", json.dumps(timestamp), file=rcfile)
 
-            # dump configuration options
-            print("log_browser=", json.dumps(options["browser"]), file=rcfile)
-            print("browser_stdin=", json.dumps(options["browser_stdin"]), file=rcfile)
-            print("cmd_valgrind1=", json.dumps(options["valgrind1"]), file=rcfile)
-            print("cmd_valgrind2=", json.dumps(options["valgrind2"]), file=rcfile)
-            print("valgrind_exit=", json.dumps(options["valgrind_exit"]), file=rcfile)
-            print("seed_regexp=", json.dumps(options["seed_regexp"]), file=rcfile)
-            print("trace_dir=", json.dumps(options["trace_dir"]), file=rcfile)
-            print("exit_clean_trace=", json.dumps(options["exit_clean_trace"]), file=rcfile)
-            print("startup_import_trace=", json.dumps(options["startup_import_trace"]), file=rcfile)
-            print("copy_executable=", json.dumps(options["copy_executable"]), file=rcfile)
-            print("enable_tool_tips=", json.dumps(options["enable_tool_tips"]), file=rcfile)
-
-            # dump font selection
-            print("font_content=", json.dumps(tk_utils.font_content.configure()), file=rcfile)
-            print("font_trace=", json.dumps(tk_utils.font_trace.configure()), file=rcfile)
-
-            # dump executable file history
-            print("prev_exe_file_list=", json.dumps(prev_exe_file_list), file=rcfile)
-
-            # dump dialog geometry hints
-            print("log_pane_height=", json.dumps(log_pane_height), file=rcfile)
-            print("log_pane_solo_height=", json.dumps(log_pane_solo_height), file=rcfile)
-            print("trace_pane_height=", json.dumps(trace_pane_height), file=rcfile)
-            print("trace_pane_solo_height=", json.dumps(trace_pane_solo_height), file=rcfile)
-            print("tc_list_geometry=", json.dumps(tc_list_geometry), file=rcfile)
-            print("job_list_geometry=", json.dumps(job_list_geometry), file=rcfile)
-            print("help_win_geometry=", json.dumps(help_win_geometry), file=rcfile)
+            # write option values
+            __write_rc_values(rcfile)
 
         # copy attributes on the new file
         try:
-            st = os.stat(rc_path)
+            stt = os.stat(rc_path)
             try:
-                os.chmod(rcfile.name, st.st_mode & 0o777)
-                if (os.name == "posix"):
-                    os.chown(rcfile.name, st.st_uid, st.st_gid)
-            except OSError as e:
-                print("Warning: Failed to update mode/permissions on %s: %s" % (rc_path, e.strerror), file=sys.stderr)
-        except OSError as e:
+                os.chmod(tmp_file_path, stt.st_mode & 0o777)
+                if os.name == "posix":
+                    os.chown(tmp_file_path, stt.st_uid, stt.st_gid)
+            except OSError as exc:
+                if not rcfile_error:
+                    rcfile_error = True
+                    msg = ("Warning: Failed to update file mode/permissions on "
+                           "configuration file %s: %s") % (rc_path, exc.strerror)
+                    tk_messagebox.showerror(parent=tk_utils.tk_top, message=msg)
+        except OSError:
             pass
 
         # move the new file over the old one
         try:
             # MS-Windows does not allow renaming when the target file already exists,
             # therefore remove the target first. Disadvantage: operation is not atomic.
-            if (os.name != "posix"):
+            if os.name != "posix":
                 try:
                     os.remove(rc_path)
                 except OSError:
                     pass
-            os.rename(rcfile.name, rc_path)
+            os.rename(tmp_file_path, rc_path)
             rcfile_error = False
-        except OSError as e:
+        except OSError as exc:
+            if not rcfile_error:
+                rcfile_error = True
+                msg = "Could not replace configuration file %s with temporary %s: %s" % \
+                      (rc_path, tmp_file_path, exc.strerror)
+                tk_messagebox.showerror(parent=tk_utils.tk_top, message=msg)
+            os.remove(tmp_file_path)
+
+    except OSError as exc:
+        if tmp_file_path:
+            # write error - remove the file fragment, report to user
             if not rcfile_error:
-                tk_messagebox.showerror(parent=tk_utils.tk_top, message="Could not replace rc file %s with temporary %s: %s" % (rc_path, rcfile.name, e.strerror))
-            rcfile_error = True
-            os.remove(rcfile.name)
-
-    except OSError as e:
-        # write error - remove the file fragment, report to user
-        if not rcfile_error:
-            rcfile_error = True
-            tk_messagebox.showerror(parent=tk_utils.tk_top, message="Failed to write file %s: %s" % (rcfilename, e.strerror))
-        os.remove(rcfile.name)
+                rcfile_error = True
+                msg = "Failed to write temporary file %s for configuration file update: %s" % \
+                      (rc_path, exc.strerror)
+                tk_messagebox.showerror(parent=tk_utils.tk_top, message=msg)
+            os.remove(tmp_file_path)
+        else:
+            # failed to create temporary file
+            if not rcfile_error:
+                rcfile_error = True
+                msg = "Failed to create temporary file in directory of %s: %s" % \
+                      (rc_path, exc.strerror)
+                tk_messagebox.showerror(parent=tk_utils.tk_top, message=msg)
 
     return not rcfile_error
 
 #
 # This function is used to trigger writing the RC file after changes.
 # The write is delayed by a few seconds to avoid writing the file multiple
 # times when multiple values are changed. This timer is restarted when
 # another change occurs during the delay, however only up to a limit.
 #
-def rc_file_update_after_idle():
+def __rc_file_update_after_idle():
     global tid_update_rc_sec, tid_update_rc_min
 
-    if tid_update_rc_sec: tk_utils.tk_top.after_cancel(tid_update_rc_sec)
-    tid_update_rc_sec = tk_utils.tk_top.after(3000, rc_file_update)
+    if tid_update_rc_sec:
+        tk_utils.tk_top.after_cancel(tid_update_rc_sec)
+    tid_update_rc_sec = tk_utils.tk_top.after(3000, __rc_file_update)
 
     if not tid_update_rc_min:
-        tid_update_rc_min = tk_utils.tk_top.after(60000, rc_file_update)
+        tid_update_rc_min = tk_utils.tk_top.after(60000, __rc_file_update)
+
+
+def rc_file_update_synchronously():
+    """ Update the RC file immediately in case an update is pending. """
+    global rcfile_error
+    if tid_update_rc_sec or tid_update_rc_min or rcfile_error:
+        # warn again if previous update failed
+        rcfile_error = False
 
+        return __rc_file_update()
 
-def rc_file_update_upon_exit():
-    if tid_update_rc_sec or tid_update_rc_min:
-        rc_file_update()
+    return True
```

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/dlg_browser.py` & `mote-gtest-gui-0.9.0/gtest_gui/dlg_browser.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,186 +13,223 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
+"""
+Implements function interfaces for using external applications for displaying
+trace file content, stack traces and for exporting trace files.
+"""
+
 import os
 import re
 import subprocess
-import sys
 import tempfile
 import threading
 
-if (os.name == "posix"): import fcntl
-
 import tkinter as tk
 from tkinter import messagebox as tk_messagebox
 from tkinter import filedialog as tk_filedialog
 
 import gtest_gui.config_db as config_db
-import gtest_gui.gtest as gtest
 import gtest_gui.test_db as test_db
+import gtest_gui.trace_db as trace_db
 import gtest_gui.tk_utils as tk_utils
-import gtest_gui.wid_status_line as wid_status_line
+from gtest_gui.wid_status_line import StatusLineWidget
+
+if os.name == "posix":
+    import fcntl
 
 prev_trace_export_path = ""
 
 temp_dir = None
 
 def __get_temp_dir_name():
     global temp_dir
     if not temp_dir:
         temp_dir = tempfile.TemporaryDirectory(prefix="gtest_gui_tmp")
     return temp_dir.name
 
 
-def show_trace_snippet(tk_top, file_name, file_off, length, is_extern_import):
-    browser_cmd = config_db.options["browser"]
+def show_trace_snippet(file_name, file_off, length, is_extern_import):
+    """
+    Display a part of the complete given trace file in the configured external
+    trace browser. If the external application can read text via STDIN, the
+    text chunk is read from the file and then passed that way. Else, the chunk
+    is stored to a temporary file and that file's name is passed on the command
+    line. Temporary files are deleted once the external application process
+    terminates.
+    """
+    browser_cmd = config_db.get_opt("log_browser")
     if not browser_cmd:
-        wid_status_line.show_message("error", "No trace browser app is configured")
+        StatusLineWidget.get().show_message("error", "No trace browser app is configured")
         return
 
-    if config_db.options["browser_stdin"]:
-        txt = gtest.extract_trace(file_name, file_off, length)
+    if config_db.get_opt("browser_stdin"):
+        txt = trace_db.extract_trace(file_name, file_off, length)
         if txt is None:
-            wid_status_line.show_message("error", "Failed to read trace file")
+            StatusLineWidget.get().show_message("error", "Failed to read trace file")
             return
-        elif txt == "":
-            wid_status_line.show_message("error", "Trace empty for this result")
+        if txt == "":
+            StatusLineWidget.get().show_message("error", "Trace empty for this result")
             return
+
         file_name = "-"
         shared_file = None
 
     else:
-        file_name = gtest.extract_trace_to_temp_file(__get_temp_dir_name(),
-                                                     file_name, file_off, length, is_extern_import)
+        file_name = trace_db.extract_trace_to_temp_file(__get_temp_dir_name(),
+                                                        file_name, file_off, length,
+                                                        is_extern_import)
         if not file_name:
             return
         shared_file = file_name
         txt = ""
 
-    Proc_monitor.create(re.split(r"\s+", browser_cmd) + [file_name], txt, shared_file)
+    ProcMonitor.create(re.split(r"\s+", browser_cmd) + [file_name], txt, shared_file)
 
 
-def show_trace(tk_top, file_name):
-    browser_cmd = config_db.options["browser"]
+def show_trace(file_name):
+    """ Display the complete given trace file in the configured external trace browser. """
+    browser_cmd = config_db.get_opt("log_browser")
     if browser_cmd:
-        Proc_monitor.create(re.split(r"\s+", browser_cmd) + [file_name], "", None)
+        ProcMonitor.create(re.split(r"\s+", browser_cmd) + [file_name], "", None)
     else:
-        wid_status_line.show_message("error", "No trace browser app is configured")
+        StatusLineWidget.get().show_message("error", "No trace browser app is configured")
 
 
 def show_stack_trace(tk_top, tc_name, exe_name, exe_ts, core_name):
+    """
+    Extract and display a stack trace from the given core file using a simple
+    window containing a read-only text frame. Stack trace extraction is done
+    using gdb.
+    """
     cmd_filename = os.path.join(__get_temp_dir_name(), "gdb_command.bat")
     if not os.path.exists(cmd_filename):
         try:
-            with open(cmd_filename, "w") as f:
-                print("info thread", file=f)
-                print("thread apply all backtrace", file=f)
-        except Exception as e:
-            msg = "Error writing command input file for gdb: " + str(e)
+            with open(cmd_filename, "w", encoding="ascii") as file_obj:
+                print("info thread", file=file_obj)
+                print("thread apply all backtrace", file=file_obj)
+        except OSError as exc:
+            msg = "Error writing command input file for gdb: " + str(exc)
             tk_messagebox.showerror(parent=tk_top, message=msg)
             return
 
     if not exe_name:
         msg = "Executable from which this core originates is unknown. " \
               "Use current executable? Press 'No' to manually select an executable."
         answer = tk_messagebox.askyesnocancel(parent=tk_top, message=msg)
         if answer is None:
             return
         if not answer:
-            if (os.name == "posix"):
+            if os.name == "posix":
                 filetypes = [("all", "*"), ("Executable", "*.exe")]
             else:
                 filetypes = [("Executable", "*.exe"), ("all", "*")]
             exe_file = tk_filedialog.askopenfilename(
-                            parent=tk_top, filetypes=filetypes,
-                            title="Select test executable",
-                            initialfile="",
-                            initialdir=os.path.dirname(core_name))
+                parent=tk_top, filetypes=filetypes,
+                title="Select test executable",
+                initialfile="",
+                initialdir=os.path.dirname(core_name))
             if not exe_file:
                 return
         else:
             exe_file = test_db.test_exe_name
     else:
-        exe_file = gtest.gtest_control_get_exe_file_link_name(exe_name, exe_ts)
+        exe_file = trace_db.get_exe_file_link_name(exe_name, exe_ts)
 
     try:
         cmd = ["gdb", "-batch", "-x", cmd_filename, exe_file, core_name]
         # Null device to prevent gdb from getting suspended by SIGTTIN
         proc = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
                                 stdin=subprocess.DEVNULL, text=True)
         flags = fcntl.fcntl(proc.stdout, fcntl.F_GETFL)
         fcntl.fcntl(proc.stdout, fcntl.F_SETFL, flags | os.O_NONBLOCK)
 
-    except Exception as e:
-        tk_messagebox.showerror(parent=tk_top, message="Failed to run gdb: " + str(e))
+    except (OSError, subprocess.SubprocessError) as exc:
+        tk_messagebox.showerror(parent=tk_top, message="Failed to run gdb: " + str(exc))
         return
 
     title = "GtestGui: Stack trace - %s (%s)" % (tc_name, core_name)
-    Log_browser(tk_top, title, proc)
+    LogBrowser(tk_top, title, proc)
 
 
 def export_traces(tk_top, log_idx_sel):
+    """
+    Export trace file chunks of test results with the given indices from the
+    database into an archive file using an external application. The chunks are
+    first read and stored in temporary files. A list of names of those files is
+    passed to the archiver on the command line. Afterward the files are
+    deleted.
+    """
     global prev_trace_export_path
 
     types = [("ZIP archive", "*.zip"), ("all", "*")]
     out_name = tk_filedialog.asksaveasfilename(
-                    parent=tk_top, filetypes=types,
-                    title="Select output file for trace export",
-                    initialfile=os.path.basename(prev_trace_export_path),
-                    initialdir=os.path.dirname(prev_trace_export_path))
+        parent=tk_top, filetypes=types,
+        title="Select output file for trace export",
+        initialfile=os.path.basename(prev_trace_export_path),
+        initialdir=os.path.dirname(prev_trace_export_path))
     if not out_name:
         return
 
     out_name = os.path.abspath(out_name)
     prev_trace_export_path = out_name
 
     with tempfile.TemporaryDirectory() as tempdir:
         file_list = []
         file_idx = 0
         for log_idx in log_idx_sel:
             log = test_db.test_results[log_idx]
             if log[4]:
-                txt = gtest.extract_trace(log[4], log[5], log[6])
+                txt = trace_db.extract_trace(log[4], log[5], log[6])
                 if txt:
                     filename = "trace.%d.%s" % (file_idx, log[0])
                     abs_filename = os.path.join(tempdir, filename)
                     try:
-                        with open(abs_filename, "w") as f:
-                            f.write(txt)
-                    except OSError as e:
+                        with open(abs_filename, "w") as file_obj:
+                            file_obj.write(txt)
+                    except OSError as exc:
                         tk_messagebox.showerror(
                             parent=tk_top,
-                            message="Failed to write temporary file: " + str(e))
+                            message="Failed to write temporary file: " + str(exc))
                         break
 
                     file_list.append(filename)
                     file_idx += 1
 
         if file_list:
             try:
                 cmd = ["zip", "-9", out_name]
                 cmd.extend(file_list)
-                proc = subprocess.run(cmd, check=True, timeout=20, cwd=tempdir,
-                                      stdout=subprocess.DEVNULL)
-            except Exception as e:
+                subprocess.run(cmd, check=True, timeout=20, cwd=tempdir, stdout=subprocess.DEVNULL)
+            except (OSError, subprocess.SubprocessError) as exc:
                 tk_messagebox.showerror(parent=tk_top,
-                                        message="Failed to create archive: " + str(e))
+                                        message="Failed to create archive: " + str(exc))
 
 
 
 # ----------------------------------------------------------------------------
 #
 # Mini dialog only used for displaying text snippets
 #
-class Log_browser(object):
+
+class LogBrowser:
+    # This class has no public interfaces as it only interacts via event handlers.
+    # pylint: disable=too-few-public-methods
+    """
+    This class implements a simple top-level window for displaying a read-only
+    text that is read from the given subprocess pipe. Text is appended
+    dynamically as it is read from the pipe. There is no interaction with
+    other application classes.
+    """
     def __init__(self, tk_top, title, proc):
+        """ Create an instance of the read-only text browser dialog window. """
         wid_top = tk.Toplevel(tk_top)
         wid_top.wm_group(tk_top)
         wid_top.wm_title(title)
 
         wid_txt = tk.Text(wid_top, width=100, height=50, wrap=tk.NONE, relief=tk.FLAT,
                           font=tk_utils.font_content, insertofftime=0, cursor="top_left_arrow")
         wid_txt.pack(side=tk.LEFT, fill=tk.BOTH, expand=1, padx=5, pady=5)
@@ -254,102 +291,127 @@
         if self.proc:
             self.proc.terminate()
             self.proc = None
 
 
 # ----------------------------------------------------------------------------
 #
-# Helper class for monitoring external application
-# - catching error messages
-# - cleaning up temporary input file after exit
 
-class Proc_monitor(object):
+class ProcMonitor:
+    """
+    Helper class for spawning a process using the given command line and then
+    monitoring its status until it exits. After exit, alert the user if exit
+    status is non-zero and clean up the given temporary file (if any).
+    """
     procs = []
     shared_files = {}
     tid = None
 
     @staticmethod
     def create(cmd, txt, file_name):
+        """ Starts a process with the given command line and then waits for it to finish. """
         try:
             proc = subprocess.Popen(cmd, stdin=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
 
             if file_name:
-                Proc_monitor.alloc_shared_file(file_name)
+                ProcMonitor.alloc_shared_file(file_name)
 
-            Proc_monitor.procs.append(Proc_monitor(proc, txt, file_name))
+            ProcMonitor.procs.append(ProcMonitor(proc, txt, file_name))
 
-            if Proc_monitor.tid is None:
-                Proc_monitor.tid = tk_utils.tk_top.after(1000, Proc_monitor.proc_monitor)
+            if ProcMonitor.tid is None:
+                ProcMonitor.tid = tk_utils.tk_top.after(1000, ProcMonitor.proc_monitor)
 
-        except Exception as e:
+        except (OSError, subprocess.SubprocessError) as exc:
             tk_messagebox.showerror(parent=tk_utils.tk_top,
-                                    message="Failed to start external trace browser: " + str(e))
+                                    message="Failed to start external trace browser: " + str(exc))
 
 
     @staticmethod
     def alloc_shared_file(name):
-        if Proc_monitor.shared_files.get(name, None):
-            Proc_monitor.shared_files[name] += 1
+        """
+        Internal method for registering a temporary file that may be shared
+        with other subprocesses.
+        """
+        if ProcMonitor.shared_files.get(name, None):
+            ProcMonitor.shared_files[name] += 1
         else:
-            Proc_monitor.shared_files[name] = 1
+            ProcMonitor.shared_files[name] = 1
 
 
     @staticmethod
     def release_shared_file(name):
-        reg = Proc_monitor.shared_files.get(name, None)
+        """
+        Internal method for releasing a temporary file from a process. The file
+        is removed if the usage counter drops to zero.
+        """
+        reg = ProcMonitor.shared_files.get(name, None)
         if reg is not None:
             if reg > 1:
-                Proc_monitor.shared_files[name] -= 1
+                ProcMonitor.shared_files[name] -= 1
             else:
-                del Proc_monitor.shared_files[name]
+                del ProcMonitor.shared_files[name]
                 try:
                     os.unlink(name)
                 except OSError:
                     pass
 
 
     @staticmethod
     def remove(proc):
-        Proc_monitor.procs = [x for x in Proc_monitor.procs if x is not proc]
-        if not Proc_monitor.procs and Proc_monitor.tid:
-            tk_utils.tk_top.after_cancel(Proc_monitor.tid)
-            Proc_monitor.tid = None
+        """
+        Internal method for removing a process from the watch list after it
+        exited.
+        """
+        ProcMonitor.procs = [x for x in ProcMonitor.procs if x is not proc]
+        if not ProcMonitor.procs and ProcMonitor.tid:
+            tk_utils.tk_top.after_cancel(ProcMonitor.tid)
+            ProcMonitor.tid = None
 
 
     @staticmethod
     def proc_monitor():
-        for proc in Proc_monitor.procs:
+        """
+        Internal method for adding a process to the watch list. If this is the
+        first watched process, a timer is started for periodically checking the
+        process' status.
+        """
+        for proc in ProcMonitor.procs:
             proc.monitor()
 
-        if Proc_monitor.procs:
-            Proc_monitor.tid = tk_utils.tk_top.after(1000, Proc_monitor.proc_monitor)
+        if ProcMonitor.procs:
+            ProcMonitor.tid = tk_utils.tk_top.after(1000, ProcMonitor.proc_monitor)
         else:
-            Proc_monitor.tid = None
+            ProcMonitor.tid = None
 
 
     def __init__(self, proc, txt, file_name):
         self.file_name = file_name
         self.done = False
         self.stderr = None
         self.proc = proc
-        self.thr = threading.Thread(target=lambda:self.__thread_browser(txt), daemon=True)
+        self.thr = threading.Thread(target=lambda: self.__thread_browser(txt), daemon=True)
         self.thr.start()
 
 
     def __thread_browser(self, txt):
         output = self.proc.communicate(input=txt)
 
         self.stderr = output[1]
         self.done = True
 
 
     def monitor(self):
+        """
+        Internal method that is called by the class static monitoring timer
+        periodically on all instances for monitoring process status. If the
+        process has exited, its exit status is checked and an error popup
+        displayed for reporting errors to the user. Afterwards possible
+        temporary files are cleaned up.
+        """
         if self.done:
             if self.proc.returncode != 0:
                 msg = "External trace browser reported error code %d: %s" % \
                         (self.proc.returncode, self.stderr)
                 tk_messagebox.showerror(parent=tk_utils.tk_top, message=msg)
             if self.file_name:
-                Proc_monitor.release_shared_file(self.file_name)
-            Proc_monitor.remove(self)
-
-
+                ProcMonitor.release_shared_file(self.file_name)
+            ProcMonitor.remove(self)
```

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/dlg_config.py` & `mote-gtest-gui-0.9.0/gtest_gui/dlg_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,55 +13,74 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
-#
-# This class implements the configuration parameter dialog.
-#
+"""
+Implements the configuration parameter dialog class.
+"""
 
 import os
 import re
 import tkinter as tk
 from tkinter import messagebox as tk_messagebox
 from tkinter import filedialog as tk_filedialog
 
 import gtest_gui.config_db as config_db
-import gtest_gui.gtest as gtest
+import gtest_gui.gtest_ctrl as gtest_ctrl
 import gtest_gui.tk_utils as tk_utils
+import gtest_gui.trace_db as trace_db
 import gtest_gui.wid_tool_tip as wid_tool_tip
 
-prev_dialog_wid = None
 
-def create_dialog(tk_top):
-    global prev_dialog_wid
+class ConfigDialog:
+    """
+    This class implements a configuration dialog window as a singleton. Instances of the class are
+    created via class function create_dialog(), which only creates a new instance if none exists
+    yet. The dialog window allows entering values for major configuration options. When the "Apply"
+    or "Ok" buttons are clicked, the new values are checked for consistency and if they pass, they
+    are stored in the configuration file.
+    """
+    __prev_dialog_wid = None
+
+    @classmethod
+    def create_dialog(cls, tk_top):
+        """
+        Open the configuration dialog window. If an instance of the dialog
+        already exists, the window is raised, else an instance is created.
+        """
+        if (cls.__prev_dialog_wid and
+                tk_utils.wid_exists(cls.__prev_dialog_wid.wid_top)):
+            cls.__prev_dialog_wid.raise_window()
+        else:
+            cls.__prev_dialog_wid = cls(tk_top)
+
+
+    @classmethod
+    def __destroyed_dialog(cls):
+        cls.__prev_dialog_wid = None
 
-    if prev_dialog_wid and tk_utils.wid_exists(prev_dialog_wid.wid_top):
-        prev_dialog_wid.raise_window()
-    else:
-        prev_dialog_wid = Config_dialog(tk_top)
 
-
-class Config_dialog(object):
     def __init__(self, tk_top):
-        self.tk = tk_top
-        self.var_cfg_browser = tk.StringVar(tk_top, config_db.options["browser"])
-        self.var_cfg_browser_stdin = tk.BooleanVar(tk_top, config_db.options["browser_stdin"])
-        self.var_cfg_seed_regexp = tk.StringVar(tk_top, config_db.options["seed_regexp"])
-
-        self.var_cfg_trace_dir = tk.StringVar(tk_top, config_db.options["trace_dir"])
-        self.var_cfg_exit_clean_trace = tk.BooleanVar(tk_top, config_db.options["exit_clean_trace"])
-        self.var_cfg_startup_import = tk.BooleanVar(tk_top, config_db.options["startup_import_trace"])
-        self.var_cfg_copy_executable = tk.BooleanVar(tk_top, config_db.options["copy_executable"])
-
-        self.var_cfg_valgrind1 = tk.StringVar(tk_top, config_db.options["valgrind1"])
-        self.var_cfg_valgrind2 = tk.StringVar(tk_top, config_db.options["valgrind2"])
-        self.var_cfg_valgrind_exit = tk.BooleanVar(tk_top, config_db.options["valgrind_exit"])
+        self.tk_top = tk_top
+        self.var_cfg_browser = tk.StringVar(tk_top, config_db.get_opt("log_browser"))
+        self.var_cfg_browser_stdin = tk.BooleanVar(tk_top, config_db.get_opt("browser_stdin"))
+        self.var_cfg_seed_regexp = tk.StringVar(tk_top, config_db.get_opt("seed_regexp"))
+
+        self.var_cfg_trace_dir = tk.StringVar(tk_top, config_db.get_opt("trace_dir"))
+        self.var_cfg_exit_clean_trace = tk.BooleanVar(tk_top, config_db.get_opt("exit_clean_trace"))
+        self.var_cfg_startup_import = tk.BooleanVar(tk_top,
+                                                    config_db.get_opt("startup_import_trace"))
+        self.var_cfg_copy_executable = tk.BooleanVar(tk_top, config_db.get_opt("copy_executable"))
+
+        self.var_cfg_valgrind1 = tk.StringVar(tk_top, config_db.get_opt("cmd_valgrind1"))
+        self.var_cfg_valgrind2 = tk.StringVar(tk_top, config_db.get_opt("cmd_valgrind2"))
+        self.var_cfg_valgrind_exit = tk.BooleanVar(tk_top, config_db.get_opt("valgrind_exit"))
 
         self.wid_top = tk.Toplevel(tk_top)
         self.wid_top.wm_group(tk_top)
         self.wid_top.wm_title("GtestGui: Configuration options")
 
         self.wid_top.columnconfigure(1, weight=1)
 
@@ -77,16 +96,18 @@
                                self.var_cfg_exit_clean_trace, "config.exit_clean_trace")
         self.__add_checkbutton(6, "Automatically import trace files upon start",
                                self.var_cfg_startup_import, "config.startup_import_trace")
         self.__add_checkbutton(7, "Create copy of executable file under test",
                                self.var_cfg_copy_executable, "config.copy_executable")
         self.__add_separator(8)
 
-        self.__add_entry_widget(9, "Valgrind command line:", self.var_cfg_valgrind1, "config.valgrind1")
-        self.__add_entry_widget(10, "Valgrind alternate:", self.var_cfg_valgrind2, "config.valgrind2")
+        self.__add_entry_widget(9, "Valgrind command line:",
+                                self.var_cfg_valgrind1, "config.valgrind1")
+        self.__add_entry_widget(10, "Valgrind alternate:",
+                                self.var_cfg_valgrind2, "config.valgrind2")
         self.__add_checkbutton(11, "Valgrind supports --error-exitcode",
                                self.var_cfg_valgrind_exit, "config.valgrind_exit")
 
         wid_frm = tk.Frame(self.wid_top)
         wid_but_abort = tk.Button(wid_frm, text="Cancel", command=self.__quit)
         wid_but_abort.pack(side=tk.LEFT, padx=10)
         wid_but_apply = tk.Button(wid_frm, text="Apply", command=self.__apply_config)
@@ -133,99 +154,105 @@
 
     def __add_separator(self, grid_row):
         wid_sep = tk.Frame(self.wid_top, borderwidth=1, relief=tk.SUNKEN, height=2)
         wid_sep.grid(row=grid_row, column=0, columnspan=2, sticky="we", padx=0, pady=5)
 
 
     def raise_window(self):
+        """ Raises the dialog window above all other windows."""
         self.wid_top.wm_deiconify()
         self.wid_top.lift()
 
 
     def __quit(self):
-        global prev_dialog_wid
         tk_utils.safe_destroy(self.wid_top)
-        prev_dialog_wid = None
+        ConfigDialog.__destroyed_dialog()
 
 
     def __open_trace_dir_file_browser(self):
         dirname = tk_filedialog.askdirectory(
                         parent=self.wid_top, title="Select trace directory",
                         initialdir=self.var_cfg_trace_dir.get())
         if dirname:
             self.var_cfg_trace_dir.set(dirname)
 
 
     def __check_seed_pattern(self, seed_exp):
         try:
             re.compile(seed_exp)
-        except Exception as e:
+        except re.error as exc:
             tk_messagebox.showerror(
-                    parent=self.wid_top,
-                    message="Syntax error in regular expression for \"seed\": " + str(e))
+                parent=self.wid_top,
+                message="Syntax error in regular expression for \"seed\": " + str(exc))
             return False
         return True
 
 
     def __check_trace_dir(self, trace_dir):
         if not os.path.isdir(trace_dir):
             if os.path.exists(trace_dir):
                 tk_messagebox.showerror(parent=self.wid_top,
                                         message="Trace directory is not a directory")
                 return False
 
-            if not tk_messagebox.askokcancel(
-                        parent=self.wid_top,
-                        message="Trace directory does not exist - Do you want to create it?"):
+            msg = "Trace directory does not exist - Do you want to create it?"
+            if not tk_messagebox.askokcancel(parent=self.wid_top, message=msg):
                 return False
 
             try:
                 os.mkdir(trace_dir)
-            except OSError as e:
+            except OSError as exc:
                 tk_messagebox.showerror(parent=self.wid_top,
-                                        message="Failed to create directory: " + str(e))
+                                        message="Failed to create directory: " + str(exc))
                 return False
 
         return True
 
 
+    @staticmethod
+    def __normalize_shell_cmd(var):
+        return re.sub(r"\s+", " ", var.get()).strip()
+
+
     def __apply_config(self):
         seed_exp = self.var_cfg_seed_regexp.get()
         if seed_exp and not self.__check_seed_pattern(seed_exp):
             return False
 
         trace_dir = self.var_cfg_trace_dir.get().strip()
         if trace_dir:
             trace_dir = os.path.abspath(trace_dir)
             if not self.__check_trace_dir(trace_dir):
                 return False
 
-        if ((trace_dir != config_db.options["trace_dir"]) or
-            (self.var_cfg_copy_executable.get() != config_db.options["copy_executable"])):
-            if gtest.gtest_ctrl.is_active():
+        if ((trace_dir != config_db.get_opt("trace_dir")) or
+                (self.var_cfg_copy_executable.get() != config_db.get_opt("copy_executable"))):
+            if gtest_ctrl.gtest_ctrl.is_active():
                 msg = "Need to stop running tests for changing the trace directory " \
                       "or copy-executable options."
                 if not tk_messagebox.askokcancel(parent=self.wid_top, message=msg):
                     return False
-                gtest.gtest_ctrl.stop(kill=True)
-
-            gtest.release_exe_file_copy()
-
-        config_db.options["browser"] = re.sub(r"\s+", " ", self.var_cfg_browser.get()).strip()
-        config_db.options["browser_stdin"] = self.var_cfg_browser_stdin.get()
-        config_db.options["seed_regexp"] = seed_exp
+                gtest_ctrl.gtest_ctrl.stop(kill=True)
 
-        config_db.options["trace_dir"] = trace_dir
-        config_db.options["exit_clean_trace"] = self.var_cfg_exit_clean_trace.get()
-        config_db.options["startup_import_trace"] = self.var_cfg_startup_import.get()
-        config_db.options["copy_executable"] = self.var_cfg_copy_executable.get()
+            trace_db.release_exe_file_copy()
 
-        config_db.options["valgrind1"] = re.sub(r"\s+", " ", self.var_cfg_valgrind1.get()).strip()
-        config_db.options["valgrind2"] = re.sub(r"\s+", " ", self.var_cfg_valgrind2.get()).strip()
-        config_db.options["valgrind_exit"] = self.var_cfg_valgrind_exit.get()
+        config_db.set_opt("log_browser", ConfigDialog.__normalize_shell_cmd(self.var_cfg_browser))
+        config_db.set_opt("browser_stdin", self.var_cfg_browser_stdin.get())
+        config_db.set_opt("seed_regexp", seed_exp)
+
+        config_db.set_opt("trace_dir", trace_dir)
+        config_db.set_opt("exit_clean_trace", self.var_cfg_exit_clean_trace.get())
+        config_db.set_opt("startup_import_trace", self.var_cfg_startup_import.get())
+        config_db.set_opt("copy_executable", self.var_cfg_copy_executable.get())
+
+        config_db.set_opt("cmd_valgrind1",
+                          ConfigDialog.__normalize_shell_cmd(self.var_cfg_valgrind1))
+        config_db.set_opt("cmd_valgrind2",
+                          ConfigDialog.__normalize_shell_cmd(self.var_cfg_valgrind2))
+        config_db.set_opt("valgrind_exit", self.var_cfg_valgrind_exit.get())
 
-        return config_db.rc_file_update()
+        return config_db.rc_file_update_synchronously()
 
 
     def __save_and_close(self):
         if self.__apply_config():
             self.__quit()
```

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/dlg_font_sel.py` & `mote-gtest-gui-0.9.0/gtest_gui/dlg_font_sel.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,76 +15,99 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
 # This code is derived from Trace Browser (trowser.py)
 
+"""
+Implements the font selection dialog class.
+"""
+
 import tkinter as tk
 import tkinter.font as tkf
 
 import gtest_gui.tk_utils as tk_utils
 
-prev_dialog_wid = {}
 
-def create_dialog(tk_top, ftype, font, callback):
-    global prev_dialog_wid
+class FontSelectionDialog:
+    """
+    This class implements a font selection dialog. Instances of the class are created via class
+    function create_dialog(): If a window created for the same value of parameter "ftype" already
+    exists it is raised, else a new window is created. The dialog presents a list of all fonts,
+    which is queried from the windowing sytem, and a demo text frame where a sample text is rendered
+    with the font selected in the listbox. When the "Apply" or "Ok" buttons are clicked, the given
+    font variable is configured to the new font and the given callback is invoked.
+    """
+    __prev_dialog_wid = {}
+
+    @classmethod
+    def create_dialog(cls, tk_top, ftype, font, callback):
+        """
+        Static function for opening a font selection dialog window for a given font variable.
+        """
+        if (cls.__prev_dialog_wid.get(ftype, None) and
+                tk_utils.wid_exists(cls.__prev_dialog_wid[ftype].wid_top)):
+            cls.__prev_dialog_wid[ftype].raise_window()
+        else:
+            cls.__prev_dialog_wid[ftype] = FontSelectionDialog(tk_top, ftype, font, callback)
+
 
-    if prev_dialog_wid.get(ftype, None) and tk_utils.wid_exists(prev_dialog_wid[ftype].wid_top):
-        prev_dialog_wid[ftype].raise_window()
-    else:
-        prev_dialog_wid[ftype] = Font_selection_dialog(tk_top, ftype, font, callback)
+    @classmethod
+    def __destroyed_dialog(cls, ftype):
+        cls.__prev_dialog_wid.pop(ftype, None)
 
 
-class Font_selection_dialog(object):
     def __init__(self, tk_top, ftype, font, callback):
-        self.tk = tk_top
+        """ Creates a new font selection dialog window """
+        self.tk_top = tk_top
         self.ftype = ftype
         self.font = font
         self.callback = callback
 
-        self.wid_top = tk.Toplevel(self.tk)
+        self.wid_top = tk.Toplevel(self.tk_top)
         self.wid_top.wm_title("GtestGui: Font selection")
-        self.wid_top.wm_group(self.tk)
+        self.wid_top.wm_group(self.tk_top)
 
-        self.var_font_bold = tk.BooleanVar(self.tk, False)
-        self.var_font_size = tk.IntVar(self.tk, 10)
+        self.var_font_bold = tk.BooleanVar(self.tk_top, False)
+        self.var_font_size = tk.IntVar(self.tk_top, 10)
 
         # frame #1: listbox with all available fonts
         wid_frm = tk.Frame(self.wid_top)
         self.wid_font_list = tk.Listbox(wid_frm, width=40, height=10, font=tk_utils.font_normal,
                                         exportselection=0, cursor="top_left_arrow",
                                         selectmode=tk.BROWSE)
         self.wid_font_list.pack(side=tk.LEFT, fill=tk.BOTH, expand=1)
         wid_sb = tk.Scrollbar(wid_frm, orient=tk.VERTICAL, command=self.wid_font_list.yview,
                               takefocus=0)
         wid_sb.pack(side=tk.LEFT, fill=tk.Y)
         self.wid_font_list.configure(yscrollcommand=wid_sb.set)
         wid_frm.pack(side=tk.TOP, fill=tk.BOTH, expand=1, padx=5, pady=5)
-        self.wid_font_list.bind("<<ListboxSelect>>",
-                                lambda e: tk_utils.bind_call_and_break(
-                                            self.__handle_selection_change))
+        self.wid_font_list.bind("<<ListboxSelect>>", lambda e:
+                                tk_utils.bind_call_and_break(self.__handle_selection_change))
 
         # frame #2: size and weight controls
         wid_frm2 = tk.Frame(self.wid_top)
         wid_lab = tk.Label(wid_frm2, text="Font size:")
         wid_lab.pack(side=tk.LEFT)
         wid_spin = tk.Spinbox(wid_frm2, from_=1, to=99, width=3,
-                              textvariable=self.var_font_size, command=self.__handle_selection_change)
+                              textvariable=self.var_font_size,
+                              command=self.__handle_selection_change)
         wid_spin.pack(side=tk.LEFT)
         wid_chk = tk.Checkbutton(wid_frm2, text="bold",
-                                 variable=self.var_font_bold, command=self.__handle_selection_change)
+                                 variable=self.var_font_bold,
+                                 command=self.__handle_selection_change)
         wid_chk.pack(side=tk.LEFT, padx=15)
         wid_frm2.pack(side=tk.TOP, fill=tk.X, padx=5, pady=5)
 
         # frame #3: demo text
         self.wid_demo = tk.Text(self.wid_top, width=20, height=4, wrap=tk.NONE,
                                 exportselection=tk.FALSE, relief=tk.RIDGE, takefocus=0)
         self.wid_demo.pack(side=tk.TOP, fill=tk.X, padx=15, pady=10)
-        self.wid_demo.bindtags([self.wid_demo, "TextReadOnly", self.tk, "all"])
+        self.wid_demo.bindtags([self.wid_demo, "TextReadOnly", self.tk_top, "all"])
 
         self.wid_demo.insert("end", "ABCDEFGHIJKLMNOPQRSTUVWXYZ\n")
         self.wid_demo.insert("end", "abcdefghijklmnopqrstuvwxyz\n")
         self.wid_demo.insert("end", "0123456789\n")
         self.wid_demo.insert("end", "AAA ,,,...---;;;:::___+++=== AAA\n")
 
         # frame #4: ok/abort buttons
@@ -117,56 +140,57 @@
             pass
 
         # finally update demo box with the currently selected font
         self.__handle_selection_change()
 
 
     def raise_window(self):
+        """ Raises the dialog window above all other windows."""
         self.wid_top.wm_deiconify()
         self.wid_top.lift()
         self.wid_font_list.focus_set()
 
 
     def __fill_font_list(self):
         # remove duplicates, then sort alphabetically
-        self.font_families = sorted(set(tkf.families(displayof=self.tk)))
+        self.font_families = sorted(set(tkf.families(displayof=self.tk_top)))
 
-        for f in self.font_families:
-            self.wid_font_list.insert("end", f)
+        for family in self.font_families:
+            self.wid_font_list.insert("end", family)
 
 
     def __handle_selection_change(self):
         sel = self.wid_font_list.curselection()
         if (len(sel) == 1) and (sel[0] < len(self.font_families)):
-          name = "{%s} %d" % (self.font_families[sel[0]], self.var_font_size.get())
-          if self.var_font_bold.get():
-              name = name + " bold"
+            name = "{%s} %d" % (self.font_families[sel[0]], self.var_font_size.get())
+            if self.var_font_bold.get():
+                name = name + " bold"
 
-          # succeeds even for unknown fonts, therefore try/except not needed
-          self.wid_demo.configure(font=name)
+            # succeeds even for unknown fonts, therefore try/except not needed
+            self.wid_demo.configure(font=name)
 
 
     def __quit(self):
         tk_utils.safe_destroy(self.wid_top)
-        prev_dialog_wid.pop(self.ftype, None)
+        FontSelectionDialog.__destroyed_dialog(self.ftype)
 
 
     def __apply_config(self):
         sel = self.wid_font_list.curselection()
         if (len(sel) == 1) and (sel[0] < len(self.font_families)):
             self.font.configure(family=self.font_families[sel[0]],
                                 size=self.var_font_size.get(),
                                 weight=(tkf.BOLD if self.var_font_bold.get() else tkf.NORMAL))
             try:
                 self.callback(self.font)
                 return True
 
-            except Exception as e:
+            except tk.TclError as exc:
                 tk.messagebox.showerror(parent=self.wid_top,
-                                        message="Selected font is unavailable: " + str(e))
+                                        message="Selected font is unavailable: " + str(exc))
         else:
             tk.messagebox.showerror(parent=self.wid_top,
                                     message=("No font is selected - "
                                              "Use \"Abort\" to leave without changes."))
         return False
```

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/dlg_help.py` & `mote-gtest-gui-0.9.0/gtest_gui/dlg_help.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,89 +13,111 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
-#
-# This class implements the help dialog.
-#
+"""
+Implements the help dialog window class.
+"""
 
 import re
 import tkinter as tk
 import tkinter.font as tkf
 
 import gtest_gui.tk_utils as tk_utils
 import gtest_gui.config_db as config_db
 import gtest_gui.help_db as help_db
 
-prev_dialog_wid = None
-
-help_titles = []
-help_fg = "black"
-help_bg = "#FFFFA0"
-help_font_normal = None
-help_font_fixed = None
-help_font_bold = None
-help_font_title1 = None
-help_font_title2 = None
-
-
-def create_dialog(tk_top, index, subheading="", subrange=""):
-    global prev_dialog_wid
-
-    if not help_font_normal:
-        define_fonts()
-
-    if prev_dialog_wid and tk_utils.wid_exists(prev_dialog_wid.wid_top):
-        prev_dialog_wid.raise_window(index, subheading, subrange)
-    else:
-        prev_dialog_wid = Help_dialog(tk_top, index, subheading, subrange)
-
 
-def define_fonts():
-    global help_font_normal, help_font_fixed, help_font_title1, help_font_title2, help_font_bold
+class HelpDialog:
+    """
+    Help dialog window class (singleton): The dialog displays documentation
+    text and a few basic command buttons for navigation.
+    """
+    __prev_dialog_wid = None
+
+    __help_fg = "black"
+    __help_bg = "#FFFFA0"
+    __help_font_normal = None
+    __help_font_fixed = None
+    __help_font_bold = None
+    __help_font_title1 = None
+    __help_font_title2 = None
+
+
+    @classmethod
+    def create_dialog(cls, tk_top, index, subheading="", subrange=""):
+        """
+        Open the help dialog window. If an instance of the dialog already
+        exists, the window is raised, else an instance is created.
+        """
+        if not cls.__help_font_normal:
+            cls.__define_fonts()
 
-    help_font_fixed = "TkFixedFont"
-    help_font_normal = tkf.Font(font="TkTextFont")
+        if cls.__prev_dialog_wid and tk_utils.wid_exists(cls.__prev_dialog_wid.wid_top):
+            cls.__prev_dialog_wid.raise_window(index, subheading, subrange)
+        else:
+            cls.__prev_dialog_wid = HelpDialog(tk_top, index, subheading, subrange)
 
-    opt = help_font_normal.configure()
-    opt["weight"] = tkf.BOLD
-    help_font_bold = tkf.Font(**opt)
-    opt["size"] += 2
-    help_font_title2 = tkf.Font(**opt)
-    opt["size"] += 2
-    help_font_title1 = tkf.Font(**opt)
 
+    @classmethod
+    def __destroyed_dialog(cls):
+        cls.__prev_dialog_wid = None
+
+
+    @classmethod
+    def __define_fonts(cls):
+        cls.__help_font_fixed = "TkFixedFont"
+        cls.__help_font_normal = tkf.Font(font="TkTextFont")
+
+        opt = cls.__help_font_normal.configure()
+        opt["weight"] = tkf.BOLD
+        cls.__help_font_bold = tkf.Font(**opt)
+        opt["size"] += 2
+        cls.__help_font_title2 = tkf.Font(**opt)
+        opt["size"] += 2
+        cls.__help_font_title1 = tkf.Font(**opt)
 
-def add_menu_commands(tk_top, wid_men):
-    global help_titles
 
-    for title, idx in help_db.helpIndex.items():
-        help_titles.append(title)
+    @staticmethod
+    def add_menu_commands(tk_top, wid_men):
+        """
+        Adds a menu command for each help text chapter in the database to the
+        given menu item. Each of the commands open the help dialog window if
+        not yet open, then display the respective help text.
+        """
+        for idx in range(len(help_db.HELP_INDEX)):
+            wid_men.add_command(label=help_db.HELP_INDEX[idx],
+                                command=lambda idx=idx: HelpDialog.create_dialog(tk_top, idx))
+            for sub in sorted([x[1] for x in help_db.HELP_SECTIONS if x[0] == idx]):
+                title = help_db.HELP_SECTIONS[(idx, sub)]
+                wid_men.add_command(label="- " + title,
+                                    command=lambda idx=idx, title=title:
+                                    HelpDialog.create_dialog(tk_top, idx, title))
 
-    Help_dialog.fill_menu(tk_top, wid_men)
 
+    # -------------------------------------------------------------------------
 
-class Help_dialog(object):
     def __init__(self, tk_top, index, subheading, subrange):
+        """ Create a Help dialog window and initially display the given chapter's text. """
         self.tk_top = tk_top
         self.chapter_idx = -1
         self.help_stack = []
 
         self.wid_top = tk.Toplevel(self.tk_top)
         self.wid_top.wm_title("GtestGui: Manual")
         self.wid_top.wm_group(self.tk_top)
 
         self.__create_buttons()
         self.__create_text_widget()
 
-        if config_db.help_win_geometry:
-            self.wid_top.wm_geometry(config_db.help_win_geometry)
+        if config_db.get_opt("help_win_geometry"):
+            self.wid_top.wm_geometry(config_db.get_opt("help_win_geometry"))
 
         self.wid_top.bind("<Configure>", lambda e: self.__handle_window_resize(e.widget))
         self.wid_txt.focus_set()
 
         self.__fill_help_text(index, subheading, subrange)
 
 
@@ -113,155 +135,150 @@
         wid_frm.columnconfigure(2, weight=1)
         wid_frm.columnconfigure(5, weight=1)
         wid_frm.pack(side=tk.TOP, fill=tk.X)
         wid_frm.bind("<Destroy>", lambda e: self.__destroy_window())
 
         men_chpt = tk.Menu(but_cmd_chpt, tearoff=0)
         but_cmd_chpt.configure(menu=men_chpt)
-        Help_dialog.fill_menu(self.tk_top, men_chpt)
+        HelpDialog.add_menu_commands(self.tk_top, men_chpt)
 
         self.but_cmd_prev = but_cmd_prev
         self.but_cmd_next = but_cmd_next
 
-    @staticmethod
-    def fill_menu(tk_top, wid_men):
-        for idx in range(len(help_titles)):
-            wid_men.add_command(label=help_titles[idx],
-                                command=lambda idx=idx: create_dialog(tk_top, idx))
-            for foo, sub in sorted([x for x in help_db.helpSections.keys() if x[0] == idx]):
-                title = help_db.helpSections[(idx, sub)]
-                wid_men.add_command(label="- " + title,
-                            command=lambda idx=idx, title=title: create_dialog(tk_top, idx, title))
-
-
     def __create_text_widget(self):
         wid_frm = tk.Frame(self.wid_top)
         wid_txt = tk.Text(wid_frm, width=80, wrap=tk.WORD,
-                          foreground=help_fg, background=help_bg, font=help_font_normal,
+                          foreground=HelpDialog.__help_fg, background=HelpDialog.__help_bg,
+                          font=HelpDialog.__help_font_normal,
                           spacing3=6, cursor="circle", takefocus=1)
         wid_txt.pack(side=tk.LEFT, fill=tk.BOTH, expand=1)
         wid_sb = tk.Scrollbar(wid_frm, orient=tk.VERTICAL, command=wid_txt.yview, takefocus=0)
         wid_txt.configure(yscrollcommand=wid_sb.set)
         wid_sb.pack(fill=tk.Y, anchor=tk.E, side=tk.LEFT)
         wid_frm.pack(side=tk.TOP, fill=tk.BOTH, expand=1)
 
         # define tags for various nroff text formats
-        wid_txt.tag_configure("title1", font=help_font_title1, spacing3=10)
-        wid_txt.tag_configure("title2", font=help_font_title2, spacing1=20, spacing3=10)
+        wid_txt.tag_configure("title1", font=HelpDialog.__help_font_title1, spacing3=10)
+        wid_txt.tag_configure("title2", font=HelpDialog.__help_font_title2,
+                              spacing1=20, spacing3=10)
         wid_txt.tag_configure("indent", lmargin1=30, lmargin2=30)
-        wid_txt.tag_configure("bold", font=help_font_bold)
+        wid_txt.tag_configure("bold", font=HelpDialog.__help_font_bold)
         wid_txt.tag_configure("underlined", underline=1)
-        wid_txt.tag_configure("fixed", font=help_font_fixed)
-        wid_txt.tag_configure("pfixed", font=help_font_fixed, spacing1=0, spacing2=0, spacing3=0)
+        wid_txt.tag_configure("fixed", font=HelpDialog.__help_font_fixed)
+        wid_txt.tag_configure("pfixed", font=HelpDialog.__help_font_fixed,
+                              spacing1=0, spacing2=0, spacing3=0)
         wid_txt.tag_configure("href", underline=1, foreground="blue")
         wid_txt.tag_bind("href", "<ButtonRelease-1>", lambda e: self.__follow_help_hyperlink())
-        wid_txt.tag_bind("href", "<Enter>", lambda e: self.wid_txt.configure(cursor="top_left_arrow"))
+        wid_txt.tag_bind("href", "<Enter>",
+                         lambda e: self.wid_txt.configure(cursor="top_left_arrow"))
         wid_txt.tag_bind("href", "<Leave>", lambda e: self.wid_txt.configure(cursor="circle"))
 
         # allow to scroll the text with the cursor keys
         wid_txt.bindtags([wid_txt, "TextReadOnly", self.wid_top, "all"])
         wid_txt.bind("<Up>", lambda e, self=self: tk_utils.bind_call_and_break(
-                                lambda: wid_txt.yview(tk.SCROLL, -1, "unit")))
+            lambda: wid_txt.yview(tk.SCROLL, -1, "unit")))
         wid_txt.bind("<Down>", lambda e, self=self: tk_utils.bind_call_and_break(
-                                lambda: wid_txt.yview(tk.SCROLL, 1, "unit")))
+            lambda: wid_txt.yview(tk.SCROLL, 1, "unit")))
         wid_txt.bind("<Prior>", lambda e, self=self: tk_utils.bind_call_and_break(
-                                lambda: wid_txt.yview(tk.SCROLL, -1, "pages")))
+            lambda: wid_txt.yview(tk.SCROLL, -1, "pages")))
         wid_txt.bind("<Next>", lambda e, self=self: tk_utils.bind_call_and_break(
-                                lambda: wid_txt.yview(tk.SCROLL, 1, "pages")))
+            lambda: wid_txt.yview(tk.SCROLL, 1, "pages")))
         wid_txt.bind("<Home>", lambda e, self=self: tk_utils.bind_call_and_break(
-                                lambda: wid_txt.yview(tk.MOVETO, 0.0)))
+            lambda: wid_txt.yview(tk.MOVETO, 0.0)))
         wid_txt.bind("<End>", lambda e, self=self: tk_utils.bind_call_and_break(
-                                lambda: wid_txt.yview(tk.MOVETO, 1.0)))
+            lambda: wid_txt.yview(tk.MOVETO, 1.0)))
         wid_txt.bind("<Enter>", lambda e, self=self: tk_utils.bind_call_and_break(
-                                lambda: e.widget.focus_set()))
+            e.widget.focus_set))
         wid_txt.bind("<Escape>", lambda e: self.__destroy_window())
         wid_txt.bind("<Alt-Key-n>", lambda e: self.but_cmd_next.invoke())
         wid_txt.bind("<Alt-Key-p>", lambda e: self.but_cmd_prev.invoke())
 
         self.wid_txt = wid_txt
 
 
     def raise_window(self, index, subheading="", subrange=""):
+        """ Raises the dialog window above all other windows."""
         self.wid_top.lift()
         self.__fill_help_text(index, subheading, subrange)
 
 
     def __fill_help_text(self, index, subheading, subrange):
         self.wid_txt.configure(state=tk.NORMAL)
         self.wid_txt.delete("1.0", "end")
         self.wid_txt.yview(tk.MOVETO, 0.0)
 
         # fill the widget with the formatted text
-        for htext, tlabel in help_db.helpTexts[index]:
+        for htext, tlabel in help_db.HELP_TEXTS[index]:
             self.wid_txt.insert("end", htext, tlabel)
 
         self.wid_txt.configure(state=tk.DISABLED)
 
         # bring the given text section into view
         if (len(subrange) == 2) and subrange[0]:
             self.wid_txt.see(subrange[1])
             self.wid_txt.see(subrange[0])
         elif subheading:
-            # search for the string at the beginning of the line only (prevents matches on hyperlinks)
+            # search for the string at the beginning of the line only
+            # (prevents matches on hyperlinks)
             pattern = "^" + str(subheading)
             pos = self.wid_txt.search(pattern, regexp=True, index="1.0")
             if pos:
                 self.wid_txt.see(pos)
                 # make sure the header is at the top of the page
                 bbox = self.wid_txt.bbox(pos)
                 if bbox:
                     bbox_y = bbox[1]
                     bbox_h = bbox[3]
                     self.wid_txt.yview(tk.SCROLL, bbox_y // bbox_h, "units")
                     self.wid_txt.see(pos)
 
         # define/update bindings for left/right command buttons
-        if help_db.helpTexts.get(index - 1, None):
-            self.but_cmd_prev.configure(command=lambda: self.raise_window(index - 1), state=tk.NORMAL)
+        if index > 0:
+            self.but_cmd_prev.configure(command=lambda:
+                                        self.raise_window(index - 1), state=tk.NORMAL)
         else:
             self.but_cmd_prev.configure(command=lambda: None, state=tk.DISABLED)
 
-        if help_db.helpTexts.get(index + 1, None):
-            self.but_cmd_next.configure(command=lambda: self.raise_window(index + 1), state=tk.NORMAL)
+        if index + 1 < len(help_db.HELP_TEXTS):
+            self.but_cmd_next.configure(command=lambda:
+                                        self.raise_window(index + 1), state=tk.NORMAL)
         else:
             self.but_cmd_next.configure(command=lambda: None, state=tk.DISABLED)
 
         self.chapter_idx = index
 
 
     def __destroy_window(self):
-        global prev_dialog_wid
         tk_utils.safe_destroy(self.wid_top)
-        prev_dialog_wid = None
+        HelpDialog.__destroyed_dialog()
 
 
     def __follow_help_hyperlink(self):
-        global helpIndex
-
         # the text under the mouse carries the mark 'current'
         curidx = self.wid_txt.index("current + 1 char")
 
         # determine the range of the 'href' tag under the mouse
-        range = self.wid_txt.tag_prevrange("href", curidx)
+        href_range = self.wid_txt.tag_prevrange("href", curidx)
 
         # cut out the text in that range
-        hlink = self.wid_txt.get(*range)
+        hlink = self.wid_txt.get(*href_range)
 
         # check if the text contains a sub-section specification
         match = re.match(r"(.*): *(.*)", hlink)
         if match:
             hlink = match.group(1)
             subsect = match.group(2)
         else:
             subsect = ""
 
-        if help_db.helpIndex.get(hlink, None):
-            self.raise_window(help_db.helpIndex[hlink], subsect)
+        try:
+            idx = help_db.HELP_INDEX.index(hlink)
+            self.raise_window(idx, subsect)
+        except ValueError:
+            pass
 
 
     # callback for Configure (aka resize) event on the toplevel window
     def __handle_window_resize(self, wid):
         if wid == self.wid_top:
             new_size = self.wid_top.wm_geometry()
-            if new_size != config_db.help_win_geometry:
-                config_db.help_win_geometry = new_size
-                config_db.rc_file_update_after_idle()
+            config_db.set_opt("help_win_geometry", new_size)
```

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/dlg_job_list.py` & `mote-gtest-gui-0.9.0/gtest_gui/dlg_job_list.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,95 +13,105 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
-#
-# This class implements the test case list dialog.
-#
+"""
+Implements the job list dialog window class.
+"""
 
 import tkinter as tk
 from tkinter import messagebox as tk_messagebox
 
 import gtest_gui.config_db as config_db
 import gtest_gui.dlg_browser as dlg_browser
-import gtest_gui.filter_expr as filter_expr
-import gtest_gui.gtest as gtest
+import gtest_gui.gtest_ctrl as gtest_ctrl
 import gtest_gui.test_db as test_db
 import gtest_gui.tk_utils as tk_utils
-import gtest_gui.wid_test_ctrl as wid_test_ctrl
-import gtest_gui.wid_text_sel as wid_text_sel
-
+from gtest_gui.wid_text_sel import TextSelWidget
 
-prev_dialog_wid = None
-prev_export_filename = ""
 
+class JobListDialog:
+    """
+    This class implements a job list dialog window as a singleton. Instances of the class are
+    created via class function create_dialog(), which only creates a new instance if none exists
+    yet. The dialog window shows a list of all test processes started by the current test campaign.
+    For each process statistics about received trace and yet pending results are shown. Processes
+    can be aborted via a context menu.
+    """
+    __prev_dialog_wid = None
+
+    @classmethod
+    def create_dialog(cls, tk_top):
+        """
+        Open the configuration dialog window. If an instance of the dialog
+        already exists, the window is raised, else an instance is created.
+        """
+        if not test_db.test_case_names:
+            msg = "Test case list is empty, no tests can run."
+            tk_messagebox.showerror(parent=tk_top, message=msg)
+            return
 
-def create_dialog(tk_top):
-    global prev_dialog_wid
+        if cls.__prev_dialog_wid and tk_utils.wid_exists(cls.__prev_dialog_wid.wid_top):
+            cls.__prev_dialog_wid.raise_window()
+        else:
+            cls.__prev_dialog_wid = JobListDialog(tk_top)
 
-    if not test_db.test_case_names:
-        tk_messagebox.showerror(parent=tk_top, message="Test case list is empty, no tests can run.")
-        return
 
-    if prev_dialog_wid and tk_utils.wid_exists(prev_dialog_wid.wid_top):
-        prev_dialog_wid.raise_window()
-    else:
-        prev_dialog_wid = Job_list_dialog(tk_top)
+    @classmethod
+    def __destroyed_dialog(cls):
+        cls.__prev_dialog_wid = None
 
 
-class Job_list_dialog(object):
     def __init__(self, tk_top):
-        self.tk = tk_top
-        self.table_header_txt = ("PID", "Traced", "#Results", "Current test case")
+        self.tk_top = tk_top
+        self.table_header_txt = ("PID", "BgJob", "Traced", "#Results", "Done", "Current test case")
 
         self.__create_dialog_window()
         self.__populate_table()
-        self.timer_id = self.tk.after(500, self.__update_by_timer)
+        self.timer_id = self.tk_top.after(500, self.__update_by_timer)
 
 
     def __destroy_window(self):
-        global prev_dialog_wid
         tk_utils.safe_destroy(self.wid_top)
-        self.tk.after_cancel(self.timer_id)
-        prev_dialog_wid = None
+        self.tk_top.after_cancel(self.timer_id)
+        JobListDialog.__destroyed_dialog()
 
 
     def raise_window(self):
+        """ Raises the dialog window above all other windows."""
         self.wid_top.wm_deiconify()
         self.wid_top.lift()
 
 
     def __create_dialog_window(self):
-        self.wid_top = tk.Toplevel(self.tk)
+        self.wid_top = tk.Toplevel(self.tk_top)
         self.wid_top.wm_title("GtestGui: Test job list")
-        self.wid_top.wm_group(self.tk)
+        self.wid_top.wm_group(self.tk_top)
 
-        self.__create_table_widget()
+        self.wid_table, self.wid_header = self.__create_table_widget()
 
         self.wid_top.bind("<ButtonRelease-3>", lambda e: self.__post_context_menu(e.widget,
                                                                                   e.x, e.y))
         self.wid_top.bind("<Configure>", lambda e: self.__handle_window_resize(e.widget))
         self.wid_top.bind("<Destroy>", lambda e: self.__destroy_window())
 
-        self.wid_header.tag_configure("head", font=tk_utils.font_content_bold,
-                                      spacing1=2, spacing3=5, lmargin1=5)
+        self.wid_header.tag_configure("head", font=tk_utils.font_content_bold, lmargin1=5)
         self.wid_table.tag_configure("body", lmargin1=5)
         self.wid_table.tag_configure("bold", font=tk_utils.font_content_bold)
 
         self.wid_header.insert("0.0", "\t".join(self.table_header_txt), "head", "\n", [])
         self.__update_column_widths()
 
-        self.sel_obj = wid_text_sel.Text_sel_wid(self.wid_table,
-                                                 self.__handle_selection_change, self.__get_len)
+        self.sel_obj = TextSelWidget(self.wid_table, self.__handle_selection_change, self.__get_len)
 
-        if config_db.job_list_geometry:
-            self.wid_top.wm_geometry(config_db.job_list_geometry)
+        if config_db.get_opt("job_list_geometry"):
+            self.wid_top.wm_geometry(config_db.get_opt("job_list_geometry"))
 
         self.wid_table.focus_set()
 
 
     def __create_table_widget(self):
         initial_height = 10
 
@@ -121,75 +131,83 @@
         wid_table.configure(yscrollcommand=wid_sb.set)
         wid_sb.pack(side=tk.LEFT, fill=tk.Y)
         wid_frm1.pack(side=tk.TOP, fill=tk.BOTH, expand=1)
 
         wid_header.bindtags([wid_header, self.wid_top, "all"])
         wid_table.bindtags([wid_table, self.wid_top, "TextSel", "all"])
 
-        self.wid_table = wid_table
-        self.wid_header = wid_header
+        return (wid_table, wid_header)
 
 
     def __update_column_widths(self):
         char_w = tk_utils.font_content.measure("0")
-        if char_w == 0: char_w = 15
+        if char_w == 0:
+            char_w = 15
 
         title_text = self.table_header_txt
         tab_widths = [tk_utils.font_content_bold.measure(x) + 2*char_w for x in title_text]
 
         max_width = tk_utils.font_content.measure("9999999") + 2*char_w
         if max_width > tab_widths[0]:
             tab_widths[0] = max_width
 
         max_width = tk_utils.font_content.measure("99999999") + 2*char_w
-        if max_width > tab_widths[1]:
-            tab_widths[1] = max_width
+        if max_width > tab_widths[2]:
+            tab_widths[2] = max_width
+
+        max_width = tk_utils.font_content.measure("100%") + 2*char_w
+        if max_width > tab_widths[4]:
+            tab_widths[4] = max_width
 
         max_width = max([tk_utils.font_content.measure(x)
-                            for x in test_db.test_case_names]) + 2*char_w
-        if max_width > tab_widths[3]:
-            tab_widths[3] = max_width
+                         for x in test_db.test_case_names]) + 2*char_w
+        if max_width > tab_widths[5]:
+            tab_widths[5] = max_width
 
         off = char_w + tab_widths[0]
-        tabs = [off + tab_widths[1]/2, "center",
-                off + tab_widths[1] + tab_widths[2]/2, "center",
-                off + tab_widths[1] + tab_widths[2] + char_w, "left"]
+        tabs = []
+        for width in tab_widths[1:5]:
+            tabs.extend([off + width/2, "center"])
+            off += width
+        tabs.extend([off + char_w, "left"])
 
         self.wid_header.tag_configure("head", font=tk_utils.font_content_bold, tabs=tabs,
-                                      spacing1=2, spacing3=5, lmargin1=5)
+                                      lmargin1=5)
         self.wid_table.tag_configure("body", tabs=tabs, lmargin1=5)
 
         # Convert pixel width to a character count (assuming "0" has average char width)
         nof_chars = (sum(tab_widths) + char_w * 3 - 1) // char_w
 
         self.wid_header.configure(width=nof_chars)
         self.wid_table.configure(width=nof_chars)
 
 
     def __handle_window_resize(self, wid):
         if wid == self.wid_top:
             new_size = self.wid_top.wm_geometry()
-            if new_size != config_db.job_list_geometry:
-                config_db.job_list_geometry = new_size
-                config_db.rc_file_update_after_idle()
+            config_db.set_opt("job_list_geometry", new_size)
 
 
-    def __format_table_row(self, stats):
-        msg = "%d\t%d\t%d\t%s\n" % (stats[0], stats[2], stats[3], stats[4])
+    @staticmethod
+    def __format_table_row(stats):
+        perc_done = (100 * stats[4]) // stats[5] if stats[5] else 100
+        is_bg_job = "yes" if stats[2] else "no"
+        msg = ("%d\t%s\t%d\t%d\t%d%%\t%s\n" %
+               (stats[0], is_bg_job, stats[3], stats[4], perc_done, stats[6]))
         return [msg, "body"]
 
 
     def __populate_table(self):
         self.sel_obj.text_sel_set_selection([])
         self.wid_table.delete("1.0", "end")
 
-        self.job_stats = gtest.gtest_ctrl.get_job_stats()
+        self.job_stats = gtest_ctrl.gtest_ctrl.get_job_stats()
         if self.job_stats:
-            for idx in range(len(self.job_stats)):
-                msg = self.__format_table_row(self.job_stats[idx])
+            for stat in self.job_stats:
+                msg = JobListDialog.__format_table_row(stat)
                 self.wid_table.insert("end", *msg)
         else:
             self.wid_table.insert("end", "\nCurrently, no jobs are running\n")
 
 
     def __update_by_timer(self):
         sel_pids = [self.job_stats[x][0] for x in self.sel_obj.text_sel_get_selection()]
@@ -201,45 +219,49 @@
         for pid in sel_pids:
             try:
                 new_sel.append(new_pids.index(pid))
             except ValueError:
                 pass
         self.sel_obj.text_sel_set_selection(new_sel)
 
-        self.timer_id = self.tk.after(500, self.__update_by_timer)
+        self.timer_id = self.tk_top.after(500, self.__update_by_timer)
 
 
     def __handle_selection_change(self, sel):
+        # abstract interface: unused parameter needed by other classes
+        # pylint: disable=unused-argument
         self.sel_obj.text_sel_copy_clipboard(False)
 
 
     def __get_len(self):
         return len(self.job_stats)
 
 
     def __post_context_menu(self, parent, xcoo, ycoo):
         wid_men = tk_utils.get_context_menu_widget()
 
-        if (parent == self.wid_table) and gtest.gtest_ctrl.is_active():
+        if (parent == self.wid_table) and gtest_ctrl.gtest_ctrl.is_active():
             self.sel_obj.text_sel_context_selection(xcoo, ycoo)
             sel = self.sel_obj.text_sel_get_selection()
             if sel:
                 if len(sel) == 1:
                     wid_men.add_command(label="Open trace output file",
                                         command=lambda file_name=self.job_stats[sel[0]][1]:
-                                            self.__do_open_trace(file_name))
+                                        JobListDialog.__do_open_trace(file_name))
                     wid_men.add_separator()
 
                 wid_men.add_command(label="Send ABORT signal to selected processes",
                                     command=lambda pids=[self.job_stats[x][0] for x in sel]:
-                                            self.__do_abort_jobs(pids))
+                                    JobListDialog.__do_abort_jobs(pids))
 
                 tk_utils.post_context_menu(parent, xcoo, ycoo)
 
 
-    def __do_abort_jobs(self, pids):
+    @staticmethod
+    def __do_abort_jobs(pids):
         for pid in pids:
-          gtest.gtest_ctrl.abort_job(pid)
+            gtest_ctrl.gtest_ctrl.abort_job(pid)
 
 
-    def __do_open_trace(self, trace_file_name):
-        dlg_browser.show_trace(self.tk, trace_file_name)
+    @staticmethod
+    def __do_open_trace(trace_file_name):
+        dlg_browser.show_trace(trace_file_name)
```

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/dlg_main.py` & `mote-gtest-gui-0.9.0/gtest_gui/dlg_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,52 +13,66 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
+"""
+Implements the main window class.
+"""
+
 import os
 from datetime import datetime
 
 import tkinter as tk
 from tkinter import messagebox as tk_messagebox
 from tkinter import filedialog as tk_filedialog
 
+from gtest_gui.dlg_config import ConfigDialog
+from gtest_gui.dlg_debug import DebugDialog
+from gtest_gui.dlg_font_sel import FontSelectionDialog
+from gtest_gui.dlg_job_list import JobListDialog
+from gtest_gui.dlg_tc_list import TcListDialog
+from gtest_gui.dlg_help import HelpDialog
+
+from gtest_gui.wid_test_ctrl import TestControlWidget
+from gtest_gui.wid_test_log import TestLogWidget
+from gtest_gui.wid_status_line import StatusLineWidget
+
+import gtest_gui.gtest_ctrl as gtest_ctrl
+import gtest_gui.gtest_list_tests as gtest_list_tests
 import gtest_gui.config_db as config_db
-import gtest_gui.dlg_config as dlg_config
-import gtest_gui.dlg_debug as dlg_debug
-import gtest_gui.dlg_font_sel as dlg_font_sel
-import gtest_gui.dlg_job_list as dlg_job_list
-import gtest_gui.dlg_tc_list as dlg_tc_list
-import gtest_gui.dlg_help as dlg_help
-import gtest_gui.gtest as gtest
 import gtest_gui.test_db as test_db
+import gtest_gui.trace_db as trace_db
 import gtest_gui.tk_utils as tk_utils
-import gtest_gui.wid_status_line as wid_status_line
-import gtest_gui.wid_test_ctrl as wid_test_ctrl
-import gtest_gui.wid_test_log as wid_test_log
 import gtest_gui.wid_tool_tip as wid_tool_tip
 
 
 wid_test_ctrl_ = None
 wid_test_log_ = None
 
-class Main_window(object):
+class MainWindow:
+    """
+    Main window class (singleton): This class manages the main menubar and its
+    commands. It also is a container for the test control and test result log
+    widgets, which it creates at start-up.
+    """
+
     def __init__(self, tk_top, exe_name):
-        self.tk = tk_top
+        self.tk_top = tk_top
 
         global wid_test_ctrl_
-        wid_test_ctrl_ = wid_test_ctrl.Test_control_widget(tk_top, tk_top)
+        wid_test_ctrl_ = TestControlWidget(tk_top, tk_top)
         wid_test_ctrl_.get_widget().pack(side=tk.TOP, fill=tk.BOTH)
 
-        wid_status_line.create_widget(tk_top, wid_test_ctrl_.get_widget())
+        StatusLineWidget.create_widget(tk_top, wid_test_ctrl_.get_widget())
 
         global wid_test_log_
-        wid_test_log_ = wid_test_log.Test_log_widget(tk_top, tk_top)
+        wid_test_log_ = TestLogWidget(tk_top, tk_top)
         wid_test_log_.get_widget().pack(side=tk.TOP, fill=tk.BOTH, expand=1)
 
         wid_test_log_.set_wid_test_ctrl(wid_test_ctrl_)
         wid_test_ctrl_.set_wid_test_log(wid_test_log_)
 
         self.__create_menubar()
 
@@ -69,147 +83,151 @@
 
         # Bindings that apply to all widgets in the main window
         tk_top.bind("<Control-Key-r>", lambda e: wid_test_ctrl_.start_campaign())
         tk_top.bind("<Control-Key-s>", lambda e: wid_test_ctrl_.stop_campaign())
         tk_top.bind("<Control-Key-q>", lambda e: wid_test_ctrl_.resume_campaign())
         tk_top.bind("<Control-Key-t>", lambda e: wid_test_ctrl_.start_repetition())
 
-        tk_top.protocol(name="WM_DELETE_WINDOW", func=self.quit)
+        tk_top.protocol(name="WM_DELETE_WINDOW", func=self.__quit)
 
 
     def __create_menubar(self):
-        wid_men = tk.Menu(self.tk, name="menubar", tearoff=0)
-        self.var_opt_test_ctrl = tk.BooleanVar(self.tk, True)
-        self.var_opt_tool_tips = tk.BooleanVar(self.tk, config_db.options["enable_tool_tips"])
+        wid_men = tk.Menu(self.tk_top, name="menubar", tearoff=0)
+        self.var_opt_test_ctrl = tk.BooleanVar(self.tk_top, True)
+        self.var_opt_tool_tips = tk.BooleanVar(self.tk_top, config_db.get_opt("enable_tool_tips"))
 
-        wid_tool_tip.enable_tips(config_db.options["enable_tool_tips"])
+        wid_tool_tip.enable_tips(config_db.get_opt("enable_tool_tips"))
 
         wid_men_ctrl = wid_tool_tip.Menu(wid_men, tearoff=0)
         wid_men.add_cascade(menu=wid_men_ctrl, label="Control", underline=0)
         # Included here only for documenting the keyboard shortcut
         wid_men_ctrl.add_command(label="Start tests", tooltip="test_ctrl.cmd_start_campaign",
                                  command=wid_test_ctrl_.start_campaign, accelerator="Ctrl-r")
         wid_men_ctrl.add_command(label="Stop tests", tooltip="test_ctrl.cmd_stop_campaign",
                                  command=wid_test_ctrl_.stop_campaign, accelerator="Ctrl-s")
         wid_men_ctrl.add_command(label="Resume tests", tooltip="test_ctrl.cmd_resume_campaign",
                                  command=wid_test_ctrl_.resume_campaign, accelerator="Ctrl-q")
         wid_men_ctrl.add_command(label="Repeat tests", tooltip="test_ctrl.cmd_repeat",
                                  command=wid_test_ctrl_.start_repetition, accelerator="Ctrl-t")
         wid_men_ctrl.add_separator()
         wid_men_ctrl.add_command(label="Open test case list...", tooltip="test_ctrl.cmd_tc_list",
-                                 command=lambda: dlg_tc_list.create_dialog(self.tk, wid_test_ctrl_))
+                                 command=lambda: TcListDialog.create_dialog(
+                                     self.tk_top, wid_test_ctrl_))
         wid_men_ctrl.add_command(label="Open job list...", tooltip="test_ctrl.cmd_job_list",
-                                 command=lambda: dlg_job_list.create_dialog(self.tk))
+                                 command=lambda: JobListDialog.create_dialog(self.tk_top))
         wid_men_ctrl.add_separator()
         wid_men_ctrl.add_command(label="Refresh test case list", tooltip="test_ctrl.cmd_refresh",
                                  command=self.reload_exe)
         wid_men_set_exe = wid_tool_tip.Menu(wid_men_ctrl, tearoff=0,
                                             postcommand=self.__fill_prev_exe_menu)
         wid_men_ctrl.add_cascade(menu=wid_men_set_exe, label="Select test executable")
         wid_men_set_exe.add_command(label="Select executable file...", command=self.select_exe)
         wid_men_ctrl.add_separator()
-        wid_men_ctrl.add_command(label="Quit", command=self.quit)
+        wid_men_ctrl.add_command(label="Quit", command=self.__quit)
 
         wid_men_cfg = wid_tool_tip.Menu(wid_men, tearoff=0)
         wid_men.add_cascade(menu=wid_men_cfg, label="Configure", underline=1)
         wid_men_cfg.add_command(label="Options...",
-                                command=lambda: dlg_config.create_dialog(self.tk))
+                                command=lambda: ConfigDialog.create_dialog(self.tk_top))
         wid_men_cfg.add_separator()
         wid_men_cfg.add_command(label="Select font for result log...",
                                 tooltip="config.select_font_content",
-                                command=lambda: dlg_font_sel.create_dialog(
-                                            self.tk, "content",
-                                            tk_utils.font_content, self.__change_font))
+                                command=lambda: FontSelectionDialog.create_dialog(
+                                    self.tk_top, "content",
+                                    tk_utils.font_content, MainWindow.__change_font))
         wid_men_cfg.add_command(label="Select font for trace preview...",
                                 tooltip="config.select_font_trace",
-                                command=lambda: dlg_font_sel.create_dialog(
-                                            self.tk, "trace",
-                                            tk_utils.font_trace, self.__change_font))
+                                command=lambda: FontSelectionDialog.create_dialog(
+                                    self.tk_top, "trace",
+                                    tk_utils.font_trace, MainWindow.__change_font))
         wid_men_cfg.add_separator()
         wid_men_cfg.add_checkbutton(label="Show test controls", tooltip="config.show_controls",
                                     command=self.show_test_ctrl, variable=self.var_opt_test_ctrl)
         wid_men_cfg.add_checkbutton(label="Show tool tip popups", tooltip="config.show_tool_tips",
                                     command=self.toggle_tool_tips, variable=self.var_opt_tool_tips)
 
         wid_men_log = wid_tool_tip.Menu(wid_men, tearoff=0)
         wid_men.add_cascade(menu=wid_men_log, label="Result log", underline=0)
         wid_test_log_.add_menu_commands(wid_men_log)
 
-        self.tk.eval("option add *Menu.useMotifHelp true")
+        self.tk_top.eval("option add *Menu.useMotifHelp true")
         wid_men_help = tk.Menu(wid_men, name="help", tearoff=0)
         wid_men.add_cascade(menu=wid_men_help, label="Help", underline=0)
-        dlg_help.add_menu_commands(self.tk, wid_men_help)
+        HelpDialog.add_menu_commands(self.tk_top, wid_men_help)
         wid_men_help.add_separator()
         wid_men_help.add_command(label="Debug console",
-                                 command=lambda: dlg_debug.create_dialog(self.tk, globals()))
-        wid_men_help.add_command(label="About",
-                                 command=self.show_about_dialog)
+                                 command=lambda: DebugDialog.create_dialog(self.tk_top, globals()))
+        wid_men_help.add_command(label="About", command=self.__show_about_dialog)
 
-        self.var_prev_exe_name = tk.StringVar(self.tk, "")
+        self.var_prev_exe_name = tk.StringVar(self.tk_top, "")
         self.wid_men_set_exe = wid_men_set_exe
-        self.tk.config(menu=wid_men)
+        self.tk_top.config(menu=wid_men)
+
 
+    def __quit(self):
+        if gtest_ctrl.gtest_ctrl.is_active():
+            msg = "Really stop tests and quit?"
+            if not tk_messagebox.askokcancel(parent=self.tk_top, message=msg):
+                return False
 
-    def quit(self):
-        if gtest.gtest_ctrl.is_active():
-            if not tk_messagebox.askokcancel(parent=self.tk, message="Really stop tests and quit?"):
-                return
+        config_db.rc_file_update_synchronously()
 
-        config_db.rc_file_update_upon_exit()
-        gtest.gtest_ctrl.stop(kill=True)
-        gtest.release_exe_file_copy()
-        if config_db.options["exit_clean_trace"]:
-            gtest.clean_all_trace_files()
+        gtest_ctrl.gtest_ctrl.stop(kill=True)
+        trace_db.release_exe_file_copy()
+        if config_db.get_opt("exit_clean_trace"):
+            trace_db.clean_all_trace_files()
 
-        tk_utils.safe_destroy(self.tk)
+        tk_utils.safe_destroy(self.tk_top)
         return True
 
 
     def __check_tests_active(self):
-        if gtest.gtest_ctrl.is_active():
+        if gtest_ctrl.gtest_ctrl.is_active():
             msg = "This operation requires stopping ongoing tests."
-            if not tk_messagebox.askokcancel(parent=self.tk, message=msg):
-                return True
-            gtest.gtest_ctrl.stop(kill=True)
-        return False
+            if not tk_messagebox.askokcancel(parent=self.tk_top, message=msg):
+                return False
+            gtest_ctrl.gtest_ctrl.stop(kill=True)
+        return True
 
 
-    def __change_font(self, foo):
+    @staticmethod
+    def __change_font(_font):
         tk_utils.update_derived_fonts()
-        config_db.rc_file_update()
+        config_db.update_fonts()
 
 
     @staticmethod
     def __get_unique_prev_exe_name(input_paths, mapped):
         # Build reverse list of path elements: split at separators
         input_paths = sorted(input_paths)
         path_lists = []
         for path in input_paths:
             path_list = []
             while path:
-                p1, p2 = os.path.split(path)
-                if not p2 or p1 == os.path.sep:
+                part1, part2 = os.path.split(path)
+                if not part2 or part1 == os.path.sep:
                     path_list.append(path)
                     break
-                path_list.append(p2)
-                path = p1
+                path_list.append(part2)
+                path = part1
 
             path_lists.append(path_list)
 
         # Determine indices where paths differ
         delta_sets = [set() for x in path_lists]
         for idx1 in range(len(path_lists) - 1):
             prev_path_list = path_lists[idx1]
             idx2 = 0
             for path_list in path_lists[idx1:]:
+                # pylint: disable=consider-using-enumerate
                 for idx in range(0, len(path_list)):
                     if idx >= len(prev_path_list):
                         delta_sets[idx2].add(idx)
                         break
-                    elif path_list[idx] != prev_path_list[idx]:
+                    if path_list[idx] != prev_path_list[idx]:
                         delta_sets[idx1].add(idx)
                         delta_sets[idx2].add(idx)
                         break
                 idx2 += 1
 
         # Reassemble paths, while skipping equal elements
         idx1 = 0
@@ -239,145 +257,152 @@
             base = os.path.basename(exe_name)
             if base_names.get(base) is None:
                 base_names[os.path.basename(exe_name)] = [exe_name]
             else:
                 base_names[os.path.basename(exe_name)].append(exe_name)
 
         mapped = {}
-        for base_name, paths in base_names.items():
+        for paths in base_names.values():
             if len(paths) > 1:
-                Main_window.__get_unique_prev_exe_name(paths, mapped)
+                MainWindow.__get_unique_prev_exe_name(paths, mapped)
             else:
                 mapped[paths[0]] = os.path.basename(paths[0])
 
         return mapped
 
 
     def __fill_prev_exe_menu(self):
         end_idx = self.wid_men_set_exe.index("end")
         if int(end_idx) > 0:
             self.wid_men_set_exe.delete(1, "end")
 
         self.var_prev_exe_name.set(test_db.test_exe_name)
 
-        mapped = Main_window.__get_prev_exe_names(config_db.prev_exe_file_list)
+        prev_exe_file_list = config_db.get_opt("prev_exe_file_list")
+        mapped = MainWindow.__get_prev_exe_names(prev_exe_file_list)
         need_sep = True
-        for exe_name in reversed(config_db.prev_exe_file_list):
+        for exe_name in reversed(prev_exe_file_list):
             if need_sep:
                 self.wid_men_set_exe.add_separator()
                 need_sep = False
 
             tip_text = exe_name + "\n"
             try:
                 exe_ts = os.stat(exe_name).st_mtime
                 # RFC 2822-compliant date format
                 tip_text += datetime.fromtimestamp(exe_ts).strftime("Timestamp: %a, %d %b %Y %T %z")
                 state = tk.NORMAL
-            except OSError as e:
+            except OSError:
                 tip_text += "File not found"
                 state = tk.DISABLED
 
             self.wid_men_set_exe.add_radiobutton(
                 label=mapped[exe_name], state=state,
                 variable=self.var_prev_exe_name, value=exe_name,
                 tooltip=lambda tip_text=tip_text: tip_text,
                 command=lambda path=exe_name: self.__select_prev_exe(path))
 
 
     def select_exe(self):
-        if self.__check_tests_active():
+        """ Opens a file selection dialog for selecting the test executable."""
+
+        if not self.__check_tests_active():
             return
 
         def_name = test_db.test_exe_name
         if not os.path.isfile(def_name):
             def_name = ""
 
-        if (os.name == "posix"):
+        if os.name == "posix":
             filetypes = [("all", "*"), ("Executable", "*.exe")]
         else:
             filetypes = [("Executable", "*.exe"), ("all", "*")]
 
         filename = tk_filedialog.askopenfilename(
-                        parent=self.tk, filetypes=filetypes,
+                        parent=self.tk_top, filetypes=filetypes,
                         title="Select test executable",
                         initialfile=os.path.basename(def_name),
                         initialdir=os.path.dirname(def_name))
         if filename:
             self.__update_executable(filename)
 
 
     def reload_exe(self):
-        if self.__check_tests_active():
+        """ Checks for a change of the current executable file and if changed,
+            reads the test case list from it if changed.
+        """
+
+        if not self.__check_tests_active():
             return
 
         if test_db.test_exe_name:
             self.__update_executable(test_db.test_exe_name)
         else:
             self.select_exe()
 
 
     def __select_prev_exe(self, filename):
-        if self.__check_tests_active():
+        if not self.__check_tests_active():
             return
         self.__update_executable(filename)
 
 
     def __update_executable(self, filename):
         try:
             exe_ts = int(os.stat(filename).st_mtime)  # cast away sub-second fraction
-        except OSError as e:
-            tk_messagebox.showerror(parent=self.tk,
-                                    message="Failed to access executable: " + str(e))
+        except OSError as exp:
+            tk_messagebox.showerror(parent=self.tk_top,
+                                    message="Failed to access executable: " + str(exp))
             return
 
         prev_exe = test_db.test_exe_name
         prev_names = test_db.test_case_names
 
-        tc_names = gtest.gtest_list_tests(exe_file=filename)
+        tc_names = gtest_list_tests.gtest_list_tests(exe_file=filename)
         if tc_names is None:
             return
 
         if filename != test_db.test_exe_name:
-            self.tk.wm_title("GtestGui: " + os.path.basename(filename))
-            gtest.release_exe_file_copy()
-            test_db.update_executable(filename, exe_ts, tc_names)
-
+            self.tk_top.wm_title("GtestGui: " + os.path.basename(filename))
+            trace_db.release_exe_file_copy()
             config_db.update_prev_exe_file_list(filename)
 
+        test_db.update_executable(filename, exe_ts, tc_names)
+
         if prev_exe: # no message during startup
             if prev_exe != filename:
-                wid_status_line.show_message("info", "Switched to new executable.")
+                StatusLineWidget.get().show_message("info", "Switched to new executable.")
             elif prev_names != test_db.test_case_names:
-                wid_status_line.show_message("info", "New test case list loaded.")
+                StatusLineWidget.get().show_message("info", "New test case list loaded.")
             else:
-                wid_status_line.show_message("warning", "Test case list is unchanged.")
+                StatusLineWidget.get().show_message("warning", "Test case list is unchanged.")
 
 
-    def show_about_dialog(self):
-        wid_about = tk.Toplevel(self.tk, name="dlg_about")
+    def __show_about_dialog(self):
+        wid_about = tk.Toplevel(self.tk_top, name="dlg_about")
 
-        wid_about.wm_transient(self.tk)
+        wid_about.wm_transient(self.tk_top)
         wid_about.wm_resizable(1, 1)
-        wid_about.wm_group(self.tk)
+        wid_about.wm_group(self.tk_top)
         wid_about.wm_title("About Gtest GUI")
 
         wid_lab1 = tk.Label(wid_about, text="Module tester's GoogleTest GUI",
                             font=tk_utils.font_bold)
         wid_lab1.pack(side=tk.TOP, pady=5)
 
-        wid_lab2 = tk.Label(wid_about, text="Version 0.8.1\n"
+        wid_lab2 = tk.Label(wid_about, text="Version 0.9.0\n"
                                             "Copyright (C) 2023 T. Zoerner")
         wid_lab2.pack(side=tk.TOP)
 
         url = "https://github.com/tomzox/gtest_gui"
         wid_lab3 = tk.Label(wid_about, text=url, fg="blue",
                             cursor="top_left_arrow")
         wid_lab3.pack(side=tk.TOP, pady=5)
 
-        msg ="""
+        msg = """
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
         wid_lab4 = tk.Message(wid_about, font=tk_utils.font_normal, text=msg)
@@ -389,24 +414,27 @@
         wid_but.bind("<Return>", lambda e: e.widget.event_generate("<Key-space>"))
         wid_but.bind("<Escape>", lambda e: e.widget.event_generate("<Key-space>"))
         wid_lab3.bind("<ButtonRelease-1>", lambda e: tk_utils.xselection_export(url, True))
         wid_but.focus_set()
 
 
     def show_test_ctrl(self):
-        geom = self.tk.wm_geometry()
-        self.tk.wm_geometry(geom)
+        """ Show or hide of the test control frame in the main window after config changes."""
+        geom = self.tk_top.wm_geometry()
+        self.tk_top.wm_geometry(geom)
 
         if self.var_opt_test_ctrl.get():
             wid_test_log_.toggle_test_ctrl_visible(True)
             wid_test_ctrl_.get_widget().pack(
                 side=tk.TOP, fill=tk.BOTH, before=wid_test_log_.get_widget())
         else:
             wid_test_log_.toggle_test_ctrl_visible(False)
             wid_test_ctrl_.get_widget().forget()
 
 
     def toggle_tool_tips(self):
-        config_db.options["enable_tool_tips"] = self.var_opt_tool_tips.get()
-        config_db.rc_file_update_after_idle()
+        """ Reconfigure tool-tip widget to show or hide tool-tips after config changes."""
+
+        new_val = self.var_opt_tool_tips.get()
+        config_db.set_opt("enable_tool_tips", new_val)
 
-        wid_tool_tip.enable_tips(config_db.options["enable_tool_tips"])
+        wid_tool_tip.enable_tips(new_val)
```

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/dlg_tc_list.py` & `mote-gtest-gui-0.9.0/gtest_gui/wid_text_sel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 # ------------------------------------------------------------------------ #
-# Copyright (C) 2023 Th. Zoerner
+# Copyright (C) 2007-2010,2019-2023 Th. Zoerner
 # ------------------------------------------------------------------------ #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -13,512 +13,535 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
-#
-# This class implements the test case list dialog.
-#
-
-from enum import Enum
-import os
-import tkinter as tk
-from tkinter import messagebox as tk_messagebox
-from tkinter import filedialog as tk_filedialog
-
-import gtest_gui.bisect as bisect
-import gtest_gui.config_db as config_db
-import gtest_gui.filter_expr as filter_expr
-import gtest_gui.gtest as gtest
-import gtest_gui.test_db as test_db
-import gtest_gui.tk_utils as tk_utils
-import gtest_gui.wid_test_ctrl as wid_test_ctrl
-import gtest_gui.wid_text_sel as wid_text_sel
-
-
-prev_dialog_wid = None
-prev_export_filename = ""
-
-class Sort_mode(Enum):
-    by_name = 0
-    by_exec_cnt = 1
-    by_fail_cnt = 2
-    by_duration = 3
-
-
-def create_dialog(tk_top, test_ctrl):
-    global prev_dialog_wid
-
-    if not test_db.test_case_names:
-        tk_messagebox.showerror(parent=tk_top, message="Test case list is empty.")
-        return
-
-    if not test_ctrl.check_filter_expression():
-        return
-
-    if prev_dialog_wid and tk_utils.wid_exists(prev_dialog_wid.wid_top):
-        prev_dialog_wid.raise_window()
-    else:
-        prev_dialog_wid = Tc_list_dialog(tk_top, test_ctrl)
-
-
-class Tc_list_dialog(object):
-    def __init__(self, tk_top, test_ctrl):
-        self.tk = tk_top
-        self.test_ctrl = test_ctrl
-        self.table_header_txt = ("Run", "Name", "Passed", "Failed", "Exec time")
-        self.opt_sort_modes = []
-
-        self.__create_dialog_window()
-        self.__handle_filter_change()
-
-        test_db.Test_db_slots.tc_stats_update = self.__handle_tc_stats_update
-        test_db.Test_db_slots.tc_names_update = self.__handle_tc_names_update
-        test_db.Test_db_slots.campaign_stats_reset = self.__handle_campaign_status_change
-        self.test_ctrl.register_filter_change_slot(self.__handle_main_tc_filter_expr_change)
-
-
-    def __destroy_window(self):
-        global prev_dialog_wid
-        test_db.Test_db_slots.tc_stats_update = None
-        test_db.Test_db_slots.tc_names_update = None
-        test_db.Test_db_slots.campaign_stats_reset = None
-
-        self.test_ctrl.register_filter_change_slot(None)
-
-        tk_utils.safe_destroy(self.wid_top)
-        prev_dialog_wid = None
-
-
-    def raise_window(self):
-        self.wid_top.wm_deiconify()
-        self.wid_top.lift()
-
-
-    def __create_dialog_window(self):
-        self.wid_top = tk.Toplevel(self.tk)
-        self.wid_top.wm_title("GtestGui: Test case list")
-        self.wid_top.wm_group(self.tk)
-
-        self.var_filter_run = tk.BooleanVar(self.tk, False)
-        self.var_filter_failed = tk.BooleanVar(self.tk, False)
-        self.var_filter_disabled = tk.BooleanVar(self.tk, False)
-
-        self.var_sort_name = tk.BooleanVar(self.tk, False)
-        self.var_sort_exec_cnt = tk.BooleanVar(self.tk, False)
-        self.var_sort_fail_cnt = tk.BooleanVar(self.tk, False)
-        self.var_sort_duration = tk.BooleanVar(self.tk, False)
-
-        self.__create_table_widget()
-
-        self.wid_table.bind("<Key-Return>", lambda e: self.__do_filter_selected_tests(True))
-        self.wid_table.bind("<Key-Delete>", lambda e: self.__do_filter_selected_tests(False))
-        self.wid_table.bind("<FocusIn>", lambda e: self.test_ctrl.check_filter_expression(False))
-
-        self.wid_top.bind("<ButtonRelease-3>", lambda e: self.__post_context_menu(e.widget, e.x, e.y))
-        self.wid_top.bind("<Configure>", lambda e: self.__handle_window_resize(e.widget))
-        self.wid_top.bind("<Destroy>", lambda e: self.__destroy_window())
-
-        self.wid_header.tag_configure("head", font=tk_utils.font_content_bold,
-                                      lmargin1=5, spacing1=2, spacing3=5)
-        self.wid_table.tag_configure("body", lmargin1=5)
-        self.wid_table.tag_configure("bold", font=tk_utils.font_content_bold)
-
-        self.wid_header.insert("0.0", "\t".join(self.table_header_txt), "head", "\n", [])
-        self.__update_column_widths()
-
-        self.sel_obj = wid_text_sel.Text_sel_wid(self.wid_table,
-                                                 self.__handle_selection_change, self.__get_len)
-
-        if config_db.tc_list_geometry:
-            self.wid_top.wm_geometry(config_db.tc_list_geometry)
-
-        self.wid_table.focus_set()
-
-
-    def __create_table_widget(self):
-        initial_height = min(40, len(test_db.test_case_names) + 1)
-
-        wid_frm1 = tk.Frame(self.wid_top)
-        wid_frm2 = tk.Frame(wid_frm1, borderwidth=2, relief=tk.SUNKEN)
-        wid_header = tk.Text(wid_frm2, height=1, font=tk_utils.font_content,
-                             insertofftime=0, wrap=tk.NONE, cursor="top_left_arrow",
-                             exportselection=0, relief=tk.FLAT, takefocus=0)
-        wid_table = tk.Text(wid_frm2, height=initial_height, font=tk_utils.font_content,
-                            insertofftime=0, wrap=tk.NONE, cursor="top_left_arrow",
-                            exportselection=0, relief=tk.FLAT)
-        wid_header.pack(side=tk.TOP, fill=tk.X)
-        wid_table.pack(side=tk.TOP, fill=tk.BOTH, expand=1)
-        wid_frm2.pack(side=tk.LEFT, fill=tk.BOTH, expand=1)
-
-        wid_sb = tk.Scrollbar(wid_frm1, orient=tk.VERTICAL, command=wid_table.yview, takefocus=0)
-        wid_table.configure(yscrollcommand=wid_sb.set)
-        wid_sb.pack(side=tk.LEFT, fill=tk.Y)
-        wid_frm1.pack(side=tk.TOP, fill=tk.BOTH, expand=1)
-
-        wid_header.bindtags([wid_header, self.wid_top, "all"])
-        wid_table.bindtags([wid_table, self.wid_top, "TextSel", "all"])
-
-        self.wid_table = wid_table
-        self.wid_header = wid_header
-
+# This code is copied from Trace Browser (trowser.py)
 
-    def __update_column_widths(self):
-        char_w = tk_utils.font_content.measure("0")
-        if char_w == 0: char_w = 15
+""" Implements the TextSelWidget class. """
 
-        title_text = self.table_header_txt
-        tab_widths = [tk_utils.font_content_bold.measure(x) + 2*char_w for x in title_text]
-
-        tc_max_width = max([tk_utils.font_content.measure(x)
-                                for x in test_db.test_case_names]) + 2*char_w
-        if tc_max_width > tab_widths[1]:
-            tab_widths[1] = tc_max_width
-
-        tabs = [char_w + tab_widths[0], "left"]
-        off = tab_widths[0] + tab_widths[1]
-        for width in tab_widths[2:]:
-            tabs.extend([off + width/2, "center"])
-            off += width
-
-        self.wid_header.tag_configure("head", font=tk_utils.font_content_bold, tabs=tabs,
-                                      lmargin1=5, spacing1=2, spacing3=5)
-        self.wid_table.tag_configure("body", tabs=tabs, lmargin1=5)
-
-        # Convert pixel width to a character count (assuming "0" has average char width)
-        nof_chars = (off + char_w - 1) // char_w
-
-        self.wid_header.configure(width=nof_chars)
-        self.wid_table.configure(width=nof_chars)
-
-
-    def __handle_window_resize(self, wid):
-        if wid == self.wid_top:
-            new_size = self.wid_top.wm_geometry()
-            if new_size != config_db.tc_list_geometry:
-                config_db.tc_list_geometry = new_size
-                config_db.rc_file_update_after_idle()
-
-
-    def __format_table_row(self, tc_name):
-        tc_stats = test_db.test_case_stats[tc_name]
-        txt = []
-
-        ena = "yes\t" if tc_name in self.tc_enabled else "no\t"
-        txt.extend([ena + tc_name, "body"])
-
-        nof_pass = tc_stats[0]
-        if nof_pass > 0:
-            txt.extend(["\t%d" % nof_pass, ["body", "bold"]])
-        else:
-            txt.extend(["\t%d" % nof_pass, "body"])
+import gtest_gui.tk_utils as tk_utils
 
-        nof_fail = tc_stats[1]
-        if nof_fail > 0:
-            txt.extend(["\t%d" % nof_fail, ["body", "bold"]])
+class TextSelWidget:
+    """
+    This class allows using a text widget in the way of a listbox, i.e.
+    allowing to select one or more lines. The mouse bindings are similar to the
+    Tk listbox in "extended" mode. The cursor key bindings differ from the
+    listbox, as there is no "active" element (i.e. there's no separate cursor
+    from the selection.)
+    """
+
+    def __init__(self, wid, cb_proc, len_proc, mode="extended"):
+        """
+        This constructor is called after a text widget is created for
+        initializing all member variables and for adding key and mouse event
+        bindings for handling the selection.
+        """
+        # Text widget whose selection is managed by the class instance
+        self.wid = wid
+        # Callback to invoke after selection changes
+        self.cb_proc = cb_proc
+        # Callback which returns the content list length
+        self.len_proc = len_proc
+        # ID of "after" event handler while scrolling via mouse, or None
+        self.scroll_tid = None
+        # Scrolling speed while dragging the mouse above or below the text window.
+        self.scroll_speed = 0
+        # Anchor element index OR last selection cursor pos
+        self.anchor_idx = -1
+        # List of indices of selected lines (starting at zero)
+        self.sel = []
+
+        self.wid.bind("<Control-ButtonPress-1>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(lambda: self.__text_sel_pick(e.x, e.y)))
+        self.wid.bind("<Shift-ButtonPress-1>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(lambda: self.__text_sel_resize(e.x, e.y)))
+        self.wid.bind("<ButtonPress-1>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(lambda: self.__text_sel_button(e.x, e.y)))
+        self.wid.bind("<ButtonRelease-1>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(self.__text_sel_motion_end))
+        if mode == "browse":
+            self.wid.bind("<B1-Motion>", lambda e, self=self:
+                          tk_utils.bind_call_and_break(lambda: self.__text_sel_button(e.x, e.y)))
         else:
-            txt.extend(["\t%d" % nof_fail, "body"])
+            self.wid.bind("<B1-Motion>", lambda e, self=self:
+                          tk_utils.bind_call_and_break(lambda: self.__text_sel_motion(e.x, e.y)))
 
-        duration = tc_stats[3] / 1000 # FP result
-        if duration < 10:
-            duration = "\t%.3f" % duration
-        elif duration < 3600:
-            duration = "\t%02d:%02d" % (duration/60, duration%60)
+        self.wid.bind("<Shift-Key-Up>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(lambda: self.__text_sel_key_resize(-1)))
+        self.wid.bind("<Shift-Key-Down>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(lambda: self.__text_sel_key_resize(1)))
+        self.wid.bind("<Key-Up>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(lambda: self.__text_sel_key_up_down(-1)))
+        self.wid.bind("<Key-Down>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(lambda: self.__text_sel_key_up_down(1)))
+        self.wid.bind("<Shift-Key-Home>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(lambda: self.__text_sel_key_home_end(False,
+                                                                                        True)))
+        self.wid.bind("<Shift-Key-End>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(lambda: self.__text_sel_key_home_end(True,
+                                                                                        True)))
+        self.wid.bind("<Key-Home>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(lambda: self.__text_sel_key_home_end(False,
+                                                                                        False)))
+        self.wid.bind("<Key-End>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(lambda: self.__text_sel_key_home_end(True,
+                                                                                        False)))
+
+        self.wid.bind("<Control-Key-a>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(self.__text_sel_select_all))
+        self.wid.bind("<Control-Key-c>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(lambda: self.text_sel_copy_clipboard(True)))
+
+        self.wid.bind("<Key-Prior>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(lambda: self.__text_sel_key_page_up_down(-1)))
+        self.wid.bind("<Key-Next>", lambda e, self=self:
+                      tk_utils.bind_call_and_break(lambda: self.__text_sel_key_page_up_down(1)))
+
+
+    def text_sel_get_selection(self):
+        """
+        This is an interface function which allows outside users to retrieve a
+        list of selected elements (i.e. a list of indices)
+        """
+        return self.sel
+
+
+    def text_sel_set_selection(self, sel, do_callback=True):
+        """
+        This is an interface function which allows to modify the selection
+        externally.
+        """
+        if len(sel) > 0:
+            self.anchor_idx = sel[0]
+        self.sel = sel
+
+        self.text_sel_show_selection()
+
+        if do_callback:
+            self.cb_proc(self.sel)
+
+
+    def text_sel_context_selection(self, xcoo, ycoo):
+        """
+        This is an interface function which is used by context menus to check
+        if the item under the mouse pointer is included in the selection.
+        If not, the selection is set to consist only of the pointed item.
+        """
+        line = self.__text_sel_coo2_line(xcoo, ycoo)
+        if line != -1:
+            if len(self.sel) != 0:
+                if not line in self.sel:
+                    # click was outside the current selection -> replace selection
+                    self.text_sel_set_selection([line])
+            else:
+                # nothing selected yet -> select element under the mouse pointer
+                self.text_sel_set_selection([line])
         else:
-            duration = "\t%d:%02d:%02d" % (duration/3600, (duration/60)%60, duration%60)
-        txt.extend([duration + "\n", "body"])
-
-        return txt
+            self.text_sel_set_selection([])
 
 
-    def __handle_tc_stats_update(self, tc_name):
-        try:
-            line_idx = self.tc_list_sorted.index(tc_name)
-        except ValueError:
-            line_idx = None
-
-        if line_idx is None:
-            if self.__matches_filter(tc_name):
-                line_idx = bisect.bisect_left(self.tc_list_sorted, tc_name,
-                                              self.__get_sort_key_fn())
-                self.__insert_single(tc_name, line_idx)
+    def __text_sel_button(self, xcoo, ycoo):
+        """
+        This function is bound to button-press events in the text widget while
+        neither Control nor Shift keys are pressed.  A previous selection is is
+        cleared and the entry below the mouse (if any) is selected.
+        """
+        line = self.__text_sel_coo2_line(xcoo, ycoo)
+        old_sel = self.sel
+        if 0 <= line < self.len_proc():
+            # select the entry under the mouse pointer
+            self.anchor_idx = line
+            self.sel = [line]
+            notify = True
         else:
-            if self.__matches_filter(tc_name):
-                if self.__check_sort_order(tc_name, line_idx):
-                    self.__replace_single(tc_name, line_idx)
-                else:
-                    self.__delete_single(tc_name, line_idx)
-                    line_idx = bisect.bisect_left(self.tc_list_sorted, tc_name,
-                                                  self.__get_sort_key_fn())
-                    self.__insert_single(tc_name, line_idx)
-            else:
-                self.__delete_single(tc_name, line_idx)
-
-
-    def __replace_single(self, tc_name, line_idx):
-        txt = self.__format_table_row(tc_name)
-        self.wid_table.replace("%d.0" % (line_idx + 1), "%d.0" % (line_idx + 2), *txt)
-        self.sel_obj.text_sel_show_selection()
+            # mouse pointer is not above a list entry -> clear selection
+            self.sel = []
+            notify = False
+
+        # update display if the selection changed
+        if old_sel != self.sel:
+            self.text_sel_show_selection()
+            notify = True
+
+        # invoke notification callback if an element was selected or de-selected
+        if notify:
+            self.cb_proc(self.sel)
+
+        self.wid.focus_set()
+
+
+    def __text_sel_motion(self, xcoo, ycoo):
+        """
+        This function is bound to mouse pointer motion events in the text widget
+        while the mouse button is pressed down. This allows changing the extent
+        of the selection. The originally selected item ("anchor") always remains
+        selected.  If the pointer is moved above or below the widget borders,
+        the text is scrolled.
+        """
+        # the anchor element is the one above which the mouse button was pressed
+        # (the check here is for fail-safety only, should always be fulfilled)
+        if self.anchor_idx >= 0:
+            win_h = self.wid.winfo_height()
+            # check if the mouse is still inside of the widget area
+            if 0 <= ycoo < win_h:
+                # identify the item under the mouse pointer
+                line = self.__text_sel_coo2_line(xcoo, ycoo)
+                if line != -1:
+                    # build list of all consecutive indices between the anchor and the mouse pos.
+                    sel = TextSelWidget.__idx_range(self.anchor_idx, line)
+                    # update display and invoke notification callback if the selection changed
+                    if sel != self.sel:
+                        self.sel = sel
+                        self.text_sel_show_selection()
+                        self.cb_proc(self.sel)
+
+                # cancel scrolling timer, as the mouse is now back inside the widget
+                if self.scroll_tid is not None:
+                    tk_utils.tk_top.after_cancel(self.scroll_tid)
+                    self.scroll_tid = None
 
+            else:
+                # mouse is outside of the text widget - start scrolling
+                # scrolling speed is determined by how far the mouse is outside
+                font_h = tk_utils.tk_top.call("font", "metrics", self.wid.cget("font"),
+                                              "-linespace")
+                if ycoo < 0:
+                    delta = 0 - ycoo
+                else:
+                    delta = ycoo - win_h
 
-    def __insert_single(self, tc_name, line_idx):
-        txt = self.__format_table_row(tc_name)
-        self.wid_table.insert("%d.0" % (line_idx + 1), *txt)
+                delay = 500 - delta * 100 // font_h
+                if delay > 500:
+                    delay = 500
+                elif delay < 50:
+                    delay = 50
+                if self.scroll_tid is None:
+                    # start timer and remember it's ID to be able to cancel it later
+                    delta = -1 if (ycoo < 0) else 1
+                    self.scroll_tid = tk_utils.tk_top.after(delay, lambda:
+                                                            self.__text_sel_motion_scroll(delta))
+                    self.scroll_delay = delay
+                else:
+                    # timer already active - just update the delay
+                    self.scroll_delay = delay
 
-        self.tc_list_sorted.insert(line_idx, tc_name)
-        self.sel_obj.text_sel_adjust_insert(line_idx)
 
+    def __text_sel_motion_scroll(self, delta):
+        """
+        This timer event handler is activated when the mouse is moved outside of
+        the text widget while the mouse button is pressed. The handler re-installs
+        itself and is only stopped when the button is released or the mouse is
+        moved back inside the widget area.  The function invariably scrolls the
+        text by one line. Scrolling speed is varied by means of the delay time.
+        """
+        # scroll up or down by one line
+        self.wid.yview_scroll(delta, "units")
+
+        # extend the selection to the end of the viewable area
+        if delta < 0:
+            self.__text_sel_motion(0, 0)
+        else:
+            self.__text_sel_motion(0, self.wid.winfo_height() - 1)
 
-    def __delete_single(self, tc_name, line_idx):
-        line_1 = "%d.0" % (line_idx + 1)
-        line_2 = "%d.0" % (line_idx + 2)
-        self.wid_table.delete(line_1, line_2)
+        # install the timer again (possibly with a changed delay if the mouse was moved)
+        self.scroll_tid = tk_utils.tk_top.after(self.scroll_speed,
+                                                lambda: self.__text_sel_motion_scroll(delta))
+
+
+    def __text_sel_motion_end(self):
+        """
+        This function is boud to mouse button release events and stops a
+        possible on-going scrolling timer.
+        """
+        if self.scroll_tid is not None:
+            tk_utils.tk_top.after_cancel(self.scroll_tid)
+            self.scroll_tid = None
+
+
+    def __text_sel_pick(self, xcoo, ycoo):
+        """
+        This function is bound to mouse button events while the Control key is
+        pressed. The item below the mouse pointer is toggled in the selection.
+        Otherwise the selection is left unchanged.  Note this operation always
+        clears the "anchor" element, i.e. the selection cannot be modified
+        using "Shift-Click" afterwards.
+        """
+        line = self.__text_sel_coo2_line(xcoo, ycoo)
+        if line != -1:
+            # check if the item is already selected
+            try:
+                pick_idx = self.sel.index(line)
+                # already selected -> remove from selection
+                del self.sel[pick_idx]
+            except ValueError:
+                pick_idx = -1
+                self.sel.append(line)
+
+            if len(self.sel) <= 1:
+                self.anchor_idx = line
+
+            self.text_sel_show_selection()
+            self.cb_proc(self.sel)
+
+
+    def __text_sel_resize(self, xcoo, ycoo):
+        """
+        This function is bound to mouse button events while the Shift key is
+        pressed. The selection is changed to cover all items starting at the
+        anchor item and the item under the mouse pointer.  If no anchor is
+        defined, the selection is reset and only the item under the mouse is
+        selected.
+        """
+        line = self.__text_sel_coo2_line(xcoo, ycoo)
+        if line != -1:
+            if self.anchor_idx != -1:
+                self.sel = TextSelWidget.__idx_range(self.anchor_idx, line)
+                self.text_sel_show_selection()
+                self.cb_proc(self.sel)
+            else:
+                self.__text_sel_button(xcoo, ycoo)
 
-        del self.tc_list_sorted[line_idx]
-        self.sel_obj.text_sel_adjust_deletion(line_idx)
 
+    def __text_sel_key_page_up_down(self, delta):
+        """
+        This function is bound to the page up/down cursor keys.
+        """
+        content_len = self.len_proc()
+        if content_len == 0:
+            return
 
-    def __populate_table(self):
-        self.wid_table.delete("1.0", "end")
-        for tc_name in self.tc_list_sorted:
-            txt = self.__format_table_row(tc_name)
-            self.wid_table.insert("end", *txt)
+        if (delta < 0) and (self.wid.bbox("1.0") is not None):
+            self.__text_sel_select_line(0)
 
-        self.sel_obj.text_sel_set_selection([])
+        elif (delta > 0) and (self.wid.bbox("%d.0" % content_len) is not None):
+            self.__text_sel_select_line(content_len - 1)
 
+        else:
+            if self.sel:
+                prev_line = min(self.sel) if delta < 0 else max(self.sel)
+            else:
+                prev_line = -1
 
-    def __refill_table(self):
-        prev_yview = self.wid_table.yview()[0]
-        prev_sel = self.sel_obj.text_sel_get_selection()
+            self.wid.yview("scroll", delta, "pages")
 
-        self.__populate_table()
+            line = self.__text_sel_coo2_line(1, self.wid.winfo_height() / 2)
+            if line != -1:
+                if delta < 0 and line > prev_line and prev_line != -1:
+                    line = prev_line
+                if delta > 0 and line < prev_line:
+                    line = prev_line
+
+                # set selection on the new line
+                self.__text_sel_select_line(line)
+
+
+    def __text_sel_key_up_down(self, delta):
+        """
+        This function is bound to the up/down cursor keys. If no selection
+        exists, the viewable first item in cursor direction is selected.
+        If a selection exists, it's cleared and the item next to the
+        previous selection in cursor direction is selected.
+        """
+        content_len = self.len_proc()
+        if content_len > 0:
+            sel = sorted(self.sel)
+            if len(sel) != 0:
+                # selection already exists -> determine item below or above
+                if delta < 0:
+                    line = sel[0]
+                else:
+                    line = sel[-1]
 
-        self.wid_table.yview_moveto(prev_yview)
-        self.sel_obj.text_sel_set_selection(prev_sel)
+                # determine the newly selected item
+                line += delta
 
+                if 0 <= line < content_len:
+                    # set selection on the new line
+                    self.__text_sel_select_line(line)
+
+                elif len(sel) > 1:
+                    # selection already includes last line - restrict selection to this single line
+                    if delta < 0:
+                        line = 0
+                    else:
+                        line = content_len - 1
 
-    def __handle_campaign_status_change(self):
-        for tc_name in test_db.test_case_names:
-            self.__handle_tc_stats_update(tc_name)
+                    self.__text_sel_select_line(line)
 
+            else:
+                # no selection exists yet -> use last anchor, or top/bottom visible line
+                if ((self.anchor_idx >= 0) and
+                        (self.wid.bbox("%d.0" % (self.anchor_idx + 1)) is not None)):
+                    idx = "%d.0" % (self.anchor_idx + 1)
+                else:
+                    if delta > 0:
+                        idx = "@1,1"
+                    else:
+                        idx = "@1,%d" % (self.wid.winfo_height() - 1)
+
+                pos = self.wid.index(idx)
+                if pos != "":
+                    line = int(pos.split(".")[0])
+                    if line > 0:
+                        line -= 1
+                        if line >= content_len:
+                            line = content_len - 1
+                        self.__text_sel_select_line(line)
+
+
+    def __text_sel_key_resize(self, delta):
+        """
+        This function is bound to the up/down cursor keys while the Shift key
+        is pressed. The selection is changed to cover all items starting at the
+        anchor item and the next item above or below the current selection.
+        """
+        content_len = self.len_proc()
+        if len(self.sel) > 0:
+            sel = sorted(self.sel)
+            # decide if we manipulate the upper or lower end of the selection:
+            # use the opposite side of the anchor element
+            if self.anchor_idx == sel[-1]:
+                line = sel[0]
+            else:
+                line = sel[-1]
 
-    def __handle_main_tc_filter_expr_change(self, expr):
-        self.tc_enabled = expr.get_selected_tests()
+            line += delta
+            if 0 <= line < content_len:
+                self.sel = TextSelWidget.__idx_range(self.anchor_idx, line)
+
+                self.text_sel_show_selection()
+                self.wid.see("%d.0" % (line + 1))
+                self.cb_proc(self.sel)
 
-        if self.var_filter_run.get():
-            self.__handle_filter_change()
         else:
-            self.__refill_table()
-
-
-    def __handle_tc_names_update(self):
-        self.__update_column_widths()
-        self.__handle_filter_change()
+            self.__text_sel_key_up_down(delta)
 
 
-    def __handle_filter_change(self):
-        self.tc_enabled = self.test_ctrl.get_test_filter_expr().get_selected_tests()
-
-        filter_run = self.var_filter_run.get()
-        filter_failed = self.var_filter_failed.get()
-        filter_disabled = self.var_filter_disabled.get()
-        tc_list = []
+    def __text_sel_key_home_end(self, is_end, is_resize):
+        """
+        This function is bound to the "Home" and "End" keys.  While the Shift
+        key is not pressed, the first or last element in the list are selected.
+        If the Shift key is pressed, the selection is extended to include all
+        items between the anchor and the first or last item.
+        """
+        content_len = self.len_proc()
+        if content_len > 0:
+            if is_end:
+                line = content_len - 1
+            else:
+                line = 0
 
-        for tc_name in test_db.test_case_names:
-            if self.__matches_filter(tc_name):
-                tc_list.append(tc_name)
+            if not is_resize:
+                self.anchor_idx = line
+                self.sel = [line]
+            else:
+                if self.anchor_idx >= 0:
+                    self.sel = TextSelWidget.__idx_range(self.anchor_idx, line)
 
-        self.tc_list_sorted = self.__sort_tc_list(tc_list)
-        self.__populate_table()
+            self.text_sel_show_selection()
+            self.wid.see("%d.0" % (line + 1))
+            self.cb_proc(self.sel)
+
+
+    def __text_sel_select_all(self):
+        """
+        This function is bound to the "CTRL-A" key to select all entries in
+        the list.
+        """
+        content_len = self.len_proc()
+        if content_len > 0:
+            self.sel = TextSelWidget.__idx_range(0, content_len - 1)
 
+            self.text_sel_show_selection()
+            self.cb_proc(self.sel)
 
-    def __matches_filter(self, tc_name):
-        tc_stats = test_db.test_case_stats[tc_name]
-        return ( (not self.var_filter_run.get() or tc_name in self.tc_enabled) and
-                 (not self.var_filter_failed.get() or tc_stats[1]) and
-                 (not self.var_filter_disabled.get() or not filter_expr.is_disabled_by_name(tc_name)) )
 
+    @staticmethod
+    def __idx_range(start, end):
+        """
+        This helper function is used to build a list of all indices between
+        (and including) two given values in increasing order.
+        """
+        if start > end:
+            return list(range(end, start + 1))
+        return list(range(start, end + 1))
+
+
+    def text_sel_show_selection(self):
+        """
+        This interface function displays a selection in the text widget by adding
+        the "sel" tag to all selected lines. (Note the view is not affected, i.e.
+        the selection may be outside of the viewable area.)
+        """
+        # first remove any existing highlight
+        self.wid.tag_remove("sel", "1.0", "end")
+
+        # select each selected line (may be non-consecutive)
+        for line in self.sel:
+            self.wid.tag_add("sel", "%d.0" % (line + 1), "%d.0" % (line + 2))
 
-    def __get_sort_key_fn(self):
-        if self.opt_sort_modes:
-            return lambda x: Tc_list_dialog.__get_sort_keys(self.opt_sort_modes, x)
+        if (len(self.sel) == 0) or (self.anchor_idx == -1):
+            self.wid.mark_set("insert", "end")
         else:
-            return lambda x: x
-
+            self.wid.mark_set("insert", "%d.0" % (self.anchor_idx + 1))
 
-    @staticmethod
-    def __get_sort_keys(opt_sort_modes, tc_name):
-        keys = []
-        for mode in opt_sort_modes:
-            if mode == Sort_mode.by_name:
-                keys.append(tc_name)
-
-            elif mode == Sort_mode.by_exec_cnt:
-                keys.append(0 - test_db.test_case_stats[tc_name][0]
-                              - test_db.test_case_stats[tc_name][1]
-                              - test_db.test_case_stats[tc_name][2])
-
-            elif mode == Sort_mode.by_fail_cnt:
-                keys.append(0 - test_db.test_case_stats[tc_name][1])
-
-            elif mode == Sort_mode.by_duration:
-                keys.append(0 - test_db.test_case_stats[tc_name][3])
-        return keys
-
-
-    def __sort_tc_list(self, tc_list):
-        for mode in reversed(self.opt_sort_modes):
-            if mode == Sort_mode.by_name:
-                tc_list = sorted(tc_list)
-            elif mode == Sort_mode.by_exec_cnt:
-                tc_list = sorted(tc_list, key=lambda x: 0 - test_db.test_case_stats[x][0]
-                                                          - test_db.test_case_stats[x][1]
-                                                          - test_db.test_case_stats[x][2])
-            elif mode == Sort_mode.by_fail_cnt:
-                tc_list = sorted(tc_list, key=lambda x: 0 - test_db.test_case_stats[x][1])
-            elif mode == Sort_mode.by_duration:
-                tc_list = sorted(tc_list, key=lambda x: 0 - test_db.test_case_stats[x][3])
-        return tc_list
-
-
-    def __check_sort_order(self, tc_name, line_idx):
-        if self.opt_sort_modes:
-            if line_idx > 0:
-                prev_name = self.tc_list_sorted[line_idx - 1]
-                if (Tc_list_dialog.__get_sort_keys(self.opt_sort_modes, tc_name)
-                        < Tc_list_dialog.__get_sort_keys(self.opt_sort_modes, prev_name)):
-                    return False
-
-            if line_idx + 1 < len(self.tc_list_sorted):
-                next_name = self.tc_list_sorted[line_idx + 1]
-                if (Tc_list_dialog.__get_sort_keys(self.opt_sort_modes, next_name)
-                        < Tc_list_dialog.__get_sort_keys(self.opt_sort_modes, tc_name)):
-                    return False
-
-        return True
-
-
-    def __get_len(self):
-        return len(self.tc_list_sorted)
-
-
-    def __handle_selection_change(self, sel):
-        self.sel_obj.text_sel_copy_clipboard(False)
-
-
-    def __get_mapped_selection(self):
-        sel = self.sel_obj.text_sel_get_selection()
-        return [self.tc_list_sorted[x] for x in sel]
-
-
-    def __post_context_menu(self, parent, xcoo, ycoo):
-        wid_men = tk_utils.get_context_menu_widget()
-
-        if (parent == self.wid_table) and not gtest.gtest_ctrl.is_active():
-            self.sel_obj.text_sel_context_selection(xcoo, ycoo)
-            expr = self.test_ctrl.get_test_filter_expr()
-
-            sel = self.__get_mapped_selection()
-            if not expr.run_disabled():
-                sel = [x for x in sel if not filter_expr.is_disabled_by_name(x)]
-
-            if sel:
-                plural_s = "" if len(sel) == 1 else "s"
-                need_sep = False
-
-                if any([expr.can_select_test(x) for x in sel]):
-                    wid_men.add_command(label="Add selected test case%s to filter" % plural_s,
-                                        command=lambda: self.test_ctrl.select_tcs(sel, True))
-                    need_sep = True
-                if any([expr.can_deselect_test(x) for x in sel]):
-                    wid_men.add_command(label="Remove selected test case%s from filter" % plural_s,
-                                        command=lambda: self.test_ctrl.select_tcs(sel, False))
-                    need_sep = True
-
-                all_tc_names = filter_expr.get_test_list(expr.run_disabled())
-                tc_names = []
-                for tc_suite in filter_expr.get_test_suite_names(sel):
-                    tc_names.extend(filter_expr.get_tests_in_test_suite(tc_suite, all_tc_names))
-
-                if any([expr.can_select_test(x) for x in tc_names]):
-                    wid_men.add_command(label="Add selected test suites to filter",
-                                        command=lambda: self.test_ctrl.select_tcs(tc_names, True))
-                    need_sep = True
-                if any([expr.can_deselect_test(x) for x in tc_names]):
-                    wid_men.add_command(label="Remove selected test suites from filter",
-                                        command=lambda: self.test_ctrl.select_tcs(tc_names, False))
-                    need_sep = True
-
-                if need_sep:
-                    wid_men.add_separator()
-
-        wid_men.add_checkbutton(label="Show only tests enabled to run",
-                                 command=self.__handle_filter_change, variable=self.var_filter_run)
-        wid_men.add_checkbutton(label="Show only failed tests",
-                                 command=self.__handle_filter_change, variable=self.var_filter_failed)
-        wid_men.add_checkbutton(label="Show no DISABLED tests",
-                                 command=self.__handle_filter_change, variable=self.var_filter_disabled)
-        wid_men.add_separator()
-
-        wid_men.add_checkbutton(
-                label="Sort by test case name",
-                command=lambda: self.__do_toggle_sort_mode(self.var_sort_name.get(), Sort_mode.by_name),
-                variable=self.var_sort_name)
-        wid_men.add_checkbutton(
-                label="Sort by execution count",
-                command=lambda: self.__do_toggle_sort_mode(self.var_sort_exec_cnt.get(), Sort_mode.by_exec_cnt),
-                variable=self.var_sort_exec_cnt)
-        wid_men.add_checkbutton(
-                label="Sort by failure count",
-                command=lambda: self.__do_toggle_sort_mode(self.var_sort_fail_cnt.get(), Sort_mode.by_fail_cnt),
-                variable=self.var_sort_fail_cnt)
-        wid_men.add_checkbutton(
-                label="Sort by duration",
-                command=lambda: self.__do_toggle_sort_mode(self.var_sort_duration.get(), Sort_mode.by_duration),
-                variable=self.var_sort_duration)
-        wid_men.add_separator()
-
-        wid_men.add_command(label="Export list to file...", command=self.__do_export_pass_fail)
-        wid_men.add_command(label="Close window", command=self.__destroy_window)
-
-        tk_utils.post_context_menu(parent, xcoo, ycoo)
-
-
-    def __do_export_pass_fail(self):
-        global prev_export_filename
-        filename = tk_filedialog.asksaveasfilename(
-                        parent=self.wid_top,
-                        filetypes=[("all", "*"), ("Text", "*.txt")],
-                        title="Select output file",
-                        initialfile=os.path.basename(prev_export_filename),
-                        initialdir=os.path.dirname(prev_export_filename))
-        if filename:
-            prev_export_filename = filename
-            try:
-                with open(filename, "w") as f:
-                    for tc_name in self.tc_list_sorted:
-                        tc_stats = test_db.test_case_stats[tc_name]
-                        txt = "%s\t%d\t%d\t%d" % (tc_name, tc_stats[0], tc_stats[1], tc_stats[2])
-                        print(txt, file=f)
-
-            except OSError as e:
-                tk_messagebox.showerror(parent=self.wid_top,
-                                        message="Error writing to file: %s" % str(e))
-
-
-    def __do_toggle_sort_mode(self, enable, mode):
-        self.opt_sort_modes = [x for x in self.opt_sort_modes if x != mode]
-        if enable:
-            self.opt_sort_modes.append(mode)
-        self.__handle_filter_change()
-
-
-    def __do_filter_selected_tests(self, enable):
-        sel = self.__get_mapped_selection()
-        if len(sel) != 0:
-            expr = self.test_ctrl.get_test_filter_expr()
-            if enable and not expr.run_disabled():
-                sel = [x for x in sel if not filter_expr.is_disabled_by_name(x)]
 
-            self.test_ctrl.select_tcs(sel, enable)
+    def __text_sel_select_line(self, line):
+        """
+        This function changes the selection to the single given line.
+        """
+        self.anchor_idx = line
+        self.sel = [line]
+
+        self.text_sel_show_selection()
+        self.wid.see("%d.0" % (line + 1))
+        self.cb_proc(self.sel)
+
+
+    def __text_sel_coo2_line(self, xcoo, ycoo):
+        """
+        This function determines the line under the mouse pointer.
+        If the pointer is not above a content line, -1 is returned.
+        """
+        pos = self.wid.index("@%d,%d" % (xcoo, ycoo))
+        if pos != "":
+            line = int(pos.split(".")[0]) - 1
+            if 0 <= line < self.len_proc():
+                return line
+        return -1
+
+
+    def text_sel_adjust_insert(self, line):
+        """
+        This function has to be called when an item has been inserted into the
+        list to adapt the selection: Indices following the insertion are
+        incremented.  The new element is not included in the selection.
+        """
+        self.sel = [(x if x < line else x+1) for x in self.sel]
+
+        if self.anchor_idx >= line:
+            self.anchor_idx += 1
+
+
+    def text_sel_adjust_deletion(self, line):
+        """
+        This function has to be called when an item has been deleted from the
+        list (asynchronously, i.e. not via a command related to the selection)
+        to adapt the list of selected lines: The deleted line is removed from
+        the selection (if included) and following indices are decremented.
+        """
+        self.sel = [(x if x < line else x-1) for x in self.sel if x != line]
+
+        if self.anchor_idx > line:
+            self.anchor_idx -= 1
+
+    def text_sel_copy_clipboard(self, to_clipboard):
+        """
+        This handler is bound to CTRL-C in the selection and performs <<Copy>>
+        (i.e. copies the content of all selected lines to the clipboard.)
+        """
+        msg = "".join([self.wid.get("%d.0" % (line + 1), "%d.0" % (line + 2))
+                       for line in self.sel])
+        tk_utils.xselection_export(msg, to_clipboard)
```

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/gtest.py` & `mote-gtest-gui-0.9.0/gtest_gui/gtest_ctrl.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,118 +13,130 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
-from io import StringIO
+"""
+Implements Interface classes to GTest command line and trace output.
+"""
+
 import os
 import queue
 import re
 import signal
 import subprocess
-import sys
 import selectors
 import threading
 import time
 
 from tkinter import messagebox as tk_messagebox
 
+from gtest_gui.gtest_sharding import GtestSharding
 import gtest_gui.config_db as config_db
 import gtest_gui.test_db as test_db
 import gtest_gui.tk_utils as tk_utils
+import gtest_gui.trace_db as trace_db
 import gtest_gui.fcntl
 
 
 gtest_ctrl = None
 
 def initialize():
+    """ Creates the singleton instance of GtestControl. """
     global gtest_ctrl
-    gtest_ctrl = Gtest_control()
+    gtest_ctrl = GtestControl()
+
 
+class GtestControl:
+    """
+    This class starts and controls processes spawned from the selected test
+    executable for a test campaign. If offers start and stop interfaces for the
+    test campaign and various status queries.
+    """
 
-class Gtest_control(object):
     def __init__(self):
+        """ Creates an idle instance of GtestControl. """
         self.__jobs = []
         self.__result_queue = queue.Queue()
         self.__thr_lock = threading.Lock()
         self.__thr_inst = None
-        self.__tid = None
+        self.__max_fail = 0
+        self.__exe_ts = None
 
 
     def start(self, job_cnt, job_runall_cnt, rep_cnt, filter_str, tc_list, is_resume,
               run_disabled, shuffle, valgrind_cmd, maxfail, clean_trace, clean_core,
               break_on_fail, break_on_except):
+        """
+        Start a test campaign with the given options. Errors are reported via GUI directly.
+        Test results and campaign status are reported to the test results database module.
+        """
         self.__max_fail = maxfail
         self.__exe_ts = test_db.test_exe_ts
 
-        trace_dir_path = gtest_control_get_trace_dir(self.__exe_ts)
+        trace_dir_path = trace_db.get_trace_dir(self.__exe_ts)
         if not os.path.exists(trace_dir_path):
             try:
                 os.mkdir(trace_dir_path)
-            except OSError as e:
-                tk_messagebox.showerror(parent=tk_utils.tk_top,
-                                        message="Failed to create trace output directory: " + str(e))
+            except OSError as exc:
+                msg = "Failed to create trace output directory: " + str(exc)
+                tk_messagebox.showerror(parent=tk_utils.tk_top, message=msg)
                 return
 
-        exe_name = gtest_control_get_exe_file_link_name(test_db.test_exe_name, self.__exe_ts)
-        if config_db.options["copy_executable"] and not os.access(exe_name, os.X_OK):
+        exe_name = trace_db.get_exe_file_link_name(test_db.test_exe_name, self.__exe_ts)
+        if config_db.get_opt("copy_executable") and not os.access(exe_name, os.X_OK):
             try:
                 os.link(test_db.test_exe_name, exe_name)
-            except OSError as e:
+            except OSError as exc:
                 msg = ("Failed to link or copy executable: %s. Will use executable directly. "
-                       "See Configuration to disable this warning.") % str(e)
+                       "See Configuration to disable this warning.") % str(exc)
                 answer = tk_messagebox.showwarning(parent=tk_utils.tk_top, message=msg)
                 if answer == "cancel":
                     return
                 exe_name = test_db.test_exe_name
 
-        (shard_parts, shard_reps) = calc_sharding_partitioning(
-                                        len(tc_list), rep_cnt, job_cnt - job_runall_cnt)
-        for idx in range(job_runall_cnt):
-            shard_parts.append(1)
-            shard_reps.append(rep_cnt)
-
-        part_idx = 0
-        shard_idx = 0
+        sharding = GtestSharding(len(tc_list), rep_cnt, job_cnt, job_runall_cnt)
 
-        trace_idx = gtest_control_first_free_trace_file_idx(self.__exe_ts)
+        trace_idx = trace_db.first_free_trace_file_idx(self.__exe_ts)
         for idx in range(job_cnt):
             if idx >= job_cnt - job_runall_cnt:
                 filter_str = ""
+            (job_rep_cnt, job_cpu_cnt, job_cpu_idx) = sharding.next()
+            shard_tc_cnt = sharding.get_tc_count_per_shard(len(tc_list), job_rep_cnt,
+                                                           job_cpu_cnt, job_cpu_idx)
+
             try:
-                self.__jobs.append(Gtest_job(self, exe_name, self.__exe_ts,
-                                             gtest_control_get_trace_file_name(self.__exe_ts, trace_idx),
-                                             filter_str, run_disabled, shuffle, valgrind_cmd,
-                                             clean_trace, clean_core, break_on_fail, break_on_except,
-                                             shard_reps[part_idx], shard_parts[part_idx], shard_idx,
-                                             idx >= job_cnt - job_runall_cnt,
-                                             self.__result_queue))
-            except OSError as e:
+                self.__jobs.append(GtestJob(exe_name, self.__exe_ts,
+                                            trace_db.get_trace_file_name(self.__exe_ts, trace_idx),
+                                            filter_str, run_disabled, shuffle, valgrind_cmd,
+                                            clean_trace, clean_core,
+                                            break_on_fail, break_on_except,
+                                            job_rep_cnt, job_cpu_cnt, job_cpu_idx, shard_tc_cnt,
+                                            idx >= job_cnt - job_runall_cnt,
+                                            self.__result_queue))
+            except OSError as exc:
                 tk_messagebox.showerror(parent=tk_utils.tk_top,
-                                        message="Failed to start jobs: " + str(e))
+                                        message="Failed to start jobs: " + str(exc))
                 break
 
             trace_idx += 1
-            shard_idx += 1
-            if shard_idx >= shard_parts[part_idx]:
-                shard_idx = 0
-                part_idx += 1
 
-        self.__tid = tk_utils.tk_top.after(250, self.__poll_queue)
+        tk_utils.tk_top.after(250, self.__poll_queue)
 
+        # Clean up zombie processes from previous run, if any
         if self.__thr_inst:
             self.__thr_inst.join(timeout=0)
 
         self.__thr_inst = threading.Thread(target=self.__thread_main, daemon=True)
         self.__thr_inst.start()
 
         test_db.reset_run_stats(len(tc_list) * rep_cnt, is_resume)
-        test_db.set_job_status(len(self.__jobs))
+        test_db.set_job_status(len(self.__jobs), time.time())
 
 
     def __thread_main(self):
         if os.name == "posix":
             self.__thread_main_select()
         else:
             self.__thread_main_polling()
@@ -143,17 +155,17 @@
 
             with self.__thr_lock:
                 # Process events under lock to support abort with clean-up by main control
                 if not self.__jobs:
                     return
 
                 for event in pending_events:
-                    fd = event[0].data.get_pipe()
+                    event_fd = event[0].data.get_pipe()
                     if not event[0].data.communicate():
-                        selector.unregister(fd)
+                        selector.unregister(event_fd)
 
             # Add minimum delay between reading pipes for reducing parser overhead
             sleep = next_poll - time.time()
             next_poll += 0.150
 
             if sleep > 0:
                 time.sleep(sleep)
@@ -187,54 +199,82 @@
                     test_db.add_result(result[0], result[1])
                 else:
                     self.__report_exit(result[1])
         except queue.Empty:
             pass
 
         if self.__jobs:
-            self.__tid = tk_utils.tk_top.after(250, self.__poll_queue)
-        else:
-            self.__tid = None
+            tk_utils.tk_top.after(250, self.__poll_queue)
 
 
     def stop(self, kill=False):
+        """
+        Terminates all processes in the current test campaign by sending them a
+        respective signal. The campaign status will not be changed to "idle"
+        until the processes have been reported by the OS to have exited.  If
+        parameter "kill" is True, OS will be asked to kill the process with a
+        "KILL" signal that they cannot catch, on platforms that support it.
+        """
         with self.__thr_lock:
             for job in self.__jobs:
                 job.terminate(kill)
 
             if kill:
                 self.__jobs = []
 
 
     def is_active(self):
+        """
+        Queries if a campaign is currently running. This is the case as long as
+        a test process is still running.
+        """
         return bool(self.__jobs)
 
 
     def update_options(self, clean_trace, clean_core):
+        """
+        Updates values of the "clean_trace" and "clean_core" options for a
+        currently running campaign.  Changing other options than these two
+        requires stopping and resuming.
+        """
         with self.__thr_lock:
             for job in self.__jobs:
                 job.update_options(clean_trace, clean_core)
 
 
     def get_job_stats(self):
+        """ Returns a list containing status of each running test process. """
         with self.__thr_lock:
             stats = []
             for job in self.__jobs:
                 stats.append(job.get_stats())
         return stats
 
 
     def abort_job(self, pid):
+        """
+        Sends an ABORT signal to a test process with the given PID, if it is
+        still running. On POSIX systems this will result in a core dump that
+        can be analyzed post-mortem, if core dumps are enabled. As a
+        side-effect, the test case the process is currently executing will be
+        marked as "crashed" in the result log. Other test processes are
+        unaffected.
+        """
         with self.__thr_lock:
             for job in self.__jobs:
                 if job.get_stats()[0] == pid:
                     job.abort()
 
 
     def get_out_file_names(self):
+        """
+        Returns a list of output trace file names of all currently running test
+        processes.  The files must not be removed via the GUI when user deletes
+        results from the log in the GUI.
+        """
         used_files = set()
         with self.__thr_lock:
             for job in self.__jobs:
                 used_files.add(job.get_out_file_name())
         return used_files
 
 
@@ -249,304 +289,41 @@
         for idx in range(len(self.__jobs)):
             if self.__jobs[idx] == job:
                 del self.__jobs[idx]
                 break
         test_db.set_job_status(len(self.__jobs))
 
         with self.__thr_lock:
-            have_non_bg = any([not job.is_bg_job() for job in self.__jobs])
+            have_non_bg = any(not job.is_bg_job() for job in self.__jobs)
 
         if not have_non_bg:
             tk_utils.tk_top.after_idle(self.stop)
 
 
 # ----------------------------------------------------------------------------
 
+class GtestJob:
+    """
+    This class spawns a process from the given test executable file with the
+    given GTest parameters. Afterwards it reads the trace output via a pipe.
+    The pipe is read non-blocking. The caller has to periodically call the
+    communicate() interface to read data from the pipe. Results are added to
+    the given queue.  Process termination is reported via a special type of
+    queue entry.
+    """
 
-def calc_parts_sub(pre_part, cpu_cnt, tc_cnt, rep_cnt, max_cpu_cnt):
-    #print("DBG %s | %d,%d,%d,%d" % (str(pre_part), cpu_cnt, tc_cnt, rep_cnt, max_cpu_cnt))
-    partitions = []
-    prev_c = 0
-    div = 1
-    while True:
-        c = int((tc_cnt + div - 1) / div)
-
-        if c != prev_c and c <= max_cpu_cnt:
-            if c > 1:
-                cnt = int(cpu_cnt / c)
-                part = pre_part + ([c] * cnt)
-                remainder = cpu_cnt - (c * cnt)
-
-                if remainder > 0:
-                    partitions.extend(calc_parts_sub(part, remainder, tc_cnt, rep_cnt,
-                                                     min(remainder, c)))
-                else:
-                    partitions.append(part)
-            else:
-                partitions.append(pre_part + [1] * cpu_cnt)
-
-        prev_c = c
-        if c <= 1:
-            break
-        div += 1
-
-    if not partitions:
-        partitions.append(pre_part + [cpu_cnt])
-
-    return partitions
-
-
-def calc_partitions(tc_cnt, job_cnt, rep_cnt):
-    partitions = calc_parts_sub([], job_cnt, tc_cnt, rep_cnt, job_cnt)
-    return partitions
-
-
-def calc_repetitions(partitions, tc_cnt, rep_cnt):
-    min_time = tc_cnt * rep_cnt
-    min_parts = None
-    min_reps = None
-    for part in partitions:
-        tcs = [int((tc_cnt + c - 1) / c) for c in part]
-
-        # step #1: estimate repetiton count based on TC# relation between CPU partitions
-        # (needed for reducing the number of iterations in step 2)
-        tc_est = [tcs[0] / x for x in tcs]
-        sum_est = sum(tc_est)
-        reps = [int(rep_cnt / sum_est * x) for x in tc_est]
-        tcs_rep = tcs.copy()
-        for rep_idx in range(len(tcs_rep)):
-            tcs_rep[rep_idx] *= reps[rep_idx]
-
-        # step #2: distribute remaining repetitons to partitions
-        for rep_idx in range(sum(reps), rep_cnt):
-            min_idx = 0
-            min_val = tcs_rep[0] + tcs[0]
-            for idx in range(1, len(tcs)):
-                if tcs_rep[idx] + tcs[idx] < min_val:
-                    min_idx = idx
-                    min_val = tcs_rep[idx] + tcs[idx]
-            tcs_rep[min_idx] = min_val
-            reps[min_idx] += 1
-        new_max = max(tcs_rep)
-        #print("DBG part: " + str(part) + " -> " + str(tcs) + " -> " + str(new_max))
-
-        # among all possible sharding partitions, select that with minimum TC# per CPU
-        if (new_max < min_time) or (min_parts is None):
-            min_time = new_max
-            min_reps = reps
-            min_parts = part.copy()
-
-    #print(("Choice: %d " % min_time) + str(min_parts) + " * " + str(min_reps))
-    return (min_parts, min_reps)
-
-
-def calc_sharding_partitioning(tc_cnt, rep_cnt, job_cnt):
-    if tc_cnt and rep_cnt and job_cnt:
-        return calc_repetitions(calc_partitions(tc_cnt, job_cnt, rep_cnt), tc_cnt, rep_cnt)
-    else:
-        return ([job_cnt], [rep_cnt])
-
-
-def gtest_control_first_free_trace_file_idx(exe_ts):
-    free_idx = 0
-    for entry in os.scandir(gtest_control_get_trace_dir(exe_ts)):
-        if entry.is_file():
-            match = re.match(r"^trace\.(\d+)$", entry.name)
-            if match:
-                this_idx = int(match.group(1))
-                if this_idx >= free_idx:
-                    free_idx = this_idx + 1
-    return free_idx
-
-
-def gtest_control_search_trace_dirs():
-    if config_db.options["trace_dir"]:
-        trace_dir_path = config_db.options["trace_dir"]
-    else:
-        trace_dir_path = "."
-
-    trace_files = []
-    if os.path.isdir(trace_dir_path):
-        for base_entry in os.scandir(trace_dir_path):
-            if re.match(r"^trace\.\d+$", base_entry.name):
-                for entry in os.scandir(os.path.join(trace_dir_path, base_entry.name)):
-                    if entry.is_file():
-                        if re.match(r"^trace\.(\d+)$", entry.name):
-                            trace_files.append(os.path.join(trace_dir_path,
-                                                            base_entry.name, entry.name))
-
-    return trace_files
-
-
-def gtest_control_get_trace_dir(exe_ts):
-    trace_dir_path = "trace.%d" % exe_ts
-    if config_db.options["trace_dir"]:
-        trace_dir_path = os.path.join(config_db.options["trace_dir"], trace_dir_path)
-    return trace_dir_path
-
-
-def gtest_control_get_exe_file_link_name(exe_name, exe_ts):
-    if config_db.options["copy_executable"]:
-        trace_dir_path = gtest_control_get_trace_dir(exe_ts)
-        return os.path.join(trace_dir_path, os.path.basename(exe_name))
-    else:
-        return exe_name
-
-
-def gtest_control_get_trace_file_name(exe_ts, idx):
-    return os.path.join(gtest_control_get_trace_dir(exe_ts), "trace.%d" % idx)
-
-
-def gtest_control_get_temp_name_for_trace(file_name, file_off, is_extern_import):
-    if is_extern_import:
-        return "imported!" + file_name.replace(os.path.sep, "!") + "." + str(file_off)
-    else:
-        trace_path, trace_name = os.path.split(file_name)
-        return "%s.%s.%d" % (os.path.basename(trace_path), trace_name, file_off)
-
-
-def gtest_control_get_core_file_name(trace_name, is_valgrind):
-    split_name = os.path.split(trace_name)
-    core_name = "vgcore" if is_valgrind else "core"
-
-    return os.path.join(split_name[0], core_name + "." + split_name[1])
-
-
-def release_exe_file_copy(exe_name=None, exe_ts=None):
-    if exe_name is None:
-        exe_name = test_db.test_exe_name
-    if exe_ts is None:
-        exe_ts = test_db.test_exe_ts
-    if not exe_name or not exe_ts:
-        return
-
-    if not config_db.options["copy_executable"]:
-        return
-
-    trace_dir_path = gtest_control_get_trace_dir(exe_ts)
-    if os.path.exists(trace_dir_path):
-        dir_list = os.listdir(trace_dir_path)
-
-        if not any([x.startswith(("core.", "vgcore.")) for x in dir_list]):
-            exe_link = gtest_control_get_exe_file_link_name(exe_name, exe_ts)
-            try:
-                os.unlink(exe_link)
-                try:
-                    dir_list.remove(os.path.basename(exe_link))
-                except:
-                    pass
-            except OSError:
-                pass
-
-            if not dir_list:
-                try:
-                    os.rmdir(trace_dir_path)
-                except OSError:
-                    pass
-
-
-def remove_trace_or_core_files(rm_files, rm_exe):
-    if config_db.options["copy_executable"]:
-        for exe_name_ts in rm_exe:
-            rm_files.add(gtest_control_get_exe_file_link_name(exe_name_ts[0], exe_name_ts[1]))
-
-    try:
-        for file_name in rm_files:
-            os.remove(file_name);
-    except OSError:
-        pass
-
-    rm_dirs = {os.path.dirname(x) for x in rm_files}
-    for adir in rm_dirs:
-        try:
-            if not os.listdir(adir):
-                os.rmdir(adir)
-        except OSError:
-            pass
-
-
-def clean_all_trace_files(clean_failed=False):
-    contains_fail = set()
-    pass_parts = {}
-    rm_files = set()
-    rm_exe = set()
-    for log in test_db.test_results:
-        # never auto-clean imported files: could interfere with other GUI instance
-        if log[4] and not log[13]:
-            rm_files.add(log[4])
-            if not clean_failed:
-                if log[3] == 2 or log[3] == 3:
-                    contains_fail.add(log[4])
-                elif log[3] == 4: # valgrind: keep all pass traces
-                    del pass_parts[log[4]]
-                else:
-                    __add_passed_section(pass_parts, log[4], log[5], log[6])
-
-        if clean_failed and log[7]:
-            rm_files.add(log[7])
-            if log[1]:
-                rm_exe.add((log[1], log[2]))
-
-    if not clean_failed:
-        for name in contains_fail:
-            rm_files.remove(name)
-            pp = pass_parts.get(name)
-            if pp:
-                __compress_trace_file(name, pp)
-
-    remove_trace_or_core_files(rm_files, rm_exe)
-
-
-def __add_passed_section(pass_parts, name, start, end):
-    parts = pass_parts.get(name)
-    if parts:
-        if parts[-1][1] == start:
-            parts[-1] = (pp[-1][0], end)
-        else:
-            pass_parts[name].append((start, end))
-    else:
-        pass_parts[name] = [(start, end)]
-
-
-def __compress_trace_file(name, parts):
-    if sys.platform == "win32":
-        fd = os.open(name, os.O_RDWR | os.O_BINARY)
-    else:
-        fd = os.open(name, os.O_RDWR)
-    size = os.stat(name).st_size
-    off = parts[0][0]
-    for idx in range(len(parts)):
-        if idx + 1 < len(parts):
-            next_start = parts[idx + 1][0]
-        else:
-            next_start = size
-        cur_end = parts[idx][0] + parts[idx][1]
-
-        os.lseek(fd, cur_end, os.SEEK_SET)
-        data = os.read(fd, next_start - cur_end)
-
-        os.lseek(fd, off, os.SEEK_SET)
-        os.write(fd, data)
-
-        off += len(data)
-        idx += 1
-
-    os.close(fd)
-    os.truncate(name, off)
-
-
-
-# ----------------------------------------------------------------------------
-
-class Gtest_job(object):
-    def __init__(self, parent, exe_name, exe_ts, out_file_name,
+    def __init__(self, exe_name, exe_ts, out_file_name,
                  filter_str, run_disabled, shuffle, valgrind_cmd,
                  clean_trace, clean_core, break_on_fail, break_on_except,
-                 rep_cnt, shard_cnt, shard_idx, is_bg_job, result_queue):
-        self.__parent = parent
+                 rep_cnt, shard_cnt, shard_idx, expexted_result_cnt,
+                 is_bg_job, result_queue):
+        """
+        Spawns a new test process from the given test executable file with the
+        given GTest parameters.
+        """
         self.__exe_name = test_db.test_exe_name
         self.__exe_ts = exe_ts
         self.__out_file_name = out_file_name
         self.__clean_trace = clean_trace
         self.__clean_core = clean_core
         self.__is_valgrind = bool(valgrind_cmd)
         self.__is_bg_job = is_bg_job
@@ -555,22 +332,24 @@
         self.__buf_data = b""
         self.__snippet_name = b""
         self.__snippet_data = b""
         self.__trailer = False
         self.__clean_trace_file = clean_trace
         self.__sum_input_trace = 0
         self.__failed_cnt = 0
+        self.__expected_result_cnt = expexted_result_cnt
         self.__result_cnt = 0
         self.__terminated = False
+        self.__io_error = None
         self.log = ""
 
         cmd = []
         if valgrind_cmd:
             cmd.extend(re.split(r"\s+", valgrind_cmd))
-        if valgrind_cmd and config_db.options["valgrind_exit"]:
+        if valgrind_cmd and config_db.get_opt("valgrind_exit"):
             self.__valgrind_exit = 125
             cmd.append("--error-exitcode=125")
         cmd.append(exe_name)
 
         if rep_cnt != 1:
             cmd.append("--gtest_repeat=" + str(rep_cnt))
         if filter_str:
@@ -610,20 +389,23 @@
 
         # exceptions to be caught by caller
         self.__proc = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
                                        stdin=subprocess.DEVNULL, env=env,
                                        creationflags=gtest_gui.fcntl.subprocess_creationflags())
         # Configure output pipe as non-blocking:
         # Caller is responsible for periodically calling communicate() to collect trace output
-        flags = gtest_gui.fcntl.set_nonblocking(self.__proc.stdout)
+        gtest_gui.fcntl.set_nonblocking(self.__proc.stdout)
 
         self.__out_file = open(out_file_name, "wb", buffering=0)
 
 
     def terminate(self, kill=False):
+        """
+        Terminates the controlled process by sending it the standard termination signal.
+        """
         if self.__proc:
             if kill or self.__terminated: # use more force in 2nd attempt
                 self.__proc.kill()
             else:
                 self.__proc.terminate()
 
             self.__terminated = True
@@ -635,105 +417,103 @@
                     os.remove("vgcore.%d" % self.__proc.pid)
                     os.remove("core.%d" % self.__proc.pid)
                 except OSError:
                     pass
 
 
     def abort(self):
+        """
+        Terminates the controlled process by sending it an abort signal, or a
+        regular termination signals on platforms that don't support abort.
+        """
         if self.__proc:
             if os.name == "posix":
                 self.__proc.send_signal(signal.SIGABRT)
             else:
                 self.__proc.terminate()
 
 
     def update_options(self, clean_trace, clean_core):
+        """
+        Updates values of the "clean_trace" and "clean_core" options for a
+        currently running campaign.
+        """
         self.__clean_trace = clean_trace
         self.__clean_core = clean_core
 
 
     def get_out_file_name(self):
+        """
+        Returns the name of the output file where trace read from the process'
+        pipe is stored to.
+        """
         return self.__out_file_name
 
 
     def get_stats(self):
+        """
+        Returns statistics and parameters about the test process and trace output.
+        """
         return [self.__proc.pid if self.__proc else 0,
                 self.__out_file_name,
+                self.__is_bg_job,
                 self.__sum_input_trace,
                 self.__result_cnt,
+                self.__expected_result_cnt,
                 self.__snippet_name.decode(errors="backslashreplace")]
 
 
     def is_bg_job(self):
+        """
+        Queries if the test process is configured as a "background process".
+        """
         return self.__is_bg_job
 
 
     def get_pipe(self):
+        """
+        Returns the pipe object which connects to the test processes output.
+        Returns None after the process has exited.
+        """
         return self.__proc.stdout if self.__proc else None
 
 
     def communicate(self):
+        """
+        Check for new data in pipe connected to the test process' output and
+        process it. If there is no new data, check if the process terminated.
+        New results or process exit are reported to the result queue.
+        """
         if not self.__proc:
             return False
 
-        data = gtest_gui.fcntl.read_nonblocking(self.__proc.stdout, 256*1024)
+        try:
+            # read input from the pipe to the test process
+            data = gtest_gui.fcntl.read_nonblocking(self.__proc.stdout, 256*1024)
+        except OSError as exc:
+            self.__io_error = "Error reading pipe from test process: " + str(exc)
+            self.__proc.terminate()
+            self.__terminated = True
+            data = None
 
         if data:
-            self.__sum_input_trace += len(data)
-            self.__buf_data += data
-            done_off = 0
-            for match in re.finditer(
-                  b"^\[( +RUN +| +OK +| +FAILED +| +SKIPPED +|----------|==========)\] +"
-                  b"(\S+)(?:\s+\((\d+)\s*ms\))?[^\n\r]*[\r\n]",
-                  self.__buf_data, re.MULTILINE):
-
-                if b"RUN" in match.group(1):
-                    self.__trace_to_file(self.__snippet_data)
-                    self.__trace_to_file(self.__buf_data[done_off : match.start()])
-                    self.__snippet_name = match.group(2)
-                    self.__snippet_data = self.__buf_data[match.start() : match.end()]
-                    self.__trailer = False
-
-                elif b" " in match.group(1) and not self.__trailer:
-                    if b"OK" in match.group(1):
-                        is_failed = 0
-                    elif b"SKIPPED" in match.group(1):
-                        is_failed = 1
-                    else:
-                        is_failed = 2
-                    self.__snippet_data += self.__buf_data[done_off : match.end()]
-                    self.__process_trace(match.group(2), is_failed, match.group(3), None)
-                    self.__snippet_data = b""
-                    self.__snippet_name = b""
-
-                else:
-                    self.__trace_to_file(self.__snippet_data)
-                    self.__trace_to_file(self.__buf_data[done_off : match.end()])
-                    self.__snippet_data = b""
-                    self.__snippet_name = b""
-                    self.__trailer = True
-
-                done_off = match.end()
-
-            last_line_off = find_last_line_start(self.__buf_data, done_off)
-            if self.__snippet_data:
-                self.__snippet_data += self.__buf_data[done_off : last_line_off]
-            else:
-                self.__trace_to_file(self.__buf_data[done_off : last_line_off])
-            self.__buf_data = self.__buf_data[last_line_off:]
+            self.__process_pipe(data)
+            if self.__io_error:
+                self.__proc.terminate()
+                self.__terminated = True
             return True
 
-        else:
-            retval = self.__proc.poll()
-            if retval is not None:
-                self.__process_exit(retval)
-                self.__proc = None
-                return False
+        # no data read: check if process is still alive
+        retval = self.__proc.poll()
+        if retval is not None:
+            self.__process_exit(retval)
+            self.__proc = None
+            return False
 
-            return True
+        return True
 
 
     def __process_exit(self, retval):
         # Detect TEST_PREMATURE_EXIT_FILE
         try:
             os.remove(self.__out_file_name + ".running")
             aborted = True
@@ -745,26 +525,26 @@
                 # Detect crash under valgrind
                 # (A core file from valgrind itself crashing is intentionally ignored)
                 try:
                     if self.__clean_core:
                         os.remove("vgcore.%d" % self.__proc.pid)
                         core_file = None
                     else:
-                        core_file = gtest_control_get_core_file_name(self.__out_file_name, True)
+                        core_file = trace_db.get_core_file_name(self.__out_file_name, True)
                         os.rename("vgcore.%d" % self.__proc.pid, core_file)
                 except OSError:
                     core_file = None
             else:
                 # Detect POSIX core dump file
                 try:
                     if self.__clean_core:
                         os.remove("core.%d" % self.__proc.pid)
                         core_file = None
                     else:
-                        core_file = gtest_control_get_core_file_name(self.__out_file_name, False)
+                        core_file = trace_db.get_core_file_name(self.__out_file_name, False)
                         os.rename("core.%d" % self.__proc.pid, core_file)
                 except OSError:
                     core_file = None
 
             # Detect error reported by valgrind
             valgrind_error = self.__is_valgrind and (retval == self.__valgrind_exit)
 
@@ -781,256 +561,227 @@
                 # this is a special case as we don't know which test case caused the error
                 self.__process_trace(b"", 4, 0, None)
             elif not self.__failed_cnt:
                 self.__snippet_data += self.__buf_data
                 self.__snippet_data += (b"\n[----------] Exit code: %d\n" % retval)
                 self.__process_trace(b"", 5, 0, None)
 
+        elif self.__io_error:
+            self.__snippet_data += (b"\n[----------] %s\n" % bytes(self.__io_error, "ascii"))
+            self.__process_trace(b"", 5, 0, None)
+
         else:
             self.__trace_to_file(self.__buf_data)
 
         self.__close_trace_file()
 
         # report exit to parent
         self.__result_queue.put((None, self))
 
 
+    def __process_pipe(self, data):
+        self.__sum_input_trace += len(data)
+        self.__buf_data += data
+        done_off = 0
+        for match in re.finditer(
+                rb"^\[( +RUN +| +OK +| +FAILED +| +SKIPPED +|----------|==========)\] +"
+                rb"(\S+)(?:\s+\((\d+)\s*ms\))?[^\n\r]*[\r\n]",
+                self.__buf_data, re.MULTILINE):
+
+            if b"RUN" in match.group(1):
+                self.__trace_to_file(self.__snippet_data)
+                self.__trace_to_file(self.__buf_data[done_off : match.start()])
+                self.__snippet_name = match.group(2)
+                self.__snippet_data = self.__buf_data[match.start() : match.end()]
+                self.__trailer = False
+
+            elif b" " in match.group(1) and not self.__trailer:
+                if b"OK" in match.group(1):
+                    is_failed = 0
+                elif b"SKIPPED" in match.group(1):
+                    is_failed = 1
+                else:
+                    is_failed = 2
+                self.__snippet_data += self.__buf_data[done_off : match.end()]
+                self.__process_trace(match.group(2), is_failed, match.group(3), None)
+                self.__snippet_data = b""
+                self.__snippet_name = b""
+
+            else:
+                self.__trace_to_file(self.__snippet_data)
+                self.__trace_to_file(self.__buf_data[done_off : match.end()])
+                self.__snippet_data = b""
+                self.__snippet_name = b""
+                self.__trailer = True
+
+            done_off = match.end()
+
+        last_line_off = _find_last_line_start(self.__buf_data, done_off)
+        if self.__snippet_data:
+            self.__snippet_data += self.__buf_data[done_off : last_line_off]
+        else:
+            self.__trace_to_file(self.__buf_data[done_off : last_line_off])
+        self.__buf_data = self.__buf_data[last_line_off:]
+
+
     def __process_trace(self, tc_name, is_failed, duration, core_file):
         tc_name = tc_name.decode(errors="backslashreplace")
         duration = int(duration) if duration else 0
         fail_file = ""
         fail_line = 0
         if is_failed >= 2:
             match = re.search(b"^(.*):([0-9]+): Failure", self.__snippet_data, re.MULTILINE)
             if match:
                 fail_file = os.path.basename(match.group(1).decode(errors="backslashreplace"))
                 fail_line = int(match.group(2))
             self.__failed_cnt += 1
 
         seed = ""
-        pat = config_db.options.get("seed_regexp")
+        pat = config_db.get_opt("seed_regexp")
         if pat:
             try:
                 match = re.search(pat.encode(), self.__snippet_data, re.MULTILINE)
                 if match:
                     seed = match.group(1).decode(errors="backslashreplace")
-            except:
+            except (re.error, IndexError):
                 pass
 
         trace_start_off = self.__out_file.tell()
         trace_length = len(self.__snippet_data)
         store_trace = is_failed or not self.__clean_trace
         if store_trace:
             self.__clean_trace_file = False
             self.__trace_to_file(self.__snippet_data)
 
         if is_failed >= 4: # summary error: show complete trace
             trace_start_off = 0
             trace_length = self.__out_file.tell()
 
-        self.__result_queue.put( ((tc_name, self.__exe_name, self.__exe_ts, is_failed,
-                                   self.__out_file_name if store_trace else None,
-                                   trace_start_off, trace_length, core_file,
-                                   fail_file, fail_line, duration, int(time.time()),
-                                   self.__is_valgrind, False, seed),
-                                  self.__is_bg_job) )
+        self.__result_queue.put(((tc_name, self.__exe_name, self.__exe_ts, is_failed,
+                                  self.__out_file_name if store_trace else None,
+                                  trace_start_off, trace_length, core_file,
+                                  fail_file, fail_line, duration, int(time.time()),
+                                  self.__is_valgrind, False, seed),
+                                 self.__is_bg_job))
         self.__result_cnt += 1
 
 
     def __trace_to_file(self, data):
-        # TODO catch error -> abort process
-        self.__out_file.write(data)
+        try:
+            self.__out_file.write(data)
+        except OSError as exc:
+            self.__io_error = "Error writing trace output to file: " + str(exc)
 
 
     def __close_trace_file(self):
-        self.__out_file.close()
+        try:
+            self.__out_file.close()
+        except OSError:
+            pass
+
         # delete output if "clean" option, or no result log entry (i.e. file would be invisible)
         if self.__clean_trace_file or (self.__result_cnt == 0):
             os.remove(self.__out_file_name)
         self.__out_file = None
 
 
 # ----------------------------------------------------------------------------
 
-def gtest_list_tests(pattern="", exe_file=None):
-    if exe_file is None:
-        exe_file = test_db.test_exe_name
-    cmd = [exe_file, "--gtest_list_tests"]
-    if pattern:
-        cmd.append("--gtest_filter=" + pattern)
-    try:
-        proc = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE,
-                                universal_newlines=True,
-                                creationflags=gtest_gui.fcntl.subprocess_creationflags())
-        result = proc.communicate(timeout=10)
-        if proc.returncode == 0:
-            tc_names = gtest_parse_test_list(result[0].rstrip())
-            if not tc_names:
-                msg = ('Read empty test case list from executable "--gtest_list_tests". '
-                       'Continue anyway?')
-                if not tk_messagebox.askokcancel(parent=tk_utils.tk_top, message=msg):
-                    return None
-            return tc_names
-        else:
-            msg = ("Gtest exited with error code %d when querying test case list: "
-                          % proc.returncode) + str(result[1].rstrip())
-            tk_messagebox.showerror(parent=tk_utils.tk_top, message=msg)
-            return None
-
-    except OSError as e:
-        msg = "Failed to read test case list: " + str(e)
-        tk_messagebox.showerror(parent=tk_utils.tk_top, message=msg)
-        return None
-
-
-def gtest_parse_test_list(lines):
-    tc_names = []
-    tc_suite = ""
-    for line in lines.split("\n"):
-        match = re.match(r"^([^0-9\s]\S+\.)$", line)
-        if match:
-            tc_suite = match.group(1)
-        elif tc_suite:
-            match = re.match(r"^\s+([^0-9\s]\S+)$", line)
-            if match:
-                tc_name = tc_suite + match.group(1)
-                tc_names.append(tc_name)
-            else:
-                tc_suite = ""
-    return tc_names
-
-
-def find_last_line_start(buf, off):
-    nl = b"\n"[0]
+def _find_last_line_start(buf, off):
+    nl_char = b"\n"[0]
     for idx in reversed(range(off, len(buf))):
-        if buf[idx] == nl:
+        if buf[idx] == nl_char:
             return idx + 1
     return off
 
 
-def find_prev_line_end(buf, off):
-    nl = b"\n"[0]
+def _find_prev_line_end(buf, off):
+    nl_char = b"\n"[0]
     for idx in reversed(range(off, len(buf))):
-        if buf[idx] == nl:
+        if buf[idx] == nl_char:
             return idx
     return off
 
 
-def find_next_line_end(buf, off):
-    nl = b"\n"[0]
+def _find_next_line_end(buf, off):
+    nl_char = b"\n"[0]
     for idx in range(off, len(buf)):
-        if buf[idx] == nl:
+        if buf[idx] == nl_char:
             return idx + 1
     return off
 
 
-def extract_trace(file_name, file_offs, length):
-    try:
-        with open(file_name, "rb") as f:
-            if f.seek(file_offs) == file_offs:
-                snippet = f.read(length)
-                if snippet:
-                    return snippet.decode(errors="backslashreplace")
-            #else:
-            #  print("Failed to seek in %s to %d: length %d" % (file_name, file_offs, f.seek(0, 2)), file=sys.stderr)
-    except OSError as e:
-      # use print as this function may be called from context of secondary threads
-      print("Failed to read trace file:" + str(e), file=sys.stderr)
-
-    return None
-
-
-def extract_trace_to_temp_file(tmp_dir, trace_name, file_offs, length, is_extern_import):
-    tmp_name = os.path.join(
-                    tmp_dir,
-                    gtest_control_get_temp_name_for_trace(trace_name, file_offs, is_extern_import))
-    if not os.path.exists(tmp_name):
-        try:
-            with open(trace_name, "rb") as fread:
-                if fread.seek(file_offs) == file_offs:
-                    with open(tmp_name, "wb") as fwrite:
-                        snippet = fread.read(length)
-                        fwrite.write(snippet)
-        except OSError as e:
-            tk_messagebox.showerror(parent=tk_utils.tk_top,
-                                    message="Failed to copy trace to temporary file: " + str(e))
-            tmp_name = None
-
-    return tmp_name
-
-
-# ----------------------------------------------------------------------------
-
-def gtest_import_tc_result(tc_name, is_failed, duration, snippet, start_off,
-                           file_name, file_ts, import_flag):
+def _gtest_import_tc_result(tc_name, is_failed, duration, snippet, start_off,
+                            file_name, file_ts, import_flag):
     tc_name = tc_name.decode(errors="backslashreplace")
 
     if not duration:
         duration = 0
     else:
         try:
             duration = int(duration.decode())
-        except:
+        except ValueError:
             duration = 0
 
     core_path = None
     if is_failed == 3: # CRASHED
         file_split = os.path.split(file_name)
         for with_valgrind in (False, True):
             path = os.path.join(file_split[0],
-                                gtest_control_get_core_file_name(file_split[1], with_valgrind))
+                                trace_db.get_core_file_name(file_split[1], with_valgrind))
             if os.access(path, os.R_OK):
                 core_path = path
 
     fail_file = ""
     fail_line = 0
     if is_failed:
         match = re.search(b"^(.*):([0-9]+): Failure", snippet, re.MULTILINE)
         if match:
             fail_file = os.path.basename(match.group(1).decode(errors="backslashreplace"))
             fail_line = int(match.group(2))
 
     seed = ""
-    pat = config_db.options.get("seed_regexp")
+    pat = config_db.get_opt("seed_regexp")
     if pat:
         try:
             match = re.search(pat.encode(), snippet, re.MULTILINE)
             if match:
                 seed = match.group(1).decode(errors="backslashreplace")
-        except:
+        except (re.error, IndexError):
             pass
 
     test_db.import_result((tc_name, None, 0, is_failed, file_name, start_off, len(snippet),
                            core_path, fail_file, fail_line, duration, file_ts, False,
                            import_flag, seed))
 
 
 def gtest_import_result_file(file_name, is_auto):
+    """ Import test results from the given file previously written by GTest. """
     import_flag = 1 if is_auto else 2
     file_ts = int(os.stat(file_name).st_mtime)  # cast away sub-second fraction
-    with open(file_name, "rb", buffering=0) as f:
+    with open(file_name, "rb", buffering=0) as file_obj:
         snippet_start = 0
         snippet_name = b""
         snippet_data = b""
         is_trailer = False
         # Initializing with newline to allow preceding match with "\n", as "^" is extremely slow
         buf_data = b"\n"
         file_off = -1
 
         while True:
-            new_data = f.read(256*1024)
+            new_data = file_obj.read(256*1024)
             if not new_data:
                 break
 
             buf_data += new_data
             done_off = 0
             for match in re.finditer(
-                  b"\n\[( +RUN +| +OK +| +FAILED +| +SKIPPED +| +CRASHED +|----------|==========)\] +"
-                  b"(\S+)(?:\s+\((\d+)\s*ms\))?",
-                  buf_data):
+                    rb"\n\[( +RUN +| +OK +| +FAILED +| +SKIPPED +| +CRASHED +|----------|"
+                    rb"==========)\] +(\S+)(?:\s+\((\d+)\s*ms\))?",
+                    buf_data):
 
                 if b"RUN" in match.group(1):
                     snippet_name = match.group(2)
                     snippet_data = buf_data[match.start() + 1 : match.end()]
                     snippet_start = file_off + match.start() + 1
                     is_trailer = False
 
@@ -1040,38 +791,42 @@
                     elif b"SKIPPED" in match.group(1):
                         is_failed = 1
                     elif b"FAILED" in match.group(1):
                         is_failed = 2
                     else:
                         is_failed = 3
 
-                    end_off = find_next_line_end(buf_data, match.end())
+                    end_off = _find_next_line_end(buf_data, match.end())
                     snippet_data += buf_data[done_off : end_off]
 
-                    gtest_import_tc_result(snippet_name, is_failed, match.group(3),
-                                           snippet_data, snippet_start,
-                                           file_name, file_ts, import_flag)
+                    _gtest_import_tc_result(snippet_name, is_failed, match.group(3),
+                                            snippet_data, snippet_start,
+                                            file_name, file_ts, import_flag)
                     snippet_name = b""
                     snippet_data = b""
 
                 else:
                     snippet_name = b""
                     snippet_data = b""
                     is_trailer = True
 
                 done_off = match.end()
 
-            last_line_off = find_prev_line_end(buf_data, done_off)
+            last_line_off = _find_prev_line_end(buf_data, done_off)
             if snippet_data:
                 snippet_data += buf_data[done_off : last_line_off]
             buf_data = buf_data[last_line_off:]
             file_off += last_line_off
 
 
 def gtest_automatic_import():
+    """
+    Automatically import test results from all trace files found below the
+    configured trace directory.
+    """
     try:
-        for file_name in gtest_control_search_trace_dirs():
+        for file_name in trace_db.search_trace_sub_dirs():
             gtest_import_result_file(file_name, True)
-    except OSError as e:
+    except OSError as exc:
         tk_messagebox.showerror(parent=tk_utils.tk_top,
-                                message="Error during automatic import of trace files: " + str(e))
+                                message="Error during automatic import of trace files: " + str(exc))
         return
```

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/help_db.py` & `mote-gtest-gui-0.9.0/gtest_gui/help_db.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,70 @@
 # This file is automatically generated - do not edit
 # Generated by ./doc/pod2help.py from doc/gtest_gui.pod
 
-helpIndex = {}
-helpIndex['Description'] = 0
-helpIndex['Test control'] = 1
-helpIndex['Result log'] = 2
-helpIndex['Configuration'] = 3
-helpIndex['Caveats'] = 4
-helpIndex['Files'] = 5
+""" Database containing help texts for display in the Help dialog window. """
 
-helpSections = {}
-helpSections[(1,1)] = '''Test campaign control buttons'''
-helpSections[(1,2)] = '''Test case filter'''
-helpSections[(1,3)] = '''Test control options'''
-helpSections[(3,1)] = '''User-interface options'''
-helpSections[(3,2)] = '''Test management options'''
-
-helpTexts = {}
-helpTexts[0] = (('''Description''', 'title1'), ('''
-''', ''), ('''Module-tester's GtestGui''', 'bold'), (''' is a full-featured graphical user-interface to C++ test applications using the GoogleTest framework.
-''', ''), ('''The tool will work with any application with Gtest command line interface, however it is designed especially for C++ developers using test-driven design based on module testing and integration testing. These differ from unit-testing by longer execution times and usually not fully predictable results, which in turn require multiple repetitions of each test case. To support this well, GtestGui offers firstly easily accessible ways for test case filtering and concurrent scheduling across multiple CPUs; Secondly, there are multiple features for tracking progress and managing results via sorting and filtering, which are fully usable already while a test campaign still is in progress.
+HELP_INDEX = [
+    '''Description''',
+    '''Test control''',
+    '''Result log''',
+    '''Test case list dialog''',
+    '''Job list dialog''',
+    '''Configuration''',
+    '''Caveats''',
+    '''Files''',
+]
+
+HELP_SECTIONS = {
+    (1, 1): '''Executable selection''',
+    (1, 2): '''Test campaign control buttons''',
+    (1, 3): '''Test case filter''',
+    (1, 4): '''Test control options''',
+    (1, 5): '''Status and progress monitoring''',
+    (2, 1): '''Post-mortem core dump analysis''',
+    (5, 1): '''User-interface options''',
+    (5, 2): '''Test management options''',
+}
+
+# pylint: disable=line-too-long
+HELP_TEXTS = [
+    (('''Description''', 'title1'), ('''
+''', ''), ('''Module-tester's GtestGui''', 'bold'), (''' is a test-runner with graphical user-interface for C++ test applications using the GoogleTest framework.
+''', ''), ('''GtestGui will work with any application that implements the Gtest command line interface, however it is designed especially for C++ developers using test-driven design based on module testing and integration testing. These differ from unit-testing by longer execution times and usually not fully predictable results (i.e. "flakiness"), which in turn require multiple repetitions of each test case. To support this well, GtestGui offers firstly easily accessible ways for test case filtering and concurrent scheduling across multiple CPUs; Secondly, there are multiple features for tracking progress and managing results via sorting and filtering, which are fully usable already while a test campaign still is in progress.
 ''', ''), ('''GtestGui typically is started with the path of an executable on the command line which is built using the gtest library. Using the "Run" button in the GUI, this executable can then be started and its progress be monitored live in the result log frame of the main window. Additional controls allow specifying options such as test case filter string and repetition count, which are forwarded to the executable via the respective "''', ''), ('''--gtest_*''', 'fixed'), ('''" command line arguments.
 ''', ''), ('''While tests are running, test verdicts can be monitored live in the result log. Traces of passed or failed tests can already be analyzed simply by double-clicking on an entry in the result log, which will open the trace of that particular test case run. For this purpose GtestGui comes bundled with ''', ''), ('''Trowser''', 'underlined'), (''', which is a graphical browser for large line-oriented text files. Trowser in principle is just a text browser with syntax highlighting and search, but its search capabilities are designed especially to facilitate analysis of complex debug logs, essentially by allowing to build a condensed (filtered) view of the trace file in the search result window via incremental searches and manual manipulations. By default, GtestGui is configured to user ''', ''), ('''trowser.py''', 'underlined'), (''', but there is also a more modern-looking Qt5 variant. GtestGui can also be configured to use any other GUI application for opening traces.
-''', ''), )
-
-helpTexts[1] = (('''Test control''', 'title1'), ('''
+''', ''), ),
+    (('''Test control''', 'title1'), ('''
 ''', ''), ('''The application main window consists of a menu bar, a frame containing test controls, a frame containing the test result log, and a text frame for trace preview. This chapter describes the top-most frame with the test controls.
+''', ''), ('''Executable selection''', 'title2'), ('''
+''', ''), ('''Before tests can be started or a test filter be defined, a target executable has to be selected. If the executable file was not already specified on the command line, then this is done via ''', ''), ('''Select executable file...''', 'underlined'), (''' in the ''', ''), ('''Control''', 'underlined'), (''' menu. Either select a file via the file selector dialog, or choose one from the list of previously used executables. (Note when hovering the mouse over enries in this list, the full path and timestamp of the file is displayed as tool-tip. The entry is grayed out if the file no longer exists.)
+''', ''), ('''Upon selecting an executable file, the test case list is read automatocally by running it with the "''', ''), ('''--gtest_list_tests''', 'fixed'), ('''" command line option. If that fails with an error, or if the list is empty, executable selection is aborted.
+''', ''), ('''Whenever starting a new test campaign, GtestGui will automatically check if a new executable version is available by checking the file timestamp. If a change is detected, the test case list is read again. The ''', ''), ('''Refresh test case list''', 'underlined'), (''' command in the menu allows performing the same steps independently. That command is useful if you want to specify newly added test case names in the test case filter string before starting a new test campaign (maybe to only run the new test cases.)
+''', ''), ('''Results of the previous executable are kept in the result log window, but the log entries are updated to include the executable name. Repeating test cases of other executables via the ''', ''), ('''Repeat''', 'underlined'), (''' button is not possible; You have to manually switch back to the respective executable to allow that.
+''', ''), ('''The executable cannot be "refreshed" or switched while a test campaign is running.
 ''', ''), ('''Test campaign control buttons''', 'title2'), ('''
-''', ''), ('''Most prominent in the test control frame are the green buttons, which directly control execution of the configured executable file:
+''', ''), ('''Most prominent in the test control frame are the green buttons, which directly control execution of the configured executable file. The same commands are also in the "Control" menu:
 ''', ''), ('''Run''', 'underlined'), (''':
 ''', ''), ('''Starts the text executable in a separate process, with its output redirected into a pipe which is read by GtestGui for progress monitoring. The output is also saved into a file.
-''', 'indent'), ('''Note when the timestamp of the executable file on disk has changed, GtestGui automatically reads the test case list to check for changes. An error will be reported if the current test case filter contains pattern that no longer match any test case. Note after adding a new test case, use the ''', 'indent'), ('''Refresh test case list''', ('underlined', 'indent')), (''' command in the ''', 'indent'), ('''Control''', ('underlined', 'indent')), (''' menu to read the test case list, for allowing to use the new test case name in a filter pattern.
+''', 'indent'), ('''Note when the timestamp of the executable file on disk has changed, GtestGui automatically reads the test case list to check for changes. An error will be reported if the current test case filter contains pattern that no longer match any test case. If the timestamp has not changed, the age of the file is shown in a status message below the buttons, to warn you about this in case you forget to build the executable after making changes.
 ''', 'indent'), ('''Multiple processes are started if the ''', 'indent'), ('''CPUs''', ('underlined', 'indent')), (''' value is larger than 1. Most of the time, GtestGui will use gtest's "sharding" feature, which assigns a static sub-set of tests to each process. However, if repetition count is larger than one and the number of configured CPUs is larger than the number of test cases, or if the remainder of division of test cases by CPUs is large, GtestGui may instead or additionally partition by repetitions.
-''', 'indent'), ('''Note when a test process crashes, it is currently not restarted. That is because gtest's static sharding does not allow disabling the instable test case without influencing test case partitioning.
+''', 'indent'), ('''Note when a test process crashes during a campaign, it is currently not restarted. That is because gtest's static sharding does not allow disabling the instable test case without influencing test case partitioning.
 ''', 'indent'), ('''Stop''', 'underlined'), (''':
 ''', ''), ('''Sends a TERM signal to the test processes and waits for them to finish. When termination takes a long time (possibly because the executable is hung) and the button is clicked a second time, a KILL signal is sent.
 ''', 'indent'), ('''Resume''', 'underlined'), (''':
 ''', ''), ('''Restarts test case execution using the same test case filter setting and executable version as previously used, without resetting the test result statistics. Other options, such as repetition or CPU count may be modified. This operation is useful when a long test run has to be paused temporarily as the CPUs are needed otherwise, or for changing options such as the number of used CPUs.
 ''', 'indent'), ('''This command will also use the same version of the test executable as used previously if option ''', 'indent'), ('''Create copy of executable file''', ('underlined', 'indent')), (''' is enabled, see ''', 'indent'), ('''Configuration''', ('href', 'indent')), ('''. This allows resuming execution even when the executable at the configured path no longer exists, for example due to a failed build.
 ''', 'indent'), ('''When resuming, scheduling cannot restart exactly where it was stopped due to limitations in gtest. If repetition count is 1, all test cases will be rescheduled. For higher repetition count, the lowest number of remaining repetitions across all selected test cases is rescheduled.
 ''', 'indent'), ('''Repeat''', 'underlined'), (''':
 ''', ''), ('''Repeats the test cases marked manually for repetition via the result log, or all previously failed test cases if none were selected. This allows quick repetition of individual test cases without changing the test case filter.
 ''', 'indent'), ('''Test case filter''', 'title2'), ('''
 ''', ''), ('''The entry field at the top of the test control frame allows specifying a test case filter, so that only a matching sub-set of test cases is run. The filter can be entered manually using the same syntax as the "''', ''), ('''--gtest-filter''', 'fixed'), ('''" command line option: The format of a filter expression is a ":"-separated list of test case names of wildcard patterns (positive patterns), optionally followed by a "-" and another ":"-separated pattern list (negative patterns). A test matches the filter if and only if it matches any of the positive patterns, but none of the negative ones. Wildcard characters are "*" (matching any sub-string) and "?" (matching any single character). As a special case, when no positive pattern is specified, all test cases are considered matching.
 ''', ''), ('''Alternatively, the test case filter can be modified via the drop-down menu below the entry field (which can be opened by the Cursor-Down key or a click on the drop-down button next to the entry field). The menu has entries for selecting and deselecting entries test suites as well as individual test cases. When modifying the filter this way, GtestGui will update the entry field with the shortest filter expression it can find using trailing wild card and negative patterns.
 ''', ''), ('''Yet another alternative for modifying test case filters is the test case list dialog, either via its context menu or the "Return" and "Delete" key bindings. Finally note any modification to the test case filter can be undone using "Control-Z" key binding in the entry field, or redone using "Control-Y" key binding.
+''', ''), ('''After renaming a test case or adding a new test case, use the ''', ''), ('''Refresh test case list''', 'underlined'), (''' command in the ''', ''), ('''Control''', 'underlined'), (''' menu to read the test case list from the executable file. Afterward the new test case names can be used in the filter string.
 ''', ''), ('''Test control options''', 'title2'), ('''
 ''', ''), ('''Repetitions''', 'underlined'), (''':
 ''', ''), ('''If a value larger than 1 is entered here, it is passed via the "''', 'indent'), ('''--gtest_repeat=NNN''', ('fixed', 'indent')), ('''" option on the executable's command line. This causes each test case to be repeated the given number of times.
 ''', 'indent'), ('''CPUs''', 'underlined'), (''':
 ''', ''), ('''This option is described in ''', 'indent'), ('''Test control: Test campaign control buttons''', ('href', 'indent')), ('''.
 ''', 'indent'), ('''Ignore filter''', 'underlined'), (''':
 ''', ''), ('''When more than one CPU is configured, this option can be used for scheduling different sets of test cases on different CPUs: The first set of CPUs runs only test cases matching the test case filter. The second set of CPUs runs all test cases. The size of the second set is determined by the given number.
@@ -69,47 +85,81 @@
 ''', ''), ('''When enabled, "''', 'indent'), ('''--gtest_break_on_failure''', ('fixed', 'indent')), ('''" option is set via the executable's command line. This will cause SIGTRAP to be sent to the test process upon the first failure. As no debugger is attached, this will cause the process to crash.
 ''', 'indent'), ('''When core dumps are enabled in the kernel, the core will be saved by GtestGui and can be analyzed via the ''', 'indent'), ('''Extract stack trace from core dump''', ('underlined', 'indent')), (''' command in the result log's context menu. When core dumps are not enabled, this option is probably not useful.
 ''', 'indent'), ('''Break on exception''', 'underlined'), (''':
 ''', ''), ('''When enabled, "''', 'indent'), ('''--gtest_catch_exceptions=0''', ('fixed', 'indent')), ('''" option is set via the executable's command line. This will disable catching of exceptions by the Gtest framework, which means any exception not caught by the test case itself causes the test process to crash due to an unhandled exception.
 ''', 'indent'), ('''When core dumps are enabled in the kernel, the core will be saved by GtestGui and can be analyzed via the ''', 'indent'), ('''Extract stack trace from core dump''', ('underlined', 'indent')), (''' command in the result log's context menu. When core dumps are not enabled, this option is probably not useful.
 ''', 'indent'), ('''Valgrind''', 'underlined'), (''' and ''', ''), ('''Valgrind - 2nd option set''', 'underlined'), (''':
 ''', ''), ('''The two valgrind options serve to run each execution of the test executable under valgrind using the configured command line. Notably, valgrind checks are performed across the complete lifetime of the test process, thus spanning all test cases or test repetitions. Therefore, if for example a memory leak is reported at the end, it cannot be determined which test case caused it (or it may even be caused by interaction of the test sequence.) Therefore valgrind errors are reported with a special entry in the result log. Some kind of errors such as invalid memory accesses can be mapped to test cases based on the position of the error report in the output stream. Note however that the position may not exactly reflect the timing of occurrence due to possible buffering in output streams within the test executable.) See ''', 'indent'), ('''Result log''', ('href', 'indent')), (''' and ''', 'indent'), ('''Configuration''', ('href', 'indent')), (''' for more details.
-''', 'indent'), )
-
-helpTexts[2] = (('''Result log''', 'title1'), ('''
+''', 'indent'), ('''Status and progress monitoring''', 'title2'), ('''
+''', ''), ('''The lower left part of the test control frame shows the status of the latest test campaign. The left box with label "Status" shows three numbers with the following meaning:
+''', ''), ('''Running''', 'underlined'), (''':
+''', ''), ('''Shows the number of test processes currently executing test cases. (See ''', 'indent'), ('''Caveats''', ('href', 'indent')), (''' for an explanation why this number may be lower than the number of requested "CPUs".)
+''', 'indent'), ('''Passed''', 'underlined'), (''':
+''', ''), ('''Shows the number of test cases that were passed or skipped.
+''', 'indent'), ('''Failed''', 'underlined'), (''':
+''', ''), ('''Shows the number of test cases that failed or crashed. The number also includes a possible additional fail verdict by valgrind at the end of a test process.
+''', 'indent'), ('''The left box with label "Progress" shows the completion ratio in form of a progress bar. The ratio is calculated as the number of received results (i.e. passed, skipped, failed, or crashed) divided by the number of expected results. The number of expected results is the number of test cases selected by the test case filter, multiplied with the repetition count.
+''', ''), ('''In case the ''', ''), ('''Ignore filter''', 'underlined'), (''' option in ''', ''), ('''Test control: Test control options''', 'href'), (''' is set to a non-zero value, completion ratio of the respective test jobs is disregarded for the progress display, as these jobs are terminated automatically once the regular test jobs have completed. Note the "Status" frame however does include results received from these jobs, so that the numbers shown there may exceed the configured repetition count for tests matching the test case filter.
+''', ''), ('''When hovering the mouse over the progress bar, a tool-tip text shows additional details about the progress, namely the ratio of completed test cases and repetitions and estimated remaining run time.
+''', ''), ),
+    (('''Result log''', 'title1'), ('''
 ''', ''), ('''The result log frame is located in the middle of the main window. When started for the first time, the log is usually empty. However, results can also be imported via the command line, for example from a file that contains output from a test executable that was redirected into a file. The result log may also show results from a previous run of GtestGui, if auto-import is enabled in ''', ''), ('''Configuration''', 'href'), ('''.
 ''', ''), ('''The result log contains one line for each ''', ''), ('''[ OK ]''', 'fixed'), (''', ''', ''), ('''[ SKIPPED ]''', 'fixed'), (''' and ''', ''), ('''[ FAILED ]''', 'fixed'), (''' line in the test application's gtest-generated output. The test executable's output stream is redirected to a pipe that is read continuously by GtestGui for this purpose. GtestGui also stores this output to a file, so that the trace output between ''', ''), ('''[ RUN ]''', 'fixed'), (''' and verdict text line can be opened in a trace browser.
 ''', ''), ('''In addition to the standard verdicts generated by the gtest library, GtestGui supports verdict ''', ''), ('''[ CRASHED ]''', 'fixed'), (''', which is appended to the trace file when an executable terminates with a non-zero exit code within a test case.
 ''', ''), ('''When running tests under ''', ''), ('''valgrind''', 'bold'), (''', a special result log entry "Valgrind error" is added if valgrind's exit code signals detection of an error. This case is special, as it's not known which test case caused the error, if more than one was running. Double-clicking this entry will therefore open the complete trace file.
 ''', ''), ('''Each entry in the result log contains the following information:
 ''', ''), ('''Local time at which the result was captured.
 ''', 'indent'), ('''Verdict: Passed, failed, skipped, crashed, or special case valgrind of startup errors.
 ''', 'indent'), ('''Test case name.
 ''', 'indent'), ('''"Seed" value parsed from trace output, if a regular expression was configured for that purpose in ''', 'indent'), ('''Configuration''', ('href', 'indent')), ('''.
 ''', 'indent'), ('''Test duration as reported by gtest (in milliseconds).
 ''', 'indent'), ('''In case of failure, source code file and line where of the first "Failure" was reported in trace output.
 ''', 'indent'), ('''Timestamp or name of executable that generated the test output, in case the executable has changed since running the test.
 ''', 'indent'), ('''When selecting an entry by clicking on it, the corresponding trace output is shown in the trace preview frame below the result log. In case of a test case failure, the view is centered on the first line containing "Failure" and the text is marked by light red background.
-''', ''), ('''When clicking on an entry with the right mouse button, a context menu opens that allow opening the trace file, adding or removing the selected test case from the filter option, scheduling a test for repetition, excluding a result from the log display, or removing results.
-''', ''), ('''Additional commands are offered in the "Result log" drop-down of the main window menu. The commands allow sorting and filtering the result log by various criteria.
-''', ''), ('''On UNIX platform, the context menu additionally supports extracting a thread overview and stack-trace (backtrace) of each thread from a core dump in case of a crash during execution of a test case. To allow this, ''', ''), ('''/proc/sys/kernel/core_pattern''', 'underlined'), (''' needs to be configured as "''', ''), ('''core.%p''', 'fixed'), ('''", or alternatively as "''', ''), ('''core''', 'fixed'), ('''", when additionally ''', ''), ('''/proc/sys/kernel/core_uses_pid''', 'underlined'), (''' is set to "1". If GtestGui thus finds a file named "core.PID" with PID matching that of the test executable process after a process crashed, it will automatically preserve that core file for analysis by renaming it and moving it into the directory where trace text output files are stored. It will also preserve the executable file version by keeping a hard link to the same executable.
-''', ''), )
-
-helpTexts[3] = (('''Configuration''', 'title1'), ('''
+''', ''), ('''Double-clicking on an entry opens the trace of that entry in an external application, which can be selected via the Configuration dialog. Default application is "trace browser", a text browser with syntax highlighting and search and filtering capabilities especially tailored for trace analysis. As GTest writes trace output of all test cases into a single file, only the portion between "''', ''), ('''[ RUN ]''', 'fixed'), ('''" and "''', ''), ('''[ OK ]''', 'fixed'), ('''" or "''', ''), ('''[ FAILED ]''', 'fixed'), ('''" respectively of the selected test case is extracted and passed to the application.
+''', ''), ('''When clicking on an entry with the right mouse button, a context menu opens that allow opening the trace file, adding or removing the selected test case from the filter option, scheduling a test for repetition, excluding a result from the log display, or removing results. The context menu also has an entry for sending the complete trace file to the external trace browser application; This may be needed in rare cases when behavior of a test case depends on the sequence of preceding tests.
+''', ''), ('''Additional commands are offered in the "Result log" drop-down of the main window menu. The commands allow sorting and filtering the result log by various criteria. By default, log entries are sorted by the time they were created at. When running a test campaign, it's recommended to enabled the ''', ''), ('''Show only failed''', 'underlined'), (''' filter, so that it's easy to track which test cases failed.
+''', ''), ('''While a test campaign is running, new result entries are added at the bottom (when in default sort order) and the view is scrolled automatically to keep the added entry visible. This auto-scrolling can be stopped by selecting any entry in the list. To return to auto-scrolling, deselect the last entry either by clicking on it while holding the ''', ''), ('''Control''', 'underlined'), (''' key, or by clicking in the empty line at the end of the list.
+''', ''), ('''Result entries can be deleted using the context menu or by pressing the ''', ''), ('''Delete''', 'underlined'), (''' key. To delete all entries, press ''', ''), ('''Control-A''', 'underlined'), (''' (i.e. select complete list) and then ''', ''), ('''Delete''', 'underlined'), ('''. Note actual trace files are removed from disk only if all test case results stored in it have been deleted from the log.
+''', ''), ('''Post-mortem core dump analysis''', 'title2'), ('''
+''', ''), ('''POSIX platforms only: When selecting the result of a test case that caused a crash of the test process, the context menu has an entry that allows analyzing the generated core dump file. The Analysis consists of a thread overview and stack-trace (backtrace) of each thread.
+''', ''), ('''To allow this, ''', ''), ('''/proc/sys/kernel/core_pattern''', 'underlined'), (''' needs to be configured as "''', ''), ('''core.%p''', 'fixed'), ('''", or alternatively as "''', ''), ('''core''', 'fixed'), ('''", when additionally ''', ''), ('''/proc/sys/kernel/core_uses_pid''', 'underlined'), (''' is set to "1". This way, a file named "''', ''), ('''core.PID''', 'fixed'), ('''" will be created by the operating system in the directory where GtestGui was started.
+''', ''), ('''If GtestGui thus finds a core file with a matching process ID after a process crashed, it will automatically preserve that core file for analysis by moving it into the directory where trace text output files are stored and renaming it to the same name of the corresponding trace file with prefix "core". It will also preserve the executable file version by keeping a hard link to the same executable in the trace directory for as long as the core file exists.
+''', ''), ),
+    (('''Test case list dialog''', 'title1'), ('''
+''', ''), ('''A dialog showing the list of test cases read from the selected executable file can be opened via the control menu.
+''', ''), ('''For each test case, the list shows in the first column if the test case is currently enabled for execution, the test case name, the number of times it has passed and failed in the current campaign and its accumulated execution time.
+''', ''), ('''By default, test cases in the list are in the order as received. The list can be sorted in different ways using the context menu: The list can be sorted alpabetically, by execution or failure count within the current test campaign, or by test case execution duration.
+''', ''), ('''By default, all test cases defined in the executable are listed. You can filter the list via the context menu to show only test cases enabled via test case filter in the main window, or only test cases that failed in the current test campaign, or only test cases whose name or test suite namedoesn't start with "''', ''), ('''DISABLED_''', 'fixed'), ('''".
+''', ''), ('''The "Run" column is updated to reflect changes in the "Test filter" entry field in the main window. Updates occur when you press the "Return" key, or when keyboard focus is moved out of the entry field. When the "Show only tests enabled to run" filter is active in the test case list dialog, the test case sub-set shown in the list is also updated to match the current filter string. This feature can be used for testing the manually entered filter string against the list, as you'll see exactly which test cases it selects.
+''', ''), ('''Inversely, you can use the list for modifying the test case filter in the main window: This can be done via the ''', ''), ('''Add/Remove selected test case''', 'underlined'), (''' and ''', ''), ('''Add/Remove selected test suite''', 'underlined'), (''' commands in the list's context menu. The latter works on all test cases in the test suite of the selected test case. The same can be achive via key bindings: ''', ''), ('''Return''', 'underlined'), (''' adds selected test cases and ''', ''), ('''Del''', 'underlined'), (''' removes selected test cases. Note for selecting multiple lines in the list via keyboard, hold the ''', ''), ('''Shift''', 'underlined'), (''' button while moving the cursor via the Up/Down keys.
+''', ''), ('''Test cases named "''', ''), ('''DISABLED_''', 'fixed'), ('''" can only be enabled via the test case list commands when option ''', ''), ('''Run disabled tests''', 'underlined'), (''' in the main window is checked.
+''', ''), ('''Note while the filter string is empty, all test cases are considered as enabled.  Nevertheless, the context menu will offer adding selected test cases. If you do so, then implictly all test cases except for the one added by the command get disabled.
+''', ''), ('''After making changes to the test case filter via the dialog, the filter string in the main window is updated automatically to reflect the selection. The filter uses wildcards to minimize the filter string length.
+''', ''), ),
+    (('''Job list dialog''', 'title1'), ('''
+''', ''), ('''A dialog window showing the status of test processes in a currently ongoing test campaign can be opened via the ''', ''), ('''Open job list''', 'underlined'), (''' command in the control menu. If no test campaign is active, it will only show a message informing that currently no processes are running.
+''', ''), ('''During an ongoing test campaign, the list shows for each process its ID assigned by the operating system ("PID"), if it is a background job ("BgJob"), the number of bytes of trace output received from it ("Traced"), the number of test case results found in received trace ("Results"), the percentage of completed results from expected results ("Done"), and finally the name of the current test case reported via "''', ''), ('''[ RUN ]''', 'fixed'), ('''" in received trace.
+''', ''), ('''Note a "background job" is one for which the test case filter is ignored as per ''', ''), ('''Ignore filter''', 'underlined'), (''' option in ''', ''), ('''Test control: Test control options''', 'href'), ('''. These jobs are special as they are terminated automatically when the last regular job is completed. For this reason their completion ratio (i.e. "Done" column) is disregarded for progress display in the main window.
+''', ''), ('''The dialog is useful in case you suspect that a test campaign may be hung (for example when a test case ran into a deadlock or busy loop.) You could notice that firstly by the number of results not increasing and if that's the case, by the number of received bytes received as trace output not increasing. (The latter will however not if your test cases generate few or no trace output.)
+''', ''), ('''The context menu allows sending an ''', ''), ('''ABORT''', 'underlined'), (''' signal to the process, which will terminate it and cause a core image to be dumped on UNIX. The test case will be reported as crashed in the result log. This can be used for debugging a hung process: You can find where it was hung by using the ''', ''), ('''Extract stack trace from core dump''', 'underlined'), (''' command in context menu of the result log entry. Alternatively, you could use the PID for attaching a debugger to the live process (e.g. "''', ''), ('''gdb -p PID exe_file''', 'fixed'), ('''").
+''', ''), ),
+    (('''Configuration''', 'title1'), ('''
 ''', ''), ('''User-interface options''', 'title2'), ('''
 ''', ''), ('''A few simple options for the user interface are available directly in the ''', ''), ('''Configure''', 'underlined'), (''' menu:
 ''', ''), ('''Select font for result log''', 'underlined'), (''':
 ''', ''), ('''Selects the font used in the result log list in the main window, as well as in the test case list and job list dialogs. By default, the font is determined by Python's Tkinter and depends on the platform.
 ''', 'indent'), ('''Select font for trace preview''', 'underlined'), (''':
 ''', ''), ('''Selects the font used in the trace preview frame at the bottom of the main window. By default, a fixed font is used; Font family and size are determined by Python's Tkinter and depend on the platform.
 ''', 'indent'), ('''Show test controls''', 'underlined'), (''':
 ''', ''), ('''This option can be unchecked for temporarily hiding the test control frame in the main window. This allows for more space for the result log during result analysis. This option is not stored in persistent configuration and will always be enabled upon start of the application. Note while the controls are not shown, some operations are still possible via key bindings as well as the ''', 'indent'), ('''Control''', ('underlined', 'indent')), (''' menu.
 ''', 'indent'), ('''Show tool-tip popups''', 'underlined'), (''':
 ''', ''), ('''The option can be unchecked to disable display of "tool-tip" popup windows when hovering with the mouse on labels or check-buttons in the main window and dialogs which have such built-in help. Changes of the option are stored in the configuration file, so that it is persistent. This may be useful once you are sufficiently familiar with the tool.
 ''', 'indent'), ('''Test management options''', 'title2'), ('''
+''', ''), ('''The following configuration options are available in the ''', ''), ('''Options''', 'underlined'), (''' dialog window that can be opened via the ''', ''), ('''Configure''', 'underlined'), (''' menu:
 ''', ''), ('''Trace browser''', 'underlined'), ('''
 ''', ''), ('''This entry field selects the external application used for displaying trace files and trace snippets, when double-clicking on an entry in the result log. By default, trace browser ''', 'indent'), ('''trowser.py''', ('underlined', 'indent')), (''' is used. You can either specify just the application file name, or its full path if it is not found via ''', 'indent'), ('''PATH''', ('fixed', 'indent')), (''' configured in environment. The path of the trace file to be displayed will be appended to the given command line.
 ''', 'indent'), ('''Currently the application path name or parameters cannot contain space characters, as these are assumed to be separators.
 ''', 'indent'), ('''Note for the Windows platform: When using the default of ''', 'indent'), ('''trowser.py''', ('fixed', 'indent')), (''', you may need to insert the Python interpreter in front of "trowser.py", depending on your Python installation. In that case you need to add the full path to where ''', 'indent'), ('''trowser.py''', ('fixed', 'indent')), (''' is installed.
 ''', 'indent'), ('''Enable option ''', 'indent'), ('''Browser supports reading from STDIN''', ('underlined', 'indent')), (''' if the selected trace browser supports reading text from "standard input" via a pipeline. In this case filename "''', 'indent'), ('''-''', ('fixed', 'indent')), ('''" is passed on the command line instead of a file name.  The default browser ''', 'indent'), ('''trowser.py''', ('underlined', 'indent')), (''' supports this. When not enabled, GtestGui has to create temporary files for passing trace snippets to the browser application.
 ''', 'indent'), ('''Pattern for seed''', 'underlined'), ('''
 ''', ''), ('''If a regular expression pattern is specified here, it will be applied to the trace of each test case. The string returned by the first match group (i.e. the first set of capturing parenthesis) will be shown in the corresponding result log as "seed". (This is intended for allowing repeat of a test sequence exactly even for test cases using randomness, by starting their PRNG with the same seed. This is not yet supported however, due to lack of an interface for passing a list of seed values via the GTest command line interface.)
@@ -124,34 +174,32 @@
 ''', 'indent'), ('''Valgrind command line''', 'underlined'), ('''
 ''', ''), ('''UNIX only:''', ('underlined', 'indent')), (''' Command lines to use for running test executables when one of the "Valgrind" options in the main window is enabled. The executable name and gtest options will be appended to the given command line.
 ''', 'indent'), ('''There are two separate entry fields, corresponding to the two check-buttons in the main window. This is intended for allowing to configure a configuration variant that runs faster and one that is slower but performs deeper analysis. By default, the command will perform check for memory leaks (notably at end of all test cases, not for individual test cases in a run of multiple tests) and for use of uninitialized memory. The second command line has additional options for tracking the origin of uninitialized memory.
 ''', 'indent'), ('''Currently the path or parameters cannot contain space characters, as these are assumed to be separators.
 ''', 'indent'), ('''Valgrind supports --exit-code''', 'underlined'), ('''
 ''', ''), ('''When this option is set, parameter "--error-exitcode=125" will be appended to the given valgrind command lines. This is required for detecting automatically that valgrind found errors during test execution. Only when enabled, result logs will report valgrind errors.
 ''', 'indent'), ('''The debugger used for extracting stack traces from core files (POSIX only) is currently not configurable; It is hard-coded to "''', ''), ('''gdb''', 'fixed'), ('''", which should be somewhere in the ''', ''), ('''PATH''', 'fixed'), (''' configured in environment.
-''', ''), )
-
-helpTexts[4] = (('''Caveats''', 'title1'), ('''
+''', ''), ),
+    (('''Caveats''', 'title1'), ('''
 ''', ''), ('''This chapter lists notable limitations that are not easy to overcome due to design choices.
 ''', ''), ('''Concurrent scheduling
-''', ''), ('''Concurrent scheduling requested via option ''', 'indent'), ('''CPUs''', ('underlined', 'indent')), (''' is based on the "sharding" feature provided by Gtest framework. Unfortunately, Gtest only supports static case test partitioning, which means for example when using two CPUs, the set of test cases is split in two parts, of which the first is executed in one test process and the second in the second process.
-''', 'indent'), ('''One problem arises when the number of test cases is smaller than the number of CPUs. This typically occurs, when trying to run a single test case many times. Sharding would then only use a single CPU, as it does not consider repetitions in its "sharding" algorithm. GtestGui works around that by calculating if it is more efficient to partition test cases by repetition than by sharding, or if a combination of both is even better. In the mentioned example, it would not use sharding, but instead run half the number of repetitions in one process, and the second half in the second. For more complex configurations such as 10 repetitions of 9 test cases on 8 CPUs, a combination of both methods will be used.
-''', 'indent'), ('''A second problem that GtestGui cannot work around occurs when test cases have non-uniform execution time. As the "sharding" algorithm uses static partitioning solely based on the number of test cases per process, differences in execution times are not considered. For example, when two tests are scheduled for 100 times and test case A takes 1 second, but test case B only 1 millisecond, Gtest will still schedule all runs of A in the first process and all runs of B in the second process. Thus, the second process will sit idle for 99.9% of the total test execution time.
+''', ''), ('''Concurrent scheduling requested via option ''', 'indent'), ('''CPUs''', ('underlined', 'indent')), (''' is based on the "sharding" feature provided by Gtest framework. Unfortunately, Gtest only supports static case test partitioning, which means for example when using two CPUs, the set of test cases is split in two parts, of which the first is executed in one test process and the second in the other process.
+''', 'indent'), ('''One problem arises when the number of test cases is smaller than the number of requested CPUs. This typically occurs when trying to run a single test case many times.  Sharding would then only use a single CPU, as it does not consider repetitions in its "sharding" algorithm. GtestGui works around that by calculating if it is more efficient to partition test cases by repetition than by sharding, or if a combination of both is even better. In the mentioned example, it would not use sharding, but instead run half the number of repetitions in one process, and the second half in the second. For more complex configurations such as 10 repetitions of 9 test cases on 8 CPUs, a combination of both methods will be used.
+''', 'indent'), ('''A second problem, that GtestGui cannot work around, occurs when test cases have non-uniform execution time. As the "sharding" algorithm uses static partitioning solely based on the number of test cases per process, differences in execution times are not considered. For example, when two tests are scheduled for 100 times and test case A takes 1 second, but test case B only 1 millisecond, Gtest will still schedule all runs of A in the first process and all runs of B in the second process. Thus, the second process will sit idle for 99.9% of the total test execution time.
 ''', 'indent'), ('''Test case crashes
 ''', ''), ('''In a well-behaved test application, failures are normally reported via Gtest macros or exceptions. Thus, the failure is recorded and the next test case is executed. Sometimes however, a test case may have a bug that leads to a crash of the complete process. In this case all following test cases or test case repetitions are no longer executed.
 ''', 'indent'), ('''Currently GtestGui will not attempt to restart tests after a crash, because it expects that the same test case will crash again and thus keep blocking following tests. It is not possible to disable the instable test, as this would interfere with partitioning by Gtest "sharding", i.e. the set of test cases run by that test case would be altered. The only way around is for the use to manually disable the instable test case and then restart the test campaign.
 ''', 'indent'), ('''Overload of GUI by concurrent unit-testing
 ''', ''), ('''When using multiple CPUs for running very short-running test cases, such as typical unit-tests, the GUI application may be overloaded and thus appear unresponsive and hung. This is a result of Python's implementation of multi-threading, which does not allow using more than one effective CPU due to exclusive locks in interpreter execution. Therefore, when parsing of test output streams takes 100% of a CPU, no time is left for updating the GUI even though separate threads are used.
 ''', 'indent'), ('''For more minor constraints and ideas for enhancements see file ''', ''), ('''TODO.txt''', 'fixed'), (''', which is part of the package.
-''', ''), )
-
-helpTexts[5] = (('''Files''', 'title1'), ('''
+''', ''), ),
+    (('''Files''', 'title1'), ('''
 ''', ''), ('''$HOME/.config/gtest_gui/gtest_gui.rc''', 'bold'), ('''
 ''', ''), ('''This file stores parameters that are configured via the ''', 'indent'), ('''Configuration''', ('href', 'indent')), (''' dialog. Additional it contains persistent state such as the list of previously loaded executable files and the size and position of resizable dialog windows.
 ''', 'indent'), ('''trace.NNNN/trace.NNNN''', 'bold'), ('''
 ''', ''), ('''Output from test applications is stored to sub-directories files called "''', 'indent'), ('''trace.''', ('fixed', 'indent')), ('''" with a number appended. The number is an arbitrary identifier for the test executable whose output they contain. The directory contains a separate output file for each spawned test process.  Files in this directory are removed when removing results in the ''', 'indent'), ('''Result log''', ('href', 'indent')), (''' of the GUI. By default, traces containing only passed test case results are also cleaned upon exiting the GUI.
 ''', 'indent'), ('''By default, the sub-directories are created in the current working directory where GtestGui is started. Another base directory may be specified in ''', 'indent'), ('''Configuration''', ('href', 'indent')), ('''.
 ''', 'indent'), ('''If multiple instances of the GUI are started, they will use the same directory for storage. For single-user systems this works well enough, as conflicts may occur only when pressing "Run" button concurrently in different instances. For multi-user setup it is not recommended to share the directory. (Seeing other user's test results would be confusing anyway.)
 ''', 'indent'), ('''TEMP/gtest_gui_tmpXXX''', 'bold'), ('''
 ''', ''), ('''A temporary directory at the default place used by the operating system for such purpose will be created, for for example for unpacking trace snippets for display, or exporting trace files to archives. A different directory is used by each instance of GtestGui. The directory is removed automatically when the GUI is closed. Note the latter may fail on some platforms if a trace browser application still has opened an exported trace file at the time of quitting the GUI.
-''', 'indent'), )
-
+''', 'indent'), ),
+]
```

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/main.py` & `mote-gtest-gui-0.9.0/gtest_gui/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,113 +13,127 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
+"""
+This module implements the main entry point which starts-up Tk, parses the
+command line and processes command line arguments and then creates the main
+window. Finally, control is passed to the Tk event handler.
+"""
+
 import os
 import sys
 from tkinter import messagebox as tk_messagebox
 import tkinter as tk
 
+from gtest_gui.dlg_main import MainWindow
+from gtest_gui.dlg_config import ConfigDialog
+
 import gtest_gui.config_db as config_db
-import gtest_gui.dlg_main as dlg_main
-import gtest_gui.dlg_config as dlg_config
-import gtest_gui.gtest as gtest
-import gtest_gui.test_db as test_db
+import gtest_gui.gtest_ctrl as gtest_ctrl
 import gtest_gui.tk_utils as tk_utils
 
 
 def parse_argv_error(tk_top, msg, with_usage=True):
+    """ Print usage and exit upon command line parser error. """
     if msg[-1] != "\n":
         msg += "\n"
     if with_usage:
         msg += "Usage: %s {[-trace] file}* [executable]" % sys.argv[0]
 
-    if (os.name == "posix"):
+    if os.name == "posix":
         print(msg, file=sys.stderr)
     else:
         tk_messagebox.showerror(parent=tk_top, message=msg)
 
     sys.exit(1)
 
 
 def parse_argv(tk_top):
+    """ Parse command line arguments and return them in form of a list. """
     exe_name = ""
     trace_files = []
     next_is_trace = False
     for file_name in sys.argv[1:]:
         if file_name.startswith("-trace"):
             next_is_trace = True
             continue
-        elif file_name.startswith("-"):
+        if file_name.startswith("-"):
             parse_argv_error(tk_top, "Unknown command line option: %s" % file_name)
 
-        try:
-            st = os.stat(file_name)
-        except OSError as e:
-            # Note the file name is already included in the exception text
-            parse_argv_error(tk_top, "Failed to access file: %s" % str(e), False)
+        if not os.access(file_name, os.R_OK):
+            parse_argv_error(tk_top, "Trace file '%s' not found or inaccessible" % file_name, False)
 
-        if (os.name == "posix"):
+        if os.name == "posix":
             is_exe = os.access(file_name, os.X_OK)
         else:
             is_exe = os.path.splitext(file_name)[1] == ".exe"
 
         if is_exe and not next_is_trace:
             if exe_name:
-                parse_argv_error(tk_top, "More than one executable on the command line: %s" % file_name)
+                parse_argv_error(tk_top,
+                                 "More than one executable on the command line: %s" % file_name)
             exe_name = file_name
         else:
             trace_files.append(file_name)
 
         next_is_trace = False
 
     return (exe_name, trace_files)
 
 
 # ----------------------------------------------------------------------------
 
 def main():
+    """
+    Main entry point of the application: Initialize Tk and internal modules,
+    parse the command line arguments, import pre-existing results from files
+    and then create the GUI widgets and pass control to Tk. Upon errors,
+    application process is terminated with exit code 1.
+    """
     try:
         tk_top = tk.Tk(className="gtest_gui")
         tk_top.wm_withdraw()
         tk_top.wm_title("GtestGui")
-    except Exception as e:
-        print("Tk initialization failed: " + str(e), file=sys.stderr)
+    except tk.TclError as exc:
+        print("Tk initialization failed: " + str(exc), file=sys.stderr)
         sys.exit(1)
 
     exe_name, trace_files = parse_argv(tk_top)
 
     tk_utils.initialize(tk_top)
-    gtest.initialize()
+    gtest_ctrl.initialize()
 
     config_db.rc_file_load()
 
-    if config_db.options["startup_import_trace"]:
-        if config_db.options["trace_dir"] and not os.path.exists(config_db.options["trace_dir"]):
+    if config_db.get_opt("startup_import_trace"):
+        if config_db.get_opt("trace_dir") and not os.path.exists(config_db.get_opt("trace_dir")):
             answer = tk_messagebox.showwarning(
                 parent=tk_top, type="okcancel",
-                message="Warning: Configured trace directory does not exist. Please check configuration.")
+                message="Warning: Configured trace directory does not exist. " \
+                        "Please check configuration.")
             if answer == "ok":
-                dlg_config.create_dialog(tk_top)
+                ConfigDialog.create_dialog(tk_top)
         else:
-            gtest.gtest_automatic_import()
+            gtest_ctrl.gtest_automatic_import()
 
     for file_name in trace_files:
         try:
-            gtest.gtest_import_result_file(file_name, False)
-        except OSError as e:
-            msg = "Failed to import %s: %s" % (file_name, str(e))
+            gtest_ctrl.gtest_import_result_file(file_name, False)
+        except OSError as exc:
+            msg = "Failed to import %s: %s" % (file_name, str(exc))
             tk_messagebox.showerror(parent=tk_top, message=msg)
             sys.exit(1)
 
-    global wid_main
-    wid_main = dlg_main.Main_window(tk_top, exe_name)
+    # Construct the main window. This object is used only indirectly via Tk event handling.
+    # pylint: disable=unused-variable
+    wid_main = MainWindow(tk_top, exe_name)
 
     tk_top.wm_deiconify()
 
     try:
         tk_top.mainloop()
     except KeyboardInterrupt:
         pass
```

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/tool_tip_db.py` & `mote-gtest-gui-0.9.0/gtest_gui/tool_tip_db.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,328 +13,388 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
-tips = {
-
-# Main window: Control menu
-'test_ctrl.cmd_start_campaign':
-'''
+"""
+This module stores help texts to be displayed as tool tips when hovering the
+mouse over GUI widgets. The database is a dict containing a unique key and
+assigned help texts. The keys are used to avoid including the texts directly
+within the code creating the dialogs. Note white-space in help texts is
+removed before display, as the text is formatted automatically.
+"""
+
+TOOL_TIP_DB = {
+
+    # Main window: Control menu
+    'test_ctrl.cmd_start_campaign':
+    '''
 Resets result counters and starts a new test campaign by running the configured
 executable in a process with the selected test case filter and options. If the
 executable has changed since the last run, the test case list is refreshed
 automatically.
 ''',
 
-'test_ctrl.cmd_stop_campaign':
-'''
+    'test_ctrl.cmd_stop_campaign':
+    '''
 Stops an ongoing test campaign by terminating the test processes. (Stop again
 for killing the processes in case they do not terminated.)
 ''',
 
-'test_ctrl.cmd_resume_campaign':
-'''
+    'test_ctrl.cmd_resume_campaign':
+    '''
 Resumes a previously stopped test campaign with the same test case filter.
 There will be a warning if the test case selection changed since the previous
 run. Other options, such as CPU or repetition counts may be changed freely.
 ''',
 
-'test_ctrl.cmd_repeat':
-'''
+    'test_ctrl.cmd_repeat':
+    '''
 Repeats the test cases marked manually for repetition via the result log, or
 all previously failed test cases if none were selected. This command allows
 quick repetition of individual test cases without changing the filter.
 ''',
 
-'test_ctrl.cmd_tc_list':
-'''
+    'test_ctrl.cmd_tc_list':
+    '''
 Open a dialog window that displays all test case names read from the configured
 executable via option "--gtest_list_tests". Use the dialog's context menu for
 filtering or sorting.
 ''',
 
-'test_ctrl.cmd_job_list':
-'''
+    'test_ctrl.cmd_job_list':
+    '''
 Open a dialog window that displays the status of currently running test
 processes. Use the dialog's context menu for aborting a process in case it is
 hung.
 ''',
 
-'test_ctrl.cmd_refresh':
-'''
+    'test_ctrl.cmd_refresh':
+    '''
 Reads the list of test cases from the current executable using gtest command
 line option "--gtest_list_tests". Afterward, newly added test case names can be
 used in test case filter.
 ''',
 
-# Main window: test case filter entry field
-'test_ctrl.tc_filter':
-'''
+    # Main window: test case filter entry field
+    'test_ctrl.tc_filter':
+    '''
 If not blank, only test cases matching this filter expression are run. Either
 specify complete test case names, or use patterns containing "*" (matches any
 string) or "?" (matches any single character). The format of a filter
 expression is a ":"-separated list of wildcard patterns (positive patterns),
 optionally followed by a "-" and another ":"-separated pattern list (negative
 patterns). A test matches the filter if and only if it matches any of the
 positive patterns, but none of the negative ones.
 This entry field supports undo/redo via Control-Z and Control-Y.
 ''',
 
-# Main window: test control spinbox options
-'test_ctrl.job_count':
-'''
+    # Main window: test control spinbox options
+    'test_ctrl.job_count':
+    '''
 Number of processes to spawn which will execute tests concurrently.
 Gtest\'s "sharding" feature is used for partitioning the set of test cases into
 sub-sets. For small number of tests, GtestGui may additionally partition by
 repetiton count for achieving better load distribution.  Due to static
 partitioning, some processes may finish early if test case execution times are
 non-uniform.
 ''',
 
-'test_ctrl.job_runall':
-'''
+    'test_ctrl.job_runall':
+    '''
 Number of test processes in which to run the full set of test cases instead of
 the sub-set specified by the "Test filter" expression. The number has to be
 less than that given for "CPUs". These "background" processes will be
 terminated once the regular test processes have completed; Their results are
 displayed normally, but they are not reflected in "Progress" reporting. Note
 this feature is intended for allowing increase of repetition rate of a sub-set
 of tests in long-running stress testing.
 ''',
 
-'test_ctrl.repetitions':
-'Number of times to run each test case',
+    'test_ctrl.repetitions':
+    'Number of times to run each test case',
 
-'test_ctrl.max_fail':
-'''
+    'test_ctrl.max_fail':
+    '''
 Stop all test processes when the given number of test failures is reached, or
 never when the limit is set to 0. (Due to pipelining and concurrency, the
 actual number of reported failures may exceed this value.)
 ''',
 
-# Main window: test control checkbuttons
-'test_ctrl.clean_trace':
-'''
+    # Main window: test control checkbuttons
+    'test_ctrl.clean_trace':
+    '''
 When enabled, trace output of passed test case runs is discarded. This avoids
 filling up your disk with traces when using high repetition counts.
 ''',
 
-'test_ctrl.clean_core':
-'''
+    'test_ctrl.clean_core':
+    '''
 When enabled, core dump files generated by crashes of the test executable are
 removed from disk automatically. When not enabled, core dump files are renamed
 and stack traces can be extracted via the result log.  Note this feature only
 works if pattern for core files is configured as "core.%PID". The feature is
 only applicable if core dumps are enabled in the kernel.
 ''',
 
-'test_ctrl.shuffle':
-'''
+    'test_ctrl.shuffle':
+    '''
 Sets option "--gtest_shuffle", which randomizes the order in which test cases
 are executed.
 ''',
 
-'test_ctrl.run_disabled':
-'''
+    'test_ctrl.run_disabled':
+    '''
 Sets option "--gtest_also_run_disabled_tests", which enables execution of test
 cases or test suites with prefix "DISABLED" (if also matching the given test
 filter expression.)
 ''',
 
-'test_ctrl.break_on_fail':
-'''
+    'test_ctrl.break_on_fail':
+    '''
 Sets option "--gtest_break_on_failure", which will have the test executable
 crash with signal "TRAP" upon the first test case failure. This is useful only
 when core dumps are enabled.
 ''',
 
-'test_ctrl.break_on_except':
-'''
+    'test_ctrl.break_on_except':
+    '''
 Sets option "--gtest_catch_exceptions=0", which will have the test executable
 crash when a test case throws an unhandled exception. This is useful only when
 core dumps are enabled.
 ''',
 
-'test_ctrl.valgrind1':
-'''
+    'test_ctrl.valgrind1':
+    '''
 Executes test processes under valgrind, using the valgrind command line
 specified in configuration.  If valgrind detects errors, a special "valgrind"
 entry is added to the result log after all test cases have run. To find which
 test case caused the error, use "Open trace of complete test run" and search it
 for valgrind messages (e.g. lines starting with "==").
 ''',
 
-'test_ctrl.valgrind2':
-'''
+    'test_ctrl.valgrind2':
+    '''
 Executes test processes under valgrind, using the alternate valgrind command
 line specified in configuration.
 ''',
 
-# Main window: Configuration menu
-'config.select_font_content':
-'''
+    # Main window: Configuration menu
+    'config.select_font_content':
+    '''
 Configures the font used for displaying the result log in the main window and
 test case or job lists in dialog windows.
 ''',
 
-'config.select_font_trace':
-'''
+    'config.select_font_trace':
+    '''
 Configures the font used for displaying trace output text at the bottom of the
 main window.
 ''',
 
-'config.show_controls':
-'''
+    'config.show_controls':
+    '''
 When unchecked, the part of the main window showing the test case filter,
 options and start/stop buttons is hidden, so that there is more screen space
 for the result log.  You can still start and stop test campaigns via the
 control menu.
 ''',
 
-'config.show_tool_tips':
-'''
+    'config.show_tool_tips':
+    '''
 When unchecked, tool-tips like this one are globally disabled.
 ''',
 
-# Configuration dialog
-'config.trowser':
-'''
+    # Main window: Result log menu
+    'result_log.filter_failed':
+    '''
+Show only results of failed test cases in the result log.
+''',
+
+    'result_log.filter_exe_file':
+    '''
+Show only results generated by the executable file currently configured as test
+target. (This filter is updated when switching to a different executable.)
+''',
+
+    'result_log.filter_exe_version':
+    '''
+Show only results generated by the same same or newer version (i.e. timestamp)
+of the currently selected executable, or the latest version if no result is
+selected. The version threshold is selected only when enabling the filter;
+The version threshold is not updated when starting tests with a new executable
+version.
+''',
+
+    'result_log.filter_tc_name':
+    '''
+Show only results generated by the same test cases with the same name as
+currently selected results. At least one test case in the result log needs to be
+selected for enabling the filter.
+''',
+
+    'result_log.sort_tc_name':
+    '''
+Sort results shown in the log by test case name.
+''',
+
+    'result_log.sort_seed':
+    '''
+Sort results shown in the log by the "seed" value. (The seed value is a
+string extracted from trace output by a freely configurable regular
+expression.)
+''',
+
+    'result_log.sort_duration':
+    '''
+Sort results shown in the log by test case execution duration.
+''',
+
+    'result_log.sort_failure':
+    '''
+Sort results shown in the log by source code module and line number where
+the first failure occurred.
+''',
+
+
+    # Configuration dialog
+    'config.trowser':
+    '''
 Defines which application to use for opening trace snippets and complete trace
 files. The file name will be appended to the given command line. The
 application path or parameters must not contain spaces. The PATH configured in
 environment will be used to search for the comment, so that normally the full
 path need not be specified. (Note for the Windows platform, you may need to add
 the Python interpreter in front of "trowser.py", depending on your Python
 installation.)
 ''',
 
-'config.trowser_stdin':
-'''
+    'config.trowser_stdin':
+    '''
 Enable this if the selected trace browser supports reading text from "standard
 input" via a pipeline. In this case filename "-" is passed on the command line.
 The default browser "trowser" supports this. When not enabled, GtestGui has to
 create temporary files for passing trace snippets to the browser application.
 ''',
 
-'config.seed':
-'''
+    'config.seed':
+    '''
 If a regular expression pattern is specified here, it will be applied to the
 trace of each test case. The string returned by the first match group (i.e.
 the first set of capturing parenthesis) will be shown in the corresponding
 result log as "seed". (This is intended for allowing repeat of a test sequence
 exactly even for test cases using randomness, by starting their PRNG with the
 same seed. This is not yet supported however, due to lack of an interface for
 passing a list of seed values via the GTest command line interface.)
 ''',
 
-'config.trace_dir':
-'''
+    'config.trace_dir':
+    '''
 Specifies the directory where to store temporary files for trace output and
 core dump files collected from the executable under test. If empty, the current
 working directory at the time of starting GtestGui is used. Note
 sub-directories will be created in the given directory for each executable file
 version. If you want to use the "copy executable" option, the specified
 directory needs to be in the same filesystem as the executables. If you want to
 keep core dumps, the directory needs to be in the same filesystem as the
 working directory (because they will be moved, not copied due to size.)
 ''',
 
-'config.exit_clean_trace':
-'''
+    'config.exit_clean_trace':
+    '''
 When enabled, output from passed test cases is automatically removed from
 created trace files upon exiting the application. Trace files and
 sub-directories only containing passed test results are thus removed entirely.
 Note imported trace files are never modified or removed automatically, so you
 may need to remove these manually once after enabling this option (e.g. via
 result log context menu).
 ''',
 
-'config.startup_import_trace':
-'''
+    'config.startup_import_trace':
+    '''
 When enabled, all trace files found in sub-directories under the configured
 trace directory are read after starting GtestGui. Test case results found in
 the files are shown in the result log window.
 ''',
 
-'config.copy_executable':
-'''
+    'config.copy_executable':
+    '''
 When enabled, a copy of the current executable under test is made within the
 configured trace directory. (Technically, the copy is achieved by creating a
 so-called "hard link", so that no additional disk space is needed.) This is
 recommended so that recompiling the executable does not affect the current test
 run (i.e. compilation may either fail with error "file busy" when tests are
 running, or tests may crash). This option is required for allowing to extract
 stack traces from core dump files taken from an older executable version. Note
 this option may not work when using trace directories in locations such as /tmp
 on UNIX-like systems, as these usually are configured to disallow executable
 files for security reasons.
 ''',
 
-'config.valgrind1':
-'''
+    'config.valgrind1':
+    '''
 Command line to use for running test executables when the "Valgrind" option in
 the main window is enabled. The executable name and gtest options will be
 appended to the given command line. (Note command line parameters must not
 contain spaces, as space is assumed to be separator character.)
 ''',
 
-'config.valgrind2':
-'''
+    'config.valgrind2':
+    '''
 Command line to use for running test executables when "Valgrind - 2nd option set"
 is enabled in the main window.
 ''',
 
-'config.valgrind_exit':
-'''
+    'config.valgrind_exit':
+    '''
 When this option is set, parameter "--error-exitcode=125" will be appended to
 the given valgrind command lines. This is required for detecting automatically
 that valgrind found errors during test execution. Only when enabled, result
 logs will report valgrind errors.
 ''',
 
-# Debug dialog
-'debug.lookup':
-'''
+    # Debug dialog
+    'debug.lookup':
+    '''
 After clicking this button, all global variables with the prefix entered in the
 entry field to the left are shown in the "Output" frame. When the field is
 empty, all globals of module "dlg_main" are shown. To see globals of other
 modules, enter the module name followed by a dot. To see attributes of a class
 instance, type the name of the variable holding the reference followed by a
 dot. When clicking on a name shown in the "Output" frame afterward, the
 variable's value is shown in the "Input" frame in form of an assignment. (The
 idea is that the value can then by modified by editing the content and
 "Execute", however this only works for integral values and types that print
 their value in form of a constructor call.)
 ''',
 
-'debug.eval':
-'''
+    'debug.eval':
+    '''
 When clicking this button, the complete content of the "Input" text entry field
 is passed to Python's "eval()" function. The result is converted to a string
 and shown in the "Output" frame. Note Python's "eval()" only accepts
 expressions (including function calls, but not for example assignments.)
 You can run this command also via key binding "Control-E".
 ''',
 
-'debug.exec':
-'''
+    'debug.exec':
+    '''
 When clicking this button, the complete content of the "Input" text entry field
 is passed to Python's "exec()" function. The "Output" frame will show "None" in
 case of success, or else an error or exception message. Note the output of
 "print()" will be shown on the console where you started Python instead of this
 window. You can run this command also via key binding "Control-X".
 ''',
 
-'debug.clear':
-'''
+    'debug.clear':
+    '''
 Clears the content of the "Output" frame.
 ''',
 
-'debug.new':
-'''
+    'debug.new':
+    '''
 Opens a new window just as this one.
 ''',
 
 }
```

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/wid_status_line.py` & `mote-gtest-gui-0.9.0/gtest_gui/wid_status_line.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,45 +13,61 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
-import re
+"""
+This module implements the status line widget class.
+"""
+
 import tkinter as tk
 
 import gtest_gui.tk_utils as tk_utils
 
-stline = None
-
-def create_widget(tk_top, parent):
-    global stline
-    stline = Status_line_widget(tk_top, parent)
-
-
-def show_message(msg_type, msg_txt):
-    stline.show_message(msg_type, msg_txt)
+class StatusLineWidget:
+    """
+    Status line widget class (singleton). An instance of this class is created
+    once during start-up. A reference to it can be retrieved using the getter
+    interface and then be used for displaying temporary messages. The message is
+    displayed using a temporary widget that is as an overlay into the main
+    window.
+    """
+    __stline = None
+
+    @classmethod
+    def create_widget(cls, tk_top, parent):
+        """ Initializes the class. """
+        cls.__stline = StatusLineWidget(tk_top, parent)
+
+
+    @classmethod
+    def get(cls):
+        """ Returns the status line widget (singleton)."""
+        return cls.__stline
 
 
-def clear_message():
-    stline.clear()
-
-
-class Status_line_widget(object):
     def __init__(self, tk_top, parent):
-        self.tk = tk_top
+        """ Creates the singleton instance. """
+        self.tk_top = tk_top
         self.wid_parent = parent
         self.timer_id = None
         self.wid_message = None
         self.msg_type = None
         self.fade_val = 0.0
 
 
     def show_message(self, msg_type, msg_txt):
+        """
+        Displays the status overlay widget with the given text within the main
+        window. The text fades to black after a few seconds and is destroyed
+        once invisible.
+        """
+
         self.msg_type = msg_type
         self.fade_val = 0.0
         color = self.__get_color()
 
         if not tk_utils.wid_exists(self.wid_message):
             self.wid_message = tk.Label(self.wid_parent, text=msg_txt, foreground=color,
                                         anchor=tk.W, font=tk_utils.font_normal)
@@ -62,53 +78,63 @@
 
             self.wid_message.bind("<Motion>", lambda e: self.__handle_motion())
 
         else:
             self.wid_message.configure(text=msg_txt, foreground=color)
 
         if self.timer_id:
-            self.tk.after_cancel(self.timer_id)
-        self.timer_id = self.tk.after(5000, self.__handle_timer)
+            self.tk_top.after_cancel(self.timer_id)
+        self.timer_id = self.tk_top.after(5000, self.__handle_timer)
 
 
     def __get_color(self):
+        """
+        Calculate and return RGB color code for the text, considering the
+        initial color that depends on the status message type and the status of
+        fading.
+        """
         if self.msg_type == "error":
             color = (0xff, 0, 0)
         elif self.msg_type == "warning":
             color = (0xff, 0xc0, 0)
         else:
             color = (0xff, 0xff, 0xff)
 
         factor = (1.0 - self.fade_val)
         color = [int(x * factor) for x in color]
 
         return "#%02X%02X%02X" % (color[0], color[1], color[2])
 
 
     def __handle_motion(self):
+        """ Callback for mouse motion on the text: Stops and reverts fade-out.
+        """
         self.msg_type = "motion"
         self.fade_val = 0
         self.wid_message.configure(foreground=self.__get_color())
 
         if self.timer_id:
-            self.tk.after_cancel(self.timer_id)
-        self.timer_id = self.tk.after(5000, self.__handle_timer)
+            self.tk_top.after_cancel(self.timer_id)
+        self.timer_id = self.tk_top.after(5000, self.__handle_timer)
 
 
     def __handle_timer(self):
+        """ Timer handler used for fading out and finally destroying the text.
+        """
         self.fade_val += 0.015
         if self.fade_val < 1:
             self.wid_message.config(foreground=self.__get_color())
-            self.timer_id = self.tk.after(50, self.__handle_timer)
+            self.timer_id = self.tk_top.after(50, self.__handle_timer)
 
         else:
             self.timer_id = None
-            self.clear()
+            self.clear_message()
 
 
-    def clear(self):
+    def clear_message(self):
+        """ Clears the status message by destroying the overlay widget. """
         if self.timer_id:
-            self.tk.after_cancel(self.timer_id)
+            self.tk_top.after_cancel(self.timer_id)
             self.timer_id = None
 
         tk_utils.safe_destroy(self.wid_message)
         self.wid_message = None
```

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/wid_test_ctrl.py` & `mote-gtest-gui-0.9.0/gtest_gui/wid_test_ctrl.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,106 +13,131 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
+"""
+This module implements the test control widget class.
+"""
+
 from datetime import datetime
 import os
 import re
-import sys
 import time
+import sys
 
 import tkinter as tk
 from tkinter import messagebox as tk_messagebox
 
+from gtest_gui.dlg_config import ConfigDialog
+from gtest_gui.wid_status_line import StatusLineWidget
 import gtest_gui.config_db as config_db
-import gtest_gui.dlg_config as dlg_config
 import gtest_gui.filter_expr as filter_expr
-import gtest_gui.gtest as gtest
+import gtest_gui.gtest_ctrl as gtest_ctrl
+import gtest_gui.gtest_list_tests as gtest_list_tests
 import gtest_gui.test_db as test_db
+import gtest_gui.trace_db as trace_db
 import gtest_gui.tk_utils as tk_utils
-import gtest_gui.wid_status_line as wid_status_line
 import gtest_gui.wid_tool_tip as wid_tool_tip
 
 
-class Test_control_widget(object):
+class TestControlWidget:
+    """
+    This class implements the upper half of the main window, containing
+    options, control buttons and status display for test campaigns.
+    """
+
     def __init__(self, tk_top, parent):
-        self.tk = tk_top
+        """ Constructs an instance of the TestControlWidget within the given parent widget. """
+        self.tk_top = tk_top
 
         self.var_men_chkb = {}
         self.wid_men_cascades = []
         self.wid_men = None
         self.prev_campaign_options = None
         self.prev_exec_status = None
+        self.wid_test_log = None  # set later due to circular dependency
 
         self.filter_undo_history = []
         self.filter_redo_history = []
         self.filter_undo_lock = False
         self.filter_expr_error = []
+        # further attributes added by sub-functions: child widgets
 
         self.__create_widgets(parent)
 
-        test_db.Test_db_slots.campaign_stats_update = self.__update_campaign_status
+        test_db.register_slot(test_db.SlotTypes.campaign_stats_update,
+                              self.__update_campaign_status)
         self.slot_filter_change = None
 
 
     def get_widget(self):
+        """ Returns the root widget used by this instance. """
         return self.wid_top
 
 
     def set_wid_test_log(self, test_log):
+        """
+        Links the widget with the test result log widget. This link is
+        currently only used for updating repetition status. The link cannot be
+        set in the constructor due to circular dependency.
+        """
         self.wid_test_log = test_log
 
 
     def __create_widgets(self, parent):
         # dark theme
-        app_name = self.tk.cget("class")
-        self.tk.eval("option add %s.test_ctrl.*background {#000000}" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*foreground {#FFFFFF}" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*highlightBackground {#000000}" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*highlightColor {#FFE848}" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*Entry*background {#FFFFFF}" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*Entry*foreground {#000000}" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*Spinbox*background {#FFFFFF}" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*Spinbox*foreground {#000000}" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*Checkbutton*selectColor {#783060}" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*Checkbutton*activeBackground {#303030}" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*Checkbutton*activeForeground {#FFFFFF}" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*Checkbutton*cursor top_left_arrow" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*Button*activeBackground {#D0E028}" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*Button*activeForeground {#202020}" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*Button*background {#A0E028}" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*Button*foreground {#000000}" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*Button*highlightthickness 2" % app_name)
-        self.tk.eval("option add %s.test_ctrl.*Button*cursor top_left_arrow" % app_name)
-
-        self.var_opt_filter = tk.StringVar(self.tk, "")
-        self.var_opt_repetitions = tk.IntVar(self.tk, 1)
-        self.var_opt_job_count = tk.IntVar(self.tk, 1)
-        self.var_opt_job_runall = tk.IntVar(self.tk, 0)
-        self.var_opt_valgrind = tk.IntVar(self.tk, 0)
-        self.var_opt_fail_max = tk.IntVar(self.tk, 0)
-        self.var_opt_clean_trace = tk.BooleanVar(self.tk, False)
-        self.var_opt_clean_core = tk.BooleanVar(self.tk, False)
-        self.var_opt_shuffle = tk.BooleanVar(self.tk, False)
-        self.var_opt_run_disabled = tk.BooleanVar(self.tk, False)
-        self.var_opt_break_on_fail = tk.BooleanVar(self.tk, False)
-        self.var_opt_break_on_except = tk.BooleanVar(self.tk, False)
+        app_name = self.tk_top.cget("class")
+        for opt in ("background {#000000}",
+                    "foreground {#FFFFFF}",
+                    "highlightBackground {#000000}",
+                    "highlightColor {#FFE848}",
+                    "Entry*background {#FFFFFF}",
+                    "Entry*foreground {#000000}",
+                    "Spinbox*background {#FFFFFF}",
+                    "Spinbox*foreground {#000000}",
+                    "Checkbutton*selectColor {#783060}",
+                    "Checkbutton*activeBackground {#303030}",
+                    "Checkbutton*activeForeground {#FFFFFF}",
+                    "Checkbutton*cursor top_left_arrow",
+                    "Button*activeBackground {#D0E028}",
+                    "Button*activeForeground {#202020}",
+                    "Button*background {#A0E028}",
+                    "Button*foreground {#000000}",
+                    "Button*highlightthickness 2",
+                    "Button*cursor top_left_arrow"):
+            self.tk_top.eval("option add %s.test_ctrl.*%s" % (app_name, opt))
+
+        self.var_opt_filter = tk.StringVar(self.tk_top, "")
+        self.var_opt_repetitions = tk.IntVar(self.tk_top, 1)
+        self.var_opt_job_count = tk.IntVar(self.tk_top, 1)
+        self.var_opt_job_runall = tk.IntVar(self.tk_top, 0)
+        self.var_opt_valgrind = tk.IntVar(self.tk_top, 0)
+        self.var_opt_fail_max = tk.IntVar(self.tk_top, 0)
+        self.var_opt_clean_trace = tk.BooleanVar(self.tk_top, False)
+        self.var_opt_clean_core = tk.BooleanVar(self.tk_top, False)
+        self.var_opt_shuffle = tk.BooleanVar(self.tk_top, False)
+        self.var_opt_run_disabled = tk.BooleanVar(self.tk_top, False)
+        self.var_opt_break_on_fail = tk.BooleanVar(self.tk_top, False)
+        self.var_opt_break_on_except = tk.BooleanVar(self.tk_top, False)
 
         self.wid_top = tk.Frame(parent, name="test_ctrl") # name needed for "option add"
+        self.state_dep_wids = []
 
         wid_frm_opt = tk.Frame(self.wid_top)
         wid_frm_opt.columnconfigure(1, weight=0)
         wid_frm_opt.columnconfigure(2, weight=1)
         wid_frm_opt.columnconfigure(3, weight=0)
         wid_frm_opt.columnconfigure(4, weight=1)
 
-        self.__create_filter_entry_widget(wid_frm_opt, 1, 1, 1 + 4 + 2) # spans spinbox & option columns
+        self.wid_tc_filter = \
+            self.__create_filter_entry_widget(wid_frm_opt, 1, 1,
+                                              1 + 4 + 2) # span spinbox & option cols
         self.__create_spinbox_widgets(wid_frm_opt, 2, 1) # occupies 4 columns
         self.__create_option_widgets(wid_frm_opt, 2, 1 + 4) # occupies 2 columns
         wid_frm_opt.pack(side=tk.TOP, fill=tk.X, expand=1)
 
         wid_frm_cmd = tk.Frame(self.wid_top)
         self.__create_status_widget(wid_frm_cmd, 1, 1)
         self.__create_progress_widget(wid_frm_cmd, 1, 2)
@@ -128,165 +153,180 @@
 
 
     def __create_filter_entry_widget(self, parent, grid_row, grid_col, grid_col_span):
         wid_lab = tk.Label(parent, text="Test filter:")
         wid_lab.grid(row=grid_row, column=grid_col, sticky="e", padx=10)
         wid_tool_tip.tool_tip_add(wid_lab, 'test_ctrl.tc_filter')
 
-        validate_filter_cmd = self.tk.register(self.__validate_tc_filter)
+        validate_filter_cmd = self.tk_top.register(self.__validate_tc_filter)
         wid_frm = tk.Frame(parent, relief=tk.SUNKEN, borderwidth=2)
         wid_ent = tk.Entry(wid_frm, width=40, relief=tk.FLAT, borderwidth=0,
                            textvariable=self.var_opt_filter,
                            validate="key", validatecommand=(validate_filter_cmd, "%d", "%s", "%P"))
         wid_ent.pack(side=tk.LEFT, fill=tk.BOTH, expand=1)
 
         wid_but = tk.Button(wid_frm, image="img_drop_down", takefocus=0, borderwidth=1,
                             relief=tk.RAISED, highlightthickness=1,
                             command=self.__popup_test_case_menu)
         wid_but.pack(side=tk.LEFT, fill=tk.Y)
         wid_frm.grid(row=grid_row, column=grid_col+1, columnspan=grid_col_span,
                      sticky="we", padx=10, pady=10)
 
-        wid_ent.bind("<Control-Key-z>", lambda e: tk_utils.bind_call_and_break(self.__undo_tc_filter_edit))
-        wid_ent.bind("<Control-Key-y>", lambda e: tk_utils.bind_call_and_break(self.__redo_tc_filter_edit))
-        wid_ent.bind("<Control-Shift-Key-z>", lambda e: tk_utils.bind_call_and_break(self.__redo_tc_filter_edit))
+        wid_ent.bind("<Control-Key-z>",
+                     lambda e: tk_utils.bind_call_and_break(self.__undo_tc_filter_edit))
+        wid_ent.bind("<Control-Key-y>",
+                     lambda e: tk_utils.bind_call_and_break(self.__redo_tc_filter_edit))
+        wid_ent.bind("<Control-Shift-Key-z>",
+                     lambda e: tk_utils.bind_call_and_break(self.__redo_tc_filter_edit))
         wid_ent.bind("<Return>", lambda e: self.check_filter_expression())
         wid_ent.bind("<Key-Down>", lambda e: self.__popup_test_case_menu())
 
-        self.wid_tc_filter = wid_ent
-        self.wid_filter_men_but = wid_but
+        return wid_ent
 
 
     def __create_spinbox_widgets(self, parent, grid_row, grid_col):
-        validate_int_cmd = self.tk.register(self.__validate_int)
+        validate_int_cmd = self.tk_top.register(TestControlWidget.__validate_int)
 
         wid_lab = tk.Label(parent, text="Repetitions:")
         wid_lab.grid(row=grid_row, column=grid_col+0, sticky="e", padx=10)
         wid_tool_tip.tool_tip_add(wid_lab, 'test_ctrl.repetitions')
-        self.wid_run_count = tk.Spinbox(
-                    parent, from_=1, to=99999, increment=1, width=6,
-                    textvariable=self.var_opt_repetitions,
-                    validate="key", validatecommand=(validate_int_cmd, "%P"))
-        self.wid_run_count.grid(row=grid_row, column=grid_col+1, sticky="w", padx=10)
+        wid_run_count = tk.Spinbox(
+            parent, from_=1, to=99999, increment=1, width=6,
+            textvariable=self.var_opt_repetitions,
+            validate="key", validatecommand=(validate_int_cmd, "%P"))
+        wid_run_count.grid(row=grid_row, column=grid_col+1, sticky="w", padx=10)
 
         wid_lab = tk.Label(parent, text="CPUs:")
         wid_lab.grid(row=grid_row, column=grid_col+2, sticky="e", padx=10)
         wid_tool_tip.tool_tip_add(wid_lab, 'test_ctrl.job_count')
-        self.wid_job_count = tk.Spinbox(
-                    parent, from_=1, to=1024, increment=1, width=6,
-                    textvariable=self.var_opt_job_count,
-                    validate="key", validatecommand=(validate_int_cmd, "%P"))
-        self.wid_job_count.grid(row=grid_row, column=grid_col+3, sticky="w", padx=10)
+        wid_job_count = tk.Spinbox(
+            parent, from_=1, to=1024, increment=1, width=6,
+            textvariable=self.var_opt_job_count,
+            validate="key", validatecommand=(validate_int_cmd, "%P"))
+        wid_job_count.grid(row=grid_row, column=grid_col+3, sticky="w", padx=10)
         grid_row += 1
 
         wid_lab = tk.Label(parent, text="Fail limit:")
         wid_lab.grid(row=grid_row, column=grid_col+0, sticky="e", padx=10)
         wid_tool_tip.tool_tip_add(wid_lab, 'test_ctrl.max_fail')
-        self.wid_fail_limit = tk.Spinbox(
-                    parent, from_=0, to=99999, increment=1, width=6,
-                    textvariable=self.var_opt_fail_max,
-                    validate="key", validatecommand=(validate_int_cmd, "%P"))
-        self.wid_fail_limit.grid(row=grid_row, column=grid_col+1, sticky="w", padx=10)
+        wid_fail_limit = tk.Spinbox(
+            parent, from_=0, to=99999, increment=1, width=6,
+            textvariable=self.var_opt_fail_max,
+            validate="key", validatecommand=(validate_int_cmd, "%P"))
+        wid_fail_limit.grid(row=grid_row, column=grid_col+1, sticky="w", padx=10)
 
         wid_lab = tk.Label(parent, text="Ignore filter:")
         wid_lab.grid(row=grid_row, column=grid_col+2, sticky="e", padx=10)
         wid_tool_tip.tool_tip_add(wid_lab, 'test_ctrl.job_runall')
-        self.wid_job_runall = tk.Spinbox(
-                    parent, from_=0, to=1024, increment=1, width=6,
-                    textvariable=self.var_opt_job_runall,
-                    validate="key", validatecommand=(validate_int_cmd, "%P"))
-        self.wid_job_runall.grid(row=grid_row, column=grid_col+3, sticky="w", padx=10)
+        wid_job_runall = tk.Spinbox(
+            parent, from_=0, to=1024, increment=1, width=6,
+            textvariable=self.var_opt_job_runall,
+            validate="key", validatecommand=(validate_int_cmd, "%P"))
+        wid_job_runall.grid(row=grid_row, column=grid_col+3, sticky="w", padx=10)
+
+        # widgets that need to be disabled during running test campaign
+        self.state_dep_wids.extend([wid_run_count, wid_job_count, wid_fail_limit, wid_job_runall])
 
 
     def __create_option_widgets(self, parent, grid_row, grid_col):
         wid_lab = tk.Label(parent, text="Options:")
         wid_lab.grid(row=grid_row, column=grid_col, sticky="e", padx=10)
 
         wid_frm = tk.Frame(parent)
-        self.wid_opt_clean_trace = tk.Checkbutton(
-                    wid_frm, text="Clean traces of passed tests",
-                    variable=self.var_opt_clean_trace, command=self.__handle_option_change)
-        self.wid_opt_clean_trace.pack(side=tk.LEFT)
-        wid_tool_tip.tool_tip_add(self.wid_opt_clean_trace, 'test_ctrl.clean_trace')
-
-        self.wid_opt_clean_core = tk.Checkbutton(
-                    wid_frm, text="Clean core files", variable=self.var_opt_clean_core,
-                    command=lambda: self.__handle_option_change())
-        self.wid_opt_clean_core.pack(side=tk.LEFT)
+        wid_opt_clean_trace = tk.Checkbutton(
+            wid_frm, text="Clean traces of passed tests",
+            variable=self.var_opt_clean_trace, command=self.__handle_option_change)
+        if sys.platform != "win32":
+            wid_opt_clean_trace.pack(side=tk.LEFT)
+        wid_tool_tip.tool_tip_add(wid_opt_clean_trace, 'test_ctrl.clean_trace')
+
+        wid_opt_clean_core = tk.Checkbutton(
+            wid_frm, text="Clean core files", variable=self.var_opt_clean_core,
+            command=self.__handle_option_change)
+        wid_opt_clean_core.pack(side=tk.LEFT)
         wid_frm.grid(row=grid_row, column=grid_col+1, sticky="w", padx=10)
-        wid_tool_tip.tool_tip_add(self.wid_opt_clean_core, 'test_ctrl.clean_core')
+        wid_tool_tip.tool_tip_add(wid_opt_clean_core, 'test_ctrl.clean_core')
         grid_row += 1
 
         wid_frm = tk.Frame(parent)
-        self.wid_opt_shuffle = tk.Checkbutton(
-                    wid_frm, text="Shuffle execution order", variable=self.var_opt_shuffle)
-        self.wid_opt_shuffle.pack(side=tk.LEFT)
-        wid_tool_tip.tool_tip_add(self.wid_opt_shuffle, 'test_ctrl.shuffle')
-
-        self.wid_opt_run_disabled = tk.Checkbutton(
-                    wid_frm, text="Run disabled tests", variable=self.var_opt_run_disabled,
-                    command=self.__handle_run_disabled_change)
-        self.wid_opt_run_disabled.pack(side=tk.LEFT, padx=10)
+        wid_opt_shuffle = tk.Checkbutton(
+            wid_frm, text="Shuffle execution order", variable=self.var_opt_shuffle)
+        wid_opt_shuffle.pack(side=tk.LEFT)
+        wid_tool_tip.tool_tip_add(wid_opt_shuffle, 'test_ctrl.shuffle')
+
+        wid_opt_run_disabled = tk.Checkbutton(
+            wid_frm, text="Run disabled tests", variable=self.var_opt_run_disabled,
+            command=self.__handle_run_disabled_change)
+        wid_opt_run_disabled.pack(side=tk.LEFT, padx=10)
         wid_frm.grid(row=grid_row, column=grid_col+1, sticky="w", padx=10)
-        wid_tool_tip.tool_tip_add(self.wid_opt_run_disabled, 'test_ctrl.run_disabled')
+        wid_tool_tip.tool_tip_add(wid_opt_run_disabled, 'test_ctrl.run_disabled')
         grid_row += 1
 
         wid_frm = tk.Frame(parent)
-        self.wid_opt_break_on_fail = tk.Checkbutton(
-                    wid_frm, text="Break on failure", variable=self.var_opt_break_on_fail)
-        self.wid_opt_break_on_fail.pack(side=tk.LEFT)
-        wid_tool_tip.tool_tip_add(self.wid_opt_break_on_fail, 'test_ctrl.break_on_fail')
-
-        self.wid_opt_break_on_except = tk.Checkbutton(
-                    wid_frm, text="Break on exception", variable=self.var_opt_break_on_except)
-        self.wid_opt_break_on_except.pack(side=tk.LEFT, padx=10)
+        wid_opt_break_on_fail = tk.Checkbutton(
+            wid_frm, text="Break on failure", variable=self.var_opt_break_on_fail)
+        wid_opt_break_on_fail.pack(side=tk.LEFT)
+        wid_tool_tip.tool_tip_add(wid_opt_break_on_fail, 'test_ctrl.break_on_fail')
+
+        wid_opt_break_on_except = tk.Checkbutton(
+            wid_frm, text="Break on exception", variable=self.var_opt_break_on_except)
+        wid_opt_break_on_except.pack(side=tk.LEFT, padx=10)
         wid_frm.grid(row=grid_row, column=grid_col+1, sticky="w", padx=10)
-        wid_tool_tip.tool_tip_add(self.wid_opt_break_on_except, 'test_ctrl.break_on_except')
+        wid_tool_tip.tool_tip_add(wid_opt_break_on_except, 'test_ctrl.break_on_except')
         grid_row += 1
 
         wid_frm = tk.Frame(parent)
-        self.wid_opt_valgrind1 = tk.Checkbutton(
-                    wid_frm, text="Valgrind",
-                    variable=self.var_opt_valgrind, offvalue=0, onvalue=1)
-        self.wid_opt_valgrind1.pack(side=tk.LEFT)
-        wid_tool_tip.tool_tip_add(self.wid_opt_valgrind1, 'test_ctrl.valgrind1')
-
-        self.wid_opt_valgrind2 = tk.Checkbutton(
-                    wid_frm, text="Valgrind - 2nd option set",
-                    variable=self.var_opt_valgrind, offvalue=0, onvalue=2)
-        self.wid_opt_valgrind2.pack(side=tk.LEFT)
-        wid_frm.grid(row=grid_row, column=grid_col+1, sticky="w", padx=10)
-        wid_tool_tip.tool_tip_add(self.wid_opt_valgrind2, 'test_ctrl.valgrind2')
+        wid_opt_valgrind1 = tk.Checkbutton(
+            wid_frm, text="Valgrind",
+            variable=self.var_opt_valgrind, offvalue=0, onvalue=1)
+        wid_opt_valgrind1.pack(side=tk.LEFT)
+        wid_tool_tip.tool_tip_add(wid_opt_valgrind1, 'test_ctrl.valgrind1')
+
+        wid_opt_valgrind2 = tk.Checkbutton(
+            wid_frm, text="Valgrind - 2nd option set",
+            variable=self.var_opt_valgrind, offvalue=0, onvalue=2)
+        wid_opt_valgrind2.pack(side=tk.LEFT)
+        if sys.platform != "win32":
+            wid_frm.grid(row=grid_row, column=grid_col+1, sticky="w", padx=10)
+        wid_tool_tip.tool_tip_add(wid_opt_valgrind2, 'test_ctrl.valgrind2')
         grid_row += 1
 
+        # widgets that need to be disabled during running test campaign
+        self.state_dep_wids.extend([wid_opt_shuffle, wid_opt_run_disabled, wid_opt_break_on_fail,
+                                    wid_opt_break_on_except, wid_opt_valgrind1, wid_opt_valgrind2])
+
 
     def __create_control_buttons(self, parent, grid_row, grid_col):
+        # This method is only called within __init__
+        # pylint: disable=attribute-defined-outside-init
         width = max([tk_utils.font_normal.measure(x)
-                            for x in ("Run", "Stop", "Resume", "Repeat")]) + 20
+                     for x in ("Run", "Stop", "Resume", "Repeat")]) + 20
         wid_frm = tk.Frame(parent)
         self.wid_cmd_run = tk.Button(
-                    wid_frm, image="img_run", text="Run", compound=tk.LEFT, width=width,
-                    command=self.start_campaign)
+            wid_frm, image="img_run", text="Run", compound=tk.LEFT, width=width,
+            command=self.start_campaign)
         self.wid_cmd_stop = tk.Button(
-                    wid_frm, image="img_stop", text="Stop", compound=tk.LEFT, width=width,
-                    command=self.stop_campaign)
+            wid_frm, image="img_stop", text="Stop", compound=tk.LEFT, width=width,
+            command=self.stop_campaign)
         self.wid_cmd_resume = tk.Button(
-                    wid_frm, image="img_resume", text="Resume", compound=tk.LEFT, width=width,
-                    command=self.resume_campaign)
+            wid_frm, image="img_resume", text="Resume", compound=tk.LEFT, width=width,
+            command=self.resume_campaign)
         self.wid_cmd_repeat = tk.Button(
-                    wid_frm, image="img_repeat", text="Repeat", compound=tk.LEFT, width=width,
-                    command=self.start_repetition)
+            wid_frm, image="img_repeat", text="Repeat", compound=tk.LEFT, width=width,
+            command=self.start_repetition)
         self.wid_cmd_run.pack(side=tk.LEFT, padx=5)
         self.wid_cmd_stop.pack(side=tk.LEFT, padx=5)
         self.wid_cmd_resume.pack(side=tk.LEFT, padx=5)
         self.wid_cmd_repeat.pack(side=tk.LEFT, padx=5)
         wid_frm.grid(row=grid_row, column=grid_col)
 
 
     def __create_status_widget(self, parent, grid_row, grid_col):
+        # This method is only called within __init__
+        # pylint: disable=attribute-defined-outside-init
         wid_frm = tk.LabelFrame(parent, text="Status", borderwidth=2, relief=tk.GROOVE)
 
         wid_lab = tk.Label(wid_frm, text="Running:")
         wid_lab.grid(row=1, column=0, sticky="w", padx=2)
         self.wid_stats_exec_cnt = tk.Label(wid_frm, text="0")
         self.wid_stats_exec_cnt.grid(row=1, column=1, sticky="e", padx=2)
 
@@ -298,54 +338,78 @@
         wid_lab = tk.Label(wid_frm, text="Failed:")
         wid_lab.grid(row=3, column=0, sticky="w", padx=2)
         self.wid_stats_fail_cnt = tk.Label(wid_frm, text="0")
         self.wid_stats_fail_cnt.grid(row=3, column=1, sticky="e", padx=2)
 
         wid_noshrink = tk.Frame(wid_frm)
         wid_noshrink.grid(row=4, column=1, sticky="we")
-        wid_noshrink.bind("<Configure>", lambda e: self.__status_widget_resized(e.widget, e.width))
+        wid_noshrink.bind("<Configure>", lambda e:
+                          TestControlWidget.__status_widget_resized(e.widget, e.width))
         wid_frm.grid(row=grid_row, column=grid_col, sticky="ns", padx=5)
 
 
     def __create_progress_widget(self, parent, grid_row, grid_col):
+        # This method is only called within __init__
+        # pylint: disable=attribute-defined-outside-init
         wid_frm = tk.LabelFrame(parent, text="Progress", borderwidth=2, relief=tk.GROOVE)
         self.wid_progress_frm = tk.Frame(wid_frm)
         self.wid_progress_bar = tk.Frame(self.wid_progress_frm, width=20,
                                          background="#6868FF", borderwidth=1, relief=tk.RAISED)
         self.wid_progress_frm.pack(side=tk.TOP, fill=tk.Y, expand=1)
         wid_tool_tip.tool_tip_add(wid_frm, self.__get_progress_tool_tip)
         wid_frm.grid(row=grid_row, column=grid_col, sticky="ns")
 
 
     def __get_progress_tool_tip(self, xcoo, ycoo):
+        # abstract interface: unused parameter needed by other classes
+        # pylint: disable=unused-argument
         totals = test_db.campaign_stats
-        if totals[4]:
-            filter_str = self.prev_campaign_options["filter_str"]
-            expr = filter_expr.Filter_expr(filter_str, self.prev_campaign_options["run_disabled"])
-            tc_list = expr.get_selected_tests()
-            tc_exec = [test_db.test_case_stats[x][0] +
-                       test_db.test_case_stats[x][1] +
-                       test_db.test_case_stats[x][2] for x in tc_list]
-            min_cnt = min(tc_exec)
-            max_cnt = max(tc_exec)
-            rep_cnt = int(self.var_opt_repetitions.get())
+        if not totals[4]:
+            return ""
 
-            if len(tc_list) > 1 and (rep_cnt > 1):
-                if max_cnt < min_cnt + 2:
-                    return ("%d of %d test case runs\n%d of %d repetitions" %
-                            (totals[5], totals[4], min_cnt, rep_cnt))
-                else:
-                    return ("%d of %d test case runs\n%d..%d of %d repetitions" %
-                            (totals[5], totals[4], min_cnt, max_cnt, rep_cnt))
-            elif rep_cnt > 1:
-                return "%d of %d repetitions" % (min_cnt, rep_cnt)
+        filter_str = self.prev_campaign_options["filter_str"]
+        expr = filter_expr.FilterExpr(filter_str, self.prev_campaign_options["run_disabled"])
+        tc_list = expr.get_selected_tests()
+        tc_exec = [test_db.test_case_stats[x][0] +
+                   test_db.test_case_stats[x][1] +
+                   test_db.test_case_stats[x][2] for x in tc_list]
+        min_cnt = min(tc_exec)
+        max_cnt = max(tc_exec)
+        rep_cnt = int(self.var_opt_repetitions.get())
+
+        if len(tc_list) > 1 and (rep_cnt > 1):
+            if max_cnt < min_cnt + 2:
+                txt = ("%d of %d test case runs\n%d of %d repetitions" %
+                       (totals[5], totals[4], min_cnt, rep_cnt))
             else:
-                return "%d of %d test case runs" % (totals[5], totals[4])
+                txt = ("%d of %d test case runs\n%d..%d of %d repetitions" %
+                       (totals[5], totals[4], min_cnt, max_cnt, rep_cnt))
+        elif rep_cnt > 1:
+            txt = "%d of %d repetitions" % (min_cnt, rep_cnt)
         else:
-            return ""
+            txt = "%d of %d test case runs" % (totals[5], totals[4])
+
+        # get stats, but ignore background jobs
+        job_stats = [x for x in gtest_ctrl.gtest_ctrl.get_job_stats() if not x[2]]
+        if job_stats:
+            min_job_done = min([x[4] / x[5] if x[5] else 100 for x in job_stats])
+            if min_job_done:
+                time_delta = time.time() - totals[7]
+                time_remain = time_delta / min_job_done - time_delta
+
+                if time_remain < 2*60:
+                    txt += "\n%d seconds remaining" % time_remain
+                elif time_remain < 90*60:
+                    txt += "\n%.1f minutes remaining" % (time_remain / 60)
+                elif time_remain < 24*60*60:
+                    txt += "\n%.1f hours remaining" % (time_remain / (60*60))
+                else:
+                    txt += "\n%.1f days remaining" % (time_remain / (24*60*60))
+
+        return txt
 
 
     def __update_campaign_status(self):
         # Update counters in status frame
         totals = test_db.campaign_stats
         self.wid_stats_pass_cnt.configure(text="%d" % totals[0])
         self.wid_stats_fail_cnt.configure(text="%d" % (totals[1] + totals[6]))
@@ -371,65 +435,56 @@
         if self.prev_exec_status != tests_active:
             if tests_active:
                 self.wid_stats_pass_cnt.configure(foreground="#18FF18", font=tk_utils.font_bold)
                 self.wid_stats_fail_cnt.configure(foreground="#FF1818", font=tk_utils.font_bold)
 
                 self.wid_cmd_run.configure(cursor="top_left_arrow")
                 self.wid_cmd_stop.configure(state=tk.NORMAL)
-                cmd_state = state=tk.DISABLED
+                cmd_state = tk.DISABLED
 
             else:
                 self.wid_stats_pass_cnt.configure(foreground="#FFFFFF", font=tk_utils.font_normal)
                 self.wid_stats_fail_cnt.configure(foreground="#FFFFFF", font=tk_utils.font_normal)
 
                 self.wid_cmd_stop.configure(state=tk.DISABLED, cursor="top_left_arrow")
-                cmd_state = state=tk.NORMAL
+                cmd_state = tk.NORMAL
 
-            for wid in (self.wid_cmd_run,
+            for wid in [self.wid_cmd_run,
                         self.wid_cmd_repeat,
-                        self.wid_tc_filter,
-                        self.wid_filter_men_but,
-                        self.wid_run_count,
-                        self.wid_fail_limit,
-                        self.wid_job_count,
-                        self.wid_job_runall,
-                        self.wid_opt_shuffle,
-                        self.wid_opt_run_disabled,
-                        self.wid_opt_break_on_fail,
-                        self.wid_opt_break_on_except,
-                        self.wid_opt_valgrind1,
-                        self.wid_opt_valgrind2):
+                        self.wid_tc_filter] + self.state_dep_wids:
                 wid.configure(state=cmd_state)
 
             if tests_active or (self.prev_campaign_options is None):
-                cmd_state = state=tk.DISABLED
+                cmd_state = tk.DISABLED
             else:
-                cmd_state = state=tk.NORMAL
+                cmd_state = tk.NORMAL
             self.wid_cmd_resume.configure(state=cmd_state)
 
         self.prev_exec_status = tests_active
 
 
-    def __status_widget_resized(self, wid, new_width):
+    @staticmethod
+    def __status_widget_resized(wid, new_width):
         cur_width = wid.cget("width")
         if new_width > cur_width:
             wid.configure(width=new_width)
 
 
-    def __validate_int(self, val):
+    @staticmethod
+    def __validate_int(val):
         return bool(re.match(r"^\d*$", val))
 
 
     def __validate_tc_filter(self, kind, old_val, new_val):
         self.filter_expr_error.clear()
         if (new_val != old_val) and not self.filter_undo_lock:
             kind = int(kind)
-            if (  (not self.filter_undo_history) or
-                  (kind == -1) or
-                  (kind != self.filter_undo_history[-1][1])):
+            if ((not self.filter_undo_history) or
+                    (kind == -1) or
+                    (kind != self.filter_undo_history[-1][1])):
                 self.filter_undo_history.append((old_val, kind))
             # else: combine with last item on undo stack
 
             self.filter_redo_history = []
         return True
 
 
@@ -454,22 +509,22 @@
 
 
     def __popup_test_case_menu(self):
         if not self.check_filter_expression():
             return
 
         if self.var_opt_filter.get():
-            expr = filter_expr.Filter_expr(self.var_opt_filter.get(),
-                                           self.var_opt_run_disabled.get())
+            expr = filter_expr.FilterExpr(self.var_opt_filter.get(),
+                                          self.var_opt_run_disabled.get())
             matches = expr.get_selected_tests()
         else:
             matches = []
 
         if not tk_utils.wid_exists(self.wid_men):
-            self.wid_men = tk.Menu(self.tk, tearoff=0)
+            self.wid_men = tk.Menu(self.tk_top, tearoff=0)
         else:
             self.wid_men.delete(0, "end")
 
         all_tc_names = filter_expr.get_test_list(self.var_opt_run_disabled.get())
         if all_tc_names:
             idx = 0
             for tc_suite in filter_expr.get_test_suite_names(all_tc_names):
@@ -486,76 +541,97 @@
                     if tc_name in matches:
                         all_disabled = False
                     else:
                         all_enabled = False
 
                 if not all_enabled:
                     self.wid_men_cascades[idx].add_command(
-                            label="Enable all",
-                            command=lambda x=tc_names: self.select_tcs(x, True)) # pass copy to lambda
+                        label="Enable all",
+                        command=lambda x=tc_names: self.select_tcs(x, True)) # pass copy to lambda
                 if not all_disabled or not matches:
                     self.wid_men_cascades[idx].add_command(
-                            label="Disable all",
-                            command=lambda x=tc_names: self.select_tcs(x, False)) # pass copy to lambda
+                        label="Disable all",
+                        command=lambda x=tc_names: self.select_tcs(x, False)) # pass copy to lambda
                 self.wid_men_cascades[idx].add_separator()
 
                 # entries for each test case
                 for tc_name in tc_names:
                     if self.var_men_chkb.get(tc_name) is None:
-                        self.var_men_chkb[tc_name] = tk.BooleanVar(self.tk, False)
+                        self.var_men_chkb[tc_name] = tk.BooleanVar(self.tk_top, False)
                     self.wid_men_cascades[idx].add_checkbutton(
-                            label=tc_name[len(tc_suite):],
-                            command=lambda x=tc_name: self.__toggle_tc(x), # pass copy to lambda
-                            variable=self.var_men_chkb[tc_name], onvalue=1, offvalue=0)
+                        label=tc_name[len(tc_suite):],
+                        command=lambda x=tc_name: self.__toggle_tc(x), # pass copy to lambda
+                        variable=self.var_men_chkb[tc_name], onvalue=1, offvalue=0)
                     self.var_men_chkb[tc_name].set(tc_name in matches)
                 idx += 1
         elif test_db.test_exe_name:
             self.wid_men.add_command(label="List of test cases is empty", state=tk.DISABLED)
         else:
             self.wid_men.add_command(label="Please set executable path via the Control menu",
                                      state=tk.DISABLED)
 
         wid = self.wid_tc_filter
-        self.tk.call("tk_popup", self.wid_men,
-                     wid.winfo_rootx(), wid.winfo_rooty() + wid.winfo_height(), 0)
+        self.tk_top.call("tk_popup", self.wid_men,
+                         wid.winfo_rootx(), wid.winfo_rooty() + wid.winfo_height(), 0)
 
 
     def __toggle_tc(self, tc_name):
-        expr = filter_expr.Filter_expr(self.var_opt_filter.get(), self.var_opt_run_disabled.get())
-        expr.select_test_cases([tc_name], self.var_men_chkb[tc_name].get())
-        self.var_opt_filter.set(expr.get_expr())
-        if self.slot_filter_change:
-            self.slot_filter_change(expr)
+        """ Add or remove a single given test case name from the test case filter expression. """
+        if not gtest_ctrl.gtest_ctrl.is_active():
+            expr = filter_expr.FilterExpr(self.var_opt_filter.get(),
+                                          self.var_opt_run_disabled.get())
+            expr.select_test_cases([tc_name], self.var_men_chkb[tc_name].get())
+            self.var_opt_filter.set(expr.get_expr())
+            if self.slot_filter_change:
+                self.slot_filter_change(expr)
+        else:
+            tk_messagebox.showerror(parent=self.tk_top,
+                                    message="Cannot modify filter during running campaign.")
 
 
     def select_tcs(self, tc_names, enable):
-        expr = filter_expr.Filter_expr(self.var_opt_filter.get(), self.var_opt_run_disabled.get())
-        expr.select_test_cases(tc_names, enable)
-        self.var_opt_filter.set(expr.get_expr())
-        if self.slot_filter_change:
-            self.slot_filter_change(expr)
+        """ Add or remove all given test case names from the test case filter expression. """
+        if not gtest_ctrl.gtest_ctrl.is_active():
+            expr = filter_expr.FilterExpr(self.var_opt_filter.get(),
+                                          self.var_opt_run_disabled.get())
+            expr.select_test_cases(tc_names, enable)
+            self.var_opt_filter.set(expr.get_expr())
+            if self.slot_filter_change:
+                self.slot_filter_change(expr)
+        else:
+            tk_messagebox.showerror(parent=self.tk_top,
+                                    message="Cannot modify filter during running campaign.")
 
 
     def get_test_filter_expr(self):
+        """
+        Create and return a test case filter expression object reflecting the
+        current content of the filter entry field.
+        """
         filter_str = self.var_opt_filter.get()
-        return filter_expr.Filter_expr(filter_str, self.var_opt_run_disabled.get())
+        return filter_expr.FilterExpr(filter_str, self.var_opt_run_disabled.get())
 
 
     def __handle_run_disabled_change(self):
-        expr = filter_expr.Filter_expr(self.var_opt_filter.get(), self.var_opt_run_disabled.get())
+        expr = filter_expr.FilterExpr(self.var_opt_filter.get(), self.var_opt_run_disabled.get())
         if self.slot_filter_change:
             self.slot_filter_change(expr)
 
 
     def register_filter_change_slot(self, func):
+        """
+        Register a callback that is invoked upon changes to the test case
+        filter expression. At most one other widget can register the callback.
+        """
         self.slot_filter_change = func
 
 
     def start_campaign(self):
-        if gtest.gtest_ctrl.is_active(): # block call via key binding
+        """ Start a test campaign with the current option values in the widget. """
+        if gtest_ctrl.gtest_ctrl.is_active(): # block call via key binding
             return
 
         if not self.__check_executable_update():
             return
 
         # check if given test case exists - needs to be done after exe update & reading new TC list
         if not self.check_filter_expression():
@@ -563,150 +639,164 @@
         if not self.__check_test_options():
             return
 
         self.__start_campaign_sub(self.var_opt_filter.get())
 
 
     def stop_campaign(self):
+        """ Stop the currently ongoing test campaign. """
         self.wid_cmd_stop.configure(cursor="watch")
-        gtest.gtest_ctrl.stop()
+        gtest_ctrl.gtest_ctrl.stop()
 
 
     def resume_campaign(self):
-        if gtest.gtest_ctrl.is_active(): # block call via key binding
+        """ Resume a previously stopped test campaign with current options. """
+        if gtest_ctrl.gtest_ctrl.is_active(): # block call via key binding
             return
 
         if self.prev_campaign_options is None:
-            wid_status_line.show_message("warn", "Campaign cannot be resumed.")
+            StatusLineWidget.get().show_message("warn", "Campaign cannot be resumed.")
             return
 
         if ((self.prev_campaign_options["filter_str"] != self.var_opt_filter.get()) or
-            (self.prev_campaign_options["run_disabled"] != self.var_opt_run_disabled.get())):
-            if not tk_messagebox.askokcancel(
-                    parent=self.tk,
-                    message="Test filter options have been changed. Really resume with previous filter?"):
+                (self.prev_campaign_options["run_disabled"] != self.var_opt_run_disabled.get())):
+            msg = "Test filter options have been changed. Really resume with previous filter?"
+            if not tk_messagebox.askokcancel(parent=self.tk_top, message=msg):
                 return
 
         if not os.access(test_db.test_exe_name, os.X_OK):
-            tk_messagebox.showerror(parent=self.tk,
-                                    message="Test executable inaccessible: " + str(e))
-            return False
+            msg = "Test executable does not exist or is inaccessible: " + test_db.test_exe_name
+            tk_messagebox.showerror(parent=self.tk_top, message=msg)
+            return
 
         if not self.__check_test_options():
             return
 
         remaining_rep_cnt = self.__calc_remaining_repetitions()
         if remaining_rep_cnt <= 0:
             tk_messagebox.showerror(
-                    parent=self.tk,
-                    message="Configured number of repetitions were already completed.")
+                parent=self.tk_top,
+                message="The configured number of repetitions was already completed.")
             return
 
         self.__start_campaign_sub(self.prev_campaign_options["filter_str"],
                                   resume_rep_cnt=remaining_rep_cnt)
 
 
     def start_repetition(self):
-        if gtest.gtest_ctrl.is_active(): # block call via key binding
+        """
+        Start a test campaign the only runs test cases marked for repetition.
+        If none were marked, all failed tests are marked automatically. A
+        warning is issued if the executable is still the same as in the
+        original run (because for many kinds of tests this will mean result
+        will be the same.)
+        """
+        if gtest_ctrl.gtest_ctrl.is_active(): # block call via key binding
             return
 
         # Mark selected tests for repetiton, if none marked yet
         if not self.wid_test_log.do_request_repetition(True):
             return
 
         tc_names = test_db.repeat_requests.keys()
 
         if not tc_names:
             tk_messagebox.showerror(
-                  parent=self.tk,
-                  message="Nothing to repeat: "
-                          "No results selected and no repetitions requested previously.")
+                parent=self.tk_top,
+                message="Nothing to repeat: "
+                        "No results selected and no repetitions requested previously.")
             return
 
         if not self.__check_executable_update():
             return
 
         current_exe_cnt = sum([test_db.repeat_requests[x] == test_db.test_exe_ts
-                                for x in tc_names])
+                               for x in tc_names])
         if current_exe_cnt:
             msg = ("Really repeat %d test%s with the same executable version?" %
-                        (current_exe_cnt, "s" if current_exe_cnt > 1 else ""))
-            if not tk_messagebox.askokcancel(parent=self.tk, message=msg):
+                   (current_exe_cnt, "s" if current_exe_cnt > 1 else ""))
+            if not tk_messagebox.askokcancel(parent=self.tk_top, message=msg):
                 return
 
-            for tc_name in test_db.repeat_requests.keys():
+            for tc_name in test_db.repeat_requests:
                 if test_db.repeat_requests[tc_name] == test_db.test_exe_ts:
                     test_db.repeat_requests[tc_name] -= 1
                     self.wid_test_log.update_repetition_status(tc_name)
 
         if not self.__check_test_options():
             return
 
         # create fake pattern that selects the test cases
         self.__start_campaign_sub(":".join(tc_names), is_repeat=True)
 
 
     def __check_executable_update(self):
         if not test_db.test_exe_name:
-            tk_messagebox.showerror(parent=self.tk,
+            tk_messagebox.showerror(parent=self.tk_top,
                                     message="Please select an executable via the Control menu")
             return False
 
         try:
-            latest_exe_ts = int(os.stat(test_db.test_exe_name).st_mtime)  # cast away sub-second fraction
-        except OSError as e:
-            tk_messagebox.showerror(parent=self.tk,
-                                    message="Test executable inaccessible: " + str(e))
+            latest_exe_ts = int(os.stat(test_db.test_exe_name).st_mtime)  # cast away fraction
+        except OSError as exc:
+            tk_messagebox.showerror(parent=self.tk_top,
+                                    message="Test executable inaccessible: " + str(exc))
             return False
 
         if test_db.test_exe_ts == latest_exe_ts:
             delta = time.time() - latest_exe_ts
             if delta < 2*60:
                 msg = ""
             elif delta < 90*60:
                 msg = "%d minutes ago" % (delta // 60)
             elif delta < 11*60*60:
                 msg = "%.1f hours ago" % (delta / (60*60))
             else:
                 msg = datetime.fromtimestamp(test_db.test_exe_ts).strftime("%a %d.%m %H:%M")
 
             if msg:
-                wid_status_line.show_message("info", "Executable compiled " + msg)
+                StatusLineWidget.get().show_message("info", "Executable compiled " + msg)
 
         else:
-            tc_names = gtest.gtest_list_tests()
+            tc_names = gtest_list_tests.gtest_list_tests()
             if tc_names is None:
                 return False
 
             self.prev_campaign_options = None
-            gtest.release_exe_file_copy()
+            trace_db.release_exe_file_copy()
             test_db.update_executable(test_db.test_exe_name, latest_exe_ts, tc_names)
 
         return True
 
 
     def check_filter_expression(self, reset_suppressions=True):
+        """
+        Check if the current content of the test case filter entry field is a
+        valid expression and each sub-expression matches at least one test
+        case and inform the user in case of such errors.
+        """
         if reset_suppressions:
             self.filter_expr_error.clear()
-        ok, msg = filter_expr.check_pattern(self.var_opt_filter.get(),
-                                            self.var_opt_run_disabled.get(),
-                                            self.filter_expr_error)
-        if not ok and msg:
-            tk_messagebox.showerror(parent=self.tk, message=msg)
-
-        if ok and self.slot_filter_change:
-            expr = filter_expr.Filter_expr(self.var_opt_filter.get(),
-                                           self.var_opt_run_disabled.get())
+        is_ok, msg = filter_expr.check_pattern(self.var_opt_filter.get(),
+                                               self.var_opt_run_disabled.get(),
+                                               self.filter_expr_error)
+        if not is_ok and msg:
+            tk_messagebox.showerror(parent=self.tk_top, message=msg)
+
+        if is_ok and self.slot_filter_change:
+            expr = filter_expr.FilterExpr(self.var_opt_filter.get(),
+                                          self.var_opt_run_disabled.get())
             self.slot_filter_change(expr)
-        return ok
+
+        return is_ok
 
 
     def __calc_remaining_repetitions(self):
         filter_str = self.prev_campaign_options["filter_str"]
-        expr = filter_expr.Filter_expr(filter_str, self.prev_campaign_options["run_disabled"])
+        expr = filter_expr.FilterExpr(filter_str, self.prev_campaign_options["run_disabled"])
         tc_list = expr.get_selected_tests()
         if tc_list:
             rep_cnt = int(self.var_opt_repetitions.get())
 
             min_cnt = min([test_db.test_case_stats[x][0] +
                            test_db.test_case_stats[x][1] +
                            test_db.test_case_stats[x][2] for x in tc_list])
@@ -714,58 +804,58 @@
                 return rep_cnt - min_cnt
         return 0
 
 
     def __check_test_options(self):
         msg = ""
         try:
-            msg = 'Value for "CPUs" is not a number.';
+            msg = 'Value for "CPUs" is not a number.'
             int(self.var_opt_job_count.get())
-            msg = 'Value for "Ignore filter" is not a number.';
+            msg = 'Value for "Ignore filter" is not a number.'
             int(self.var_opt_job_runall.get())
-            msg = 'Value for "Repetitions" is not a number.';
+            msg = 'Value for "Repetitions" is not a number.'
             int(self.var_opt_repetitions.get())
-            msg = 'Value for "Fail limit" is not a number.';
+            msg = 'Value for "Fail limit" is not a number.'
             int(self.var_opt_fail_max.get())
-        except:
-            tk_messagebox.showerror(parent=self.tk, message=msg)
+        except ValueError:
+            tk_messagebox.showerror(parent=self.tk_top, message=msg)
             return False
 
         if (self.var_opt_filter.get() and
-            (self.var_opt_job_runall.get() >= self.var_opt_job_count.get())):
-            answer = tk_messagebox.askokcancel(
-                        parent=self.tk,
-                        message="Really ignore filter string for all test jobs?")
+                (self.var_opt_job_runall.get() >= self.var_opt_job_count.get())):
+            msg = "Really ignore filter string for all test jobs?"
+            answer = tk_messagebox.askokcancel(parent=self.tk_top, message=msg)
             if not answer:
                 return False
 
         return True
 
 
     def __start_campaign_sub(self, filter_str, resume_rep_cnt=0, is_repeat=False):
         run_disabled = self.var_opt_run_disabled.get() if resume_rep_cnt == 0 \
                             else self.prev_campaign_options["run_disabled"]
-        expr = filter_expr.Filter_expr(filter_str, run_disabled)
+        expr = filter_expr.FilterExpr(filter_str, run_disabled)
         tc_list = expr.get_selected_tests()
 
         valgrind_cmd = ""
         if self.var_opt_valgrind.get() == 1:
-            valgrind_cmd = config_db.options["valgrind1"]
+            valgrind_cmd = config_db.get_opt("cmd_valgrind1")
         elif self.var_opt_valgrind.get() == 2:
-            valgrind_cmd = config_db.options["valgrind2"]
+            valgrind_cmd = config_db.get_opt("cmd_valgrind2")
         if self.var_opt_valgrind.get() and not valgrind_cmd:
             if tk_messagebox.askokcancel(
-                    parent=self.tk,
+                    parent=self.tk_top,
                     message="Valgrind command line is unknown. Configure now?"):
-                dlg_config.create_dialog(self.tk)
+                ConfigDialog.create_dialog(self.tk_top)
             return
 
         clean_trace = self.var_opt_clean_trace.get()
         if clean_trace and valgrind_cmd:
-            wid_status_line.show_message("warning", "Ignoring clean-trace option with valgrind")
+            StatusLineWidget.get().show_message("warning",
+                                                "Ignoring clean-trace option with valgrind")
             clean_trace = False
 
         if not resume_rep_cnt:
             rep_cnt = 1 if is_repeat else self.var_opt_repetitions.get()
         else:
             rep_cnt = resume_rep_cnt
 
@@ -774,15 +864,15 @@
                 "exe_name": test_db.test_exe_name,
                 "filter_str": filter_str,
                 "run_disabled": run_disabled,
             }
 
         self.wid_cmd_run.configure(cursor="watch")
 
-        gtest.gtest_ctrl.start(
+        gtest_ctrl.gtest_ctrl.start(
             self.var_opt_job_count.get(),
             self.var_opt_job_runall.get() if not is_repeat else 0,
             rep_cnt,
             filter_str,
             tc_list,
             resume_rep_cnt != 0,
             self.var_opt_run_disabled.get(),
@@ -792,9 +882,9 @@
             clean_trace,
             self.var_opt_clean_core.get(),
             self.var_opt_break_on_fail.get(),
             self.var_opt_break_on_except.get())
 
 
     def __handle_option_change(self):
-        gtest.gtest_ctrl.update_options(self.var_opt_clean_trace.get(),
-                                        self.var_opt_clean_core.get())
+        gtest_ctrl.gtest_ctrl.update_options(self.var_opt_clean_trace.get(),
+                                             self.var_opt_clean_core.get())
```

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/wid_test_log.py` & `mote-gtest-gui-0.9.0/gtest_gui/wid_test_log.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,251 +13,306 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
+"""
+This module implements the test result log class.
+"""
+
 from datetime import datetime
 from enum import Enum
 import bisect
 import os
-import re
 import time
 
 import tkinter as tk
 from tkinter import messagebox as tk_messagebox
 
 import gtest_gui.bisect
 import gtest_gui.config_db as config_db
 import gtest_gui.dlg_browser as dlg_browser
-import gtest_gui.filter_expr as filter_expr
-import gtest_gui.gtest as gtest
+import gtest_gui.gtest_ctrl as gtest_ctrl
 import gtest_gui.test_db as test_db
+import gtest_gui.trace_db as trace_db
 import gtest_gui.tk_utils as tk_utils
-import gtest_gui.wid_status_line as wid_status_line
-import gtest_gui.wid_test_ctrl as wid_test_ctrl
-import gtest_gui.wid_text_sel as wid_text_sel
+from gtest_gui.wid_status_line import StatusLineWidget
+from gtest_gui.wid_text_sel import TextSelWidget
 
 
-class Sort_mode(Enum):
+class SortMode(Enum):
+    """ Internal enumeration for sort options selectable by the user. """
     by_name = 0
     by_failure = 1
     by_duration = 2
     by_seed = 3
 
 
-class Test_log_widget(object):
+class TestLogWidget:
+    """
+    This class implements the lower half of the main window, containing test
+    result log in form of a list. The list reflect the "test_results" list in
+    the test database and thus initially contains imported results and
+    subsequently is updated when test campaigns are running via registered
+    callback. The user can remove elements from the data base and list using
+    menu or key bindings.
+    """
+
     def __init__(self, tk_top, parent):
-        self.tk = tk_top
+        """
+        Constructs an instance of the TestLogWidget within the given parent
+        widget. The result log is initially empty and should be populated with
+        database contents by calling populate_log() after main window is fully
+        constructed.
+        """
+        self.tk_top = tk_top
+        self.test_ctrl = None # set later
         self.test_ctrl_visible = True
         self.opt_sort_modes = []
         self.opt_filter_exe_ts = 0
         self.opt_filter_tc_names = None
         self.log_idx_map = []
 
+        self.var_opt_sort_tc_name = tk.BooleanVar(self.tk_top, False)
+        self.var_opt_sort_seed = tk.BooleanVar(self.tk_top, False)
+        self.var_opt_sort_duration = tk.BooleanVar(self.tk_top, False)
+        self.var_opt_sort_exception = tk.BooleanVar(self.tk_top, False)
+
+        self.var_opt_filter_pass = tk.BooleanVar(self.tk_top, False)
+        self.var_opt_filter_exe_name = tk.BooleanVar(self.tk_top, False)
+        self.var_opt_filter_exe_ts = tk.BooleanVar(self.tk_top, False)
+        self.var_opt_filter_tc_name = tk.BooleanVar(self.tk_top, False)
+
         self.wid_pane = tk.PanedWindow(parent, orient=tk.VERTICAL)
         self.__create_log_widget(self.wid_pane)
         self.__create_trace_widget(self.wid_pane)
 
-        test_db.Test_db_slots.result_appended = self.__append_new_result
-        test_db.Test_db_slots.repeat_req_update = self.update_repetition_status
-        test_db.Test_db_slots.executable_update = self.__refill_log
+        test_db.register_slot(test_db.SlotTypes.result_appended, self.__append_new_result)
+        test_db.register_slot(test_db.SlotTypes.repeat_req_update, self.update_repetition_status)
+        test_db.register_slot(test_db.SlotTypes.executable_update, self.__refill_log)
 
 
     def get_widget(self):
+        """ Returns the root widget used by this instance. """
         return self.wid_pane
 
 
     def set_wid_test_ctrl(self, test_ctrl):
+        """
+        Links the widget with the test control widget. This link is currently
+        only used for access to the test case filter value.
+        """
         self.test_ctrl = test_ctrl
 
 
     def __create_log_widget(self, wid_pane):
         wid_frm = tk.Frame(wid_pane)
         wid_txt = tk.Text(wid_frm, width=1, height=20, font=tk_utils.font_content, wrap=tk.NONE,
                           exportselection=0, insertofftime=0, cursor="top_left_arrow")
         wid_txt.pack(side=tk.LEFT, fill=tk.BOTH, expand=1)
         wid_sb = tk.Scrollbar(wid_frm, orient=tk.VERTICAL, command=wid_txt.yview, takefocus=0)
         wid_sb.pack(side=tk.LEFT, fill=tk.Y)
         wid_txt.configure(yscrollcommand=wid_sb.set)
 
         wid_txt.tag_configure("highlight", font=tk_utils.font_content_bold, foreground="#2020A0")
 
-        wid_txt.bindtags([wid_txt, self.tk, "TextSel", "all"])
+        wid_txt.bindtags([wid_txt, self.tk_top, "TextSel", "all"])
         wid_txt.bind("<ButtonRelease-3>", lambda e: self.__post_context_menu(e.widget, e.x, e.y))
-        wid_txt.bind("<Double-Button-1>", lambda e: tk_utils.bind_call_and_break(self.do_open_trace_browser))
-        wid_txt.bind("<Key-Return>", lambda e: self.do_open_trace_browser())
-        wid_txt.bind("<Key-Delete>", lambda e: self.do_remove_selected_results())
+        wid_txt.bind("<Double-Button-1>", lambda e:
+                     tk_utils.bind_call_and_break(self.__do_open_trace_browser))
+        wid_txt.bind("<Key-Return>", lambda e: self.__do_open_trace_browser())
+        wid_txt.bind("<Key-Delete>", lambda e: self.__do_remove_selected_results())
 
-        self.sel_obj = wid_text_sel.Text_sel_wid(wid_txt,
-                                                 self.__handle_selection_change, self.__get_len)
+        self.sel_obj = TextSelWidget(wid_txt, self.__handle_selection_change, self.__get_len)
 
-        if config_db.log_pane_height:
-            wid_pane.add(wid_frm, sticky="news", height=config_db.log_pane_height)
+        if config_db.get_opt("log_pane_height"):
+            wid_pane.add(wid_frm, sticky="news", height=config_db.get_opt("log_pane_height"))
         else:
             wid_pane.add(wid_frm, sticky="news")
 
         wid_frm.bind("<Configure>", lambda e: self.__window_resized(True, e.height))
         self.wid_log = wid_txt
         self.wid_frm1 = wid_frm
 
 
     def __create_trace_widget(self, wid_pane):
         wid_frm = tk.Frame(wid_pane)
         wid_txt = tk.Text(wid_frm, width=40, height=1, wrap=tk.NONE,
                           insertofftime=0, font=tk_utils.font_trace)
         wid_txt.pack(side=tk.LEFT, fill=tk.BOTH, expand=1)
-        wid_txt.bindtags([wid_txt, "TextReadOnly", self.tk, "all"])
+        wid_txt.bindtags([wid_txt, "TextReadOnly", self.tk_top, "all"])
         wid_txt.tag_configure("failure", background="#FF4040")
         wid_sb = tk.Scrollbar(wid_frm, orient=tk.VERTICAL, command=wid_txt.yview, takefocus=0)
         wid_sb.pack(side=tk.LEFT, fill=tk.Y)
         wid_txt.configure(yscrollcommand=wid_sb.set)
 
-        if not config_db.trace_pane_height:
-            config_db.trace_pane_height = 9 * tk_utils.font_trace.metrics("linespace")
-        wid_pane.add(wid_frm, sticky="news", height=config_db.trace_pane_height)
+        if not config_db.get_opt("trace_pane_height"):
+            config_db.set_opt("trace_pane_height", 9 * tk_utils.font_trace.metrics("linespace"))
+        wid_pane.add(wid_frm, sticky="news", height=config_db.get_opt("trace_pane_height"))
 
         wid_frm.bind("<Configure>", lambda e: self.__window_resized(False, e.height))
         self.wid_trace = wid_txt
         self.wid_frm2 = wid_frm
 
 
     def add_menu_commands(self, wid_men):
-        self.var_opt_sort_tc_name = tk.BooleanVar(self.tk, False)
-        self.var_opt_sort_seed = tk.BooleanVar(self.tk, False)
-        self.var_opt_sort_duration = tk.BooleanVar(self.tk, False)
-        self.var_opt_sort_exception = tk.BooleanVar(self.tk, False)
-
-        self.var_opt_filter_pass = tk.BooleanVar(self.tk, False)
-        self.var_opt_filter_exe_name = tk.BooleanVar(self.tk, False)
-        self.var_opt_filter_exe_ts = tk.BooleanVar(self.tk, False)
-        self.var_opt_filter_tc_name = tk.BooleanVar(self.tk, False)
-
+        """
+        Populates the given menu (which is part of the main menubar) with
+        commands operating on the result log widget.
+        """
         wid_men.add_checkbutton(label="Show only failed results",
-                                command=self.__toggle_verdict_filter, variable=self.var_opt_filter_pass)
+                                tooltip="result_log.filter_failed",
+                                command=self.__toggle_verdict_filter,
+                                variable=self.var_opt_filter_pass)
         wid_men.add_checkbutton(label="Show only results from current exe. file",
-                                command=self.__toggle_exe_name_filter, variable=self.var_opt_filter_exe_name)
-        wid_men.add_checkbutton(label="Show only results from current exe. version",
-                                command=self.__toggle_exe_ts_filter, variable=self.var_opt_filter_exe_ts)
+                                tooltip="result_log.filter_exe_file",
+                                command=self.__toggle_exe_name_filter,
+                                variable=self.var_opt_filter_exe_name)
+        wid_men.add_checkbutton(label="Show only results from selected exe. version",
+                                tooltip="result_log.filter_exe_version",
+                                command=self.__toggle_exe_ts_filter,
+                                variable=self.var_opt_filter_exe_ts)
         wid_men.add_checkbutton(label="Show only selected test cases",
-                                command=self.__toggle_tc_name_filter, variable=self.var_opt_filter_tc_name)
+                                tooltip="result_log.filter_tc_name",
+                                command=self.__toggle_tc_name_filter,
+                                variable=self.var_opt_filter_tc_name)
         wid_men.add_separator()
 
         wid_men.add_checkbutton(
-                label="Sort by test case name",
-                command=lambda: self.__toggle_sort_mode(self.var_opt_sort_tc_name.get(), Sort_mode.by_name),
-                variable=self.var_opt_sort_tc_name)
+            label="Sort by test case name",
+            tooltip="result_log.sort_tc_name",
+            command=lambda: self.__toggle_sort_mode(self.var_opt_sort_tc_name.get(),
+                                                    SortMode.by_name),
+            variable=self.var_opt_sort_tc_name)
         wid_men.add_checkbutton(
-                label="Sort by seed",
-                command=lambda: self.__toggle_sort_mode(self.var_opt_sort_seed.get(), Sort_mode.by_seed),
-                variable=self.var_opt_sort_seed)
+            label="Sort by seed",
+            tooltip="result_log.sort_seed",
+            command=lambda: self.__toggle_sort_mode(self.var_opt_sort_seed.get(),
+                                                    SortMode.by_seed),
+            variable=self.var_opt_sort_seed)
         wid_men.add_checkbutton(
-                label="Sort by duration",
-                command=lambda: self.__toggle_sort_mode(self.var_opt_sort_duration.get(), Sort_mode.by_duration),
-                variable=self.var_opt_sort_duration)
+            label="Sort by duration",
+            tooltip="result_log.sort_duration",
+            command=lambda: self.__toggle_sort_mode(self.var_opt_sort_duration.get(),
+                                                    SortMode.by_duration),
+            variable=self.var_opt_sort_duration)
         wid_men.add_checkbutton(
-                label="Sort by failure type",
-                command=lambda: self.__toggle_sort_mode(self.var_opt_sort_exception.get(), Sort_mode.by_failure),
-                variable=self.var_opt_sort_exception)
+            label="Sort by failure type",
+            tooltip="result_log.sort_failure",
+            command=lambda: self.__toggle_sort_mode(self.var_opt_sort_exception.get(),
+                                                    SortMode.by_failure),
+            variable=self.var_opt_sort_exception)
 
 
     def __window_resized(self, is_log, height):
         if is_log:
             if self.test_ctrl_visible:
-                config_db.log_pane_height = height
+                config_db.set_opt("log_pane_height", height)
             else:
-                config_db.log_pane_solo_height = height
+                config_db.set_opt("log_pane_solo_height", height)
         else:
             if self.test_ctrl_visible:
-                config_db.trace_pane_height = height
+                config_db.set_opt("trace_pane_height", height)
             else:
-                config_db.trace_pane_solo_height = height
-
-        config_db.rc_file_update_after_idle()
+                config_db.set_opt("trace_pane_solo_height", height)
 
 
     def toggle_test_ctrl_visible(self, visible):
+        """
+        Perform geometry management after the test control widget visibility
+        was toggled. Specifically, the requested size of the widget is updated
+        to the previously used size in this mode. Sizes are remembered
+        separately for the case that the test control widget is shown in the
+        main window, and not shown.
+        """
         self.test_ctrl_visible = visible
 
         if visible:
-            if config_db.log_pane_height:
-                self.wid_pane.paneconfigure(self.wid_frm1, height=config_db.log_pane_height)
-            if config_db.trace_pane_height:
-                self.wid_pane.paneconfigure(self.wid_frm2, height=config_db.trace_pane_height)
-        else:
-            if config_db.log_pane_solo_height:
-                self.wid_pane.paneconfigure(self.wid_frm1, height=config_db.log_pane_solo_height)
-            if config_db.trace_pane_solo_height:
-                self.wid_pane.paneconfigure(self.wid_frm2, height=config_db.trace_pane_solo_height)
+            if config_db.get_opt("log_pane_height"):
+                self.wid_pane.paneconfigure(self.wid_frm1,
+                                            height=config_db.get_opt("log_pane_height"))
+            if config_db.get_opt("trace_pane_height"):
+                self.wid_pane.paneconfigure(self.wid_frm2,
+                                            height=config_db.get_opt("trace_pane_height"))
+        else:
+            if config_db.get_opt("log_pane_solo_height"):
+                self.wid_pane.paneconfigure(self.wid_frm1,
+                                            height=config_db.get_opt("log_pane_solo_height"))
+            if config_db.get_opt("trace_pane_solo_height"):
+                self.wid_pane.paneconfigure(self.wid_frm2,
+                                            height=config_db.get_opt("trace_pane_solo_height"))
 
 
     def __get_len(self):
         return len(self.log_idx_map)
 
 
     def __handle_selection_change(self, sel):
         if len(sel) == 1:
             log_idx = self.log_idx_map[sel[0]]
-            self.show_trace_preview(log_idx)
+            self.__show_trace_preview(log_idx)
         else:
-            self.clear_trace_preview()
+            self.__clear_trace_preview()
 
 
     def __get_mapped_selection(self):
         sel = self.sel_obj.text_sel_get_selection()
         return [self.log_idx_map[idx] for idx in sel]
 
 
     def __append_new_result(self):
         log_idx = len(test_db.test_results) - 1
         log = test_db.test_results[log_idx]
 
         if self.__matches_filter(log):
             if self.opt_sort_modes:
                 list_idx = gtest_gui.bisect.bisect_left(self.log_idx_map, log_idx,
-                                                       self.__get_sort_key_fn())
+                                                        self.__get_sort_key_fn())
                 self.log_idx_map.insert(list_idx, log_idx)
             else:
+                list_idx = len(self.log_idx_map)
                 self.log_idx_map.append(log_idx)
-                list_idx = len(test_db.test_results) - 1
 
             txt = self.__format_log_line(log_idx)
 
             line = "%d.0" % (list_idx + 1)
             self.wid_log.insert(line, *txt)
 
             if self.sel_obj.text_sel_get_selection():
                 self.sel_obj.text_sel_adjust_insert(list_idx)
-            else:
+            elif not self.opt_sort_modes:
                 self.wid_log.see(line)
 
 
     def update_repetition_status(self, tc_name):
+        """ Updates the result log after a change of the given test case's repetiton status. """
+        match_fn = self.__get_filter_match_fn()
         for idx in range(len(self.log_idx_map)):
             log_idx = self.log_idx_map[idx]
             log = test_db.test_results[log_idx]
             if log[0] == tc_name:
-                if self.__matches_filter(log):
+                if match_fn(log):
                     self.__update_log_line(idx, log_idx)
                 else:
                     self.__remove_log_line(idx)
                     idx -= 1
 
 
     def __remove_log_line(self, list_idx):
-        line_1 = "%d.0" % (idx + 1)
-        line_2 = "%d.0" % (idx + 2)
+        line_1 = "%d.0" % (list_idx + 1)
+        line_2 = "%d.0" % (list_idx + 2)
         self.wid_log.delete(line_1, line_2)
 
-        del self.log_idx_map[idx]
-        self.sel_obj.text_sel_adjust_deletion(idx)
+        del self.log_idx_map[list_idx]
+        self.sel_obj.text_sel_adjust_deletion(list_idx)
 
         if not self.sel_obj.text_sel_get_selection():
-            self.clear_trace_preview()
+            self.__clear_trace_preview()
 
 
     def __update_log_line(self, list_idx, log_idx):
         txt = self.__format_log_line(log_idx)
         line_1 = "%d.0" % (list_idx + 1)
         line_2 = "%d.0" % (list_idx + 2)
 
@@ -331,35 +386,45 @@
                 tagged_txt.append([])
             else:
                 tagged_txt.append(" (%s)" % os.path.basename(log[1]))
                 tagged_txt.append([])
 
         elif log[2] != test_db.test_exe_ts:
             if now - log[2] <= 11*60*60:
-                tagged_txt.append(datetime.fromtimestamp(log[2]).strftime(" (old exe: %H:%M:%S)"))
+                tagged_txt.append(datetime.fromtimestamp(log[2]).strftime(
+                    " (old exe: %H:%M:%S)"))
                 tagged_txt.append([])
             else:
-                tagged_txt.append(datetime.fromtimestamp(log[2]).strftime(" (old exe: %a %d.%m %H:%M)"))
+                tagged_txt.append(datetime.fromtimestamp(log[2]).strftime(
+                    " (old exe: %a %d.%m %H:%M)"))
                 tagged_txt.append([])
 
         tagged_txt.extend(["\n", []])
         return tagged_txt
 
 
     def populate_log(self):
+        """
+        Refill the result log widget with results in the database from scratch
+        and set the view to the last item in the list.
+        """
         self.wid_log.delete("1.0", "end")
 
+        match_fn = self.__get_filter_match_fn()
         logs = [idx for idx in range(len(test_db.test_results))
-                    if self.__matches_filter(test_db.test_results[idx])]
+                if match_fn(test_db.test_results[idx])]
 
         self.log_idx_map = self.__sort_idx_map(logs)
 
+        content = []
         for log_idx in self.log_idx_map:
-            txt = self.__format_log_line(log_idx)
-            self.wid_log.insert("end", *txt)
+            content.extend(self.__format_log_line(log_idx))
+        if content:
+            # pylint: disable=no-value-for-parameter # false positive b/c content never empty
+            self.wid_log.insert("end", *content)
 
 
     def __refill_log(self, restore_view=False, restore_selection=False):
         if restore_view or restore_selection:
             prev_log = self.log_idx_map
             prev_sel = self.sel_obj.text_sel_get_selection()
             prev_log_idx = self.log_idx_map[prev_sel[0]] if prev_sel else None
@@ -382,102 +447,159 @@
         if restore_view and (self.log_idx_map == prev_log):
             self.sel_obj.text_sel_set_selection(prev_sel)
         elif restore_selection and new_sel is not None:
             self.wid_log.see("%d.0" % (new_sel + 1))
             self.sel_obj.text_sel_set_selection([new_sel])
         else:
             self.sel_obj.text_sel_set_selection([])
-            self.clear_trace_preview()
+            self.__clear_trace_preview()
 
 
     def __sort_idx_map(self, logs):
         for mode in reversed(self.opt_sort_modes):
-            if mode == Sort_mode.by_name:
+            if mode == SortMode.by_name:
                 logs = sorted(logs, key=lambda x: test_db.test_results[x][0])
-            elif mode == Sort_mode.by_failure:
+            elif mode == SortMode.by_failure:
                 logs = sorted(logs, key=lambda x: test_db.test_results[x][9])
                 logs = sorted(logs, key=lambda x: test_db.test_results[x][8])
-            elif mode == Sort_mode.by_duration:
+            elif mode == SortMode.by_duration:
                 logs = sorted(logs, key=lambda x: test_db.test_results[x][10])
-            elif mode == Sort_mode.by_seed:
+            elif mode == SortMode.by_seed:
                 logs = sorted(logs, key=lambda x: test_db.test_results[x][14])
         return logs
 
 
     def __get_sort_key_fn(self):
         if len(self.opt_sort_modes) == 1:
             mode = self.opt_sort_modes[0]
-            if mode == Sort_mode.by_name:
+            if mode == SortMode.by_name:
                 return lambda x: test_db.test_results[x][0]
 
-            elif mode == Sort_mode.by_failure:
+            if mode == SortMode.by_failure:
                 return lambda x: (test_db.test_results[x][8], test_db.test_results[x][9])
 
-            elif mode == Sort_mode.by_duration:
+            if mode == SortMode.by_duration:
                 return lambda x: test_db.test_results[x][10]
 
-            elif mode == Sort_mode.by_seed:
+            if mode == SortMode.by_seed:
                 return lambda x: test_db.test_results[x][14]
 
         elif len(self.opt_sort_modes) > 1:
             key_idx = []
             for mode in self.opt_sort_modes:
-                if mode == Sort_mode.by_name:
+                if mode == SortMode.by_name:
                     key_idx.append(0)
 
-                elif mode == Sort_mode.by_failure:
+                elif mode == SortMode.by_failure:
                     key_idx.append(8)
                     key_idx.append(9)
 
-                elif mode == Sort_mode.by_duration:
+                elif mode == SortMode.by_duration:
                     key_idx.append(10)
 
-                elif mode == Sort_mode.by_seed:
+                elif mode == SortMode.by_seed:
                     key_idx.append(14)
 
             return lambda log_idx: [test_db.test_results[log_idx][x] for x in key_idx]
 
         return lambda x: x
 
 
     def __matches_filter(self, log):
-        return ( ((not self.var_opt_filter_pass.get()) or
-                    (log[3] >= 2)) and
-                 ((not self.var_opt_filter_exe_name.get()) or
-                    (log[1] == test_db.test_exe_name)) and
-                 ((not self.var_opt_filter_exe_ts.get()) or
-                    ((log[2] >= self.opt_filter_exe_ts) and (log[1] == test_db.test_exe_name))) and
-                 ((not self.var_opt_filter_tc_name.get()) or
-                    (log[0] in self.opt_filter_tc_names)) )
+        """
+        Check if the given resultlog entry matches current result log filter configuration.
+        """
+        return (((not self.var_opt_filter_pass.get()) or
+                 (log[3] >= 2)) and
+                ((not self.var_opt_filter_exe_name.get()) or
+                 (log[1] == test_db.test_exe_name)) and
+                ((not self.var_opt_filter_exe_ts.get()) or
+                 ((log[2] >= self.opt_filter_exe_ts) and (log[1] == test_db.test_exe_name))) and
+                ((not self.var_opt_filter_tc_name.get()) or
+                 (log[0] in self.opt_filter_tc_names)))
+
+
+    def __get_filter_match_fn(self):
+        """
+        Returns a lambda function that when invoked, performs an equivalent
+        check as function __matches_filter(). This should be used when
+        filtering is done on many log items in a loop. Using the returned
+        lambda is faster than calling the generic filter function directly, as
+        it performs fewer comparisons.
+        """
+        filter_pass = self.var_opt_filter_pass.get()
+        filter_exe_name = self.var_opt_filter_exe_name.get()
+        filter_exe_ts = self.var_opt_filter_exe_ts.get()
+        filter_tc_name = self.var_opt_filter_tc_name.get()
+
+        nof_filters = sum((filter_pass, filter_exe_name, filter_exe_ts, filter_tc_name))
+
+        if nof_filters == 0:
+            return lambda log: True
+
+        if nof_filters == 1:
+            if filter_pass:
+                return lambda log: (log[3] >= 2)
+            if filter_exe_name:
+                return lambda log, exe_name=test_db.test_exe_name: (log[1] == exe_name)
+            if filter_exe_ts:
+                return lambda log, \
+                              exe_ts=self.opt_filter_exe_ts, \
+                              exe_name=test_db.test_exe_name: \
+                                ((log[2] >= exe_ts) and (log[1] == exe_name))
+            # else: filter_tc_name
+            return lambda log, names=self.opt_filter_tc_names: (log[0] in names)
+
+        # else: nof_filters > 1
+        return lambda log, \
+                      exe_ts=self.opt_filter_exe_ts, \
+                      exe_name=test_db.test_exe_name, \
+                      names=self.opt_filter_tc_names: \
+                ((not filter_pass or (log[3] >= 2)) and
+                 (not filter_exe_name or (log[1] == exe_name)) and
+                 (not filter_exe_ts or ((log[2] >= exe_ts) and (log[1] == exe_name))) and
+                 (not filter_tc_name or (log[0] in names)))
 
 
     def __toggle_verdict_filter(self):
         self.__refill_log(restore_selection=True)
 
 
     def __toggle_exe_name_filter(self):
-        self.__refill_log(restore_selection=True)
+        if test_db.test_exe_name:
+            self.__refill_log(restore_selection=True)
 
+        else:
+            self.var_opt_filter_exe_name.set(False)
+            msg = "No executable selected yet. Please select one via the Control menu."
+            tk_messagebox.showerror(parent=self.tk_top, message=msg)
 
-    def __toggle_exe_ts_filter(self, exe_ts = None):
-        if not exe_ts:
-            exe_ts = test_db.test_exe_ts
 
-        self.opt_filter_exe_ts = exe_ts
-        self.__refill_log(restore_selection=True)
+    def __toggle_exe_ts_filter(self, exe_ts=None):
+        if exe_ts or test_db.test_exe_name:
+            if not exe_ts:
+                exe_ts = test_db.test_exe_ts
+
+            self.opt_filter_exe_ts = exe_ts
+            self.__refill_log(restore_selection=True)
 
+        elif self.var_opt_filter_exe_ts.get():
+            self.var_opt_filter_exe_ts.set(False)
+            msg = "No executable selected yet. Please select one via the Control menu."
+            tk_messagebox.showerror(parent=self.tk_top, message=msg)
 
-    def __toggle_tc_name_filter(self, tc_names = None):
+
+    def __toggle_tc_name_filter(self, tc_names=None):
         if self.var_opt_filter_tc_name.get():
             if tc_names is None:
                 tc_names = [test_db.test_results[log_idx][0]
-                                for log_idx in self.__get_mapped_selection()]
+                            for log_idx in self.__get_mapped_selection()]
             if not tc_names:
                 self.var_opt_filter_tc_name.set(False) # must come before messagebox
-                tk_messagebox.showerror(parent=self.tk, message="No results selected")
+                tk_messagebox.showerror(parent=self.tk_top, message="No results selected")
                 return
 
             self.opt_filter_tc_names = set(tc_names)
         else:
             self.opt_filter_tc_names = None
 
         self.__refill_log(restore_selection=True)
@@ -488,44 +610,32 @@
         if enable:
             self.opt_sort_modes.append(mode)
 
         self.__refill_log(restore_selection=True)
 
 
     def __delete_multiple_results(self, idx_list):
-        idx_list = sorted(idx_list)
-        # Copy items to a new list, except for those at selected indices. As the result list
-        # can be rather large, this is significantly faster than deleting items in place.
-        new_list = []
-        rm_idx = 0
-        for idx in range(len(test_db.test_results)):
-            if idx == idx_list[rm_idx]:
-                if rm_idx + 1 < len(idx_list):
-                    rm_idx += 1
-            else:
-                new_list.append(test_db.test_results[idx])
-
-        test_db.test_results = new_list
+        test_db.delete_results(idx_list)
         self.__refill_log()
 
 
     def __delete_single_result(self, idx):
         log_idx = bisect.bisect_left(self.log_idx_map, idx)
         if (log_idx >= len(self.log_idx_map)) or (self.log_idx_map[log_idx] != idx):
             raise ValueError
 
         line_1 = "%d.0" % (log_idx + 1)
         line_2 = "%d.0" % (log_idx + 2)
         self.wid_log.delete(line_1, line_2)
 
         self.sel_obj.text_sel_adjust_deletion(log_idx)
         if not self.sel_obj.text_sel_get_selection():
-            self.clear_trace_preview()
+            self.__clear_trace_preview()
 
-        del test_db.test_results[idx]
+        test_db.delete_results([idx])
 
         new_list = self.log_idx_map[:log_idx]
         if log_idx + 1 < len(self.log_idx_map):
             new_list.extend([x - 1 for x in self.log_idx_map[log_idx + 1:]])
         self.log_idx_map = new_list
 
 
@@ -564,23 +674,23 @@
                     elif expr.can_deselect_test(tc_name):
                         any_can_deselect = True
 
             if len(sel) == 1:
                 log = test_db.test_results[sel[0]]
                 if log[4]:
                     wid_men.add_command(label="Open trace of this test case",
-                                        command=lambda: self.do_open_trace_browser(False))
+                                        command=lambda: self.__do_open_trace_browser(False))
                     wid_men.add_command(label="Open trace of complete test run",
-                                        command=lambda: self.do_open_trace_browser(True))
+                                        command=lambda: self.__do_open_trace_browser(True))
 
                 if log[7]:
                     wid_men.add_command(label="Extract stack trace from core dump file",
                                         command=lambda name=log[0], exe_name=log[1],
                                                        exe_ts=log[2], core=log[7]:
-                                            self.do_open_stack_trace(name, exe_name, exe_ts, core))
+                                        self.__do_open_stack_trace(name, exe_name, exe_ts, core))
 
                 if log[4] or log[7]:
                     wid_men.add_separator()
 
             need_sep = False
             if any_can_select:
                 wid_men.add_command(label="Add selected test case%s to filter" % plural_s,
@@ -598,234 +708,247 @@
             if any_rep_req:
                 wid_men.add_command(label="Clear selected repeat request%s" % plural_s,
                                     command=lambda: self.do_request_repetition(False))
                 need_sep = True
 
             if len(sel) == 1:
                 wid_men.add_command(label="Do not show result logs from this exe. version",
-                                    command=self.do_filter_exe_ts)
+                                    command=self.__do_filter_exe_ts)
                 need_sep = True
 
             if need_sep:
                 wid_men.add_separator()
 
             wid_men.add_command(label="Delete selected test result%s" % plural_s,
-                                command=self.do_remove_selected_results)
+                                command=self.__do_remove_selected_results)
 
             if any_with_trace:
                 wid_men.add_command(label="Export selected trace%s into a ZIP archive" % plural_s,
-                                    command=self.do_export_trace)
+                                    command=self.__do_export_trace)
             post_menu = True
 
         need_sep = post_menu
         if len(self.log_idx_map) < len(test_db.test_results):
-            if need_sep: wid_men.add_separator()
+            if need_sep:
+                wid_men.add_separator()
             wid_men.add_command(label="Remove all currently filtered results",
-                                command=self.do_remove_filtered_results)
+                                command=self.__do_remove_filtered_results)
             need_sep = False
             post_menu = True
 
         for log in test_db.test_results:
             if ((log[3] == 0) and
                     ((log[1] != test_db.test_exe_name) or (log[2] < test_db.test_exe_ts))):
-                if need_sep: wid_men.add_separator()
+                if need_sep:
+                    wid_men.add_separator()
                 wid_men.add_command(label="Remove results of passed tests from old exe.",
-                                    command=self.do_remove_old_pass_results)
+                                    command=self.__do_remove_old_pass_results)
                 post_menu = True
                 break
 
         if post_menu:
             tk_utils.post_context_menu(parent, xcoo, ycoo)
 
 
-    def do_remove_selected_results(self):
+    def __do_remove_selected_results(self):
         sel = self.__get_mapped_selection()
         if sel:
             self.__remove_trace_files(sel)
         else:
-            wid_status_line.show_message("warning", "Selection is empty - nothing to remove.")
+            StatusLineWidget.get().show_message("warning",
+                                                "Selection is empty - nothing to remove.")
 
 
-    def do_remove_old_pass_results(self):
+    def __do_remove_old_pass_results(self):
         idx_list = []
         for idx in range(len(test_db.test_results)):
             log = test_db.test_results[idx]
             if ((log[3] == 0) and
                     ((log[1] != test_db.test_exe_name) or (log[2] < test_db.test_exe_ts))):
                 idx_list.append(idx)
 
         if idx_list:
             self.__remove_trace_files(idx_list)
         else:
             msg = "There are no results of passed tests from old executables."
-            tk_messagebox.showerror(parent=self.tk, message=msg)
+            tk_messagebox.showerror(parent=self.tk_top, message=msg)
 
 
-    def do_remove_filtered_results(self):
-        idx_list = []
-        for idx in range(len(test_db.test_results)):
-            log = test_db.test_results[idx]
-            if not self.__matches_filter(log):
-                idx_list.append(idx)
-
+    def __do_remove_filtered_results(self):
+        idx_list = set(range(len(test_db.test_results))) - set(self.log_idx_map)
         if idx_list:
             self.__remove_trace_files(idx_list)
         else:
-            tk_messagebox.showerror(parent=self.tk, message="There are no filtered log entries.")
+            msg = "There are no filtered log entries."
+            tk_messagebox.showerror(parent=self.tk_top, message=msg)
 
 
     def __remove_trace_files(self, idx_list):
         idx_list = sorted(idx_list)
-        rm_files = set()
+        rm_trace_files = set()
+        rm_core_files = set()
         rm_exe = set()
         rm_idx = 0
-        used_files = set()
+        used_trace_files = set()
         used_exe = set()
         for idx in range(len(test_db.test_results)):
             log = test_db.test_results[idx]
             if idx == idx_list[rm_idx]:
                 if log[4] and log[13] != 2:  # never remove traces imported via cmd line
-                    rm_files.add(log[4])
+                    rm_trace_files.add(log[4])
                 if log[7]:
-                    rm_files.add(log[7])
+                    rm_core_files.add(log[7])
                     if log[1]:
                         rm_exe.add((log[1], log[2]))
                 if rm_idx + 1 < len(idx_list):
                     rm_idx += 1
             else:
                 if log[4]:
-                    used_files.add(log[4])
-                if log[7]:
-                    used_files.add(log[7])
-                    if log[1]:
-                        used_exe.add((log[1], log[2]))
+                    used_trace_files.add(log[4])
+                if log[7] and log[1]:
+                    used_exe.add((log[1], log[2]))
 
-        rm_files -= used_files
-        rm_files -= gtest.gtest_ctrl.get_out_file_names()
+        rm_trace_files -= used_trace_files
+        rm_trace_files -= gtest_ctrl.gtest_ctrl.get_out_file_names()
 
         rm_exe -= used_exe
         rm_exe.discard((test_db.test_exe_name, test_db.test_exe_ts))
 
         count = len(idx_list)
         if count == 1:
-            msg = "Really remove this result log entry"
+            msg = "Really remove this result log entry?"
         else:
-            msg = "Really remove %d result log entries" % count
+            msg = "Really remove %d result log entries?" % count
+
+        if rm_trace_files or rm_core_files:
+            msg += " This will also remove "
+
+            if len(rm_trace_files) == 1:
+                msg += "one trace output file"
+            elif rm_trace_files:
+                msg += "%d trace files" % len(rm_trace_files)
+
+            if rm_core_files and rm_trace_files:
+                msg += " and "
 
-        if len(rm_files) == 1:
-            msg += " and their trace output file"
-        elif rm_files:
-            msg += " and %d trace output and core dump files" % len(rm_files)
+            if len(rm_core_files) == 1:
+                msg += "one core dump file"
+            elif rm_core_files:
+                msg += "%d core dump files" % len(rm_core_files)
 
-        msg += "? (This cannot be undone.)"
-        answer = tk_messagebox.askokcancel(parent=self.tk, message=msg)
+            msg += "."
+
+        msg += " (This cannot be undone.)"
+
+        answer = tk_messagebox.askokcancel(parent=self.tk_top, message=msg)
         if answer:
             if len(idx_list) == 1:
                 self.__delete_single_result(idx_list[0])
             else:
                 self.__delete_multiple_results(idx_list)
 
-            gtest.remove_trace_or_core_files(rm_files, rm_exe)
+            trace_db.remove_trace_or_core_files(rm_trace_files, rm_exe)
 
 
-    def check_tc_names_in_exe(self, sel):
+    def __check_tc_names_in_exe(self, sel):
         for idx in sel:
             log = test_db.test_results[idx]
             if log[1] and (log[1] != test_db.test_exe_name):
                 msg = 'Test case "%s" is from a different executable file "%s".' % (log[0], log[1])
-                tk_messagebox.showerror(parent=self.tk, message=msg)
+                tk_messagebox.showerror(parent=self.tk_top, message=msg)
                 return False
-            elif test_db.test_case_stats.get(log[0], None) is None:
+
+            if test_db.test_case_stats.get(log[0], None) is None:
                 msg = 'Test case "%s" no longer exists in current executable' % log[0]
                 if log[1] is None:
                     msg += " or may be from a different executable"
-                tk_messagebox.showerror(parent=self.tk, message=msg + ".")
+                tk_messagebox.showerror(parent=self.tk_top, message=msg + ".")
                 return False
 
         return True
 
 
     def do_request_repetition(self, enable_rep):
+        """
+        Add or remove repetition request for currently selected results. This
+        request may originate from internal bindings or the "Repeat" button in
+        the test control widget.
+        """
         sel = self.__get_mapped_selection()
 
         if not sel:
             if test_db.repeat_requests:
                 return True
 
             for idx in self.log_idx_map:
                 log = test_db.test_results[idx]
                 if log[3] == 2 or log[3] == 3:
                     # Silently skip results from other executables or removed test cases
                     if ((not log[1] or (log[1] == test_db.test_exe_name)) and
                             (test_db.test_case_stats.get(log[0], None) is not None)):
                         sel.append(idx)
 
-        if not self.check_tc_names_in_exe(sel):
+        if not self.__check_tc_names_in_exe(sel):
             return False
 
         for log in {test_db.test_results[x] for x in sel}:
             if log[3] <= 3: # exclude valgrind summary error
                 tc_name = log[0]
-                if enable_rep:
-                    test_db.repeat_requests[tc_name] = test_db.test_case_stats[tc_name][4]
-                else:
-                    test_db.repeat_requests.pop(tc_name, None)
-
-                self.update_repetition_status(tc_name)
+                test_db.set_repetition_request(tc_name, enable_rep)
 
         return True
 
 
-    def do_filter_exe_ts(self):
+    def __do_filter_exe_ts(self):
         sel = self.__get_mapped_selection()
         if len(sel) == 1:
             log = test_db.test_results[sel[0]]
 
             self.var_opt_filter_exe_ts.set(True)
             self.__toggle_exe_ts_filter(log[2] + 1)
 
 
-    def do_export_trace(self):
+    def __do_export_trace(self):
         sel = self.__get_mapped_selection()
         if sel:
-            dlg_browser.export_traces(self.tk, sel)
+            dlg_browser.export_traces(self.tk_top, sel)
 
 
-    def do_open_stack_trace(self, tc_name, exe_name, exe_ts, core_name):
-        dlg_browser.show_stack_trace(self.tk, tc_name, exe_name, exe_ts, core_name)
+    def __do_open_stack_trace(self, tc_name, exe_name, exe_ts, core_name):
+        dlg_browser.show_stack_trace(self.tk_top, tc_name, exe_name, exe_ts, core_name)
 
 
-    def do_open_trace_browser(self, complete_trace=False):
+    def __do_open_trace_browser(self, complete_trace=False):
         sel = self.__get_mapped_selection()
         if len(sel) == 1:
             log = test_db.test_results[sel[0]]
             if log[4]:
                 if complete_trace:
-                    dlg_browser.show_trace(self.tk, log[4])
+                    dlg_browser.show_trace(log[4])
                 else:
-                    dlg_browser.show_trace_snippet(self.tk, log[4], log[5], log[6], log[13]==2)
+                    dlg_browser.show_trace_snippet(log[4], log[5], log[6], log[13] == 2)
             else:
-                wid_status_line.show_message("warning", "No trace available for this result")
+                StatusLineWidget.get().show_message("warning", "No trace available for this result")
 
 
-    def show_trace_preview(self, log_idx):
+    def __show_trace_preview(self, log_idx):
         log = test_db.test_results[log_idx]
         if log[4]:
-            txt = gtest.extract_trace(log[4], log[5], log[6])
+            txt = trace_db.extract_trace(log[4], log[5], log[6])
             if txt:
                 self.wid_trace.replace("1.0", "end", txt)
                 self.wid_trace.see("end - 1 lines")
 
                 if log[3] >= 2:
                     line = self.wid_trace.search(": Failure", "1.0")
                     if line:
                         self.wid_trace.see(line + " linestart")
                         self.wid_trace.tag_add("failure", line + " linestart", line + " lineend")
 
             else:
-                self.clear_trace_preview()
+                self.__clear_trace_preview()
         else:
-            self.clear_trace_preview()
+            self.__clear_trace_preview()
 
 
-    def clear_trace_preview(self):
+    def __clear_trace_preview(self):
         self.wid_trace.delete("1.0", "end")
```

### Comparing `mote-gtest-gui-0.8.1/gtest_gui/wid_text_sel.py` & `mote-gtest-gui-0.9.0/gtest_gui/dlg_tc_list.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/env python3
 
-import gtest_gui.tk_utils as tk_utils
-
 # ------------------------------------------------------------------------ #
-# Copyright (C) 2007-2010,2019-2023 Th. Zoerner
+# Copyright (C) 2023 Th. Zoerner
 # ------------------------------------------------------------------------ #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -15,503 +13,528 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # ------------------------------------------------------------------------ #
 
-# This code is copied from Trace Browser (trowser.py)
-#
-# The following class allows using a text widget in the way of a listbox, i.e.
-# allowing to select one or more lines. The mouse bindings are similar to the
-# listbox "extended" mode. The cursor key bindings differ from the listbox, as
-# there is no "active" element (i.e. there's no separate cursor from the
-# selection.)
-#
-# Member variables:
-# - text widget whose selection is managed by the class instance
-# - callback to invoke after selection changes
-# - callback which provides the content list length
-# - ID of "after" event handler while scrolling via mouse, or None
-# - scrolling speed
-# - anchor element index OR last selection cursor pos
-# - list of indices of selected lines (starting at zero)
-#
-class Text_sel_wid(object):
-    #
-    # This constructor is called after a text widget is created for initializing
-    # all member variables and for adding key and mouse event bindings for
-    # handling the selection.
-    #
-    def __init__(self, wid, cb_proc, len_proc, mode="extended"):
-        self.wid = wid
-        self.cb_proc = cb_proc
-        self.len_proc = len_proc
-        self.scroll_tid = None
-        self.scroll_speed = 0
-        self.anchor_idx = -1
-        self.sel = []
-
-        self.wid.bind("<Control-ButtonPress-1>", lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_pick(e.x, e.y)))
-        self.wid.bind("<Shift-ButtonPress-1>", lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_resize(e.x, e.y)))
-        self.wid.bind("<ButtonPress-1>",   lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_button(e.x, e.y)))
-        self.wid.bind("<ButtonRelease-1>", lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_motion_end()))
-        if mode == "browse":
-            self.wid.bind("<B1-Motion>",    lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_button(e.x, e.y)))
-        else:
-            self.wid.bind("<B1-Motion>",    lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_motion(e.x, e.y)))
+"""
+Implements the test case list dialog class.
+"""
+
+from enum import Enum
+import os
+import tkinter as tk
+from tkinter import messagebox as tk_messagebox
+from tkinter import filedialog as tk_filedialog
+
+import gtest_gui.bisect as bisect
+import gtest_gui.config_db as config_db
+import gtest_gui.filter_expr as filter_expr
+import gtest_gui.gtest_ctrl as gtest_ctrl
+import gtest_gui.test_db as test_db
+import gtest_gui.tk_utils as tk_utils
+from gtest_gui.wid_text_sel import TextSelWidget
 
-        self.wid.bind("<Shift-Key-Up>",   lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_key_resize(-1)))
-        self.wid.bind("<Shift-Key-Down>", lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_key_resize(1)))
-        self.wid.bind("<Key-Up>",         lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_key_up_down(-1)))
-        self.wid.bind("<Key-Down>",       lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_key_up_down(1)))
-        self.wid.bind("<Shift-Key-Home>", lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_key_home_end(False, True)))
-        self.wid.bind("<Shift-Key-End>",  lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_key_home_end(True, True)))
-        self.wid.bind("<Key-Home>",       lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_key_home_end(False, False)))
-        self.wid.bind("<Key-End>",        lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_key_home_end(True, False)))
-
-        self.wid.bind("<Control-Key-a>", lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_select_all()))
-        self.wid.bind("<Control-Key-c>", lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.text_sel_copy_clipboard(True)))
-
-        self.wid.bind("<Key-Prior>", lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_key_page_up_down(-1)))
-        self.wid.bind("<Key-Next>",  lambda e, self=self: tk_utils.bind_call_and_break(lambda: self.__text_sel_key_page_up_down(1)))
-
-
-    #
-    # This is an interface function which allows outside users to retrieve a
-    # list of selected elements (i.e. a list of indices)
-    #
-    def text_sel_get_selection(self):
-        return self.sel
-
-
-    #
-    # This is an interface function which allows to modify the selection
-    # externally.
-    #
-    def text_sel_set_selection(self, sel, do_callback=True):
-        if len(sel) > 0:
-            self.anchor_idx = sel[0]
-        self.sel = sel
-
-        self.text_sel_show_selection()
-
-        if do_callback:
-            self.cb_proc(self.sel)
-
-
-    #
-    # This is an interface function which is used by context menus to check
-    # if the item under the mouse pointer is included in the selection.
-    # If not, the selection is set to consist only of the pointed item.
-    #
-    def text_sel_context_selection(self, xcoo, ycoo):
-        line = self.__text_sel_coo2_line(xcoo, ycoo)
-        if line != -1:
-            if len(self.sel) != 0:
-                if not line in self.sel:
-                    # click was outside the current selection -> replace selection
-                    self.text_sel_set_selection([line])
-            else:
-                # nothing selected yet -> select element under the mouse pointer
-                self.text_sel_set_selection([line])
-        else:
-            self.text_sel_set_selection([])
 
+class SortMode(Enum):
+    """ Internal enumeration for sort options selectable by the user. """
+    by_name = 0
+    by_exec_cnt = 1
+    by_fail_cnt = 2
+    by_duration = 3
+
+
+class TcListDialog:
+    """
+    This class implements a test case list dialog window as a singleton. Instances of the class are
+    created via class function create_dialog(), which only creates a new instance if none exists
+    yet. The dialog window shows a list of all test case names extraced from the configured
+    executable. The list can be sorted and filtered via a context menu. Besides the names, the list
+    shows statistics about the current test campaign's results, which are updated continuously.
+    """
+    __prev_dialog_wid = None
+    __prev_export_filename = ""
+
+    @classmethod
+    def create_dialog(cls, tk_top, test_ctrl):
+        """
+        Open the configuration dialog window. If an instance of the dialog
+        already exists, the window is raised, else an instance is created.
+        """
+        if not test_db.test_case_names:
+            tk_messagebox.showerror(parent=tk_top, message="Test case list is empty.")
+            return
 
-    #
-    # This function is bound to button-press events in the text widget while
-    # neither Control nor Shift keys are pressed.  A previous selection is
-    # is cleared and the entry below the mouse (if any) is selected.
-    #
-    def __text_sel_button(self, xcoo, ycoo):
-        line = self.__text_sel_coo2_line(xcoo, ycoo)
-        old_sel = self.sel
-        if (line >= 0) and (line < self.len_proc()):
-            # select the entry under the mouse pointer
-            self.anchor_idx = line
-            self.sel = [line]
-            notify = True
+        if not test_ctrl.check_filter_expression():
+            return
+
+        if cls.__prev_dialog_wid and tk_utils.wid_exists(cls.__prev_dialog_wid.wid_top):
+            cls.__prev_dialog_wid.raise_window()
         else:
-            # mouse pointer is not above a list entry -> clear selection
-            self.sel = []
-            notify = False
-
-        # update display if the selection changed
-        if old_sel != self.sel:
-            self.text_sel_show_selection()
-            notify = True
-
-        # invoke notification callback if an element was selected or de-selected
-        if notify:
-            self.cb_proc(self.sel)
-
-        self.wid.focus_set()
-
-
-    #
-    # This function is bound to mouse pointer motion events in the text widget
-    # while the mouse button is pressed down. This allows changing the extent
-    # of the selection. The originally selected item ("anchor") always remains
-    # selected.  If the pointer is moved above or below the widget borders,
-    # the text is scrolled.
-    #
-    def __text_sel_motion(self, xcoo, ycoo):
-        # the anchor element is the one above which the mouse button was pressed
-        # (the check here is for fail-safety only, should always be fulfilled)
-        if self.anchor_idx >= 0:
-            wh = self.wid.winfo_height()
-            # check if the mouse is still inside of the widget area
-            if (ycoo >= 0) and (ycoo < wh):
-                # identify the item under the mouse pointer
-                line = self.__text_sel_coo2_line(xcoo, ycoo)
-                if line != -1:
-                    # build list of all consecutive indices between the anchor and the mouse position
-                    sel = Text_sel_wid.__idx_range(self.anchor_idx, line)
-                    # update display and invoke notification callback if the selection changed
-                    if sel != self.sel:
-                        self.sel = sel
-                        self.text_sel_show_selection()
-                        self.cb_proc(self.sel)
-
-                # cancel scrolling timer, as the mouse is now back inside the widget
-                if self.scroll_tid is not None:
-                    tk_utils.tk_top.after_cancel(self.scroll_tid)
-                    self.scroll_tid = None
+            cls.__prev_dialog_wid = TcListDialog(tk_top, test_ctrl)
 
-            else:
-                # mouse is outside of the text widget - start scrolling
-                # scrolling speed is determined by how far the mouse is outside
-                fh = tk_utils.tk_top.call("font", "metrics", self.wid.cget("font"), "-linespace")
-                if ycoo < 0:
-                    delta = 0 - ycoo
-                else:
-                    delta = ycoo - wh
 
-                delay = 500 - delta * 100 // fh
-                if (delay > 500): delay = 500
-                if (delay <  50): delay =  50
-                if self.scroll_tid is None:
-                    # start timer and remember it's ID to be able to cancel it later
-                    delta = -1 if (ycoo < 0) else 1
-                    self.scroll_tid = tk_utils.tk_top.after(delay, lambda: self.__text_sel_motion_scroll(delta))
-                    self.scroll_delay = delay
-                else:
-                    # timer already active - just update the delay
-                    self.scroll_delay = delay
+    @classmethod
+    def __destroyed_dialog(cls):
+        cls.__prev_dialog_wid = None
 
 
-    #
-    # This timer event handler is activated when the mouse is moved outside of
-    # the text widget while the mouse button is pressed. The handler re-installs
-    # itself and is only stopped when the button is released or the mouse is
-    # moved back inside the widget area.  The function invariably scrolls the
-    # text by one line. Scrolling speed is varied by means of the delay time.
-    #
-    def __text_sel_motion_scroll(self, delta):
-        # scroll up or down by one line
-        self.wid.yview_scroll(delta, "units")
-
-        # extend the selection to the end of the viewable area
-        if delta < 0:
-            self.__text_sel_motion(0, 0)
-        else:
-            self.__text_sel_motion(0, self.wid.winfo_height() - 1)
+    def __init__(self, tk_top, test_ctrl):
+        self.tk_top = tk_top
+        self.test_ctrl = test_ctrl
+        self.table_header_txt = ("Run", "Name", "Passed", "Failed", "Exec time")
+        self.opt_sort_modes = []
+        self.tc_enabled = []
 
-        # install the timer again (possibly with a changed delay if the mouse was moved)
-        self.scroll_tid = tk_utils.tk_top.after(self.scroll_speed, lambda: self.__text_sel_motion_scroll(delta))
+        self.__create_dialog_window()
+        self.__handle_filter_change()
 
+        test_db.register_slot(test_db.SlotTypes.tc_stats_update, self.__handle_tc_stats_update)
+        test_db.register_slot(test_db.SlotTypes.tc_names_update, self.__handle_tc_names_update)
+        test_db.register_slot(test_db.SlotTypes.campaign_stats_reset,
+                              self.__handle_campaign_status_change)
+        self.test_ctrl.register_filter_change_slot(self.__handle_main_tc_filter_expr_change)
 
-    #
-    # This function is boud to mouse button release events and stops a
-    # possible on-going scrolling timer.
-    #
-    def __text_sel_motion_end(self):
-        if self.scroll_tid is not None:
-            tk_utils.tk_top.after_cancel(self.scroll_tid)
-            self.scroll_tid = None
-
-
-    #
-    # This function is bound to mouse button events while the Control key is
-    # pressed. The item below the mouse pointer is toggled in the selection.
-    # Otherwise the selection is left unchanged.  Note this operation always
-    # clears the "anchor" element, i.e. the selection cannot be modified
-    # using "Shift-Click" afterwards.
-    #
-    def __text_sel_pick(self, xcoo, ycoo):
-        line = self.__text_sel_coo2_line(xcoo, ycoo)
-        if line != -1:
-            # check if the item is already selected
-            try:
-                pick_idx = self.sel.index(line)
-                # already selected -> remove from selection
-                del self.sel[pick_idx]
-            except:
-                pick_idx = -1
-                self.sel.append(line)
-
-            if len(self.sel) <= 1:
-                self.anchor_idx = line
-
-            self.text_sel_show_selection()
-            self.cb_proc(self.sel)
-
-
-    #
-    # This function is bound to mouse button events while the Shift key is
-    # pressed. The selection is changed to cover all items starting at the
-    # anchor item and the item under the mouse pointer.  If no anchor is
-    # defined, the selection is reset and only the item under the mouse is
-    # selected.
-    #
-    def __text_sel_resize(self, xcoo, ycoo):
-        line = self.__text_sel_coo2_line(xcoo, ycoo)
-        if line != -1:
-            if self.anchor_idx != -1:
-                self.sel = Text_sel_wid.__idx_range(self.anchor_idx, line)
-                self.text_sel_show_selection()
-                self.cb_proc(self.sel)
-            else:
-                self.__text_sel_button(xcoo, ycoo)
 
+    def __destroy_window(self):
+        test_db.deregister_slot(test_db.SlotTypes.tc_stats_update)
+        test_db.deregister_slot(test_db.SlotTypes.tc_names_update)
+        test_db.deregister_slot(test_db.SlotTypes.campaign_stats_reset)
 
-    #
-    # This function is bound to the page up/down cursor keys.
-    #
-    def __text_sel_key_page_up_down(self, delta):
-        content_len = self.len_proc()
-        if content_len == 0:
-            return
+        self.test_ctrl.register_filter_change_slot(None)
 
-        if (delta < 0) and (self.wid.bbox("1.0") is not None):
-            self.__text_sel_select_line(0)
+        tk_utils.safe_destroy(self.wid_top)
+        TcListDialog.__destroyed_dialog()
 
-        elif (delta > 0) and (self.wid.bbox("%d.0" % content_len) is not None):
-            self.__text_sel_select_line(content_len - 1)
 
-        else:
-            if self.sel:
-                prev_line = min(self.sel) if delta < 0 else max(self.sel)
-            else:
-                prev_line = -1
+    def raise_window(self):
+        """ Raises the dialog window above all other windows."""
+        self.wid_top.wm_deiconify()
+        self.wid_top.lift()
 
-            self.wid.yview("scroll", delta, "pages")
 
-            line = self.__text_sel_coo2_line(1, self.wid.winfo_height() / 2)
-            if line != -1:
-                if delta < 0 and line > prev_line and prev_line != -1:
-                    line = prev_line
-                if delta > 0 and line < prev_line:
-                    line = prev_line
-
-                # set selection on the new line
-                self.__text_sel_select_line(line)
-
-
-    #
-    # This function is bound to the up/down cursor keys. If no selection
-    # exists, the viewable first item in cursor direction is selected.
-    # If a selection exists, it's cleared and the item next to the
-    # previous selection in cursor direction is selected.
-    #
-    def __text_sel_key_up_down(self, delta):
-        content_len = self.len_proc()
-        if content_len > 0:
-            sel = sorted(self.sel)
-            if len(sel) != 0:
-                # selection already exists -> determine item below or above
-                if delta < 0:
-                    line = sel[0]
-                else:
-                    line = sel[-1]
+    def __create_dialog_window(self):
+        self.wid_top = tk.Toplevel(self.tk_top)
+        self.wid_top.wm_title("GtestGui: Test case list")
+        self.wid_top.wm_group(self.tk_top)
 
-                # determine the newly selected item
-                line += delta
+        self.var_filter_run = tk.BooleanVar(self.tk_top, False)
+        self.var_filter_failed = tk.BooleanVar(self.tk_top, False)
+        self.var_filter_disabled = tk.BooleanVar(self.tk_top, False)
 
-                if (line >= 0) and (line < content_len):
-                    # set selection on the new line
-                    self.__text_sel_select_line(line)
-
-                elif len(sel) > 1:
-                    # selection already includes last line - restrict selection to this single line
-                    if delta < 0:
-                        line = 0
-                    else:
-                        line = content_len - 1
+        self.var_sort_name = tk.BooleanVar(self.tk_top, False)
+        self.var_sort_exec_cnt = tk.BooleanVar(self.tk_top, False)
+        self.var_sort_fail_cnt = tk.BooleanVar(self.tk_top, False)
+        self.var_sort_duration = tk.BooleanVar(self.tk_top, False)
 
-                    self.__text_sel_select_line(line)
+        self.wid_table, self.wid_header = self.__create_table_widget()
+
+        self.wid_table.bind("<Key-Return>", lambda e: self.__do_filter_selected_tests(True))
+        self.wid_table.bind("<Key-Delete>", lambda e: self.__do_filter_selected_tests(False))
+        self.wid_table.bind("<FocusIn>", lambda e: self.test_ctrl.check_filter_expression(False))
+
+        self.wid_top.bind("<ButtonRelease-3>",
+                          lambda e: self.__post_context_menu(e.widget, e.x, e.y))
+        self.wid_top.bind("<Configure>", lambda e: self.__handle_window_resize(e.widget))
+        self.wid_top.bind("<Destroy>", lambda e: self.__destroy_window())
+
+        self.wid_header.tag_configure("head", font=tk_utils.font_content_bold,
+                                      lmargin1=5, spacing1=2, spacing3=5)
+        self.wid_table.tag_configure("body", lmargin1=5)
+        self.wid_table.tag_configure("bold", font=tk_utils.font_content_bold)
+
+        self.wid_header.insert("0.0", "\t".join(self.table_header_txt), "head", "\n", [])
+        self.__update_column_widths()
+
+        self.sel_obj = TextSelWidget(self.wid_table, self.__handle_selection_change, self.__get_len)
+
+        if config_db.get_opt("tc_list_geometry"):
+            self.wid_top.wm_geometry(config_db.get_opt("tc_list_geometry"))
+
+        self.wid_table.focus_set()
+
+
+    def __create_table_widget(self):
+        initial_height = min(40, len(test_db.test_case_names) + 1)
+
+        wid_frm1 = tk.Frame(self.wid_top)
+        wid_frm2 = tk.Frame(wid_frm1, borderwidth=2, relief=tk.SUNKEN)
+        wid_header = tk.Text(wid_frm2, height=1, font=tk_utils.font_content,
+                             insertofftime=0, wrap=tk.NONE, cursor="top_left_arrow",
+                             exportselection=0, relief=tk.FLAT, takefocus=0)
+        wid_table = tk.Text(wid_frm2, height=initial_height, font=tk_utils.font_content,
+                            insertofftime=0, wrap=tk.NONE, cursor="top_left_arrow",
+                            exportselection=0, relief=tk.FLAT)
+        wid_header.pack(side=tk.TOP, fill=tk.X)
+        wid_table.pack(side=tk.TOP, fill=tk.BOTH, expand=1)
+        wid_frm2.pack(side=tk.LEFT, fill=tk.BOTH, expand=1)
+
+        wid_sb = tk.Scrollbar(wid_frm1, orient=tk.VERTICAL, command=wid_table.yview, takefocus=0)
+        wid_table.configure(yscrollcommand=wid_sb.set)
+        wid_sb.pack(side=tk.LEFT, fill=tk.Y)
+        wid_frm1.pack(side=tk.TOP, fill=tk.BOTH, expand=1)
+
+        wid_header.bindtags([wid_header, self.wid_top, "all"])
+        wid_table.bindtags([wid_table, self.wid_top, "TextSel", "all"])
+
+        return (wid_table, wid_header)
 
-            else:
-                # no selection exists yet -> use last anchor, or top/bottom visible line
-                if ((self.anchor_idx >= 0) and
-                    (self.wid.bbox("%d.0" % (self.anchor_idx + 1)) is not None)):
-                    idx = "%d.0" % (self.anchor_idx + 1)
-                else:
-                    if delta > 0:
-                        idx = "@1,1"
-                    else:
-                        idx = "@1,%d" % (self.wid.winfo_height() - 1)
-
-                pos = self.wid.index(idx)
-                if pos != "":
-                    line = int(pos.split(".")[0])
-                    if line > 0:
-                        line -= 1
-                        if line >= content_len:
-                            line = content_len - 1
-                        self.__text_sel_select_line(line)
-
-
-    #
-    # This function is bound to the up/down cursor keys while the Shift key
-    # is pressed. The selection is changed to cover all items starting at the
-    # anchor item and the next item above or below the current selection.
-    #
-    def __text_sel_key_resize(self, delta):
-        content_len = self.len_proc()
-        if len(self.sel) > 0:
-            sel = sorted(self.sel)
-            # decide if we manipulate the upper or lower end of the selection:
-            # use the opposite side of the anchor element
-            if self.anchor_idx == sel[-1]:
-                line = sel[0]
-            else:
-                line = sel[-1]
 
-            line += delta
-            if (line >= 0) and (line < content_len):
-                self.sel = Text_sel_wid.__idx_range(self.anchor_idx, line)
-
-                self.text_sel_show_selection()
-                self.wid.see("%d.0" % (line + 1))
-                self.cb_proc(self.sel)
+    def __update_column_widths(self):
+        char_w = tk_utils.font_content.measure("0")
+        if char_w == 0:
+            char_w = 15
 
+        title_text = self.table_header_txt
+        tab_widths = [tk_utils.font_content_bold.measure(x) + 2*char_w for x in title_text]
+
+        tc_max_width = max([tk_utils.font_content.measure(x)
+                            for x in test_db.test_case_names]) + 2*char_w
+        if tc_max_width > tab_widths[1]:
+            tab_widths[1] = tc_max_width
+
+        tabs = [char_w + tab_widths[0], "left"]
+        off = tab_widths[0] + tab_widths[1]
+        for width in tab_widths[2:]:
+            tabs.extend([off + width/2, "center"])
+            off += width
+
+        self.wid_header.tag_configure("head", font=tk_utils.font_content_bold, tabs=tabs,
+                                      lmargin1=5, spacing1=2, spacing3=5)
+        self.wid_table.tag_configure("body", tabs=tabs, lmargin1=5)
+
+        # Convert pixel width to a character count (assuming "0" has average char width)
+        nof_chars = (off + char_w - 1) // char_w
+
+        self.wid_header.configure(width=nof_chars)
+        self.wid_table.configure(width=nof_chars)
+
+
+    def __handle_window_resize(self, wid):
+        if wid == self.wid_top:
+            new_size = self.wid_top.wm_geometry()
+            config_db.set_opt("tc_list_geometry", new_size)
+
+
+    def __format_table_row(self, tc_name):
+        tc_stats = test_db.test_case_stats[tc_name]
+
+        ena = "yes\t" if tc_name in self.tc_enabled else "no\t"
+        txt = [ena + tc_name, "body"]
+
+        nof_pass = tc_stats[0]
+        if nof_pass > 0:
+            txt.extend(["\t%d" % nof_pass, ["body", "bold"]])
         else:
-            self.__text_sel_key_up_down(delta)
+            txt.extend(["\t%d" % nof_pass, "body"])
 
+        nof_fail = tc_stats[1]
+        if nof_fail > 0:
+            txt.extend(["\t%d" % nof_fail, ["body", "bold"]])
+        else:
+            txt.extend(["\t%d" % nof_fail, "body"])
 
-    #
-    # This function is bound to the "Home" and "End" keys.  While the Shift
-    # key is not pressed, the first or last element in the list are selected.
-    # If the Shift key is pressed, the selection is extended to include all
-    # items between the anchor and the first or last item.
-    #
-    def __text_sel_key_home_end(self, is_end, is_resize):
-        content_len = self.len_proc()
-        if content_len > 0:
-            if is_end:
-                line = content_len - 1
-            else:
-                line = 0
+        duration = tc_stats[3] / 1000 # FP result
+        if duration < 10:
+            duration = "\t%.3f" % duration
+        elif duration < 3600:
+            duration = "\t%02d:%02d" % (duration/60, duration%60)
+        else:
+            duration = "\t%d:%02d:%02d" % (duration/3600, (duration/60)%60, duration%60)
+        txt.extend([duration + "\n", "body"])
 
-            if not is_resize:
-                self.anchor_idx = line
-                self.sel = [line]
-            else:
-                if self.anchor_idx >= 0:
-                    self.sel = Text_sel_wid.__idx_range(self.anchor_idx, line)
+        return txt
 
-            self.text_sel_show_selection()
-            self.wid.see("%d.0" % (line + 1))
-            self.cb_proc(self.sel)
-
-
-    #
-    # This function is bound to the "CTRL-A" key to select all entries in
-    # the list.
-    #
-    def __text_sel_select_all(self):
-        content_len = self.len_proc()
-        if content_len > 0:
-            self.sel = Text_sel_wid.__idx_range(0, content_len - 1)
-
-            self.text_sel_show_selection()
-            self.cb_proc(self.sel)
-
-
-    #
-    # This helper function is used to build a list of all indices between
-    # (and including) two given values in increasing order.
-    #
-    def __idx_range(start, end):
-        if start > end:
-            return list(range(end, start + 1))
+
+    def __handle_tc_stats_update(self, tc_name):
+        try:
+            line_idx = self.tc_list_sorted.index(tc_name)
+        except ValueError:
+            line_idx = None
+
+        if line_idx is None:
+            if self.__matches_filter(tc_name):
+                line_idx = bisect.bisect_left(self.tc_list_sorted, tc_name,
+                                              self.__get_sort_key_fn())
+                self.__insert_single(tc_name, line_idx)
         else:
-            return list(range(start, end + 1))
+            if self.__matches_filter(tc_name):
+                if self.__check_sort_order(tc_name, line_idx):
+                    self.__replace_single(tc_name, line_idx)
+                else:
+                    self.__delete_single(line_idx)
+                    line_idx = bisect.bisect_left(self.tc_list_sorted, tc_name,
+                                                  self.__get_sort_key_fn())
+                    self.__insert_single(tc_name, line_idx)
+            else:
+                self.__delete_single(line_idx)
+
 
+    def __replace_single(self, tc_name, line_idx):
+        txt = self.__format_table_row(tc_name)
+        self.wid_table.replace("%d.0" % (line_idx + 1), "%d.0" % (line_idx + 2), *txt)
+        self.sel_obj.text_sel_show_selection()
 
-    #
-    # This interface function displays a selection in the text widget by adding
-    # the "sel" tag to all selected lines. (Note the view is not affected, i.e.
-    # the selection may be outside of the viewable area.)
-    #
-    def text_sel_show_selection(self):
-        # first remove any existing highlight
-        self.wid.tag_remove("sel", "1.0", "end")
-
-        # select each selected line (may be non-consecutive)
-        for line in self.sel:
-            self.wid.tag_add("sel", "%d.0" % (line + 1), "%d.0" % (line + 2))
 
-        if (len(self.sel) == 0) or (self.anchor_idx == -1):
-            self.wid.mark_set("insert", "end")
+    def __insert_single(self, tc_name, line_idx):
+        txt = self.__format_table_row(tc_name)
+        self.wid_table.insert("%d.0" % (line_idx + 1), *txt)
+
+        self.tc_list_sorted.insert(line_idx, tc_name)
+        self.sel_obj.text_sel_adjust_insert(line_idx)
+
+
+    def __delete_single(self, line_idx):
+        line_1 = "%d.0" % (line_idx + 1)
+        line_2 = "%d.0" % (line_idx + 2)
+        self.wid_table.delete(line_1, line_2)
+
+        del self.tc_list_sorted[line_idx]
+        self.sel_obj.text_sel_adjust_deletion(line_idx)
+
+
+    def __populate_table(self):
+        self.wid_table.delete("1.0", "end")
+        for tc_name in self.tc_list_sorted:
+            txt = self.__format_table_row(tc_name)
+            self.wid_table.insert("end", *txt)
+
+        self.sel_obj.text_sel_set_selection([])
+
+
+    def __refill_table(self):
+        prev_yview = self.wid_table.yview()[0]
+        prev_sel = self.sel_obj.text_sel_get_selection()
+
+        self.__populate_table()
+
+        self.wid_table.yview_moveto(prev_yview)
+        self.sel_obj.text_sel_set_selection(prev_sel)
+
+
+    def __handle_campaign_status_change(self):
+        for tc_name in test_db.test_case_names:
+            self.__handle_tc_stats_update(tc_name)
+
+
+    def __handle_main_tc_filter_expr_change(self, expr):
+        self.tc_enabled = expr.get_selected_tests()
+
+        if self.var_filter_run.get():
+            self.__handle_filter_change()
         else:
-            self.wid.mark_set("insert", "%d.0" % (self.anchor_idx + 1))
+            self.__refill_table()
 
 
-    #
-    # This function changes the selection to the single given line.
-    #
-    def __text_sel_select_line(self, line):
-        self.anchor_idx = line
-        self.sel = [line]
-
-        self.text_sel_show_selection()
-        self.wid.see("%d.0" % (line + 1))
-        self.cb_proc(self.sel)
-
-
-    #
-    # This function determines the line under the mouse pointer.
-    # If the pointer is not above a content line, -1 is returned.
-    #
-    def __text_sel_coo2_line(self, xcoo, ycoo):
-        pos = self.wid.index("@%d,%d" % (xcoo,ycoo))
-        if pos != "":
-            line = int(pos.split(".")[0]) - 1
-            if (line >= 0) and (line < self.len_proc()):
-                return line
-        return -1
-
-
-    #
-    # This function has to be called when an item has been inserted into the
-    # list to adapt the selection: Indices following the insertion are
-    # incremented.  The new element is not included in the selection.
-    #
-    def text_sel_adjust_insert(self, line):
-        self.sel = [(x if x < line else x+1) for x in self.sel]
-
-        if self.anchor_idx >= line:
-            self.anchor_idx += 1
-
-
-    #
-    # This function has to be called when an item has been deleted from the
-    # list (asynchronously, i.e. not via a command related to the selection)
-    # to adapt the list of selected lines: The deleted line is removed from
-    # the selection (if included) and following indices are decremented.
-    #
-    def text_sel_adjust_deletion(self, line):
-        self.sel = [(x if x < line else x-1) for x in self.sel if x != line]
-
-        if self.anchor_idx > line:
-            self.anchor_idx -= 1
-
-    #
-    # This handler is bound to CTRL-C in the selection and performs <<Copy>>
-    # (i.e. copies the content of all selected lines to the clipboard.)
-    #
-    def text_sel_copy_clipboard(self, to_clipboard):
-        msg = "".join([self.wid.get("%d.0" % (line + 1), "%d.0" % (line + 2)) for line in self.sel])
-        tk_utils.xselection_export(msg, to_clipboard)
+    def __handle_tc_names_update(self):
+        self.__update_column_widths()
+        self.__handle_filter_change()
+
+
+    def __handle_filter_change(self):
+        self.tc_enabled = self.test_ctrl.get_test_filter_expr().get_selected_tests()
+
+        tc_list = [x for x in test_db.test_case_names if self.__matches_filter(x)]
+
+        self.tc_list_sorted = self.__sort_tc_list(tc_list)
+        self.__populate_table()
+
+
+    def __matches_filter(self, tc_name):
+        tc_stats = test_db.test_case_stats[tc_name]
+        return ((not self.var_filter_run.get() or tc_name in self.tc_enabled) and
+                (not self.var_filter_failed.get() or tc_stats[1]) and
+                (not self.var_filter_disabled.get()
+                 or not filter_expr.is_disabled_by_name(tc_name)))
+
+
+    def __get_sort_key_fn(self):
+        if not self.opt_sort_modes:
+            return lambda x: x
+
+        return lambda x: TcListDialog.__get_sort_keys(self.opt_sort_modes, x)
+
+
+    @staticmethod
+    def __get_sort_keys(opt_sort_modes, tc_name):
+        keys = []
+        for mode in opt_sort_modes:
+            if mode == SortMode.by_name:
+                keys.append(tc_name)
+
+            elif mode == SortMode.by_exec_cnt:
+                keys.append(0 - test_db.test_case_stats[tc_name][0]
+                            - test_db.test_case_stats[tc_name][1]
+                            - test_db.test_case_stats[tc_name][2])
+
+            elif mode == SortMode.by_fail_cnt:
+                keys.append(0 - test_db.test_case_stats[tc_name][1])
+
+            elif mode == SortMode.by_duration:
+                keys.append(0 - test_db.test_case_stats[tc_name][3])
+        return keys
+
+
+    def __sort_tc_list(self, tc_list):
+        for mode in reversed(self.opt_sort_modes):
+            if mode == SortMode.by_name:
+                tc_list = sorted(tc_list)
+            elif mode == SortMode.by_exec_cnt:
+                tc_list = sorted(tc_list, key=lambda x:
+                                 0 - test_db.test_case_stats[x][0]
+                                 - test_db.test_case_stats[x][1]
+                                 - test_db.test_case_stats[x][2])
+            elif mode == SortMode.by_fail_cnt:
+                tc_list = sorted(tc_list, key=lambda x: 0 - test_db.test_case_stats[x][1])
+            elif mode == SortMode.by_duration:
+                tc_list = sorted(tc_list, key=lambda x: 0 - test_db.test_case_stats[x][3])
+        return tc_list
+
+
+    def __check_sort_order(self, tc_name, line_idx):
+        if self.opt_sort_modes:
+            if line_idx > 0:
+                prev_name = self.tc_list_sorted[line_idx - 1]
+                if (TcListDialog.__get_sort_keys(self.opt_sort_modes, tc_name)
+                        < TcListDialog.__get_sort_keys(self.opt_sort_modes, prev_name)):
+                    return False
+
+            if line_idx + 1 < len(self.tc_list_sorted):
+                next_name = self.tc_list_sorted[line_idx + 1]
+                if (TcListDialog.__get_sort_keys(self.opt_sort_modes, next_name)
+                        < TcListDialog.__get_sort_keys(self.opt_sort_modes, tc_name)):
+                    return False
+
+        return True
+
+
+    def __get_len(self):
+        return len(self.tc_list_sorted)
+
+
+    def __handle_selection_change(self, sel):
+        # abstract interface: unused parameter needed by other classes
+        # pylint: disable=unused-argument
+        self.sel_obj.text_sel_copy_clipboard(False)
+
+
+    def __get_mapped_selection(self):
+        sel = self.sel_obj.text_sel_get_selection()
+        return [self.tc_list_sorted[x] for x in sel]
+
+
+    def __post_context_menu(self, parent, xcoo, ycoo):
+        wid_men = tk_utils.get_context_menu_widget()
+
+        if (parent == self.wid_table) and not gtest_ctrl.gtest_ctrl.is_active():
+            self.sel_obj.text_sel_context_selection(xcoo, ycoo)
+            expr = self.test_ctrl.get_test_filter_expr()
+
+            sel = self.__get_mapped_selection()
+            if not expr.run_disabled():
+                sel = [x for x in sel if not filter_expr.is_disabled_by_name(x)]
+
+            if sel:
+                plural_s = "" if len(sel) == 1 else "s"
+                need_sep = False
+
+                if any(expr.can_select_test(x) for x in sel):
+                    wid_men.add_command(label="Add selected test case%s to filter" % plural_s,
+                                        command=lambda: self.test_ctrl.select_tcs(sel, True))
+                    need_sep = True
+                if any(expr.can_deselect_test(x) for x in sel):
+                    wid_men.add_command(label="Remove selected test case%s from filter" % plural_s,
+                                        command=lambda: self.test_ctrl.select_tcs(sel, False))
+                    need_sep = True
+
+                all_tc_names = filter_expr.get_test_list(expr.run_disabled())
+                tc_names = []
+                for tc_suite in filter_expr.get_test_suite_names(sel):
+                    tc_names.extend(filter_expr.get_tests_in_test_suite(tc_suite, all_tc_names))
+
+                if any(expr.can_select_test(x) for x in tc_names):
+                    wid_men.add_command(label="Add selected test suites to filter",
+                                        command=lambda: self.test_ctrl.select_tcs(tc_names, True))
+                    need_sep = True
+                if any(expr.can_deselect_test(x) for x in tc_names):
+                    wid_men.add_command(label="Remove selected test suites from filter",
+                                        command=lambda: self.test_ctrl.select_tcs(tc_names, False))
+                    need_sep = True
+
+                if need_sep:
+                    wid_men.add_separator()
+
+        wid_men.add_checkbutton(label="Show only tests enabled to run",
+                                command=self.__handle_filter_change,
+                                variable=self.var_filter_run)
+        wid_men.add_checkbutton(label="Show only failed tests",
+                                command=self.__handle_filter_change,
+                                variable=self.var_filter_failed)
+        wid_men.add_checkbutton(label="Show no DISABLED tests",
+                                command=self.__handle_filter_change,
+                                variable=self.var_filter_disabled)
+        wid_men.add_separator()
+
+        wid_men.add_checkbutton(
+            label="Sort by test case name",
+            command=lambda: self.__do_toggle_sort_mode(self.var_sort_name.get(), SortMode.by_name),
+            variable=self.var_sort_name)
+        wid_men.add_checkbutton(
+            label="Sort by execution count",
+            command=lambda: self.__do_toggle_sort_mode(self.var_sort_exec_cnt.get(),
+                                                       SortMode.by_exec_cnt),
+            variable=self.var_sort_exec_cnt)
+        wid_men.add_checkbutton(
+            label="Sort by failure count",
+            command=lambda: self.__do_toggle_sort_mode(self.var_sort_fail_cnt.get(),
+                                                       SortMode.by_fail_cnt),
+            variable=self.var_sort_fail_cnt)
+        wid_men.add_checkbutton(
+            label="Sort by duration",
+            command=lambda: self.__do_toggle_sort_mode(self.var_sort_duration.get(),
+                                                       SortMode.by_duration),
+            variable=self.var_sort_duration)
+        wid_men.add_separator()
+
+        wid_men.add_command(label="Export list to file...", command=self.__do_export_pass_fail)
+        wid_men.add_command(label="Close window", command=self.__destroy_window)
+
+        tk_utils.post_context_menu(parent, xcoo, ycoo)
+
+
+    def __do_export_pass_fail(self):
+        filename = tk_filedialog.asksaveasfilename(
+                        parent=self.wid_top,
+                        filetypes=[("all", "*"), ("Text", "*.txt")],
+                        title="Select output file",
+                        initialfile=os.path.basename(TcListDialog.__prev_export_filename),
+                        initialdir=os.path.dirname(TcListDialog.__prev_export_filename))
+        if filename:
+            TcListDialog.__prev_export_filename = filename
+            try:
+                with open(filename, "w") as file_obj:
+                    for tc_name in self.tc_list_sorted:
+                        tc_stats = test_db.test_case_stats[tc_name]
+                        txt = "%s\t%d\t%d\t%d" % (tc_name, tc_stats[0], tc_stats[1], tc_stats[2])
+                        print(txt, file=file_obj)
+
+            except OSError as exc:
+                tk_messagebox.showerror(parent=self.wid_top,
+                                        message="Error writing to file: %s" % str(exc))
+
+
+    def __do_toggle_sort_mode(self, enable, mode):
+        self.opt_sort_modes = [x for x in self.opt_sort_modes if x != mode]
+        if enable:
+            self.opt_sort_modes.append(mode)
+        self.__handle_filter_change()
+
+
+    def __do_filter_selected_tests(self, enable):
+        sel = self.__get_mapped_selection()
+        if len(sel) != 0:
+            expr = self.test_ctrl.get_test_filter_expr()
+            if enable and not expr.run_disabled():
+                sel = [x for x in sel if not filter_expr.is_disabled_by_name(x)]
+
+            self.test_ctrl.select_tcs(sel, enable)
```

### Comparing `mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/PKG-INFO` & `mote-gtest-gui-0.9.0/mote_gtest_gui.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mote-gtest-gui
-Version: 0.8.1
+Version: 0.9.0
 Summary: Module tester's Gtest GUI is a full-featured graphical user-interface to C++ test applications using the GoogleTest framework.
 Home-page: https://github.com/tomzox/gtest_gui
 Author: T. Zoerner
 Author-email: tomzox@gmail.com
 License: UNKNOWN
 Keywords: google-test,gtest,testing-tools,test-runners,tkinter,GUI
 Platform: posix
@@ -23,40 +23,53 @@
 
 Module-Tester's Gtest GUI
 =========================
 
 Description
 -----------
 
-**Module-tester's GtestGui** is a full-featured graphical user-interface to C++ test applications using the GoogleTest framework.
+**Module-tester's GtestGui** is a test-runner with graphical user-interface for C++ test applications using the GoogleTest framework.
 
-The tool will work with any application with Gtest command line interface, however it is designed especially for C++ developers using test-driven design based on module testing and integration testing. These differ from unit-testing by longer execution times and usually not fully predictable results, which in turn require multiple repetitions of each test case. To support this well, GtestGui offers firstly easily accessible ways for test case filtering and concurrent scheduling across multiple CPUs; Secondly, there are multiple features for tracking progress and managing results via sorting and filtering, which are fully usable already while a test campaign still is in progress.
+GtestGui will work with any application that implements the Gtest command line interface, however it is designed especially for C++ developers using test-driven design based on module testing and integration testing. These differ from unit-testing by longer execution times and usually not fully predictable results (i.e. "flakiness"), which in turn require multiple repetitions of each test case. To support this well, GtestGui offers firstly easily accessible ways for test case filtering and concurrent scheduling across multiple CPUs; Secondly, there are multiple features for tracking progress and managing results via sorting and filtering, which are fully usable already while a test campaign still is in progress.
 
 GtestGui typically is started with the path of an executable on the command line which is built using the gtest library. Using the "Run" button in the GUI, this executable can then be started and its progress be monitored live in the result log frame of the main window. Additional controls allow specifying options such as test case filter string and repetition count, which are forwarded to the executable via the respective "\ ``--gtest_*``" command line arguments.
 
 While tests are running, test verdicts can be monitored live in the result log. Traces of passed or failed tests can already be analyzed simply by double-clicking on an entry in the result log, which will open the trace of that particular test case run. For this purpose GtestGui comes bundled with *Trowser*, which is a graphical browser for large line-oriented text files. Trowser in principle is just a text browser with syntax highlighting and search, but its search capabilities are designed especially to facilitate analysis of complex debug logs, essentially by allowing to build a condensed (filtered) view of the trace file in the search result window via incremental searches and manual manipulations. By default, GtestGui is configured to user *trowser.py*, but there is also a more modern-looking Qt5 variant. GtestGui can also be configured to use any other GUI application for opening traces.
 
 Test control
 ------------
 
 The application main window consists of a menu bar, a frame containing test controls, a frame containing the test result log, and a text frame for trace preview. This chapter describes the top-most frame with the test controls.
 
+Executable selection
+~~~~~~~~~~~~~~~~~~~~
+
+Before tests can be started or a test filter be defined, a target executable has to be selected. If the executable file was not already specified on the command line, then this is done via *Select executable file...* in the *Control* menu. Either select a file via the file selector dialog, or choose one from the list of previously used executables. (Note when hovering the mouse over enries in this list, the full path and timestamp of the file is displayed as tool-tip. The entry is grayed out if the file no longer exists.)
+
+Upon selecting an executable file, the test case list is read automatocally by running it with the "\ ``--gtest_list_tests``" command line option. If that fails with an error, or if the list is empty, executable selection is aborted.
+
+Whenever starting a new test campaign, GtestGui will automatically check if a new executable version is available by checking the file timestamp. If a change is detected, the test case list is read again. The *Refresh test case list* command in the menu allows performing the same steps independently. That command is useful if you want to specify newly added test case names in the test case filter string before starting a new test campaign (maybe to only run the new test cases.)
+
+Results of the previous executable are kept in the result log window, but the log entries are updated to include the executable name. Repeating test cases of other executables via the *Repeat* button is not possible; You have to manually switch back to the respective executable to allow that.
+
+The executable cannot be "refreshed" or switched while a test campaign is running.
+
 Test campaign control buttons
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Most prominent in the test control frame are the green buttons, which directly control execution of the configured executable file:
+Most prominent in the test control frame are the green buttons, which directly control execution of the configured executable file. The same commands are also in the "Control" menu:
 
 *Run*:
   Starts the text executable in a separate process, with its output redirected into a pipe which is read by GtestGui for progress monitoring. The output is also saved into a file.
 
-  Note when the timestamp of the executable file on disk has changed, GtestGui automatically reads the test case list to check for changes. An error will be reported if the current test case filter contains pattern that no longer match any test case. Note after adding a new test case, use the *Refresh test case list* command in the *Control* menu to read the test case list, for allowing to use the new test case name in a filter pattern.
+  Note when the timestamp of the executable file on disk has changed, GtestGui automatically reads the test case list to check for changes. An error will be reported if the current test case filter contains pattern that no longer match any test case. If the timestamp has not changed, the age of the file is shown in a status message below the buttons, to warn you about this in case you forget to build the executable after making changes.
 
   Multiple processes are started if the *CPUs* value is larger than 1. Most of the time, GtestGui will use gtest's "sharding" feature, which assigns a static sub-set of tests to each process. However, if repetition count is larger than one and the number of configured CPUs is larger than the number of test cases, or if the remainder of division of test cases by CPUs is large, GtestGui may instead or additionally partition by repetitions.
 
-  Note when a test process crashes, it is currently not restarted. That is because gtest's static sharding does not allow disabling the instable test case without influencing test case partitioning.
+  Note when a test process crashes during a campaign, it is currently not restarted. That is because gtest's static sharding does not allow disabling the instable test case without influencing test case partitioning.
 
 *Stop*:
   Sends a TERM signal to the test processes and waits for them to finish. When termination takes a long time (possibly because the executable is hung) and the button is clicked a second time, a KILL signal is sent.
 
 *Resume*:
   Restarts test case execution using the same test case filter setting and executable version as previously used, without resetting the test result statistics. Other options, such as repetition or CPU count may be modified. This operation is useful when a long test run has to be paused temporarily as the CPUs are needed otherwise, or for changing options such as the number of used CPUs.
 
@@ -72,14 +85,16 @@
 
 The entry field at the top of the test control frame allows specifying a test case filter, so that only a matching sub-set of test cases is run. The filter can be entered manually using the same syntax as the "\ ``--gtest-filter``" command line option: The format of a filter expression is a ":"-separated list of test case names of wildcard patterns (positive patterns), optionally followed by a "-" and another ":"-separated pattern list (negative patterns). A test matches the filter if and only if it matches any of the positive patterns, but none of the negative ones. Wildcard characters are "*" (matching any sub-string) and "?" (matching any single character). As a special case, when no positive pattern is specified, all test cases are considered matching.
 
 Alternatively, the test case filter can be modified via the drop-down menu below the entry field (which can be opened by the Cursor-Down key or a click on the drop-down button next to the entry field). The menu has entries for selecting and deselecting entries test suites as well as individual test cases. When modifying the filter this way, GtestGui will update the entry field with the shortest filter expression it can find using trailing wild card and negative patterns.
 
 Yet another alternative for modifying test case filters is the test case list dialog, either via its context menu or the "Return" and "Delete" key bindings. Finally note any modification to the test case filter can be undone using "Control-Z" key binding in the entry field, or redone using "Control-Y" key binding.
 
+After renaming a test case or adding a new test case, use the *Refresh test case list* command in the *Control* menu to read the test case list from the executable file. Afterward the new test case names can be used in the filter string.
+
 Test control options
 ~~~~~~~~~~~~~~~~~~~~
 
 *Repetitions*:
   If a value larger than 1 is entered here, it is passed via the "\ ``--gtest_repeat=NNN``" option on the executable's command line. This causes each test case to be repeated the given number of times.
 
 *CPUs*:
@@ -118,14 +133,34 @@
   When enabled, "\ ``--gtest_catch_exceptions=0``" option is set via the executable's command line. This will disable catching of exceptions by the Gtest framework, which means any exception not caught by the test case itself causes the test process to crash due to an unhandled exception.
 
   When core dumps are enabled in the kernel, the core will be saved by GtestGui and can be analyzed via the *Extract stack trace from core dump* command in the result log's context menu. When core dumps are not enabled, this option is probably not useful.
 
 *Valgrind* and *Valgrind - 2nd option set*:
   The two valgrind options serve to run each execution of the test executable under valgrind using the configured command line. Notably, valgrind checks are performed across the complete lifetime of the test process, thus spanning all test cases or test repetitions. Therefore, if for example a memory leak is reported at the end, it cannot be determined which test case caused it (or it may even be caused by interaction of the test sequence.) Therefore valgrind errors are reported with a special entry in the result log. Some kind of errors such as invalid memory accesses can be mapped to test cases based on the position of the error report in the output stream. Note however that the position may not exactly reflect the timing of occurrence due to possible buffering in output streams within the test executable.) See `Result log`_ and `Configuration`_ for more details.
 
+Status and progress monitoring
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The lower left part of the test control frame shows the status of the latest test campaign. The left box with label "Status" shows three numbers with the following meaning:
+
+*Running*:
+  Shows the number of test processes currently executing test cases. (See `Caveats`_ for an explanation why this number may be lower than the number of requested "CPUs".)
+
+*Passed*:
+  Shows the number of test cases that were passed or skipped.
+
+*Failed*:
+  Shows the number of test cases that failed or crashed. The number also includes a possible additional fail verdict by valgrind at the end of a test process.
+
+The left box with label "Progress" shows the completion ratio in form of a progress bar. The ratio is calculated as the number of received results (i.e. passed, skipped, failed, or crashed) divided by the number of expected results. The number of expected results is the number of test cases selected by the test case filter, multiplied with the repetition count.
+
+In case the *Ignore filter* option in `Test control options`_ is set to a non-zero value, completion ratio of the respective test jobs is disregarded for the progress display, as these jobs are terminated automatically once the regular test jobs have completed. Note the "Status" frame however does include results received from these jobs, so that the numbers shown there may exceed the configured repetition count for tests matching the test case filter.
+
+When hovering the mouse over the progress bar, a tool-tip text shows additional details about the progress, namely the ratio of completed test cases and repetitions and estimated remaining run time.
+
 Result log
 ----------
 
 The result log frame is located in the middle of the main window. When started for the first time, the log is usually empty. However, results can also be imported via the command line, for example from a file that contains output from a test executable that was redirected into a file. The result log may also show results from a previous run of GtestGui, if auto-import is enabled in `Configuration`_.
 
 The result log contains one line for each ``[ OK ]``, ``[ SKIPPED ]`` and ``[ FAILED ]`` line in the test application's gtest-generated output. The test executable's output stream is redirected to a pipe that is read continuously by GtestGui for this purpose. GtestGui also stores this output to a file, so that the trace output between ``[ RUN ]`` and verdict text line can be opened in a trace browser.
 
@@ -147,19 +182,66 @@
 
 -   In case of failure, source code file and line where of the first "Failure" was reported in trace output.
 
 -   Timestamp or name of executable that generated the test output, in case the executable has changed since running the test.
 
 When selecting an entry by clicking on it, the corresponding trace output is shown in the trace preview frame below the result log. In case of a test case failure, the view is centered on the first line containing "Failure" and the text is marked by light red background.
 
-When clicking on an entry with the right mouse button, a context menu opens that allow opening the trace file, adding or removing the selected test case from the filter option, scheduling a test for repetition, excluding a result from the log display, or removing results.
+Double-clicking on an entry opens the trace of that entry in an external application, which can be selected via the Configuration dialog. Default application is "trace browser", a text browser with syntax highlighting and search and filtering capabilities especially tailored for trace analysis. As GTest writes trace output of all test cases into a single file, only the portion between "\ ``[ RUN ]``" and "\ ``[ OK ]``" or "\ ``[ FAILED ]``" respectively of the selected test case is extracted and passed to the application.
+
+When clicking on an entry with the right mouse button, a context menu opens that allow opening the trace file, adding or removing the selected test case from the filter option, scheduling a test for repetition, excluding a result from the log display, or removing results. The context menu also has an entry for sending the complete trace file to the external trace browser application; This may be needed in rare cases when behavior of a test case depends on the sequence of preceding tests.
+
+Additional commands are offered in the "Result log" drop-down of the main window menu. The commands allow sorting and filtering the result log by various criteria. By default, log entries are sorted by the time they were created at. When running a test campaign, it's recommended to enabled the *Show only failed* filter, so that it's easy to track which test cases failed.
+
+While a test campaign is running, new result entries are added at the bottom (when in default sort order) and the view is scrolled automatically to keep the added entry visible. This auto-scrolling can be stopped by selecting any entry in the list. To return to auto-scrolling, deselect the last entry either by clicking on it while holding the *Control* key, or by clicking in the empty line at the end of the list.
+
+Result entries can be deleted using the context menu or by pressing the *Delete* key. To delete all entries, press *Control-A* (i.e. select complete list) and then *Delete*. Note actual trace files are removed from disk only if all test case results stored in it have been deleted from the log.
 
-Additional commands are offered in the "Result log" drop-down of the main window menu. The commands allow sorting and filtering the result log by various criteria.
+Post-mortem core dump analysis
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-On UNIX platform, the context menu additionally supports extracting a thread overview and stack-trace (backtrace) of each thread from a core dump in case of a crash during execution of a test case. To allow this, ``/proc/sys/kernel/core_pattern`` needs to be configured as "\ ``core.%p``", or alternatively as "\ ``core``", when additionally ``/proc/sys/kernel/core_uses_pid`` is set to "1". If GtestGui thus finds a file named "core.PID" with PID matching that of the test executable process after a process crashed, it will automatically preserve that core file for analysis by renaming it and moving it into the directory where trace text output files are stored. It will also preserve the executable file version by keeping a hard link to the same executable.
+POSIX platforms only: When selecting the result of a test case that caused a crash of the test process, the context menu has an entry that allows analyzing the generated core dump file. The Analysis consists of a thread overview and stack-trace (backtrace) of each thread. This allows finding quickly at which test step the crash occurred.
+
+To allow this, ``/proc/sys/kernel/core_pattern`` needs to be configured as "\ ``core.%p``", or alternatively as "\ ``core``", when additionally ``/proc/sys/kernel/core_uses_pid`` is set to "1". This way, a file named "\ ``core.PID``" will be created by the operating system in the directory where GtestGui was started.
+
+If GtestGui thus finds a core file with a matching process ID after a process crashed, it will automatically preserve that core file for analysis by moving it into the directory where trace text output files are stored and renaming it to the same name of the corresponding trace file with prefix "core". It will also preserve the executable file version by keeping a hard link to the same executable in the trace directory for as long as the core file exists.
+
+Test case list dialog
+---------------------
+
+A dialog showing the list of test cases read from the selected executable file can be opened via the control menu.
+
+For each test case, the list shows in the first column if the test case is currently enabled for execution, the test case name, the number of times it has passed and failed in the current campaign and its accumulated execution time.
+
+By default, test cases in the list are in the order as received. The list can be sorted in different ways using the context menu: The list can be sorted alpabetically, by execution or failure count within the current test campaign, or by test case execution duration.
+
+By default, all test cases defined in the executable are listed. You can filter the list via the context menu to show only test cases enabled via test case filter in the main window, or only test cases that failed in the current test campaign, or only test cases whose name or test suite namedoesn't start with "\ ``DISABLED_``".
+
+The "Run" column is updated to reflect changes in the "Test filter" entry field in the main window. Updates occur when you press the "Return" key, or when keyboard focus is moved out of the entry field. When the "Show only tests enabled to run" filter is active in the test case list dialog, the test case sub-set shown in the list is also updated to match the current filter string. This feature can be used for testing the manually entered filter string against the list, as you'll see exactly which test cases it selects.
+
+Inversely, you can use the list for modifying the test case filter in the main window: This can be done via the *Add/Remove selected test case* and *Add/Remove selected test suite* commands in the list's context menu. The latter works on all test cases in the test suite of the selected test case. The same can be achive via key bindings: *Return* adds selected test cases and *Del* removes selected test cases. Note for selecting multiple lines in the list via keyboard, hold the *Shift* button while moving the cursor via the Up/Down keys.
+
+Test cases named "\ ``DISABLED_``" can only be enabled via the test case list commands when option *Run disabled tests* in the main window is checked.
+
+Note while the filter string is empty, all test cases are considered as enabled.  Nevertheless, the context menu will offer adding selected test cases. If you do so, then implictly all test cases except for the one added by the command get disabled.
+
+After making changes to the test case filter via the dialog, the filter string in the main window is updated automatically to reflect the selection. The filter uses wildcards to minimize the filter string length.
+
+Job list dialog
+---------------
+
+A dialog window showing the status of test processes in a currently ongoing test campaign can be opened via the *Open job list* command in the control menu. If no test campaign is active, it will only show a message informing that currently no processes are running.
+
+During an ongoing test campaign, the list shows for each process its ID assigned by the operating system ("PID"), if it is a background job ("BgJob"), the number of bytes of trace output received from it ("Traced"), the number of test case results found in received trace ("Results"), the percentage of completed results from expected results ("Done"), and finally the name of the current test case reported via "\ ``[ RUN ]``" in received trace.
+
+Note a "background job" is one for which the test case filter is ignored as per *Ignore filter* option in `Test control options`_. These jobs are special as they are terminated automatically when the last regular job is completed. For this reason their completion ratio (i.e. "Done" column) is disregarded for progress display in the main window.
+
+The dialog is useful in case you suspect that a test campaign may be hung (for example when a test case ran into a deadlock or busy loop.) You could notice that firstly by the number of results not increasing and if that's the case, by the number of received bytes received as trace output not increasing. (The latter will however not if your test cases generate few or no trace output.)
+
+The context menu allows sending an *ABORT* signal to the process, which will terminate it and cause a core image to be dumped on UNIX. The test case will be reported as crashed in the result log. This can be used for debugging a hung process: You can find where it was hung by using the *Extract stack trace from core dump* command in context menu of the result log entry. Alternatively, you could use the PID for attaching a debugger to the live process (e.g. "\ ``gdb -p PID exe_file``").
 
 Configuration
 -------------
 
 User-interface options
 ~~~~~~~~~~~~~~~~~~~~~~
 
@@ -176,14 +258,16 @@
 
 *Show tool-tip popups*:
   The option can be unchecked to disable display of "tool-tip" popup windows when hovering with the mouse on labels or check-buttons in the main window and dialogs which have such built-in help. Changes of the option are stored in the configuration file, so that it is persistent. This may be useful once you are sufficiently familiar with the tool.
 
 Test management options
 ~~~~~~~~~~~~~~~~~~~~~~~
 
+The following configuration options are available in the *Options* dialog window that can be opened via the *Configure* menu:
+
 *Trace browser*
   This entry field selects the external application used for displaying trace files and trace snippets, when double-clicking on an entry in the result log. By default, trace browser *trowser.py* is used. You can either specify just the application file name, or its full path if it is not found via ``PATH`` configured in environment. The path of the trace file to be displayed will be appended to the given command line.
 
   Currently the application path name or parameters cannot contain space characters, as these are assumed to be separators.
 
   Note for the Windows platform: When using the default of ``trowser.py``, you may need to insert the Python interpreter in front of "trowser.py", depending on your Python installation. In that case you need to add the full path to where ``trowser.py`` is installed.
 
@@ -218,19 +302,19 @@
 
 Caveats
 -------
 
 This chapter lists notable limitations that are not easy to overcome due to design choices.
 
 Concurrent scheduling
-  Concurrent scheduling requested via option *CPUs* is based on the "sharding" feature provided by Gtest framework. Unfortunately, Gtest only supports static case test partitioning, which means for example when using two CPUs, the set of test cases is split in two parts, of which the first is executed in one test process and the second in the second process.
+  Concurrent scheduling requested via option *CPUs* is based on the "sharding" feature provided by Gtest framework. Unfortunately, Gtest only supports static case test partitioning, which means for example when using two CPUs, the set of test cases is split in two parts, of which the first is executed in one test process and the second in the other process.
 
-  One problem arises when the number of test cases is smaller than the number of CPUs. This typically occurs, when trying to run a single test case many times. Sharding would then only use a single CPU, as it does not consider repetitions in its "sharding" algorithm. GtestGui works around that by calculating if it is more efficient to partition test cases by repetition than by sharding, or if a combination of both is even better. In the mentioned example, it would not use sharding, but instead run half the number of repetitions in one process, and the second half in the second. For more complex configurations such as 10 repetitions of 9 test cases on 8 CPUs, a combination of both methods will be used.
+  One problem arises when the number of test cases is smaller than the number of requested CPUs. This typically occurs when trying to run a single test case many times.  Sharding would then only use a single CPU, as it does not consider repetitions in its "sharding" algorithm. GtestGui works around that by calculating if it is more efficient to partition test cases by repetition than by sharding, or if a combination of both is even better. In the mentioned example, it would not use sharding, but instead run half the number of repetitions in one process, and the second half in the second. For more complex configurations such as 10 repetitions of 9 test cases on 8 CPUs, a combination of both methods will be used.
 
-  A second problem that GtestGui cannot work around occurs when test cases have non-uniform execution time. As the "sharding" algorithm uses static partitioning solely based on the number of test cases per process, differences in execution times are not considered. For example, when two tests are scheduled for 100 times and test case A takes 1 second, but test case B only 1 millisecond, Gtest will still schedule all runs of A in the first process and all runs of B in the second process. Thus, the second process will sit idle for 99.9% of the total test execution time.
+  A second problem, that GtestGui cannot work around, occurs when test cases have non-uniform execution time. As the "sharding" algorithm uses static partitioning solely based on the number of test cases per process, differences in execution times are not considered. For example, when two tests are scheduled for 100 times and test case A takes 1 second, but test case B only 1 millisecond, Gtest will still schedule all runs of A in the first process and all runs of B in the second process. Thus, the second process will sit idle for 99.9% of the total test execution time.
 
 Test case crashes
   In a well-behaved test application, failures are normally reported via Gtest macros or exceptions. Thus, the failure is recorded and the next test case is executed. Sometimes however, a test case may have a bug that leads to a crash of the complete process. In this case all following test cases or test case repetitions are no longer executed.
 
   Currently GtestGui will not attempt to restart tests after a crash, because it expects that the same test case will crash again and thus keep blocking following tests. It is not possible to disable the instable test, as this would interfere with partitioning by Gtest "sharding", i.e. the set of test cases run by that test case would be altered. The only way around is for the use to manually disable the instable test case and then restart the test campaign.
 
 Overload of GUI by concurrent unit-testing
```

### Comparing `mote-gtest-gui-0.8.1/mote_gtest_gui.egg-info/SOURCES.txt` & `mote-gtest-gui-0.9.0/mote_gtest_gui.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,20 +14,23 @@
 gtest_gui/dlg_font_sel.py
 gtest_gui/dlg_help.py
 gtest_gui/dlg_job_list.py
 gtest_gui/dlg_main.py
 gtest_gui/dlg_tc_list.py
 gtest_gui/fcntl.py
 gtest_gui/filter_expr.py
-gtest_gui/gtest.py
+gtest_gui/gtest_ctrl.py
+gtest_gui/gtest_list_tests.py
+gtest_gui/gtest_sharding.py
 gtest_gui/help_db.py
 gtest_gui/main.py
 gtest_gui/test_db.py
 gtest_gui/tk_utils.py
 gtest_gui/tool_tip_db.py
+gtest_gui/trace_db.py
 gtest_gui/wid_status_line.py
 gtest_gui/wid_test_ctrl.py
 gtest_gui/wid_test_log.py
 gtest_gui/wid_text_sel.py
 gtest_gui/wid_tool_tip.py
 mote_gtest_gui.egg-info/PKG-INFO
 mote_gtest_gui.egg-info/SOURCES.txt
```

### Comparing `mote-gtest-gui-0.8.1/setup.py` & `mote-gtest-gui-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,19 +11,20 @@
                               stdout=subprocess.PIPE, text=True, check=True)
     long_description = proc_rst.stdout
 else:
     long_description = None
 
 setup(
     name='mote-gtest-gui',
-    version='0.8.1',
+    version='0.9.0',
     packages=['gtest_gui'],
     scripts=['bin/gtest_gui'],
 
-    install_requires=['trowser'],
+    install_requires=['trowser',
+                      'appdirs ; platform_system=="Windows"'],
 
     author='T. Zoerner',
     author_email='tomzox@gmail.com',
 
     url='https://github.com/tomzox/gtest_gui',
 
     description="Module tester's Gtest GUI is a full-featured graphical user-interface " \
```

