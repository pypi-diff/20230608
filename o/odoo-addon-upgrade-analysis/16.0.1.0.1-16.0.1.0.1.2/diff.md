# Comparing `tmp/odoo_addon_upgrade_analysis-16.0.1.0.1-py3-none-any.whl.zip` & `tmp/odoo_addon_upgrade_analysis-16.0.1.0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,56 +1,56 @@
-Zip file size: 65394 bytes, number of entries: 54
--rw-r--r--  2.0 unx     4374 b- defN 23-May-18 08:36 odoo/addons/upgrade_analysis/README.rst
--rw-r--r--  2.0 unx      140 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/__init__.py
--rw-r--r--  2.0 unx     1077 b- defN 23-May-18 08:36 odoo/addons/upgrade_analysis/__manifest__.py
--rw-r--r--  2.0 unx      362 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/blacklist.py
--rw-r--r--  2.0 unx    20132 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/compare.py
--rw-r--r--  2.0 unx     8297 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/upgrade_log.py
--rw-r--r--  2.0 unx    21729 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/i18n/es_AR.po
--rw-r--r--  2.0 unx    19394 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/i18n/fr.po
--rw-r--r--  2.0 unx    19158 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot
--rw-r--r--  2.0 unx      163 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/models/__init__.py
--rw-r--r--  2.0 unx     1031 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/models/ir_module_module.py
--rw-r--r--  2.0 unx    22546 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/models/upgrade_analysis.py
--rw-r--r--  2.0 unx      536 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/models/upgrade_attribute.py
--rw-r--r--  2.0 unx     3098 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/models/upgrade_comparison_config.py
--rw-r--r--  2.0 unx     6006 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/models/upgrade_record.py
--rw-r--r--  2.0 unx       65 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/__init__.py
--rw-r--r--  2.0 unx     1843 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo_patch.py
--rw-r--r--  2.0 unx       66 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/addons/__init__.py
--rw-r--r--  2.0 unx      270 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/addons/mrp/__init__.py
--rw-r--r--  2.0 unx      371 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/addons/point_of_sale/__init__.py
--rw-r--r--  2.0 unx      259 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/addons/stock/__init__.py
--rw-r--r--  2.0 unx       84 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/__init__.py
--rw-r--r--  2.0 unx      739 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/models.py
--rw-r--r--  2.0 unx       19 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/__init__.py
--rw-r--r--  2.0 unx       23 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/__init__.py
--rw-r--r--  2.0 unx     1482 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/ir_model.py
--rw-r--r--  2.0 unx       23 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/__init__.py
--rw-r--r--  2.0 unx     1112 b- defN 23-May-18 08:36 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/registry.py
--rw-r--r--  2.0 unx       22 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/__init__.py
--rw-r--r--  2.0 unx      397 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/convert.py
--rw-r--r--  2.0 unx      308 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/readme/CONTRIBUTORS.rst
--rw-r--r--  2.0 unx      675 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/readme/DESCRIPTION.rst
--rw-r--r--  2.0 unx      263 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/readme/ROADMAP.rst
--rw-r--r--  2.0 unx       71 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/readme/USAGE.rst
--rw-r--r--  2.0 unx      696 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/security/ir.model.access.csv
--rw-r--r--  2.0 unx     9455 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/static/description/icon.png
--rw-r--r--  2.0 unx    14699 b- defN 23-May-18 08:36 odoo/addons/upgrade_analysis/static/description/index.html
--rw-r--r--  2.0 unx      744 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/static/src/module_coverage_template.rst.mako
--rw-r--r--  2.0 unx       26 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/tests/__init__.py
--rw-r--r--  2.0 unx     1787 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/tests/test_module.py
--rw-r--r--  2.0 unx      200 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/views/menu.xml
--rw-r--r--  2.0 unx     2640 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/views/view_upgrade_analysis.xml
--rw-r--r--  2.0 unx     2826 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/views/view_upgrade_comparison_config.xml
--rw-r--r--  2.0 unx     2834 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/views/view_upgrade_record.xml
--rw-r--r--  2.0 unx       82 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/wizards/__init__.py
--rw-r--r--  2.0 unx     4527 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/wizards/upgrade_generate_record_wizard.py
--rw-r--r--  2.0 unx     4040 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py
--rw-r--r--  2.0 unx     1787 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml
--rw-r--r--  2.0 unx     3289 b- defN 23-May-18 08:35 odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml
--rw-r--r--  2.0 unx     5093 b- defN 23-May-18 08:36 odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-18 08:36 odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-18 08:36 odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6017 b- defN 23-May-18 08:36 odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/RECORD
-54 files, 196995 bytes uncompressed, 55210 bytes compressed:  72.0%
+Zip file size: 65564 bytes, number of entries: 54
+-rw-r--r--  2.0 unx     4374 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/README.rst
+-rw-r--r--  2.0 unx      140 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/__init__.py
+-rw-r--r--  2.0 unx     1077 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/__manifest__.py
+-rw-r--r--  2.0 unx      362 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/blacklist.py
+-rw-r--r--  2.0 unx    20132 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/compare.py
+-rw-r--r--  2.0 unx     8297 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/upgrade_log.py
+-rw-r--r--  2.0 unx    22496 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/i18n/es_AR.po
+-rw-r--r--  2.0 unx    20161 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/i18n/fr.po
+-rw-r--r--  2.0 unx    19925 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot
+-rw-r--r--  2.0 unx      163 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/models/__init__.py
+-rw-r--r--  2.0 unx     1031 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/models/ir_module_module.py
+-rw-r--r--  2.0 unx    22546 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/models/upgrade_analysis.py
+-rw-r--r--  2.0 unx      536 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/models/upgrade_attribute.py
+-rw-r--r--  2.0 unx     3098 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/models/upgrade_comparison_config.py
+-rw-r--r--  2.0 unx     6006 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/models/upgrade_record.py
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/__init__.py
+-rw-r--r--  2.0 unx     1843 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/odoo_patch.py
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/addons/__init__.py
+-rw-r--r--  2.0 unx      270 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/addons/mrp/__init__.py
+-rw-r--r--  2.0 unx      371 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/addons/point_of_sale/__init__.py
+-rw-r--r--  2.0 unx      259 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/addons/stock/__init__.py
+-rw-r--r--  2.0 unx       84 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/odoo/__init__.py
+-rw-r--r--  2.0 unx      739 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/odoo/models.py
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/__init__.py
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/__init__.py
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/__init__.py
+-rw-r--r--  2.0 unx     1482 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/ir_model.py
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/__init__.py
+-rw-r--r--  2.0 unx     1112 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/registry.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/__init__.py
+-rw-r--r--  2.0 unx      397 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/convert.py
+-rw-r--r--  2.0 unx      308 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/readme/CONTRIBUTORS.rst
+-rw-r--r--  2.0 unx      675 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/readme/DESCRIPTION.rst
+-rw-r--r--  2.0 unx      263 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/readme/ROADMAP.rst
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/readme/USAGE.rst
+-rw-r--r--  2.0 unx      696 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/security/ir.model.access.csv
+-rw-r--r--  2.0 unx     9455 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/static/description/icon.png
+-rw-r--r--  2.0 unx    14699 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/static/description/index.html
+-rw-r--r--  2.0 unx      744 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/static/src/module_coverage_template.rst.mako
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/tests/__init__.py
+-rw-r--r--  2.0 unx     1787 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/tests/test_module.py
+-rw-r--r--  2.0 unx      200 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/views/menu.xml
+-rw-r--r--  2.0 unx     2640 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/views/view_upgrade_analysis.xml
+-rw-r--r--  2.0 unx     2826 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/views/view_upgrade_comparison_config.xml
+-rw-r--r--  2.0 unx     2834 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/views/view_upgrade_record.xml
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/wizards/__init__.py
+-rw-r--r--  2.0 unx     4527 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/wizards/upgrade_generate_record_wizard.py
+-rw-r--r--  2.0 unx     4040 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py
+-rw-r--r--  2.0 unx     1787 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml
+-rw-r--r--  2.0 unx     3289 b- defN 23-Jun-08 05:27 odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml
+-rw-r--r--  2.0 unx     5095 b- defN 23-Jun-08 05:28 odoo_addon_upgrade_analysis-16.0.1.0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 05:28 odoo_addon_upgrade_analysis-16.0.1.0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-08 05:28 odoo_addon_upgrade_analysis-16.0.1.0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     6025 b- defN 23-Jun-08 05:28 odoo_addon_upgrade_analysis-16.0.1.0.1.2.dist-info/RECORD
+54 files, 199306 bytes uncompressed, 55364 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -144,20 +144,20 @@
 
 Filename: odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml
 Comment: 
 
 Filename: odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/METADATA
+Filename: odoo_addon_upgrade_analysis-16.0.1.0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/WHEEL
+Filename: odoo_addon_upgrade_analysis-16.0.1.0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/top_level.txt
+Filename: odoo_addon_upgrade_analysis-16.0.1.0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/RECORD
+Filename: odoo_addon_upgrade_analysis-16.0.1.0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/upgrade_analysis/i18n/es_AR.po

```diff
@@ -376,14 +376,25 @@
 "modifies an attribute of an existing field, set to Modify."
 msgstr ""
 "Establézcalo en Crear si se crea un campo recientemente en este módulo. Si "
 "este módulo modifica un atributo de un campo existente, configúrelo en "
 "Modificar."
 
 #. module: upgrade_analysis
+#: model:ir.model.fields,field_description:upgrade_analysis.field_ir_module_module__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_attribute__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_comparison_config__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_record__smart_search
+msgid "Smart Search"
+msgstr ""
+
+#. module: upgrade_analysis
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis__state
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard__state
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__state
 msgid "State"
 msgstr "Estado"
 
 #. module: upgrade_analysis
```

## odoo/addons/upgrade_analysis/i18n/fr.po

```diff
@@ -370,14 +370,25 @@
 #: model:ir.model.fields,help:upgrade_analysis.field_upgrade_record__mode
 msgid ""
 "Set to Create if a field is newly created in this module. If this module "
 "modifies an attribute of an existing field, set to Modify."
 msgstr ""
 
 #. module: upgrade_analysis
+#: model:ir.model.fields,field_description:upgrade_analysis.field_ir_module_module__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_attribute__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_comparison_config__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_record__smart_search
+msgid "Smart Search"
+msgstr ""
+
+#. module: upgrade_analysis
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis__state
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard__state
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__state
 msgid "State"
 msgstr ""
 
 #. module: upgrade_analysis
```

## odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot

```diff
@@ -367,14 +367,25 @@
 #: model:ir.model.fields,help:upgrade_analysis.field_upgrade_record__mode
 msgid ""
 "Set to Create if a field is newly created in this module. If this module "
 "modifies an attribute of an existing field, set to Modify."
 msgstr ""
 
 #. module: upgrade_analysis
+#: model:ir.model.fields,field_description:upgrade_analysis.field_ir_module_module__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_attribute__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_comparison_config__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__smart_search
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_record__smart_search
+msgid "Smart Search"
+msgstr ""
+
+#. module: upgrade_analysis
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis__state
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard__state
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__state
 msgid "State"
 msgstr ""
 
 #. module: upgrade_analysis
```

## Comparing `odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/METADATA` & `odoo_addon_upgrade_analysis-16.0.1.0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addon-upgrade-analysis
-Version: 16.0.1.0.1
+Version: 16.0.1.0.1.2
 Summary: Performs a difference analysis between modules installed on two different Odoo instances
 Home-page: https://github.com/OCA/server-tools
 Author: Therp BV, Opener B.V., GRAP, Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

## Comparing `odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/RECORD` & `odoo_addon_upgrade_analysis-16.0.1.0.1.2.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 odoo/addons/upgrade_analysis/README.rst,sha256=L7fJmx5z1ACd9xMUYSPAYUCMyK-_myiqZNYyH-OMuRk,4374
 odoo/addons/upgrade_analysis/__init__.py,sha256=1X8E6viDvX9QCI3au33OFkjFkJbFw6TazruSkrDurdI,140
 odoo/addons/upgrade_analysis/__manifest__.py,sha256=2OZzZt_W_D_UHpRmz5g55BHdbvtbP0Mf9sflPZLieyY,1077
 odoo/addons/upgrade_analysis/blacklist.py,sha256=BIu8cYUB6j3FYtSaRcs4nSxB6yUwyjhxzOaex1AiIHY,362
 odoo/addons/upgrade_analysis/compare.py,sha256=XSetlfvLS0LBy9nI5kF1gcneaaMo7kjd2uAwPz4KSoQ,20132
 odoo/addons/upgrade_analysis/upgrade_log.py,sha256=aUeWhlnpxJIF5lgHoLfbZTlqHpgXcK-GNsYs92IidGw,8297
-odoo/addons/upgrade_analysis/i18n/es_AR.po,sha256=-YEVyBWFRo-zlhetYhVNY7UEOVJ8jMupvB8Wnmab-Eo,21729
-odoo/addons/upgrade_analysis/i18n/fr.po,sha256=xJ7BoW6ECLVdZ16y2Mkx9UKKCg908RX-mya-ujdY0II,19394
-odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot,sha256=734gkxUCJftNZDDpZwY72jMURStqFssecT0K2eq6MD0,19158
+odoo/addons/upgrade_analysis/i18n/es_AR.po,sha256=fHZ_DD9rAwE5ecWSzlX3WMep0t3FG3I7Qsqnchq5f2Y,22496
+odoo/addons/upgrade_analysis/i18n/fr.po,sha256=uzNf1Vqaxcu3y6-CHg_IXUPFdNg6DHVOAB3mR75VDaY,20161
+odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot,sha256=oudXK6RkCZ2S6B3aoy7Mxf4moyBC8sJVYV8P8Rb6i6I,19925
 odoo/addons/upgrade_analysis/models/__init__.py,sha256=V3z7qRHAST0ArkG6eGCgABdDHniOvY7Mcna8I4M5duk,163
 odoo/addons/upgrade_analysis/models/ir_module_module.py,sha256=Wy2bfWlulZ-ucpxh6flDgGcvCPBpeL1TztPCxW1x-9U,1031
 odoo/addons/upgrade_analysis/models/upgrade_analysis.py,sha256=6UBaqInIMil8iw9ZDiu9-qNLetFDxYwe6_UyxxEQ1u4,22546
 odoo/addons/upgrade_analysis/models/upgrade_attribute.py,sha256=j2K_dqArvAHThW51VWhiNSiyoy9g5BnPS01khhaaovw,536
 odoo/addons/upgrade_analysis/models/upgrade_comparison_config.py,sha256=2v-0S5vXoFZsL7e-wXlHdWdf3j5v222pYK5kKcbLCmk,3098
 odoo/addons/upgrade_analysis/models/upgrade_record.py,sha256=-z1YaxulCLJPD4Y6RgkHpndmoe3J9ytllKo1qFxBvyk,6006
 odoo/addons/upgrade_analysis/odoo_patch/__init__.py,sha256=dd3BGgBnbgdu740xmYrIfYX8F-S42Ia4m_JDFX5HHqA,65
@@ -44,11 +44,11 @@
 odoo/addons/upgrade_analysis/views/view_upgrade_comparison_config.xml,sha256=pBTVmGOGkohO1tguxKFXAWGHkrSVJdok3jjuhERcGa4,2826
 odoo/addons/upgrade_analysis/views/view_upgrade_record.xml,sha256=oBxhlkz42bJxhrFMydpKpEDYt1sX0Z9WMipuA5Bpq2M,2834
 odoo/addons/upgrade_analysis/wizards/__init__.py,sha256=6973yn8jkeAaHm-ofIILbHUCB6KQ7RUMSDCK0Xk18xE,82
 odoo/addons/upgrade_analysis/wizards/upgrade_generate_record_wizard.py,sha256=DTeLN_1rez_v82EA16H2Bsk4TGk9aA_n7Wn6_qQoKUE,4527
 odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py,sha256=4g8E1EdR83R84hGVWHx45JVjnz8naQlBfvHNj5bNE6Q,4040
 odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml,sha256=80IblSl5Jux1jYoh0bJGBJikNRk39HDgiRylMWPdkJo,1787
 odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml,sha256=_6uw3NVhdBp_gP5mybo--AI97n3_v6tIcyX2Z0WoCrE,3289
-odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/METADATA,sha256=vURFSRPnJIq6BXGn-td8-g_vcRyighNcDzo7HAIpzP4,5093
-odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo_addon_upgrade_analysis-16.0.1.0.1.dist-info/RECORD,,
+odoo_addon_upgrade_analysis-16.0.1.0.1.2.dist-info/METADATA,sha256=7ZvUqxMbzF3kYsvpjs1jTAzS_NxPkQNzN1dNmaBwgvU,5095
+odoo_addon_upgrade_analysis-16.0.1.0.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+odoo_addon_upgrade_analysis-16.0.1.0.1.2.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo_addon_upgrade_analysis-16.0.1.0.1.2.dist-info/RECORD,,
```

