# Comparing `tmp/gramex-1.90.0.tar.gz` & `tmp/gramex-1.91.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gramex-1.90.0.tar", last modified: Sun May  7 15:53:06 2023, max compression
+gzip compressed data, was "gramex-1.91.0.tar", last modified: Thu Jun  8 09:28:38 2023, max compression
```

## Comparing `gramex-1.90.0.tar` & `gramex-1.91.0.tar`

### file list

```diff
@@ -1,398 +1,398 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.808865 gramex-1.90.0/
--rw-rw-rw-   0        0        0     1900 2023-04-10 11:33:47.000000 gramex-1.90.0/.gitignore
--rw-rw-rw-   0        0        0     1274 2022-03-03 08:20:08.000000 gramex-1.90.0/LICENSE
--rw-rw-rw-   0        0        0      641 2023-04-11 12:20:36.000000 gramex-1.90.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2956 2023-05-07 15:53:06.808865 gramex-1.90.0/PKG-INFO
--rw-rw-rw-   0        0        0     1212 2022-09-13 04:40:48.000000 gramex-1.90.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.110353 gramex-1.90.0/gramex/
--rw-rw-rw-   0        0        0    15366 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/__init__.py
--rw-rw-rw-   0        0        0      242 2022-07-03 06:28:06.000000 gramex-1.90.0/gramex/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.194902 gramex-1.90.0/gramex/apps/
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:01.000000 gramex-1.90.0/gramex/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.202226 gramex-1.90.0/gramex/apps/admin/
--rw-rw-rw-   0        0        0        9 2019-01-01 03:16:23.000000 gramex-1.90.0/gramex/apps/admin/.gitignore
--rw-rw-rw-   0        0        0      129 2023-01-03 16:10:30.000000 gramex-1.90.0/gramex/apps/admin/gramex.yaml
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.239841 gramex-1.90.0/gramex/apps/admin2/
--rw-rw-rw-   0        0        0      226 2023-04-10 11:33:47.000000 gramex-1.90.0/gramex/apps/admin2/.snyk
--rw-rw-rw-   0        0        0      228 2019-04-01 03:34:34.000000 gramex-1.90.0/gramex/apps/admin2/admin.css
--rw-rw-rw-   0        0        0     3116 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/admin2/gramex.yaml
--rw-rw-rw-   0        0        0    12257 2022-11-23 04:49:14.000000 gramex-1.90.0/gramex/apps/admin2/gramexadmin.py
--rw-rw-rw-   0        0        0     8420 2023-04-24 07:27:25.000000 gramex-1.90.0/gramex/apps/admin2/index.html
--rw-rw-rw-   0        0        0     5216 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/admin2/schedule.js
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.260237 gramex-1.90.0/gramex/apps/capture/
--rw-rw-rw-   0        0        0     4061 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/capture/README.md
--rw-rw-rw-   0        0        0     9374 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/capture/capture.js
--rw-rw-rw-   0        0        0    12034 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/capture/chromecapture.js
--rw-rw-rw-   0        0        0     4197 2020-05-27 03:04:19.000000 gramex-1.90.0/gramex/apps/capture/index.html
--rw-rw-rw-   0        0        0   141595 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/capture/package-lock.json
--rw-rw-rw-   0        0        0      863 2023-02-08 17:06:15.000000 gramex-1.90.0/gramex/apps/capture/package.json
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.291007 gramex-1.90.0/gramex/apps/filemanager/
--rw-rw-rw-   0        0        0      305 2022-04-02 07:29:37.000000 gramex-1.90.0/gramex/apps/filemanager/.snyk
--rw-rw-rw-   0        0        0     2845 2022-10-17 06:55:24.000000 gramex-1.90.0/gramex/apps/filemanager/README.html
--rw-rw-rw-   0        0        0      700 2020-05-27 03:04:19.000000 gramex-1.90.0/gramex/apps/filemanager/drivehandler-snippet.html
--rw-rw-rw-   0        0        0      612 2022-10-17 06:55:24.000000 gramex-1.90.0/gramex/apps/filemanager/filemanager-snippet.html
--rw-rw-rw-   0        0        0     2578 2022-02-19 09:58:43.000000 gramex-1.90.0/gramex/apps/filemanager/filemanager.html
--rw-rw-rw-   0        0        0     3068 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/filemanager/filemanager.js
--rw-rw-rw-   0        0        0      926 2022-02-19 09:58:43.000000 gramex-1.90.0/gramex/apps/filemanager/filemanager.py
--rw-rw-rw-   0        0        0      621 2020-05-27 03:04:19.000000 gramex-1.90.0/gramex/apps/filemanager/gramex.yaml
--rw-rw-rw-   0        0        0      914 2020-05-27 03:04:19.000000 gramex-1.90.0/gramex/apps/filemanager/index.html
--rw-rw-rw-   0        0        0      872 2020-05-27 03:04:19.000000 gramex-1.90.0/gramex/apps/filemanager/navbar.html
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:04.945276 gramex-1.90.0/gramex/apps/init/
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.337348 gramex-1.90.0/gramex/apps/init/default/
--rw-rw-rw-   0        0        0      578 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/.eslintrc.yml
--rw-rw-rw-   0        0        0       71 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/init/default/.flake8
--rw-rw-rw-   0        0        0      756 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      386 2022-02-19 10:03:02.000000 gramex-1.90.0/gramex/apps/init/default/.secrets.yaml
--rw-rw-rw-   0        0        0     1635 2022-02-19 10:03:02.000000 gramex-1.90.0/gramex/apps/init/default/.template.gitignore
--rw-rw-rw-   0        0        0      248 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/init/default/README.template.md
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.337348 gramex-1.90.0/gramex/apps/init/default/assets/
--rw-rw-rw-   0        0        0      519 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/init/default/assets/README.template.md
--rw-rw-rw-   0        0        0     1756 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/gramex.template.yaml
--rw-rw-rw-   0        0        0      694 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/index.template.html
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.337348 gramex-1.90.0/gramex/apps/init/default/js/
--rw-rw-rw-   0        0        0      602 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/init/default/js/README.template.md
--rw-rw-rw-   0        0        0     2608 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/login.template.html
--rw-rw-rw-   0        0        0      352 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/package.template.json
--rw-rw-rw-   0        0        0       80 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/style.scss
--rw-rw-rw-   0        0        0     3499 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/default/template-navbar.template.html
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.337348 gramex-1.90.0/gramex/apps/init/ide/
--rw-rw-rw-   0        0        0      378 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/ide/.gitlab-ci.template.yml
--rw-rw-rw-   0        0        0      244 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/ide/gramex.template.yaml
--rw-rw-rw-   0        0        0      738 2023-04-24 06:54:58.000000 gramex-1.90.0/gramex/apps/init/ide/index.template.html
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.354087 gramex-1.90.0/gramex/apps/init/minimal/
--rw-rw-rw-   0        0        0      247 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/minimal/gramex.template.yaml
--rw-rw-rw-   0        0        0      757 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/init/minimal/index.template.html
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.368927 gramex-1.90.0/gramex/apps/languagetool/
--rw-rw-rw-   0        0        0      709 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/languagetool/README.md
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:41.000000 gramex-1.90.0/gramex/apps/languagetool/__init__.py
--rw-rw-rw-   0        0        0      788 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/languagetool/gramex.yaml
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.429595 gramex-1.90.0/gramex/apps/logviewer/
--rw-rw-rw-   0        0        0        0 2022-06-20 08:40:32.000000 gramex-1.90.0/gramex/apps/logviewer/__init__.py
--rw-rw-rw-   0        0        0     3466 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/logviewer/config.yaml
--rw-rw-rw-   0        0        0     6291 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/logviewer/gramex.yaml
--rw-rw-rw-   0        0        0     4958 2020-05-27 03:04:19.000000 gramex-1.90.0/gramex/apps/logviewer/index.html
--rw-rw-rw-   0        0        0    13287 2023-04-10 11:33:47.000000 gramex-1.90.0/gramex/apps/logviewer/logviewer.py
--rw-rw-rw-   0        0        0      210 2018-12-27 08:44:54.000000 gramex-1.90.0/gramex/apps/logviewer/lv-card-deck.html
--rw-rw-rw-   0        0        0      386 2018-04-14 05:44:28.000000 gramex-1.90.0/gramex/apps/logviewer/lv-card.html
--rw-rw-rw-   0        0        0      526 2018-04-14 05:44:28.000000 gramex-1.90.0/gramex/apps/logviewer/lv-datepicker.html
--rw-rw-rw-   0        0        0      331 2018-04-14 05:44:28.000000 gramex-1.90.0/gramex/apps/logviewer/lv-dropdown.html
--rw-rw-rw-   0        0        0      465 2018-12-27 08:44:54.000000 gramex-1.90.0/gramex/apps/logviewer/lv-filters.html
--rw-rw-rw-   0        0        0      113 2018-04-14 05:44:28.000000 gramex-1.90.0/gramex/apps/logviewer/lv-header.html
--rw-rw-rw-   0        0        0      335 2018-04-14 05:44:28.000000 gramex-1.90.0/gramex/apps/logviewer/lv-kpi.html
--rw-rw-rw-   0        0        0      775 2023-05-07 15:42:40.000000 gramex-1.90.0/gramex/apps/logviewer/package-lock.json
--rw-rw-rw-   0        0        0      179 2021-07-06 10:52:07.000000 gramex-1.90.0/gramex/apps/logviewer/package.json
--rw-rw-rw-   0        0        0     6928 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/logviewer/render.js
--rw-rw-rw-   0        0        0     5390 2023-04-10 11:33:47.000000 gramex-1.90.0/gramex/apps/logviewer/script.js
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.447178 gramex-1.90.0/gramex/apps/mail/
--rw-rw-rw-   0        0        0      430 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/mail/gramex.yaml
--rw-rw-rw-   0        0        0     3032 2019-01-15 12:01:13.000000 gramex-1.90.0/gramex/apps/mail/index.html
--rw-rw-rw-   0        0        0      251 2018-03-15 10:39:12.000000 gramex-1.90.0/gramex/apps/mail/mailapp.py
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.447178 gramex-1.90.0/gramex/apps/mlhandler/
--rw-rw-rw-   0        0        0    15225 2022-05-03 15:40:40.000000 gramex-1.90.0/gramex/apps/mlhandler/template.html
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.466873 gramex-1.90.0/gramex/apps/pynode/
--rw-rw-rw-   0        0        0      318 2022-02-19 10:03:03.000000 gramex-1.90.0/gramex/apps/pynode/.snyk
--rw-rw-rw-   0        0        0       47 2018-10-22 05:47:08.000000 gramex-1.90.0/gramex/apps/pynode/README.md
--rw-rw-rw-   0        0        0     4122 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/pynode/index.js
--rw-rw-rw-   0        0        0     2953 2023-05-07 15:42:44.000000 gramex-1.90.0/gramex/apps/pynode/package-lock.json
--rw-rw-rw-   0        0        0      187 2022-07-03 06:28:06.000000 gramex-1.90.0/gramex/apps/pynode/package.json
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.480425 gramex-1.90.0/gramex/apps/smartalerts/
--rw-rw-rw-   0        0        0       89 2018-03-15 10:39:12.000000 gramex-1.90.0/gramex/apps/smartalerts/gramex.yaml
--rw-rw-rw-   0        0        0      429 2018-02-10 11:30:50.000000 gramex-1.90.0/gramex/apps/smartalerts/index.html
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.511699 gramex-1.90.0/gramex/apps/ui/
--rw-rw-rw-   0        0        0     1019 2023-04-10 11:33:47.000000 gramex-1.90.0/gramex/apps/ui/.snyk
--rw-rw-rw-   0        0        0    12878 2022-12-20 15:16:57.000000 gramex-1.90.0/gramex/apps/ui/__init__.py
--rw-rw-rw-   0        0        0      648 2023-04-24 07:13:24.000000 gramex-1.90.0/gramex/apps/ui/bootstrap-theme.scss
--rw-rw-rw-   0        0        0     1056 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/config.yaml
--rw-rw-rw-   0        0        0     2082 2022-11-13 06:15:28.000000 gramex-1.90.0/gramex/apps/ui/gramex.yaml
--rw-rw-rw-   0        0        0    25259 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/gramexui.scss
--rw-rw-rw-   0        0        0   588333 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/ui/package-lock.json
--rw-rw-rw-   0        0        0      341 2023-04-11 12:20:36.000000 gramex-1.90.0/gramex/apps/ui/package.json
--rw-rw-rw-   0        0        0     2486 2022-12-05 03:38:51.000000 gramex-1.90.0/gramex/apps/ui/setup.js
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.524255 gramex-1.90.0/gramex/apps/ui/theme/
--rw-rw-rw-   0        0        0    19343 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/bootstrap5.scss
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.736434 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/
--rw-rw-rw-   0        0        0     6324 2022-02-19 10:03:03.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cerulean.png
--rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cerulean.scss
--rw-rw-rw-   0        0        0     4833 2022-02-19 10:03:03.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cosmo.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cosmo.scss
--rw-rw-rw-   0        0        0     6569 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cyborg.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cyborg.scss
--rw-rw-rw-   0        0        0     5932 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/darkly.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/darkly.scss
--rw-rw-rw-   0        0        0     5114 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/flatly.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/flatly.scss
--rw-rw-rw-   0        0        0     5335 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/journal.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/journal.scss
--rw-rw-rw-   0        0        0     6141 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/litera.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/litera.scss
--rw-rw-rw-   0        0        0     4958 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/lumen.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/lumen.scss
--rw-rw-rw-   0        0        0     4818 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/lux.png
--rw-rw-rw-   0        0        0      160 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/lux.scss
--rw-rw-rw-   0        0        0     5791 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/materia.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/materia.scss
--rw-rw-rw-   0        0        0     5662 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/minty.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/minty.scss
--rw-rw-rw-   0        0        0     4777 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/pulse.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/pulse.scss
--rw-rw-rw-   0        0        0     5246 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/sandstone.png
--rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/sandstone.scss
--rw-rw-rw-   0        0        0     6213 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/simplex.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/simplex.scss
--rw-rw-rw-   0        0        0     7371 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/sketchy.png
--rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/sketchy.scss
--rw-rw-rw-   0        0        0     6288 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/slate.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/slate.scss
--rw-rw-rw-   0        0        0     6158 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/solar.png
--rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/solar.scss
--rw-rw-rw-   0        0        0     6501 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/spacelab.png
--rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/spacelab.scss
--rw-rw-rw-   0        0        0     6357 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/superhero.png
--rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/superhero.scss
--rw-rw-rw-   0        0        0     5432 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/united.png
--rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/united.scss
--rw-rw-rw-   0        0        0     4842 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/yeti.png
--rw-rw-rw-   0        0        0      163 2022-06-22 13:49:07.000000 gramex-1.90.0/gramex/apps/ui/theme/bootswatch/yeti.scss
--rw-rw-rw-   0        0        0     4573 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/default.png
--rw-rw-rw-   0        0        0       20 2022-02-19 09:58:43.000000 gramex-1.90.0/gramex/apps/ui/theme/default.scss
--rw-rw-rw-   0        0        0      831 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/index.html
--rw-rw-rw-   0        0        0    71063 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/sample.html
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.838240 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/
--rw-rw-rw-   0        0        0     6383 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/blue_voltage.png
--rw-rw-rw-   0        0        0      630 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/blue_voltage.scss
--rw-rw-rw-   0        0        0     6282 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/boldstrap.png
--rw-rw-rw-   0        0        0      478 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/boldstrap.scss
--rw-rw-rw-   0        0        0     6215 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png
--rw-rw-rw-   0        0        0      268 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.scss
--rw-rw-rw-   0        0        0     6153 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/darkster.png
--rw-rw-rw-   0        0        0     2559 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/darkster.scss
--rw-rw-rw-   0        0        0     5497 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/fresca.png
--rw-rw-rw-   0        0        0      362 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/fresca.scss
--rw-rw-rw-   0        0        0     5525 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/greyson.png
--rw-rw-rw-   0        0        0      571 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/greyson.scss
--rw-rw-rw-   0        0        0     5153 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.png
--rw-rw-rw-   0        0        0      621 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss
--rw-rw-rw-   0        0        0     5523 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/herbie.png
--rw-rw-rw-   0        0        0      480 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/herbie.scss
--rw-rw-rw-   0        0        0     6585 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/hootstrap.png
--rw-rw-rw-   0        0        0      487 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/hootstrap.scss
--rw-rw-rw-   0        0        0     5491 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/lovey.png
--rw-rw-rw-   0        0        0      461 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/lovey.scss
--rw-rw-rw-   0        0        0     6009 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/monotony.png
--rw-rw-rw-   0        0        0      486 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/monotony.scss
--rw-rw-rw-   0        0        0     5546 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/poypull.png
--rw-rw-rw-   0        0        0      541 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/poypull.scss
--rw-rw-rw-   0        0        0     5430 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/signal.png
--rw-rw-rw-   0        0        0      576 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/signal.scss
--rw-rw-rw-   0        0        0     5338 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/tequila.png
--rw-rw-rw-   0        0        0      371 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/ui/theme/themes-guide/tequila.scss
--rw-rw-rw-   0        0        0      801 2022-09-13 04:40:48.000000 gramex-1.90.0/gramex/apps/ui/theme/themes.json
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.952648 gramex-1.90.0/gramex/apps/uifactory/
--rw-rw-rw-   0        0        0      739 2022-11-02 08:06:14.000000 gramex-1.90.0/gramex/apps/uifactory/.eslintrc.js
--rw-rw-rw-   0        0        0       46 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/.gitattributes
--rw-rw-rw-   0        0        0       57 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.952648 gramex-1.90.0/gramex/apps/uifactory/assets/
--rw-rw-rw-   0        0        0      432 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/assets/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.959658 gramex-1.90.0/gramex/apps/uifactory/assets/data/
--rw-rw-rw-   0        0        0     1674 2022-09-13 04:40:51.000000 gramex-1.90.0/gramex/apps/uifactory/assets/data/input.json
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.959658 gramex-1.90.0/gramex/apps/uifactory/assets/img/
--rw-rw-rw-   0        0        0      706 2022-06-23 02:35:29.000000 gramex-1.90.0/gramex/apps/uifactory/assets/img/arrows-move.svg
--rw-rw-rw-   0        0        0      496 2022-06-23 02:35:29.000000 gramex-1.90.0/gramex/apps/uifactory/assets/img/clipboard.svg
--rw-rw-rw-   0        0        0      978 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png
--rw-rw-rw-   0        0        0      573 2022-06-23 02:35:29.000000 gramex-1.90.0/gramex/apps/uifactory/assets/img/trash.svg
--rw-rw-rw-   0        0        0     6667 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/create.html
--rw-rw-rw-   0        0        0     2673 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/edit.html
--rw-rw-rw-   0        0        0      694 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/field-actions.html
--rw-rw-rw-   0        0        0     4361 2022-11-06 08:24:31.000000 gramex-1.90.0/gramex/apps/uifactory/form_builder.py
--rw-rw-rw-   0        0        0     4749 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/gramex.yaml
--rw-rw-rw-   0        0        0     6274 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/index.html
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.993004 gramex-1.90.0/gramex/apps/uifactory/js/
--rw-rw-rw-   0        0        0      601 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/README.md
--rw-rw-rw-   0        0        0      435 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/embed.js
--rw-rw-rw-   0        0        0    16411 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/fields.js
--rw-rw-rw-   0        0        0     1942 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/fork-form.js
--rw-rw-rw-   0        0        0     3080 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/index.js
--rw-rw-rw-   0        0        0     9228 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/script.js
--rw-rw-rw-   0        0        0      829 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/utils.js
--rw-rw-rw-   0        0        0     2776 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/js/viewform.js
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.010178 gramex-1.90.0/gramex/apps/uifactory/modals/
--rw-rw-rw-   0        0        0     1117 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/modals/add-field.html
--rw-rw-rw-   0        0        0     4107 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/modals/embed.html
--rw-rw-rw-   0        0        0      898 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/modals/remove.html
--rw-rw-rw-   0        0        0      952 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/modals/rename.html
--rw-rw-rw-   0        0        0     1323 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/modals/themes.html
--rw-rw-rw-   0        0        0     5781 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/uifactory/package-lock.json
--rw-rw-rw-   0        0        0      206 2022-03-03 08:20:09.000000 gramex-1.90.0/gramex/apps/uifactory/package.json
--rw-rw-rw-   0        0        0     1548 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/popover-form.html
--rw-rw-rw-   0        0        0     1952 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/sample.html
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.017264 gramex-1.90.0/gramex/apps/uifactory/snippets/
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.021247 gramex-1.90.0/gramex/apps/uifactory/snippets/button/
--rw-rw-rw-   0        0        0     2795 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/button/bs4-button.js
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.024264 gramex-1.90.0/gramex/apps/uifactory/snippets/checkbox/
--rw-rw-rw-   0        0        0     1225 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.036034 gramex-1.90.0/gramex/apps/uifactory/snippets/email/
--rw-rw-rw-   0        0        0      604 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/email/bs4-email.js
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.038838 gramex-1.90.0/gramex/apps/uifactory/snippets/hidden/
--rw-rw-rw-   0        0        0      327 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/hidden/bs4-hidden.js
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.049232 gramex-1.90.0/gramex/apps/uifactory/snippets/html/
--rw-rw-rw-   0        0        0      292 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/html/bs4-html.js
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.049232 gramex-1.90.0/gramex/apps/uifactory/snippets/multiselect/
--rw-rw-rw-   0        0        0     4735 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.057921 gramex-1.90.0/gramex/apps/uifactory/snippets/number/
--rw-rw-rw-   0        0        0      736 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/number/bs4-number.js
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.063055 gramex-1.90.0/gramex/apps/uifactory/snippets/password/
--rw-rw-rw-   0        0        0      375 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/password/bs4-password.js
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.067634 gramex-1.90.0/gramex/apps/uifactory/snippets/radio/
--rw-rw-rw-   0        0        0     1034 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/radio/bs4-radio.js
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.075899 gramex-1.90.0/gramex/apps/uifactory/snippets/range/
--rw-rw-rw-   0        0        0      610 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/range/bs4-range.js
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.079284 gramex-1.90.0/gramex/apps/uifactory/snippets/select/
--rw-rw-rw-   0        0        0     1617 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/select/bs4-select.js
--rw-rw-rw-   0        0        0      946 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/setup.js
--rw-rw-rw-   0        0        0        3 2023-04-17 10:18:07.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/snippets.json
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.084684 gramex-1.90.0/gramex/apps/uifactory/snippets/text/
--rw-rw-rw-   0        0        0      974 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/text/bs4-text.js
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.091213 gramex-1.90.0/gramex/apps/uifactory/snippets/textarea/
--rw-rw-rw-   0        0        0     1094 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js
--rw-rw-rw-   0        0        0     1815 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps/uifactory/style.scss
--rw-rw-rw-   0        0        0     2013 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/template-navbar-view-form.html
--rw-rw-rw-   0        0        0     1020 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/template-navbar.html
--rw-rw-rw-   0        0        0      415 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/toast.html
--rw-rw-rw-   0        0        0     6516 2022-02-19 10:03:04.000000 gramex-1.90.0/gramex/apps/uifactory/viewform.html
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.109236 gramex-1.90.0/gramex/apps/update/
--rw-rw-rw-   0        0        0      565 2018-10-30 07:47:04.000000 gramex-1.90.0/gramex/apps/update/README.md
--rw-rw-rw-   0        0        0     2397 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/apps/update/gramex.yaml
--rw-rw-rw-   0        0        0     4593 2022-11-06 08:24:31.000000 gramex-1.90.0/gramex/apps/update/gramexupdate.py
--rw-rw-rw-   0        0        0     3310 2022-03-03 08:20:09.000000 gramex-1.90.0/gramex/apps/update/index.html
--rw-rw-rw-   0        0        0      277 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/apps.yaml
--rw-rw-rw-   0        0        0    56930 2023-04-15 03:29:37.000000 gramex-1.90.0/gramex/cache.py
--rw-rw-rw-   0        0        0    35221 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/config.py
--rw-rw-rw-   0        0        0    93430 2023-04-20 06:58:42.000000 gramex-1.90.0/gramex/data.py
--rw-rw-rw-   0        0        0     6353 2022-11-23 04:49:14.000000 gramex-1.90.0/gramex/debug.py
--rw-rw-rw-   0        0        0     1825 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/deploy.yaml
--rw-rw-rw-   0        0        0     1466 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/download.vega.js
--rw-rw-rw-   0        0        0    12057 2018-10-22 05:47:08.000000 gramex-1.90.0/gramex/favicon.ico
--rw-rw-rw-   0        0        0    16670 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/gramex.yaml
--rw-rw-rw-   0        0        0     2011 2023-04-18 07:09:40.000000 gramex-1.90.0/gramex/gramexfeatures.csv
--rw-rw-rw-   0        0        0    14445 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/gramexsize.csv
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.309057 gramex-1.90.0/gramex/handlers/
--rw-rw-rw-   0        0        0     1368 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/400.html
--rw-rw-rw-   0        0        0     2081 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/401.html
--rw-rw-rw-   0        0        0     2374 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/403.html
--rw-rw-rw-   0        0        0     1399 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/404.html
--rw-rw-rw-   0        0        0     2163 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/500.html
--rw-rw-rw-   0        0        0     2643 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/handlers/__init__.py
--rw-rw-rw-   0        0        0      532 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/auth.recaptcha.template.html
--rw-rw-rw-   0        0        0     3862 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/handlers/auth.template.html
--rw-rw-rw-   0        0        0    17394 2023-04-10 11:33:47.000000 gramex-1.90.0/gramex/handlers/authhandler.py
--rw-rw-rw-   0        0        0    60917 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/handlers/basehandler.py
--rw-rw-rw-   0        0        0    15648 2022-12-20 15:16:57.000000 gramex-1.90.0/gramex/handlers/capturehandler.py
--rw-rw-rw-   0        0        0     1477 2022-11-06 08:24:25.000000 gramex-1.90.0/gramex/handlers/comichandler.py
--rw-rw-rw-   0        0        0     8922 2022-11-06 08:24:26.000000 gramex-1.90.0/gramex/handlers/drivehandler.py
--rw-rw-rw-   0        0        0    14849 2023-02-24 08:15:32.000000 gramex-1.90.0/gramex/handlers/filehandler.py
--rw-rw-rw-   0        0        0     1271 2022-07-03 06:28:09.000000 gramex-1.90.0/gramex/handlers/filehandler.template.html
--rw-rw-rw-   0        0        0      198 2023-01-03 16:10:30.000000 gramex-1.90.0/gramex/handlers/filterhandler.py
--rw-rw-rw-   0        0        0    13238 2023-01-03 16:10:30.000000 gramex-1.90.0/gramex/handlers/formhandler.py
--rw-rw-rw-   0        0        0     3774 2022-11-23 03:19:45.000000 gramex-1.90.0/gramex/handlers/functionhandler.py
--rw-rw-rw-   0        0        0     6622 2022-11-23 03:19:45.000000 gramex-1.90.0/gramex/handlers/jsonhandler.py
--rw-rw-rw-   0        0        0     6838 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/handlers/messagehandler.py
--rw-rw-rw-   0        0        0    16154 2022-11-23 04:49:14.000000 gramex-1.90.0/gramex/handlers/mlhandler.py
--rw-rw-rw-   0        0        0     7492 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/modelhandler.py
--rw-rw-rw-   0        0        0     1413 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/openapiconfig.yaml
--rw-rw-rw-   0        0        0     7193 2022-12-20 15:16:57.000000 gramex-1.90.0/gramex/handlers/openapihandler.py
--rw-rw-rw-   0        0        0      818 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/handlers/pptxhandler.py
--rw-rw-rw-   0        0        0     6216 2022-11-23 03:19:45.000000 gramex-1.90.0/gramex/handlers/processhandler.py
--rw-rw-rw-   0        0        0     7715 2022-11-23 03:19:45.000000 gramex-1.90.0/gramex/handlers/proxyhandler.py
--rw-rw-rw-   0        0        0     1362 2022-10-17 06:55:24.000000 gramex-1.90.0/gramex/handlers/queryhandler.template.html
--rw-rw-rw-   0        0        0    11443 2022-11-23 03:19:45.000000 gramex-1.90.0/gramex/handlers/socialhandler.py
--rw-rw-rw-   0        0        0     9415 2022-11-23 03:19:45.000000 gramex-1.90.0/gramex/handlers/uploadhandler.py
--rw-rw-rw-   0        0        0     2121 2022-11-23 03:19:45.000000 gramex-1.90.0/gramex/handlers/websockethandler.py
--rw-rw-rw-   0        0        0     1458 2022-11-23 04:49:14.000000 gramex-1.90.0/gramex/http.py
--rw-rw-rw-   0        0        0    35070 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/install.py
--rw-rw-rw-   0        0        0     2086 2022-09-13 04:40:51.000000 gramex-1.90.0/gramex/license.py
--rw-rw-rw-   0        0        0     2005 2023-02-08 17:06:16.000000 gramex-1.90.0/gramex/migrate.py
--rw-rw-rw-   0        0        0    18498 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/ml.py
--rw-rw-rw-   0        0        0    13687 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/ml_api.py
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.542414 gramex-1.90.0/gramex/pptgen/
--rw-rw-rw-   0        0        0     9976 2022-11-23 04:49:14.000000 gramex-1.90.0/gramex/pptgen/__init__.py
--rw-rw-rw-   0        0        0    18876 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/pptgen/color.py
--rw-rw-rw-   0        0        0     7779 2018-01-31 16:40:23.000000 gramex-1.90.0/gramex/pptgen/colors.json
--rw-rw-rw-   0        0        0    45490 2022-11-02 08:06:17.000000 gramex-1.90.0/gramex/pptgen/commands.py
--rw-rw-rw-   0        0        0     6351 2018-01-31 16:40:23.000000 gramex-1.90.0/gramex/pptgen/fonts.json
--rw-rw-rw-   0        0        0     1304 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/pptgen/fontwidth.py
--rw-rw-rw-   0        0        0    26306 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/pptgen/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.542414 gramex-1.90.0/gramex/pptgen2/
--rw-rw-rw-   0        0        0    23501 2023-04-26 11:16:23.000000 gramex-1.90.0/gramex/pptgen2/__init__.py
--rw-rw-rw-   0        0        0    34484 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/pptgen2/commands.py
--rw-rw-rw-   0        0        0    12068 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/pptgen2/config.yaml
--rw-rw-rw-   0        0        0     4208 2022-11-23 04:49:14.000000 gramex-1.90.0/gramex/pynode.py
--rw-rw-rw-   0        0        0     2985 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/scale.py
--rw-rw-rw-   0        0        0     1057 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/secrets.py
--rw-rw-rw-   0        0        0     2508 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/servicenow.yaml
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.604612 gramex-1.90.0/gramex/services/
--rw-rw-rw-   0        0        0    39493 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/services/__init__.py
--rw-rw-rw-   0        0        0    11176 2023-05-07 15:51:36.000000 gramex-1.90.0/gramex/services/emailer.py
--rw-rw-rw-   0        0        0     3615 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/services/rediscache.py
--rw-rw-rw-   0        0        0     7164 2023-02-08 17:06:16.000000 gramex-1.90.0/gramex/services/scheduler.py
--rw-rw-rw-   0        0        0     3668 2022-11-06 08:24:30.000000 gramex-1.90.0/gramex/services/sms.py
--rw-rw-rw-   0        0        0     6385 2022-11-23 04:49:14.000000 gramex-1.90.0/gramex/services/ttlcache.py
--rw-rw-rw-   0        0        0     4529 2022-11-06 08:24:30.000000 gramex-1.90.0/gramex/services/urlcache.py
--rw-rw-rw-   0        0        0     5762 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/services/watcher.py
--rw-rw-rw-   0        0        0     3831 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/sm_api.py
--rw-rw-rw-   0        0        0     8638 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/topcause.py
--rw-rw-rw-   0        0        0     8710 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/transformers.py
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.623721 gramex-1.90.0/gramex/transforms/
--rw-rw-rw-   0        0        0      777 2023-04-14 07:12:43.000000 gramex-1.90.0/gramex/transforms/__init__.py
--rw-rw-rw-   0        0        0     1658 2022-09-13 04:40:51.000000 gramex-1.90.0/gramex/transforms/auth.py
--rw-rw-rw-   0        0        0     3542 2022-11-02 08:06:18.000000 gramex-1.90.0/gramex/transforms/template.py
--rw-rw-rw-   0        0        0    32281 2023-04-14 04:57:01.000000 gramex-1.90.0/gramex/transforms/transforms.py
--rw-rw-rw-   0        0        0    10122 2022-11-06 08:24:30.000000 gramex-1.90.0/gramex/transforms/twitterstream.py
--rw-rw-rw-   0        0        0     6808 2022-11-13 04:18:56.000000 gramex-1.90.0/gramex/winservice.py
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:05.191893 gramex-1.90.0/gramex.egg-info/
--rw-rw-rw-   0        0        0     2956 2023-05-07 15:53:01.000000 gramex-1.90.0/gramex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11970 2023-05-07 15:53:04.000000 gramex-1.90.0/gramex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 15:53:01.000000 gramex-1.90.0/gramex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-05-07 15:53:01.000000 gramex-1.90.0/gramex.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      945 2023-05-07 15:53:01.000000 gramex-1.90.0/gramex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-07 15:53:01.000000 gramex-1.90.0/gramex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6088 2023-05-07 15:51:36.000000 gramex-1.90.0/pyproject.toml
--rw-rw-rw-   0        0        0      540 2023-05-07 15:53:06.841813 gramex-1.90.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-07 15:53:06.808865 gramex-1.90.0/tests/
--rw-rw-rw-   0        0        0     5233 2022-11-06 08:24:18.000000 gramex-1.90.0/tests/test_admin.py
--rw-rw-rw-   0        0        0     9054 2023-04-18 08:45:54.000000 gramex-1.90.0/tests/test_alerts.py
--rw-rw-rw-   0        0        0     3981 2022-11-06 08:24:18.000000 gramex-1.90.0/tests/test_args.py
--rw-rw-rw-   0        0        0    39027 2023-05-07 15:51:36.000000 gramex-1.90.0/tests/test_auth.py
--rw-rw-rw-   0        0        0    14612 2022-11-06 08:24:18.000000 gramex-1.90.0/tests/test_cache.py
--rw-rw-rw-   0        0        0    15062 2022-11-23 04:49:14.000000 gramex-1.90.0/tests/test_capturehandler.py
--rw-rw-rw-   0        0        0     1288 2022-11-06 08:24:19.000000 gramex-1.90.0/tests/test_comichandler.py
--rw-rw-rw-   0        0        0    11152 2022-11-06 08:24:20.000000 gramex-1.90.0/tests/test_drivehandler.py
--rw-rw-rw-   0        0        0    17841 2022-11-06 08:24:20.000000 gramex-1.90.0/tests/test_filehandler.py
--rw-rw-rw-   0        0        0     6797 2022-11-24 04:51:52.000000 gramex-1.90.0/tests/test_filterhandler.py
--rw-rw-rw-   0        0        0    35746 2023-01-03 16:10:30.000000 gramex-1.90.0/tests/test_formhandler.py
--rw-rw-rw-   0        0        0     8784 2022-11-06 08:24:22.000000 gramex-1.90.0/tests/test_functionhandler.py
--rw-rw-rw-   0        0        0     3201 2022-11-06 08:24:22.000000 gramex-1.90.0/tests/test_gramexlog.py
--rw-rw-rw-   0        0        0    15699 2022-11-23 04:49:14.000000 gramex-1.90.0/tests/test_handlers.py
--rw-rw-rw-   0        0        0     1475 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_init.py
--rw-rw-rw-   0        0        0     8931 2022-11-23 04:49:14.000000 gramex-1.90.0/tests/test_install.py
--rw-rw-rw-   0        0        0     6361 2022-11-06 08:24:23.000000 gramex-1.90.0/tests/test_jsonhandler.py
--rw-rw-rw-   0        0        0     3896 2022-11-06 08:24:23.000000 gramex-1.90.0/tests/test_ldapauth.py
--rw-rw-rw-   0        0        0     7519 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_logviewer.py
--rw-rw-rw-   0        0        0    32878 2022-11-23 04:49:14.000000 gramex-1.90.0/tests/test_mlhandler.py
--rw-rw-rw-   0        0        0     4745 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_modelhandler.py
--rw-rw-rw-   0        0        0     7082 2022-12-20 15:16:57.000000 gramex-1.90.0/tests/test_openapihandler.py
--rw-rw-rw-   0        0        0     1411 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_pptxhandler.py
--rw-rw-rw-   0        0        0     3530 2022-11-06 08:24:24.000000 gramex-1.90.0/tests/test_processhandler.py
--rw-rw-rw-   0        0        0     3834 2022-11-06 08:24:24.000000 gramex-1.90.0/tests/test_proxyhandler.py
--rw-rw-rw-   0        0        0     1527 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_pynode.py
--rw-rw-rw-   0        0        0     1220 2022-11-06 08:24:24.000000 gramex-1.90.0/tests/test_schedule.py
--rw-rw-rw-   0        0        0      757 2022-02-19 10:03:06.000000 gramex-1.90.0/tests/test_secrets.py
--rw-rw-rw-   0        0        0      330 2020-05-27 03:04:19.000000 gramex-1.90.0/tests/test_sms.py
--rw-rw-rw-   0        0        0      180 2017-08-29 07:52:03.000000 gramex-1.90.0/tests/test_subapp.py
--rw-rw-rw-   0        0        0     5382 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_subprocess.py
--rw-rw-rw-   0        0        0     2277 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_translater.py
--rw-rw-rw-   0        0        0     2895 2022-11-06 08:24:24.000000 gramex-1.90.0/tests/test_twitterresthandler.py
--rw-rw-rw-   0        0        0     2352 2022-11-06 08:24:24.000000 gramex-1.90.0/tests/test_ui.py
--rw-rw-rw-   0        0        0     2359 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_update.py
--rw-rw-rw-   0        0        0     6563 2022-11-06 08:24:25.000000 gramex-1.90.0/tests/test_uploadhandler.py
--rw-rw-rw-   0        0        0     1966 2022-11-02 08:06:18.000000 gramex-1.90.0/tests/test_watcher.py
--rw-rw-rw-   0        0        0     2647 2022-11-06 08:24:25.000000 gramex-1.90.0/tests/test_websockethandler.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.568195 gramex-1.91.0/
+-rw-rw-rw-   0        0        0     1968 2023-06-08 09:27:24.000000 gramex-1.91.0/.gitignore
+-rw-rw-rw-   0        0        0     1274 2022-03-03 08:20:08.000000 gramex-1.91.0/LICENSE
+-rw-rw-rw-   0        0        0      641 2023-05-13 04:30:57.000000 gramex-1.91.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2956 2023-06-08 09:28:38.569297 gramex-1.91.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2022-09-13 04:40:48.000000 gramex-1.91.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.165996 gramex-1.91.0/gramex/
+-rw-rw-rw-   0        0        0    15366 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/__init__.py
+-rw-rw-rw-   0        0        0      242 2022-07-03 06:28:06.000000 gramex-1.91.0/gramex/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.215174 gramex-1.91.0/gramex/apps/
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:01.000000 gramex-1.91.0/gramex/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.218175 gramex-1.91.0/gramex/apps/admin/
+-rw-rw-rw-   0        0        0        9 2019-01-01 03:16:23.000000 gramex-1.91.0/gramex/apps/admin/.gitignore
+-rw-rw-rw-   0        0        0      129 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/admin/gramex.yaml
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.247430 gramex-1.91.0/gramex/apps/admin2/
+-rw-rw-rw-   0        0        0      226 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/admin2/.snyk
+-rw-rw-rw-   0        0        0      228 2019-04-01 03:34:34.000000 gramex-1.91.0/gramex/apps/admin2/admin.css
+-rw-rw-rw-   0        0        0     3116 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/admin2/gramex.yaml
+-rw-rw-rw-   0        0        0    12257 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/admin2/gramexadmin.py
+-rw-rw-rw-   0        0        0     8420 2023-04-24 07:27:25.000000 gramex-1.91.0/gramex/apps/admin2/index.html
+-rw-rw-rw-   0        0        0     5216 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/admin2/schedule.js
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.266968 gramex-1.91.0/gramex/apps/capture/
+-rw-rw-rw-   0        0        0     4061 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/capture/README.md
+-rw-rw-rw-   0        0        0     9374 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/capture/capture.js
+-rw-rw-rw-   0        0        0    12051 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/apps/capture/chromecapture.js
+-rw-rw-rw-   0        0        0     4197 2020-05-27 03:04:19.000000 gramex-1.91.0/gramex/apps/capture/index.html
+-rw-rw-rw-   0        0        0   142301 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/apps/capture/package-lock.json
+-rw-rw-rw-   0        0        0      863 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/capture/package.json
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.297507 gramex-1.91.0/gramex/apps/filemanager/
+-rw-rw-rw-   0        0        0      305 2022-04-02 07:29:37.000000 gramex-1.91.0/gramex/apps/filemanager/.snyk
+-rw-rw-rw-   0        0        0     2845 2022-10-17 06:55:24.000000 gramex-1.91.0/gramex/apps/filemanager/README.html
+-rw-rw-rw-   0        0        0      700 2020-05-27 03:04:19.000000 gramex-1.91.0/gramex/apps/filemanager/drivehandler-snippet.html
+-rw-rw-rw-   0        0        0      612 2022-10-17 06:55:24.000000 gramex-1.91.0/gramex/apps/filemanager/filemanager-snippet.html
+-rw-rw-rw-   0        0        0     2578 2022-02-19 09:58:43.000000 gramex-1.91.0/gramex/apps/filemanager/filemanager.html
+-rw-rw-rw-   0        0        0     3068 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/filemanager/filemanager.js
+-rw-rw-rw-   0        0        0      926 2022-02-19 09:58:43.000000 gramex-1.91.0/gramex/apps/filemanager/filemanager.py
+-rw-rw-rw-   0        0        0      621 2020-05-27 03:04:19.000000 gramex-1.91.0/gramex/apps/filemanager/gramex.yaml
+-rw-rw-rw-   0        0        0      914 2020-05-27 03:04:19.000000 gramex-1.91.0/gramex/apps/filemanager/index.html
+-rw-rw-rw-   0        0        0      872 2020-05-27 03:04:19.000000 gramex-1.91.0/gramex/apps/filemanager/navbar.html
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.034280 gramex-1.91.0/gramex/apps/init/
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.332967 gramex-1.91.0/gramex/apps/init/default/
+-rw-rw-rw-   0        0        0      578 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/init/default/.eslintrc.yml
+-rw-rw-rw-   0        0        0       71 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/init/default/.flake8
+-rw-rw-rw-   0        0        0      756 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/init/default/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      386 2022-02-19 10:03:02.000000 gramex-1.91.0/gramex/apps/init/default/.secrets.yaml
+-rw-rw-rw-   0        0        0     1635 2022-02-19 10:03:02.000000 gramex-1.91.0/gramex/apps/init/default/.template.gitignore
+-rw-rw-rw-   0        0        0      248 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/init/default/README.template.md
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.335977 gramex-1.91.0/gramex/apps/init/default/assets/
+-rw-rw-rw-   0        0        0      519 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/init/default/assets/README.template.md
+-rw-rw-rw-   0        0        0     1756 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/init/default/gramex.template.yaml
+-rw-rw-rw-   0        0        0      694 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/init/default/index.template.html
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.342142 gramex-1.91.0/gramex/apps/init/default/js/
+-rw-rw-rw-   0        0        0      602 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/init/default/js/README.template.md
+-rw-rw-rw-   0        0        0     2608 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/init/default/login.template.html
+-rw-rw-rw-   0        0        0      352 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/init/default/package.template.json
+-rw-rw-rw-   0        0        0       80 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/init/default/style.scss
+-rw-rw-rw-   0        0        0     3499 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/init/default/template-navbar.template.html
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.357569 gramex-1.91.0/gramex/apps/init/ide/
+-rw-rw-rw-   0        0        0      378 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/init/ide/.gitlab-ci.template.yml
+-rw-rw-rw-   0        0        0      244 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/init/ide/gramex.template.yaml
+-rw-rw-rw-   0        0        0      738 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/init/ide/index.template.html
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.362599 gramex-1.91.0/gramex/apps/init/minimal/
+-rw-rw-rw-   0        0        0      247 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/init/minimal/gramex.template.yaml
+-rw-rw-rw-   0        0        0      757 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/init/minimal/index.template.html
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.370105 gramex-1.91.0/gramex/apps/languagetool/
+-rw-rw-rw-   0        0        0      709 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/languagetool/README.md
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:41.000000 gramex-1.91.0/gramex/apps/languagetool/__init__.py
+-rw-rw-rw-   0        0        0      788 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/languagetool/gramex.yaml
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.418012 gramex-1.91.0/gramex/apps/logviewer/
+-rw-rw-rw-   0        0        0        0 2022-06-20 08:40:32.000000 gramex-1.91.0/gramex/apps/logviewer/__init__.py
+-rw-rw-rw-   0        0        0     3466 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/logviewer/config.yaml
+-rw-rw-rw-   0        0        0     6291 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/logviewer/gramex.yaml
+-rw-rw-rw-   0        0        0     4958 2020-05-27 03:04:19.000000 gramex-1.91.0/gramex/apps/logviewer/index.html
+-rw-rw-rw-   0        0        0    13287 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/logviewer/logviewer.py
+-rw-rw-rw-   0        0        0      210 2018-12-27 08:44:54.000000 gramex-1.91.0/gramex/apps/logviewer/lv-card-deck.html
+-rw-rw-rw-   0        0        0      386 2018-04-14 05:44:28.000000 gramex-1.91.0/gramex/apps/logviewer/lv-card.html
+-rw-rw-rw-   0        0        0      526 2018-04-14 05:44:28.000000 gramex-1.91.0/gramex/apps/logviewer/lv-datepicker.html
+-rw-rw-rw-   0        0        0      331 2018-04-14 05:44:28.000000 gramex-1.91.0/gramex/apps/logviewer/lv-dropdown.html
+-rw-rw-rw-   0        0        0      465 2018-12-27 08:44:54.000000 gramex-1.91.0/gramex/apps/logviewer/lv-filters.html
+-rw-rw-rw-   0        0        0      113 2018-04-14 05:44:28.000000 gramex-1.91.0/gramex/apps/logviewer/lv-header.html
+-rw-rw-rw-   0        0        0      335 2018-04-14 05:44:28.000000 gramex-1.91.0/gramex/apps/logviewer/lv-kpi.html
+-rw-rw-rw-   0        0        0      775 2023-06-08 09:14:28.000000 gramex-1.91.0/gramex/apps/logviewer/package-lock.json
+-rw-rw-rw-   0        0        0      179 2021-07-06 10:52:07.000000 gramex-1.91.0/gramex/apps/logviewer/package.json
+-rw-rw-rw-   0        0        0     6928 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/logviewer/render.js
+-rw-rw-rw-   0        0        0     5390 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/logviewer/script.js
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.428142 gramex-1.91.0/gramex/apps/mail/
+-rw-rw-rw-   0        0        0      430 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/mail/gramex.yaml
+-rw-rw-rw-   0        0        0     3032 2019-01-15 12:01:13.000000 gramex-1.91.0/gramex/apps/mail/index.html
+-rw-rw-rw-   0        0        0      251 2018-03-15 10:39:12.000000 gramex-1.91.0/gramex/apps/mail/mailapp.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.430172 gramex-1.91.0/gramex/apps/mlhandler/
+-rw-rw-rw-   0        0        0    15225 2022-05-03 15:40:40.000000 gramex-1.91.0/gramex/apps/mlhandler/template.html
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.443320 gramex-1.91.0/gramex/apps/pynode/
+-rw-rw-rw-   0        0        0      318 2022-02-19 10:03:03.000000 gramex-1.91.0/gramex/apps/pynode/.snyk
+-rw-rw-rw-   0        0        0       47 2018-10-22 05:47:08.000000 gramex-1.91.0/gramex/apps/pynode/README.md
+-rw-rw-rw-   0        0        0     4122 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/pynode/index.js
+-rw-rw-rw-   0        0        0     2953 2023-06-08 09:14:33.000000 gramex-1.91.0/gramex/apps/pynode/package-lock.json
+-rw-rw-rw-   0        0        0      187 2022-07-03 06:28:06.000000 gramex-1.91.0/gramex/apps/pynode/package.json
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.447318 gramex-1.91.0/gramex/apps/smartalerts/
+-rw-rw-rw-   0        0        0       89 2018-03-15 10:39:12.000000 gramex-1.91.0/gramex/apps/smartalerts/gramex.yaml
+-rw-rw-rw-   0        0        0      429 2018-02-10 11:30:50.000000 gramex-1.91.0/gramex/apps/smartalerts/index.html
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.474119 gramex-1.91.0/gramex/apps/ui/
+-rw-rw-rw-   0        0        0     1019 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/ui/.snyk
+-rw-rw-rw-   0        0        0    12872 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/apps/ui/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-04-24 07:13:24.000000 gramex-1.91.0/gramex/apps/ui/bootstrap-theme.scss
+-rw-rw-rw-   0        0        0     1056 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/config.yaml
+-rw-rw-rw-   0        0        0     2082 2022-11-13 06:15:28.000000 gramex-1.91.0/gramex/apps/ui/gramex.yaml
+-rw-rw-rw-   0        0        0    25259 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/gramexui.scss
+-rw-rw-rw-   0        0        0   589144 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/apps/ui/package-lock.json
+-rw-rw-rw-   0        0        0      341 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/ui/package.json
+-rw-rw-rw-   0        0        0     2486 2022-12-05 03:38:51.000000 gramex-1.91.0/gramex/apps/ui/setup.js
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.501792 gramex-1.91.0/gramex/apps/ui/theme/
+-rw-rw-rw-   0        0        0    19343 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/bootstrap5.scss
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.712455 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/
+-rw-rw-rw-   0        0        0     6324 2022-02-19 10:03:03.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/cerulean.png
+-rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/cerulean.scss
+-rw-rw-rw-   0        0        0     4833 2022-02-19 10:03:03.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/cosmo.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/cosmo.scss
+-rw-rw-rw-   0        0        0     6569 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/cyborg.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/cyborg.scss
+-rw-rw-rw-   0        0        0     5932 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/darkly.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/darkly.scss
+-rw-rw-rw-   0        0        0     5114 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/flatly.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/flatly.scss
+-rw-rw-rw-   0        0        0     5335 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/journal.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/journal.scss
+-rw-rw-rw-   0        0        0     6141 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/litera.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/litera.scss
+-rw-rw-rw-   0        0        0     4958 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/lumen.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/lumen.scss
+-rw-rw-rw-   0        0        0     4818 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/lux.png
+-rw-rw-rw-   0        0        0      160 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/lux.scss
+-rw-rw-rw-   0        0        0     5791 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/materia.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/materia.scss
+-rw-rw-rw-   0        0        0     5662 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/minty.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/minty.scss
+-rw-rw-rw-   0        0        0     4777 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/pulse.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/pulse.scss
+-rw-rw-rw-   0        0        0     5246 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/sandstone.png
+-rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/sandstone.scss
+-rw-rw-rw-   0        0        0     6213 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/simplex.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/simplex.scss
+-rw-rw-rw-   0        0        0     7371 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/sketchy.png
+-rw-rw-rw-   0        0        0      172 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/sketchy.scss
+-rw-rw-rw-   0        0        0     6288 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/slate.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/slate.scss
+-rw-rw-rw-   0        0        0     6158 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/solar.png
+-rw-rw-rw-   0        0        0      166 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/solar.scss
+-rw-rw-rw-   0        0        0     6501 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/spacelab.png
+-rw-rw-rw-   0        0        0      175 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/spacelab.scss
+-rw-rw-rw-   0        0        0     6357 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/superhero.png
+-rw-rw-rw-   0        0        0      178 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/superhero.scss
+-rw-rw-rw-   0        0        0     5432 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/united.png
+-rw-rw-rw-   0        0        0      169 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/united.scss
+-rw-rw-rw-   0        0        0     4842 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/yeti.png
+-rw-rw-rw-   0        0        0      163 2022-06-22 13:49:07.000000 gramex-1.91.0/gramex/apps/ui/theme/bootswatch/yeti.scss
+-rw-rw-rw-   0        0        0     4573 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/default.png
+-rw-rw-rw-   0        0        0       20 2022-02-19 09:58:43.000000 gramex-1.91.0/gramex/apps/ui/theme/default.scss
+-rw-rw-rw-   0        0        0      831 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/index.html
+-rw-rw-rw-   0        0        0    71063 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/sample.html
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.867299 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/
+-rw-rw-rw-   0        0        0     6383 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/blue_voltage.png
+-rw-rw-rw-   0        0        0      630 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/blue_voltage.scss
+-rw-rw-rw-   0        0        0     6282 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/boldstrap.png
+-rw-rw-rw-   0        0        0      478 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/boldstrap.scss
+-rw-rw-rw-   0        0        0     6215 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png
+-rw-rw-rw-   0        0        0      268 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.scss
+-rw-rw-rw-   0        0        0     6153 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/darkster.png
+-rw-rw-rw-   0        0        0     2559 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/darkster.scss
+-rw-rw-rw-   0        0        0     5497 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/fresca.png
+-rw-rw-rw-   0        0        0      362 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/fresca.scss
+-rw-rw-rw-   0        0        0     5525 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/greyson.png
+-rw-rw-rw-   0        0        0      571 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/greyson.scss
+-rw-rw-rw-   0        0        0     5153 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.png
+-rw-rw-rw-   0        0        0      621 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss
+-rw-rw-rw-   0        0        0     5523 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/herbie.png
+-rw-rw-rw-   0        0        0      480 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/herbie.scss
+-rw-rw-rw-   0        0        0     6585 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/hootstrap.png
+-rw-rw-rw-   0        0        0      487 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/hootstrap.scss
+-rw-rw-rw-   0        0        0     5491 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/lovey.png
+-rw-rw-rw-   0        0        0      461 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/lovey.scss
+-rw-rw-rw-   0        0        0     6009 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/monotony.png
+-rw-rw-rw-   0        0        0      486 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/monotony.scss
+-rw-rw-rw-   0        0        0     5546 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/poypull.png
+-rw-rw-rw-   0        0        0      541 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/poypull.scss
+-rw-rw-rw-   0        0        0     5430 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/signal.png
+-rw-rw-rw-   0        0        0      576 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/signal.scss
+-rw-rw-rw-   0        0        0     5338 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/tequila.png
+-rw-rw-rw-   0        0        0      371 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/ui/theme/themes-guide/tequila.scss
+-rw-rw-rw-   0        0        0      801 2022-09-13 04:40:48.000000 gramex-1.91.0/gramex/apps/ui/theme/themes.json
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.917569 gramex-1.91.0/gramex/apps/uifactory/
+-rw-rw-rw-   0        0        0      739 2022-11-02 08:06:14.000000 gramex-1.91.0/gramex/apps/uifactory/.eslintrc.js
+-rw-rw-rw-   0        0        0       46 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/.gitattributes
+-rw-rw-rw-   0        0        0       57 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.919462 gramex-1.91.0/gramex/apps/uifactory/assets/
+-rw-rw-rw-   0        0        0      432 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/assets/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.924991 gramex-1.91.0/gramex/apps/uifactory/assets/data/
+-rw-rw-rw-   0        0        0     1674 2022-09-13 04:40:51.000000 gramex-1.91.0/gramex/apps/uifactory/assets/data/input.json
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.936607 gramex-1.91.0/gramex/apps/uifactory/assets/img/
+-rw-rw-rw-   0        0        0      706 2022-06-23 02:35:29.000000 gramex-1.91.0/gramex/apps/uifactory/assets/img/arrows-move.svg
+-rw-rw-rw-   0        0        0      496 2022-06-23 02:35:29.000000 gramex-1.91.0/gramex/apps/uifactory/assets/img/clipboard.svg
+-rw-rw-rw-   0        0        0      978 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png
+-rw-rw-rw-   0        0        0      573 2022-06-23 02:35:29.000000 gramex-1.91.0/gramex/apps/uifactory/assets/img/trash.svg
+-rw-rw-rw-   0        0        0     6667 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/create.html
+-rw-rw-rw-   0        0        0     2673 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/edit.html
+-rw-rw-rw-   0        0        0      694 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/field-actions.html
+-rw-rw-rw-   0        0        0     4361 2022-11-06 08:24:31.000000 gramex-1.91.0/gramex/apps/uifactory/form_builder.py
+-rw-rw-rw-   0        0        0     4749 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/gramex.yaml
+-rw-rw-rw-   0        0        0     6274 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/index.html
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.965344 gramex-1.91.0/gramex/apps/uifactory/js/
+-rw-rw-rw-   0        0        0      601 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/js/README.md
+-rw-rw-rw-   0        0        0      435 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/js/embed.js
+-rw-rw-rw-   0        0        0    16411 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/js/fields.js
+-rw-rw-rw-   0        0        0     1942 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/js/fork-form.js
+-rw-rw-rw-   0        0        0     3080 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/js/index.js
+-rw-rw-rw-   0        0        0     9228 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/js/script.js
+-rw-rw-rw-   0        0        0      829 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/js/utils.js
+-rw-rw-rw-   0        0        0     2776 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/js/viewform.js
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.979380 gramex-1.91.0/gramex/apps/uifactory/modals/
+-rw-rw-rw-   0        0        0     1117 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/modals/add-field.html
+-rw-rw-rw-   0        0        0     4107 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/modals/embed.html
+-rw-rw-rw-   0        0        0      898 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/modals/remove.html
+-rw-rw-rw-   0        0        0      952 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/modals/rename.html
+-rw-rw-rw-   0        0        0     1323 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/modals/themes.html
+-rw-rw-rw-   0        0        0     5781 2023-06-08 09:15:18.000000 gramex-1.91.0/gramex/apps/uifactory/package-lock.json
+-rw-rw-rw-   0        0        0      206 2022-03-03 08:20:09.000000 gramex-1.91.0/gramex/apps/uifactory/package.json
+-rw-rw-rw-   0        0        0     1548 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/popover-form.html
+-rw-rw-rw-   0        0        0     1952 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/sample.html
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.983123 gramex-1.91.0/gramex/apps/uifactory/snippets/
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.984577 gramex-1.91.0/gramex/apps/uifactory/snippets/button/
+-rw-rw-rw-   0        0        0     2795 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/snippets/button/bs4-button.js
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.987563 gramex-1.91.0/gramex/apps/uifactory/snippets/checkbox/
+-rw-rw-rw-   0        0        0     1225 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.992092 gramex-1.91.0/gramex/apps/uifactory/snippets/email/
+-rw-rw-rw-   0        0        0      604 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/snippets/email/bs4-email.js
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.994096 gramex-1.91.0/gramex/apps/uifactory/snippets/hidden/
+-rw-rw-rw-   0        0        0      327 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/snippets/hidden/bs4-hidden.js
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.995185 gramex-1.91.0/gramex/apps/uifactory/snippets/html/
+-rw-rw-rw-   0        0        0      292 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/snippets/html/bs4-html.js
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.003508 gramex-1.91.0/gramex/apps/uifactory/snippets/multiselect/
+-rw-rw-rw-   0        0        0     4735 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.009320 gramex-1.91.0/gramex/apps/uifactory/snippets/number/
+-rw-rw-rw-   0        0        0      736 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/snippets/number/bs4-number.js
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.012601 gramex-1.91.0/gramex/apps/uifactory/snippets/password/
+-rw-rw-rw-   0        0        0      375 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/snippets/password/bs4-password.js
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.014599 gramex-1.91.0/gramex/apps/uifactory/snippets/radio/
+-rw-rw-rw-   0        0        0     1034 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/snippets/radio/bs4-radio.js
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.016738 gramex-1.91.0/gramex/apps/uifactory/snippets/range/
+-rw-rw-rw-   0        0        0      610 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/snippets/range/bs4-range.js
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.019251 gramex-1.91.0/gramex/apps/uifactory/snippets/select/
+-rw-rw-rw-   0        0        0     1617 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/snippets/select/bs4-select.js
+-rw-rw-rw-   0        0        0      946 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/snippets/setup.js
+-rw-rw-rw-   0        0        0        3 2023-04-17 10:18:07.000000 gramex-1.91.0/gramex/apps/uifactory/snippets/snippets.json
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.023772 gramex-1.91.0/gramex/apps/uifactory/snippets/text/
+-rw-rw-rw-   0        0        0      974 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/snippets/text/bs4-text.js
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.026776 gramex-1.91.0/gramex/apps/uifactory/snippets/textarea/
+-rw-rw-rw-   0        0        0     1094 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js
+-rw-rw-rw-   0        0        0     1815 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps/uifactory/style.scss
+-rw-rw-rw-   0        0        0     2013 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/template-navbar-view-form.html
+-rw-rw-rw-   0        0        0     1020 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/template-navbar.html
+-rw-rw-rw-   0        0        0      415 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/toast.html
+-rw-rw-rw-   0        0        0     6516 2022-02-19 10:03:04.000000 gramex-1.91.0/gramex/apps/uifactory/viewform.html
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.034413 gramex-1.91.0/gramex/apps/update/
+-rw-rw-rw-   0        0        0      565 2018-10-30 07:47:04.000000 gramex-1.91.0/gramex/apps/update/README.md
+-rw-rw-rw-   0        0        0     2397 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/apps/update/gramex.yaml
+-rw-rw-rw-   0        0        0     4593 2022-11-06 08:24:31.000000 gramex-1.91.0/gramex/apps/update/gramexupdate.py
+-rw-rw-rw-   0        0        0     3310 2022-03-03 08:20:09.000000 gramex-1.91.0/gramex/apps/update/index.html
+-rw-rw-rw-   0        0        0      277 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/apps.yaml
+-rw-rw-rw-   0        0        0    56842 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/cache.py
+-rw-rw-rw-   0        0        0    35221 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/config.py
+-rw-rw-rw-   0        0        0    93430 2023-05-27 08:02:09.000000 gramex-1.91.0/gramex/data.py
+-rw-rw-rw-   0        0        0     6408 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/debug.py
+-rw-rw-rw-   0        0        0     1825 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/deploy.yaml
+-rw-rw-rw-   0        0        0     1466 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/download.vega.js
+-rw-rw-rw-   0        0        0    12057 2018-10-22 05:47:08.000000 gramex-1.91.0/gramex/favicon.ico
+-rw-rw-rw-   0        0        0    16670 2023-06-08 09:04:46.000000 gramex-1.91.0/gramex/gramex.yaml
+-rw-rw-rw-   0        0        0     6262 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/gramexfeatures.csv
+-rw-rw-rw-   0        0        0    14444 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/gramexsize.csv
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.178019 gramex-1.91.0/gramex/handlers/
+-rw-rw-rw-   0        0        0     1368 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/handlers/400.html
+-rw-rw-rw-   0        0        0     2081 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/handlers/401.html
+-rw-rw-rw-   0        0        0     2483 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/handlers/403.html
+-rw-rw-rw-   0        0        0     1399 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/handlers/404.html
+-rw-rw-rw-   0        0        0     2163 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/handlers/500.html
+-rw-rw-rw-   0        0        0     2980 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/handlers/__init__.py
+-rw-rw-rw-   0        0        0      532 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/handlers/auth.recaptcha.template.html
+-rw-rw-rw-   0        0        0     3862 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/handlers/auth.template.html
+-rw-rw-rw-   0        0        0    17341 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/handlers/authhandler.py
+-rw-rw-rw-   0        0        0    63468 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/handlers/basehandler.py
+-rw-rw-rw-   0        0        0    15771 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/handlers/capturehandler.py
+-rw-rw-rw-   0        0        0     1477 2023-06-08 09:04:46.000000 gramex-1.91.0/gramex/handlers/comichandler.py
+-rw-rw-rw-   0        0        0     8904 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/handlers/drivehandler.py
+-rw-rw-rw-   0        0        0    14924 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/handlers/filehandler.py
+-rw-rw-rw-   0        0        0     1271 2022-07-03 06:28:09.000000 gramex-1.91.0/gramex/handlers/filehandler.template.html
+-rw-rw-rw-   0        0        0      198 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/handlers/filterhandler.py
+-rw-rw-rw-   0        0        0    13238 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/handlers/formhandler.py
+-rw-rw-rw-   0        0        0     3774 2023-06-08 09:04:46.000000 gramex-1.91.0/gramex/handlers/functionhandler.py
+-rw-rw-rw-   0        0        0     6706 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/handlers/jsonhandler.py
+-rw-rw-rw-   0        0        0     6838 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/handlers/messagehandler.py
+-rw-rw-rw-   0        0        0    16154 2023-06-02 05:59:12.000000 gramex-1.91.0/gramex/handlers/mlhandler.py
+-rw-rw-rw-   0        0        0     7492 2023-06-08 09:04:46.000000 gramex-1.91.0/gramex/handlers/modelhandler.py
+-rw-rw-rw-   0        0        0     1413 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/handlers/openapiconfig.yaml
+-rw-rw-rw-   0        0        0     7193 2023-06-08 09:04:46.000000 gramex-1.91.0/gramex/handlers/openapihandler.py
+-rw-rw-rw-   0        0        0      818 2023-06-08 09:04:46.000000 gramex-1.91.0/gramex/handlers/pptxhandler.py
+-rw-rw-rw-   0        0        0     5145 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/handlers/processhandler.py
+-rw-rw-rw-   0        0        0     7882 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/handlers/proxyhandler.py
+-rw-rw-rw-   0        0        0     1362 2022-10-17 06:55:24.000000 gramex-1.91.0/gramex/handlers/queryhandler.template.html
+-rw-rw-rw-   0        0        0    11338 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/handlers/socialhandler.py
+-rw-rw-rw-   0        0        0     9434 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/handlers/uploadhandler.py
+-rw-rw-rw-   0        0        0     2121 2022-11-23 03:19:45.000000 gramex-1.91.0/gramex/handlers/websockethandler.py
+-rw-rw-rw-   0        0        0     1458 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/http.py
+-rw-rw-rw-   0        0        0    35069 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/install.py
+-rw-rw-rw-   0        0        0     2086 2022-09-13 04:40:51.000000 gramex-1.91.0/gramex/license.py
+-rw-rw-rw-   0        0        0     2005 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/migrate.py
+-rw-rw-rw-   0        0        0    18629 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/ml.py
+-rw-rw-rw-   0        0        0    13687 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/ml_api.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.211088 gramex-1.91.0/gramex/pptgen/
+-rw-rw-rw-   0        0        0     9967 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/pptgen/__init__.py
+-rw-rw-rw-   0        0        0    18868 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/pptgen/color.py
+-rw-rw-rw-   0        0        0     7779 2018-01-31 16:40:23.000000 gramex-1.91.0/gramex/pptgen/colors.json
+-rw-rw-rw-   0        0        0    45490 2022-11-02 08:06:17.000000 gramex-1.91.0/gramex/pptgen/commands.py
+-rw-rw-rw-   0        0        0     6351 2018-01-31 16:40:23.000000 gramex-1.91.0/gramex/pptgen/fonts.json
+-rw-rw-rw-   0        0        0     1304 2022-11-02 08:06:18.000000 gramex-1.91.0/gramex/pptgen/fontwidth.py
+-rw-rw-rw-   0        0        0    26250 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/pptgen/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.220340 gramex-1.91.0/gramex/pptgen2/
+-rw-rw-rw-   0        0        0    23438 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/pptgen2/__init__.py
+-rw-rw-rw-   0        0        0    34432 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/pptgen2/commands.py
+-rw-rw-rw-   0        0        0    12068 2022-11-02 08:06:18.000000 gramex-1.91.0/gramex/pptgen2/config.yaml
+-rw-rw-rw-   0        0        0     4278 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/pynode.py
+-rw-rw-rw-   0        0        0     2979 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/scale.py
+-rw-rw-rw-   0        0        0     1057 2022-11-02 08:06:18.000000 gramex-1.91.0/gramex/secrets.py
+-rw-rw-rw-   0        0        0     2508 2022-11-02 08:06:18.000000 gramex-1.91.0/gramex/servicenow.yaml
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.350418 gramex-1.91.0/gramex/services/
+-rw-rw-rw-   0        0        0    39443 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/services/__init__.py
+-rw-rw-rw-   0        0        0    11176 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/services/emailer.py
+-rw-rw-rw-   0        0        0     3681 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/services/rediscache.py
+-rw-rw-rw-   0        0        0     7164 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/services/scheduler.py
+-rw-rw-rw-   0        0        0     3684 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/services/sms.py
+-rw-rw-rw-   0        0        0     6385 2023-05-13 04:30:57.000000 gramex-1.91.0/gramex/services/ttlcache.py
+-rw-rw-rw-   0        0        0     4521 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/services/urlcache.py
+-rw-rw-rw-   0        0        0     5822 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/services/watcher.py
+-rw-rw-rw-   0        0        0     3831 2022-11-02 08:06:18.000000 gramex-1.91.0/gramex/sm_api.py
+-rw-rw-rw-   0        0        0     8638 2022-11-02 08:06:18.000000 gramex-1.91.0/gramex/topcause.py
+-rw-rw-rw-   0        0        0     8710 2022-11-02 08:06:18.000000 gramex-1.91.0/gramex/transformers.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.396434 gramex-1.91.0/gramex/transforms/
+-rw-rw-rw-   0        0        0      777 2023-04-14 07:12:43.000000 gramex-1.91.0/gramex/transforms/__init__.py
+-rw-rw-rw-   0        0        0     1658 2022-09-13 04:40:51.000000 gramex-1.91.0/gramex/transforms/auth.py
+-rw-rw-rw-   0        0        0     3542 2022-11-02 08:06:18.000000 gramex-1.91.0/gramex/transforms/template.py
+-rw-rw-rw-   0        0        0    32280 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/transforms/transforms.py
+-rw-rw-rw-   0        0        0    10095 2023-06-08 09:27:24.000000 gramex-1.91.0/gramex/transforms/twitterstream.py
+-rw-rw-rw-   0        0        0     6808 2022-11-13 04:18:56.000000 gramex-1.91.0/gramex/winservice.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:37.213174 gramex-1.91.0/gramex.egg-info/
+-rw-rw-rw-   0        0        0     2956 2023-06-08 09:28:33.000000 gramex-1.91.0/gramex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11970 2023-06-08 09:28:37.000000 gramex-1.91.0/gramex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 09:28:33.000000 gramex-1.91.0/gramex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-06-08 09:28:33.000000 gramex-1.91.0/gramex.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      953 2023-06-08 09:28:33.000000 gramex-1.91.0/gramex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-08 09:28:33.000000 gramex-1.91.0/gramex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6123 2023-06-08 09:27:24.000000 gramex-1.91.0/pyproject.toml
+-rw-rw-rw-   0        0        0      540 2023-06-08 09:28:38.579324 gramex-1.91.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-08 09:28:38.566196 gramex-1.91.0/tests/
+-rw-rw-rw-   0        0        0     5233 2022-11-06 08:24:18.000000 gramex-1.91.0/tests/test_admin.py
+-rw-rw-rw-   0        0        0     9054 2023-04-18 08:45:54.000000 gramex-1.91.0/tests/test_alerts.py
+-rw-rw-rw-   0        0        0     3981 2022-11-06 08:24:18.000000 gramex-1.91.0/tests/test_args.py
+-rw-rw-rw-   0        0        0    39027 2023-06-08 09:04:47.000000 gramex-1.91.0/tests/test_auth.py
+-rw-rw-rw-   0        0        0    14612 2022-11-06 08:24:18.000000 gramex-1.91.0/tests/test_cache.py
+-rw-rw-rw-   0        0        0    15062 2023-05-13 04:30:57.000000 gramex-1.91.0/tests/test_capturehandler.py
+-rw-rw-rw-   0        0        0     1288 2022-11-06 08:24:19.000000 gramex-1.91.0/tests/test_comichandler.py
+-rw-rw-rw-   0        0        0    11152 2022-11-06 08:24:20.000000 gramex-1.91.0/tests/test_drivehandler.py
+-rw-rw-rw-   0        0        0    17841 2022-11-06 08:24:20.000000 gramex-1.91.0/tests/test_filehandler.py
+-rw-rw-rw-   0        0        0     6797 2023-05-13 04:30:57.000000 gramex-1.91.0/tests/test_filterhandler.py
+-rw-rw-rw-   0        0        0    35746 2023-05-27 08:02:33.000000 gramex-1.91.0/tests/test_formhandler.py
+-rw-rw-rw-   0        0        0     8784 2022-11-06 08:24:22.000000 gramex-1.91.0/tests/test_functionhandler.py
+-rw-rw-rw-   0        0        0     3201 2022-11-06 08:24:22.000000 gramex-1.91.0/tests/test_gramexlog.py
+-rw-rw-rw-   0        0        0    18143 2023-06-08 09:27:24.000000 gramex-1.91.0/tests/test_handlers.py
+-rw-rw-rw-   0        0        0     1475 2022-11-02 08:06:18.000000 gramex-1.91.0/tests/test_init.py
+-rw-rw-rw-   0        0        0     8931 2023-05-13 04:30:57.000000 gramex-1.91.0/tests/test_install.py
+-rw-rw-rw-   0        0        0     6361 2022-11-06 08:24:23.000000 gramex-1.91.0/tests/test_jsonhandler.py
+-rw-rw-rw-   0        0        0     3896 2022-11-06 08:24:23.000000 gramex-1.91.0/tests/test_ldapauth.py
+-rw-rw-rw-   0        0        0     7519 2022-11-02 08:06:18.000000 gramex-1.91.0/tests/test_logviewer.py
+-rw-rw-rw-   0        0        0    32878 2022-11-23 04:49:14.000000 gramex-1.91.0/tests/test_mlhandler.py
+-rw-rw-rw-   0        0        0     4745 2022-11-02 08:06:18.000000 gramex-1.91.0/tests/test_modelhandler.py
+-rw-rw-rw-   0        0        0     7082 2023-05-13 04:30:57.000000 gramex-1.91.0/tests/test_openapihandler.py
+-rw-rw-rw-   0        0        0     1411 2022-11-02 08:06:18.000000 gramex-1.91.0/tests/test_pptxhandler.py
+-rw-rw-rw-   0        0        0     3530 2022-11-06 08:24:24.000000 gramex-1.91.0/tests/test_processhandler.py
+-rw-rw-rw-   0        0        0     3834 2022-11-06 08:24:24.000000 gramex-1.91.0/tests/test_proxyhandler.py
+-rw-rw-rw-   0        0        0     1527 2022-11-02 08:06:18.000000 gramex-1.91.0/tests/test_pynode.py
+-rw-rw-rw-   0        0        0     1220 2022-11-06 08:24:24.000000 gramex-1.91.0/tests/test_schedule.py
+-rw-rw-rw-   0        0        0      757 2022-02-19 10:03:06.000000 gramex-1.91.0/tests/test_secrets.py
+-rw-rw-rw-   0        0        0      330 2020-05-27 03:04:19.000000 gramex-1.91.0/tests/test_sms.py
+-rw-rw-rw-   0        0        0      180 2017-08-29 07:52:03.000000 gramex-1.91.0/tests/test_subapp.py
+-rw-rw-rw-   0        0        0     5382 2022-11-02 08:06:18.000000 gramex-1.91.0/tests/test_subprocess.py
+-rw-rw-rw-   0        0        0     2277 2022-11-02 08:06:18.000000 gramex-1.91.0/tests/test_translater.py
+-rw-rw-rw-   0        0        0     2895 2022-11-06 08:24:24.000000 gramex-1.91.0/tests/test_twitterresthandler.py
+-rw-rw-rw-   0        0        0     2352 2022-11-06 08:24:24.000000 gramex-1.91.0/tests/test_ui.py
+-rw-rw-rw-   0        0        0     2359 2022-11-02 08:06:18.000000 gramex-1.91.0/tests/test_update.py
+-rw-rw-rw-   0        0        0     6563 2022-11-06 08:24:25.000000 gramex-1.91.0/tests/test_uploadhandler.py
+-rw-rw-rw-   0        0        0     1966 2022-11-02 08:06:18.000000 gramex-1.91.0/tests/test_watcher.py
+-rw-rw-rw-   0        0        0     2647 2022-11-06 08:24:25.000000 gramex-1.91.0/tests/test_websockethandler.py
```

### Comparing `gramex-1.90.0/.gitignore` & `gramex-1.91.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 tests/*.pkl
 testlib/**/gen.*
 testlib/**/*.temp.*
 tests/*.db
 tests/uploads/
 tests/drive/
 tests/watcher.txt
+# Ignore pytest/messages.db, etc. generated by pytest.
+pytest/*.db
+
 
 # Don't commit data files, except what's required for testing or by Gramex apps
 *.csv
 *.xls*
 
 !reports/*.csv
 !tests/**/*.csv
```

### Comparing `gramex-1.90.0/LICENSE` & `gramex-1.91.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/MANIFEST.in` & `gramex-1.91.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/PKG-INFO` & `gramex-1.91.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramex
-Version: 1.90.0
+Version: 1.91.0
 Summary: Gramex: Low Code Data Solutions Platform
 Author-email: Anand S <s.anand@gramener.com>, Pratap Vardhan <pratapapvr@gmail.com>, Jaidev Deshpande <jaidev.deshpande@gramener.com>, Bhanu Kamapantula <talk2kish@gmail.com>, Radheya Kale <radheya.kale@gramener.com>, Karmanya Aggarwal <karmanyaaggarwal@gmail.com>, Sandeep Bhat <sandeep.bhat@gramener.com>, Shraddheya Shrivastava <shraddheya.shrivastava@gramener.com>, Sundeep Reddy Mallu <sundeep.mally@gramener.com>
 License: MIT
 Project-URL: Homepage, https://gramener.com/gramex/
 Project-URL: Documentation, https://gramener.com/gramex/guide/
 Project-URL: Repository, https://github.com/gramener/gramex
 Project-URL: Changelog, https://gramener.com/gramex/guide/release/
```

### Comparing `gramex-1.90.0/README.md` & `gramex-1.91.0/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/__init__.py` & `gramex-1.91.0/gramex/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 gramex install                Install an app
 gramex update                 Update an app
 gramex setup                  Run make, npm install, bower install etc on app
 gramex run                    Run an installed app
 gramex uninstall              Uninstall an app
 '''
 
-__version__ = '1.90.0'
+__version__ = '1.91.0'
 
 paths = AttrDict()  # Paths where configurations are stored
 conf = AttrDict()  # Final merged configurations
 config_layers = ChainConfig()  # Loads all configurations. init() updates it
 appconfig = AttrDict()  # Final app configuration
 
 paths['source'] = Path(__file__).absolute().parent  # Where gramex source code is
```

### Comparing `gramex-1.90.0/gramex/apps/admin2/gramex.yaml` & `gramex-1.91.0/gramex/apps/admin2/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/admin2/gramexadmin.py` & `gramex-1.91.0/gramex/apps/admin2/gramexadmin.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/admin2/index.html` & `gramex-1.91.0/gramex/apps/admin2/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/admin2/schedule.js` & `gramex-1.91.0/gramex/apps/admin2/schedule.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/capture/README.md` & `gramex-1.91.0/gramex/apps/capture/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/capture/capture.js` & `gramex-1.91.0/gramex/apps/capture/capture.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/capture/chromecapture.js` & `gramex-1.91.0/gramex/apps/capture/chromecapture.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -72,14 +72,15 @@
         .split("|")
         .map((v) => `<span>${v}</span>`)
         .join("");
 }
 
 const browser_setup = async (args) => {
     browser = await puppeteer.launch({
+        headless: "new",
         args: args
     });
     browser.on("disconnected", () => {
         console.log("Reconnecting browser");
         browser.close();
         browser_setup(args);
     });
```

### Comparing `gramex-1.90.0/gramex/apps/capture/index.html` & `gramex-1.91.0/gramex/apps/capture/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/capture/package-lock.json` & `gramex-1.91.0/gramex/apps/capture/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987836104269293%*

 * *Differences: {"'dependencies'": "{'@types/node': {'version': '20.2.5', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@types/node/-/node-20.2.5.tgz', 'integrity': "*

 * *                   "'sha512-JJulVEQXmiY9Px5axXHeYGLSjhkZEnD+MDPDGbCbIAbMslkKwmygtZFy1X6s/075Yo94sf8GuSlFfPzysQrWZQ=='}, "*

 * *                   "'get-intrinsic': {'version': '1.2.1', 'resolved': "*

 * *                   "'https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.1.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha […]*

```diff
@@ -50,18 +50,18 @@
                 "unbzip2-stream": "1.4.3",
                 "yargs": "17.7.1"
             },
             "resolved": "https://registry.npmjs.org/@puppeteer/browsers/-/browsers-0.5.0.tgz",
             "version": "0.5.0"
         },
         "@types/node": {
-            "integrity": "sha512-O+z53uwx64xY7D6roOi4+jApDGFg0qn6WHcxe5QeqjMaTezBO/mxdfFXIVAVVyNWKx84OmPB3L8kbVYOTeN34A==",
+            "integrity": "sha512-JJulVEQXmiY9Px5axXHeYGLSjhkZEnD+MDPDGbCbIAbMslkKwmygtZFy1X6s/075Yo94sf8GuSlFfPzysQrWZQ==",
             "optional": true,
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.1.0.tgz",
-            "version": "20.1.0"
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.2.5.tgz",
+            "version": "20.2.5"
         },
         "@types/yauzl": {
             "integrity": "sha512-Cn6WYCm0tXv8p6k+A8PvbDG763EDpBoTzHdA+Q/MF6H3sapGjCm9NzoaJncJS9tUKSuCoDs9XHxYYsQDgxR6kw==",
             "optional": true,
             "requires": {
                 "@types/node": "*"
             },
@@ -616,22 +616,23 @@
         },
         "get-caller-file": {
             "integrity": "sha512-DyFP3BM/3YHTQOCUL/w0OZHR0lpKeGrxotcHWcqNEdnltqFwXVfhEBQ94eIo34AfQpo0rGki4cyIiftY06h2Fg==",
             "resolved": "https://registry.npmjs.org/get-caller-file/-/get-caller-file-2.0.5.tgz",
             "version": "2.0.5"
         },
         "get-intrinsic": {
-            "integrity": "sha512-L049y6nFOuom5wGyRc3/gdTLO94dySVKRACj1RmJZBQXlbTMhtNIgkWkUHq+jYmZvKf14EW1EoJnnjbmoHij0Q==",
+            "integrity": "sha512-2DcsyfABl+gVHEfCOaTrWgyt+tb6MSEGmKq+kI5HwLbIYgjgmMcV8KQ41uaKz1xxUcn9tJtgFbQUEVcEbd0FYw==",
             "requires": {
                 "function-bind": "^1.1.1",
                 "has": "^1.0.3",
+                "has-proto": "^1.0.1",
                 "has-symbols": "^1.0.3"
             },
-            "resolved": "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.0.tgz",
-            "version": "1.2.0"
+            "resolved": "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.1.tgz",
+            "version": "1.2.1"
         },
         "get-stream": {
             "integrity": "sha512-nBF+F1rAZVCu/p7rjzgA+Yb4lfYXrpl7a6VmJrU8wF9I1CKvP/QwPNZHnOlwbTkY6dvtFIzFMSyQXbLoTQPRpA==",
             "requires": {
                 "pump": "^3.0.0"
             },
             "resolved": "https://registry.npmjs.org/get-stream/-/get-stream-5.2.0.tgz",
@@ -664,14 +665,19 @@
             "version": "1.0.3"
         },
         "has-flag": {
             "integrity": "sha512-sKJf1+ceQBr4SMkvQnBDNDtf4TXpVhVGateu0t918bl30FnbE2m4vNLX+VWe/dpjlb+HugGYzW7uQXH98HPEYw==",
             "resolved": "https://registry.npmjs.org/has-flag/-/has-flag-3.0.0.tgz",
             "version": "3.0.0"
         },
+        "has-proto": {
+            "integrity": "sha512-7qE+iP+O+bgF9clE5+UoBFzE65mlBiVj3tKCrlNQ0Ogwm0BjpT/gK4SlLYDMybDh5I3TCTKnPPa0oMG7JDYrhg==",
+            "resolved": "https://registry.npmjs.org/has-proto/-/has-proto-1.0.1.tgz",
+            "version": "1.0.1"
+        },
         "has-symbols": {
             "integrity": "sha512-l3LCuF6MgDNwTDKkdYGEihYjt5pRPbEg46rtlmnSPlUbgmB8LOIrKJbYYFBSbnPaJexMKtiPO8hmeRjRz2Td+A==",
             "resolved": "https://registry.npmjs.org/has-symbols/-/has-symbols-1.0.3.tgz",
             "version": "1.0.3"
         },
         "http-errors": {
             "integrity": "sha512-FtwrG/euBzaEjYeRqOgly7G0qviiXoJWnvEH2Z1plBdXgbyjv34pHTSb9zoeHMyDy33+DWy5Wt9Wo+TURtOYSQ==",
@@ -1626,18 +1632,18 @@
         },
         "node_modules/@puppeteer/browsers/node_modules/ms": {
             "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
             "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
             "version": "2.1.2"
         },
         "node_modules/@types/node": {
-            "integrity": "sha512-O+z53uwx64xY7D6roOi4+jApDGFg0qn6WHcxe5QeqjMaTezBO/mxdfFXIVAVVyNWKx84OmPB3L8kbVYOTeN34A==",
+            "integrity": "sha512-JJulVEQXmiY9Px5axXHeYGLSjhkZEnD+MDPDGbCbIAbMslkKwmygtZFy1X6s/075Yo94sf8GuSlFfPzysQrWZQ==",
             "optional": true,
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.1.0.tgz",
-            "version": "20.1.0"
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.2.5.tgz",
+            "version": "20.2.5"
         },
         "node_modules/@types/yauzl": {
             "dependencies": {
                 "@types/node": "*"
             },
             "integrity": "sha512-Cn6WYCm0tXv8p6k+A8PvbDG763EDpBoTzHdA+Q/MF6H3sapGjCm9NzoaJncJS9tUKSuCoDs9XHxYYsQDgxR6kw==",
             "optional": true,
@@ -2350,22 +2356,23 @@
             "resolved": "https://registry.npmjs.org/get-caller-file/-/get-caller-file-2.0.5.tgz",
             "version": "2.0.5"
         },
         "node_modules/get-intrinsic": {
             "dependencies": {
                 "function-bind": "^1.1.1",
                 "has": "^1.0.3",
+                "has-proto": "^1.0.1",
                 "has-symbols": "^1.0.3"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-L049y6nFOuom5wGyRc3/gdTLO94dySVKRACj1RmJZBQXlbTMhtNIgkWkUHq+jYmZvKf14EW1EoJnnjbmoHij0Q==",
-            "resolved": "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.0.tgz",
-            "version": "1.2.0"
+            "integrity": "sha512-2DcsyfABl+gVHEfCOaTrWgyt+tb6MSEGmKq+kI5HwLbIYgjgmMcV8KQ41uaKz1xxUcn9tJtgFbQUEVcEbd0FYw==",
+            "resolved": "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.1.tgz",
+            "version": "1.2.1"
         },
         "node_modules/get-stream": {
             "dependencies": {
                 "pump": "^3.0.0"
             },
             "engines": {
                 "node": ">=8"
@@ -2416,14 +2423,25 @@
             "engines": {
                 "node": ">=4"
             },
             "integrity": "sha512-sKJf1+ceQBr4SMkvQnBDNDtf4TXpVhVGateu0t918bl30FnbE2m4vNLX+VWe/dpjlb+HugGYzW7uQXH98HPEYw==",
             "resolved": "https://registry.npmjs.org/has-flag/-/has-flag-3.0.0.tgz",
             "version": "3.0.0"
         },
+        "node_modules/has-proto": {
+            "engines": {
+                "node": ">= 0.4"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/ljharb"
+            },
+            "integrity": "sha512-7qE+iP+O+bgF9clE5+UoBFzE65mlBiVj3tKCrlNQ0Ogwm0BjpT/gK4SlLYDMybDh5I3TCTKnPPa0oMG7JDYrhg==",
+            "resolved": "https://registry.npmjs.org/has-proto/-/has-proto-1.0.1.tgz",
+            "version": "1.0.1"
+        },
         "node_modules/has-symbols": {
             "engines": {
                 "node": ">= 0.4"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
```

### Comparing `gramex-1.90.0/gramex/apps/capture/package.json` & `gramex-1.91.0/gramex/apps/capture/package.json`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/filemanager/README.html` & `gramex-1.91.0/gramex/apps/filemanager/README.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/filemanager/drivehandler-snippet.html` & `gramex-1.91.0/gramex/apps/filemanager/drivehandler-snippet.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/filemanager/filemanager-snippet.html` & `gramex-1.91.0/gramex/apps/filemanager/filemanager-snippet.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/filemanager/filemanager.html` & `gramex-1.91.0/gramex/apps/filemanager/filemanager.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/filemanager/filemanager.js` & `gramex-1.91.0/gramex/apps/filemanager/filemanager.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/filemanager/filemanager.py` & `gramex-1.91.0/gramex/apps/filemanager/filemanager.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/filemanager/gramex.yaml` & `gramex-1.91.0/gramex/apps/filemanager/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/filemanager/index.html` & `gramex-1.91.0/gramex/apps/filemanager/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/filemanager/navbar.html` & `gramex-1.91.0/gramex/apps/filemanager/navbar.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/init/default/.eslintrc.yml` & `gramex-1.91.0/gramex/apps/init/default/.eslintrc.yml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/init/default/.gitlab-ci.yml` & `gramex-1.91.0/gramex/apps/init/default/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/init/default/.template.gitignore` & `gramex-1.91.0/gramex/apps/init/default/.template.gitignore`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/init/default/assets/README.template.md` & `gramex-1.91.0/gramex/apps/init/default/assets/README.template.md`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/init/default/gramex.template.yaml` & `gramex-1.91.0/gramex/apps/init/default/gramex.template.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/init/default/index.template.html` & `gramex-1.91.0/gramex/apps/init/default/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/init/default/js/README.template.md` & `gramex-1.91.0/gramex/apps/init/default/js/README.template.md`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/init/default/login.template.html` & `gramex-1.91.0/gramex/apps/init/default/login.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/init/default/template-navbar.template.html` & `gramex-1.91.0/gramex/apps/init/default/template-navbar.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/init/ide/index.template.html` & `gramex-1.91.0/gramex/apps/init/ide/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/init/minimal/index.template.html` & `gramex-1.91.0/gramex/apps/init/minimal/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/languagetool/README.md` & `gramex-1.91.0/gramex/apps/languagetool/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/languagetool/gramex.yaml` & `gramex-1.91.0/gramex/apps/languagetool/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/logviewer/config.yaml` & `gramex-1.91.0/gramex/apps/logviewer/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/logviewer/gramex.yaml` & `gramex-1.91.0/gramex/apps/logviewer/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/logviewer/index.html` & `gramex-1.91.0/gramex/apps/logviewer/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/logviewer/logviewer.py` & `gramex-1.91.0/gramex/apps/logviewer/logviewer.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/logviewer/lv-datepicker.html` & `gramex-1.91.0/gramex/apps/logviewer/lv-datepicker.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/logviewer/package-lock.json` & `gramex-1.91.0/gramex/apps/logviewer/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/logviewer/render.js` & `gramex-1.91.0/gramex/apps/logviewer/render.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/logviewer/script.js` & `gramex-1.91.0/gramex/apps/logviewer/script.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/mail/index.html` & `gramex-1.91.0/gramex/apps/mail/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/mlhandler/template.html` & `gramex-1.91.0/gramex/apps/mlhandler/template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/pynode/index.js` & `gramex-1.91.0/gramex/apps/pynode/index.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/pynode/package-lock.json` & `gramex-1.91.0/gramex/apps/pynode/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/.snyk` & `gramex-1.91.0/gramex/apps/ui/.snyk`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/__init__.py` & `gramex-1.91.0/gramex/apps/ui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,20 +131,18 @@
 ) -> bytes:
     '''Compile a SASS file using custom variables from URL query parameters.
 
     Examples:
         >>> sass2(handler, 'x.sass')
 
     Parameters:
-
         handler: the[FileHandler][gramex.handlers.FileHandler] serving this file
         path: absolute path of input SASS file to compile into CSS
 
     Returns:
-
         compiled CSS file or source map if ?_map is specified
 
     URL query parameters in `handler.args` are converted into SASS variables.
     For example, `?primary=red` becomes `primary: red;` at the start of the SASS file.
 
     You can specify
     [`?@import=`](https://sass-lang.com/documentation/at-rules/import),
@@ -232,26 +230,24 @@
 
     Examples:
         >>> jscompiler(
         ...     handler, path='x.ts', target_ext='.js', exe='/path/to/tsc',
         ...     cmd='node $exe $filename --outDir $targetDir --sourceMap')
 
     Parameters:
-
         handler: the[FileHandler][gramex.handlers.FileHandler] serving this file
         path: absolute path of input file to compile into JavaScript
         target_ext: extension of output file (e.g. `.js`, `.min.js`)
         exe: path to the compiler's JS executable (e.g. `/path/to/tsc`)
         cmd: command line to run. This substitutes 3 variables:
             - `$exe` for the `exe` parameter
             - `$filename` for the absolute path to the input file
             - `$targetDir` for the absolute path to the output directory
 
     Returns:
-
         compiled JS file or source map if ?_map is specified
     '''
     # Get valid variables from URL query parameters
     # Create cache key based on state = path. Output to <cache-key>.js
     path = os.path.normpath(path).replace('\\', '/')
     ext = os.path.splitext(path)[-1]
     cache_key = _get_cache_key([path])
@@ -290,21 +286,19 @@
 def _sourcemap(handler: gramex.handlers.FileHandler, target: str, mime: str) -> bytes:
     '''Returns the compiled target file OR the source map if ?_map is set.
 
     Examples:
         >>> _sourcemap(handler, 'output.js', 'text/javascript')
 
     Parameters:
-
         handler: the [FileHandler][gramex.handlers.FileHandler] serving this file
         target: absolute path of compiled output
         mime: MIME type of compiled output
 
     Returns:
-
         source map or target file contents
 
     This is used by FileHandlers compiling Vue, TS, SASS, etc.
 
     If the URL has a ?_map, it serves `{target}.map` as a JSON file.
     Else it serves the `{target}` as `mime` type,
     replacing `sourceMappingURL` with the current URL + `?_map`.
```

### Comparing `gramex-1.90.0/gramex/apps/ui/bootstrap-theme.scss` & `gramex-1.91.0/gramex/apps/ui/bootstrap-theme.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/config.yaml` & `gramex-1.91.0/gramex/apps/ui/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/gramex.yaml` & `gramex-1.91.0/gramex/apps/ui/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/gramexui.scss` & `gramex-1.91.0/gramex/apps/ui/gramexui.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/package-lock.json` & `gramex-1.91.0/gramex/apps/ui/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962225089442797%*

 * *Differences: {"'dependencies'": "{'@babel/compat-data': {'version': '7.22.3', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@babel/compat-data/-/compat-data-7.22.3.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-aNtko9OPOwVESUFp3MZfD8Uzxl7JzSeJpd7npIoxCasU37PFbAQRpKglkaKwlHOyeJdrREpo8TW8ldrkYWwvIQ=='}, "*

 * *                   "'@babel/core': {'version': '7.22.1', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@babel/core/-/core-7.22.1.tgz', 'integrity': "*

 * *               […]*

```diff
@@ -25,70 +25,70 @@
             "requires": {
                 "@babel/highlight": "^7.18.6"
             },
             "resolved": "https://registry.npmjs.org/@babel/code-frame/-/code-frame-7.21.4.tgz",
             "version": "7.21.4"
         },
         "@babel/compat-data": {
-            "integrity": "sha512-KYMqFYTaenzMK4yUtf4EW9wc4N9ef80FsbMtkwool5zpwl4YrT1SdWYSTRcT94KO4hannogdS+LxY7L+arP3gA==",
-            "resolved": "https://registry.npmjs.org/@babel/compat-data/-/compat-data-7.21.7.tgz",
-            "version": "7.21.7"
+            "integrity": "sha512-aNtko9OPOwVESUFp3MZfD8Uzxl7JzSeJpd7npIoxCasU37PFbAQRpKglkaKwlHOyeJdrREpo8TW8ldrkYWwvIQ==",
+            "resolved": "https://registry.npmjs.org/@babel/compat-data/-/compat-data-7.22.3.tgz",
+            "version": "7.22.3"
         },
         "@babel/core": {
-            "integrity": "sha512-YeM22Sondbo523Sz0+CirSPnbj9bG3P0CdHcBZdqUuaeOaYEFbOLoGU7lebvGP6P5J/WE9wOn7u7C4J9HvS1xQ==",
+            "integrity": "sha512-Hkqu7J4ynysSXxmAahpN1jjRwVJ+NdpraFLIWflgjpVob3KNyK3/tIUc7Q7szed8WMp0JNa7Qtd1E9Oo22F9gA==",
             "peer": true,
             "requires": {
                 "@ampproject/remapping": "^2.2.0",
                 "@babel/code-frame": "^7.21.4",
-                "@babel/generator": "^7.21.5",
-                "@babel/helper-compilation-targets": "^7.21.5",
-                "@babel/helper-module-transforms": "^7.21.5",
-                "@babel/helpers": "^7.21.5",
-                "@babel/parser": "^7.21.8",
-                "@babel/template": "^7.20.7",
-                "@babel/traverse": "^7.21.5",
-                "@babel/types": "^7.21.5",
+                "@babel/generator": "^7.22.0",
+                "@babel/helper-compilation-targets": "^7.22.1",
+                "@babel/helper-module-transforms": "^7.22.1",
+                "@babel/helpers": "^7.22.0",
+                "@babel/parser": "^7.22.0",
+                "@babel/template": "^7.21.9",
+                "@babel/traverse": "^7.22.1",
+                "@babel/types": "^7.22.0",
                 "convert-source-map": "^1.7.0",
                 "debug": "^4.1.0",
                 "gensync": "^1.0.0-beta.2",
                 "json5": "^2.2.2",
                 "semver": "^6.3.0"
             },
-            "resolved": "https://registry.npmjs.org/@babel/core/-/core-7.21.8.tgz",
-            "version": "7.21.8"
+            "resolved": "https://registry.npmjs.org/@babel/core/-/core-7.22.1.tgz",
+            "version": "7.22.1"
         },
         "@babel/generator": {
-            "integrity": "sha512-SrKK/sRv8GesIW1bDagf9cCG38IOMYZusoe1dfg0D8aiUe3Amvoj1QtjTPAWcfrZFvIwlleLb0gxzQidL9w14w==",
+            "integrity": "sha512-C17MW4wlk//ES/CJDL51kPNwl+qiBQyN7b9SKyVp11BLGFeSPoVaHrv+MNt8jwQFhQWowW88z1eeBx3pFz9v8A==",
             "peer": true,
             "requires": {
-                "@babel/types": "^7.21.5",
+                "@babel/types": "^7.22.3",
                 "@jridgewell/gen-mapping": "^0.3.2",
                 "@jridgewell/trace-mapping": "^0.3.17",
                 "jsesc": "^2.5.1"
             },
-            "resolved": "https://registry.npmjs.org/@babel/generator/-/generator-7.21.5.tgz",
-            "version": "7.21.5"
+            "resolved": "https://registry.npmjs.org/@babel/generator/-/generator-7.22.3.tgz",
+            "version": "7.22.3"
         },
         "@babel/helper-compilation-targets": {
-            "integrity": "sha512-1RkbFGUKex4lvsB9yhIfWltJM5cZKUftB2eNajaDv3dCMEp49iBG0K14uH8NnX9IPux2+mK7JGEOB0jn48/J6w==",
+            "integrity": "sha512-Rqx13UM3yVB5q0D/KwQ8+SPfX/+Rnsy1Lw1k/UwOC4KC6qrzIQoY3lYnBu5EHKBlEHHcj0M0W8ltPSkD8rqfsQ==",
             "requires": {
-                "@babel/compat-data": "^7.21.5",
+                "@babel/compat-data": "^7.22.0",
                 "@babel/helper-validator-option": "^7.21.0",
                 "browserslist": "^4.21.3",
                 "lru-cache": "^5.1.1",
                 "semver": "^6.3.0"
             },
-            "resolved": "https://registry.npmjs.org/@babel/helper-compilation-targets/-/helper-compilation-targets-7.21.5.tgz",
-            "version": "7.21.5"
+            "resolved": "https://registry.npmjs.org/@babel/helper-compilation-targets/-/helper-compilation-targets-7.22.1.tgz",
+            "version": "7.22.1"
         },
         "@babel/helper-environment-visitor": {
-            "integrity": "sha512-IYl4gZ3ETsWocUWgsFZLM5i1BYx9SoemminVEXadgLBa9TdeorzgLKm8wWLA6J1N/kT3Kch8XIk1laNzYoHKvQ==",
+            "integrity": "sha512-Z2tgopurB/kTbidvzeBrc2To3PUP/9i5MUe+fU6QJCQDyPwSH2oRapkLw3KGECDYSjhQZCNxEvNvZlLw8JjGwA==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/helper-environment-visitor/-/helper-environment-visitor-7.21.5.tgz",
-            "version": "7.21.5"
+            "resolved": "https://registry.npmjs.org/@babel/helper-environment-visitor/-/helper-environment-visitor-7.22.1.tgz",
+            "version": "7.22.1"
         },
         "@babel/helper-function-name": {
             "integrity": "sha512-HfK1aMRanKHpxemaY2gqBmL04iAPOPRj7DxtNbiDOrJK+gdwkiNRVpCpUJYbUT+aZyemKN8brqTOxzCaG6ExRg==",
             "peer": true,
             "requires": {
                 "@babel/template": "^7.20.7",
                 "@babel/types": "^7.21.0"
@@ -111,28 +111,28 @@
             "requires": {
                 "@babel/types": "^7.21.4"
             },
             "resolved": "https://registry.npmjs.org/@babel/helper-module-imports/-/helper-module-imports-7.21.4.tgz",
             "version": "7.21.4"
         },
         "@babel/helper-module-transforms": {
-            "integrity": "sha512-bI2Z9zBGY2q5yMHoBvJ2a9iX3ZOAzJPm7Q8Yz6YeoUjU/Cvhmi2G4QyTNyPBqqXSgTjUxRg3L0xV45HvkNWWBw==",
+            "integrity": "sha512-dxAe9E7ySDGbQdCVOY/4+UcD8M9ZFqZcZhSPsPacvCG4M+9lwtDDQfI2EoaSvmf7W/8yCBkGU0m7Pvt1ru3UZw==",
             "peer": true,
             "requires": {
-                "@babel/helper-environment-visitor": "^7.21.5",
+                "@babel/helper-environment-visitor": "^7.22.1",
                 "@babel/helper-module-imports": "^7.21.4",
                 "@babel/helper-simple-access": "^7.21.5",
                 "@babel/helper-split-export-declaration": "^7.18.6",
                 "@babel/helper-validator-identifier": "^7.19.1",
-                "@babel/template": "^7.20.7",
-                "@babel/traverse": "^7.21.5",
-                "@babel/types": "^7.21.5"
+                "@babel/template": "^7.21.9",
+                "@babel/traverse": "^7.22.1",
+                "@babel/types": "^7.22.0"
             },
-            "resolved": "https://registry.npmjs.org/@babel/helper-module-transforms/-/helper-module-transforms-7.21.5.tgz",
-            "version": "7.21.5"
+            "resolved": "https://registry.npmjs.org/@babel/helper-module-transforms/-/helper-module-transforms-7.22.1.tgz",
+            "version": "7.22.1"
         },
         "@babel/helper-simple-access": {
             "integrity": "sha512-ENPDAMC1wAjR0uaCUwliBdiSl1KBJAVnMTzXqi64c2MG8MPR6ii4qf7bSXDqSFbr4W6W028/rf5ivoHop5/mkg==",
             "peer": true,
             "requires": {
                 "@babel/types": "^7.21.5"
             },
@@ -161,79 +161,79 @@
         },
         "@babel/helper-validator-option": {
             "integrity": "sha512-rmL/B8/f0mKS2baE9ZpyTcTavvEuWhTTW8amjzXNvYG4AwBsqTLikfXsEofsJEfKHf+HQVQbFOHy6o+4cnC/fQ==",
             "resolved": "https://registry.npmjs.org/@babel/helper-validator-option/-/helper-validator-option-7.21.0.tgz",
             "version": "7.21.0"
         },
         "@babel/helpers": {
-            "integrity": "sha512-BSY+JSlHxOmGsPTydUkPf1MdMQ3M81x5xGCOVgWM3G8XH77sJ292Y2oqcp0CbbgxhqBuI46iUz1tT7hqP7EfgA==",
+            "integrity": "sha512-jBJ7jWblbgr7r6wYZHMdIqKc73ycaTcCaWRq4/2LpuPHcx7xMlZvpGQkOYc9HeSjn6rcx15CPlgVcBtZ4WZJ2w==",
             "peer": true,
             "requires": {
-                "@babel/template": "^7.20.7",
-                "@babel/traverse": "^7.21.5",
-                "@babel/types": "^7.21.5"
+                "@babel/template": "^7.21.9",
+                "@babel/traverse": "^7.22.1",
+                "@babel/types": "^7.22.3"
             },
-            "resolved": "https://registry.npmjs.org/@babel/helpers/-/helpers-7.21.5.tgz",
-            "version": "7.21.5"
+            "resolved": "https://registry.npmjs.org/@babel/helpers/-/helpers-7.22.3.tgz",
+            "version": "7.22.3"
         },
         "@babel/highlight": {
             "integrity": "sha512-u7stbOuYjaPezCuLj29hNW1v64M2Md2qupEKP1fHc7WdOA3DgLh37suiSrZYY7haUB7iBeQZ9P1uiRF359do3g==",
             "requires": {
                 "@babel/helper-validator-identifier": "^7.18.6",
                 "chalk": "^2.0.0",
                 "js-tokens": "^4.0.0"
             },
             "resolved": "https://registry.npmjs.org/@babel/highlight/-/highlight-7.18.6.tgz",
             "version": "7.18.6"
         },
         "@babel/parser": {
-            "integrity": "sha512-6zavDGdzG3gUqAdWvlLFfk+36RilI+Pwyuuh7HItyeScCWP3k6i8vKclAQ0bM/0y/Kz/xiwvxhMv9MgTJP5gmA==",
+            "integrity": "sha512-VLLsx06XkEYqBtE5YGPwfSGwfrjnyPP5oiGty3S8pQLFDFLaS8VwWSIxkTXpcvr5zeYLE6+MBNl2npl/YnfofA==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.21.8.tgz",
-            "version": "7.21.8"
+            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.22.4.tgz",
+            "version": "7.22.4"
         },
         "@babel/template": {
-            "integrity": "sha512-8SegXApWe6VoNw0r9JHpSteLKTpTiLZ4rMlGIm9JQ18KiCtyQiAMEazujAHrUS5flrcqYZa75ukev3P6QmUwUw==",
+            "integrity": "sha512-MK0X5k8NKOuWRamiEfc3KEJiHMTkGZNUjzMipqCGDDc6ijRl/B7RGSKVGncu4Ro/HdyzzY6cmoXuKI2Gffk7vQ==",
             "peer": true,
             "requires": {
-                "@babel/code-frame": "^7.18.6",
-                "@babel/parser": "^7.20.7",
-                "@babel/types": "^7.20.7"
+                "@babel/code-frame": "^7.21.4",
+                "@babel/parser": "^7.21.9",
+                "@babel/types": "^7.21.5"
             },
-            "resolved": "https://registry.npmjs.org/@babel/template/-/template-7.20.7.tgz",
-            "version": "7.20.7"
+            "resolved": "https://registry.npmjs.org/@babel/template/-/template-7.21.9.tgz",
+            "version": "7.21.9"
         },
         "@babel/traverse": {
-            "integrity": "sha512-AhQoI3YjWi6u/y/ntv7k48mcrCXmus0t79J9qPNlk/lAsFlCiJ047RmbfMOawySTHtywXhbXgpx/8nXMYd+oFw==",
+            "integrity": "sha512-Tn1pDsjIcI+JcLKq1AVlZEr4226gpuAQTsLMorsYg9tuS/kG7nuwwJ4AB8jfQuEgb/COBwR/DqJxmoiYFu5/rQ==",
             "peer": true,
             "requires": {
                 "@babel/code-frame": "^7.21.4",
-                "@babel/generator": "^7.21.5",
-                "@babel/helper-environment-visitor": "^7.21.5",
+                "@babel/generator": "^7.22.3",
+                "@babel/helper-environment-visitor": "^7.22.1",
                 "@babel/helper-function-name": "^7.21.0",
                 "@babel/helper-hoist-variables": "^7.18.6",
                 "@babel/helper-split-export-declaration": "^7.18.6",
-                "@babel/parser": "^7.21.5",
-                "@babel/types": "^7.21.5",
+                "@babel/parser": "^7.22.4",
+                "@babel/types": "^7.22.4",
                 "debug": "^4.1.0",
                 "globals": "^11.1.0"
             },
-            "resolved": "https://registry.npmjs.org/@babel/traverse/-/traverse-7.21.5.tgz",
-            "version": "7.21.5"
+            "resolved": "https://registry.npmjs.org/@babel/traverse/-/traverse-7.22.4.tgz",
+            "version": "7.22.4"
         },
         "@babel/types": {
-            "integrity": "sha512-m4AfNvVF2mVC/F7fDEdH2El3HzUg9It/XsCxZiOTTA3m3qYfcSVSbTfM6Q9xG+hYDniZssYhlXKKUMD5m8tF4Q==",
+            "integrity": "sha512-Tx9x3UBHTTsMSW85WB2kphxYQVvrZ/t1FxD88IpSgIjiUJlCm9z+xWIDwyo1vffTwSqteqyznB8ZE9vYYk16zA==",
             "peer": true,
             "requires": {
                 "@babel/helper-string-parser": "^7.21.5",
                 "@babel/helper-validator-identifier": "^7.19.1",
                 "to-fast-properties": "^2.0.0"
             },
-            "resolved": "https://registry.npmjs.org/@babel/types/-/types-7.21.5.tgz",
-            "version": "7.21.5"
+            "resolved": "https://registry.npmjs.org/@babel/types/-/types-7.22.4.tgz",
+            "version": "7.22.4"
         },
         "@colors/colors": {
             "integrity": "sha512-ooWCrlZP11i8GImSjTHYHLkvFDP48nS4+204nGb1RiX/WXYHmJA2III9/e2DWVabCESdW7hBAEzHRqUn9OUVvQ==",
             "resolved": "https://registry.npmjs.org/@colors/colors/-/colors-1.5.0.tgz",
             "version": "1.5.0"
         },
         "@dabh/diagnostics": {
@@ -352,18 +352,18 @@
         },
         "@polka/url": {
             "integrity": "sha512-a5Sab1C4/icpTZVzZc5Ghpz88yQtGOyNqYXcZgOssB2uuAr+wF/MvN6bgtW32q7HHrvBki+BsZ0OuNv6EV3K9g==",
             "resolved": "https://registry.npmjs.org/@polka/url/-/url-1.0.0-next.21.tgz",
             "version": "1.0.0-next.21"
         },
         "@popperjs/core": {
-            "integrity": "sha512-Cr4OjIkipTtcXKjAsm8agyleBuDHvxzeBoa1v543lbv1YaIwQjESsVcmjiWiPEbC1FIeHOG/Op9kdCmAmiS3Kw==",
+            "integrity": "sha512-P1st0aksCrn9sGZhp8GMYwBnQsbvAWsZAX44oXNNvLHGqAOcoVxmjZiohstwQ7SqKnbR47akdNi+uleWD8+g6A==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@popperjs/core/-/core-2.11.7.tgz",
-            "version": "2.11.7"
+            "resolved": "https://registry.npmjs.org/@popperjs/core/-/core-2.11.8.tgz",
+            "version": "2.11.8"
         },
         "@sideway/address": {
             "integrity": "sha512-7vwq+rOHVWjyXxVlR76Agnvhy8I9rpzjosTESvmhNeXOXdZZB15Fl+TI9x1SiHZH5Jv2wTGduSxFDIaq0m3DUw==",
             "requires": {
                 "@hapi/hoek": "^9.0.0"
             },
             "resolved": "https://registry.npmjs.org/@sideway/address/-/address-4.1.4.tgz",
@@ -484,21 +484,21 @@
                 "@types/express-serve-static-core": "*",
                 "@types/node": "*"
             },
             "resolved": "https://registry.npmjs.org/@types/connect-history-api-fallback/-/connect-history-api-fallback-1.5.0.tgz",
             "version": "1.5.0"
         },
         "@types/eslint": {
-            "integrity": "sha512-Piet7dG2JBuDIfohBngQ3rCt7MgO9xCO4xIMKxBThCq5PNRB91IjlJ10eJVwfoNtvTErmxLzwBZ7rHZtbOMmFQ==",
+            "integrity": "sha512-nbq2mvc/tBrK9zQQuItvjJl++GTN5j06DaPtp3hZCpngmG6Q3xoyEmd0TwZI0gAy/G1X0zhGBbr2imsGFdFV0g==",
             "requires": {
                 "@types/estree": "*",
                 "@types/json-schema": "*"
             },
-            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-8.37.0.tgz",
-            "version": "8.37.0"
+            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-8.40.0.tgz",
+            "version": "8.40.0"
         },
         "@types/eslint-scope": {
             "integrity": "sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==",
             "requires": {
                 "@types/eslint": "*",
                 "@types/estree": "*"
             },
@@ -518,23 +518,23 @@
                 "@types/qs": "*",
                 "@types/serve-static": "*"
             },
             "resolved": "https://registry.npmjs.org/@types/express/-/express-4.17.17.tgz",
             "version": "4.17.17"
         },
         "@types/express-serve-static-core": {
-            "integrity": "sha512-fvr49XlCGoUj2Pp730AItckfjat4WNb0lb3kfrLWffd+RLeoGAMsq7UOy04PAPtoL01uKwcp6u8nhzpgpDYr3w==",
+            "integrity": "sha512-wALWQwrgiB2AWTT91CB62b6Yt0sNHpznUXeZEcnPU3DRdlDIz74x8Qg1UUYKSVFi+va5vKOLYRBI1bRKiLLKIg==",
             "requires": {
                 "@types/node": "*",
                 "@types/qs": "*",
                 "@types/range-parser": "*",
                 "@types/send": "*"
             },
-            "resolved": "https://registry.npmjs.org/@types/express-serve-static-core/-/express-serve-static-core-4.17.34.tgz",
-            "version": "4.17.34"
+            "resolved": "https://registry.npmjs.org/@types/express-serve-static-core/-/express-serve-static-core-4.17.35.tgz",
+            "version": "4.17.35"
         },
         "@types/html-minifier-terser": {
             "integrity": "sha512-oh/6byDPnL1zeNXFrDXFLyZjkr1MsBG667IM792caf1L2UPOOMf65NFzjUH/ltyfwjAGfs1rsX1eftK0jC/KIg==",
             "resolved": "https://registry.npmjs.org/@types/html-minifier-terser/-/html-minifier-terser-6.1.0.tgz",
             "version": "6.1.0"
         },
         "@types/http-proxy": {
@@ -542,32 +542,32 @@
             "requires": {
                 "@types/node": "*"
             },
             "resolved": "https://registry.npmjs.org/@types/http-proxy/-/http-proxy-1.17.11.tgz",
             "version": "1.17.11"
         },
         "@types/json-schema": {
-            "integrity": "sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==",
-            "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.11.tgz",
-            "version": "7.0.11"
+            "integrity": "sha512-Hr5Jfhc9eYOQNPYO5WLDq/n4jqijdHNlDXjuAQkkt+mWdQR+XJToOHrsD4cPaMXpn6KO7y2+wM8AZEs8VpBLVA==",
+            "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.12.tgz",
+            "version": "7.0.12"
         },
         "@types/mime": {
             "integrity": "sha512-YATxVxgRqNH6nHEIsvg6k2Boc1JHI9ZbH5iWFFv/MTkchz3b1ieGDa5T0a9RznNdI0KhVbdbWSN+KWWrQZRxTw==",
             "resolved": "https://registry.npmjs.org/@types/mime/-/mime-1.3.2.tgz",
             "version": "1.3.2"
         },
         "@types/minimist": {
             "integrity": "sha512-jhuKLIRrhvCPLqwPcx6INqmKeiA5EWrsCOPhrlFSrbrmU4ZMPjj5Ul/oLCMDO98XRUIwVm78xICz4EPCektzeQ==",
             "resolved": "https://registry.npmjs.org/@types/minimist/-/minimist-1.2.2.tgz",
             "version": "1.2.2"
         },
         "@types/node": {
-            "integrity": "sha512-O+z53uwx64xY7D6roOi4+jApDGFg0qn6WHcxe5QeqjMaTezBO/mxdfFXIVAVVyNWKx84OmPB3L8kbVYOTeN34A==",
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.1.0.tgz",
-            "version": "20.1.0"
+            "integrity": "sha512-JJulVEQXmiY9Px5axXHeYGLSjhkZEnD+MDPDGbCbIAbMslkKwmygtZFy1X6s/075Yo94sf8GuSlFfPzysQrWZQ==",
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.2.5.tgz",
+            "version": "20.2.5"
         },
         "@types/normalize-package-data": {
             "integrity": "sha512-Gj7cI7z+98M282Tqmp2K5EIsoouUEzbBJhQQzDE3jSIRk6r9gsz0oUokqIUR4u1R3dMHo0pDHM7sNOHyhulypw==",
             "resolved": "https://registry.npmjs.org/@types/normalize-package-data/-/normalize-package-data-2.4.1.tgz",
             "version": "2.4.1"
         },
         "@types/parse-json": {
@@ -760,20 +760,20 @@
                     "requires": {
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
-                    "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
+                    "integrity": "sha512-Wvss5ivl8TMRZXXESstBA4uR5iXgEN/VC5/sOcuXdVLzcdkz4HWetIoRfG5gb5X+ij/G9rw9YoGn3QoQ8OCSpw==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
-                    "version": "7.5.0"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.1.tgz",
+                    "version": "7.5.1"
                 },
                 "supports-color": {
                     "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
                     "requires": {
                         "has-flag": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
@@ -875,143 +875,143 @@
         },
         "@vue/web-component-wrapper": {
             "integrity": "sha512-Iu8Tbg3f+emIIMmI2ycSI8QcEuAUgPTgHwesDU1eKMLE4YC/c/sFbGc70QgMq31ijRftV0R7vCm9co6rldCeOA==",
             "resolved": "https://registry.npmjs.org/@vue/web-component-wrapper/-/web-component-wrapper-1.3.0.tgz",
             "version": "1.3.0"
         },
         "@webassemblyjs/ast": {
-            "integrity": "sha512-LHY/GSAZZRpsNQH+/oHqhRQ5FT7eoULcBqgfyTB5nQHogFnK3/7QoN7dLnwSE/JkUAF0SrRuclT7ODqMFtWxxQ==",
+            "integrity": "sha512-IN1xI7PwOvLPgjcf180gC1bqn3q/QaOCwYUahIOhbYUu8KA/3tw2RT/T0Gidi1l7Hhj5D/INhJxiICObqpMu4Q==",
             "requires": {
-                "@webassemblyjs/helper-numbers": "1.11.5",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.5"
+                "@webassemblyjs/helper-numbers": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.5.tgz",
-            "version": "1.11.5"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/floating-point-hex-parser": {
-            "integrity": "sha512-1j1zTIC5EZOtCplMBG/IEwLtUojtwFVwdyVMbL/hwWqbzlQoJsWCOavrdnLkemwNoC/EOwtUFch3fuo+cbcXYQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-ejAj9hfRJ2XMsNHk/v6Fu2dGS+i4UaXBXGemOfQ/JfQ6mdQg/WXtwleQRLLS4OvfDhv8rYnVwH27YJLMyYsxhw==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/helper-api-error": {
-            "integrity": "sha512-L65bDPmfpY0+yFrsgz8b6LhXmbbs38OnwDCf6NpnMUYqa+ENfE5Dq9E42ny0qz/PdR0LJyq/T5YijPnU8AXEpA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-o0YkoP4pVu4rN8aTJgAyj9hC2Sv5UlkzCHhxqWj8butaLvnpdc2jOwh4ewE6CX0txSfLn/UYaV/pheS2Txg//Q==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/helper-buffer": {
-            "integrity": "sha512-fDKo1gstwFFSfacIeH5KfwzjykIE6ldh1iH9Y/8YkAZrhmu4TctqYjSh7t0K2VyDSXOZJ1MLhht/k9IvYGcIxg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-z3nFzdcp1mb8nEOFFk8DrYLpHvhKC3grJD2ardfKOzmbmJvEf/tPIqCY+sNcwZIY8ZD7IkB2l7/pqhUhqm7hLA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/helper-numbers": {
-            "integrity": "sha512-DhykHXM0ZABqfIGYNv93A5KKDw/+ywBFnuWybZZWcuzWHfbp21wUfRkbtz7dMGwGgT4iXjWuhRMA2Mzod6W4WA==",
+            "integrity": "sha512-vUIhZ8LZoIWHBohiEObxVm6hwP034jwmc9kuq5GdHZH0wiLVLIPcMCdpJzG4C11cHoQ25TFIQj9kaVADVX7N3g==",
             "requires": {
-                "@webassemblyjs/floating-point-hex-parser": "1.11.5",
-                "@webassemblyjs/helper-api-error": "1.11.5",
+                "@webassemblyjs/floating-point-hex-parser": "1.11.6",
+                "@webassemblyjs/helper-api-error": "1.11.6",
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.5.tgz",
-            "version": "1.11.5"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/helper-wasm-bytecode": {
-            "integrity": "sha512-oC4Qa0bNcqnjAowFn7MPCETQgDYytpsfvz4ujZz63Zu/a/v71HeCAAmZsgZ3YVKec3zSPYytG3/PrRCqbtcAvA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-sFFHKwcmBprO9e7Icf0+gddyWYDViL8bpPjJJl0WHxCdETktXdmtWLGVzoHbqUcY4Be1LkNfwTmXOJUFZYSJdA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/helper-wasm-section": {
-            "integrity": "sha512-uEoThA1LN2NA+K3B9wDo3yKlBfVtC6rh0i4/6hvbz071E8gTNZD/pT0MsBf7MeD6KbApMSkaAK0XeKyOZC7CIA==",
+            "integrity": "sha512-LPpZbSOwTpEC2cgn4hTydySy1Ke+XEu+ETXuoyvuyezHO3Kjdu90KK95Sh9xTbmjrCsUwvWwCOQQNta37VrS9g==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.5",
-                "@webassemblyjs/helper-buffer": "1.11.5",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
-                "@webassemblyjs/wasm-gen": "1.11.5"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/wasm-gen": "1.11.6"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.5.tgz",
-            "version": "1.11.5"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/ieee754": {
-            "integrity": "sha512-37aGq6qVL8A8oPbPrSGMBcp38YZFXcHfiROflJn9jxSdSMMM5dS5P/9e2/TpaJuhE+wFrbukN2WI6Hw9MH5acg==",
+            "integrity": "sha512-LM4p2csPNvbij6U1f19v6WR56QZ8JcHg3QIJTlSwzFcmx6WSORicYj6I63f9yU1kEUtrpG+kjkiIAkevHpDXrg==",
             "requires": {
                 "@xtuc/ieee754": "^1.2.0"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.5.tgz",
-            "version": "1.11.5"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/leb128": {
-            "integrity": "sha512-ajqrRSXaTJoPW+xmkfYN6l8VIeNnR4vBOTQO9HzR7IygoCcKWkICbKFbVTNMjMgMREqXEr0+2M6zukzM47ZUfQ==",
+            "integrity": "sha512-m7a0FhE67DQXgouf1tbN5XQcdWoNgaAuoULHIfGFIEVKA6tu/edls6XnIlkmS6FrXAquJRPni3ZZKjw6FSPjPQ==",
             "requires": {
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.5.tgz",
-            "version": "1.11.5"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/utf8": {
-            "integrity": "sha512-WiOhulHKTZU5UPlRl53gHR8OxdGsSOxqfpqWeA2FmcwBMaoEdz6b2x2si3IwC9/fSPLfe8pBMRTHVMk5nlwnFQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-vtXf2wTQ3+up9Zsg8sa2yWiQpzSsMyXj0qViVP6xKGCUT8p8YJ6HqI7l5eCnWx1T/FYdsv07HQs2wTFbbof/RA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/wasm-edit": {
-            "integrity": "sha512-C0p9D2fAu3Twwqvygvf42iGCQ4av8MFBLiTb+08SZ4cEdwzWx9QeAHDo1E2k+9s/0w1DM40oflJOpkZ8jW4HCQ==",
+            "integrity": "sha512-Ybn2I6fnfIGuCR+Faaz7YcvtBKxvoLV3Lebn1tM4o/IAJzmi9AWYIPWpyBfU8cC+JxAO57bk4+zdsTjJR+VTOw==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.5",
-                "@webassemblyjs/helper-buffer": "1.11.5",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
-                "@webassemblyjs/helper-wasm-section": "1.11.5",
-                "@webassemblyjs/wasm-gen": "1.11.5",
-                "@webassemblyjs/wasm-opt": "1.11.5",
-                "@webassemblyjs/wasm-parser": "1.11.5",
-                "@webassemblyjs/wast-printer": "1.11.5"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/helper-wasm-section": "1.11.6",
+                "@webassemblyjs/wasm-gen": "1.11.6",
+                "@webassemblyjs/wasm-opt": "1.11.6",
+                "@webassemblyjs/wasm-parser": "1.11.6",
+                "@webassemblyjs/wast-printer": "1.11.6"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.5.tgz",
-            "version": "1.11.5"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/wasm-gen": {
-            "integrity": "sha512-14vteRlRjxLK9eSyYFvw1K8Vv+iPdZU0Aebk3j6oB8TQiQYuO6hj9s4d7qf6f2HJr2khzvNldAFG13CgdkAIfA==",
+            "integrity": "sha512-3XOqkZP/y6B4F0PBAXvI1/bky7GryoogUtfwExeP/v7Nzwo1QLcq5oQmpKlftZLbT+ERUOAZVQjuNVak6UXjPA==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.5",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
-                "@webassemblyjs/ieee754": "1.11.5",
-                "@webassemblyjs/leb128": "1.11.5",
-                "@webassemblyjs/utf8": "1.11.5"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/ieee754": "1.11.6",
+                "@webassemblyjs/leb128": "1.11.6",
+                "@webassemblyjs/utf8": "1.11.6"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.5.tgz",
-            "version": "1.11.5"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/wasm-opt": {
-            "integrity": "sha512-tcKwlIXstBQgbKy1MlbDMlXaxpucn42eb17H29rawYLxm5+MsEmgPzeCP8B1Cl69hCice8LeKgZpRUAPtqYPgw==",
+            "integrity": "sha512-cOrKuLRE7PCe6AsOVl7WasYf3wbSo4CeOk6PkrjS7g57MFfVUF9u6ysQBBODX0LdgSvQqRiGz3CXvIDKcPNy4g==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.5",
-                "@webassemblyjs/helper-buffer": "1.11.5",
-                "@webassemblyjs/wasm-gen": "1.11.5",
-                "@webassemblyjs/wasm-parser": "1.11.5"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/wasm-gen": "1.11.6",
+                "@webassemblyjs/wasm-parser": "1.11.6"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.5.tgz",
-            "version": "1.11.5"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/wasm-parser": {
-            "integrity": "sha512-SVXUIwsLQlc8srSD7jejsfTU83g7pIGr2YYNb9oHdtldSxaOhvA5xwvIiWIfcX8PlSakgqMXsLpLfbbJ4cBYew==",
+            "integrity": "sha512-6ZwPeGzMJM3Dqp3hCsLgESxBGtT/OeCvCZ4TA1JUPYgmhAx38tTPR9JaKy0S5H3evQpO/h2uWs2j6Yc/fjkpTQ==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.5",
-                "@webassemblyjs/helper-api-error": "1.11.5",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
-                "@webassemblyjs/ieee754": "1.11.5",
-                "@webassemblyjs/leb128": "1.11.5",
-                "@webassemblyjs/utf8": "1.11.5"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-api-error": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/ieee754": "1.11.6",
+                "@webassemblyjs/leb128": "1.11.6",
+                "@webassemblyjs/utf8": "1.11.6"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.5.tgz",
-            "version": "1.11.5"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@webassemblyjs/wast-printer": {
-            "integrity": "sha512-f7Pq3wvg3GSPUPzR0F6bmI89Hdb+u9WXrSKc4v+N0aV0q6r42WoF92Jp2jEorBEBRoRNXgjp53nBniDXcqZYPA==",
+            "integrity": "sha512-JM7AhRcE+yW2GWYaKeHL5vt4xqee5N2WcezptmgyhNS+ScggqcT1OtXykhAb13Sn5Yas0j2uv9tHgrjwvzAP4A==",
             "requires": {
-                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/ast": "1.11.6",
                 "@xtuc/long": "4.2.2"
             },
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.5.tgz",
-            "version": "1.11.5"
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "@xtuc/ieee754": {
             "integrity": "sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==",
             "resolved": "https://registry.npmjs.org/@xtuc/ieee754/-/ieee754-1.2.0.tgz",
             "version": "1.2.0"
         },
         "@xtuc/long": {
@@ -1030,18 +1030,18 @@
         },
         "acorn": {
             "integrity": "sha512-xjIYgE8HBrkpd/sJqOGNspf8uHG+NOHGOw6a/Urj8taM2EXfdNAH2oFcPeIFfsv3+kz/mJrS5VuMqbNLjCa2vw==",
             "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.8.2.tgz",
             "version": "8.8.2"
         },
         "acorn-import-assertions": {
-            "integrity": "sha512-m7VZ3jwz4eK6A4Vtt8Ew1/mNbP24u0FhdyfA7fSvnJR6LMdfOYnmuIrrJAgrYfYJ10F/otaHTtrtrtmHdMNzEw==",
+            "integrity": "sha512-cmMwop9x+8KFhxvKrKfPYmN6/pKTYYHBqLa0DfvVZcKMJWNyWLnaqND7dx/qn66R7ewM1UX5XMaDVP5wlVTaVA==",
             "requires": {},
-            "resolved": "https://registry.npmjs.org/acorn-import-assertions/-/acorn-import-assertions-1.8.0.tgz",
-            "version": "1.8.0"
+            "resolved": "https://registry.npmjs.org/acorn-import-assertions/-/acorn-import-assertions-1.9.0.tgz",
+            "version": "1.9.0"
         },
         "acorn-walk": {
             "integrity": "sha512-k+iyHEuPgSw6SbuDpGQM+06HQUa04DZ3o+F6CSzXMvvI5KMvnaEqXe+YVe555R9nn6GPt404fos4wcgpw12SDA==",
             "resolved": "https://registry.npmjs.org/acorn-walk/-/acorn-walk-8.2.0.tgz",
             "version": "8.2.0"
         },
         "address": {
@@ -1275,18 +1275,18 @@
         "bootstrap": {
             "integrity": "sha512-51Bbp/Uxr9aTuy6ca/8FbFloBUJZLHwnhTcnjIeRn2suQWsWzcuJhGjKDB5eppVte/8oCdOL3VuwxvZDUggwGQ==",
             "requires": {},
             "resolved": "https://registry.npmjs.org/bootstrap/-/bootstrap-4.6.2.tgz",
             "version": "4.6.2"
         },
         "bootstrap5": {
-            "integrity": "sha512-cEKPM+fwb3cT8NzQZYEu4HilJ3anCrWqh3CHAok1p9jXqMPsPTBhU25fBckEJHJ/p+tTxTFTsFQGM+gaHpi3QQ==",
+            "integrity": "sha512-UnBV3E3v4STVNQdms6jSGO2CvOkjUMdDAVR2V5N4uCMdaIkaQjbcEAMqRimDHIs4uqBYzDAKCQwCB+97tJgHQw==",
             "requires": {},
-            "resolved": "https://registry.npmjs.org/bootstrap/-/bootstrap-5.2.3.tgz",
-            "version": "npm:bootstrap@5.2.3"
+            "resolved": "https://registry.npmjs.org/bootstrap/-/bootstrap-5.3.0.tgz",
+            "version": "npm:bootstrap@5.3.0"
         },
         "brace-expansion": {
             "integrity": "sha512-XnAIvQ8eM+kC6aULx6wuQiwVsnzsi9d3WxzV3FpWTGA19F621kwdbsAcFKXgKUHZWsy+mY6iL1sHTxWEFCytDA==",
             "requires": {
                 "balanced-match": "^1.0.0"
             },
             "resolved": "https://registry.npmjs.org/brace-expansion/-/brace-expansion-2.0.1.tgz",
@@ -1305,23 +1305,23 @@
             "requires": {
                 "base64-js": "^1.1.2"
             },
             "resolved": "https://registry.npmjs.org/brotli/-/brotli-1.3.3.tgz",
             "version": "1.3.3"
         },
         "browserslist": {
-            "integrity": "sha512-tUkiguQGW7S3IhB7N+c2MV/HZPSCPAAiYBZXLsBhFB/PCy6ZKKsZrmBayHV9fdGV/ARIfJ14NkxKzRDjvp7L6w==",
+            "integrity": "sha512-BauCXrQ7I2ftSqd2mvKHGo85XR0u7Ru3C/Hxsy/0TkfCtjrmAbPdzLGasmoiBxplpDXlPvdjX9u7srIMfgasNA==",
             "requires": {
-                "caniuse-lite": "^1.0.30001449",
-                "electron-to-chromium": "^1.4.284",
-                "node-releases": "^2.0.8",
-                "update-browserslist-db": "^1.0.10"
+                "caniuse-lite": "^1.0.30001489",
+                "electron-to-chromium": "^1.4.411",
+                "node-releases": "^2.0.12",
+                "update-browserslist-db": "^1.0.11"
             },
-            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.21.5.tgz",
-            "version": "4.21.5"
+            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.21.7.tgz",
+            "version": "4.21.7"
         },
         "buffer": {
             "integrity": "sha512-EHcyIPBQ4BSGlvjB16k5KgAJ27CIsHY/2JBmCRReo48y9rQ3MaUzWX3KVlBa4U7MyX02HdVj0K7C3WaB3ju7FQ==",
             "requires": {
                 "base64-js": "^1.3.1",
                 "ieee754": "^1.1.13"
             },
@@ -1369,17 +1369,17 @@
                 "lodash.memoize": "^4.1.2",
                 "lodash.uniq": "^4.5.0"
             },
             "resolved": "https://registry.npmjs.org/caniuse-api/-/caniuse-api-3.0.0.tgz",
             "version": "3.0.0"
         },
         "caniuse-lite": {
-            "integrity": "sha512-uv7/gXuHi10Whlj0pp5q/tsK/32J2QSqVRKQhs2j8VsDCjgyruAh/eEXHF822VqO9yT6iZKw3nRwZRSPBE9OQg==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001486.tgz",
-            "version": "1.0.30001486"
+            "integrity": "sha512-F6x5IEuigtUfU5ZMQK2jsy5JqUUlEFRVZq8bO2a+ysq5K7jD6PPc9YXZj78xDNS3uNchesp1Jw47YXEqr+Viyg==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001495.tgz",
+            "version": "1.0.30001495"
         },
         "case-sensitive-paths-webpack-plugin": {
             "integrity": "sha512-roIFONhcxog0JSSWbvVAh3OocukmSgpqOH6YpMkCvav/ySIV3JKg4Dc8vYtQjYi/UxpNE36r/9v+VqTQqgkYmw==",
             "resolved": "https://registry.npmjs.org/case-sensitive-paths-webpack-plugin/-/case-sensitive-paths-webpack-plugin-2.4.0.tgz",
             "version": "2.4.0"
         },
         "chalk": {
@@ -1865,40 +1865,40 @@
                     "requires": {
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
-                    "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
+                    "integrity": "sha512-Wvss5ivl8TMRZXXESstBA4uR5iXgEN/VC5/sOcuXdVLzcdkz4HWetIoRfG5gb5X+ij/G9rw9YoGn3QoQ8OCSpw==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
-                    "version": "7.5.0"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.1.tgz",
+                    "version": "7.5.1"
                 },
                 "yallist": {
                     "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
                     "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
                     "version": "4.0.0"
                 }
             },
-            "integrity": "sha512-qhOH1KlBMnZP8FzRO6YCH9UHXQhVMcEGLyNdb7Hv2cpcmJbW0YrddO+tG1ab5nT41KpHIYGsbeHqxB9xPu1pKQ==",
+            "integrity": "sha512-xDAXtEVGlD0gJ07iclwWVkLoZOpEvAWaSyf6W18S2pOC//K8+qUDIx8IIT3D+HjnmkJPQeesOPv5aiUaJsCM2g==",
             "requires": {
                 "icss-utils": "^5.1.0",
-                "postcss": "^8.4.19",
+                "postcss": "^8.4.21",
                 "postcss-modules-extract-imports": "^3.0.0",
-                "postcss-modules-local-by-default": "^4.0.0",
+                "postcss-modules-local-by-default": "^4.0.3",
                 "postcss-modules-scope": "^3.0.0",
                 "postcss-modules-values": "^4.0.0",
                 "postcss-value-parser": "^4.2.0",
                 "semver": "^7.3.8"
             },
-            "resolved": "https://registry.npmjs.org/css-loader/-/css-loader-6.7.3.tgz",
-            "version": "6.7.3"
+            "resolved": "https://registry.npmjs.org/css-loader/-/css-loader-6.8.1.tgz",
+            "version": "6.8.1"
         },
         "css-minimizer-webpack-plugin": {
             "dependencies": {
                 "ajv": {
                     "integrity": "sha512-sRu1kpcO9yLtYxBKvqfTeh9KzZEwO3STyX1HT+4CaDzC6HpTGYhIhPIzj9XuKU7KYDwnaeh5hcOwjy1QuJzBPA==",
                     "requires": {
                         "fast-deep-equal": "^3.1.1",
@@ -1919,23 +1919,23 @@
                 },
                 "json-schema-traverse": {
                     "integrity": "sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==",
                     "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz",
                     "version": "1.0.0"
                 },
                 "schema-utils": {
-                    "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
+                    "integrity": "sha512-Jw+GZVbP5IggB2WAn6UHI02LBwGmsIeYN/lNbSMZyDziQ7jmtAUrqKqDja+W89YHVs+KL/3IkIMltAklqB1vAw==",
                     "requires": {
                         "@types/json-schema": "^7.0.9",
                         "ajv": "^8.9.0",
                         "ajv-formats": "^2.1.1",
                         "ajv-keywords": "^5.1.0"
                     },
-                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
-                    "version": "4.0.1"
+                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.1.0.tgz",
+                    "version": "4.1.0"
                 }
             },
             "integrity": "sha512-1u6D71zeIfgngN2XNRJefc/hY7Ybsxd74Jm4qngIXyUEk7fss3VUzuHxLAq/R8NAba4QU9OUSaMZlbpRc7bM4Q==",
             "requires": {
                 "cssnano": "^5.0.6",
                 "jest-worker": "^27.0.2",
                 "postcss": "^8.3.5",
@@ -2291,17 +2291,17 @@
         },
         "ee-first": {
             "integrity": "sha512-WMwm9LhRUo+WUaRN+vRuETqG89IgZphVSNkdFgeb6sS/E4OrDIN7t48CAewSHXc6C8lefD8KKfr5vY61brQlow==",
             "resolved": "https://registry.npmjs.org/ee-first/-/ee-first-1.1.1.tgz",
             "version": "1.1.1"
         },
         "electron-to-chromium": {
-            "integrity": "sha512-L9zlje9bIw0h+CwPQumiuVlfMcV4boxRjFIWDcLfFqTZNbkwOExBzfmswytHawObQX4OUhtNv8gIiB21kOurIg==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.385.tgz",
-            "version": "1.4.385"
+            "integrity": "sha512-wv1NufHxu11zfDbY4fglYQApMswleE9FL/DSeyOyauVXDZ+Kco96JK/tPfBUaDqfRarYp2WH2hJ/5UnVywp9Jg==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.425.tgz",
+            "version": "1.4.425"
         },
         "emoji-regex": {
             "integrity": "sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==",
             "resolved": "https://registry.npmjs.org/emoji-regex/-/emoji-regex-8.0.0.tgz",
             "version": "8.0.0"
         },
         "emojis-list": {
@@ -2324,21 +2324,21 @@
             "requires": {
                 "once": "^1.4.0"
             },
             "resolved": "https://registry.npmjs.org/end-of-stream/-/end-of-stream-1.4.4.tgz",
             "version": "1.4.4"
         },
         "enhanced-resolve": {
-            "integrity": "sha512-eyV8f0y1+bzyfh8xAwW/WTSZpLbjhqc4ne9eGSH4Zo2ejdyiNG9pU6mf9DG8a7+Auk6MFTlNOT4Y2y/9k8GKVg==",
+            "integrity": "sha512-Vklwq2vDKtl0y/vtwjSesgJ5MYS7Etuk5txS8VdKL4AOS1aUlD96zqIfsOSLQsdv3xgMRbtkWM8eG9XDfKUPow==",
             "requires": {
                 "graceful-fs": "^4.2.4",
                 "tapable": "^2.2.0"
             },
-            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.13.0.tgz",
-            "version": "5.13.0"
+            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.14.1.tgz",
+            "version": "5.14.1"
         },
         "entities": {
             "integrity": "sha512-p92if5Nz619I0w+akJrLZH0MX0Pb5DX39XOwQTtXSdQQOaYH03S1uIQp4mhOZtAXrxq4ViO67YTiLBo2638o9A==",
             "resolved": "https://registry.npmjs.org/entities/-/entities-2.2.0.tgz",
             "version": "2.2.0"
         },
         "error-ex": {
@@ -2697,17 +2697,17 @@
                 "jsonfile": "^6.0.1",
                 "universalify": "^2.0.0"
             },
             "resolved": "https://registry.npmjs.org/fs-extra/-/fs-extra-9.1.0.tgz",
             "version": "9.1.0"
         },
         "fs-monkey": {
-            "integrity": "sha512-cybjIfiiE+pTWicSCLFHSrXZ6EilF30oh91FDP9S2B051prEa7QWfrVTQm10/dDpswBDXZugPa1Ogu8Yh+HV0Q==",
-            "resolved": "https://registry.npmjs.org/fs-monkey/-/fs-monkey-1.0.3.tgz",
-            "version": "1.0.3"
+            "integrity": "sha512-INM/fWAxMICjttnD0DX1rBvinKskj5G1w+oy/pnm9u/tSlnBrzFonJMcalKJ30P8RRsPzKcCG7Q8l0jx5Fh9YQ==",
+            "resolved": "https://registry.npmjs.org/fs-monkey/-/fs-monkey-1.0.4.tgz",
+            "version": "1.0.4"
         },
         "fs.realpath": {
             "integrity": "sha512-OO0pH2lK6a0hZnAdau5ItzHPI6pUlvI7jMVnxUQRtw4owF2wk8lOSabtGDCTP4Ggrg2MbGnWO9X8K1t4+fGMDw==",
             "resolved": "https://registry.npmjs.org/fs.realpath/-/fs.realpath-1.0.0.tgz",
             "version": "1.0.0"
         },
         "fsevents": {
@@ -2729,22 +2729,23 @@
         },
         "get-caller-file": {
             "integrity": "sha512-DyFP3BM/3YHTQOCUL/w0OZHR0lpKeGrxotcHWcqNEdnltqFwXVfhEBQ94eIo34AfQpo0rGki4cyIiftY06h2Fg==",
             "resolved": "https://registry.npmjs.org/get-caller-file/-/get-caller-file-2.0.5.tgz",
             "version": "2.0.5"
         },
         "get-intrinsic": {
-            "integrity": "sha512-L049y6nFOuom5wGyRc3/gdTLO94dySVKRACj1RmJZBQXlbTMhtNIgkWkUHq+jYmZvKf14EW1EoJnnjbmoHij0Q==",
+            "integrity": "sha512-2DcsyfABl+gVHEfCOaTrWgyt+tb6MSEGmKq+kI5HwLbIYgjgmMcV8KQ41uaKz1xxUcn9tJtgFbQUEVcEbd0FYw==",
             "requires": {
                 "function-bind": "^1.1.1",
                 "has": "^1.0.3",
+                "has-proto": "^1.0.1",
                 "has-symbols": "^1.0.3"
             },
-            "resolved": "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.0.tgz",
-            "version": "1.2.0"
+            "resolved": "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.1.tgz",
+            "version": "1.2.1"
         },
         "get-stream": {
             "integrity": "sha512-GMat4EJ5161kIy2HevLlr4luNjBgvmj413KaQA7jt4V8B4RDsfpHk7WQ9GVqfYyyx8OS/L66Kox+rJRNklLK7w==",
             "requires": {
                 "pump": "^3.0.0"
             },
             "resolved": "https://registry.npmjs.org/get-stream/-/get-stream-4.1.0.tgz",
@@ -2826,14 +2827,19 @@
             "version": "1.0.3"
         },
         "has-flag": {
             "integrity": "sha512-sKJf1+ceQBr4SMkvQnBDNDtf4TXpVhVGateu0t918bl30FnbE2m4vNLX+VWe/dpjlb+HugGYzW7uQXH98HPEYw==",
             "resolved": "https://registry.npmjs.org/has-flag/-/has-flag-3.0.0.tgz",
             "version": "3.0.0"
         },
+        "has-proto": {
+            "integrity": "sha512-7qE+iP+O+bgF9clE5+UoBFzE65mlBiVj3tKCrlNQ0Ogwm0BjpT/gK4SlLYDMybDh5I3TCTKnPPa0oMG7JDYrhg==",
+            "resolved": "https://registry.npmjs.org/has-proto/-/has-proto-1.0.1.tgz",
+            "version": "1.0.1"
+        },
         "has-symbols": {
             "integrity": "sha512-l3LCuF6MgDNwTDKkdYGEihYjt5pRPbEg46rtlmnSPlUbgmB8LOIrKJbYYFBSbnPaJexMKtiPO8hmeRjRz2Td+A==",
             "resolved": "https://registry.npmjs.org/has-symbols/-/has-symbols-1.0.3.tgz",
             "version": "1.0.3"
         },
         "hash-sum": {
             "integrity": "sha512-WdZTbAByD+pHfl/g9QSsBIIwy8IT+EsPiKDs0KNX+zSHhdDLFKdZu0BQHljvO+0QI/BasbMSUa8wYNCZTvhslg==",
@@ -2897,17 +2903,17 @@
         },
         "hsluv": {
             "integrity": "sha512-08iL2VyCRbkQKBySkSh6m8zMUa3sADAxGVWs3Z1aPcUkTJeK0ETG4Fc27tEmQBGUAXZjIsXOZqBvacuVNSC/fQ==",
             "resolved": "https://registry.npmjs.org/hsluv/-/hsluv-0.0.3.tgz",
             "version": "0.0.3"
         },
         "html-entities": {
-            "integrity": "sha512-DV5Ln36z34NNTDgnz0EWGBLZENelNAtkiFA4kyNOG2tDI6Mz1uSWiq1wAKdyjnJwyDiDO7Fa2SO1CTxPXL8VxA==",
-            "resolved": "https://registry.npmjs.org/html-entities/-/html-entities-2.3.3.tgz",
-            "version": "2.3.3"
+            "integrity": "sha512-72TJlcMkYsEJASa/3HnX7VT59htM7iSHbH59NSZbtc+22Ap0Txnlx91sfeB+/A7wNZg7UxtZdhAW4y+/jimrdg==",
+            "resolved": "https://registry.npmjs.org/html-entities/-/html-entities-2.3.5.tgz",
+            "version": "2.3.5"
         },
         "html-minifier-terser": {
             "integrity": "sha512-YXxSlJBZTP7RS3tWnQw74ooKa6L9b9i9QYXY21eUEvhZ3u9XLfv6OnFsQq6RxkhHygsaUMvYsZRV5rU/OVNZxw==",
             "requires": {
                 "camel-case": "^4.1.2",
                 "clean-css": "^5.2.2",
                 "commander": "^8.3.0",
@@ -3063,20 +3069,20 @@
             "requires": {
                 "binary-extensions": "^2.0.0"
             },
             "resolved": "https://registry.npmjs.org/is-binary-path/-/is-binary-path-2.1.0.tgz",
             "version": "2.1.0"
         },
         "is-core-module": {
-            "integrity": "sha512-RECHCBCd/viahWmwj6enj19sKbHfJrddi/6cBDsNTKbNq0f7VeaUkBo60BqzvPqo/W54ChS62Z5qyun7cfOMqQ==",
+            "integrity": "sha512-Q4ZuBAe2FUsKtyQJoQHlvP8OvBERxO3jEmy1I7hcRXcJBGGHFh/aJBswbXuS9sgrDH2QUO8ilkwNPHvHMd8clg==",
             "requires": {
                 "has": "^1.0.3"
             },
-            "resolved": "https://registry.npmjs.org/is-core-module/-/is-core-module-2.12.0.tgz",
-            "version": "2.12.0"
+            "resolved": "https://registry.npmjs.org/is-core-module/-/is-core-module-2.12.1.tgz",
+            "version": "2.12.1"
         },
         "is-docker": {
             "integrity": "sha512-F+i2BKsFrH66iaUFc0woD8sLy8getkwTwtOBjvs56Cx4CgJDeKQeqfz8wAYiSb8JOprWhHH5p77PbmYCvvUuXQ==",
             "resolved": "https://registry.npmjs.org/is-docker/-/is-docker-2.2.1.tgz",
             "version": "2.2.1"
         },
         "is-extglob": {
@@ -3200,18 +3206,18 @@
                 "@sideway/formula": "^3.0.1",
                 "@sideway/pinpoint": "^2.0.0"
             },
             "resolved": "https://registry.npmjs.org/joi/-/joi-17.9.2.tgz",
             "version": "17.9.2"
         },
         "jquery": {
-            "integrity": "sha512-v28EW9DWDFpzcD9O5iyJXg3R3+q+mET5JhnjJzQUZMHOv67bpSIHq81GEYpPNZHG+XXHsfSme3nxp/hndKEcsQ==",
+            "integrity": "sha512-umpJ0/k8X0MvD1ds0P9SfowREz2LenHsQaxSohMZ5OMNEU2r0tf8pdeEFTHMFxWVxKNyU9rTtK3CWzUCTKJUeQ==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/jquery/-/jquery-3.6.4.tgz",
-            "version": "3.6.4"
+            "resolved": "https://registry.npmjs.org/jquery/-/jquery-3.7.0.tgz",
+            "version": "3.7.0"
         },
         "js-message": {
             "integrity": "sha512-efJLHhLjIyKRewNS9EGZ4UpI8NguuL6fKkhRxVuMmrGV2xN/0APGdQYwLFky5w9naebSZ0OwAGp0G6/2Cg90rA==",
             "resolved": "https://registry.npmjs.org/js-message/-/js-message-1.0.7.tgz",
             "version": "1.0.7"
         },
         "js-tokens": {
@@ -3527,20 +3533,20 @@
         },
         "media-typer": {
             "integrity": "sha512-dq+qelQ9akHpcOl/gUVRTxVIOkAJ1wR3QAvb4RsVjS8oVoFjDGTc679wJYmUmknUF5HwMLOgb5O+a3KxfWapPQ==",
             "resolved": "https://registry.npmjs.org/media-typer/-/media-typer-0.3.0.tgz",
             "version": "0.3.0"
         },
         "memfs": {
-            "integrity": "sha512-UWbFJKvj5k+nETdteFndTpYxdeTMox/ULeqX5k/dpaQJCCFmj5EeKv3dBcyO2xmkRAx2vppRu5dVG7SOtsGOzA==",
+            "integrity": "sha512-UERzLsxzllchadvbPs5aolHh65ISpKpM+ccLbOJ8/vvpBKmAWf+la7dXFy7Mr0ySHbdHrFv5kGFCUHHe6GFEmw==",
             "requires": {
-                "fs-monkey": "^1.0.3"
+                "fs-monkey": "^1.0.4"
             },
-            "resolved": "https://registry.npmjs.org/memfs/-/memfs-3.5.1.tgz",
-            "version": "3.5.1"
+            "resolved": "https://registry.npmjs.org/memfs/-/memfs-3.5.3.tgz",
+            "version": "3.5.3"
         },
         "merge-descriptors": {
             "integrity": "sha512-cCi6g3/Zr1iqQi6ySbseM1Xvooa98N0w31jzUYrXPX2xqObmFGHJ0tQ5u74H3mVh7wLouTseZyYIq39g8cNp1w==",
             "resolved": "https://registry.npmjs.org/merge-descriptors/-/merge-descriptors-1.0.1.tgz",
             "version": "1.0.1"
         },
         "merge-source-map": {
@@ -3626,31 +3632,31 @@
                 },
                 "json-schema-traverse": {
                     "integrity": "sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==",
                     "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz",
                     "version": "1.0.0"
                 },
                 "schema-utils": {
-                    "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
+                    "integrity": "sha512-Jw+GZVbP5IggB2WAn6UHI02LBwGmsIeYN/lNbSMZyDziQ7jmtAUrqKqDja+W89YHVs+KL/3IkIMltAklqB1vAw==",
                     "requires": {
                         "@types/json-schema": "^7.0.9",
                         "ajv": "^8.9.0",
                         "ajv-formats": "^2.1.1",
                         "ajv-keywords": "^5.1.0"
                     },
-                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
-                    "version": "4.0.1"
+                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.1.0.tgz",
+                    "version": "4.1.0"
                 }
             },
-            "integrity": "sha512-9HaR++0mlgom81s95vvNjxkg52n2b5s//3ZTI1EtzFb98awsLSivs2LMsVqnQ3ay0PVhqWcGNyDaTE961FOcjQ==",
+            "integrity": "sha512-Qk7HcgaPkGG6eD77mLvZS1nmxlao3j+9PkrT9Uc7HAE1id3F41+DdBRYRYkbyfNRGzm8/YWtzhw7nVPmwhqTQw==",
             "requires": {
                 "schema-utils": "^4.0.0"
             },
-            "resolved": "https://registry.npmjs.org/mini-css-extract-plugin/-/mini-css-extract-plugin-2.7.5.tgz",
-            "version": "2.7.5"
+            "resolved": "https://registry.npmjs.org/mini-css-extract-plugin/-/mini-css-extract-plugin-2.7.6.tgz",
+            "version": "2.7.6"
         },
         "minimalistic-assert": {
             "integrity": "sha512-UtJcAD4yEaGtjPezWuO9wC4nwUnVH/8/Im3yEHQP4b67cXlD/Qr9hdITCU1xDbSEXg2XKNaP8jsReV7vQd00/A==",
             "resolved": "https://registry.npmjs.org/minimalistic-assert/-/minimalistic-assert-1.0.1.tgz",
             "version": "1.0.1"
         },
         "minimatch": {
@@ -3691,17 +3697,17 @@
         },
         "mkdirp-classic": {
             "integrity": "sha512-gKLcREMhtuZRwRAfqP3RFW+TK4JqApVBtOIftVgjuABpAtpxhPGaDcfvbhNvD0B8iD1oUr/txX35NjcaY6Ns/A==",
             "resolved": "https://registry.npmjs.org/mkdirp-classic/-/mkdirp-classic-0.5.3.tgz",
             "version": "0.5.3"
         },
         "module-alias": {
-            "integrity": "sha512-A/78XjoX2EmNvppVWEhM2oGk3x4lLxnkEA4jTbaK97QKSDjkIoOsKQlfylt/d3kKKi596Qy3NP5XrXJ6fZIC9Q==",
-            "resolved": "https://registry.npmjs.org/module-alias/-/module-alias-2.2.2.tgz",
-            "version": "2.2.2"
+            "integrity": "sha512-23g5BFj4zdQL/b6tor7Ji+QY4pEfNH784BMslY9Qb0UnJWRAt+lQGLYmRaM0KDBwIG23ffEBELhZDP2rhi9f/Q==",
+            "resolved": "https://registry.npmjs.org/module-alias/-/module-alias-2.2.3.tgz",
+            "version": "2.2.3"
         },
         "moment": {
             "integrity": "sha512-5LC9SOxjSc2HF6vO2CyuTDNivEdoz2IvyJJGj6X8DJ0eFyfszE0QiEd+iXmBvUP3WHxSjFH/vIsA0EN00cgr8w==",
             "resolved": "https://registry.npmjs.org/moment/-/moment-2.29.4.tgz",
             "version": "2.29.4"
         },
         "mrmime": {
@@ -3787,56 +3793,56 @@
                     "requires": {
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
-                    "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
+                    "integrity": "sha512-Wvss5ivl8TMRZXXESstBA4uR5iXgEN/VC5/sOcuXdVLzcdkz4HWetIoRfG5gb5X+ij/G9rw9YoGn3QoQ8OCSpw==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
-                    "version": "7.5.0"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.1.tgz",
+                    "version": "7.5.1"
                 },
                 "yallist": {
                     "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
                     "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
                     "version": "4.0.0"
                 }
             },
-            "integrity": "sha512-zNy02qivjjRosswoYmPi8hIKJRr8MpQyeKT6qlcq/OnOgA3Rhoae+IYOqsM9V5+JnHWmxKnWOT2GxvtqdtOCXA==",
+            "integrity": "sha512-MYjZTiAETGG28/7fBH1RjuY7vzDwYC5q5U4whCgM4jNEQcC0gAvN339LxXukmL2T2tGpzYTfp+LZ5RN7E5DwEg==",
             "requires": {
                 "semver": "^7.3.5"
             },
-            "resolved": "https://registry.npmjs.org/node-abi/-/node-abi-3.40.0.tgz",
-            "version": "3.40.0"
+            "resolved": "https://registry.npmjs.org/node-abi/-/node-abi-3.44.0.tgz",
+            "version": "3.44.0"
         },
         "node-addon-api": {
             "integrity": "sha512-eh0GgfEkpnoWDq+VY8OyvYhFEzBk6jIYbRKdIlyTiAXIVJ8PyBaKb0rp7oDtoddbdoHWhq8wwr+XZ81F1rpNdA==",
             "resolved": "https://registry.npmjs.org/node-addon-api/-/node-addon-api-5.1.0.tgz",
             "version": "5.1.0"
         },
         "node-fetch": {
-            "integrity": "sha512-DJm/CJkZkRjKKj4Zi4BsKVZh3ValV5IR5s7LVZnW+6YMh0W1BfNA8XSs6DLMGYlId5F3KnA70uu2qepcR08Qqg==",
+            "integrity": "sha512-4I6pdBY1EthSqDmJkiNk3JIT8cswwR9nfeW/cPdUagJYEQG7R95WRH74wpz7ma8Gh/9dI9FP+OU+0E4FvtA55w==",
             "requires": {
                 "whatwg-url": "^5.0.0"
             },
-            "resolved": "https://registry.npmjs.org/node-fetch/-/node-fetch-2.6.9.tgz",
-            "version": "2.6.9"
+            "resolved": "https://registry.npmjs.org/node-fetch/-/node-fetch-2.6.11.tgz",
+            "version": "2.6.11"
         },
         "node-forge": {
             "integrity": "sha512-dPEtOeMvF9VMcYV/1Wb8CPoVAXtp6MKMlcbAt4ddqmGqUJ6fQZFXkNZNkNlfevtNkGtaSoXf/vNNNSvgrdXwtA==",
             "resolved": "https://registry.npmjs.org/node-forge/-/node-forge-1.3.1.tgz",
             "version": "1.3.1"
         },
         "node-releases": {
-            "integrity": "sha512-5GFldHPXVG/YZmFzJvKK2zDSzPKhEp0+ZR5SVaoSag9fsL5YgHbUHDfnG5494ISANDcK4KwPXAx2xqVEydmd7w==",
-            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.10.tgz",
-            "version": "2.0.10"
+            "integrity": "sha512-QzsYKWhXTWx8h1kIvqfnC++o0pEmpRQA/aenALsL2F4pqNVr7YzcdMlDij5WBnwftRbJCNJL/O7zdKaxKPHqgQ==",
+            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.12.tgz",
+            "version": "2.0.12"
         },
         "normalize-package-data": {
             "dependencies": {
                 "semver": {
                     "integrity": "sha512-sauaDf/PZdVgrLTNYHRtpXa1iRiKcaebiKQ1BJdpQlWH2lCvexQdX55snPFyK7QzpudqbCI0qXFfOasHdyNDGQ==",
                     "resolved": "https://registry.npmjs.org/semver/-/semver-5.7.1.tgz",
                     "version": "5.7.1"
@@ -4200,22 +4206,22 @@
                 "debug": "^3.2.7",
                 "mkdirp": "^0.5.6"
             },
             "resolved": "https://registry.npmjs.org/portfinder/-/portfinder-1.0.32.tgz",
             "version": "1.0.32"
         },
         "postcss": {
-            "integrity": "sha512-bQ3qMcpF6A/YjR55xtoTr0jGOlnPOKAIMdOWiv0EIT6HVPEaJiJB4NLljSbiHoC2RX7DN5Uvjtpbg1NPdwv1oA==",
+            "integrity": "sha512-M0RzbcI0sO/XJNucsGjvWU9ERWxb/ytp1w6dKtxTKgixdtQDq4rmx/g8W1hnaheq9jgwL/oyEdH5Bc4WwJKMqg==",
             "requires": {
                 "nanoid": "^3.3.6",
                 "picocolors": "^1.0.0",
                 "source-map-js": "^1.0.2"
             },
-            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.23.tgz",
-            "version": "8.4.23"
+            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.24.tgz",
+            "version": "8.4.24"
         },
         "postcss-calc": {
             "integrity": "sha512-SmWMSJmB8MRnnULldx0lQIyhSNvuDl9HfrZkaqqE/WHAhToYsAvDq+yAsA/kIyINDszOp3Rh0GFoNuH5Ypsm3Q==",
             "requires": {
                 "postcss-selector-parser": "^6.0.9",
                 "postcss-value-parser": "^4.2.0"
             },
@@ -4273,20 +4279,20 @@
                     "requires": {
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
-                    "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
+                    "integrity": "sha512-Wvss5ivl8TMRZXXESstBA4uR5iXgEN/VC5/sOcuXdVLzcdkz4HWetIoRfG5gb5X+ij/G9rw9YoGn3QoQ8OCSpw==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
-                    "version": "7.5.0"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.1.tgz",
+                    "version": "7.5.1"
                 },
                 "yallist": {
                     "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
                     "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
                     "version": "4.0.0"
                 }
             },
@@ -4358,22 +4364,22 @@
         "postcss-modules-extract-imports": {
             "integrity": "sha512-bdHleFnP3kZ4NYDhuGlVK+CMrQ/pqUm8bx/oGL93K6gVwiclvX5x0n76fYMKuIGKzlABOy13zsvqjb0f92TEXw==",
             "requires": {},
             "resolved": "https://registry.npmjs.org/postcss-modules-extract-imports/-/postcss-modules-extract-imports-3.0.0.tgz",
             "version": "3.0.0"
         },
         "postcss-modules-local-by-default": {
-            "integrity": "sha512-sT7ihtmGSF9yhm6ggikHdV0hlziDTX7oFoXtuVWeDd3hHObNkcHRo9V3yg7vCAY7cONyxJC/XXCmmiHHcvX7bQ==",
+            "integrity": "sha512-2/u2zraspoACtrbFRnTijMiQtb4GW4BvatjaG/bCjYQo8kLTdevCUlwuBHx2sCnSyrI3x3qj4ZK1j5LQBgzmwA==",
             "requires": {
                 "icss-utils": "^5.0.0",
                 "postcss-selector-parser": "^6.0.2",
                 "postcss-value-parser": "^4.1.0"
             },
-            "resolved": "https://registry.npmjs.org/postcss-modules-local-by-default/-/postcss-modules-local-by-default-4.0.0.tgz",
-            "version": "4.0.0"
+            "resolved": "https://registry.npmjs.org/postcss-modules-local-by-default/-/postcss-modules-local-by-default-4.0.3.tgz",
+            "version": "4.0.3"
         },
         "postcss-modules-scope": {
             "integrity": "sha512-hncihwFA2yPath8oZ15PZqvWGkWf+XUfQgUGamS4LqoP1anQLOsOJw0vr7J7IwLpoY9fatA2qiGUGmuZL0Iqlg==",
             "requires": {
                 "postcss-selector-parser": "^6.0.4"
             },
             "resolved": "https://registry.npmjs.org/postcss-modules-scope/-/postcss-modules-scope-3.0.0.tgz",
@@ -4482,21 +4488,21 @@
             "requires": {
                 "postcss-value-parser": "^4.2.0"
             },
             "resolved": "https://registry.npmjs.org/postcss-reduce-transforms/-/postcss-reduce-transforms-5.1.0.tgz",
             "version": "5.1.0"
         },
         "postcss-selector-parser": {
-            "integrity": "sha512-NdxGCAZdRrwVI1sy59+Wzrh+pMMHxapGnpfenDVlMEXoOcvt4pGE0JLK9YY2F5dLxcFYA/YbVQKhcGU+FtSYQg==",
+            "integrity": "sha512-EaV1Gl4mUEV4ddhDnv/xtj7sxwrwxdetHdWUGnT4VJQf+4d05v6lHYZr8N573k5Z0BViss7BDhfWtKS3+sfAqQ==",
             "requires": {
                 "cssesc": "^3.0.0",
                 "util-deprecate": "^1.0.2"
             },
-            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.0.12.tgz",
-            "version": "6.0.12"
+            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.0.13.tgz",
+            "version": "6.0.13"
         },
         "postcss-svgo": {
             "integrity": "sha512-D75KsH1zm5ZrHyxPakAxJWtkyXew5qwS70v56exwvw542d9CRtTo78K0WeFxZB4G7JXKKMbEZtZayTGdIky/eA==",
             "requires": {
                 "postcss-value-parser": "^4.2.0",
                 "svgo": "^2.7.0"
             },
@@ -4828,32 +4834,32 @@
         },
         "safer-buffer": {
             "integrity": "sha512-YZo3K82SD7Riyi0E1EQPojLz7kpepnSQI9IyPbHHg1XXXevb5dJI7tpyN2ADxGcQbHG7vcyRHk0cbwqcQriUtg==",
             "resolved": "https://registry.npmjs.org/safer-buffer/-/safer-buffer-2.1.2.tgz",
             "version": "2.1.2"
         },
         "sass": {
-            "integrity": "sha512-NHpxIzN29MXvWiuswfc1W3I0N8SXBd8UR26WntmDlRYf0bSADnwnOjsyMZ3lMezSlArD33Vs3YFhp7dWvL770A==",
+            "integrity": "sha512-u56TU0AIFqMtauKl/OJ1AeFsXqRHkgO7nCWmHaDwfxDo9GUMSqBA4NEh6GMuh1CYVM7zuROYtZrHzPc2ixK+ww==",
             "requires": {
                 "chokidar": ">=3.0.0 <4.0.0",
                 "immutable": "^4.0.0",
                 "source-map-js": ">=0.6.2 <2.0.0"
             },
-            "resolved": "https://registry.npmjs.org/sass/-/sass-1.62.1.tgz",
-            "version": "1.62.1"
+            "resolved": "https://registry.npmjs.org/sass/-/sass-1.63.2.tgz",
+            "version": "1.63.2"
         },
         "schema-utils": {
-            "integrity": "sha512-pvjEHOgWc9OWA/f/DE3ohBWTD6EleVLf7iFUkoSwAxttdBhB9QUebQgxER2kWueOvRJXPHNnyrvvh9eZINB8Eg==",
+            "integrity": "sha512-0zTyLGyDJYd/MBxG1AhJkKa6fpEBds4OQO2ut0w7OYG+ZGhGea09lijvzsqegYSik88zc7cUtIlnnO+/BvD6gQ==",
             "requires": {
                 "@types/json-schema": "^7.0.8",
                 "ajv": "^6.12.5",
                 "ajv-keywords": "^3.5.2"
             },
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.2.tgz",
-            "version": "3.1.2"
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.2.0.tgz",
+            "version": "3.2.0"
         },
         "select-hose": {
             "integrity": "sha512-mEugaLK+YfkijB4fx0e6kImuJdCIt2LxCRcbEYPqRGCs4F2ogyfZU5IAZRdjCP8JPq2AtdNoC/Dux63d9Kiryg==",
             "resolved": "https://registry.npmjs.org/select-hose/-/select-hose-2.0.0.tgz",
             "version": "2.0.0"
         },
         "selfsigned": {
@@ -5010,20 +5016,20 @@
                     "requires": {
                         "yallist": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
                     "version": "6.0.0"
                 },
                 "semver": {
-                    "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
+                    "integrity": "sha512-Wvss5ivl8TMRZXXESstBA4uR5iXgEN/VC5/sOcuXdVLzcdkz4HWetIoRfG5gb5X+ij/G9rw9YoGn3QoQ8OCSpw==",
                     "requires": {
                         "lru-cache": "^6.0.0"
                     },
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
-                    "version": "7.5.0"
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.1.tgz",
+                    "version": "7.5.1"
                 },
                 "yallist": {
                     "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
                     "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
                     "version": "4.0.0"
                 }
             },
@@ -5345,35 +5351,35 @@
             "dependencies": {
                 "commander": {
                     "integrity": "sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==",
                     "resolved": "https://registry.npmjs.org/commander/-/commander-2.20.3.tgz",
                     "version": "2.20.3"
                 }
             },
-            "integrity": "sha512-hVl35zClmpisy6oaoKALOpS0rDYLxRFLHhRuDlEGTKey9qHjS1w9GMORjuwIMt70Wan4lwsLYyWDVnWgF+KUEw==",
+            "integrity": "sha512-/bi0Zm2C6VAexlGgLlVxA0P2lru/sdLyfCVaRMfKVo9nWxbmz7f/sD8VPybPeSUJaJcwmCJis9pBIhcVcG1QcQ==",
             "requires": {
-                "@jridgewell/source-map": "^0.3.2",
-                "acorn": "^8.5.0",
+                "@jridgewell/source-map": "^0.3.3",
+                "acorn": "^8.8.2",
                 "commander": "^2.20.0",
                 "source-map-support": "~0.5.20"
             },
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.17.1.tgz",
-            "version": "5.17.1"
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.17.7.tgz",
+            "version": "5.17.7"
         },
         "terser-webpack-plugin": {
-            "integrity": "sha512-WiHL3ElchZMsK27P8uIUh4604IgJyAW47LVXGbEoB21DbQcZ+OuMpGjVYnEUaqcWM6dO8uS2qUbA7LSCWqvsbg==",
+            "integrity": "sha512-ZuXsqE07EcggTWQjXUj+Aot/OMcD0bMKGgF63f7UxYcu5/AJF53aIpK1YoP5xR9l6s/Hy2b+t1AM0bLNPRuhwA==",
             "requires": {
                 "@jridgewell/trace-mapping": "^0.3.17",
                 "jest-worker": "^27.4.5",
                 "schema-utils": "^3.1.1",
                 "serialize-javascript": "^6.0.1",
                 "terser": "^5.16.8"
             },
-            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.8.tgz",
-            "version": "5.3.8"
+            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.9.tgz",
+            "version": "5.3.9"
         },
         "text-hex": {
             "integrity": "sha512-uuVGNWzgJ4yhRaNSiubPY7OjISw4sw4E5Uv0wbjp+OzcbmVU/rsT8ujgcXJhn9ypzsgr5vlzpPqP+MBBKcGvbg==",
             "resolved": "https://registry.npmjs.org/text-hex/-/text-hex-1.0.0.tgz",
             "version": "1.0.0"
         },
         "thenify": {
@@ -5457,17 +5463,17 @@
         },
         "triple-beam": {
             "integrity": "sha512-XrHUvV5HpdLmIj4uVMxHggLbFSZYIn7HEWsqePZcI50pco+MPqJ50wMGY794X7AOOhxOBAjbkqfAbEe/QMp2Lw==",
             "resolved": "https://registry.npmjs.org/triple-beam/-/triple-beam-1.3.0.tgz",
             "version": "1.3.0"
         },
         "tslib": {
-            "integrity": "sha512-336iVw3rtn2BUK7ORdIAHTyxHGRIHVReokCR3XjbckJMK7ms8FysBfhLR8IXnAgy7T0PTPNBWKiH514FOW/WSg==",
-            "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.5.0.tgz",
-            "version": "2.5.0"
+            "integrity": "sha512-mSxlJJwl3BMEQCUNnxXBU9jP4JBktcEGhURcPR6VQVlnP0FdDEsIaz0C35dXNGLyRfrATNofF0F5p2KPxQgB+w==",
+            "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.5.3.tgz",
+            "version": "2.5.3"
         },
         "tunnel-agent": {
             "integrity": "sha512-McnNiV1l8RYeY8tBgEpuodCC1mLUdbSN+CYBL7kJsJNInOP8UjDDEwdk6Mw60vdLLrr5NHKZhMAOSrR2NZuQ+w==",
             "requires": {
                 "safe-buffer": "^5.0.1"
             },
             "resolved": "https://registry.npmjs.org/tunnel-agent/-/tunnel-agent-0.6.0.tgz",
@@ -5618,22 +5624,22 @@
                     "requires": {
                         "has-flag": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
                     "version": "7.2.0"
                 }
             },
-            "integrity": "sha512-zAjrT+TNWTpgRODxqDfzbDyvuTf5kCP9xmMk8aspQKuYNnTY2r0XK/bHu1DKLpSpk0I6fkQph5OLKB7HcRIPZw==",
+            "integrity": "sha512-aqNvKJvnz2A/6VWeJZodAo8XLoAlVwBv+2Z6dama+LHsAF+P/xijQ+OfWrxIs0wcGSJduvdzvTuATzXbNKkpiw==",
             "requires": {
                 "chalk": "^4.1.0",
                 "hash-sum": "^2.0.0",
                 "watchpack": "^2.4.0"
             },
-            "resolved": "https://registry.npmjs.org/vue-loader/-/vue-loader-17.1.0.tgz",
-            "version": "17.1.0"
+            "resolved": "https://registry.npmjs.org/vue-loader/-/vue-loader-17.2.2.tgz",
+            "version": "17.2.2"
         },
         "vue-style-loader": {
             "dependencies": {
                 "hash-sum": {
                     "integrity": "sha512-fUs4B4L+mlt8/XAtSOGMUO1TXmAelItBPtJG7CyHJfYTdDjwisntGO2JQz7oUsatOY9o68+57eziUVNw/mRHmA==",
                     "resolved": "https://registry.npmjs.org/hash-sum/-/hash-sum-1.0.2.tgz",
                     "version": "1.0.2"
@@ -5688,26 +5694,26 @@
         },
         "webidl-conversions": {
             "integrity": "sha512-2JAn3z8AR6rjK8Sm8orRC0h/bcl/DqL7tRPdGZ4I1CjdF+EaMLmYxBHyXuKL849eucPFhvBoxMsflfOb8kxaeQ==",
             "resolved": "https://registry.npmjs.org/webidl-conversions/-/webidl-conversions-3.0.1.tgz",
             "version": "3.0.1"
         },
         "webpack": {
-            "integrity": "sha512-iGNA2fHhnDcV1bONdUu554eZx+XeldsaeQ8T67H6KKHl2nUSwX8Zm7cmzOA46ox/X1ARxf7Bjv8wQ/HsB5fxBg==",
+            "integrity": "sha512-3BOvworZ8SO/D4GVP+GoRC3fVeg5MO4vzmq8TJJEkdmopxyazGDxN8ClqN12uzrZW9Tv8EED8v5VSb6Sqyi0pg==",
             "requires": {
                 "@types/eslint-scope": "^3.7.3",
                 "@types/estree": "^1.0.0",
                 "@webassemblyjs/ast": "^1.11.5",
                 "@webassemblyjs/wasm-edit": "^1.11.5",
                 "@webassemblyjs/wasm-parser": "^1.11.5",
                 "acorn": "^8.7.1",
-                "acorn-import-assertions": "^1.7.6",
+                "acorn-import-assertions": "^1.9.0",
                 "browserslist": "^4.14.5",
                 "chrome-trace-event": "^1.0.2",
-                "enhanced-resolve": "^5.13.0",
+                "enhanced-resolve": "^5.14.1",
                 "es-module-lexer": "^1.2.1",
                 "eslint-scope": "5.1.1",
                 "events": "^3.2.0",
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.2.9",
                 "json-parse-even-better-errors": "^2.3.1",
                 "loader-runner": "^4.2.0",
@@ -5715,16 +5721,16 @@
                 "neo-async": "^2.6.2",
                 "schema-utils": "^3.1.2",
                 "tapable": "^2.1.1",
                 "terser-webpack-plugin": "^5.3.7",
                 "watchpack": "^2.4.0",
                 "webpack-sources": "^3.2.3"
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.82.0.tgz",
-            "version": "5.82.0"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.86.0.tgz",
+            "version": "5.86.0"
         },
         "webpack-bundle-analyzer": {
             "dependencies": {
                 "ansi-styles": {
                     "integrity": "sha512-zbB9rCJAT1rbjiVDb2hqKFHNYLxgtk8NURxZ3IZwD3F6NtxbXZQCnnSi1Lkx+IDohdPlFp222wVALIheZJQSEg==",
                     "requires": {
                         "color-convert": "^2.0.1"
@@ -5769,29 +5775,29 @@
                     "requires": {
                         "has-flag": "^4.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
                     "version": "7.2.0"
                 }
             },
-            "integrity": "sha512-ZzoSBePshOKhr+hd8u6oCkZVwpVaXgpw23ScGLFpR6SjYI7+7iIWYarjN6OEYOfRt8o7ZyZZQk0DuMizJ+LEIg==",
+            "integrity": "sha512-+bXGmO1LyiNx0i9enBu3H8mv42sj/BJWhZNFwjz92tVnBa9J3JMGo2an2IXlEleoDOPn/Hofl5hr/xCpObUDtw==",
             "requires": {
                 "@discoveryjs/json-ext": "0.5.7",
                 "acorn": "^8.0.4",
                 "acorn-walk": "^8.0.0",
                 "chalk": "^4.1.0",
                 "commander": "^7.2.0",
                 "gzip-size": "^6.0.0",
                 "lodash": "^4.17.20",
                 "opener": "^1.5.2",
                 "sirv": "^1.0.7",
                 "ws": "^7.3.1"
             },
-            "resolved": "https://registry.npmjs.org/webpack-bundle-analyzer/-/webpack-bundle-analyzer-4.8.0.tgz",
-            "version": "4.8.0"
+            "resolved": "https://registry.npmjs.org/webpack-bundle-analyzer/-/webpack-bundle-analyzer-4.9.0.tgz",
+            "version": "4.9.0"
         },
         "webpack-chain": {
             "integrity": "sha512-7doO/SRtLu8q5WM0s7vPKPWX580qhi0/yBHkOxNkv50f6qB76Zy9o2wRTrrPULqYTvQlVHuvbA8v+G5ayuUDsA==",
             "requires": {
                 "deepmerge": "^1.5.2",
                 "javascript-stringify": "^2.0.1"
             },
@@ -5821,23 +5827,23 @@
                 },
                 "json-schema-traverse": {
                     "integrity": "sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==",
                     "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz",
                     "version": "1.0.0"
                 },
                 "schema-utils": {
-                    "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
+                    "integrity": "sha512-Jw+GZVbP5IggB2WAn6UHI02LBwGmsIeYN/lNbSMZyDziQ7jmtAUrqKqDja+W89YHVs+KL/3IkIMltAklqB1vAw==",
                     "requires": {
                         "@types/json-schema": "^7.0.9",
                         "ajv": "^8.9.0",
                         "ajv-formats": "^2.1.1",
                         "ajv-keywords": "^5.1.0"
                     },
-                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
-                    "version": "4.0.1"
+                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.1.0.tgz",
+                    "version": "4.1.0"
                 }
             },
             "integrity": "sha512-hj5CYrY0bZLB+eTO+x/j67Pkrquiy7kWepMHmUMoPsmcUaeEnQJqFzHJOyxgWlq746/wUuA64p9ta34Kyb01pA==",
             "requires": {
                 "colorette": "^2.0.10",
                 "memfs": "^3.4.3",
                 "mime-types": "^2.1.31",
@@ -5865,33 +5871,33 @@
                     "requires": {
                         "fast-deep-equal": "^3.1.3"
                     },
                     "resolved": "https://registry.npmjs.org/ajv-keywords/-/ajv-keywords-5.1.0.tgz",
                     "version": "5.1.0"
                 },
                 "ipaddr.js": {
-                    "integrity": "sha512-1qTgH9NG+IIJ4yfKs2e6Pp1bZg8wbDbKHT21HrLIeYBTRLgMYKnMTPAuI3Lcs61nfx5h1xlXnbJtH1kX5/d/ng==",
-                    "resolved": "https://registry.npmjs.org/ipaddr.js/-/ipaddr.js-2.0.1.tgz",
-                    "version": "2.0.1"
+                    "integrity": "sha512-LlbxQ7xKzfBusov6UMi4MFpEg0m+mAm9xyNGEduwXMEDuf4WfzB/RZwMVYEd7IKGvh4IUkEXYxtAVu9T3OelJQ==",
+                    "resolved": "https://registry.npmjs.org/ipaddr.js/-/ipaddr.js-2.1.0.tgz",
+                    "version": "2.1.0"
                 },
                 "json-schema-traverse": {
                     "integrity": "sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==",
                     "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz",
                     "version": "1.0.0"
                 },
                 "schema-utils": {
-                    "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
+                    "integrity": "sha512-Jw+GZVbP5IggB2WAn6UHI02LBwGmsIeYN/lNbSMZyDziQ7jmtAUrqKqDja+W89YHVs+KL/3IkIMltAklqB1vAw==",
                     "requires": {
                         "@types/json-schema": "^7.0.9",
                         "ajv": "^8.9.0",
                         "ajv-formats": "^2.1.1",
                         "ajv-keywords": "^5.1.0"
                     },
-                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
-                    "version": "4.0.1"
+                    "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.1.0.tgz",
+                    "version": "4.1.0"
                 },
                 "ws": {
                     "integrity": "sha512-x9vcZYTrFPC7aSIbj7sRCYo7L/Xb8Iy+pW0ng0wt2vCJv7M9HOMy0UoN3rr+IFC7hb7vXoqS+P9ktyLLLhO+LA==",
                     "requires": {},
                     "resolved": "https://registry.npmjs.org/ws/-/ws-8.13.0.tgz",
                     "version": "8.13.0"
                 }
@@ -5929,21 +5935,21 @@
                 "webpack-dev-middleware": "^5.3.1",
                 "ws": "^8.13.0"
             },
             "resolved": "https://registry.npmjs.org/webpack-dev-server/-/webpack-dev-server-4.15.0.tgz",
             "version": "4.15.0"
         },
         "webpack-merge": {
-            "integrity": "sha512-/SaI7xY0831XwP6kzuwhKWVKDP9t1QY1h65lAFLbZqMPIuYcD9QAW4u9STIbU9kaJbPBB/geU/gLr1wDjOhQ+Q==",
+            "integrity": "sha512-6NbRQw4+Sy50vYNTw7EyOn41OZItPiXB8GNv3INSoe3PSFaHJEz3SHTrYVaRm2LilNGnFUzh0FAwqPEmU/CwDg==",
             "requires": {
                 "clone-deep": "^4.0.1",
                 "wildcard": "^2.0.0"
             },
-            "resolved": "https://registry.npmjs.org/webpack-merge/-/webpack-merge-5.8.0.tgz",
-            "version": "5.8.0"
+            "resolved": "https://registry.npmjs.org/webpack-merge/-/webpack-merge-5.9.0.tgz",
+            "version": "5.9.0"
         },
         "webpack-sources": {
             "integrity": "sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==",
             "resolved": "https://registry.npmjs.org/webpack-sources/-/webpack-sources-3.2.3.tgz",
             "version": "3.2.3"
         },
         "webpack-virtual-modules": {
@@ -6002,30 +6008,30 @@
                 },
                 "is-stream": {
                     "integrity": "sha512-hFoiJiTl63nn+kstHGBtewWSKnQLpyb155KHheA1l39uvtO9nWIop1p3udqPcUd/xbF1VLMO4n7OI6p7RbngDg==",
                     "resolved": "https://registry.npmjs.org/is-stream/-/is-stream-2.0.1.tgz",
                     "version": "2.0.1"
                 }
             },
-            "integrity": "sha512-MsE1gRx1m5jdTTO9Ld/vND4krP2To+lgDoMEHGGa4HIlAUyXJtfc7CxQcGXVyz2IBpw5hbFkj2b/AtUdQwyRew==",
+            "integrity": "sha512-jW51iW/X95BCW6MMtZWr2jKQBP4hV5bIDq9QrIjfDk6Q9QuxvTKEAlpUNAzP+HYHFFCeENhph16s0zEunu4uuQ==",
             "requires": {
                 "@colors/colors": "1.5.0",
                 "@dabh/diagnostics": "^2.0.2",
                 "async": "^3.2.3",
                 "is-stream": "^2.0.0",
                 "logform": "^2.4.0",
                 "one-time": "^1.0.0",
                 "readable-stream": "^3.4.0",
                 "safe-stable-stringify": "^2.3.1",
                 "stack-trace": "0.0.x",
                 "triple-beam": "^1.3.0",
                 "winston-transport": "^4.5.0"
             },
-            "resolved": "https://registry.npmjs.org/winston/-/winston-3.8.2.tgz",
-            "version": "3.8.2"
+            "resolved": "https://registry.npmjs.org/winston/-/winston-3.9.0.tgz",
+            "version": "3.9.0"
         },
         "winston-daily-rotate-file": {
             "integrity": "sha512-7LGPiYGBPNyGHLn9z33i96zx/bd71pjBn9tqQzO3I4Tayv94WPmBNwKC7CO1wPHdP9uvu+Md/1nr6VSH9h0iaA==",
             "requires": {
                 "file-stream-rotator": "^0.6.1",
                 "object-hash": "^2.0.1",
                 "triple-beam": "^1.3.0",
@@ -6176,89 +6182,89 @@
             "resolved": "https://registry.npmjs.org/@babel/code-frame/-/code-frame-7.21.4.tgz",
             "version": "7.21.4"
         },
         "node_modules/@babel/compat-data": {
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-KYMqFYTaenzMK4yUtf4EW9wc4N9ef80FsbMtkwool5zpwl4YrT1SdWYSTRcT94KO4hannogdS+LxY7L+arP3gA==",
-            "resolved": "https://registry.npmjs.org/@babel/compat-data/-/compat-data-7.21.7.tgz",
-            "version": "7.21.7"
+            "integrity": "sha512-aNtko9OPOwVESUFp3MZfD8Uzxl7JzSeJpd7npIoxCasU37PFbAQRpKglkaKwlHOyeJdrREpo8TW8ldrkYWwvIQ==",
+            "resolved": "https://registry.npmjs.org/@babel/compat-data/-/compat-data-7.22.3.tgz",
+            "version": "7.22.3"
         },
         "node_modules/@babel/core": {
             "dependencies": {
                 "@ampproject/remapping": "^2.2.0",
                 "@babel/code-frame": "^7.21.4",
-                "@babel/generator": "^7.21.5",
-                "@babel/helper-compilation-targets": "^7.21.5",
-                "@babel/helper-module-transforms": "^7.21.5",
-                "@babel/helpers": "^7.21.5",
-                "@babel/parser": "^7.21.8",
-                "@babel/template": "^7.20.7",
-                "@babel/traverse": "^7.21.5",
-                "@babel/types": "^7.21.5",
+                "@babel/generator": "^7.22.0",
+                "@babel/helper-compilation-targets": "^7.22.1",
+                "@babel/helper-module-transforms": "^7.22.1",
+                "@babel/helpers": "^7.22.0",
+                "@babel/parser": "^7.22.0",
+                "@babel/template": "^7.21.9",
+                "@babel/traverse": "^7.22.1",
+                "@babel/types": "^7.22.0",
                 "convert-source-map": "^1.7.0",
                 "debug": "^4.1.0",
                 "gensync": "^1.0.0-beta.2",
                 "json5": "^2.2.2",
                 "semver": "^6.3.0"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/babel"
             },
-            "integrity": "sha512-YeM22Sondbo523Sz0+CirSPnbj9bG3P0CdHcBZdqUuaeOaYEFbOLoGU7lebvGP6P5J/WE9wOn7u7C4J9HvS1xQ==",
+            "integrity": "sha512-Hkqu7J4ynysSXxmAahpN1jjRwVJ+NdpraFLIWflgjpVob3KNyK3/tIUc7Q7szed8WMp0JNa7Qtd1E9Oo22F9gA==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/core/-/core-7.21.8.tgz",
-            "version": "7.21.8"
+            "resolved": "https://registry.npmjs.org/@babel/core/-/core-7.22.1.tgz",
+            "version": "7.22.1"
         },
         "node_modules/@babel/generator": {
             "dependencies": {
-                "@babel/types": "^7.21.5",
+                "@babel/types": "^7.22.3",
                 "@jridgewell/gen-mapping": "^0.3.2",
                 "@jridgewell/trace-mapping": "^0.3.17",
                 "jsesc": "^2.5.1"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-SrKK/sRv8GesIW1bDagf9cCG38IOMYZusoe1dfg0D8aiUe3Amvoj1QtjTPAWcfrZFvIwlleLb0gxzQidL9w14w==",
+            "integrity": "sha512-C17MW4wlk//ES/CJDL51kPNwl+qiBQyN7b9SKyVp11BLGFeSPoVaHrv+MNt8jwQFhQWowW88z1eeBx3pFz9v8A==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/generator/-/generator-7.21.5.tgz",
-            "version": "7.21.5"
+            "resolved": "https://registry.npmjs.org/@babel/generator/-/generator-7.22.3.tgz",
+            "version": "7.22.3"
         },
         "node_modules/@babel/helper-compilation-targets": {
             "dependencies": {
-                "@babel/compat-data": "^7.21.5",
+                "@babel/compat-data": "^7.22.0",
                 "@babel/helper-validator-option": "^7.21.0",
                 "browserslist": "^4.21.3",
                 "lru-cache": "^5.1.1",
                 "semver": "^6.3.0"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-1RkbFGUKex4lvsB9yhIfWltJM5cZKUftB2eNajaDv3dCMEp49iBG0K14uH8NnX9IPux2+mK7JGEOB0jn48/J6w==",
+            "integrity": "sha512-Rqx13UM3yVB5q0D/KwQ8+SPfX/+Rnsy1Lw1k/UwOC4KC6qrzIQoY3lYnBu5EHKBlEHHcj0M0W8ltPSkD8rqfsQ==",
             "peerDependencies": {
                 "@babel/core": "^7.0.0"
             },
-            "resolved": "https://registry.npmjs.org/@babel/helper-compilation-targets/-/helper-compilation-targets-7.21.5.tgz",
-            "version": "7.21.5"
+            "resolved": "https://registry.npmjs.org/@babel/helper-compilation-targets/-/helper-compilation-targets-7.22.1.tgz",
+            "version": "7.22.1"
         },
         "node_modules/@babel/helper-environment-visitor": {
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-IYl4gZ3ETsWocUWgsFZLM5i1BYx9SoemminVEXadgLBa9TdeorzgLKm8wWLA6J1N/kT3Kch8XIk1laNzYoHKvQ==",
+            "integrity": "sha512-Z2tgopurB/kTbidvzeBrc2To3PUP/9i5MUe+fU6QJCQDyPwSH2oRapkLw3KGECDYSjhQZCNxEvNvZlLw8JjGwA==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/helper-environment-visitor/-/helper-environment-visitor-7.21.5.tgz",
-            "version": "7.21.5"
+            "resolved": "https://registry.npmjs.org/@babel/helper-environment-visitor/-/helper-environment-visitor-7.22.1.tgz",
+            "version": "7.22.1"
         },
         "node_modules/@babel/helper-function-name": {
             "dependencies": {
                 "@babel/template": "^7.20.7",
                 "@babel/types": "^7.21.0"
             },
             "engines": {
@@ -6291,30 +6297,30 @@
             "integrity": "sha512-orajc5T2PsRYUN3ZryCEFeMDYwyw09c/pZeaQEZPH0MpKzSvn3e0uXsDBu3k03VI+9DBiRo+l22BfKTpKwa/Wg==",
             "peer": true,
             "resolved": "https://registry.npmjs.org/@babel/helper-module-imports/-/helper-module-imports-7.21.4.tgz",
             "version": "7.21.4"
         },
         "node_modules/@babel/helper-module-transforms": {
             "dependencies": {
-                "@babel/helper-environment-visitor": "^7.21.5",
+                "@babel/helper-environment-visitor": "^7.22.1",
                 "@babel/helper-module-imports": "^7.21.4",
                 "@babel/helper-simple-access": "^7.21.5",
                 "@babel/helper-split-export-declaration": "^7.18.6",
                 "@babel/helper-validator-identifier": "^7.19.1",
-                "@babel/template": "^7.20.7",
-                "@babel/traverse": "^7.21.5",
-                "@babel/types": "^7.21.5"
+                "@babel/template": "^7.21.9",
+                "@babel/traverse": "^7.22.1",
+                "@babel/types": "^7.22.0"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-bI2Z9zBGY2q5yMHoBvJ2a9iX3ZOAzJPm7Q8Yz6YeoUjU/Cvhmi2G4QyTNyPBqqXSgTjUxRg3L0xV45HvkNWWBw==",
+            "integrity": "sha512-dxAe9E7ySDGbQdCVOY/4+UcD8M9ZFqZcZhSPsPacvCG4M+9lwtDDQfI2EoaSvmf7W/8yCBkGU0m7Pvt1ru3UZw==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/helper-module-transforms/-/helper-module-transforms-7.21.5.tgz",
-            "version": "7.21.5"
+            "resolved": "https://registry.npmjs.org/@babel/helper-module-transforms/-/helper-module-transforms-7.22.1.tgz",
+            "version": "7.22.1"
         },
         "node_modules/@babel/helper-simple-access": {
             "dependencies": {
                 "@babel/types": "^7.21.5"
             },
             "engines": {
                 "node": ">=6.9.0"
@@ -6359,25 +6365,25 @@
             },
             "integrity": "sha512-rmL/B8/f0mKS2baE9ZpyTcTavvEuWhTTW8amjzXNvYG4AwBsqTLikfXsEofsJEfKHf+HQVQbFOHy6o+4cnC/fQ==",
             "resolved": "https://registry.npmjs.org/@babel/helper-validator-option/-/helper-validator-option-7.21.0.tgz",
             "version": "7.21.0"
         },
         "node_modules/@babel/helpers": {
             "dependencies": {
-                "@babel/template": "^7.20.7",
-                "@babel/traverse": "^7.21.5",
-                "@babel/types": "^7.21.5"
+                "@babel/template": "^7.21.9",
+                "@babel/traverse": "^7.22.1",
+                "@babel/types": "^7.22.3"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-BSY+JSlHxOmGsPTydUkPf1MdMQ3M81x5xGCOVgWM3G8XH77sJ292Y2oqcp0CbbgxhqBuI46iUz1tT7hqP7EfgA==",
+            "integrity": "sha512-jBJ7jWblbgr7r6wYZHMdIqKc73ycaTcCaWRq4/2LpuPHcx7xMlZvpGQkOYc9HeSjn6rcx15CPlgVcBtZ4WZJ2w==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/helpers/-/helpers-7.21.5.tgz",
-            "version": "7.21.5"
+            "resolved": "https://registry.npmjs.org/@babel/helpers/-/helpers-7.22.3.tgz",
+            "version": "7.22.3"
         },
         "node_modules/@babel/highlight": {
             "dependencies": {
                 "@babel/helper-validator-identifier": "^7.18.6",
                 "chalk": "^2.0.0",
                 "js-tokens": "^4.0.0"
             },
@@ -6391,67 +6397,67 @@
         "node_modules/@babel/parser": {
             "bin": {
                 "parser": "bin/babel-parser.js"
             },
             "engines": {
                 "node": ">=6.0.0"
             },
-            "integrity": "sha512-6zavDGdzG3gUqAdWvlLFfk+36RilI+Pwyuuh7HItyeScCWP3k6i8vKclAQ0bM/0y/Kz/xiwvxhMv9MgTJP5gmA==",
+            "integrity": "sha512-VLLsx06XkEYqBtE5YGPwfSGwfrjnyPP5oiGty3S8pQLFDFLaS8VwWSIxkTXpcvr5zeYLE6+MBNl2npl/YnfofA==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.21.8.tgz",
-            "version": "7.21.8"
+            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.22.4.tgz",
+            "version": "7.22.4"
         },
         "node_modules/@babel/template": {
             "dependencies": {
-                "@babel/code-frame": "^7.18.6",
-                "@babel/parser": "^7.20.7",
-                "@babel/types": "^7.20.7"
+                "@babel/code-frame": "^7.21.4",
+                "@babel/parser": "^7.21.9",
+                "@babel/types": "^7.21.5"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-8SegXApWe6VoNw0r9JHpSteLKTpTiLZ4rMlGIm9JQ18KiCtyQiAMEazujAHrUS5flrcqYZa75ukev3P6QmUwUw==",
+            "integrity": "sha512-MK0X5k8NKOuWRamiEfc3KEJiHMTkGZNUjzMipqCGDDc6ijRl/B7RGSKVGncu4Ro/HdyzzY6cmoXuKI2Gffk7vQ==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/template/-/template-7.20.7.tgz",
-            "version": "7.20.7"
+            "resolved": "https://registry.npmjs.org/@babel/template/-/template-7.21.9.tgz",
+            "version": "7.21.9"
         },
         "node_modules/@babel/traverse": {
             "dependencies": {
                 "@babel/code-frame": "^7.21.4",
-                "@babel/generator": "^7.21.5",
-                "@babel/helper-environment-visitor": "^7.21.5",
+                "@babel/generator": "^7.22.3",
+                "@babel/helper-environment-visitor": "^7.22.1",
                 "@babel/helper-function-name": "^7.21.0",
                 "@babel/helper-hoist-variables": "^7.18.6",
                 "@babel/helper-split-export-declaration": "^7.18.6",
-                "@babel/parser": "^7.21.5",
-                "@babel/types": "^7.21.5",
+                "@babel/parser": "^7.22.4",
+                "@babel/types": "^7.22.4",
                 "debug": "^4.1.0",
                 "globals": "^11.1.0"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-AhQoI3YjWi6u/y/ntv7k48mcrCXmus0t79J9qPNlk/lAsFlCiJ047RmbfMOawySTHtywXhbXgpx/8nXMYd+oFw==",
+            "integrity": "sha512-Tn1pDsjIcI+JcLKq1AVlZEr4226gpuAQTsLMorsYg9tuS/kG7nuwwJ4AB8jfQuEgb/COBwR/DqJxmoiYFu5/rQ==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/traverse/-/traverse-7.21.5.tgz",
-            "version": "7.21.5"
+            "resolved": "https://registry.npmjs.org/@babel/traverse/-/traverse-7.22.4.tgz",
+            "version": "7.22.4"
         },
         "node_modules/@babel/types": {
             "dependencies": {
                 "@babel/helper-string-parser": "^7.21.5",
                 "@babel/helper-validator-identifier": "^7.19.1",
                 "to-fast-properties": "^2.0.0"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-m4AfNvVF2mVC/F7fDEdH2El3HzUg9It/XsCxZiOTTA3m3qYfcSVSbTfM6Q9xG+hYDniZssYhlXKKUMD5m8tF4Q==",
+            "integrity": "sha512-Tx9x3UBHTTsMSW85WB2kphxYQVvrZ/t1FxD88IpSgIjiUJlCm9z+xWIDwyo1vffTwSqteqyznB8ZE9vYYk16zA==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@babel/types/-/types-7.21.5.tgz",
-            "version": "7.21.5"
+            "resolved": "https://registry.npmjs.org/@babel/types/-/types-7.22.4.tgz",
+            "version": "7.22.4"
         },
         "node_modules/@colors/colors": {
             "engines": {
                 "node": ">=0.1.90"
             },
             "integrity": "sha512-ooWCrlZP11i8GImSjTHYHLkvFDP48nS4+204nGb1RiX/WXYHmJA2III9/e2DWVabCESdW7hBAEzHRqUn9OUVvQ==",
             "resolved": "https://registry.npmjs.org/@colors/colors/-/colors-1.5.0.tgz",
@@ -6599,18 +6605,18 @@
             "version": "1.0.0-next.21"
         },
         "node_modules/@popperjs/core": {
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/popperjs"
             },
-            "integrity": "sha512-Cr4OjIkipTtcXKjAsm8agyleBuDHvxzeBoa1v543lbv1YaIwQjESsVcmjiWiPEbC1FIeHOG/Op9kdCmAmiS3Kw==",
+            "integrity": "sha512-P1st0aksCrn9sGZhp8GMYwBnQsbvAWsZAX44oXNNvLHGqAOcoVxmjZiohstwQ7SqKnbR47akdNi+uleWD8+g6A==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/@popperjs/core/-/core-2.11.7.tgz",
-            "version": "2.11.7"
+            "resolved": "https://registry.npmjs.org/@popperjs/core/-/core-2.11.8.tgz",
+            "version": "2.11.8"
         },
         "node_modules/@sideway/address": {
             "dependencies": {
                 "@hapi/hoek": "^9.0.0"
             },
             "integrity": "sha512-7vwq+rOHVWjyXxVlR76Agnvhy8I9rpzjosTESvmhNeXOXdZZB15Fl+TI9x1SiHZH5Jv2wTGduSxFDIaq0m3DUw==",
             "resolved": "https://registry.npmjs.org/@sideway/address/-/address-4.1.4.tgz",
@@ -6760,17 +6766,17 @@
             "version": "1.5.0"
         },
         "node_modules/@types/eslint": {
             "dependencies": {
                 "@types/estree": "*",
                 "@types/json-schema": "*"
             },
-            "integrity": "sha512-Piet7dG2JBuDIfohBngQ3rCt7MgO9xCO4xIMKxBThCq5PNRB91IjlJ10eJVwfoNtvTErmxLzwBZ7rHZtbOMmFQ==",
-            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-8.37.0.tgz",
-            "version": "8.37.0"
+            "integrity": "sha512-nbq2mvc/tBrK9zQQuItvjJl++GTN5j06DaPtp3hZCpngmG6Q3xoyEmd0TwZI0gAy/G1X0zhGBbr2imsGFdFV0g==",
+            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-8.40.0.tgz",
+            "version": "8.40.0"
         },
         "node_modules/@types/eslint-scope": {
             "dependencies": {
                 "@types/eslint": "*",
                 "@types/estree": "*"
             },
             "integrity": "sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==",
@@ -6796,17 +6802,17 @@
         "node_modules/@types/express-serve-static-core": {
             "dependencies": {
                 "@types/node": "*",
                 "@types/qs": "*",
                 "@types/range-parser": "*",
                 "@types/send": "*"
             },
-            "integrity": "sha512-fvr49XlCGoUj2Pp730AItckfjat4WNb0lb3kfrLWffd+RLeoGAMsq7UOy04PAPtoL01uKwcp6u8nhzpgpDYr3w==",
-            "resolved": "https://registry.npmjs.org/@types/express-serve-static-core/-/express-serve-static-core-4.17.34.tgz",
-            "version": "4.17.34"
+            "integrity": "sha512-wALWQwrgiB2AWTT91CB62b6Yt0sNHpznUXeZEcnPU3DRdlDIz74x8Qg1UUYKSVFi+va5vKOLYRBI1bRKiLLKIg==",
+            "resolved": "https://registry.npmjs.org/@types/express-serve-static-core/-/express-serve-static-core-4.17.35.tgz",
+            "version": "4.17.35"
         },
         "node_modules/@types/html-minifier-terser": {
             "integrity": "sha512-oh/6byDPnL1zeNXFrDXFLyZjkr1MsBG667IM792caf1L2UPOOMf65NFzjUH/ltyfwjAGfs1rsX1eftK0jC/KIg==",
             "resolved": "https://registry.npmjs.org/@types/html-minifier-terser/-/html-minifier-terser-6.1.0.tgz",
             "version": "6.1.0"
         },
         "node_modules/@types/http-proxy": {
@@ -6814,32 +6820,32 @@
                 "@types/node": "*"
             },
             "integrity": "sha512-HC8G7c1WmaF2ekqpnFq626xd3Zz0uvaqFmBJNRZCGEZCXkvSdJoNFn/8Ygbd9fKNQj8UzLdCETaI0UWPAjK7IA==",
             "resolved": "https://registry.npmjs.org/@types/http-proxy/-/http-proxy-1.17.11.tgz",
             "version": "1.17.11"
         },
         "node_modules/@types/json-schema": {
-            "integrity": "sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==",
-            "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.11.tgz",
-            "version": "7.0.11"
+            "integrity": "sha512-Hr5Jfhc9eYOQNPYO5WLDq/n4jqijdHNlDXjuAQkkt+mWdQR+XJToOHrsD4cPaMXpn6KO7y2+wM8AZEs8VpBLVA==",
+            "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.12.tgz",
+            "version": "7.0.12"
         },
         "node_modules/@types/mime": {
             "integrity": "sha512-YATxVxgRqNH6nHEIsvg6k2Boc1JHI9ZbH5iWFFv/MTkchz3b1ieGDa5T0a9RznNdI0KhVbdbWSN+KWWrQZRxTw==",
             "resolved": "https://registry.npmjs.org/@types/mime/-/mime-1.3.2.tgz",
             "version": "1.3.2"
         },
         "node_modules/@types/minimist": {
             "integrity": "sha512-jhuKLIRrhvCPLqwPcx6INqmKeiA5EWrsCOPhrlFSrbrmU4ZMPjj5Ul/oLCMDO98XRUIwVm78xICz4EPCektzeQ==",
             "resolved": "https://registry.npmjs.org/@types/minimist/-/minimist-1.2.2.tgz",
             "version": "1.2.2"
         },
         "node_modules/@types/node": {
-            "integrity": "sha512-O+z53uwx64xY7D6roOi4+jApDGFg0qn6WHcxe5QeqjMaTezBO/mxdfFXIVAVVyNWKx84OmPB3L8kbVYOTeN34A==",
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.1.0.tgz",
-            "version": "20.1.0"
+            "integrity": "sha512-JJulVEQXmiY9Px5axXHeYGLSjhkZEnD+MDPDGbCbIAbMslkKwmygtZFy1X6s/075Yo94sf8GuSlFfPzysQrWZQ==",
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.2.5.tgz",
+            "version": "20.2.5"
         },
         "node_modules/@types/normalize-package-data": {
             "integrity": "sha512-Gj7cI7z+98M282Tqmp2K5EIsoouUEzbBJhQQzDE3jSIRk6r9gsz0oUokqIUR4u1R3dMHo0pDHM7sNOHyhulypw==",
             "resolved": "https://registry.npmjs.org/@types/normalize-package-data/-/normalize-package-data-2.4.1.tgz",
             "version": "2.4.1"
         },
         "node_modules/@types/parse-json": {
@@ -7120,17 +7126,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
-            "version": "7.5.0"
+            "integrity": "sha512-Wvss5ivl8TMRZXXESstBA4uR5iXgEN/VC5/sOcuXdVLzcdkz4HWetIoRfG5gb5X+ij/G9rw9YoGn3QoQ8OCSpw==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.1.tgz",
+            "version": "7.5.1"
         },
         "node_modules/@vue/cli-shared-utils/node_modules/supports-color": {
             "dependencies": {
                 "has-flag": "^4.0.0"
             },
             "engines": {
                 "node": ">=8"
@@ -7235,142 +7241,142 @@
         "node_modules/@vue/web-component-wrapper": {
             "integrity": "sha512-Iu8Tbg3f+emIIMmI2ycSI8QcEuAUgPTgHwesDU1eKMLE4YC/c/sFbGc70QgMq31ijRftV0R7vCm9co6rldCeOA==",
             "resolved": "https://registry.npmjs.org/@vue/web-component-wrapper/-/web-component-wrapper-1.3.0.tgz",
             "version": "1.3.0"
         },
         "node_modules/@webassemblyjs/ast": {
             "dependencies": {
-                "@webassemblyjs/helper-numbers": "1.11.5",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.5"
+                "@webassemblyjs/helper-numbers": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6"
             },
-            "integrity": "sha512-LHY/GSAZZRpsNQH+/oHqhRQ5FT7eoULcBqgfyTB5nQHogFnK3/7QoN7dLnwSE/JkUAF0SrRuclT7ODqMFtWxxQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-IN1xI7PwOvLPgjcf180gC1bqn3q/QaOCwYUahIOhbYUu8KA/3tw2RT/T0Gidi1l7Hhj5D/INhJxiICObqpMu4Q==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/floating-point-hex-parser": {
-            "integrity": "sha512-1j1zTIC5EZOtCplMBG/IEwLtUojtwFVwdyVMbL/hwWqbzlQoJsWCOavrdnLkemwNoC/EOwtUFch3fuo+cbcXYQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-ejAj9hfRJ2XMsNHk/v6Fu2dGS+i4UaXBXGemOfQ/JfQ6mdQg/WXtwleQRLLS4OvfDhv8rYnVwH27YJLMyYsxhw==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/helper-api-error": {
-            "integrity": "sha512-L65bDPmfpY0+yFrsgz8b6LhXmbbs38OnwDCf6NpnMUYqa+ENfE5Dq9E42ny0qz/PdR0LJyq/T5YijPnU8AXEpA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-o0YkoP4pVu4rN8aTJgAyj9hC2Sv5UlkzCHhxqWj8butaLvnpdc2jOwh4ewE6CX0txSfLn/UYaV/pheS2Txg//Q==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/helper-buffer": {
-            "integrity": "sha512-fDKo1gstwFFSfacIeH5KfwzjykIE6ldh1iH9Y/8YkAZrhmu4TctqYjSh7t0K2VyDSXOZJ1MLhht/k9IvYGcIxg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-z3nFzdcp1mb8nEOFFk8DrYLpHvhKC3grJD2ardfKOzmbmJvEf/tPIqCY+sNcwZIY8ZD7IkB2l7/pqhUhqm7hLA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/helper-numbers": {
             "dependencies": {
-                "@webassemblyjs/floating-point-hex-parser": "1.11.5",
-                "@webassemblyjs/helper-api-error": "1.11.5",
+                "@webassemblyjs/floating-point-hex-parser": "1.11.6",
+                "@webassemblyjs/helper-api-error": "1.11.6",
                 "@xtuc/long": "4.2.2"
             },
-            "integrity": "sha512-DhykHXM0ZABqfIGYNv93A5KKDw/+ywBFnuWybZZWcuzWHfbp21wUfRkbtz7dMGwGgT4iXjWuhRMA2Mzod6W4WA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-vUIhZ8LZoIWHBohiEObxVm6hwP034jwmc9kuq5GdHZH0wiLVLIPcMCdpJzG4C11cHoQ25TFIQj9kaVADVX7N3g==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/helper-wasm-bytecode": {
-            "integrity": "sha512-oC4Qa0bNcqnjAowFn7MPCETQgDYytpsfvz4ujZz63Zu/a/v71HeCAAmZsgZ3YVKec3zSPYytG3/PrRCqbtcAvA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-sFFHKwcmBprO9e7Icf0+gddyWYDViL8bpPjJJl0WHxCdETktXdmtWLGVzoHbqUcY4Be1LkNfwTmXOJUFZYSJdA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/helper-wasm-section": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.5",
-                "@webassemblyjs/helper-buffer": "1.11.5",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
-                "@webassemblyjs/wasm-gen": "1.11.5"
-            },
-            "integrity": "sha512-uEoThA1LN2NA+K3B9wDo3yKlBfVtC6rh0i4/6hvbz071E8gTNZD/pT0MsBf7MeD6KbApMSkaAK0XeKyOZC7CIA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.5.tgz",
-            "version": "1.11.5"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/wasm-gen": "1.11.6"
+            },
+            "integrity": "sha512-LPpZbSOwTpEC2cgn4hTydySy1Ke+XEu+ETXuoyvuyezHO3Kjdu90KK95Sh9xTbmjrCsUwvWwCOQQNta37VrS9g==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/ieee754": {
             "dependencies": {
                 "@xtuc/ieee754": "^1.2.0"
             },
-            "integrity": "sha512-37aGq6qVL8A8oPbPrSGMBcp38YZFXcHfiROflJn9jxSdSMMM5dS5P/9e2/TpaJuhE+wFrbukN2WI6Hw9MH5acg==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-LM4p2csPNvbij6U1f19v6WR56QZ8JcHg3QIJTlSwzFcmx6WSORicYj6I63f9yU1kEUtrpG+kjkiIAkevHpDXrg==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/leb128": {
             "dependencies": {
                 "@xtuc/long": "4.2.2"
             },
-            "integrity": "sha512-ajqrRSXaTJoPW+xmkfYN6l8VIeNnR4vBOTQO9HzR7IygoCcKWkICbKFbVTNMjMgMREqXEr0+2M6zukzM47ZUfQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-m7a0FhE67DQXgouf1tbN5XQcdWoNgaAuoULHIfGFIEVKA6tu/edls6XnIlkmS6FrXAquJRPni3ZZKjw6FSPjPQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/utf8": {
-            "integrity": "sha512-WiOhulHKTZU5UPlRl53gHR8OxdGsSOxqfpqWeA2FmcwBMaoEdz6b2x2si3IwC9/fSPLfe8pBMRTHVMk5nlwnFQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-vtXf2wTQ3+up9Zsg8sa2yWiQpzSsMyXj0qViVP6xKGCUT8p8YJ6HqI7l5eCnWx1T/FYdsv07HQs2wTFbbof/RA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/wasm-edit": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.5",
-                "@webassemblyjs/helper-buffer": "1.11.5",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
-                "@webassemblyjs/helper-wasm-section": "1.11.5",
-                "@webassemblyjs/wasm-gen": "1.11.5",
-                "@webassemblyjs/wasm-opt": "1.11.5",
-                "@webassemblyjs/wasm-parser": "1.11.5",
-                "@webassemblyjs/wast-printer": "1.11.5"
-            },
-            "integrity": "sha512-C0p9D2fAu3Twwqvygvf42iGCQ4av8MFBLiTb+08SZ4cEdwzWx9QeAHDo1E2k+9s/0w1DM40oflJOpkZ8jW4HCQ==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.5.tgz",
-            "version": "1.11.5"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/helper-wasm-section": "1.11.6",
+                "@webassemblyjs/wasm-gen": "1.11.6",
+                "@webassemblyjs/wasm-opt": "1.11.6",
+                "@webassemblyjs/wasm-parser": "1.11.6",
+                "@webassemblyjs/wast-printer": "1.11.6"
+            },
+            "integrity": "sha512-Ybn2I6fnfIGuCR+Faaz7YcvtBKxvoLV3Lebn1tM4o/IAJzmi9AWYIPWpyBfU8cC+JxAO57bk4+zdsTjJR+VTOw==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/wasm-gen": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.5",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
-                "@webassemblyjs/ieee754": "1.11.5",
-                "@webassemblyjs/leb128": "1.11.5",
-                "@webassemblyjs/utf8": "1.11.5"
-            },
-            "integrity": "sha512-14vteRlRjxLK9eSyYFvw1K8Vv+iPdZU0Aebk3j6oB8TQiQYuO6hj9s4d7qf6f2HJr2khzvNldAFG13CgdkAIfA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.5.tgz",
-            "version": "1.11.5"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/ieee754": "1.11.6",
+                "@webassemblyjs/leb128": "1.11.6",
+                "@webassemblyjs/utf8": "1.11.6"
+            },
+            "integrity": "sha512-3XOqkZP/y6B4F0PBAXvI1/bky7GryoogUtfwExeP/v7Nzwo1QLcq5oQmpKlftZLbT+ERUOAZVQjuNVak6UXjPA==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/wasm-opt": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.5",
-                "@webassemblyjs/helper-buffer": "1.11.5",
-                "@webassemblyjs/wasm-gen": "1.11.5",
-                "@webassemblyjs/wasm-parser": "1.11.5"
-            },
-            "integrity": "sha512-tcKwlIXstBQgbKy1MlbDMlXaxpucn42eb17H29rawYLxm5+MsEmgPzeCP8B1Cl69hCice8LeKgZpRUAPtqYPgw==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.5.tgz",
-            "version": "1.11.5"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-buffer": "1.11.6",
+                "@webassemblyjs/wasm-gen": "1.11.6",
+                "@webassemblyjs/wasm-parser": "1.11.6"
+            },
+            "integrity": "sha512-cOrKuLRE7PCe6AsOVl7WasYf3wbSo4CeOk6PkrjS7g57MFfVUF9u6ysQBBODX0LdgSvQqRiGz3CXvIDKcPNy4g==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/wasm-parser": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.5",
-                "@webassemblyjs/helper-api-error": "1.11.5",
-                "@webassemblyjs/helper-wasm-bytecode": "1.11.5",
-                "@webassemblyjs/ieee754": "1.11.5",
-                "@webassemblyjs/leb128": "1.11.5",
-                "@webassemblyjs/utf8": "1.11.5"
-            },
-            "integrity": "sha512-SVXUIwsLQlc8srSD7jejsfTU83g7pIGr2YYNb9oHdtldSxaOhvA5xwvIiWIfcX8PlSakgqMXsLpLfbbJ4cBYew==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.5.tgz",
-            "version": "1.11.5"
+                "@webassemblyjs/ast": "1.11.6",
+                "@webassemblyjs/helper-api-error": "1.11.6",
+                "@webassemblyjs/helper-wasm-bytecode": "1.11.6",
+                "@webassemblyjs/ieee754": "1.11.6",
+                "@webassemblyjs/leb128": "1.11.6",
+                "@webassemblyjs/utf8": "1.11.6"
+            },
+            "integrity": "sha512-6ZwPeGzMJM3Dqp3hCsLgESxBGtT/OeCvCZ4TA1JUPYgmhAx38tTPR9JaKy0S5H3evQpO/h2uWs2j6Yc/fjkpTQ==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@webassemblyjs/wast-printer": {
             "dependencies": {
-                "@webassemblyjs/ast": "1.11.5",
+                "@webassemblyjs/ast": "1.11.6",
                 "@xtuc/long": "4.2.2"
             },
-            "integrity": "sha512-f7Pq3wvg3GSPUPzR0F6bmI89Hdb+u9WXrSKc4v+N0aV0q6r42WoF92Jp2jEorBEBRoRNXgjp53nBniDXcqZYPA==",
-            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.5.tgz",
-            "version": "1.11.5"
+            "integrity": "sha512-JM7AhRcE+yW2GWYaKeHL5vt4xqee5N2WcezptmgyhNS+ScggqcT1OtXykhAb13Sn5Yas0j2uv9tHgrjwvzAP4A==",
+            "resolved": "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.6.tgz",
+            "version": "1.11.6"
         },
         "node_modules/@xtuc/ieee754": {
             "integrity": "sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==",
             "resolved": "https://registry.npmjs.org/@xtuc/ieee754/-/ieee754-1.2.0.tgz",
             "version": "1.2.0"
         },
         "node_modules/@xtuc/long": {
@@ -7398,20 +7404,20 @@
                 "node": ">=0.4.0"
             },
             "integrity": "sha512-xjIYgE8HBrkpd/sJqOGNspf8uHG+NOHGOw6a/Urj8taM2EXfdNAH2oFcPeIFfsv3+kz/mJrS5VuMqbNLjCa2vw==",
             "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.8.2.tgz",
             "version": "8.8.2"
         },
         "node_modules/acorn-import-assertions": {
-            "integrity": "sha512-m7VZ3jwz4eK6A4Vtt8Ew1/mNbP24u0FhdyfA7fSvnJR6LMdfOYnmuIrrJAgrYfYJ10F/otaHTtrtrtmHdMNzEw==",
+            "integrity": "sha512-cmMwop9x+8KFhxvKrKfPYmN6/pKTYYHBqLa0DfvVZcKMJWNyWLnaqND7dx/qn66R7ewM1UX5XMaDVP5wlVTaVA==",
             "peerDependencies": {
                 "acorn": "^8"
             },
-            "resolved": "https://registry.npmjs.org/acorn-import-assertions/-/acorn-import-assertions-1.8.0.tgz",
-            "version": "1.8.0"
+            "resolved": "https://registry.npmjs.org/acorn-import-assertions/-/acorn-import-assertions-1.9.0.tgz",
+            "version": "1.9.0"
         },
         "node_modules/acorn-walk": {
             "engines": {
                 "node": ">=0.4.0"
             },
             "integrity": "sha512-k+iyHEuPgSw6SbuDpGQM+06HQUa04DZ3o+F6CSzXMvvI5KMvnaEqXe+YVe555R9nn6GPt404fos4wcgpw12SDA==",
             "resolved": "https://registry.npmjs.org/acorn-walk/-/acorn-walk-8.2.0.tgz",
@@ -7767,21 +7773,21 @@
                     "url": "https://github.com/sponsors/twbs"
                 },
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/bootstrap"
                 }
             ],
-            "integrity": "sha512-cEKPM+fwb3cT8NzQZYEu4HilJ3anCrWqh3CHAok1p9jXqMPsPTBhU25fBckEJHJ/p+tTxTFTsFQGM+gaHpi3QQ==",
+            "integrity": "sha512-UnBV3E3v4STVNQdms6jSGO2CvOkjUMdDAVR2V5N4uCMdaIkaQjbcEAMqRimDHIs4uqBYzDAKCQwCB+97tJgHQw==",
             "name": "bootstrap",
             "peerDependencies": {
-                "@popperjs/core": "^2.11.6"
+                "@popperjs/core": "^2.11.7"
             },
-            "resolved": "https://registry.npmjs.org/bootstrap/-/bootstrap-5.2.3.tgz",
-            "version": "5.2.3"
+            "resolved": "https://registry.npmjs.org/bootstrap/-/bootstrap-5.3.0.tgz",
+            "version": "5.3.0"
         },
         "node_modules/brace-expansion": {
             "dependencies": {
                 "balanced-match": "^1.0.0"
             },
             "integrity": "sha512-XnAIvQ8eM+kC6aULx6wuQiwVsnzsi9d3WxzV3FpWTGA19F621kwdbsAcFKXgKUHZWsy+mY6iL1sHTxWEFCytDA==",
             "resolved": "https://registry.npmjs.org/brace-expansion/-/brace-expansion-2.0.1.tgz",
@@ -7807,35 +7813,39 @@
             "version": "1.3.3"
         },
         "node_modules/browserslist": {
             "bin": {
                 "browserslist": "cli.js"
             },
             "dependencies": {
-                "caniuse-lite": "^1.0.30001449",
-                "electron-to-chromium": "^1.4.284",
-                "node-releases": "^2.0.8",
-                "update-browserslist-db": "^1.0.10"
+                "caniuse-lite": "^1.0.30001489",
+                "electron-to-chromium": "^1.4.411",
+                "node-releases": "^2.0.12",
+                "update-browserslist-db": "^1.0.11"
             },
             "engines": {
                 "node": "^6 || ^7 || ^8 || ^9 || ^10 || ^11 || ^12 || >=13.7"
             },
             "funding": [
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/browserslist"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/browserslist"
+                },
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-tUkiguQGW7S3IhB7N+c2MV/HZPSCPAAiYBZXLsBhFB/PCy6ZKKsZrmBayHV9fdGV/ARIfJ14NkxKzRDjvp7L6w==",
-            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.21.5.tgz",
-            "version": "4.21.5"
+            "integrity": "sha512-BauCXrQ7I2ftSqd2mvKHGo85XR0u7Ru3C/Hxsy/0TkfCtjrmAbPdzLGasmoiBxplpDXlPvdjX9u7srIMfgasNA==",
+            "resolved": "https://registry.npmjs.org/browserslist/-/browserslist-4.21.7.tgz",
+            "version": "4.21.7"
         },
         "node_modules/buffer": {
             "dependencies": {
                 "base64-js": "^1.3.1",
                 "ieee754": "^1.1.13"
             },
             "funding": [
@@ -7920,17 +7930,17 @@
                     "url": "https://tidelift.com/funding/github/npm/caniuse-lite"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-uv7/gXuHi10Whlj0pp5q/tsK/32J2QSqVRKQhs2j8VsDCjgyruAh/eEXHF822VqO9yT6iZKw3nRwZRSPBE9OQg==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001486.tgz",
-            "version": "1.0.30001486"
+            "integrity": "sha512-F6x5IEuigtUfU5ZMQK2jsy5JqUUlEFRVZq8bO2a+ysq5K7jD6PPc9YXZj78xDNS3uNchesp1Jw47YXEqr+Viyg==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001495.tgz",
+            "version": "1.0.30001495"
         },
         "node_modules/case-sensitive-paths-webpack-plugin": {
             "engines": {
                 "node": ">=4"
             },
             "integrity": "sha512-roIFONhcxog0JSSWbvVAh3OocukmSgpqOH6YpMkCvav/ySIV3JKg4Dc8vYtQjYi/UxpNE36r/9v+VqTQqgkYmw==",
             "resolved": "https://registry.npmjs.org/case-sensitive-paths-webpack-plugin/-/case-sensitive-paths-webpack-plugin-2.4.0.tgz",
@@ -8536,35 +8546,35 @@
             },
             "resolved": "https://registry.npmjs.org/css-declaration-sorter/-/css-declaration-sorter-6.4.0.tgz",
             "version": "6.4.0"
         },
         "node_modules/css-loader": {
             "dependencies": {
                 "icss-utils": "^5.1.0",
-                "postcss": "^8.4.19",
+                "postcss": "^8.4.21",
                 "postcss-modules-extract-imports": "^3.0.0",
-                "postcss-modules-local-by-default": "^4.0.0",
+                "postcss-modules-local-by-default": "^4.0.3",
                 "postcss-modules-scope": "^3.0.0",
                 "postcss-modules-values": "^4.0.0",
                 "postcss-value-parser": "^4.2.0",
                 "semver": "^7.3.8"
             },
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-qhOH1KlBMnZP8FzRO6YCH9UHXQhVMcEGLyNdb7Hv2cpcmJbW0YrddO+tG1ab5nT41KpHIYGsbeHqxB9xPu1pKQ==",
+            "integrity": "sha512-xDAXtEVGlD0gJ07iclwWVkLoZOpEvAWaSyf6W18S2pOC//K8+qUDIx8IIT3D+HjnmkJPQeesOPv5aiUaJsCM2g==",
             "peerDependencies": {
                 "webpack": "^5.0.0"
             },
-            "resolved": "https://registry.npmjs.org/css-loader/-/css-loader-6.7.3.tgz",
-            "version": "6.7.3"
+            "resolved": "https://registry.npmjs.org/css-loader/-/css-loader-6.8.1.tgz",
+            "version": "6.8.1"
         },
         "node_modules/css-loader/node_modules/lru-cache": {
             "dependencies": {
                 "yallist": "^4.0.0"
             },
             "engines": {
                 "node": ">=10"
@@ -8579,17 +8589,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
-            "version": "7.5.0"
+            "integrity": "sha512-Wvss5ivl8TMRZXXESstBA4uR5iXgEN/VC5/sOcuXdVLzcdkz4HWetIoRfG5gb5X+ij/G9rw9YoGn3QoQ8OCSpw==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.1.tgz",
+            "version": "7.5.1"
         },
         "node_modules/css-loader/node_modules/yallist": {
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/css-minimizer-webpack-plugin": {
@@ -8670,17 +8680,17 @@
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
-            "version": "4.0.1"
+            "integrity": "sha512-Jw+GZVbP5IggB2WAn6UHI02LBwGmsIeYN/lNbSMZyDziQ7jmtAUrqKqDja+W89YHVs+KL/3IkIMltAklqB1vAw==",
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.1.0.tgz",
+            "version": "4.1.0"
         },
         "node_modules/css-select": {
             "dependencies": {
                 "boolbase": "^1.0.0",
                 "css-what": "^6.0.1",
                 "domhandler": "^4.3.1",
                 "domutils": "^2.8.0",
@@ -9172,17 +9182,17 @@
         },
         "node_modules/ee-first": {
             "integrity": "sha512-WMwm9LhRUo+WUaRN+vRuETqG89IgZphVSNkdFgeb6sS/E4OrDIN7t48CAewSHXc6C8lefD8KKfr5vY61brQlow==",
             "resolved": "https://registry.npmjs.org/ee-first/-/ee-first-1.1.1.tgz",
             "version": "1.1.1"
         },
         "node_modules/electron-to-chromium": {
-            "integrity": "sha512-L9zlje9bIw0h+CwPQumiuVlfMcV4boxRjFIWDcLfFqTZNbkwOExBzfmswytHawObQX4OUhtNv8gIiB21kOurIg==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.385.tgz",
-            "version": "1.4.385"
+            "integrity": "sha512-wv1NufHxu11zfDbY4fglYQApMswleE9FL/DSeyOyauVXDZ+Kco96JK/tPfBUaDqfRarYp2WH2hJ/5UnVywp9Jg==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.425.tgz",
+            "version": "1.4.425"
         },
         "node_modules/emoji-regex": {
             "integrity": "sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==",
             "resolved": "https://registry.npmjs.org/emoji-regex/-/emoji-regex-8.0.0.tgz",
             "version": "8.0.0"
         },
         "node_modules/emojis-list": {
@@ -9218,17 +9228,17 @@
             "dependencies": {
                 "graceful-fs": "^4.2.4",
                 "tapable": "^2.2.0"
             },
             "engines": {
                 "node": ">=10.13.0"
             },
-            "integrity": "sha512-eyV8f0y1+bzyfh8xAwW/WTSZpLbjhqc4ne9eGSH4Zo2ejdyiNG9pU6mf9DG8a7+Auk6MFTlNOT4Y2y/9k8GKVg==",
-            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.13.0.tgz",
-            "version": "5.13.0"
+            "integrity": "sha512-Vklwq2vDKtl0y/vtwjSesgJ5MYS7Etuk5txS8VdKL4AOS1aUlD96zqIfsOSLQsdv3xgMRbtkWM8eG9XDfKUPow==",
+            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.14.1.tgz",
+            "version": "5.14.1"
         },
         "node_modules/entities": {
             "funding": {
                 "url": "https://github.com/fb55/entities?sponsor=1"
             },
             "integrity": "sha512-p92if5Nz619I0w+akJrLZH0MX0Pb5DX39XOwQTtXSdQQOaYH03S1uIQp4mhOZtAXrxq4ViO67YTiLBo2638o9A==",
             "resolved": "https://registry.npmjs.org/entities/-/entities-2.2.0.tgz",
@@ -9676,17 +9686,17 @@
                 "node": ">=10"
             },
             "integrity": "sha512-hcg3ZmepS30/7BSFqRvoo3DOMQu7IjqxO5nCDt+zM9XWjb33Wg7ziNT+Qvqbuc3+gWpzO02JubVyk2G4Zvo1OQ==",
             "resolved": "https://registry.npmjs.org/fs-extra/-/fs-extra-9.1.0.tgz",
             "version": "9.1.0"
         },
         "node_modules/fs-monkey": {
-            "integrity": "sha512-cybjIfiiE+pTWicSCLFHSrXZ6EilF30oh91FDP9S2B051prEa7QWfrVTQm10/dDpswBDXZugPa1Ogu8Yh+HV0Q==",
-            "resolved": "https://registry.npmjs.org/fs-monkey/-/fs-monkey-1.0.3.tgz",
-            "version": "1.0.3"
+            "integrity": "sha512-INM/fWAxMICjttnD0DX1rBvinKskj5G1w+oy/pnm9u/tSlnBrzFonJMcalKJ30P8RRsPzKcCG7Q8l0jx5Fh9YQ==",
+            "resolved": "https://registry.npmjs.org/fs-monkey/-/fs-monkey-1.0.4.tgz",
+            "version": "1.0.4"
         },
         "node_modules/fs.realpath": {
             "integrity": "sha512-OO0pH2lK6a0hZnAdau5ItzHPI6pUlvI7jMVnxUQRtw4owF2wk8lOSabtGDCTP4Ggrg2MbGnWO9X8K1t4+fGMDw==",
             "resolved": "https://registry.npmjs.org/fs.realpath/-/fs.realpath-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/fsevents": {
@@ -9724,22 +9734,23 @@
             "resolved": "https://registry.npmjs.org/get-caller-file/-/get-caller-file-2.0.5.tgz",
             "version": "2.0.5"
         },
         "node_modules/get-intrinsic": {
             "dependencies": {
                 "function-bind": "^1.1.1",
                 "has": "^1.0.3",
+                "has-proto": "^1.0.1",
                 "has-symbols": "^1.0.3"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-L049y6nFOuom5wGyRc3/gdTLO94dySVKRACj1RmJZBQXlbTMhtNIgkWkUHq+jYmZvKf14EW1EoJnnjbmoHij0Q==",
-            "resolved": "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.0.tgz",
-            "version": "1.2.0"
+            "integrity": "sha512-2DcsyfABl+gVHEfCOaTrWgyt+tb6MSEGmKq+kI5HwLbIYgjgmMcV8KQ41uaKz1xxUcn9tJtgFbQUEVcEbd0FYw==",
+            "resolved": "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.1.tgz",
+            "version": "1.2.1"
         },
         "node_modules/get-stream": {
             "dependencies": {
                 "pump": "^3.0.0"
             },
             "engines": {
                 "node": ">=6"
@@ -9854,14 +9865,25 @@
             "engines": {
                 "node": ">=4"
             },
             "integrity": "sha512-sKJf1+ceQBr4SMkvQnBDNDtf4TXpVhVGateu0t918bl30FnbE2m4vNLX+VWe/dpjlb+HugGYzW7uQXH98HPEYw==",
             "resolved": "https://registry.npmjs.org/has-flag/-/has-flag-3.0.0.tgz",
             "version": "3.0.0"
         },
+        "node_modules/has-proto": {
+            "engines": {
+                "node": ">= 0.4"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/ljharb"
+            },
+            "integrity": "sha512-7qE+iP+O+bgF9clE5+UoBFzE65mlBiVj3tKCrlNQ0Ogwm0BjpT/gK4SlLYDMybDh5I3TCTKnPPa0oMG7JDYrhg==",
+            "resolved": "https://registry.npmjs.org/has-proto/-/has-proto-1.0.1.tgz",
+            "version": "1.0.1"
+        },
         "node_modules/has-symbols": {
             "engines": {
                 "node": ">= 0.4"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
@@ -9935,17 +9957,17 @@
         },
         "node_modules/hsluv": {
             "integrity": "sha512-08iL2VyCRbkQKBySkSh6m8zMUa3sADAxGVWs3Z1aPcUkTJeK0ETG4Fc27tEmQBGUAXZjIsXOZqBvacuVNSC/fQ==",
             "resolved": "https://registry.npmjs.org/hsluv/-/hsluv-0.0.3.tgz",
             "version": "0.0.3"
         },
         "node_modules/html-entities": {
-            "integrity": "sha512-DV5Ln36z34NNTDgnz0EWGBLZENelNAtkiFA4kyNOG2tDI6Mz1uSWiq1wAKdyjnJwyDiDO7Fa2SO1CTxPXL8VxA==",
-            "resolved": "https://registry.npmjs.org/html-entities/-/html-entities-2.3.3.tgz",
-            "version": "2.3.3"
+            "integrity": "sha512-72TJlcMkYsEJASa/3HnX7VT59htM7iSHbH59NSZbtc+22Ap0Txnlx91sfeB+/A7wNZg7UxtZdhAW4y+/jimrdg==",
+            "resolved": "https://registry.npmjs.org/html-entities/-/html-entities-2.3.5.tgz",
+            "version": "2.3.5"
         },
         "node_modules/html-minifier-terser": {
             "bin": {
                 "html-minifier-terser": "cli.js"
             },
             "dependencies": {
                 "camel-case": "^4.1.2",
@@ -10187,17 +10209,17 @@
         "node_modules/is-core-module": {
             "dependencies": {
                 "has": "^1.0.3"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-RECHCBCd/viahWmwj6enj19sKbHfJrddi/6cBDsNTKbNq0f7VeaUkBo60BqzvPqo/W54ChS62Z5qyun7cfOMqQ==",
-            "resolved": "https://registry.npmjs.org/is-core-module/-/is-core-module-2.12.0.tgz",
-            "version": "2.12.0"
+            "integrity": "sha512-Q4ZuBAe2FUsKtyQJoQHlvP8OvBERxO3jEmy1I7hcRXcJBGGHFh/aJBswbXuS9sgrDH2QUO8ilkwNPHvHMd8clg==",
+            "resolved": "https://registry.npmjs.org/is-core-module/-/is-core-module-2.12.1.tgz",
+            "version": "2.12.1"
         },
         "node_modules/is-docker": {
             "bin": {
                 "is-docker": "cli.js"
             },
             "engines": {
                 "node": ">=8"
@@ -10379,18 +10401,18 @@
                 "@sideway/pinpoint": "^2.0.0"
             },
             "integrity": "sha512-Itk/r+V4Dx0V3c7RLFdRh12IOjySm2/WGPMubBT92cQvRfYZhPM2W0hZlctjj72iES8jsRCwp7S/cRmWBnJ4nw==",
             "resolved": "https://registry.npmjs.org/joi/-/joi-17.9.2.tgz",
             "version": "17.9.2"
         },
         "node_modules/jquery": {
-            "integrity": "sha512-v28EW9DWDFpzcD9O5iyJXg3R3+q+mET5JhnjJzQUZMHOv67bpSIHq81GEYpPNZHG+XXHsfSme3nxp/hndKEcsQ==",
+            "integrity": "sha512-umpJ0/k8X0MvD1ds0P9SfowREz2LenHsQaxSohMZ5OMNEU2r0tf8pdeEFTHMFxWVxKNyU9rTtK3CWzUCTKJUeQ==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/jquery/-/jquery-3.6.4.tgz",
-            "version": "3.6.4"
+            "resolved": "https://registry.npmjs.org/jquery/-/jquery-3.7.0.tgz",
+            "version": "3.7.0"
         },
         "node_modules/js-message": {
             "engines": {
                 "node": ">=0.6.0"
             },
             "integrity": "sha512-efJLHhLjIyKRewNS9EGZ4UpI8NguuL6fKkhRxVuMmrGV2xN/0APGdQYwLFky5w9naebSZ0OwAGp0G6/2Cg90rA==",
             "resolved": "https://registry.npmjs.org/js-message/-/js-message-1.0.7.tgz",
@@ -10799,22 +10821,22 @@
             },
             "integrity": "sha512-dq+qelQ9akHpcOl/gUVRTxVIOkAJ1wR3QAvb4RsVjS8oVoFjDGTc679wJYmUmknUF5HwMLOgb5O+a3KxfWapPQ==",
             "resolved": "https://registry.npmjs.org/media-typer/-/media-typer-0.3.0.tgz",
             "version": "0.3.0"
         },
         "node_modules/memfs": {
             "dependencies": {
-                "fs-monkey": "^1.0.3"
+                "fs-monkey": "^1.0.4"
             },
             "engines": {
                 "node": ">= 4.0.0"
             },
-            "integrity": "sha512-UWbFJKvj5k+nETdteFndTpYxdeTMox/ULeqX5k/dpaQJCCFmj5EeKv3dBcyO2xmkRAx2vppRu5dVG7SOtsGOzA==",
-            "resolved": "https://registry.npmjs.org/memfs/-/memfs-3.5.1.tgz",
-            "version": "3.5.1"
+            "integrity": "sha512-UERzLsxzllchadvbPs5aolHh65ISpKpM+ccLbOJ8/vvpBKmAWf+la7dXFy7Mr0ySHbdHrFv5kGFCUHHe6GFEmw==",
+            "resolved": "https://registry.npmjs.org/memfs/-/memfs-3.5.3.tgz",
+            "version": "3.5.3"
         },
         "node_modules/merge-descriptors": {
             "integrity": "sha512-cCi6g3/Zr1iqQi6ySbseM1Xvooa98N0w31jzUYrXPX2xqObmFGHJ0tQ5u74H3mVh7wLouTseZyYIq39g8cNp1w==",
             "resolved": "https://registry.npmjs.org/merge-descriptors/-/merge-descriptors-1.0.1.tgz",
             "version": "1.0.1"
         },
         "node_modules/merge-source-map": {
@@ -10914,20 +10936,20 @@
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-9HaR++0mlgom81s95vvNjxkg52n2b5s//3ZTI1EtzFb98awsLSivs2LMsVqnQ3ay0PVhqWcGNyDaTE961FOcjQ==",
+            "integrity": "sha512-Qk7HcgaPkGG6eD77mLvZS1nmxlao3j+9PkrT9Uc7HAE1id3F41+DdBRYRYkbyfNRGzm8/YWtzhw7nVPmwhqTQw==",
             "peerDependencies": {
                 "webpack": "^5.0.0"
             },
-            "resolved": "https://registry.npmjs.org/mini-css-extract-plugin/-/mini-css-extract-plugin-2.7.5.tgz",
-            "version": "2.7.5"
+            "resolved": "https://registry.npmjs.org/mini-css-extract-plugin/-/mini-css-extract-plugin-2.7.6.tgz",
+            "version": "2.7.6"
         },
         "node_modules/mini-css-extract-plugin/node_modules/ajv": {
             "dependencies": {
                 "fast-deep-equal": "^3.1.1",
                 "json-schema-traverse": "^1.0.0",
                 "require-from-string": "^2.0.2",
                 "uri-js": "^4.2.2"
@@ -10966,17 +10988,17 @@
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
-            "version": "4.0.1"
+            "integrity": "sha512-Jw+GZVbP5IggB2WAn6UHI02LBwGmsIeYN/lNbSMZyDziQ7jmtAUrqKqDja+W89YHVs+KL/3IkIMltAklqB1vAw==",
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.1.0.tgz",
+            "version": "4.1.0"
         },
         "node_modules/minimalistic-assert": {
             "integrity": "sha512-UtJcAD4yEaGtjPezWuO9wC4nwUnVH/8/Im3yEHQP4b67cXlD/Qr9hdITCU1xDbSEXg2XKNaP8jsReV7vQd00/A==",
             "resolved": "https://registry.npmjs.org/minimalistic-assert/-/minimalistic-assert-1.0.1.tgz",
             "version": "1.0.1"
         },
         "node_modules/minimatch": {
@@ -11027,17 +11049,17 @@
         },
         "node_modules/mkdirp-classic": {
             "integrity": "sha512-gKLcREMhtuZRwRAfqP3RFW+TK4JqApVBtOIftVgjuABpAtpxhPGaDcfvbhNvD0B8iD1oUr/txX35NjcaY6Ns/A==",
             "resolved": "https://registry.npmjs.org/mkdirp-classic/-/mkdirp-classic-0.5.3.tgz",
             "version": "0.5.3"
         },
         "node_modules/module-alias": {
-            "integrity": "sha512-A/78XjoX2EmNvppVWEhM2oGk3x4lLxnkEA4jTbaK97QKSDjkIoOsKQlfylt/d3kKKi596Qy3NP5XrXJ6fZIC9Q==",
-            "resolved": "https://registry.npmjs.org/module-alias/-/module-alias-2.2.2.tgz",
-            "version": "2.2.2"
+            "integrity": "sha512-23g5BFj4zdQL/b6tor7Ji+QY4pEfNH784BMslY9Qb0UnJWRAt+lQGLYmRaM0KDBwIG23ffEBELhZDP2rhi9f/Q==",
+            "resolved": "https://registry.npmjs.org/module-alias/-/module-alias-2.2.3.tgz",
+            "version": "2.2.3"
         },
         "node_modules/moment": {
             "engines": {
                 "node": "*"
             },
             "integrity": "sha512-5LC9SOxjSc2HF6vO2CyuTDNivEdoz2IvyJJGj6X8DJ0eFyfszE0QiEd+iXmBvUP3WHxSjFH/vIsA0EN00cgr8w==",
             "resolved": "https://registry.npmjs.org/moment/-/moment-2.29.4.tgz",
@@ -11147,17 +11169,17 @@
         "node_modules/node-abi": {
             "dependencies": {
                 "semver": "^7.3.5"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-zNy02qivjjRosswoYmPi8hIKJRr8MpQyeKT6qlcq/OnOgA3Rhoae+IYOqsM9V5+JnHWmxKnWOT2GxvtqdtOCXA==",
-            "resolved": "https://registry.npmjs.org/node-abi/-/node-abi-3.40.0.tgz",
-            "version": "3.40.0"
+            "integrity": "sha512-MYjZTiAETGG28/7fBH1RjuY7vzDwYC5q5U4whCgM4jNEQcC0gAvN339LxXukmL2T2tGpzYTfp+LZ5RN7E5DwEg==",
+            "resolved": "https://registry.npmjs.org/node-abi/-/node-abi-3.44.0.tgz",
+            "version": "3.44.0"
         },
         "node_modules/node-abi/node_modules/lru-cache": {
             "dependencies": {
                 "yallist": "^4.0.0"
             },
             "engines": {
                 "node": ">=10"
@@ -11172,17 +11194,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
-            "version": "7.5.0"
+            "integrity": "sha512-Wvss5ivl8TMRZXXESstBA4uR5iXgEN/VC5/sOcuXdVLzcdkz4HWetIoRfG5gb5X+ij/G9rw9YoGn3QoQ8OCSpw==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.1.tgz",
+            "version": "7.5.1"
         },
         "node_modules/node-abi/node_modules/yallist": {
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/node-addon-api": {
@@ -11193,38 +11215,38 @@
         "node_modules/node-fetch": {
             "dependencies": {
                 "whatwg-url": "^5.0.0"
             },
             "engines": {
                 "node": "4.x || >=6.0.0"
             },
-            "integrity": "sha512-DJm/CJkZkRjKKj4Zi4BsKVZh3ValV5IR5s7LVZnW+6YMh0W1BfNA8XSs6DLMGYlId5F3KnA70uu2qepcR08Qqg==",
+            "integrity": "sha512-4I6pdBY1EthSqDmJkiNk3JIT8cswwR9nfeW/cPdUagJYEQG7R95WRH74wpz7ma8Gh/9dI9FP+OU+0E4FvtA55w==",
             "peerDependencies": {
                 "encoding": "^0.1.0"
             },
             "peerDependenciesMeta": {
                 "encoding": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/node-fetch/-/node-fetch-2.6.9.tgz",
-            "version": "2.6.9"
+            "resolved": "https://registry.npmjs.org/node-fetch/-/node-fetch-2.6.11.tgz",
+            "version": "2.6.11"
         },
         "node_modules/node-forge": {
             "engines": {
                 "node": ">= 6.13.0"
             },
             "integrity": "sha512-dPEtOeMvF9VMcYV/1Wb8CPoVAXtp6MKMlcbAt4ddqmGqUJ6fQZFXkNZNkNlfevtNkGtaSoXf/vNNNSvgrdXwtA==",
             "resolved": "https://registry.npmjs.org/node-forge/-/node-forge-1.3.1.tgz",
             "version": "1.3.1"
         },
         "node_modules/node-releases": {
-            "integrity": "sha512-5GFldHPXVG/YZmFzJvKK2zDSzPKhEp0+ZR5SVaoSag9fsL5YgHbUHDfnG5494ISANDcK4KwPXAx2xqVEydmd7w==",
-            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.10.tgz",
-            "version": "2.0.10"
+            "integrity": "sha512-QzsYKWhXTWx8h1kIvqfnC++o0pEmpRQA/aenALsL2F4pqNVr7YzcdMlDij5WBnwftRbJCNJL/O7zdKaxKPHqgQ==",
+            "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.12.tgz",
+            "version": "2.0.12"
         },
         "node_modules/normalize-package-data": {
             "dependencies": {
                 "hosted-git-info": "^2.1.4",
                 "resolve": "^1.10.0",
                 "semver": "2 || 3 || 4 || 5",
                 "validate-npm-package-license": "^3.0.1"
@@ -11736,17 +11758,17 @@
                     "url": "https://tidelift.com/funding/github/npm/postcss"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-bQ3qMcpF6A/YjR55xtoTr0jGOlnPOKAIMdOWiv0EIT6HVPEaJiJB4NLljSbiHoC2RX7DN5Uvjtpbg1NPdwv1oA==",
-            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.23.tgz",
-            "version": "8.4.23"
+            "integrity": "sha512-M0RzbcI0sO/XJNucsGjvWU9ERWxb/ytp1w6dKtxTKgixdtQDq4rmx/g8W1hnaheq9jgwL/oyEdH5Bc4WwJKMqg==",
+            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.24.tgz",
+            "version": "8.4.24"
         },
         "node_modules/postcss-calc": {
             "dependencies": {
                 "postcss-selector-parser": "^6.0.9",
                 "postcss-value-parser": "^4.2.0"
             },
             "integrity": "sha512-SmWMSJmB8MRnnULldx0lQIyhSNvuDl9HfrZkaqqE/WHAhToYsAvDq+yAsA/kIyINDszOp3Rh0GFoNuH5Ypsm3Q==",
@@ -11870,17 +11892,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
-            "version": "7.5.0"
+            "integrity": "sha512-Wvss5ivl8TMRZXXESstBA4uR5iXgEN/VC5/sOcuXdVLzcdkz4HWetIoRfG5gb5X+ij/G9rw9YoGn3QoQ8OCSpw==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.1.tgz",
+            "version": "7.5.1"
         },
         "node_modules/postcss-loader/node_modules/yallist": {
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/postcss-merge-longhand": {
@@ -11991,20 +12013,20 @@
                 "icss-utils": "^5.0.0",
                 "postcss-selector-parser": "^6.0.2",
                 "postcss-value-parser": "^4.1.0"
             },
             "engines": {
                 "node": "^10 || ^12 || >= 14"
             },
-            "integrity": "sha512-sT7ihtmGSF9yhm6ggikHdV0hlziDTX7oFoXtuVWeDd3hHObNkcHRo9V3yg7vCAY7cONyxJC/XXCmmiHHcvX7bQ==",
+            "integrity": "sha512-2/u2zraspoACtrbFRnTijMiQtb4GW4BvatjaG/bCjYQo8kLTdevCUlwuBHx2sCnSyrI3x3qj4ZK1j5LQBgzmwA==",
             "peerDependencies": {
                 "postcss": "^8.1.0"
             },
-            "resolved": "https://registry.npmjs.org/postcss-modules-local-by-default/-/postcss-modules-local-by-default-4.0.0.tgz",
-            "version": "4.0.0"
+            "resolved": "https://registry.npmjs.org/postcss-modules-local-by-default/-/postcss-modules-local-by-default-4.0.3.tgz",
+            "version": "4.0.3"
         },
         "node_modules/postcss-modules-scope": {
             "dependencies": {
                 "postcss-selector-parser": "^6.0.4"
             },
             "engines": {
                 "node": "^10 || ^12 || >= 14"
@@ -12203,17 +12225,17 @@
             "dependencies": {
                 "cssesc": "^3.0.0",
                 "util-deprecate": "^1.0.2"
             },
             "engines": {
                 "node": ">=4"
             },
-            "integrity": "sha512-NdxGCAZdRrwVI1sy59+Wzrh+pMMHxapGnpfenDVlMEXoOcvt4pGE0JLK9YY2F5dLxcFYA/YbVQKhcGU+FtSYQg==",
-            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.0.12.tgz",
-            "version": "6.0.12"
+            "integrity": "sha512-EaV1Gl4mUEV4ddhDnv/xtj7sxwrwxdetHdWUGnT4VJQf+4d05v6lHYZr8N573k5Z0BViss7BDhfWtKS3+sfAqQ==",
+            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.0.13.tgz",
+            "version": "6.0.13"
         },
         "node_modules/postcss-svgo": {
             "dependencies": {
                 "postcss-value-parser": "^4.2.0",
                 "svgo": "^2.7.0"
             },
             "engines": {
@@ -12712,34 +12734,34 @@
                 "chokidar": ">=3.0.0 <4.0.0",
                 "immutable": "^4.0.0",
                 "source-map-js": ">=0.6.2 <2.0.0"
             },
             "engines": {
                 "node": ">=14.0.0"
             },
-            "integrity": "sha512-NHpxIzN29MXvWiuswfc1W3I0N8SXBd8UR26WntmDlRYf0bSADnwnOjsyMZ3lMezSlArD33Vs3YFhp7dWvL770A==",
-            "resolved": "https://registry.npmjs.org/sass/-/sass-1.62.1.tgz",
-            "version": "1.62.1"
+            "integrity": "sha512-u56TU0AIFqMtauKl/OJ1AeFsXqRHkgO7nCWmHaDwfxDo9GUMSqBA4NEh6GMuh1CYVM7zuROYtZrHzPc2ixK+ww==",
+            "resolved": "https://registry.npmjs.org/sass/-/sass-1.63.2.tgz",
+            "version": "1.63.2"
         },
         "node_modules/schema-utils": {
             "dependencies": {
                 "@types/json-schema": "^7.0.8",
                 "ajv": "^6.12.5",
                 "ajv-keywords": "^3.5.2"
             },
             "engines": {
                 "node": ">= 10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-pvjEHOgWc9OWA/f/DE3ohBWTD6EleVLf7iFUkoSwAxttdBhB9QUebQgxER2kWueOvRJXPHNnyrvvh9eZINB8Eg==",
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.1.2.tgz",
-            "version": "3.1.2"
+            "integrity": "sha512-0zTyLGyDJYd/MBxG1AhJkKa6fpEBds4OQO2ut0w7OYG+ZGhGea09lijvzsqegYSik88zc7cUtIlnnO+/BvD6gQ==",
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-3.2.0.tgz",
+            "version": "3.2.0"
         },
         "node_modules/select-hose": {
             "integrity": "sha512-mEugaLK+YfkijB4fx0e6kImuJdCIt2LxCRcbEYPqRGCs4F2ogyfZU5IAZRdjCP8JPq2AtdNoC/Dux63d9Kiryg==",
             "resolved": "https://registry.npmjs.org/select-hose/-/select-hose-2.0.0.tgz",
             "version": "2.0.0"
         },
         "node_modules/selfsigned": {
@@ -12949,17 +12971,17 @@
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-+XC0AD/R7Q2mPSRuy2Id0+CGTZ98+8f+KvwirxOKIEyid+XSx6HbC63p+O4IndTHuX5Z+JxQ0TghCkO5Cg/2HA==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.0.tgz",
-            "version": "7.5.0"
+            "integrity": "sha512-Wvss5ivl8TMRZXXESstBA4uR5iXgEN/VC5/sOcuXdVLzcdkz4HWetIoRfG5gb5X+ij/G9rw9YoGn3QoQ8OCSpw==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.1.tgz",
+            "version": "7.5.1"
         },
         "node_modules/sharp/node_modules/yallist": {
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/shebang-command": {
@@ -13369,25 +13391,25 @@
             "version": "2.2.0"
         },
         "node_modules/terser": {
             "bin": {
                 "terser": "bin/terser"
             },
             "dependencies": {
-                "@jridgewell/source-map": "^0.3.2",
-                "acorn": "^8.5.0",
+                "@jridgewell/source-map": "^0.3.3",
+                "acorn": "^8.8.2",
                 "commander": "^2.20.0",
                 "source-map-support": "~0.5.20"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-hVl35zClmpisy6oaoKALOpS0rDYLxRFLHhRuDlEGTKey9qHjS1w9GMORjuwIMt70Wan4lwsLYyWDVnWgF+KUEw==",
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.17.1.tgz",
-            "version": "5.17.1"
+            "integrity": "sha512-/bi0Zm2C6VAexlGgLlVxA0P2lru/sdLyfCVaRMfKVo9nWxbmz7f/sD8VPybPeSUJaJcwmCJis9pBIhcVcG1QcQ==",
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.17.7.tgz",
+            "version": "5.17.7"
         },
         "node_modules/terser-webpack-plugin": {
             "dependencies": {
                 "@jridgewell/trace-mapping": "^0.3.17",
                 "jest-worker": "^27.4.5",
                 "schema-utils": "^3.1.1",
                 "serialize-javascript": "^6.0.1",
@@ -13396,31 +13418,31 @@
             "engines": {
                 "node": ">= 10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-WiHL3ElchZMsK27P8uIUh4604IgJyAW47LVXGbEoB21DbQcZ+OuMpGjVYnEUaqcWM6dO8uS2qUbA7LSCWqvsbg==",
+            "integrity": "sha512-ZuXsqE07EcggTWQjXUj+Aot/OMcD0bMKGgF63f7UxYcu5/AJF53aIpK1YoP5xR9l6s/Hy2b+t1AM0bLNPRuhwA==",
             "peerDependencies": {
                 "webpack": "^5.1.0"
             },
             "peerDependenciesMeta": {
                 "@swc/core": {
                     "optional": true
                 },
                 "esbuild": {
                     "optional": true
                 },
                 "uglify-js": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.8.tgz",
-            "version": "5.3.8"
+            "resolved": "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.9.tgz",
+            "version": "5.3.9"
         },
         "node_modules/terser/node_modules/commander": {
             "integrity": "sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==",
             "resolved": "https://registry.npmjs.org/commander/-/commander-2.20.3.tgz",
             "version": "2.20.3"
         },
         "node_modules/text-hex": {
@@ -13535,17 +13557,17 @@
         },
         "node_modules/triple-beam": {
             "integrity": "sha512-XrHUvV5HpdLmIj4uVMxHggLbFSZYIn7HEWsqePZcI50pco+MPqJ50wMGY794X7AOOhxOBAjbkqfAbEe/QMp2Lw==",
             "resolved": "https://registry.npmjs.org/triple-beam/-/triple-beam-1.3.0.tgz",
             "version": "1.3.0"
         },
         "node_modules/tslib": {
-            "integrity": "sha512-336iVw3rtn2BUK7ORdIAHTyxHGRIHVReokCR3XjbckJMK7ms8FysBfhLR8IXnAgy7T0PTPNBWKiH514FOW/WSg==",
-            "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.5.0.tgz",
-            "version": "2.5.0"
+            "integrity": "sha512-mSxlJJwl3BMEQCUNnxXBU9jP4JBktcEGhURcPR6VQVlnP0FdDEsIaz0C35dXNGLyRfrATNofF0F5p2KPxQgB+w==",
+            "resolved": "https://registry.npmjs.org/tslib/-/tslib-2.5.3.tgz",
+            "version": "2.5.3"
         },
         "node_modules/tunnel-agent": {
             "dependencies": {
                 "safe-buffer": "^5.0.1"
             },
             "engines": {
                 "node": "*"
@@ -13707,28 +13729,28 @@
         },
         "node_modules/vue-loader": {
             "dependencies": {
                 "chalk": "^4.1.0",
                 "hash-sum": "^2.0.0",
                 "watchpack": "^2.4.0"
             },
-            "integrity": "sha512-zAjrT+TNWTpgRODxqDfzbDyvuTf5kCP9xmMk8aspQKuYNnTY2r0XK/bHu1DKLpSpk0I6fkQph5OLKB7HcRIPZw==",
+            "integrity": "sha512-aqNvKJvnz2A/6VWeJZodAo8XLoAlVwBv+2Z6dama+LHsAF+P/xijQ+OfWrxIs0wcGSJduvdzvTuATzXbNKkpiw==",
             "peerDependencies": {
                 "webpack": "^4.1.0 || ^5.0.0-0"
             },
             "peerDependenciesMeta": {
                 "@vue/compiler-sfc": {
                     "optional": true
                 },
                 "vue": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/vue-loader/-/vue-loader-17.1.0.tgz",
-            "version": "17.1.0"
+            "resolved": "https://registry.npmjs.org/vue-loader/-/vue-loader-17.2.2.tgz",
+            "version": "17.2.2"
         },
         "node_modules/vue-loader/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "engines": {
                 "node": ">=8"
@@ -13858,18 +13880,18 @@
             "dependencies": {
                 "@types/eslint-scope": "^3.7.3",
                 "@types/estree": "^1.0.0",
                 "@webassemblyjs/ast": "^1.11.5",
                 "@webassemblyjs/wasm-edit": "^1.11.5",
                 "@webassemblyjs/wasm-parser": "^1.11.5",
                 "acorn": "^8.7.1",
-                "acorn-import-assertions": "^1.7.6",
+                "acorn-import-assertions": "^1.9.0",
                 "browserslist": "^4.14.5",
                 "chrome-trace-event": "^1.0.2",
-                "enhanced-resolve": "^5.13.0",
+                "enhanced-resolve": "^5.14.1",
                 "es-module-lexer": "^1.2.1",
                 "eslint-scope": "5.1.1",
                 "events": "^3.2.0",
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.2.9",
                 "json-parse-even-better-errors": "^2.3.1",
                 "loader-runner": "^4.2.0",
@@ -13884,22 +13906,22 @@
             "engines": {
                 "node": ">=10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-iGNA2fHhnDcV1bONdUu554eZx+XeldsaeQ8T67H6KKHl2nUSwX8Zm7cmzOA46ox/X1ARxf7Bjv8wQ/HsB5fxBg==",
+            "integrity": "sha512-3BOvworZ8SO/D4GVP+GoRC3fVeg5MO4vzmq8TJJEkdmopxyazGDxN8ClqN12uzrZW9Tv8EED8v5VSb6Sqyi0pg==",
             "peerDependenciesMeta": {
                 "webpack-cli": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.82.0.tgz",
-            "version": "5.82.0"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.86.0.tgz",
+            "version": "5.86.0"
         },
         "node_modules/webpack-bundle-analyzer": {
             "bin": {
                 "webpack-bundle-analyzer": "lib/bin/analyzer.js"
             },
             "dependencies": {
                 "@discoveryjs/json-ext": "0.5.7",
@@ -13912,17 +13934,17 @@
                 "opener": "^1.5.2",
                 "sirv": "^1.0.7",
                 "ws": "^7.3.1"
             },
             "engines": {
                 "node": ">= 10.13.0"
             },
-            "integrity": "sha512-ZzoSBePshOKhr+hd8u6oCkZVwpVaXgpw23ScGLFpR6SjYI7+7iIWYarjN6OEYOfRt8o7ZyZZQk0DuMizJ+LEIg==",
-            "resolved": "https://registry.npmjs.org/webpack-bundle-analyzer/-/webpack-bundle-analyzer-4.8.0.tgz",
-            "version": "4.8.0"
+            "integrity": "sha512-+bXGmO1LyiNx0i9enBu3H8mv42sj/BJWhZNFwjz92tVnBa9J3JMGo2an2IXlEleoDOPn/Hofl5hr/xCpObUDtw==",
+            "resolved": "https://registry.npmjs.org/webpack-bundle-analyzer/-/webpack-bundle-analyzer-4.9.0.tgz",
+            "version": "4.9.0"
         },
         "node_modules/webpack-bundle-analyzer/node_modules/ansi-styles": {
             "dependencies": {
                 "color-convert": "^2.0.1"
             },
             "engines": {
                 "node": ">=8"
@@ -14067,17 +14089,17 @@
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
-            "version": "4.0.1"
+            "integrity": "sha512-Jw+GZVbP5IggB2WAn6UHI02LBwGmsIeYN/lNbSMZyDziQ7jmtAUrqKqDja+W89YHVs+KL/3IkIMltAklqB1vAw==",
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.1.0.tgz",
+            "version": "4.1.0"
         },
         "node_modules/webpack-dev-server": {
             "bin": {
                 "webpack-dev-server": "bin/webpack-dev-server.js"
             },
             "dependencies": {
                 "@types/bonjour": "^3.5.9",
@@ -14159,17 +14181,17 @@
             "resolved": "https://registry.npmjs.org/ajv-keywords/-/ajv-keywords-5.1.0.tgz",
             "version": "5.1.0"
         },
         "node_modules/webpack-dev-server/node_modules/ipaddr.js": {
             "engines": {
                 "node": ">= 10"
             },
-            "integrity": "sha512-1qTgH9NG+IIJ4yfKs2e6Pp1bZg8wbDbKHT21HrLIeYBTRLgMYKnMTPAuI3Lcs61nfx5h1xlXnbJtH1kX5/d/ng==",
-            "resolved": "https://registry.npmjs.org/ipaddr.js/-/ipaddr.js-2.0.1.tgz",
-            "version": "2.0.1"
+            "integrity": "sha512-LlbxQ7xKzfBusov6UMi4MFpEg0m+mAm9xyNGEduwXMEDuf4WfzB/RZwMVYEd7IKGvh4IUkEXYxtAVu9T3OelJQ==",
+            "resolved": "https://registry.npmjs.org/ipaddr.js/-/ipaddr.js-2.1.0.tgz",
+            "version": "2.1.0"
         },
         "node_modules/webpack-dev-server/node_modules/json-schema-traverse": {
             "integrity": "sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==",
             "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/webpack-dev-server/node_modules/schema-utils": {
@@ -14182,17 +14204,17 @@
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-lELhBAAly9NowEsX0yZBlw9ahZG+sK/1RJ21EpzdYHKEs13Vku3LJ+MIPhh4sMs0oCCeufZQEQbMekiA4vuVIQ==",
-            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.1.tgz",
-            "version": "4.0.1"
+            "integrity": "sha512-Jw+GZVbP5IggB2WAn6UHI02LBwGmsIeYN/lNbSMZyDziQ7jmtAUrqKqDja+W89YHVs+KL/3IkIMltAklqB1vAw==",
+            "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.1.0.tgz",
+            "version": "4.1.0"
         },
         "node_modules/webpack-dev-server/node_modules/ws": {
             "engines": {
                 "node": ">=10.0.0"
             },
             "integrity": "sha512-x9vcZYTrFPC7aSIbj7sRCYo7L/Xb8Iy+pW0ng0wt2vCJv7M9HOMy0UoN3rr+IFC7hb7vXoqS+P9ktyLLLhO+LA==",
             "peerDependencies": {
@@ -14214,17 +14236,17 @@
             "dependencies": {
                 "clone-deep": "^4.0.1",
                 "wildcard": "^2.0.0"
             },
             "engines": {
                 "node": ">=10.0.0"
             },
-            "integrity": "sha512-/SaI7xY0831XwP6kzuwhKWVKDP9t1QY1h65lAFLbZqMPIuYcD9QAW4u9STIbU9kaJbPBB/geU/gLr1wDjOhQ+Q==",
-            "resolved": "https://registry.npmjs.org/webpack-merge/-/webpack-merge-5.8.0.tgz",
-            "version": "5.8.0"
+            "integrity": "sha512-6NbRQw4+Sy50vYNTw7EyOn41OZItPiXB8GNv3INSoe3PSFaHJEz3SHTrYVaRm2LilNGnFUzh0FAwqPEmU/CwDg==",
+            "resolved": "https://registry.npmjs.org/webpack-merge/-/webpack-merge-5.9.0.tgz",
+            "version": "5.9.0"
         },
         "node_modules/webpack-sources": {
             "engines": {
                 "node": ">=10.13.0"
             },
             "integrity": "sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==",
             "resolved": "https://registry.npmjs.org/webpack-sources/-/webpack-sources-3.2.3.tgz",
@@ -14299,17 +14321,17 @@
                 "stack-trace": "0.0.x",
                 "triple-beam": "^1.3.0",
                 "winston-transport": "^4.5.0"
             },
             "engines": {
                 "node": ">= 12.0.0"
             },
-            "integrity": "sha512-MsE1gRx1m5jdTTO9Ld/vND4krP2To+lgDoMEHGGa4HIlAUyXJtfc7CxQcGXVyz2IBpw5hbFkj2b/AtUdQwyRew==",
-            "resolved": "https://registry.npmjs.org/winston/-/winston-3.8.2.tgz",
-            "version": "3.8.2"
+            "integrity": "sha512-jW51iW/X95BCW6MMtZWr2jKQBP4hV5bIDq9QrIjfDk6Q9QuxvTKEAlpUNAzP+HYHFFCeENhph16s0zEunu4uuQ==",
+            "resolved": "https://registry.npmjs.org/winston/-/winston-3.9.0.tgz",
+            "version": "3.9.0"
         },
         "node_modules/winston-daily-rotate-file": {
             "dependencies": {
                 "file-stream-rotator": "^0.6.1",
                 "object-hash": "^2.0.1",
                 "triple-beam": "^1.3.0",
                 "winston-transport": "^4.4.0"
```

### Comparing `gramex-1.90.0/gramex/apps/ui/setup.js` & `gramex-1.91.0/gramex/apps/ui/setup.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootstrap5.scss` & `gramex-1.91.0/gramex/apps/ui/theme/bootstrap5.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cerulean.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/cerulean.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cosmo.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/cosmo.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/cyborg.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/cyborg.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/darkly.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/darkly.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/flatly.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/flatly.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/journal.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/journal.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/litera.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/litera.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/lumen.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/lumen.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/lux.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/lux.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/materia.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/materia.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/minty.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/minty.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/pulse.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/pulse.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/sandstone.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/sandstone.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/simplex.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/simplex.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/sketchy.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/sketchy.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/slate.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/slate.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/solar.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/solar.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/spacelab.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/spacelab.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/superhero.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/superhero.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/united.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/united.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/bootswatch/yeti.png` & `gramex-1.91.0/gramex/apps/ui/theme/bootswatch/yeti.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/default.png` & `gramex-1.91.0/gramex/apps/ui/theme/default.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/index.html` & `gramex-1.91.0/gramex/apps/ui/theme/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/sample.html` & `gramex-1.91.0/gramex/apps/ui/theme/sample.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/blue_voltage.png` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/blue_voltage.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/blue_voltage.scss` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/blue_voltage.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/boldstrap.png` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/boldstrap.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/darkster.png` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/darkster.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/darkster.scss` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/darkster.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/fresca.png` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/fresca.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/greyson.png` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/greyson.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/greyson.scss` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/greyson.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.png` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/herbie.png` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/herbie.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/hootstrap.png` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/hootstrap.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/lovey.png` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/lovey.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/monotony.png` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/monotony.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/poypull.png` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/poypull.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/poypull.scss` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/poypull.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/signal.png` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/signal.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/signal.scss` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/signal.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes-guide/tequila.png` & `gramex-1.91.0/gramex/apps/ui/theme/themes-guide/tequila.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/ui/theme/themes.json` & `gramex-1.91.0/gramex/apps/ui/theme/themes.json`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/.eslintrc.js` & `gramex-1.91.0/gramex/apps/uifactory/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/assets/data/input.json` & `gramex-1.91.0/gramex/apps/uifactory/assets/data/input.json`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/assets/img/arrows-move.svg` & `gramex-1.91.0/gramex/apps/uifactory/assets/img/arrows-move.svg`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png` & `gramex-1.91.0/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/assets/img/trash.svg` & `gramex-1.91.0/gramex/apps/uifactory/assets/img/trash.svg`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/create.html` & `gramex-1.91.0/gramex/apps/uifactory/create.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/edit.html` & `gramex-1.91.0/gramex/apps/uifactory/edit.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/field-actions.html` & `gramex-1.91.0/gramex/apps/uifactory/field-actions.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/form_builder.py` & `gramex-1.91.0/gramex/apps/uifactory/form_builder.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/gramex.yaml` & `gramex-1.91.0/gramex/apps/uifactory/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/index.html` & `gramex-1.91.0/gramex/apps/uifactory/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/js/README.md` & `gramex-1.91.0/gramex/apps/uifactory/js/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/js/fields.js` & `gramex-1.91.0/gramex/apps/uifactory/js/fields.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/js/fork-form.js` & `gramex-1.91.0/gramex/apps/uifactory/js/fork-form.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/js/index.js` & `gramex-1.91.0/gramex/apps/uifactory/js/index.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/js/script.js` & `gramex-1.91.0/gramex/apps/uifactory/js/script.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/js/utils.js` & `gramex-1.91.0/gramex/apps/uifactory/js/utils.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/js/viewform.js` & `gramex-1.91.0/gramex/apps/uifactory/js/viewform.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/modals/add-field.html` & `gramex-1.91.0/gramex/apps/uifactory/modals/add-field.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/modals/embed.html` & `gramex-1.91.0/gramex/apps/uifactory/modals/embed.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/modals/remove.html` & `gramex-1.91.0/gramex/apps/uifactory/modals/remove.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/modals/rename.html` & `gramex-1.91.0/gramex/apps/uifactory/modals/rename.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/modals/themes.html` & `gramex-1.91.0/gramex/apps/uifactory/modals/themes.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/package-lock.json` & `gramex-1.91.0/gramex/apps/uifactory/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/popover-form.html` & `gramex-1.91.0/gramex/apps/uifactory/popover-form.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/sample.html` & `gramex-1.91.0/gramex/apps/uifactory/sample.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/snippets/button/bs4-button.js` & `gramex-1.91.0/gramex/apps/uifactory/snippets/button/bs4-button.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js` & `gramex-1.91.0/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/snippets/email/bs4-email.js` & `gramex-1.91.0/gramex/apps/uifactory/snippets/email/bs4-email.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js` & `gramex-1.91.0/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/snippets/number/bs4-number.js` & `gramex-1.91.0/gramex/apps/uifactory/snippets/number/bs4-number.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/snippets/radio/bs4-radio.js` & `gramex-1.91.0/gramex/apps/uifactory/snippets/radio/bs4-radio.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/snippets/range/bs4-range.js` & `gramex-1.91.0/gramex/apps/uifactory/snippets/range/bs4-range.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/snippets/select/bs4-select.js` & `gramex-1.91.0/gramex/apps/uifactory/snippets/select/bs4-select.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/snippets/setup.js` & `gramex-1.91.0/gramex/apps/uifactory/snippets/setup.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/snippets/text/bs4-text.js` & `gramex-1.91.0/gramex/apps/uifactory/snippets/text/bs4-text.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js` & `gramex-1.91.0/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/style.scss` & `gramex-1.91.0/gramex/apps/uifactory/style.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/template-navbar-view-form.html` & `gramex-1.91.0/gramex/apps/uifactory/template-navbar-view-form.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/template-navbar.html` & `gramex-1.91.0/gramex/apps/uifactory/template-navbar.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/uifactory/viewform.html` & `gramex-1.91.0/gramex/apps/uifactory/viewform.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/update/README.md` & `gramex-1.91.0/gramex/apps/update/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/update/gramex.yaml` & `gramex-1.91.0/gramex/apps/update/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/update/gramexupdate.py` & `gramex-1.91.0/gramex/apps/update/gramexupdate.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/apps/update/index.html` & `gramex-1.91.0/gramex/apps/update/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/cache.py` & `gramex-1.91.0/gramex/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,24 +75,22 @@
     **kwargs: dict,
 ) -> Any:
     '''Reads a file, processes it via a callback, caches the result and returns it.
 
     When called again, returns the cached result unless the file has updated.
 
     Examples:
-
         >>> gramex.cache.open('data.yaml')
         >>> gramex.cache.open('data.csv')
         >>> # Load data.json as JSON into an AttrDict
         >>> gramex.cache.open('data.json', 'json', object_pairs_hook=AttrDict)
         >>> # Load data.csv as CSV into a Pandas DataFrame
         >>> gramex.cache.open('data.csv', 'csv', encoding='cp1252')
 
     Parameters:
-
         path: path to the file to open
         callback: type of file, e.g. `csv`, `json`, or callback function
         transform: function to transform the data before caching
         rel: if True, path is relative to the calling file. Default: False
         **kwargs: passed to the callback function
 
     `callback=` accepts these predefined types:
@@ -133,30 +131,31 @@
         # Returns the count of the CSV file, updating it only when changed
         open('data.csv', 'csv', transform=lambda data: len(data))
 
         # After loading data.xlsx into a DataFrame, returned the grouped result
         open('data.xlsx', 'xslx', transform=lambda data: data.groupby('city')['sales'].sum())
 
     If `transform=` is not a function, it is used as a cache key.
-    You can use this to fetch multiple cached version of the file. For example:
+    You can use this to fetch multiple cached version of the file.
 
+    Examples:
         >>> original = open('data.csv', 'csv', transform='v1')
         >>> same_copy = open('data.csv', 'csv', transform='v1')
         >>> new_copy = open('data.csv', 'csv', transform='v2')
         >>> original.columns = ['x', 'y', 'z']
         >>> same_copy.columns
         ['x', 'y', 'z']
         >>> new_copy.columns
         ['a', 'b', 'c']
 
     `rel=True` opens the path relative to the caller function's file path. If
     `D:/app/calc.py` calls `open('data.csv', 'csv', rel=True)`, the path
     is replaced with `D:/app/data.csv`.
 
-    All ``kwargs`` are passed directly to the callback. If the callback is a predefined string
+    All `kwargs` are passed directly to the callback. If the callback is a predefined string
     using `io.open()`, all `io.open()` arguments are passed to `io.open()`, rest to the callback.
     '''
     # Pass _reload_status = True for testing purposes. This returns a tuple:
     # (result, reloaded) instead of just the result.
     _reload_status = kwargs.pop('_reload_status', False)
     reloaded = False
     _cache = kwargs.pop('_cache', _OPEN_CACHE)
@@ -222,23 +221,21 @@
     range: str = None,
     header: Union[None, int, List[int]] = ...,
     **kwargs: dict,
 ) -> pd.DataFrame:
     '''Read data from an XLSX as a DataFrame using `openpyxl`.
 
     Examples:
-
         >>> gramex.cache.read_excel('data.xlsx', sheet_name='Sheet1')
         >>> gramex.cache.read_excel('data.xlsx', sheet_name=0)
         >>> gramex.cache.read_excel('data.xlsx', table='Table1')
         >>> gramex.cache.read_excel('data.xlsx', name='NamedRange')
         >>> gramex.cache.read_excel('data.xlsx', range='A1:D10', header=[0, 1])
 
     Parameters:
-
         io: path or file-like object pointing to an Excel file
         sheet_name: sheet to load data from. Sheet names are specified as strings.
             Integers pick zero-indexed sheet position. default: 0
         table: Worksheet table to load from sheet, e.g. `'Table1'`
         name: Defined name to load from sheet, e.g. `'MyNamedRange'`
         range: Cell range to load from sheet, e.g. `'A1:C10'`
         header: Row (0-indexed) to use for the column labels. A list of integers is combined into
@@ -309,15 +306,14 @@
     rel: bool = False,
     callback: Union[str, Callable] = None,
     **kwargs: dict,
 ) -> None:
     '''Saves a Pandas DataFrame into file at url.
 
     Examples:
-
         >>> gramex.cache.save(pd.DataFrame({'x': [1, 2]}), 'sample.csv')
         >>> gramex.cache.save(pd.DataFrame({'x': [1, 2]}), 'sample.xlsx', sheet_name='data')
 
     Parameters:
         data: Pandas dataframe which has to be saved to a file.
         url: path where the dataframe has to be saved.
         rel: if True, path is relative to the calling file. Default: False
@@ -345,15 +341,14 @@
     **kwargs: dict,
 ):
     '''Read SQL query or database table into a DataFrame, cached.
 
     It uses `state` to determine whether to run the query again or not.
 
     Examples:
-
         >>> engine = sqlalchemy.create_engine('sqlite:///path/to/file.db')
         >>> gramex.cache.query('SELECT * FROM table', engine, state='SELECT max(date) FROM table')
 
     Parameters:
 
         sql: SQL query or table name to read from the database.
         engine: SQLAlchemy engine to read from.
@@ -413,15 +408,14 @@
     return (result, reloaded) if _reload_status else result
 
 
 def stat(path: str) -> Union[Tuple[float, int], Tuple[None, None]]:
     '''Returns a file's modified time and size. Used to check if a file has changed.
 
     Examples:
-
         >>> gramex.cache.stat('gramex.yaml')
         (1654149106.1422858, 7675)
         >>> gramex.cache.stat('non-existent-file')
         (None, None)
 
     Parameters:
         path: Absolute file path/Path relative to gramex root folder
@@ -442,15 +436,14 @@
     )
 
 
 def cache_key(*args: List[Any]) -> str:
     '''Converts arguments into a stable string suitable for use as a cache key.
 
     Examples:
-
         >>> t1 = gramex.cache.cache_key(tweet1)
         >>> data[t1] = tweet1
         >>> t2 = gramex.cache.cache_key(tweet2)
         >>> data[t2] = tweet2
 
     Parameters:
 
@@ -478,15 +471,14 @@
 _MODULE_CACHE = {}
 
 
 def reload_module(*modules: List[ModuleType]) -> None:
     '''Reloads one or more modules if they have changed on disk.
 
     Examples:
-
         >>> import mymodule1
         >>> import mymodule2
         >>> reload_module(mymodule1, mymodule2)
 
     Parameters:
 
         *modules: Pass the module which has to reload.
@@ -519,15 +511,14 @@
         _MODULE_CACHE[name] = fstat
 
 
 def urlfetch(url: str, info: bool = False, **kwargs: dict) -> Union[str, Dict]:
     '''Fetch the content in the url and return a file path where it is downloaded.
 
     Examples:
-
         >>> gramex.cache.urlfetch('https://gramener.com/gramex/guide/mlhandler/titanic')
         '/path/to/tmpfile.json'
 
     Parameters:
         url: A http, https or file path
         info: True if metadata of the requested file is required. If true, it
             returns a dict with (filename), r (request) url, ext (extension), content_type.
@@ -570,15 +561,14 @@
     '''Wraps `subprocess.Popen` to run in a Tornado IOLoop.
 
     [`tornado.process.Subprocess()`](https://www.tornadoweb.org/en/stable/process.html)
     [fails on Windows](https://github.com/tornadoweb/tornado/issues/1585).
     This is a threaded alternative.
 
     Examples:
-
         Run a program async and wait for it to execute. Then get its output:
 
         >>> stdout, stderr = yield Subprocess(['ls', '-la']).wait_for_exit()
 
         Run a program async and send each line to the handler as it writes:
 
         >>> yield Subprocess(
@@ -777,32 +767,30 @@
     buffer_size: Union[int, Literal['line']] = 'line',
     **kwargs,
 ) -> Future:
     '''Run a long-running process in the background, and wait till it starts properly.
 
     This is used to run & cache servers like Node web servers, Elasticsearch, etc. in Tornado.
 
-    Examples:
-
-        ```python
-        @tornado.gen.coroutine
-        def fetch_from_server(handler):
-            server = yield gramex.cache.daemon(
-                ['python', '-m', 'http_server', '8000']
-                restart=3,
-                first_line=re.compile(r'Serving HTTP on .* port 8000'),
-                timeout=5,
-                stream=sys.stdout.write,
-                buffer_size='line',
-            )
-            return requests.get('http://localhost:8000/').text
-        ```
+    ```python
+    @tornado.gen.coroutine
+    def fetch_from_server(handler):
+        server = yield gramex.cache.daemon(
+            ['python', '-m', 'http_server', '8000']
+            restart=3,
+            first_line=re.compile(r'Serving HTTP on .* port 8000'),
+            timeout=5,
+            stream=sys.stdout.write,
+            buffer_size='line',
+        )
+        return requests.get('http://localhost:8000/').text
+    ```
 
-        The first time `fetch_from_server` is called, it starts a Python web server on port 8000.
-        Subsequent calls use the same server.
+    The first time `fetch_from_server` is called, it starts a Python web server on port 8000.
+    Subsequent calls use the same server.
 
     Parameters:
 
         args: command to run. Can be a list of strings or a string. See
             [subprocess.Popen](https://docs.python.org/3/library/subprocess.html#subprocess.Popen)
         restart: number of times to restart the process if it fails. Set to 0 to never restart.
         first_line: wait until the first line of output matches this string, regex or function
@@ -1252,15 +1240,14 @@
 
 def opener(callback, read=False, **open_kwargs):
     '''
     Converts any function that accepts a string or handle as its parameter into
     a function that takes the first parameter from a file path.
 
     Examples:
-
         >>> jsonload = opener(json.load)
         >>> jsonload('x.json')      # opens x.json and runs json.load(handle)
         >>> gramex.cache.open('x.json', jsonload)   # Loads x.json, cached
 
         >>> # read=True parameter passes the contents (not handle) to the function
         >>> template = opener(string.Template, read=True)
         >>> template('abc.txt').substitute(x=val)
```

### Comparing `gramex-1.90.0/gramex/config.py` & `gramex-1.91.0/gramex/config.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/data.py` & `gramex-1.91.0/gramex/data.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/debug.py` & `gramex-1.91.0/gramex/debug.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,17 @@
     '''_caller() returns the "file:function:line" of the calling function'''
     parent = inspect.getouterframes(inspect.currentframe())[2]
     return f'[{parent[1]}:{parent[3]}:{parent[2]}]'
 
 
 class Timer:
     '''
-    Find how long a code blocks takes to execute. Wrap any code block like this::
+    Find how long a code blocks takes to execute. Wrap any code block like this:
 
+    Examples:
         >>> from gramex.debug import Timer
         >>> with Timer('optional message'):
         >>>     slow_running_code()
         WARNING:gramex:1.000s optional message [<file>:<func>:line]
     '''
 
     def __init__(self, msg='', level=logging.WARNING):
@@ -53,17 +54,18 @@
         text = indent(text, ' .. ' + ' ' * len(prefix) + '   ')
         stream.write(' .. ' + prefix + ' = ' + text[7 + len(prefix) :])
     stream.write('\n')
 
 
 def print(*args, **kwargs):  # noqa
     '''
-    A replacement for the ``print`` function that also logs the (file, function,
-    line, msg) from where it is called. For example::
+    A replacement for the `print` function that also logs the (file, function,
+    line, msg) from where it is called. For example:
 
+    Examples:
         >>> from gramex.debug import print              # import print function
         >>> print('hello world')                        # It works like the print function
         <file>(line).<function>: hello world
         >>> print(x=1, y=2)                             # Use kwargs to print variable names
         <file>(line).<function>:
          .. x = 1
          .. y = 2
@@ -82,21 +84,23 @@
         for key, val in kwargs.items():
             _write(val, key, stream=stream)
         stream.write('\n')
 
 
 def trace(trace=True, exclude=None, **kwargs):
     '''
-    Decorator to trace line execution. Usage::
+    Decorator to trace line execution. Usage:
 
-        @trace()
-        def method(...):
-            ...
+    ```python
+    @trace()
+    def method(...):
+        ...
+    ```
 
-    When ``method()`` is called, every line of execution is traced.
+    When `method()` is called, every line of execution is traced.
     '''
     if exclude is None:
         ignoredirs = (sys.prefix,)
     elif isinstance(exclude, str):
         ignoredirs = (sys.prefix, os.path.abspath(exclude))
     elif isinstance(exclude, (list, tuple)):
         ignoredirs = [sys.prefix] + [os.path.abspath(path) for path in exclude]
@@ -111,16 +115,17 @@
 
     return decorator
 
 
 def lineprofile(func):
     '''
     A decorator that prints the time taken for each line of a function every
-    time it is called. This example prints each line's performance::
+    time it is called. This example prints each line's performance:
 
+    Examples:
         >>> from gramex.debug import lineprofile
         >>> @lineprofile
         >>> def calc():
         >>>     ...
     '''
     try:
         import line_profiler
@@ -193,16 +198,17 @@
 
         def getch():
             return None
 
 
 def _make_timer():
     '''
-    ``timer("msg")`` prints the time elapsed since the last timer call::
+    `timer("msg")` prints the time elapsed since the last timer call:
 
+    Examples:
         >>> from gramex.debug import timer
         >>> gramex.debug.timer('abc')
         WARNING:gramex:7.583s abc [<file>:<function>:1]     # Time since Gramex start
         >>> gramex.debug.timer('def')
         WARNING:gramex:3.707s def [<file>:<function>:1]     # Time since last call
     '''
```

### Comparing `gramex-1.90.0/gramex/deploy.yaml` & `gramex-1.91.0/gramex/deploy.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/download.vega.js` & `gramex-1.91.0/gramex/download.vega.js`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/favicon.ico` & `gramex-1.91.0/gramex/favicon.ico`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/gramex.yaml` & `gramex-1.91.0/gramex/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/gramexsize.csv` & `gramex-1.91.0/gramex/gramexsize.csv`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 gramex.handlers.basehandler.BaseMixin.cors_origin,url.*.kwargs.cors,5
 gramex.handlers.basehandler.BaseMixin._cors_options,url.*.kwargs.cors,9
 gramex.handlers.basehandler.BaseMixin.setup_default_kwargs,url,1
 gramex.handlers.basehandler.BaseMixin.setup_transform,url.*.kwargs.session,2
 gramex.handlers.basehandler.BaseMixin._purge_keys,url.*.kwargs.auth,7
 gramex.handlers.basehandler.BaseMixin._get_store,url.*.kwargs.cache,2
 gramex.handlers.basehandler.BaseMixin.setup_session,url.*.kwargs.session,3
-gramex.handlers.basehandler.BaseMixin.setup_ratelimit,url.*.kwargs.ratelimit,18
+gramex.handlers.basehandler.BaseMixin.setup_ratelimit,url.*.kwargs.ratelimit,5
 gramex.handlers.basehandler.BaseMixin.reset_ratelimit,url.*.kwargs.ratelimit,2
 gramex.handlers.basehandler.BaseMixin.setup_redirect,url.*.kwargs.redirect,13
 gramex.handlers.basehandler.BaseMixin.setup_auth,url.*.kwargs.auth,8
 gramex.handlers.basehandler.BaseMixin.authorize,url.*.kwargs.auth,1
 gramex.handlers.basehandler.BaseMixin.setup_log,url.*.kwargs.log,1
 gramex.handlers.basehandler.BaseMixin._error_fn,url.*.kwargs.error,5
 gramex.handlers.basehandler.BaseMixin.setup_error,url.*.kwargs.error,13
@@ -99,16 +99,16 @@
 gramex.handlers.basehandler.BaseMixin.otp,url.*.kwargs.auth,2
 gramex.handlers.basehandler.BaseMixin.get_otp,url.*.kwargs.auth,4
 gramex.handlers.basehandler.BaseMixin.revoke_otp,url.*.kwargs.auth,1
 gramex.handlers.basehandler.BaseMixin.apikey,url.*.kwargs.auth,1
 gramex.handlers.basehandler.BaseMixin.revoke_apikey,url.*.kwargs.auth,1
 gramex.handlers.basehandler.BaseMixin.override_user,url.*.kwargs.auth,7
 gramex.handlers.basehandler.BaseMixin.set_last_visited,url.*.kwargs.auth,3
-gramex.handlers.basehandler.BaseMixin.check_ratelimit,url.*.kwargs.ratelimit,2
-gramex.handlers.basehandler.BaseMixin.update_ratelimit,url.*.kwargs.ratelimit,2
+gramex.handlers.basehandler.BaseMixin.check_ratelimit,url.*.kwargs.ratelimit,3
+gramex.handlers.basehandler.BaseMixin.update_ratelimit,url.*.kwargs.ratelimit,4
 gramex.handlers.basehandler.BaseMixin.set_ratelimit_headers,url.*.kwargs.ratelimit,2
 gramex.handlers.basehandler.BaseHandler.initialize,url,3
 gramex.handlers.basehandler.BaseHandler.get_arg,url,3
 gramex.handlers.basehandler.BaseHandler.prepare,url,2
 gramex.handlers.basehandler.BaseHandler.set_default_headers,url,1
 gramex.handlers.basehandler.BaseHandler.on_finish,url,2
 gramex.handlers.basehandler.BaseHandler.get_current_user,url,1
@@ -137,15 +137,15 @@
 gramex.handlers.processhandler.*,url.*.handler=ProcessHandler|Process,17
 gramex.handlers.proxyhandler.*,url.*.handler=ProxyHandler|Proxy,23
 gramex.handlers.socialhandler.SocialHandler.*,url.*.handler=TwitterRESTHandler|Twitter|FacebookGraphHandler|Facebook,23
 gramex.handlers.socialhandler.TwitterRESTHandler.*,url.*.handler=TwitterRESTHandler|Twitter,8
 gramex.handlers.socialhandler.FacebookGraphHandler.*,url.*.handler=FacebookGraphHandler|Facebook,6
 gramex.handlers.uploadhandler.*,url.*.handler=UploadHandler|Upload,44
 gramex.handlers.websockethandler.*,url.*.handler=WebSocketHandler|Websocket,7
-gramex.handlers.__init__.*,url.*.handler=OAuth2|FacebookAuth|TwitterAuth|SAMLAuth|SAMLAuth2|LDAPAuth|DBAuth|IntegratedAuth|SMSAuth|EmailAuth,4
+gramex.handlers.__init__.*,url.*.handler=OAuth2|FacebookAuth|TwitterAuth|SAMLAuth|SAMLAuth2|LDAPAuth|DBAuth|IntegratedAuth|SMSAuth|EmailAuth,7
 gramex.pptgen.*,url.*.handler=PPTXHandler,363
 gramex.pptgen2.*,url.*.handler=PPTXHandler,244
 gramex.services.emailer.*,email,34
 gramex.services.rediscache.*,cache.*.type=redis,23
 gramex.services.scheduler.*,schedule,26
 gramex.services.sms.*,sms,10
 gramex.services.ttlcache.*,cache.*.type=memory,46
```

### Comparing `gramex-1.90.0/gramex/handlers/400.html` & `gramex-1.91.0/gramex/handlers/400.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/401.html` & `gramex-1.91.0/gramex/handlers/401.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/403.html` & `gramex-1.91.0/gramex/handlers/403.html`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,19 @@
       {% try %}{% import gramex %}{% set login_url = gramex.conf.app.settings.login_url %}{% except %}{% end %}
     {% end %}
     {% if handler.request.method not in {'GET', 'HEAD', 'OPTIONS'} and not xsrf %}
       <p>Your app sent a {{ handler.request.method }} request without an XSRF cookie.</p>
     {% elif handler.current_user %}
       <p>You are logged in, but as a user that cannot access this page.</p>
       {% import yaml %}
-      <pre>{{ yaml.safe_dump(handler.current_user, default_flow_style=False) }}</pre>
+      {% try %}
+        <pre>{{ yaml.safe_dump(handler.current_user, default_flow_style=False) }}</pre>
+      {% except Exception %}
+        <pre>{{ handler.current_user }}</pre>
+      {% end %}
       {% if login_url %}<p><a href="{{ login_url }}">Try logging in again</a>.</p>{% end %}
     {% else %}
       <p>You <strong>are not</strong> logged in.</p>
       {% if login_url %}<p><a href="{{ login_url }}">Try logging in</a>.</p>{% end %}
     {% end %}
     <p>Contact the app owner for more information.</p>
     {% set exception = kwargs['exc_info'][1] %}
```

#### html2text {}

```diff
@@ -6,17 +6,19 @@
 handler.kwargs.auth.login_url %}{% except %} {% try %}{% import gramex %}{% set
 login_url = gramex.conf.app.settings.login_url %}{% except %}{% end %} {% end
 %} {% if handler.request.method not in {'GET', 'HEAD', 'OPTIONS'} and not xsrf
 %}
 Your app sent a {{ handler.request.method }} request without an XSRF cookie.
 {% elif handler.current_user %}
 You are logged in, but as a user that cannot access this page.
-{% import yaml %}
+{% import yaml %} {% try %}
 {{ yaml.safe_dump(handler.current_user, default_flow_style=False) }}
-{% if login_url %}
+{% except Exception %}
+{{ handler.current_user }}
+{% end %} {% if login_url %}
 Try_logging_in_again.
 {% end %} {% else %}
 You are not logged in.
 {% if login_url %}
 Try_logging_in.
 {% end %} {% end %}
 Contact the app owner for more information.
```

### Comparing `gramex-1.90.0/gramex/handlers/404.html` & `gramex-1.91.0/gramex/handlers/404.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/500.html` & `gramex-1.91.0/gramex/handlers/500.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/__init__.py` & `gramex-1.91.0/gramex/handlers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 '''Handlers set up the micro-services for [gramex.services.url][].'''
 
 from .basehandler import BaseMixin, BaseHandler, BaseWebSocketHandler, SetupFailedHandler
 from .functionhandler import FunctionHandler
 from .websockethandler import WebSocketHandler
 from .filehandler import FileHandler
-from .authhandler import GoogleAuth, SimpleAuth, LogoutHandler
+from .authhandler import AuthHandler, GoogleAuth, SimpleAuth, LogoutHandler
 from .processhandler import ProcessHandler
 from .jsonhandler import JSONHandler
 from .socialhandler import TwitterRESTHandler, FacebookGraphHandler
 from .uploadhandler import UploadHandler
 from .capturehandler import CaptureHandler, Capture
 from .formhandler import FormHandler
 from .pptxhandler import PPTXHandler
 from .proxyhandler import ProxyHandler
 from .modelhandler import ModelHandler
-from .mlhandler import MLHandler, MLPredictor
 from .filterhandler import FilterHandler
 from .drivehandler import DriveHandler
 from .comichandler import ComicHandler
 from .openapihandler import OpenAPIHandler
 from .messagehandler import MessageHandler
 
 # Aliases
@@ -27,26 +26,26 @@
 Message = CommentHandler = MessageHandler
 Data = FormHandler
 Facebook = FacebookGraphHandler
 File = DirectoryHandler = FileHandler
 Filter = FilterHandler
 Function = FunctionHandler
 JSON = JSONHandler
-ML = MLHandler
 OpenAPI = OpenAPIHandler
 Proxy = ProxyHandler
 Screenshot = CaptureHandler
 Slide = PPTXHandler
 Storage = DriveHandler
 Twitter = TwitterRESTHandler
 Upload = UploadHandler
 Websocket = WebSocketHandler
 
 
 __all__ = [
+    'AuthHandler',
     'BaseHandler',
     'BaseWebSocketHandler',
     'BaseMixin',
     'Capture',
     'CaptureHandler',
     'Command',
     'CommentHandler',
@@ -66,17 +65,14 @@
     'GoogleAuth',
     'JSON',
     'JSONHandler',
     'LogoutHandler',
     'Message',
     'MessageHandler',
     'ModelHandler',
-    'ML',
-    'MLHandler',
-    'MLPredictor',
     'OpenAPI',
     'OpenAPIHandler',
     'PPTXHandler',
     'ProcessHandler',
     'Proxy',
     'ProxyHandler',
     'Screenshot',
@@ -88,14 +84,27 @@
     'TwitterRESTHandler',
     'Upload',
     'UploadHandler',
     'Websocket',
     'WebSocketHandler',
 ]
 
+
+# MLHandler requires optional dependencies scikit-learn and statsmodels.
+# If they're not installed, ignore the import error and skip MLHandler.
+try:
+    from .mlhandler import MLHandler, MLPredictor
+
+    ML = MLHandler
+    __all__ += ['ML', 'MLHandler', 'MLPredictor']
+except ImportError as e:
+    from gramex.config import app_log
+
+    app_log.warning('url: MLHandler/MLPredictor dependency missing. %s', e)
+
 try:
     # If Gramex enterprise is available, import all handlers
     import gramexenterprise.handlers
 
     if hasattr(gramexenterprise, 'handlers'):
         from gramexenterprise.handlers import *  # noqa
```

### Comparing `gramex-1.90.0/gramex/handlers/auth.recaptcha.template.html` & `gramex-1.91.0/gramex/handlers/auth.recaptcha.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/auth.template.html` & `gramex-1.91.0/gramex/handlers/auth.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/authhandler.py` & `gramex-1.91.0/gramex/handlers/authhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,37 +292,39 @@
                 scope=scope,
                 response_type='code',
                 extra_params=self.kwargs.get('extra_params', {}),
             )
 
     @classmethod
     @coroutine
-    def exchange_refresh_token(cls, user, refresh_token=None):
+    def exchange_refresh_token(cls, user: dict, refresh_token: str = None):
         '''
         Exchange the refresh token for the current user for a new access token.
 
         See https://developers.google.com/android-publisher/authorizatio#using_the_refresh_token
 
         The token is picked up from the persistent user info store. Developers can explicitly pass
         a refresh_token as well.
 
-        Sample usage in a FunctionHandler coroutine::
+        Sample usage in a FunctionHandler coroutine
 
-            @tornado.gen.coroutine
-            def refresh(handler):
-                # Get the Google auth handler though which the current user logged in
-                auth_handler = gramex.service.url['google-handler'].handler_class
-                # Exchange refresh token for access token
-                yield auth_handler.exchange_refresh_token(handler.current_user)
-
-        It accepts the following parameters:
-
-        :arg dict user: current user object, i.e. ``handler.current_user`` (read-only)
-        :arg str refresh_token: optional. By default, the refresh token is picked up from
-            ``handler.current_user.refresh_token``
+        ```python
+        @tornado.gen.coroutine
+        def refresh(handler):
+            # Get the Google auth handler though which the current user logged in
+            auth_handler = gramex.service.url['google-handler'].handler_class
+            # Exchange refresh token for access token
+            yield auth_handler.exchange_refresh_token(handler.current_user)
+        ```
+
+        Parameters:
+
+            user: current user object, i.e. `handler.current_user` (read-only)
+            refresh_token: optional. By default, the refresh token is picked up from
+                `handler.current_user.refresh_token`
         '''
         if refresh_token is None:
             if 'refresh_token' in user:
                 refresh_token = user['refresh_token']
             else:
                 raise HTTPError(FORBIDDEN, "No refresh_token provided")
         body = urlencode(
@@ -343,45 +345,51 @@
 
 class SimpleAuth(AuthHandler):
     '''
     Eventually, change this to use an abstract base class for local
     authentication methods -- i.e. where **we** render the login screen, not a third party service.
 
     The login page is rendered in case of a login error as well. The page is a
-    Tornado template that is passed an ``error`` variable. ``error`` is ``None``
-    by default. If the login fails, it must be a ``dict`` with attributes
+    Tornado template that is passed an `error` variable. `error` is `None`
+    by default. If the login fails, it must be a `dict` with attributes
     specific to the handler.
 
-    The simplest configuration (``kwargs``) for SimpleAuth is::
+    The simplest configuration (`kwargs`) for SimpleAuth is
 
-        credentials:                        # Mapping of user IDs and passwords
-            user1: password1                # user1 maps to password1
-            user2: password2
-
-    An alternate configuration is::
-
-        credentials:                        # Mapping of user IDs and user info
-            user1:                          # Each user ID has a dictionary of keys
-                password: password1         # One of them MUST be password
-                email: user1@example.org    # Any other attributes can be added
-                role: employee              # These are available from the session info
-            user2:
-                password: password2
-                email: user2@example.org
-                role: manager
-
-    The full configuration (``kwargs``) for SimpleAuth looks like this::
-
-        template: $YAMLPATH/auth.template.html  # Render the login form template
-        user:
-            arg: user                       # ... the ?user= argument from the form.
-        password:
-            arg: password                   # ... the ?password= argument from the form
-        data:
-            ...                             # Same as above
+    ```yaml
+    credentials:                        # Mapping of user IDs and passwords
+        user1: password1                # user1 maps to password1
+        user2: password2
+    ```
+
+    An alternate configuration is
+
+    ```yaml
+    credentials:                        # Mapping of user IDs and user info
+        user1:                          # Each user ID has a dictionary of keys
+            password: password1         # One of them MUST be password
+            email: user1@example.org    # Any other attributes can be added
+            role: employee              # These are available from the session info
+        user2:
+            password: password2
+            email: user2@example.org
+            role: manager
+    ```
+
+    The full configuration (`kwargs`) for SimpleAuth looks like this
+
+    ```yaml
+    template: $YAMLPATH/auth.template.html  # Render the login form template
+    user:
+        arg: user                       # ... the ?user= argument from the form.
+    password:
+        arg: password                   # ... the ?password= argument from the form
+    data:
+        ...                             # Same as above
+    ```
 
     The login flow is as follows:
 
     1. User visits the SimpleAuth page => shows template (with the user name and password inputs)
     2. User enters user name and password, and submits. Browser redirects with a POST request
     3. Application checks username and password. On match, redirects.
     4. On any error, shows template (with error)
```

### Comparing `gramex-1.90.0/gramex/handlers/basehandler.py` & `gramex-1.91.0/gramex/handlers/basehandler.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,17 @@
 
 # Python 3.8+ supports SameSite cookie attribute. Monkey-patch it for Python 3.7
 # https://stackoverflow.com/a/50813092/100904
 Morsel._reserved.setdefault('samesite', 'SameSite')
 
 
 class BaseMixin:
-    '''Common utilities for all handlers. This is usde by [gramex.handlers.BaseHandler][] and
-    [gramex.handlers.BaseWebSocketHandler][].
+    '''Common utilities for all handlers. This is used by
+    [BaseHandler][gramex.handlers.BaseHandler] and
+    [BaseWebSocketHandler][gramex.handlers.BaseWebSocketHandler].
     '''
 
     @classmethod
     def setup(
         cls,
         transform={},
         redirect={},
@@ -64,15 +65,15 @@
         cls._on_finish_methods = []
         cls._set_xsrf = set_xsrf
 
         cls.kwargs = cls.conf.get('kwargs', AttrDict())
 
         cls.setup_transform(transform)
         cls.setup_redirect(redirect)
-        # Note: call setup_session before setup_auth to ensure that
+        # Note: call setup_session before setup_auth to ensure that .session is available.
         # This also ensures we override_user before auth
         cls.setup_session(conf.app.get('session'))
         cls.setup_ratelimit(ratelimit, conf.app.get('ratelimit'))
         cls.setup_auth(auth)
         cls.setup_error(error)
         cls.setup_xsrf(xsrf_cookies)
         cls.setup_log()
@@ -140,15 +141,16 @@
             val = ''
         if not isinstance(val, str):
             err = f'url:{cls.name}.{key}: {val!r} not a string/list'
             err = err + f', e.g. {eg}' if eg else err
             raise ValueError(err)
         if caps:
             val = val.upper()
-        return set(val.replace(',', ' ').split())
+        # Return de-duplicated list. Avoid set(), use dict to preserve order
+        return list(dict.fromkeys(val.replace(',', ' ').split()))
 
     @classmethod
     def setup_httpmethods(cls, methods: Union[list, tuple, str]):
         methods = cls.get_list(methods, key='methods', eg='[GET, POST]', caps=True)
         if methods:
             cls._http_methods = methods
             cls._on_init_methods.append(cls.check_http_method)
@@ -371,40 +373,57 @@
         cls._on_finish_methods.append(cls.save_session)
 
     @classmethod
     def setup_ratelimit(cls, ratelimit: Union[dict, None], ratelimit_app_conf: Union[dict, None]):
         '''Initialize rate limiting checks'''
         if ratelimit is None:
             return
-        if ratelimit_app_conf is None:
+        if not ratelimit_app_conf:
             raise ValueError(f"url:{cls.name}.ratelimit: no app.ratelimit defined")
-        if 'keys' not in ratelimit:
-            raise ValueError(f'url:{cls.name}.ratelimit.keys: missing')
-        if 'limit' not in ratelimit:
-            raise ValueError(f'url:{cls.name}.ratelimit.limit: missing')
 
         # All ratelimit related info is stored in self._ratelimit
-        cls._ratelimit = AttrDict(key_fn=[])
+        cls._ratelimit = []
+        cls._on_init_methods.append(cls.check_ratelimit)
+        cls._on_finish_methods.append(cls.update_ratelimit)
+
+        if isinstance(ratelimit, (list, tuple)):
+            for ratelimit_conf in ratelimit:
+                cls._setup_ratelimit(ratelimit_conf, ratelimit_app_conf)
+        else:
+            cls._setup_ratelimit(ratelimit, ratelimit_app_conf)
 
-        # Default the pool name to `pattern:`
-        cls._ratelimit.pool = ratelimit.get('pool', cls.conf.pattern)
+    @classmethod
+    def _setup_ratelimit(cls, ratelimit, ratelimit_app_conf):
+        for key in ('keys', 'limit'):
+            if key not in ratelimit:
+                raise ValueError(f'url:{cls.name}.ratelimit.{key}: missing')
+
+        # All info for current ratelimit is in _ratelimit, which is added to cls._ratelimit
+        _ratelimit = AttrDict(
+            # Default the pool name to `pattern:`
+            pool=ratelimit.get('pool', cls.conf.pattern),
+            # Pick up the store location from the default app config
+            store=cls._get_store(ratelimit_app_conf),
+            key_fn=[],
+        )
+        cls._ratelimit.append(_ratelimit)
 
         # Convert keys: into list
         keys_spec = ratelimit['keys']
         # keys: daily, user => keys: [daily, user]
         if isinstance(keys_spec, str):
             keys_spec = cls.get_list(keys_spec, key=cls.name, eg='daily, user', caps=False)
         # keys: {function: ...} => keys: [{function: ...}]
         elif isinstance(keys_spec, dict):
             keys_spec = [keys_spec]
         # keys: must be a list
         elif not isinstance(keys_spec, (list, tuple)):
             raise ValueError(f'url:{cls.name}.ratelimit.keys: needs dict list, not {keys_spec}')
 
-        # Pre-compile keys: into self._ratelimit.keys = [key_fn, key_fn, ...]
+        # Pre-compile keys: into _ratelimit.key_fn = [key_fn, key_fn, ...]
         #   key_fn['function'](self) will return nth key
         #   key_fn['expiry'](self) will return nth expiry (in seconds)
         predefined_keys = ratelimit_app_conf.get('keys', {})
         for index, key_spec in enumerate(keys_spec):
             if isinstance(key_spec, str):
                 # Look up string keys like daily to predefined_keys.
                 if key_spec in predefined_keys:
@@ -414,57 +433,51 @@
                     try:
                         key_spec = {'function': handler_expr(key_spec)}
                     except ValueError:
                         raise ValueError(f'url:{cls.name}.ratelimit.keys: {key_spec} is unknown')
             # {function: ...} MUST be defined for a key. {expiry: ... } is optional
             if not isinstance(key_spec, dict) or 'function' not in key_spec:
                 raise ValueError(f'url:{cls.name}.ratelimit.keys: {key_spec} has no function:')
-            # Compile key/expiry functions into cls._ratelimit.keys[index]['function' / 'expiry']
+            # Compile key/expiry functions into _ratelimit.key_fn[index]['function' / 'expiry']
             key_fn = {}
             for fn in ('function', 'expiry'):
                 if fn in key_spec:
                     key_fn[fn] = build_transform(
                         {'function': key_spec[fn]},
                         vars={'handler': None},
                         filename=f'url:{cls.name}.ratelimit.keys[{index}].{fn}',
                         iter=False,
                     )
-            cls._ratelimit.key_fn.append(key_fn)
+            _ratelimit.key_fn.append(key_fn)
 
         # Ensure limit: is a number or a {function: ...}
         limit_spec = ratelimit['limit']
         if isinstance(limit_spec, (int, float)):
             limit_spec = {'function': limit_spec}
         elif not isinstance(ratelimit['limit'], dict) or 'function' not in ratelimit['limit']:
             example = "{'function': number}"
             raise ValueError(f'url:{cls.name}.ratelimit.limit: needs {example}, not {limit_spec}')
 
-        # Pre-compile limit: into self._ratelimit.limit_fn
-        cls._ratelimit.limit_fn = build_transform(
+        # Pre-compile limit: into _ratelimit.limit_fn
+        _ratelimit.limit_fn = build_transform(
             limit_spec,
             vars={'handler': None},
             filename=f'url:{cls.name}.ratelimit.limit',
             iter=False,
         )
 
-        cls._ratelimit.store = cls._get_store(ratelimit_app_conf)
-        cls._on_init_methods.append(cls.check_ratelimit)
-        cls._on_finish_methods.append(cls.update_ratelimit)
-
     @classmethod
     def reset_ratelimit(cls, pool: str, keys: List[Any], value: int = 0) -> bool:
         '''Reset the rate limit usage for a specific pool.
 
         Examples:
-
             >>> reset_ratelimit('/api', ['2022-01-01', 'x@example.org'])
             >>> reset_ratelimit('/api', ['2022-01-01', 'x@example.org'], 10)
 
         Parameters:
-
             pool: Rate limit pool to use. This is the url's `pattern:` unless you specified a
                 `kwargs.ratelimit.pool:`
             keys: specific instance to reset. If your `ratelimit.keys` is `[daily, user.id]`,
                 keys might look like `['2022-01-01', 'x@example.org']` to clear for that day/user
             value: sets the usage counter to this number (default: `0`)
         '''
         store = cls._get_store(conf.app.get('ratelimit'))
@@ -475,38 +488,42 @@
             store.dump(key, val)
         else:
             return False
 
     @classmethod
     def setup_redirect(cls, redirect):
         '''
-        Any handler can have a ``redirect:`` kwarg that looks like this::
+        Any handler can have a `redirect:` kwarg that looks like this:
 
-            redirect:
-                query: next         # If the URL has a ?next=..., redirect to that page next
-                header: X-Next      # Else if the header has an X-Next=... redirect to that
-                url: ...            # Else redirect to this URL
+        ```yaml
+        redirect:
+            query: next         # If the URL has a ?next=..., redirect to that page next
+            header: X-Next      # Else if the header has an X-Next=... redirect to that
+            url: ...            # Else redirect to this URL
+        ```
 
         Only these 3 keys are allowed. All are optional, and checked in the
-        order specified. So, for example::
+        order specified. So, for example:
 
-            redirect:
-                header: X-Next      # Checks the X-Next header first
-                query: next         # If it's missing, uses the ?next=
+        ```yaml
+        redirect:
+            header: X-Next      # Checks the X-Next header first
+            query: next         # If it's missing, uses the ?next=
+        ```
 
-        You can also specify a string for redirect. ``redirect: ...`` is the same
-        as ``redirect: {url: ...}``.
+        You can also specify a string for redirect. `redirect: ...` is the same
+        as `redirect: {url: ...}`.
 
-        When any BaseHandler subclass calls ``self.save_redirect_page()``, it
-        stores the redirect URL in ``session['_next_url']``. The URL is
+        When any BaseHandler subclass calls `self.save_redirect_page()`, it
+        stores the redirect URL in `session['_next_url']`. The URL is
         calculated relative to the handler's URL.
 
-        After that, when the subclass calls ``self.redirect_next()``, it
-        redirects to ``session['_next_url']`` and clears the value. (If the
-        ``_next_url`` was not stored, we redirect to the home page ``/``.)
+        After that, when the subclass calls `self.redirect_next()`, it
+        redirects to `session['_next_url']` and clears the value. (If the
+        `_next_url` was not stored, we redirect to the home page `/`.)
 
         Only some handlers implement redirection. But they all implement it in
         this same consistent way.
         '''
         # Ensure that redirect is a dictionary before proceeding.
         if isinstance(redirect, str):
             redirect = {'url': redirect}
@@ -607,26 +624,28 @@
             return tmpl.generate(*args, **kwargs)
 
         return error
 
     @classmethod
     def setup_error(cls, error):
         '''
-        Sample configuration::
+        Sample configuration:
 
-            error:
-                404:
-                    path: template.json         # Use a template
-                    autoescape: false           # with no autoescape
-                    whitespace: single          # as a single line
-                    headers:
-                        Content-Type: application/json
-                500:
-                    function: module.fn
-                    args: [=status_code, =kwargs, =handler]
+        ```yaml
+        error:
+            404:
+                path: template.json         # Use a template
+                autoescape: false           # with no autoescape
+                whitespace: single          # as a single line
+                headers:
+                    Content-Type: application/json
+            500:
+                function: module.fn
+                args: [=status_code, =kwargs, =handler]
+        ```
         '''
         if not error:
             return
         if not isinstance(error, dict):
             return app_log.error(f'url:{cls.name}.error is not a dict')
         # Compile all errors handlers
         cls.error = {}
@@ -668,18 +687,20 @@
             if error_code in cls.error:
                 cls.error[error_code]['conf'] = error_config
         cls._write_error, cls.write_error = cls.write_error, cls._write_custom_error
 
     @classmethod
     def setup_xsrf(cls, xsrf_cookies):
         '''
-        Sample configuration::
+        Sample configuration:
 
-            xsrf_cookies: false         # Disables xsrf_cookies
-            xsrf_cookies: true          # or anything other than false keeps it enabled
+        ```yaml
+        xsrf_cookies: false         # Disables xsrf_cookies
+        xsrf_cookies: true          # or anything other than false keeps it enabled
+        ```
         '''
         cls.check_xsrf_cookie = cls.noop if xsrf_cookies is False else cls.xsrf_ajax
 
     def xsrf_check_required(self):
         '''Returns True if the request is (likely) from a browser and needs XSRF check.
 
         This is used to handle XSRF. If the request is NOT from a browser (e.g. server, AJAX),
@@ -707,31 +728,31 @@
     def noop(self):
         '''Does nothing. Used when overriding functions or providing a dummy operation'''
         pass
 
     def save_redirect_page(self):
         '''
         Loop through all redirect: methods and save the first available redirect
-        page against the session. Defaults to previously set value, else ``/``.
+        page against the session. Defaults to previously set value, else `/`.
 
-        See :py:func:`setup_redirect`
+        See [setup_redirect][gramex.handlers.BaseMixin.setup_redirect].
         '''
         for method in self.redirects:
             next_url = method(self)
             if next_url:
                 self.session['_next_url'] = urljoin(self.xrequest_uri, next_url)
                 return
         self.session.setdefault('_next_url', '/')
 
     def redirect_next(self):
         '''
-        Redirect the user ``session['_next_url']``. If it does not exist,
+        Redirect the user `session['_next_url']`. If it does not exist,
         set it up first. Then redirect.
 
-        See :py:func:`setup_redirect`
+        See [setup_redirect][gramex.handlers.BaseMixin.setup_redirect].
         '''
         if '_next_url' not in self.session:
             self.save_redirect_page()
         self.redirect(self.session.pop('_next_url', '/'))
 
     @tornado.gen.coroutine
     def _cached_get(self, *args, **kwargs):
@@ -778,26 +799,27 @@
                     self.write(result)
                 else:
                     for item in result:
                         self.write(item)
                 return
             except Exception:
                 app_log.exception(f'url:{self.name}.error.{status_code} raised an exception')
-        # HTTP 429 error code reports ratelimits
+        # HTTP 429 error code reports ratelimits. Set the headers if ratelimit is set.
+        # Note: Previous headers are cleared, so we need to explicitly write them here.
         if status_code == TOO_MANY_REQUESTS and hasattr(self, '_ratelimit'):
             self.set_ratelimit_headers()
         # If error was not written, use the default error
         self._write_error(status_code, **kwargs)
 
     @property
     def session(self):
         '''
         By default, session is not implemented. You need to specify a
-        ``session:`` section in ``gramex.yaml`` to activate it. It is replaced by
-        the ``get_session`` method as a property.
+        `session:` section in `gramex.yaml` to activate it. It is replaced by
+        the `get_session` method as a property.
         '''
         raise NotImplementedError('Specify a session: section in gramex.yaml')
 
     def _set_new_session_id(self, expires_days):
         '''Sets a new random session ID as the sid: cookie. Returns a bytes object'''
         session_id = b2a_base64(os.urandom(24))[:-1]
         kwargs = dict(self._session_cookie)
@@ -830,23 +852,23 @@
         If no session object exists for the sid, create it.
         By default, the session object contains a "id" holding the "sid" value.
 
         The session is a dict. You must ensure that it is JSON serializable.
 
         Sessions use these pre-defined timing keys (values are timestamps):
 
-        - ``_t`` is the expiry time of the session
-        - ``_l`` is the last time the user accessed a page. Updated by
-          :py:func:`BaseHandler.set_last_visited`
-        - ``_i`` is the inactive expiry duration in seconds, i.e. if ``now > _l +
-          _i``, the session has expired.
+        - `_t` is the expiry time of the session
+        - `_l` is the last time the user accessed a page. Updated by
+          [setup_redirect][gramex.handlers.BaseMixin.set_last_visited]
+        - `_i` is the inactive expiry duration in seconds, i.e. if `now > _l +
+          _i`, the session has expired.
 
-        ``new=`` creates a new session to avoid session fixation.
+        `new=` creates a new session to avoid session fixation.
         https://www.owasp.org/index.php/Session_fixation.
-        :py:func:`gramex.handlers.authhandler.AuthHandler.set_user` uses it.
+        [`set_user()`][gramex.handlers.AuthHandler.set_user] uses it.
         When the user logs in:
 
         - If no old session exists, it returns a new session object.
         - If an old session exists, it creates a new "sid" and new session
           object, copying all old contents, but updates the "id" and expiry (_t).
         '''
         if expires_days is None:
@@ -892,15 +914,15 @@
     def otp(
         self,
         expire: float = 60,
         user: Union[str, dict] = None,
         size: int = None,
         type: str = 'OTP',
     ) -> str:
-        '''Return one-time password valid for ``expire`` seconds.
+        '''Return one-time password valid for `expire` seconds.
 
         The OTP is used as the X-Gramex-OTP header or in `?gramex-otp=` on any request.
         This overrides the user with the passed `user` object for that session.
 
         Parameters:
             expire: Time when this token expires, in seconds (e.g. `60` means 1 minute from now)
             user: User object to store against token. Defaults to current user. Raises HTTP 403
@@ -1019,63 +1041,99 @@
                 self.session['user'] = row['user']
 
     def set_last_visited(self):
         '''Update session last visited time if we track inactive expiry.
 
         - `session._l` is the last time the user accessed a page.
         - `session._i` is the seconds of inactivity after which the session expires.
-        - If `session._i` is set (we track inactive expiry), we set ``session._l` to now.
+        - If `session._i` is set (we track inactive expiry), we set `session._l` to now.
         '''
         # Called by BaseHandler.prepare() when any user accesses a page.
         # For efficiency reasons, don't call get_session every time. Check
         # session only if there's a valid sid cookie (with possibly long expiry)
         if self.get_secure_cookie(self._session_cookie_id, max_age_days=9999999):
             session = self.get_session()
             if '_i' in session:
                 session['_l'] = time.time()
 
     def check_ratelimit(self):
         '''Raise HTTP 429 if usage exceeds rate limit. Set X-Ratelimit-* HTTP headers'''
-        ratelimit = self._ratelimit
-        # Get the rate limit key, limit and expiry
-        ratelimit.key = json.dumps(
-            [ratelimit.pool] + [key_fn['function'](self) for key_fn in ratelimit.key_fn]
-        )
-        ratelimit.limit = ratelimit.limit_fn(self)
-        expiries = [key_fn['expiry'](self) for key_fn in ratelimit.key_fn if 'expiry' in key_fn]
-        # If no expiry is specified, store for 100 years
-        ratelimit.expiry = min(expiries + [3155760000])
-
-        # Ensure usage does not hit limit
-        ratelimit.usage = ratelimit.store.load(ratelimit.key, {'n': 0}).get('n', 0)
-        if ratelimit.usage >= ratelimit.limit:
-            raise HTTPError(TOO_MANY_REQUESTS, f'{ratelimit.key} hit rate limit {ratelimit.limit}')
+        for ratelimit in self._ratelimit:
+            # Get the rate limit key, limit and expiry
+            ratelimit.key = json.dumps(
+                [ratelimit.pool] + [key_fn['function'](self) for key_fn in ratelimit.key_fn]
+            )
+            # Note: if ratelimit_fn() returns a non-int, check_ratelimit will fail. Let it fail.
+            ratelimit.limit = ratelimit.limit_fn(self)
+            expiries = [
+                key_fn['expiry'](self) for key_fn in ratelimit.key_fn if 'expiry' in key_fn
+            ]
+            # If no expiry is specified, store for 100 years
+            ratelimit.expiry = min(expiries + [3155760000])
+
+            # Ensure usage does not hit limit
+            ratelimit.usage = ratelimit.store.load(ratelimit.key, {'n': 0}).get('n', 0)
+            if ratelimit.usage >= ratelimit.limit:
+                raise HTTPError(
+                    TOO_MANY_REQUESTS,
+                    f'{ratelimit.pool}: {ratelimit.key} hit rate limit {ratelimit.limit}',
+                )
         self.set_ratelimit_headers()
 
     def update_ratelimit(self):
         '''If request succeeds, increase rate limit usage count by 1'''
-        ratelimit = self._ratelimit
-        # If check_ratelimit failed (e.g. invalid function) and didn't set a key, skip update
         # If response is a HTTP error, don't count towards rate limit
-        if 'key' not in ratelimit or self.get_status() >= 400:
+        if self.get_status() >= 400:
             return
-        # Increment the rate limit by 1
-        usage_obj = ratelimit.store.load(ratelimit.key, {'n': 0})
-        usage_obj['n'] += 1
-        usage_obj['_t'] = time.time() + ratelimit.expiry
-        ratelimit.store.dump(ratelimit.key, usage_obj)
+        for ratelimit in self._ratelimit:
+            # If check_ratelimit failed (e.g. invalid function) and didn't set a key, skip update
+            if 'key' not in ratelimit:
+                return
+            # Increment the rate limit by 1
+            usage_obj = ratelimit.store.load(ratelimit.key, {'n': 0})
+            usage_obj['n'] += 1
+            usage_obj['_t'] = time.time() + ratelimit.expiry
+            ratelimit.store.dump(ratelimit.key, usage_obj)
+
+    def get_ratelimit(self):
+        '''Get the rate limit with the least remaining usage for the current request.
+
+        If there are multiple rate limits, it picks the one with least remaining usage and
+        returns an AttrDict with these keys:
+
+        - `limit`: the limit on the rate limit (e.g. 3)
+        - `usage`: the usage so far (BEFORE current request, e.g. 0, 1, 2, 3, ...)
+        - `remaining`: the remaining requests (AFTER current request, e.g. 2, 1, 0, 0, ...)
+        - `expiry`: seconds to expiry for this rate limit
+        '''
+        ratelimit = min(self._ratelimit, key=lambda r: r.limit - r.usage)
+        return AttrDict(
+            limit=ratelimit.limit,
+            usage=ratelimit.usage,
+            # ratelimit.usage goes 0, 1, 2, ...
+            # If limit is 3, remaining goes 2, 1, 0, ... -- use (limit - usage - 1)
+            # But when usage hits 3, don't show remaining = -1. Show remaining = 0 using max()
+            remaining=max(ratelimit.limit - ratelimit.usage - 1, 0),
+            expiry=ratelimit.expiry,
+        )
 
     def set_ratelimit_headers(self):
-        ratelimit = self._ratelimit
-        # ratelimit.usage goes 0, 1, 2, ...
-        # If limit is 3, remaining goes 3, 2, 1, ... -- use (limit - usage - 1)
-        # But when usage hits 3, don't show remaining = -1. Show remaining = 0 using max()
-        remaining = max(ratelimit.limit - ratelimit.usage - 1, 0)
+        '''Sets the headers from the [Ratelimit HTTP headers draft][1].
+
+        - `X-Ratelimit-Limit` is the rate limit
+        - `X-Ratelimit-Remaining` has the remaining requests
+        - `X-Ratelimit-Reset` has seconds after which the rate limit resets
+        - `Retry-After` is same as X-Ratelimit-Reset, but is set only if the limit is exceeded
+
+        [1]: https://www.ietf.org/archive/id/draft-polli-ratelimit-headers-02.html
+        '''
+        # Pick the rate limit with the lowest remaining count
+        ratelimit = self.get_ratelimit()
         self.set_header('X-Ratelimit-Limit', str(ratelimit.limit))
-        self.set_header('X-Ratelimit-Remaining', str(remaining))
+        self.set_header('X-Ratelimit-Remaining', str(ratelimit.remaining))
         self.set_header('X-RateLimit-Reset', str(ratelimit.expiry))
         if ratelimit.usage >= ratelimit.limit:
             self.set_header('Retry-After', str(ratelimit.expiry))
 
     def initialize_handler(self):
         '''Initialize self.args and other handler attributes'''
         # self.request.arguments does not handle unicode keys well. It returns latin-1 unicode.
@@ -1114,23 +1172,23 @@
             self.request.method = self.args.pop('x-http-method-override')[0].upper()
         elif 'X-HTTP-Method-Override' in self.request.headers:
             self.request.method = self.request.headers['X-HTTP-Method-Override'].upper()
 
     def get_arg(self, name, default=..., first=False):
         '''
         Returns the value of the argument with the given name. Similar to
-        ``.get_argument`` but uses ``self.args`` instead.
+        `.get_argument` but uses `self.args` instead.
 
         If default is not provided, the argument is considered to be
         required, and we raise a `MissingArgumentError` if it is missing.
 
-        If the argument is repeated, we return the last value. If ``first=True``
+        If the argument is repeated, we return the last value. If `first=True`
         is passed, we return the first value.
 
-        ``self.args`` is always UTF-8 decoded unicode. Whitespaces are stripped.
+        `self.args` is always UTF-8 decoded unicode. Whitespaces are stripped.
         '''
         if name not in self.args:
             if default is ...:
                 raise MissingArgumentError(name)
             return default
         return self.args[name][0 if first else -1]
 
@@ -1160,15 +1218,15 @@
 
     def on_finish(self):
         # Loop through class-level callbacks
         for callback in self._on_finish_methods:
             callback(self)
 
     def get_current_user(self):
-        '''Return the ``user`` key from the session as an AttrDict if it exists.'''
+        '''Return the `user` key from the session as an AttrDict if it exists.'''
         result = self.session.get('user')
         return AttrDict(result) if isinstance(result, dict) else result
 
     def log_exception(self, typ, value, tb):
         '''Store the exception value for logging'''
         super(BaseHandler, self).log_exception(typ, value, tb)
         # _exception is stored for use by log_request. Sample error string:
@@ -1209,83 +1267,99 @@
                     if template:
                         self.set_status(FORBIDDEN)
                         self.render(template)
                     raise HTTPError(FORBIDDEN)
 
     def argparse(self, *args, **kwargs):
         '''
-        Parse URL query parameters and return an AttrDict. For example::
+        Parse URL query parameters and return an AttrDict. For example:
 
-            args = handler.argparse('x', 'y')
-            args.x      # is the last value of ?x=value
-            args.y      # is the last value of ?y=value
+        ```python
+        args = handler.argparse('x', 'y')
+        args.x      # is the last value of ?x=value
+        args.y      # is the last value of ?y=value
+        ```
 
-        A missing ``?x=`` or ``?y=`` raises a HTTP 400 error mentioning the
+        A missing `?x=` or `?y=` raises a HTTP 400 error mentioning the
         missing key.
 
-        For optional arguments, use::
-
-            args = handler.argparse(z={'default': ''})
-            args.z      # returns '' if ?z= is missing
+        For optional arguments, use:
 
-        You can convert the value to a type::
-
-            args = handler.argparse(limit={'type': int, 'default': 100})
-            args.limit      # returns ?limit= as an integer
+        ```python
+        args = handler.argparse(z={'default': ''})
+        args.z      # returns '' if ?z= is missing
+        ```
+
+        You can convert the value to a type:
+
+        ```python
+        args = handler.argparse(limit={'type': int, 'default': 100})
+        args.limit      # returns ?limit= as an integer
+        ```
 
         You can restrict the choice of values. If the query parameter is not in
-        choices, we raise a HTTP 400 error mentioning the invalid key & value::
-
-            args = handler.argparse(gender={'choices': ['M', 'F']})
-            args.gender      # returns ?gender= which will be 'M' or 'F'
+        choices, we raise a HTTP 400 error mentioning the invalid key & value:
 
-        You can retrieve multiple values as a list::
-
-            args = handler.argparse(cols={'nargs': '*', 'default': []})
-            args.cols       # returns an array with all ?col= values
-
-        ``type:`` conversion and ``choices:`` apply to each value in the list.
-
-        To return all arguments as a list, pass ``list`` as the first parameter::
-
-            args = handler.argparse(list, 'x', 'y')
-            args.x      # ?x=1 sets args.x to ['1'], not '1'
-            args.y      # Similarly for ?y=1
-
-        To handle unicode arguments and return all arguments as ``str`` or
-        ``unicode`` or ``bytes``, pass the type as the first parameter::
-
-            args = handler.argparse(str, 'x', 'y')
-            args = handler.argparse(bytes, 'x', 'y')
-            args = handler.argparse(unicode, 'x', 'y')
+        ```python
+        args = handler.argparse(gender={'choices': ['M', 'F']})
+        args.gender      # returns ?gender= which will be 'M' or 'F'
+        ```
+
+        You can retrieve multiple values as a list:
+
+        ```python
+        args = handler.argparse(cols={'nargs': '*', 'default': []})
+        args.cols       # returns an array with all ?col= values
+        ```
+
+        `type:` conversion and `choices:` apply to each value in the list.
+
+        To return all arguments as a list, pass `list` as the first parameter:
+
+        ```python
+        args = handler.argparse(list, 'x', 'y')
+        args.x      # ?x=1 sets args.x to ['1'], not '1'
+        args.y      # Similarly for ?y=1
+        ```
+
+        To handle unicode arguments and return all arguments as `str` or
+        `unicode` or `bytes`, pass the type as the first parameter:
+
+        ```python
+        args = handler.argparse(str, 'x', 'y')
+        args = handler.argparse(bytes, 'x', 'y')
+        args = handler.argparse(unicode, 'x', 'y')
+        ```
 
         By default, all arguments are added as str in PY3 and unicode in PY2.
 
         There are the full list of parameters you can pass to each keyword
         argument:
 
         - name: Name of the URL query parameter to read. Defaults to the key
         - required: Whether or not the query parameter may be omitted
         - default: The value produced if the argument is missing. Implies required=False
         - nargs: The number of parameters that should be returned. '*' or '+'
           return all values as a list.
         - type: Python type to which the parameter should be converted (e.g. `int`)
         - choices: A container of the allowable values for the argument (after type conversion)
 
-        You can combine all these options. For example::
+        You can combine all these options. For example:
 
-            args = handler.argparse(
-                'name',                         # Raise error if ?name= is missing
-                department={'name': 'dept'},    # ?dept= is mapped to args.department
-                org={'default': 'Gramener'},    # If ?org= is missing, defaults to Gramener
-                age={'type': int},              # Convert ?age= to an integer
-                married={'type': bool},         # Convert ?married to a boolean
-                alias={'nargs': '*'},           # Convert all ?alias= to a list
-                gender={'choices': ['M', 'F']}, # Raise error if gender is not M or F
-            )
+        ```python
+        args = handler.argparse(
+            'name',                         # Raise error if ?name= is missing
+            department={'name': 'dept'},    # ?dept= is mapped to args.department
+            org={'default': 'Gramener'},    # If ?org= is missing, defaults to Gramener
+            age={'type': int},              # Convert ?age= to an integer
+            married={'type': bool},         # Convert ?married to a boolean
+            alias={'nargs': '*'},           # Convert all ?alias= to a list
+            gender={'choices': ['M', 'F']}, # Raise error if gender is not M or F
+        )
+        ```
         '''
         result = AttrDict()
 
         args_type = str
         if len(args) > 0 and args[0] in (str, bytes, list, None):
             args_type, args = args[0], args[1:]
 
@@ -1376,15 +1450,15 @@
 
     def on_close(self):
         # Loop through class-level callbacks
         for callback in self._on_finish_methods:
             callback(self)
 
     def get_current_user(self):
-        '''Return the ``user`` key from the session as an AttrDict if it exists.'''
+        '''Return the `user` key from the session as an AttrDict if it exists.'''
         result = self.session.get('user')
         return AttrDict(result) if isinstance(result, dict) else result
 
     def authorize(self):
         '''If a valid user isn't logged in, send a message and close connection'''
         if not self.current_user:
             raise HTTPError(UNAUTHORIZED)
```

### Comparing `gramex-1.90.0/gramex/handlers/capturehandler.py` & `gramex-1.91.0/gramex/handlers/capturehandler.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,38 +49,44 @@
             script='chromecapture.js',
             first_line=b'node\\.js.*chromecapture\\.js',
             name='ChromeCapture',
             version='1.1',
         ),
     )
 
-    '''
-    Create a proxy for capture.js. Typical usage::
-
-        capture = Capture()
-        with open('screenshot.png', 'wb') as handle:
-            handle.write(capture.png('https://gramener.com/'))
-        with open('screenshot.pdf', 'wb') as handle:
-            handle.write(capture.pdf('https://gramener.com/'))
-
-    The constructor accepts these optional parameters:
-
-    :arg int port: port where capture.js is running. Default: 9900
-    :arg string url: URL:port where PhantomJS is running with capture.js.
-        Default: ``http://localhost:<port>/``
-    :arg string cmd: Command to run PhantomJS with capture.js at the specified
-        port. Default: ``phantomjs $GRAMEXPATH/apps/capture/capture.js --port=<port>``
-    :arg int timeout: Seconds to wait for PhantomJS to timeout. Default: 10
-
-    The constructor runs :meth:`Capture.start` in a new thread, which checks if
-    capture.js is running at ``url``. If not, it runs ``cmd`` and checks again.
-    Until capture.js is detected, all capture methods will fail.
-    '''
-
-    def __init__(self, port=None, url=None, engine=None, cmd=None, timeout=DEFAULT_TIMEOUT):
+    def __init__(
+        self,
+        port: int = None,
+        url: str = None,
+        engine: str = None,
+        cmd: str = None,
+        timeout: int = DEFAULT_TIMEOUT,
+    ):
+        '''
+        Create a proxy for capture.js.
+
+        Examples:
+            >>> capture = Capture()
+            >>> with open('screenshot.png', 'wb') as handle:
+            ...    handle.write(capture.png('https://gramener.com/'))
+            >>> with open('screenshot.pdf', 'wb') as handle:
+            ...    handle.write(capture.pdf('https://gramener.com/'))
+
+        Parameters:
+            port: port where capture.js is running. Default: 9900
+            url: URL:port where PhantomJS is running with capture.js.
+                Default: `http://localhost:<port>/`
+            cmd: Command to run PhantomJS with capture.js at the specified
+                port. Default: `phantomjs $GRAMEXPATH/apps/capture/capture.js --port=<port>`
+            timeout: Seconds to wait for PhantomJS to timeout. Default: 10
+
+        The constructor runs `Capture.start()` in a new thread, which checks if
+        capture.js is running at `url`. If not, it runs `cmd` and checks again.
+        Until capture.js is detected, all capture methods will fail.
+        '''
         # Set default values for port, url and cmd
         self.engine = self.engines['phantomjs' if engine is None else engine]
         port = self.default_port if port is None else port
         if url is None:
             url = f'http://localhost:{port}/'
             if cmd is None:
                 script = os.path.join(variables.GRAMEXPATH, 'apps', 'capture', self.engine.script)
@@ -92,29 +98,29 @@
         self.browser = AsyncHTTPClient()
         self.lock = Lock()
         self.started = False
         self.start()
 
     def start(self):
         '''
-        Starts a thread and check if capture is already running at ``url``. If
-        not, start ``cmd`` and check again. Print logs from ``cmd``.
+        Starts a thread and check if capture is already running at `url`. If
+        not, start `cmd` and check again. Print logs from `cmd`.
 
         This method is thread-safe. It may be called as often as required.
-        :class:`CaptureHandler` calls this method if ``?start`` is passed.
+        CaptureHandler calls this method if `?start` is passed.
         '''
         with self.lock:
             thread = Thread(target=self._start, name=f'Capture {self.engine} @ {self.url}')
             thread.daemon = True
             thread.start()
 
     def _start(self):
         '''
-        Check if capture is already running at ``url``. If not, start ``cmd``
-        and check again. Print logs from ``cmd``.
+        Check if capture is already running at `url`. If not, start `cmd`
+        and check again. Print logs from `cmd`.
         '''
         self.started = False
         script = self.engine.script
         try:
             # Check if capture.js is at the url specified
             app_log.info(f'Pinging {script} at {self.url}')
             r = requests.get(self.url, timeout=self.timeout)
@@ -179,15 +185,15 @@
         if len(parts) != 2 or parts[0] != self.engine.name or parts[1] < self.engine.version:
             raise RuntimeError(f'Server: {server} at {self.url} is not {script}')
 
     @tornado.gen.coroutine
     def capture_async(self, headers=None, **kwargs):
         '''
         Returns a screenshot of the URL. Runs asynchronously in Gramex. Arguments
-        are same as :py:func:`capture`
+        are same as [capture][gramex.handlers.capturehandler.Capture.capture]
         '''
         # If ?start is provided, start server and wait until timeout
         if 'start' in kwargs:
             self.start()
             end_time = time.time() + self.timeout
             while not self.started and time.time() < end_time:
                 yield tornado.gen.sleep(self.check_interval)
@@ -206,32 +212,36 @@
             self._validate_server(r)
         raise tornado.gen.Return(r)
 
     def capture(self, url, **kwargs):
         '''
         Return a screenshot of the URL.
 
-        :arg str url: URL to take a screenshot of
-        :arg str ext: format of output. Can be pdf, png, gif or jpg
-        :arg str selector: Restrict screenshot to (optional) CSS selector in URL
-        :arg int delay: milliseconds (or expression) to wait for before taking a screenshot
-        :arg str format: A3, A4, A5, Legal, Letter or Tabloid. Defaults to A4. For PDF
-        :arg str layout: A3, A4, A5, Legal, 16x9, 16x10, 4x3. Defaults to 4x3. For PPTX
-        :arg str orientation: portrait or landscape. Defaults to portrait. For PDF
-        :arg str header: header for the page. For PDF
-        :arg str footer: footer for the page. For PDF
-        :arg int width: screen width. Default: 1200. For PNG/GIF/JPG
-        :arg int height: screen height. Default: 768. For PNG/GIF/JPG
-        :arg float scale: zooms the screen by a factor. For PNG/GIF/JPG
-        :arg int dpi: dots (pixels) per inch. For PPTX
-        :arg str title: slide title. For PPTX
-        :arg int debug: sets log level for HTTP requests (2) and responses (1)
-        :return: a bytestring with the binary contents of the screenshot
-        :rtype: bytes
-        :raises RuntimeError: if capture.js is not running or fails
+        Parameters:
+            url (str): URL to take a screenshot of
+            ext (str): format of output. Can be pdf, png, gif or jpg
+            selector (str): Restrict screenshot to (optional) CSS selector in URL
+            delay (int): milliseconds (or expression) to wait for before taking a screenshot
+            format (str): A3, A4, A5, Legal, Letter or Tabloid. Defaults to A4. For PDF
+            layout (str): A3, A4, A5, Legal, 16x9, 16x10, 4x3. Defaults to 4x3. For PPTX
+            orientation (str): portrait or landscape. Defaults to portrait. For PDF
+            header (str): header for the page. For PDF
+            footer (str): footer for the page. For PDF
+            width (int): screen width. Default: 1200. For PNG/GIF/JPG
+            height (int): screen height. Default: 768. For PNG/GIF/JPG
+            scale (float): zooms the screen by a factor. For PNG/GIF/JPG
+            dpi (int): dots (pixels) per inch. For PPTX
+            title (str): slide title. For PPTX
+            debug (int): sets log level for HTTP requests (2) and responses (1)
+
+        Returns:
+            a bytestring with the binary contents of the screenshot
+
+        Raises:
+            RuntimeError: if capture.js is not running or fails
         '''
         # Ensure that we're connecting to the right version of capture.js
         if not self.started:
             end_time = time.time() + self.timeout
             while not self.started and time.time() < end_time:
                 time.sleep(self.check_interval)
             if not self.started:
@@ -241,46 +251,46 @@
         if r.status_code == OK:
             self._validate_server(r)
             return r.content
         else:
             raise RuntimeError(f'{self.engine.script} error: {r.content}')
 
     def pdf(self, url, **kwargs):
-        '''An alias for :meth:`Capture.capture` with ``ext='pdf'``.'''
+        '''An alias for `Capture.capture()` with `ext='pdf'`.'''
         kwargs['ext'] = 'pdf'
         return self.capture(url, **kwargs)
 
     def png(self, url, **kwargs):
-        '''An alias for :meth:`Capture.capture` with ``ext='png'``.'''
+        '''An alias for `Capture.capture()` with `ext='png'`.'''
         kwargs['ext'] = 'png'
         return self.capture(url, **kwargs)
 
     def pptx(self, url, **kwargs):
-        '''An alias for :meth:`Capture.capture` with ``ext='pptx'``.'''
+        '''An alias for `Capture.capture()` with `ext='pptx'`.'''
         kwargs['ext'] = 'pptx'
         return self.capture(url, **kwargs)
 
     def jpg(self, url, **kwargs):
-        '''An alias for :meth:`Capture.capture` with ``ext='jpg'``.'''
+        '''An alias for `Capture.capture()` with `ext='jpg'`.'''
         kwargs['ext'] = 'jpg'
         return self.capture(url, **kwargs)
 
     def gif(self, url, **kwargs):
-        '''An alias for :meth:`Capture.capture` with ``ext='gif'``.'''
+        '''An alias for `Capture.capture()` with `ext='gif'`.'''
         kwargs['ext'] = 'gif'
         return self.capture(url, **kwargs)
 
 
 class CaptureHandler(BaseHandler):
     '''
     Renders a web page as a PDF or as an image. It accepts the same arguments as
-    :class:`Capture`.
+    `Capture`.
 
-    The page is called with the same args as :meth:`Capture.capture`. It also
-    accepts a ``?start`` parameter that restarts capture.js if required.
+    The page is called with the same args as `Capture.capture()`. It also
+    accepts a `?start` parameter that restarts capture.js if required.
     '''
 
     # Each config maps to a Capture() object. cls.captures[config] = Capture()
     captures = {}
 
     @classmethod
     def setup(cls, port=None, url=None, engine=None, cmd=None, timeout=DEFAULT_TIMEOUT, **kwargs):
```

### Comparing `gramex-1.90.0/gramex/handlers/comichandler.py` & `gramex-1.91.0/gramex/handlers/comichandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/drivehandler.py` & `gramex-1.91.0/gramex/handlers/drivehandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 from gramex.config import objectpath, slug
 from gramex.http import NOT_FOUND, REQUEST_ENTITY_TOO_LARGE, UNSUPPORTED_MEDIA_TYPE
 from .formhandler import FormHandler
 
 
 class DriveHandler(FormHandler):
     '''
-    Lets users manage files. Here's a typical configuration::
+    Lets users manage files. Here's a typical configuration
 
-        path: $GRAMEXDATA/apps/appname/     # Save files here
-        user_fields: [id, role, hd]         # user attributes to store
-        tags: [tag]                         # <input name=""> to store
-        allow: [.doc, .docx]                # Only allow these files
-        ignore: [.pdf]                      # Don't allow these files
-        max_file_size: 100000               # Files must be smaller than this
-        redirect:                           # After uploading the file,
-            query: next                     #   ... redirect to ?next=
-            url: /$YAMLURL/                 #   ... else to this directory
+    ```yaml
+    path: $GRAMEXDATA/apps/appname/     # Save files here
+    user_fields: [id, role, hd]         # user attributes to store
+    tags: [tag]                         # <input name=""> to store
+    allow: [.doc, .docx]                # Only allow these files
+    ignore: [.pdf]                      # Don't allow these files
+    max_file_size: 100000               # Files must be smaller than this
+    redirect:                           # After uploading the file,
+        query: next                     #   ... redirect to ?next=
+        url: /$YAMLURL/                 #   ... else to this directory
+    ```
 
     File metadata is stored in <path>/.meta.db as SQLite
     '''
 
     @classmethod
     def setup(
         cls,
```

### Comparing `gramex-1.90.0/gramex/handlers/filehandler.py` & `gramex-1.91.0/gramex/handlers/filehandler.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,92 +28,87 @@
     '''
     Check if path matches pattern -- case insensitively.
     '''
     return fnmatch(str(path).lower(), '*/' + pat.lower())
 
 
 class FileHandler(BaseHandler):
-    '''
-    Serves files with transformations. It accepts these parameters:
-
-    :arg string path: Can be one of these:
-
-        - The filename to serve. For all files matching the pattern, this
-          filename is returned.
-        - The root directory from which files are served. The first parameter of
-          the URL pattern is the file path under this directory. Relative paths
-          are specified from where gramex was run.
-        - A wildcard path where `*` is replaced by the URL pattern's first
-          `(..)` group.
-        - A list of files to serve. These files are concatenated and served one
-          after the other.
-        - A dict of {regex: path}. If the URL matches the regex, the path is
-          served. The path is string formatted using the regex capture groups
-
-    :arg string default_filename: If the URL maps to a directory, this filename
-        is displayed by default. For example, ``index.html`` or ``README.md``.
-        It can be a list of default filenames tried in order, e.g.
-        ``[index.template.html, index.html, README.md]``.
-        The default is ``None``, which displays all files in the directory
-        using the ``index_template`` option.
-    :arg boolean index: If ``true``, shows a directory index. If ``false``,
-        raises a HTTP 404: Not Found error when users try to access a directory.
-    :arg list ignore: List of glob patterns to ignore. Even if the path matches
-        these, the files will not be served.
-    :arg list allow: List of glob patterns to allow. This overrides the ignore
-        patterns, so use with care.
-    :arg string index_template: The file to be used as the template for
-        displaying the index. If this file is missing, it defaults to Gramex's
-        default ``filehandler.template.html``. It can use these string
-        variables:
-
-        - ``$path`` - the directory name
-        - ``$body`` - an unordered list with all filenames as links
-    :arg dict headers: HTTP headers to set on the response.
-    :arg dict transform: Transformations that should be applied to the files.
-        The key matches one or more `glob patterns`_ separated by space/comma
-        (e.g. ``'*.md, 'data/**'``.) The value is a dict with the same
-        structure as :class:`FunctionHandler`, and accepts these keys:
-
-        ``function``
-            The expression to return. Example: ``function: mymodule.transform(content, handler)``.
-            ``content`` has the file contents. ``handler`` has the FileHandler object
-
-        ``encoding``
-            The encoding to read the file with, e.g. ``utf-8``. If ``None`` (the default), the
-            file is read as bytes, and the transform `function` MUST accept the content as bytes
-
-        ``headers``:
-            HTTP headers to set on the response
-    :arg string template: ``template="*.html"`` renders all HTML files as Tornado templates.
-        ``template=True`` renders all files as Tornado templates (new in Gramex 1.14).
-    :arg string sass: ``sass="*.sass"`` renders all SASS files as CSS (new in Gramex 1.66).
-    :arg string scss: ``scss="*.scss"`` renders all SCSS files as CSS (new in Gramex 1.66).
-    :arg string ts: ``ts="*.ts"`` renders all TypeScript files as JS (new in Gramex 1.78).
-
-    .. _glob patterns: https://docs.python.org/3/library/pathlib.html#pathlib.Path.glob
-
-    FileHandler exposes these attributes:
-
-    - ``root``: Root path for this handler. Aligns with the ``path`` argument
-    - ``path``; Absolute path requested by the user, without adding a default filename
-    - ``file``: Absolute path served to the user, after adding a default filename
-    '''
-
     @classmethod
     def setup(
         cls,
-        path,
-        default_filename=None,
-        index=None,
-        index_template=None,
-        headers={},
+        path: str,
+        default_filename: str = None,
+        index: bool = None,
+        index_template: str = None,
+        headers: dict = {},
         default={},
         **kwargs,
     ):
+        '''
+        Serves files with transformations.
+
+        Parameters:
+
+            path: Can be one of these:
+
+                - The filename to serve. For all files matching the pattern, this
+                filename is returned.
+                - The root directory from which files are served. The first parameter of
+                the URL pattern is the file path under this directory. Relative paths
+                are specified from where gramex was run.
+                - A wildcard path where `*` is replaced by the URL pattern's first
+                `(..)` group.
+                - A list of files to serve. These files are concatenated and served one
+                after the other.
+                - A dict of {regex: path}. If the URL matches the regex, the path is
+                served. The path is string formatted using the regex capture groups
+
+            default_filename: If the URL maps to a directory, this filename
+                is displayed by default. For example, `index.html` or `README.md`.
+                It can be a list of default filenames tried in order, e.g.
+                `[index.template.html, index.html, README.md]`.
+                The default is `None`, which displays all files in the directory
+                using the `index_template` option.
+            index: If `true`, shows a directory index. If `false`,
+                raises a HTTP 404: Not Found error when users try to access a directory.
+            ignore: List of glob patterns to ignore. Even if the path matches
+                these, the files will not be served.
+            allow: List of glob patterns to allow. This overrides the ignore
+                patterns, so use with care.
+            index_template: The file to be used as the template for
+                displaying the index. If this file is missing, it defaults to Gramex's
+                default `filehandler.template.html`. It can use these string
+                variables:
+
+                - `$path` - the directory name
+                - `$body` - an unordered list with all filenames as links
+            headers: HTTP headers to set on the response.
+            transform: Transformations that should be applied to the files.
+                The key matches one or more `glob patterns` separated by space/comma
+                (e.g. `'*.md, 'data/**'`.) The value is a dict with the same
+                structure as [FunctionHandler][gramex.handlers.FunctionHandler], and accepts keys:
+
+                - `function`: The expression to return. E.g.: `function: method(content, handler)`.
+                    `content` has the file contents. `handler` has the FileHandler object
+                - `encoding`: Encoding to read the file with, e.g. `utf-8`. If `None` (default),
+                    file is read as bytes. Transform `function` MUST accept the content as bytes
+                - `headers`: HTTP headers to set on the response
+
+            template: `template="*.html"` renders all HTML files as Tornado templates.
+                `template=True` renders all files as Tornado templates (new in Gramex 1.14).
+            sass: `sass="*.sass"` renders all SASS files as CSS (new in Gramex 1.66).
+            scss: `scss="*.scss"` renders all SCSS files as CSS (new in Gramex 1.66).
+            ts: `ts="*.ts"` renders all TypeScript files as JS (new in Gramex 1.78).
+
+        FileHandler exposes these attributes:
+
+        - `root`: Root path for this handler. Aligns with the `path` argument
+        - `path`; Absolute path requested by the user, without adding a default filename
+        - `file`: Absolute path served to the user, after adding a default filename
+        '''
         # Convert template: '*.html' into transform: {'*.html': {function: template}}
         # Convert sass: ['*.scss', '*.sass'] into transform: {'*.scss': {function: sass}}
         # Do this before BaseHandler setup so that it can invoke the transforms required
         for key in ('template', 'sass', 'scss', 'ts', 'vue'):
             val = kwargs.pop(key, None)
             if val:
                 # template/sass/...: true is the same as template: '*'
```

### Comparing `gramex-1.90.0/gramex/handlers/filehandler.template.html` & `gramex-1.91.0/gramex/handlers/filehandler.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/formhandler.py` & `gramex-1.91.0/gramex/handlers/formhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/functionhandler.py` & `gramex-1.91.0/gramex/handlers/functionhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/jsonhandler.py` & `gramex-1.91.0/gramex/handlers/jsonhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,42 @@
 # stored in _loaded[path].
 store = {}  # Contents of the JSON data stores
 _loaded = {}  # Time when persistent stores were last loaded
 _jsonstores = store  # Internal legacy alias for store
 
 
 class JSONHandler(BaseHandler):
-    '''
-    Provides a REST API for managing and persisting JSON data.
+    @classmethod
+    def setup(cls, path: str = None, data: str = None, **kwargs):
+        '''
+        Provides a REST API for managing and persisting JSON data.
 
-    Sample URL configuration::
+        Sample URL configuration
 
+        ```yaml
         pattern: /$YAMLURL/data/(.*)
         handler: JSONHandler
         kwargs:
             path: $YAMLPATH/data.json
+        ```
+
+        Parameters:
 
-    :arg string path: optional file where the JSON data is persisted. If not
-        specified, the JSON data is not persisted.
-    :arg string data: optional initial dataset, used only if path is not
-        specified. Defaults to null
-    '''
+            path: optional file where the JSON data is persisted. If not
+                specified, the JSON data is not persisted.
+            data: optional initial dataset, used only if path is not
+                specified. Defaults to null
+        '''
+        super(JSONHandler, cls).setup(**kwargs)
+        cls.path = path
+        cls.default_data = data
+        cls.json_kwargs = {
+            'ensure_ascii': True,
+            'separators': (',', ':'),
+        }
 
     def parse_body_as_json(self):
         try:
             return tornado.escape.json_decode(self.request.body)
         except ValueError:
             raise tornado.web.HTTPError(BAD_REQUEST, 'Bad JSON')
 
@@ -86,24 +99,14 @@
                     parent[keys[index]] = data = {}
                 data[key] = {}
                 parent, data = data, data[key]
                 continue
             return parent, key, None
         return parent, key, data
 
-    @classmethod
-    def setup(cls, path=None, data=None, **kwargs):
-        super(JSONHandler, cls).setup(**kwargs)
-        cls.path = path
-        cls.default_data = data
-        cls.json_kwargs = {
-            'ensure_ascii': True,
-            'separators': (',', ':'),
-        }
-
     def initialize(self, **kwargs):
         super(JSONHandler, self).initialize(**kwargs)
         self.set_header('Content-Type', 'application/json')
 
     def get(self, jsonpath):
         '''Return the JSON data at jsonpath. Return null for invalid paths.'''
         parent, key, data = self.jsonwalk(jsonpath, create=False)
```

### Comparing `gramex-1.90.0/gramex/handlers/messagehandler.py` & `gramex-1.91.0/gramex/handlers/messagehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/mlhandler.py` & `gramex-1.91.0/gramex/handlers/mlhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/modelhandler.py` & `gramex-1.91.0/gramex/handlers/modelhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/openapiconfig.yaml` & `gramex-1.91.0/gramex/handlers/openapiconfig.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/openapihandler.py` & `gramex-1.91.0/gramex/handlers/openapihandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/pptxhandler.py` & `gramex-1.91.0/gramex/handlers/pptxhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/proxyhandler.py` & `gramex-1.91.0/gramex/handlers/proxyhandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,83 @@
 import tornado.web
 import tornado.gen
 from urllib.parse import urlsplit, urlunsplit, parse_qs, urlencode
 from tornado.httputil import HTTPHeaders
 from tornado.httpclient import AsyncHTTPClient, HTTPRequest
+from typing import Callable
 from gramex.transforms import build_transform
 from gramex.config import app_log
 from gramex.http import MOVED_PERMANENTLY, FOUND
 from .basehandler import BaseWebSocketHandler, BaseHandler
 from gramex.handlers import WebSocketHandler
 
 
 class ProxyHandler(BaseHandler, BaseWebSocketHandler):
-    '''
-    Passes the request to another HTTP REST API endpoint and returns its
-    response. This is useful when:
-
-    - exposing another website but via Gramex authentication (e.g. R-Shiny apps)
-    - a server-side REST API must be accessed via the browser (e.g. Twitter)
-    - passing requests to an API that requires authentication (e.g. Google)
-    - the request or response needs to be transformed (e.g. add sentiment)
-    - caching is required on the API (e.g. cache for 10 min)
-
-    :arg string url: URL endpoint to forward to. If the pattern ends with
-        ``(.*)``, that part is added to this url.
-    :arg dict request_headers: HTTP headers to be passed to the url.
-        - ``"*": true`` forwards all HTTP headers from the request as-is.
-        - A value of ``true`` forwards this header from the request as-is.
-        - Any string value is formatted with ``handler`` as a variable.
-    :arg dict default: Default URL query parameters
-    :arg dict headers: HTTP headers to set on the response
-    :arg function prepare: A function that accepts any of ``handler`` and ``request``
-        (a tornado.httpclient.HTTPRequest) and modifies the ``request`` in-place
-    :arg function modify: A function that accepts any of ``handler``, ``request``
-        and ``response`` (tornado.httpclient.HTTPResponse) and modifies the
-        ``response`` in-place
-    :arg int connect_timeout: Timeout for initial connection in seconds (default: 20)
-    :arg int request_timeout: Timeout for entire request in seconds (default: 20)
+    @classmethod
+    def setup(
+        cls,
+        url: str,
+        request_headers: dict = {},
+        default: dict = {},
+        prepare: Callable = None,
+        modify: Callable = None,
+        headers: dict = {},
+        connect_timeout: int = 20,
+        request_timeout: int = 20,
+        **kwargs,
+    ):
+        '''
+        Passes the request to another HTTP REST API endpoint and returns its
+        response. This is useful when:
+
+        - exposing another website but via Gramex authentication (e.g. R-Shiny apps)
+        - a server-side REST API must be accessed via the browser (e.g. Twitter)
+        - passing requests to an API that requires authentication (e.g. Google)
+        - the request or response needs to be transformed (e.g. add sentiment)
+        - caching is required on the API (e.g. cache for 10 min)
+
+        Parameters:
+
+            url: URL endpoint to forward to. If the pattern ends with
+                `(.*)`, that part is added to this url.
+            request_headers: HTTP headers to be passed to the url.
+                - `"*": true` forwards all HTTP headers from the request as-is.
+                - A value of `true` forwards this header from the request as-is.
+                - Any string value is formatted with `handler` as a variable.
+            default: Default URL query parameters
+            headers: HTTP headers to set on the response
+            prepare: A function that accepts any of `handler` and `request`
+                (a tornado.httpclient.HTTPRequest) and modifies the `request` in-place
+            modify: A function that accepts any of `handler`, `request`
+                and `response` (tornado.httpclient.HTTPResponse) and modifies the
+                `response` in-place
+            connect_timeout: Timeout for initial connection in seconds (default: 20)
+            request_timeout: Timeout for entire request in seconds (default: 20)
+
+        The response has the same HTTP headers and body as the proxied request, but:
 
-    Example YAML configuration::
+        - Connection and Transfer-Encoding headers are ignored
+        - `X-Proxy-Url:` header has the final URL that responded (after redirects)
 
+        These headers can be over-ridden by the `headers:` section.
+
+        ```yaml
         pattern: /gmail/(.*)
         handler: ProxyHandler
         kwargs:
             url: https://www.googleapis.com/gmail/v1/
             request_headers:
                 "*": true           # Pass on all HTTP headers
                 Cookie: true        # Pass on the Cookie HTTP header
                 # Over-ride the Authorization header
                 Authorization: 'Bearer {handler.session[google_access_token]}'
             default:
                 alt: json
-
-    The response has the same HTTP headers and body as the proxied request, but:
-
-    - Connection and Transfer-Encoding headers are ignored
-    - ``X-Proxy-Url:`` header has the final URL that responded (after redirects)
-
-    These headers can be over-ridden by the ``headers:`` section.
-    '''
-
-    @classmethod
-    def setup(
-        cls,
-        url,
-        request_headers={},
-        default={},
-        prepare=None,
-        modify=None,
-        headers={},
-        connect_timeout=20,
-        request_timeout=20,
-        **kwargs,
-    ):
+        ```
+        '''
         super(ProxyHandler, cls).setup(**kwargs)
         WebSocketHandler._setup(cls, **kwargs)
         cls.url, cls.request_headers, cls.default = url, request_headers, default
         cls.headers = headers
         cls.connect_timeout, cls.request_timeout = connect_timeout, request_timeout
         cls.info = {}
         for key, fn in (('prepare', prepare), ('modify', modify)):
```

### Comparing `gramex-1.90.0/gramex/handlers/queryhandler.template.html` & `gramex-1.91.0/gramex/handlers/queryhandler.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/handlers/socialhandler.py` & `gramex-1.91.0/gramex/handlers/socialhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,35 +125,37 @@
         if token is None:  # Ensure token is present
             raise HTTPError(BAD_REQUEST, f'token {key} missing')
         return token
 
 
 class TwitterRESTHandler(SocialHandler, TwitterMixin):
     '''
-    Proxy for the Twitter 1.1 REST API via these ``kwargs``::
+    Proxy for the Twitter 1.1 REST API via these `kwargs`:
 
-        pattern: /twitter/(.*)
-        handler: TwitterRESTHandler
-        kwargs:
-            key: your-consumer-key
-            secret: your-consumer-secret
-            access_key: your-access-key         # Optional -- picked up from session
-            access_secret: your-access-token    # Optional -- picked up from session
-            methods: [get, post]                # HTTP methods to use for the API
-            path: /search/tweets.json           # Freeze Twitter API request
+    ```yaml
+    pattern: /twitter/(.*)
+    handler: TwitterRESTHandler
+    kwargs:
+        key: your-consumer-key
+        secret: your-consumer-secret
+        access_key: your-access-key         # Optional -- picked up from session
+        access_secret: your-access-token    # Optional -- picked up from session
+        methods: [get, post]                # HTTP methods to use for the API
+        path: /search/tweets.json           # Freeze Twitter API request
+    ```
 
-    Now ``POST /twitter/search/tweets.json?q=gramener`` returns the same response
-    as the Twitter REST API ``/search/tweets.json``.
+    Now `POST /twitter/search/tweets.json?q=gramener` returns the same response
+    as the Twitter REST API `/search/tweets.json`.
 
-    If you only want to expose a specific API, specify a ``path:``. It overrides
+    If you only want to expose a specific API, specify a `path:`. It overrides
     the URL path. The query parameters will still work.
 
-    By default, ``methods`` is POST, and GET logs the user in, storing the access
-    token in the session for future use. But you can specify the ``access_...``
-    values and set ``methods`` to ``[get, post]`` to use both GET and POST
+    By default, `methods` is POST, and GET logs the user in, storing the access
+    token in the session for future use. But you can specify the `access_...`
+    values and set `methods` to `[get, post]` to use both GET and POST
     requests to proxy the API.
     '''
 
     @staticmethod
     def get_from_token(info, key, val):
         return info.get('access_token', {}).get(key.replace('access_', ''), val)
 
@@ -204,40 +206,40 @@
 
     def _oauth_consumer_token(self):
         return {'key': self.kwargs['key'], 'secret': self.kwargs['secret']}
 
 
 class FacebookGraphHandler(SocialHandler, FacebookGraphMixin):
     '''
-    Proxy for the Facebook Graph API via these ``kwargs``::
+    Proxy for the Facebook Graph API via these `kwargs`:
 
-        pattern: /facebook/(.*)
-        handler: FacebookGraphHandler
-        kwargs:
-            key: your-consumer-key
-            secret: your-consumer-secret
-            access_token: your-access-token     # Optional -- picked up from session
-            methods: [get, post]                # HTTP methods to use for the API
-            scope: user_posts,user_photos       # Permissions requested for the user
-            path: /me/feed                      # Freeze Facebook Graph API request
-
-    Now ``POST /facebook/me`` returns the same response as the Facebook Graph API
-    ``/me``. To request specific access rights, specify the ``scope`` based on
-    `permissions`_ required by the `Graph API`_.
+    ```yaml
+    pattern: /facebook/(.*)
+    handler: FacebookGraphHandler
+    kwargs:
+        key: your-consumer-key
+        secret: your-consumer-secret
+        access_token: your-access-token     # Optional -- picked up from session
+        methods: [get, post]                # HTTP methods to use for the API
+        scope: user_posts,user_photos       # Permissions requested for the user
+        path: /me/feed                      # Freeze Facebook Graph API request
+    ```
+
+    Now `POST /facebook/me` returns the same response as the Facebook Graph API
+    `/me`. To request specific access rights, specify the `scope` based on
+    [permissions](https://developers.facebook.com/docs/facebook-login/permissions) required by the
+    [Graph API](https://developers.facebook.com/docs/graph-api/reference).
 
-    If you only want to expose a specific API, specify a ``path:``. It overrides
+    If you only want to expose a specific API, specify a `path:`. It overrides
     the URL path. The query parameters will still work.
 
-    By default, ``methods`` is POST, and GET logs the user in, storing the access
-    token in the session for future use. But you can specify the ``access_token``
-    values and set ``methods`` to ``[get, post]`` to use both GET and POST
+    By default, `methods` is POST, and GET logs the user in, storing the access
+    token in the session for future use. But you can specify the `access_token`
+    values and set `methods` to `[get, post]` to use both GET and POST
     requests to proxy the API.
-
-    .. _permissions: https://developers.facebook.com/docs/facebook-login/permissions
-    .. _Graph API: https://developers.facebook.com/docs/graph-api/reference
     '''
 
     @classmethod
     def setup(cls, **kwargs):
         super(FacebookGraphHandler, cls).setup(**kwargs)
         cls.setup_social('user.facebook', **kwargs)
```

### Comparing `gramex-1.90.0/gramex/handlers/uploadhandler.py` & `gramex-1.91.0/gramex/handlers/uploadhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,24 +156,26 @@
                         stat['success'] = True
                 status.append(stat)
         return status
 
 
 class UploadHandler(BaseHandler):
     '''
-    UploadHandler lets users upload files. Here's a typical configuration::
+    UploadHandler lets users upload files. Here's a typical configuration:
 
+    ```yaml
         path: /$GRAMEXDATA/apps/appname/    # Save files here
         keys: [upload, file]                # <input name=""> can be upload / file
         store:
             type: sqlite                    # Store metadata in a SQLite store
             path: ...                       #   ... at the specified path
         redirect:                           # After uploading the file,
             query: next                     #   ... redirect to ?next=
             url: /$YAMLURL/                 #   ... else to this directory
+    ```
     '''
 
     @classmethod
     def setup(cls, path, keys=None, if_exists='unique', transform=None, methods=[], **kwargs):
         super(UploadHandler, cls).setup(**kwargs)
         cls.if_exists = if_exists
         # FileUpload uses the store= from **kwargs and ignores the rest
```

### Comparing `gramex-1.90.0/gramex/handlers/websockethandler.py` & `gramex-1.91.0/gramex/handlers/websockethandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/http.py` & `gramex-1.91.0/gramex/http.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/install.py` & `gramex-1.91.0/gramex/install.py`

 * *Files 0% similar despite different names*

```diff
@@ -588,15 +588,15 @@
                 if yamlpaths[key] in yaml_value.split('|'):
                     used.add(gramex_code['codepath'])
     gramex_complexity = gramexsize.set_index('codepath')['complexity'][list(used)].sum()
 
     # Calculate JS complexity
     # B602:subprocess_popen_with_shell_equals_true and
     # B607:start_process_with_partial_path are safe to skip since this is a Gramex internal cmd
-    output = check_output(['npx', '@gramex/escomplexity'], cwd=project_path, shell=True)  # nosec
+    output = check_output('npx --yes @gramex/escomplexity', cwd=project_path, shell=True)  # nosec
     es_complexity = int(output.decode('utf-8').split('\n')[-2].strip())
     return pd.DataFrame(
         {
             'py': [py_complexity],
             'js': [es_complexity],
             'gramex': [gramex_complexity],
         }
@@ -879,15 +879,15 @@
     with user_conf_file.open(mode='w', encoding='utf-8') as handle:
         yaml.safe_dump(user_config, handle, indent=4, default_flow_style=False)
 
 
 def get_app_config(appname, kwargs):
     '''
     Get the stored configuration for appname, and override it with kwargs.
-    ``.target`` defaults to $GRAMEXDATA/apps/<appname>.
+    `.target` defaults to $GRAMEXDATA/apps/<appname>.
     '''
     apps_config['cmd'] = {appname: kwargs}
     app_config = AttrDict((+apps_config).get(appname, {}))
     app_config.setdefault('target', str(app_dir / app_config.get('target', appname)))
     app_config.target = os.path.abspath(app_config.target)
     return app_config
```

### Comparing `gramex-1.90.0/gramex/license.py` & `gramex-1.91.0/gramex/license.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/migrate.py` & `gramex-1.91.0/gramex/migrate.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/ml.py` & `gramex-1.91.0/gramex/ml.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 from gramex.config import locate, app_log, merge, variables
 
 # Expose joblob.load via gramex.ml
 load = joblib.load
 
 
 class Classifier:
-    '''
-    :arg data DataFrame: data to train / re-train the model with
-    :arg model_class str: model class to use (default: ``sklearn.naive_bayes.BernoulliNB``)
-    :arg model_kwargs dict: kwargs to pass to model class constructor (defaults: ``{}``)
-    :arg output str: output column name (default: last column in training data)
-    :arg input list: input column names (default: all columns except ``output``)
-    :arg labels list: list of possible output values (default: unique ``output`` in training)
-    '''
-
     def __init__(self, **kwargs):
+        '''
+        Parameters:
+
+            data DataFrame: data to train / re-train the model with
+            model_class str: model class to use (default: `sklearn.naive_bayes.BernoulliNB`)
+            model_kwargs dict: kwargs to pass to model class constructor (defaults: `{}`)
+            output str: output column name (default: last column in training data)
+            input list: input column names (default: all columns except `output`)
+            labels list: list of possible output values (default: unique `output` in training)
+        '''
+
         vars(self).update(kwargs)
         self.model_class = kwargs.get('model_class', 'sklearn.naive_bayes.BernoulliNB')
         self.trained = False  # Boolean Flag
 
     def __str__(self):
         return repr(vars(self))
 
@@ -39,22 +41,24 @@
             for k, v in params.items()
             if k in model_keys
         }
         if model_params:
             self.trained = params.get('trained', False)
         vars(self).update(model_params)
 
-    def train(self, data):
+    def train(self, data: pd.DataFrame):
         '''
-        :arg data DataFrame: data to train / re-train the model with
-        :arg model_class str: model class to use (default: ``sklearn.naive_bayes.BernoulliNB``)
-        :arg model_kwargs dict: kwargs to pass to model class constructor (defaults: ``{}``)
-        :arg output str: output column name (default: last column in training data)
-        :arg input list: input column names (default: all columns except ``output``)
-        :arg labels list: list of possible output values (default: unique ``output`` in training)
+        Parameters:
+
+            data DataFrame: data to train / re-train the model with
+            model_class str: model class to use (default: `sklearn.naive_bayes.BernoulliNB`)
+            model_kwargs dict: kwargs to pass to model class constructor (defaults: `{}`)
+            output str: output column name (default: last column in training data)
+            input list: input column names (default: all columns except `output`)
+            labels list: list of possible output values (default: unique `output` in training)
 
         Notes:
         - If model has already been trained, extend the model. Else create it
         '''
         self.output = vars(self).get('output', data.columns[-1])
         self.input = vars(self).get('input', list(data.columns[:-1]))
         self.model_kwargs = vars(self).get('model_kwargs', {})
@@ -127,31 +131,33 @@
     if os.path.isdir(os.path.join(r_home, 'bin')):
         return r_home
     app_log.error('Anaconda R not installed')
     return None
 
 
 def r(
-    code=None,
-    path=None,
-    rel=True,
-    conda=True,
-    convert=True,
-    repo='https://cran.r-project.org/',
+    code: str = None,
+    path: str = None,
+    rel: bool = True,
+    conda: bool = True,
+    convert: bool = True,
+    repo: str = 'https://cran.r-project.org/',
     **kwargs,
 ):
     '''
     Runs the R script and returns the result.
 
-    :arg str code: R code to execute.
-    :arg str path: R script path. Cannot be used if code is specified
-    :arg bool rel: True treats path as relative to the caller function's file
-    :arg bool conda: True overrides R_HOME to use the Conda R
-    :arg bool convert: True converts R objects to Pandas and vice versa
-    :arg str repo: CRAN repo URL
+    Parameters:
+
+        code: R code to execute.
+        path: R script path. Cannot be used if code is specified
+        rel: True treats path as relative to the caller function's file
+        conda: True overrides R_HOME to use the Conda R
+        convert: True converts R objects to Pandas and vice versa
+        repo: CRAN repo URL
 
     All other keyword arguments as passed as parameters
     '''
     # Use Conda R if possible
     if conda:
         r_home = _conda_r_home()
         if r_home:
@@ -194,32 +200,42 @@
         result = result[0]
     else:
         result = r(code)
 
     return result
 
 
-def groupmeans(data, groups, numbers, cutoff=0.01, quantile=0.95, minsize=None, weight=None):
+def groupmeans(
+    data: pd.DataFrame,
+    groups: list,
+    numbers: list,
+    cutoff: float = 0.01,
+    quantile: float = 0.95,
+    minsize: int = None,
+    weight: str = None,
+):
     '''
     **DEPRECATED**. Use TopCause() instead.
 
     Yields the significant differences in average between every pair of
     groups and numbers.
 
-    :arg DataFrame data: pandas.DataFrame to analyze
-    :arg list groups: category column names to group data by
-    :arg list numbers: numeric column names in to summarize data by
-    :arg float cutoff: ignore anything with prob > cutoff.
-        cutoff=None ignores significance checks, speeding it up a LOT.
-    :arg float quantile: number that represents target improvement. Defaults to .95.
-        The ``diff`` returned is the % impact of everyone moving to the 95th
-        percentile
-    :arg int minsize: each group should contain at least minsize values.
-        If minsize=None, automatically set the minimum size to
-        1% of the dataset, or 10, whichever is larger.
+    Parameters:
+
+        data: pandas.DataFrame to analyze
+        groups: category column names to group data by
+        numbers: numeric column names in to summarize data by
+        cutoff: ignore anything with prob > cutoff.
+            cutoff=None ignores significance checks, speeding it up a LOT.
+        float quantile: number that represents target improvement. Defaults to .95.
+            The `diff` returned is the % impact of everyone moving to the 95th
+            percentile
+        int minsize: each group should contain at least minsize values.
+            If minsize=None, automatically set the minimum size to
+            1% of the dataset, or 10, whichever is larger.
     '''
     from scipy.stats.mstats import ttest_ind
 
     if minsize is None:
         minsize = max(len(data.index) // 100, 10)
 
     if weight is None:
@@ -303,47 +319,58 @@
 
 translate_api = {'google': _google_translate}
 # Prevent translate cache from being accessed concurrently across threads.
 # TODO: avoid threads and use Tornado ioloop/gen instead.
 _translate_cache_lock = threading.Lock()
 
 
-def translate(*q, **kwargs):
+def translate(
+    *q: str,
+    source: str = None,
+    target: str = None,
+    key: str = None,
+    cache: dict = None,
+    api: str = 'google',
+    **kwargs,
+):
     '''
-    Translate strings using the Google Translate API. Example::
-
-        translate('Hello', 'World', source='en', target='de', key='...')
-
-    returns a DataFrame::
-
-        source  target  q       t
-        en      de      Hello   ...
-        en      de      World   ...
-
-    The results can be cached via a ``cache={...}`` that has parameters for
-    :py:func:`gramex.data.filter`. Example::
-
-        translate('Hello', key='...', cache={'url': 'translate.xlsx'})
+    Translate strings using the Google Translate API.
 
-    :arg str q: one or more strings to translate
-    :arg str source: 2-letter source language (e.g. en, fr, es, hi, cn, etc).
-    :arg str target: 2-letter target language (e.g. en, fr, es, hi, cn, etc).
-    :arg str key: Google Translate API key
-    :arg dict cache: kwargs for :py:func:`gramex.data.filter`. Has keys such as
-        url (required), table (for databases), sheet_name (for Excel), etc.
+    ```python
+    translate('Hello', 'World', source='en', target='de', key='...')
+    ```
+
+    returns a DataFrame
+
+    ```text
+    source  target  q       t
+    en      de      Hello   ...
+    en      de      World   ...
+    ```
+
+    The results can be cached via a `cache={...}` that has parameters for
+    [gramex.data.filter]. Example:
+
+    ```python
+    translate('Hello', key='...', cache={'url': 'translate.xlsx'})
+    ```
+
+    Parameters:
+
+        q: one or more strings to translate
+        source: 2-letter source language (e.g. en, fr, es, hi, cn, etc).
+        target: 2-letter target language (e.g. en, fr, es, hi, cn, etc).
+        key: Google Translate API key
+        cache: kwargs for [gramex.data.filter]. Has keys such as
+            url (required), table (for databases), sheet_name (for Excel), etc.
 
     Reference: https://cloud.google.com/translate/docs/apis
     '''
     import gramex.data
 
-    source = kwargs.pop('source', None)
-    target = kwargs.pop('target', None)
-    key = kwargs.pop('key', None)
-    cache = kwargs.pop('cache', None)
-    api = kwargs.pop('api', 'google')
     if cache is not None and not isinstance(cache, dict):
         raise ValueError('cache= must be a FormHandler dict config, not %r' % cache)
 
     # Store data in cache with fixed columns: source, target, q, t
     result = pd.DataFrame(columns=['source', 'target', 'q', 't'])
     if not q:
         return result
```

### Comparing `gramex-1.90.0/gramex/ml_api.py` & `gramex-1.91.0/gramex/ml_api.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/pptgen/__init__.py` & `gramex-1.91.0/gramex/pptgen/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,30 +27,29 @@
     unit testing of run_commands.
     '''
     run_commands(sys.argv[1:], pptgen)
 
 
 def run_commands(commands, callback):
     '''
-    For example::
-
-        run_commands(['a.yaml', 'b.yaml', '--x=1'], method)
+    Examples:
+        >>> run_commands(['a.yaml', 'b.yaml', '--x=1'], method)
 
     will do the following:
 
     - Load a.yaml into config
         - Set config['a'] = 1
         - Change to directory where a.yaml is
         - Call method(config)
     - Load b.yaml into config
         - Set config['a'] = 1
         - Change to directory where b.yaml is
         - Call method(config)
 
-    Command line arguments are passed as ``commands``.
+    Command line arguments are passed as `commands`.
     Callback is a function that is called for each config file.
     '''
     args = parse_command_line(commands)
     original_path = os.getcwd()
     for config_file in args.pop('_'):
         config = gramex.cache.open(config_file, 'config')
         config = merge(old=config, new=args, mode='overwrite')
@@ -204,17 +203,17 @@
     else:
         prs.save(target)
 
 
 def change_shapes(collection, change, data, handler, **kwargs):
     '''
     Apply changes to a collection of shapes in the context of data.
-    ``collection`` is a slide.shapes or group shapes.
-    ``change`` is typically a dict of <shape-name>: commands.
-    ``data`` is a dictionary passed to the template engine.
+    `collection` is a slide.shapes or group shapes.
+    `change` is typically a dict of <shape-name>: commands.
+    `data` is a dictionary passed to the template engine.
     '''
     prs = kwargs.get('prs')
     new_slide = kwargs.get('new_slide')
     copy_slide = kwargs.get('copy_slide', False)
     source_slide = kwargs.get('source_slide')
 
     dest = prs.slides.add_slide(new_slide) if copy_slide else None
```

### Comparing `gramex-1.90.0/gramex/pptgen/color.py` & `gramex-1.91.0/gramex/pptgen/color.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 A color and gradient management system.
 
 *Do not pick colors yourself*. A lot of research has gone into color
 palettes. Specifically, for:
 
 Numeric data
-    use `ColorBrewer <http://colorbrewer2.org/>`_ themes
+    use [ColorBrewer](http://colorbrewer2.org/) themes
 
 Non-numeric data
-    use `ColorBrewer <http://colorbrewer2.org/>`_
-    or `Microsoft Office themes`_
+    use [ColorBrewer](http://colorbrewer2.org/)
+    or Microsoft Office themes
 
 Page design
-    use `kuler.adobe.com <https://kuler.adobe.com/#create/fromanimage>`_
+    use [kuler.adobe.com](https://kuler.adobe.com/#create/fromanimage)
     *from an image* (not directly).
 
 
 Microsoft office themes
 -----------------------
 
 The following color palettes based on Microsoft Office are available:
@@ -57,14 +57,15 @@
 import re
 import json
 import operator
 import colorsys
 import warnings
 import numpy as np
 from io import open
+from typing import Union
 
 
 BASE_0 = 0
 BASE_1 = 1
 BASE_2 = 2
 BASE_3 = 3
 BASE_4 = 4
@@ -122,61 +123,57 @@
     def __repr__(self):
         return '_MSO' + repr(self.values)
 
 
 def _rgb(color):
     """
     .. deprecated:: 0.1
-        Use :func:`rgba` instead
+        Use `rgba` instead
     """
     warnings.warn('Use color.rgba instead of color._rgb', FutureWarning, stacklevel=2)
     return (int(color[-6:-4], BASE_16), int(color[-4:-2], BASE_16), int(color[-2:], BASE_16))
 
 
-def gradient(value, grad, opacity=1, sort=True):
-    """
-    Converts a number or list ``x`` into a color using a gradient.
-
-
-    :arg number value: int, float, list, numpy array or any iterable.
-        If an iterable is passed, a list of colors is returned.
-    :arg list grad: tuple/list of ``(value, color)`` tuples
-        For example, ``((0, 'red'), (.5, 'yellow'), (1, 'green'))``.
-        Values will be sorted automatically
-    :arg float opacity: optional alpha to be added to the returned color
-    :arg bool sort: optional. If ``grad`` is already sorted, set ``sort=False``
+def gradient(
+    value: Union[int, float, list, np.array],
+    grad: Union[list, tuple],
+    opacity: float = 1,
+    sort: bool = True,
+):
+    """
+    Converts a number or list `x` into a color using a gradient.
+
+    Parameters:
+        value: int, float, list, numpy array or any iterable.
+            If an iterable is passed, a list of colors is returned.
+        grad: tuple/list of `(value, color)` tuples
+            For example, `((0, 'red'), (.5, 'yellow'), (1, 'green'))`.
+            Values will be sorted automatically
+        opacity: optional alpha to be added to the returned color
+        sort: optional. If `grad` is already sorted, set `sort=False`
 
     These gradients are available:
 
-    **divergent gradients** : on a ``[-1, 1]`` scale
-        multi-color
-            ``RdGy``, ``RdYlGn``, ``Spectral``
-        ... also print-friendly and color-blind safe
-            ``BrBG``, ``PiYG``, ``PRGn``, ``RdBu``, ``RdYlBu``
-        ... and also photocopyable
-            ``PuOr``
-    **sequential gradients** : on a ``[0, 1]`` scale
-        one-color
-            ``Reds``, ``Blues``, ``Greys``, ``Greens``, ``Oranges``,
-            ``Purples``, ``Browns``, ``Yellows``
-        two-color
-            ``BuGn``, ``BuPu``, ``GnBu``, ``OrRd``, ``PuBu``, ``PuRd``,
-            ``RdPu``, ``YlGn``
-        three-color
-            ``YlGnBu``, ``YlOrBr``, ``YlOrRd``, ``PuBuGn``
+    - **divergent gradients** : on a `[-1, 1]` scale
+        - Multi-color: `RdGy`, `RdYlGn`, `Spectral`
+        - Plus print-friendly and color-blind safe: `BrBG`, `PiYG`, `PRGn`, `RdBu`, `RdYlBu`
+        - Plus photocopyable: `PuOr`
+    - **sequential gradients** : on a `[0, 1]` scale
+        - one-color: `Reds`, `Blues`, `Greys`, `Greens`, `Oranges`, `Purples`, `Browns`, `Yellows`
+        - two-color: `BuGn`, `BuPu`, `GnBu`, `OrRd`, `PuBu`, `PuRd`, `RdPu`, `YlGn`
+        - three-color: `YlGnBu`, `YlOrBr`, `YlOrRd`, `PuBuGn`
 
     The following are also available, but do not use them.
 
-    - ``RYG`` maps ``[0, 1]`` to Red-Yellow-Green
-    - ``RWG`` maps ``[0, 1]`` to Red-White-Green
-    - ``RYG_1`` maps ``[-1, -1]`` to Red-Yellow-Green
-    - ``RWG_1`` maps ``[-1, -1]`` to Red-White-Green
-
-    Examples::
+    - `RYG` maps `[0, 1]` to Red-Yellow-Green
+    - `RWG` maps `[0, 1]` to Red-White-Green
+    - `RYG_1` maps `[-1, -1]` to Red-Yellow-Green
+    - `RWG_1` maps `[-1, -1]` to Red-White-Green
 
+    Examples:
         # Get a value that is 40% blue and 60% white, use:
         >>> gradient(0.4, ((0, 'blue'), (1, 'white')))
         '#66f'
 
         # A list (or any iterable) input returns a list of colors
         >>> gradient([0.2, 0.6, 0.8], ((0, 'blue'), (1, 'white')))
         ['#33f', '#99f', '#ccf']
@@ -242,98 +239,97 @@
     "#bcbd22",
     "#dbdb8d",
     "#17becf",
     "#9edae5",
 ]
 
 
-def distinct(count):
+def distinct(count: int):
     """
-    Generates a list of ``count`` distinct colors, for up to 20 colors.
+    Generates a list of `count` distinct colors, for up to 20 colors.
 
-    :arg int count: number of colors to return
-
-    Examples::
+    Parameters:
+        count: number of colors to return
 
+    Examples:
         >>> distinct(4)
         ['#1f77b4', '#ff7f0e', '#2ca02c', '#d62728']
 
     Notes:
 
     - Colour conversion between RGB and HCL are available on
-      `color.py <http://2sn.org/python/color.py>`_ and
-      `python-colormath <http://python-colormath.readthedocs.org/>`_
+      [color.py](http://2sn.org/python/color.py) and
+      [python-colormath](http://python-colormath.readthedocs.org/)
     - People seem to struggle with about
-      `26 colours
-      <http://eleanormaclure.files.wordpress.com/2011/03/colour-coding.pdf>`_
+      [26 colours](http://eleanormaclure.files.wordpress.com/2011/03/colour-coding.pdf)
       so this may be an upper bound
     - A good starting point for resources is on
-      `stackoverflow <http://stackoverflow.com/q/470690/100904>`_ and the
-      `graphic design <http://graphicdesign.stackexchange.com/q/3682>`_
+      [stackoverflow](http://stackoverflow.com/q/470690/100904) and the
+      [graphic design](http://graphicdesign.stackexchange.com/q/3682)
       stackexchange
     - More palettes are available from
-      `Kenneth Kelly (22) <http://www.iscc.org/pdf/PC54_1724_001.pdf>`_ and
-      `ggplot2 <http://learnr.wordpress.com/2009/04/15/ggplot2/>`_
-    - See also: http://epub.wu.ac.at/1692/1/document.pdf
+      [Kenneth Kelly (22)](http://www.iscc.org/pdf/PC54_1724_001.pdf>) and
+      [ggplot2](http://learnr.wordpress.com/2009/04/15/ggplot2/)
+    - See also: <http://epub.wu.ac.at/1692/1/document.pdf>
     """
     tens_count = 10
     twenty_count = 20
     _distinct = 2
     if count <= tens_count:
         return [_DISTINCTS[_distinct * i] for i in range(count)]
     elif count <= twenty_count:
         return _DISTINCTS[:count]
     else:
         return _DISTINCTS[:]
 
 
-def contrast(color, white='#ffffff', black='#000000'):
+def contrast(color: str, white: str = '#ffffff', black: str = '#000000'):
     """
     Returns the colour (white or black) that contrasts best with a given
     color.
 
-    :arg color color: color string recognied by :func:`rgba`.
-        If this color is dark, returns white. Else, black
-    :arg color white: color string, optional.
-        Replace this with any light colour you want to use instead of white
-    :arg color black: color string, optional.
-        Replace this with any dark colour you want to use instead of black
-
-    Examples::
+    Parameters:
+        color: color string recognied by `rgba`.
+            If this color is dark, returns white. Else, black
+        white: color string, optional.
+            Replace this with any light colour you want to use instead of white
+        black: color string, optional.
+            Replace this with any dark colour you want to use instead of black
 
+    Examples:
         >>> contrast('blue')
         '#fff'
         >>> contrast('lime')
         '#000'
 
-    Note: `Decolorize <http://www.eyemaginary.com/Rendering/TurnColorsGray.pdf>`_
+    Note: [Decolorize](http://www.eyemaginary.com/Rendering/TurnColorsGray.pdf)
     algorithm used. Appears to be the most preferred
-    (`ref <http://dcgi.felk.cvut.cz/home/cadikm/color_to_gray_evaluation/>`_).
+    ([ref](http://dcgi.felk.cvut.cz/home/cadikm/color_to_gray_evaluation/)).
     """
     idx = 3
     red, green, blue = rgba(color)[:idx]
     red_opac = 0.299
     blue_opac = 0.114
     green_opac = 0.582
     cut_off = 0.5
 
     luminosity = red_opac * red + green_opac * green + blue_opac * blue
     return black if luminosity > cut_off else white
 
 
-def brighten(color, percent):
+def brighten(color: str, percent: float):
     """
-    Brighten or darken a color by percentage. If ``percent`` is positive,
+    Brighten or darken a color by percentage. If `percent` is positive,
     brighten the color. Else darken the color.
 
-    :arg str color: color string recognied by :func:`rgba`
-    :arg float percent: -1 indicates black, +1 indicates white. Rest are interpolated.
-
-    Examples::
+    Parameters:
+        color: color string recognied by `rgba`
+        percent: -1 indicates black, +1 indicates white. Rest are interpolated.
 
+    Examples:
         >>> brighten('lime', -1)    # 100% darker, i.e. black
         '#000'
         >>> brighten('lime', -0.5)  # 50% darker
         '#007f00'
         >>> brighten('lime', 0)     # Returns the color as-is
         '#0f0'
         >>> brighten('lime', 0.5)   # 50% brighter
@@ -347,79 +343,77 @@
     _mid = 0
     _max = +1
     black = '#0000000'
     white = '#ffffff'
     return gradient(percent, ((_min, black), (_mid, color), (_max, white)))
 
 
-def msrgb(value, grad=None):
+def msrgb(value: str, grad: tuple = None):
     """
     Returns the Microsoft
-    `RGB color <http://msdn.microsoft.com/en-in/library/dd355244.aspx>`_
+    [RGB color](http://msdn.microsoft.com/en-in/library/dd355244.aspx)
     corresponding to a given a color. This is used for Microsoft office
     output (e.g. Excel, PowerPoint, etc.)
 
-    :arg color value: color or int/float. If ``grad`` is not specified, this
-        should be a color that will get converted into a Microsoft RGB value. If
-        ``grad`` is specified, this should be a number. It will be converted into
-        a color using the gradient, and then into a Microsoft RGB value.
-    :arg tuple grad: tuple/list of ``(value, color)`` tuples For example, ``((0,
-        'red'), (.5, 'yellow'), (1, 'green'))``. This is passed as an input to
-        :func:`gradient`
-
-    Examples::
+    Parameters:
+        value: color or int/float. If `grad` is not specified, this
+            should be a color that will get converted into a Microsoft RGB value. If
+            `grad` is specified, this should be a number. It will be converted into
+            a color using the gradient, and then into a Microsoft RGB value.
+        grad: tuple/list of `(value, color)` tuples For example, `((0,
+            'red'), (.5, 'yellow'), (1, 'green'))`. This is passed as an input to
+            `gradient`
 
+    Examples:
         >>> msrgb('#fff')
         16777215
         >>> msrgb('red')
         255
         >>> msrgb(0.5, RYG) # == msrgb(gradient(0.5, RYG))
         65535
     """
     idx = 3
     red, green, blue = rgba(gradient(value, grad) if grad else value)[:idx]
     return int((blue * BASE_255 * BASE_256 + green * BASE_255) * BASE_256 + red * BASE_255)
 
 
-def msrgbt(value, grad=None):
+def msrgbt(value: str, grad=None):
     """
-    Returns the Microsoft RGB value (same as :func:`msrgbt`) and transparency
+    Returns the Microsoft RGB value (same as `msrgbt`) and transparency
     as a tuple.
 
-    For example::
-
-        color, transparency = msrgbt('rgba(255, 0, 0, .5)')
-        shp.Fill.ForeColor.RGB, shp.Fill.Transparency = color, transparency
-
-    See :func:`msrgbt`. The parameters are identical.
+    Examples:
+        >> color, transparency = msrgbt('rgba(255, 0, 0, .5)')
+        >> shp.Fill.ForeColor.RGB, shp.Fill.Transparency = color, transparency
 
-    Examples::
+    See `msrgbt`. The parameters are identical.
 
+    Examples:
         >>> msrgbt('rgba(255,0,0,.5)')
         (255, 0.5)
         >>> msrgbt('red')
         (255, 0.0)
     """
     _alpha = 1
     red, green, blue, alpha = rgba(gradient(value, grad) if grad else value)
     alpha = _alpha - alpha
     col = (blue * BASE_255 * BASE_256 + green * BASE_255) * BASE_256 + red * BASE_255
     return int(col), alpha
 
 
-def rgba(color):
+def rgba(color: str):
     """
     Returns red, green, blue and alpha values (as a 0-1 float) of a color.
 
-    :arg color color: a string representing the color.
-        Most color formats defined in
-        `CSS3 <http://dev.w3.org/csswg/css3-color/>`_ are allowed.
-
-    Examples::
+    Parameters:
+        color: a string representing the color.
+            Most color formats defined in
+            [CSS3](http://dev.w3.org/csswg/css3-color/) are allowed.
 
+    Examples:
         >>> rgba('#f00')
         (1.0, 0.0, 0.0, 1.0)
         >>> rgba('#f003')
         (1.0, 0.0, 0.0, 0.2)
         >>> rgba('#ff0000')
         (1.0, 0.0, 0.0, 1.0)
         >>> rgba('#ff000033')
@@ -512,25 +506,25 @@
         raise ValueError(f'{color}: invalid color')
 
     return tuple(
         float(BASE_0) if val < BASE_0 else float(BASE_1) if val > BASE_1 else val for val in result
     )
 
 
-def hsla(color):
+def hsla(color: str):
     """
     Returns hue, saturation, luminosity and alpha values (as a 0-1 float) for
     a color.
 
-    :arg color color: a string representing the color.
-        Most color formats defined in
-        `CSS3 <http://dev.w3.org/csswg/css3-color/>`_ are allowed.
-
-    Examples::
+    Parameters:
+        color: a string representing the color.
+            Most color formats defined in
+            [CSS3](http://dev.w3.org/csswg/css3-color/) are allowed.
 
+    Examples:
         >>> hsla('#f00')
         (0.0, 1.0, 1.0, 1.0)
         >>> hsla('#f003')
         (0.0, 1.0, 1.0, 0.2)
         >>> hsla('#ff0000')
         (0.0, 1.0, 1.0, 1.0)
         >>> hsla('#ff000033')
@@ -546,27 +540,26 @@
         >>> hsla('hsla(0,1,1,.2)')
         (0.0, 1.0, 1.0, 0.2)
     """
     result = rgba(color)
     return colorsys.rgb_to_hsv(result[BASE_0], result[BASE_1], result[BASE_2]) + (result[BASE_3],)
 
 
-def name(red, green, blue, alpha=1):
+def name(red: float, green: float, blue: float, alpha: float = 1):
     """
     Returns a short color string
 
-    :arg float red: red color value (0-1)
-    :arg float green: green color value (0-1)
-    :arg float blue: blue color value (0-1)
-    :arg float alpha: float, optional transparency value between 0-1.
-        ``alpha=1`` produces color strings like ``#abc``
-        Lower values produce ``rgba(...)```.
-
-    Examples::
+    Parameters:
+        red: red color value (0-1)
+        green: green color value (0-1)
+        blue: blue color value (0-1)
+        alpha: float, optional transparency value between 0-1. `alpha=1` produces color strings
+            like `#abc`. Lower values produce `rgba(...)`.
 
+    Examples:
         >>> name(1, 0, 0)       # Short color versions preferred
         '#f00'
         >>> name(1, 0, 0, .2)   # Alpha creates rgba() with 2 decimals
         'rgba(255,0,0,0.20)'
         >>> name(.5, .25, .75)  # Multiply by 255 and round to nearest
         '#8040bf'
         >>> name(-1, 2, 0)      # Values are truncated to 0-1
```

### Comparing `gramex-1.90.0/gramex/pptgen/colors.json` & `gramex-1.91.0/gramex/pptgen/colors.json`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/pptgen/commands.py` & `gramex-1.91.0/gramex/pptgen/commands.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/pptgen/fonts.json` & `gramex-1.91.0/gramex/pptgen/fonts.json`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/pptgen/fontwidth.py` & `gramex-1.91.0/gramex/pptgen/fontwidth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/pptgen/utils.py` & `gramex-1.91.0/gramex/pptgen/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 from pptx.enum.base import EnumValue
 from pptx.enum.text import PP_ALIGN, MSO_ANCHOR
 from gramex.transforms import build_transform
 
 
 def is_slide_allowed(change, slide, number):
     '''
-    Given a change like one of the below::
+    Given a change like one of the below:
 
-        slide-number: 1
-        slide-number: [1, 2, 3]
-        slide-title: 'company'
-        slide-title: ['company', 'industry']
+    ```yaml
+    slide-number: 1
+    slide-number: [1, 2, 3]
+    slide-title: 'company'
+    slide-title: ['company', 'industry']
+    ```
 
     ... return True if:
 
-    1. ``number`` matches a slide-number
-    2. ``slide`` title matches a slide-title regex (case-insensitive)
+    1. `number` matches a slide-number
+    2. `slide` title matches a slide-title regex (case-insensitive)
 
     If none of these are specified, return True.
     '''
     match = True
     # Restrict to specific slide number(s), if specified
     if 'slide-number' in change:
         slide_number = change['slide-number']
@@ -201,50 +203,50 @@
 def scale(series, lo=None, hi=None):
     '''
     Returns the values linearly scaled from 0 - 1.
 
     The lowest value becomes 0, the highest value becomes 1, and all other
     values are proportionally multiplied and have a range between 0 and 1.
 
-    :arg Series series: Data to scale. Pandas Series, numpy array, list or iterable
-    :arg float lo: Value that becomes 0. Values lower than ``lo`` in ``series``
-        will be mapped to negative numbers.
-    :arg float hi: Value that becomes 1. Values higher than ``hi`` in ``series``
-        will be mapped to numbers greater than 1.
+    Parameters:
 
-    Examples::
+        series: Data to scale. Pandas Series, numpy array, list or iterable
+        lo: Value that becomes 0. Values lower than `lo` in `series`
+            will be mapped to negative numbers.
+        hi: Value that becomes 1. Values higher than `hi` in `series`
+            will be mapped to numbers greater than 1.
 
+    Examples:
         >>> stats.scale([1, 2, 3, 4, 5])
         ... array([ 0.  ,  0.25,  0.5 ,  0.75,  1.  ])
-
         >>> stats.scale([1, 2, 3, 4, 5], lo=2, hi=4)
         ... array([-0.5,  0. ,  0.5,  1. ,  1.5])
     '''
     series = np.array(series, dtype=float)
     lo = np.nanmin(series) if lo is None or np.isnan(lo) else lo
     hi = np.nanmax(series) if hi is None or np.isnan(hi) else hi
     return (series - lo) / ((hi - lo) or np.nan)
 
 
 def decimals(series):
     '''
-    Given a ``series`` of numbers, returns the number of decimals
+    Given a `series` of numbers, returns the number of decimals
     *just enough* to differentiate between most numbers.
 
-    :arg Series series: Pandas Series, numpy array, list or iterable.
-        Data to find the required decimal precision for
-    :return: The minimum number of decimals required to differentiate between
-        most numbers
-
-    Examples::
-
-        stats.decimals([1, 2, 3])       # 0: All integers. No decimals needed
-        stats.decimals([.1, .2, .3])    # 1: 1 decimal is required
-        stats.decimals([.01, .02, .3])  # 2: 2 decimals are required
-        stats.decimals(.01)             # 2: Only 1 no. of 2 decimal precision
+    Parameters:
+        series: Pandas Series, numpy array, list or iterable. Data to find decimal precision for
+
+    Returns:
+        The minimum number of decimals required to differentiate between most numbers
+
+    Examples:
+        >>> stats.decimals([1, 2, 3])       # 0: All integers. No decimals needed
+        >>> stats.decimals([.1, .2, .3])    # 1: 1 decimal is required
+        >>> stats.decimals([.01, .02, .3])  # 2: 2 decimals are required
+        >>> stats.decimals(.01)             # 2: Only 1 no. of 2 decimal precision
 
     Note: This function first calculates the smallest difference between any pair
     of numbers (ignoring floating-point errors). It then finds the log10 of that
     difference, which represents the minimum decimals required to differentiate
     between these numbers.
     '''
     series = np.ma.masked_array(series, mask=np.isnan(series)).astype(float)
@@ -461,26 +463,23 @@
 def squarified(x, y, w, h, data):
     '''
     Draw a squarified treemap.
 
     See <http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.36.6685>
     Returns a numpy array with (x, y, w, h) for each item in data.
 
-    Examples::
-
-        # The result is a 2x2 numpy array::
+    Examples:
         >>> squarified(x=0, y=0, w=6, h=4, data=[6, 6, 4, 3, 2, 2, 1])
         array([[ 0.        ,  0.        ,  3.        ,  2.        ],
                [ 0.        ,  2.        ,  3.        ,  2.        ],
                [ 3.        ,  0.        ,  1.71428571,  2.33333333],
                [ 4.71428571,  0.        ,  1.28571429,  2.33333333],
                [ 3.        ,  2.33333333,  1.2       ,  1.66666667],
                [ 4.2       ,  2.33333333,  1.2       ,  1.66666667],
                [ 5.4       ,  2.33333333,  0.6       ,  1.66666667]])
-
         >>> squarified(x=0, y=0, w=1, h=1, data=[np.nan, 0, 1, 2])
         array([[ 0.        ,  0.        ,  0.        ,  0.        ],
                [ 0.        ,  0.        ,  0.        ,  0.        ],
                [ 0.        ,  0.        ,  0.33333333,  1.        ],
                [ 0.33333333,  0.        ,  0.66666667,  1.        ]])
     '''
     w, h = float(w), float(h)
```

### Comparing `gramex-1.90.0/gramex/pptgen2/__init__.py` & `gramex-1.91.0/gramex/pptgen2/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-pptgen2.pptgen() modifies a ``source`` PPTX using ``rules`` and ``data``.
+pptgen2.pptgen() modifies a `source` PPTX using `rules` and `data`.
 
-The main loop is in :py:func:`pptgen`, which calls other functions as required.
+The main loop is in [pptgen()][gramex.pptgen2.pptgen], which calls other functions as required.
 '''
 
 import copy
 import gramex
 import gramex.data
 import os
 import pandas as pd
@@ -34,27 +34,28 @@
     unit: str = 'Inches',
     mode: str = 'literal',
     handler=None,
     **config,
 ) -> pptx.presentation.Presentation:
     '''
     Process a configuration. This loads a Presentation from source, applies the
-    (optional) configuration changes and (optionally) saves it into target. Returns the modified
+    (optional) configuration changes and (optionally) saves it into target. Returns modified PPTX.
 
-    :arg PPTX source: string or pptx.Presentation object to transform
-    :arg list rules: list of rules to apply to the ``source`` PPTX. Each rule
-    :arg str target: optional path save file
-    :arg int/list only: slide number(s) to process. 1 is the first slide. [1, 3] is slides 1 & 3
-    :arg dict register: new commands to register via :py:func:`register_commands`.
-    :arg str unit: default length unit (Inches, Cm, Centipoints, etc)
-    :arg str mode: default expression mode. Values in Python are treated as 'literals'
-        (e.g. 'red' is the STRING red). But PPTXHandler passes the mode as `expr`. Values are
-        treated as expressions (e.g. 'red' is the VARIABLE red).
-    :arg handler: if PPTXHandler passes a handler, make it available to the commands as a variable
-    :return: target PPTX
+    Parameters:
+
+        source: string or pptx.Presentation object to transform
+        rules: list of rules to apply to the `source` PPTX. Each rule
+        target: optional path save file
+        only: slide number(s) to process. 1 is the first slide. [1, 3] is slides 1 & 3
+        register: new commands to register via [gramex.pptgen2.register_commands][]
+        unit: default length unit (Inches, Cm, Centipoints, etc)
+        mode: default expression mode. Values in Python are treated as 'literals'
+            (e.g. 'red' is the STRING red). But PPTXHandler passes the mode as `expr`. Values are
+            treated as expressions (e.g. 'red' is the VARIABLE red).
+        handler: if PPTXHandler passes a handler, make it available to the commands as a variable
     '''
     # TODO: source can be an expression. PPTXHandler may need to use multiple themes
     prs = source if isinstance(source, pptx.presentation.Presentation) else Presentation(source)
     # Load data with additional variables:
     #   prs: source presentation
     #   handler: if PPTXHandler passes a handler, allow commands to use it as a variable
     #   _expr_mode: Allows commands.expr() to evaluate specs as literals or expressions correctly
@@ -128,18 +129,20 @@
 }
 
 
 def apply_commands(rule: Dict[str, dict], shapes, data: dict):
     '''
     Apply commands in rule to change shapes using data.
 
-    :arg dict rule: a dict of shape names, and commands to apply on each.
-        e.g. ``{"Oval 1": {"fill": "red"}, "Oval 2": {"text": "OK"}}``
-    :arg Shapes shapes: a slide.shapes or group.shapes object on which the rule should be applied
-    :arg dict data: data context for the commands in the rule
+    Parameters:
+
+        rule: a dict of shape names, and commands to apply on each.
+            e.g. `{"Oval 1": {"fill": "red"}, "Oval 2": {"text": "OK"}}`
+        shapes: a slide.shapes or group.shapes object on which the rule should be applied
+        data: data context for the commands in the rule
     '''
     # Apply every rule to every pattern -- as long as the rule key matches the shape name
     for pattern, spec in rule.items():
         if pattern in rule_cmdlist:
             continue
         matched_shapes = [shape for shape in shapes if fnmatchcase(shape.name, pattern)]
         for shape in matched_shapes:
@@ -187,35 +190,38 @@
             app_log.warn(f'pptgen2: No shape matches pattern: {pattern}')
 
 
 def load_data(_conf, _default_key: str = None, **kwargs) -> dict:
     '''
     Loads datasets based on configuration and returns a dict of those datasets.
 
-    :arg dataset _conf: The dataset configuration
-    :arg str _default_key: Can be ``function``, ``url`` or ``None`` (default).
-        If specified, it converts string data configurations into ``{_default_key: _conf}``.
-    :return: A dict of datasets loaded based on the configuration.
-
-    ``_conf`` is processed as follows:
-
-    - String ``'data.xlsx'`` is loaded via :py:func:`gramex.cache.open` into ``{data: ...}`` if
-        ``_default_key == 'url'``
-    - String ``'data[0]'`` is evaluated via :py:func:`gramex.transforms.build_transform` into
-        ``{data: ...}``` if ``_default_key == 'function'``
-    - String ``anything``` raises an Exception if ``_default_key`` is None
-    - Dict ``{url: ...}`` is loaded with :py:func:`gramex.data.filter` into ``{data: ...}``
-    - Dict ``{function: ...}`` is evaluated via :py:func:`gramex.transforms.build_transform`
-        into ``{data: ...}``
-    - Dict ``{x: ..., y: ...}`` loads the respective datasets into ``x`` and ``y`` instead of
-        ``data``. Each dataset is processed using the above rules.
-    - Any other datatype passed is returned as is in ``{data: ...}``
+    Parameters:
+        _conf: The dataset configuration
+        _default_key: Can be `function`, `url` or `None` (default).
+            If specified, it converts string data configurations into `{_default_key: _conf}`.
+
+    Returns:
+        A dict of datasets loaded based on the configuration.
+
+    `_conf` is processed as follows:
+
+    - String `'data.xlsx'` is loaded via [gramex.cache.open] into `{data: ...}` if
+        `_default_key == 'url'`
+    - String `'data[0]'` is evaluated via [gramex.transforms.build_transform] into
+        `{data: ...}` if `_default_key == 'function'`
+    - String `anything` raises an Exception if `_default_key` is None
+    - Dict `{url: ...}` is loaded with [gramex.data.filter] into `{data: ...}`
+    - Dict `{function: ...}` is evaluated via [gramex.transforms.build_transform]
+        into `{data: ...}`
+    - Dict `{x: ..., y: ...}` loads the respective datasets into `x` and `y` instead of
+        `data`. Each dataset is processed using the above rules.
+    - Any other datatype passed is returned as is in `{data: ...}`
 
     Any keyword arguments passed are also added to the resulting dataset, but overwritten only if
-    ``_conf`` loaded a dataset that's not ``None``.
+    `_conf` loaded a dataset that's not `None`.
     '''
 
     def str2conf(data, key):
         '''Convert string configurations to {url: str} or {function:str} based on _default_key'''
         # If data is not a string, return data as-is
         if not isinstance(data, str):
             return data
@@ -253,33 +259,38 @@
     return kwargs
 
 
 def register_commands(register: Dict[str, str]) -> None:
     '''
     Register a new command to the command list.
 
-    :arg dict register: keys are the command name. Values are the Python expression to run to apply
-        the command. The expression can use 3 variables: ``shape`` (the Shape object to modify),
-        ``spec`` (the configuration passed to your command) and ``data``.
+    Parameters:
+
+        register: keys are the command name. Values are the Python expression to run to apply
+            the command. The expression can use 3 variables: `shape` (the Shape object to modify),
+            `spec` (the configuration passed to your command) and `data`.
     '''
     if not isinstance(register, dict):
         raise TypeError(f'register: must be a dict, not {type(register)}')
     for key, conf in register.items():
         commands.cmdlist[key] = build_transform(
             {'function': conf}, vars={'shape': None, 'spec': None, 'data': None}, iter=False
         )
 
 
 def pick_only_slides(prs: Presentation, only: Union[int, List[int]] = None) -> list:
     '''
-    Delete slides except those specified in ``only``.
+    Delete slides except those specified in `only`.
+
+    Parameters:
+        prs: presentation to delete slides from
+        only: slide number(s) to process. 1 is the first slide. [1, 3] is slides 1 & 3
 
-    :arg Presentation prs: presentation to delete slides from
-    :arg int/list only: slide number(s) to process. 1 is the first slide. [1, 3] is slides 1 & 3
-    :return: list of slides to process. These slides are also DELETED in the original prs
+    Returns:
+        list of slides to process. These slides are also DELETED in the original prs
     '''
     if only is None:
         return list(prs.slides)
     if isinstance(only, int):
         only = [only]
     if not isinstance(only, list):
         raise TypeError(f'pptgen(only=) takes slide number or list, not {type(only)}')
@@ -291,21 +302,24 @@
     return list(prs.slides)
 
 
 def slide_filter(slides, rule: dict, data: dict):
     '''
     Filter slides. Return iterable of (index, slide) for only those slides matching numbers/titles.
 
-    :arg Slides slides: a Slides object (e.g. ``prs.slides``) to select slides from
-    :arg dict rule: a dict that may have a ``slide-number`` or ``slide-title`` key to filter by.
-        These can be expressions. ``slide-number`` is the slide number(s) to filter. 1 is the first
-        slide. ``[1, 3]`` is slides 1 & 3. ``slide-title`` has the slide title pattern(s) to filter
-        e.g. ``*Match*`` matches all slides with "match" anywhere in the title (case-insensitive).
-    :arg dict data: data context for the rule
-    :return: an iterable that yields (index, slide)
+    Parameters:
+        slides: a Slides object (e.g. `prs.slides`) to select slides from
+        rule: a dict that may have a `slide-number` or `slide-title` key to filter by.
+            These can be expressions. `slide-number` is the slide number(s) to filter. 1 is the 1st
+            slide. `[1, 3]` is slides 1 & 3. `slide-title` has the slide title pattern(s) to filter
+            e.g. `*Match*` matches all slides with "match" anywhere in the title (case-insensitive)
+        data: data context for the rule
+
+    Returns:
+        an iterable that yields (index, slide)
     '''
     numbers = commands.expr(rule.get('slide-number', []), data)
     titles = commands.expr(rule.get('slide-title', []), data)
     # numbers is the SET of 1-indexed slide numbers this rule applies to
     numbers = set(numbers if isinstance(numbers, list) else [numbers])
     # titles is a LIST of title patterns - ANY of which the slide title must match
     titles = titles if isinstance(titles, list) else [titles]
@@ -315,23 +329,24 @@
             continue
         title = slide.shapes.title.text if slide.shapes.title else ''
         if titles and (not any(fnmatchcase(title.lower(), pattern.lower()) for pattern in titles)):
             continue
         yield index, slide
 
 
-def copy_slide(prs, source, target_index):
+def copy_slide(prs: Presentation, source, target_index: int):
     '''
-    Copy ``source`` slide from presentatation ``prs`` to appear at ``target_index``. python-pptx
+    Copy `source` slide from presentatation `prs` to appear at `target_index`. python-pptx
     does not have this feature, so we tweak XML directly. Does not copy slides with diagrams or
     charts yet.
 
-    :arg Presentation prs: presentation to copy the slide in
-    :arg Slide source: slide to copy
-    :arg target_index: location to copy into. 0 makes it the first slide
+    Parameters:
+        Presentation prs: presentation to copy the slide in
+        Slide source: slide to copy
+        target_index: location to copy into. 0 makes it the first slide
     '''
     # Append slide with source's layout. Then delete shapes to get a blank slide
     dest = prs.slides.add_slide(source.slide_layout)
     for shp in dest.shapes:
         shp.element.getparent().remove(shp.element)
     # Copy background
     if source.background.element.bg is not None:
@@ -370,19 +385,20 @@
 
 
 def transition(slide, spec: Union[str, dict], data: dict):
     '''
     Apply transition on slide based on spec. python-pptx does not have this feature, so we tweak
     XML directly.
 
-    :arg Slide slide: slide to apply the transition to
-    :arg dict/str spec: type of transition to apply. ``config.yaml`` lists transitions and options.
-        It can also be a dict specifying ``type`` (type of transition), ``duration`` (in seconds)
-        and ``advance`` (auto-advance after seconds)
-    :arg dict data: data context for the ``spec`` expression
+    Parameters:
+        slide: slide to apply the transition to
+        spec: type of transition to apply. `config.yaml` lists transitions and options.
+            It can also be a dict specifying `type` (type of transition), `duration` (in seconds)
+            and `advance` (auto-advance after seconds)
+        data: data context for the `spec` expression
     '''
     if spec is None:
         return
     # Convert spec into this format: {type: ..., advance: ..., duration: ...}
     if isinstance(spec, str):
         spec = {'type': spec}
     if not isinstance(spec, dict):
@@ -424,32 +440,35 @@
             trans = slide.element.find('mc:AlternateContent/mc:Choice/p:transition', _nsmap)
             if trans is not None:
                 trans.set(attr, f'{float(val) * 1000:.0f}')
 
 
 def iterate_on(spec, data: dict):
     '''
-    ``clone:`` and ``copy:`` iterate on data to return a (key, val) pair. This method performs the
+    `clone:` and `copy:` iterate on data to return a (key, val) pair. This method performs the
     iteration for different data types and returns (key, val) consistently.
 
-    :arg expr spec: an expression to iterate on. It can be a dict, tuple, list, pd.Index,
-        pd.DataFrame, or pd.DataFrameGroupBy
-    :arg dict data: data context for the ``spec`` expression
-    :return: an iterable that yields (key, val) tuples
+    Parameters:
+        spec: an expression to iterate on. It can be a dict, tuple, list, pd.Index,
+            pd.DataFrame, or pd.DataFrameGroupBy
+        data: data context for the `spec` expression
+
+    Returns:
+        an iterable that yields (key, val) tuples
     '''
     val = commands.expr(spec, data)
     # {x: 1} -> (x, 1)
     if isinstance(val, dict):
         return val.items()
     # [x, y] -> (0, x), (1, y)
     elif isinstance(val, (tuple, list, pd.Index)):
         return enumerate(val)
     # pd.Series({x: 1}) -> (x, 1)
     elif isinstance(val, pd.Series):
-        return val.iteritems()
+        return val.items()
     # pd.DataFrame([{x:1, y:2], {x:3, y:4}]) -> (0, {x: 1, y:2}), ...
     elif isinstance(val, pd.DataFrame):
         return val.iterrows()
     # df.groupby(key) -> (key1, group_df1), (key2, group_df2), ...
     elif isinstance(val, pd.core.groupby.generic.DataFrameGroupBy):
         return val
     else:
```

### Comparing `gramex-1.90.0/gramex/pptgen2/commands.py` & `gramex-1.91.0/gramex/pptgen2/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
-pptgen2.pptgen() modifies slides using commands (in ``__init__.py``). This file maps the commands
-and their functions in ``cmdlist``.
+pptgen2.pptgen() modifies slides using commands (in `__init__.py`). This file maps the commands
+and their functions in `cmdlist`.
 
-Each command accepts ``(shape, spec, data)`` and modifies shape based on spec(ification) and data.
+Each command accepts `(shape, spec, data)` and modifies shape based on spec(ification) and data.
 '''
 
 import copy
 import gramex.cache
 import io
 import matplotlib.cm
 import matplotlib.colors
@@ -134,22 +134,22 @@
 )
 
 
 def fill_color(fill: FillFormat, val: Union[str, tuple, list, None]) -> None:
     '''
     Set the FillFormat color to value specified as a:
 
-    - a named color, like ``black``
-    - a hex value, like ``#f80`` or ``#ff8800``
-    - an RGB value, like ``rgb(255, 255, 0)`` or ``rgb(1, 0.5, 0.1)``
-    - a tuple or list of RGB values, like ``(255, 255, 0)`` or ``[255, 255, 0]``
-    - a theme color, like ``ACCENT_1``, ``ACCENT_2``, ``BACKGROUND_1``, ``DARK_1``, ``LIGHT_2``
-    - a theme color with a brightness modifier, like ``ACCENT_1+40``, which is 40% brighter than
-      Accent 1, or ``ACCENT_2-20`` which is 20% darker than Accent 2
-    - ``'none'`` clears the color, i.e. makes it transparent
+    - a named color, like `black`
+    - a hex value, like `#f80` or `#ff8800`
+    - an RGB value, like `rgb(255, 255, 0)` or `rgb(1, 0.5, 0.1)`
+    - a tuple or list of RGB values, like `(255, 255, 0)` or `[255, 255, 0]`
+    - a theme color, like `ACCENT_1`, `ACCENT_2`, `BACKGROUND_1`, `DARK_1`, `LIGHT_2`
+    - a theme color with a brightness modifier, like `ACCENT_1+40`, which is 40% brighter than
+      Accent 1, or `ACCENT_2-20` which is 20% darker than Accent 2
+    - `'none'` clears the color, i.e. makes it transparent
     '''
     fill.solid()
     if val == 'none':
         fill.background()
     elif isinstance(val, (list, tuple)):
         val = val[:3]
         if any(isinstance(v, float) for v in val) and all(0 <= v <= 1 for v in val):
@@ -693,15 +693,15 @@
             or (expr_mode and 'value' in cmdspec)
             or (not expr_mode and 'expr' in cmdspec)
         ):
             cmdspec = {column: cmdspec for column in table_data.columns}
         # Apply commands that run on each cell
         if key in table_cell_commands:
             for i, (index, row) in enumerate(table_data.iterrows()):
-                for j, (column, val) in enumerate(row.iteritems()):
+                for j, (column, val) in enumerate(row.items()):
                     data['cell'] = AttrDict(
                         val=val,
                         column=column,
                         index=index,
                         row=row,
                         data=table_data,
                         pos=AttrDict(row=i, column=j),
@@ -752,21 +752,21 @@
         )
     else:
         chart_type = conf['chart-type'][chart_tag]
         # Create a new instance of CategoryChartData(), XYChartData() or BubbleChartData()
         new_chart_data = getattr(pptxchartdata, chart_type + 'ChartData')()
         new_chart_data.categories = chart_data.index
         if chart_type == 'Category':
-            for name, col in chart_data.iteritems():
+            for name, col in chart_data.items():
                 new_chart_data.add_series(name, col.values)
         # TODO: This messes up the resulting Excel sheet, and is not extensible. Rewrite via lxml
         elif chart_type == 'Xy':
-            for name, col in chart_data.iteritems():
+            for name, col in chart_data.items():
                 series = new_chart_data.add_series(name)
-                for index, v in col.iteritems():
+                for index, v in col.items():
                     series.add_data_point(index, v)
         shape.chart.replace_data(new_chart_data)
 
     data = dict(**data, chartdata=chart_data)
     for attrname, method in (
         ('fill', partial(set_color, 'format.fill')),
         ('stroke', partial(set_color, 'format.line.fill')),
```

### Comparing `gramex-1.90.0/gramex/pptgen2/config.yaml` & `gramex-1.91.0/gramex/pptgen2/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/pynode.py` & `gramex-1.91.0/gramex/pynode.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,25 +11,26 @@
 from gramex.cache import daemon
 from gramex.config import app_log
 
 _info = {}
 
 
 class Node:
-    '''
-    Usage::
-
-        node = Node(port=9966, node_path='/tmp/')
-        total = await node.js('return {"total": x + y}', x='a', y=10)['total']
-    '''
-
     _source = os.path.join(variables['GRAMEXAPPS'], 'pynode')
     _delay = 0.01
 
-    def __init__(self, port=9966, cwd=None, node_path=None, timeout=10):
+    def __init__(
+        self, port: int = 9966, cwd: str = None, node_path: str = None, timeout: int = 10
+    ):
+        '''
+        Example:
+
+            >>> node = Node(port=9966, node_path='/tmp/')
+            >>> total = await node.js('return {"total": x + y}', x='a', y=10)['total']
+        '''
         self.port = port
         # cwd is the directory where node runs. Defaults to $GRAMEXDATA/pynode/
         # node_modules is updated under this.
         self.cwd = os.path.join(variables['GRAMEXDATA'], 'pynode') if cwd is None else cwd
         if not os.path.exists(self.cwd):
             os.makedirs(self.cwd)
         # node_path is where the node executable is. Autodetect from PATH by default
```

### Comparing `gramex-1.90.0/gramex/scale.py` & `gramex-1.91.0/gramex/scale.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 _color_convert = {'rgba': lambda v: v}
 
 
 def color(domain, range, bin=False, to='hex', name='Gramex color'):
     '''
     Returns a function that scales a number in domain to a color in the range.
 
-    - ``color(domain=[0, 1], range=['white', 'blue'])``
+    - `color(domain=[0, 1], range=['white', 'blue'])`
       maps values between 0 to 1 smoothly from white to blue.
 
     Use multiple colors in a smooth gradient.
 
-    - ``color(domain=[-1, 0, 1], range=['red', 'yellow', 'green'])``
+    - `color(domain=[-1, 0, 1], range=['red', 'yellow', 'green'])`
       maps values between -1 to +1 smoothly from red to yellow to green
 
     Use multiple colors discretely by binning into buckets (called quantization).
 
-    - ``color(domain=[-1, 0, 1], range=['red', 'green'], bin=True)``
+    - `color(domain=[-1, 0, 1], range=['red', 'green'], bin=True)`
       maps (-1, 0) to red, and (0, 1) to green
     '''
     import numpy as np
     import matplotlib.colors as colors
     import matplotlib.cm as cm
 
     if bin:
```

### Comparing `gramex-1.90.0/gramex/secrets.py` & `gramex-1.91.0/gramex/secrets.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/servicenow.yaml` & `gramex-1.91.0/gramex/servicenow.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/services/__init__.py` & `gramex-1.91.0/gramex/services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Each key in `gramex.yaml` calls the corresponding function in this file. For example,
 
 ```yaml
 log:
     version: 1
 ```
 
-... calls [gramex.service.log()][gramex.services.log] as ``log({"version": 1})``.
+... calls [gramex.service.log()][gramex.services.log] as `log({"version": 1})`.
 If no such function exists, a warning is raised.
 '''
 import io
 import re
 import os
 import sys
 import json
@@ -901,22 +901,22 @@
 def _get_cache_key(conf, name):
     '''
     Parse the cache.key parameter. Return a function that takes the request and
     returns the cache key value.
 
     The cache key is a string or a list of strings. The strings can be:
 
-    - ``request.attr`` => ``request.attr`` can be any request attribute, as str
-    - ``header.key`` => ``request.headers[key]``
-    - ``cookies.key`` => ``request.cookies[key].value``
-    - ``args.key`` => ``handler.args[key]`` joined with a comma.
-    - ``user.key`` => ``handler.current_user[key]`` as str
+    - `request.attr` => `request.attr` can be any request attribute, as str
+    - `header.key` => `request.headers[key]`
+    - `cookies.key` => `request.cookies[key].value`
+    - `args.key` => `handler.args[key]` joined with a comma.
+    - `user.key` => `handler.current_user[key]` as str
 
     Invalid key strings are ignored with a warning. If all key strings are
-    invalid, the default cache.key of ``request.uri`` is used.
+    invalid, the default cache.key of `request.uri` is used.
     '''
     default_key = 'request.uri'
     keys = conf.get('key', default_key)
     if not isinstance(keys, list):
         keys = [keys]
     key_getters = []
     for key in keys:
@@ -957,43 +957,42 @@
     # B102:exec_used is safe since the code is constructed entirely in this function
     exec(method, context)  # nosec B102
     return context['cache_key']
 
 
 def _cache_generator(conf, name):
     '''
-    The ``url:`` section of ``gramex.yaml`` can specify a ``cache:`` section. For
-    example::
+    The `url:` section of `gramex.yaml` can specify a `cache:` section.
 
-        url:
-            home:
-                pattern: /
-                handler: ...
-                cache:
-                    key: request.uri
-                    store: memory
-                    expires:
-                        duration: 1 minute
+    ```yaml
+    url:
+        home:
+            pattern: /
+            handler: ...
+            cache:
+                key: request.uri
+                store: memory
+                expires:
+                    duration: 1 minute
+    ```
 
-    This function takes the ``cache`` section of the configuration and returns a
+    This function takes the `cache` section of the configuration and returns a
     "cache" function. This function accepts a RequestHandler and returns a
-    ``CacheFile`` instance.
+    `CacheFile` instance.
 
-    Here's a typical usage::
+    Example:
 
-        cache_method = _cache_generator(conf.cache)     # one-time initialisation
-        cache_file = cache_method(handler)              # used inside a hander
-
-    The cache_file instance exposes the following interface::
-
-        cache_file.get()        # returns None
-        cache_file.write('abc')
-        cache_file.write('def')
-        cache_file.close()
-        cache_file.get()        # returns 'abcdef'
+        >>> cache_method = _cache_generator(conf.cache)     # one-time initialisation
+        >>> cache_file = cache_method(handler)              # used inside a hander
+        >>> # The cache_file instance exposes the following interface
+        >>> cache_file.get()        # returns None
+        >>> cache_file.write('abc')
+        >>> cache_file.write('def')
+        >>> cache_file.close()
+        >>> cache_file.get()        # returns 'abcdef'
     '''
     # cache: can be True (to use default settings) or False (to disable cache)
     if conf is True:
         conf = {}
     elif conf is False:
         return None
```

### Comparing `gramex-1.90.0/gramex/services/emailer.py` & `gramex-1.91.0/gramex/services/emailer.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/services/rediscache.py` & `gramex-1.91.0/gramex/services/rediscache.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,36 +16,37 @@
         redis_kwargs = dict(part.split('=', 1) for part in parts)
     for key, val in kwargs.items():
         redis_kwargs.setdefault(key, val)
     return StrictRedis(host=host, port=port, db=db, **redis_kwargs)
 
 
 class RedisCache:
-    '''
-    LRU Cache that stores data in a Redis database. Typical usage::
+    def __init__(self, path: str = None, maxsize: int = None, *args, **kwargs):
+        '''
+        LRU Cache that stores data in a Redis database.
 
-        >>> store = RedisCache('localhost:6379:1:password=x:...', 500000) # host:port:db:params
-        >>> value = store.get(key)
-        >>> store.set(key, value, expire)
+        Example:
 
-    The path in the constructor contains parameters separated by colon (:):
+            >>> store = RedisCache('localhost:6379:1:password=x:...', 500000) # host:port:db:params
+            >>> value = store.get(key)
+            >>> store.set(key, value, expire)
 
-    - `host`: the Redis server location (default: localhost)
-    - `port`: the Redis server port (default: 6379)
-    - `db`: the Redis server DB number (default: 0)
-    - zero or more parameters passed to StrictRedis (e.g. password=abc)
+        The path in the constructor contains parameters separated by colon (:):
 
-    `maxsize` defines the maximum limit of cache. This will set maxmemory for the redis instance
-    and not specific to a db. If it's false-y (None, 0, etc.) no limit is set.
+        - `host`: the Redis server location (default: localhost)
+        - `port`: the Redis server port (default: 6379)
+        - `db`: the Redis server DB number (default: 0)
+        - zero or more parameters passed to StrictRedis (e.g. password=abc)
 
-    Both Keys and Values are stored as pickle dump.
-    This is an approximate LRU implementation. Read more here.(https://redis.io/topics/lru-cache)
-    '''
+        `maxsize` is the maximum limit of cache. This will set maxmemory for the redis instance
+        and not specific to a db. If it's false-y (None, 0, etc.) no limit is set.
 
-    def __init__(self, path=None, maxsize=None, *args, **kwargs):
+        Both Keys and Values are stored as pickle dump.
+        This is an approximate LRU implementation. [Read more](https://redis.io/topics/lru-cache)
+        '''
         self.store = get_redis(path, decode_responses=False)
         self.size = 0
         if maxsize:
             if self.currsize > maxsize:
                 self.flush()
             self.store.config_set('maxmemory', maxsize)
             self.store.config_set('maxmemory-policy', 'allkeys-lru')  # Approximate LRU cache
```

### Comparing `gramex-1.90.0/gramex/services/scheduler.py` & `gramex-1.91.0/gramex/services/scheduler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/services/sms.py` & `gramex-1.91.0/gramex/services/sms.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 from gramex.http import OK
 from gramex.config import app_log
 
 
 class Notifier:
     def send(self, to, subject, sender):
         '''
-        Send an SMS to the ``to`` mobile with ``subject`` as the contents. ``sender`` optional.
+        Send an SMS to the `to` mobile with `subject` as the contents. `sender` optional.
 
         Return API-specific response object.
         Raise Exception if API access fails. (This does not guarantee SMS delivery.)
         '''
         raise NotImplementedError()
 
     def status(self, result):
         '''
-        Returns the delivery status of the SMS. The ``result`` is the output from ``.send()``.
+        Returns the delivery status of the SMS. The `result` is the output from `.send()`.
         '''
         raise NotImplementedError()
 
 
 class AmazonSNS(Notifier):
     '''
-    Send messages via AmazonSNS::
+    Send messages via AmazonSNS.
 
+    Examples:
         >>> notifier = AmazonSNS(
         ...     aws_access_key_id='...',
         ...     aws_secret_access_key='...',
         ...     region_name='ap-southeast-1',
         ...     smstype='Transactional')
         >>> notifier.send(
         ...     to='+919741552552',
@@ -65,16 +66,17 @@
         )
         app_log.info(f'SMS sent. SNS MessageId: {result["MessageId"]}')
         return result
 
 
 class Exotel(Notifier):
     '''
-    Send messages via Exotel::
+    Send messages via Exotel.
 
+    Examples:
         >>> notifier = Exotel(
         ...     sid='...',
         ...     token='...',
         ...     key='...',
         ...     domain='...',
         ...     priority='high',
         ... )
```

### Comparing `gramex-1.90.0/gramex/services/ttlcache.py` & `gramex-1.91.0/gramex/services/ttlcache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/services/urlcache.py` & `gramex-1.91.0/gramex/services/urlcache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 The CacheFile object exposes a get, wrap and close interface to handlers.
 
-- ``.get()`` reads all data against the key
-- ``.wrap(handler)`` is used to wrap the ``.write()`` method to append into a
-  write queue, and the ``.on_finish()`` method to save the result.
+- `.get()` reads all data against the key
+- `.wrap(handler)` is used to wrap the `.write()` method to append into a
+  write queue, and the `.on_finish()` method to save the result.
 
 Each type of store has a separate CacheFile. (MemoryCacheFile, DiskCacheFile,
 etc.) The parent CacheFile implements the no-caching behaviour.
 
 See gramex.handlers.BaseHandler for examples on how to use these objects.
 '''
 # B403:import_public we only pickle Gramex internal objects
```

### Comparing `gramex-1.90.0/gramex/services/watcher.py` & `gramex-1.91.0/gramex/services/watcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 '''
-The file watch service uses `watchdog <https://pythonhosted.org/watchdog/>`_ to
+The file watch service uses [watchdog](https://pythonhosted.org/watchdog/) to
 monitor files, and run functions when the file changes.
 '''
 
 import os
 import atexit
 from fnmatch import fnmatch
 from orderedattrdict import AttrDict
+from typing import List, Dict, Callable
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 from gramex.config import app_log
 
 # Terminology:
 #   observer    - a single instance class that has all scheduler related behavior
 #   watch       - an instance that watches a single *folder*
@@ -38,46 +39,49 @@
 
     def dispatch(self, event):
         path = os.path.abspath(event.src_path)
         if any(fnmatch(path, pattern) for pattern in self.patterns):
             super(FileEventHandler, self).dispatch(event)
 
 
-def watch(name, paths, **events):
+def watch(name: str, paths: List[str], **events: Dict[str, Callable]):
     '''
     Watch one or more paths, and trigger an event function.
 
-    Example::
-
-        watch('test', ['test.txt'],
+    Examples:
+        >>> watch('test', ['test.txt'],
               on_modified: lambda event: logging.info('Modified test.txt'),
               on_created: lambda event: logging.info('Created test.txt'))
 
-    When ``test.txt`` is modified or created, it logs one of the above messages.
+    When `test.txt` is modified or created, it logs one of the above messages.
 
-    To replace the same handler with another, use the same ``name``::
+    To replace the same handler with another, use the same `name`.
 
-        watch('test', ['test.txt'],
+    Examples:
+        >>> watch('test', ['test.txt'],
               on_deleted: lambda event: logging.info('Deleted test.txt'))
 
-    Now, when ``test.txt`` is deleted, it logs a message. But when ``test.txt``
+    Now, when `test.txt` is deleted, it logs a message. But when `test.txt`
     is created or modified, no message is shown, since the old handler has been
     replaced.
 
-    To remove this watch, call ``unwatch('test')``.
+    To remove this watch, call `unwatch('test')`.
+
+    Parameters:
 
-    :arg string name: Unique name of the watch.  To replace an existing watch,
-        re-use the same name.
-    :arg list paths: List of relative or absolute paths to watch.  The paths
-        can be strings or ``pathlib.Path`` objects.
-    :arg function on_modified(event): Called when any path is modified.
-    :arg function on_created(event): Called when any path is created.
-    :arg function on_deleted(event): Called when any path is deleted.
-    :arg function on_moved(event): Called when any path is moved.
-    :arg function on_any_event(event): Called on any of the above events.
+        name: Unique name of the watch.  To replace an existing watch,
+            re-use the same name.
+        paths: List of relative or absolute paths to watch.  The paths
+            can be strings or `pathlib.Path` objects.
+        events: a map of event handlers, called with an `event` object. Keys can be:
+            - `on_modified`: path is modified.
+            - `on_created`: path is created.
+            - `on_deleted`: path is deleted.
+            - `on_moved`: path is moved.
+            - `on_any_event`: any of the above events.
     '''
     # Create a series of schedules and handlers
     unwatch(name)
 
     patterns = set()  # List of absolute path patterns
     folders = set()  # List of folders matching these paths
     for path in paths:
```

### Comparing `gramex-1.90.0/gramex/sm_api.py` & `gramex-1.91.0/gramex/sm_api.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/topcause.py` & `gramex-1.91.0/gramex/topcause.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/transformers.py` & `gramex-1.91.0/gramex/transformers.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/transforms/__init__.py` & `gramex-1.91.0/gramex/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/transforms/auth.py` & `gramex-1.91.0/gramex/transforms/auth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/transforms/template.py` & `gramex-1.91.0/gramex/transforms/template.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex/transforms/transforms.py` & `gramex-1.91.0/gramex/transforms/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -508,15 +508,14 @@
         return args[-1]
 
 
 def flattener(fields: dict, default: Any = None, filename: str = 'flatten'):
     '''Generates a function that flattens deep dictionaries.
 
     Examples:
-
         >>> flat = flattener({
         ...     'id': 'id',
         ...     'name': 'user.screen_name'
         ... })
         >>> flat({'id': 1, 'user': {'screen_name': 'name'}})
         ... {'id': 1, 'name': 'name'}
```

### Comparing `gramex-1.90.0/gramex/transforms/twitterstream.py` & `gramex-1.91.0/gramex/transforms/twitterstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,31 +17,32 @@
     INTERNAL_SERVER_ERROR,
     GATEWAY_TIMEOUT,
 )
 
 
 class TwitterStream:
     '''
-    Starts a Twitter Streaming client. Sample usage::
+    Starts a Twitter Streaming client.
 
+    Examples:
         >>> from gramex.transforms.twitterstream import TwitterStream
         >>> stream = TwitterStream(
         ...     track='modi,mms',
         ...     path='save-as-file.json',
         ...     key='...',
         ...     secret='...',
         ...     access_key='...',
         ...     access_secret='...',
         ...     flush=True)
 
-    This saves all tweets mentioning ``modi`` or ``mms`` in ``save-as-file.json``
+    This saves all tweets mentioning `modi` or `mms` in `save-as-file.json`
     with each line representing a tweet in JSN format.
 
-    If ``flush=True``, the file is flushed on every tweet. If ``flush=<number>``,
-    the file is flushed every ``<number>`` seconds. If ``flush=False`` (default),
+    If `flush=True`, the file is flushed on every tweet. If `flush=<number>`,
+    the file is flushed every `<number>` seconds. If `flush=False` (default),
     the file is flushed only when the file or app is closed.
 
     This function runs forever, so run it in a separate thread.
     '''
 
     def __init__(self, **kwargs):
         self.params = kwargs
@@ -221,22 +222,22 @@
         if self.stream is not None:
             self.stream.flush()
 
     def rotate(self):
         '''
         Create and rotate file streams.
 
-        The ``path`` format string determines the filename. For example,
-        ``tweets.{:%Y-%m-%d}.jsonl`` creates a filename based on the current
-        date, e.g. ``tweets.2016-12-31.jsonl``. When rotating, if the new
+        The `path` format string determines the filename. For example,
+        `tweets.{:%Y-%m-%d}.jsonl` creates a filename based on the current
+        date, e.g. `tweets.2016-12-31.jsonl`. When rotating, if the new
         filename is the same as the old, the file continues. If it's a different
         file, the old file is closed and the new file is created.
 
         The rotation frequency is based on the crontab entries in the config,
-        i.e. based on ``hours``, ``days``, ``weeks``, etc. It defaults to every
+        i.e. based on `hours`, `days`, `weeks`, etc. It defaults to every
         minute.
         '''
         # First, flush the stream to ensure that data is not lost.
         # Then set up new stream (if required, based on the filename)
         self.flush()
         path = self.path.format(datetime.datetime.utcnow())
         if path != self.stream_path:
```

### Comparing `gramex-1.90.0/gramex/winservice.py` & `gramex-1.91.0/gramex/winservice.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex.egg-info/PKG-INFO` & `gramex-1.91.0/gramex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramex
-Version: 1.90.0
+Version: 1.91.0
 Summary: Gramex: Low Code Data Solutions Platform
 Author-email: Anand S <s.anand@gramener.com>, Pratap Vardhan <pratapapvr@gmail.com>, Jaidev Deshpande <jaidev.deshpande@gramener.com>, Bhanu Kamapantula <talk2kish@gmail.com>, Radheya Kale <radheya.kale@gramener.com>, Karmanya Aggarwal <karmanyaaggarwal@gmail.com>, Sandeep Bhat <sandeep.bhat@gramener.com>, Shraddheya Shrivastava <shraddheya.shrivastava@gramener.com>, Sundeep Reddy Mallu <sundeep.mally@gramener.com>
 License: MIT
 Project-URL: Homepage, https://gramener.com/gramex/
 Project-URL: Documentation, https://gramener.com/gramex/guide/
 Project-URL: Repository, https://github.com/gramener/gramex
 Project-URL: Changelog, https://gramener.com/gramex/guide/release/
```

### Comparing `gramex-1.90.0/gramex.egg-info/SOURCES.txt` & `gramex-1.91.0/gramex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/gramex.egg-info/requires.txt` & `gramex-1.91.0/gramex.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 astor
+blinker
 cachetools>=3.0.0
 colorlog>=2.7.0
 cron-descriptor
 crontab>=0.21
 diskcache>=2.8.3
 h5py
 joblib
@@ -19,15 +20,14 @@
 psutil
 python-dateutil
 python-pptx<=0.6.19,>=0.6.6
 python-slugify
 pyyaml>=5.1
 redis>=2.10.0
 requests
-scikit-learn
 seaborn
 six
 sqlalchemy<2
 sqlitedict>=1.5.0
 tables
 tornado>=5.1.1
 typing_extensions
@@ -41,14 +41,15 @@
 [full]
 boto3
 datasets
 line_profiler
 pymysql
 scipy
 spacy
+scikit-learn
 statsmodels
 transformers
 xlrd
 
 [influxdb]
 influxdb_client[ciso]
 
@@ -75,15 +76,15 @@
 cssselect
 datasets
 elasticsearch7
 gramexenterprise
 mccabe
 nose
 pdfminer.six
-psycopg2>=2.7.1
+psycopg2-binary
 pymongo
 pymysql
 pytest
 scipy
 spacy
 statsmodels
 testfixtures
```

### Comparing `gramex-1.90.0/pyproject.toml` & `gramex-1.91.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gramex"
-version = "1.90.0"
+version = "1.91.0"
 description = "Gramex: Low Code Data Solutions Platform"
 # People with 2+ contributions on https://github.com/gramener/gramex/graphs/contributors
 authors = [
     {name = "Anand S", email = "s.anand@gramener.com"},
     {name = "Pratap Vardhan", email = "pratapapvr@gmail.com"},
     {name = "Jaidev Deshpande", email = "jaidev.deshpande@gramener.com"},
     {name = "Bhanu Kamapantula", email = "talk2kish@gmail.com"},
@@ -33,14 +33,15 @@
 ]
 requires-python = ">=3.7"
 readme = "README.md"
 dependencies = [
     # It's OK to specify minimum versions, i.e. >=.
     # But avoid <= or == without a strong reason. Makes it hard to mix with other libraries.
     "astor",  # for gramex.transforms.build_transform
+    "blinker",  # for MessageHandler
     "cachetools>=3.0.0",  # for services.cache for memory cache
     "colorlog>=2.7.0",  # for Coloured log files
     "cron-descriptor",  # for gramex.apps.admin2.gramexadmin admin/schedule to pretty-print
     "crontab>=0.21",  # for services.schedule to parse crontab entries
     "diskcache>=2.8.3",  # for urlcache.DiskCache
     "h5py",  # for MLHandler saves .h5 files. TODO: Migrate away from .h5
     "joblib",  # for gramex.ml
@@ -58,15 +59,14 @@
     "python-dateutil",  # for gramex.config.CustomJSONEncoder, gramex.data._convertor
     # See https://github.com/scanny/python-pptx/issues/754
     "python-pptx>=0.6.6,<=0.6.19",  # for pptgen2
     "python-slugify",  # for pre-defined slugs at gramex.config.slug
     "pyyaml>=5.1",  # for parsing YAML files for config
     "redis>=2.10.0",  # for RedisStore
     "requests",  # for all HTTP requests
-    "scikit-learn",  # for MLHandler, gramex.ml. TODO: version >=0.23.2,<1.0
     "seaborn",  # OPT: gramex.data.download()
     "six",  # for gramex.yaml backward compatibility
     "sqlalchemy<2",  # for gramex.data.filter()
     "sqlitedict>=1.5.0",  # for SQLiteStore
     "tables",  # for HDF5 reading / writing. TODO: Where do we need this?
     "tornado>=5.1.1",  # for Web server
     "typing_extensions",  # for future-proof typing
@@ -98,14 +98,15 @@
 full = [
     "boto3",  # for gramex.services.sns.AmazonSNS
     "datasets",  # for gramex.transformers
     "line_profiler",  # for gramex.debug.lineprofile
     "pymysql",  # for MySQL connections
     "scipy",  # for gramex.topcause
     "spacy",  # for gramex.transformers
+    "scikit-learn",  # for MLHandler, gramex.ml. TODO: version >=0.23.2,<1.0
     "statsmodels",  # for gramex.ml_api
     "transformers",  # for gramex.transformers
     "xlrd",  # for gramex.cache.open .XLS support (not .xlsx)
     # "conda",  # not required except for rpy2 or reporting conda version
     # "rpy2",  # deprecated
 ]
 influxdb = ["influxdb_client[ciso]"]
@@ -140,15 +141,15 @@
     "cssselect",  # for tests.check_css() in test_admin, test_auth, test_alerts
     "datasets",  # for gramex.transformers
     "elasticsearch7",  # for gramexlog: features
     "gramexenterprise",  # for auth testing
     "mccabe",  # for pkg/usage/pycomplexity.py
     "nose",  # for all test cases
     "pdfminer.six",  # for test_capturehandler
-    "psycopg2 >= 2.7.1",  # for PostgreSQL tests
+    "psycopg2-binary",  # for PostgreSQL tests
     "pymongo",  # for MongoDB tests
     "pymysql",  # for MySQL tests
     "pytest",  # for newer test cases
     "scipy",  # for gramex.topcause
     "spacy",  # for gramex.transformers
     "statsmodels",  # for gramex.ml_api
     "testfixtures",  # For logcapture
```

### Comparing `gramex-1.90.0/setup.cfg` & `gramex-1.91.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_admin.py` & `gramex-1.91.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_alerts.py` & `gramex-1.91.0/tests/test_alerts.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_args.py` & `gramex-1.91.0/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_auth.py` & `gramex-1.91.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_cache.py` & `gramex-1.91.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_capturehandler.py` & `gramex-1.91.0/tests/test_capturehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_comichandler.py` & `gramex-1.91.0/tests/test_comichandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_drivehandler.py` & `gramex-1.91.0/tests/test_drivehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_filehandler.py` & `gramex-1.91.0/tests/test_filehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_filterhandler.py` & `gramex-1.91.0/tests/test_filterhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_formhandler.py` & `gramex-1.91.0/tests/test_formhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_functionhandler.py` & `gramex-1.91.0/tests/test_functionhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_gramexlog.py` & `gramex-1.91.0/tests/test_gramexlog.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_handlers.py` & `gramex-1.91.0/tests/test_handlers.py`

 * *Files 11% similar despite different names*

```diff
@@ -242,135 +242,187 @@
         # ratelimit: requires app.ratelimit
         with assert_raises(ValueError) as cm:
             setup({}, None)
         eq_(cm.exception.args[0], "url:test.ratelimit: no app.ratelimit defined")
 
         # ratelimit.keys required
         with assert_raises(ValueError) as cm:
-            setup({}, {})
+            setup({}, gramex.conf.app.ratelimit)
         eq_(cm.exception.args[0], 'url:test.ratelimit.keys: missing')
 
         # ratelimit.limit required
         with assert_raises(ValueError) as cm:
-            setup({'keys': 'daily'}, {})
+            setup({'keys': 'daily'}, gramex.conf.app.ratelimit)
         eq_(cm.exception.args[0], 'url:test.ratelimit.limit: missing')
 
         # ratelimit.keys strings MUST be predefined
         with assert_raises(ValueError) as cm:
-            setup({'keys': 'daily', 'limit': 5}, {})
-        eq_(cm.exception.args[0], 'url:test.ratelimit.keys: daily is unknown')
+            setup({'keys': 'secondly', 'limit': 5}, gramex.conf.app.ratelimit)
+        eq_(cm.exception.args[0], 'url:test.ratelimit.keys: secondly is unknown')
 
         # ratelimit.keys strings MUST be str/list
         with assert_raises(ValueError) as cm:
-            setup({'keys': 0, 'limit': 5}, {})
+            setup({'keys': 0, 'limit': 5}, gramex.conf.app.ratelimit)
         eq_(cm.exception.args[0], 'url:test.ratelimit.keys: needs dict list, not 0')
 
         # ratelimit.keys: invalid function compilation directly raises exceptions, e.g. SyntaxError
         with assert_raises(SyntaxError):
-            setup({'keys': [{'function': ';$@'}], 'limit': 5}, {})
+            setup({'keys': [{'function': ';$@'}], 'limit': 5}, gramex.conf.app.ratelimit)
 
         # ratelimit.keys dicts need a function:
         with assert_raises(ValueError) as cm:
-            setup({'keys': {'x': 0}, 'limit': 5}, {})
+            setup({'keys': {'x': 0}, 'limit': 5}, gramex.conf.app.ratelimit)
         eq_(cm.exception.args[0], "url:test.ratelimit.keys: {'x': 0} has no function:")
         with assert_raises(ValueError) as cm:
-            setup({'keys': [{'x': 0}], 'limit': 5}, {})
+            setup({'keys': [{'x': 0}], 'limit': 5}, gramex.conf.app.ratelimit)
         eq_(cm.exception.args[0], "url:test.ratelimit.keys: {'x': 0} has no function:")
 
         # ratelimit.keys can be a predefined key string
         for key in ('hourly', 'daily', 'weekly', 'monthly', 'yearly', 'user'):
-            ok_(setup({'keys': key, 'limit': 5}, gramex.conf.app.ratelimit)._ratelimit.store)
+            ok_(setup({'keys': key, 'limit': 5}, gramex.conf.app.ratelimit)._ratelimit[0].store)
 
         # ratelimit.keys can be a dict with a function. Defines a single key
         ok_(setup({'keys': {'function': '0'}, 'limit': 5}, gramex.conf.app.ratelimit))
 
         # ratelimit.keys can be a comma-separated string
         cls = setup({'keys': 'daily, user', 'limit': 5}, gramex.conf.app.ratelimit)
-        eq_(len(cls._ratelimit.key_fn), 2)
+        eq_(len(cls._ratelimit[0].key_fn), 2)
 
         # ratelimit.keys can be an array of strings
         cls = setup({'keys': ['daily', 'user'], 'limit': 5}, gramex.conf.app.ratelimit)
-        eq_(len(cls._ratelimit.key_fn), 2)
+        eq_(len(cls._ratelimit[0].key_fn), 2)
 
         # ratelimit.limit must be a number
         with assert_raises(ValueError) as cm:
             setup({'keys': 'daily', 'limit': 'x'}, gramex.conf.app.ratelimit)
         eq_(cm.exception.args[0], "url:test.ratelimit.limit: needs {'function': number}, not x")
 
         # ratelimit.limit can be a function
         cls = setup({'keys': 'user', 'limit': {'function': '5'}}, gramex.conf.app.ratelimit)
-        eq_(cls._ratelimit.limit_fn(None), 5)
+        eq_(cls._ratelimit[0].limit_fn(None), 5)
 
         # EVERY handler supports rate-limiting via `ratelimit:`
         for base in (
             gramex.handlers.FunctionHandler,
             gramex.handlers.FormHandler,
             gramex.handlers.FileHandler,
             gramex.handlers.DriveHandler,
         ):
             cls = setup({'keys': 'daily, user', 'limit': 5}, gramex.conf.app.ratelimit, base)
             ok_(issubclass(cls, base))
 
         # ratelimit.keys return the expected values
         all_keys = ['hourly', 'daily', 'weekly', 'monthly', 'yearly', 'user']
         cls = setup({'keys': all_keys, 'limit': 5}, gramex.conf.app.ratelimit)
-        key_fn = dict(zip(all_keys, cls._ratelimit.key_fn))
+        key_fn = dict(zip(all_keys, cls._ratelimit[0].key_fn))
         handler = AttrDict(current_user=AttrDict(id='a@b'))
         eq_(key_fn['hourly']['function'](handler), pd.Timestamp.utcnow().strftime('%Y-%m-%d %H'))
         eq_(key_fn['daily']['function'](handler), pd.Timestamp.utcnow().strftime('%Y-%m-%d'))
         eq_(key_fn['weekly']['function'](handler), pd.Timestamp.utcnow().strftime('%Y %U'))
         eq_(key_fn['monthly']['function'](handler), pd.Timestamp.utcnow().strftime('%Y-%m'))
         eq_(key_fn['yearly']['function'](handler), pd.Timestamp.utcnow().strftime('%Y'))
         eq_(key_fn['user']['function'](handler), 'a@b')
 
-    def test_ratelimit(self):
-        def check(url, user, limit, remaining, code=OK):
-            # If user= is specified, send an {'id': user} object via headers
-            headers = {}
-            if user is not None:
-                cookie_secret = gramex.service.app.settings['cookie_secret']
-                sign = create_signed_value(cookie_secret, 'user', json.dumps({'id': user}))
-                headers['X-Gramex-User'] = sign
-
-            # Check the status code and X-Ratelimit-* headers
-            r = self.check(url, code=code, request_headers=headers)
-            if code in (OK, TOO_MANY_REQUESTS):
-                eq_(r.headers['X-Ratelimit-Limit'], str(limit))
-                eq_(r.headers['X-Ratelimit-Remaining'], str(remaining))
-                # Check expiry time to plus/minus 2 seconds.
-                # NOTE: This test may fail if running exactly at UTC midnight
-                eod = pd.Timestamp.utcnow().normalize() + pd.Timedelta(days=1)
-                expiry = int((eod - pd.Timestamp.utcnow()).total_seconds())
-                ok_(expiry - 2 <= int(r.headers['X-Ratelimit-Reset']) <= expiry + 2)
-                # Retry-After header should be sent only for
-                if code == TOO_MANY_REQUESTS:
-                    eq_(r.headers['Retry-After'], r.headers['X-Ratelimit-Reset'])
-                else:
-                    ok_('Retry-After' not in r.headers)
+        # Multiple pools are supported
+        cls = setup(
+            [{'keys': 'daily, user', 'limit': 5}, {'keys': 'daily', 'limit': 10}],
+            gramex.conf.app.ratelimit,
+        )
+        key_fn0, key_fn1 = cls._ratelimit[0].key_fn, cls._ratelimit[1].key_fn
+        eq_(key_fn0[0]['function'](handler), pd.Timestamp.utcnow().strftime('%Y-%m-%d'))
+        eq_(key_fn0[1]['function'](handler), 'a@b')
+        eq_(key_fn1[0]['function'](handler), pd.Timestamp.utcnow().strftime('%Y-%m-%d'))
+        eq_(len(key_fn1), 1)
+
+        # If any pool has an error, entire class is not set up
+        with assert_raises(ValueError) as cm:
+            setup([{'keys': 'daily', 'limit': 10}, {'keys': 'weekly'}], gramex.conf.app.ratelimit)
+
+    def check_rate(self, url, user, limit, remaining, code=OK):
+        # If user= is specified, send an {'id': user} object via headers
+        headers = {}
+        if user is not None:
+            cookie_secret = gramex.service.app.settings['cookie_secret']
+            sign = create_signed_value(cookie_secret, 'user', json.dumps({'id': user}))
+            headers['X-Gramex-User'] = sign
+
+        # Check the status code and X-Ratelimit-* headers
+        r = self.check(url, code=code, request_headers=headers)
+        if code in (OK, TOO_MANY_REQUESTS):
+            eq_(r.headers['X-Ratelimit-Limit'], str(limit))
+            eq_(r.headers['X-Ratelimit-Remaining'], str(remaining))
+            # Check expiry time to plus/minus 2 seconds.
+            # NOTE: This test may fail if running exactly at UTC midnight
+            eod = pd.Timestamp.utcnow().normalize() + pd.Timedelta(days=1)
+            expiry = int((eod - pd.Timestamp.utcnow()).total_seconds())
+            ok_(expiry - 2 <= int(r.headers['X-Ratelimit-Reset']) <= expiry + 2)
+            # Retry-After header should be sent only for
+            if code == TOO_MANY_REQUESTS:
+                eq_(r.headers['Retry-After'], r.headers['X-Ratelimit-Reset'])
             else:
-                # No headers sent for HTTP errors
-                ok_('X-Ratelimit-Limit' not in r.headers)
-                ok_('X-Ratelimit-Remaining' not in r.headers)
-                ok_('X-Ratelimit-Reset' not in r.headers)
                 ok_('Retry-After' not in r.headers)
+        else:
+            # No headers sent for HTTP errors
+            ok_('X-Ratelimit-Limit' not in r.headers)
+            ok_('X-Ratelimit-Remaining' not in r.headers)
+            ok_('X-Ratelimit-Reset' not in r.headers)
+            ok_('Retry-After' not in r.headers)
 
+    def test_ratelimit(self):
         # Reset usage count for all users before beginning the test
         self.check('/ratelimit/reset')
         self.check('/ratelimit/reset?user=alpha')
         self.check('/ratelimit/reset?user=beta')
 
         # All HTTP headers come through OK. First usage leaves us with 2 remaining
-        check('/ratelimit/a', None, 3, 2)
+        self.check_rate('/ratelimit/a', None, 3, 2)
         # /ratelimit/b uses the same pool as /a
-        check('/ratelimit/b', None, 3, 1)
+        self.check_rate('/ratelimit/b', None, 3, 1)
         # HTTP errors don't deduct from usage
-        check('/ratelimit/a?n=0', None, 3, 1, INTERNAL_SERVER_ERROR)
-        check('/ratelimit/b?n=0', None, 3, 1, INTERNAL_SERVER_ERROR)
+        self.check_rate('/ratelimit/a?n=0', None, 3, 1, INTERNAL_SERVER_ERROR)
+        self.check_rate('/ratelimit/b?n=0', None, 3, 1, INTERNAL_SERVER_ERROR)
         # When usage exceeds, we get HTTP 429
-        check('/ratelimit/a', None, 3, 0)
-        check('/ratelimit/a', None, 3, 0, TOO_MANY_REQUESTS)
-        check('/ratelimit/b', None, 3, 0, TOO_MANY_REQUESTS)
+        self.check_rate('/ratelimit/a', None, 3, 0)
+        self.check_rate('/ratelimit/a', None, 3, 0, TOO_MANY_REQUESTS)
+        self.check_rate('/ratelimit/b', None, 3, 0, TOO_MANY_REQUESTS)
         # Different users get a different limits
-        check('/ratelimit/a', 'alpha', 3, 2)
-        check('/ratelimit/a', 'beta', 3, 2)
-        check('/ratelimit/b', 'alpha', 3, 1)
-        check('/ratelimit/b', 'beta', 3, 1)
+        self.check_rate('/ratelimit/a', 'alpha', 3, 2)
+        self.check_rate('/ratelimit/a', 'beta', 3, 2)
+        self.check_rate('/ratelimit/b', 'alpha', 3, 1)
+        self.check_rate('/ratelimit/b', 'beta', 3, 1)
+
+    def test_multiple_ratelimit(self):
+        self.check('/ratelimit/reset')
+        self.check('/ratelimit/reset?user=alpha')
+        self.check('/ratelimit/reset?user=beta')
+        self.check('/ratelimit/reset2')
+
+        # Pool: None: 0/3, alpha: 0/3, beta: 0/3, all: 0/4
+        self.check_rate('/ratelimit/ab', None, 3, 2)
+        # Pool: None: 1/3, alpha: 0/3, beta: 0/3, all: 1/4
+        self.check_rate('/ratelimit/ab', 'alpha', 3, 2)
+        # Pool: None: 1/3, alpha: 1/3, beta: 0/3, all: 2/4
+        self.check_rate('/ratelimit/ab', 'beta', 4, 1)
+        # Pool: None: 1/3, alpha: 1/3, beta: 1/3, all: 3/4
+        self.check_rate('/ratelimit/ab', None, 4, 0)
+        # Pool: None: 2/3, alpha: 1/3, beta: 1/3, all: 4/4
+        self.check_rate('/ratelimit/ab', 'alpha', 4, 0, TOO_MANY_REQUESTS)
+
+        # We can reset just a single pool
+        self.check('/ratelimit/reset2')
+        # Pool: None: 2/3, alpha: 2/3, beta: 1/3, all: 0/4
+        self.check_rate('/ratelimit/ab', 'beta', 3, 1)
+
+    def test_get_ratelimit(self):
+        self.check('/ratelimit/reset')
+
+        def check(limit, usage):
+            result = self.check('/ratelimit/info').json()
+            eq_(result['limit'], limit)
+            eq_(result['usage'], usage)
+            eq_(result['remaining'], max(limit - usage - 1, 0))
+            ok_(result['expiry'] < 86400)
+
+        check(limit=3, usage=0)
+        check(limit=3, usage=1)
+        check(limit=3, usage=2)
+        self.check('/ratelimit/info', code=TOO_MANY_REQUESTS)
```

### Comparing `gramex-1.90.0/tests/test_init.py` & `gramex-1.91.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_install.py` & `gramex-1.91.0/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_jsonhandler.py` & `gramex-1.91.0/tests/test_jsonhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_ldapauth.py` & `gramex-1.91.0/tests/test_ldapauth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_logviewer.py` & `gramex-1.91.0/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_mlhandler.py` & `gramex-1.91.0/tests/test_mlhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_modelhandler.py` & `gramex-1.91.0/tests/test_modelhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_openapihandler.py` & `gramex-1.91.0/tests/test_openapihandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_pptxhandler.py` & `gramex-1.91.0/tests/test_pptxhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_processhandler.py` & `gramex-1.91.0/tests/test_processhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_proxyhandler.py` & `gramex-1.91.0/tests/test_proxyhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_pynode.py` & `gramex-1.91.0/tests/test_pynode.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_schedule.py` & `gramex-1.91.0/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_secrets.py` & `gramex-1.91.0/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_subprocess.py` & `gramex-1.91.0/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_translater.py` & `gramex-1.91.0/tests/test_translater.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_twitterresthandler.py` & `gramex-1.91.0/tests/test_twitterresthandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_ui.py` & `gramex-1.91.0/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_update.py` & `gramex-1.91.0/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_uploadhandler.py` & `gramex-1.91.0/tests/test_uploadhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_watcher.py` & `gramex-1.91.0/tests/test_watcher.py`

 * *Files identical despite different names*

### Comparing `gramex-1.90.0/tests/test_websockethandler.py` & `gramex-1.91.0/tests/test_websockethandler.py`

 * *Files identical despite different names*

