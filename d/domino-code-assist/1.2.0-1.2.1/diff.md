# Comparing `tmp/domino_code_assist-1.2.0.tar.gz` & `tmp/domino_code_assist-1.2.1.tar.gz`

## Comparing `domino_code_assist-1.2.0.tar` & `domino_code_assist-1.2.1.tar`

### file list

```diff
@@ -1,110 +1,126 @@
--rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/DominoLogoGrey.svg
--rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/DominoLogoWhite.svg
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/__init__.py
--rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/action.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/action_ui.py
--rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/actions_store.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/app.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/app_entrypoint.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/code.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/code.vue
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/components.py
--rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/crossfilter_widgets.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/css.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/css.vue
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/df_select.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/df_select.vue
--rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/domino_api.py
--rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/domino_lab_mock.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/express.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/hooks.py
--rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/layout.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/logging_workaround.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/nb_app.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/py36.py
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/sample_project_md.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/serialize.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/settings.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/thumbnail.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/util.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/widgets.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/__init__.py
--rw-r--r--   0        0        0    25081 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/assistant.py
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/assistant.vue
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/drawer.py
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/drawer.vue
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/handle_user_install.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/menu.vue
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/mixpanel.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/mixpanel.vue
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/assistant/notebook.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/data/__init__.py
--rw-r--r--   0        0        0    19263 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/data/penguins.csv
--rw-r--r--   0        0        0   239436 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/data/small_molecule_drugbank.csv
--rw-r--r--   0        0        0     9951 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/data/stocks_long.parquet
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/app_checker.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/app_checker.vue
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/button_clipboard.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/button_clipboard.vue
--rw-r--r--   0        0        0    91330 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/deploy-sync.png
--rw-r--r--   0        0        0    27326 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/deployer.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/filesystem_watcher.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/deploy/filesystem_watcher.vue
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/jupyter/__init__.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/jupyter/mixpanel_handler.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/jupyter/server_extension.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/__init__.py
--rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/big_query.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/data_source.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/drawer.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/object_store.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/panel.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/quick_start.py
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/snowflake_redshift.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/load_data/state.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/playwright/__init__.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/playwright/app.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/playwright/assistant.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/playwright/load_data.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/playwright/notebook.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/playwright/transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/snippets/__init__.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/snippets/snippet_drawer.py
--rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/snippets/snippets.py
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/snippets/snippets_ui.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/snippets/tree.vue
--rw-r--r--   0        0        0  1192947 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/app.png
--rw-r--r--   0        0        0   530421 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/code_inserted.png
--rw-r--r--   0        0        0    17644 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/hover_cell.png
--rw-r--r--   0        0        0    35728 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/hover_icon.png
--rw-r--r--   0        0        0   357737 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/load_data.png
--rw-r--r--   0        0        0    93452 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/menu.png
--rw-r--r--   0        0        0    60379 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/menu_app.png
--rw-r--r--   0        0        0    61042 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/menu_transform.png
--rw-r--r--   0        0        0    60333 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/menu_visualizations.png
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/tour.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/tour.vue
--rw-r--r--   0        0        0   634871 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/transform.png
--rw-r--r--   0        0        0   587193 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/tour/visualizations.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/transform/__init__.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/transform/column_description.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/transform/column_description.vue
--rw-r--r--   0        0        0    13897 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/transform/transform_action_ui.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/transform/transform_drawer.py
--rw-r--r--   0        0        0     9843 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/transform/transform_panel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/viz/__init__.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/viz/drawer.py
--rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/viz/plot_builder.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/domino_code_assist/viz/state.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/low_code_assistant/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/low_code_assistant/app.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/low_code_assistant/app_entrypoint.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/low_code_assistant/deploy.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/low_code_assistant/express.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/low_code_assistant/layout.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/low_code_assistant/widgets.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/.gitignore
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/LICENSE.md
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 domino_code_assist-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7378 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/DominoLogoGrey.svg
+-rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/DominoLogoWhite.svg
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/__init__.py
+-rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/action.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/action_ui.py
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/actions_store.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/app.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/app_entrypoint.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/code.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/code.vue
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/components.py
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/crossfilter_widgets.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/css.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/css.vue
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/df_select.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/df_select.vue
+-rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/domino_api.py
+-rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/domino_lab_mock.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/express.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/hooks.py
+-rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/layout.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/logging_workaround.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/nb_app.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/py36.py
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/sample_project_md.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/serialize.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/settings.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/thumbnail.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/util.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/widgets.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/__init__.py
+-rw-r--r--   0        0        0    25812 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/assistant.py
+-rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/assistant.vue
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/drawer.py
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/drawer.vue
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/handle_user_install.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/menu.vue
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/mixpanel.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/mixpanel.vue
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/assistant/notebook.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/__init__.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/above_output.vue
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/code.py
+-rw-r--r--   0        0        0    29157 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/drawer.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/experiment_search.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/experiment_search.vue
+-rw-r--r--   0        0        0     8382 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/flaml_api.py
+-rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/hyper_parameters.py
+-rw-r--r--   0        0        0    13789 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/icon_classification.svg
+-rw-r--r--   0        0        0    18124 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/icon_forecasting.svg
+-rw-r--r--   0        0        0    16613 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/icon_regression.svg
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/open_experiment.py
+-rw-r--r--   0        0        0    14661 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/placeholder.png
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/select_description.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/select_description.vue
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/automl/store.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/data/__init__.py
+-rw-r--r--   0        0        0    19263 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/data/penguins.csv
+-rw-r--r--   0        0        0   239436 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/data/small_molecule_drugbank.csv
+-rw-r--r--   0        0        0     9951 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/data/stocks_long.parquet
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/app_checker.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/app_checker.vue
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/button_clipboard.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/button_clipboard.vue
+-rw-r--r--   0        0        0    91330 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/deploy-sync.png
+-rw-r--r--   0        0        0    27326 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/deployer.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/filesystem_watcher.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/deploy/filesystem_watcher.vue
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/jupyter/__init__.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/jupyter/mixpanel_handler.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/jupyter/server_extension.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/__init__.py
+-rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/big_query.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/data_source.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/drawer.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/object_store.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/panel.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/quick_start.py
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/snowflake_redshift.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/load_data/state.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/playwright/__init__.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/playwright/app.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/playwright/assistant.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/playwright/load_data.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/playwright/notebook.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/playwright/transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/snippets/__init__.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/snippets/snippet_drawer.py
+-rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/snippets/snippets.py
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/snippets/snippets_ui.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/snippets/tree.vue
+-rw-r--r--   0        0        0  1192947 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/app.png
+-rw-r--r--   0        0        0   530421 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/code_inserted.png
+-rw-r--r--   0        0        0    17644 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/hover_cell.png
+-rw-r--r--   0        0        0    35728 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/hover_icon.png
+-rw-r--r--   0        0        0   357737 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/load_data.png
+-rw-r--r--   0        0        0    93452 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/menu.png
+-rw-r--r--   0        0        0    60379 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/menu_app.png
+-rw-r--r--   0        0        0    61042 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/menu_transform.png
+-rw-r--r--   0        0        0    60333 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/menu_visualizations.png
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/tour.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/tour.vue
+-rw-r--r--   0        0        0   634871 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/transform.png
+-rw-r--r--   0        0        0   587193 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/tour/visualizations.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/transform/__init__.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/transform/column_description.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/transform/column_description.vue
+-rw-r--r--   0        0        0    13897 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/transform/transform_action_ui.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/transform/transform_drawer.py
+-rw-r--r--   0        0        0     9843 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/transform/transform_panel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/viz/__init__.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/viz/drawer.py
+-rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/viz/plot_builder.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/domino_code_assist/viz/state.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/low_code_assistant/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/low_code_assistant/app.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/low_code_assistant/app_entrypoint.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/low_code_assistant/deploy.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/low_code_assistant/express.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/low_code_assistant/layout.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/low_code_assistant/widgets.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/.gitignore
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/LICENSE.md
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 domino_code_assist-1.2.1/PKG-INFO
```

### Comparing `domino_code_assist-1.2.0/domino_code_assist/DominoLogoGrey.svg` & `domino_code_assist-1.2.1/domino_code_assist/DominoLogoGrey.svg`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/DominoLogoWhite.svg` & `domino_code_assist-1.2.1/domino_code_assist/DominoLogoWhite.svg`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/__init__.py` & `domino_code_assist-1.2.1/domino_code_assist/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Dominocode"""
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 import os
 
 # isort: skip_file
 
 import domino_code_assist.logging_workaround
 
 from . import data
 from .assistant import init
 from .components import MarkdownFromCell, CardGridLayout
-
+from .util import mlflow_log_notebook
 
 try:
     if not os.environ.get("DOMINO_PROJECT_ID"):
         from dotenv import load_dotenv
 
         load_dotenv()
 except ImportError:
```

### Comparing `domino_code_assist-1.2.0/domino_code_assist/action.py` & `domino_code_assist-1.2.1/domino_code_assist/action.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/action_ui.py` & `domino_code_assist-1.2.1/domino_code_assist/action_ui.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/actions_store.py` & `domino_code_assist-1.2.1/domino_code_assist/actions_store.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/app.py` & `domino_code_assist-1.2.1/domino_code_assist/app.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/app_entrypoint.py` & `domino_code_assist-1.2.1/domino_code_assist/app_entrypoint.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/code.py` & `domino_code_assist-1.2.1/domino_code_assist/code.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/code.vue` & `domino_code_assist-1.2.1/domino_code_assist/code.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/components.py` & `domino_code_assist-1.2.1/domino_code_assist/components.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/crossfilter_widgets.py` & `domino_code_assist-1.2.1/domino_code_assist/crossfilter_widgets.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/domino_api.py` & `domino_code_assist-1.2.1/domino_code_assist/domino_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -122,14 +122,36 @@
     def get_useable_environments(self):
         pass
 
     @abstractmethod
     def get_current_environment_id(self):
         pass
 
+    def get_experiments(self):
+        return [
+            {
+                "experiment_id": "17",
+                "name": "popular-fish-163",
+                "artifact_location": "mlflow-artifacts:/mlflow",
+                "lifecycle_stage": "active",
+                "last_update_time": 1682528255165,
+                "creation_time": 1682528255165,
+                "tags": [{"key": "mlflow.domino.project", "value": "DCA-latest"}],
+            },
+            {
+                "experiment_id": "16",
+                "name": "gaudy-donkey-172",
+                "artifact_location": "mlflow-artifacts:/mlflow",
+                "lifecycle_stage": "active",
+                "last_update_time": 1682514840966,
+                "creation_time": 1682514840966,
+                "tags": [{"key": "mlflow.domino.project", "value": "DCA-latest"}],
+            },
+        ]
+
 
 class DominoApi(IDominoApi):
     def get_datasource_list(self):
         project_id = settings.domino_project_id
         return self._get_domino_client().request_manager.get(f"{host}/v4/datasource/projects/{project_id}").json()
 
     def get_datasource_names(self):
@@ -223,7 +245,17 @@
         project_id = settings.domino_project_id
         run_id = settings.domino_run_id
         return (
             self._get_domino_client()
             .request_manager.get(f"{host}/v4/workspaces/{run_id}/runtimeExecutionDetails?projectId={project_id}")
             .json()["environment"]["environmentId"]
         )
+
+    def get_experiments(self):
+        project_id = settings.domino_project_id
+        return (
+            self._get_domino_client()
+            .request_manager.post(
+                f"{host}/api/2.0/mlflow/experiments/search", json={"max_results": 3000}, headers={"X-Domino-Mlflow-Data": f'{{ "projectId": "{project_id}" }}'}
+            )
+            .json()["experiments"]
+        )
```

### Comparing `domino_code_assist-1.2.0/domino_code_assist/domino_lab_mock.py` & `domino_code_assist-1.2.1/domino_code_assist/domino_lab_mock.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/layout.py` & `domino_code_assist-1.2.1/domino_code_assist/layout.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/nb_app.py` & `domino_code_assist-1.2.1/domino_code_assist/nb_app.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/py36.py` & `domino_code_assist-1.2.1/domino_code_assist/py36.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/sample_project_md.py` & `domino_code_assist-1.2.1/domino_code_assist/sample_project_md.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/serialize.py` & `domino_code_assist-1.2.1/domino_code_assist/serialize.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 import json
 
 import domino_code_assist.actions_store as actions_store
 import domino_code_assist.viz.state
 
 from . import action, crossfilter_widgets
+from .settings import settings
 
 
 class AEncoder(json.JSONEncoder):
     def default(self, obj):
         encoded = action.to_json(obj)
         if not encoded:
             encoded = actions_store.to_json(obj)
         if not encoded:
             encoded = crossfilter_widgets.to_json(obj)
         if not encoded:
             encoded = domino_code_assist.viz.state.to_json(obj)
+        if not encoded:
+            encoded = domino_code_assist.automl.store.to_json(obj)
         return encoded if encoded else json.JSONEncoder.default(self, obj)
 
 
 def from_json(dct):
     decoded = action.from_json(dct)
     if not decoded:
         decoded = actions_store.from_json(dct)
     if not decoded:
         decoded = domino_code_assist.viz.state.from_json(dct)
     if not decoded:
         decoded = crossfilter_widgets.from_json(dct)
+    if not decoded:
+        decoded = domino_code_assist.automl.store.from_json(dct)
     return decoded if decoded else dct
 
 
 def dumps(value):
     return json.dumps(value, cls=AEncoder)
 
 
 def loads(str):
-    data = json.loads(str, object_hook=from_json)
-    # convert previously stored action list to action state
-    if type(data) == list and len(data) > 0 and isinstance(data[0], action.Action):
-        data = actions_store.ActionsState(preview=True, actions=data)
-    return data
+    try:
+        data = json.loads(str, object_hook=from_json)
+        # convert previously stored action list to action state
+        if type(data) == list and len(data) > 0 and isinstance(data[0], action.Action):
+            data = actions_store.ActionsState(preview=True, actions=data)
+        return data
+    except Exception as e:
+        if settings.domino_code_assist_dev:
+            raise e
```

### Comparing `domino_code_assist-1.2.0/domino_code_assist/settings.py` & `domino_code_assist-1.2.1/domino_code_assist/settings.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/thumbnail.py` & `domino_code_assist-1.2.1/domino_code_assist/thumbnail.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/assistant/assistant.py` & `domino_code_assist-1.2.1/domino_code_assist/assistant/assistant.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 from domino_code_assist.layout import CardGridLayoutBuilder
 from domino_code_assist.serialize import dumps, loads
 from domino_code_assist.settings import settings
 from domino_code_assist.util import get_vars
 from domino_code_assist.viz.state import Viz
 
 from ..action import ActionFilter, ActionUseNbLocals
+from ..automl.drawer import AutoMlDrawer
+from ..automl.store import MLTask
 from ..crossfilter_widgets import WidgetState, _generate_map, to_json
 from ..load_data.drawer import LoadDataDrawer
 from ..snippets import snippets, snippets_ui
 from ..snippets.snippet_drawer import SnippetDrawer
 from ..tour.tour import TourWidget
 from ..transform.transform_drawer import TransformDrawer
 from ..viz import plot_builder
@@ -173,14 +175,19 @@
 items = [
     {
         "title": "Load data",
         "icon": "mdi-cloud-upload-outline",
         "action": "load_data",
     },
     {
+        "title": "AutoML",
+        "icon": "mdi-head-cog-outline",
+        "action": "automl",
+    },
+    {
         "title": "Transformations",
         "icon": "mdi-function-variant",
         "action": "transformations",
     },
     {
         "title": "Visualizations",
         "icon": "mdi-chart-bar-stacked",
@@ -210,14 +217,16 @@
 
 
 @reacton.component
 def Menu(selected, on_selected, decoded, snippet_edit_mode, on_snippet_edit_mode, disabled, overwrite):
     menu_action = None
     if decoded and decoded.__class__ in [action.ActionOpen, action.ActionDownloadDataSource, action.ActionDemo]:
         menu_action = "load_data"
+    elif decoded and type(decoded) == MLTask:
+        menu_action = "automl"
     elif decoded and isinstance(decoded, actions_store.ActionsState):
         menu_action = "transformations"
     elif decoded and type(decoded) == Viz:
         menu_action = "visualizations"
     elif decoded and isinstance(decoded, crossfilter_widgets.WidgetState):
         menu_action = "x-widgets"
     elif decoded and "type_card_grid_layout" in decoded:
@@ -573,14 +582,25 @@
             set_code,
             open=(selected and selected.get("action")) == "load_data",
             edit=selected and selected.get("edit"),
             on_close=lambda: set_selected(None),
             overwrite_warning=overwrite_warning,
         ).meta(ref="load_data")
 
+        AutoMlDrawer(
+            edit_data,
+            set_code,
+            dfs,
+            is_open=(selected and selected.get("action")) == "automl",
+            edit=selected and selected.get("edit"),
+            on_close=lambda: set_selected(None),
+            on_load_own_data=lambda: set_selected({"title": "Load data", "icon": "mdi-cloud-upload-outline", "action": "load_data"}),
+            overwrite_warning=overwrite_warning,
+        ).key("automl-drawer")
+
         TransformDrawer(
             edit_data,
             set_code,
             dfs,
             open=(selected and selected.get("action")) == "transformations",
             edit=selected and selected.get("edit"),
             on_close=lambda: set_selected(None),
```

### Comparing `domino_code_assist-1.2.0/domino_code_assist/assistant/assistant.vue` & `domino_code_assist-1.2.1/domino_code_assist/assistant/assistant.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/assistant/drawer.py` & `domino_code_assist-1.2.1/domino_code_assist/assistant/drawer.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     edit = traitlets.Bool(False).tag(sync=True)
     apply_disabled = traitlets.Bool(False).tag(sync=True)
     show_var_out = traitlets.Bool(False).tag(sync=True)
     var_out = traitlets.Unicode().tag(sync=True)
     valid_variable_name = traitlets.Bool(True).tag(sync=True)
     width = traitlets.Unicode("unset").tag(sync=True)
     warning_widget = traitlets.Any().tag(sync=True, **ipywidgets.widget_serialization)
+    class_ = traitlets.Unicode("").tag(sync=True)
 
     def vue_apply(self, *ignored):
         self.on_apply and self.on_apply()
 
 
 @reacton.component
 def RightDrawer(
@@ -40,14 +41,15 @@
     edit: bool = False,
     apply_disabled: bool = False,
     show_var_out: bool = False,
     var_out: str = "",
     on_var_out: Optional[Callable[[str], None]] = lambda *_: None,
     width: str = "unset",
     warning_widget: Optional[reacton.core.Element] = None,
+    class_: str = "",
 ):
     valid_variable_name = util.is_valid_variable_name(var_out)
 
     content = None
     if children and len(children) == 1:
         content = children[0]
     elif children:
@@ -63,8 +65,9 @@
         apply_disabled=(show_var_out and not valid_variable_name) or apply_disabled,
         show_var_out=show_var_out,
         var_out=var_out,
         on_var_out=on_var_out,
         valid_variable_name=valid_variable_name,
         width=width,
         warning_widget=warning_widget,
+        class_=class_,
     )
```

### Comparing `domino_code_assist-1.2.0/domino_code_assist/assistant/drawer.vue` & `domino_code_assist-1.2.1/domino_code_assist/assistant/drawer.vue`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <template>
   <div>
     <v-bottom-sheet v-model="is_open" :width="width" transition="right-sheet-transition">
-      <v-card :class="['domino-right-sheet', inIframe && 'domino-right-sheet--in-iframe']">
+      <v-card :class="['domino-right-sheet', inIframe && 'domino-right-sheet--in-iframe', class_]">
         <v-card-title class_="text-h5" style="background-color: #2d71c7; color: white">
           <span>{{ title }}</span>
           <v-spacer></v-spacer>
           <v-btn icon dark @click="is_open = false">
             <v-icon>mdi-close</v-icon>
           </v-btn>
         </v-card-title>
```

### Comparing `domino_code_assist-1.2.0/domino_code_assist/assistant/handle_user_install.py` & `domino_code_assist-1.2.1/domino_code_assist/assistant/handle_user_install.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/assistant/menu.vue` & `domino_code_assist-1.2.1/domino_code_assist/assistant/menu.vue`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     <template v-slot:activator="{ on }">
       <v-btn v-on="on" color="primary" rounded small style="min-width: 28px; padding: 0; margin: 2px" :disabled="disabled">
         <v-img :src="logo" style="height: 16px; max-width: 16px; border-radius: 8px"/>
       </v-btn>
     </template>
     <v-list flat dense>
       <v-list-item-group
-          v-model="selected"
-          @change="(item) => {if (item) {overlay_open = true}}"
+          :value="selected"
+          @change="setSelected"
           color="primary"
       >
         <template v-for="item in items">
           <v-list-item
               :key="item.action"
               :value="item"
           >
@@ -50,7 +50,21 @@
           <v-divider v-if="item.divider" :key="'div'+item"></v-divider>
         </template>
       </v-list-item-group>
     </v-list>
   </v-menu>
   </div>
 </template>
+<script>
+  module.exports = {
+    methods: {
+      setSelected(item) {
+        if (!DCA.kernelBusy(DCA.getNotebookId(this.$el))) {
+          if (item) {
+            this.overlay_open = true
+          }
+          this.selected = item
+        }
+      }
+    },
+  }
+</script>
```

### Comparing `domino_code_assist-1.2.0/domino_code_assist/assistant/mixpanel.py` & `domino_code_assist-1.2.1/domino_code_assist/assistant/mixpanel.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/assistant/mixpanel.vue` & `domino_code_assist-1.2.1/domino_code_assist/assistant/mixpanel.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/data/penguins.csv` & `domino_code_assist-1.2.1/domino_code_assist/data/penguins.csv`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/data/small_molecule_drugbank.csv` & `domino_code_assist-1.2.1/domino_code_assist/data/small_molecule_drugbank.csv`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/data/stocks_long.parquet` & `domino_code_assist-1.2.1/domino_code_assist/data/stocks_long.parquet`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/deploy/app_checker.py` & `domino_code_assist-1.2.1/domino_code_assist/deploy/app_checker.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/deploy/app_checker.vue` & `domino_code_assist-1.2.1/domino_code_assist/deploy/app_checker.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/deploy/button_clipboard.vue` & `domino_code_assist-1.2.1/domino_code_assist/deploy/button_clipboard.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/deploy/deploy-sync.png` & `domino_code_assist-1.2.1/domino_code_assist/deploy/deploy-sync.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/deploy/deployer.py` & `domino_code_assist-1.2.1/domino_code_assist/deploy/deployer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/deploy/filesystem_watcher.py` & `domino_code_assist-1.2.1/domino_code_assist/deploy/filesystem_watcher.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/deploy/filesystem_watcher.vue` & `domino_code_assist-1.2.1/domino_code_assist/deploy/filesystem_watcher.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/jupyter/mixpanel_handler.py` & `domino_code_assist-1.2.1/domino_code_assist/jupyter/mixpanel_handler.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/jupyter/server_extension.py` & `domino_code_assist-1.2.1/domino_code_assist/jupyter/server_extension.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/load_data/big_query.py` & `domino_code_assist-1.2.1/domino_code_assist/load_data/big_query.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/load_data/data_source.py` & `domino_code_assist-1.2.1/domino_code_assist/load_data/data_source.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/load_data/drawer.py` & `domino_code_assist-1.2.1/domino_code_assist/load_data/drawer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/load_data/object_store.py` & `domino_code_assist-1.2.1/domino_code_assist/load_data/object_store.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/load_data/panel.py` & `domino_code_assist-1.2.1/domino_code_assist/load_data/panel.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/load_data/quick_start.py` & `domino_code_assist-1.2.1/domino_code_assist/load_data/quick_start.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/load_data/snowflake_redshift.py` & `domino_code_assist-1.2.1/domino_code_assist/load_data/snowflake_redshift.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/load_data/state.py` & `domino_code_assist-1.2.1/domino_code_assist/load_data/state.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/playwright/app.py` & `domino_code_assist-1.2.1/domino_code_assist/playwright/app.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/playwright/assistant.py` & `domino_code_assist-1.2.1/domino_code_assist/playwright/assistant.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/playwright/load_data.py` & `domino_code_assist-1.2.1/domino_code_assist/playwright/load_data.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/playwright/notebook.py` & `domino_code_assist-1.2.1/domino_code_assist/playwright/notebook.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/playwright/transform.py` & `domino_code_assist-1.2.1/domino_code_assist/playwright/transform.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/snippets/snippet_drawer.py` & `domino_code_assist-1.2.1/domino_code_assist/snippets/snippet_drawer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/snippets/snippets.py` & `domino_code_assist-1.2.1/domino_code_assist/snippets/snippets.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/snippets/snippets_ui.py` & `domino_code_assist-1.2.1/domino_code_assist/snippets/snippets_ui.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/snippets/tree.vue` & `domino_code_assist-1.2.1/domino_code_assist/snippets/tree.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/tour/app.png` & `domino_code_assist-1.2.1/domino_code_assist/tour/app.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/tour/code_inserted.png` & `domino_code_assist-1.2.1/domino_code_assist/tour/code_inserted.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/tour/hover_cell.png` & `domino_code_assist-1.2.1/domino_code_assist/tour/hover_cell.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/tour/hover_icon.png` & `domino_code_assist-1.2.1/domino_code_assist/tour/hover_icon.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/tour/load_data.png` & `domino_code_assist-1.2.1/domino_code_assist/tour/load_data.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/tour/menu.png` & `domino_code_assist-1.2.1/domino_code_assist/tour/menu.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/tour/menu_app.png` & `domino_code_assist-1.2.1/domino_code_assist/tour/menu_app.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/tour/menu_transform.png` & `domino_code_assist-1.2.1/domino_code_assist/tour/menu_transform.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/tour/menu_visualizations.png` & `domino_code_assist-1.2.1/domino_code_assist/tour/menu_visualizations.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/tour/tour.py` & `domino_code_assist-1.2.1/domino_code_assist/tour/tour.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/tour/tour.vue` & `domino_code_assist-1.2.1/domino_code_assist/tour/tour.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/tour/transform.png` & `domino_code_assist-1.2.1/domino_code_assist/tour/transform.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/tour/visualizations.png` & `domino_code_assist-1.2.1/domino_code_assist/tour/visualizations.png`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/transform/column_description.py` & `domino_code_assist-1.2.1/domino_code_assist/transform/column_description.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/transform/column_description.vue` & `domino_code_assist-1.2.1/domino_code_assist/transform/column_description.vue`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/transform/transform_action_ui.py` & `domino_code_assist-1.2.1/domino_code_assist/transform/transform_action_ui.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/transform/transform_drawer.py` & `domino_code_assist-1.2.1/domino_code_assist/transform/transform_drawer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/transform/transform_panel.py` & `domino_code_assist-1.2.1/domino_code_assist/transform/transform_panel.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/viz/drawer.py` & `domino_code_assist-1.2.1/domino_code_assist/viz/drawer.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/viz/plot_builder.py` & `domino_code_assist-1.2.1/domino_code_assist/viz/plot_builder.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/domino_code_assist/viz/state.py` & `domino_code_assist-1.2.1/domino_code_assist/viz/state.py`

 * *Files identical despite different names*

### Comparing `domino_code_assist-1.2.0/pyproject.toml` & `domino_code_assist-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,31 +7,39 @@
 #authors = [
 #    {name = "Maarten A. Breddels", email = "maartenbreddels@gmail.com"},
 #    {name = "Mario Buikhuizen", email = "mariobuikhuizen@gmail.com"}]
 # license = {file = "LICENSE"}
 # classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 dependencies = [
-    "reacton~=1.5.0",
-    "solara[assets]~=1.10.0",
+    "reacton~=1.6.0",
+    "solara[assets]~=1.13.0",
     "ipyvue",
-    "ipyvuetify",
+    "ipyvuetify>=1.8.5",
     "ipywidgets<8",
     "pandas",
     "plotly>=5.5",
     "dominodatalab; python_version >= '3.8'",
     "humanize",
     "pydantic",
     "nbformat>=4.5",  # to support cell ids
     "notebook>=4.6",  # to support cell ids
     "openpyxl",
     "xlrd",
     "vaex-core",
+    "flaml",
+    "mlflow",
+    "lightgbm",
+    "hcrystalball",
+    "statsmodels",
 ]
 
+[tool.hatch.metadata]
+allow-direct-references = true
+
 [tool.hatch.version]
 path = "domino_code_assist/__init__.py"
 
 [tool.hatch.build.targets.wheel]
 packages = ["low_code_assistant", "domino_code_assist"]
 
 [tool.hatch.build.targets.sdist]
```

### Comparing `domino_code_assist-1.2.0/PKG-INFO` & `domino_code_assist-1.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: domino-code-assist
-Version: 1.2.0
+Version: 1.2.1
 Project-URL: Home, https://github.com/cerebrotech/domino-code-assist
 License-File: LICENSE.md
 Requires-Dist: dominodatalab; python_version >= '3.8'
+Requires-Dist: flaml
+Requires-Dist: hcrystalball
 Requires-Dist: humanize
 Requires-Dist: ipyvue
-Requires-Dist: ipyvuetify
+Requires-Dist: ipyvuetify>=1.8.5
 Requires-Dist: ipywidgets<8
+Requires-Dist: lightgbm
+Requires-Dist: mlflow
 Requires-Dist: nbformat>=4.5
 Requires-Dist: notebook>=4.6
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: plotly>=5.5
 Requires-Dist: pydantic
-Requires-Dist: reacton~=1.5.0
-Requires-Dist: solara[assets]~=1.10.0
+Requires-Dist: reacton~=1.6.0
+Requires-Dist: solara[assets]~=1.13.0
+Requires-Dist: statsmodels
 Requires-Dist: vaex-core
 Requires-Dist: xlrd
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: bump2version; extra == 'dev'
 Requires-Dist: dominodatalab-data; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
```

