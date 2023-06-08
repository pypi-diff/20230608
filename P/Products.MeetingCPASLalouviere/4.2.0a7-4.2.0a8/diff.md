# Comparing `tmp/Products.MeetingCPASLalouviere-4.2.0a7.tar.gz` & `tmp/Products.MeetingCPASLalouviere-4.2.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.MeetingCPASLalouviere-4.2.0a7.tar", last modified: Mon Jun  5 13:50:37 2023, max compression
+gzip compressed data, was "Products.MeetingCPASLalouviere-4.2.0a8.tar", last modified: Thu Jun  8 14:15:08 2023, max compression
```

## Comparing `Products.MeetingCPASLalouviere-4.2.0a7.tar` & `Products.MeetingCPASLalouviere-4.2.0a8.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.948615 Products.MeetingCPASLalouviere-4.2.0a7/
--rw-rw-r--   0 oli       (1000) oli       (1000)     3432 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/CHANGES.rst
--rw-rw-r--   0 oli       (1000) oli       (1000)      353 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/MANIFEST.in
--rw-rw-r--   0 oli       (1000) oli       (1000)     4072 2023-06-05 13:50:37.948615 Products.MeetingCPASLalouviere-4.2.0a7/PKG-INFO
--rw-rw-r--   0 oli       (1000) oli       (1000)       23 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/README.rst
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.936615 Products.MeetingCPASLalouviere-4.2.0a7/docs/
--rw-rw-r--   0 oli       (1000) oli       (1000)    18092 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/docs/LICENSE.GPL
--rw-rw-r--   0 oli       (1000) oli       (1000)      734 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/docs/LICENSE.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)     1121 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/docs/MIGRATION.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)       38 2023-06-05 13:50:37.948615 Products.MeetingCPASLalouviere-4.2.0a7/setup.cfg
--rw-rw-r--   0 oli       (1000) oli       (1000)     1248 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/setup.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.932615 Products.MeetingCPASLalouviere-4.2.0a7/src/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.936615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.936615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/
--rw-rw-r--   0 oli       (1000) oli       (1000)      981 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/README.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)     1773 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)    14191 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/adapters.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.936615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/browser/
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/browser/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/browser/configure.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)      120 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/browser/overrides.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      805 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/browser/views.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     3203 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/config.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      724 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/configure.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)      615 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/events.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     3719 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/interfaces.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.936615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/
--rw-rw-r--   0 oli       (1000) oli       (1000)     1794 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/PloneMeeting.pot
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.936615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/en/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.936615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/
--rw-rw-r--   0 oli       (1000) oli       (1000)     1206 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 oli       (1000) oli       (1000)     2089 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/plone.po
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.936615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/fr/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.936615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 oli       (1000) oli       (1000)     2227 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 oli       (1000) oli       (1000)     2939 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 oli       (1000) oli       (1000)     1970 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/plone.pot
--rwxrwxr-x   0 oli       (1000) oli       (1000)      267 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/sync_pos.sh
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.936615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/migrations/
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/migrations/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)    15699 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/migrations/migrate_to_4200.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.936615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/model/
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/model/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1627 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/model/pm_updates.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      946 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/overrides.zcml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.936615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/
--rw-rw-r--   0 oli       (1000) oli       (1000)       23 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/__init__.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.940615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/
--rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/MeetingCPASLalouviere_marker.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      768 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/cssregistry.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      824 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/import_steps.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      423 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/jsregistry.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      246 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/metadata.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      601 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/rolemap.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      999 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/skins.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      167 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/toolset.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      931 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/workflows.xml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.940615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/
--rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/MeetingCPASLalouviere_testing_marker.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/__init__.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.940615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/
--rw-rw-r--   0 oli       (1000) oli       (1000)     3352 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/attach.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      630 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/budget.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      492 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/budgetAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      731 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/cahier.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/decisionAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      742 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/financialAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/itemAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      332 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/legalAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      411 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/negative.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      880 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/overheadAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     1147 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/positive.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      355 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/remarks.png
--rwxrwxr-x   0 oli       (1000) oli       (1000)     2669 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/import_data.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)      361 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/import_steps.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      180 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/metadata.xml
--rwxrwxr-x   0 oli       (1000) oli       (1000)      167 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/toolset.xml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.940615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/
--rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/MeetingCPASLalouviere_lalouviere_marker.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/__init__.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.940615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/
--rw-rw-r--   0 oli       (1000) oli       (1000)     3352 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/attach.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      630 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/budget.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      492 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/budgetAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     1032 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.gif
--rw-rw-r--   0 oli       (1000) oli       (1000)      731 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/decisionAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      742 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/financialAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/itemAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      761 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/legalAdvice.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      332 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/legalAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     3555 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/logo.gif
--rw-rw-r--   0 oli       (1000) oli       (1000)      885 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/negative.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      305 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/nil.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      880 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/overheadAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      583 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/positive.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      705 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/remarks.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      730 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/secretary_remarks.png
--rwxrwxr-x   0 oli       (1000) oli       (1000)     2192 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_data.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)     1015 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_steps.xml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.944615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/
--rw-rw-r--   0 oli       (1000) oli       (1000)     9511 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)     9909 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib_recto_verso.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)     9605 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_pv.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12386 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendance-stats.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    17906 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendees.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    18256 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/avis-df.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    22380 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-oj.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    22958 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-pv.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12890 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-rapport.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    13154 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/dashboard.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    32698 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    32449 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation_recto_verso.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)     9652 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/history.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12705 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/meeting_assemblies.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    24785 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-annexes.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    24316 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-table-des-matieres.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    24585 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12170 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/organizations-export.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    16342 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/publications.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    23881 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/pv.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12630 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    11565 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    13706 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/report.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    10369 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles1.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12815 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles2.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    18137 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-avis-df.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    14290 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-df-tb.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    13865 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/users-groups-export.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    14862 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/votes.odt
--rwxrwxr-x   0 oli       (1000) oli       (1000)      167 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/toolset.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)     1361 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/refresh.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)     4388 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/setuphandlers.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.936615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.944615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/
--rw-rw-r--   0 oli       (1000) oli       (1000)      329 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/ask_advices_by_itemcreator.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToPresented.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN1.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN2.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToPresident.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToSecretaire.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     6337 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      343 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/cdld.gif
--rw-rw-r--   0 oli       (1000) oli       (1000)      737 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToBudgetImpactReviewer.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      638 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN1.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      608 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN2.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      626 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToPresident.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      626 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToSecretaire.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      610 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/validate.png
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.944615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/
--rw-rw-r--   0 oli       (1000) oli       (1000)     1557 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/imioapps_properties.props
--rw-rw-r--   0 oli       (1000) oli       (1000)     1425 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/meetingcpaslalouviere.css
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.944615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/
--rw-rw-r--   0 oli       (1000) oli       (1000)     7737 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/meetingitem_edit.pt
--rw-rw-r--   0 oli       (1000) oli       (1000)    40254 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/meetingitem_view.pt
--rw-rw-r--   0 oli       (1000) oli       (1000)     1044 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/testing.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      624 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/testing.zcml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.948615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/
--rwxrwxr-x   0 oli       (1000) oli       (1000)     1447 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/MeetingCPASLalouviereTestCase.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1293 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     4864 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/helpers.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1392 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testAdvices.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1259 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testAnnexes.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1362 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testChangeItemOrderView.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1253 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testColumns.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1298 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testContacts.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)      537 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testCustomMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1281 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingConfig.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1351 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingItem.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      365 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testCustomSearches.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1376 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testCustomToolPloneMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1318 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testCustomUtils.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      506 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testCustomViews.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      497 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testCustomWFAdaptations.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1365 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testCustomWorkflows.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1286 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testFaceted.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1311 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1339 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testMeetingCategory.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     4834 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testMeetingConfig.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)     1729 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testMeetingItem.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1299 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testPortlets.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     9198 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testSearches.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1290 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testSetup.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1344 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testToolPloneMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     2862 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testUtils.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1302 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testValidators.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1248 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testViews.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1246 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testVotes.py
--rw-rw-r--   0 oli       (1000) oli       (1000)    17692 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testWFAdaptations.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)     7170 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testWorkflows.py
--rw-rw-r--   0 oli       (1000) oli       (1000)       11 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/version.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)       56 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products/__init__.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-06-05 13:50:37.936615 Products.MeetingCPASLalouviere-4.2.0a7/src/Products.MeetingCPASLalouviere.egg-info/
--rw-rw-r--   0 oli       (1000) oli       (1000)     4072 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products.MeetingCPASLalouviere.egg-info/PKG-INFO
--rw-rw-r--   0 oli       (1000) oli       (1000)    12099 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products.MeetingCPASLalouviere.egg-info/SOURCES.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        1 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products.MeetingCPASLalouviere.egg-info/dependency_links.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        9 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products.MeetingCPASLalouviere.egg-info/namespace_packages.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        1 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products.MeetingCPASLalouviere.egg-info/not-zip-safe
--rw-rw-r--   0 oli       (1000) oli       (1000)      139 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products.MeetingCPASLalouviere.egg-info/requires.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        9 2023-06-05 13:50:37.000000 Products.MeetingCPASLalouviere-4.2.0a7/src/Products.MeetingCPASLalouviere.egg-info/top_level.txt
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.387099 Products.MeetingCPASLalouviere-4.2.0a8/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3587 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/CHANGES.rst
+-rw-rw-r--   0 adu       (1000) adu       (1000)      353 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/MANIFEST.in
+-rw-rw-r--   0 adu       (1000) adu       (1000)     4227 2023-06-08 14:15:08.387099 Products.MeetingCPASLalouviere-4.2.0a8/PKG-INFO
+-rw-rw-r--   0 adu       (1000) adu       (1000)       23 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/README.rst
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.371099 Products.MeetingCPASLalouviere-4.2.0a8/docs/
+-rw-rw-r--   0 adu       (1000) adu       (1000)    18092 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/docs/LICENSE.GPL
+-rw-rw-r--   0 adu       (1000) adu       (1000)      734 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/docs/LICENSE.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1121 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/docs/MIGRATION.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)       38 2023-06-08 14:15:08.387099 Products.MeetingCPASLalouviere-4.2.0a8/setup.cfg
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1248 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/setup.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.367099 Products.MeetingCPASLalouviere-4.2.0a8/src/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.371099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.371099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      981 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/README.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1773 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)    13135 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/adapters.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.375099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/browser/
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/browser/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/browser/configure.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      120 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/browser/overrides.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      805 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/browser/views.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3203 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/config.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      724 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/configure.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      615 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/events.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3719 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/interfaces.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.375099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1794 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/PloneMeeting.pot
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.367099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/en/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.375099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1206 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2089 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/plone.po
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.367099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/fr/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.375099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2219 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2939 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1970 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/plone.pot
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      267 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/sync_pos.sh
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.375099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/migrations/
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/migrations/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)    15699 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/migrations/migrate_to_4200.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.375099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/model/
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/model/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1627 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/model/pm_updates.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      946 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/overrides.zcml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.375099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/
+-rw-rw-r--   0 adu       (1000) adu       (1000)       23 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.375099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/MeetingCPASLalouviere_marker.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      768 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/cssregistry.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      824 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/import_steps.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      423 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/jsregistry.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      246 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/metadata.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      601 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/rolemap.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      999 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/skins.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      167 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/toolset.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      931 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/workflows.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.375099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/MeetingCPASLalouviere_testing_marker.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.379099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3352 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/attach.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/budget.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      492 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/budgetAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      731 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/cahier.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/decisionAnnex.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      742 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/financialAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/itemAnnex.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      332 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/legalAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      411 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/negative.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      880 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/overheadAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1147 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/positive.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      355 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/remarks.png
+-rwxrwxr-x   0 adu       (1000) adu       (1000)     2669 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/import_data.py
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      361 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/import_steps.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      180 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/metadata.xml
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      167 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/toolset.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.379099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/MeetingCPASLalouviere_lalouviere_marker.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.379099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3352 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/attach.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/budget.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      492 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/budgetAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1032 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.gif
+-rw-rw-r--   0 adu       (1000) adu       (1000)      731 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/decisionAnnex.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      742 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/financialAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/itemAnnex.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      761 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/legalAdvice.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      332 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/legalAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3555 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/logo.gif
+-rw-rw-r--   0 adu       (1000) adu       (1000)      885 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/negative.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      305 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/nil.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      880 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/overheadAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      583 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/positive.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      705 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/remarks.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      730 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/secretary_remarks.png
+-rwxrwxr-x   0 adu       (1000) adu       (1000)     2192 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_data.py
+-rwxrwxr-x   0 adu       (1000) adu       (1000)     1015 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_steps.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.383099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     9511 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     9909 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib_recto_verso.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     9605 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_pv.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    12386 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendance-stats.ods
+-rw-rw-r--   0 adu       (1000) adu       (1000)    17906 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendees.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    18256 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/avis-df.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    22380 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-oj.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    22958 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-pv.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    12890 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-rapport.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    13154 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/dashboard.ods
+-rw-rw-r--   0 adu       (1000) adu       (1000)    32698 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    32449 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation_recto_verso.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     9652 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/history.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    12705 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/meeting_assemblies.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    24785 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-annexes.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    24316 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-table-des-matieres.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    24585 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    12170 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/organizations-export.ods
+-rw-rw-r--   0 adu       (1000) adu       (1000)    16342 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/publications.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    23881 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/pv.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    12630 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.ods
+-rw-rw-r--   0 adu       (1000) adu       (1000)    11565 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    13706 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/report.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    10369 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles1.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    12815 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles2.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    18137 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-avis-df.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    14290 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-df-tb.ods
+-rw-rw-r--   0 adu       (1000) adu       (1000)    13865 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/users-groups-export.ods
+-rw-rw-r--   0 adu       (1000) adu       (1000)    14862 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/votes.odt
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      167 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/toolset.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1361 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/refresh.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     4388 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/setuphandlers.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.371099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.383099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      329 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/ask_advices_by_itemcreator.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToPresented.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN1.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN2.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToPresident.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToSecretaire.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     6337 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      343 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/cdld.gif
+-rw-rw-r--   0 adu       (1000) adu       (1000)      737 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToBudgetImpactReviewer.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      638 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN1.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      608 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN2.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      626 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToPresident.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      626 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToSecretaire.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      610 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/validate.png
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.383099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1557 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/imioapps_properties.props
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1425 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/meetingcpaslalouviere.css
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.387099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     7737 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/meetingitem_edit.pt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    40254 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/meetingitem_view.pt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1044 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/testing.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      624 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/testing.zcml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.387099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/
+-rwxrwxr-x   0 adu       (1000) adu       (1000)     1447 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/MeetingCPASLalouviereTestCase.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1293 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     4864 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/helpers.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1392 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testAdvices.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1259 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testAnnexes.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1362 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testChangeItemOrderView.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1253 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testColumns.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1298 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testContacts.py
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      537 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testCustomMeeting.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1281 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingConfig.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1351 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingItem.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      365 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testCustomSearches.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1376 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testCustomToolPloneMeeting.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1318 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testCustomUtils.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      506 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testCustomViews.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      497 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testCustomWFAdaptations.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1365 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testCustomWorkflows.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1286 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testFaceted.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1311 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testMeeting.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1339 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testMeetingCategory.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     4834 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testMeetingConfig.py
+-rwxrwxr-x   0 adu       (1000) adu       (1000)     1729 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testMeetingItem.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1299 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testPortlets.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     9198 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testSearches.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1290 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testSetup.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1344 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testToolPloneMeeting.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2862 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testUtils.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1302 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testValidators.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1248 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testViews.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1246 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testVotes.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)    17692 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testWFAdaptations.py
+-rwxrwxr-x   0 adu       (1000) adu       (1000)     7170 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testWorkflows.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)       11 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/version.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)       56 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-06-08 14:15:08.371099 Products.MeetingCPASLalouviere-4.2.0a8/src/Products.MeetingCPASLalouviere.egg-info/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     4227 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products.MeetingCPASLalouviere.egg-info/PKG-INFO
+-rw-rw-r--   0 adu       (1000) adu       (1000)    12099 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products.MeetingCPASLalouviere.egg-info/SOURCES.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        1 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products.MeetingCPASLalouviere.egg-info/dependency_links.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        9 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products.MeetingCPASLalouviere.egg-info/namespace_packages.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        1 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products.MeetingCPASLalouviere.egg-info/not-zip-safe
+-rw-rw-r--   0 adu       (1000) adu       (1000)      139 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products.MeetingCPASLalouviere.egg-info/requires.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        9 2023-06-08 14:15:08.000000 Products.MeetingCPASLalouviere-4.2.0a8/src/Products.MeetingCPASLalouviere.egg-info/top_level.txt
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/CHANGES.rst` & `Products.MeetingCPASLalouviere-4.2.0a8/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 Products.MeetingCPASLalouviere Changelog
 ====================================
 
 The Products.MeetingCommunes version must be the same as the Products.PloneMeeting version
 
+4.2.0a8 (2023-06-08)
+--------------------
+
+- SUP-30699. Adapt translation.
+  [aduchene]
+- SUP-30700. Adapt LLO_WAITING_ADVICES_FROM_STATES.
+  [aduchene]
+
+
 4.2.0a7 (2023-06-05)
 --------------------
 
 - Fix AttributeError: onTransitionFieldTransforms/transition.
   [odelaere]
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/PKG-INFO` & `Products.MeetingCPASLalouviere-4.2.0a8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingCPASLalouviere
-Version: 4.2.0a7
+Version: 4.2.0a8
 Summary: PloneMeeting profile for CPAS of La Louviere.
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Olivier Delaere
 Author-email: olivier.delaere@imio.be
 License: GPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -18,14 +18,23 @@
 
 Check 'docs/README.txt'
 Products.MeetingCPASLalouviere Changelog
 ====================================
 
 The Products.MeetingCommunes version must be the same as the Products.PloneMeeting version
 
+4.2.0a8 (2023-06-08)
+--------------------
+
+- SUP-30699. Adapt translation.
+  [aduchene]
+- SUP-30700. Adapt LLO_WAITING_ADVICES_FROM_STATES.
+  [aduchene]
+
+
 4.2.0a7 (2023-06-05)
 --------------------
 
 - Fix AttributeError: onTransitionFieldTransforms/transition.
   [odelaere]
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/docs/LICENSE.GPL` & `Products.MeetingCPASLalouviere-4.2.0a8/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/docs/LICENSE.txt` & `Products.MeetingCPASLalouviere-4.2.0a8/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/docs/MIGRATION.txt` & `Products.MeetingCPASLalouviere-4.2.0a8/docs/MIGRATION.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/setup.py` & `Products.MeetingCPASLalouviere-4.2.0a8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "4.2.0a7"
+version = "4.2.0a8"
 
 setup(name='Products.MeetingCPASLalouviere',
       version=version,
       description="PloneMeeting profile for CPAS of La Louviere.",
       long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
       classifiers=[
           "Environment :: Web Environment",
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/README.txt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/README.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/__init__.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/adapters.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/adapters.py`

 * *Files 10% similar despite different names*

```diff
@@ -302,30 +302,10 @@
          'use_custom_state_title': False,
          'use_custom_transition_title_for': {},
          'remove_modify_access': True,
          'adviser_may_validate': True,
          # must end with _waiting_advices
          'new_state_id': None,
          },
-        {'from_states': ('proposed_to_president', ),
-         'back_states': ('proposed_to_president', ),
-         'perm_cloned_state': 'validated',
-         'use_custom_icon': False,
-         # default to "validated", this avoid using the backToValidated title that
-         # is translated to "Remove from meeting"
-         'use_custom_back_transition_title_for': ("validated", ),
-         # we can define some back transition id for some back_to_state
-         # if not, a generated transition is used, here we could have for example
-         # 'defined_back_transition_ids': {"validated": "validate"}
-         'defined_back_transition_ids': {},
-         # if () given, a custom transition icon is used for every back transitions
-         'only_use_custom_back_transition_icon_for': ("validated", ),
-         'use_custom_state_title': True,
-         'use_custom_transition_title_for': {},
-         'remove_modify_access': True,
-         'adviser_may_validate': False,
-         # must end with _waiting_advices
-         'new_state_id': None,
-         },
     ),
 }
 adaptations.WAITING_ADVICES_FROM_STATES.update(LLO_WAITING_ADVICES_FROM_STATES)
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/browser/views.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/browser/views.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/config.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/config.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/configure.zcml` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/events.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/events.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/interfaces.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/interfaces.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/PloneMeeting.pot` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/PloneMeeting.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/plone.po` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po`

 * *Files 4% similar despite different names*

```diff
@@ -66,16 +66,16 @@
 
 #. Default: "Items proposed to n+2"
 msgid "searchproposedton2"
 msgstr "Points proposés au N+2"
 
 #. Default: "Items proposed to ceo"
 msgid "searchproposedtosecretaire"
-msgstr "Points proposés au Secrétaire"
+msgstr "Points proposés au DG"
 
 #. Default: "Items proposed to president"
 msgid "searchproposedtopresident"
 msgstr "Points proposés au Président"
 
 #. Default: "Emergency Motivation"
 msgid "MeetingCPASLalouviere_label_emergencyMotivation"
-msgstr "Motivation de l'urgence"
+msgstr "Motivation de l'urgence"
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/plone.po` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/locales/plone.pot` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/migrations/migrate_to_4200.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/migrations/migrate_to_4200.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/model/pm_updates.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/model/pm_updates.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/overrides.zcml` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/overrides.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/cssregistry.xml` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/import_steps.xml` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/rolemap.xml` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/skins.xml` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/default/workflows.xml` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/attach.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/budget.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/cahier.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/financialAnalysis.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/overheadAnalysis.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/images/positive.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/testing/import_data.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/testing/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/attach.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/budget.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.gif` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/financialAnalysis.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/legalAdvice.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/logo.gif` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/logo.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/negative.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/overheadAnalysis.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/positive.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/remarks.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/secretary_remarks.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/images/secretary_remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_data.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_steps.xml` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib_recto_verso.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_delib_recto_verso.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_pv.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/all_pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendance-stats.ods` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendance-stats.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendees.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/attendees.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/avis-df.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/avis-df.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-oj.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-pv.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-rapport.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/council-rapport.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/dashboard.ods` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/dashboard.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation_recto_verso.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/deliberation_recto_verso.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/history.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/history.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/meeting_assemblies.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/meeting_assemblies.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-annexes.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-annexes.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-table-des-matieres.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj-avec-table-des-matieres.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/organizations-export.ods` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/organizations-export.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/publications.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/publications.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/pv.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.ods` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/recapitulatif-tb.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/report.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/report.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles1.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles1.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles2.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/styles2.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-avis-df.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-avis-df.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-df-tb.ods` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/synthese-df-tb.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/users-groups-export.ods` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/users-groups-export.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/votes.odt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles/zlalouvierecpas/templates/votes.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/profiles.zcml` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/profiles.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/setuphandlers.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToPresented.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToPresented.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN1.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN1.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN2.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToN2.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToPresident.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToPresident.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToSecretaire.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backToProposedToSecretaire.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToBudgetImpactReviewer.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToBudgetImpactReviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN1.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN1.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN2.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToN2.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToPresident.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToPresident.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToSecretaire.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/proposeToSecretaire.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/validate.png` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_images/validate.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/imioapps_properties.props` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/imioapps_properties.props`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/meetingcpaslalouviere.css` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_styles/meetingcpaslalouviere.css`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/meetingitem_edit.pt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/meetingitem_edit.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/meetingitem_view.pt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/skins/meetingcpaslalouviere_templates/meetingitem_view.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/testing.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/testing.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/testing.zcml` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/testing.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/MeetingCPASLalouviereTestCase.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/MeetingCPASLalouviereTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/__init__.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/helpers.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testAdvices.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testAdvices.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testAnnexes.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testAnnexes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testChangeItemOrderView.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testChangeItemOrderView.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testColumns.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testColumns.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testContacts.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testContacts.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testCustomMeeting.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testCustomMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingConfig.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingItem.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testCustomMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testCustomToolPloneMeeting.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testCustomToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testCustomUtils.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testCustomUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testCustomWorkflows.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testCustomWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testFaceted.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testFaceted.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testMeeting.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testMeetingCategory.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testMeetingCategory.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testMeetingConfig.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testMeetingItem.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testPortlets.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testPortlets.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testSearches.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testSearches.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testSetup.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testSetup.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testToolPloneMeeting.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testUtils.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testValidators.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testValidators.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testViews.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testViews.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testVotes.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testVotes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testWFAdaptations.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testWFAdaptations.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products/MeetingCPASLalouviere/tests/testWorkflows.py` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products/MeetingCPASLalouviere/tests/testWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products.MeetingCPASLalouviere.egg-info/PKG-INFO` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products.MeetingCPASLalouviere.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingCPASLalouviere
-Version: 4.2.0a7
+Version: 4.2.0a8
 Summary: PloneMeeting profile for CPAS of La Louviere.
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Olivier Delaere
 Author-email: olivier.delaere@imio.be
 License: GPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -18,14 +18,23 @@
 
 Check 'docs/README.txt'
 Products.MeetingCPASLalouviere Changelog
 ====================================
 
 The Products.MeetingCommunes version must be the same as the Products.PloneMeeting version
 
+4.2.0a8 (2023-06-08)
+--------------------
+
+- SUP-30699. Adapt translation.
+  [aduchene]
+- SUP-30700. Adapt LLO_WAITING_ADVICES_FROM_STATES.
+  [aduchene]
+
+
 4.2.0a7 (2023-06-05)
 --------------------
 
 - Fix AttributeError: onTransitionFieldTransforms/transition.
   [odelaere]
```

### Comparing `Products.MeetingCPASLalouviere-4.2.0a7/src/Products.MeetingCPASLalouviere.egg-info/SOURCES.txt` & `Products.MeetingCPASLalouviere-4.2.0a8/src/Products.MeetingCPASLalouviere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

