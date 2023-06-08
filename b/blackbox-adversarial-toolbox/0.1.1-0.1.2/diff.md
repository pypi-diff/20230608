# Comparing `tmp/blackbox-adversarial-toolbox-0.1.1.tar.gz` & `tmp/blackbox-adversarial-toolbox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/wuhanstudio/Desktop/blackbox-adversarial-toolbox/dist/.tmp-s5iensif/blackbox-adversarial-toolbox-0.1.1.tar", last modified: Thu Jun  8 15:18:07 2023, max compression
+gzip compressed data, was "/home/wuhanstudio/Desktop/blackbox-adversarial-toolbox/dist/.tmp-1u0hkmic/blackbox-adversarial-toolbox-0.1.2.tar", last modified: Thu Jun  8 15:24:12 2023, max compression
```

## Comparing `blackbox-adversarial-toolbox-0.1.1.tar` & `blackbox-adversarial-toolbox-0.1.2.tar`

### file list

```diff
@@ -1,106 +1,111 @@
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.292251 blackbox-adversarial-toolbox-0.1.1/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1063 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.1/LICENSE
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       66 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.1/MANIFEST.in
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3084 2023-06-08 15:18:07.292251 blackbox-adversarial-toolbox-0.1.1/PKG-INFO
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2047 2023-06-08 15:17:10.000000 blackbox-adversarial-toolbox-0.1.1/README.md
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.084251 blackbox-adversarial-toolbox-0.1.1/bat/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      664 2023-06-08 15:17:28.000000 blackbox-adversarial-toolbox-0.1.1/bat/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       32 2023-05-29 16:18:42.000000 blackbox-adversarial-toolbox-0.1.1/bat/__main__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6142 2023-05-31 19:12:14.000000 blackbox-adversarial-toolbox-0.1.1/bat/_main.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.084251 blackbox-adversarial-toolbox-0.1.1/bat/apis/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1423 2023-05-31 19:52:33.000000 blackbox-adversarial-toolbox-0.1.1/bat/apis/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7399 2023-05-30 15:37:52.000000 blackbox-adversarial-toolbox-0.1.1/bat/apis/deepapi.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1762 2023-05-30 13:00:18.000000 blackbox-adversarial-toolbox-0.1.1/bat/apis/google.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1740 2023-05-30 10:10:16.000000 blackbox-adversarial-toolbox-0.1.1/bat/apis/imagga.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.084251 blackbox-adversarial-toolbox-0.1.1/bat/attacks/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      647 2023-05-31 19:58:51.000000 blackbox-adversarial-toolbox-0.1.1/bat/attacks/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     9770 2023-05-31 15:05:16.000000 blackbox-adversarial-toolbox-0.1.1/bat/attacks/bandits_attack.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      456 2023-05-30 13:18:48.000000 blackbox-adversarial-toolbox-0.1.1/bat/attacks/base_attack.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7697 2023-05-31 15:02:36.000000 blackbox-adversarial-toolbox-0.1.1/bat/attacks/simba_attack.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    11962 2023-05-31 14:32:21.000000 blackbox-adversarial-toolbox-0.1.1/bat/attacks/square_attack.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.084251 blackbox-adversarial-toolbox-0.1.1/bat/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      101 2023-05-31 19:20:30.000000 blackbox-adversarial-toolbox-0.1.1/bat/utils/__init__.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      417 2023-05-31 19:21:21.000000 blackbox-adversarial-toolbox-0.1.1/bat/utils/proj_lp.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.084251 blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3084 2023-06-08 15:18:07.000000 blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/PKG-INFO
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2254 2023-06-08 15:18:07.000000 blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        1 2023-06-08 15:18:07.000000 blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       39 2023-06-08 15:18:07.000000 blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/entry_points.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      121 2023-06-08 15:18:07.000000 blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/requires.txt
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        4 2023-06-08 15:18:07.000000 blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/top_level.txt
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.104251 blackbox-adversarial-toolbox-0.1.1/docs/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       65 2023-05-31 19:45:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/.gitignore
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       18 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.1/docs/CNAME
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.116251 blackbox-adversarial-toolbox-0.1.1/docs/bat/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    89180 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/_main.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.128251 blackbox-adversarial-toolbox-0.1.1/docs/bat/apis/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   215108 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/apis/deepapi.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    79194 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/apis/google.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    78801 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/apis/imagga.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    47991 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/apis.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.136251 blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   241850 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/bandits_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    51220 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/base_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   207128 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/simba_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   320760 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/square_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    39236 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.144251 blackbox-adversarial-toolbox-0.1.1/docs/bat/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    43263 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/utils/proj_lp.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    36169 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat/utils.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    39713 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.1/docs/bat.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.144251 blackbox-adversarial-toolbox-0.1.1/docs/images/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    20406 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.1/docs/images/bat.png
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    78710 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.1/docs/images/bat_dark.png
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      134 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/index.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    58126 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.1/docs/search.js
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.160251 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.180251 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.180251 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.180251 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis/deepapi/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    64415 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis/deepapi/vgg16_cifar10.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    33716 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis/deepapi.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    35555 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.184251 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/attacks/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   100303 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/attacks/simba.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    33350 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/attacks.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.192251 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    37997 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/utils/proj_lp.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    33067 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/utils.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    34852 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    32039 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/index.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    26612 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/search.js
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.220251 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.248252 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    89180 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/_main.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.264252 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   215108 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis/deepapi.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    79194 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis/google.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    78801 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis/imagga.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    46920 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.272251 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   241850 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/bandits_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    51220 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/base_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   207128 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/simba_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   320760 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/square_attack.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    38456 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks.html
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.272251 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/utils/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    43263 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/utils/proj_lp.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    36169 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/utils.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    40297 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      134 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/index.html
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    57902 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/search.js
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1447 2023-06-08 15:17:16.000000 blackbox-adversarial-toolbox-0.1.1/pyproject.toml
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       38 2023-06-08 15:18:07.292251 blackbox-adversarial-toolbox-0.1.1/setup.cfg
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1996 2023-06-08 15:17:10.000000 blackbox-adversarial-toolbox-0.1.1/setup.py
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.276251 blackbox-adversarial-toolbox-0.1.1/tests/
-drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:18:07.284252 blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2334 2023-05-30 13:40:51.000000 blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_deepapi.cpython-38-pytest-7.3.1.pyc
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1329 2023-05-30 13:32:48.000000 blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_deepapi.cpython-38.pyc
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2582 2023-05-30 13:40:51.000000 blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_simba.cpython-38-pytest-7.3.1.pyc
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1581 2023-05-30 13:38:49.000000 blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_simba.cpython-38.pyc
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2971 2023-05-31 14:56:46.000000 blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_square.cpython-38-pytest-7.3.1.pyc
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    57480 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.1/tests/cat.jpg
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    19151 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.1/tests/dog.jpg
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1263 2023-05-30 13:32:43.000000 blackbox-adversarial-toolbox-0.1.1/tests/test_deepapi.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1835 2023-05-30 13:38:48.000000 blackbox-adversarial-toolbox-0.1.1/tests/test_simba.py
--rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2309 2023-05-31 14:56:43.000000 blackbox-adversarial-toolbox-0.1.1/tests/test_square.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.796849 blackbox-adversarial-toolbox-0.1.2/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1063 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.2/LICENSE
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       66 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.2/MANIFEST.in
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3084 2023-06-08 15:24:12.796849 blackbox-adversarial-toolbox-0.1.2/PKG-INFO
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2047 2023-06-08 15:17:10.000000 blackbox-adversarial-toolbox-0.1.2/README.md
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.788849 blackbox-adversarial-toolbox-0.1.2/bat/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      711 2023-06-08 15:23:17.000000 blackbox-adversarial-toolbox-0.1.2/bat/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       32 2023-05-29 16:18:42.000000 blackbox-adversarial-toolbox-0.1.2/bat/__main__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     6142 2023-05-31 19:12:14.000000 blackbox-adversarial-toolbox-0.1.2/bat/_main.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.788849 blackbox-adversarial-toolbox-0.1.2/bat/apis/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1423 2023-05-31 19:52:33.000000 blackbox-adversarial-toolbox-0.1.2/bat/apis/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7399 2023-05-30 15:37:52.000000 blackbox-adversarial-toolbox-0.1.2/bat/apis/deepapi.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1762 2023-05-30 13:00:18.000000 blackbox-adversarial-toolbox-0.1.2/bat/apis/google.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1740 2023-05-30 10:10:16.000000 blackbox-adversarial-toolbox-0.1.2/bat/apis/imagga.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.788849 blackbox-adversarial-toolbox-0.1.2/bat/attacks/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      647 2023-05-31 19:58:51.000000 blackbox-adversarial-toolbox-0.1.2/bat/attacks/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     9770 2023-05-31 15:05:16.000000 blackbox-adversarial-toolbox-0.1.2/bat/attacks/bandits_attack.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      456 2023-05-30 13:18:48.000000 blackbox-adversarial-toolbox-0.1.2/bat/attacks/base_attack.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7697 2023-05-31 15:02:36.000000 blackbox-adversarial-toolbox-0.1.2/bat/attacks/simba_attack.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    11962 2023-05-31 14:32:21.000000 blackbox-adversarial-toolbox-0.1.2/bat/attacks/square_attack.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.788849 blackbox-adversarial-toolbox-0.1.2/bat/examples/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      256 2023-06-08 15:22:52.000000 blackbox-adversarial-toolbox-0.1.2/bat/examples/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2399 2023-05-30 20:53:50.000000 blackbox-adversarial-toolbox-0.1.2/bat/examples/bandits_attack_deepapi.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2484 2023-05-30 20:53:43.000000 blackbox-adversarial-toolbox-0.1.2/bat/examples/simba_attack_deepapi.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2493 2023-05-31 19:17:39.000000 blackbox-adversarial-toolbox-0.1.2/bat/examples/square_attack_deepapi.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.788849 blackbox-adversarial-toolbox-0.1.2/bat/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      101 2023-05-31 19:20:30.000000 blackbox-adversarial-toolbox-0.1.2/bat/utils/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      417 2023-05-31 19:21:21.000000 blackbox-adversarial-toolbox-0.1.2/bat/utils/proj_lp.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.792849 blackbox-adversarial-toolbox-0.1.2/blackbox_adversarial_toolbox.egg-info/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3084 2023-06-08 15:24:12.000000 blackbox-adversarial-toolbox-0.1.2/blackbox_adversarial_toolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2393 2023-06-08 15:24:12.000000 blackbox-adversarial-toolbox-0.1.2/blackbox_adversarial_toolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        1 2023-06-08 15:24:12.000000 blackbox-adversarial-toolbox-0.1.2/blackbox_adversarial_toolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       39 2023-06-08 15:24:12.000000 blackbox-adversarial-toolbox-0.1.2/blackbox_adversarial_toolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      121 2023-06-08 15:24:12.000000 blackbox-adversarial-toolbox-0.1.2/blackbox_adversarial_toolbox.egg-info/requires.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        4 2023-06-08 15:24:12.000000 blackbox-adversarial-toolbox-0.1.2/blackbox_adversarial_toolbox.egg-info/top_level.txt
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.792849 blackbox-adversarial-toolbox-0.1.2/docs/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       65 2023-05-31 19:45:15.000000 blackbox-adversarial-toolbox-0.1.2/docs/.gitignore
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       18 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.2/docs/CNAME
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.792849 blackbox-adversarial-toolbox-0.1.2/docs/bat/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    89180 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.2/docs/bat/_main.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.792849 blackbox-adversarial-toolbox-0.1.2/docs/bat/apis/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   215108 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.2/docs/bat/apis/deepapi.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    79194 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.2/docs/bat/apis/google.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    78801 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.2/docs/bat/apis/imagga.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    47991 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.2/docs/bat/apis.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.792849 blackbox-adversarial-toolbox-0.1.2/docs/bat/attacks/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   241850 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.2/docs/bat/attacks/bandits_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    51220 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.2/docs/bat/attacks/base_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   207128 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.2/docs/bat/attacks/simba_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   320760 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.2/docs/bat/attacks/square_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    39236 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.2/docs/bat/attacks.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.792849 blackbox-adversarial-toolbox-0.1.2/docs/bat/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    43263 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.2/docs/bat/utils/proj_lp.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    36169 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.2/docs/bat/utils.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    39713 2023-05-31 19:58:52.000000 blackbox-adversarial-toolbox-0.1.2/docs/bat.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.792849 blackbox-adversarial-toolbox-0.1.2/docs/images/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    20406 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.2/docs/images/bat.png
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    78710 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.2/docs/images/bat_dark.png
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      134 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.2/docs/index.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    58126 2023-05-31 19:58:53.000000 blackbox-adversarial-toolbox-0.1.2/docs/search.js
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.792849 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.792849 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.792849 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/apis/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.792849 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/apis/deepapi/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    64415 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/apis/deepapi/vgg16_cifar10.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    33716 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/apis/deepapi.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    35555 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/apis.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.792849 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/attacks/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   100303 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/attacks/simba.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    33350 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/attacks.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.792849 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    37997 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/utils/proj_lp.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    33067 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/utils.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    34852 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    32039 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/index.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    26612 2023-05-31 18:35:15.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/search.js
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.792849 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.796849 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    89180 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/_main.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.796849 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/apis/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   215108 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/apis/deepapi.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    79194 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/apis/google.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    78801 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/apis/imagga.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    46920 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/apis.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.796849 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/attacks/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   241850 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/attacks/bandits_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    51220 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/attacks/base_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   207128 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/attacks/simba_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)   320760 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/attacks/square_attack.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    38456 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/attacks.html
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.796849 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    43263 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/utils/proj_lp.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    36169 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/utils.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    40297 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      134 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/index.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    57902 2023-05-31 19:21:27.000000 blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/search.js
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1447 2023-06-08 15:23:06.000000 blackbox-adversarial-toolbox-0.1.2/pyproject.toml
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       38 2023-06-08 15:24:12.796849 blackbox-adversarial-toolbox-0.1.2/setup.cfg
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1996 2023-06-08 15:17:10.000000 blackbox-adversarial-toolbox-0.1.2/setup.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.796849 blackbox-adversarial-toolbox-0.1.2/tests/
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-06-08 15:24:12.796849 blackbox-adversarial-toolbox-0.1.2/tests/__pycache__/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2334 2023-05-30 13:40:51.000000 blackbox-adversarial-toolbox-0.1.2/tests/__pycache__/test_deepapi.cpython-38-pytest-7.3.1.pyc
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1329 2023-05-30 13:32:48.000000 blackbox-adversarial-toolbox-0.1.2/tests/__pycache__/test_deepapi.cpython-38.pyc
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2582 2023-05-30 13:40:51.000000 blackbox-adversarial-toolbox-0.1.2/tests/__pycache__/test_simba.cpython-38-pytest-7.3.1.pyc
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1581 2023-05-30 13:38:49.000000 blackbox-adversarial-toolbox-0.1.2/tests/__pycache__/test_simba.cpython-38.pyc
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2971 2023-05-31 14:56:46.000000 blackbox-adversarial-toolbox-0.1.2/tests/__pycache__/test_square.cpython-38-pytest-7.3.1.pyc
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    57480 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.2/tests/cat.jpg
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    19151 2023-05-29 14:04:55.000000 blackbox-adversarial-toolbox-0.1.2/tests/dog.jpg
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1263 2023-05-30 13:32:43.000000 blackbox-adversarial-toolbox-0.1.2/tests/test_deepapi.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1835 2023-05-30 13:38:48.000000 blackbox-adversarial-toolbox-0.1.2/tests/test_simba.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2309 2023-05-31 14:56:43.000000 blackbox-adversarial-toolbox-0.1.2/tests/test_square.py
```

### Comparing `blackbox-adversarial-toolbox-0.1.1/LICENSE` & `blackbox-adversarial-toolbox-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/PKG-INFO` & `blackbox-adversarial-toolbox-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackbox-adversarial-toolbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: Black-box Adversarial Toolbox (BAT) - Python Library for Deep Learning Security
 Home-page: https://github.com/wuhanstudio/blackbox-adversarial-toolbox
 Author: wuhanstudio
 Author-email: wuhanstudio <wuhanstudios@gmail.com>
 Maintainer: wuhanstudio
 Maintainer-email: wuhanstudio <wuhanstudios@gmail.com>
 License: MIT License
```

### Comparing `blackbox-adversarial-toolbox-0.1.1/README.md` & `blackbox-adversarial-toolbox-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/bat/__init__.py` & `blackbox-adversarial-toolbox-0.1.2/bat/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,10 +25,12 @@
 This module implements utility functions.
 
 '''
 
 # Project Imports
 from bat import apis
 from bat import attacks
+from bat import examples
+from bat import utils
 
 # Semantic Version
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

### Comparing `blackbox-adversarial-toolbox-0.1.1/bat/_main.py` & `blackbox-adversarial-toolbox-0.1.2/bat/_main.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/bat/apis/__init__.py` & `blackbox-adversarial-toolbox-0.1.2/bat/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/bat/apis/deepapi.py` & `blackbox-adversarial-toolbox-0.1.2/bat/apis/deepapi.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/bat/apis/google.py` & `blackbox-adversarial-toolbox-0.1.2/bat/apis/google.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/bat/apis/imagga.py` & `blackbox-adversarial-toolbox-0.1.2/bat/apis/imagga.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/bat/attacks/__init__.py` & `blackbox-adversarial-toolbox-0.1.2/bat/attacks/__init__.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/bat/attacks/bandits_attack.py` & `blackbox-adversarial-toolbox-0.1.2/bat/attacks/bandits_attack.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/bat/attacks/simba_attack.py` & `blackbox-adversarial-toolbox-0.1.2/bat/attacks/simba_attack.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/bat/attacks/square_attack.py` & `blackbox-adversarial-toolbox-0.1.2/bat/attacks/square_attack.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/PKG-INFO` & `blackbox-adversarial-toolbox-0.1.2/blackbox_adversarial_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackbox-adversarial-toolbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: Black-box Adversarial Toolbox (BAT) - Python Library for Deep Learning Security
 Home-page: https://github.com/wuhanstudio/blackbox-adversarial-toolbox
 Author: wuhanstudio
 Author-email: wuhanstudio <wuhanstudios@gmail.com>
 Maintainer: wuhanstudio
 Maintainer-email: wuhanstudio <wuhanstudios@gmail.com>
 License: MIT License
```

### Comparing `blackbox-adversarial-toolbox-0.1.1/blackbox_adversarial_toolbox.egg-info/SOURCES.txt` & `blackbox-adversarial-toolbox-0.1.2/blackbox_adversarial_toolbox.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 bat/apis/google.py
 bat/apis/imagga.py
 bat/attacks/__init__.py
 bat/attacks/bandits_attack.py
 bat/attacks/base_attack.py
 bat/attacks/simba_attack.py
 bat/attacks/square_attack.py
+bat/examples/__init__.py
+bat/examples/bandits_attack_deepapi.py
+bat/examples/simba_attack_deepapi.py
+bat/examples/square_attack_deepapi.py
 bat/utils/__init__.py
 bat/utils/proj_lp.py
 blackbox_adversarial_toolbox.egg-info/PKG-INFO
 blackbox_adversarial_toolbox.egg-info/SOURCES.txt
 blackbox_adversarial_toolbox.egg-info/dependency_links.txt
 blackbox_adversarial_toolbox.egg-info/entry_points.txt
 blackbox_adversarial_toolbox.egg-info/requires.txt
```

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/bat/_main.html` & `blackbox-adversarial-toolbox-0.1.2/docs/bat/_main.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/bat/apis/deepapi.html` & `blackbox-adversarial-toolbox-0.1.2/docs/bat/apis/deepapi.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/bat/apis/google.html` & `blackbox-adversarial-toolbox-0.1.2/docs/bat/apis/google.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/bat/apis/imagga.html` & `blackbox-adversarial-toolbox-0.1.2/docs/bat/apis/imagga.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/bat/apis.html` & `blackbox-adversarial-toolbox-0.1.2/docs/bat/apis.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/bandits_attack.html` & `blackbox-adversarial-toolbox-0.1.2/docs/bat/attacks/bandits_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/base_attack.html` & `blackbox-adversarial-toolbox-0.1.2/docs/bat/attacks/base_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/simba_attack.html` & `blackbox-adversarial-toolbox-0.1.2/docs/bat/attacks/simba_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks/square_attack.html` & `blackbox-adversarial-toolbox-0.1.2/docs/bat/attacks/square_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/bat/attacks.html` & `blackbox-adversarial-toolbox-0.1.2/docs/bat/attacks.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/bat/utils/proj_lp.html` & `blackbox-adversarial-toolbox-0.1.2/docs/bat/utils/proj_lp.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/bat/utils.html` & `blackbox-adversarial-toolbox-0.1.2/docs/bat/utils.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/bat.html` & `blackbox-adversarial-toolbox-0.1.2/docs/bat.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/images/bat.png` & `blackbox-adversarial-toolbox-0.1.2/docs/images/bat.png`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/images/bat_dark.png` & `blackbox-adversarial-toolbox-0.1.2/docs/images/bat_dark.png`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/search.js` & `blackbox-adversarial-toolbox-0.1.2/docs/search.js`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis/deepapi/vgg16_cifar10.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/apis/deepapi/vgg16_cifar10.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis/deepapi.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/apis/deepapi.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/apis.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/apis.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/attacks/simba.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/attacks/simba.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/attacks.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/attacks.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/utils/proj_lp.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/utils/proj_lp.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat/utils.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat/utils.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/bat.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/bat.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/index.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/index.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.0.8/search.js` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.0.8/search.js`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/_main.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/_main.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis/deepapi.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/apis/deepapi.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis/google.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/apis/google.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis/imagga.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/apis/imagga.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/apis.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/apis.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/bandits_attack.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/attacks/bandits_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/base_attack.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/attacks/base_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/simba_attack.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/attacks/simba_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks/square_attack.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/attacks/square_attack.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/attacks.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/attacks.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/utils/proj_lp.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/utils/proj_lp.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat/utils.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat/utils.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/bat.html` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/bat.html`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/docs/v0.1.0/search.js` & `blackbox-adversarial-toolbox-0.1.2/docs/v0.1.0/search.js`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/pyproject.toml` & `blackbox-adversarial-toolbox-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "google-cloud-vision",
     "validators"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "blackbox-adversarial-toolbox"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="wuhanstudio", email="wuhanstudios@gmail.com" },
 ]
 maintainers = [
   { name="wuhanstudio", email="wuhanstudios@gmail.com" },
 ]
 description = "Black-box Adversarial Toolbox (BAT) - Python Library for Deep Learning Security"
```

### Comparing `blackbox-adversarial-toolbox-0.1.1/setup.py` & `blackbox-adversarial-toolbox-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_deepapi.cpython-38-pytest-7.3.1.pyc` & `blackbox-adversarial-toolbox-0.1.2/tests/__pycache__/test_deepapi.cpython-38-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_deepapi.cpython-38.pyc` & `blackbox-adversarial-toolbox-0.1.2/tests/__pycache__/test_deepapi.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_simba.cpython-38-pytest-7.3.1.pyc` & `blackbox-adversarial-toolbox-0.1.2/tests/__pycache__/test_simba.cpython-38-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_simba.cpython-38.pyc` & `blackbox-adversarial-toolbox-0.1.2/tests/__pycache__/test_simba.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/tests/__pycache__/test_square.cpython-38-pytest-7.3.1.pyc` & `blackbox-adversarial-toolbox-0.1.2/tests/__pycache__/test_square.cpython-38-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/tests/cat.jpg` & `blackbox-adversarial-toolbox-0.1.2/tests/cat.jpg`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/tests/dog.jpg` & `blackbox-adversarial-toolbox-0.1.2/tests/dog.jpg`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/tests/test_deepapi.py` & `blackbox-adversarial-toolbox-0.1.2/tests/test_deepapi.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/tests/test_simba.py` & `blackbox-adversarial-toolbox-0.1.2/tests/test_simba.py`

 * *Files identical despite different names*

### Comparing `blackbox-adversarial-toolbox-0.1.1/tests/test_square.py` & `blackbox-adversarial-toolbox-0.1.2/tests/test_square.py`

 * *Files identical despite different names*

