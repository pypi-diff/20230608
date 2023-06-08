# Comparing `tmp/cycode-0.2.5.dev3.tar.gz` & `tmp/cycode-0.2.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-0.2.5.dev3.tar", max compression
+gzip compressed data, was "cycode-0.2.5.dev4.tar", max compression
```

## Comparing `cycode-0.2.5.dev3.tar` & `cycode-0.2.5.dev4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    32320 2023-06-06 14:03:24.278248 cycode-0.2.5.dev3/README.md
--rw-r--r--   0        0        0      115 2023-06-06 14:03:51.456434 cycode-0.2.5.dev3/cycode/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 14:03:24.278248 cycode-0.2.5.dev3/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 14:03:24.278248 cycode-0.2.5.dev3/cycode/cli/auth/__init__.py
--rw-r--r--   0        0        0     2813 2023-06-06 14:03:24.278248 cycode-0.2.5.dev3/cycode/cli/auth/auth_command.py
--rw-r--r--   0        0        0     4761 2023-06-06 14:03:24.278248 cycode-0.2.5.dev3/cycode/cli/auth/auth_manager.py
--rw-r--r--   0        0        0     1652 2023-06-06 14:03:24.278248 cycode-0.2.5.dev3/cycode/cli/ci_integrations.py
--rw-r--r--   0        0        0    47480 2023-06-06 14:03:24.278248 cycode-0.2.5.dev3/cycode/cli/code_scanner.py
--rw-r--r--   0        0        0      453 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/config.py
--rw-r--r--   0        0        0      387 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/config.yaml
--rw-r--r--   0        0        0     5039 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     1698 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0        0 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/helpers/maven/__init__.py
--rw-r--r--   0        0        0     2196 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0      992 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/helpers/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     2993 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/helpers/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     5835 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/helpers/sca_code_scanner.py
--rw-r--r--   0        0        0     7213 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/main.py
--rw-r--r--   0        0        0     1332 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/models.py
--rw-r--r--   0        0        0       93 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0      564 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/printers/base_printer.py
--rw-r--r--   0        0        0     1709 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/printers/console_printer.py
--rw-r--r--   0        0        0     1537 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     5813 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/printers/table_printer.py
--rw-r--r--   0        0        0     9166 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      533 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4821 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     6925 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     1908 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0     6853 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/user_settings/user_settings_commands.py
--rw-r--r--   0        0        0        0 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0     2162 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0      195 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      941 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     1229 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2700 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      815 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      929 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cli/zip_file.py
--rw-r--r--   0        0        0       57 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1708 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     2458 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      119 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      220 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     3617 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      543 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     1705 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0     9102 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/models.py
--rw-r--r--   0        0        0     6222 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0        0 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/scan_config/__init__.py
--rw-r--r--   0        0        0     1090 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/scan_config/scan_config_base.py
--rw-r--r--   0        0        0     1021 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/scan_config/scan_config_creator.py
--rw-r--r--   0        0        0      197 2023-06-06 14:03:24.282248 cycode-0.2.5.dev3/cycode/cyclient/utils.py
--rw-r--r--   0        0        0     2032 2023-06-06 14:03:51.452434 cycode-0.2.5.dev3/pyproject.toml
--rw-r--r--   0        0        0    33844 1970-01-01 00:00:00.000000 cycode-0.2.5.dev3/PKG-INFO
+-rw-r--r--   0        0        0    32320 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/README.md
+-rw-r--r--   0        0        0      115 2023-06-08 10:17:46.553493 cycode-0.2.5.dev4/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/auth/__init__.py
+-rw-r--r--   0        0        0     2813 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/auth/auth_command.py
+-rw-r--r--   0        0        0     4761 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/auth/auth_manager.py
+-rw-r--r--   0        0        0     1652 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/ci_integrations.py
+-rw-r--r--   0        0        0    47480 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/code_scanner.py
+-rw-r--r--   0        0        0      453 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/config.py
+-rw-r--r--   0        0        0      387 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     5039 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     1698 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/helpers/maven/__init__.py
+-rw-r--r--   0        0        0     2196 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0      992 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/helpers/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     2993 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/helpers/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     5835 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/helpers/sca_code_scanner.py
+-rw-r--r--   0        0        0     7213 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/main.py
+-rw-r--r--   0        0        0     1332 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0      564 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/printers/base_printer.py
+-rw-r--r--   0        0        0     1709 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     1537 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     6108 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/printers/table_printer.py
+-rw-r--r--   0        0        0     9166 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      533 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4821 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     6925 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     1908 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0     6853 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/user_settings/user_settings_commands.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0     2162 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0      195 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      941 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     1229 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2700 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      815 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      929 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cli/zip_file.py
+-rw-r--r--   0        0        0       57 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1708 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     2458 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      119 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      220 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     3617 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      543 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     1705 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0     9102 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     6222 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cyclient/scan_config/__init__.py
+-rw-r--r--   0        0        0     1090 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cyclient/scan_config/scan_config_base.py
+-rw-r--r--   0        0        0     1021 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cyclient/scan_config/scan_config_creator.py
+-rw-r--r--   0        0        0      197 2023-06-08 10:17:21.875515 cycode-0.2.5.dev4/cycode/cyclient/utils.py
+-rw-r--r--   0        0        0     2032 2023-06-08 10:17:46.553493 cycode-0.2.5.dev4/pyproject.toml
+-rw-r--r--   0        0        0    33844 1970-01-01 00:00:00.000000 cycode-0.2.5.dev4/PKG-INFO
```

### Comparing `cycode-0.2.5.dev3/README.md` & `cycode-0.2.5.dev4/README.md`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/auth/auth_command.py` & `cycode-0.2.5.dev4/cycode/cli/auth/auth_command.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/auth/auth_manager.py` & `cycode-0.2.5.dev4/cycode/cli/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/ci_integrations.py` & `cycode-0.2.5.dev4/cycode/cli/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/code_scanner.py` & `cycode-0.2.5.dev4/cycode/cli/code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/consts.py` & `cycode-0.2.5.dev4/cycode/cli/consts.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/exceptions/custom_exceptions.py` & `cycode-0.2.5.dev4/cycode/cli/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/helpers/maven/base_restore_maven_dependencies.py` & `cycode-0.2.5.dev4/cycode/cli/helpers/maven/base_restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/helpers/maven/restore_gradle_dependencies.py` & `cycode-0.2.5.dev4/cycode/cli/helpers/maven/restore_gradle_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/helpers/maven/restore_maven_dependencies.py` & `cycode-0.2.5.dev4/cycode/cli/helpers/maven/restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/helpers/sca_code_scanner.py` & `cycode-0.2.5.dev4/cycode/cli/helpers/sca_code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/main.py` & `cycode-0.2.5.dev4/cycode/cli/main.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/models.py` & `cycode-0.2.5.dev4/cycode/cli/models.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/printers/base_printer.py` & `cycode-0.2.5.dev4/cycode/cli/printers/base_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/printers/console_printer.py` & `cycode-0.2.5.dev4/cycode/cli/printers/console_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/printers/json_printer.py` & `cycode-0.2.5.dev4/cycode/cli/printers/json_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/printers/table_printer.py` & `cycode-0.2.5.dev4/cycode/cli/printers/table_printer.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,43 +115,51 @@
 
         click.echo(text_table.draw())
 
     @staticmethod
     def set_table_width(headers: List[str], text_table: Texttable) -> None:
         header_width_size_cols = []
         for header in headers:
-            header_width_size_cols.append(len(header))
-
+            header_len = len(header)
+            if header == CVE_COLUMN:
+                header_width_size_cols.append(header_len * 5)
+            elif header == UPGRADE_COLUMN:
+                header_width_size_cols.append(header_len * 2)
+            else:
+                header_width_size_cols.append(header_len)
         text_table.set_cols_width(header_width_size_cols)
 
     @staticmethod
     def _print_summary_issues(detections: List, title: str) -> None:
         click.echo(f'⛔ Found {len(detections)} issues of type: {click.style(title, bold=True)}')
 
     def _get_common_detection_fields(self, detection: Detection) -> List[str]:
         row = [
             detection.detection_details.get('file_name'),
             detection.detection_details.get('ecosystem'),
             detection.detection_details.get('package_name'),
             detection.detection_details.get('is_direct_dependency_str'),
-            detection.detection_details.get('is_dev_dependency_str'),
-            detection.detection_details.get('vulnerability_id')
+            detection.detection_details.get('is_dev_dependency_str')
         ]
 
         if self._is_git_repository():
             row = [detection.detection_details.get('repository_name')] + row
 
         return row
 
     def _is_git_repository(self) -> bool:
         return self.context.obj.get("remote_url") is not None
 
     def _get_upgrade_package_vulnerability(self, detection: Detection) -> List[str]:
         alert = detection.detection_details.get('alert')
-        row = [detection.detection_details.get('advisory_severity')] + self._get_common_detection_fields(detection)
+        row = [
+            detection.detection_details.get('advisory_severity'),
+            *self._get_common_detection_fields(detection),
+            detection.detection_details.get('vulnerability_id')
+        ]
 
         upgrade = ''
         if alert.get("first_patched_version"):
             upgrade = f'{alert.get("vulnerable_requirements")} -> {alert.get("first_patched_version")}'
         row.append(upgrade)
 
         return row
```

### Comparing `cycode-0.2.5.dev3/cycode/cli/printers/text_printer.py` & `cycode-0.2.5.dev4/cycode/cli/printers/text_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/user_settings/base_file_manager.py` & `cycode-0.2.5.dev4/cycode/cli/user_settings/base_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/user_settings/config_file_manager.py` & `cycode-0.2.5.dev4/cycode/cli/user_settings/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/user_settings/configuration_manager.py` & `cycode-0.2.5.dev4/cycode/cli/user_settings/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/user_settings/credentials_manager.py` & `cycode-0.2.5.dev4/cycode/cli/user_settings/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/user_settings/user_settings_commands.py` & `cycode-0.2.5.dev4/cycode/cli/user_settings/user_settings_commands.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/utils/path_utils.py` & `cycode-0.2.5.dev4/cycode/cli/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/utils/shell_executor.py` & `cycode-0.2.5.dev4/cycode/cli/utils/shell_executor.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/utils/string_utils.py` & `cycode-0.2.5.dev4/cycode/cli/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/utils/task_timer.py` & `cycode-0.2.5.dev4/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/utils/yaml_utils.py` & `cycode-0.2.5.dev4/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cli/zip_file.py` & `cycode-0.2.5.dev4/cycode/cli/zip_file.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cyclient/auth_client.py` & `cycode-0.2.5.dev4/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cyclient/config.py` & `cycode-0.2.5.dev4/cycode/cyclient/config.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cyclient/cycode_client_base.py` & `cycode-0.2.5.dev4/cycode/cyclient/cycode_client_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cyclient/cycode_dev_based_client.py` & `cycode-0.2.5.dev4/cycode/cyclient/cycode_dev_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cyclient/cycode_token_based_client.py` & `cycode-0.2.5.dev4/cycode/cyclient/cycode_token_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cyclient/models.py` & `cycode-0.2.5.dev4/cycode/cyclient/models.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cyclient/scan_client.py` & `cycode-0.2.5.dev4/cycode/cyclient/scan_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cyclient/scan_config/scan_config_base.py` & `cycode-0.2.5.dev4/cycode/cyclient/scan_config/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/cycode/cyclient/scan_config/scan_config_creator.py` & `cycode-0.2.5.dev4/cycode/cyclient/scan_config/scan_config_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.5.dev3/pyproject.toml` & `cycode-0.2.5.dev4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "0.2.5.dev3" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
+version = "0.2.5.dev4" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Perform secrets/iac scans for your sources using Cycode's engine"
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq-public/cycode-cli"
 readme = "README.md"
 classifiers = [
```

### Comparing `cycode-0.2.5.dev3/PKG-INFO` & `cycode-0.2.5.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 0.2.5.dev3
+Version: 0.2.5.dev4
 Summary: Perform secrets/iac scans for your sources using Cycode's engine
 Home-page: https://github.com/cycodehq-public/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<3.12
```

