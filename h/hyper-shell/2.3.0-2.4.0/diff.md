# Comparing `tmp/hyper-shell-2.3.0.tar.gz` & `tmp/hyper-shell-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyper-shell-2.3.0.tar", last modified: Thu Apr 13 15:55:39 2023, max compression
+gzip compressed data, was "hyper-shell-2.4.0.tar", last modified: Thu Jun  8 21:00:08 2023, max compression
```

## Comparing `hyper-shell-2.3.0.tar` & `hyper-shell-2.4.0.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.763179 hyper-shell-2.3.0/
--rw-r--r--   0 geoffrey   (501) staff       (20)    11357 2020-12-21 02:22:57.000000 hyper-shell-2.3.0/LICENSE
--rw-r--r--   0 geoffrey   (501) staff       (20)     3771 2023-04-13 15:55:39.762696 hyper-shell-2.3.0/PKG-INFO
--rw-r--r--   0 geoffrey   (501) staff       (20)     2883 2023-04-02 14:55:21.000000 hyper-shell-2.3.0/README.rst
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.740072 hyper-shell-2.3.0/man/
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.743531 hyper-shell-2.3.0/man/man1/
--rw-r--r--   0 geoffrey   (501) staff       (20)    50674 2023-04-13 15:55:03.000000 hyper-shell-2.3.0/man/man1/hyper-shell.1
--rw-r--r--   0 geoffrey   (501) staff       (20)      100 2022-01-10 02:23:40.000000 hyper-shell-2.3.0/pyproject.toml
--rw-r--r--   0 geoffrey   (501) staff       (20)       38 2023-04-13 15:55:39.763324 hyper-shell-2.3.0/setup.cfg
--rw-r--r--   0 geoffrey   (501) staff       (20)     2652 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/setup.py
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.740878 hyper-shell-2.3.0/src/
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.746119 hyper-shell-2.3.0/src/hyper_shell.egg-info/
--rw-r--r--   0 geoffrey   (501) staff       (20)     3771 2023-04-13 15:55:39.000000 hyper-shell-2.3.0/src/hyper_shell.egg-info/PKG-INFO
--rw-r--r--   0 geoffrey   (501) staff       (20)      975 2023-04-13 15:55:39.000000 hyper-shell-2.3.0/src/hyper_shell.egg-info/SOURCES.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)        1 2023-04-13 15:55:39.000000 hyper-shell-2.3.0/src/hyper_shell.egg-info/dependency_links.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)       48 2023-04-13 15:55:39.000000 hyper-shell-2.3.0/src/hyper_shell.egg-info/entry_points.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)      132 2023-04-13 15:55:39.000000 hyper-shell-2.3.0/src/hyper_shell.egg-info/requires.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)       11 2023-04-13 15:55:39.000000 hyper-shell-2.3.0/src/hyper_shell.egg-info/top_level.txt
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.749046 hyper-shell-2.3.0/src/hypershell/
--rw-r--r--   0 geoffrey   (501) staff       (20)     3577 2023-04-13 15:55:03.000000 hyper-shell-2.3.0/src/hypershell/__init__.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    34622 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/client.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    25277 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/cluster.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    11691 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/config.py
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.759991 hyper-shell-2.3.0/src/hypershell/core/
--rw-r--r--   0 geoffrey   (501) staff       (20)      132 2023-04-02 14:55:21.000000 hyper-shell-2.3.0/src/hypershell/core/__init__.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     5835 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/ansi.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     9053 2023-04-02 14:55:21.000000 hyper-shell-2.3.0/src/hypershell/core/config.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     4771 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/exceptions.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     1833 2023-04-02 14:55:21.000000 hyper-shell-2.3.0/src/hypershell/core/fsm.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     1892 2023-04-02 14:55:21.000000 hyper-shell-2.3.0/src/hypershell/core/heartbeat.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     6009 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/logging.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     2869 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/platform.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     5347 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/queue.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     6733 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/remote.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     7244 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/template.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     1597 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/thread.py
--rw-r--r--   0 geoffrey   (501) staff       (20)      793 2023-04-02 14:55:21.000000 hyper-shell-2.3.0/src/hypershell/core/types.py
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.761845 hyper-shell-2.3.0/src/hypershell/database/
--rw-r--r--   0 geoffrey   (501) staff       (20)     4615 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/database/__init__.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     7873 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/database/core.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    14166 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/database/model.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    36057 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/server.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    21890 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/submit.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    25736 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/task.py
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.783147 hyper-shell-2.4.0/
+-rw-r--r--   0 geoffrey   (501) staff       (20)    11357 2020-12-21 02:22:57.000000 hyper-shell-2.4.0/LICENSE
+-rw-r--r--   0 geoffrey   (501) staff       (20)     3771 2023-06-08 21:00:08.783044 hyper-shell-2.4.0/PKG-INFO
+-rw-r--r--   0 geoffrey   (501) staff       (20)     2883 2023-04-02 14:55:21.000000 hyper-shell-2.4.0/README.rst
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.778245 hyper-shell-2.4.0/man/
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.779183 hyper-shell-2.4.0/man/man1/
+-rw-r--r--   0 geoffrey   (501) staff       (20)    63611 2023-06-08 20:56:49.000000 hyper-shell-2.4.0/man/man1/hyper-shell.1
+-rw-r--r--   0 geoffrey   (501) staff       (20)      100 2022-01-10 02:23:40.000000 hyper-shell-2.4.0/pyproject.toml
+-rw-r--r--   0 geoffrey   (501) staff       (20)       38 2023-06-08 21:00:08.783178 hyper-shell-2.4.0/setup.cfg
+-rw-r--r--   0 geoffrey   (501) staff       (20)     2652 2023-04-13 15:30:41.000000 hyper-shell-2.4.0/setup.py
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.778416 hyper-shell-2.4.0/src/
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.779886 hyper-shell-2.4.0/src/hyper_shell.egg-info/
+-rw-r--r--   0 geoffrey   (501) staff       (20)     3771 2023-06-08 21:00:08.000000 hyper-shell-2.4.0/src/hyper_shell.egg-info/PKG-INFO
+-rw-r--r--   0 geoffrey   (501) staff       (20)     1067 2023-06-08 21:00:08.000000 hyper-shell-2.4.0/src/hyper_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)        1 2023-06-08 21:00:08.000000 hyper-shell-2.4.0/src/hyper_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)       48 2023-06-08 21:00:08.000000 hyper-shell-2.4.0/src/hyper_shell.egg-info/entry_points.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)      132 2023-06-08 21:00:08.000000 hyper-shell-2.4.0/src/hyper_shell.egg-info/requires.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)       11 2023-06-08 21:00:08.000000 hyper-shell-2.4.0/src/hyper_shell.egg-info/top_level.txt
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.780580 hyper-shell-2.4.0/src/hypershell/
+-rw-r--r--   0 geoffrey   (501) staff       (20)     3573 2023-06-08 20:56:49.000000 hyper-shell-2.4.0/src/hypershell/__init__.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)    39835 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/client.py
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.781066 hyper-shell-2.4.0/src/hypershell/cluster/
+-rw-r--r--   0 geoffrey   (501) staff       (20)    18282 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/cluster/__init__.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     3460 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/cluster/local.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)    18159 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/cluster/remote.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     8520 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/cluster/ssh.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)    11715 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/config.py
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.782575 hyper-shell-2.4.0/src/hypershell/core/
+-rw-r--r--   0 geoffrey   (501) staff       (20)      118 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/core/__init__.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     5906 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/core/ansi.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     9811 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/core/config.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     5087 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/core/exceptions.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     2010 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/core/fsm.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     1964 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/core/heartbeat.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     6373 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/core/logging.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     2952 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/core/platform.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     5347 2023-04-13 15:30:41.000000 hyper-shell-2.4.0/src/hypershell/core/queue.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     6733 2023-04-13 15:30:41.000000 hyper-shell-2.4.0/src/hypershell/core/remote.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     7244 2023-04-13 15:30:41.000000 hyper-shell-2.4.0/src/hypershell/core/template.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     1597 2023-04-13 15:30:41.000000 hyper-shell-2.4.0/src/hypershell/core/thread.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)      793 2023-04-02 14:55:21.000000 hyper-shell-2.4.0/src/hypershell/core/types.py
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.782880 hyper-shell-2.4.0/src/hypershell/data/
+-rw-r--r--   0 geoffrey   (501) staff       (20)     4611 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/data/__init__.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     7873 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/data/core.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)    20916 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/data/model.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)    36448 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/server.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)    22576 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/submit.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)    31601 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/task.py
```

### Comparing `hyper-shell-2.3.0/LICENSE` & `hyper-shell-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyper-shell-2.3.0/PKG-INFO` & `hyper-shell-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyper-shell
-Version: 2.3.0
+Version: 2.4.0
 Summary: Process shell commands over a distributed, asynchronous queue.
 Home-page: https://github.com/glentner/hyper-shell
 Author: Geoffrey Lentner
 Author-email: glentner@purdue.edu
 License: Apache Software License
 Keywords: distributed-computing command-line-tool shell-scripting high-performance-computing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hyper-shell-2.3.0/README.rst` & `hyper-shell-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `hyper-shell-2.3.0/man/man1/hyper-shell.1` & `hyper-shell-2.4.0/man/man1/hyper-shell.1`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "HYPER-SHELL" "1" "Apr 13, 2023" "2.3.0" "hyper-shell"
+.TH "HYPER-SHELL" "1" "Jun 08, 2023" "2.4.0" "hyper-shell"
 .SH NAME
 hyper-shell \- Process shell commands over a distributed, asynchronous queue
 .SH SYNOPSIS
 .nf
 hyper\-shell [\-h] [\-v] ...
 .fi
 .sp
@@ -72,33 +72,35 @@
 This can function as a pure in\-memory queue; however, one can configure a database in\-the\-loop
 to manage task scheduling and persistence. Stand up the \fBserver\fP on its own and persistent
 \fBclients\fP on the nodes in the cluster, and \fBsubmit\fP tasks independently.
 .SH CLUSTER USAGE
 .INDENT 0.0
 .TP
 .B \fBhyper\-shell cluster [\-h]\fP
-\fB[FILE | \-\-restart | \-\-forever]\fP
-\fB[\-N NUM]\fP \fB[\-t CMD]\fP \fB[\-b SIZE]\fP \fB[\-w SEC]\fP \fB[\-p PORT]\fP
-\fB[\-r NUM [\-\-eager]]\fP \fB[\-f PATH]\fP \fB[\-\-capture | [\-o PATH] [\-e PATH]]\fP
+\fB[\-p PORT]\fP \fB[\-r NUM [\-\-eager]]\fP \fB[\-f PATH]\fP \fB[\-\-capture | [\-o PATH] [\-e PATH]]\fP
+\fB[\-\-no\-db | \-\-initdb]\fP \fB[\-\-no\-confirm]\fP \fB[\-\-delay\-start SEC]\fP \fB[\-T SEC]\fP \fB[\-W SEC]\fP
 \fB[\-\-ssh [HOST... | \-\-ssh\-group NAME] [\-\-env] | \-\-mpi | \-\-launcher=ARGS...]\fP
-\fB[\-\-no\-db | \-\-initdb]\fP \fB[\-\-no\-confirm]\fP \fB[\-\-delay\-start SEC]\fP
+\fB[\-\-autoscaling [MODE] [\-P SEC] [\-F VALUE] [\-I NUM] [\-X NUM] [\-Y NUM]]\fP
 .UNINDENT
 .sp
-Start the cluster either locally or with remote clients over \fIssh\fP or a custom \fIlauncher\fP\&. This
-mode should be the most common entry\-point for general usage. It fully encompasses all of the
+Start the cluster either locally or with remote clients with \fIssh\fP or a custom \fIlauncher\fP\&.
+This mode should be the most common entry\-point for general usage. It fully encompasses all of the
 different agents in the system in a concise workflow.
 .sp
 The input source for tasks is file\-like, either a local path, or from \fIstdin\fP if no argument is
 given. The command\-line tasks are pulled in and either directly published to a distributed queue
 (see \fB\-\-no\-db\fP) or committed to a database first before being scheduled later.
 .sp
 For large, long running workflows, it might be a good idea to configure a database and run an
 initial \fBsubmit\fP job to populate the database, and then run the cluster with \fB\-\-restart\fP and no
 input \fIFILE\fP\&. If the cluster is interrupted for whatever reason it can gracefully restart where it
 left off.
+.sp
+Use \fB\-\-autoscaling\fP with either \fIfixed\fP or \fIdynamic\fP to run a persistent, elastically scalable
+cluster using an external \fB\-\-launcher\fP to bring up clients as needed.
 .SS Arguments
 .INDENT 0.0
 .TP
 .B FILE
 Path to input task file (default: <stdin>).
 .UNINDENT
 .SS Modes
@@ -278,14 +280,100 @@
 .TP
 .B \fB\-f\fP, \fB\-\-failures\fP \fIPATH\fP
 File path to write failed task args (default: <none>).
 .sp
 The \fIserver\fP acts like a sieve, reading task args from \fIstdin\fP and redirecting those original
 args to \fIstdout\fP if the task had a non\-zero exit status. The \fIcluster\fP will run the \fIserver\fP
 for you and if \fB\-\-failures\fP is enabled these task args will be sent to a local file \fIPATH\fP\&.
+.TP
+.B \fB\-\-timeout\fP \fISEC\fP
+Timeout in seconds for clients. Automatically shutdown if no tasks received (default: never).
+.sp
+This option is only valid for an \fB\-\-autoscaling\fP cluster. This feature allows for gracefully
+scaling down a cluster when task throughput subsides.
+.TP
+.B \fB\-\-task\-timeout\fP \fISEC\fP
+Task\-level walltime limit (default: none).
+.sp
+Executors will send a progression of SIGINT, SIGTERM, and SIGKILL.
+If the process still persists the executor itself will shutdown.
+.TP
+.B \fB\-A\fP, \fB\-\-autoscaling\fP [\fIMODE\fP]
+Enable autoscaling (default: disabled). Used with \fB\-\-launcher\fP\&.
+.sp
+Specifying this option on its own triggers the use of the autoscaler, with the default
+\fIpolicy\fP or the configured policy. The \fIpolicy\fP can be specified directly here
+as either \fIfixed\fP or \fIdynamic\fP (e.g., \fB\-\-autoscaling=dynamic\fP). The default is \fIfixed\fP\&.
+.sp
+The specified \fB\-\-launcher\fP is used to bring up each individual instance of the client
+as a discrete scaling unit. This is different than using \fB\-\-launcher\fP on its own where
+it specifies a single invocation that should launch all clients (e.g., like an \fBmpirun\fP).
+Without this option, clients will simply be run locally.
+.sp
+A \fIfixed\fP policy will seek to maintain a definite size and allows for recovery in the
+event that clients halt for some reason (e.g., due to expected faults or timeouts).
+.sp
+A \fIdynamic\fP policy maintains a \fB\-\-min\-size\fP (default: 0) and grows up to some
+\fB\-\-max\-size\fP depending on the observed \fItask pressure\fP given the specified scaling
+\fB\-\-factor\fP\&.
+.sp
+See also \fB\-\-factor\fP, \fB\-\-period\fP, \fB\-\-init\-size\fP, \fB\-\-min\-size\fP, and \fB\-\-max\-size\fP\&.
+.TP
+.B \fB\-F\fP, \fB\-\-factor\fP \fIVALUE\fP
+Scaling factor (default: 1).
+.sp
+A configurable, dimensionless quantity used by the \fB\-\-autoscaling=dynamic\fP policy.
+This value expresses some multiple of the average task duration in seconds.
+.sp
+The autoscaler periodically checks \fBtoc / (factor x avg_duration)\fP, where
+\fBtoc\fP is the estimated time of completion for all remaining tasks given current
+throughput of active clients. This ratio is referred to as \fItask pressure\fP, and if
+it exceeds 1, the pressure is considered \fIhigh\fP and we will add another client if
+we are not already at the given \fB\-\-max\-size\fP of the cluster.
+.sp
+For example, if the average task length is 30 minutes, and we set \fB\-\-factor=2\fP, then if
+the estimated time of completion of remaining tasks given currently connected executors
+exceeds 1 hour, we will scale up by one unit.
+.sp
+See also \fB\-\-period\fP\&.  Only valid with \fB\-\-autoscaling\fP\&.
+.TP
+.B \fB\-P\fP, \fB\-\-period\fP \fISEC\fP
+Scaling period in seconds (default: 60).
+.sp
+The autoscaler waits for this period of time in between checks and scaling events.
+A shorter period makes the scaling behavior more responsive but can effect database
+performance if checks happen too rapidly.
+.sp
+Only valid with \fB\-\-autoscaling\fP\&.
+.TP
+.B \fB\-I\fP, \fB\-\-init\-size\fP \fISIZE\fP
+Initial size of cluster (default: 1).
+.sp
+When the cluster starts, this number of clients will be launched.
+For a \fIfixed\fP policy cluster, this should be given with a \fB\-\-min\-size\fP, and likely
+the same value.
+.sp
+Only valid with \fB\-\-autoscaling\fP\&.
+.TP
+.B \fB\-X\fP, \fB\-\-min\-size\fP \fISIZE\fP
+Minimum size of cluster (default: 0).
+.sp
+Regardless of autoscaling policy, if the number of launched clients drops below this
+value we will scale up by one. Allowing \fB\-\-min\-size=0\fP is an important feature for
+efficient use of computing resources in the absence of tasks.
+.sp
+Only valid with \fB\-\-autoscaling\fP\&.
+.TP
+.B \fB\-Y\fP, \fB\-\-max\-size\fP \fISIZE\fP
+Maximum size of cluster (default: 2).
+.sp
+For a \fIdynamic\fP autoscaling policy, this sets an upper limit on the number of launched
+clients. When this number is reached, scaling stops regardless of task pressure.
+.sp
+Only valid with \fB\-\-autoscaling\fP\&.
 .UNINDENT
 .SH SERVER USAGE
 .INDENT 0.0
 .TP
 .B \fBhyper\-shell\fP \fBserver\fP \fB[\-h]\fP
 \fB[FILE | \-\-forever | \-\-restart]\fP \fB[\-b NUM]\fP \fB[\-w SEC]\fP \fB[\-r NUM [\-\-eager]]\fP
 \fB[\-H ADDR]\fP \fB[\-p PORT]\fP \fB[\-k KEY]\fP \fB[\-\-no\-db | \-\-initdb]\fP \fB[\-\-print | \-f PATH]\fP
@@ -293,15 +381,15 @@
 .UNINDENT
 .sp
 Launch server, schedule directly or asynchronously from database.
 .sp
 The server includes a scheduler component that pulls tasks from the database and offers
 them up on a distributed queue to clients. It also has a receiver that collects the results
 of finished tasks. Optionally, the server can submit tasks (\fIFILE\fP). When submitting tasks,
-the \fB\-w\fP/\fB\-\-bundlewait\fP and \fB\-b\fP/\fBbundlesize\fP options are the same as for the
+the \fB\-w\fP/\fB\-\-bundlewait\fP and \fB\-b\fP/\fB\-\-bundlesize\fP options are the same as for the
 \fIsubmit\fP workflow.
 .sp
 With \fB\-\-max\-retries\fP greater than zero, the scheduler will check for a non\-zero exit status
 for tasks and re\-submit them if their previous number of attempts is less.
 .sp
 Tasks are bundled and clients pull them in these bundles. However, by default the bundle size
 is one, meaning that at small scales there is greater concurrency.
@@ -428,17 +516,17 @@
 .sp
 Mutually exclusive to \fB\-\-print\fP\&.
 .UNINDENT
 .SH CLIENT USAGE
 .INDENT 0.0
 .TP
 .B \fBhyper\-shell\fP \fBclient\fP \fB[\-h]\fP
-\fB[\-N NUM]\fP \fB[\-t CMD]\fP \fB[\-b SIZE]\fP \fB[\-w SEC]\fP \fB[\-d SEC]\fP
-\fB[\-H ADDR]\fP \fB[\-p PORT]\fP \fB[\-k KEY]\fP \fB[\-c | [\-o PATH] [\-e PATH]]\fP
-\fB[\-\-no\-confirm]\fP \fB[\-\-delay\-start SEC]\fP
+\fB[\-N NUM]\fP \fB[\-t TEMPLATE]\fP \fB[\-b SIZE]\fP \fB[\-w SEC]\fP \fB[\-H ADDR]\fP \fB[\-p PORT]\fP
+\fB[\-k KEY]\fP \fB[\-\-capture | [\-o PATH] [\-e PATH]]\fP \fB[\-\-no\-confirm]\fP
+\fB[\-\-delay\-start SEC]\fP \fB[\-\-timeout SEC]\fP \fB[\-\-task\-timeout SEC]\fP
 .UNINDENT
 .sp
 Launch client directly, run tasks in parallel.
 .sp
 The client connects to the server and pulls bundles of tasks off the shared queue.
 These tasks are run locally by some number of a parallel task executors.
 .sp
@@ -524,30 +612,43 @@
 tasks need to manage their own output, you can specify a redirect as part of a \fB\-\-template\fP,
 or use \fB\-\-capture\fP to capture these as \fB\&.out\fP and \fB\&.err\fP files.
 .sp
 These are stored local to the \fIclient\fP under \fI<prefix>/lib/task/<uuid>.[out,err]\fP\&.
 Task outputs can be automatically retrieved via SFTP, see \fItask\fP usage.
 .sp
 Mutually exclusive with both \fB\-\-output\fP and \fB\-\-errors\fP\&.
+.TP
+.B \fB\-\-timeout\fP \fISEC\fP
+Timeout in seconds for client. Automatically shutdown if no tasks received (default: never).
+.sp
+This feature allows for gracefully scaling down a cluster when task throughput subsides.
+.TP
+.B \fB\-\-task\-timeout\fP \fISEC\fP
+Task\-level walltime limit (default: none).
+.sp
+Executors will send a progression of SIGINT, SIGTERM, and SIGKILL.
+If the process still persists the executor itself will shutdown.
 .UNINDENT
 .SH SUBMIT USAGE
 .INDENT 0.0
 .TP
 .B \fBhyper\-shell\fP \fBsubmit\fP \fB[\-h]\fP
 \fB[FILE]\fP \fB[\-b NUM]\fP \fB[\-w SEC]\fP \fB[\-t CMD]\fP \fB[\-\-initdb]\fP
+\fB[\-\-tag TAG [TAG...]]\fP
 .UNINDENT
 .sp
 Submit tasks from a file.
 .sp
 Tasks are accumulated and published in bundles to the database.
 The \fB\-b\fP/\fB\-\-bundlesize\fP and \fB\-w\fP/\fB\-\-bundlewait\fP options control the
 size of these bundles and how long to wait before flushing tasks regardless of
 how many have accumulated.
 .sp
 Pre\-format tasks at \fIsubmit\fP\-time with template expansion using \fB\-t\fP/\fB\-\-template\fP\&.
+Any tags specified with \fB\-\-tag\fP are applied to all tasks submitted.
 .SS Arguments
 .INDENT 0.0
 .TP
 .B FILE
 Path to input task file (default: <stdin>).
 .UNINDENT
 .SS Options
@@ -585,14 +686,22 @@
 Auto\-initialize database.
 .sp
 If a database is configured for use with the workflow (e.g., PostgreSQL), auto\-initialize
 tables if they don\(aqt already exist. This is a short\-hand for pre\-creating tables with the
 \fBhyper\-shell initdb\fP command. This happens by default with SQLite databases.
 .sp
 See \fBhyper\-shell initdb\fP command.
+.TP
+.B \fB\-\-tag\fP \fITAG\fP\&...
+Assign one or more tags
+.sp
+Tags allow for user\-defined tracking of information related to individual tasks or large
+groups of tasks. They are defined with both a \fIkey\fP and \fIvalue\fP (e.g., \fB\-\-tag file:a\fP).
+The default \fIvalue\fP for tags is blank. When searching with tags, not specifying a \fIvalue\fP
+will return any task with that \fIkey\fP defined regardless of \fIvalue\fP (including blank).
 .UNINDENT
 .SH INITDB USAGE
 .sp
 \fBhyper\-shell\fP \fBinitdb\fP \fB[\-h]\fP \fB[\-\-truncate [\-\-yes]]\fP
 .sp
 Initialize database.
 .sp
@@ -702,15 +811,15 @@
 .INDENT 0.0
 .TP
 .B SECTION[...].VAR
 Path to variable.
 .UNINDENT
 .SH TASK SUBMIT USAGE
 .sp
-\fBhyper\-shell\fP \fBtask\fP \fBsubmit\fP \fB[\-h]\fP \fBARGS...\fP
+\fBhyper\-shell\fP \fBtask\fP \fBsubmit\fP \fB[\-h]\fP \fB[\-t TAG [TAG...]]\fP \fBARGS...\fP
 .sp
 Submit individual task to the database.
 .sp
 A database must be configured. The task will not run until scheduled
 by the server process. The task UUID will be printed to standard out.
 .sp
 See \fBtask info\fP command.
@@ -719,19 +828,30 @@
 .TP
 .B ARGS...
 Command\-line arguments.
 .sp
 The full command\-line for some shell task.
 To use options, preface with leading \fB\-\-\fP\&.
 .UNINDENT
+.SS Options
+.INDENT 0.0
+.TP
+.B \fB\-t\fP, \fB\-\-tag\fP \fITAG\fP\&...
+Assign one or more tags
+.sp
+Tags allow for user\-defined tracking of information related to individual tasks or large
+groups of tasks. They are defined with both a \fIkey\fP and \fIvalue\fP (e.g., \fB\-\-tag file:a\fP).
+The default \fIvalue\fP for tags is blank. When searching with tags, not specifying a \fIvalue\fP
+will return any task with that \fIkey\fP defined regardless of \fIvalue\fP (including blank).
+.UNINDENT
 .SH TASK INFO USAGE
 .INDENT 0.0
 .TP
 .B \fBhyper\-shell\fP \fBtask\fP \fBinfo\fP \fB[\-h]\fP
-\fBID\fP \fB[\-\-yaml | \-\-json | \-\-stdout | \-\-stderr | \-\-x FIELD]\fP
+\fBID\fP \fB[\-\-stdout | \-\-stderr | \-x FIELD]\fP \fB[\-f FORMAT]\fP
 .UNINDENT
 .sp
 Get metadata and/or task outputs.
 .sp
 Query for the full metadata on task by ID.
 Extract a specific field using \fB\-x\fP/\fB\-\-extract\fP\&.
 .sp
@@ -743,34 +863,37 @@
 .TP
 .B ID
 Unique task UUID.
 .UNINDENT
 .SS Options
 .INDENT 0.0
 .TP
-.B \fB\-\-yaml\fP
-Format metadata output as YAML.
+.B \fB\-f\fP, \fB\-\-format\fP \fIFORMAT\fP
+Format task info ([normal], json, yaml).
 .TP
 .B \fB\-\-json\fP
 Format metadata output as JSON.
 .TP
+.B \fB\-\-yaml\fP
+Format metadata output as YAML.
+.TP
 .B \fB\-x\fP/\fB\-\-extract\fP \fIFIELD\fP
 Print this field only (e.g., \fB\-x submit_time\fP).
 .TP
 .B \fB\-\-stdout\fP
 Print <stdout> of task if captured, fetch from client if necessary.
 .TP
 .B \fB\-\-stderr\fP
 Print <stderr> of task if captured, fetch from client if necessary.
 .UNINDENT
 .SH TASK WAIT USAGE
 .INDENT 0.0
 .TP
 .B \fBhyper\-shell\fP \fBtask\fP \fBwait\fP \fB[\-h]\fP
-\fBID\fP \fB[\-n SEC]\fP \fB[\-\-info [\-\-json] | \-\-status]\fP
+\fBID\fP \fB[\-n SEC]\fP \fB[\-\-info [\-f FORMAT] | \-\-status | \-\-return]\fP
 .UNINDENT
 .sp
 Wait for task to complete.
 .sp
 Poll the database periodically for the completion status
 of the task. Block until completed.
 .sp
@@ -783,24 +906,33 @@
 .UNINDENT
 .SS Options
 .INDENT 0.0
 .TP
 .B \fB\-n\fP, \fB\-\-interval\fP \fISEC\fP
 Time in seconds to wait between polling (default: 5).
 .TP
-.B \fB\-\-info\fP
+.B \fB\-i\fP, \fB\-\-info\fP
 Print task info after completion.
 .sp
 See \fBtask info\fP command.
 .TP
+.B \fB\-f\fP, \fB\-\-format\fP \fIFORMAT\fP
+Format task info ([normal], json, yaml).
+.TP
 .B \fB\-\-json\fP
 Format metadata output as JSON.
 .TP
-.B \fB\-\-status\fP
+.B \fB\-\-yaml\fP
+Format metadata output as YAML.
+.TP
+.B \fB\-s\fP, \fB\-\-status\fP
 Print task exit status only.
+.TP
+.B \fB\-r\fP, \fB\-\-return\fP
+Use exit status from task.
 .UNINDENT
 .SH TASK RUN USAGE
 .sp
 \fBhyper\-shell\fP \fBtask\fP \fBrun\fP \fB[\-h]\fP \fB[\-n SEC]\fP \fBARGS...\fP
 .sp
 Submit individual task and wait for completion.
 .sp
@@ -824,59 +956,77 @@
 .B \fB\-n\fP, \fB\-\-interval\fP \fISEC\fP
 Time in seconds to wait between polling (default: 5).
 .UNINDENT
 .SH TASK SEARCH USAGE
 .INDENT 0.0
 .TP
 .B \fBhyper\-shell\fP \fBtask\fP \fBsearch\fP \fB[\-h]\fP
-\fB[FIELD [FIELD ...]]\fP \fB[\-\-where COND [COND ...]]\fP
+\fB[FIELD [FIELD ...]]\fP \fB[\-w COND [COND ...]]\fP \fB[\-t TAG [TAG...]]\fP
 \fB[\-\-order\-by FIELD [\-\-desc]]\fP \fB[\-\-count | \-\-limit NUM]\fP
 \fB[\-\-format FORMAT | \-\-json | \-\-csv]\fP \fB[\-d CHAR]\fP
 .UNINDENT
 .sp
 Search for tasks in database.
 .sp
 A database must be configured.
-Fields will be columns in the output.
-Options relate to SQL concepts.
-For single column output, use \fB\-x\fP/\fB\-\-extract\fP to disable
-formatting and quotations (useful for piping output).
+Specifying \fIFIELD\fP names defines what is included in the output
+(by default all fields are included).
+.sp
+This command maps directly to underlying SQL queries.
 .SS Arguments
 .INDENT 0.0
 .TP
 .B FIELD
 Select specific named fields to include in output.
 Default is to include all fields.
 .UNINDENT
 .SS Options
 .INDENT 0.0
 .TP
 .B \fB\-w\fP, \fB\-\-where\fP \fICOND...\fP
-List of conditional statements to filter results (e.g., \fB\-w \(aqexit_status != 0\(aq\fP).
+List of conditional statements to filter results (e.g., \fB\-w \(aqduration >= 600\(aq\fP).
+.sp
+Operators include \fB==\fP, \fB!=\fP, \fB>=\fP, \fB<=\fP, \fB>\fP, \fB<\fP, \fB~\fP\&.
+The \fB~\fP operator applies a regular expression.
 .TP
-.B \fB\-s\fP, \fB\-\-order\-by\fP \fIFIELD\fP
-Order results by field.
+.B \fB\-t\fP, \fB\-\-tag\fP \fITAG\fP\&...
+Filter on one or more tags. (e.g., \fB\-t special\fP or \fB\-t file:a\fP).
+.sp
+Leaving the \fIvalue\fP unspecified will return any task for which the \fIkey\fP exists.
+Specifying a full \fIkey\fP:\fIvalue\fP pair will match on both.
+.TP
+.B \fB\-s\fP, \fB\-\-order\-by\fP \fIFIELD\fP \fB[\-\-desc]\fP
+Order results by field. Optionally, in descending order.
 .TP
 .B \fB\-\-failed\fP
 Alias for \fB\-w \(aqexit_status != 0\(aq\fP\&.
 .TP
 .B \fB\-\-succeeded\fP
 Alias for \fB\-w \(aqexit_status == 0\(aq\fP\&.
 .TP
 .B \fB\-\-finished\fP
 Alias for \fB\-w \(aqexit_status != null\(aq\fP\&.
 .TP
 .B \fB\-\-remaining\fP
 Alias for \fB\-w \(aqexit_status == null\(aq\fP\&.
 .TP
-.B \fB\-\-json\fP
-Format output as JSON.
+.B \fB\-\-format\fP \fIFORMAT\fP
+Specify output format (either \fBnormal\fP, \fBplain\fP, \fBtable\fP, \fBcsv\fP, \fBjson\fP).
+.sp
+Default is \fBnormal\fP for whole\-task output. If any \fIFIELD\fP names are given, output is
+formatted in simple \fBplain\fP text; use \fBcsv\fP for compliant output. The pretty\-printed
+\fBtable\fP formatting is good for presentation on wide screens.
+.sp
+See \fB\-\-csv\fP, \fB\-\-json\fP, and \fB\-\-delimiter\fP\&.
 .TP
 .B \fB\-\-csv\fP
-Format output as CSV.
+Format output as CSV. (Shorthand for \fB\-\-format=csv\fP).
+.TP
+.B \fB\-\-json\fP
+Format output as JSON. (Shorthand for \fB\-\-format=json\fP).
 .TP
 .B \fB\-d\fP, \fB\-\-delimiter\fP \fICHAR\fP
 Field seperator for plain/csv formats.
 .TP
 .B \fB\-l\fP, \fB\-\-limit\fP \fINUM\fP
 Limit the number of results.
 .TP
@@ -899,14 +1049,17 @@
 Unique UUID.
 .TP
 .B FIELD
 Task field name (e.g., \(dqargs\(dq).
 .TP
 .B VALUE
 New value.
+.sp
+Use \fBkey:value\fP notation for tasks.
+Updating \fBtag\fP will add or update any pre\-existing tag with that \fBkey\fP\&.
 .UNINDENT
 .SH TEMPLATES
 .sp
 Incoming command\-line arguments are expanded using a template pattern.
 Workloads often have a common form and only a small part of the shell command
 need be different.
 .sp
@@ -1146,27 +1299,52 @@
 .TP
 .B \fB[logging]\fP
 Logging configuration. See also \fI\%logging\fP section.
 .INDENT 7.0
 .TP
 .B \fB\&.level\fP
 One of \fBDEVEL\fP, \fBTRACE\fP, \fBDEBUG\fP, \fBINFO\fP, \fBWARNING\fP,
-\fBERROR\fP, or \fBCRITICAL\fP (default: \fIWARNING\fP)
+\fBERROR\fP, or \fBCRITICAL\fP (default: \fBWARNING\fP)
+.sp
+\fBINFO\fP level messages are reserved for clients when tasks begin running.
+There are numerous WARNING events (e.g., non\-zero exit status of a task).
+\fBDEBUG\fP level messages signal component thread start/stop and individual task
+level behavior. \fBTRACE\fP contains detailed information on all other behavior,
+particular iterative messages while components are waiting for something.
+.sp
+\fBERROR\fP messages track when things fail but the application can continue; e.g.,
+when command template expansion fails on an individual task.
+.sp
+\fBCRITICAL\fP messages are emitted when the application will halt or crash.
+Some of these are expected (such as incorrect command\-line arguments) but in
+the event of an uncaught exception within the application a full traceback is
+written to a file and logged.
+.sp
+\fBDEVEL\fP messages are meant for development purposes and track every single
+state\-transition in all component threads.
 .TP
 .B \fB\&.datefmt\fP
-Date/time format, standard codes apply (default: \fI\(aq%Y\-%m\-%d %H:%M:%S\(aq\fP)
+Date/time format, standard codes apply (default: \fB\(aq%Y\-%m\-%d %H:%M:%S\(aq\(ga\fP)
 .TP
 .B \fB\&.format\fP
-Log message format. Default set by the \fIdefault\fP \fBlogging.style\fP\&.
+Log message format.
+.sp
+Default set by the \(dqdefault\(dq \fBlogging.style\fP\&.
 See the \fI\%available attributes\fP
 defined by the underlying Python logging interface.
+.sp
+Additional attributes provided beyond the standard include \fIapp_id\fP, \fIhostname\fP, \fIhostname_short\fP,
+\fIrelative_name\fP, time formats in \fIelapsed\fP, \fIelapsed_ms\fP, \fIelapsed_delta\fP, and \fIelapsed_hms\fP,
+as well as all ANSI colors and formats as \fIansi_x\fP where x is one of \fIreset\fP, \fIbold\fP, \fIfaint\fP,
+\fIitalic\fP, \fIunderline\fP, \fIblack\fP, \fIred\fP, \fIgreen\fP, \fIyellow\fP, \fIblue\fP, \fImagenta\fP, \fIcyan\fP, \fIwhite\fP, and
+\fIansi_level\fP contains the standard color for the current message severity level.
 .TP
 .B \fB\&.style\fP
 Presets for \fBlogging.format\fP which can be difficult to define correctly.
-Options are \fIdefault\fP, \fIdetailed\fP, and \fIsystem\fP\&.
+Options are \fIdefault\fP, \fIdetailed\fP, \fIdetailed\-compact\fP, and \fIsystem\fP\&.
 .UNINDENT
 .TP
 .B \fB[database]\fP
 Database configuration and connection details.
 See also \fI\%database\fP section.
 .INDENT 7.0
 .TP
@@ -1323,14 +1501,19 @@
 .sp
 See also \fB\-w\fP/\fB\-\-bundlewait\fP command\-line option.
 .TP
 .B \fB\&.heartrate\fP
 Interval in seconds between heartbeats sent to server (default \fI10\fP).
 .sp
 Even on the largest scales the default interval should be fine.
+.TP
+.B \fB\&.timeout\fP
+Timeout in seconds for client. Automatically shutdown if no tasks received (default: never).
+.sp
+This feature allows for gracefully scaling down a cluster when task throughput subsides.
 .UNINDENT
 .TP
 .B \fB[submit]\fP
 Section for \fIsubmit\fP workflow parameters.
 .INDENT 7.0
 .TP
 .B \fB\&.bundlesize\fP
@@ -1353,33 +1536,132 @@
 .TP
 .B \fB[task]\fP
 Section for task runtime settings.
 .INDENT 7.0
 .TP
 .B \fB\&.cwd\fP
 Explicitly set the working directory for all tasks.
+.TP
+.B \fB\&.timeout\fP
+Task\-level walltime limit (default: none).
+.sp
+Executors will send a progression of SIGINT, SIGTERM, and SIGKILL.
+If the process still persists the executor itself will shutdown.
 .UNINDENT
 .TP
 .B \fB[ssh]\fP
 SSH configuration section.
 .INDENT 7.0
 .TP
 .B \fB\&.args\fP
 SSH connection arguments; e.g., \fB\-i ~/.ssh/some.key\fP\&.
 It is preferable to configure SSH directly however, in \fB~/.ssh/config\fP\&.
 .TP
-.B \fB[group]\fP
-Setting a \fIlist\fP for the \fB\&.group\fP allows for a global list of available client hosts.
-Or, set one or more named groups and reference them by name with \fB\-\-ssh\-group\fP\&.
+.B \fB[nodelist]\fP
+This can be a single list of hostnames or a section when multiple named lists.
+Reference named groups from the command\-line with \fB\-\-ssh\-group\fP\&.
+.sp
+Such as,
+.sp
+\fB\&.mycluster = [\(aqmycluster\-01\(aq, \(aqmycluster\-02\(aq, \(aqmycluster\-03\(aq]\fP
+.UNINDENT
+.TP
+.B \fB[autoscale]\fP
+Define an autoscaling policy and parameters.
+.INDENT 7.0
+.TP
+.B \fB\&.policy\fP
+Either \fIfixed\fP or \fIdynamic\fP\&.
+.sp
+A \fIfixed\fP policy will seek to maintain a definite size and allows for recovery in the
+event that clients halt for some reason (e.g., due to expected faults or timeouts).
+.sp
+A \fIdynamic\fP policy maintains a minimum size and grows up to some maximum size
+depending on the observed \fItask pressure\fP given the specified scaling factor.
+.sp
+See also \fB\&.factor\fP, \fB\&.period\fP, \fB\&.size.init\fP, \fB\&.size.min\fP, and \fB\&.size.max\fP\&.
+.TP
+.B \fB\&.factor\fP
+Scaling factor (default: 1).
+.sp
+A dimensionless quantity used by the \fIdynamic\fP policy.
+This value expresses some multiple of the average task duration in seconds.
+.sp
+The autoscaler periodically checks \fBtoc / (factor x avg_duration)\fP, where
+\fBtoc\fP is the estimated time of completion for all remaining tasks given current
+throughput of active clients. This ratio is referred to as \fItask pressure\fP, and if
+it exceeds 1, the pressure is considered \fIhigh\fP and we will add another client if
+we are not already at the maximum size of the cluster.
+.sp
+For example, if the average task length is 30 minutes, and we set \fBfactor = 2\fP, then if
+the estimated time of completion of remaining tasks given currently connected executors
+exceeds 1 hour, we will scale up by one unit.
+.sp
+See also \fB\&.period\fP\&.
+.TP
+.B \fB\&.period\fP
+Scaling period in seconds (default: 60).
+.sp
+The autoscaler waits for this period of time in between checks and scaling events.
+A shorter period makes the scaling behavior more responsive but can effect database
+performance if checks happen too rapidly.
+.TP
+.B \fB[size]\fP
+.INDENT 7.0
+.TP
+.B \fB\&.init\fP
+Initial size of cluster (default: 1).
+.sp
+When the the cluster starts, this number of clients will be launched.
+For a \fIfixed\fP policy cluster, this should be given with a \fB\&.min\fP size, and likely
+the same value.
+.TP
+.B \fB\&.min\fP
+Minimum size of cluster (default: 0).
 .sp
-\fB\&.<name> = [\(aqhost\-01\(aq, \(aqhost\-02\(aq, \(aqhost\-03\(aq]\fP
+Regardless of autoscaling policy, if the number of launched clients drops below this
+value we will scale up by one. Allowing \fBmin = 0\fP is an important feature for
+efficient use of computing resources in the absence of tasks.
+.TP
+.B \fB\&.max\fP
+Maximum size of cluster (default: 2).
+.sp
+For a \fIdynamic\fP autoscaling policy, this sets an upper limit on the number of launched
+clients. WHen this number is reached, scaling stops regardless of task pressure.
+.UNINDENT
+.UNINDENT
+.TP
+.B \fB[console]\fP
+Rich text display and output parameters.
+.INDENT 7.0
+.TP
+.B \fB\&.theme\fP
+Color scheme to use by default in output (such as with \fBtask info\fP and \fBtask search\fP).
+.sp
+This option is passed to the \fIrich\fP library.
+.UNINDENT
+.TP
+.B \fB[export]\fP
+Any variable defined here is injected as an environment variable for tasks.
+.sp
+Example,
+.INDENT 7.0
+.TP
+.B \fBfoo = 1\fP
+The environment variable \fBFOO=1\fP would defined for all tasks.
 .UNINDENT
 .UNINDENT
 .SH ENVIRONMENT VARIABLES
 .sp
+As stated for configuration, any environment variable prefixed as \fBHYPERSHELL_\fP
+where the name aligns to the path to some option, delimited by underscores,
+will set that option.
+.sp
+Example, \fBHYPERSHELL_CLIENT_TIMEOUT\fP maps to the corresponding configuration option.
+.sp
 A few common environment variables are defined for every task.
 .INDENT 0.0
 .TP
 .B \fBTASK_ID\fP
 Universal identifier (UUID) for the current task.
 .TP
 .B \fBTASK_ARGS\fP
@@ -1449,14 +1731,26 @@
 [export]
 foo = \(dqvalue\(dq
 path = [\(dq/some/bin\(dq, \(dq/some/other/bin\(dq]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
+.sp
+We also respect setting the following environment variables to force disable/enable
+the use of colors in all console output.
+.INDENT 0.0
+.TP
+.B \fBNO_COLOR\fP
+If this variable is set to anything but a blank string, all colors are disabled.
+.TP
+.B \fBFORCE_COLOR\fP
+If this variable is set to anything but a blank string, colors will be enabled
+regardless of whether \fIstdout\fP or \fIstderr\fP are a TTY.
+.UNINDENT
 .SH EXIT STATUS
 .INDENT 0.0
 .TP
 .B 0
 Success
 .TP
 .B 1
```

### Comparing `hyper-shell-2.3.0/setup.py` & `hyper-shell-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `hyper-shell-2.3.0/src/hyper_shell.egg-info/PKG-INFO` & `hyper-shell-2.4.0/src/hyper_shell.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyper-shell
-Version: 2.3.0
+Version: 2.4.0
 Summary: Process shell commands over a distributed, asynchronous queue.
 Home-page: https://github.com/glentner/hyper-shell
 Author: Geoffrey Lentner
 Author-email: glentner@purdue.edu
 License: Apache Software License
 Keywords: distributed-computing command-line-tool shell-scripting high-performance-computing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hyper-shell-2.3.0/src/hyper_shell.egg-info/SOURCES.txt` & `hyper-shell-2.4.0/src/hyper_shell.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,28 +7,31 @@
 src/hyper_shell.egg-info/SOURCES.txt
 src/hyper_shell.egg-info/dependency_links.txt
 src/hyper_shell.egg-info/entry_points.txt
 src/hyper_shell.egg-info/requires.txt
 src/hyper_shell.egg-info/top_level.txt
 src/hypershell/__init__.py
 src/hypershell/client.py
-src/hypershell/cluster.py
 src/hypershell/config.py
 src/hypershell/server.py
 src/hypershell/submit.py
 src/hypershell/task.py
+src/hypershell/cluster/__init__.py
+src/hypershell/cluster/local.py
+src/hypershell/cluster/remote.py
+src/hypershell/cluster/ssh.py
 src/hypershell/core/__init__.py
 src/hypershell/core/ansi.py
 src/hypershell/core/config.py
 src/hypershell/core/exceptions.py
 src/hypershell/core/fsm.py
 src/hypershell/core/heartbeat.py
 src/hypershell/core/logging.py
 src/hypershell/core/platform.py
 src/hypershell/core/queue.py
 src/hypershell/core/remote.py
 src/hypershell/core/template.py
 src/hypershell/core/thread.py
 src/hypershell/core/types.py
-src/hypershell/database/__init__.py
-src/hypershell/database/core.py
-src/hypershell/database/model.py
+src/hypershell/data/__init__.py
+src/hypershell/data/core.py
+src/hypershell/data/model.py
```

### Comparing `hyper-shell-2.3.0/src/hypershell/__init__.py` & `hyper-shell-2.4.0/src/hypershell/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 from hypershell.core.logging import Logger, initialize_logging
 from hypershell.submit import SubmitApp
 from hypershell.server import ServerApp
 from hypershell.client import ClientApp
 from hypershell.cluster import ClusterApp
 from hypershell.task import TaskGroupApp
 from hypershell.config import ConfigApp
-from hypershell.database import InitDBApp
+from hypershell.data import InitDBApp
 
 # public interface
 __all__ = ['HyperShellApp', 'main', '__version__', '__license__']
 
 # project metadata
-__version__     = '2.3.0'
+__version__     = '2.4.0'
 __authors__     = 'Geoffrey Lentner'
 __contact__     = 'glentner@purdue.edu'
 __license__     = 'Apache Software License'
 __copyright__   = '2019-2023. All Rights Reserved.'
 __website__     = 'https://github.com/glentner/hyper-shell'
 __keywords__    = 'distributed-computing command-line-tool shell-scripting high-performance-computing'
 __description__ = 'Process shell commands over a distributed, asynchronous queue.'
```

### Comparing `hyper-shell-2.3.0/src/hypershell/client.py` & `hyper-shell-2.4.0/src/hypershell/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 # standard libs
 import os
 import sys
 import time
 import json
 import random
+import signal
 import functools
 from enum import Enum
 from datetime import datetime, timedelta
 from queue import Queue, Empty as QueueEmpty, Full as QueueFull
 from subprocess import Popen, TimeoutExpired
 from socket import gaierror
 from dataclasses import dataclass
@@ -50,15 +51,15 @@
 
 # external libs
 from cmdkit.app import Application, exit_status
 from cmdkit.cli import Interface, ArgumentError
 from cmdkit.config import Namespace
 
 # internal libs
-from hypershell.database.model import Task
+from hypershell.data.model import Task
 from hypershell.core.ansi import colorize_usage
 from hypershell.core.heartbeat import Heartbeat, ClientState
 from hypershell.core.platform import default_path
 from hypershell.core.config import default, config, load_task_env
 from hypershell.core.fsm import State, StateMachine
 from hypershell.core.thread import Thread
 from hypershell.core.queue import QueueClient, QueueConfig
@@ -128,61 +129,76 @@
     """Receive task bundles from server and schedule locally."""
 
     queue: QueueClient
     local: Queue[Optional[Task]]
     bundle: List[bytes]
     client_info: Optional[bytes]
     no_confirm: bool
+    timeout: Optional[timedelta]
+
+    previous_received: datetime
 
     task: Task
     tasks: List[Task]
 
     state = SchedulerState.START
     states = SchedulerState
 
-    def __init__(self: ClientScheduler, queue: QueueClient, local: Queue[Optional[Task]], no_confirm: bool = False) -> None:
+    def __init__(self: ClientScheduler,
+                 queue: QueueClient,
+                 local: Queue[Optional[Task]],
+                 no_confirm: bool = False,
+                 timeout: int = None) -> None:
         """Assign remote queue client and local task queue."""
         self.queue = queue
         self.local = local
         self.bundle = []
         self.tasks = []
         self.client_info = None
         self.no_confirm = no_confirm
+        self.timeout = None if not timeout else timedelta(seconds=timeout)
+        self.previous_received = datetime.now()
 
     @functools.cached_property
     def actions(self: ClientScheduler) -> Dict[SchedulerState, Callable[[], SchedulerState]]:
         return {
             SchedulerState.START: self.start,
             SchedulerState.GET_REMOTE: self.get_remote,
             SchedulerState.UNPACK: self.unpack_bundle,
             SchedulerState.PUT_CONFIRM: self.put_confirm,
             SchedulerState.POP_TASK: self.pop_task,
             SchedulerState.PUT_LOCAL: self.put_local,
             SchedulerState.FINAL: self.finalize,
         }
 
-    @staticmethod
-    def start() -> SchedulerState:
+    def start(self: ClientScheduler) -> SchedulerState:
         """Jump to GET_REMOTE state."""
-        log.debug('Started (scheduler)')
+        timeout_label = self.timeout or 'no'
+        log.debug(f'Started (scheduler: {timeout_label} timeout)')
         return SchedulerState.GET_REMOTE
 
     def get_remote(self: ClientScheduler) -> SchedulerState:
         """Get the next task bundle from the server."""
         try:
             self.bundle = self.queue.scheduled.get(timeout=2)
             self.queue.scheduled.task_done()
+            self.previous_received = datetime.now()
             if self.bundle is not None:
                 log.debug(f'Received {len(self.bundle)} tasks ({HOSTNAME}: {INSTANCE})')
                 return SchedulerState.UNPACK
             else:
                 log.debug('Disconnect received')
                 return SchedulerState.FINAL
         except QueueEmpty:
-            return SchedulerState.GET_REMOTE
+            waited = datetime.now() - self.previous_received
+            if self.timeout is None or waited < self.timeout:
+                return SchedulerState.GET_REMOTE
+            else:
+                log.debug(f'Timeout reached ({waited})')
+                return SchedulerState.FINAL
 
     def unpack_bundle(self: ClientScheduler) -> SchedulerState:
         """Unpack latest bundle of tasks."""
         self.tasks = [Task.unpack(data) for data in self.bundle]
         if not self.no_confirm:
             self.client_info = ClientInfo.from_tasks(self.tasks).pack()
             return SchedulerState.PUT_CONFIRM
@@ -220,18 +236,22 @@
         log.debug('Done (scheduler)')
         return SchedulerState.HALT
 
 
 class ClientSchedulerThread(Thread):
     """Run client scheduler in dedicated thread."""
 
-    def __init__(self: ClientSchedulerThread, queue: QueueClient, local: Queue[Optional[bytes]], no_confirm: bool = False) -> None:
+    def __init__(self: ClientSchedulerThread,
+                 queue: QueueClient,
+                 local: Queue[Optional[bytes]],
+                 no_confirm: bool = False,
+                 timeout: int = None) -> None:
         """Initialize machine."""
         super().__init__(name='hypershell-client-scheduler')
-        self.machine = ClientScheduler(queue=queue, local=local, no_confirm=no_confirm)
+        self.machine = ClientScheduler(queue=queue, local=local, no_confirm=no_confirm, timeout=timeout)
 
     def run_with_exceptions(self: ClientSchedulerThread) -> None:
         """Run machine."""
         self.machine.run()
 
     def stop(self: ClientSchedulerThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
@@ -315,34 +335,34 @@
         """Check state of task bundle and proceed with return if necessary."""
         wait_time = (datetime.now() - self.previous_send)
         since_last = wait_time.total_seconds()
         if len(self.tasks) >= self.bundlesize:
             log.trace(f'Bundle size reached ({len(self.tasks)} tasks)')
             return CollectorState.PACK_BUNDLE
         elif since_last >= self.bundlewait:
-            log.trace(f'Wait time exceeded ({wait_time})')
+            log.trace(f'Bundle wait exceeded ({wait_time})')
             return CollectorState.PACK_BUNDLE
         else:
             return CollectorState.GET_LOCAL
 
     def pack_bundle(self: ClientCollector) -> CollectorState:
         """Pack tasks into bundle before pushing back to server."""
         self.bundle = [task.pack() for task in self.tasks]
         return CollectorState.PUT_REMOTE
 
     def put_remote(self: ClientCollector) -> CollectorState:
         """Push out bundle of completed tasks."""
         if self.bundle:
             self.queue.completed.put(self.bundle)
-            log.trace(f'Returned bundle ({len(self.bundle)} tasks)')
+            log.trace(f'Bundle returned ({len(self.bundle)} tasks)')
             self.tasks.clear()
             self.bundle.clear()
             self.previous_send = datetime.now()
         else:
-            log.trace('No local tasks to return')
+            log.trace('Bundle empty')
         return CollectorState.GET_LOCAL
 
     def finalize(self: ClientCollector) -> CollectorState:
         """Push out any remaining tasks and halt."""
         self.put_remote()
         log.debug('Done (collector)')
         return CollectorState.HALT
@@ -366,73 +386,93 @@
         log.warning('Stopping (collector)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
 def task_env(task: Task) -> Dict[str, str]:
     """Build environment dictionary for the given `task`."""
+    task_data = task.to_json()
+    task_data.pop('tag')  # do not include tags in environ
     return {
         **os.environ,
         **load_task_env(),
-        **Namespace.from_dict(task.to_json()).to_env().flatten(prefix='TASK'),
+        **Namespace.from_dict(task_data).to_env().flatten(prefix='TASK'),
         'TASK_CWD': config.task.cwd,
         'TASK_OUTPATH': os.path.join(default_path.lib, 'task', f'{task.id}.out'),
         'TASK_ERRPATH': os.path.join(default_path.lib, 'task', f'{task.id}.err'),
     }
 
 
 class TaskState(State, Enum):
     """Finite states for task executor."""
     START = 0
     GET_LOCAL = 1
     CREATE_TASK = 2
     START_TASK = 3
     WAIT_TASK = 4
-    PUT_LOCAL = 5
-    FINAL = 6
-    HALT = 7
+    STOP_TASK = 5
+    TERM_TASK = 6
+    KILL_TASK = 7
+    PUT_LOCAL = 8
+    FINAL = 9
+    HALT = 10
 
 
 class TaskExecutor(StateMachine):
     """Run tasks locally."""
 
     id: int
     task: Task
     process: Popen
     template: Template
     redirect_output: IO
     redirect_errors: IO
     capture: bool
 
+    timeout: Optional[int]
+    attempted_sigint: bool
+    attempted_sigterm: bool
+    attempted_sigkill: bool
+
     inbound: Queue[Optional[Task]]
     outbound: Queue[Optional[Task]]
 
     state = TaskState.START
     states = TaskState
 
-    def __init__(self: TaskExecutor, id: int, inbound: Queue[Optional[Task]], outbound: Queue[Optional[Task]],
-                 template: str = DEFAULT_TEMPLATE, redirect_output: IO = None, redirect_errors: IO = None,
-                 capture: bool = False) -> None:
+    def __init__(self: TaskExecutor,
+                 id: int,
+                 inbound: Queue[Optional[Task]],
+                 outbound: Queue[Optional[Task]],
+                 template: str = DEFAULT_TEMPLATE,
+                 redirect_output: IO = None,
+                 redirect_errors: IO = None,
+                 capture: bool = False,
+                 timeout: int = None) -> None:
         """Initialize task executor."""
         self.id = id
         self.template = Template(template)
         self.inbound = inbound
         self.outbound = outbound
         self.redirect_output = redirect_output or sys.stdout
         self.redirect_errors = redirect_errors or sys.stderr
         self.capture = capture
+        self.timeout = timeout
 
     @functools.cached_property
     def actions(self: TaskExecutor) -> Dict[TaskState, Callable[[], TaskState]]:
         return {
             TaskState.START: self.start,
             TaskState.GET_LOCAL: self.get_local,
             TaskState.CREATE_TASK: self.create_task,
             TaskState.START_TASK: self.start_task,
             TaskState.WAIT_TASK: self.wait_task,
+            TaskState.STOP_TASK: self.stop_task,
+            TaskState.TERM_TASK: self.term_task,
+            TaskState.KILL_TASK: self.kill_task,
             TaskState.PUT_LOCAL: self.put_local,
             TaskState.FINAL: self.finalize,
         }
 
     def start(self: TaskExecutor) -> TaskState:
         """Jump to GET_LOCAL state."""
         log.debug(f'Started (executor-{self.id})')
@@ -466,68 +506,121 @@
         env = task_env(self.task)
         if self.capture:
             self.task.outpath = env['TASK_OUTPATH']
             self.task.errpath = env['TASK_ERRPATH']
             self.redirect_output = open(self.task.outpath, mode='w')
             self.redirect_errors = open(self.task.errpath, mode='w')
         self.task.start_time = datetime.now().astimezone()
+        # NOTE: enforce tz aware submit_time (in case of sqlite backend)
+        self.task.waited = int((self.task.start_time - self.task.submit_time.astimezone()).total_seconds())
+        self.attempted_sigint = False
+        self.attempted_sigterm = False
+        self.attempted_sigkill = False
         self.process = Popen(self.task.command, shell=True,
                              stdout=self.redirect_output, stderr=self.redirect_errors,
                              cwd=config.task.cwd, env=env)
         log.info(f'Running task ({self.task.id})')
         log.debug(f'Running task ({self.task.id}: {self.task.command})')
         log.trace(f'Running task ({self.task.id}: pid={self.process.pid}, argv={self.task.command})')
         return TaskState.WAIT_TASK
 
     def wait_task(self: TaskExecutor) -> TaskState:
         """Wait for current task to complete."""
         try:
-            self.task.exit_status = self.process.wait(timeout=2)
+            self.task.exit_status = self.process.wait(timeout=1)
             self.task.completion_time = datetime.now().astimezone()
+            self.task.duration = int((self.task.completion_time - self.task.start_time).total_seconds())
             log.debug(f'Completed task ({self.task.id})')
             if self.capture:
                 self.redirect_output.close()
                 self.redirect_errors.close()
             return TaskState.PUT_LOCAL
         except TimeoutExpired:
             # Only include time elapsed to the nearest second (we don't need fractions)
             elapsed = timedelta(seconds=round((datetime.now().astimezone() - self.task.start_time).total_seconds()))
             log.trace(f'Waiting on task ({self.task.id}: {elapsed})')
+            if self.timeout is None or elapsed.total_seconds() < self.timeout:
+                return TaskState.WAIT_TASK
+            elif self.attempted_sigint is False:
+                log.warning(f'Task exceeded walltime limit ({elapsed})')
+                return TaskState.STOP_TASK
+            elif self.attempted_sigterm is False:
+                log.error(f'Interrupt ignored ({self.task.id})')
+                return TaskState.TERM_TASK
+            else:
+                log.error(f'Terminate ignored ({self.task.id})')
+                return TaskState.KILL_TASK
+
+    def stop_task(self: TaskExecutor) -> TaskState:
+        """Send SIGINT to task process."""
+        log.debug(f'Sending SIGINT ({self.task.id}: {self.process.pid})')
+        self.process.send_signal(signal.SIGINT)
+        self.attempted_sigint = True
+        time.sleep(2)  # additional grace period
+        return TaskState.WAIT_TASK
+
+    def term_task(self: TaskExecutor) -> TaskState:
+        """Send SIGTERM to task process."""
+        log.debug(f'Sending SIGTERM ({self.task.id}: {self.process.pid})')
+        self.process.terminate()
+        self.attempted_sigterm = True
+        time.sleep(2)  # additional grace period
+        return TaskState.WAIT_TASK
+
+    def kill_task(self: TaskExecutor) -> TaskState:
+        """Send SIGKILL or halt executor if ignored."""
+        if self.attempted_sigkill is False:
+            log.debug(f'Sending SIGKILL ({self.task.id}: {self.process.pid})')
+            self.process.kill()
+            self.attempted_sigkill = True
+            time.sleep(2)  # additional grace period
             return TaskState.WAIT_TASK
+        else:
+            log.critical(f'Process ignored SIGKILL ({self.task.id}: {self.process.pid})')
+            log.critical(f'Shutting down executor ({self.id})')
+            return TaskState.FINAL
 
     def put_local(self: TaskExecutor) -> TaskState:
         """Put completed task on outbound queue."""
         try:
             self.outbound.put(self.task, timeout=1)
             return TaskState.GET_LOCAL
         except QueueFull:
             return TaskState.PUT_LOCAL
 
     def finalize(self: TaskExecutor) -> TaskState:
         """Push out any remaining tasks and halt."""
         log.debug(f'Done (executor-{self.id})')
+        if self.redirect_output is not sys.stdout:
+            self.redirect_output.close()
+        if self.redirect_errors is not sys.stderr:
+            self.redirect_errors.close()
         return TaskState.HALT
 
 
 class TaskThread(Thread):
     """Run task executor within dedicated thread."""
 
     id: int
 
     def __init__(self: TaskThread,
                  id: int,
-                 inbound: Queue[Optional[str]], outbound: Queue[Optional[str]],
-                 template: str = DEFAULT_TEMPLATE, capture: bool = False,
-                 redirect_output: IO = None, redirect_errors: IO = None) -> None:
+                 inbound: Queue[Optional[str]],
+                 outbound: Queue[Optional[str]],
+                 template: str = DEFAULT_TEMPLATE,
+                 capture: bool = False,
+                 redirect_output: IO = None,
+                 redirect_errors: IO = None,
+                 timeout: int = None) -> None:
         """Initialize task executor."""
         self.id = id
         super().__init__(name=f'hypershell-executor-{id}')
         self.machine = TaskExecutor(id=id, inbound=inbound, outbound=outbound, template=template,
                                     redirect_output=redirect_output, redirect_errors=redirect_errors,
-                                    capture=capture)
+                                    capture=capture, timeout=timeout)
 
     def run_with_exceptions(self: TaskThread) -> None:
         """Run machine."""
         self.machine.run()
 
     def stop(self: TaskThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
@@ -659,37 +752,44 @@
     outbound: Queue[Optional[Task]]
     scheduler: ClientSchedulerThread
     collector: ClientCollectorThread
     executors: List[TaskThread]
 
     def __init__(self: ClientThread,
                  num_tasks: int = DEFAULT_NUM_TASKS,
-                 bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT,
+                 bundlesize: int = DEFAULT_BUNDLESIZE,
+                 bundlewait: int = DEFAULT_BUNDLEWAIT,
                  address: Tuple[str, int] = (QueueConfig.host, QueueConfig.port),
-                 auth: str = QueueConfig.auth, template: str = DEFAULT_TEMPLATE,
-                 redirect_output: IO = None, redirect_errors: IO = None,
-                 heartrate: int = DEFAULT_HEARTRATE, capture: bool = False,
-                 delay_start: float = DEFAULT_DELAY, no_confirm: bool = False) -> None:
+                 auth: str = QueueConfig.auth,
+                 template: str = DEFAULT_TEMPLATE,
+                 redirect_output: IO = None,
+                 redirect_errors: IO = None,
+                 heartrate: int = DEFAULT_HEARTRATE,
+                 capture: bool = False,
+                 delay_start: float = DEFAULT_DELAY,
+                 no_confirm: bool = False,
+                 client_timeout: int = None,
+                 task_timeout: int = None) -> None:
         """Initialize queue manager and child threads."""
         super().__init__(name='hypershell-client')
         self.num_tasks = num_tasks
         self.delay_start = delay_start
         self.no_confirm = no_confirm
         self.client = QueueClient(config=QueueConfig(host=address[0], port=address[1], auth=auth))
         self.inbound = Queue(maxsize=bundlesize)
         self.outbound = Queue(maxsize=bundlesize)
-        self.received = Queue(maxsize=1)  # NOTE: block new bundles until signaling previous
-        self.scheduler = ClientSchedulerThread(queue=self.client, local=self.inbound, no_confirm=no_confirm)
+        self.scheduler = ClientSchedulerThread(queue=self.client, local=self.inbound,
+                                               no_confirm=no_confirm, timeout=client_timeout)
         self.heartbeat = ClientHeartbeatThread(queue=self.client, heartrate=heartrate)
         self.collector = ClientCollectorThread(queue=self.client, local=self.outbound,
                                                bundlesize=bundlesize, bundlewait=bundlewait)
         self.executors = [TaskThread(id=count+1,
                                      inbound=self.inbound, outbound=self.outbound,
                                      redirect_output=redirect_output, redirect_errors=redirect_errors,
-                                     template=template, capture=capture)
+                                     template=template, capture=capture, timeout=task_timeout)
                           for count in range(num_tasks)]
 
     def run_with_exceptions(self: ClientThread) -> None:
         """Start child threads, wait."""
         log.debug(f'Started ({self.num_tasks} executors)')
         self.wait_start()
         with self.client:
@@ -754,59 +854,63 @@
 
 
 def run_client(num_tasks: int = DEFAULT_NUM_TASKS,
                bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT,
                address: Tuple[str, int] = (QueueConfig.host, QueueConfig.port), auth: str = QueueConfig.auth,
                template: str = DEFAULT_TEMPLATE, redirect_output: IO = None, redirect_errors: IO = None,
                capture: bool = False, heartrate: int = DEFAULT_HEARTRATE,
-               delay_start: float = DEFAULT_DELAY, no_confirm: bool = False) -> None:
+               delay_start: float = DEFAULT_DELAY, no_confirm: bool = False,
+               client_timeout: int = None, task_timeout: int = None) -> None:
     """Run client until disconnect signal received."""
     thread = ClientThread.new(num_tasks=num_tasks, bundlesize=bundlesize, bundlewait=bundlewait,
                               address=address, auth=auth, template=template, capture=capture,
                               redirect_output=redirect_output, redirect_errors=redirect_errors,
-                              heartrate=heartrate, delay_start=delay_start, no_confirm=no_confirm)
+                              heartrate=heartrate, delay_start=delay_start, no_confirm=no_confirm,
+                              client_timeout=client_timeout, task_timeout=task_timeout)
     try:
         thread.join()
     except Exception:
         thread.stop()
         raise
 
 
 APP_NAME = 'hyper-shell client'
 APP_USAGE = f"""\
 Usage:
-hyper-shell client [-h] [-N NUM] [-t TEMPLATE] [-b SIZE] [-w SEC] [-d SEC]
-                   [-H ADDR] [-p PORT] [-k KEY] [-c | [-o PATH] [-e PATH]]
-                   [--no-confirm] [--delay-start SEC]
+hyper-shell client [-h] [-N NUM] [-t CMD] [-b SIZE] [-w SEC] [-H ADDR] [-p PORT]
+                   [-k KEY] [--capture | [-o PATH] [-e PATH]] [--no-confirm]
+                   [--delay-start SEC] [--timeout SEC] [--task-timeout SEC]
 
 Launch client directly, run tasks in parallel.\
 """
 
 APP_HELP = f"""\
 {APP_USAGE}
 
 Tasks are pulled off of the shared queue in bundles from the server and run
 locally within the same shell as the client. By default the bundle size is one,
 meaning that at small scales there is greater responsiveness. It is recommended
 to coordinate these parameters to be the same as the server.
 
 Options:
-  -N, --num-tasks    NUM   Number of tasks to run in parallel (default: {DEFAULT_NUM_TASKS}).
-  -t, --template     CMD   Command-line template pattern (default: "{DEFAULT_TEMPLATE}").
-  -b, --bundlesize   SIZE  Bundle size for finished tasks (default: {DEFAULT_BUNDLESIZE}).
-  -w, --bundlewait   SEC   Seconds to wait before flushing tasks (default: {DEFAULT_BUNDLEWAIT}).
-  -H, --host         ADDR  Hostname for server.
-  -p, --port         NUM   Port number for server.
-  -k, --auth         KEY   Cryptographic key to connect to server.
-  -d, --delay-start  SEC   Seconds to wait before start-up (default: {DEFAULT_DELAY}).
-      --no-confirm         Disable confirmation of task bundle received.
-  -o, --output       PATH  Redirect task output (default: <stdout>).
-  -e, --errors       PATH  Redirect task errors (default: <stderr>).
-  -c, --capture            Capture individual task <stdout> and <stderr>.
-  -h, --help               Show this message and exit.\
+  -N, --num-tasks     NUM   Number of tasks to run in parallel (default: {DEFAULT_NUM_TASKS}).
+  -t, --template      CMD   Command-line template pattern (default: "{DEFAULT_TEMPLATE}").
+  -b, --bundlesize    SIZE  Bundle size for finished tasks (default: {DEFAULT_BUNDLESIZE}).
+  -w, --bundlewait    SEC   Seconds to wait before flushing tasks (default: {DEFAULT_BUNDLEWAIT}).
+  -H, --host          ADDR  Hostname for server.
+  -p, --port          NUM   Port number for server.
+  -k, --auth          KEY   Cryptographic key to connect to server.
+  -d, --delay-start   SEC   Seconds to wait before start-up (default: {DEFAULT_DELAY}).
+      --no-confirm          Disable confirmation of task bundle received.
+  -o, --output        PATH  Redirect task output (default: <stdout>).
+  -e, --errors        PATH  Redirect task errors (default: <stderr>).
+  -c, --capture             Capture individual task <stdout> and <stderr>.
+  -T, --timeout       SEC   Automatically shutdown if no tasks received (default: never).
+  -W, --task-timeout  SEC   Task-level walltime limit (default: none).
+  -h, --help                Show this message and exit.\
 """
 
 
 class ClientApp(Application):
     """Run individual client directly."""
 
     name = APP_NAME
@@ -834,14 +938,19 @@
 
     bundlewait: int = config.submit.bundlewait
     interface.add_argument('-w', '--bundlewait', type=int, default=bundlewait)
 
     delay_start: float = DEFAULT_DELAY
     interface.add_argument('-d', '--delay-start', type=float, default=delay_start)
 
+    task_timeout: int = config.task.timeout
+    client_timeout: int = config.client.timeout
+    interface.add_argument('-T', '--timeout', type=int, default=client_timeout, dest='client_timeout')
+    interface.add_argument('-W', '--task-timeout', type=int, default=task_timeout, dest='task_timeout')
+
     no_confirm: bool = False
     interface.add_argument('--no-confirm', action='store_true')
 
     output_path: str = None
     errors_path: str = None
     interface.add_argument('-o', '--output', default=None, dest='output_path')
     interface.add_argument('-e', '--errors', default=None, dest='errors_path')
@@ -858,26 +967,39 @@
         **get_shared_exception_mapping(__name__),
     }
 
     def run(self: ClientApp) -> None:
         """Run client."""
         try:
             self.check_args()
-            run_client(num_tasks=self.num_tasks, bundlesize=self.bundlesize, bundlewait=self.bundlewait,
-                       address=(self.host, self.port), auth=self.auth, template=self.template,
-                       redirect_output=self.output_stream, redirect_errors=self.errors_stream,
-                       capture=self.capture, delay_start=self.delay_start, no_confirm=self.no_confirm,
-                       heartrate=config.client.heartrate)
+            run_client(num_tasks=self.num_tasks,
+                       bundlesize=self.bundlesize,
+                       bundlewait=self.bundlewait,
+                       address=(self.host, self.port),
+                       auth=self.auth,
+                       template=self.template,
+                       redirect_output=self.output_stream,
+                       redirect_errors=self.errors_stream,
+                       capture=self.capture,
+                       delay_start=self.delay_start,
+                       no_confirm=self.no_confirm,
+                       heartrate=config.client.heartrate,
+                       client_timeout=self.client_timeout,
+                       task_timeout=self.task_timeout)
         except gaierror:
             raise HostAddressInfo(f'Could not resolve host \'{self.host}\'')
 
     def check_args(self: ClientApp) -> None:
         """Check for logical errors in command-line arguments."""
         if self.capture and (self.output_path or self.errors_path):
             raise ArgumentError('Cannot specify --capture with either --output or --errors')
+        if self.client_timeout is not None and self.client_timeout <= 0:
+            raise ArgumentError('Client --timeout should be positive integer')
+        if self.task_timeout is not None and self.task_timeout <= 0:
+            raise ArgumentError('Client --task-timeout should be positive integer')
 
     @functools.cached_property
     def output_stream(self: ClientApp) -> IO:
         """IO stream for task outputs."""
         return sys.stdout if not self.output_path else open(self.output_path, mode='w')
 
     @functools.cached_property
```

### Comparing `hyper-shell-2.3.0/src/hypershell/config.py` & `hyper-shell-2.4.0/src/hypershell/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 {GET_USAGE}
 
 If --user/--system not specified, the output is the merged configuration
 from all sources. Use `hyper-shell config which` to see where a specific
 option originates from.
 
 Arguments:
-  SECTION[...].VAR          Path to variable.
+  SECTION[...].VAR          Path to variable (default: '.').
 
 Options:
       --system              Load from system configuration.
       --user                Load from user configuration.
   -x, --expand              Expand variable.
   -h, --help                Show this message and exit.\
 """
@@ -115,15 +115,15 @@
     """Get configuration option."""
 
     interface = Interface(GET_PROGRAM,
                           colorize_usage(GET_USAGE),
                           colorize_usage(GET_HELP))
 
     varpath: str = None
-    interface.add_argument('varpath', metavar='VAR')
+    interface.add_argument('varpath', nargs='?', default='.')
 
     site_name: str = None
     site_interface = interface.add_mutually_exclusive_group()
     site_interface.add_argument('--user', action='store_const', const='user', dest='site_name')
     site_interface.add_argument('--system', action='store_const', const='system', dest='site_name')
 
     expand: bool = False
```

### Comparing `hyper-shell-2.3.0/src/hypershell/core/ansi.py` & `hyper-shell-2.4.0/src/hypershell/core/ansi.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,49 +12,56 @@
 import os
 import re
 import sys
 import functools
 from enum import Enum
 
 # public interface
-__all__ = ['NO_TTY', 'Ansi', 'format_ansi',
+__all__ = ['NO_COLOR', 'FORCE_COLOR', 'COLOR_STDOUT', 'COLOR_STDERR', 'Ansi', 'format_ansi',
            'bold', 'faint', 'italic', 'underline',
            'black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'white',
            'colorize_usage', ]
 
 
-# Automatically disable colors if necessary
-NO_TTY = False
-if not sys.stderr.isatty():
-    NO_TTY = True
-if 'HYPERSHELL_FORCE_COLOR' in os.environ:
-    NO_TTY = False
+# Enable/disable colors if necessary
+NO_COLOR = False if not os.getenv('NO_COLOR') else True
+FORCE_COLOR = False if not os.getenv('FORCE_COLOR') else True
+
+COLOR_STDOUT = True
+COLOR_STDERR = True
+if not sys.stdout.isatty() and not FORCE_COLOR:
+    COLOR_STDOUT = False
+if not sys.stderr.isatty() and not FORCE_COLOR:
+    COLOR_STDERR = False
+if NO_COLOR:
+    COLOR_STDOUT = False
+    COLOR_STDERR = False
 
 
 class Ansi(Enum):
     """ANSI escape sequences for colors."""
     NULL = ''
-    RESET = '\033[0m' if not NO_TTY else ''
-    BOLD = '\033[1m' if not NO_TTY else ''
-    FAINT = '\033[2m' if not NO_TTY else ''
-    ITALIC = '\033[3m' if not NO_TTY else ''
-    UNDERLINE = '\033[4m' if not NO_TTY else ''
-    BLACK = '\033[30m' if not NO_TTY else ''
-    RED = '\033[31m' if not NO_TTY else ''
-    GREEN = '\033[32m' if not NO_TTY else ''
-    YELLOW = '\033[33m' if not NO_TTY else ''
-    BLUE = '\033[34m' if not NO_TTY else ''
-    MAGENTA = '\033[35m' if not NO_TTY else ''
-    CYAN = '\033[36m' if not NO_TTY else ''
-    WHITE = '\033[37m' if not NO_TTY else ''
+    RESET = '\033[0m'
+    BOLD = '\033[1m'
+    FAINT = '\033[2m'
+    ITALIC = '\033[3m'
+    UNDERLINE = '\033[4m'
+    BLACK = '\033[30m'
+    RED = '\033[31m'
+    GREEN = '\033[32m'
+    YELLOW = '\033[33m'
+    BLUE = '\033[34m'
+    MAGENTA = '\033[35m'
+    CYAN = '\033[36m'
+    WHITE = '\033[37m'
 
 
 def format_ansi(seq: Ansi, text: str) -> str:
     """Apply escape sequence with reset afterward."""
-    if NO_TTY:
+    if NO_COLOR:
         return text
     elif text.endswith(Ansi.RESET.value):
         return f'{seq.value}{text}'
     else:
         return f'{seq.value}{text}{Ansi.RESET.value}'
 
 
@@ -70,16 +77,19 @@
 blue = functools.partial(format_ansi, Ansi.BLUE)
 magenta = functools.partial(format_ansi, Ansi.MAGENTA)
 cyan = functools.partial(format_ansi, Ansi.CYAN)
 white = functools.partial(format_ansi, Ansi.WHITE)
 
 
 def colorize_usage(text: str) -> str:
-    """Apply rich ANSI formatting to usage and help text if TTY-mode."""
-    if not sys.stdout.isatty():  # NOTE: usage is on stdout not stderr
+    """
+    Apply rich ANSI formatting to usage and help text.
+    Has no effect if NO_COLOR is set or stdout is not a TTY.
+    """
+    if not COLOR_STDOUT:  # NOTE: usage is on stdout not stderr
         return text
     else:
         return _apply_formatters(text,
                                  _format_headers,
                                  _format_options,
                                  _format_special_args,
                                  _format_special_marker,
@@ -118,16 +128,16 @@
     """Add rich ANSI formatting to option syntax."""
     option_pattern = r'(?P<leader>[ /\[,])(?P<option>-[a-zA-Z]|--[a-z]+(-[a-z]+)?)\b'
     return re.sub(option_pattern + NOT_QUOTED, r'\g<leader>' + cyan(r'\g<option>'), text)
 
 
 def _format_special_args(text: str) -> str:
     """Add rich ANSI formatting to special argument syntax."""
-    metavars = ['FILE', 'PATH', 'ARGS', 'ID', 'NUM', 'CMD', 'SIZE', 'SEC', 'NAME', 'TEMPLATE', 'CHAR',
-                'ADDR', 'HOST', 'PORT', 'KEY', 'SECTION', 'VAR', 'VALUE', 'FIELD', 'COND', 'FORMAT']
+    metavars = ['FILE', 'PATH', 'ARGS', 'ID', 'NUM', 'CMD', 'SIZE', 'SEC', 'NAME', 'TEMPLATE', 'CHAR', 'MODE',
+                'ADDR', 'HOST', 'PORT', 'KEY', 'SECTION', 'VAR', 'VALUE', 'FIELD', 'COND', 'FORMAT', 'TAG']
     metavars_pattern = r'\b(?P<arg>' + '|'.join(metavars) + r')\b'
     return re.sub(metavars_pattern + NOT_QUOTED, italic(r'\g<arg>'), text)
 
 
 def _format_special_marker(text: str) -> str:
     """Add rich ANSI formatting to special markers (e.g., '<stdout>')."""
     args = ['<stdout>', '<stderr>', '<stdin>', '<devnull>', '<none>', '<command>', '<args>', ]
@@ -144,14 +154,15 @@
     return re.sub(r'"(?P<subtext>.*)"', yellow(r'"\g<subtext>"'), text)
 
 
 def _format_backtick_string(text: str) -> str:
     """Add rich ANSI formatting to quoted strings."""
     return re.sub(r'`(?P<subtext>.*)`', yellow(r'`\g<subtext>`'), text)
 
+
 def _format_digit(text: str) -> str:
     """Add rich ANSI formatting to numerical digits."""
     return re.sub(r'\b(?P<num>\d+|null|NULL)\b' + NOT_QUOTED, green(r'\g<num>'), text)
 
 
 def _format_external_commands(text: str) -> str:
     """Add rich ANSI formatting to external command mentions."""
```

### Comparing `hyper-shell-2.3.0/src/hypershell/core/config.py` & `hyper-shell-2.4.0/src/hypershell/core/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,19 @@
     'system': {
         'format': '%(asctime)s.%(msecs)03d %(hostname)s %(levelname)8s [%(app_id)s] [%(name)s] %(message)s',
     },
     'detailed': {
         'format': ('%(ansi_faint)s%(asctime)s.%(msecs)03d %(hostname)s %(ansi_reset)s'
                    '%(ansi_level)s%(ansi_bold)s%(levelname)8s%(ansi_reset)s '
                    '%(ansi_faint)s[%(name)s]%(ansi_reset)s %(message)s'),
+    },
+    'detailed-compact': {
+        'format': ('%(ansi_faint)s%(elapsed_hms)s [%(hostname_short)s] %(ansi_reset)s'
+                   '%(ansi_level)s%(ansi_bold)s%(levelname)8s%(ansi_reset)s '
+                   '%(ansi_faint)s[%(relative_name)s]%(ansi_reset)s %(message)s'),
     }
 }
 
 
 # environment variables and configuration files are automatically
 # depth-first merged with defaults
 default = Namespace({
@@ -62,14 +67,15 @@
         'level': 'warning',
         'datefmt': '%Y-%m-%d %H:%M:%S',
         'style': DEFAULT_LOGGING_STYLE,
         **LOGGING_STYLES.get(DEFAULT_LOGGING_STYLE),
     },
     'task': {
         'cwd': os.getcwd(),
+        'timeout': None,  # Seconds, period to wait before killing tasks
     },
     'submit': {
         'bundlesize': 1,
         'bundlewait': 5  # seconds
     },
     'server': {
         'bind': 'localhost',
@@ -83,18 +89,30 @@
         'wait': 5,  # seconds to wait between database queries
         'evict': 600,  # assume client is gone if no heartbeat after this many seconds
     },
     'client': {
         'bundlesize': 1,
         'bundlewait': 5,  # Seconds
         'heartrate': 10,  # Seconds, period to wait between heartbeats
+        'timeout': None,  # seconds, period to wait on tasks before shutting down
     },
     'ssh': {
         'config': os.path.join(home, '.ssh', 'config'),
     },
+    'autoscale': {
+        'policy': 'fixed',  # Either 'fixed' or 'dynamic'
+        'factor': 1,
+        'period': 60,  # seconds to wait between checks
+        'launcher': '',  # empty means just 'hyper-shell client'
+        'size': {
+            'init': 1,
+            'min': 0,
+            'max': 2,
+        },
+    },
     'console': {
         'theme': 'monokai',
     },
     'export': {
         # NOTE: defining HYPERSHELL_EXPORT_XXX defines XXX within task env
     }
 })
```

### Comparing `hyper-shell-2.3.0/src/hypershell/core/exceptions.py` & `hyper-shell-2.4.0/src/hypershell/core/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,30 +18,34 @@
 
 # external libs
 from cmdkit.app import exit_status
 from cmdkit.config import Namespace
 from cmdkit.config import ConfigurationError
 
 # internal libs
-from hypershell.core.ansi import faint, bold, magenta, yellow, red
+from hypershell.core.ansi import faint, bold, magenta, yellow, red, COLOR_STDERR
 from hypershell.core.platform import default_path
 
 # public interface
 __all__ = ['display_warning', 'display_error', 'display_critical', 'traceback_filepath', 'write_traceback',
-           'handle_exception', 'handle_disconnect', 'handle_address_unknown',
+           'handle_exception', 'handle_exception_silently', 'handle_disconnect', 'handle_address_unknown',
            'HostAddressInfo', 'DatabaseUninitialized',
            'get_shared_exception_mapping', ]
 
 
 def _display_message(levelname: str, error: Union[Exception, str],
                      module: str = None, colorized: Callable[[str], str] = None) -> None:
     """Generic message display for import-time warnings and errors."""
     text = error if isinstance(error, str) else f'{error.__class__.__name__}: {error}'
-    name = '' if not module else faint(f'[{module}]')
-    level = levelname if colorized is None else bold(colorized(levelname))
+    if COLOR_STDERR:
+        name = '' if not module else faint(f'[{module}]')
+        level = levelname if colorized is None else bold(colorized(levelname))
+    else:
+        name = '' if not module else f'[{module}]'
+        level = levelname
     print(f'{level} {name} {text}', file=sys.stderr)
 
 
 # Specialized methods for each severity level
 display_warning = functools.partial(_display_message, 'WARNING', colorized=yellow)
 display_error = functools.partial(_display_message, 'ERROR', colorized=red)
 display_critical = functools.partial(_display_message, 'CRITICAL', colorized=magenta)
@@ -82,14 +86,20 @@
 
 def handle_exception(exc: Exception, logger: logging.Logger, status: int) -> int:
     """Log the exception argument and exit with `status`."""
     logger.critical(f'{exc.__class__.__name__}: ' + str(exc).replace('\n', ' - '))
     return status
 
 
+def handle_exception_silently(exc: Exception) -> int:
+    """Return status held by `exc.args` without logging."""
+    status, = exc.args
+    return status
+
+
 def handle_address_unknown(exc: Exception,  # noqa: unused
                            logger: logging.Logger,
                            status: int = exit_status.runtime_error) -> int:
     """Could not get address info for hostname (see `socket.gaierror`)."""
     logger.critical(f'{exc.__class__.__name__}: {exc}')
     return status
```

### Comparing `hyper-shell-2.3.0/src/hypershell/core/fsm.py` & `hyper-shell-2.4.0/src/hypershell/core/fsm.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 
 # type annotations
 from __future__ import annotations
 from typing import Dict, Callable, Type
 
 # standard libs
+# import time  # NOTE: commented section below
+# import random
 from enum import Enum
 from abc import ABC
 
 # internal libs
 from hypershell.core.exceptions import write_traceback
 from hypershell.core.logging import Logger
 
@@ -46,14 +48,16 @@
                 action = self.actions.get(previous_state)
                 next_state = action()
         except Exception as error:
             log.critical(f'Uncaught exception from {self.__class__}')
             write_traceback(error, logger=log, module=__name__)
             raise
         else:
+            # NOTE: Development aids not typically engaged
+            # time.sleep(random.uniform(0, 5))  # FUZZ
             log.devel(f'{self.__class__.__name__}: {previous_state} -> {next_state}')
             return next_state
 
     def run(self) -> None:
         """Run machine until state is set to `HALT`."""
         while self.state is not self.states.HALT:  # noqa: HALT defined in implemented State enums
             self.state = self.next()
```

### Comparing `hyper-shell-2.3.0/src/hypershell/core/heartbeat.py` & `hyper-shell-2.4.0/src/hypershell/core/heartbeat.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 from enum import Enum
 from datetime import datetime
 from dataclasses import dataclass
 
 # internal libs
 from hypershell.core.logging import HOSTNAME, INSTANCE
 
+# public interface
+__all__ = ['ClientState', 'Heartbeat']
+
 
 class ClientState(Enum):
     """Client state."""
 
     RUNNING = 0
     FINISHED = 1
 
@@ -44,15 +47,15 @@
             uuid: str = None,
             host: str = None,
             time: datetime = None,
             state: ClientState = None) -> Heartbeat:
         """Create new instance."""
         return cls(uuid=(uuid or INSTANCE),
                    host=(host or HOSTNAME),
-                   time=(time or datetime.now()),
+                   time=(time or datetime.now().astimezone()),
                    state=(state or ClientState.RUNNING))
 
     def pack(self: Heartbeat) -> bytes:
         """Serialize data."""
         return json.dumps({'uuid': self.uuid,
                            'host': self.host,
                            'time': str(self.time),
```

### Comparing `hyper-shell-2.3.0/src/hypershell/core/logging.py` & `hyper-shell-2.4.0/src/hypershell/core/logging.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import datetime
 
 # external libs
 from cmdkit.app import exit_status
 from cmdkit.config import ConfigurationError
 
 # internal libs
-from hypershell.core.ansi import Ansi
+from hypershell.core.ansi import Ansi, COLOR_STDERR
 from hypershell.core.config import config, blame
 from hypershell.core.exceptions import write_traceback
 
 # public interface
 __all__ = ['Logger', 'HOSTNAME', 'INSTANCE', 'handler', 'initialize_logging', ]
 
 
@@ -102,40 +102,40 @@
         reltime_delta,
         f'{reltime_delta.days:02d}-{reltime_delta_hours:02d}:{reltime_delta_minutes:02d}:'
         f'{reltime_delta_seconds:02d}.{reltime_delta_milliseconds:03d}'
     )
 
 
 class LogRecord(logging.LogRecord):
-    """Extends LogRecord to include the hostname and ANSI color codes."""
+    """Extends LogRecord to include ANSI colors, time formats, and other attributes."""
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
         # Context attributes
         self.app_id = INSTANCE
         self.hostname = HOSTNAME
         self.hostname_short = HOSTNAME_SHORT
         self.relative_name = self.name.split('.', 1)[-1]
 
         # Formatting attributes
-        self.ansi_level = level_color.get(self.levelname, Ansi.NULL).value
-        self.ansi_reset = Ansi.RESET.value
-        self.ansi_bold = Ansi.BOLD.value
-        self.ansi_faint = Ansi.FAINT.value
-        self.ansi_italic = Ansi.ITALIC.value
-        self.ansi_underline = Ansi.UNDERLINE.value
-        self.ansi_black = Ansi.BLACK.value
-        self.ansi_red = Ansi.RED.value
-        self.ansi_green = Ansi.GREEN.value
-        self.ansi_yellow = Ansi.YELLOW.value
-        self.ansi_blue = Ansi.BLUE.value
-        self.ansi_magenta = Ansi.MAGENTA.value
-        self.ansi_cyan = Ansi.CYAN.value
-        self.ansi_white = Ansi.WHITE.value
+        self.ansi_level = level_color.get(self.levelname, Ansi.NULL).value if COLOR_STDERR else ''
+        self.ansi_reset = Ansi.RESET.value if COLOR_STDERR else ''
+        self.ansi_bold = Ansi.BOLD.value if COLOR_STDERR else ''
+        self.ansi_faint = Ansi.FAINT.value if COLOR_STDERR else ''
+        self.ansi_italic = Ansi.ITALIC.value if COLOR_STDERR else ''
+        self.ansi_underline = Ansi.UNDERLINE.value if COLOR_STDERR else ''
+        self.ansi_black = Ansi.BLACK.value if COLOR_STDERR else ''
+        self.ansi_red = Ansi.RED.value if COLOR_STDERR else ''
+        self.ansi_green = Ansi.GREEN.value if COLOR_STDERR else ''
+        self.ansi_yellow = Ansi.YELLOW.value if COLOR_STDERR else ''
+        self.ansi_blue = Ansi.BLUE.value if COLOR_STDERR else ''
+        self.ansi_magenta = Ansi.MAGENTA.value if COLOR_STDERR else ''
+        self.ansi_cyan = Ansi.CYAN.value if COLOR_STDERR else ''
+        self.ansi_white = Ansi.WHITE.value if COLOR_STDERR else ''
 
         # Timing attributes
         (self.elapsed,
          self.elapsed_ms,
          self.elapsed_delta,
          self.elapsed_hms) = solve_relative_time(self.relativeCreated / 1000)
```

### Comparing `hyper-shell-2.3.0/src/hypershell/core/platform.py` & `hyper-shell-2.4.0/src/hypershell/core/platform.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,10 +74,19 @@
 if 'HYPERSHELL_SITE' in os.environ:
     default_path = path.local
 else:
     default_path = path.user if not is_admin else path.system
 
 
 # Automatically initialize default site directories
-os.makedirs(default_path.lib, exist_ok=True)
-os.makedirs(default_path.log, exist_ok=True)
-os.makedirs(os.path.join(default_path.lib, 'task'), exist_ok=True)
+default_dirs = [
+    default_path.lib,
+    default_path.log,
+    os.path.join(default_path.lib, 'task'),
+]
+
+
+for default_dir in default_dirs:
+    try:
+        os.makedirs(default_dir, exist_ok=True)
+    except PermissionError:
+        pass
```

### Comparing `hyper-shell-2.3.0/src/hypershell/core/queue.py` & `hyper-shell-2.4.0/src/hypershell/core/queue.py`

 * *Files identical despite different names*

### Comparing `hyper-shell-2.3.0/src/hypershell/core/remote.py` & `hyper-shell-2.4.0/src/hypershell/core/remote.py`

 * *Files identical despite different names*

### Comparing `hyper-shell-2.3.0/src/hypershell/core/template.py` & `hyper-shell-2.4.0/src/hypershell/core/template.py`

 * *Files identical despite different names*

### Comparing `hyper-shell-2.3.0/src/hypershell/core/thread.py` & `hyper-shell-2.4.0/src/hypershell/core/thread.py`

 * *Files identical despite different names*

### Comparing `hyper-shell-2.3.0/src/hypershell/core/types.py` & `hyper-shell-2.4.0/src/hypershell/core/types.py`

 * *Files identical despite different names*

### Comparing `hyper-shell-2.3.0/src/hypershell/database/__init__.py` & `hyper-shell-2.4.0/src/hypershell/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
 # internal libs
 from hypershell.core.ansi import colorize_usage
 from hypershell.core.logging import Logger
 from hypershell.core.config import config
 from hypershell.core.exceptions import (write_traceback, handle_exception, DatabaseUninitialized,
                                         get_shared_exception_mapping)
-from hypershell.database.core import engine, in_memory, schema
-from hypershell.database.model import Model, Task
+from hypershell.data.core import engine, in_memory, schema
+from hypershell.data.model import Entity, Task
 
 # public interface
 __all__ = ['InitDBApp', 'initdb', 'truncatedb', 'checkdb', 'ensuredb', 'DATABASE_ENABLED', ]
 
 # initialize logger
 log = Logger.with_name(__name__)
 
@@ -43,25 +43,25 @@
 except Exception as error:
     write_traceback(error, module=__name__)
     sys.exit(exit_status.bad_config)
 
 
 def initdb() -> None:
     """Initialize database tables."""
-    Model.metadata.create_all(engine)
+    Entity.metadata.create_all(engine)
 
 
 def truncatedb() -> None:
     """Truncate database tables."""
     # NOTE: We still might hang here if other sessions exist outside this app instance
     close_all_sessions()
     log.trace('Dropping all tables')
-    Model.metadata.drop_all(engine)
+    Entity.metadata.drop_all(engine)
     log.trace('Creating all tables')
-    Model.metadata.create_all(engine)
+    Entity.metadata.create_all(engine)
     log.warning(f'Truncated database')
 
 
 def checkdb() -> None:
     """Ensure database connection and tables exist."""
     if not inspect(engine).has_table('task', schema=schema):
         raise DatabaseUninitialized('Use \'initdb\' to initialize the database')
```

### Comparing `hyper-shell-2.3.0/src/hypershell/database/core.py` & `hyper-shell-2.4.0/src/hypershell/data/core.py`

 * *Files identical despite different names*

### Comparing `hyper-shell-2.3.0/src/hypershell/server.py` & `hyper-shell-2.4.0/src/hypershell/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 from hypershell.core.exceptions import get_shared_exception_mapping
 from hypershell.core.config import config, default
 from hypershell.core.logging import Logger
 from hypershell.core.fsm import State, StateMachine
 from hypershell.core.thread import Thread
 from hypershell.core.queue import QueueServer, QueueConfig
 from hypershell.core.heartbeat import Heartbeat, ClientState
-from hypershell.database.model import Task
-from hypershell.database import ensuredb, DATABASE_ENABLED
+from hypershell.data.model import Task, Client
+from hypershell.data import ensuredb, DATABASE_ENABLED
 from hypershell.submit import SubmitThread, LiveSubmitThread, DEFAULT_BUNDLEWAIT
 from hypershell.client import ClientInfo
 
 # public interface
 __all__ = ['serve_from', 'serve_file', 'serve_forever', 'ServerThread', 'ServerApp',
            'DEFAULT_BUNDLESIZE', 'DEFAULT_ATTEMPTS', ]
 
@@ -444,15 +444,15 @@
     state = HeartbeatState.START
     states = HeartbeatState
 
     def __init__(self: HeartMonitor, queue: QueueServer, evict_after: int = DEFAULT_EVICT,
                  in_memory: bool = False, no_confirm: bool = False) -> None:
         """Initialize with queue server."""
         self.queue = queue
-        self.last_check = datetime.now()
+        self.last_check = datetime.now().astimezone()
         self.beats = {}
         self.in_memory = in_memory
         self.no_confirm = no_confirm
         if evict_after >= 10:
             self.wait_check = timedelta(seconds=int(evict_after / 10))
             self.evict_after = timedelta(seconds=evict_after)
         else:
@@ -492,33 +492,37 @@
 
     def update_client(self: HeartMonitor) -> HeartbeatState:
         """Update client with heartbeat or disconnect."""
         hb = self.latest_heartbeat
         if hb.state is not ClientState.FINISHED:
             if hb.uuid not in self.beats:
                 log.debug(f'Registered client ({hb.host}: {hb.uuid})')
+                if not self.in_memory:
+                    Client.add(Client.from_heartbeat(hb))
             else:
                 log.trace(f'Heartbeat - running ({hb.host}: {hb.uuid})')
             self.beats[hb.uuid] = hb
             return HeartbeatState.SWITCH
         else:
             log.trace(f'Client disconnected ({hb.host}: {hb.uuid})')
             if hb.uuid in self.beats:
                 self.beats.pop(hb.uuid)
+                if not self.in_memory:
+                    Client.update(hb.uuid, disconnected_at=datetime.now().astimezone())
             return HeartbeatState.SWITCH
 
     def switch_mode(self: HeartMonitor) -> HeartbeatState:
         """Decide to bail, signal, check, or get another heartbeat."""
         if self.startup_phase:
             return HeartbeatState.NEXT
         if self.should_signal:
             return HeartbeatState.SIGNAL
         if not self.beats and self.scheduler_done:
             return HeartbeatState.FINAL
-        now = datetime.now()
+        now = datetime.now().astimezone()
         if (now - self.last_check) > self.wait_check:
             self.last_check = now
             return HeartbeatState.CHECK
         else:
             return HeartbeatState.NEXT
 
     def check_clients(self: HeartMonitor) -> HeartbeatState:
@@ -526,14 +530,16 @@
         log.debug(f'Checking clients ({len(self.beats)} connected)')
         for uuid in list(self.beats):
             hb = self.beats.get(uuid)
             age = self.last_check - hb.time
             if age > self.evict_after:
                 log.warning(f'Evicting client ({hb.host}: {uuid})')
                 self.beats.pop(uuid)
+                if not self.in_memory:
+                    Client.update(hb.uuid, disconnected_at=datetime.now().astimezone(), evicted=True)
                 if not self.in_memory and not self.no_confirm:
                     log.warning(f'Reverting orphaned tasks ({hb.host}: {uuid})')
                     Task.revert_orphaned(uuid)
         return HeartbeatState.SWITCH
 
     def signal_clients(self: HeartMonitor) -> HeartbeatState:
         """Send shutdown signal to all connected clients."""
```

### Comparing `hyper-shell-2.3.0/src/hypershell/submit.py` & `hyper-shell-2.4.0/src/hypershell/submit.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,16 +60,17 @@
 from hypershell.core.logging import Logger
 from hypershell.core.config import config, default
 from hypershell.core.fsm import State, StateMachine
 from hypershell.core.queue import QueueClient, QueueConfig
 from hypershell.core.thread import Thread
 from hypershell.core.template import Template, DEFAULT_TEMPLATE
 from hypershell.core.exceptions import get_shared_exception_mapping
-from hypershell.database.model import Task
-from hypershell.database import initdb, checkdb
+from hypershell.data.model import Task
+from hypershell.data import initdb, checkdb
+from hypershell.task import Tag
 
 # public interface
 __all__ = ['submit_from', 'submit_file', 'SubmitThread', 'LiveSubmitThread',
            'SubmitApp', 'DEFAULT_BUNDLESIZE', 'DEFAULT_BUNDLEWAIT']
 
 # initialize logger
 log = Logger.with_name(__name__)
@@ -88,23 +89,29 @@
     """Enqueue tasks from iterable source."""
 
     task: Task
     source: Iterator[str]
     queue: Queue[Optional[Task]]
     template: Template
     count: int
+    tags: Dict[str, str]
 
     state = LoaderState.START
     states = LoaderState
 
-    def __init__(self: Loader, source: Iterable[str], queue: Queue[Optional[Task]], template: str = DEFAULT_TEMPLATE) -> None:
+    def __init__(self: Loader,
+                 source: Iterable[str],
+                 queue: Queue[Optional[Task]],
+                 template: str = DEFAULT_TEMPLATE,
+                 tags: Dict[str, str] = None) -> None:
         """Initialize source to read tasks and submit to database."""
         self.template = Template(template)
         self.source = map(self.template.expand, map(str.strip, map(str, source)))
         self.queue = queue
+        self.tags = tags
         self.count = 0
 
     @functools.cached_property
     def actions(self: Loader) -> Dict[LoaderState, Callable[[], LoaderState]]:
         return {
             LoaderState.START: self.start,
             LoaderState.GET: self.get_task,
@@ -117,15 +124,15 @@
         """Jump to GET state."""
         log.debug('Started (loader)')
         return LoaderState.GET
 
     def get_task(self: Loader) -> LoaderState:
         """Get the next task from the source."""
         try:
-            self.task = Task.new(args=next(self.source))
+            self.task = Task.new(args=next(self.source), tag=self.tags)
             log.trace(f'Loaded task ({self.task.args})')
             return LoaderState.PUT
         except StopIteration:
             return LoaderState.FINAL
 
     def put_task(self: Loader) -> LoaderState:
         """Enqueue loaded task."""
@@ -145,18 +152,19 @@
 
 class LoaderThread(Thread):
     """Run loader within dedicated thread."""
 
     def __init__(self: LoaderThread,
                  source: Iterable[str],
                  queue: Queue[Optional[Task]],
-                 template: str = DEFAULT_TEMPLATE) -> None:
+                 template: str = DEFAULT_TEMPLATE,
+                 tags: Dict[str, str] = None) -> None:
         """Initialize machine."""
         super().__init__(name='hypershell-submit-loader')
-        self.machine = Loader(source=source, queue=queue, template=template)
+        self.machine = Loader(source=source, queue=queue, template=template, tags=tags)
 
     def run_with_exceptions(self: LoaderThread) -> None:
         """Run machine."""
         self.machine.run()
 
     def stop(self: LoaderThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
@@ -274,19 +282,20 @@
 
     source: Iterable[str]
     queue: Queue[Optional[Task]]
     loader: LoaderThread
     committer: DatabaseCommitterThread
 
     def __init__(self: SubmitThread, source: Iterable[str], bundlesize: int = DEFAULT_BUNDLESIZE,
-                 bundlewait: int = DEFAULT_BUNDLEWAIT, template: str = DEFAULT_TEMPLATE) -> None:
+                 bundlewait: int = DEFAULT_BUNDLEWAIT, template: str = DEFAULT_TEMPLATE,
+                 tags: Dict[str, str] = None) -> None:
         """Initialize queue and child threads."""
         self.source = source
         self.queue = Queue(maxsize=bundlesize)
-        self.loader = LoaderThread(source=source, queue=self.queue, template=template)
+        self.loader = LoaderThread(source=source, queue=self.queue, template=template, tags=tags)
         self.committer = DatabaseCommitterThread(queue=self.queue, bundlesize=bundlesize, bundlewait=bundlewait)
         super().__init__(name='hypershell-submit')
 
     def run_with_exceptions(self: SubmitThread) -> None:
         """Start child threads, wait."""
         log.debug(f'Started ({self.source_name})')
         self.loader.start()
@@ -448,19 +457,20 @@
     committer: QueueCommitterThread
 
     def __init__(self: LiveSubmitThread,
                  source: Iterable[str],
                  queue_config: QueueConfig,
                  template: str = DEFAULT_TEMPLATE,
                  bundlesize: int = DEFAULT_BUNDLESIZE,
-                 bundlewait: int = DEFAULT_BUNDLEWAIT) -> None:
+                 bundlewait: int = DEFAULT_BUNDLEWAIT,
+                 tags: Dict[str, str] = None) -> None:
         """Initialize queue and child threads."""
         self.source = source
         self.local = Queue(maxsize=bundlesize)
-        self.loader = LoaderThread(source=source, queue=self.local, template=template)
+        self.loader = LoaderThread(source=source, queue=self.local, template=template, tags=tags)
         self.client = QueueClient(config=queue_config)
         self.committer = QueueCommitterThread(local=self.local, client=self.client,
                                               bundlesize=bundlesize, bundlewait=bundlewait)
         super().__init__(name='hypershell-submit')
 
     def run_with_exceptions(self: LiveSubmitThread) -> None:
         """Start child threads, wait."""
@@ -497,22 +507,22 @@
     def task_count(self: LiveSubmitThread) -> int:
         """Count of submitted tasks."""
         return self.loader.machine.count
 
 
 def submit_from(source: Iterable[str], queue_config: QueueConfig = None,
                 bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT,
-                template: str = DEFAULT_TEMPLATE) -> int:
+                template: str = DEFAULT_TEMPLATE, tags: Dict[str, str] = None) -> int:
     """Submit all task arguments from `source`, return count of submitted tasks."""
     if not queue_config:
         thread = SubmitThread.new(source=source, bundlesize=bundlesize, bundlewait=bundlewait,
-                                  template=template)
+                                  template=template, tags=tags)
     else:
         thread = LiveSubmitThread.new(source=source, queue_config=queue_config, template=template,
-                                      bundlesize=bundlesize, bundlewait=bundlewait)
+                                      bundlesize=bundlesize, bundlewait=bundlewait, tags=tags)
     try:
         thread.join()
     except Exception:
         thread.stop()
         raise
     else:
         return thread.task_count
@@ -526,31 +536,32 @@
         return submit_from(stream, queue_config=queue_config, bundlesize=bundlesize,
                            bundlewait=bundlewait, template=template)
 
 
 APP_NAME = 'hyper-shell submit'
 APP_USAGE = f"""\
 Usage:
-{APP_NAME} [-h] [FILE] [-b NUM] [-w SEC] [-t CMD] [--initdb]
+{APP_NAME} [-h] [FILE] [-b NUM] [-w SEC] [-t CMD] [--initdb] [--tag TAG [TAG...]]
 
 Submit tasks from a file.\
 """
 
 APP_HELP = f"""\
 {APP_USAGE}
 
 Arguments:
-  FILE                    Path to task file ("-" for <stdin>).
+  FILE                       Path to task file ("-" for <stdin>).
 
 Options:
-  -t, --template     CMD  Submit-time template expansion (default: "{DEFAULT_TEMPLATE}").
-  -b, --bundlesize   NUM  Number of lines to buffer (default: {DEFAULT_BUNDLESIZE}).
-  -w, --bundlewait   SEC  Seconds to wait before flushing tasks (default: {DEFAULT_BUNDLEWAIT}).
-      --initdb            Auto-initialize database.
-  -h, --help              Show this message and exit.\
+  -t, --template     CMD     Submit-time template expansion (default: "{DEFAULT_TEMPLATE}").
+  -b, --bundlesize   NUM     Number of lines to buffer (default: {DEFAULT_BUNDLESIZE}).
+  -w, --bundlewait   SEC     Seconds to wait before flushing tasks (default: {DEFAULT_BUNDLEWAIT}).
+      --initdb               Auto-initialize database.
+      --tag          TAG...  Assign tags as `key:value`.
+  -h, --help                 Show this message and exit.\
 """
 
 
 class SubmitApp(Application):
     """Submit tasks to the database."""
 
     name = APP_NAME
@@ -570,29 +581,33 @@
 
     template: str = DEFAULT_TEMPLATE
     interface.add_argument('-t', '--template', default=template)
 
     auto_initdb: bool = False
     interface.add_argument('--initdb', action='store_true', dest='auto_initdb')
 
+    taglist: List[str] = None
+    interface.add_argument('--tag', nargs='*', default=[], dest='taglist')
+
     count: int = 0
 
     exceptions = {
         **get_shared_exception_mapping(__name__)
     }
 
     def run(self: SubmitApp) -> None:
         """Run submit thread."""
         self.submit_all()
         log.info(f'Submitted {self.count} tasks')
 
     def submit_all(self: SubmitApp) -> None:
         """Submit all tasks from source."""
         self.count = submit_from(self.source, template=self.template,
-                                 bundlesize=self.bundlesize, bundlewait=self.bundlewait)
+                                 bundlesize=self.bundlesize, bundlewait=self.bundlewait,
+                                 tags=Tag.parse_cmdline_list(self.taglist))
 
     @staticmethod
     def check_config():
         """Halt if we are not connected to database."""
         db = config.database.get('file', None) or config.database.get('database', None)
         if config.database.provider == 'sqlite' and db in ('', ':memory:', None):
             raise ConfigurationError('Submitting tasks to in-memory database has no effect')
```

### Comparing `hyper-shell-2.3.0/src/hypershell/task.py` & `hyper-shell-2.4.0/src/hypershell/task.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,86 +12,91 @@
 import os
 import re
 import sys
 import csv
 import json
 import time
 import functools
+from datetime import timedelta
 from dataclasses import dataclass
 from shutil import copyfileobj
 
 # external libs
 import yaml
 from rich.console import Console
 from rich.syntax import Syntax
 from rich.table import Table
 from cmdkit.app import Application, ApplicationGroup, exit_status
 from cmdkit.cli import Interface, ArgumentError
-from sqlalchemy import Column
+from sqlalchemy import Column, type_coerce, JSON, text
 from sqlalchemy.exc import StatementError
 from sqlalchemy.orm import Query
 from sqlalchemy.orm.exc import StaleDataError
 from sqlalchemy.sql.elements import BinaryExpression
 
 # internal libs
 from hypershell.core.ansi import colorize_usage
 from hypershell.core.platform import default_path
 from hypershell.core.config import config
-from hypershell.core.exceptions import handle_exception
+from hypershell.core.exceptions import handle_exception, handle_exception_silently, get_shared_exception_mapping
 from hypershell.core.logging import Logger, HOSTNAME
 from hypershell.core.remote import SSHConnection
 from hypershell.core.types import smart_coerce
-from hypershell.core.exceptions import get_shared_exception_mapping
-from hypershell.database.model import Task, to_json_type
-from hypershell.database import ensuredb
+from hypershell.data.model import Task, to_json_type
+from hypershell.data import ensuredb
 
 # public interface
-__all__ = ['TaskGroupApp', ]
+__all__ = ['TaskGroupApp', 'Tag', ]
 
 # initialize logger
 log = Logger.with_name(__name__)
 
 
 SUBMIT_PROGRAM = 'hyper-shell task submit'
 SUBMIT_USAGE = f"""\
 Usage:
-{SUBMIT_PROGRAM} [-h] ARGS...
+{SUBMIT_PROGRAM} [-h] [-t TAG [TAG...]] ARGS...
 
 Submit individual task to database.\
 """
 
 SUBMIT_HELP = f"""\
 {SUBMIT_USAGE}
 
 Arguments:
   ARGS...                Command-line arguments.
 
 Options:
+  -t, --tag    TAG...    Assign tags as `key:value`.
   -h, --help             Show this message and exit.\
 """
 
 
 class TaskSubmitApp(Application):
     """Submit task to database."""
 
     interface = Interface(SUBMIT_PROGRAM,
                           colorize_usage(SUBMIT_USAGE),
                           colorize_usage(SUBMIT_HELP))
 
     argv: List[str] = []
     interface.add_argument('argv', nargs='+')
 
+    taglist: List[str] = []
+    interface.add_argument('-t', '--tag', nargs='*', dest='taglist')
+
     exceptions = {
         **get_shared_exception_mapping(__name__)
     }
 
     def run(self: TaskSubmitApp) -> None:
         """Submit task to database."""
         ensuredb()
-        task = Task.new(args=' '.join(self.argv))
+        task = Task.new(args=' '.join(self.argv),
+                        tag=(None if not self.taglist else Tag.parse_cmdline_list(self.taglist)))
         Task.add(task)
         print(task.id)
 
 
 # Catch bad UUID before we touch the database
 UUID_PATTERN: re.Pattern = re.compile(
     r'^[0-9a-fA-F]{8}\b-[0-9a-fA-F]{4}\b-[0-9a-fA-F]{4}\b-[0-9a-fA-F]{4}\b-[0-9a-fA-F]{12}$'
@@ -103,32 +108,33 @@
     if not UUID_PATTERN.match(value):
         raise ArgumentError(f'Bad UUID: \'{value}\'')
 
 
 INFO_PROGRAM = 'hyper-shell task info'
 INFO_USAGE = f"""\
 Usage: 
-{INFO_PROGRAM} [-h] ID [--yaml | --json | --stdout | --stderr | -x FIELD]
+{INFO_PROGRAM} [-h] ID [--stdout | --stderr | -x FIELD] [-f FORMAT]
 
 Get metadata and/or task outputs.\
 """
 
 INFO_HELP = f"""\
 {INFO_USAGE}
 
 Arguments:
-  ID                    Unique task UUID.
+  ID                     Unique task UUID.
 
 Options:
-      --yaml            Format task metadata as YAML.
-      --json            Format task metadata as JSON.
-  -x, --extract  FIELD  Print single field.
-      --stdout          Fetch <stdout> from task.
-      --stderr          Fetch <stderr> from task.
-  -h, --help            Show this message and exit.\
+  -f, --format   FORMAT  Format task info ([normal], json, yaml).
+      --json             Format task metadata as JSON.
+      --yaml             Format task metadata as YAML.
+  -x, --extract  FIELD   Print single field.
+      --stdout           Print <stdout> from task.
+      --stderr           Print <stderr> from task.
+  -h, --help             Show this message and exit.\
 """
 
 
 class TaskInfoApp(Application):
     """Get metadata/status/outputs of task."""
 
     interface = Interface(INFO_PROGRAM,
@@ -137,23 +143,25 @@
 
     uuid: str
     interface.add_argument('uuid')
 
     print_stdout: bool = False
     print_stderr: bool = False
     extract_field: str = None
+    print_interface = interface.add_mutually_exclusive_group()
+    print_interface.add_argument('--stdout', action='store_true', dest='print_stdout')
+    print_interface.add_argument('--stderr', action='store_true', dest='print_stderr')
+    print_interface.add_argument('-x', '--extract', default=None, choices=Task.columns, dest='extract_field')
+
     output_format: str = 'normal'
     output_formats: List[str] = ['normal', 'json', 'yaml']
     output_interface = interface.add_mutually_exclusive_group()
-    output_interface.add_argument('--format', default=output_format, dest='output_format', choices=output_formats)
+    output_interface.add_argument('-f', '--format', default=output_format, dest='output_format', choices=output_formats)
     output_interface.add_argument('--json', action='store_const', const='json', dest='output_format')
     output_interface.add_argument('--yaml', action='store_const', const='yaml', dest='output_format')
-    output_interface.add_argument('--stdout', action='store_true', dest='print_stdout')
-    output_interface.add_argument('--stderr', action='store_true', dest='print_stderr')
-    output_interface.add_argument('-x', '--extract', default=None, choices=Task.columns, dest='extract_field')
 
     exceptions = {
         Task.NotFound: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
         **get_shared_exception_mapping(__name__)
     }
 
     def run(self: TaskInfoApp) -> None:
@@ -169,15 +177,27 @@
         elif self.output_format == 'normal':
             print_normal(self.task)
         else:
             self.print_formatted()
 
     def print_field(self: TaskInfoApp) -> None:
         """Print single field."""
-        print(json.dumps(self.task.to_json().get(self.extract_field)).strip('"'))
+        if self.extract_field != 'tag':
+            print(json.dumps(self.task.to_json().get(self.extract_field)).strip('"'))
+        elif self.output_format == 'normal':
+            print(', '.join(f'{k}:{v}' if v else k for k, v in self.task.tag.items()))
+        else:
+            formatter = self.format_method[self.output_format]
+            output = formatter(self.task.tag)
+            if sys.stdout.isatty():
+                output = Syntax(output, self.output_format, word_wrap=True,
+                                theme=config.console.theme, background_color='default')
+                Console().print(output)
+            else:
+                print(output, file=sys.stdout, flush=True)
 
     def print_formatted(self: TaskInfoApp) -> None:
         """Format and print task metadata to console."""
         formatter = self.format_method[self.output_format]
         output = formatter(self.task.to_json())  # NOTE: to_json() just means dict with converted value types
         if sys.stdout.isatty():
             output = Syntax(output, self.output_format, word_wrap=True,
@@ -229,31 +249,34 @@
 # Time to wait between database queries
 DEFAULT_INTERVAL = 5
 
 
 WAIT_PROGRAM = 'hyper-shell task wait'
 WAIT_USAGE = f"""\
 Usage: 
-{WAIT_PROGRAM} [-h] ID [-n SEC] [--info [--json] | --status]
+{WAIT_PROGRAM} [-h] ID [-n SEC] [--info [-f FORMAT] | --status | --return]
 
 Wait for task to complete.\
 """
 
 WAIT_HELP = f"""\
 {WAIT_USAGE}
 
 Arguments:
-  ID                    Unique UUID.
+  ID                     Unique UUID.
 
 Options:
-  -n, --interval  SEC   Time to wait between polling (default: {DEFAULT_INTERVAL}).
-      --info            Print info on task.
-      --json            Format info as JSON.
-      --status          Print exit status for task.
-  -h, --help            Show this message and exit.\
+  -n, --interval  SEC    Time to wait between polling (default: {DEFAULT_INTERVAL}).
+  -i, --info             Print info on task.
+  -f, --format   FORMAT  Format task info ([normal], json, yaml).
+      --json             Format info as JSON.
+      --yaml             Format info as YAML.
+  -s, --status           Print exit status for task.
+  -r, --return           Use exit status from task.
+  -h, --help             Show this message and exit.\
 """
 
 
 class TaskWaitApp(Application):
     """Wait for task to complete."""
 
     interface = Interface(WAIT_PROGRAM,
@@ -263,35 +286,50 @@
     uuid: str
     interface.add_argument('uuid')
 
     interval: int = DEFAULT_INTERVAL
     interface.add_argument('-n', '--interval', type=int, default=interval)
 
     print_info: bool = False
-    format_json: bool = False
     print_status: bool = False
+    return_status: bool = False
+    print_interface = interface.add_mutually_exclusive_group()
+    print_interface.add_argument('-i', '--info', action='store_true', dest='print_info')
+    print_interface.add_argument('-s', '--status', action='store_true', dest='print_status')
+    print_interface.add_argument('-r', '--return', action='store_true', dest='return_status')
+
+    output_format: str = 'normal'
+    output_formats: List[str] = ['normal', 'json', 'yaml']
     output_interface = interface.add_mutually_exclusive_group()
-    output_interface.add_argument('--info', action='store_true', dest='print_info')
-    output_interface.add_argument('--json', action='store_true', dest='format_json')
-    output_interface.add_argument('--status', action='store_true', dest='print_status')
+    output_interface.add_argument('-f', '--format', default=output_format,
+                                  dest='output_format', choices=output_formats)
+    output_interface.add_argument('--json', action='store_const', const='json', dest='output_format')
+    output_interface.add_argument('--yaml', action='store_const', const='yaml', dest='output_format')
+
+    class NonZeroStatus(Exception):
+        """Exception holds non-zero exit status of returned task."""
 
     exceptions = {
         Task.NotFound: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
+        NonZeroStatus: handle_exception_silently,
         **get_shared_exception_mapping(__name__)
     }
 
     def run(self: TaskWaitApp) -> None:
         """Wait for task to complete."""
         ensuredb()
         check_uuid(self.uuid)
         self.wait_task()
-        if self.print_info or self.format_json:
-            TaskInfoApp(uuid=self.uuid, format_json=self.format_json).run()
+        if self.print_info:
+            TaskInfoApp(uuid=self.uuid, output_format=self.output_format).run()
         elif self.print_status:
             TaskInfoApp(uuid=self.uuid, extract_field='exit_status').run()
+        elif self.return_status:
+            if status := Task.from_id(self.uuid).exit_status:
+                raise self.NonZeroStatus(status)
 
     def wait_task(self: TaskWaitApp):
         """Wait for the task to complete."""
         log.info(f'Waiting on task ({self.uuid})')
         while True:
             task = Task.from_id(self.uuid, caching=False)
             if task.exit_status is None:
@@ -350,37 +388,38 @@
         TaskInfoApp(uuid=task.id, print_stdout=True).run()
         TaskInfoApp(uuid=task.id, print_stderr=True).run()
 
 
 SEARCH_PROGRAM = 'hyper-shell task search'
 SEARCH_USAGE = f"""\
 Usage:
-hyper-shell task search [-h] [FIELD [FIELD ...]] [--where COND [COND ...]] 
+hyper-shell task search [-h] [FIELD [FIELD ...]] [-w COND [COND ...]] [-t TAG [TAG...]]
                         [--order-by FIELD [--desc]] [--count | --limit NUM]
                         [--format FORMAT | --json | --csv]  [-d CHAR]
                         
 Search for tasks in the database.\
 """
 
 SEARCH_HELP = f"""\
 {SEARCH_USAGE}
 
 Arguments:
   FIELD                      Select specific named fields.
 
 Options:
   -w, --where      COND...   List of conditional statements.
+  -t, --with-tag   TAG...    List of tags.
   -s, --order-by   FIELD     Order output by field.
-      --failed               Alias for "exit_status != 0"
-      --succeeded            Alias for "exit_status == 0"
-      --finished             Alias for "exit_status != null"
-      --remaining            Alias for "exit_status == null"
-      --json                 Format output as JSON.
-      --csv                  Format output as CSV.
+      --failed               Alias for `exit_status != 0`
+      --succeeded            Alias for `exit_status == 0`
+      --finished             Alias for `exit_status != null`
+      --remaining            Alias for `exit_status == null`
       --format     FORMAT    Format output (normal, plain, table, csv, json).
+      --json                 Format output as JSON (alias for `--format=json`).
+      --csv                  Format output as CSV (alias for `--format=csv`.
   -d, --delimiter  CHAR      Field seperator for plain/csv formats.
   -l, --limit      NUM       Limit the number of results.
   -c, --count                Show count of results.
   -h, --help                 Show this message and exit.\
 """
 
 
@@ -401,14 +440,17 @@
 
     field_names: List[str] = ALL_FIELDS
     interface.add_argument('field_names', nargs='*', default=field_names)
 
     where_clauses: List[str] = None
     interface.add_argument('-w', '--where', nargs='*', default=[], dest='where_clauses')
 
+    taglist: List[str] = None
+    interface.add_argument('-t', '--with-tag', nargs='*', default=[], dest='taglist')
+
     order_by: str = None
     order_desc: bool = False
     interface.add_argument('-s', '--order-by', default=None, choices=field_names)
     interface.add_argument('--desc', action='store_true', dest='order_desc')
 
     limit: int = None
     interface.add_argument('-l', '--limit', type=int, default=None)
@@ -450,26 +492,54 @@
             print(self.build_query().count())
         else:
             self.print_output(self.build_query().all())
 
     def build_query(self: TaskSearchApp) -> Query:
         """Build original query interface."""
         query = Task.query(*self.fields)
+        query = self.__build_order_by_clause(query)
+        query = self.__build_where_clause(query)
+        query = self.__build_where_clause_for_tags(query)
+        return query.limit(self.limit)
+
+    def __build_where_clause_for_tags(self: TaskSearchApp, query: Query) -> Query:
+        """Add JSON-based tag where-clauses to query if necessary."""
+        tags_name_only = []
+        tags_with_value = Tag.parse_cmdline_list(self.taglist)
+        for name in list(tags_with_value.keys()):
+            if not tags_with_value[name]:
+                tags_name_only.append(name)
+                tags_with_value.pop(name)
+        for name in tags_name_only:
+            if config.database.provider == 'sqlite':
+                # NOTE: sqlalchemy adds `json_quote(json_extract(task.tag, ?)) is not null`
+                # and cannot find a way to exclude `json_quote`, so we do it ourselves
+                query = query.filter(text('json_extract(task.tag, :tag) is not null')).params(tag=f'$."{name}"')
+            else:
+                query = query.filter(Task.tag[name].isnot(None))
+        for name, value in tags_with_value.items():
+            query = query.filter(Task.tag[name] == type_coerce(str(value), JSON))
+        return query
+
+    def __build_where_clause(self: TaskSearchApp, query: Query) -> Query:
+        """Add explicit where-clauses to query if necessary."""
+        for where_clause in self.__build_filters():
+            query = query.filter(where_clause.compile())
+        return query
+
+    def __build_order_by_clause(self: TaskSearchApp, query: Query) -> Query:
+        """Add order by clause to query if necessary."""
         if self.order_by:
             field = getattr(Task, self.order_by)
             if self.order_desc:
                 field = field.desc()
             query = query.order_by(field)
-        for where_clause in self.build_filters():
-            query = query.filter(where_clause.compile())
-        if self.limit:
-            query = query.limit(self.limit)
         return query
 
-    def build_filters(self: TaskSearchApp) -> List[WhereClause]:
+    def __build_filters(self: TaskSearchApp) -> List[WhereClause]:
         """Create list of field selectors from command-line arguments."""
         if self.show_failed:
             self.where_clauses.append('exit_status != 0')
         if self.show_succeeded:
             self.where_clauses.append('exit_status == 0')
         if self.show_finished:
             self.where_clauses.append('exit_status != null')
@@ -594,27 +664,37 @@
     uuid: str
     interface.add_argument('uuid')
 
     field: str
     interface.add_argument('field', choices=list(Task.columns)[1:])  # NOTE: not ID!
 
     value: str
-    interface.add_argument('value', type=smart_coerce)
+    interface.add_argument('value')
 
     exceptions = {
         Task.NotFound: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
         **get_shared_exception_mapping(__name__)
     }
 
     def run(self: TaskUpdateApp) -> None:
         """Update individual task attribute directly."""
         ensuredb()
         check_uuid(self.uuid)
         try:
-            Task.update(self.uuid, **{self.field: self.value, })
+            if self.field == 'tag':
+                Task.update(self.uuid, tag={**Task.from_id(self.uuid).tag,
+                                            **Tag.parse_cmdline_list([self.value, ])})
+            else:
+                if Task.columns.get(self.field) is str:
+                    # We want to coerce the value (e.g., as an int or None)
+                    # But also allow for, e.g., args==1 which expects type str.
+                    value = None if self.value.lower() in {'none', 'null'} else self.value
+                else:
+                    value = smart_coerce(self.value)
+                Task.update(self.uuid, **{self.field: value, })
         except StaleDataError as err:
             raise Task.NotFound(str(err)) from err
 
 
 TASK_PROGRAM = 'hyper-shell task'
 TASK_USAGE = f"""\
 Usage: 
@@ -691,31 +771,67 @@
         Example:
             >>> WhereClause.from_cmdline('exit_status != 0')
             WhereClause(field='exit_status', value=0, operand='!=')
         """
         match = cls.pattern.match(argument)
         if match:
             field, operand, value = match.groups()
-            return WhereClause(field=field, value=smart_coerce(value), operand=operand)
+            if Task.columns.get(field) is str:
+                # We want to coerce the value (e.g., as an int or None)
+                # But also allow for, e.g., args==1 which expects type str.
+                value = None if value.lower() in {'none', 'null'} else value
+            else:
+                value = smart_coerce(value)
+            return WhereClause(field=field, value=value, operand=operand)
         else:
             raise ArgumentError(f'Where clause not understood ({argument})')
 
 
+@dataclass
+class Tag:
+    """Tag specification.."""
+
+    name: str
+    value: str = ''
+
+    def to_dict(self: Tag) -> Dict[str, str]:
+        """Format tag specification as dictionary."""
+        return {self.name: self.value, }
+
+    @classmethod
+    def from_cmdline(cls: Type[Tag], arg: str) -> Tag:
+        """Construct from command-line `arg`."""
+        tag_part = arg.strip().split(':', 1)
+        if len(tag_part) == 1:
+            return cls(name=tag_part[0].strip())
+        else:
+            return cls(name=tag_part[0].strip(), value=tag_part[1].strip())
+
+    @classmethod
+    def parse_cmdline_list(cls: Type[Tag], args: List[str]) -> Dict[str, Optional[str]]:
+        """Parse command-line list of tags."""
+        return {tag.name: tag.value for tag in map(cls.from_cmdline, args)}
+
+
 def print_normal(task: Task) -> None:
     """Print semi-structured task metadata with all field names."""
     task_data = {k: json.dumps(to_json_type(v)).strip('"') for k, v in task.to_dict().items()}
+    task_data['waited'] = 'null' if not task.waited else timedelta(seconds=int(task_data['waited']))
+    task_data['duration'] = 'null' if not task.duration else timedelta(seconds=int(task_data['duration']))
+    task_data['tag'] = ', '.join(f'{k}:{v}' if v else k for k, v in task.tag.items())
     print(f'          id: {task_data["id"]}')
     print(f'     command: {task_data["command"]} ({task_data["args"]})')
     print(f' exit_status: {task_data["exit_status"]}')
     print(f'   submitted: {task_data["submit_time"]}')
     print(f'   scheduled: {task_data["schedule_time"]}')
-    print(f'     started: {task_data["start_time"]}')
-    print(f'   completed: {task_data["completion_time"]}')
+    print(f'     started: {task_data["start_time"]} (waited: {task_data["waited"]})')
+    print(f'   completed: {task_data["completion_time"]} (duration: {task_data["duration"]})')
     print(f' submit_host: {task_data["submit_host"]} ({task_data["submit_id"]})')
     print(f' server_host: {task_data["server_host"]} ({task_data["server_id"]})')
     print(f' client_host: {task_data["client_host"]} ({task_data["client_id"]})')
     print(f'     attempt: {task_data["attempt"]}')
     print(f'     retried: {task_data["retried"]}')
     print(f'     outpath: {task_data["outpath"]}')
     print(f'     errpath: {task_data["errpath"]}')
     print(f' previous_id: {task_data["previous_id"]}')
     print(f'     next_id: {task_data["next_id"]}')
+    print(f'        tags: {task_data["tag"]}')
```

