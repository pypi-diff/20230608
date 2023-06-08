# Comparing `tmp/odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8-py2-none-any.whl.zip` & `tmp/odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9-py2-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,43 +1,78 @@
-Zip file size: 43699 bytes, number of entries: 41
--rw-r--r--  2.0 unx      320 b- defN 16-Oct-10 20:45 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8-py2.7-nspkg.pth
--rw-r--r--  2.0 unx     1329 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/__openerp__.py
+Zip file size: 78780 bytes, number of entries: 76
+-rw-r--r--  2.0 unx      320 b- defN 16-Nov-30 03:41 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9-py2.7-nspkg.pth
+-rw-r--r--  2.0 unx       12 b- defN 16-Nov-30 03:41 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx       92 b- defN 16-Nov-30 03:41 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/WHEEL
+-rw-r--r--  2.0 unx     7994 b- defN 17-Apr-08 19:09 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/RECORD
+-rw-r--r--  2.0 unx      684 b- defN 17-Apr-08 19:09 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/metadata.json
+-rw-r--r--  2.0 unx     1811 b- defN 16-Nov-30 03:41 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/DESCRIPTION.rst
+-rw-r--r--  2.0 unx     2283 b- defN 17-Apr-08 19:09 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/METADATA
+-rw-r--r--  2.0 unx       12 b- defN 16-Nov-30 03:41 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx     1329 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/__openerp__.py
 -rw-r--r--  2.0 unx       46 b- defN 16-Apr-05 19:58 odoo_addons/purchase_order_type/__init__.py
 -rw-r--r--  2.0 unx     1809 b- defN 16-Apr-05 19:58 odoo_addons/purchase_order_type/README.rst
 -rw-r--r--  2.0 unx      316 b- defN 16-Apr-05 19:58 odoo_addons/purchase_order_type/security/ir.model.access.csv
 -rw-r--r--  2.0 unx      995 b- defN 16-Apr-05 19:58 odoo_addons/purchase_order_type/models/res_partner.py
 -rw-r--r--  2.0 unx     2004 b- defN 16-Apr-05 19:58 odoo_addons/purchase_order_type/models/purchase_order.py
 -rw-r--r--  2.0 unx     1523 b- defN 16-Apr-05 19:58 odoo_addons/purchase_order_type/models/purchase_order_type.py
 -rw-r--r--  2.0 unx      114 b- defN 16-Apr-05 19:58 odoo_addons/purchase_order_type/models/__init__.py
--rw-r--r--  2.0 unx     2669 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/zh_CN.po
--rw-r--r--  2.0 unx     2691 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/pt.po
--rw-r--r--  2.0 unx     3396 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/it.po
--rw-r--r--  2.0 unx     3450 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/es.po
--rw-r--r--  2.0 unx     2660 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/tr.po
--rw-r--r--  2.0 unx     2762 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/hr.po
--rw-r--r--  2.0 unx     2806 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/bg.po
--rw-r--r--  2.0 unx     2679 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/gl.po
--rw-r--r--  2.0 unx     2676 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/ca.po
--rw-r--r--  2.0 unx     4009 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/sl.po
--rw-r--r--  2.0 unx     2692 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/es_ES.po
--rw-r--r--  2.0 unx     2708 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/pt_PT.po
--rw-r--r--  2.0 unx     2658 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/nl.po
--rw-r--r--  2.0 unx     2677 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/am.po
--rw-r--r--  2.0 unx     3421 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/de.po
--rw-r--r--  2.0 unx     2878 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/fr.po
--rw-r--r--  2.0 unx     2870 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/pt_BR.po
--rw-r--r--  2.0 unx     2792 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/el_GR.po
--rw-r--r--  2.0 unx     2682 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/fi.po
--rw-r--r--  2.0 unx     2776 b- defN 16-Oct-10 20:45 odoo_addons/purchase_order_type/i18n/hr_HR.po
+-rw-r--r--  2.0 unx     2689 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/ja.po
+-rw-r--r--  2.0 unx     2718 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/lv.po
+-rw-r--r--  2.0 unx     2711 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/zh_CN.po
+-rw-r--r--  2.0 unx     2876 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/uk.po
+-rw-r--r--  2.0 unx     2754 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/es_AR.po
+-rw-r--r--  2.0 unx     2699 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/ko.po
+-rw-r--r--  2.0 unx     2760 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/ru.po
+-rw-r--r--  2.0 unx     2623 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/gl_ES.po
+-rw-r--r--  2.0 unx     2735 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/pt.po
+-rw-r--r--  2.0 unx     2668 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/fr_CH.po
+-rw-r--r--  2.0 unx     3406 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/it.po
+-rw-r--r--  2.0 unx     3469 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/es.po
+-rw-r--r--  2.0 unx     2724 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/nl_BE.po
+-rw-r--r--  2.0 unx     2845 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/ar.po
+-rw-r--r--  2.0 unx     2808 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/lt.po
+-rw-r--r--  2.0 unx     2664 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/tr.po
+-rw-r--r--  2.0 unx     2832 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/mk.po
+-rw-r--r--  2.0 unx     2777 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/hr.po
+-rw-r--r--  2.0 unx     2842 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/bg.po
+-rw-r--r--  2.0 unx     2760 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/es_EC.po
+-rw-r--r--  2.0 unx     2705 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/zh_TW.po
+-rw-r--r--  2.0 unx     2622 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/fr_CA.po
+-rw-r--r--  2.0 unx     2700 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/gl.po
+-rw-r--r--  2.0 unx     2676 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/ca.po
+-rw-r--r--  2.0 unx     2646 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/es_CR.po
+-rw-r--r--  2.0 unx     2771 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/he.po
+-rw-r--r--  2.0 unx     2716 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/es_CO.po
+-rw-r--r--  2.0 unx     4009 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/sl.po
+-rw-r--r--  2.0 unx     2778 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/sr@latin.po
+-rw-r--r--  2.0 unx     2926 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/th.po
+-rw-r--r--  2.0 unx     2737 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/es_PE.po
+-rw-r--r--  2.0 unx     2692 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/es_ES.po
+-rw-r--r--  2.0 unx     2735 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/cs.po
+-rw-r--r--  2.0 unx     2753 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/pt_PT.po
+-rw-r--r--  2.0 unx     2681 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/eu.po
+-rw-r--r--  2.0 unx     2710 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/nb.po
+-rw-r--r--  2.0 unx     2713 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/da.po
+-rw-r--r--  2.0 unx     2823 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/mn.po
+-rw-r--r--  2.0 unx     2730 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/nl.po
+-rw-r--r--  2.0 unx     2677 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/am.po
+-rw-r--r--  2.0 unx     3424 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/de.po
+-rw-r--r--  2.0 unx     2738 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/vi.po
+-rw-r--r--  2.0 unx     2881 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/fr.po
+-rw-r--r--  2.0 unx     2779 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/pl.po
+-rw-r--r--  2.0 unx     2813 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/fa.po
+-rw-r--r--  2.0 unx     2768 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/bs.po
+-rw-r--r--  2.0 unx     2887 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/pt_BR.po
+-rw-r--r--  2.0 unx     2717 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/en_GB.po
+-rw-r--r--  2.0 unx     2812 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/el_GR.po
+-rw-r--r--  2.0 unx     2754 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/es_VE.po
+-rw-r--r--  2.0 unx     2753 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/es_MX.po
+-rw-r--r--  2.0 unx     2696 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/sv.po
+-rw-r--r--  2.0 unx     2735 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/sk.po
+-rw-r--r--  2.0 unx     2694 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/fi.po
+-rw-r--r--  2.0 unx     2776 b- defN 16-Nov-30 03:40 odoo_addons/purchase_order_type/i18n/hr_HR.po
 -rw-r--r--  2.0 unx     1460 b- defN 16-Apr-05 19:58 odoo_addons/purchase_order_type/views/view_purchase_order_type.xml
 -rw-r--r--  2.0 unx      779 b- defN 16-Apr-05 19:58 odoo_addons/purchase_order_type/views/res_partner_view.xml
 -rw-r--r--  2.0 unx     1565 b- defN 16-Apr-05 19:58 odoo_addons/purchase_order_type/views/view_purchase_order.xml
 -rw-r--r--  2.0 unx      567 b- defN 16-Apr-05 19:58 odoo_addons/purchase_order_type/data/purchase_order_type.xml
 -rw-r--r--  2.0 unx     9455 b- defN 16-Apr-05 19:58 odoo_addons/purchase_order_type/static/description/icon.png
--rw-r--r--  2.0 unx       12 b- defN 16-Oct-10 20:45 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/top_level.txt
--rw-r--r--  2.0 unx       92 b- defN 16-Oct-10 20:45 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/WHEEL
--rw-r--r--  2.0 unx     4449 b- defN 17-Apr-08 19:10 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/RECORD
--rw-r--r--  2.0 unx      556 b- defN 17-Apr-08 19:10 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/metadata.json
--rw-r--r--  2.0 unx     1811 b- defN 16-Oct-10 20:45 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx     2228 b- defN 17-Apr-08 19:10 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/METADATA
--rw-r--r--  2.0 unx       12 b- defN 16-Oct-10 20:45 odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/namespace_packages.txt
-41 files, 89394 bytes uncompressed, 36281 bytes compressed:  59.4%
+76 files, 189557 bytes uncompressed, 65672 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,8 +1,29 @@
-Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8-py2.7-nspkg.pth
+Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9-py2.7-nspkg.pth
+Comment: 
+
+Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/top_level.txt
+Comment: 
+
+Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/WHEEL
+Comment: 
+
+Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/RECORD
+Comment: 
+
+Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/metadata.json
+Comment: 
+
+Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/DESCRIPTION.rst
+Comment: 
+
+Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/METADATA
+Comment: 
+
+Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/namespace_packages.txt
 Comment: 
 
 Filename: odoo_addons/purchase_order_type/__openerp__.py
 Comment: 
 
 Filename: odoo_addons/purchase_order_type/__init__.py
 Comment: 
@@ -21,104 +42,188 @@
 
 Filename: odoo_addons/purchase_order_type/models/purchase_order_type.py
 Comment: 
 
 Filename: odoo_addons/purchase_order_type/models/__init__.py
 Comment: 
 
+Filename: odoo_addons/purchase_order_type/i18n/ja.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/lv.po
+Comment: 
+
 Filename: odoo_addons/purchase_order_type/i18n/zh_CN.po
 Comment: 
 
+Filename: odoo_addons/purchase_order_type/i18n/uk.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/es_AR.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/ko.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/ru.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/gl_ES.po
+Comment: 
+
 Filename: odoo_addons/purchase_order_type/i18n/pt.po
 Comment: 
 
+Filename: odoo_addons/purchase_order_type/i18n/fr_CH.po
+Comment: 
+
 Filename: odoo_addons/purchase_order_type/i18n/it.po
 Comment: 
 
 Filename: odoo_addons/purchase_order_type/i18n/es.po
 Comment: 
 
+Filename: odoo_addons/purchase_order_type/i18n/nl_BE.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/ar.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/lt.po
+Comment: 
+
 Filename: odoo_addons/purchase_order_type/i18n/tr.po
 Comment: 
 
+Filename: odoo_addons/purchase_order_type/i18n/mk.po
+Comment: 
+
 Filename: odoo_addons/purchase_order_type/i18n/hr.po
 Comment: 
 
 Filename: odoo_addons/purchase_order_type/i18n/bg.po
 Comment: 
 
+Filename: odoo_addons/purchase_order_type/i18n/es_EC.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/zh_TW.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/fr_CA.po
+Comment: 
+
 Filename: odoo_addons/purchase_order_type/i18n/gl.po
 Comment: 
 
 Filename: odoo_addons/purchase_order_type/i18n/ca.po
 Comment: 
 
+Filename: odoo_addons/purchase_order_type/i18n/es_CR.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/he.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/es_CO.po
+Comment: 
+
 Filename: odoo_addons/purchase_order_type/i18n/sl.po
 Comment: 
 
+Filename: odoo_addons/purchase_order_type/i18n/sr@latin.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/th.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/es_PE.po
+Comment: 
+
 Filename: odoo_addons/purchase_order_type/i18n/es_ES.po
 Comment: 
 
+Filename: odoo_addons/purchase_order_type/i18n/cs.po
+Comment: 
+
 Filename: odoo_addons/purchase_order_type/i18n/pt_PT.po
 Comment: 
 
+Filename: odoo_addons/purchase_order_type/i18n/eu.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/nb.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/da.po
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/i18n/mn.po
+Comment: 
+
 Filename: odoo_addons/purchase_order_type/i18n/nl.po
 Comment: 
 
 Filename: odoo_addons/purchase_order_type/i18n/am.po
 Comment: 
 
 Filename: odoo_addons/purchase_order_type/i18n/de.po
 Comment: 
 
+Filename: odoo_addons/purchase_order_type/i18n/vi.po
+Comment: 
+
 Filename: odoo_addons/purchase_order_type/i18n/fr.po
 Comment: 
 
-Filename: odoo_addons/purchase_order_type/i18n/pt_BR.po
+Filename: odoo_addons/purchase_order_type/i18n/pl.po
 Comment: 
 
-Filename: odoo_addons/purchase_order_type/i18n/el_GR.po
+Filename: odoo_addons/purchase_order_type/i18n/fa.po
 Comment: 
 
-Filename: odoo_addons/purchase_order_type/i18n/fi.po
+Filename: odoo_addons/purchase_order_type/i18n/bs.po
 Comment: 
 
-Filename: odoo_addons/purchase_order_type/i18n/hr_HR.po
+Filename: odoo_addons/purchase_order_type/i18n/pt_BR.po
 Comment: 
 
-Filename: odoo_addons/purchase_order_type/views/view_purchase_order_type.xml
+Filename: odoo_addons/purchase_order_type/i18n/en_GB.po
 Comment: 
 
-Filename: odoo_addons/purchase_order_type/views/res_partner_view.xml
+Filename: odoo_addons/purchase_order_type/i18n/el_GR.po
 Comment: 
 
-Filename: odoo_addons/purchase_order_type/views/view_purchase_order.xml
+Filename: odoo_addons/purchase_order_type/i18n/es_VE.po
 Comment: 
 
-Filename: odoo_addons/purchase_order_type/data/purchase_order_type.xml
+Filename: odoo_addons/purchase_order_type/i18n/es_MX.po
 Comment: 
 
-Filename: odoo_addons/purchase_order_type/static/description/icon.png
+Filename: odoo_addons/purchase_order_type/i18n/sv.po
 Comment: 
 
-Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/top_level.txt
+Filename: odoo_addons/purchase_order_type/i18n/sk.po
 Comment: 
 
-Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/WHEEL
+Filename: odoo_addons/purchase_order_type/i18n/fi.po
 Comment: 
 
-Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/RECORD
+Filename: odoo_addons/purchase_order_type/i18n/hr_HR.po
 Comment: 
 
-Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/metadata.json
+Filename: odoo_addons/purchase_order_type/views/view_purchase_order_type.xml
 Comment: 
 
-Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/DESCRIPTION.rst
+Filename: odoo_addons/purchase_order_type/views/res_partner_view.xml
 Comment: 
 
-Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/METADATA
+Filename: odoo_addons/purchase_order_type/views/view_purchase_order.xml
 Comment: 
 
-Filename: odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/namespace_packages.txt
+Filename: odoo_addons/purchase_order_type/data/purchase_order_type.xml
+Comment: 
+
+Filename: odoo_addons/purchase_order_type/static/description/icon.png
 Comment: 
 
 Zip file comment:
```

## odoo_addons/purchase_order_type/i18n/zh_CN.po

```diff
@@ -3,15 +3,15 @@
 # * purchase_order_type
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: purchase-workflow (8.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-30 13:27+0000\n"
+"POT-Creation-Date: 2016-11-16 12:06+0000\n"
 "PO-Revision-Date: 2016-03-08 10:17+0000\n"
 "Last-Translator: <>\n"
 "Language-Team: Chinese (China) (http://www.transifex.com/oca/OCA-purchase-workflow-8-0/language/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: zh_CN\n"
@@ -36,40 +36,40 @@
 #: field:purchase.order.type,create_date:0
 msgid "Created on"
 msgstr "创建时间"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,display_name:0
 msgid "Display Name"
-msgstr ""
+msgstr "显示名称"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,id:0
 msgid "ID"
 msgstr "ID"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,__last_update:0
 msgid "Last Modified on"
-msgstr ""
+msgstr "最后修改时间"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,write_uid:0
 msgid "Last Updated by"
 msgstr "最后更新者"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,write_date:0
 msgid "Last Updated on"
 msgstr "上次更新日期"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,name:0
 msgid "Name"
-msgstr ""
+msgstr "名称"
 
 #. module: purchase_order_type
 #: model:ir.model,name:purchase_order_type.model_res_partner
 msgid "Partner"
 msgstr ""
 
 #. module: purchase_order_type
@@ -91,8 +91,8 @@
 msgid "Purchase Order Types"
 msgstr ""
 
 #. module: purchase_order_type
 #: view:purchase.order:purchase_order_type.view_purchase_order_filter
 #: field:purchase.order,order_type:0
 msgid "Type"
-msgstr ""
+msgstr "类型"
```

## odoo_addons/purchase_order_type/i18n/pt.po

```diff
@@ -3,15 +3,15 @@
 # * purchase_order_type
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: purchase-workflow (8.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-15 11:37+0000\n"
+"POT-Creation-Date: 2016-11-16 12:06+0000\n"
 "PO-Revision-Date: 2016-03-08 10:17+0000\n"
 "Last-Translator: <>\n"
 "Language-Team: Portuguese (http://www.transifex.com/oca/OCA-purchase-workflow-8-0/language/pt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: pt\n"
@@ -36,45 +36,45 @@
 #: field:purchase.order.type,create_date:0
 msgid "Created on"
 msgstr "Criado em"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,display_name:0
 msgid "Display Name"
-msgstr ""
+msgstr "Nome"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,id:0
 msgid "ID"
 msgstr "ID"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,__last_update:0
 msgid "Last Modified on"
-msgstr ""
+msgstr "Modificado a última vez por"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,write_uid:0
 msgid "Last Updated by"
 msgstr "Atualizado pela última vez por"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,write_date:0
 msgid "Last Updated on"
 msgstr "Atualizado pela última vez em"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,name:0
 msgid "Name"
-msgstr ""
+msgstr "Nome"
 
 #. module: purchase_order_type
 #: model:ir.model,name:purchase_order_type.model_res_partner
 msgid "Partner"
-msgstr ""
+msgstr "Parceiro"
 
 #. module: purchase_order_type
 #: model:ir.model,name:purchase_order_type.model_purchase_order
 msgid "Purchase Order"
 msgstr ""
 
 #. module: purchase_order_type
```

## odoo_addons/purchase_order_type/i18n/it.po

```diff
@@ -17,28 +17,28 @@
 # Rudolf Schnapka <rs@techno-flex.de>, 2016
 # Rudolf Schnapka <schnapkar@golive-saar.de>, 2015
 # SaFi J. <safi2266@gmail.com>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: purchase-workflow (8.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-30 13:27+0000\n"
-"PO-Revision-Date: 2016-10-04 09:42+0000\n"
+"POT-Creation-Date: 2016-11-16 12:06+0000\n"
+"PO-Revision-Date: 2016-11-25 14:57+0000\n"
 "Last-Translator: OCA Transbot <transbot@odoo-community.org>\n"
 "Language-Team: Italian (http://www.transifex.com/oca/OCA-purchase-workflow-8-0/language/it/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: it\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,active:0
 msgid "Active"
-msgstr ""
+msgstr "Attivo"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,invoice_method:0
 msgid "Create Invoice"
 msgstr ""
 
 #. module: purchase_order_type
@@ -75,15 +75,15 @@
 #: field:purchase.order.type,write_date:0
 msgid "Last Updated on"
 msgstr "Ultimo aggiornamento il"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,name:0
 msgid "Name"
-msgstr ""
+msgstr "Nome"
 
 #. module: purchase_order_type
 #: model:ir.model,name:purchase_order_type.model_res_partner
 msgid "Partner"
 msgstr "Partner"
 
 #. module: purchase_order_type
```

## odoo_addons/purchase_order_type/i18n/es.po

```diff
@@ -18,33 +18,33 @@
 # Pedro M. Baeza <pedro.baeza@gmail.com>, 2015
 # Rudolf Schnapka <rs@techno-flex.de>, 2016
 # SaFi J. <safi2266@gmail.com>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: purchase-workflow (8.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-30 13:27+0000\n"
-"PO-Revision-Date: 2016-10-04 09:43+0000\n"
+"POT-Creation-Date: 2016-11-16 12:06+0000\n"
+"PO-Revision-Date: 2016-11-25 14:55+0000\n"
 "Last-Translator: OCA Transbot <transbot@odoo-community.org>\n"
 "Language-Team: Spanish (http://www.transifex.com/oca/OCA-purchase-workflow-8-0/language/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: es\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,active:0
 msgid "Active"
-msgstr ""
+msgstr "Activo"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,invoice_method:0
 msgid "Create Invoice"
-msgstr ""
+msgstr "Crear factura"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,create_uid:0
 msgid "Created by"
 msgstr "Creado por"
 
 #. module: purchase_order_type
```

## odoo_addons/purchase_order_type/i18n/tr.po

```diff
@@ -3,15 +3,15 @@
 # * purchase_order_type
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: purchase-workflow (8.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-15 11:37+0000\n"
+"POT-Creation-Date: 2016-11-16 12:06+0000\n"
 "PO-Revision-Date: 2016-03-08 10:17+0000\n"
 "Last-Translator: <>\n"
 "Language-Team: Turkish (http://www.transifex.com/oca/OCA-purchase-workflow-8-0/language/tr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: tr\n"
@@ -61,15 +61,15 @@
 #: field:purchase.order.type,write_date:0
 msgid "Last Updated on"
 msgstr "Son güncelleme"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,name:0
 msgid "Name"
-msgstr ""
+msgstr "Adı"
 
 #. module: purchase_order_type
 #: model:ir.model,name:purchase_order_type.model_res_partner
 msgid "Partner"
 msgstr ""
 
 #. module: purchase_order_type
```

## odoo_addons/purchase_order_type/i18n/hr.po

```diff
@@ -3,28 +3,28 @@
 # * purchase_order_type
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: purchase-workflow (8.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-30 13:27+0000\n"
+"POT-Creation-Date: 2016-11-16 12:06+0000\n"
 "PO-Revision-Date: 2016-03-08 10:17+0000\n"
 "Last-Translator: <>\n"
 "Language-Team: Croatian (http://www.transifex.com/oca/OCA-purchase-workflow-8-0/language/hr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: hr\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,active:0
 msgid "Active"
-msgstr ""
+msgstr "Aktivno"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,invoice_method:0
 msgid "Create Invoice"
 msgstr ""
 
 #. module: purchase_order_type
@@ -61,15 +61,15 @@
 #: field:purchase.order.type,write_date:0
 msgid "Last Updated on"
 msgstr "Zadnje ažuriranje"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,name:0
 msgid "Name"
-msgstr ""
+msgstr "Naziv"
 
 #. module: purchase_order_type
 #: model:ir.model,name:purchase_order_type.model_res_partner
 msgid "Partner"
 msgstr "Partner"
 
 #. module: purchase_order_type
@@ -91,8 +91,8 @@
 msgid "Purchase Order Types"
 msgstr ""
 
 #. module: purchase_order_type
 #: view:purchase.order:purchase_order_type.view_purchase_order_filter
 #: field:purchase.order,order_type:0
 msgid "Type"
-msgstr ""
+msgstr "Tip"
```

## odoo_addons/purchase_order_type/i18n/bg.po

```diff
@@ -3,15 +3,15 @@
 # * purchase_order_type
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: purchase-workflow (8.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-30 13:27+0000\n"
+"POT-Creation-Date: 2016-11-16 12:06+0000\n"
 "PO-Revision-Date: 2016-03-08 10:17+0000\n"
 "Last-Translator: <>\n"
 "Language-Team: Bulgarian (http://www.transifex.com/oca/OCA-purchase-workflow-8-0/language/bg/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: bg\n"
@@ -36,15 +36,15 @@
 #: field:purchase.order.type,create_date:0
 msgid "Created on"
 msgstr "Създадено на"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,display_name:0
 msgid "Display Name"
-msgstr ""
+msgstr "Име за Показване"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,id:0
 msgid "ID"
 msgstr "ID"
 
 #. module: purchase_order_type
@@ -91,8 +91,8 @@
 msgid "Purchase Order Types"
 msgstr ""
 
 #. module: purchase_order_type
 #: view:purchase.order:purchase_order_type.view_purchase_order_filter
 #: field:purchase.order,order_type:0
 msgid "Type"
-msgstr ""
+msgstr "Вид"
```

## odoo_addons/purchase_order_type/i18n/gl.po

```diff
@@ -3,15 +3,15 @@
 # * purchase_order_type
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: purchase-workflow (8.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-15 11:37+0000\n"
+"POT-Creation-Date: 2016-11-16 12:06+0000\n"
 "PO-Revision-Date: 2016-03-08 10:17+0000\n"
 "Last-Translator: <>\n"
 "Language-Team: Galician (http://www.transifex.com/oca/OCA-purchase-workflow-8-0/language/gl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: gl\n"
@@ -46,15 +46,15 @@
 #: field:purchase.order.type,id:0
 msgid "ID"
 msgstr "ID"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,__last_update:0
 msgid "Last Modified on"
-msgstr ""
+msgstr "Última modificación"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,write_uid:0
 msgid "Last Updated by"
 msgstr "ültima actualización por"
 
 #. module: purchase_order_type
```

## odoo_addons/purchase_order_type/i18n/pt_PT.po

```diff
@@ -3,15 +3,15 @@
 # * purchase_order_type
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: purchase-workflow (8.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-15 11:37+0000\n"
+"POT-Creation-Date: 2016-11-16 12:06+0000\n"
 "PO-Revision-Date: 2016-03-08 10:17+0000\n"
 "Last-Translator: <>\n"
 "Language-Team: Portuguese (Portugal) (http://www.transifex.com/oca/OCA-purchase-workflow-8-0/language/pt_PT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: pt_PT\n"
@@ -36,40 +36,40 @@
 #: field:purchase.order.type,create_date:0
 msgid "Created on"
 msgstr "Criado em"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,display_name:0
 msgid "Display Name"
-msgstr ""
+msgstr "Nome a Apresentar"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,id:0
 msgid "ID"
 msgstr "ID"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,__last_update:0
 msgid "Last Modified on"
-msgstr ""
+msgstr "Última Modificação Em"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,write_uid:0
 msgid "Last Updated by"
 msgstr "Atualizado pela última vez por"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,write_date:0
 msgid "Last Updated on"
 msgstr "Atualizado pela última vez em"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,name:0
 msgid "Name"
-msgstr ""
+msgstr "Nome"
 
 #. module: purchase_order_type
 #: model:ir.model,name:purchase_order_type.model_res_partner
 msgid "Partner"
 msgstr ""
 
 #. module: purchase_order_type
```

## odoo_addons/purchase_order_type/i18n/nl.po

```diff
@@ -3,15 +3,15 @@
 # * purchase_order_type
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: purchase-workflow (8.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-15 11:37+0000\n"
+"POT-Creation-Date: 2016-11-16 12:06+0000\n"
 "PO-Revision-Date: 2016-03-08 10:17+0000\n"
 "Last-Translator: <>\n"
 "Language-Team: Dutch (http://www.transifex.com/oca/OCA-purchase-workflow-8-0/language/nl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: nl\n"
@@ -26,45 +26,45 @@
 #: field:purchase.order.type,invoice_method:0
 msgid "Create Invoice"
 msgstr ""
 
 #. module: purchase_order_type
 #: field:purchase.order.type,create_uid:0
 msgid "Created by"
-msgstr ""
+msgstr "Aangemaakt door"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,create_date:0
 msgid "Created on"
-msgstr ""
+msgstr "Aangemaakt op"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,display_name:0
 msgid "Display Name"
 msgstr "Te tonen naam"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,id:0
 msgid "ID"
-msgstr ""
+msgstr "ID"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,__last_update:0
 msgid "Last Modified on"
 msgstr "Laatst bijgewerkt op"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,write_uid:0
 msgid "Last Updated by"
-msgstr ""
+msgstr "Laatst bijgewerkt door"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,write_date:0
 msgid "Last Updated on"
-msgstr ""
+msgstr "Laatst bijgewerkt op"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,name:0
 msgid "Name"
 msgstr "Naam"
 
 #. module: purchase_order_type
```

## odoo_addons/purchase_order_type/i18n/de.po

```diff
@@ -18,16 +18,16 @@
 # Pedro M. Baeza <pedro.baeza@gmail.com>, 2015
 # Rudolf Schnapka <rs@techno-flex.de>, 2015-2016
 # SaFi J. <safi2266@gmail.com>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: purchase-workflow (8.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-30 13:27+0000\n"
-"PO-Revision-Date: 2016-10-04 09:43+0000\n"
+"POT-Creation-Date: 2016-11-16 12:06+0000\n"
+"PO-Revision-Date: 2016-11-25 14:55+0000\n"
 "Last-Translator: OCA Transbot <transbot@odoo-community.org>\n"
 "Language-Team: German (http://www.transifex.com/oca/OCA-purchase-workflow-8-0/language/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -106,8 +106,8 @@
 msgid "Purchase Order Types"
 msgstr ""
 
 #. module: purchase_order_type
 #: view:purchase.order:purchase_order_type.view_purchase_order_filter
 #: field:purchase.order,order_type:0
 msgid "Type"
-msgstr ""
+msgstr "Art"
```

## odoo_addons/purchase_order_type/i18n/fr.po

```diff
@@ -5,16 +5,16 @@
 # Translators:
 # Matjaž Mozetič <m.mozetic@matmoz.si>, 2016
 # Rudolf Schnapka <rs@techno-flex.de>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: purchase-workflow (8.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-15 11:37+0000\n"
-"PO-Revision-Date: 2016-09-16 21:46+0000\n"
+"POT-Creation-Date: 2016-11-16 12:06+0000\n"
+"PO-Revision-Date: 2016-11-25 14:55+0000\n"
 "Last-Translator: OCA Transbot <transbot@odoo-community.org>\n"
 "Language-Team: French (http://www.transifex.com/oca/OCA-purchase-workflow-8-0/language/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: fr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -63,15 +63,15 @@
 #: field:purchase.order.type,write_date:0
 msgid "Last Updated on"
 msgstr "Dernière modification le"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,name:0
 msgid "Name"
-msgstr ""
+msgstr "Nom"
 
 #. module: purchase_order_type
 #: model:ir.model,name:purchase_order_type.model_res_partner
 msgid "Partner"
 msgstr "Partenaire"
 
 #. module: purchase_order_type
```

## odoo_addons/purchase_order_type/i18n/pt_BR.po

```diff
@@ -5,28 +5,28 @@
 # Translators:
 # Matjaž Mozetič <m.mozetic@matmoz.si>, 2015
 # Thomas A. Jaeger, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: purchase-workflow (8.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-30 13:27+0000\n"
-"PO-Revision-Date: 2016-10-04 09:42+0000\n"
+"POT-Creation-Date: 2016-11-16 12:06+0000\n"
+"PO-Revision-Date: 2016-11-25 14:55+0000\n"
 "Last-Translator: OCA Transbot <transbot@odoo-community.org>\n"
 "Language-Team: Portuguese (Brazil) (http://www.transifex.com/oca/OCA-purchase-workflow-8-0/language/pt_BR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: pt_BR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,active:0
 msgid "Active"
-msgstr ""
+msgstr "Ativo"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,invoice_method:0
 msgid "Create Invoice"
 msgstr ""
 
 #. module: purchase_order_type
@@ -63,20 +63,20 @@
 #: field:purchase.order.type,write_date:0
 msgid "Last Updated on"
 msgstr "Ultima Atualização em"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,name:0
 msgid "Name"
-msgstr ""
+msgstr "Nome"
 
 #. module: purchase_order_type
 #: model:ir.model,name:purchase_order_type.model_res_partner
 msgid "Partner"
-msgstr ""
+msgstr "Parceiro"
 
 #. module: purchase_order_type
 #: model:ir.model,name:purchase_order_type.model_purchase_order
 msgid "Purchase Order"
 msgstr "Ordem de Compra"
 
 #. module: purchase_order_type
```

## odoo_addons/purchase_order_type/i18n/el_GR.po

```diff
@@ -3,15 +3,15 @@
 # * purchase_order_type
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: purchase-workflow (8.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-15 11:37+0000\n"
+"POT-Creation-Date: 2016-11-16 12:06+0000\n"
 "PO-Revision-Date: 2016-03-08 10:17+0000\n"
 "Last-Translator: <>\n"
 "Language-Team: Greek (Greece) (http://www.transifex.com/oca/OCA-purchase-workflow-8-0/language/el_GR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: el_GR\n"
@@ -66,15 +66,15 @@
 #: field:purchase.order.type,name:0
 msgid "Name"
 msgstr ""
 
 #. module: purchase_order_type
 #: model:ir.model,name:purchase_order_type.model_res_partner
 msgid "Partner"
-msgstr ""
+msgstr "Συνεργάτης"
 
 #. module: purchase_order_type
 #: model:ir.model,name:purchase_order_type.model_purchase_order
 msgid "Purchase Order"
 msgstr ""
 
 #. module: purchase_order_type
```

## odoo_addons/purchase_order_type/i18n/fi.po

```diff
@@ -3,15 +3,15 @@
 # * purchase_order_type
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: purchase-workflow (8.0)\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2016-09-15 11:37+0000\n"
+"POT-Creation-Date: 2016-11-16 12:06+0000\n"
 "PO-Revision-Date: 2016-03-08 10:17+0000\n"
 "Last-Translator: <>\n"
 "Language-Team: Finnish (http://www.transifex.com/oca/OCA-purchase-workflow-8-0/language/fi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Language: fi\n"
@@ -61,20 +61,20 @@
 #: field:purchase.order.type,write_date:0
 msgid "Last Updated on"
 msgstr "Viimeksi päivitetty"
 
 #. module: purchase_order_type
 #: field:purchase.order.type,name:0
 msgid "Name"
-msgstr ""
+msgstr "Nimi"
 
 #. module: purchase_order_type
 #: model:ir.model,name:purchase_order_type.model_res_partner
 msgid "Partner"
-msgstr ""
+msgstr "Kumppani"
 
 #. module: purchase_order_type
 #: model:ir.model,name:purchase_order_type.model_purchase_order
 msgid "Purchase Order"
 msgstr ""
 
 #. module: purchase_order_type
```

## Comparing `odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/metadata.json` & `odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/metadata.json`

 * *Files 21% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9416666666666667%*

 * *Differences: {"'extensions'": "{'python.details': {'contacts': [OrderedDict([('email', "*

 * *                 "'support@odoo-community.org'), ('name', 'Camptocamp,Odoo Community Association "*

 * *                 "(OCA)'), ('role', 'author')])]}}",*

 * * "'version'": "'8.0.1.0.0.99.dev9'"}*

```diff
@@ -2,14 +2,21 @@
     "classifiers": [
         "Programming Language :: Python :: 2.7",
         "Framework :: Odoo",
         "License :: OSI Approved :: GNU Affero General Public License v3"
     ],
     "extensions": {
         "python.details": {
+            "contacts": [
+                {
+                    "email": "support@odoo-community.org",
+                    "name": "Camptocamp,Odoo Community Association (OCA)",
+                    "role": "author"
+                }
+            ],
             "document_names": {
                 "description": "DESCRIPTION.rst"
             },
             "project_urls": {
                 "Home": "http://www.camptocamp.com"
             }
         }
@@ -23,9 +30,9 @@
         {
             "requires": [
                 "odoo (<9.0a,>=8.0a)"
             ]
         }
     ],
     "summary": "Purchase Order Type",
-    "version": "8.0.1.0.0.99.dev8"
+    "version": "8.0.1.0.0.99.dev9"
 }
```

## Comparing `odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/DESCRIPTION.rst` & `odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

## Comparing `odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev8.dist-info/METADATA` & `odoo8_addon_purchase_order_type-8.0.1.0.0.99.dev9.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.0
 Name: odoo8-addon-purchase-order-type
-Version: 8.0.1.0.0.99.dev8
+Version: 8.0.1.0.0.99.dev9
 Summary: Purchase Order Type
 Home-page: http://www.camptocamp.com
-Author: UNKNOWN
-Author-email: UNKNOWN
+Author: Camptocamp,Odoo Community Association (OCA)
+Author-email: support@odoo-community.org
 License: AGPL-3
 Platform: UNKNOWN
 Requires-Dist: odoo (<9.0a,>=8.0a)
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Framework :: Odoo
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

