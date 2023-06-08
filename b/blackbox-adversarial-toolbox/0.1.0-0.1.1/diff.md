# Comparing `tmp/blackbox-adversarial-toolbox-0.1.0.tar.gz` & `tmp/blackbox-adversarial-toolbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/wuhanstudio/Desktop/blackbox-adversarial-toolbox/dist/.tmp-trjizarc/blackbox-adversarial-toolbox-0.1.0.tar", last modified: Wed May 31 20:03:45 2023, max compression
+gzip compressed data, was "/home/wuhanstudio/Desktop/blackbox-adversarial-toolbox/dist/.tmp-s5iensif/blackbox-adversarial-toolbox-0.1.1.tar", last modified: Thu Jun  8 15:18:07 2023, max compression
```

## Comparing `blackbox-adversarial-toolbox-0.1.0.tar` & `blackbox-adversarial-toolbox-0.1.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.618601 blackbox-adversarial-toolbox-0.1.0/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1063 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.0/LICENSE
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       66 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.0/MANIFEST.in
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2814 2023-05-31 20:03:45.618601 blackbox-adversarial-toolbox-0.1.0/PKG-INFO
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2003 2023-05-31 18:15:05.000000 blackbox-adversarial-toolbox-0.1.0/README.md
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.386601 blackbox-adversarial-toolbox-0.1.0/bat/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      664 2023-05-31 19:49:55.000000 blackbox-adversarial-toolbox-0.1.0/bat/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       32 2023-05-29 16:18:42.000000 blackbox-adversarial-toolbox-0.1.0/bat/__main__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6142 2023-05-31 19:12:14.000000 blackbox-adversarial-toolbox-0.1.0/bat/_main.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.386601 blackbox-adversarial-toolbox-0.1.0/bat/apis/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1423 2023-05-31 19:52:33.000000 blackbox-adversarial-toolbox-0.1.0/bat/apis/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7399 2023-05-30 15:37:52.000000 blackbox-adversarial-toolbox-0.1.0/bat/apis/deepapi.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1762 2023-05-30 13:00:18.000000 blackbox-adversarial-toolbox-0.1.0/bat/apis/google.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1740 2023-05-30 10:10:16.000000 blackbox-adversarial-toolbox-0.1.0/bat/apis/imagga.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.386601 blackbox-adversarial-toolbox-0.1.0/bat/attacks/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      647 2023-05-31 19:58:51.000000 blackbox-adversarial-toolbox-0.1.0/bat/attacks/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     9770 2023-05-31 15:05:16.000000 blackbox-adversarial-toolbox-0.1.0/bat/attacks/bandits_attack.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      456 2023-05-30 13:18:48.000000 blackbox-adversarial-toolbox-0.1.0/bat/attacks/base_attack.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7697 2023-05-31 15:02:36.000000 blackbox-adversarial-toolbox-0.1.0/bat/attacks/simba_attack.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    11962 2023-05-31 14:32:21.000000 blackbox-adversarial-toolbox-0.1.0/bat/attacks/square_attack.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.386601 blackbox-adversarial-toolbox-0.1.0/bat/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      101 2023-05-31 19:20:30.000000 blackbox-adversarial-toolbox-0.1.0/bat/utils/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      417 2023-05-31 19:21:21.000000 blackbox-adversarial-toolbox-0.1.0/bat/utils/proj_lp.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.386601 blackbox-adversarial-toolbox-0.1.0/blackbox_adversarial_toolbox.egg-info/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2814 2023-05-31 20:03:45.000000 blackbox-adversarial-toolbox-0.1.0/blackbox_adversarial_toolbox.egg-info/PKG-INFO
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2254 2023-05-31 20:03:45.000000 blackbox-adversarial-toolbox-0.1.0/blackbox_adversarial_toolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        1 2023-05-31 20:03:45.000000 blackbox-adversarial-toolbox-0.1.0/blackbox_adversarial_toolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       39 2023-05-31 20:03:45.000000 blackbox-adversarial-toolbox-0.1.0/blackbox_adversarial_toolbox.egg-info/entry_points.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      121 2023-05-31 20:03:45.000000 blackbox-adversarial-toolbox-0.1.0/blackbox_adversarial_toolbox.egg-info/requires.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        4 2023-05-31 20:03:45.000000 blackbox-adversarial-toolbox-0.1.0/blackbox_adversarial_toolbox.egg-info/top_level.txt
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.410601 blackbox-adversarial-toolbox-0.1.0/docs/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       65 2023-05-31 19:45:15.000000 blackbox-adversarial-toolbox-0.1.0/docs/.gitignore
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       18 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.0/docs/CNAME
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.422601 blackbox-adversarial-toolbox-0.1.0/docs/bat/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    89180 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.0/docs/bat/_main.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.426601 blackbox-adversarial-toolbox-0.1.0/docs/bat/apis/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   215108 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.0/docs/bat/apis/deepapi.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    79194 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.0/docs/bat/apis/google.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    78801 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.0/docs/bat/apis/imagga.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    47991 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.0/docs/bat/apis.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.426601 blackbox-adversarial-toolbox-0.1.0/docs/bat/attacks/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   241850 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.0/docs/bat/attacks/bandits_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    51220 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.0/docs/bat/attacks/base_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   207128 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.0/docs/bat/attacks/simba_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   320760 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.0/docs/bat/attacks/square_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    39236 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.0/docs/bat/attacks.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.426601 blackbox-adversarial-toolbox-0.1.0/docs/bat/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    43263 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.0/docs/bat/utils/proj_lp.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    36169 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.0/docs/bat/utils.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    39713 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.0/docs/bat.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.426601 blackbox-adversarial-toolbox-0.1.0/docs/images/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    20406 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.0/docs/images/bat.png
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    78710 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.0/docs/images/bat_dark.png
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      134 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.0/docs/index.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    58126 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.0/docs/search.js
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.426601 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.470601 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.514601 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/apis/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.514601 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/apis/deepapi/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    64415 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/apis/deepapi/vgg16_cifar10.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    33716 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/apis/deepapi.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    35555 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/apis.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.526601 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/attacks/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   100303 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/attacks/simba.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    33350 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/attacks.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.526601 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    37997 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/utils/proj_lp.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    33067 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/utils.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    34852 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    32039 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/index.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    26612 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/search.js
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.534601 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.554601 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    89180 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/_main.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.558601 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/apis/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   215108 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/apis/deepapi.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    79194 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/apis/google.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    78801 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/apis/imagga.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    46920 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/apis.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.558601 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/attacks/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   241850 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/attacks/bandits_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    51220 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/attacks/base_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   207128 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/attacks/simba_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   320760 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/attacks/square_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    38456 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/attacks.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.558601 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    43263 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/utils/proj_lp.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    36169 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/utils.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    40297 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      134 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/index.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    57902 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/search.js
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1241 2023-05-31 18:35:39.000000 blackbox-adversarial-toolbox-0.1.0/pyproject.toml
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       38 2023-05-31 20:03:45.618601 blackbox-adversarial-toolbox-0.1.0/setup.cfg
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2253 2023-05-31 18:41:26.000000 blackbox-adversarial-toolbox-0.1.0/setup.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.578601 blackbox-adversarial-toolbox-0.1.0/tests/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-31 20:03:45.610601 blackbox-adversarial-toolbox-0.1.0/tests/__pycache__/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2334 2023-05-30 13:40:51.000000 blackbox-adversarial-toolbox-0.1.0/tests/__pycache__/test_deepapi.cpython-38-pytest-7.3.1.pyc
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1329 2023-05-30 13:32:48.000000 blackbox-adversarial-toolbox-0.1.0/tests/__pycache__/test_deepapi.cpython-38.pyc
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2582 2023-05-30 13:40:51.000000 blackbox-adversarial-toolbox-0.1.0/tests/__pycache__/test_simba.cpython-38-pytest-7.3.1.pyc
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1581 2023-05-30 13:38:49.000000 blackbox-adversarial-toolbox-0.1.0/tests/__pycache__/test_simba.cpython-38.pyc
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2971 2023-05-31 14:56:46.000000 blackbox-adversarial-toolbox-0.1.0/tests/__pycache__/test_square.cpython-38-pytest-7.3.1.pyc
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    57480 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.0/tests/cat.jpg
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    19151 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.0/tests/dog.jpg
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1263 2023-05-30 13:32:43.000000 blackbox-adversarial-toolbox-0.1.0/tests/test_deepapi.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1835 2023-05-30 13:38:48.000000 blackbox-adversarial-toolbox-0.1.0/tests/test_simba.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2309 2023-05-31 14:56:43.000000 blackbox-adversarial-toolbox-0.1.0/tests/test_square.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.292251 blackbox-adversarial-toolbox-0.1.1/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1063 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.1/LICENSE
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       66 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.1/MANIFEST.in
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3084 2023-06-08 15:18:07.292251 blackbox-adversarial-toolbox-0.1.1/PKG-INFO
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2047 2023-06-08 15:17:10.000000 blackbox-adversarial-toolbox-0.1.1/README.md
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.084251 blackbox-adversarial-toolbox-0.1.1/bat/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      664 2023-06-08 15:17:28.000000 blackbox-adversarial-toolbox-0.1.1/bat/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       32 2023-05-29 16:18:42.000000 blackbox-adversarial-toolbox-0.1.1/bat/__main__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6142 2023-05-31 19:12:14.000000 blackbox-adversarial-toolbox-0.1.1/bat/_main.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.084251 blackbox-adversarial-toolbox-0.1.1/bat/apis/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1423 2023-05-31 19:52:33.000000 blackbox-adversarial-toolbox-0.1.1/bat/apis/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7399 2023-05-30 15:37:52.000000 blackbox-adversarial-toolbox-0.1.1/bat/apis/deepapi.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1762 2023-05-30 13:00:18.000000 blackbox-adversarial-toolbox-0.1.1/bat/apis/google.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1740 2023-05-30 10:10:16.000000 blackbox-adversarial-toolbox-0.1.1/bat/apis/imagga.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.084251 blackbox-adversarial-toolbox-0.1.1/bat/attacks/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      647 2023-05-31 19:58:51.000000 blackbox-adversarial-toolbox-0.1.1/bat/attacks/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     9770 2023-05-31 15:05:16.000000 blackbox-adversarial-toolbox-0.1.1/bat/attacks/bandits_attack.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      456 2023-05-30 13:18:48.000000 blackbox-adversarial-toolbox-0.1.1/bat/attacks/base_attack.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7697 2023-05-31 15:02:36.000000 blackbox-adversarial-toolbox-0.1.1/bat/attacks/simba_attack.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    11962 2023-05-31 14:32:21.000000 blackbox-adversarial-toolbox-0.1.1/bat/attacks/square_attack.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.084251 blackbox-adversarial-toolbox-0.1.1/bat/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      101 2023-05-31 19:20:30.000000 blackbox-adversarial-toolbox-0.1.1/bat/utils/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      417 2023-05-31 19:21:21.000000 blackbox-adversarial-toolbox-0.1.1/bat/utils/proj_lp.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.084251 blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3084 2023-06-08 15:18:07.000000 blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2254 2023-06-08 15:18:07.000000 blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        1 2023-06-08 15:18:07.000000 blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       39 2023-06-08 15:18:07.000000 blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      121 2023-06-08 15:18:07.000000 blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/requires.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        4 2023-06-08 15:18:07.000000 blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/top_level.txt
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.104251 blackbox-adversarial-toolbox-0.1.1/docs/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       65 2023-05-31 19:45:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/.gitignore
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       18 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.1/docs/CNAME
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.116251 blackbox-adversarial-toolbox-0.1.1/docs/bat/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    89180 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/_main.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.128251 blackbox-adversarial-toolbox-0.1.1/docs/bat/apis/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   215108 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/apis/deepapi.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    79194 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/apis/google.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    78801 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/apis/imagga.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    47991 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/apis.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.136251 blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   241850 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/bandits_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    51220 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/base_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   207128 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/simba_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   320760 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/square_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    39236 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.144251 blackbox-adversarial-toolbox-0.1.1/docs/bat/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    43263 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/utils/proj_lp.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    36169 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/utils.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    39713 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.144251 blackbox-adversarial-toolbox-0.1.1/docs/images/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    20406 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.1/docs/images/bat.png
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    78710 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.1/docs/images/bat_dark.png
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      134 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/index.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    58126 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/search.js
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.160251 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.180251 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.180251 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.180251 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis/deepapi/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    64415 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis/deepapi/vgg16_cifar10.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    33716 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis/deepapi.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    35555 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.184251 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/attacks/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   100303 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/attacks/simba.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    33350 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/attacks.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.192251 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    37997 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/utils/proj_lp.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    33067 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/utils.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    34852 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    32039 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/index.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    26612 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/search.js
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.220251 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.248252 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    89180 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/_main.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.264252 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   215108 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis/deepapi.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    79194 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis/google.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    78801 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis/imagga.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    46920 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.272251 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   241850 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/bandits_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    51220 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/base_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   207128 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/simba_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   320760 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/square_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    38456 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.272251 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    43263 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/utils/proj_lp.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    36169 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/utils.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    40297 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      134 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/index.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    57902 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/search.js
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1447 2023-06-08 15:17:16.000000 blackbox-adversarial-toolbox-0.1.1/pyproject.toml
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       38 2023-06-08 15:18:07.292251 blackbox-adversarial-toolbox-0.1.1/setup.cfg
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1996 2023-06-08 15:17:10.000000 blackbox-adversarial-toolbox-0.1.1/setup.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.276251 blackbox-adversarial-toolbox-0.1.1/tests/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.284252 blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2334 2023-05-30 13:40:51.000000 blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_deepapi.cpython-38-pytest-7.3.1.pyc
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1329 2023-05-30 13:32:48.000000 blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_deepapi.cpython-38.pyc
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2582 2023-05-30 13:40:51.000000 blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_simba.cpython-38-pytest-7.3.1.pyc
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1581 2023-05-30 13:38:49.000000 blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_simba.cpython-38.pyc
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2971 2023-05-31 14:56:46.000000 blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_square.cpython-38-pytest-7.3.1.pyc
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    57480 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.1/tests/cat.jpg
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    19151 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.1/tests/dog.jpg
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1263 2023-05-30 13:32:43.000000 blackbox-adversarial-toolbox-0.1.1/tests/test_deepapi.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1835 2023-05-30 13:38:48.000000 blackbox-adversarial-toolbox-0.1.1/tests/test_simba.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2309 2023-05-31 14:56:43.000000 blackbox-adversarial-toolbox-0.1.1/tests/test_square.py
```

### Comparing `blackbox-adversarial-toolbox-0.1.0/LICENSE` & `blackbox-adversarial-toolbox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/PKG-INFO` & `blackbox-adversarial-toolbox-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 626c 6163  : 2.1.Name: blac
 00000020: 6b62 6f78 2d61 6476 6572 7361 7269 616c  kbox-adversarial
 00000030: 2d74 6f6f 6c62 6f78 0a56 6572 7369 6f6e  -toolbox.Version
-00000040: 3a20 302e 312e 300a 5375 6d6d 6172 793a  : 0.1.0.Summary:
+00000040: 3a20 302e 312e 310a 5375 6d6d 6172 793a  : 0.1.1.Summary:
 00000050: 2042 6c61 636b 2d62 6f78 2041 6476 6572   Black-box Adver
 00000060: 7361 7269 616c 2054 6f6f 6c62 6f78 2028  sarial Toolbox (
 00000070: 4241 5429 202d 2050 7974 686f 6e20 4c69  BAT) - Python Li
 00000080: 6272 6172 7920 666f 7220 4465 6570 204c  brary for Deep L
 00000090: 6561 726e 696e 6720 5365 6375 7269 7479  earning Security
 000000a0: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
 000000b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f77  s://github.com/w
@@ -30,147 +30,164 @@
 000001d0: 782d 6164 7665 7273 6172 6961 6c2d 746f  x-adversarial-to
 000001e0: 6f6c 626f 780a 5072 6f6a 6563 742d 5552  olbox.Project-UR
 000001f0: 4c3a 2042 7567 2054 7261 636b 6572 2c20  L: Bug Tracker, 
 00000200: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
 00000210: 6f6d 2f77 7568 616e 7374 7564 696f 2f62  om/wuhanstudio/b
 00000220: 6c61 636b 626f 782d 6164 7665 7273 6172  lackbox-adversar
 00000230: 6961 6c2d 746f 6f6c 626f 782f 6973 7375  ial-toolbox/issu
-00000240: 6573 0a43 6c61 7373 6966 6965 723a 2050  es.Classifier: P
-00000250: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000260: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000270: 2033 0a43 6c61 7373 6966 6965 723a 204c   3.Classifier: L
-00000280: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-00000290: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
-000002a0: 6365 6e73 650a 436c 6173 7369 6669 6572  cense.Classifier
-000002b0: 3a20 4f70 6572 6174 696e 6720 5379 7374  : Operating Syst
-000002c0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-000002d0: 6465 6e74 0a52 6571 7569 7265 732d 5079  dent.Requires-Py
-000002e0: 7468 6f6e 3a20 3e3d 332e 360a 4465 7363  thon: >=3.6.Desc
-000002f0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-00000300: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-00000310: 6f77 6e0a 4c69 6365 6e73 652d 4669 6c65  own.License-File
-00000320: 3a20 4c49 4345 4e53 450a 0a3c 696d 6720  : LICENSE..<img 
-00000330: 7372 633d 2268 7474 7073 3a2f 2f62 6174  src="https://bat
-00000340: 2e77 7568 616e 7374 7564 696f 2e75 6b2f  .wuhanstudio.uk/
-00000350: 696d 6167 6573 2f62 6174 2e70 6e67 2220  images/bat.png" 
-00000360: 7769 6474 683d 3330 3070 7820 7374 796c  width=300px styl
-00000370: 653d 2266 6c6f 6174 3a20 6c65 6674 3b22  e="float: left;"
-00000380: 203e 0a0a 2320 426c 6163 6b2d 626f 7820   >..# Black-box 
-00000390: 4164 7665 7273 6172 6961 6c20 546f 6f6c  Adversarial Tool
-000003a0: 626f 7820 2842 4154 290a 0a0a 5b21 5b42  box (BAT)...[![B
-000003b0: 7569 6c64 2053 7461 7475 735d 2868 7474  uild Status](htt
-000003c0: 7073 3a2f 2f61 7070 2e74 7261 7669 732d  ps://app.travis-
-000003d0: 6369 2e63 6f6d 2f77 7568 616e 7374 7564  ci.com/wuhanstud
-000003e0: 696f 2f62 6c61 636b 626f 782d 6164 7665  io/blackbox-adve
-000003f0: 7273 6172 6961 6c2d 746f 6f6c 626f 782e  rsarial-toolbox.
-00000400: 7376 673f 6272 616e 6368 3d6d 6173 7465  svg?branch=maste
-00000410: 7229 5d28 6874 7470 733a 2f2f 6170 702e  r)](https://app.
-00000420: 7472 6176 6973 2d63 692e 636f 6d2f 7775  travis-ci.com/wu
-00000430: 6861 6e73 7475 6469 6f2f 626c 6163 6b62  hanstudio/blackb
-00000440: 6f78 2d61 6476 6572 7361 7269 616c 2d74  ox-adversarial-t
-00000450: 6f6f 6c62 6f78 290a 5b21 5b50 7950 4920  oolbox).[![PyPI 
-00000460: 7665 7273 696f 6e5d 2868 7474 7073 3a2f  version](https:/
-00000470: 2f62 6164 6765 2e66 7572 792e 696f 2f70  /badge.fury.io/p
-00000480: 792f 626c 6163 6b62 6f78 2d61 6476 6572  y/blackbox-adver
-00000490: 7361 7269 616c 2d74 6f6f 6c62 6f78 2e73  sarial-toolbox.s
-000004a0: 7667 295d 2868 7474 7073 3a2f 2f62 6164  vg)](https://bad
-000004b0: 6765 2e66 7572 792e 696f 2f70 792f 626c  ge.fury.io/py/bl
-000004c0: 6163 6b62 6f78 2d61 6476 6572 7361 7269  ackbox-adversari
-000004d0: 616c 2d74 6f6f 6c62 6f78 290a 5b21 5b4c  al-toolbox).[![L
-000004e0: 6963 656e 7365 3a20 4d49 545d 2868 7474  icense: MIT](htt
-000004f0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000500: 2e69 6f2f 6261 6467 652f 4c69 6365 6e73  .io/badge/Licens
-00000510: 652d 4d49 542d 7965 6c6c 6f77 2e73 7667  e-MIT-yellow.svg
-00000520: 295d 2868 7474 7073 3a2f 2f6f 7065 6e73  )](https://opens
-00000530: 6f75 7263 652e 6f72 672f 6c69 6365 6e73  ource.org/licens
-00000540: 6573 2f4d 4954 290a 5b21 5b50 7950 4920  es/MIT).[![PyPI 
-00000550: 2d20 5079 7468 6f6e 2056 6572 7369 6f6e  - Python Version
-00000560: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000570: 6965 6c64 732e 696f 2f70 7970 692f 7079  ields.io/pypi/py
-00000580: 7665 7273 696f 6e73 2f62 6c61 636b 626f  versions/blackbo
-00000590: 782d 6164 7665 7273 6172 6961 6c2d 746f  x-adversarial-to
-000005a0: 6f6c 626f 7829 5d28 6874 7470 733a 2f2f  olbox)](https://
-000005b0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-000005c0: 2f62 6c61 636b 626f 782d 6164 7665 7273  /blackbox-advers
-000005d0: 6172 6961 6c2d 746f 6f6c 626f 782f 290a  arial-toolbox/).
-000005e0: 0a41 2050 7974 686f 6e20 4c69 6272 6172  .A Python Librar
-000005f0: 7920 666f 7220 4465 6570 204c 6561 726e  y for Deep Learn
-00000600: 696e 6720 5365 6375 7269 7479 2074 6861  ing Security tha
-00000610: 7420 666f 6375 7365 7320 6f6e 2044 6973  t focuses on Dis
-00000620: 7472 6962 7574 6564 2042 6c61 636b 2d62  tributed Black-b
-00000630: 6f78 2061 7474 6163 6b73 2e0a 0a0a 2323  ox attacks....##
-00000640: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a60   Installation..`
-00000650: 6060 7079 7468 6f6e 0a70 6970 2069 6e73  ``python.pip ins
-00000660: 7461 6c6c 2062 6c61 636b 626f 782d 6164  tall blackbox-ad
-00000670: 7665 7273 6172 6961 6c2d 746f 6f6c 626f  versarial-toolbo
-00000680: 780a 6060 600a 0a0a 2323 2055 7361 6765  x.```...## Usage
-00000690: 2028 434c 4929 0a0a 6060 600a 5573 6167   (CLI)..```.Usag
-000006a0: 653a 2062 6174 205b 4f50 5449 4f4e 535d  e: bat [OPTIONS]
-000006b0: 2043 4f4d 4d41 4e44 205b 4152 4753 5d2e   COMMAND [ARGS].
-000006c0: 2e2e 0a0a 2020 5468 6520 434c 4920 746f  ....  The CLI to
-000006d0: 6f6c 2066 6f72 2042 6c61 636b 2d62 6f78  ol for Black-box
-000006e0: 2041 6476 6572 7361 7269 616c 2054 6f6f   Adversarial Too
-000006f0: 6c62 6f78 2028 4241 5429 2e0a 0a4f 7074  lbox (BAT)...Opt
-00000700: 696f 6e73 3a0a 2020 2d2d 6865 6c70 2020  ions:.  --help  
-00000710: 5368 6f77 2074 6869 7320 6d65 7373 6167  Show this messag
-00000720: 6520 616e 6420 6578 6974 2e0a 0a43 6f6d  e and exit...Com
-00000730: 6d61 6e64 733a 0a20 2061 7069 2020 2020  mands:.  api    
-00000740: 2020 4d61 6e61 6765 2043 6c6f 7564 2041    Manage Cloud A
-00000750: 5049 730a 2020 6174 7461 636b 2020 204d  PIs.  attack   M
-00000760: 616e 6167 6520 4174 7461 636b 730a 2020  anage Attacks.  
-00000770: 6578 616d 706c 6520 204d 616e 6167 6520  example  Manage 
-00000780: 4578 616d 706c 6573 0a60 6060 0a55 7365  Examples.```.Use
-00000790: 6675 6c20 636f 6d6d 616e 6473 3a0a 6060  ful commands:.``
-000007a0: 600a 2320 4c69 7374 2073 7570 706f 7274  `.# List support
-000007b0: 6564 2043 6c6f 7564 2041 5049 730a 6261  ed Cloud APIs.ba
-000007c0: 7420 6170 6920 6c69 7374 0a0a 2320 4c69  t api list..# Li
-000007d0: 7374 2073 7570 6f72 7465 6420 4174 7461  st suported Atta
-000007e0: 636b 730a 6261 7420 6174 7461 636b 206c  cks.bat attack l
-000007f0: 6973 740a 0a23 2054 6573 7420 436c 6f75  ist..# Test Clou
-00000800: 6420 4150 4973 0a62 6174 2061 7069 2072  d APIs.bat api r
-00000810: 756e 2064 6565 7061 7069 0a62 6174 2061  un deepapi.bat a
-00000820: 7069 2072 756e 2067 6f6f 676c 650a 6261  pi run google.ba
-00000830: 7420 6170 6920 7275 6e20 696d 6167 6761  t api run imagga
-00000840: 0a0a 2320 5275 6e20 6578 6d61 706c 6573  ..# Run exmaples
-00000850: 0a62 6174 2065 7861 6d70 6c65 2072 756e  .bat example run
-00000860: 2073 696d 6261 5f64 6565 7061 7069 0a62   simba_deepapi.b
-00000870: 6174 2065 7861 6d70 6c65 2072 756e 2062  at example run b
-00000880: 616e 6469 7473 5f64 6565 7061 7069 0a62  andits_deepapi.b
-00000890: 6174 2065 7861 6d70 6c65 2072 756e 2073  at example run s
-000008a0: 7175 6172 655f 6465 6570 6170 690a 6060  quare_deepapi.``
-000008b0: 600a 0a23 2320 5573 6167 6520 2850 7974  `..## Usage (Pyt
-000008c0: 686f 6e29 0a0a 6060 6070 7974 686f 6e0a  hon)..```python.
-000008d0: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
-000008e0: 6e70 0a66 726f 6d20 5049 4c20 696d 706f  np.from PIL impo
-000008f0: 7274 2049 6d61 6765 0a0a 6672 6f6d 2062  rt Image..from b
-00000900: 6174 2e61 7474 6163 6b73 2069 6d70 6f72  at.attacks impor
-00000910: 7420 5369 6d42 410a 6672 6f6d 2062 6174  t SimBA.from bat
-00000920: 2e61 7069 732e 6465 6570 6170 6920 696d  .apis.deepapi im
-00000930: 706f 7274 2044 6565 7041 5049 5f56 4747  port DeepAPI_VGG
-00000940: 3136 5f43 6966 6172 3130 0a0a 2320 4c6f  16_Cifar10..# Lo
-00000950: 6164 2049 6d61 6765 0a78 203d 206e 702e  ad Image.x = np.
-00000960: 6173 6172 7261 7928 496d 6167 652e 6f70  asarray(Image.op
-00000970: 656e 2822 646f 672e 6a70 6722 292e 636f  en("dog.jpg").co
-00000980: 6e76 6572 7428 2752 4742 2729 290a 7820  nvert('RGB')).x 
-00000990: 3d20 6e70 2e61 7272 6179 285b 785d 290a  = np.array([x]).
-000009a0: 0a23 2049 6e69 7469 616c 697a 6520 7468  .# Initialize th
-000009b0: 6520 436c 6f75 6420 4150 4920 4d6f 6465  e Cloud API Mode
-000009c0: 6c0a 4445 4550 5f41 5049 5f55 524c 203d  l.DEEP_API_URL =
-000009d0: 2027 6874 7470 3a2f 2f6c 6f63 616c 686f   'http://localho
-000009e0: 7374 3a38 3038 3027 0a6d 6f64 656c 203d  st:8080'.model =
-000009f0: 2044 6565 7041 5049 5f56 4747 3136 5f43   DeepAPI_VGG16_C
-00000a00: 6966 6172 3130 2844 4545 505f 4150 495f  ifar10(DEEP_API_
-00000a10: 5552 4c29 0a0a 2320 4765 7420 5072 6564  URL)..# Get Pred
-00000a20: 6974 6374 696f 6e0a 795f 7072 6564 203d  itction.y_pred =
-00000a30: 206d 6f64 656c 2e70 7265 6469 6374 2878   model.predict(x
-00000a40: 295b 305d 0a0a 2320 4469 7374 7269 6275  )[0]..# Distribu
-00000a50: 7465 6420 5369 6d42 4120 4174 7461 636b  ted SimBA Attack
-00000a60: 0a73 696d 6261 203d 2053 696d 4241 286d  .simba = SimBA(m
-00000a70: 6f64 656c 290a 785f 6164 7620 3d20 7369  odel).x_adv = si
-00000a80: 6d62 612e 6174 7461 636b 2878 2c20 6e70  mba.attack(x, np
-00000a90: 2e61 7267 6d61 7828 795f 7072 6564 292c  .argmax(y_pred),
-00000aa0: 2065 7073 696c 6f6e 3d30 2e30 352c 206d   epsilon=0.05, m
-00000ab0: 6178 5f69 743d 3130 290a 6060 600a 0a3c  ax_it=10).```..<
-00000ac0: 6833 3e20 3c61 2068 7265 663d 2268 7474  h3> <a href="htt
-00000ad0: 7073 3a2f 2f62 6174 2e77 7568 616e 7374  ps://bat.wuhanst
-00000ae0: 7564 696f 2e75 6b2f 223e 2044 6f63 756d  udio.uk/"> Docum
-00000af0: 656e 7461 7469 6f6e 203c 2f61 3e0a       entation </a>.
+00000240: 6573 0a43 6c61 7373 6966 6965 723a 2049  es.Classifier: I
+00000250: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+00000260: 203a 3a20 5363 6965 6e63 652f 5265 7365   :: Science/Rese
+00000270: 6172 6368 0a43 6c61 7373 6966 6965 723a  arch.Classifier:
+00000280: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
+00000290: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+000002a0: 4c69 6365 6e73 650a 436c 6173 7369 6669  License.Classifi
+000002b0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000002c0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002d0: 6f6e 203a 3a20 332e 360a 436c 6173 7369  on :: 3.6.Classi
+000002e0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000002f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000300: 7468 6f6e 203a 3a20 332e 370a 436c 6173  thon :: 3.7.Clas
+00000310: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000320: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000330: 5079 7468 6f6e 203a 3a20 332e 380a 436c  Python :: 3.8.Cl
+00000340: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000350: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000360: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
+00000370: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+00000380: 6320 3a3a 2053 6369 656e 7469 6669 632f  c :: Scientific/
+00000390: 456e 6769 6e65 6572 696e 6720 3a3a 2041  Engineering :: A
+000003a0: 7274 6966 6963 6961 6c20 496e 7465 6c6c  rtificial Intell
+000003b0: 6967 656e 6365 0a52 6571 7569 7265 732d  igence.Requires-
+000003c0: 5079 7468 6f6e 3a20 3e3d 332e 360a 4465  Python: >=3.6.De
+000003d0: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
+000003e0: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
+000003f0: 6b64 6f77 6e0a 4c69 6365 6e73 652d 4669  kdown.License-Fi
+00000400: 6c65 3a20 4c49 4345 4e53 450a 0a3c 696d  le: LICENSE..<im
+00000410: 6720 7372 633d 2268 7474 7073 3a2f 2f62  g src="https://b
+00000420: 6174 2e77 7568 616e 7374 7564 696f 2e75  at.wuhanstudio.u
+00000430: 6b2f 696d 6167 6573 2f62 6174 2e70 6e67  k/images/bat.png
+00000440: 2220 7769 6474 683d 3330 3070 7820 7374  " width=300px st
+00000450: 796c 653d 2266 6c6f 6174 3a20 6c65 6674  yle="float: left
+00000460: 3b22 203e 0a0a 2320 426c 6163 6b2d 626f  ;" >..# Black-bo
+00000470: 7820 4164 7665 7273 6172 6961 6c20 546f  x Adversarial To
+00000480: 6f6c 626f 7820 2842 4154 290a 0a5b 215b  olbox (BAT)..[![
+00000490: 4275 696c 6420 5374 6174 7573 5d28 6874  Build Status](ht
+000004a0: 7470 733a 2f2f 6170 702e 7472 6176 6973  tps://app.travis
+000004b0: 2d63 692e 636f 6d2f 7775 6861 6e73 7475  -ci.com/wuhanstu
+000004c0: 6469 6f2f 626c 6163 6b62 6f78 2d61 6476  dio/blackbox-adv
+000004d0: 6572 7361 7269 616c 2d74 6f6f 6c62 6f78  ersarial-toolbox
+000004e0: 2e73 7667 3f62 7261 6e63 683d 6d61 7374  .svg?branch=mast
+000004f0: 6572 295d 2868 7474 7073 3a2f 2f61 7070  er)](https://app
+00000500: 2e74 7261 7669 732d 6369 2e63 6f6d 2f77  .travis-ci.com/w
+00000510: 7568 616e 7374 7564 696f 2f62 6c61 636b  uhanstudio/black
+00000520: 626f 782d 6164 7665 7273 6172 6961 6c2d  box-adversarial-
+00000530: 746f 6f6c 626f 7829 0a5b 215b 5079 5049  toolbox).[![PyPI
+00000540: 2076 6572 7369 6f6e 5d28 6874 7470 733a   version](https:
+00000550: 2f2f 6261 6467 652e 6675 7279 2e69 6f2f  //badge.fury.io/
+00000560: 7079 2f62 6c61 636b 626f 782d 6164 7665  py/blackbox-adve
+00000570: 7273 6172 6961 6c2d 746f 6f6c 626f 782e  rsarial-toolbox.
+00000580: 7376 6729 5d28 6874 7470 733a 2f2f 6261  svg)](https://ba
+00000590: 6467 652e 6675 7279 2e69 6f2f 7079 2f62  dge.fury.io/py/b
+000005a0: 6c61 636b 626f 782d 6164 7665 7273 6172  lackbox-adversar
+000005b0: 6961 6c2d 746f 6f6c 626f 7829 0a5b 215b  ial-toolbox).[![
+000005c0: 4c69 6365 6e73 653a 204d 4954 5d28 6874  License: MIT](ht
+000005d0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000005e0: 732e 696f 2f62 6164 6765 2f4c 6963 656e  s.io/badge/Licen
+000005f0: 7365 2d4d 4954 2d79 656c 6c6f 772e 7376  se-MIT-yellow.sv
+00000600: 6729 5d28 6874 7470 733a 2f2f 6f70 656e  g)](https://open
+00000610: 736f 7572 6365 2e6f 7267 2f6c 6963 656e  source.org/licen
+00000620: 7365 732f 4d49 5429 0a5b 215b 5079 5049  ses/MIT).[![PyPI
+00000630: 202d 2050 7974 686f 6e20 5665 7273 696f   - Python Versio
+00000640: 6e5d 2868 7474 7073 3a2f 2f69 6d67 2e73  n](https://img.s
+00000650: 6869 656c 6473 2e69 6f2f 7079 7069 2f70  hields.io/pypi/p
+00000660: 7976 6572 7369 6f6e 732f 626c 6163 6b62  yversions/blackb
+00000670: 6f78 2d61 6476 6572 7361 7269 616c 2d74  ox-adversarial-t
+00000680: 6f6f 6c62 6f78 295d 2868 7474 7073 3a2f  oolbox)](https:/
+00000690: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+000006a0: 742f 626c 6163 6b62 6f78 2d61 6476 6572  t/blackbox-adver
+000006b0: 7361 7269 616c 2d74 6f6f 6c62 6f78 2f29  sarial-toolbox/)
+000006c0: 0a5b 215b 5d28 6874 7470 733a 2f2f 696d  .[![](https://im
+000006d0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+000006e0: 6765 2f44 6f63 756d 656e 7461 7469 6f6e  ge/Documentation
+000006f0: 2d69 6e66 726f 6d61 7469 6f6e 616c 295d  -infromational)]
+00000700: 2868 7474 7073 3a2f 2f62 6174 2e77 7568  (https://bat.wuh
+00000710: 616e 7374 7564 696f 2e75 6b2f 290a 0a41  anstudio.uk/)..A
+00000720: 2050 7974 686f 6e20 4c69 6272 6172 7920   Python Library 
+00000730: 666f 7220 4465 6570 204c 6561 726e 696e  for Deep Learnin
+00000740: 6720 5365 6375 7269 7479 2074 6861 7420  g Security that 
+00000750: 666f 6375 7365 7320 6f6e 2044 6973 7472  focuses on Distr
+00000760: 6962 7574 6564 2042 6c61 636b 2d62 6f78  ibuted Black-box
+00000770: 2061 7474 6163 6b73 2e0a 0a23 2320 496e   attacks...## In
+00000780: 7374 616c 6c61 7469 6f6e 0a0a 6060 6070  stallation..```p
+00000790: 7974 686f 6e0a 7069 7020 696e 7374 616c  ython.pip instal
+000007a0: 6c20 626c 6163 6b62 6f78 2d61 6476 6572  l blackbox-adver
+000007b0: 7361 7269 616c 2d74 6f6f 6c62 6f78 0a60  sarial-toolbox.`
+000007c0: 6060 0a0a 0a23 2320 5573 6167 6520 2843  ``...## Usage (C
+000007d0: 4c49 290a 0a60 6060 0a55 7361 6765 3a20  LI)..```.Usage: 
+000007e0: 6261 7420 5b4f 5054 494f 4e53 5d20 434f  bat [OPTIONS] CO
+000007f0: 4d4d 414e 4420 5b41 5247 535d 2e2e 2e0a  MMAND [ARGS]....
+00000800: 0a20 2054 6865 2043 4c49 2074 6f6f 6c20  .  The CLI tool 
+00000810: 666f 7220 426c 6163 6b2d 626f 7820 4164  for Black-box Ad
+00000820: 7665 7273 6172 6961 6c20 546f 6f6c 626f  versarial Toolbo
+00000830: 7820 2842 4154 292e 0a0a 4f70 7469 6f6e  x (BAT)...Option
+00000840: 733a 0a20 202d 2d68 656c 7020 2053 686f  s:.  --help  Sho
+00000850: 7720 7468 6973 206d 6573 7361 6765 2061  w this message a
+00000860: 6e64 2065 7869 742e 0a0a 436f 6d6d 616e  nd exit...Comman
+00000870: 6473 3a0a 2020 6170 6920 2020 2020 204d  ds:.  api      M
+00000880: 616e 6167 6520 436c 6f75 6420 4150 4973  anage Cloud APIs
+00000890: 0a20 2061 7474 6163 6b20 2020 4d61 6e61  .  attack   Mana
+000008a0: 6765 2041 7474 6163 6b73 0a20 2065 7861  ge Attacks.  exa
+000008b0: 6d70 6c65 2020 4d61 6e61 6765 2045 7861  mple  Manage Exa
+000008c0: 6d70 6c65 730a 6060 600a 5573 6566 756c  mples.```.Useful
+000008d0: 2063 6f6d 6d61 6e64 733a 0a60 6060 0a23   commands:.```.#
+000008e0: 204c 6973 7420 7375 7070 6f72 7465 6420   List supported 
+000008f0: 436c 6f75 6420 4150 4973 0a24 2062 6174  Cloud APIs.$ bat
+00000900: 2061 7069 206c 6973 740a 0a23 204c 6973   api list..# Lis
+00000910: 7420 7375 7070 6f72 7465 6420 4174 7461  t supported Atta
+00000920: 636b 730a 2420 6261 7420 6174 7461 636b  cks.$ bat attack
+00000930: 206c 6973 740a 0a23 2054 6573 7420 436c   list..# Test Cl
+00000940: 6f75 6420 4150 4973 0a24 2062 6174 2061  oud APIs.$ bat a
+00000950: 7069 2072 756e 2064 6565 7061 7069 0a24  pi run deepapi.$
+00000960: 2062 6174 2061 7069 2072 756e 2067 6f6f   bat api run goo
+00000970: 676c 650a 2420 6261 7420 6170 6920 7275  gle.$ bat api ru
+00000980: 6e20 696d 6167 6761 0a0a 2320 5275 6e20  n imagga..# Run 
+00000990: 6578 6d61 706c 6573 0a24 2062 6174 2065  exmaples.$ bat e
+000009a0: 7861 6d70 6c65 2072 756e 2073 696d 6261  xample run simba
+000009b0: 5f64 6565 7061 7069 0a24 2062 6174 2065  _deepapi.$ bat e
+000009c0: 7861 6d70 6c65 2072 756e 2062 616e 6469  xample run bandi
+000009d0: 7473 5f64 6565 7061 7069 0a24 2062 6174  ts_deepapi.$ bat
+000009e0: 2065 7861 6d70 6c65 2072 756e 2073 7175   example run squ
+000009f0: 6172 655f 6465 6570 6170 690a 6060 600a  are_deepapi.```.
+00000a00: 0a23 2320 5573 6167 6520 2850 7974 686f  .## Usage (Pytho
+00000a10: 6e29 0a0a 6060 6070 7974 686f 6e0a 696d  n)..```python.im
+00000a20: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
+00000a30: 0a66 726f 6d20 5049 4c20 696d 706f 7274  .from PIL import
+00000a40: 2049 6d61 6765 0a0a 6672 6f6d 2062 6174   Image..from bat
+00000a50: 2e61 7474 6163 6b73 2069 6d70 6f72 7420  .attacks import 
+00000a60: 5369 6d42 410a 6672 6f6d 2062 6174 2e61  SimBA.from bat.a
+00000a70: 7069 732e 6465 6570 6170 6920 696d 706f  pis.deepapi impo
+00000a80: 7274 2044 6565 7041 5049 5f56 4747 3136  rt DeepAPI_VGG16
+00000a90: 5f43 6966 6172 3130 0a0a 2320 4c6f 6164  _Cifar10..# Load
+00000aa0: 2049 6d61 6765 0a78 203d 206e 702e 6173   Image.x = np.as
+00000ab0: 6172 7261 7928 496d 6167 652e 6f70 656e  array(Image.open
+00000ac0: 2822 646f 672e 6a70 6722 292e 636f 6e76  ("dog.jpg").conv
+00000ad0: 6572 7428 2752 4742 2729 290a 7820 3d20  ert('RGB')).x = 
+00000ae0: 6e70 2e61 7272 6179 285b 785d 290a 0a23  np.array([x])..#
+00000af0: 2049 6e69 7469 616c 697a 6520 7468 6520   Initialize the 
+00000b00: 436c 6f75 6420 4150 4920 4d6f 6465 6c0a  Cloud API Model.
+00000b10: 4445 4550 5f41 5049 5f55 524c 203d 2027  DEEP_API_URL = '
+00000b20: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
+00000b30: 3a38 3038 3027 0a6d 6f64 656c 203d 2044  :8080'.model = D
+00000b40: 6565 7041 5049 5f56 4747 3136 5f43 6966  eepAPI_VGG16_Cif
+00000b50: 6172 3130 2844 4545 505f 4150 495f 5552  ar10(DEEP_API_UR
+00000b60: 4c29 0a0a 2320 4765 7420 5072 6564 6974  L)..# Get Predit
+00000b70: 6374 696f 6e0a 795f 7072 6564 203d 206d  ction.y_pred = m
+00000b80: 6f64 656c 2e70 7265 6469 6374 2878 295b  odel.predict(x)[
+00000b90: 305d 0a0a 2320 4469 7374 7269 6275 7465  0]..# Distribute
+00000ba0: 6420 5369 6d42 4120 4174 7461 636b 0a73  d SimBA Attack.s
+00000bb0: 696d 6261 203d 2053 696d 4241 286d 6f64  imba = SimBA(mod
+00000bc0: 656c 290a 785f 6164 7620 3d20 7369 6d62  el).x_adv = simb
+00000bd0: 612e 6174 7461 636b 2878 2c20 6e70 2e61  a.attack(x, np.a
+00000be0: 7267 6d61 7828 795f 7072 6564 292c 2065  rgmax(y_pred), e
+00000bf0: 7073 696c 6f6e 3d30 2e30 352c 206d 6178  psilon=0.05, max
+00000c00: 5f69 743d 3130 290a 6060 600a            _it=10).```.
```

### Comparing `blackbox-adversarial-toolbox-0.1.0/README.md` & `blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,126 +1,193 @@
-00000000: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000010: 2f2f 6261 742e 7775 6861 6e73 7475 6469  //bat.wuhanstudi
-00000020: 6f2e 756b 2f69 6d61 6765 732f 6261 742e  o.uk/images/bat.
-00000030: 706e 6722 2077 6964 7468 3d33 3030 7078  png" width=300px
-00000040: 2073 7479 6c65 3d22 666c 6f61 743a 206c   style="float: l
-00000050: 6566 743b 2220 3e0a 0a23 2042 6c61 636b  eft;" >..# Black
-00000060: 2d62 6f78 2041 6476 6572 7361 7269 616c  -box Adversarial
-00000070: 2054 6f6f 6c62 6f78 2028 4241 5429 0a0a   Toolbox (BAT)..
-00000080: 0a5b 215b 4275 696c 6420 5374 6174 7573  .[![Build Status
-00000090: 5d28 6874 7470 733a 2f2f 6170 702e 7472  ](https://app.tr
-000000a0: 6176 6973 2d63 692e 636f 6d2f 7775 6861  avis-ci.com/wuha
-000000b0: 6e73 7475 6469 6f2f 626c 6163 6b62 6f78  nstudio/blackbox
-000000c0: 2d61 6476 6572 7361 7269 616c 2d74 6f6f  -adversarial-too
-000000d0: 6c62 6f78 2e73 7667 3f62 7261 6e63 683d  lbox.svg?branch=
-000000e0: 6d61 7374 6572 295d 2868 7474 7073 3a2f  master)](https:/
-000000f0: 2f61 7070 2e74 7261 7669 732d 6369 2e63  /app.travis-ci.c
-00000100: 6f6d 2f77 7568 616e 7374 7564 696f 2f62  om/wuhanstudio/b
-00000110: 6c61 636b 626f 782d 6164 7665 7273 6172  lackbox-adversar
-00000120: 6961 6c2d 746f 6f6c 626f 7829 0a5b 215b  ial-toolbox).[![
-00000130: 5079 5049 2076 6572 7369 6f6e 5d28 6874  PyPI version](ht
-00000140: 7470 733a 2f2f 6261 6467 652e 6675 7279  tps://badge.fury
-00000150: 2e69 6f2f 7079 2f62 6c61 636b 626f 782d  .io/py/blackbox-
-00000160: 6164 7665 7273 6172 6961 6c2d 746f 6f6c  adversarial-tool
-00000170: 626f 782e 7376 6729 5d28 6874 7470 733a  box.svg)](https:
-00000180: 2f2f 6261 6467 652e 6675 7279 2e69 6f2f  //badge.fury.io/
-00000190: 7079 2f62 6c61 636b 626f 782d 6164 7665  py/blackbox-adve
-000001a0: 7273 6172 6961 6c2d 746f 6f6c 626f 7829  rsarial-toolbox)
-000001b0: 0a5b 215b 4c69 6365 6e73 653a 204d 4954  .[![License: MIT
-000001c0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000001d0: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
-000001e0: 6963 656e 7365 2d4d 4954 2d79 656c 6c6f  icense-MIT-yello
-000001f0: 772e 7376 6729 5d28 6874 7470 733a 2f2f  w.svg)](https://
-00000200: 6f70 656e 736f 7572 6365 2e6f 7267 2f6c  opensource.org/l
-00000210: 6963 656e 7365 732f 4d49 5429 0a5b 215b  icenses/MIT).[![
-00000220: 5079 5049 202d 2050 7974 686f 6e20 5665  PyPI - Python Ve
-00000230: 7273 696f 6e5d 2868 7474 7073 3a2f 2f69  rsion](https://i
-00000240: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000250: 7069 2f70 7976 6572 7369 6f6e 732f 626c  pi/pyversions/bl
-00000260: 6163 6b62 6f78 2d61 6476 6572 7361 7269  ackbox-adversari
-00000270: 616c 2d74 6f6f 6c62 6f78 295d 2868 7474  al-toolbox)](htt
-00000280: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-00000290: 6f6a 6563 742f 626c 6163 6b62 6f78 2d61  oject/blackbox-a
-000002a0: 6476 6572 7361 7269 616c 2d74 6f6f 6c62  dversarial-toolb
-000002b0: 6f78 2f29 0a0a 4120 5079 7468 6f6e 204c  ox/)..A Python L
-000002c0: 6962 7261 7279 2066 6f72 2044 6565 7020  ibrary for Deep 
-000002d0: 4c65 6172 6e69 6e67 2053 6563 7572 6974  Learning Securit
-000002e0: 7920 7468 6174 2066 6f63 7573 6573 206f  y that focuses o
-000002f0: 6e20 4469 7374 7269 6275 7465 6420 426c  n Distributed Bl
-00000300: 6163 6b2d 626f 7820 6174 7461 636b 732e  ack-box attacks.
-00000310: 0a0a 0a23 2320 496e 7374 616c 6c61 7469  ...## Installati
-00000320: 6f6e 0a0a 6060 6070 7974 686f 6e0a 7069  on..```python.pi
-00000330: 7020 696e 7374 616c 6c20 626c 6163 6b62  p install blackb
-00000340: 6f78 2d61 6476 6572 7361 7269 616c 2d74  ox-adversarial-t
-00000350: 6f6f 6c62 6f78 0a60 6060 0a0a 0a23 2320  oolbox.```...## 
-00000360: 5573 6167 6520 2843 4c49 290a 0a60 6060  Usage (CLI)..```
-00000370: 0a55 7361 6765 3a20 6261 7420 5b4f 5054  .Usage: bat [OPT
-00000380: 494f 4e53 5d20 434f 4d4d 414e 4420 5b41  IONS] COMMAND [A
-00000390: 5247 535d 2e2e 2e0a 0a20 2054 6865 2043  RGS].....  The C
-000003a0: 4c49 2074 6f6f 6c20 666f 7220 426c 6163  LI tool for Blac
-000003b0: 6b2d 626f 7820 4164 7665 7273 6172 6961  k-box Adversaria
-000003c0: 6c20 546f 6f6c 626f 7820 2842 4154 292e  l Toolbox (BAT).
-000003d0: 0a0a 4f70 7469 6f6e 733a 0a20 202d 2d68  ..Options:.  --h
-000003e0: 656c 7020 2053 686f 7720 7468 6973 206d  elp  Show this m
-000003f0: 6573 7361 6765 2061 6e64 2065 7869 742e  essage and exit.
-00000400: 0a0a 436f 6d6d 616e 6473 3a0a 2020 6170  ..Commands:.  ap
-00000410: 6920 2020 2020 204d 616e 6167 6520 436c  i      Manage Cl
-00000420: 6f75 6420 4150 4973 0a20 2061 7474 6163  oud APIs.  attac
-00000430: 6b20 2020 4d61 6e61 6765 2041 7474 6163  k   Manage Attac
-00000440: 6b73 0a20 2065 7861 6d70 6c65 2020 4d61  ks.  example  Ma
-00000450: 6e61 6765 2045 7861 6d70 6c65 730a 6060  nage Examples.``
-00000460: 600a 5573 6566 756c 2063 6f6d 6d61 6e64  `.Useful command
-00000470: 733a 0a60 6060 0a23 204c 6973 7420 7375  s:.```.# List su
-00000480: 7070 6f72 7465 6420 436c 6f75 6420 4150  pported Cloud AP
-00000490: 4973 0a62 6174 2061 7069 206c 6973 740a  Is.bat api list.
-000004a0: 0a23 204c 6973 7420 7375 706f 7274 6564  .# List suported
-000004b0: 2041 7474 6163 6b73 0a62 6174 2061 7474   Attacks.bat att
-000004c0: 6163 6b20 6c69 7374 0a0a 2320 5465 7374  ack list..# Test
-000004d0: 2043 6c6f 7564 2041 5049 730a 6261 7420   Cloud APIs.bat 
-000004e0: 6170 6920 7275 6e20 6465 6570 6170 690a  api run deepapi.
-000004f0: 6261 7420 6170 6920 7275 6e20 676f 6f67  bat api run goog
-00000500: 6c65 0a62 6174 2061 7069 2072 756e 2069  le.bat api run i
-00000510: 6d61 6767 610a 0a23 2052 756e 2065 786d  magga..# Run exm
-00000520: 6170 6c65 730a 6261 7420 6578 616d 706c  aples.bat exampl
-00000530: 6520 7275 6e20 7369 6d62 615f 6465 6570  e run simba_deep
-00000540: 6170 690a 6261 7420 6578 616d 706c 6520  api.bat example 
-00000550: 7275 6e20 6261 6e64 6974 735f 6465 6570  run bandits_deep
-00000560: 6170 690a 6261 7420 6578 616d 706c 6520  api.bat example 
-00000570: 7275 6e20 7371 7561 7265 5f64 6565 7061  run square_deepa
-00000580: 7069 0a60 6060 0a0a 2323 2055 7361 6765  pi.```..## Usage
-00000590: 2028 5079 7468 6f6e 290a 0a60 6060 7079   (Python)..```py
-000005a0: 7468 6f6e 0a69 6d70 6f72 7420 6e75 6d70  thon.import nump
-000005b0: 7920 6173 206e 700a 6672 6f6d 2050 494c  y as np.from PIL
-000005c0: 2069 6d70 6f72 7420 496d 6167 650a 0a66   import Image..f
-000005d0: 726f 6d20 6261 742e 6174 7461 636b 7320  rom bat.attacks 
-000005e0: 696d 706f 7274 2053 696d 4241 0a66 726f  import SimBA.fro
-000005f0: 6d20 6261 742e 6170 6973 2e64 6565 7061  m bat.apis.deepa
-00000600: 7069 2069 6d70 6f72 7420 4465 6570 4150  pi import DeepAP
-00000610: 495f 5647 4731 365f 4369 6661 7231 300a  I_VGG16_Cifar10.
-00000620: 0a23 204c 6f61 6420 496d 6167 650a 7820  .# Load Image.x 
-00000630: 3d20 6e70 2e61 7361 7272 6179 2849 6d61  = np.asarray(Ima
-00000640: 6765 2e6f 7065 6e28 2264 6f67 2e6a 7067  ge.open("dog.jpg
-00000650: 2229 2e63 6f6e 7665 7274 2827 5247 4227  ").convert('RGB'
-00000660: 2929 0a78 203d 206e 702e 6172 7261 7928  )).x = np.array(
-00000670: 5b78 5d29 0a0a 2320 496e 6974 6961 6c69  [x])..# Initiali
-00000680: 7a65 2074 6865 2043 6c6f 7564 2041 5049  ze the Cloud API
-00000690: 204d 6f64 656c 0a44 4545 505f 4150 495f   Model.DEEP_API_
-000006a0: 5552 4c20 3d20 2768 7474 703a 2f2f 6c6f  URL = 'http://lo
-000006b0: 6361 6c68 6f73 743a 3830 3830 270a 6d6f  calhost:8080'.mo
-000006c0: 6465 6c20 3d20 4465 6570 4150 495f 5647  del = DeepAPI_VG
-000006d0: 4731 365f 4369 6661 7231 3028 4445 4550  G16_Cifar10(DEEP
-000006e0: 5f41 5049 5f55 524c 290a 0a23 2047 6574  _API_URL)..# Get
-000006f0: 2050 7265 6469 7463 7469 6f6e 0a79 5f70   Preditction.y_p
-00000700: 7265 6420 3d20 6d6f 6465 6c2e 7072 6564  red = model.pred
-00000710: 6963 7428 7829 5b30 5d0a 0a23 2044 6973  ict(x)[0]..# Dis
-00000720: 7472 6962 7574 6564 2053 696d 4241 2041  tributed SimBA A
-00000730: 7474 6163 6b0a 7369 6d62 6120 3d20 5369  ttack.simba = Si
-00000740: 6d42 4128 6d6f 6465 6c29 0a78 5f61 6476  mBA(model).x_adv
-00000750: 203d 2073 696d 6261 2e61 7474 6163 6b28   = simba.attack(
-00000760: 782c 206e 702e 6172 676d 6178 2879 5f70  x, np.argmax(y_p
-00000770: 7265 6429 2c20 6570 7369 6c6f 6e3d 302e  red), epsilon=0.
-00000780: 3035 2c20 6d61 785f 6974 3d31 3029 0a60  05, max_it=10).`
-00000790: 6060 0a0a 3c68 333e 203c 6120 6872 6566  ``..<h3> <a href
-000007a0: 3d22 6874 7470 733a 2f2f 6261 742e 7775  ="https://bat.wu
-000007b0: 6861 6e73 7475 6469 6f2e 756b 2f22 3e20  hanstudio.uk/"> 
-000007c0: 446f 6375 6d65 6e74 6174 696f 6e20 3c2f  Documentation </
-000007d0: 613e 0a                                  a>.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 626c 6163  : 2.1.Name: blac
+00000020: 6b62 6f78 2d61 6476 6572 7361 7269 616c  kbox-adversarial
+00000030: 2d74 6f6f 6c62 6f78 0a56 6572 7369 6f6e  -toolbox.Version
+00000040: 3a20 302e 312e 310a 5375 6d6d 6172 793a  : 0.1.1.Summary:
+00000050: 2042 6c61 636b 2d62 6f78 2041 6476 6572   Black-box Adver
+00000060: 7361 7269 616c 2054 6f6f 6c62 6f78 2028  sarial Toolbox (
+00000070: 4241 5429 202d 2050 7974 686f 6e20 4c69  BAT) - Python Li
+00000080: 6272 6172 7920 666f 7220 4465 6570 204c  brary for Deep L
+00000090: 6561 726e 696e 6720 5365 6375 7269 7479  earning Security
+000000a0: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
+000000b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f77  s://github.com/w
+000000c0: 7568 616e 7374 7564 696f 2f62 6c61 636b  uhanstudio/black
+000000d0: 626f 782d 6164 7665 7273 6172 6961 6c2d  box-adversarial-
+000000e0: 746f 6f6c 626f 780a 4175 7468 6f72 3a20  toolbox.Author: 
+000000f0: 7775 6861 6e73 7475 6469 6f0a 4175 7468  wuhanstudio.Auth
+00000100: 6f72 2d65 6d61 696c 3a20 7775 6861 6e73  or-email: wuhans
+00000110: 7475 6469 6f20 3c77 7568 616e 7374 7564  tudio <wuhanstud
+00000120: 696f 7340 676d 6169 6c2e 636f 6d3e 0a4d  ios@gmail.com>.M
+00000130: 6169 6e74 6169 6e65 723a 2077 7568 616e  aintainer: wuhan
+00000140: 7374 7564 696f 0a4d 6169 6e74 6169 6e65  studio.Maintaine
+00000150: 722d 656d 6169 6c3a 2077 7568 616e 7374  r-email: wuhanst
+00000160: 7564 696f 203c 7775 6861 6e73 7475 6469  udio <wuhanstudi
+00000170: 6f73 4067 6d61 696c 2e63 6f6d 3e0a 4c69  os@gmail.com>.Li
+00000180: 6365 6e73 653a 204d 4954 204c 6963 656e  cense: MIT Licen
+00000190: 7365 0a50 726f 6a65 6374 2d55 524c 3a20  se.Project-URL: 
+000001a0: 486f 6d65 7061 6765 2c20 6874 7470 733a  Homepage, https:
+000001b0: 2f2f 6769 7468 7562 2e63 6f6d 2f77 7568  //github.com/wuh
+000001c0: 616e 7374 7564 696f 2f62 6c61 636b 626f  anstudio/blackbo
+000001d0: 782d 6164 7665 7273 6172 6961 6c2d 746f  x-adversarial-to
+000001e0: 6f6c 626f 780a 5072 6f6a 6563 742d 5552  olbox.Project-UR
+000001f0: 4c3a 2042 7567 2054 7261 636b 6572 2c20  L: Bug Tracker, 
+00000200: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000210: 6f6d 2f77 7568 616e 7374 7564 696f 2f62  om/wuhanstudio/b
+00000220: 6c61 636b 626f 782d 6164 7665 7273 6172  lackbox-adversar
+00000230: 6961 6c2d 746f 6f6c 626f 782f 6973 7375  ial-toolbox/issu
+00000240: 6573 0a43 6c61 7373 6966 6965 723a 2049  es.Classifier: I
+00000250: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+00000260: 203a 3a20 5363 6965 6e63 652f 5265 7365   :: Science/Rese
+00000270: 6172 6368 0a43 6c61 7373 6966 6965 723a  arch.Classifier:
+00000280: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
+00000290: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+000002a0: 4c69 6365 6e73 650a 436c 6173 7369 6669  License.Classifi
+000002b0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000002c0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002d0: 6f6e 203a 3a20 332e 360a 436c 6173 7369  on :: 3.6.Classi
+000002e0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000002f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000300: 7468 6f6e 203a 3a20 332e 370a 436c 6173  thon :: 3.7.Clas
+00000310: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000320: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000330: 5079 7468 6f6e 203a 3a20 332e 380a 436c  Python :: 3.8.Cl
+00000340: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000350: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000360: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
+00000370: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+00000380: 6320 3a3a 2053 6369 656e 7469 6669 632f  c :: Scientific/
+00000390: 456e 6769 6e65 6572 696e 6720 3a3a 2041  Engineering :: A
+000003a0: 7274 6966 6963 6961 6c20 496e 7465 6c6c  rtificial Intell
+000003b0: 6967 656e 6365 0a52 6571 7569 7265 732d  igence.Requires-
+000003c0: 5079 7468 6f6e 3a20 3e3d 332e 360a 4465  Python: >=3.6.De
+000003d0: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
+000003e0: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
+000003f0: 6b64 6f77 6e0a 4c69 6365 6e73 652d 4669  kdown.License-Fi
+00000400: 6c65 3a20 4c49 4345 4e53 450a 0a3c 696d  le: LICENSE..<im
+00000410: 6720 7372 633d 2268 7474 7073 3a2f 2f62  g src="https://b
+00000420: 6174 2e77 7568 616e 7374 7564 696f 2e75  at.wuhanstudio.u
+00000430: 6b2f 696d 6167 6573 2f62 6174 2e70 6e67  k/images/bat.png
+00000440: 2220 7769 6474 683d 3330 3070 7820 7374  " width=300px st
+00000450: 796c 653d 2266 6c6f 6174 3a20 6c65 6674  yle="float: left
+00000460: 3b22 203e 0a0a 2320 426c 6163 6b2d 626f  ;" >..# Black-bo
+00000470: 7820 4164 7665 7273 6172 6961 6c20 546f  x Adversarial To
+00000480: 6f6c 626f 7820 2842 4154 290a 0a5b 215b  olbox (BAT)..[![
+00000490: 4275 696c 6420 5374 6174 7573 5d28 6874  Build Status](ht
+000004a0: 7470 733a 2f2f 6170 702e 7472 6176 6973  tps://app.travis
+000004b0: 2d63 692e 636f 6d2f 7775 6861 6e73 7475  -ci.com/wuhanstu
+000004c0: 6469 6f2f 626c 6163 6b62 6f78 2d61 6476  dio/blackbox-adv
+000004d0: 6572 7361 7269 616c 2d74 6f6f 6c62 6f78  ersarial-toolbox
+000004e0: 2e73 7667 3f62 7261 6e63 683d 6d61 7374  .svg?branch=mast
+000004f0: 6572 295d 2868 7474 7073 3a2f 2f61 7070  er)](https://app
+00000500: 2e74 7261 7669 732d 6369 2e63 6f6d 2f77  .travis-ci.com/w
+00000510: 7568 616e 7374 7564 696f 2f62 6c61 636b  uhanstudio/black
+00000520: 626f 782d 6164 7665 7273 6172 6961 6c2d  box-adversarial-
+00000530: 746f 6f6c 626f 7829 0a5b 215b 5079 5049  toolbox).[![PyPI
+00000540: 2076 6572 7369 6f6e 5d28 6874 7470 733a   version](https:
+00000550: 2f2f 6261 6467 652e 6675 7279 2e69 6f2f  //badge.fury.io/
+00000560: 7079 2f62 6c61 636b 626f 782d 6164 7665  py/blackbox-adve
+00000570: 7273 6172 6961 6c2d 746f 6f6c 626f 782e  rsarial-toolbox.
+00000580: 7376 6729 5d28 6874 7470 733a 2f2f 6261  svg)](https://ba
+00000590: 6467 652e 6675 7279 2e69 6f2f 7079 2f62  dge.fury.io/py/b
+000005a0: 6c61 636b 626f 782d 6164 7665 7273 6172  lackbox-adversar
+000005b0: 6961 6c2d 746f 6f6c 626f 7829 0a5b 215b  ial-toolbox).[![
+000005c0: 4c69 6365 6e73 653a 204d 4954 5d28 6874  License: MIT](ht
+000005d0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000005e0: 732e 696f 2f62 6164 6765 2f4c 6963 656e  s.io/badge/Licen
+000005f0: 7365 2d4d 4954 2d79 656c 6c6f 772e 7376  se-MIT-yellow.sv
+00000600: 6729 5d28 6874 7470 733a 2f2f 6f70 656e  g)](https://open
+00000610: 736f 7572 6365 2e6f 7267 2f6c 6963 656e  source.org/licen
+00000620: 7365 732f 4d49 5429 0a5b 215b 5079 5049  ses/MIT).[![PyPI
+00000630: 202d 2050 7974 686f 6e20 5665 7273 696f   - Python Versio
+00000640: 6e5d 2868 7474 7073 3a2f 2f69 6d67 2e73  n](https://img.s
+00000650: 6869 656c 6473 2e69 6f2f 7079 7069 2f70  hields.io/pypi/p
+00000660: 7976 6572 7369 6f6e 732f 626c 6163 6b62  yversions/blackb
+00000670: 6f78 2d61 6476 6572 7361 7269 616c 2d74  ox-adversarial-t
+00000680: 6f6f 6c62 6f78 295d 2868 7474 7073 3a2f  oolbox)](https:/
+00000690: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+000006a0: 742f 626c 6163 6b62 6f78 2d61 6476 6572  t/blackbox-adver
+000006b0: 7361 7269 616c 2d74 6f6f 6c62 6f78 2f29  sarial-toolbox/)
+000006c0: 0a5b 215b 5d28 6874 7470 733a 2f2f 696d  .[![](https://im
+000006d0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+000006e0: 6765 2f44 6f63 756d 656e 7461 7469 6f6e  ge/Documentation
+000006f0: 2d69 6e66 726f 6d61 7469 6f6e 616c 295d  -infromational)]
+00000700: 2868 7474 7073 3a2f 2f62 6174 2e77 7568  (https://bat.wuh
+00000710: 616e 7374 7564 696f 2e75 6b2f 290a 0a41  anstudio.uk/)..A
+00000720: 2050 7974 686f 6e20 4c69 6272 6172 7920   Python Library 
+00000730: 666f 7220 4465 6570 204c 6561 726e 696e  for Deep Learnin
+00000740: 6720 5365 6375 7269 7479 2074 6861 7420  g Security that 
+00000750: 666f 6375 7365 7320 6f6e 2044 6973 7472  focuses on Distr
+00000760: 6962 7574 6564 2042 6c61 636b 2d62 6f78  ibuted Black-box
+00000770: 2061 7474 6163 6b73 2e0a 0a23 2320 496e   attacks...## In
+00000780: 7374 616c 6c61 7469 6f6e 0a0a 6060 6070  stallation..```p
+00000790: 7974 686f 6e0a 7069 7020 696e 7374 616c  ython.pip instal
+000007a0: 6c20 626c 6163 6b62 6f78 2d61 6476 6572  l blackbox-adver
+000007b0: 7361 7269 616c 2d74 6f6f 6c62 6f78 0a60  sarial-toolbox.`
+000007c0: 6060 0a0a 0a23 2320 5573 6167 6520 2843  ``...## Usage (C
+000007d0: 4c49 290a 0a60 6060 0a55 7361 6765 3a20  LI)..```.Usage: 
+000007e0: 6261 7420 5b4f 5054 494f 4e53 5d20 434f  bat [OPTIONS] CO
+000007f0: 4d4d 414e 4420 5b41 5247 535d 2e2e 2e0a  MMAND [ARGS]....
+00000800: 0a20 2054 6865 2043 4c49 2074 6f6f 6c20  .  The CLI tool 
+00000810: 666f 7220 426c 6163 6b2d 626f 7820 4164  for Black-box Ad
+00000820: 7665 7273 6172 6961 6c20 546f 6f6c 626f  versarial Toolbo
+00000830: 7820 2842 4154 292e 0a0a 4f70 7469 6f6e  x (BAT)...Option
+00000840: 733a 0a20 202d 2d68 656c 7020 2053 686f  s:.  --help  Sho
+00000850: 7720 7468 6973 206d 6573 7361 6765 2061  w this message a
+00000860: 6e64 2065 7869 742e 0a0a 436f 6d6d 616e  nd exit...Comman
+00000870: 6473 3a0a 2020 6170 6920 2020 2020 204d  ds:.  api      M
+00000880: 616e 6167 6520 436c 6f75 6420 4150 4973  anage Cloud APIs
+00000890: 0a20 2061 7474 6163 6b20 2020 4d61 6e61  .  attack   Mana
+000008a0: 6765 2041 7474 6163 6b73 0a20 2065 7861  ge Attacks.  exa
+000008b0: 6d70 6c65 2020 4d61 6e61 6765 2045 7861  mple  Manage Exa
+000008c0: 6d70 6c65 730a 6060 600a 5573 6566 756c  mples.```.Useful
+000008d0: 2063 6f6d 6d61 6e64 733a 0a60 6060 0a23   commands:.```.#
+000008e0: 204c 6973 7420 7375 7070 6f72 7465 6420   List supported 
+000008f0: 436c 6f75 6420 4150 4973 0a24 2062 6174  Cloud APIs.$ bat
+00000900: 2061 7069 206c 6973 740a 0a23 204c 6973   api list..# Lis
+00000910: 7420 7375 7070 6f72 7465 6420 4174 7461  t supported Atta
+00000920: 636b 730a 2420 6261 7420 6174 7461 636b  cks.$ bat attack
+00000930: 206c 6973 740a 0a23 2054 6573 7420 436c   list..# Test Cl
+00000940: 6f75 6420 4150 4973 0a24 2062 6174 2061  oud APIs.$ bat a
+00000950: 7069 2072 756e 2064 6565 7061 7069 0a24  pi run deepapi.$
+00000960: 2062 6174 2061 7069 2072 756e 2067 6f6f   bat api run goo
+00000970: 676c 650a 2420 6261 7420 6170 6920 7275  gle.$ bat api ru
+00000980: 6e20 696d 6167 6761 0a0a 2320 5275 6e20  n imagga..# Run 
+00000990: 6578 6d61 706c 6573 0a24 2062 6174 2065  exmaples.$ bat e
+000009a0: 7861 6d70 6c65 2072 756e 2073 696d 6261  xample run simba
+000009b0: 5f64 6565 7061 7069 0a24 2062 6174 2065  _deepapi.$ bat e
+000009c0: 7861 6d70 6c65 2072 756e 2062 616e 6469  xample run bandi
+000009d0: 7473 5f64 6565 7061 7069 0a24 2062 6174  ts_deepapi.$ bat
+000009e0: 2065 7861 6d70 6c65 2072 756e 2073 7175   example run squ
+000009f0: 6172 655f 6465 6570 6170 690a 6060 600a  are_deepapi.```.
+00000a00: 0a23 2320 5573 6167 6520 2850 7974 686f  .## Usage (Pytho
+00000a10: 6e29 0a0a 6060 6070 7974 686f 6e0a 696d  n)..```python.im
+00000a20: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
+00000a30: 0a66 726f 6d20 5049 4c20 696d 706f 7274  .from PIL import
+00000a40: 2049 6d61 6765 0a0a 6672 6f6d 2062 6174   Image..from bat
+00000a50: 2e61 7474 6163 6b73 2069 6d70 6f72 7420  .attacks import 
+00000a60: 5369 6d42 410a 6672 6f6d 2062 6174 2e61  SimBA.from bat.a
+00000a70: 7069 732e 6465 6570 6170 6920 696d 706f  pis.deepapi impo
+00000a80: 7274 2044 6565 7041 5049 5f56 4747 3136  rt DeepAPI_VGG16
+00000a90: 5f43 6966 6172 3130 0a0a 2320 4c6f 6164  _Cifar10..# Load
+00000aa0: 2049 6d61 6765 0a78 203d 206e 702e 6173   Image.x = np.as
+00000ab0: 6172 7261 7928 496d 6167 652e 6f70 656e  array(Image.open
+00000ac0: 2822 646f 672e 6a70 6722 292e 636f 6e76  ("dog.jpg").conv
+00000ad0: 6572 7428 2752 4742 2729 290a 7820 3d20  ert('RGB')).x = 
+00000ae0: 6e70 2e61 7272 6179 285b 785d 290a 0a23  np.array([x])..#
+00000af0: 2049 6e69 7469 616c 697a 6520 7468 6520   Initialize the 
+00000b00: 436c 6f75 6420 4150 4920 4d6f 6465 6c0a  Cloud API Model.
+00000b10: 4445 4550 5f41 5049 5f55 524c 203d 2027  DEEP_API_URL = '
+00000b20: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
+00000b30: 3a38 3038 3027 0a6d 6f64 656c 203d 2044  :8080'.model = D
+00000b40: 6565 7041 5049 5f56 4747 3136 5f43 6966  eepAPI_VGG16_Cif
+00000b50: 6172 3130 2844 4545 505f 4150 495f 5552  ar10(DEEP_API_UR
+00000b60: 4c29 0a0a 2320 4765 7420 5072 6564 6974  L)..# Get Predit
+00000b70: 6374 696f 6e0a 795f 7072 6564 203d 206d  ction.y_pred = m
+00000b80: 6f64 656c 2e70 7265 6469 6374 2878 295b  odel.predict(x)[
+00000b90: 305d 0a0a 2320 4469 7374 7269 6275 7465  0]..# Distribute
+00000ba0: 6420 5369 6d42 4120 4174 7461 636b 0a73  d SimBA Attack.s
+00000bb0: 696d 6261 203d 2053 696d 4241 286d 6f64  imba = SimBA(mod
+00000bc0: 656c 290a 785f 6164 7620 3d20 7369 6d62  el).x_adv = simb
+00000bd0: 612e 6174 7461 636b 2878 2c20 6e70 2e61  a.attack(x, np.a
+00000be0: 7267 6d61 7828 795f 7072 6564 292c 2065  rgmax(y_pred), e
+00000bf0: 7073 696c 6f6e 3d30 2e30 352c 206d 6178  psilon=0.05, max
+00000c00: 5f69 743d 3130 290a 6060 600a            _it=10).```.
```

### Comparing `blackbox-adversarial-toolbox-0.1.0/bat/__init__.py` & `blackbox-adversarial-toolbox-0.1.1/bat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 '''
 
 # Project Imports
 from bat import apis
 from bat import attacks
 
 # Semantic Version
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

### Comparing `blackbox-adversarial-toolbox-0.1.0/bat/_main.py` & `blackbox-adversarial-toolbox-0.1.1/bat/_main.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/bat/apis/__init__.py` & `blackbox-adversarial-toolbox-0.1.1/bat/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/bat/apis/deepapi.py` & `blackbox-adversarial-toolbox-0.1.1/bat/apis/deepapi.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/bat/apis/google.py` & `blackbox-adversarial-toolbox-0.1.1/bat/apis/google.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/bat/apis/imagga.py` & `blackbox-adversarial-toolbox-0.1.1/bat/apis/imagga.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/bat/attacks/__init__.py` & `blackbox-adversarial-toolbox-0.1.1/bat/attacks/__init__.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/bat/attacks/bandits_attack.py` & `blackbox-adversarial-toolbox-0.1.1/bat/attacks/bandits_attack.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/bat/attacks/simba_attack.py` & `blackbox-adversarial-toolbox-0.1.1/bat/attacks/simba_attack.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/bat/attacks/square_attack.py` & `blackbox-adversarial-toolbox-0.1.1/bat/attacks/square_attack.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/blackbox_adversarial_toolbox.egg-info/SOURCES.txt` & `blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/bat/_main.html` & `blackbox-adversarial-toolbox-0.1.1/docs/bat/_main.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/bat/apis/deepapi.html` & `blackbox-adversarial-toolbox-0.1.1/docs/bat/apis/deepapi.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/bat/apis/google.html` & `blackbox-adversarial-toolbox-0.1.1/docs/bat/apis/google.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/bat/apis/imagga.html` & `blackbox-adversarial-toolbox-0.1.1/docs/bat/apis/imagga.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/bat/apis.html` & `blackbox-adversarial-toolbox-0.1.1/docs/bat/apis.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/bat/attacks/bandits_attack.html` & `blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/bandits_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/bat/attacks/base_attack.html` & `blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/base_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/bat/attacks/simba_attack.html` & `blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/simba_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/bat/attacks/square_attack.html` & `blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/square_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/bat/attacks.html` & `blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/bat/utils/proj_lp.html` & `blackbox-adversarial-toolbox-0.1.1/docs/bat/utils/proj_lp.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/bat/utils.html` & `blackbox-adversarial-toolbox-0.1.1/docs/bat/utils.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/bat.html` & `blackbox-adversarial-toolbox-0.1.1/docs/bat.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/images/bat.png` & `blackbox-adversarial-toolbox-0.1.1/docs/images/bat.png`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/images/bat_dark.png` & `blackbox-adversarial-toolbox-0.1.1/docs/images/bat_dark.png`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/search.js` & `blackbox-adversarial-toolbox-0.1.1/docs/search.js`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/apis/deepapi/vgg16_cifar10.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis/deepapi/vgg16_cifar10.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/apis/deepapi.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis/deepapi.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/apis.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/attacks/simba.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/attacks/simba.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/attacks.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/attacks.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/utils/proj_lp.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/utils/proj_lp.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat/utils.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/utils.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/bat.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/index.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/index.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.0.8/search.js` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/search.js`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/_main.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/_main.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/apis/deepapi.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis/deepapi.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/apis/google.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis/google.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/apis/imagga.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis/imagga.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/apis.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/attacks/bandits_attack.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/bandits_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/attacks/base_attack.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/base_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/attacks/simba_attack.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/simba_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/attacks/square_attack.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/square_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/attacks.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/utils/proj_lp.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/utils/proj_lp.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat/utils.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/utils.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/bat.html` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/docs/v0.1.0/search.js` & `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/search.js`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/pyproject.toml` & `blackbox-adversarial-toolbox-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,29 +12,33 @@
     "google-cloud-vision",
     "validators"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "blackbox-adversarial-toolbox"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="wuhanstudio", email="wuhanstudios@gmail.com" },
 ]
 maintainers = [
   { name="wuhanstudio", email="wuhanstudios@gmail.com" },
 ]
 description = "Black-box Adversarial Toolbox (BAT) - Python Library for Deep Learning Security"
 readme = "README.md"
 license = {text = "MIT License"}
 requires-python = ">=3.6"
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "numpy>=1.18.0",
     "scipy>=1.4.1",
     "scikit-learn>=0.22.2",
     "pillow",
     "requests",
```

### Comparing `blackbox-adversarial-toolbox-0.1.0/setup.py` & `blackbox-adversarial-toolbox-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,21 +54,16 @@
             'bat=bat._main:main',
         ],
     },
     packages=setuptools.find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Topic :: Software Development :: Libraries",
-        "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
 )
```

### Comparing `blackbox-adversarial-toolbox-0.1.0/tests/__pycache__/test_deepapi.cpython-38-pytest-7.3.1.pyc` & `blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_deepapi.cpython-38-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/tests/__pycache__/test_deepapi.cpython-38.pyc` & `blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_deepapi.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/tests/__pycache__/test_simba.cpython-38-pytest-7.3.1.pyc` & `blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_simba.cpython-38-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/tests/__pycache__/test_simba.cpython-38.pyc` & `blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_simba.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/tests/__pycache__/test_square.cpython-38-pytest-7.3.1.pyc` & `blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_square.cpython-38-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/tests/cat.jpg` & `blackbox-adversarial-toolbox-0.1.1/tests/cat.jpg`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/tests/dog.jpg` & `blackbox-adversarial-toolbox-0.1.1/tests/dog.jpg`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/tests/test_deepapi.py` & `blackbox-adversarial-toolbox-0.1.1/tests/test_deepapi.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/tests/test_simba.py` & `blackbox-adversarial-toolbox-0.1.1/tests/test_simba.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.0/tests/test_square.py` & `blackbox-adversarial-toolbox-0.1.1/tests/test_square.py`

 * *Files identical despite different names*

