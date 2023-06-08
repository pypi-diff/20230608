# Comparing `tmp/dbt_coves-1.5.5.tar.gz` & `tmp/dbt_coves-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_coves-1.5.5.tar", max compression
+gzip compressed data, was "dbt_coves-1.5.6.tar", max compression
```

## Comparing `dbt_coves-1.5.5.tar` & `dbt_coves-1.5.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    11357 2023-06-08 16:03:58.638032 dbt_coves-1.5.5/LICENSE
--rw-r--r--   0        0        0    22554 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/README.md
--rw-r--r--   0        0        0       22 2023-06-08 16:04:38.145759 dbt_coves-1.5.5/dbt_coves/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/config/__init__.py
--rw-r--r--   0        0        0     9769 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/config/config.py
--rw-r--r--   0        0        0        0 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/core/__init__.py
--rw-r--r--   0        0        0      650 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/core/exceptions.py
--rw-r--r--   0        0        0     8193 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/core/main.py
--rw-r--r--   0        0        0        0 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/__init__.py
--rw-r--r--   0        0        0     3008 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/base.py
--rw-r--r--   0        0        0     5056 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/dbt/main.py
--rw-r--r--   0        0        0        0 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/extract/__init__.py
--rw-r--r--   0        0        0    12365 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/extract/airbyte.py
--rw-r--r--   0        0        0      475 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/extract/base.py
--rw-r--r--   0        0        0     4574 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/extract/fivetran.py
--rw-r--r--   0        0        0      963 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/extract/main.py
--rw-r--r--   0        0        0        0 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/generate/__init__.py
--rw-r--r--   0        0        0    18472 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/generate/base.py
--rw-r--r--   0        0        0     1329 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/generate/main.py
--rw-r--r--   0        0        0    10624 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/generate/metadata.py
--rw-r--r--   0        0        0     8942 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/generate/properties.py
--rw-r--r--   0        0        0    15026 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/generate/sources.py
--rw-r--r--   0        0        0     2715 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/generate/templates.py
--rw-r--r--   0        0        0        0 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/load/__init__.py
--rw-r--r--   0        0        0    25744 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/load/airbyte.py
--rw-r--r--   0        0        0     2259 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/load/base.py
--rw-r--r--   0        0        0    18452 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/load/fivetran.py
--rw-r--r--   0        0        0      946 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/load/main.py
--rw-r--r--   0        0        0        0 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/setup/__init__.py
--rw-r--r--   0        0        0      494 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/setup/base.py
--rw-r--r--   0        0        0     4287 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/setup/dbt.py
--rw-r--r--   0        0        0     6751 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/setup/git.py
--rw-r--r--   0        0        0     1214 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/setup/main.py
--rw-r--r--   0        0        0     1664 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/setup/pre_commit.py
--rw-r--r--   0        0        0    10262 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/setup/ssh.py
--rw-r--r--   0        0        0      845 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/setup/templates/pre_commit/copier.yml
--rw-r--r--   0        0        0     2110 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja
--rw-r--r--   0        0        0       75 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluffignore{% endif %}
--rw-r--r--   0        0        0     2743 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja
--rw-r--r--   0        0        0      668 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}
--rw-r--r--   0        0        0      102 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{{ _copier_conf.answers_file }}-precommit.yaml.jinja
--rw-r--r--   0        0        0     1371 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/tasks/setup/utils.py
--rw-r--r--   0        0        0      255 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/templates/model_props.yml
--rw-r--r--   0        0        0      214 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/templates/source_props.yml
--rw-r--r--   0        0        0     1201 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/templates/staging_model.sql
--rw-r--r--   0        0        0      495 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/templates/staging_model_props.yml
--rw-r--r--   0        0        0        0 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/ui/__init__.py
--rw-r--r--   0        0        0     1202 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/ui/traceback.py
--rw-r--r--   0        0        0        0 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/utils/__init__.py
--rw-r--r--   0        0        0    11270 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/utils/api_caller.py
--rw-r--r--   0        0        0    14980 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/utils/flags.py
--rw-r--r--   0        0        0     1132 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/utils/jinja.py
--rw-r--r--   0        0        0      785 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/utils/log.py
--rw-r--r--   0        0        0      791 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/utils/shell.py
--rw-r--r--   0        0        0     1872 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/utils/tracking.py
--rw-r--r--   0        0        0     1010 2023-06-08 16:03:58.642032 dbt_coves-1.5.5/dbt_coves/utils/yaml.py
--rw-r--r--   0        0        0     3606 2023-06-08 16:04:38.141759 dbt_coves-1.5.5/pyproject.toml
--rw-r--r--   0        0        0    24503 1970-01-01 00:00:00.000000 dbt_coves-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/LICENSE
+-rw-r--r--   0        0        0    22554 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/README.md
+-rw-r--r--   0        0        0       22 2023-06-08 16:10:27.342454 dbt_coves-1.5.6/dbt_coves/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/config/__init__.py
+-rw-r--r--   0        0        0     9769 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/config/config.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/core/__init__.py
+-rw-r--r--   0        0        0      650 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/core/exceptions.py
+-rw-r--r--   0        0        0     8193 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/core/main.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/__init__.py
+-rw-r--r--   0        0        0     3008 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/base.py
+-rw-r--r--   0        0        0     5056 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/dbt/main.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/extract/__init__.py
+-rw-r--r--   0        0        0    12365 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/extract/airbyte.py
+-rw-r--r--   0        0        0      475 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/extract/base.py
+-rw-r--r--   0        0        0     4574 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/extract/fivetran.py
+-rw-r--r--   0        0        0      963 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/extract/main.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/generate/__init__.py
+-rw-r--r--   0        0        0    18472 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/generate/base.py
+-rw-r--r--   0        0        0     1329 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/generate/main.py
+-rw-r--r--   0        0        0    10624 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/generate/metadata.py
+-rw-r--r--   0        0        0     8942 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/generate/properties.py
+-rw-r--r--   0        0        0    15026 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/generate/sources.py
+-rw-r--r--   0        0        0     2715 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/generate/templates.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:09:49.081959 dbt_coves-1.5.6/dbt_coves/tasks/load/__init__.py
+-rw-r--r--   0        0        0    25744 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/load/airbyte.py
+-rw-r--r--   0        0        0     2259 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/load/base.py
+-rw-r--r--   0        0        0    18452 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/load/fivetran.py
+-rw-r--r--   0        0        0      946 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/load/main.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/setup/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/setup/base.py
+-rw-r--r--   0        0        0     4287 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/setup/dbt.py
+-rw-r--r--   0        0        0     6751 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/setup/git.py
+-rw-r--r--   0        0        0     1214 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/setup/main.py
+-rw-r--r--   0        0        0     1664 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/setup/pre_commit.py
+-rw-r--r--   0        0        0    10262 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/setup/ssh.py
+-rw-r--r--   0        0        0      845 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/setup/templates/pre_commit/copier.yml
+-rw-r--r--   0        0        0     2110 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja
+-rw-r--r--   0        0        0       75 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluffignore{% endif %}
+-rw-r--r--   0        0        0     2743 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja
+-rw-r--r--   0        0        0      668 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}
+-rw-r--r--   0        0        0      102 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{{ _copier_conf.answers_file }}-precommit.yaml.jinja
+-rw-r--r--   0        0        0     1371 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/tasks/setup/utils.py
+-rw-r--r--   0        0        0      255 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/templates/model_props.yml
+-rw-r--r--   0        0        0      214 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/templates/source_props.yml
+-rw-r--r--   0        0        0     1201 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/templates/staging_model.sql
+-rw-r--r--   0        0        0      495 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/templates/staging_model_props.yml
+-rw-r--r--   0        0        0        0 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/ui/__init__.py
+-rw-r--r--   0        0        0     1202 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/ui/traceback.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/utils/__init__.py
+-rw-r--r--   0        0        0    11270 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/utils/api_caller.py
+-rw-r--r--   0        0        0    14980 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/utils/flags.py
+-rw-r--r--   0        0        0     1132 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/utils/jinja.py
+-rw-r--r--   0        0        0      785 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/utils/log.py
+-rw-r--r--   0        0        0      791 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/utils/shell.py
+-rw-r--r--   0        0        0     1872 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/utils/tracking.py
+-rw-r--r--   0        0        0     1010 2023-06-08 16:09:49.085959 dbt_coves-1.5.6/dbt_coves/utils/yaml.py
+-rw-r--r--   0        0        0     3606 2023-06-08 16:10:27.342454 dbt_coves-1.5.6/pyproject.toml
+-rw-r--r--   0        0        0    24503 1970-01-01 00:00:00.000000 dbt_coves-1.5.6/PKG-INFO
```

### Comparing `dbt_coves-1.5.5/LICENSE` & `dbt_coves-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/README.md` & `dbt_coves-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/config/config.py` & `dbt_coves-1.5.6/dbt_coves/config/config.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/core/exceptions.py` & `dbt_coves-1.5.6/dbt_coves/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/core/main.py` & `dbt_coves-1.5.6/dbt_coves/core/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/base.py` & `dbt_coves-1.5.6/dbt_coves/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/dbt/main.py` & `dbt_coves-1.5.6/dbt_coves/tasks/dbt/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/extract/airbyte.py` & `dbt_coves-1.5.6/dbt_coves/tasks/extract/airbyte.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/extract/fivetran.py` & `dbt_coves-1.5.6/dbt_coves/tasks/extract/fivetran.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/extract/main.py` & `dbt_coves-1.5.6/dbt_coves/tasks/extract/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/generate/base.py` & `dbt_coves-1.5.6/dbt_coves/tasks/generate/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/generate/main.py` & `dbt_coves-1.5.6/dbt_coves/tasks/generate/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/generate/metadata.py` & `dbt_coves-1.5.6/dbt_coves/tasks/generate/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/generate/properties.py` & `dbt_coves-1.5.6/dbt_coves/tasks/generate/properties.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/generate/sources.py` & `dbt_coves-1.5.6/dbt_coves/tasks/generate/sources.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/generate/templates.py` & `dbt_coves-1.5.6/dbt_coves/tasks/generate/templates.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/load/airbyte.py` & `dbt_coves-1.5.6/dbt_coves/tasks/load/airbyte.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/load/base.py` & `dbt_coves-1.5.6/dbt_coves/tasks/load/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/load/fivetran.py` & `dbt_coves-1.5.6/dbt_coves/tasks/load/fivetran.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/load/main.py` & `dbt_coves-1.5.6/dbt_coves/tasks/load/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/setup/dbt.py` & `dbt_coves-1.5.6/dbt_coves/tasks/setup/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/setup/git.py` & `dbt_coves-1.5.6/dbt_coves/tasks/setup/git.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/setup/main.py` & `dbt_coves-1.5.6/dbt_coves/tasks/setup/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/setup/pre_commit.py` & `dbt_coves-1.5.6/dbt_coves/tasks/setup/pre_commit.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/setup/ssh.py` & `dbt_coves-1.5.6/dbt_coves/tasks/setup/ssh.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/setup/templates/pre_commit/copier.yml` & `dbt_coves-1.5.6/dbt_coves/tasks/setup/templates/pre_commit/copier.yml`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja` & `dbt_coves-1.5.6/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja` & `dbt_coves-1.5.6/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}` & `dbt_coves-1.5.6/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/tasks/setup/utils.py` & `dbt_coves-1.5.6/dbt_coves/tasks/setup/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/templates/staging_model.sql` & `dbt_coves-1.5.6/dbt_coves/templates/staging_model.sql`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/ui/traceback.py` & `dbt_coves-1.5.6/dbt_coves/ui/traceback.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/utils/api_caller.py` & `dbt_coves-1.5.6/dbt_coves/utils/api_caller.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/utils/flags.py` & `dbt_coves-1.5.6/dbt_coves/utils/flags.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/utils/jinja.py` & `dbt_coves-1.5.6/dbt_coves/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/utils/log.py` & `dbt_coves-1.5.6/dbt_coves/utils/log.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/utils/shell.py` & `dbt_coves-1.5.6/dbt_coves/utils/shell.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/utils/tracking.py` & `dbt_coves-1.5.6/dbt_coves/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/dbt_coves/utils/yaml.py` & `dbt_coves-1.5.6/dbt_coves/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.5/pyproject.toml` & `dbt_coves-1.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt_coves"
-version = "1.5.5"
+version = "1.5.6"
 description = "CLI tool for dbt users adopting analytics engineering best practices."
 authors = ["Datacoves <hello@datacoves.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Information Technology",
```

### Comparing `dbt_coves-1.5.5/PKG-INFO` & `dbt_coves-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-coves
-Version: 1.5.5
+Version: 1.5.6
 Summary: CLI tool for dbt users adopting analytics engineering best practices.
 Home-page: https://datacoves.com
 License: Apache 2.0
 Keywords: data engineering,analytics engineering,dbt,ETL,data modelling
 Author: Datacoves
 Author-email: hello@datacoves.com
 Requires-Python: >=3.7.2,<3.11
```

