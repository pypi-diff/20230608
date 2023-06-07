# Comparing `tmp/cedar_backup3-3.7.4.tar.gz` & `tmp/cedar_backup3-3.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cedar_backup3-3.7.4.tar", max compression
+gzip compressed data, was "cedar_backup3-3.7.5.tar", max compression
```

## Comparing `cedar_backup3-3.7.4.tar` & `cedar_backup3-3.7.5.tar`

### file list

```diff
@@ -1,189 +1,188 @@
--rw-r--r--   0        0        0    42200 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/Changelog
--rw-r--r--   0        0        0    17989 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/LICENSE
--rw-r--r--   0        0        0     9056 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/NOTICE
--rw-r--r--   0        0        0     2712 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/PyPI.md
--rw-r--r--   0        0        0     5611 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/README.md
--rw-r--r--   0        0        0       22 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/.gitignore
--rw-r--r--   0        0        0      142 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/.sphinxignore
--rw-r--r--   0        0        0     6814 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/Makefile
--rw-r--r--   0        0        0      120 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/README.md
--rw-r--r--   0        0        0      130 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/_static/custom.css
--rw-r--r--   0        0        0     1861 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/_themes/LICENSE
--rw-r--r--   0        0        0     3905 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/_themes/flask_theme_support.py
--rw-r--r--   0        0        0    13036 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/conf.py
--rw-r--r--   0        0        0     5799 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/index.rst
--rw-r--r--   0        0        0     6709 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/make.bat
--rw-r--r--   0        0        0    24291 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/basic.rst
--rw-r--r--   0        0        0    29210 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/commandline.rst
--rw-r--r--   0        0        0   108760 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/config.rst
--rw-r--r--   0        0        0    17277 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/copyright.rst
--rw-r--r--   0        0        0    11671 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/depends.rst
--rw-r--r--   0        0        0    43604 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/extensions.rst
--rw-r--r--   0        0        0     5437 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/extenspec.rst
--rw-r--r--   0        0        0     1658 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/images/note.png
--rw-r--r--   0        0        0     2331 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/images/tip.png
--rw-r--r--   0        0        0     1550 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/images/warning.png
--rw-r--r--   0        0        0      240 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/index.rst
--rw-r--r--   0        0        0     4895 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/install.rst
--rw-r--r--   0        0        0    10705 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/intro.rst
--rw-r--r--   0        0        0     3068 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/preface.rst
--rw-r--r--   0        0        0    21331 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/recovering.rst
--rw-r--r--   0        0        0     8372 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/docs/manual/securingssh.rst
--rw-r--r--   0        0        0     7391 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/manpages/cback3-amazons3-sync.1
--rw-r--r--   0        0        0     5942 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/manpages/cback3-span.1
--rw-r--r--   0        0        0    11987 2022-12-31 07:15:18.123622 cedar_backup3-3.7.4/manpages/cback3.1
--rw-r--r--   0        0        0     2829 2022-12-31 07:15:37.275559 cedar_backup3-3.7.4/pyproject.toml
--rw-r--r--   0        0        0     4608 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/samples/cback3.conf.sample
--rw-r--r--   0        0        0     2401 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/__init__.py
--rw-r--r--   0        0        0     1661 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/action.py
--rw-r--r--   0        0        0     2017 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/actions/__init__.py
--rw-r--r--   0        0        0    23234 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/actions/collect.py
--rw-r--r--   0        0        0     1230 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/actions/constants.py
--rw-r--r--   0        0        0     3108 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/actions/initialize.py
--rw-r--r--   0        0        0     3500 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/actions/purge.py
--rw-r--r--   0        0        0     6344 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/actions/rebuild.py
--rw-r--r--   0        0        0    12880 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/actions/stage.py
--rw-r--r--   0        0        0    17814 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/actions/store.py
--rw-r--r--   0        0        0    13494 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/actions/util.py
--rw-r--r--   0        0        0    12099 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/actions/validate.py
--rw-r--r--   0        0        0    82265 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/cli.py
--rw-r--r--   0        0        0   250416 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/config.py
--rw-r--r--   0        0        0     3459 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/customize.py
--rw-r--r--   0        0        0     1695 2022-12-31 07:15:18.127622 cedar_backup3-3.7.4/src/CedarBackup3/extend/__init__.py
--rw-r--r--   0        0        0    36418 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/extend/amazons3.py
--rw-r--r--   0        0        0    22063 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/extend/capacity.py
--rw-r--r--   0        0        0    21387 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/extend/encrypt.py
--rw-r--r--   0        0        0    59655 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/extend/mbox.py
--rw-r--r--   0        0        0    28213 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/extend/mysql.py
--rw-r--r--   0        0        0    25472 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/extend/postgresql.py
--rw-r--r--   0        0        0    20095 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/extend/split.py
--rw-r--r--   0        0        0    63173 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/extend/subversion.py
--rw-r--r--   0        0        0     9074 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/extend/sysinfo.py
--rw-r--r--   0        0        0    65889 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/filesystem.py
--rw-r--r--   0        0        0     1326 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/image.py
--rw-r--r--   0        0        0    13475 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/knapsack.py
--rw-r--r--   0        0        0    52144 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/peer.py
--rw-r--r--   0        0        0     2116 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/release.py
--rw-r--r--   0        0        0     1281 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/scripts.py
--rw-r--r--   0        0        0    16087 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/testutil.py
--rw-r--r--   0        0        0     1813 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/tools/__init__.py
--rw-r--r--   0        0        0    48194 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/tools/amazons3.py
--rw-r--r--   0        0        0    26110 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/tools/span.py
--rw-r--r--   0        0        0    75364 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/util.py
--rw-r--r--   0        0        0     1551 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/writer.py
--rw-r--r--   0        0        0     1398 2022-12-31 07:15:18.131622 cedar_backup3-3.7.4/src/CedarBackup3/writers/__init__.py
--rw-r--r--   0        0        0    55150 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/src/CedarBackup3/writers/cdwriter.py
--rw-r--r--   0        0        0    41298 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/src/CedarBackup3/writers/dvdwriter.py
--rw-r--r--   0        0        0    28676 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/src/CedarBackup3/writers/util.py
--rw-r--r--   0        0        0    27076 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/src/CedarBackup3/xmlutil.py
--rw-r--r--   0        0        0      797 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/__init__.py
--rw-r--r--   0        0        0       59 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/amazons3.conf.1
--rw-r--r--   0        0        0      340 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/amazons3.conf.2
--rw-r--r--   0        0        0      304 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/amazons3.conf.3
--rw-r--r--   0        0        0       59 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/capacity.conf.1
--rw-r--r--   0        0        0      172 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/capacity.conf.2
--rw-r--r--   0        0        0      170 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/capacity.conf.3
--rw-r--r--   0        0        0      172 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/capacity.conf.4
--rw-r--r--   0        0        0     2052 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.1
--rw-r--r--   0        0        0      915 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.10
--rw-r--r--   0        0        0      291 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.11
--rw-r--r--   0        0        0      753 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.12
--rw-r--r--   0        0        0      265 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.13
--rw-r--r--   0        0        0      501 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.14
--rw-r--r--   0        0        0     5175 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.15
--rw-r--r--   0        0        0      340 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.16
--rw-r--r--   0        0        0      396 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.17
--rw-r--r--   0        0        0      390 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.18
--rw-r--r--   0        0        0     1904 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.19
--rw-r--r--   0        0        0       59 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.2
--rw-r--r--   0        0        0     5271 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.20
--rw-r--r--   0        0        0     5848 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.21
--rw-r--r--   0        0        0      297 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.22
--rw-r--r--   0        0        0     1408 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.23
--rw-r--r--   0        0        0      166 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.3
--rw-r--r--   0        0        0      354 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.4
--rw-r--r--   0        0        0      386 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.5
--rw-r--r--   0        0        0     1010 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.6
--rw-r--r--   0        0        0      394 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.7
--rw-r--r--   0        0        0     2005 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.8
--rw-r--r--   0        0        0      350 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/cback.conf.9
--rw-r--r--   0        0        0       59 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/encrypt.conf.1
--rw-r--r--   0        0        0      188 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/encrypt.conf.2
--rw-r--r--   0        0        0      605 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/lotsoflines.py
--rw-r--r--   0        0        0       59 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/mbox.conf.1
--rw-r--r--   0        0        0      397 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/mbox.conf.2
--rw-r--r--   0        0        0      496 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/mbox.conf.3
--rw-r--r--   0        0        0     1355 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/mbox.conf.4
--rw-r--r--   0        0        0       59 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/mysql.conf.1
--rw-r--r--   0        0        0      263 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/mysql.conf.2
--rw-r--r--   0        0        0      303 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/mysql.conf.3
--rw-r--r--   0        0        0      346 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/mysql.conf.4
--rw-r--r--   0        0        0      307 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/mysql.conf.5
--rw-r--r--   0        0        0       59 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/postgresql.conf.1
--rw-r--r--   0        0        0      242 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/postgresql.conf.2
--rw-r--r--   0        0        0      282 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/postgresql.conf.3
--rw-r--r--   0        0        0      325 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/postgresql.conf.4
--rw-r--r--   0        0        0      310 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/postgresql.conf.5
--rw-r--r--   0        0        0       59 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/split.conf.1
--rw-r--r--   0        0        0      170 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/split.conf.2
--rw-r--r--   0        0        0      170 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/split.conf.3
--rw-r--r--   0        0        0      180 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/split.conf.4
--rw-r--r--   0        0        0      171 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/split.conf.5
--rw-r--r--   0        0        0       59 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/subversion.conf.1
--rw-r--r--   0        0        0      311 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/subversion.conf.2
--rw-r--r--   0        0        0      319 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/subversion.conf.3
--rw-r--r--   0        0        0      838 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/subversion.conf.4
--rw-r--r--   0        0        0      323 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/subversion.conf.5
--rw-r--r--   0        0        0      331 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/subversion.conf.6
--rw-r--r--   0        0        0     1243 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/subversion.conf.7
--rw-r--r--   0        0        0      263 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree1.ini
--rw-r--r--   0        0        0     1021 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree1.tar.gz
--rw-r--r--   0        0        0      391 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree10.tar.gz
--rw-r--r--   0        0        0      641 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree11.tar.gz
--rw-r--r--   0        0        0    75185 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree12.tar.gz
--rw-r--r--   0        0        0      422 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree13.tar.gz
--rw-r--r--   0        0        0      700 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree15.tar.gz
--rw-r--r--   0        0        0     8971 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree16.tar.gz
--rw-r--r--   0        0        0      997 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree17.tar.gz
--rw-r--r--   0        0        0      968 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree18.tar.gz
--rw-r--r--   0        0        0      939 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree19.tar.gz
--rw-r--r--   0        0        0      269 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree2.ini
--rw-r--r--   0        0        0      224 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree2.tar.gz
--rw-r--r--   0        0        0      976 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree20.tar.gz
--rw-r--r--   0        0        0     3557 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree21.tar.gz
--rw-r--r--   0        0        0     6158 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree22.tar.gz
--rw-r--r--   0        0        0      270 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree3.ini
--rw-r--r--   0        0        0      604 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree3.tar.gz
--rw-r--r--   0        0        0      275 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree4.ini
--rw-r--r--   0        0        0     9120 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree4.tar.gz
--rw-r--r--   0        0        0      282 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree5.ini
--rw-r--r--   0        0        0    13611 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree5.tar.gz
--rw-r--r--   0        0        0      274 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree6.ini
--rw-r--r--   0        0        0    28998 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree6.tar.gz
--rw-r--r--   0        0        0      178 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree7.tar.gz
--rw-r--r--   0        0        0      148 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree8.tar.gz
--rw-r--r--   0        0        0      272 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree9.ini
--rw-r--r--   0        0        0     1394 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/data/tree9.tar.gz
--rw-r--r--   0        0        0     9503 2022-12-31 07:15:18.135622 cedar_backup3-3.7.4/tests/test_actions_util.py
--rw-r--r--   0        0        0    36814 2022-12-31 07:15:18.139622 cedar_backup3-3.7.4/tests/test_amazons3.py
--rw-r--r--   0        0        0    33089 2022-12-31 07:15:18.139622 cedar_backup3-3.7.4/tests/test_capacity.py
--rw-r--r--   0        0        0    80468 2022-12-31 07:15:18.139622 cedar_backup3-3.7.4/tests/test_cdwriter.py
--rw-r--r--   0        0        0   674560 2022-12-31 07:15:18.139622 cedar_backup3-3.7.4/tests/test_cli.py
--rw-r--r--   0        0        0   542233 2022-12-31 07:15:18.143622 cedar_backup3-3.7.4/tests/test_config.py
--rw-r--r--   0        0        0     8124 2022-12-31 07:15:18.143622 cedar_backup3-3.7.4/tests/test_customize.py
--rw-r--r--   0        0        0    51496 2022-12-31 07:15:18.143622 cedar_backup3-3.7.4/tests/test_dvdwriter.py
--rw-r--r--   0        0        0    54326 2022-12-31 07:15:18.143622 cedar_backup3-3.7.4/tests/test_encrypt.py
--rw-r--r--   0        0        0  1291994 2022-12-31 07:15:18.147621 cedar_backup3-3.7.4/tests/test_filesystem.py
--rw-r--r--   0        0        0    99436 2022-12-31 07:15:18.147621 cedar_backup3-3.7.4/tests/test_knapsack.py
--rw-r--r--   0        0        0    84647 2022-12-31 07:15:18.147621 cedar_backup3-3.7.4/tests/test_mbox.py
--rw-r--r--   0        0        0    40974 2022-12-31 07:15:18.147621 cedar_backup3-3.7.4/tests/test_mysql.py
--rw-r--r--   0        0        0    68089 2022-12-31 07:15:18.147621 cedar_backup3-3.7.4/tests/test_peer.py
--rw-r--r--   0        0        0    39155 2022-12-31 07:15:18.147621 cedar_backup3-3.7.4/tests/test_postgresql.py
--rw-r--r--   0        0        0     4905 2022-12-31 07:15:18.147621 cedar_backup3-3.7.4/tests/test_span.py
--rw-r--r--   0        0        0    46613 2022-12-31 07:15:18.151621 cedar_backup3-3.7.4/tests/test_split.py
--rw-r--r--   0        0        0   108595 2022-12-31 07:15:18.151621 cedar_backup3-3.7.4/tests/test_subversion.py
--rw-r--r--   0        0        0   153535 2022-12-31 07:15:18.151621 cedar_backup3-3.7.4/tests/test_sync.py
--rw-r--r--   0        0        0   149942 2022-12-31 07:15:18.151621 cedar_backup3-3.7.4/tests/test_util.py
--rw-r--r--   0        0        0    70705 2022-12-31 07:15:18.151621 cedar_backup3-3.7.4/tests/test_writers_util.py
--rw-r--r--   0        0        0     4019 1970-01-01 00:00:00.000000 cedar_backup3-3.7.4/setup.py
--rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 cedar_backup3-3.7.4/PKG-INFO
+-rw-r--r--   0        0        0    42395 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/Changelog
+-rw-r--r--   0        0        0    17989 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/LICENSE
+-rw-r--r--   0        0        0     9056 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/NOTICE
+-rw-r--r--   0        0        0     2712 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/PyPI.md
+-rw-r--r--   0        0        0     5611 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/README.md
+-rw-r--r--   0        0        0       22 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/.gitignore
+-rw-r--r--   0        0        0      142 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/.sphinxignore
+-rw-r--r--   0        0        0     6814 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/Makefile
+-rw-r--r--   0        0        0      120 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/README.md
+-rw-r--r--   0        0        0      130 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/_static/custom.css
+-rw-r--r--   0        0        0     1861 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/_themes/LICENSE
+-rw-r--r--   0        0        0     3905 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/_themes/flask_theme_support.py
+-rw-r--r--   0        0        0    13036 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/conf.py
+-rw-r--r--   0        0        0     5799 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/index.rst
+-rw-r--r--   0        0        0     6709 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/make.bat
+-rw-r--r--   0        0        0    24291 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/manual/basic.rst
+-rw-r--r--   0        0        0    29210 2023-06-07 23:11:51.191817 cedar_backup3-3.7.5/docs/manual/commandline.rst
+-rw-r--r--   0        0        0   108760 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/config.rst
+-rw-r--r--   0        0        0    17277 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/copyright.rst
+-rw-r--r--   0        0        0    11671 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/depends.rst
+-rw-r--r--   0        0        0    43604 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/extensions.rst
+-rw-r--r--   0        0        0     5437 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/extenspec.rst
+-rw-r--r--   0        0        0     1658 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/images/note.png
+-rw-r--r--   0        0        0     2331 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/images/tip.png
+-rw-r--r--   0        0        0     1550 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/images/warning.png
+-rw-r--r--   0        0        0      240 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/index.rst
+-rw-r--r--   0        0        0     4895 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/install.rst
+-rw-r--r--   0        0        0    10705 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/intro.rst
+-rw-r--r--   0        0        0     3068 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/preface.rst
+-rw-r--r--   0        0        0    21331 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/recovering.rst
+-rw-r--r--   0        0        0     8372 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/docs/manual/securingssh.rst
+-rw-r--r--   0        0        0     7391 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/manpages/cback3-amazons3-sync.1
+-rw-r--r--   0        0        0     5942 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/manpages/cback3-span.1
+-rw-r--r--   0        0        0    11987 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/manpages/cback3.1
+-rw-r--r--   0        0        0     2847 2023-06-07 23:12:26.167810 cedar_backup3-3.7.5/pyproject.toml
+-rw-r--r--   0        0        0     4608 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/samples/cback3.conf.sample
+-rw-r--r--   0        0        0     2401 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/__init__.py
+-rw-r--r--   0        0        0     1661 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/action.py
+-rw-r--r--   0        0        0     2017 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/__init__.py
+-rw-r--r--   0        0        0    23235 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/collect.py
+-rw-r--r--   0        0        0     1230 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/constants.py
+-rw-r--r--   0        0        0     3109 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/initialize.py
+-rw-r--r--   0        0        0     3501 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/purge.py
+-rw-r--r--   0        0        0     6345 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/rebuild.py
+-rw-r--r--   0        0        0    12881 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/stage.py
+-rw-r--r--   0        0        0    17815 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/store.py
+-rw-r--r--   0        0        0    13494 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/util.py
+-rw-r--r--   0        0        0    12100 2023-06-07 23:11:51.195818 cedar_backup3-3.7.5/src/CedarBackup3/actions/validate.py
+-rw-r--r--   0        0        0    82264 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/cli.py
+-rw-r--r--   0        0        0   250415 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/config.py
+-rw-r--r--   0        0        0     3459 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/customize.py
+-rw-r--r--   0        0        0     1695 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/__init__.py
+-rw-r--r--   0        0        0    36418 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/amazons3.py
+-rw-r--r--   0        0        0    22064 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/capacity.py
+-rw-r--r--   0        0        0    21388 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/encrypt.py
+-rw-r--r--   0        0        0    59655 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/mbox.py
+-rw-r--r--   0        0        0    28214 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/mysql.py
+-rw-r--r--   0        0        0    25473 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/postgresql.py
+-rw-r--r--   0        0        0    20096 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/split.py
+-rw-r--r--   0        0        0    63173 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/subversion.py
+-rw-r--r--   0        0        0     9075 2023-06-07 23:11:51.199818 cedar_backup3-3.7.5/src/CedarBackup3/extend/sysinfo.py
+-rw-r--r--   0        0        0    65886 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/filesystem.py
+-rw-r--r--   0        0        0     1326 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/image.py
+-rw-r--r--   0        0        0    13471 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/knapsack.py
+-rw-r--r--   0        0        0    52142 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/peer.py
+-rw-r--r--   0        0        0     2116 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/release.py
+-rw-r--r--   0        0        0     1281 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/scripts.py
+-rw-r--r--   0        0        0    16088 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/testutil.py
+-rw-r--r--   0        0        0     1813 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/tools/__init__.py
+-rw-r--r--   0        0        0    48194 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/tools/amazons3.py
+-rw-r--r--   0        0        0    26111 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/tools/span.py
+-rw-r--r--   0        0        0    75364 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/util.py
+-rw-r--r--   0        0        0     1551 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/writer.py
+-rw-r--r--   0        0        0     1398 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/writers/__init__.py
+-rw-r--r--   0        0        0    55149 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/writers/cdwriter.py
+-rw-r--r--   0        0        0    41297 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/writers/dvdwriter.py
+-rw-r--r--   0        0        0    28675 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/writers/util.py
+-rw-r--r--   0        0        0    27076 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/src/CedarBackup3/xmlutil.py
+-rw-r--r--   0        0        0      797 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/__init__.py
+-rw-r--r--   0        0        0       59 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/amazons3.conf.1
+-rw-r--r--   0        0        0      340 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/amazons3.conf.2
+-rw-r--r--   0        0        0      304 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/amazons3.conf.3
+-rw-r--r--   0        0        0       59 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/capacity.conf.1
+-rw-r--r--   0        0        0      172 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/capacity.conf.2
+-rw-r--r--   0        0        0      170 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/capacity.conf.3
+-rw-r--r--   0        0        0      172 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/capacity.conf.4
+-rw-r--r--   0        0        0     2052 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.1
+-rw-r--r--   0        0        0      915 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.10
+-rw-r--r--   0        0        0      291 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.11
+-rw-r--r--   0        0        0      753 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.12
+-rw-r--r--   0        0        0      265 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.13
+-rw-r--r--   0        0        0      501 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.14
+-rw-r--r--   0        0        0     5175 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.15
+-rw-r--r--   0        0        0      340 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.16
+-rw-r--r--   0        0        0      396 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.17
+-rw-r--r--   0        0        0      390 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.18
+-rw-r--r--   0        0        0     1904 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.19
+-rw-r--r--   0        0        0       59 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.2
+-rw-r--r--   0        0        0     5271 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.20
+-rw-r--r--   0        0        0     5848 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.21
+-rw-r--r--   0        0        0      297 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.22
+-rw-r--r--   0        0        0     1408 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.23
+-rw-r--r--   0        0        0      166 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.3
+-rw-r--r--   0        0        0      354 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.4
+-rw-r--r--   0        0        0      386 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.5
+-rw-r--r--   0        0        0     1010 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.6
+-rw-r--r--   0        0        0      394 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.7
+-rw-r--r--   0        0        0     2005 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.8
+-rw-r--r--   0        0        0      350 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/cback.conf.9
+-rw-r--r--   0        0        0       59 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/encrypt.conf.1
+-rw-r--r--   0        0        0      188 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/encrypt.conf.2
+-rw-r--r--   0        0        0      605 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/lotsoflines.py
+-rw-r--r--   0        0        0       59 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mbox.conf.1
+-rw-r--r--   0        0        0      397 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mbox.conf.2
+-rw-r--r--   0        0        0      496 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mbox.conf.3
+-rw-r--r--   0        0        0     1355 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mbox.conf.4
+-rw-r--r--   0        0        0       59 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mysql.conf.1
+-rw-r--r--   0        0        0      263 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mysql.conf.2
+-rw-r--r--   0        0        0      303 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mysql.conf.3
+-rw-r--r--   0        0        0      346 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mysql.conf.4
+-rw-r--r--   0        0        0      307 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/mysql.conf.5
+-rw-r--r--   0        0        0       59 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/postgresql.conf.1
+-rw-r--r--   0        0        0      242 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/postgresql.conf.2
+-rw-r--r--   0        0        0      282 2023-06-07 23:11:51.203817 cedar_backup3-3.7.5/tests/data/postgresql.conf.3
+-rw-r--r--   0        0        0      325 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/postgresql.conf.4
+-rw-r--r--   0        0        0      310 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/postgresql.conf.5
+-rw-r--r--   0        0        0       59 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/split.conf.1
+-rw-r--r--   0        0        0      170 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/split.conf.2
+-rw-r--r--   0        0        0      170 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/split.conf.3
+-rw-r--r--   0        0        0      180 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/split.conf.4
+-rw-r--r--   0        0        0      171 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/split.conf.5
+-rw-r--r--   0        0        0       59 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/subversion.conf.1
+-rw-r--r--   0        0        0      311 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/subversion.conf.2
+-rw-r--r--   0        0        0      319 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/subversion.conf.3
+-rw-r--r--   0        0        0      838 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/subversion.conf.4
+-rw-r--r--   0        0        0      323 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/subversion.conf.5
+-rw-r--r--   0        0        0      331 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/subversion.conf.6
+-rw-r--r--   0        0        0     1243 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/subversion.conf.7
+-rw-r--r--   0        0        0      263 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree1.ini
+-rw-r--r--   0        0        0     1021 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree1.tar.gz
+-rw-r--r--   0        0        0      391 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree10.tar.gz
+-rw-r--r--   0        0        0      641 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree11.tar.gz
+-rw-r--r--   0        0        0    75185 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree12.tar.gz
+-rw-r--r--   0        0        0      422 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree13.tar.gz
+-rw-r--r--   0        0        0      700 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree15.tar.gz
+-rw-r--r--   0        0        0     8971 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree16.tar.gz
+-rw-r--r--   0        0        0      997 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree17.tar.gz
+-rw-r--r--   0        0        0      968 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree18.tar.gz
+-rw-r--r--   0        0        0      939 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree19.tar.gz
+-rw-r--r--   0        0        0      269 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree2.ini
+-rw-r--r--   0        0        0      224 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree2.tar.gz
+-rw-r--r--   0        0        0      976 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree20.tar.gz
+-rw-r--r--   0        0        0     3557 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree21.tar.gz
+-rw-r--r--   0        0        0     6158 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree22.tar.gz
+-rw-r--r--   0        0        0      270 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree3.ini
+-rw-r--r--   0        0        0      604 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree3.tar.gz
+-rw-r--r--   0        0        0      275 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree4.ini
+-rw-r--r--   0        0        0     9120 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree4.tar.gz
+-rw-r--r--   0        0        0      282 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree5.ini
+-rw-r--r--   0        0        0    13611 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree5.tar.gz
+-rw-r--r--   0        0        0      274 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree6.ini
+-rw-r--r--   0        0        0    28998 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree6.tar.gz
+-rw-r--r--   0        0        0      178 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree7.tar.gz
+-rw-r--r--   0        0        0      148 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree8.tar.gz
+-rw-r--r--   0        0        0      272 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree9.ini
+-rw-r--r--   0        0        0     1394 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/data/tree9.tar.gz
+-rw-r--r--   0        0        0     9503 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/test_actions_util.py
+-rw-r--r--   0        0        0    36813 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/test_amazons3.py
+-rw-r--r--   0        0        0    33089 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/test_capacity.py
+-rw-r--r--   0        0        0    80468 2023-06-07 23:11:51.207817 cedar_backup3-3.7.5/tests/test_cdwriter.py
+-rw-r--r--   0        0        0   674560 2023-06-07 23:11:51.211818 cedar_backup3-3.7.5/tests/test_cli.py
+-rw-r--r--   0        0        0   542233 2023-06-07 23:11:51.211818 cedar_backup3-3.7.5/tests/test_config.py
+-rw-r--r--   0        0        0     8124 2023-06-07 23:11:51.211818 cedar_backup3-3.7.5/tests/test_customize.py
+-rw-r--r--   0        0        0    51496 2023-06-07 23:11:51.211818 cedar_backup3-3.7.5/tests/test_dvdwriter.py
+-rw-r--r--   0        0        0    54326 2023-06-07 23:11:51.211818 cedar_backup3-3.7.5/tests/test_encrypt.py
+-rw-r--r--   0        0        0  1291994 2023-06-07 23:11:51.215818 cedar_backup3-3.7.5/tests/test_filesystem.py
+-rw-r--r--   0        0        0    99436 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_knapsack.py
+-rw-r--r--   0        0        0    84647 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_mbox.py
+-rw-r--r--   0        0        0    40974 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_mysql.py
+-rw-r--r--   0        0        0    68089 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_peer.py
+-rw-r--r--   0        0        0    39155 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_postgresql.py
+-rw-r--r--   0        0        0     4905 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_span.py
+-rw-r--r--   0        0        0    46613 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_split.py
+-rw-r--r--   0        0        0   108595 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_subversion.py
+-rw-r--r--   0        0        0   153535 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_sync.py
+-rw-r--r--   0        0        0   149942 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_util.py
+-rw-r--r--   0        0        0    70705 2023-06-07 23:11:51.219817 cedar_backup3-3.7.5/tests/test_writers_util.py
+-rw-r--r--   0        0        0     4072 1970-01-01 00:00:00.000000 cedar_backup3-3.7.5/PKG-INFO
```

### Comparing `cedar_backup3-3.7.4/Changelog` & `cedar_backup3-3.7.5/Changelog`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Version 3.7.5     07 Jun 2023
+
+	* Fix checktabs to be safe for file named '-'.
+	* Upgrade all dependencies to the latest major version.
+	* Upgrade to Poetry v1.5.1 and make related adjustments.
+
 Version 3.7.4     31 Dec 2022
 
 	* Pull Sphinx fields from metadata rather than parsing pyproject.toml.
 
 Version 3.7.3     30 Dec 2022
 
 	* Convert to latest readthedocs.io standard.
```

### Comparing `cedar_backup3-3.7.4/LICENSE` & `cedar_backup3-3.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/NOTICE` & `cedar_backup3-3.7.5/NOTICE`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ##########
 # Credits
 ##########
 
 Unless otherwise indicated, all material in this repository is under the
 following license:
 
-   Copyright (c) 2004-2022 Kenneth J. Pronovici <pronovic@ieee.org>
+   Copyright (c) 2004-2023 Kenneth J. Pronovici <pronovic@ieee.org>
 
    This program is free software; you can redistribute it and/or modify it
    under the terms of version 2 of the GNU General Public License as
    published by the Free Software Foundation.
 
    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `cedar_backup3-3.7.4/PyPI.md` & `cedar_backup3-3.7.5/PyPI.md`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/README.md` & `cedar_backup3-3.7.5/README.md`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/Makefile` & `cedar_backup3-3.7.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/_themes/LICENSE` & `cedar_backup3-3.7.5/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/_themes/flask_theme_support.py` & `cedar_backup3-3.7.5/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/conf.py` & `cedar_backup3-3.7.5/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 release = VERSION
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
```

### Comparing `cedar_backup3-3.7.4/docs/index.rst` & `cedar_backup3-3.7.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/make.bat` & `cedar_backup3-3.7.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/manual/basic.rst` & `cedar_backup3-3.7.5/docs/manual/basic.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/manual/commandline.rst` & `cedar_backup3-3.7.5/docs/manual/commandline.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/manual/config.rst` & `cedar_backup3-3.7.5/docs/manual/config.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/manual/copyright.rst` & `cedar_backup3-3.7.5/docs/manual/copyright.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/manual/depends.rst` & `cedar_backup3-3.7.5/docs/manual/depends.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/manual/extensions.rst` & `cedar_backup3-3.7.5/docs/manual/extensions.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/manual/extenspec.rst` & `cedar_backup3-3.7.5/docs/manual/extenspec.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/manual/images/note.png` & `cedar_backup3-3.7.5/docs/manual/images/note.png`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/manual/images/tip.png` & `cedar_backup3-3.7.5/docs/manual/images/tip.png`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/manual/images/warning.png` & `cedar_backup3-3.7.5/docs/manual/images/warning.png`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/manual/install.rst` & `cedar_backup3-3.7.5/docs/manual/install.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/manual/intro.rst` & `cedar_backup3-3.7.5/docs/manual/intro.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/manual/preface.rst` & `cedar_backup3-3.7.5/docs/manual/preface.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/manual/recovering.rst` & `cedar_backup3-3.7.5/docs/manual/recovering.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/docs/manual/securingssh.rst` & `cedar_backup3-3.7.5/docs/manual/securingssh.rst`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/manpages/cback3-amazons3-sync.1` & `cedar_backup3-3.7.5/manpages/cback3-amazons3-sync.1`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/manpages/cback3-span.1` & `cedar_backup3-3.7.5/manpages/cback3-span.1`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/manpages/cback3.1` & `cedar_backup3-3.7.5/manpages/cback3.1`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/pyproject.toml` & `cedar_backup3-3.7.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cedar-backup3"
-version = "3.7.4" # published version is managed using Git tags (see below)
+version = "3.7.5" # published version is managed using Git tags (see below)
 description = "Implements local and remote backups to CD/DVD and Amazon S3"
 keywords = [ 'local', 'remote', 'backup', 'scp' ]
 authors = ["Kenneth J. Pronovici <pronovic@ieee.org>"]
 license = "GPL-2.0-only"
 readme = "PyPI.md"
 homepage = "https://pypi.org/project/cedar-backup3/"
 repository = "https://github.com/pronovic/cedar-backup3"
@@ -43,34 +43,34 @@
 [tool.poetry.scripts]
 cback3 = 'CedarBackup3.scripts:cback3' 
 cback3-amazons3-sync = 'CedarBackup3.scripts:amazons3' 
 cback3-span = 'CedarBackup3.scripts:span' 
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
-chardet = "^4.0.0"
-importlib-metadata = "^5.2.0"
-sphinx = { version="^4.5.0", optional=true }
-sphinx-autoapi = { version="^1.8.4", optional=true }
+chardet = "^5.1.0"
+importlib-metadata = "^6.0.0"
+sphinx = { version="^6.1.3", optional=true }
+sphinx-autoapi = { version="^2.0.1", optional=true }
 
 [tool.poetry.extras]
 docs = [ "sphinx", "sphinx-autoapi" ]
 
 [tool.poetry.group.dev.dependencies]
-coverage = "^6.3.2"
-pylint = "^2.15.0"
-pre-commit = "^2.18.1"
-black = "^22.3.0"
-isort = "^5.10.1"
+coverage = "^6.5.0"
+pylint = "^2.16.2"
+pre-commit = "^3.1.0"
+black = "^23.1.0"
+isort = "^5.12.0"
 coveralls = "^3.3.1"
-colorama = "^0.4.5"
+colorama = "~0, >=0.4.6"
 
 [tool.black]
 line-length = 132
-target-version = ['py38', 'py39', 'py310' ]
+target-version = ['py38', 'py39', 'py310', 'py311' ]
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
   | __pycache__
   | \.tox
   | \.venv
@@ -84,9 +84,9 @@
 
 [tool.isort]
 profile = "black"
 line_length = 132
 skip_glob = [ "docs", "notes" ]
 
 [build-system]
-requires = ["poetry>=1.0.0", "poetry-dynamic-versioning"]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `cedar_backup3-3.7.4/samples/cback3.conf.sample` & `cedar_backup3-3.7.5/samples/cback3.conf.sample`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/__init__.py` & `cedar_backup3-3.7.5/src/CedarBackup3/__init__.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/action.py` & `cedar_backup3-3.7.5/src/CedarBackup3/action.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/actions/__init__.py` & `cedar_backup3-3.7.5/src/CedarBackup3/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/actions/collect.py` & `cedar_backup3-3.7.5/src/CedarBackup3/actions/collect.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 # Public functions
 ########################################################################
 
 ############################
 # executeCollect() function
 ############################
 
+
 # pylint: disable=W0613
 def executeCollect(configPath, options, config):
     """
     Executes the collect backup action.
 
     *Note:* When the collect action is complete, we will write a collect
     indicator to the collect directory, so it's obvious that the collect action
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/actions/constants.py` & `cedar_backup3-3.7.5/src/CedarBackup3/actions/constants.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/actions/initialize.py` & `cedar_backup3-3.7.5/src/CedarBackup3/actions/initialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 # Public functions
 ########################################################################
 
 ###############################
 # executeInitialize() function
 ###############################
 
+
 # pylint: disable=W0613
 def executeInitialize(configPath, options, config):
     """
     Executes the initialize action.
 
     The initialize action initializes the media currently in the writer
     device so that Cedar Backup can recognize it later.  This is an optional
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/actions/purge.py` & `cedar_backup3-3.7.5/src/CedarBackup3/actions/purge.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 # Public functions
 ########################################################################
 
 ##########################
 # executePurge() function
 ##########################
 
+
 # pylint: disable=W0613
 def executePurge(configPath, options, config):
     """
     Executes the purge backup action.
 
     For each configured directory, we create a purge item list, remove from the
     list anything that's younger than the configured retain days value, and then
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/actions/rebuild.py` & `cedar_backup3-3.7.5/src/CedarBackup3/actions/rebuild.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 # Public functions
 ########################################################################
 
 ############################
 # executeRebuild() function
 ############################
 
+
 # pylint: disable=W0613
 def executeRebuild(configPath, options, config):
     """
     Executes the rebuild backup action.
 
     This function exists mainly to recreate a disc that has been "trashed" due
     to media or hardware problems.  Note that the "stage complete" indicator
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/actions/stage.py` & `cedar_backup3-3.7.5/src/CedarBackup3/actions/stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 # Public functions
 ########################################################################
 
 ##########################
 # executeStage() function
 ##########################
 
+
 # pylint: disable=W0613
 # noinspection PyTypeChecker
 def executeStage(configPath, options, config):
     """
     Executes the stage backup action.
 
     *Note:* The daily directory is derived once and then we stick with it, just
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/actions/store.py` & `cedar_backup3-3.7.5/src/CedarBackup3/actions/store.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 # Public functions
 ########################################################################
 
 ##########################
 # executeStore() function
 ##########################
 
+
 # pylint: disable=W0613
 def executeStore(configPath, options, config):
     """
     Executes the store backup action.
 
     *Note:* The rebuild action and the store action are very similar.  The
     main difference is that while store only stores a single day's staging
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/actions/util.py` & `cedar_backup3-3.7.5/src/CedarBackup3/actions/util.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/actions/validate.py` & `cedar_backup3-3.7.5/src/CedarBackup3/actions/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 # Public functions
 ########################################################################
 
 #############################
 # executeValidate() function
 #############################
 
+
 # pylint: disable=W0613
 def executeValidate(configPath, options, config):
     """
     Executes the validate action.
 
     This action validates each of the individual sections in the config file.
     This is a "runtime" validation.  The config file itself is already valid in
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/cli.py` & `cedar_backup3-3.7.5/src/CedarBackup3/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1309,15 +1309,14 @@
 #########################################################################
 # Options class definition
 ########################################################################
 
 
 @total_ordering
 class Options(object):
-
     ######################
     # Class documentation
     ######################
 
     """
     Class representing command-line options for the cback3 script.
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/config.py` & `cedar_backup3-3.7.5/src/CedarBackup3/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -4414,15 +4414,14 @@
 ########################################################################
 # Config class definition
 ########################################################################
 
 
 @total_ordering
 class Config(object):
-
     ######################
     # Class documentation
     ######################
 
     """
     Class representing a Cedar Backup XML configuration document.
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/customize.py` & `cedar_backup3-3.7.5/src/CedarBackup3/customize.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/extend/__init__.py` & `cedar_backup3-3.7.5/src/CedarBackup3/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/extend/amazons3.py` & `cedar_backup3-3.7.5/src/CedarBackup3/extend/amazons3.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/extend/capacity.py` & `cedar_backup3-3.7.5/src/CedarBackup3/extend/capacity.py`

 * *Files 1% similar despite different names*

```diff
@@ -547,14 +547,15 @@
 # Public functions
 ########################################################################
 
 ###########################
 # executeAction() function
 ###########################
 
+
 # pylint: disable=W0613
 def executeAction(configPath, options, config):
     """
     Executes the capacity action.
 
     Args:
        configPath (String representing a path on disk): Path to configuration file on disk
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/extend/encrypt.py` & `cedar_backup3-3.7.5/src/CedarBackup3/extend/encrypt.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,14 +414,15 @@
 # Public functions
 ########################################################################
 
 ###########################
 # executeAction() function
 ###########################
 
+
 # pylint: disable=W0613
 def executeAction(configPath, options, config):
     """
     Executes the encrypt backup action.
 
     Args:
        configPath (String representing a path on disk): Path to configuration file on disk
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/extend/mbox.py` & `cedar_backup3-3.7.5/src/CedarBackup3/extend/mbox.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/extend/mysql.py` & `cedar_backup3-3.7.5/src/CedarBackup3/extend/mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,14 +557,15 @@
 # Public functions
 ########################################################################
 
 ###########################
 # executeAction() function
 ###########################
 
+
 # pylint: disable=W0613
 def executeAction(configPath, options, config):
     """
     Executes the MySQL backup action.
 
     Args:
        configPath (String representing a path on disk): Path to configuration file on disk
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/extend/postgresql.py` & `cedar_backup3-3.7.5/src/CedarBackup3/extend/postgresql.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,14 +522,15 @@
 # Public functions
 ########################################################################
 
 ###########################
 # executeAction() function
 ###########################
 
+
 # pylint: disable=W0613
 def executeAction(configPath, options, config):
     """
     Executes the PostgreSQL backup action.
 
     Args:
        configPath (String representing a path on disk): Path to configuration file on disk
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/extend/split.py` & `cedar_backup3-3.7.5/src/CedarBackup3/extend/split.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,14 +419,15 @@
 # Public functions
 ########################################################################
 
 ###########################
 # executeAction() function
 ###########################
 
+
 # pylint: disable=W0613
 def executeAction(configPath, options, config):
     """
     Executes the split backup action.
 
     Args:
        configPath (String representing a path on disk): Path to configuration file on disk
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/extend/subversion.py` & `cedar_backup3-3.7.5/src/CedarBackup3/extend/subversion.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/extend/sysinfo.py` & `cedar_backup3-3.7.5/src/CedarBackup3/extend/sysinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 # Public functions
 ########################################################################
 
 ###########################
 # executeAction() function
 ###########################
 
+
 # pylint: disable=W0613
 def executeAction(configPath, options, config):
     """
     Executes the sysinfo backup action.
 
     Args:
        configPath (String representing a path on disk): Path to configuration file on disk
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/filesystem.py` & `cedar_backup3-3.7.5/src/CedarBackup3/filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,14 @@
 
 ########################################################################
 # FilesystemList class definition
 ########################################################################
 
 
 class FilesystemList(list):
-
     ######################
     # Class documentation
     ######################
 
     """
     Represents a list of filesystem items.
 
@@ -762,15 +761,14 @@
 
 ########################################################################
 # BackupFileList class definition
 ########################################################################
 
 
 class BackupFileList(FilesystemList):  # pylint: disable=R0904
-
     ######################
     # Class documentation
     ######################
 
     """
     List of files to be backed up.
 
@@ -1249,15 +1247,14 @@
 
 ########################################################################
 # PurgeItemList class definition
 ########################################################################
 
 
 class PurgeItemList(FilesystemList):  # pylint: disable=R0904
-
     ######################
     # Class documentation
     ######################
 
     """
     List of files and directories to be purged.
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/image.py` & `cedar_backup3-3.7.5/src/CedarBackup3/image.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/knapsack.py` & `cedar_backup3-3.7.5/src/CedarBackup3/knapsack.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 
 ######################
 # firstFit() function
 ######################
 
 
 def firstFit(items, capacity):
-
     """
     Implements the first-fit knapsack algorithm.
 
     The first-fit algorithm proceeds through an unsorted list of items until
     running out of items or meeting capacity exactly.  If capacity is exceeded,
     the item that caused capacity to be exceeded is thrown away and the next one
     is tried.  This algorithm generally performs more poorly than the other
@@ -127,15 +126,14 @@
 
 #####################
 # bestFit() function
 #####################
 
 
 def bestFit(items, capacity):
-
     """
     Implements the best-fit knapsack algorithm.
 
     The best-fit algorithm proceeds through a sorted list of items (sorted from
     largest to smallest) until running out of items or meeting capacity exactly.
     If capacity is exceeded, the item that caused capacity to be exceeded is
     thrown away and the next one is tried.  The algorithm effectively includes
@@ -197,15 +195,14 @@
 
 ######################
 # worstFit() function
 ######################
 
 
 def worstFit(items, capacity):
-
     """
     Implements the worst-fit knapsack algorithm.
 
     The worst-fit algorithm proceeds through an a sorted list of items (sorted
     from smallest to largest) until running out of items or meeting capacity
     exactly.  If capacity is exceeded, the item that caused capacity to be
     exceeded is thrown away and the next one is tried.  The algorithm
@@ -265,15 +262,14 @@
 
 ##########################
 # alternateFit() function
 ##########################
 
 
 def alternateFit(items, capacity):
-
     """
     Implements the alternate-fit knapsack algorithm.
 
     This algorithm (which I'm calling "alternate-fit" as in "alternate from one
     to the other") tries to balance small and large items to achieve better
     end-of-disk performance.  Instead of just working one direction through a
     list, it alternately works from the start and end of a sorted list (sorted
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/peer.py` & `cedar_backup3-3.7.5/src/CedarBackup3/peer.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 
 ########################################################################
 # LocalPeer class definition
 ########################################################################
 
 
 class LocalPeer(object):
-
     ######################
     # Class documentation
     ######################
 
     """
     Backup peer representing a local peer in a backup pool.
 
@@ -395,15 +394,14 @@
 
 ########################################################################
 # RemotePeer class definition
 ########################################################################
 
 
 class RemotePeer(object):
-
     ######################
     # Class documentation
     ######################
 
     """
     Backup peer representing a remote peer in a backup pool.
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/release.py` & `cedar_backup3-3.7.5/src/CedarBackup3/release.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/scripts.py` & `cedar_backup3-3.7.5/src/CedarBackup3/scripts.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/testutil.py` & `cedar_backup3-3.7.5/src/CedarBackup3/testutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,14 +349,15 @@
     return "%s%s%s" % (prefix, "".join(characters), suffix)
 
 
 ####################################
 # failUnlessAssignRaises() function
 ####################################
 
+
 # pylint: disable=W0613
 def failUnlessAssignRaises(testCase, exception, obj, prop, value):
     """
     Equivalent of ``failUnlessRaises``, but used for property assignments instead.
 
     It's nice to be able to use ``failUnlessRaises`` to check that a method call
     raises the exception that you expect.  Unfortunately, this method can't be
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/tools/__init__.py` & `cedar_backup3-3.7.5/src/CedarBackup3/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/tools/amazons3.py` & `cedar_backup3-3.7.5/src/CedarBackup3/tools/amazons3.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,14 @@
 #######################################################################
 # Options class
 #######################################################################
 
 
 @total_ordering
 class Options(object):
-
     ######################
     # Class documentation
     ######################
 
     """
     Class representing command-line options for the cback3-amazons3-sync script.
 
@@ -1101,14 +1100,15 @@
     return sourceFiles
 
 
 ###############################
 # _checkSourceFiles() function
 ###############################
 
+
 # pylint: disable=W0613
 def _checkSourceFiles(sourceDir, sourceFiles):
     """
     Check source files, trying to guess which ones will have encoding problems.
     Args:
        sourceDir: Local source directory
        sourceDir: Local source directory
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/tools/span.py` & `cedar_backup3-3.7.5/src/CedarBackup3/tools/span.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,14 +305,15 @@
     fd.write("\n")
 
 
 ############################
 # _executeAction() function
 ############################
 
+
 # pylint: disable=W0613
 def _executeAction(options, config):
     """
     Implements the guts of the cback3-span tool.
 
     Args:
        options (SpanOptions object): Program command-line options
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/util.py` & `cedar_backup3-3.7.5/src/CedarBackup3/util.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/writer.py` & `cedar_backup3-3.7.5/src/CedarBackup3/writer.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/writers/__init__.py` & `cedar_backup3-3.7.5/src/CedarBackup3/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/writers/cdwriter.py` & `cedar_backup3-3.7.5/src/CedarBackup3/writers/cdwriter.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,14 @@
 
 ########################################################################
 # CdWriter class definition
 ########################################################################
 
 
 class CdWriter(object):
-
     ######################
     # Class documentation
     ######################
 
     """
     Class representing a device that knows how to write CD media.
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/writers/dvdwriter.py` & `cedar_backup3-3.7.5/src/CedarBackup3/writers/dvdwriter.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,14 @@
 
 ########################################################################
 # DvdWriter class definition
 ########################################################################
 
 
 class DvdWriter(object):
-
     ######################
     # Class documentation
     ######################
 
     """
     Class representing a device that knows how to write some kinds of DVD media.
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/writers/util.py` & `cedar_backup3-3.7.5/src/CedarBackup3/writers/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,14 @@
 
 ########################################################################
 # IsoImage class definition
 ########################################################################
 
 
 class IsoImage(object):
-
     ######################
     # Class documentation
     ######################
 
     """
     Represents an ISO filesystem image.
```

### Comparing `cedar_backup3-3.7.4/src/CedarBackup3/xmlutil.py` & `cedar_backup3-3.7.5/src/CedarBackup3/xmlutil.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/__init__.py` & `cedar_backup3-3.7.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/cback.conf.1` & `cedar_backup3-3.7.5/tests/data/cback.conf.1`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/cback.conf.10` & `cedar_backup3-3.7.5/tests/data/cback.conf.10`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/cback.conf.12` & `cedar_backup3-3.7.5/tests/data/cback.conf.12`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/cback.conf.15` & `cedar_backup3-3.7.5/tests/data/cback.conf.15`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/cback.conf.19` & `cedar_backup3-3.7.5/tests/data/cback.conf.19`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/cback.conf.20` & `cedar_backup3-3.7.5/tests/data/cback.conf.20`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/cback.conf.21` & `cedar_backup3-3.7.5/tests/data/cback.conf.21`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/cback.conf.23` & `cedar_backup3-3.7.5/tests/data/cback.conf.23`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/cback.conf.6` & `cedar_backup3-3.7.5/tests/data/cback.conf.6`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/cback.conf.8` & `cedar_backup3-3.7.5/tests/data/cback.conf.8`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/lotsoflines.py` & `cedar_backup3-3.7.5/tests/data/lotsoflines.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/mbox.conf.4` & `cedar_backup3-3.7.5/tests/data/mbox.conf.4`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/subversion.conf.4` & `cedar_backup3-3.7.5/tests/data/subversion.conf.4`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/subversion.conf.7` & `cedar_backup3-3.7.5/tests/data/subversion.conf.7`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree1.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree1.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree11.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree11.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree12.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree12.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree15.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree15.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree16.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree16.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree17.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree17.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree18.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree18.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree19.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree19.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree20.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree20.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree21.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree21.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree22.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree22.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree3.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree3.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree4.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree4.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree5.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree5.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree6.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree6.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/data/tree9.tar.gz` & `cedar_backup3-3.7.5/tests/data/tree9.tar.gz`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_actions_util.py` & `cedar_backup3-3.7.5/tests/test_actions_util.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_amazons3.py` & `cedar_backup3-3.7.5/tests/test_amazons3.py`

 * *Files 0% similar despite different names*

```diff
@@ -912,15 +912,14 @@
 
 #################
 # TestTool class
 #################
 
 
 class TestTool(unittest.TestCase):
-
     ################
     # Setup methods
     ################
 
     @classmethod
     def setUpClass(cls):
         configureLogging()
```

### Comparing `cedar_backup3-3.7.4/tests/test_capacity.py` & `cedar_backup3-3.7.5/tests/test_capacity.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_cdwriter.py` & `cedar_backup3-3.7.5/tests/test_cdwriter.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_cli.py` & `cedar_backup3-3.7.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_config.py` & `cedar_backup3-3.7.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_customize.py` & `cedar_backup3-3.7.5/tests/test_customize.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_dvdwriter.py` & `cedar_backup3-3.7.5/tests/test_dvdwriter.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_encrypt.py` & `cedar_backup3-3.7.5/tests/test_encrypt.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_filesystem.py` & `cedar_backup3-3.7.5/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_knapsack.py` & `cedar_backup3-3.7.5/tests/test_knapsack.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_mbox.py` & `cedar_backup3-3.7.5/tests/test_mbox.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_mysql.py` & `cedar_backup3-3.7.5/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_peer.py` & `cedar_backup3-3.7.5/tests/test_peer.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_postgresql.py` & `cedar_backup3-3.7.5/tests/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_span.py` & `cedar_backup3-3.7.5/tests/test_span.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_split.py` & `cedar_backup3-3.7.5/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_subversion.py` & `cedar_backup3-3.7.5/tests/test_subversion.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_sync.py` & `cedar_backup3-3.7.5/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_util.py` & `cedar_backup3-3.7.5/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/tests/test_writers_util.py` & `cedar_backup3-3.7.5/tests/test_writers_util.py`

 * *Files identical despite different names*

### Comparing `cedar_backup3-3.7.4/setup.py` & `cedar_backup3-3.7.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,69 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cedar-backup3
+Version: 3.7.5
+Summary: Implements local and remote backups to CD/DVD and Amazon S3
+Home-page: https://pypi.org/project/cedar-backup3/
+License: GPL-2.0-only
+Keywords: local,remote,backup,scp
+Author: Kenneth J. Pronovici
+Author-email: pronovic@ieee.org
+Requires-Python: >=3.8,<4
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: System :: Archiving :: Backup
+Classifier: Topic :: Utilities
+Provides-Extra: docs
+Requires-Dist: chardet (>=5.1.0,<6.0.0)
+Requires-Dist: importlib-metadata (>=6.0.0,<7.0.0)
+Requires-Dist: sphinx (>=6.1.3,<7.0.0) ; extra == "docs"
+Requires-Dist: sphinx-autoapi (>=2.0.1,<3.0.0) ; extra == "docs"
+Project-URL: Repository, https://github.com/pronovic/cedar-backup3
+Description-Content-Type: text/markdown
+
+[![pypi](https://img.shields.io/pypi/v/cedar-backup3.svg)](https://pypi.org/project/cedar-backup3/)
+[![license](https://img.shields.io/pypi/l/cedar-backup3.svg)](https://github.com/pronovic/cedar-backup3/blob/master/LICENSE)
+[![wheel](https://img.shields.io/pypi/wheel/cedar-backup3.svg)](https://pypi.org/project/cedar-backup3/)
+[![python](https://img.shields.io/pypi/pyversions/cedar-backup3.svg)](https://pypi.org/project/cedar-backup3/)
+[![Test Suite](https://github.com/pronovic/cedar-backup3/workflows/Test%20Suite/badge.svg)](https://github.com/pronovic/cedar-backup3/actions?query=workflow%3A%22Test+Suite%22)
+[![docs](https://readthedocs.org/projects/cedar-backup3/badge/?version=stable&style=flat)](https://cedar-backup3.readthedocs.io/en/stable/)
+[![coverage](https://coveralls.io/repos/github/pronovic/cedar-backup3/badge.svg?branch=master)](https://coveralls.io/github/pronovic/cedar-backup3?branch=master)
+
+[Cedar Backup](https://github.com/pronovic/cedar-backup3) is a software package
+designed to manage system backups for a pool of local and remote machines.
+Cedar Backup understands how to back up filesystem data as well as MySQL and
+PostgreSQL databases and Subversion repositories.  It can also be easily
+extended to support other kinds of data sources.
+
+Cedar Backup is focused around weekly backups to a single CD or DVD disc,
+with the expectation that the disc will be changed or overwritten at the
+beginning of each week.  If your hardware is new enough, Cedar Backup can
+write multisession discs, allowing you to add incremental data to a disc on
+a daily basis.  Alternately, Cedar Backup can write your backups to the Amazon
+S3 cloud rather than relying on physical media.  See 
+the [Cedar Backup v3 Software Manual](https://cedar-backup3.readthedocs.io/en/stable/manual/index.html) for details.
+
+Besides offering command-line utilities to manage the backup process, Cedar
+Backup provides a well-organized library of backup-related functionality.
+For more information, see 
+the [API Reference](https://cedar-backup3.readthedocs.io/en/stable/autoapi/index.html).
+
+There are many different backup software systems in the open source world.
+Cedar Backup aims to fill a niche: it aims to be a good fit for people who need
+to back up a limited amount of important data on a regular basis. Cedar Backup
+isn’t for you if you want to back up your huge MP3 collection every night, or
+if you want to back up a few hundred machines.  However, if you administer a
+small set of machines and you want to run daily incremental backups for things
+like system configuration, current email, small web sites, source code
+repositories, or small databases, then Cedar Backup is probably worth your
+time.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['CedarBackup3',
- 'CedarBackup3.actions',
- 'CedarBackup3.extend',
- 'CedarBackup3.tools',
- 'CedarBackup3.writers']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['chardet>=4.0.0,<5.0.0', 'importlib-metadata>=5.2.0,<6.0.0']
-
-extras_require = \
-{'docs': ['sphinx>=4.5.0,<5.0.0', 'sphinx-autoapi>=1.8.4,<2.0.0']}
-
-entry_points = \
-{'console_scripts': ['cback3 = CedarBackup3.scripts:cback3',
-                     'cback3-amazons3-sync = CedarBackup3.scripts:amazons3',
-                     'cback3-span = CedarBackup3.scripts:span']}
-
-setup_kwargs = {
-    'name': 'cedar-backup3',
-    'version': '3.7.4',
-    'description': 'Implements local and remote backups to CD/DVD and Amazon S3',
-    'long_description': '[![pypi](https://img.shields.io/pypi/v/cedar-backup3.svg)](https://pypi.org/project/cedar-backup3/)\n[![license](https://img.shields.io/pypi/l/cedar-backup3.svg)](https://github.com/pronovic/cedar-backup3/blob/master/LICENSE)\n[![wheel](https://img.shields.io/pypi/wheel/cedar-backup3.svg)](https://pypi.org/project/cedar-backup3/)\n[![python](https://img.shields.io/pypi/pyversions/cedar-backup3.svg)](https://pypi.org/project/cedar-backup3/)\n[![Test Suite](https://github.com/pronovic/cedar-backup3/workflows/Test%20Suite/badge.svg)](https://github.com/pronovic/cedar-backup3/actions?query=workflow%3A%22Test+Suite%22)\n[![docs](https://readthedocs.org/projects/cedar-backup3/badge/?version=stable&style=flat)](https://cedar-backup3.readthedocs.io/en/stable/)\n[![coverage](https://coveralls.io/repos/github/pronovic/cedar-backup3/badge.svg?branch=master)](https://coveralls.io/github/pronovic/cedar-backup3?branch=master)\n\n[Cedar Backup](https://github.com/pronovic/cedar-backup3) is a software package\ndesigned to manage system backups for a pool of local and remote machines.\nCedar Backup understands how to back up filesystem data as well as MySQL and\nPostgreSQL databases and Subversion repositories.  It can also be easily\nextended to support other kinds of data sources.\n\nCedar Backup is focused around weekly backups to a single CD or DVD disc,\nwith the expectation that the disc will be changed or overwritten at the\nbeginning of each week.  If your hardware is new enough, Cedar Backup can\nwrite multisession discs, allowing you to add incremental data to a disc on\na daily basis.  Alternately, Cedar Backup can write your backups to the Amazon\nS3 cloud rather than relying on physical media.  See \nthe [Cedar Backup v3 Software Manual](https://cedar-backup3.readthedocs.io/en/stable/manual/index.html) for details.\n\nBesides offering command-line utilities to manage the backup process, Cedar\nBackup provides a well-organized library of backup-related functionality.\nFor more information, see \nthe [API Reference](https://cedar-backup3.readthedocs.io/en/stable/autoapi/index.html).\n\nThere are many different backup software systems in the open source world.\nCedar Backup aims to fill a niche: it aims to be a good fit for people who need\nto back up a limited amount of important data on a regular basis. Cedar Backup\nisn’t for you if you want to back up your huge MP3 collection every night, or\nif you want to back up a few hundred machines.  However, if you administer a\nsmall set of machines and you want to run daily incremental backups for things\nlike system configuration, current email, small web sites, source code\nrepositories, or small databases, then Cedar Backup is probably worth your\ntime.\n',
-    'author': 'Kenneth J. Pronovici',
-    'author_email': 'pronovic@ieee.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://pypi.org/project/cedar-backup3/',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4',
-}
-
-
-setup(**setup_kwargs)
```

