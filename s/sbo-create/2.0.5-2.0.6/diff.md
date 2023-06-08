# Comparing `tmp/sbo-create-2.0.5.tar.gz` & `tmp/sbo-create-2.0.6.tar.gz`

## Comparing `sbo-create-2.0.5.tar` & `sbo-create-2.0.6.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-06 17:43:00.000000 sbo-create-2.0.5/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/
--rw-r--r--   0 dslackw   (1000) users      (100)     6461 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/cmake-template.SlackBuild
--rw-r--r--   0 dslackw   (1000) users      (100)     6816 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/autotools-template.SlackBuild
--rw-r--r--   0 dslackw   (1000) users      (100)      521 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/template.info
--rw-r--r--   0 dslackw   (1000) users      (100)     6786 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/meson-template.SlackBuild
--rw-r--r--   0 dslackw   (1000) users      (100)     1047 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)     6138 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/rubygem-template.SlackBuild
--rw-r--r--   0 dslackw   (1000) users      (100)     6018 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/haskell-template.SlackBuild
--rw-r--r--   0 dslackw   (1000) users      (100)     5992 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/perl-template.SlackBuild
--rw-r--r--   0 dslackw   (1000) users      (100)     1803 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      683 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/README
--rw-r--r--   0 dslackw   (1000) users      (100)     5514 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_scripts_templates/python-template.SlackBuild
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-06-06 17:42:54.000000 sbo-create-2.0.5/sbo_create.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       11 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       20 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     3936 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create.egg-info/PKG-INFO
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-06 17:42:34.000000 sbo-create-2.0.5/slackbuild/
--rwxr-xr-x   0 dslackw   (1000) users      (100)     3078 2023-06-06 17:42:34.000000 sbo-create-2.0.5/slackbuild/sbo-create.SlackBuild
--rw-r--r--   0 dslackw   (1000) users      (100)      802 2023-06-06 17:42:34.000000 sbo-create-2.0.5/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      129 2023-06-06 17:42:34.000000 sbo-create-2.0.5/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-06-06 17:42:34.000000 sbo-create-2.0.5/slackbuild/README
--rw-r--r--   0 dslackw   (1000) users      (100)      316 2023-06-06 17:42:34.000000 sbo-create-2.0.5/slackbuild/sbo-create.info
--rwxr-xr-x   0 dslackw   (1000) users      (100)      945 2023-06-06 17:42:34.000000 sbo-create-2.0.5/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3388 2023-06-06 17:42:34.000000 sbo-create-2.0.5/README.rst
--rw-r--r--   0 dslackw   (1000) users      (100)       20 2023-06-06 17:42:34.000000 sbo-create-2.0.5/requirements.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-06-06 17:42:34.000000 sbo-create-2.0.5/LICENSE
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1765 2023-06-06 17:42:34.000000 sbo-create-2.0.5/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)     2422 2023-06-06 17:42:34.000000 sbo-create-2.0.5/ChangeLog.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create/
--rw-r--r--   0 dslackw   (1000) users      (100)    30138 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_create/templates.py
--rw-r--r--   0 dslackw   (1000) users      (100)      350 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_create/__metadata__.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create/__pycache__/
--rw-r--r--   0 dslackw   (1000) users      (100)      154 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dslackw   (1000) users      (100)      580 2023-06-06 17:42:53.000000 sbo-create-2.0.5/sbo_create/__pycache__/__metadata__.cpython-39.pyc
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_create/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)    44512 2023-06-06 17:42:34.000000 sbo-create-2.0.5/sbo_create/main.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-06 17:42:34.000000 sbo-create-2.0.5/bin/
--rwxr-xr-x   0 dslackw   (1000) users      (100)      238 2023-06-06 17:42:34.000000 sbo-create-2.0.5/bin/sbo-create
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-08 19:31:04.000000 sbo-create-2.0.6/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_scripts_templates/
+-rw-r--r--   0 dslackw   (1000) users      (100)     6540 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_scripts_templates/cmake-template.SlackBuild
+-rw-r--r--   0 dslackw   (1000) users      (100)     6895 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_scripts_templates/autotools-template.SlackBuild
+-rw-r--r--   0 dslackw   (1000) users      (100)      525 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_scripts_templates/template.info
+-rw-r--r--   0 dslackw   (1000) users      (100)     6865 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_scripts_templates/meson-template.SlackBuild
+-rw-r--r--   0 dslackw   (1000) users      (100)     1109 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_scripts_templates/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)     6217 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_scripts_templates/rubygem-template.SlackBuild
+-rw-r--r--   0 dslackw   (1000) users      (100)     6097 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_scripts_templates/haskell-template.SlackBuild
+-rw-r--r--   0 dslackw   (1000) users      (100)     6071 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_scripts_templates/perl-template.SlackBuild
+-rw-r--r--   0 dslackw   (1000) users      (100)     5254 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_scripts_templates/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      683 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_scripts_templates/README
+-rw-r--r--   0 dslackw   (1000) users      (100)      182 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_scripts_templates/douninst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)     5778 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_scripts_templates/python-template.SlackBuild
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-08 19:31:01.000000 sbo-create-2.0.6/sbo_create.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-06-08 19:31:01.000000 sbo-create-2.0.6/sbo_create.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-06-08 19:31:01.000000 sbo-create-2.0.6/sbo_create.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       11 2023-06-08 19:31:01.000000 sbo-create-2.0.6/sbo_create.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       20 2023-06-08 19:31:01.000000 sbo-create-2.0.6/sbo_create.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     4132 2023-06-08 19:31:01.000000 sbo-create-2.0.6/sbo_create.egg-info/PKG-INFO
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-08 19:26:22.000000 sbo-create-2.0.6/slackbuild/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     3034 2023-06-08 19:26:22.000000 sbo-create-2.0.6/slackbuild/sbo-create.SlackBuild
+-rw-r--r--   0 dslackw   (1000) users      (100)      802 2023-06-08 19:26:22.000000 sbo-create-2.0.6/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      635 2023-06-08 19:26:22.000000 sbo-create-2.0.6/slackbuild/README
+-rw-r--r--   0 dslackw   (1000) users      (100)      316 2023-06-08 19:26:22.000000 sbo-create-2.0.6/slackbuild/sbo-create.info
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      945 2023-06-08 19:26:22.000000 sbo-create-2.0.6/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3584 2023-06-08 19:26:22.000000 sbo-create-2.0.6/README.rst
+-rw-r--r--   0 dslackw   (1000) users      (100)       20 2023-06-08 19:26:22.000000 sbo-create-2.0.6/requirements.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-06-08 19:26:22.000000 sbo-create-2.0.6/LICENSE
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1765 2023-06-08 19:26:22.000000 sbo-create-2.0.6/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)     2766 2023-06-08 19:26:22.000000 sbo-create-2.0.6/ChangeLog.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-08 19:31:01.000000 sbo-create-2.0.6/sbo_create/
+-rw-r--r--   0 dslackw   (1000) users      (100)    36674 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_create/templates.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      350 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_create/__metadata__.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-08 19:31:01.000000 sbo-create-2.0.6/sbo_create/__pycache__/
+-rw-r--r--   0 dslackw   (1000) users      (100)      154 2023-06-08 19:31:01.000000 sbo-create-2.0.6/sbo_create/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 dslackw   (1000) users      (100)      580 2023-06-08 19:31:01.000000 sbo-create-2.0.6/sbo_create/__pycache__/__metadata__.cpython-39.pyc
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_create/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    46732 2023-06-08 19:26:22.000000 sbo-create-2.0.6/sbo_create/main.py
+-rw-r--r--   0 dslackw   (1000) users      (100)       81 2023-06-08 19:26:22.000000 sbo-create-2.0.6/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-08 19:26:22.000000 sbo-create-2.0.6/bin/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      238 2023-06-08 19:26:22.000000 sbo-create-2.0.6/bin/sbo-create
```

### Comparing `sbo-create-2.0.5/sbo_scripts_templates/cmake-template.SlackBuild` & `sbo-create-2.0.6/sbo_scripts_templates/cmake-template.SlackBuild`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,17 @@
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "i686" ]; then
   SLKCFLAGS="-O2 -march=i686 -mtune=i686"
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "x86_64" ]; then
   SLKCFLAGS="-O2 -fPIC"
   LIBDIRSUFFIX="64"
+elif [ "$ARCH" = "aarch64" ]; then
+  SLKCFLAGS="-O2 -fPIC"
+  LIBDIRSUFFIX="64"
 else
   SLKCFLAGS="-O2"
   LIBDIRSUFFIX=""
 fi
 
 set -e # Exit on most errors
```

### Comparing `sbo-create-2.0.5/sbo_scripts_templates/autotools-template.SlackBuild` & `sbo-create-2.0.6/sbo_scripts_templates/autotools-template.SlackBuild`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,17 @@
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "i686" ]; then
   SLKCFLAGS="-O2 -march=i686 -mtune=i686"
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "x86_64" ]; then
   SLKCFLAGS="-O2 -fPIC"
   LIBDIRSUFFIX="64"
+elif [ "$ARCH" = "aarch64" ]; then
+  SLKCFLAGS="-O2 -fPIC"
+  LIBDIRSUFFIX="64"
 else
   SLKCFLAGS="-O2"
   LIBDIRSUFFIX=""
 fi
 
 set -e # Exit on most errors
 # If you prefer to do selective error checking with
```

### Comparing `sbo-create-2.0.5/sbo_scripts_templates/template.info` & `sbo-create-2.0.6/sbo_scripts_templates/template.info`

 * *Files 2% similar despite different names*

```diff
@@ -3,8 +3,8 @@
 HOMEPAGE="homepage of application"
 DOWNLOAD="direct download link(s) of application source tarball(s) arch-independent or x86"
 MD5SUM="md5sum(s) of the source tarball(s) defined in DOWNLOAD"
 DOWNLOAD_x86_64="direct download link(s) of application source tarball(s), x86_64 only"
 MD5SUM_x86_64="md5sum(s) of the source tarball(s) defined in DOWNLOAD_x86_64"
 REQUIRES="%README%"
 MAINTAINER="name of SlackBuild script maintainer"
-EMAIL="email address of author"
+EMAIL="email address of maintainer"
```

### Comparing `sbo-create-2.0.5/sbo_scripts_templates/meson-template.SlackBuild` & `sbo-create-2.0.6/sbo_scripts_templates/meson-template.SlackBuild`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,17 @@
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "i686" ]; then
   SLKCFLAGS="-O2 -march=i686 -mtune=i686"
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "x86_64" ]; then
   SLKCFLAGS="-O2 -fPIC"
   LIBDIRSUFFIX="64"
+elif [ "$ARCH" = "aarch64" ]; then
+  SLKCFLAGS="-O2 -fPIC"
+  LIBDIRSUFFIX="64"
 else
   SLKCFLAGS="-O2"
   LIBDIRSUFFIX=""
 fi
 
 set -e # Exit on most errors
 # If you prefer to do selective error checking with
```

### Comparing `sbo-create-2.0.5/sbo_scripts_templates/slack-desc` & `sbo-create-2.0.6/sbo_scripts_templates/slack-desc`

 * *Files 17% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 appname: colon following "appname" (and the 'handy ruler' should start at
 appname: that colon and be exactly 71 characters long).
 appname: If there is room, there might be a link to the homepage of the
 appname: application on one of these lines, but it's not necessary.
 appname:
 appname: The maximum number of lines prefixed by "appname:" is 11.
 appname: Lines without any other text should *not* have a space after the :
-appname:
+appname: NOTE Please keep the comment section at the top of this file.
```

### Comparing `sbo-create-2.0.5/sbo_scripts_templates/rubygem-template.SlackBuild` & `sbo-create-2.0.6/sbo_scripts_templates/rubygem-template.SlackBuild`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,17 @@
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "i686" ]; then
   SLKCFLAGS="-O2 -march=i686 -mtune=i686"
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "x86_64" ]; then
   SLKCFLAGS="-O2 -fPIC"
   LIBDIRSUFFIX="64"
+elif [ "$ARCH" = "aarch64" ]; then
+  SLKCFLAGS="-O2 -fPIC"
+  LIBDIRSUFFIX="64"
 else
   SLKCFLAGS="-O2"
   LIBDIRSUFFIX=""
 fi
 
 set -e
```

### Comparing `sbo-create-2.0.5/sbo_scripts_templates/haskell-template.SlackBuild` & `sbo-create-2.0.6/sbo_scripts_templates/haskell-template.SlackBuild`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,17 @@
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "i686" ]; then
   SLKCFLAGS="-O2 -march=i686 -mtune=i686"
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "x86_64" ]; then
   SLKCFLAGS="-O2 -fPIC"
   LIBDIRSUFFIX="64"
+elif [ "$ARCH" = "aarch64" ]; then
+  SLKCFLAGS="-O2 -fPIC"
+  LIBDIRSUFFIX="64"
 else
   SLKCFLAGS="-O2"
   LIBDIRSUFFIX=""
 fi
 
 set -e
```

### Comparing `sbo-create-2.0.5/sbo_scripts_templates/perl-template.SlackBuild` & `sbo-create-2.0.6/sbo_scripts_templates/perl-template.SlackBuild`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,17 @@
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "i686" ]; then
   SLKCFLAGS="-O2 -march=i686 -mtune=i686"
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "x86_64" ]; then
   SLKCFLAGS="-O2 -fPIC"
   LIBDIRSUFFIX="64"
+elif [ "$ARCH" = "aarch64" ]; then
+  SLKCFLAGS="-O2 -fPIC"
+  LIBDIRSUFFIX="64"
 else
   SLKCFLAGS="-O2"
   LIBDIRSUFFIX=""
 fi
 
 set -e
```

### Comparing `sbo-create-2.0.5/sbo_scripts_templates/README` & `sbo-create-2.0.6/sbo_scripts_templates/README`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.5/sbo_scripts_templates/python-template.SlackBuild` & `sbo-create-2.0.6/sbo_scripts_templates/python-template.SlackBuild`

 * *Files 8% similar despite different names*

```diff
@@ -83,14 +83,17 @@
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "i686" ]; then
   SLKCFLAGS="-O2 -march=i686 -mtune=i686"
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "x86_64" ]; then
   SLKCFLAGS="-O2 -fPIC"
   LIBDIRSUFFIX="64"
+elif [ "$ARCH" = "aarch64" ]; then
+  SLKCFLAGS="-O2 -fPIC"
+  LIBDIRSUFFIX="64"
 else
   SLKCFLAGS="-O2"
   LIBDIRSUFFIX=""
 fi
 
 set -e
 
@@ -105,20 +108,28 @@
  \( -perm 777 -o -perm 775 -o -perm 750 -o -perm 711 -o -perm 555 \
   -o -perm 511 \) -exec chmod 755 {} \; -o \
  \( -perm 666 -o -perm 664 -o -perm 640 -o -perm 600 -o -perm 444 \
   -o -perm 440 -o -perm 400 \) -exec chmod 644 {} \;
 
 # Your application may need different options; this is only an example
 
-# For python2
+## If your application uses setup.py:
+
+### For python2
 python2 setup.py install --root=$PKG
 
-# For python3
+### For python3
 python3 setup.py install --root=$PKG
 
+## If your application only has a pyproject.toml:
+
+python3 -m build --wheel --no-isolation
+
+python3 -m installer --destdir "$PKG" dist/*.whl
+
 # Strip binaries and libraries.
 find $PKG -print0 | xargs -0 file | grep -e "executable" -e "shared object" | grep ELF \
   | cut -f 1 -d : | xargs strip --strip-unneeded 2> /dev/null || true
 
 # Compress man pages
 # If the man pages are installed to /usr/share/man instead, you'll need to
 # move them manually.
```

### Comparing `sbo-create-2.0.5/sbo_create.egg-info/PKG-INFO` & `sbo-create-2.0.6/sbo_create.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbo-create
-Version: 2.0.5
+Version: 2.0.6
 Summary: SBo tool for creating SlackBuilds.
 Home-page: https://gitlab.com/dslackw/sbo-create
 Author: dslackw
 Author-email: dslackw@gmail.com
 License: UNKNOWN
 Keywords: sbo,templates,slackbuild
 Platform: UNKNOWN
@@ -36,14 +36,15 @@
 - Checking for already SlackBuilds in the repository and the distribution.
 - Autocorrect the quote marks for the .info file.
 - Auto-importing the SlackBuild script name.
 - Auto-importing the text from the slack-desc file into the README.
 - Auto-importing the maintainer data to the .SlackBuild script.
 - Auto-importing the version to the .SlackBuild script.
 - Auto-importing and checking the checksum signature to the .info file.
+- Auto-create all the necessary files for your SlackBuild package.
 
 
 Screenshot
 __________
 
 .. image:: https://gitlab.com/dslackw/images/raw/master/sbo-create/img_menu.png
     :target: https://gitlab.com/dslackw/sbo-create
@@ -57,16 +58,16 @@
 
 
 Install
 -------
 
 .. code-block:: bash
 
-    $ tar xvf sbo-create-2.0.5.tar.gz
-    $ cd sbo-create-2.0.5
+    $ tar xvf sbo-create-2.0.6.tar.gz
+    $ cd sbo-create-2.0.6
     $ ./install.sh
 
     or
 
     $ slpkg install sbo-create
 
 
@@ -94,14 +95,20 @@
                                         README, slack-desc}.
       -m, --maintainer           Edit the maintainer file.
       -d, --download             Download source files listed in the .info file.
       -c, --check NAME           Check if the SBo exist in the repository.
       -h, --help                 Display this message and exit.
       -v, --version              Show version and exit.
 
+The first step is to create your profile, be entering the maintainer data:
+
+.. code-block:: bash
+
+    $ sbo-create --maintainer
+
 For a new project, you should create at first a new folder with the same name as
 the project.
 For an existing project, come into the folder and start to edit, just run `sbo-create`.
 
 Alternative you can run the below command to create all the necessary files:
 
 .. code-block:: bash
```

### Comparing `sbo-create-2.0.5/slackbuild/sbo-create.SlackBuild` & `sbo-create-2.0.6/slackbuild/sbo-create.SlackBuild`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/bin/bash
 
 # Slackware build script for sbo-create
 
-# Copyright 2015-2022 Dimitris Zlatanidis Orestiada, Greece
+# Copyright 2015-2023 Dimitris Zlatanidis Orestiada, Greece
 # All rights reserved.
 #
 # Redistribution and use of this script, with or without modification, is
 # permitted provided that the following conditions are met:
 #
 # 1. Redistributions of this script must retain the above copyright
 #    notice, this list of conditions and the following disclaimer.
@@ -21,15 +21,15 @@
 #  WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 #  OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 #  ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 cd $(dirname $0) ; CWD=$(pwd)
 
 PRGNAM=sbo-create
-VERSION=${VERSION:-2.0.4}
+VERSION=${VERSION:-2.0.6}
 BUILD=${BUILD:-1}
 TAG=${TAG:-_dsw}
 PKGTYPE=${PKGTYPE:-tgz}
 
 if [ -z "$ARCH" ]; then
   case "$( uname -m )" in
     i?86) ARCH=i586 ;;
@@ -86,11 +86,10 @@
 
 mkdir -p $PKG/usr/doc/$PRGNAM-$VERSION
 cp -a README.rst ChangeLog.txt LICENSE $PKG/usr/doc/$PRGNAM-$VERSION
 cat $CWD/$PRGNAM.SlackBuild > $PKG/usr/doc/$PRGNAM-$VERSION/$PRGNAM.SlackBuild
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
-cat $CWD/doinst.sh > $PKG/install/doinst.sh
 
 cd $PKG
 /sbin/makepkg -l y -c n $OUTPUT/$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE
```

### Comparing `sbo-create-2.0.5/slackbuild/slack-desc` & `sbo-create-2.0.6/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.5/setup.py` & `sbo-create-2.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.5/README.rst` & `sbo-create-2.0.6/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 - Checking for already SlackBuilds in the repository and the distribution.
 - Autocorrect the quote marks for the .info file.
 - Auto-importing the SlackBuild script name.
 - Auto-importing the text from the slack-desc file into the README.
 - Auto-importing the maintainer data to the .SlackBuild script.
 - Auto-importing the version to the .SlackBuild script.
 - Auto-importing and checking the checksum signature to the .info file.
+- Auto-create all the necessary files for your SlackBuild package.
 
 
 Screenshot
 __________
 
 .. image:: https://gitlab.com/dslackw/images/raw/master/sbo-create/img_menu.png
     :target: https://gitlab.com/dslackw/sbo-create
@@ -39,16 +40,16 @@
 
 
 Install
 -------
 
 .. code-block:: bash
 
-    $ tar xvf sbo-create-2.0.5.tar.gz
-    $ cd sbo-create-2.0.5
+    $ tar xvf sbo-create-2.0.6.tar.gz
+    $ cd sbo-create-2.0.6
     $ ./install.sh
 
     or
 
     $ slpkg install sbo-create
 
 
@@ -76,14 +77,20 @@
                                         README, slack-desc}.
       -m, --maintainer           Edit the maintainer file.
       -d, --download             Download source files listed in the .info file.
       -c, --check NAME           Check if the SBo exist in the repository.
       -h, --help                 Display this message and exit.
       -v, --version              Show version and exit.
 
+The first step is to create your profile, be entering the maintainer data:
+
+.. code-block:: bash
+
+    $ sbo-create --maintainer
+
 For a new project, you should create at first a new folder with the same name as
 the project.
 For an existing project, come into the folder and start to edit, just run `sbo-create`.
 
 Alternative you can run the below command to create all the necessary files:
 
 .. code-block:: bash
```

### Comparing `sbo-create-2.0.5/LICENSE` & `sbo-create-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.5/install.sh` & `sbo-create-2.0.6/install.sh`

 * *Files identical despite different names*

### Comparing `sbo-create-2.0.5/ChangeLog.txt` & `sbo-create-2.0.6/ChangeLog.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+2.0.6 - 06/06/2023
+Fixed:
+- slack-desc template
+- meson template
+Updated:
+- For http error
+- maintainer config file
+- doinst.sh template
+- python template
+- autotools template
+- cmake template
+- perl template
+- rubygem template
+- haskell template
+- meson template
+Added:
+- Slackbuild repository version in the config file
+- douninst.sh script
+
 2.0.5 - 04/06/2023
 Updated:
 - Improved code quality
 Fixed:
 - Checksum in the .info file
 Added:
 - Options to the cli menu
```

### Comparing `sbo-create-2.0.5/sbo_create/templates.py` & `sbo-create-2.0.6/sbo_create/templates.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,195 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+# Templates date updated: 2023-05-13
 
-def doinst_template():
+
+def doinst_script():
     bg = "\x1b[48;5;4m"
     fg = "\x1b[38;5;7m"
     cl = f"{bg}{fg}"
 
     template: str = """
 %s################################################################################
-%s#             COPY A TEMPLATE AND PASTE IT INTO THE TEXT EDITOR                #
+%s#                     COPY WHAT YOU WANT EXIT AND PASTE                        #
 %s#                          PRESS \"q or Q\" TO EXIT                              #
 %s################################################################################
 
+# $RCSfile: doinst.sh,v $
+# $Revision: 1.9 $
+# $Date: 2023-05-11 07:58:15+01 $
+# DW
+
+# NOTE DO:
+# PLEASE only keep the functions/sections/commands that you need.
+# PLEASE delete EVERYTHING else (including these comments).
+# PLEASE let us know in the comment section of the upload form if including
+#        custom functions or commands.
+
+# NOTE PLEASE DO NOT:
+# Add or change user or group accounts.
+# Change any of the default system settings files.
+# Add commands that take forever to complete.
+# Use applications like checkinstall or installwatch, that 'touch' every file
+# on the system.
+
+
+# NOTE on paths
+# Most commands do not have an initial '/' in directory path arguments so that
+# they work correctly when using pkgtools --root <path> or $ROOT options.
+# Installpkg and friends chdir to $ROOT or --root <path> before installing packages.
+# The exceptions are the 'chroot' commands which do use an initial '/'.
+# The chroot command is used to avoid files on the host being changed when
+# using --root or $ROOT.
+#
+# Example: /usr/bin/update-desktop-database -q usr/share/applications
+#          ^Full path for command^             ^No initial slash^
+
+# NOTE on tests
+# [ -e <path> ]    => Tests if a directory or file exists.
+# [ -x <command> ] => Tests if command is executable.
+#                     Will also fail silently if not -e too.
+
+# NOTE on redirections
+# Most commands redirect stdout and stderr to /dev/null to keep down the noise.
+# If you need to see error messages while testing, the easiest way is to
+# temporarily comment out 2>&1.
+
+# FUNCTION:    config()
+# DESCRIPTION: Discards identical copies of config and rc.INIT files.
+# ARGUMENTS:   A single filename.
+# NOTE
+# Files should be installed with a .new extension.
+# Example: etc/rc.d/rc.myshinynewdaemon.new
+# We don't clobber if it's avoidable.
+# "slackpkg new-config" is one way that users can list+process .new files.
+
 config() {
   NEW="$1"
   OLD="$(dirname $NEW)/$(basename $NEW .new)"
   # If there's no config file by that name, mv it over:
   if [ ! -r $OLD ]; then
     mv $NEW $OLD
   elif [ "$(cat $OLD | md5sum)" = "$(cat $NEW | md5sum)" ]; then
     # toss the redundant copy
     rm $NEW
   fi
   # Otherwise, we leave the .new copy for the admin to consider...
 }
 
+# FUNCTION:    preserve_perms()
+# DESCRIPTION: Keeps the executable bit that a user may have set (or unset) on
+#              an rc.INIT or config file since she first installed a package.
+# ARGUMENTS:   A single filename.
+# NOTE
+# This calls the above config() function to discard identical copies.
+# Files should be installed with a .new extension.
+# Use for files in etc/rc.d/ and etc/profile.d/
+# Other config files may also need this.
+
 preserve_perms() {
   NEW="$1"
   OLD="$(dirname $NEW)/$(basename $NEW .new)"
   if [ -e $OLD ]; then
     cp -a $OLD ${NEW}.incoming
     cat $NEW > ${NEW}.incoming
     mv ${NEW}.incoming $NEW
   fi
   config $NEW
 }
 
+# FUNCTION:    schema_install()
+# DESCRIPTION: Installs options (schemas) to the gnome config database.
+# ARGUMENTS:    A single filename.
+# NOTE Not to be confused with glib schemas
+
 schema_install() {
   SCHEMA="$1"
   GCONF_CONFIG_SOURCE="xml::etc/gconf/gconf.xml.defaults" \\
   chroot . gconftool-2 --makefile-install-rule \\
     /etc/gconf/schemas/$SCHEMA \\
     1>/dev/null
 }
 
+# Examples (NOTE must be *after* their respective function definitions!)
+
+# Does the finished package have files in etc/gconf/schemas/?
 schema_install blah.schemas
+
+# Does the finished package have init files in etc/rc.d/?
 preserve_perms etc/rc.d/rc.INIT.new
+
+# Does the finished package have config files in etc/?
 config etc/configfile.new
 
+# DESCRIPTION: Updates the system desktop database.
+# Does the finished package have a .desktop file in usr/share/applications/?
 if [ -x /usr/bin/update-desktop-database ]; then
   /usr/bin/update-desktop-database -q usr/share/applications >/dev/null 2>&1
 fi
 
+# DESCRIPTION: Updates the system mime database.
+# Does the finished package have files in usr/share/mime/?
 if [ -x /usr/bin/update-mime-database ]; then
   /usr/bin/update-mime-database usr/share/mime >/dev/null 2>&1
 fi
 
+# DESCRIPTION: Updates the GTK icon cache.
+# Does the finished package have files in usr/share/icons/hicolor/?
 # If other icon themes are installed, then add to/modify this as needed
 if [ -e usr/share/icons/hicolor/icon-theme.cache ]; then
   if [ -x /usr/bin/gtk-update-icon-cache ]; then
-    /usr/bin/gtk-update-icon-cache usr/share/icons/hicolor >/dev/null 2>&1
+    /usr/bin/gtk-update-icon-cache -f usr/share/icons/hicolor >/dev/null 2>&1
   fi
 fi
 
+# DESCRIPTION: GSettings (glib2) schema compiler.
+# Does the finished package have files in usr/share/glib-2.0/schemas/?
+# NOTE Not to be confused with gnome setting schemas
 if [ -e usr/share/glib-2.0/schemas ]; then
   if [ -x /usr/bin/glib-compile-schemas ]; then
     /usr/bin/glib-compile-schemas usr/share/glib-2.0/schemas >/dev/null 2>&1
   fi
 fi
 
+# DESCRIPTION: Updates the GIO cache.
+# Does the finished package have files in /usr/lib(64)/gio/modules/?
 # If needed -- be sure to sed @LIBDIR@ inside the build script
-chroot . /usr/bin/gio-querymodules @LIBDIR@/gio/modules/ 1> /dev/null 2> /dev/null
-
-if [ -x /usr/bin/install-info ]; then
-  chroot . /usr/bin/install-info --info-dir=/usr/info /usr/info/blah.gz 2> /dev/null
-fi
+# Example: sed -i "s|@LIBDIR@|/usr/lib$LIBDIRSUFFIX|g" doinst.sh
+# NOTE An initial '/' in the lib dir here because of 'chroot'.
+# NOTE Be sure to use double-quotes ""
+chroot . /usr/bin/gio-querymodules @LIBDIR@/gio/modules/ 1> /dev/null >/dev/null 2>&1
 
 %s################################################################################
 """ % (cl, cl, cl, cl, cl)
     return template
 
 
+def douninst_script():
+    bg = "\x1b[48;5;4m"
+    fg = "\x1b[38;5;7m"
+    cl = f"{bg}{fg}"
+    template: str = """
+%s################################################################################
+%s#                          PRESS \"q or Q\" TO EXIT                              #
+%s################################################################################
+#
+# douninst.sh
+#
+# uninstall script for Slackware >= 15.0
+#
+# NOTE: This script is run AFTER package removal, so be careful!
+#       Consider it optional, use if it is really needed.""" % (cl, cl, cl)
+    return template
+
+
 def slack_desc_template(name: str) -> str:
     if not name:
-        name: str = f"{'None':4}"
+        name: str = 'None'
     template: str = f"""# HOW TO EDIT THIS FILE:
 # The "handy ruler" below makes it easier to edit a package description.
 # Line up the first '|' above the ':' following the base package name, and
 # the '|' on the right side marks the last column you can put a character in.
 # You must make exactly 11 lines for the formatting to be correct.  It's also
 # customary to leave one space after the ':' except on otherwise blank lines.
 
@@ -161,25 +262,25 @@
 PRGNAM=%s
 VERSION=${VERSION:-%s}
 BUILD=${BUILD:-1}
 TAG=${TAG:-_SBo}
 PKGTYPE=${PKGTYPE:-tgz}
 
 if [ -z "$ARCH" ]; then
-case "$( uname -m )" in
+  case "$( uname -m )" in
     i?86) ARCH=i586 ;;
     arm*) ARCH=arm ;;
-    *) ARCH=$( uname -m ) ;;
-esac
+       *) ARCH=$( uname -m ) ;;
+  esac
 fi
 
 # If the variable PRINT_PACKAGE_NAME is set, then this script will report what
 # the name of the created package would be, and then exit. This information
 # could be useful to other scripts.
-if [ ! -z "${PRINT_PACKAGE_NAME}"  ]; then
+if [ ! -z "${PRINT_PACKAGE_NAME}" ]; then
   echo "$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE"
   exit 0
 fi
 
 TMP=${TMP:-/tmp/SBo}
 PKG=$TMP/package-$PRGNAM
 OUTPUT=${OUTPUT:-/tmp}
@@ -189,14 +290,17 @@
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "i686" ]; then
   SLKCFLAGS="-O2 -march=i686 -mtune=i686"
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "x86_64" ]; then
   SLKCFLAGS="-O2 -fPIC"
   LIBDIRSUFFIX="64"
+elif [ "$ARCH" = "aarch64" ]; then
+  SLKCFLAGS="-O2 -fPIC"
+  LIBDIRSUFFIX="64"
 else
   SLKCFLAGS="-O2"
   LIBDIRSUFFIX=""
 fi
 
 set -e
 
@@ -207,58 +311,65 @@
 tar xvf $CWD/$PRGNAM-$VERSION.tar.gz
 cd $PRGNAM-$VERSION
 chown -R root:root .
 find -L . \\
  \( -perm 777 -o -perm 775 -o -perm 750 -o -perm 711 -o -perm 555 \\
   -o -perm 511 \) -exec chmod 755 {} \; -o \\
  \( -perm 666 -o -perm 664 -o -perm 640 -o -perm 600 -o -perm 444 \\
-  -o -perm 440 -o -perm 400 \) -exec chmod 644 {} \\;
+  -o -perm 440 -o -perm 400 \) -exec chmod 644 {} \;
 
 CFLAGS="$SLKCFLAGS" \\
 CXXFLAGS="$SLKCFLAGS" \\
 ./configure \\
   --prefix=/usr \\
   --libdir=/usr/lib${LIBDIRSUFFIX} \\
   --sysconfdir=/etc \\
   --localstatedir=/var \\
   --mandir=/usr/man \\
   --docdir=/usr/doc/$PRGNAM-$VERSION \\
+  --disable-static \\
   --build=$ARCH-slackware-linux
 
 make
 make install DESTDIR=$PKG
 
+# Don't ship .la files:
 rm -f $PKG/{,usr/}lib${LIBDIRSUFFIX}/*.la
 
 find $PKG -print0 | xargs -0 file | grep -e "executable" -e "shared object" | grep ELF \\
   | cut -f 1 -d : | xargs strip --strip-unneeded 2> /dev/null || true
 
 find $PKG/usr/man -type f -exec gzip -9 {} \\;
 for i in $( find $PKG/usr/man -type l ) ; do ln -s $( readlink $i ).gz $i.gz ; rm $i ; done
 
+# Compress info pages and remove the package's dir file
+# If no info pages are installed by the software, don't leave this in the script
 rm -f $PKG/usr/info/dir
 gzip -9 $PKG/usr/info/*.info*
 
+# Remove perllocal.pod and other special files that don't need to be installed,
+# as they will overwrite what's already on the system.  If this is not needed,
+# remove it from the script.
+# Remove 'special' files
 find $PKG -name perllocal.pod \\
-  -o -name ".packlist" \
+  -o -name ".packlist" \\
   -o -name "*.bs" \\
   | xargs rm -f
 
 mkdir -p $PKG/usr/doc/$PRGNAM-$VERSION
 cp -a <documentation> $PKG/usr/doc/$PRGNAM-$VERSION
 cat $CWD/$PRGNAM.SlackBuild > $PKG/usr/doc/$PRGNAM-$VERSION/$PRGNAM.SlackBuild
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 cat $CWD/doinst.sh > $PKG/install/doinst.sh
 
 cd $PKG
 /sbin/makepkg -l y -c n $OUTPUT/$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE
-""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name,
-       self.version)
+""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name, self.version)
         return autotools_template
 
     def cmake(self):
 
         cmake_template = """#!/bin/bash
 
 # Slackware build script for %s
@@ -316,72 +427,80 @@
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "i686" ]; then
   SLKCFLAGS="-O2 -march=i686 -mtune=i686"
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "x86_64" ]; then
   SLKCFLAGS="-O2 -fPIC"
   LIBDIRSUFFIX="64"
+elif [ "$ARCH" = "aarch64" ]; then
+  SLKCFLAGS="-O2 -fPIC"
+  LIBDIRSUFFIX="64"
 else
   SLKCFLAGS="-O2"
   LIBDIRSUFFIX=""
 fi
 
-set -e
+set -e # Exit on most errors
 
 rm -rf $PKG
 mkdir -p $TMP $PKG $OUTPUT
 cd $TMP
 rm -rf $PRGNAM-$VERSION
 tar xvf $CWD/$PRGNAM-$VERSION.tar.gz
 cd $PRGNAM-$VERSION
 chown -R root:root .
 find -L . \\
- \( -perm 777 -o -perm 775 -o -perm 750 -o -perm 711 -o -perm 555 \\
-  -o -perm 511 \) -exec chmod 755 {} \; -o \\
- \( -perm 666 -o -perm 664 -o -perm 640 -o -perm 600 -o -perm 444 \\
-  -o -perm 440 -o -perm 400 \) -exec chmod 644 {} \\;
+ \\( -perm 777 -o -perm 775 -o -perm 750 -o -perm 711 -o -perm 555 \\
+  -o -perm 511 \) -exec chmod 755 {} \\; -o \\
+ \\( -perm 666 -o -perm 664 -o -perm 640 -o -perm 600 -o -perm 444 \\
+  -o -perm 440 -o -perm 400 \\) -exec chmod 644 {} \\;
 
 mkdir -p build
 cd build
   cmake \\
     -DCMAKE_C_FLAGS:STRING="$SLKCFLAGS" \\
     -DCMAKE_CXX_FLAGS:STRING="$SLKCFLAGS" \\
     -DCMAKE_INSTALL_PREFIX=/usr \\
     -DLIB_SUFFIX=${LIBDIRSUFFIX} \\
     -DMAN_INSTALL_DIR=/usr/man \\
     -DCMAKE_BUILD_TYPE=Release ..
   make
-  make install DESTDIR=$PKG
+  make install/strip DESTDIR=$PKG
 cd ..
 
+# Don't ship .la files:
 rm -f $PKG/{,usr/}lib${LIBDIRSUFFIX}/*.la
 
 find $PKG -print0 | xargs -0 file | grep -e "executable" -e "shared object" | grep ELF \\
   | cut -f 1 -d : | xargs strip --strip-unneeded 2> /dev/null || true
 
 find $PKG/usr/man -type f -exec gzip -9 {} \\;
 for i in $( find $PKG/usr/man -type l ) ; do ln -s $( readlink $i ).gz $i.gz ; rm $i ; done
 
+# Compress info pages and remove the package's dir file
+# If no info pages are installed by the software, don't leave this in the script
 rm -f $PKG/usr/info/dir
 gzip -9 $PKG/usr/info/*.info*
 
+# Remove perllocal.pod and other special files that don't need to be installed,
+# as they will overwrite what's already on the system.  If this is not needed,
+# remove it from the script.
 find $PKG -name perllocal.pod -o -name ".packlist" -o -name "*.bs" | xargs rm -f || true
 
 mkdir -p $PKG/usr/doc/$PRGNAM-$VERSION
-cp -a  <documentation> $PKG/usr/doc/$PRGNAM-$VERSION
+cp -a <documentation> $PKG/usr/doc/$PRGNAM-$VERSION
 cat $CWD/$PRGNAM.SlackBuild > $PKG/usr/doc/$PRGNAM-$VERSION/$PRGNAM.SlackBuild
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 cat $CWD/doinst.sh > $PKG/install/doinst.sh
 
 cd $PKG
 /sbin/makepkg -l y -c n $OUTPUT/$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE
-""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name,
-       self.version)
+""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name, self.version)
         return cmake_template
 
     def perl(self):
 
         perl_template = """#!/bin/bash
 
 # Slackware build script for %s
@@ -441,14 +560,17 @@
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "i686" ]; then
   SLKCFLAGS="-O2 -march=i686 -mtune=i686"
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "x86_64" ]; then
   SLKCFLAGS="-O2 -fPIC"
   LIBDIRSUFFIX="64"
+elif [ "$ARCH" = "aarch64" ]; then
+  SLKCFLAGS="-O2 -fPIC"
+  LIBDIRSUFFIX="64"
 else
   SLKCFLAGS="-O2"
   LIBDIRSUFFIX=""
 fi
 
 set -e
 
@@ -456,61 +578,63 @@
 mkdir -p $TMP $PKG $OUTPUT
 cd $TMP
 rm -rf $SRCNAM-$VERSION
 tar xvf $CWD/$SRCNAM-$VERSION.tar.gz
 cd $SRCNAM-$VERSION
 chown -R root:root .
 find -L . \\
- \( -perm 777 -o -perm 775 -o -perm 750 -o -perm 711 -o -perm 555 \\
-  -o -perm 511 \) -exec chmod 755 {} \; -o \\
- \( -perm 666 -o -perm 664 -o -perm 640 -o -perm 600 -o -perm 444 \\
-  -o -perm 440 -o -perm 400 \) -exec chmod 644 {} \\;
+ \\( -perm 777 -o -perm 775 -o -perm 750 -o -perm 711 -o -perm 555 \\
+  -o -perm 511 \) -exec chmod 755 {} \\; -o \\
+ \\( -perm 666 -o -perm 664 -o -perm 640 -o -perm 600 -o -perm 444 \\
+  -o -perm 440 -o -perm 400 \\) -exec chmod 644 {} \\;
 
 # Build method #1 (preferred)
 perl Makefile.PL \\
   PREFIX=/usr \\
   INSTALLDIRS=vendor \\
   INSTALLVENDORMAN1DIR=/usr/man/man1 \\
   INSTALLVENDORMAN3DIR=/usr/man/man3
 make
 make test
 make install DESTDIR=$PKG
 
 # Build method #2
 # requires perl-Module-Build or perl-Module-Build-Tiny
-perl Build.PL \
-  --installdirs vendor \
-  --config installvendorman1dir=/usr/man/man1 \
+perl Build.PL \\
+  --installdirs vendor \\
+  --config installvendorman1dir=/usr/man/man1 \\
   --config installvendorman3dir=/usr/man/man3
 ./Build
 ./Build test
-./Build install \
+./Build install \\
   --destdir $PKG
 
 find $PKG -print0 | xargs -0 file | grep -e "executable" -e "shared object" | grep ELF \\
   | cut -f 1 -d : | xargs strip --strip-unneeded 2> /dev/null || true
 
 find $PKG/usr/man -type f -exec gzip -9 {} \\;
 for i in $( find $PKG/usr/man -type l ) ; do ln -s $( readlink $i ).gz $i.gz ; rm $i ; done
 
+# Remove perllocal.pod and other special files that don't need to be installed,
+# as they will overwrite what's already on the system.
 find $PKG -name perllocal.pod -o -name ".packlist" -o -name "*.bs" | xargs rm -f || true
 
+# Remove empty directories
 find $PKG -depth -type d -empty -delete || true
 
 mkdir -p $PKG/usr/doc/$PRGNAM-$VERSION
-cp -a  <documentation>  $PKG/usr/doc/$PRGNAM-$VERSION
+cp -a <documentation> $PKG/usr/doc/$PRGNAM-$VERSION
 cat $CWD/$PRGNAM.SlackBuild > $PKG/usr/doc/$PRGNAM-$VERSION/$PRGNAM.SlackBuild
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 
 cd $PKG
 /sbin/makepkg -l y -c n $OUTPUT/$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE
-""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name,
-       self.version)
+""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name, self.version)
         return perl_template
 
     def python(self):
 
         python_template = """#!/bin/bash
 
 # Slackware build script for %s
@@ -568,14 +692,17 @@
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "i686" ]; then
   SLKCFLAGS="-O2 -march=i686 -mtune=i686"
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "x86_64" ]; then
   SLKCFLAGS="-O2 -fPIC"
   LIBDIRSUFFIX="64"
+elif [ "$ARCH" = "aarch64" ]; then
+  SLKCFLAGS="-O2 -fPIC"
+  LIBDIRSUFFIX="64"
 else
   SLKCFLAGS="-O2"
   LIBDIRSUFFIX=""
 fi
 
 set -e
 
@@ -583,25 +710,29 @@
 mkdir -p $TMP $PKG $OUTPUT
 cd $TMP
 rm -rf $PRGNAM-$VERSION
 tar xvf $CWD/$PRGNAM-$VERSION.tar.gz
 cd $PRGNAM-$VERSION
 chown -R root:root .
 find -L . \\
- \( -perm 777 -o -perm 775 -o -perm 750 -o -perm 711 -o -perm 555 \\
-  -o -perm 511 \) -exec chmod 755 {} \; -o \\
- \( -perm 666 -o -perm 664 -o -perm 640 -o -perm 600 -o -perm 444 \\
-  -o -perm 440 -o -perm 400 \) -exec chmod 644 {} \\;
+ \\( -perm 777 -o -perm 775 -o -perm 750 -o -perm 711 -o -perm 555 \\
+  -o -perm 511 \\) -exec chmod 755 {} \\; -o \\
+ \\( -perm 666 -o -perm 664 -o -perm 640 -o -perm 600 -o -perm 444 \\
+  -o -perm 440 -o -perm 400 \\) -exec chmod 644 {} \\;
 
-# For python2
+### For python2
 python2 setup.py install --root=$PKG
 
-# For python3
+### For python3
 python3 setup.py install --root=$PKG
 
+## If your application only has a pyproject.toml:
+python3 -m build --wheel --no-isolation
+python3 -m installer --destdir "$PKG" dist/*.whl
+
 find $PKG -print0 | xargs -0 file | grep -e "executable" -e "shared object" | grep ELF \\
   | cut -f 1 -d : | xargs strip --strip-unneeded 2> /dev/null || true
 
 find $PKG/usr/man -type f -exec gzip -9 {} \\;
 for i in $( find $PKG/usr/man -type l ) ; do ln -s $( readlink $i ).gz $i.gz ; rm $i ; done
 
 mkdir -p $PKG/usr/doc/$PRGNAM-$VERSION
@@ -610,16 +741,15 @@
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 cat $CWD/doinst.sh > $PKG/install/doinst.sh
 
 cd $PKG
 /sbin/makepkg -l y -c n $OUTPUT/$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE
-""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name,
-       self.version)
+""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name, self.version)
         return python_template
 
     def rubygem(self):
 
         rubygem_template = """#!/bin/bash
 
 # Slackware build script for %s
@@ -642,21 +772,21 @@
 #  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 #  WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 #  OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 #  ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 cd $(dirname $0) ; CWD=$(pwd)
 
-PRGNAM=%s
+PRGNAM=rubygem-%s
 VERSION=${VERSION:-%s}
 BUILD=${BUILD:-1}
 TAG=${TAG:-_SBo}
 PKGTYPE=${PKGTYPE:-tgz}
 
-SRCNAM=appname
+SRCNAM=%s
 
 if [ -z "$ARCH" ]; then
   case "$( uname -m )" in
     i?86) ARCH=i586 ;;
     arm*) ARCH=arm ;;
        *) ARCH=$( uname -m ) ;;
   esac
@@ -679,84 +809,92 @@
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "i686" ]; then
   SLKCFLAGS="-O2 -march=i686 -mtune=i686"
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "x86_64" ]; then
   SLKCFLAGS="-O2 -fPIC"
   LIBDIRSUFFIX="64"
+elif [ "$ARCH" = "aarch64" ]; then
+  SLKCFLAGS="-O2 -fPIC"
+  LIBDIRSUFFIX="64"
 else
   SLKCFLAGS="-O2"
   LIBDIRSUFFIX=""
 fi
 
 set -e
 
 rm -rf $PKG
 mkdir -p $TMP $PKG $OUTPUT
 cd $TMP
 
+# Get the full path of the ruby installation, for gems
 DESTDIR=$( ruby -r rbconfig -e '
 include RbConfig
-printf("%s/%s/gems/%s\n",
-	CONFIG["libdir"],
-	CONFIG["RUBY_INSTALL_NAME"],
-	CONFIG["ruby_version"]
+printf("%s/%s/gems/%s\\n",
+    CONFIG["libdir"],
+    CONFIG["RUBY_INSTALL_NAME"],
+    CONFIG["ruby_version"]
       )
 ')
 
+# print a friendly warning of unsatisfied ":runtime" dependencies
+# good to leave in place, even if the gem doesn't have any dependencies. 
+# things could always change
 gem specification $CWD/$SRCNAM-$VERSION.gem | \\
-	ruby -r yaml -r rbconfig -e '
+    ruby -r yaml -r rbconfig -e '
 c = RbConfig::CONFIG
 path = sprintf("%s/%s/gems/%s",
         c["libdir"],
         c["RUBY_INSTALL_NAME"],
         c["ruby_version"])
-sys_gemspecs = Dir.glob(path + "/specifications/*").map {|g| gs = Gem::Specification.load(g);
-gs.name }
+sys_gemspecs = Dir.glob(path + "/specifications/**/*.gemspec").map {|g| gs = Gem::Specification.load(g); gs.name }
 obj = Gem::Specification.from_yaml($stdin)
 obj.dependencies.each {|dep|
         if not(dep.type == :runtime)
                 next
         end
         if not(sys_gemspecs.include?(dep.name))
-                $stderr.write("WARNING:
+                $stderr.write("WARNING: #{dep.name} gem not found\\n")
                 sleep 0.5
         end
 
 }'
 
 gem install \\
-	--local \\
-	--no-update-sources \\
-	--ignore-dependencies \\
-	--backtrace \\
-	--install-dir $PKG/$DESTDIR \\
-	--bindir $PKG/usr/bin \\
-	$CWD/$SRCNAM-$VERSION.gem
+    --local \\
+    --no-update-sources\ \\
+    --ignore-dependencies \\
+    --backtrace \\
+    --install-dir $PKG/$DESTDIR \\
+    --bindir $PKG/usr/bin \\
+    $CWD/$SRCNAM-$VERSION.gem
 
 find $PKG -print0 | xargs -0 file | grep -e "executable" -e "shared object" | grep ELF \\
   | cut -f 1 -d : | xargs strip --strip-unneeded 2> /dev/null || true
 
+# Remove cached gem from install, if you are so inspired ..
+#rm -rf $PKG/$DESTDIR/cache
+
 mkdir -p $PKG/usr/doc/$PRGNAM-$VERSION
 tar -x -O --file=$CWD/$SRCNAM-$VERSION.gem data.tar.gz \\
   | tar -xz -C $PKG/usr/doc/$PRGNAM-$VERSION --file=- \\
   <documentation>
 cat $CWD/$PRGNAM.SlackBuild > $PKG/usr/doc/$PRGNAM-$VERSION/$PRGNAM.SlackBuild
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 cat $CWD/doinst.sh > $PKG/install/doinst.sh
 
 cd $PKG
 /sbin/makepkg -l y -c n $OUTPUT/$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE
-""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name,
-       self.version, "%s", "%s", "%s", "%s", "%s", "%s")
+""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name, self.version, self.app_name,
+       "%s", "%s", "%s", "%s", "%s", "%s")
         return rubygem_template
 
-
     def haskell(self):
 
         haskell_template = """#!/bin/bash
 
 # Slackware build script for %s
 
 # Copyright %s %s %s
@@ -777,15 +915,15 @@
 #  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 #  WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 #  OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 #  ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 cd $(dirname $0) ; CWD=$(pwd)
 
-PRGNAM=%s
+PRGNAM=haskell-%s
 VERSION=${VERSION:-%s}
 BUILD=${BUILD:-1}
 TAG=${TAG:-_SBo}
 PKGTYPE=${PKGTYPE:-tgz}
 
 SRCNAM="$( echo $PRGNAM | cut -d- -f2- )"
 
@@ -816,14 +954,17 @@
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "i686" ]; then
   SLKCFLAGS="-O2 -march=i686 -mtune=i686"
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "x86_64" ]; then
   SLKCFLAGS="-O2 -fPIC"
   LIBDIRSUFFIX="64"
+elif [ "$ARCH" = "aarch64" ]; then
+  SLKCFLAGS="-O2 -fPIC"
+  LIBDIRSUFFIX="64"
 else
   SLKCFLAGS="-O2"
   LIBDIRSUFFIX=""
 fi
 
 set -e
 
@@ -832,18 +973,22 @@
 cd $TMP
 rm -rf $SRCNAM-$VERSION
 tar xvf $CWD/$SRCNAM-$VERSION.tar.gz
 cd $SRCNAM-$VERSION
 chown -R root:root .
 find -L . \\
  \( -perm 777 -o -perm 775 -o -perm 750 -o -perm 711 -o -perm 555 \\
-  -o -perm 511 \) -exec chmod 755 {} \; -o \\
- \( -perm 666 -o -perm 664 -o -perm 640 -o -perm 600 -o -perm 444 \\
-  -o -perm 440 -o -perm 400 \) -exec chmod 644 {} \\;
-
+  -o -perm 511 \) -exec chmod 755 {} \\; -o \\
+ \\( -perm 666 -o -perm 664 -o -perm 640 -o -perm 600 -o -perm 444 \\
+  -o -perm 440 -o -perm 400 \\) -exec chmod 644 {} \\;
+
+# Your application will probably need different configure flags;
+# these are provided as an example only.
+# Be sure to build only shared libraries unless there's some need for
+# static.
 CFLAGS="$SLKCFLAGS" \\
 CXXFLAGS="$SLKCFLAGS" \\
 runghc Setup configure \\
   --prefix=/usr \\
   --libdir=/usr/lib${LIBDIRSUFFIX} \\
   --libsubdir=ghc-${GHC_VERSION}/$SRCNAM-$VERSION \\
   --enable-shared \\
@@ -869,16 +1014,15 @@
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 cat $CWD/doinst.sh > $PKG/install/doinst.sh
 
 cd $PKG
 /sbin/makepkg -l y -c n $OUTPUT/$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE
-""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name,
-       self.version)
+""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name, self.version)
         return haskell_template
 
     def meson(self):
 
         autotools_template = """#!/bin/bash
 
 # Slackware build script for %s
@@ -908,102 +1052,108 @@
 PRGNAM=%s
 VERSION=${VERSION:-%s}
 BUILD=${BUILD:-1}
 TAG=${TAG:-_SBo}
 PKGTYPE=${PKGTYPE:-tgz}
 
 if [ -z "$ARCH" ]; then
-case "$( uname -m )" in
+  case "$( uname -m )" in
     i?86) ARCH=i586 ;;
     arm*) ARCH=arm ;;
-    *) ARCH=$( uname -m ) ;;
-esac
+       *) ARCH=$( uname -m ) ;;
+  esac
 fi
 
 # If the variable PRINT_PACKAGE_NAME is set, then this script will report what
 # the name of the created package would be, and then exit. This information
 # could be useful to other scripts.
 if [ ! -z "${PRINT_PACKAGE_NAME}" ]; then
   echo "$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE"
   exit 0
 fi
 
-CWD=$(pwd)
 TMP=${TMP:-/tmp/SBo}
 PKG=$TMP/package-$PRGNAM
 OUTPUT=${OUTPUT:-/tmp}
 
 if [ "$ARCH" = "i586" ]; then
   SLKCFLAGS="-O2 -march=i586 -mtune=i686"
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "i686" ]; then
   SLKCFLAGS="-O2 -march=i686 -mtune=i686"
   LIBDIRSUFFIX=""
 elif [ "$ARCH" = "x86_64" ]; then
   SLKCFLAGS="-O2 -fPIC"
   LIBDIRSUFFIX="64"
+elif [ "$ARCH" = "aarch64" ]; then
+  SLKCFLAGS="-O2 -fPIC"
+  LIBDIRSUFFIX="64"
 else
   SLKCFLAGS="-O2"
   LIBDIRSUFFIX=""
 fi
 
 set -e
+# If you prefer to do selective error checking with
+#   command || exit 1
+# then that's also acceptable.
 
 rm -rf $PKG
 mkdir -p $TMP $PKG $OUTPUT
 cd $TMP
 rm -rf $PRGNAM-$VERSION
 tar xvf $CWD/$PRGNAM-$VERSION.tar.gz
 cd $PRGNAM-$VERSION
 chown -R root:root .
 find -L . \\
- \( -perm 777 -o -perm 775 -o -perm 750 -o -perm 711 -o -perm 555 \\
-  -o -perm 511 \) -exec chmod 755 {} \; -o \\
- \( -perm 666 -o -perm 664 -o -perm 640 -o -perm 600 -o -perm 444 \\
-  -o -perm 440 -o -perm 400 \) -exec chmod 644 {} \\;
+ \\( -perm 777 -o -perm 775 -o -perm 750 -o -perm 711 -o -perm 555 \\
+  -o -perm 511 \) -exec chmod 755 {} \\; -o \\
+ \\( -perm 666 -o -perm 664 -o -perm 640 -o -perm 600 -o -perm 444 \\
+  -o -perm 440 -o -perm 400 \\) -exec chmod 644 {} \\;
 
 mkdir build
 cd build
-  CFLAGS="$SLKCFLAGS" \
-  CXXFLAGS="$SLKCFLAGS" \
-  meson .. \
-    --buildtype=release \
-    --infodir=/usr/info \
-    --libdir=/usr/lib${LIBDIRSUFFIX} \
-    --localstatedir=/var \
-    --mandir=/usr/man \
-    --prefix=/usr \
-    --sysconfdir=/etc \
+  CFLAGS="$SLKCFLAGS" \\
+  CXXFLAGS="$SLKCFLAGS" \\
+  meson .. \\
+    --buildtype=release \\
+    --infodir=/usr/info \\
+    --libdir=/usr/lib${LIBDIRSUFFIX} \\
+    --localstatedir=/var \\
+    --mandir=/usr/man \\
+    --prefix=/usr \\
+    --sysconfdir=/etc \\
     -Dstrip=true
   "${NINJA:=ninja}"
   DESTDIR=$PKG $NINJA install
 cd ..
 
-rm -f $PKG/{,usr/}lib${LIBDIRSUFFIX}/*.lacd ..
+rm -f $PKG/{,usr/}lib${LIBDIRSUFFIX}/*.la
 
 find $PKG -print0 | xargs -0 file | grep -e "executable" -e "shared object" | grep ELF \\
   | cut -f 1 -d : | xargs strip --strip-unneeded 2> /dev/null || true
 
 find $PKG/usr/man -type f -exec gzip -9 {} \\;
 for i in $( find $PKG/usr/man -type l ) ; do ln -s $( readlink $i ).gz $i.gz ; rm $i ; done
 
+# Compress info pages and remove the package's dir file
+# If no info pages are installed by the software, don't leave this in the script
 rm -f $PKG/usr/info/dir
 gzip -9 $PKG/usr/info/*.info*
 
 find $PKG -name perllocal.pod \\
-  -o -name ".packlist" \
+  -o -name ".packlist" \\
   -o -name "*.bs" \\
   | xargs rm -f
 
 mkdir -p $PKG/usr/doc/$PRGNAM-$VERSION
 cp -a <documentation> $PKG/usr/doc/$PRGNAM-$VERSION
 cat $CWD/$PRGNAM.SlackBuild > $PKG/usr/doc/$PRGNAM-$VERSION/$PRGNAM.SlackBuild
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 cat $CWD/doinst.sh > $PKG/install/doinst.sh
 
 cd $PKG
 /sbin/makepkg -l y -c n $OUTPUT/$PRGNAM-$VERSION-$ARCH-$BUILD$TAG.$PKGTYPE
-""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name,
-       self.version)
+""" % (self.app_name, self.year, self.maintainer, self.live, self.app_name, self.version)
         return autotools_template
```

### Comparing `sbo-create-2.0.5/sbo_create/__pycache__/__metadata__.cpython-39.pyc` & `sbo-create-2.0.6/sbo_create/__pycache__/__metadata__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Jun  6 17:42:34 2023 UTC, .py size: 350 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-00000000: 610d 0d0a 0000 0000 0a70 7f64 5e01 0000  a........p.d^...
+00000000: 610d 0d0a 0000 0000 5e2b 8264 5e01 0000  a.......^+.d^...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6c00 0000 5500  .....@...sl...U.
 00000030: 6400 5a00 6501 6502 6401 3c00 6402 5a03  d.Z.e.e.d.<.d.Z.
 00000040: 6501 6502 6403 3c00 6404 5a04 6501 6502  e.e.d.<.d.Z.e.e.
 00000050: 6405 3c00 6406 5a05 6506 6502 6407 3c00  d.<.d.Z.e.e.d.<.
 00000060: 6408 6a07 6505 8e00 5a08 6501 6502 6409  d.j.e...Z.e.e.d.
 00000070: 3c00 640a 5a09 6501 6502 640b 3c00 640c  <.d.Z.e.e.d.<.d.
 00000080: 5a0a 6501 6502 640d 3c00 640e 5a0b 6501  Z.e.e.d.<.d.Z.e.
 00000090: 6502 640f 3c00 6410 5300 2911 7a0a 7362  e.d.<.d.S.).z.sb
 000000a0: 6f2d 6372 6561 7465 da08 5f5f 7072 6f67  o-create..__prog
 000000b0: 5f5f 5a07 6473 6c61 636b 77da 0a5f 5f61  __Z.dslackw..__a
 000000c0: 7574 686f 725f 5f7a 0932 3031 352d 3230  uthor__z.2015-20
 000000d0: 3233 da0d 5f5f 636f 7079 7269 6768 745f  23..__copyright_
-000000e0: 5f29 03e9 0200 0000 e900 0000 00e9 0500  _)..............
+000000e0: 5f29 03e9 0200 0000 e900 0000 00e9 0600  _)..............
 000000f0: 0000 da10 5f5f 7665 7273 696f 6e5f 696e  ....__version_in
 00000100: 666f 5f5f 7a0b 7b30 7d2e 7b31 7d2e 7b32  fo__z.{0}.{1}.{2
 00000110: 7dda 0b5f 5f76 6572 7369 6f6e 5f5f 5a03  }..__version__Z.
 00000120: 4d49 54da 0b5f 5f6c 6963 656e 7365 5f5f  MIT..__license__
 00000130: 7a11 6473 6c61 636b 7740 676d 6169 6c2e  z.dslackw@gmail.
 00000140: 636f 6dda 095f 5f65 6d61 696c 5f5f 7a25  com..__email__z%
 00000150: 6874 7470 733a 2f2f 6769 746c 6162 2e63  https://gitlab.c
@@ -26,12 +26,12 @@
 00000190: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
 000001a0: 7202 0000 0072 0300 0000 7207 0000 00da  r....r....r.....
 000001b0: 0574 7570 6c65 da06 666f 726d 6174 7208  .tuple..formatr.
 000001c0: 0000 0072 0900 0000 720a 0000 0072 0b00  ...r....r....r..
 000001d0: 0000 a900 7210 0000 0072 1000 0000 fa43  ....r....r.....C
 000001e0: 2f68 6f6d 652f 6473 6c61 636b 772f 446f  /home/dslackw/Do
 000001f0: 776e 6c6f 6164 732f 7362 6f2d 6372 6561  wnloads/sbo-crea
-00000200: 7465 2d32 2e30 2e35 2f73 626f 5f63 7265  te-2.0.5/sbo_cre
+00000200: 7465 2d32 2e30 2e36 2f73 626f 5f63 7265  te-2.0.6/sbo_cre
 00000210: 6174 652f 5f5f 6d65 7461 6461 7461 5f5f  ate/__metadata__
 00000220: 2e70 79da 083c 6d6f 6475 6c65 3e04 0000  .py..<module>...
 00000230: 0073 0e00 0000 0e01 0c01 0c01 0c01 1201  .s..............
 00000240: 0c01 0c01                                ....
```

### Comparing `sbo-create-2.0.5/sbo_create/main.py` & `sbo-create-2.0.6/sbo_create/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,48 +10,56 @@
 import locale
 import urllib3
 import hashlib
 import subprocess
 from pathlib import Path
 from datetime import date
 from dialog import Dialog
+from urllib3.exceptions import HTTPError
 from sbo_create.templates import (
     SlackBuilds,
     slack_desc_template,
     info_template,
-    doinst_template,
+    doinst_script,
+    douninst_script
 )
 
 from sbo_create.__metadata__ import __version__
 
 locale.setlocale(locale.LC_ALL, '')
 
 
 class SBoCreate:
     """ SlackBuild Create Class. """
     def __init__(self):
         # General defines
         self.choices = None
-        self.home_path = None
         self.data: list = []
         self.fields = None
         self.code = None
         self.handy_ruler = None
         self.editor: str = str()
         self.where_you_live: str = str()
         self.email: str = str()
         self.maintainer: str = str()
         self.editor_options: str = str()
-        self.prg_name = None
         self.sources = None
         self.template = None
         self.slack_desc_comments = None
         self.slack_desc_user_text: list = []
         self.slack_desc_file_data: list = []
         self.current_folder: Path = Path.cwd()
+        self.home_path: Path = Path.home()
+        self.config_path: Path = Path(self.home_path, '.config', 'sbo-create')
+        self.config_file: str = 'maintainer.config'
+        self.maintainer_config: Path = Path(self.config_path, self.config_file)
+        if not self.config_path.is_dir():
+            self.config_path.mkdir(parents=True, exist_ok=True)
+        # Default repository version
+        self.sbo_repo_version: str = '15.0'
 
         # aboname.info initialize
         self.info_text: tuple = (
             'PRGNAM=', 'VERSION=', 'HOMEPAGE=', 'DOWNLOAD=',
             'MD5SUM=', 'DOWNLOAD_x86_64=', 'MD5SUM_x86_64=',
             'REQUIRES=', 'MAINTAINER=', 'EMAIL='
         )
@@ -60,15 +68,15 @@
         self.download_x86: str = str()
         self.md5sum_x86: str = str()
         self.download_x86_64: str = str()
         self.md5sum_x86_64: str = str()
         self.requires: str = str()
 
         # Set colors
-        self.colors: dict = {
+        self.color: dict = {
             'bold': '\Zb',
             'reset_bold': '\ZB',
             'underline': '\Zu',
             'reset_underline': '\ZU',
             'reverse': '\Zr',
             'reset_reverse': 'Zr',
             'restore': '\Zn',
@@ -77,18 +85,17 @@
             'green': '\Z2',
             'yellow': '\Z3',
             'blue': '\Z4',
             'magenta': '\Z5',
             'cyan': '\Z6',
             'white': '\Z7'
         }
-        self.error_title: str = f"{self.colors['red']}Error{self.colors['restore']}"
+        self.error_title: str = f"{self.color['red']}Error{self.color['restore']}"
 
         # Define some configurations
-        self.home_path: Path = Path.home()
         self.year: int = date.today().year
         self.dialog = Dialog(dialog='dialog')
         self.dialog.add_persistent_args(['--no-nl-expand', '--no-collapse', '--colors'])
         self.title: str = f'SlackBuild Create Tool {__version__}'
         self.dialog.set_background_title(self.title)
         self.prg_name: str = str(self.current_folder).split('/')[-1]
         self.read_maintainer_file()
@@ -117,21 +124,31 @@
             'prg-version': ['-e', '--prg-version'],
             'template': ['-t', '--template'],
             'create-files': ['-f', '--create-files'],
             'maintainer': ['-m', '--maintainer'],
             'download': ['-d', '--download'],
             'check': ['-c', '--check']
         }
-        all_options = sum(options.values(), [])
+        # Creates lists to a list
+        all_options: list = sum(options.values(), [])
+        options_with_parameter: list = sum(
+            [options['prgnam'],
+             options['prg-version'],
+             options['template'],
+             options['check']],
+            []
+        )
 
         # Checks for valid options
         invalid: list = []
         for arg in args:
             if arg.startswith('-') and arg not in all_options:
                 invalid.append(arg)
+            if not arg.startswith('-') and args[args.index(arg) - 1] not in options_with_parameter:
+                invalid.append(arg)
 
         if invalid and len(args) > 0:
             print(f"\nsbo-create: Error: Invalid options: {', '.join(set(invalid))}\n")
             raise SystemExit(1)
 
         for arg in args:
             try:
@@ -155,15 +172,14 @@
         elif len(args) == 1 and args[0] in options['help']:
             self.usage()
         elif len(args) == 1 and args[0] in options['version']:
             print(f'Version: {__version__}')
             raise SystemExit()
         elif create_files:
             self.create_files()
-            raise SystemExit()
         elif len(args) == 1 and args[0] in options['maintainer']:
             self.edit_maintainer_file()
         elif len(args) == 1 and args[0] in options['download']:
             self.sources_download()
         elif len(args) == 2 and args[0] in options['check']:
             self.is_the_sbo_exists()
 
@@ -210,23 +226,26 @@
         files: dict = {
             f'{self.prg_name}.SlackBuild': slackbuild,
             f'{self.prg_name}.info': info,
             'slack-desc': slack_desc,
             'README': readme
         }
 
+        created_files: list = []
         for file, content in files.items():
             with open(Path(self.current_folder, file), 'w') as f:
                 f.write(content)
+            created_files.append(file)
 
         print(f"Files created:\n")
-        for file in self.current_folder.iterdir():
-            if file.name in files.keys():
-                print(f"{'':>2}> {file.name}")
+        for file in created_files:
+            print(f"{'':>2}> {file}")
+
         print()
+        raise SystemExit()
 
     @staticmethod
     def usage() -> None:
         """ Optional arguments. """
         args: str = (
             "Usage: sbo-create [OPTIONS]\n\n"
             "Optional arguments:\n"
@@ -244,23 +263,22 @@
             "  -h, --help                 Display this message and exit.\n"
             "  -v, --version              Show version and exit.\n"
         )
         print(args)
         raise SystemExit()
 
     def menu_initialization(self) -> None:
-        self.md5sum_x86: str = str()
-        self.md5sum_x86_64: str = str()
         self.data: list = []
 
         self.choices: list = [
             ('Info', f'Edit {self.prg_name}.info file'),
             ('Slack desc', 'Edit slack-desc file'),
             ('SlackBuild', f'Edit {self.prg_name}.SlackBuild script'),
             ('Doinst.sh', 'Edit doinst.sh script'),
+            ('Douninst.sh', 'Edit douninst.sh script'),
             ('README', 'Edit README file'),
             ('Desktop', f'Edit {self.prg_name}.desktop file'),
             ('Permissions', f'Chmod -+ {self.prg_name}.SlackBuild script'),
             ('Download', 'Download the sources'),
             ('Checksum', 'Md5sum the sources'),
             ('Check', f'Check if the {self.prg_name} SBo exists'),
             ('Maintainer', 'Edit maintainer data'),
@@ -270,17 +288,17 @@
             ('Exit', 'Exit the program')
         ]
 
     def main_menu(self) -> None:
         """ Dialog.menu(text, height=None, width=None, menu_height=None,
         choices=[], **kwargs) Display a menu dialog box. """
         self.menu_initialization()  # reset
-        width: int = 50 + len(self.prg_name)
+        width: int = 56 + len(self.prg_name)
         text: str = "\nChoose an option or press <ESC> or <Cancel> to Exit."
-        title = f"{self.colors['bold']}{self.colors['green']}SBO Create Tool{self.colors['restore']}"
+        title = f"{self.color['bold']}{self.color['green']}SBO Create Tool{self.color['restore']}"
         code, tag = self.dialog.menu(
             text=text,
             title=title,
             height=27, width=width,
             menu_height=len(self.choices),
             choices=self.choices, help_button=True
         )
@@ -291,14 +309,15 @@
             self.get_help()
 
         case: dict = {
             'Info': self.edit_info_file,
             'Slack desc': self.edit_slack_desc_file,
             'SlackBuild': self.edit_slackbuild_file,
             'Doinst.sh': self.edit_doinst_file,
+            'Douninst.sh': self.edit_douninst_file,
             'Desktop': self.edit_desktop_file_file,
             'README': self.edit_readme_file,
             'Permissions': self.change_permissions,
             'Download': self.sources_download,
             'Checksum': self.update_the_checksum,
             'Check': self.is_the_sbo_exists,
             'Maintainer': self.edit_maintainer_file,
@@ -320,16 +339,16 @@
         maintainer: str = self.maintainer
         email: str = self.email
 
         self.read_info_file()
 
         # Replace maintainer data
         if maintainer and maintainer != self.maintainer:
-            yesno: str = self.dialog.yesno('Do you want to replace the maintainer data?',
-                                           height=7, width=50)
+            yesno: str = self.dialog.yesno('\nDo you want to replace the maintainer name or email?',
+                                           height=7, width=57)
 
             if yesno == 'ok':
                 self.maintainer: str = maintainer
                 self.email: str = email
 
         elements: list = [
             (self.info_text[0], 1, 1, self.prg_name, 1, len(self.info_text[0]) + 1,
@@ -350,15 +369,15 @@
              field_length - len(self.info_text[7]), input_length * 4, attributes),
             (self.info_text[8], 9, 1, self.maintainer, 9, len(self.info_text[8]) + 1,
              field_length - len(self.info_text[8]), input_length, attributes),
             (self.info_text[9], 10, 1, self.email, 10, len(self.info_text[9]) + 1,
              field_length - len(self.info_text[9]), input_length, attributes)
         ]
 
-        self.dialog_mixedform(comments=comments, title=info_file, elements=elements, height=19, width=79)
+        self.dialog_mixedform(comments=comments, title=info_file, elements=elements, height=19, width=78)
 
         if self.fields:
             self.version: str = self.fields[1]
             self.homepage: str = self.fields[2]
             self.download_x86: str = self.fields[3]
             self.md5sum_x86: str = self.fields[4]
             self.maintainer: str = self.fields[8]
@@ -401,15 +420,15 @@
             elements += [
                 (f'{self.prg_name}:', n, 1, line, n,
                  len(self.prg_name) + 2, field_length - len(self.prg_name),
                  input_length, attributes)
             ]
 
         self.dialog_mixedform(comments=f'\n{self.slack_desc_comments}', title='slack-desc', elements=elements,
-                              height=30, width=81 + len(self.prg_name))
+                              height=30, width=78 + len(self.prg_name))
 
         self.slack_desc_handy_ruler_comments(0)
         self.data: list = [line for line in self.slack_desc_comments.splitlines()]
 
         for line in self.fields:
             if not line.startswith(' ') and len(line) < 70:
                 line: str = f' {line}'
@@ -422,25 +441,26 @@
         self.read_info_file()
         version: str = self.version.replace('"', '')
         slackbuild: str = f'{self.prg_name}.SlackBuild'
         path_file: Path = Path(self.current_folder, slackbuild)
 
         if not path_file.is_file() and not self.template:
             choices: list = [
-                ('autotools', slackbuild, False),
-                ('cmake', slackbuild, False),
-                ('perl', slackbuild, False),
-                ('python', slackbuild, False),
-                ('rubygem', slackbuild, False),
-                ('haskell', slackbuild, False),
-                ('meson', slackbuild, False)
+                ('autotools', 'autotools-template.SlackBuild', False),
+                ('cmake', 'cmake-template.SlackBuild', False),
+                ('perl', 'perl-template.SlackBuild', False),
+                ('python', 'python-template.SlackBuild', False),
+                ('rubygem', 'rubygem-template.SlackBuild', False),
+                ('haskell', 'haskell-template.SlackBuild', False),
+                ('meson', 'meson-template.SlackBuild', False)
             ]
             message: str = f"\nChoose a template for the '{slackbuild}' file."
             code, self.template = self.dialog.radiolist(message, title=slackbuild,
-                                                        height=11, width=79, list_height=0, choices=choices)
+                                                        height=9, width=len(self.prg_name) + 50,
+                                                        list_height=0, choices=choices)
 
             if code == 'cancel':
                 self.main_menu()
 
         templates: dict = {
             'autotools': SlackBuilds(
                 self.prg_name, version, self.year, self.maintainer,
@@ -465,34 +485,47 @@
                 self.where_you_live).meson().splitlines
         }
 
         if self.template:
             try:
                 self.data = templates[self.template]()
             except KeyError:
-                message: str = '\nNo SlackBuild template was selected.'
+                message: str = f"\nThe template '{self.template}' is not exist."
                 self.dialog.msgbox(message, title=self.error_title, height=7, width=len(message) + 5)
                 self.main_menu()
 
+        if not self.template and not path_file.is_file():
+            message: str = '\nNo SlackBuild template selected.'
+            self.dialog.msgbox(message, title=self.error_title, height=7, width=len(message) + 5)
+            self.edit_slackbuild_file()
+
         if not path_file.is_file():
             message: str = f'\n{path_file.stem}.SlackBuild script created.'
             self.write_file(path_file)
             self.dialog.msgbox(message, title='Done', height=7, width=len(message) + 5)
 
         self.edit_file(path_file)
         self.main_menu()
 
     def edit_doinst_file(self) -> None:
         """ doinst.sh file handler file. """
         os.system('clear')
-        temp: str = '\n'.join(doinst_template().splitlines())
+        temp: str = '\n'.join(doinst_script().splitlines())
         pydoc.pipepager(temp, cmd='less -R')
         self.edit_file(Path(self.current_folder, 'doinst.sh'))
         self.main_menu()
 
+    def edit_douninst_file(self) -> None:
+        """ douninst.sh file handler file. """
+        os.system('clear')
+        temp: str = '\n'.join(douninst_script().splitlines())
+        pydoc.pipepager(temp, cmd='less -R')
+        self.edit_file(Path(self.current_folder, 'douninst.sh'))
+        self.main_menu()
+
     def edit_desktop_file_file(self) -> None:
         """ <prgnam>.desktop file handler. """
         desktop_file: str = f'{self.prg_name}.desktop'
         comments: str = f"\nCreates a '{desktop_file}' file."
         field_length: int = 72
         input_length: int = 100
         attributes: str = '0x0'
@@ -519,15 +552,15 @@
              attributes),
             (text[7], 8, 1, self.desktop_categories, 8, 12, field_length - len(text[7]),
              input_length, attributes),
             (text[8], 9, 1, self.desktop_generic_name, 9, 13, field_length - len(text[8]),
              input_length, attributes),
         ]
 
-        self.dialog_mixedform(comments=comments, title=desktop_file, elements=elements, height=17, width=79)
+        self.dialog_mixedform(comments=comments, title=desktop_file, elements=elements, height=18, width=78)
 
         if self.fields:
             self.prg_name: str = self.fields[1]
             self.desktop_comment: str = self.fields[2]
             self.desktop_exec: str = self.fields[3]
             self.desktop_icon: str = self.fields[4]
             self.desktop_terminal: str = self.fields[5]
@@ -632,25 +665,25 @@
 
         # Add the items to a list for choosing
         for k, v in files.items():
             choices += [
                 (v, k, False)
             ]
 
-        code1, tag1 = self.dialog.checklist(text=text1, title='Choose checksum', height=7 + len(files), width=79,
+        code1, tag1 = self.dialog.checklist(text=text1, title='Choose checksum', height=8 + len(files), width=78,
                                             list_height=0, choices=choices)
         if code1 == 'cancel':
             self.main_menu()
 
         choices: list = [
                 ('MD5SUM_x86', 'For x86 sources', False),
                 ('MD5SUM_x86_64', 'For x86_64 sources', False),
             ]
 
-        code2, tag2 = self.dialog.radiolist(text=text2, title='Select architecture', height=8, width=79,
+        code2, tag2 = self.dialog.radiolist(text=text2, title='Select architecture', height=9, width=78,
                                             list_height=0, choices=choices)
         if code2 == 'cancel':
             self.main_menu()
 
         if tag2 == 'MD5SUM_x86':
             self.md5sum_x86: str = ' '.join(tag1)
         elif tag2 == 'MD5SUM_x86_64':
@@ -661,72 +694,88 @@
     def is_the_sbo_exists(self) -> None:
         """ Checks if the SlackBuild exist in the repository. """
         self.dialog.infobox(f"\nSearching for '{self.prg_name}' please wait...",
                             width=len(self.prg_name) + 36, height=5)
         title: str = 'Done'
         message: str = f"\nNo SlackBuild found with the name '{self.prg_name}' in the repository."
 
-        repo: str = 'https://slackbuilds.org/slackbuilds/15.0/TAGS.txt'
+        mirror: str = f'https://slackbuilds.org/slackbuilds/{self.sbo_repo_version}/TAGS.txt'
         http = urllib3.PoolManager()
-        repo = http.request('GET', repo)
+
+        try:
+            repo = http.request('GET', mirror)
+        except HTTPError:
+            repo: str = str()
+            message: str = f"\nsbo-create: Error: Failed to connect to '{mirror}'"
 
         height: int = 7
         width: int = len(message) + 5
 
-        for sbo in repo.data.decode().splitlines():
-            if self.prg_name == sbo.split(':')[0]:
-                width: int = 50 + len(self.prg_name)
-                title: str = self.error_title
-                message: str = f"\nThe SlackBuild '{self.prg_name}' exists in the repository."
+        if repo:
+            for sbo in repo.data.decode().splitlines():
+                if self.prg_name == sbo.split(':')[0]:
+                    width: int = 50 + len(self.prg_name)
+                    title: str = self.error_title
+                    message: str = f"\nThe SlackBuild '{self.prg_name}' exists in the repository."
 
         self.dialog.msgbox(text=message, title=title, height=height, width=width)
         self.main_menu()
 
     def edit_maintainer_file(self) -> None:
         """ Maintainer data handler. """
         comments: str = '\nEnter the details of the maintainer data.'
         field_length: int = 68
         input_length: int = 100
         attributes: str = '0x0'
 
-        text = ['MAINTAINER=', 'EMAIL=', 'WHERE YOU LIVE=', 'EDITOR=', 'OPTIONS FOR EDITOR=']
+        text: tuple = (
+            'MAINTAINER=',
+            'EMAIL=',
+            'WHERE YOU LIVE=',
+            'EDITOR=',
+            'OPTIONS FOR EDITOR=',
+            'SBO REPOSITORY VERSION='
+        )
 
         elements: list = [
             (text[0], 1, 1, self.maintainer, 1, len(text[0]) + 1, field_length - len(text[0]), input_length,
              attributes),
             (text[1], 2, 1, self.email, 2, len(text[1]) + 1, field_length - len(text[1]), input_length,
              attributes),
             (text[2], 3, 1, self.where_you_live, 3, len(text[2]) + 1, field_length - len(text[2]), input_length,
              attributes),
             (text[3], 4, 1, self.editor, 4, len(text[3]) + 1, field_length - len(text[3]), input_length,
              attributes),
             (text[4], 5, 1, self.editor_options, 5, len(text[4]) + 1, field_length - len(text[4]), input_length,
+             attributes),
+            (text[5], 6, 1, self.sbo_repo_version, 6, len(text[5]) + 1, field_length - len(text[5]), input_length,
              attributes)
         ]
 
-        self.dialog_mixedform(comments=comments, title='Maintainer Data', elements=elements, height=14, width=75)
+        self.dialog_mixedform(comments=comments, title='Maintainer Data', elements=elements, height=15, width=75)
 
         if self.fields:
-            self.maintainer: str = self.fields[0]
-            self.email: str = self.fields[1]
-            self.where_you_live: str = self.fields[2]
-            self.editor: str = self.fields[3]
-            self.editor_options: str = self.fields[4]
+            self.maintainer: str = self.fields[0].strip()
+            self.email: str = self.fields[1].strip()
+            self.where_you_live: str = self.fields[2].strip()
+            self.editor: str = self.fields[3].strip()
+            self.editor_options: str = self.fields[4].strip()
+            self.sbo_repo_version: str = self.fields[5].strip()
 
             for item, field in zip(text, self.fields):
                 self.data.append(f'{item}{field}')
 
-        self.choose_for_write(Path(self.home_path, '.sbo-maintainer'))
+        self.choose_for_write(self.maintainer_config)
 
     def update_working_directory(self) -> None:
         comments: str = f'\nCurrent directory: {self.current_folder}'
         elements: list = [
             ('New path=', 1, 1, str(self.current_folder), 1, 10, 90, 90, '0x0'),
         ]
-        self.dialog_mixedform(comments=comments, title='Update directory', elements=elements, height=9, width=79)
+        self.dialog_mixedform(comments=comments, title='Update directory', elements=elements, height=10, width=78)
 
         if self.fields:
             if not os.path.isdir(self.fields[0].strip()):
                 message: str = f"\nDirectory '{self.fields[0].strip()}' is not exist."
                 self.dialog.msgbox(message, title=self.error_title, height=7, width=len(message) + 5)
                 self.update_working_directory()
 
@@ -736,33 +785,35 @@
             self.dialog.msgbox(message, title='Updated', height=7, width=len(message) + 5)
 
         self.main_menu()
 
     def get_help(self) -> None:
         """ Get help from slackbuilds.org. """
         message: str = ("\nFor additional assistance, visit:\n\n"
-                        f"SlackBuild Usage HOWTO: {self.colors['blue']}https://www.slackbuilds.org/howto/"
-                        f"{self.colors['restore']}\n"
-                        f"Frequently Asked Questions: {self.colors['blue']}https://www.slackbuilds.org/faq/"
-                        f"{self.colors['restore']}\n"
-                        f"Submission Guidelines: {self.colors['blue']}http://www.slackbuilds.org/guidelines/"
-                        f"{self.colors['restore']}\n")
+                        f"SlackBuild Usage HOWTO: {self.color['blue']}https://www.slackbuilds.org/howto/"
+                        f"{self.color['restore']}\n"
+                        f"Frequently Asked Questions: {self.color['blue']}https://www.slackbuilds.org/faq/"
+                        f"{self.color['restore']}\n"
+                        f"Submission Guidelines: {self.color['blue']}http://www.slackbuilds.org/guidelines/"
+                        f"{self.color['restore']}\n"
+                        f"SlackBuild Script Templates: {self.color['blue']}https://slackbuilds.org/templates/"
+                        f"{self.color['restore']}")
 
-        self.dialog.msgbox(message, title="Help", height=11, width=67)
+        self.dialog.msgbox(message, title="Help", height=12, width=68)
         self.main_menu()
 
     def about(self) -> None:
         """ About the sbo-create tool. """
         message: str = (
-            f"\n{self.colors['green']}{self.colors['bold']}"
-            f"SlackBuild Create Tool{self.colors['restore']}\n\n"
+            f"\n{self.color['green']}{self.color['bold']}"
+            f"SlackBuild Create Tool{self.color['restore']}\n\n"
             "A tool that creates easy, fast and safe SlackBuilds files scripts.\n"
             f"Version: {__version__}\n\n"
-            f"Homepage: {self.colors['blue']}https://gitlab.com/dslackw/"
-            f"sbo-create{self.colors['restore']}\n"
+            f"Homepage: {self.color['blue']}https://gitlab.com/dslackw/"
+            f"sbo-create{self.color['restore']}\n"
             "Copyright © 2015-2023 Dimitris Zlatanidis\n"
             "Email: dslackw@gmail.com\n\n"
             "Slackware ® is a Registered Trademark of Patrick Volkerding.\n"
             "Linux is a Registered Trademark of Linus Torvalds."
         )
 
         self.dialog.msgbox(message, title="About", height=17, width=70)
@@ -826,21 +877,19 @@
                 self.desktop_terminal: str = dsk[5].split('=')[1].strip()
                 self.desktop_type: str = dsk[6].split('=')[1].strip()
                 self.desktop_categories: str = dsk[7].split('=')[1].strip()
                 self.desktop_generic_name: str = dsk[8].split('=')[1].strip()
 
     def read_maintainer_file(self) -> None:
         """ Initialization maintainer data. """
-        maintainer_file: Path = Path(self.home_path, '.sbo-maintainer')
-
-        if maintainer_file.is_file():
-            with open(maintainer_file, 'r') as f:
+        if self.maintainer_config.is_file():
+            with open(self.maintainer_config, 'r') as f:
                 lines: list = f.read().splitlines()
 
-                if len(lines) == 5:
+                if len(lines) == 6:
 
                     if '=' in lines[0]:
                         self.maintainer: str = lines[0].split('=')[-1].strip()
 
                     if '=' in lines[1]:
                         self.email: str = lines[1].split('=')[-1].strip()
 
@@ -849,49 +898,52 @@
 
                     if '=' in lines[3]:
                         self.editor: str = lines[3].split('=')[-1].strip()
 
                     if '=' in lines[4]:
                         self.editor_options: str = lines[4].split('=')[-1].strip()
 
+                    if '=' in lines[5]:
+                        self.sbo_repo_version: str = lines[5].split('=')[-1].strip()
+
                 else:
-                    message: str = f"\nThe {maintainer_file} seems it's not correct."
+                    message: str = f"\nThe {self.config_file} seems it's not correct."
                     self.dialog.msgbox(message, title=self.error_title, height=7, width=len(message) + 5)
 
     def download(self, link: str) -> None:
         """ Wget downloader. """
         file: str = link.split("/")[-1]
 
         yesno: str = self.dialog.yesno(
-            f"\n{self.colors['blue']}{file}{self.colors['restore']}\n\n"
+            f"\n{self.color['blue']}{file}{self.color['restore']}\n\n"
             f"Do you want to download the file?", title='Download', height=9, width=40 + len(file)
         )
 
         if yesno == 'ok':
             self.dialog.infobox('\nDownloading, please wait...', width=32, height=5)
             time.sleep(1)
             output: int = subprocess.call(f'wget --continue {link}', shell=True,
                                           stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL)
 
             if output > 0:
-                self.dialog.msgbox(f"\nDownloading '{file}' {self.colors['red']}FAILED!{self.colors['restore']}",
+                self.dialog.msgbox(f"\nDownloading '{file}' {self.color['red']}FAILED!{self.color['restore']}",
                                    title=self.error_title, height=7, width=42 + len(self.prg_name))
             else:
                 self.dialog.msgbox(f"\nDownloading file '{file}' finished!", title="Done",
                                    height=7, width=35 + len(file))
 
     def is_package_installed(self) -> None:
         var_log_packages: Path = Path('/var/log/packages/')
         packages: list = [pkg.name for pkg in var_log_packages.iterdir()]
 
         for package in packages:
             name = '-'.join(package.split('-')[:-3])
             if name == self.prg_name:
                 yesno: str = self.dialog.yesno(
-                    f"{self.colors['red']}WARNING!{self.colors['restore']}"
+                    f"{self.color['red']}WARNING!{self.color['restore']}"
                     f" There is installed package with the name '{self.prg_name}'.\n"
                     '\nDo you want to continue?', height=8, width=60 + len(self.prg_name)
                 )
                 if yesno == 'cancel':
                     self.clear_and_exit()
 
     def dialog_mixedform(self, comments: str, title: str, elements: list, height: int, width) -> None:
@@ -1001,15 +1053,15 @@
         for info in info_file:
             if info.startswith(tag):
                 return info.split('=')[1].replace('"', '').strip()
 
     def checksum(self, md5sums: str) -> None:
         for source, md5 in zip(self.sources, md5sums.split()):
             if md5 != self.source_check_sum(source):
-                message: str = f"\nMD5SUM check for {source} {self.colors['red']}FAILED!{self.colors['restore']}"
+                message: str = f"\nMD5SUM check for {source} {self.color['red']}FAILED!{self.color['restore']}"
                 self.dialog.msgbox(message, title=self.error_title, height=7,
                                    width=len(message) + 5)
 
     def source_check_sum(self, source: str) -> str:
         """ md5sum sources. """
         file: Path = Path(self.current_folder, source)
         if file.is_file():
@@ -1052,15 +1104,7 @@
                 # Remove trailing whitespaces
                 line: str = line.rstrip()
                 f.write(f'{line}\n')
 
             # An empty line on the EOF
             if file.name == 'README':
                 f.write('\n')
-
-
-if __name__ == "__main__":
-    try:
-        app = SBoCreate()
-        app.main_menu()
-    except KeyboardInterrupt as err:
-        raise SystemExit(err)
```

