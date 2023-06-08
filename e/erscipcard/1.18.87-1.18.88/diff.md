# Comparing `tmp/erscipcard-1.18.87.tar.gz` & `tmp/erscipcard-1.18.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erscipcard-1.18.87.tar", last modified: Thu Jun  8 19:15:49 2023, max compression
+gzip compressed data, was "erscipcard-1.18.88.tar", last modified: Thu Jun  8 19:33:44 2023, max compression
```

## Comparing `erscipcard-1.18.87.tar` & `erscipcard-1.18.88.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:15:49.849084 erscipcard-1.18.87/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-06-08 19:15:41.000000 erscipcard-1.18.87/LICENSE
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-08 19:15:41.000000 erscipcard-1.18.87/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1627 2023-06-08 19:15:49.849084 erscipcard-1.18.87/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1332 2023-06-08 19:15:41.000000 erscipcard-1.18.87/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:15:49.835084 erscipcard-1.18.87/erscipcard/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/__init__.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/admin.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/apps.py
--rw-r--r--   0 root         (0) root         (0)      714 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/forms.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/inst.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:15:49.837084 erscipcard-1.18.87/erscipcard/migrations/
--rw-r--r--   0 root         (0) root         (0)     2100 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:15:49.840084 erscipcard-1.18.87/erscipcard/static/
--rw-r--r--   0 root         (0) root         (0)    11041 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/1.docx
--rw-r--r--   0 root         (0) root         (0)    11792 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/2.docx
--rw-r--r--   0 root         (0) root         (0)    60820 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/BNAZANIN.TTF
--rw-r--r--   0 root         (0) root         (0)    61268 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/BTITR.TTF
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:15:49.832084 erscipcard-1.18.87/erscipcard/static/bt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:15:49.841084 erscipcard-1.18.87/erscipcard/static/bt/css/
--rw-r--r--   0 root         (0) root         (0)   175814 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)    31000 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/css/font-awesome.min.css
--rw-r--r--   0 root         (0) root         (0)     9182 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/css/loginstyle.css
--rw-r--r--   0 root         (0) root         (0)     3804 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/css/persianDatepicker-default.css
--rw-r--r--   0 root         (0) root         (0)     5557 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/css/style.css
--rw-r--r--   0 root         (0) root         (0)    83821 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/css/util.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:15:49.842084 erscipcard-1.18.87/erscipcard/static/bt/fonts/
--rw-r--r--   0 root         (0) root         (0)    60820 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/fonts/BNAZANIN.TTF
--rw-r--r--   0 root         (0) root         (0)    61268 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/fonts/BTITR.TTF
--rw-r--r--   0 root         (0) root         (0)    84624 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/fonts/Vazir.ttf
--rw-r--r--   0 root         (0) root         (0)   165548 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/fonts/fontawesome-webfont.ttf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:15:49.843084 erscipcard-1.18.87/erscipcard/static/bt/js/
--rw-r--r--   0 root         (0) root         (0)    78694 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/js/bootstrap.bundle.min.js
--rw-r--r--   0 root         (0) root         (0)    88145 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/js/jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    29875 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/js/persianDatepicker.js
--rw-r--r--   0 root         (0) root         (0)     1728 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/js/scripts.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:15:49.843084 erscipcard-1.18.87/erscipcard/static/bt/pics/
--rw-r--r--   0 root         (0) root         (0)    29117 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/pics/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    35195 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/bt/pics/logo.png
--rw-r--r--   0 root         (0) root         (0)     4929 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/custom_modelField_with_formField
--rw-r--r--   0 root         (0) root         (0)    19286 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/ersci_app.zip
--rw-r--r--   0 root         (0) root         (0)    12683 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/ersci_viddown_tab2-1.4.xpi
--rw-r--r--   0 root         (0) root         (0)    29117 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)      696 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/inst
--rw-r--r--   0 root         (0) root         (0)    35195 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/logo.png
--rw-r--r--   0 root         (0) root         (0)     1126 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/main.css
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/s
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:15:49.848084 erscipcard-1.18.87/erscipcard/static/spinner/
--rw-r--r--   0 root         (0) root         (0)     7573 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/atebits.css
--rw-r--r--   0 root         (0) root         (0)    14641 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/ball.css
--rw-r--r--   0 root         (0) root         (0)     1716 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/circles.css
--rw-r--r--   0 root         (0) root         (0)    11683 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/dots.css
--rw-r--r--   0 root         (0) root         (0)     2705 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/echo.css
--rw-r--r--   0 root         (0) root         (0)     3476 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/flower.css
--rw-r--r--   0 root         (0) root         (0)     6259 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/gauge.css
--rw-r--r--   0 root         (0) root         (0)     3523 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/heartbeat.css
--rw-r--r--   0 root         (0) root         (0)    17599 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/hexdots.css
--rw-r--r--   0 root         (0) root         (0)     1421 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/hole-pulse.css
--rw-r--r--   0 root         (0) root         (0)     2713 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/inner-circles.css
--rw-r--r--   0 root         (0) root         (0)     6223 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/plus-loader.css
--rw-r--r--   0 root         (0) root         (0)    18677 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/plus.css
--rw-r--r--   0 root         (0) root         (0)    12802 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/pong.css
--rw-r--r--   0 root         (0) root         (0)     1437 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/pulse.css
--rw-r--r--   0 root         (0) root         (0)     1532 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/refreshing.css
--rw-r--r--   0 root         (0) root         (0)     2105 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/spinner.css
--rw-r--r--   0 root         (0) root         (0)     4661 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/spinning-pixels.css
--rw-r--r--   0 root         (0) root         (0)     1257 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/three-quarters.css
--rw-r--r--   0 root         (0) root         (0)     1599 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/throbber.css
--rw-r--r--   0 root         (0) root         (0)     2220 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/timer.css
--rw-r--r--   0 root         (0) root         (0)    22371 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/whirly.css
--rw-r--r--   0 root         (0) root         (0)     3093 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinner/wobblebar.css
--rw-r--r--   0 root         (0) root         (0)   143659 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/spinners.css
--rw-r--r--   0 root         (0) root         (0)        2 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/static/ytvid.mp4
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:15:49.848084 erscipcard-1.18.87/erscipcard/templates/
--rw-r--r--   0 root         (0) root         (0)      241 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/templates/AvatarFileUploadInput.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:15:49.849084 erscipcard-1.18.87/erscipcard/templates/erscipcard/
--rw-r--r--   0 root         (0) root         (0)     2606 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/templates/erscipcard/login.html
--rw-r--r--   0 root         (0) root         (0)    12711 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/templates/erscipcard/ou.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:15:49.849084 erscipcard-1.18.87/erscipcard/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      143 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/templatetags/basepath.py
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/tests.py
--rw-r--r--   0 root         (0) root         (0)     1342 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/urls.py
--rw-r--r--   0 root         (0) root         (0)    12726 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/views.py
--rw-r--r--   0 root         (0) root         (0)     1202 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/widget.py
--rw-r--r--   0 root         (0) root         (0)      573 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/yturls.py
--rw-r--r--   0 root         (0) root         (0)     8838 2023-06-08 19:15:41.000000 erscipcard-1.18.87/erscipcard/ytviews.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:15:49.836084 erscipcard-1.18.87/erscipcard.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1627 2023-06-08 19:15:49.000000 erscipcard-1.18.87/erscipcard.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2704 2023-06-08 19:15:49.000000 erscipcard-1.18.87/erscipcard.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 19:15:49.000000 erscipcard-1.18.87/erscipcard.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       93 2023-06-08 19:15:49.000000 erscipcard-1.18.87/erscipcard.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-08 19:15:49.000000 erscipcard-1.18.87/erscipcard.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      780 2023-06-08 19:15:49.850084 erscipcard-1.18.87/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-08 19:15:41.000000 erscipcard-1.18.87/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:33:44.783076 erscipcard-1.18.88/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-08 19:33:29.000000 erscipcard-1.18.88/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-08 19:33:29.000000 erscipcard-1.18.88/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-06-08 19:33:44.783076 erscipcard-1.18.88/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-06-08 19:33:29.000000 erscipcard-1.18.88/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:33:44.768076 erscipcard-1.18.88/erscipcard/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/admin.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/apps.py
+-rw-r--r--   0 root         (0) root         (0)      714 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/forms.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/inst.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:33:44.771076 erscipcard-1.18.88/erscipcard/migrations/
+-rw-r--r--   0 root         (0) root         (0)     2100 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:33:44.773076 erscipcard-1.18.88/erscipcard/static/
+-rw-r--r--   0 root         (0) root         (0)    11041 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/1.docx
+-rw-r--r--   0 root         (0) root         (0)    11792 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/2.docx
+-rw-r--r--   0 root         (0) root         (0)    60820 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/BNAZANIN.TTF
+-rw-r--r--   0 root         (0) root         (0)    61268 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/BTITR.TTF
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:33:44.765076 erscipcard-1.18.88/erscipcard/static/bt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:33:44.774076 erscipcard-1.18.88/erscipcard/static/bt/css/
+-rw-r--r--   0 root         (0) root         (0)   175814 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)    31000 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/css/font-awesome.min.css
+-rw-r--r--   0 root         (0) root         (0)     9182 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/css/loginstyle.css
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/css/persianDatepicker-default.css
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/css/style.css
+-rw-r--r--   0 root         (0) root         (0)    83821 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/css/util.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:33:44.775076 erscipcard-1.18.88/erscipcard/static/bt/fonts/
+-rw-r--r--   0 root         (0) root         (0)    60820 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/fonts/BNAZANIN.TTF
+-rw-r--r--   0 root         (0) root         (0)    61268 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/fonts/BTITR.TTF
+-rw-r--r--   0 root         (0) root         (0)    84624 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/fonts/Vazir.ttf
+-rw-r--r--   0 root         (0) root         (0)   165548 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/fonts/fontawesome-webfont.ttf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:33:44.777076 erscipcard-1.18.88/erscipcard/static/bt/js/
+-rw-r--r--   0 root         (0) root         (0)    78694 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/js/bootstrap.bundle.min.js
+-rw-r--r--   0 root         (0) root         (0)    88145 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/js/jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    29875 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/js/persianDatepicker.js
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/js/scripts.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:33:44.777076 erscipcard-1.18.88/erscipcard/static/bt/pics/
+-rw-r--r--   0 root         (0) root         (0)    29117 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/pics/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    35195 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/bt/pics/logo.png
+-rw-r--r--   0 root         (0) root         (0)     4929 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/custom_modelField_with_formField
+-rw-r--r--   0 root         (0) root         (0)    19286 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/ersci_app.zip
+-rw-r--r--   0 root         (0) root         (0)    12683 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/ersci_viddown_tab2-1.4.xpi
+-rw-r--r--   0 root         (0) root         (0)    29117 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)      696 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/inst
+-rw-r--r--   0 root         (0) root         (0)    35195 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/logo.png
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/main.css
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/s
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:33:44.782076 erscipcard-1.18.88/erscipcard/static/spinner/
+-rw-r--r--   0 root         (0) root         (0)     7573 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/atebits.css
+-rw-r--r--   0 root         (0) root         (0)    14641 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/ball.css
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/circles.css
+-rw-r--r--   0 root         (0) root         (0)    11683 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/dots.css
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/echo.css
+-rw-r--r--   0 root         (0) root         (0)     3476 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/flower.css
+-rw-r--r--   0 root         (0) root         (0)     6259 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/gauge.css
+-rw-r--r--   0 root         (0) root         (0)     3523 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/heartbeat.css
+-rw-r--r--   0 root         (0) root         (0)    17599 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/hexdots.css
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/hole-pulse.css
+-rw-r--r--   0 root         (0) root         (0)     2713 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/inner-circles.css
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/plus-loader.css
+-rw-r--r--   0 root         (0) root         (0)    18677 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/plus.css
+-rw-r--r--   0 root         (0) root         (0)    12802 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/pong.css
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/pulse.css
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/refreshing.css
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/spinner.css
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/spinning-pixels.css
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/three-quarters.css
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/throbber.css
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/timer.css
+-rw-r--r--   0 root         (0) root         (0)    22371 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/whirly.css
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinner/wobblebar.css
+-rw-r--r--   0 root         (0) root         (0)   143659 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/spinners.css
+-rw-r--r--   0 root         (0) root         (0)        2 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/static/ytvid.mp4
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:33:44.782076 erscipcard-1.18.88/erscipcard/templates/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/templates/AvatarFileUploadInput.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:33:44.782076 erscipcard-1.18.88/erscipcard/templates/erscipcard/
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/templates/erscipcard/login.html
+-rw-r--r--   0 root         (0) root         (0)    12711 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/templates/erscipcard/ou.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:33:44.782076 erscipcard-1.18.88/erscipcard/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      143 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/templatetags/basepath.py
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/urls.py
+-rw-r--r--   0 root         (0) root         (0)    12726 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/views.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/widget.py
+-rw-r--r--   0 root         (0) root         (0)      264 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/yturls.py
+-rw-r--r--   0 root         (0) root         (0)     8838 2023-06-08 19:33:29.000000 erscipcard-1.18.88/erscipcard/ytviews.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:33:44.770076 erscipcard-1.18.88/erscipcard.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-06-08 19:33:44.000000 erscipcard-1.18.88/erscipcard.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2704 2023-06-08 19:33:44.000000 erscipcard-1.18.88/erscipcard.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 19:33:44.000000 erscipcard-1.18.88/erscipcard.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-08 19:33:44.000000 erscipcard-1.18.88/erscipcard.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-08 19:33:44.000000 erscipcard-1.18.88/erscipcard.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      780 2023-06-08 19:33:44.783076 erscipcard-1.18.88/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-08 19:33:29.000000 erscipcard-1.18.88/setup.py
```

### Comparing `erscipcard-1.18.87/LICENSE` & `erscipcard-1.18.88/LICENSE`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/PKG-INFO` & `erscipcard-1.18.88/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erscipcard
-Version: 1.18.87
+Version: 1.18.88
 Summary: Erscipcard is a Django app to create personeli card.
 Home-page: https://github.com/epg900/erscipcard.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `erscipcard-1.18.87/README.md` & `erscipcard-1.18.88/README.md`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/forms.py` & `erscipcard-1.18.88/erscipcard/forms.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/inst.py` & `erscipcard-1.18.88/erscipcard/inst.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os,re
 
 def delproj():
     os.system('rm -r proj')
+    os.system('rm -r s')
     
 def run():
     try:
         os.system('''
         sudo apt install -y nginx
         sudo sed -i "s/root \/var\/www\/html/root \/tmp/" /etc/nginx/sites-enabled/default
         sudo sed -i "s/index index.html/index a.mp4 index.html/" /etc/nginx/sites-enabled/default
@@ -22,15 +23,20 @@
         f=open ('proj/proj/settings.py', 'w' )
         f.write(content_new)
         f.close()
         f=open ('proj/proj/urls.py', 'r' )
         content = f.read()
         content_new = re.sub('(from django.urls import path)', r"\1,include", content, flags = re.M)
         content_new = re.sub('(urlpatterns = \[)', r"\1\n\t\tpath('yt/', include('erscipcard.yturls')),", content_new, flags = re.M)
+        content_new = re.sub('(urlpatterns = \[)', r"\1\n\t\tpath('erscipcard/', include('erscipcard.urls')),", content_new, flags = re.M)
         f.close()
         f=open ('proj/proj/urls.py', 'w' )
         f.write(content_new)
-        f.close()        
+        f.close() 
+        os.system('python proj/manage.py migrate')
+        os.system('echo "python proj/manage.py runserver" > s')
+        os.system('chmod +x s')
+        os.system('python proj/manage.py createsuperuser --username=admin')
         os.system('python proj/manage.py runserver')
     except:
         print('Error in command')
```

### Comparing `erscipcard-1.18.87/erscipcard/migrations/0001_initial.py` & `erscipcard-1.18.88/erscipcard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/models.py` & `erscipcard-1.18.88/erscipcard/models.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/1.docx` & `erscipcard-1.18.88/erscipcard/static/1.docx`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/2.docx` & `erscipcard-1.18.88/erscipcard/static/2.docx`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/BNAZANIN.TTF` & `erscipcard-1.18.88/erscipcard/static/BNAZANIN.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/BTITR.TTF` & `erscipcard-1.18.88/erscipcard/static/BTITR.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/css/bootstrap.min.css` & `erscipcard-1.18.88/erscipcard/static/bt/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/css/font-awesome.min.css` & `erscipcard-1.18.88/erscipcard/static/bt/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/css/loginstyle.css` & `erscipcard-1.18.88/erscipcard/static/bt/css/loginstyle.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/css/persianDatepicker-default.css` & `erscipcard-1.18.88/erscipcard/static/bt/css/persianDatepicker-default.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/css/style.css` & `erscipcard-1.18.88/erscipcard/static/bt/css/style.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/css/util.css` & `erscipcard-1.18.88/erscipcard/static/bt/css/util.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/fonts/BNAZANIN.TTF` & `erscipcard-1.18.88/erscipcard/static/bt/fonts/BNAZANIN.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/fonts/BTITR.TTF` & `erscipcard-1.18.88/erscipcard/static/bt/fonts/BTITR.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/fonts/Vazir.ttf` & `erscipcard-1.18.88/erscipcard/static/bt/fonts/Vazir.ttf`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/fonts/fontawesome-webfont.ttf` & `erscipcard-1.18.88/erscipcard/static/bt/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/js/bootstrap.bundle.min.js` & `erscipcard-1.18.88/erscipcard/static/bt/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/js/jquery.min.js` & `erscipcard-1.18.88/erscipcard/static/bt/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/js/persianDatepicker.js` & `erscipcard-1.18.88/erscipcard/static/bt/js/persianDatepicker.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/js/scripts.js` & `erscipcard-1.18.88/erscipcard/static/bt/js/scripts.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/pics/favicon.ico` & `erscipcard-1.18.88/erscipcard/static/bt/pics/favicon.ico`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/bt/pics/logo.png` & `erscipcard-1.18.88/erscipcard/static/bt/pics/logo.png`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/custom_modelField_with_formField` & `erscipcard-1.18.88/erscipcard/static/custom_modelField_with_formField`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/ersci_app.zip` & `erscipcard-1.18.88/erscipcard/static/ersci_app.zip`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/ersci_viddown_tab2-1.4.xpi` & `erscipcard-1.18.88/erscipcard/static/ersci_viddown_tab2-1.4.xpi`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/favicon.ico` & `erscipcard-1.18.88/erscipcard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/inst` & `erscipcard-1.18.88/erscipcard/static/inst`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/logo.png` & `erscipcard-1.18.88/erscipcard/static/logo.png`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/main.css` & `erscipcard-1.18.88/erscipcard/static/main.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/atebits.css` & `erscipcard-1.18.88/erscipcard/static/spinner/atebits.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/ball.css` & `erscipcard-1.18.88/erscipcard/static/spinner/ball.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/circles.css` & `erscipcard-1.18.88/erscipcard/static/spinner/circles.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/dots.css` & `erscipcard-1.18.88/erscipcard/static/spinner/dots.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/echo.css` & `erscipcard-1.18.88/erscipcard/static/spinner/echo.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/flower.css` & `erscipcard-1.18.88/erscipcard/static/spinner/flower.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/gauge.css` & `erscipcard-1.18.88/erscipcard/static/spinner/gauge.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/heartbeat.css` & `erscipcard-1.18.88/erscipcard/static/spinner/heartbeat.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/hexdots.css` & `erscipcard-1.18.88/erscipcard/static/spinner/hexdots.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/hole-pulse.css` & `erscipcard-1.18.88/erscipcard/static/spinner/hole-pulse.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/inner-circles.css` & `erscipcard-1.18.88/erscipcard/static/spinner/inner-circles.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/plus-loader.css` & `erscipcard-1.18.88/erscipcard/static/spinner/plus-loader.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/plus.css` & `erscipcard-1.18.88/erscipcard/static/spinner/plus.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/pong.css` & `erscipcard-1.18.88/erscipcard/static/spinner/pong.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/pulse.css` & `erscipcard-1.18.88/erscipcard/static/spinner/pulse.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/refreshing.css` & `erscipcard-1.18.88/erscipcard/static/spinner/refreshing.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/spinner.css` & `erscipcard-1.18.88/erscipcard/static/spinner/spinner.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/spinning-pixels.css` & `erscipcard-1.18.88/erscipcard/static/spinner/spinning-pixels.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/three-quarters.css` & `erscipcard-1.18.88/erscipcard/static/spinner/three-quarters.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/throbber.css` & `erscipcard-1.18.88/erscipcard/static/spinner/throbber.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/timer.css` & `erscipcard-1.18.88/erscipcard/static/spinner/timer.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/whirly.css` & `erscipcard-1.18.88/erscipcard/static/spinner/whirly.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinner/wobblebar.css` & `erscipcard-1.18.88/erscipcard/static/spinner/wobblebar.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/static/spinners.css` & `erscipcard-1.18.88/erscipcard/static/spinners.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/templates/erscipcard/login.html` & `erscipcard-1.18.88/erscipcard/templates/erscipcard/login.html`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/templates/erscipcard/ou.html` & `erscipcard-1.18.88/erscipcard/templates/erscipcard/ou.html`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/urls.py` & `erscipcard-1.18.88/erscipcard/urls.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/views.py` & `erscipcard-1.18.88/erscipcard/views.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/widget.py` & `erscipcard-1.18.88/erscipcard/widget.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard/ytviews.py` & `erscipcard-1.18.88/erscipcard/ytviews.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/erscipcard.egg-info/PKG-INFO` & `erscipcard-1.18.88/erscipcard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erscipcard
-Version: 1.18.87
+Version: 1.18.88
 Summary: Erscipcard is a Django app to create personeli card.
 Home-page: https://github.com/epg900/erscipcard.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `erscipcard-1.18.87/erscipcard.egg-info/SOURCES.txt` & `erscipcard-1.18.88/erscipcard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erscipcard-1.18.87/setup.cfg` & `erscipcard-1.18.88/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = erscipcard
-version = 1.18.87
+version = 1.18.88
 description = Erscipcard is a Django app to create personeli card.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/erscipcard.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

