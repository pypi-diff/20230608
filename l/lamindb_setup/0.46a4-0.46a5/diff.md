# Comparing `tmp/lamindb_setup-0.46a4.tar.gz` & `tmp/lamindb_setup-0.46a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.46a4.tar", last modified: Mon Jun  5 12:59:52 2023, max compression
+gzip compressed data, was "lamindb_setup-0.46a5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.46a4.tar` & `lamindb_setup-0.46a5.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     4010 2023-06-04 10:03:32.188588 lamindb_setup-0.46a4/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.46a4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.46a4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.46a4/.gitignore
--rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.46a4/.gitmodules
--rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.46a4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.46a4/LICENSE
--rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.46a4/README.md
--rw-r--r--   0        0        0       52 2023-05-26 12:29:21.559991 lamindb_setup-0.46a4/docs/api.md
--rw-r--r--   0        0        0    51804 2023-06-05 12:59:32.556986 lamindb_setup-0.46a4/docs/changelog.md
--rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.46a4/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0       96 2023-06-04 10:03:32.190096 lamindb_setup-0.46a4/docs/faq/index.md
--rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.46a4/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     5058 2023-06-04 16:47:53.812781 lamindb_setup-0.46a4/docs/faq/test-sqlite-sync.ipynb
--rw-r--r--   0        0        0     8821 2023-06-04 17:52:00.959624 lamindb_setup-0.46a4/docs/guide/00-index.ipynb
--rw-r--r--   0        0        0     5037 2023-06-01 11:33:10.499992 lamindb_setup-0.46a4/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0     8081 2023-06-01 11:33:10.500188 lamindb_setup-0.46a4/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     4342 2023-06-01 11:33:10.500381 lamindb_setup-0.46a4/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     5750 2023-06-04 11:49:29.988148 lamindb_setup-0.46a4/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3271 2023-06-04 11:49:29.988389 lamindb_setup-0.46a4/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     3331 2023-05-26 12:29:21.561700 lamindb_setup-0.46a4/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-05-26 12:29:21.561778 lamindb_setup-0.46a4/docs/index.md
--rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.46a4/docs/test_notebooks.py
--rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.46a4/lamin-project.yaml
--rw-r--r--   0        0        0     2626 2023-06-05 12:59:06.828598 lamindb_setup-0.46a4/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5344 2023-06-04 19:41:00.162639 lamindb_setup-0.46a4/lamindb_setup/__main__.py
--rw-r--r--   0        0        0     1410 2023-06-05 07:31:40.592921 lamindb_setup-0.46a4/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      567 2023-06-01 11:33:10.501880 lamindb_setup-0.46a4/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2182 2023-06-01 11:33:10.502044 lamindb_setup-0.46a4/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.46a4/lamindb_setup/_docstrings.py
--rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.46a4/lamindb_setup/_info.py
--rw-r--r--   0        0        0     6969 2023-06-05 12:38:39.756205 lamindb_setup-0.46a4/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     6073 2023-06-04 19:41:00.163584 lamindb_setup-0.46a4/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0      322 2023-06-04 10:03:32.191280 lamindb_setup-0.46a4/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0     1692 2023-06-03 14:40:15.909532 lamindb_setup-0.46a4/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      825 2023-06-04 19:41:00.163739 lamindb_setup-0.46a4/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.46a4/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     1857 2023-06-04 19:41:00.164149 lamindb_setup-0.46a4/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.46a4/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.46a4/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.46a4/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3548 2023-06-04 19:41:00.164398 lamindb_setup-0.46a4/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      785 2023-06-04 19:41:00.164608 lamindb_setup-0.46a4/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.46a4/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.46a4/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0     2546 2023-06-04 19:41:00.164891 lamindb_setup-0.46a4/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.46a4/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-06-01 11:33:10.505542 lamindb_setup-0.46a4/lamindb_setup/dev/_exclusion.py
--rw-r--r--   0        0        0     8983 2023-06-04 19:41:00.165203 lamindb_setup-0.46a4/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.46a4/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.46a4/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.46a4/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.46a4/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     3419 2023-06-04 19:41:00.165550 lamindb_setup-0.46a4/lamindb_setup/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     2140 2023-06-05 07:31:40.593368 lamindb_setup-0.46a4/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     5057 2023-06-04 11:49:29.989719 lamindb_setup-0.46a4/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2563 2023-06-04 19:41:00.165849 lamindb_setup-0.46a4/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0     2811 2023-06-02 12:28:18.951248 lamindb_setup-0.46a4/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.46a4/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-30 14:21:30.384364 lamindb_setup-0.46a4/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.46a4/lnschema-core/.gitignore
--rw-r--r--   0        0        0        0 2023-06-02 12:28:18.951387 lamindb_setup-0.46a4/lnschema-core/.gitmodules
--rw-r--r--   0        0        0     1836 2023-05-30 14:21:30.384687 lamindb_setup-0.46a4/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.46a4/lnschema-core/LICENSE
--rw-r--r--   0        0        0      364 2023-05-30 14:21:30.384850 lamindb_setup-0.46a4/lnschema-core/README.md
--rw-r--r--   0        0        0    25152 2023-06-04 14:18:28.863714 lamindb_setup-0.46a4/lnschema-core/docs/changelog.md
--rw-r--r--   0        0        0     1485 2023-06-04 11:09:43.036808 lamindb_setup-0.46a4/lnschema-core/docs/guide/core-schema.ipynb
--rw-r--r--   0        0        0       52 2023-06-04 11:09:43.037197 lamindb_setup-0.46a4/lnschema-core/docs/guide/index.md
--rw-r--r--   0        0        0      112 2023-05-30 14:21:30.386018 lamindb_setup-0.46a4/lnschema-core/docs/index.md
--rw-r--r--   0        0        0      202 2023-05-30 14:21:30.386086 lamindb_setup-0.46a4/lnschema-core/lamin-project.yaml
--rw-r--r--   0        0        0      544 2023-06-04 14:18:28.863945 lamindb_setup-0.46a4/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0     1515 2023-06-04 14:18:28.864113 lamindb_setup-0.46a4/lnschema-core/lnschema_core/_lookup.py
--rw-r--r--   0        0        0      740 2023-06-04 14:37:07.398773 lamindb_setup-0.46a4/lnschema-core/lnschema_core/_types.py
--rw-r--r--   0        0        0      349 2023-06-02 12:28:18.953894 lamindb_setup-0.46a4/lnschema-core/lnschema_core/_users.py
--rw-r--r--   0        0        0     2810 2023-06-04 11:09:43.037807 lamindb_setup-0.46a4/lnschema-core/lnschema_core/ids.py
--rw-r--r--   0        0        0     9848 2023-06-05 09:38:49.986505 lamindb_setup-0.46a4/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.46a4/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0    21409 2023-06-04 14:37:07.399082 lamindb_setup-0.46a4/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      180 2023-06-04 14:37:07.399765 lamindb_setup-0.46a4/lnschema-core/lnschema_core/types.py
--rw-r--r--   0        0        0     1283 2023-06-04 14:18:28.865001 lamindb_setup-0.46a4/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      850 2023-06-04 14:37:07.399971 lamindb_setup-0.46a4/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0      475 2023-05-30 14:21:30.392155 lamindb_setup-0.46a4/lnschema-core/tests/test_notebooks.py
--rw-r--r--   0        0        0     1814 2023-06-04 07:52:37.336139 lamindb_setup-0.46a4/noxfile.py
--rw-r--r--   0        0        0     1337 2023-06-05 12:57:21.542553 lamindb_setup-0.46a4/pyproject.toml
--rw-r--r--   0        0        0      672 2023-06-04 11:49:29.990032 lamindb_setup-0.46a4/tests/test_bionty.py
--rw-r--r--   0        0        0     3041 2023-06-01 11:33:10.508406 lamindb_setup-0.46a4/tests/test_init_instance.py
--rw-r--r--   0        0        0      655 2023-06-01 11:33:10.508620 lamindb_setup-0.46a4/tests/test_load_instance.py
--rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.46a4/tests/test_set_storage.py
--rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.46a4/PKG-INFO
+-rw-r--r--   0        0        0     4010 2023-06-05 07:30:18.302219 lamindb_setup-0.46a5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-06-01 15:58:18.274054 lamindb_setup-0.46a5/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-06-01 15:58:18.274134 lamindb_setup-0.46a5/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-06-01 15:58:18.274221 lamindb_setup-0.46a5/.gitignore
+-rw-r--r--   0        0        0      100 2023-06-01 15:58:18.274299 lamindb_setup-0.46a5/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-05 07:30:18.302425 lamindb_setup-0.46a5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-06-01 15:58:18.274545 lamindb_setup-0.46a5/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-05 07:30:18.302530 lamindb_setup-0.46a5/README.md
+-rw-r--r--   0        0        0       52 2023-06-01 15:58:18.274800 lamindb_setup-0.46a5/docs/api.md
+-rw-r--r--   0        0        0    52895 2023-06-07 20:40:26.214287 lamindb_setup-0.46a5/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-05 07:30:18.302966 lamindb_setup-0.46a5/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0       96 2023-06-05 07:30:18.303105 lamindb_setup-0.46a5/docs/faq/index.md
+-rw-r--r--   0        0        0     3323 2023-06-01 15:58:18.275949 lamindb_setup-0.46a5/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     6590 2023-06-07 16:09:22.842055 lamindb_setup-0.46a5/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     8821 2023-06-01 15:58:18.276289 lamindb_setup-0.46a5/docs/guide/00-index.ipynb
+-rw-r--r--   0        0        0     5037 2023-06-01 15:58:18.276393 lamindb_setup-0.46a5/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0     8081 2023-06-01 15:58:18.276471 lamindb_setup-0.46a5/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     4342 2023-06-01 15:58:18.276562 lamindb_setup-0.46a5/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     5750 2023-06-05 07:30:18.303429 lamindb_setup-0.46a5/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     2975 2023-06-07 20:38:59.482507 lamindb_setup-0.46a5/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     3331 2023-06-01 15:58:18.276836 lamindb_setup-0.46a5/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-06-01 15:58:18.276937 lamindb_setup-0.46a5/docs/index.md
+-rw-r--r--   0        0        0      365 2023-06-01 15:58:18.277034 lamindb_setup-0.46a5/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:57:01.647274 lamindb_setup-0.46a5/lamin-project.yaml
+-rw-r--r--   0        0        0     2636 2023-06-07 20:40:28.234931 lamindb_setup-0.46a5/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5346 2023-06-07 20:38:59.482711 lamindb_setup-0.46a5/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     1410 2023-06-05 07:31:41.044617 lamindb_setup-0.46a5/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      621 2023-06-07 16:09:22.842870 lamindb_setup-0.46a5/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2006 2023-06-07 16:09:22.843059 lamindb_setup-0.46a5/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-05 07:30:18.304343 lamindb_setup-0.46a5/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-01 15:58:18.277912 lamindb_setup-0.46a5/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     6893 2023-06-07 20:38:59.483007 lamindb_setup-0.46a5/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     5411 2023-06-07 20:38:59.483209 lamindb_setup-0.46a5/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0      322 2023-06-05 07:30:18.304745 lamindb_setup-0.46a5/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1692 2023-06-03 14:25:55.266155 lamindb_setup-0.46a5/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      825 2023-06-05 07:30:18.304849 lamindb_setup-0.46a5/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-05 07:30:18.305060 lamindb_setup-0.46a5/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     1891 2023-06-07 20:38:59.483389 lamindb_setup-0.46a5/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-01 15:58:18.279311 lamindb_setup-0.46a5/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 15:58:18.279395 lamindb_setup-0.46a5/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 15:58:18.279466 lamindb_setup-0.46a5/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3548 2023-06-05 07:30:18.305347 lamindb_setup-0.46a5/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-06-05 07:30:18.305424 lamindb_setup-0.46a5/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-01 15:58:18.279648 lamindb_setup-0.46a5/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     5385 2023-06-07 16:33:24.023221 lamindb_setup-0.46a5/lamindb_setup/dev/_cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     2491 2023-06-01 15:58:18.279932 lamindb_setup-0.46a5/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0     2651 2023-06-07 16:09:22.843707 lamindb_setup-0.46a5/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 15:58:18.280089 lamindb_setup-0.46a5/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     9337 2023-06-07 16:33:24.023522 lamindb_setup-0.46a5/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 15:58:18.280386 lamindb_setup-0.46a5/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 15:58:18.280470 lamindb_setup-0.46a5/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2318 2023-06-05 07:30:18.305825 lamindb_setup-0.46a5/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 15:58:18.280631 lamindb_setup-0.46a5/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     1839 2023-06-07 20:38:59.483627 lamindb_setup-0.46a5/lamindb_setup/dev/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     2140 2023-06-05 07:31:41.044990 lamindb_setup-0.46a5/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5057 2023-06-05 07:30:18.306219 lamindb_setup-0.46a5/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2563 2023-06-05 07:30:18.306337 lamindb_setup-0.46a5/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0     2811 2023-06-05 11:32:22.995643 lamindb_setup-0.46a5/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-06-05 11:32:22.995738 lamindb_setup-0.46a5/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-06-05 11:32:22.995812 lamindb_setup-0.46a5/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-06-05 11:32:22.995890 lamindb_setup-0.46a5/lnschema-core/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-05 11:32:22.995916 lamindb_setup-0.46a5/lnschema-core/.gitmodules
+-rw-r--r--   0        0        0     1836 2023-06-05 11:32:22.996008 lamindb_setup-0.46a5/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-06-05 11:32:22.996105 lamindb_setup-0.46a5/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      364 2023-06-05 11:32:22.996173 lamindb_setup-0.46a5/lnschema-core/README.md
+-rw-r--r--   0        0        0    25740 2023-06-05 11:32:22.996389 lamindb_setup-0.46a5/lnschema-core/docs/changelog.md
+-rw-r--r--   0        0        0     1485 2023-06-05 11:32:22.996551 lamindb_setup-0.46a5/lnschema-core/docs/guide/core-schema.ipynb
+-rw-r--r--   0        0        0       52 2023-06-05 11:32:22.996748 lamindb_setup-0.46a5/lnschema-core/docs/guide/index.md
+-rw-r--r--   0        0        0      112 2023-06-05 11:32:22.996845 lamindb_setup-0.46a5/lnschema-core/docs/index.md
+-rw-r--r--   0        0        0      202 2023-06-05 11:32:22.996914 lamindb_setup-0.46a5/lnschema-core/lamin-project.yaml
+-rw-r--r--   0        0        0      592 2023-06-05 11:32:22.997066 lamindb_setup-0.46a5/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1515 2023-06-05 11:32:22.997223 lamindb_setup-0.46a5/lnschema-core/lnschema_core/_lookup.py
+-rw-r--r--   0        0        0      756 2023-06-05 11:32:22.997329 lamindb_setup-0.46a5/lnschema-core/lnschema_core/_types.py
+-rw-r--r--   0        0        0      349 2023-06-05 11:32:22.997395 lamindb_setup-0.46a5/lnschema-core/lnschema_core/_users.py
+-rw-r--r--   0        0        0     2810 2023-06-05 11:32:22.997546 lamindb_setup-0.46a5/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0    11504 2023-06-05 11:32:22.997705 lamindb_setup-0.46a5/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-05 11:32:22.997742 lamindb_setup-0.46a5/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0    24760 2023-06-05 11:32:22.997959 lamindb_setup-0.46a5/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      180 2023-06-05 11:32:22.998145 lamindb_setup-0.46a5/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0     1299 2023-06-05 11:32:22.998461 lamindb_setup-0.46a5/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      850 2023-06-05 11:32:22.998642 lamindb_setup-0.46a5/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0      475 2023-06-05 11:32:22.998792 lamindb_setup-0.46a5/lnschema-core/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1911 2023-06-07 16:33:24.024562 lamindb_setup-0.46a5/noxfile.py
+-rw-r--r--   0        0        0     1337 2023-06-07 10:17:03.860879 lamindb_setup-0.46a5/pyproject.toml
+-rw-r--r--   0        0        0      672 2023-06-05 07:30:18.308956 lamindb_setup-0.46a5/tests/test_bionty.py
+-rw-r--r--   0        0        0     3041 2023-06-01 15:58:18.282108 lamindb_setup-0.46a5/tests/test_init_instance.py
+-rw-r--r--   0        0        0      655 2023-06-01 15:58:18.282187 lamindb_setup-0.46a5/tests/test_load_instance.py
+-rw-r--r--   0        0        0      243 2023-06-01 15:58:18.282270 lamindb_setup-0.46a5/tests/test_set_storage.py
+-rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.46a5/PKG-INFO
```

### Comparing `lamindb_setup-0.46a4/.github/workflows/build.yml` & `lamindb_setup-0.46a5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/.github/workflows/latest-changes.yml` & `lamindb_setup-0.46a5/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/.gitignore` & `lamindb_setup-0.46a5/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/.pre-commit-config.yaml` & `lamindb_setup-0.46a5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/LICENSE` & `lamindb_setup-0.46a5/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/docs/changelog.md` & `lamindb_setup-0.46a5/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-🔊 Better logging | [399](https://github.com/laminlabs/lamindb-setup/pull/399) | [falexwolf](https://github.com/falexwolf) | 2023-06-05 | 0.46a3
+✅ More testing of Bionty | [405](https://github.com/laminlabs/lamindb-setup/pull/405) | [falexwolf](https://github.com/falexwolf) | 2023-06-07 | 0.46a5
+♻️ Reorder args of CLI | [407](https://github.com/laminlabs/lamindb-setup/pull/407) | [falexwolf](https://github.com/falexwolf) | 2023-06-07 |
+♻️ Refactored init & load instance | [406](https://github.com/laminlabs/lamindb-setup/pull/406) | [falexwolf](https://github.com/falexwolf) | 2023-06-07 |
+💚 Fix dependencies | [404](https://github.com/laminlabs/lamindb-setup/pull/404) | [falexwolf](https://github.com/falexwolf) | 2023-06-07 |
+♻️ Rename and set empty locker for now | [403](https://github.com/laminlabs/lamindb-setup/pull/403) | [falexwolf](https://github.com/falexwolf) | 2023-06-07 |
+🚸 Simplify remote SQLite synching & locking | [402](https://github.com/laminlabs/lamindb-setup/pull/402) | [falexwolf](https://github.com/falexwolf) | 2023-06-07 |
+:sparkles: Setup bionty version tables | [400](https://github.com/laminlabs/lamindb-setup/pull/400) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-07 |
+🔊 Better logging | [399](https://github.com/laminlabs/lamindb-setup/pull/399) | [falexwolf](https://github.com/falexwolf) | 2023-06-05 | 0.46a4
 💄 Prettier settings file names | [398](https://github.com/laminlabs/lamindb-setup/pull/398) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 |
 ⚡ Bionty versions table & performance improvements | [396](https://github.com/laminlabs/lamindb-setup/pull/396) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-04 |
 🔥 Remove all occurances of sqlmodel | [397](https://github.com/laminlabs/lamindb-setup/pull/397) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 |
 🔥 Delete SQLAlchemy related content | [395](https://github.com/laminlabs/lamindb-setup/pull/395) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 |
 🔥 Remove alembic migrations infra & fix coverage | [394](https://github.com/laminlabs/lamindb-setup/pull/394) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 |
 ✨ Add migrations management for Django (start breaking SQLAlchemy) | [393](https://github.com/laminlabs/lamindb-setup/pull/393) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 |
 ✨ Extend django to lnschema-bionty | [392](https://github.com/laminlabs/lamindb-setup/pull/392) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-04 |
```

### Comparing `lamindb_setup-0.46a4/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.46a5/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.46a5/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/docs/faq/test-sqlite-sync.ipynb` & `lamindb_setup-0.46a5/docs/faq/test-sqlite-sync.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9673387096774193%*

 * *Differences: {"'cells'": "{17: {'source': ['Delete the local sqlite file:']}, insert: [(7, "*

 * *            "OrderedDict([('attachments', OrderedDict()), ('cell_type', 'markdown'), ('id', "*

 * *            "'45967bdd'), ('metadata', OrderedDict()), ('source', ['Remote SQLite file does not "*

 * *            "yet exist upon instance init:'])])), (8, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_count', None), ('id', '037ac4f5'), ('metadata', OrderedDict()), "*

 * *            "('outputs', []), ('source', ['assert not "*

 * *  […]*

```diff
@@ -71,14 +71,90 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "sqlite_file"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "45967bdd",
+            "metadata": {},
+            "source": [
+                "Remote SQLite file does not yet exist upon instance init:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "037ac4f5",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "assert not settings.instance._sqlite_file.exists()"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "5d253504",
+            "metadata": {},
+            "source": [
+                "Create it (the user only ever calls this implicitly through `lamin close`). This runs 9s!!!"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "8a3cd72d",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "settings.instance._update_cloud_sqlite_file()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "81100c7e",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "assert settings.instance._sqlite_file.exists()"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "c764511d",
+            "metadata": {},
+            "source": [
+                "Now mimic a new user who loads the instance (this runs 4s):"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "01ef82da",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "settings.instance._update_local_sqlite_file()"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "8e39b443",
+            "metadata": {},
+            "source": [
+                "Get the mere filepath of the local file, without any update:"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "7b5a850a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "cache_file = settings.instance.storage.cloud_to_local_no_update(sqlite_file)"
@@ -96,15 +172,15 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "26d8bd48",
             "metadata": {},
             "source": [
-                "Delete the local sqlite database file."
+                "Delete the local sqlite file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2abf1dd1",
             "metadata": {},
```

### Comparing `lamindb_setup-0.46a4/docs/guide/00-index.ipynb` & `lamindb_setup-0.46a5/docs/guide/00-index.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/docs/guide/01-setup-user.ipynb` & `lamindb_setup-0.46a5/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/docs/guide/02-init-instance.ipynb` & `lamindb_setup-0.46a5/docs/guide/02-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/docs/guide/03-load-instance.ipynb` & `lamindb_setup-0.46a5/docs/guide/03-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/docs/guide/04-set-storage.ipynb` & `lamindb_setup-0.46a5/docs/guide/04-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/docs/guide/05-schema-modules.ipynb` & `lamindb_setup-0.46a5/docs/guide/05-schema-modules.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9706709956709957%*

 * *Differences: {"'cells'": "{1: {'source': {delete: [0]}}, 3: {'source': {insert: [(2, '(The `lamin1` module is "*

 * *            'an example for a configurable in-house schema that tracks lab operations: '*

 * *            "https://github.com/laminlabs/lnschema-lamin1)\\n')], delete: [2]}}, 4: {'source': "*

 * *            '[\'ln_setup.init(\\n\', \'    storage="mydata2", schema="bionty"\\n\', \')  # CLI: '*

 * *            "lamin init --storage mydata2 --schema bionty']}, 5: {'source': "*

 * *            "['ln_setup.schema.draw()']}, 6: {'cell […]*

```diff
@@ -14,15 +14,14 @@
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "!lamin close\n",
                 "!lamin delete mydata2"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -34,41 +33,56 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The `bionty` schema module maps fundamental biological entities: https://github.com/laminlabs/lnschema-bionty\n",
                 "\n",
-                "The `lamin1` module is an example for a configurable in-house schema that tracks lab operations: https://github.com/laminlabs/lnschema-lamin1\n",
+                "(The `lamin1` module is an example for a configurable in-house schema that tracks lab operations: https://github.com/laminlabs/lnschema-lamin1)\n",
                 "\n",
                 "You can configure an arbitrary number of schema modules."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "_USE_DJANGO = True\n",
-                "\n",
-                "if not _USE_DJANGO:\n",
-                "    ln_setup.init(\n",
-                "        storage=\"mydata2\", schema=\"bionty,lamin1\"\n",
-                "    )  # CLI: lamin init --storage mydata2 --schema bionty,lamin1"
+                "ln_setup.init(\n",
+                "    storage=\"mydata2\", schema=\"bionty\"\n",
+                ")  # CLI: lamin init --storage mydata2 --schema bionty"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "if not _USE_DJANGO:\n",
-                "    ln_setup.schema.draw()"
+                "ln_setup.schema.draw()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from lnschema_bionty import BiontySource\n",
+                "import pandas as pd"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pd.DataFrame(BiontySource.objects.all().values()).head()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -81,47 +95,31 @@
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "from lamindb_setup.dev._setup_knowledge import load_bionty_versions"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "if not _USE_DJANGO:\n",
-                "    load_bionty_versions(ln_setup.settings.instance, display=True)"
+                "# test loading this instance\n",
+                "ln_setup.load(\"mydata2\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "if not _USE_DJANGO:\n",
-                "    # clean up\n",
-                "    ln_setup.delete(\"mydata2\")\n",
-                "    # test with postgres\n",
-                "    from laminci.db import setup_local_test_postgres\n",
+                "from bionty.dev._handle_versions import LAMINDB_SOURCES_PATH\n",
                 "\n",
-                "    pgurl = setup_local_test_postgres()\n",
-                "    ln_setup.init(storage=\"mydata2\", schema=\"bionty,lamin1\", db=pgurl)\n",
-                "    !docker stop pgtest && docker rm pgtest\n",
-                "    ln_setup.delete(\"pgtest\")"
+                "assert LAMINDB_SOURCES_PATH.exists()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -133,15 +131,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.9.16"
         },
         "vscode": {
             "interpreter": {
                 "hash": "61b4062b24dfb1010f420dad5aa3bd73a4d2af47d0ec44eafec465a35a9d7239"
             }
         }
     },
```

### Comparing `lamindb_setup-0.46a4/docs/guide/migrate.md` & `lamindb_setup-0.46a5/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/__init__.py` & `lamindb_setup-0.46a5/lamindb_setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
    :toctree:
 
    dev
 """
 
 import os
 
-__version__ = "0.46a4"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.46a5"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
 from . import dev
 from ._close import close  # noqa
@@ -71,15 +71,15 @@
 from ._set import set, set_storage  # noqa
 from ._settings import settings  # noqa
 from ._setup_user import login, signup  # noqa
 
 
 # unlock and clear on uncaught exception
 def _clear_on_exception():
-    from .dev._exclusion import _locker
+    from .dev._cloud_sqlite_locker import _locker
 
     if _locker is not None:
         try:
             _locker._clear()
         except:
             pass
```

### Comparing `lamindb_setup-0.46a4/lamindb_setup/__main__.py` & `lamindb_setup-0.46a5/lamindb_setup/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,30 +21,14 @@
 
 description_cli = "Configure LaminDB and perform simple actions."
 parser = argparse.ArgumentParser(
     description=description_cli, formatter_class=argparse.RawTextHelpFormatter
 )
 subparsers = parser.add_subparsers(dest="command")
 
-# signup user
-signup = subparsers.add_parser("signup", help=signup_help)
-aa = signup.add_argument
-aa("email", type=str, metavar="email", help=user.email)
-
-# login user
-login = subparsers.add_parser("login", help=login_help)
-aa = login.add_argument
-aa(
-    "user",
-    type=str,
-    metavar="user",
-    help="Email or user handle. Email is needed at first login.",
-)  # noqa
-aa("--password", type=str, metavar="pw", default=None, help=user.password)
-
 # init instance
 init = subparsers.add_parser("init", help=init_help)
 aa = init.add_argument
 aa("--storage", type=str, metavar="s", help=instance.storage_root)
 aa("--db", type=str, metavar="d", default=None, help=instance.db)
 aa("--schema", type=str, metavar="schema", default=None, help=instance.schema)
 aa("--name", type=str, metavar="n", default=None, help=instance.name)
@@ -86,14 +70,32 @@
 track_parser = subparsers.add_parser("track", help=track_help)
 aa = track_parser.add_argument
 filepath_help = "A path to the notebook to track."
 aa("filepath", type=str, metavar="filepath", help=filepath_help)
 pypackage_help = "One or more (delimited by ',') python packages to track."
 aa("--pypackage", type=str, metavar="pypackage", default=None, help=pypackage_help)
 
+
+# signup user
+signup = subparsers.add_parser("signup", help=signup_help)
+aa = signup.add_argument
+aa("email", type=str, metavar="email", help=user.email)
+
+# login user
+login = subparsers.add_parser("login", help=login_help)
+aa = login.add_argument
+aa(
+    "user",
+    type=str,
+    metavar="user",
+    help="Email or user handle. Email is needed at first login.",
+)  # noqa
+aa("--password", type=str, metavar="pw", default=None, help=user.password)
+
+
 # parse args
 args = parser.parse_args()
 
 
 def process_result(result):
     if result in ["migrate-unnecessary", "migrate-success", "migrate-skipped", None]:
         return None  # is interpreted as success (exit code 0) by shell
```

### Comparing `lamindb_setup-0.46a4/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.46a5/lamindb_setup/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/_close.py` & `lamindb_setup-0.46a5/lamindb_setup/_close.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 def close() -> None:
     """Close existing instance.
 
     Returns `None` if succeeds, otherwise an exception is raised.
     """
     if current_instance_settings_file().exists():
         instance = settings.instance.identifier
+        settings.instance._update_cloud_sqlite_file()
         current_instance_settings_file().unlink()
         os.environ["LAMINDB_INSTANCE_LOADED"] = "0"
         logger.success(f"Closed {instance}")
     else:
         logger.info("No instance loaded")
```

### Comparing `lamindb_setup-0.46a4/lamindb_setup/_delete.py` & `lamindb_setup-0.46a5/lamindb_setup/_delete.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import shutil
 from pathlib import Path
 
 from lamin_logger import logger
 
+from ._close import close
 from ._settings import settings
 from .dev._settings_load import load_instance_settings
-from .dev._settings_store import current_instance_settings_file, instance_settings_file
+from .dev._settings_store import instance_settings_file
 
 
 def delete(instance_name: str):
     """Delete an instance."""
     instance_identifier = f"{settings.user.handle}/{instance_name}"
     logger.info(f"Deleting instance {instance_identifier}")
     settings_file = instance_settings_file(instance_name, settings.user.handle)
@@ -20,39 +21,33 @@
         )
         return None
     isettings = load_instance_settings(settings_file)
 
     delete_settings(settings_file)
     if settings._instance_exists:
         if instance_identifier == settings.instance.identifier:
-            current_settings_file = current_instance_settings_file()
-            logger.info(
-                f"    current instance settings {current_settings_file} deleted"
-            )
-            current_settings_file.unlink()
+            close()  # close() does further operations, unlocking...
             settings._instance_settings = None
     delete_cache(isettings.storage.cache_dir)
-    logger.info(
-        f"    consider deleting your stored data manually: {isettings.storage.root}"
-    )
     if isettings.dialect == "sqlite":
         if isettings._sqlite_file.exists():
             isettings._sqlite_file.unlink()
             logger.info("    deleted '.lndb' sqlite file")
         else:
             logger.info("    '.lndb' sqlite file does not exist")
     if isettings.is_remote:
-        logger.info("    please manually delete your remote instance on lamin.ai")
+        logger.info("    manually delete your remote instance on lamin.ai")
+    logger.info(f"    manually delete your stored data: {isettings.storage.root}")
 
 
 def delete_cache(cache_dir: Path):
     if cache_dir is not None and cache_dir.exists():
         shutil.rmtree(cache_dir)
         logger.info("    instance cache deleted")
 
 
 def delete_settings(settings_file: Path):
     if settings_file.exists():
         settings_file.unlink()
-        logger.info("    instance settings '.env' deleted")
+        logger.info(f"    deleted instance settings file: {settings_file}")
     else:
-        logger.info("    instance settings '.env' do not exist locally")
+        logger.info(f"    instance settings file doesn't exist: {settings_file}")
```

### Comparing `lamindb_setup-0.46a4/lamindb_setup/_docstrings.py` & `lamindb_setup-0.46a5/lamindb_setup/_docstrings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/_init_instance.py` & `lamindb_setup-0.46a5/lamindb_setup/_init_instance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import importlib
+import os
 import sys
 from pathlib import Path
 from typing import Optional, Union
 
 from lamin_logger import logger
 from pydantic import PostgresDsn
 
 from lamindb_setup.dev.upath import UPath
 
 from ._docstrings import instance_description as description
-from ._load_instance import load, load_from_isettings
 from ._settings import settings
 from .dev import InstanceSettings
 from .dev._docs import doc_args
-from .dev._setup_knowledge import write_bionty_versions  # noqa
 from .dev._setup_schema import load_schema
 from .dev._storage import Storage
 
 
-def register(isettings: InstanceSettings, usettings):
+def register_user_and_storage(isettings: InstanceSettings, usettings):
     """Register user & storage in DB."""
     from django.db.utils import OperationalError
     from lnschema_core.models import Storage, User
 
     try:
         user, created = User.objects.update_or_create(
             id=usettings.id,
@@ -70,24 +69,14 @@
         importlib.reload(lamindb)
     else:
         # only log if we're outside lamindb
         # lamindb itself logs upon import!
         logger.success(f"Loaded instance: {isettings.owner}/{isettings.name}")
 
 
-def persist_settings_load_schema(isettings: InstanceSettings):
-    # The reason for why the following two calls should always come together
-    # is that the schema modules need information about what type of database
-    # (sqlite or not) is mounted at time of importing the module!
-    # hence, the schema modules look for the settings file that is generated
-    # by calling isettings._persist()
-    isettings._persist()
-    load_schema(isettings)
-
-
 ERROR_SQLITE_CACHE = """
 Your cached local SQLite file exists, while your cloud SQLite file ({}) doesn't.
 Either delete your cache ({}) or add it back to the cloud (if delete was accidental).
 """
 
 
 @doc_args(
@@ -98,62 +87,63 @@
 )
 def init(
     *,
     storage: Union[str, Path, UPath],
     name: Optional[str] = None,
     db: Optional[PostgresDsn] = None,
     schema: Optional[str] = None,
-    _migrate: bool = False,  # not user-facing
     _test: bool = False,
 ) -> None:
     """Creating and loading a LaminDB instance.
 
     Args:
         storage: {}
         name: {}
         db: {}
         schema: {}
     """
+    # clean up in next refactor
     from lnhub_rest.core.instance._init_instance import (
         init_instance as init_instance_hub,
     )
     from lnhub_rest.core.instance._init_instance import (
         validate_db_arg,
         validate_schema_arg,
     )
     from lnhub_rest.core.storage._add_storage import (
         get_storage_region,
         validate_storage_root_arg,
     )
 
+    # avoid circular import
+    from ._load_instance import load
+
     assert settings.user.id  # check user is logged in
     owner = settings.user.handle
 
     schema = validate_schema_arg(schema)
     validate_storage_root_arg(str(storage))
     validate_db_arg(db)
 
     name_str = infer_instance_name(storage=storage, name=name, db=db)
     # test whether instance exists by trying to load it
-    response = load(
-        f"{owner}/{name_str}", _log_error_message=False, migrate=_migrate, _test=_test
-    )
+    response = load(f"{owner}/{name_str}", _log_error_message=False, _test=_test)
     if response is None:
         return None  # successful load!
 
     isettings = InstanceSettings(
         owner=owner,
         name=name_str,
         storage_root=storage,
         storage_region=get_storage_region(storage),
         db=db,
         schema=schema,
     )
 
-    if isettings.storage.is_cloud:
+    if isettings._is_cloud_sqlite:
         if (
             not isettings._sqlite_file.exists()
             and isettings._sqlite_file_local.exists()
         ):
             raise RuntimeError(
                 ERROR_SQLITE_CACHE.format(
                     isettings._sqlite_file, isettings._sqlite_file_local
@@ -167,41 +157,59 @@
             storage=str(storage),
             db=db,
             schema=schema,
         )
         if result == "instance-exists-already":
             pass  # everything is alright!
         elif isinstance(result, str):
-            raise RuntimeError(f"Creating instance on hub failed:\n{result}")
+            raise RuntimeError(f"Registering instance on hub failed:\n{result}")
         logger.success(
             f"Registered instance on hub: https://lamin.ai/{owner}/{name_str}"
         )
-    else:
-        logger.hint(
-            "Not registering local instance on hub, if you want, call `lamin register`"
-        )
 
     if _test:
         isettings._persist()
         return None
 
-    if not isettings._is_db_setup(mute=True)[0]:
-        load_schema(isettings, init=True)
-        register(isettings, settings.user)  # if this doesn't emit warning, we're good
-        # write_bionty_versions(isettings)
-        isettings._update_cloud_sqlite_file()
-    else:
-        # we're currently using this for testing migrations
-        # passing connection strings of databases that need to be tested
-        # for migrations
-        logger.warning("Your instance seems already set up, attempt load:")
-        load_from_isettings(isettings, migrate=_migrate)
+    if isettings._is_db_setup(mute=True)[0]:
+        raise RuntimeError(
+            "Your instance DB is already set up but couldn't be loaded, something"
+            " is off"
+        )
+    load_from_isettings(isettings, init=True)
+    if isettings._is_cloud_sqlite:
+        logger.hint("To push changes to the cloud SQLite file, call: lamin close")
+        # @Sergei, this is currently not yet enabled
+        # logger.hint(
+        #     f"In the meantime, {isettings._sqlite_file} is locked for other users"
+        # )
+    if not isettings.is_remote:
+        logger.hint(
+            "Did not register local instance on hub (if you want to, call `lamin"
+            " register`)"
+        )
+    return None
+
 
+def load_from_isettings(
+    isettings: InstanceSettings,
+    *,
+    init: bool = False,
+) -> None:
+    from .dev._setup_bionty_sources import load_bionty_sources, write_bionty_sources
+
+    load_schema(isettings, init=init)
+    register_user_and_storage(isettings, settings.user)
+    if init:
+        write_bionty_sources(isettings)
+    else:
+        load_bionty_sources(isettings)
     isettings._persist()
     reload_lamindb(isettings)
+    os.environ["LAMINDB_INSTANCE_LOADED"] = "1"
 
 
 def infer_instance_name(
     *,
     storage: Union[str, Path, UPath],
     name: Optional[str] = None,
     db: Optional[PostgresDsn] = None,
```

### Comparing `lamindb_setup-0.46a4/lamindb_setup/_load_instance.py` & `lamindb_setup-0.46a5/lamindb_setup/_load_instance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-import os
 from pathlib import Path
 from typing import Optional, Union
 
 from lamin_logger import logger
 
 from lamindb_setup.dev.upath import UPath
 
+from ._init_instance import load_from_isettings
 from ._settings import InstanceSettings, settings
 from .dev._django import setup_django
 from .dev._settings_load import load_instance_settings
 from .dev._settings_store import instance_settings_file
 from .dev._storage import StorageSettings
 
 
 def load(
     identifier: str,
     *,
-    migrate: Optional[bool] = None,
     storage: Optional[Union[str, Path, UPath]] = None,
     _log_error_message: bool = True,
     _access_token: Optional[str] = None,
     _test: bool = False,
 ) -> Optional[str]:
     """Load existing instance.
 
     Args:
         identifier: `str` - The instance identifier can the instance name (owner is
             current user), handle/name, or the URL: https://lamin.ai/handle/name.
         storage: `Optional[PathLike] = None` - Load the instance with an
             updated default storage.
-        migrate: `Optional[bool] = None` - Whether to auto-migrate or not.
     """
     owner, name = get_owner_name_from_identifier(identifier)
 
     from lnhub_rest.core.instance._load_instance import (
         load_instance as load_instance_from_hub,
     )
 
@@ -68,37 +66,30 @@
 
     if storage is not None:
         update_isettings_with_storage(isettings, storage)
     if _test:
         isettings._persist()  # this is to test the settings
         return None
 
-    check, msg = isettings._is_db_setup()
+    check, msg = isettings._is_db_setup()  # this also updates local SQLite
     if not check:
         if _log_error_message:
             raise RuntimeError(msg)
         else:
             logger.warning(
                 "Instance metadata exists, but DB might have been corrupted or deleted."
                 " Re-initializing the DB."
             )
             return "instance-not-reachable"
 
+    # need to set up Django here because we query the storage table
     setup_django(isettings)
     if storage is not None and isettings.dialect == "sqlite":
         update_root_field_in_default_storage(isettings)
-
-    if not isettings.storage.root.exists():
-        raise RuntimeError(
-            f"Storage root does not exist: {isettings.storage.root}\n"
-            "Please amend by passing --storage <my-storage-root>"
-        )
-
-    load_from_isettings(isettings, migrate)
-    os.environ["LAMINDB_INSTANCE_LOADED"] = "1"
+    load_from_isettings(isettings)
     return None
 
 
 def get_owner_name_from_identifier(identifier: str):
     if "/" in identifier:
         if identifier.startswith("https://lamin.ai/"):
             identifier = identifier.replace("https://lamin.ai/", "")
@@ -111,27 +102,14 @@
         owner, name = split
     else:
         owner = settings.user.handle
         name = identifier
     return owner, name
 
 
-def load_from_isettings(
-    isettings: InstanceSettings,
-    migrate: Optional[bool] = None,
-) -> None:
-    from ._init_instance import persist_settings_load_schema, register, reload_lamindb
-    from .dev._setup_knowledge import load_bionty_versions  # noqa
-
-    persist_settings_load_schema(isettings)
-    register(isettings, settings.user)
-    # load_bionty_versions(isettings)
-    reload_lamindb(isettings)
-
-
 def update_isettings_with_storage(
     isettings: InstanceSettings, storage: Union[str, Path, UPath]
 ) -> None:
     ssettings = StorageSettings(storage, instance_settings=isettings)
     if ssettings.is_cloud:
         try:  # triggering ssettings.id makes a lookup in the storage table
             logger.success(f"Loaded storage: {ssettings.id} / {ssettings.root_as_str}")
```

### Comparing `lamindb_setup-0.46a4/lamindb_setup/_notebook.py` & `lamindb_setup-0.46a5/lamindb_setup/_notebook.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/_register_instance.py` & `lamindb_setup-0.46a5/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/_schema.py` & `lamindb_setup-0.46a5/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/_set.py` & `lamindb_setup-0.46a5/lamindb_setup/_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import Union
 
 from lamin_logger import logger
 
 from lamindb_setup.dev.upath import UPath
 
-from ._init_instance import register
+from ._init_instance import register_user_and_storage
 from ._settings import settings
 from .dev import deprecated
 from .dev._settings_instance import InstanceSettings
 
 
 class set:
     """Set properties of current instance."""
@@ -41,15 +41,15 @@
             name=settings.instance.name,
             storage_root=root,
             db=settings.instance.db,
             schema=settings.instance._schema_str,
         )
 
         new_isettings._persist()  # this also updates the settings object
-        register(new_isettings, settings.user)
+        register_user_and_storage(new_isettings, settings.user)
         if settings.instance.is_remote:
             add_storage_hub(root, account_handle=settings.instance.owner)
 
         settings.storage._set_fs_kwargs(**fs_kwargs)
 
         logger.success(f"Set storage {root}")
```

### Comparing `lamindb_setup-0.46a4/lamindb_setup/_settings.py` & `lamindb_setup-0.46a5/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/_setup_user.py` & `lamindb_setup-0.46a5/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.46a5/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.46a5/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/dev/_django.py` & `lamindb_setup-0.46a5/lamindb_setup/dev/_django.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,16 +58,17 @@
         if create_migrations:
             call_command("makemigrations")
             return None
 
         planned_migrations = get_migrations_to_sync()
         if len(planned_migrations) > 0:
             if deploy_migrations:
-                call_command("migrate")
-                if not init:  # delay sync
+                verbosity = 0 if init else 2
+                call_command("migrate", verbosity=verbosity)
+                if not init:  # only update if this is a deploy migration command
                     isettings._update_cloud_sqlite_file()
             else:
                 logger.warning(
                     f"Your database is not up to date:\n{planned_migrations}\nConsider"
                     " migrating it: lamin migrate deploy\nIf you can't yet migrate,"
                     " consider installing an older schema module version to avoid"
                     " potential errors"
```

### Comparing `lamindb_setup-0.46a4/lamindb_setup/dev/_exclusion.py` & `lamindb_setup-0.46a5/lamindb_setup/dev/_cloud_sqlite_locker.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 from typing import Optional, Union
 
 import fsspec
 from dateutil.parser import isoparse  # type: ignore
 from lamin_logger import logger
 
+from ._settings_instance import InstanceSettings
 from .upath import UPath
 from .upath import infer_filesystem as _infer_filesystem
 
 EXPIRATION_TIME = 1800  # 30 min
 
 MAX_MSG_COUNTER = 1000  # print the msg after this number of iterations
 
@@ -151,19 +152,19 @@
         self.unlock()
         self.mapper[f"entering/{self.user}"] = b"0"
 
 
 _locker: Optional[Locker] = None
 
 
-def get_locker() -> Locker:
+def get_locker(isettings: InstanceSettings) -> Locker:
     from .._settings import settings
 
     user_id = settings.user.id
-    storage_root = settings.instance.storage.root
+    storage_root = isettings.storage.root
 
     global _locker
 
     if _locker is None:
         _locker = Locker(user_id, storage_root)
     elif user_id != _locker.user or storage_root is not _locker.root:
         _locker = Locker(user_id, storage_root)
```

### Comparing `lamindb_setup-0.46a4/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.46a5/lamindb_setup/dev/_settings_instance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import shutil
 from pathlib import Path
 from typing import Literal, Optional, Set, Tuple, Union
 
 from lamin_logger import logger
 
-from ._exclusion import empty_locker, get_locker
 from ._settings_save import save_instance_settings
 from ._settings_store import current_instance_settings_file, instance_settings_file
 from ._storage import StorageSettings
 from .upath import UPath
 
 # leave commented out until we understand more how to deal with
 # migrations in redun
@@ -96,31 +95,36 @@
     @property
     def _sqlite_file_local(self) -> Path:
         """Local SQLite file."""
         return self.storage.cloud_to_local_no_update(self._sqlite_file)
 
     def _update_cloud_sqlite_file(self) -> None:
         """Upload the local sqlite file to the cloud file."""
-        if self.is_cloud_sqlite:
-            logger.info("Updating cloud sqlite file")
+        if self._is_cloud_sqlite:
+            logger.info("Updating & unlocking cloud SQLite")
             sqlite_file = self._sqlite_file
             cache_file = self.storage.cloud_to_local_no_update(sqlite_file)
             sqlite_file.upload_from(cache_file)  # type: ignore
             cloud_mtime = sqlite_file.modified.timestamp()  # type: ignore
             # this seems to work even if there is an open connection
             # to the cache file
             os.utime(cache_file, times=(cloud_mtime, cloud_mtime))
+            self._cloud_sqlite_locker.unlock()
 
     def _update_local_sqlite_file(self) -> None:
         """Download the cloud sqlite file if it is newer than local."""
-        if self.is_cloud_sqlite:
-            logger.info("Updating local sqlite file")
+        if self._is_cloud_sqlite:
+            logger.info(
+                "Synching cloud SQLite to local, locking remote (unlock via: lamin"
+                " close)"
+            )
             sqlite_file = self._sqlite_file
             cache_file = self.storage.cloud_to_local_no_update(sqlite_file)
             sqlite_file.synchronize(cache_file)  # type: ignore
+            self._cloud_sqlite_locker.lock()
 
     @property
     def db(self) -> str:
         """Database URL."""
         if self._db is None:
             # here, we want the updated sqlite file
             # hence, we don't use self._sqlite_file_local()
@@ -148,24 +152,27 @@
         return sa.create_engine(self.db, future=True)
 
     @property
     def session(self):
         raise NotImplementedError
 
     @property
-    def is_cloud_sqlite(self) -> bool:
+    def _is_cloud_sqlite(self) -> bool:
         # can we make this a private property, Sergei?
         # as it's not relevant to the user
         """Is this a cloud instance with sqlite db."""
         return self.dialect == "sqlite" and self.storage.is_cloud
 
     @property
     def _cloud_sqlite_locker(self):
-        if self.is_cloud_sqlite:
-            return get_locker()
+        # avoid circular import
+        from ._cloud_sqlite_locker import empty_locker
+
+        if self._is_cloud_sqlite:
+            return empty_locker
         else:
             return empty_locker
 
     @property
     def storage(self) -> StorageSettings:
         """Low-level access to storage location."""
         return self._storage
@@ -184,15 +191,15 @@
             if "@127.0.0.1" in uri:
                 return True
             return False
 
         if self.dialect == "postgresql":
             if is_local_uri(self.db):
                 return False
-        # returns True for remote SQLite
+        # returns True for cloud SQLite
         # and remote postgres
         return True
 
     def _persist(self) -> None:
         assert self.name is not None
         if self.storage.type == "local":
             self.storage.root.mkdir(parents=True, exist_ok=True)
@@ -216,14 +223,17 @@
                     False,
                     f"SQLite file {self._sqlite_file} does not exist! It should be in"
                     f" the storage root: {self.storage.root}",
                 )
             else:
                 return False, f"Connection {self.db} not reachable"
 
+        # in order to proceed with the next check, we need the local sqlite
+        self._update_local_sqlite_file()
+
         import sqlalchemy as sa
 
         engine = sa.create_engine(self.db)
         with engine.connect() as conn:
             try:  # cannot import lnschema_core here, need to use plain SQL
                 result = conn.execute(
                     sa.text("select * from lnschema_core_user")
```

### Comparing `lamindb_setup-0.46a4/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.46a5/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.46a5/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.46a5/lamindb_setup/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.46a5/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.46a5/lamindb_setup/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.46a5/lamindb_setup/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lamindb_setup/dev/upath.py` & `lamindb_setup-0.46a5/lamindb_setup/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lnschema-core/.github/workflows/build.yml` & `lamindb_setup-0.46a5/lnschema-core/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.46a5/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lnschema-core/.gitignore` & `lamindb_setup-0.46a5/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.46a5/lnschema-core/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lnschema-core/LICENSE` & `lamindb_setup-0.46a5/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lnschema-core/docs/changelog.md` & `lamindb_setup-0.46a5/lnschema-core/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🎨 Adapted featureset | [185](https://github.com/laminlabs/lnschema-core/pull/185) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-05 |
+♻️ Polish schema | [184](https://github.com/laminlabs/lnschema-core/pull/184) | [falexwolf](https://github.com/falexwolf) | 2023-06-05 |
+🚸 Improve QuerySet | [182](https://github.com/laminlabs/lnschema-core/pull/182) | [falexwolf](https://github.com/falexwolf) | 2023-06-05 |
+:fire: Delete SQLAlchemy related content | [181](https://github.com/laminlabs/lnschema-core/pull/181) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 |
 :fire: Remove unncessary files | [180](https://github.com/laminlabs/lnschema-core/pull/180) | [falexwolf](https://github.com/falexwolf) | 2023-06-04 | 0.35a4
 ♻️ Absorb `DjangoORM.create()` in `DjangoORM.__init__()` | [178](https://github.com/laminlabs/lnschema-core/pull/178) | [falexwolf](https://github.com/falexwolf) | 2023-06-03 |
 ➖ Remove nbproject from code | [179](https://github.com/laminlabs/lnschema-core/pull/179) | [Koncopd](https://github.com/Koncopd) | 2023-06-03 |
 🏗️ Enable Django backend | [177](https://github.com/laminlabs/lnschema-core/pull/177) | [falexwolf](https://github.com/falexwolf) | 2023-06-02 | 0.35a3
 🚚 Rename lndb to lamindb-setup | [176](https://github.com/laminlabs/lnschema-core/pull/176) | [falexwolf](https://github.com/falexwolf) | 2023-06-01 | 0.35a2
 🏗️ Add Django backend | [175](https://github.com/laminlabs/lnschema-core/pull/175) | [falexwolf](https://github.com/falexwolf) | 2023-05-31 | 0.35a1
 👷 Refactor CI | [174](https://github.com/laminlabs/lnschema-core/pull/174) | [falexwolf](https://github.com/falexwolf) | 2023-05-30 |
```

### Comparing `lamindb_setup-0.46a4/lnschema-core/docs/guide/core-schema.ipynb` & `lamindb_setup-0.46a5/lnschema-core/docs/guide/core-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lnschema-core/lnschema_core/__init__.py` & `lamindb_setup-0.46a5/lnschema-core/lnschema_core/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 
 _INSTANCE_SETUP = _check_instance_setup()
 
 if _INSTANCE_SETUP:
     from . import ids, types
     from .models import (  # type: ignore
         BaseORM,
-        Features,
+        Featureset,
         File,
         Folder,
         Project,
         Run,
         RunInput,
         Storage,
         Transform,
         User,
     )
+
+    Features = Featureset  # backward compat
```

### Comparing `lamindb_setup-0.46a4/lnschema-core/lnschema_core/_lookup.py` & `lamindb_setup-0.46a5/lnschema-core/lnschema_core/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lnschema-core/lnschema_core/_types.py` & `lamindb_setup-0.46a5/lnschema-core/lnschema_core/_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     link = "link"
 
 
 class TransformType(Enum):
     pipeline = "pipeline"
     notebook = "notebook"
     app = "app"
+    api = "api"
 
     def __repr__(self):
         return self.name
 
     @classmethod
     def choices(cls):
         return [(item.value, item.name) for item in cls]
```

### Comparing `lamindb_setup-0.46a4/lnschema-core/lnschema_core/ids.py` & `lamindb_setup-0.46a5/lnschema-core/lnschema_core/ids.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/lnschema-core/lnschema_core/migrations/0001_initial.py` & `lamindb_setup-0.46a5/lnschema-core/lnschema_core/migrations/0001_initial.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2.1 on 2023-06-04 13:33
+# Generated by Django 4.2.1 on 2023-06-05 12:36
 
 from typing import List
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 import lnschema_core._types
@@ -16,105 +16,111 @@
     dependencies: List[str] = []
 
     operations = [
         migrations.CreateModel(
             name="File",
             fields=[
                 ("id", models.CharField(max_length=20, primary_key=True, serialize=False)),
-                ("name", models.CharField(blank=True, max_length=255, null=True)),
-                ("suffix", models.CharField(blank=True, max_length=63, null=True)),
-                ("size", models.BigIntegerField(blank=True, null=True)),
-                ("hash", models.CharField(blank=True, max_length=63, null=True)),
-                ("key", models.CharField(blank=True, max_length=255, null=True)),
-                ("created_at", models.DateTimeField(auto_now_add=True)),
-                ("updated_at", models.DateTimeField(auto_now=True)),
+                ("name", models.CharField(db_index=True, default=None, max_length=255, null=True)),
+                ("suffix", models.CharField(db_index=True, default=None, max_length=30, null=True)),
+                ("size", models.BigIntegerField(db_index=True, null=True)),
+                ("hash", models.CharField(db_index=True, default=None, max_length=86, null=True)),
+                ("key", models.CharField(db_index=True, default=None, max_length=255, null=True)),
+                ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
+                ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
             ],
             options={
                 "managed": True,
             },
         ),
         migrations.CreateModel(
             name="Folder",
             fields=[
-                ("id", models.CharField(max_length=20, primary_key=True, serialize=False)),
-                ("name", models.CharField(max_length=255)),
-                ("key", models.CharField(blank=True, max_length=255, null=True)),
-                ("created_at", models.DateTimeField(auto_now_add=True)),
-                ("updated_at", models.DateTimeField(auto_now=True)),
+                ("id", models.CharField(default=lnschema_core.ids.folder, max_length=20, primary_key=True, serialize=False)),
+                ("name", models.CharField(db_index=True, max_length=255)),
+                ("key", models.CharField(db_index=True, default=None, max_length=255, null=True)),
+                ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
+                ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
             ],
             options={
                 "managed": True,
             },
         ),
         migrations.CreateModel(
             name="Run",
             fields=[
-                ("id", models.CharField(default=lnschema_core.ids.run, max_length=12, primary_key=True, serialize=False)),
-                ("name", models.CharField(blank=True, max_length=255, null=True)),
-                ("external_id", models.CharField(blank=True, max_length=255, null=True)),
-                ("created_at", models.DateTimeField(auto_now_add=True)),
+                ("id", models.CharField(default=lnschema_core.ids.run, max_length=20, primary_key=True, serialize=False)),
+                ("name", models.CharField(db_index=True, max_length=255)),
+                ("external_id", models.CharField(db_index=True, max_length=255)),
+                ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
+                ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
             ],
             options={
                 "managed": True,
             },
         ),
         migrations.CreateModel(
             name="User",
             fields=[
                 ("id", models.CharField(max_length=8, primary_key=True, serialize=False)),
-                ("email", models.CharField(max_length=64, unique=True)),
-                ("handle", models.CharField(max_length=64, unique=True)),
-                ("name", models.CharField(blank=True, max_length=64, null=True)),
-                ("created_at", models.DateTimeField(auto_now_add=True)),
-                ("updated_at", models.DateTimeField(auto_now=True)),
+                ("handle", models.CharField(db_index=True, max_length=30, unique=True)),
+                ("email", models.CharField(db_index=True, max_length=255, unique=True)),
+                ("name", models.CharField(db_index=True, max_length=255)),
+                ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
+                ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
             ],
             options={
                 "managed": True,
             },
         ),
         migrations.CreateModel(
             name="Transform",
             fields=[
                 ("id", models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name="ID")),
-                ("name", models.CharField(max_length=255)),
-                ("hash", models.CharField(default=lnschema_core.ids.transform, max_length=12)),
-                ("version", models.CharField(default="0", max_length=10)),
+                ("name", models.CharField(db_index=True, default=None, max_length=255, null=True)),
+                ("title", models.TextField(db_index=True, default=None, null=True)),
+                ("uid", models.CharField(db_index=True, default=lnschema_core.ids.transform, max_length=12)),
+                ("version", models.CharField(db_index=True, default=None, max_length=10, null=True)),
                 (
                     "type",
                     models.CharField(
-                        choices=[("pipeline", "pipeline"), ("notebook", "notebook"), ("app", "app")],
+                        choices=[("pipeline", "pipeline"), ("notebook", "notebook"), ("app", "app"), ("api", "api")],
                         db_index=True,
                         default=lnschema_core._types.TransformType["pipeline"],
-                        max_length=63,
+                        max_length=20,
+                    ),
+                ),
+                ("reference", models.CharField(db_index=True, default=None, max_length=255, null=True)),
+                ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
+                ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
+                (
+                    "created_by",
+                    models.ForeignKey(
+                        default=lnschema_core._users.current_user_id, on_delete=django.db.models.deletion.DO_NOTHING, related_name="created_transforms", to="lnschema_core.user"
                     ),
                 ),
-                ("title", models.TextField(blank=True, null=True)),
-                ("reference", models.CharField(blank=True, max_length=255, null=True)),
-                ("created_at", models.DateTimeField(auto_now_add=True)),
-                ("updated_at", models.DateTimeField(auto_now=True)),
-                ("created_by", models.ForeignKey(default=lnschema_core._users.current_user_id, on_delete=django.db.models.deletion.DO_NOTHING, to="lnschema_core.user")),
             ],
             options={
                 "managed": True,
-                "unique_together": {("name", "version")},
+                "unique_together": {("uid", "version")},
             },
         ),
         migrations.CreateModel(
             name="Storage",
             fields=[
-                ("id", models.CharField(default=lnschema_core.ids.storage, max_length=8, primary_key=True, serialize=False)),
-                ("root", models.CharField(max_length=255)),
-                ("type", models.CharField(blank=True, max_length=63, null=True)),
-                ("region", models.CharField(blank=True, max_length=63, null=True)),
-                ("created_at", models.DateTimeField(auto_now_add=True)),
-                ("updated_at", models.DateTimeField(auto_now=True)),
+                ("id", models.CharField(db_index=True, default=lnschema_core.ids.storage, max_length=8, primary_key=True, serialize=False)),
+                ("root", models.CharField(db_index=True, max_length=255)),
+                ("type", models.CharField(db_index=True, max_length=63)),
+                ("region", models.CharField(db_index=True, max_length=63, null=True)),
+                ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
+                ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
                 (
                     "created_by",
                     models.ForeignKey(
-                        blank=True, default=lnschema_core._users.current_user_id, null=True, on_delete=django.db.models.deletion.DO_NOTHING, to="lnschema_core.user"
+                        default=lnschema_core._users.current_user_id, on_delete=django.db.models.deletion.DO_NOTHING, related_name="created_storages", to="lnschema_core.user"
                     ),
                 ),
             ],
             options={
                 "managed": True,
             },
         ),
@@ -128,84 +134,105 @@
             options={
                 "managed": True,
             },
         ),
         migrations.AddField(
             model_name="run",
             name="created_by",
-            field=models.ForeignKey(default=lnschema_core._users.current_user_id, on_delete=django.db.models.deletion.DO_NOTHING, to="lnschema_core.user"),
+            field=models.ForeignKey(
+                default=lnschema_core._users.current_user_id, on_delete=django.db.models.deletion.DO_NOTHING, related_name="created_runs", to="lnschema_core.user"
+            ),
         ),
         migrations.AddField(
             model_name="run",
             name="inputs",
             field=models.ManyToManyField(related_name="input_of", through="lnschema_core.RunInput", to="lnschema_core.file"),
         ),
         migrations.AddField(
             model_name="run",
             name="transform",
-            field=models.ForeignKey(on_delete=django.db.models.deletion.DO_NOTHING, to="lnschema_core.transform"),
+            field=models.ForeignKey(on_delete=django.db.models.deletion.DO_NOTHING, related_name="runs", to="lnschema_core.transform"),
         ),
         migrations.CreateModel(
             name="Project",
             fields=[
                 ("id", models.CharField(default=lnschema_core.ids.project, max_length=8, primary_key=True, serialize=False)),
-                ("name", models.CharField(max_length=64)),
-                ("created_at", models.DateTimeField(auto_now_add=True)),
-                ("updated_at", models.DateTimeField(auto_now=True)),
-                ("created_by", models.ForeignKey(default=lnschema_core._users.current_user_id, on_delete=django.db.models.deletion.DO_NOTHING, to="lnschema_core.user")),
-                ("files", models.ManyToManyField(to="lnschema_core.file")),
-                ("folders", models.ManyToManyField(to="lnschema_core.folder")),
+                ("name", models.CharField(db_index=True, max_length=255, unique=True)),
+                ("external_id", models.CharField(db_index=True, max_length=255)),
+                ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
+                ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
+                (
+                    "created_by",
+                    models.ForeignKey(
+                        default=lnschema_core._users.current_user_id, on_delete=django.db.models.deletion.DO_NOTHING, related_name="created_projects", to="lnschema_core.user"
+                    ),
+                ),
+                ("files", models.ManyToManyField(related_name="projects", to="lnschema_core.file")),
+                ("folders", models.ManyToManyField(related_name="projects", to="lnschema_core.folder")),
             ],
             options={
                 "managed": True,
             },
         ),
         migrations.AddField(
             model_name="folder",
             name="created_by",
-            field=models.ForeignKey(default=lnschema_core._users.current_user_id, on_delete=django.db.models.deletion.DO_NOTHING, to="lnschema_core.user"),
+            field=models.ForeignKey(
+                default=lnschema_core._users.current_user_id, on_delete=django.db.models.deletion.DO_NOTHING, related_name="created_folders", to="lnschema_core.user"
+            ),
         ),
         migrations.AddField(
             model_name="folder",
             name="files",
-            field=models.ManyToManyField(to="lnschema_core.file"),
+            field=models.ManyToManyField(related_name="folders", to="lnschema_core.file"),
         ),
         migrations.AddField(
             model_name="folder",
             name="storage",
-            field=models.ForeignKey(on_delete=django.db.models.deletion.DO_NOTHING, to="lnschema_core.storage"),
+            field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name="folders", to="lnschema_core.storage"),
         ),
         migrations.AddField(
             model_name="file",
             name="created_by",
-            field=models.ForeignKey(default=lnschema_core._users.current_user_id, on_delete=django.db.models.deletion.DO_NOTHING, to="lnschema_core.user"),
+            field=models.ForeignKey(
+                default=lnschema_core._users.current_user_id, on_delete=django.db.models.deletion.DO_NOTHING, related_name="created_files", to="lnschema_core.user"
+            ),
         ),
         migrations.AddField(
             model_name="file",
             name="run",
-            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name="outputs", to="lnschema_core.run"),
+            field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name="outputs", to="lnschema_core.run"),
         ),
         migrations.AddField(
             model_name="file",
             name="storage",
-            field=models.ForeignKey(on_delete=django.db.models.deletion.DO_NOTHING, to="lnschema_core.storage"),
+            field=models.ForeignKey(on_delete=django.db.models.deletion.DO_NOTHING, related_name="files", to="lnschema_core.storage"),
         ),
         migrations.AddField(
             model_name="file",
             name="transform",
-            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.DO_NOTHING, to="lnschema_core.transform"),
+            field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name="files", to="lnschema_core.transform"),
         ),
         migrations.CreateModel(
-            name="Features",
+            name="Featureset",
             fields=[
-                ("id", models.CharField(max_length=63, primary_key=True, serialize=False)),
-                ("type", models.CharField(max_length=63)),
-                ("created_at", models.DateTimeField(auto_now=True)),
-                ("created_by", models.ForeignKey(default=lnschema_core._users.current_user_id, on_delete=django.db.models.deletion.DO_NOTHING, to="lnschema_core.user")),
-                ("files", models.ManyToManyField(to="lnschema_core.file")),
+                ("id", models.CharField(max_length=64, primary_key=True, serialize=False)),
+                ("type", models.CharField(max_length=64)),
+                ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
+                ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
+                (
+                    "created_by",
+                    models.ForeignKey(
+                        default=lnschema_core._users.current_user_id,
+                        on_delete=django.db.models.deletion.DO_NOTHING,
+                        related_name="created_featuresets",
+                        to="lnschema_core.user",
+                    ),
+                ),
+                ("files", models.ManyToManyField(related_name="featuresets", to="lnschema_core.file")),
             ],
             options={
                 "managed": True,
             },
         ),
         migrations.AlterUniqueTogether(
             name="folder",
```

### Comparing `lamindb_setup-0.46a4/lnschema-core/lnschema_core/models.py` & `lamindb_setup-0.46a5/lnschema-core/lnschema_core/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import builtins
 from pathlib import Path, PurePosixPath
-from typing import Any, Iterable, List, NamedTuple, Optional, Union
+from typing import Dict, Iterable, List, NamedTuple, Optional, Union
 
 import pandas as pd
 from django.db import models
 from lamin_logger import logger
 from upath import UPath
 
 from . import ids
 from ._lookup import lookup as _lookup
 from ._users import current_user_id
 from .types import DataLike, PathLike, TransformType
 
 is_run_from_ipython = getattr(builtins, "__IPYTHON__", False)
+TRANSFORM_TYPE_DEFAULT = TransformType.notebook if is_run_from_ipython else TransformType.pipeline
 
 
 class NoResultFound(Exception):
     pass
 
 
 class MultipleResultsFound(Exception):
@@ -29,15 +30,16 @@
     This brings some of the SQLAlchemy/SQLModel/SQL-inspired calls.
 
     As LaminDB was based on SQLAlchemy/SQLModel in the beginning, and might
     support it again in the future, these calls will be supported longtime.
     """
 
     def df(self):
-        df = pd.DataFrame(self.values())
+        columns = [field.name for field in self.model._meta.fields]
+        df = pd.DataFrame(self.values(), columns=columns)
         if "id" in df.columns:
             df = df.set_index("id")
         return df
 
     def list(self) -> List:
         return list(self)
 
@@ -59,17 +61,18 @@
             return None
         elif len(self) == 1:
             return self[0]
         else:
             raise MultipleResultsFound
 
 
+# todo, make a CreatedUpdated Mixin, but need to figure out docs
 class BaseORM(models.Model):
     def __repr__(self) -> str:
-        fields = ", ".join([f"{k.name}={getattr(self, k.name)}" for k in self._meta.fields])
+        fields = ", ".join([f"{k.name}={getattr(self, k.name)}" for k in self._meta.fields if hasattr(self, k.name)])
         return f"{self.__class__.__name__}({fields})"
 
     @classmethod
     def lookup(cls, field: Optional[str] = None) -> NamedTuple:
         return _lookup(cls, field)
 
     def __str__(self) -> str:
@@ -91,104 +94,150 @@
     """User accounts.
 
     All data in this table is synched from the cloud user account to ensure a
     globally unique user identity.
     """
 
     id = models.CharField(max_length=8, primary_key=True)
-    email = models.CharField(max_length=64, unique=True)
-    handle = models.CharField(max_length=64, unique=True)
-    name = models.CharField(max_length=64, blank=True, null=True)
-    created_at = models.DateTimeField(auto_now_add=True)
-    updated_at = models.DateTimeField(auto_now=True)
+    """Universal id, valid across DB instances."""
+    handle = models.CharField(max_length=30, unique=True, db_index=True)
+    """Universal handle, valid across DB instances."""
+    email = models.CharField(max_length=255, unique=True, db_index=True)
+    """Latest email address."""
+    name = models.CharField(max_length=255, db_index=True)
+    """Name."""
+    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    """Time of creation of record."""
+    updated_at = models.DateTimeField(auto_now=True, db_index=True)
+    """Time of last update to record."""
 
     class Meta:
         managed = True
 
 
 class Storage(BaseORM):
-    """Storage locations, often object storage buckets.
+    """Storage locations, typically cloud buckets.
 
     A file or run-associated file can be stored in any desired S3,
     GCP bucket or local storage location.
 
     This table tracks these locations along with metadata.
     """
 
-    id = models.CharField(max_length=8, default=ids.storage, primary_key=True)
-    root = models.CharField(max_length=255)
+    id = models.CharField(max_length=8, default=ids.storage, db_index=True, primary_key=True)
+    """Universal id, valid across DB instances."""
+    root = models.CharField(max_length=255, db_index=True)
     """Path to the root of the storage location: an s3 path, a local path, etc."""
-    type = models.CharField(max_length=63, blank=True, null=True)
+    type = models.CharField(max_length=63, db_index=True)
     """Local vs. s3 vs. gcp etc."""
-    region = models.CharField(max_length=63, blank=True, null=True)
+    region = models.CharField(max_length=63, db_index=True, null=True)
     """Cloud storage region, if applicable."""
-    created_at = models.DateTimeField(auto_now_add=True)
-    updated_at = models.DateTimeField(auto_now=True)
-    created_by = models.ForeignKey(User, models.DO_NOTHING, blank=True, null=True, default=current_user_id)
+    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    """Time of creation of record."""
+    updated_at = models.DateTimeField(auto_now=True, db_index=True)
+    """Time of last update to record."""
+    created_by = models.ForeignKey(
+        User,
+        models.DO_NOTHING,
+        default=current_user_id,
+        related_name="created_storages",
+    )
+    """Creator of record."""
 
     class Meta:
         managed = True
 
 
 class Project(BaseORM):
     """Projects."""
 
     id = models.CharField(max_length=8, default=ids.project, primary_key=True)
-    name = models.CharField(max_length=64)
-    folders = models.ManyToManyField("Folder")
-    files = models.ManyToManyField("File")
-    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
-    created_at = models.DateTimeField(auto_now_add=True)
-    updated_at = models.DateTimeField(auto_now=True)
+    """Universal id, valid across DB instances."""
+    name = models.CharField(max_length=255, db_index=True, unique=True)
+    """Project name or title."""
+    external_id = models.CharField(max_length=255, db_index=True)
+    """External id (such as from a project management tool)."""
+    folders = models.ManyToManyField("Folder", related_name="projects")
+    """Project folders."""
+    files = models.ManyToManyField("File", related_name="projects")
+    """Project files."""
+    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    """Time of creation of record."""
+    updated_at = models.DateTimeField(auto_now=True, db_index=True)
+    """Time of last update to record."""
+    created_by = models.ForeignKey(
+        User,
+        models.DO_NOTHING,
+        default=current_user_id,
+        related_name="created_projects",
+    )
+    """Creator of record."""
 
     class Meta:
         managed = True
 
 
 class Transform(BaseORM):
     """Data transformations.
 
-    Jupyter notebooks, pipelines, and apps.
+    Pipelines, workflows, notebooks, app-based transforms.
 
-    A pipeline is typically versioned software that can perform a data
-    transformation/processing workflow. This can be anything from typical
-    workflow tools (Nextflow, Snakemake, Prefect, Apache Airflow, etc.) to
-    simple (versioned) scripts.
+    A pipeline is versioned software that transforms data.
+    This can be anything from typical workflow tools (Nextflow, Snakemake,
+    Prefect, Apache Airflow, etc.) to simple (versioned) scripts.
 
-    Data can also be ingested & transformed through an app.
+    Creating a file is a transform, too.
     """
 
-    name = models.CharField(max_length=255)
+    name = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """A name for the transform, a pipeline name, or a file name of a notebook or script.
     """
-    hash = models.CharField(max_length=12, default=ids.transform)
-    version = models.CharField(max_length=10, default="0")
+    title = models.TextField(db_index=True, null=True, default=None)
+    """An additional title, like a notebook title.
+    """
+    uid = models.CharField(max_length=12, default=ids.transform, db_index=True)
+    """Universal id, valid across DB instances."""
+    version = models.CharField(max_length=10, default=None, db_index=True, null=True)
     """Version identifier, defaults to `"0"`.
 
     Use this to label different versions of the same transform.
 
     Consider using `semantic versioning <https://semver.org>`__
     with `Python versioning <https://peps.python.org/pep-0440/>`__.
     """
-    type = models.CharField(max_length=63, choices=TransformType.choices(), db_index=True, default=(TransformType.notebook if is_run_from_ipython else TransformType.pipeline))
-    """Transform type. Defaults to `notebook` if run from IPython, otherwise to `pipeline`.
-    """
-    title = models.TextField(blank=True, null=True)
-    """An additional title, like a notebook title.
+    type = models.CharField(
+        max_length=20,
+        choices=TransformType.choices(),
+        db_index=True,
+        default=TRANSFORM_TYPE_DEFAULT,
+    )
+    """Transform type.
+
+    Defaults to `notebook` if run from IPython, from a script to `pipeline`.
+
+    If run from the app, it defaults to `app`.
     """
-    reference = models.CharField(max_length=255, blank=True, null=True)
+    reference = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Reference for the transform, e.g., a URL.
     """
-    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
-    created_at = models.DateTimeField(auto_now_add=True)
-    updated_at = models.DateTimeField(auto_now=True)
+    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    """Time of creation of record."""
+    updated_at = models.DateTimeField(auto_now=True, db_index=True)
+    """Time of last update to record."""
+    created_by = models.ForeignKey(
+        User,
+        models.DO_NOTHING,
+        default=current_user_id,
+        related_name="created_transforms",
+    )
+    """Creator of record."""
 
     class Meta:
         managed = True
-        unique_together = (("name", "version"),)
+        unique_together = (("uid", "version"),)
 
 
 class Run(BaseORM):
     """Runs of data transforms.
 
     A `run` is any transform of a `file`.
 
@@ -209,119 +258,135 @@
       `run` may output several `files`.
     - References to inputs are stored in the `run_in` table, a
       many-to-many link table between the `file` and `run` tables. Any
       `file` might serve as an input for many `runs`. Similarly, any
       `run` might have many `files` as inputs.
     """
 
-    id = models.CharField(max_length=12, default=ids.run, primary_key=True)
-    name = models.CharField(max_length=255, blank=True, null=True)
-    external_id = models.CharField(max_length=255, blank=True, null=True)
-    transform = models.ForeignKey(Transform, models.DO_NOTHING)
+    id = models.CharField(max_length=20, default=ids.run, primary_key=True)
+    """Universal id, valid across DB instances."""
+    name = models.CharField(max_length=255, db_index=True)
+    """Name or title of run."""
+    external_id = models.CharField(max_length=255, db_index=True)
+    """External id (such as from a workflow tool)."""
+    transform = models.ForeignKey(Transform, models.DO_NOTHING, related_name="runs")
+    """The transform :class:`~lamindb.Transform` that is being run."""
     inputs = models.ManyToManyField("File", through=RunInput, related_name="input_of")
+    """The input files for the run."""
     # outputs on File
-    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
-    created_at = models.DateTimeField(auto_now_add=True)
+    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    """Time of creation of record."""
+    updated_at = models.DateTimeField(auto_now=True, db_index=True)
+    """Time of last update to record."""
+    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id, related_name="created_runs")
+    """Creator of record."""
 
     class Meta:
         managed = True
 
 
-class Features(BaseORM):
+class Featureset(BaseORM):
     """Feature sets.
 
     A feature set is represented by the hash of the set of primary keys and the feature type.
 
     The current supported feature types are lnschema_bionty.Gene,
     lnschema_bionty.Protein & lnschema_bionty.CellMarker.
 
     Guides:
 
-    - :doc:`/guide/scrna`
-    - :doc:`guide/flow`
+    - :doc:`/biology/scrna`
+    - :doc:`/biology/flow`
 
     Examples:
 
     >>> import lnschema_bionty as bt
     >>> reference = bt.Gene(species="mouse")
     >>> features = ln.Features(adata, reference=reference)
     >>> file = ln.File(adata, name="Mouse Lymph Node scRNA-seq", features=features)
 
     Args:
         data: [Path, str, pd.DataFrame, ad.AnnData] - DataFrame or AnnData to parse.
         reference: Any = None - Reference for mapping features.
-        id: str = None - Primary key.
-        type: Any = None - Type of reference.
-        files: List[File] - Files to link against.
     """
 
-    id = models.CharField(max_length=63, primary_key=True)
-    type = models.CharField(max_length=63)
-    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
-    created_at = models.DateTimeField(auto_now=True)
-    files = models.ManyToManyField("File")
+    id = models.CharField(max_length=64, primary_key=True)
+    """A universal id, valid across DB instances: a hash of the linked set of features."""
+    type = models.CharField(max_length=64)
+    """A feature entity type."""
+    files = models.ManyToManyField("File", related_name="featuresets")
+    """Files linked to the featureset."""
+    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    """Time of creation of record."""
+    updated_at = models.DateTimeField(auto_now=True, db_index=True)
+    """Time of last update to record."""
+    created_by = models.ForeignKey(
+        User,
+        models.DO_NOTHING,
+        default=current_user_id,
+        related_name="created_featuresets",
+    )
+    """Creator of record."""
 
     class Meta:
         managed = True
 
-    def __init__(  # type: ignore
-        self,
-        iterable: Iterable = None,
-        field: models.CharField = None,
-        *,
-        id: str = None,
-        type: Any = None,
-        # continue with fields
-        files: List["File"] = [],
-        **map_kwargs,
-    ):
-        kwargs = locals()
-
-        # needed for erroring when passing pd.index
-        if kwargs["data"] is not None:
-            kwargs.pop("data")
-        if kwargs["iterable"] is not None:
-            kwargs.pop("iterable")
-
-        kwargs = {k: v for k, v in kwargs.items() if v and k != "self"}
-        super().__init__(**kwargs)
-
-    def __new__(
+    @classmethod
+    def from_iterable(
         cls,
-        iterable: Iterable = None,
-        field: models.CharField = None,
-        *,
-        id: str = None,
-        type: Any = None,
-        # continue with fields
-        files: List["File"] = [],
-        **map_kwargs,
+        iterable: Iterable,
+        field: models.CharField,
+        species: str = None,
     ):
-        if iterable is not None:
-            from lamindb._file import get_features_from_data
+        """Parse iterable & return featureset & records."""
+        from lamindb._features import parse_features_from_iterable
 
-            features = get_features_from_data(
-                iterable=iterable,
-                field=field,
-                **map_kwargs,
-            )
-        else:
-            features = super().__new__(cls)
+        features = parse_features_from_iterable(
+            iterable=iterable,
+            field=field,
+            species=species,
+        )
         return features
 
+    def __init__(self, *args, **kwargs):  # type: ignore
+        relationships: Dict = {}
+        if "genes" in kwargs:
+            relationships["genes"] = kwargs.pop("genes")
+        if "proteins" in kwargs:
+            relationships["proteins"] = kwargs.pop("proteins")
+        if "cell_markers" in kwargs:
+            relationships["cell_markers"] = kwargs.pop("cell_markers")
+        self._relationships = relationships
+
+        super().__init__(*args, **kwargs)
+
+    def save(self, *args, **kwargs):
+        super().save(*args, **kwargs)
+        for key, records in self._relationships.items():
+            [r.save() for r in records]
+            getattr(self, key).set(records)
+
 
 class Folder(BaseORM):
-    id = models.CharField(max_length=20, primary_key=True)
-    name = models.CharField(max_length=255)
-    key = models.CharField(max_length=255, blank=True, null=True)
-    storage = models.ForeignKey(Storage, models.DO_NOTHING)
-    files = models.ManyToManyField("File")
-    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
-    created_at = models.DateTimeField(auto_now_add=True)
-    updated_at = models.DateTimeField(auto_now=True)
+    id = models.CharField(max_length=20, default=ids.folder, primary_key=True)
+    """A universal random id, valid across DB instances."""
+    name = models.CharField(max_length=255, db_index=True)
+    """Name or title of the folder."""
+    key = models.CharField(max_length=255, null=True, default=None, db_index=True)
+    """Storage key of the folder."""
+    storage = models.ForeignKey(Storage, models.DO_NOTHING, related_name="folders", null=True)
+    """Storage location of the folder."""
+    files = models.ManyToManyField("File", related_name="folders")
+    """Files in folder."""
+    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    """Time of creation of record."""
+    updated_at = models.DateTimeField(auto_now=True, db_index=True)
+    """Time of last update to record."""
+    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id, related_name="created_folders")
+    """Creator of record."""
 
     class Meta:
         managed = True
         unique_together = (("storage", "key"),)
 
     @property
     def __name__(cls) -> str:
@@ -380,43 +445,48 @@
         if path is not None:
             self._local_filepath = privates["local_filepath"]
             self._cloud_filepath = privates["cloud_filepath"]
             self._files = files
 
 
 class File(BaseORM):
-    id: str = models.CharField(max_length=20, primary_key=True)
-    name = models.CharField(max_length=255, blank=True, null=True)
-    suffix = models.CharField(max_length=63, blank=True, null=True)
-    """Suffix to construct the storage key. Defaults to `None`.
+    id = models.CharField(max_length=20, primary_key=True)
+    """A universal random id, valid across DB instances."""
+    name = models.CharField(max_length=255, db_index=True, null=True, default=None)
+    """A universal random id, valid across DB instances."""
+    suffix = models.CharField(max_length=30, db_index=True, null=True, default=None)
+    """File suffix.
 
     This is a file extension if the `file` is stored in a file format.
     It's `None` if the storage format doesn't have a canonical extension.
     """
-    size = models.BigIntegerField(blank=True, null=True)
+    size = models.BigIntegerField(null=True, db_index=True)
     """Size in bytes.
 
     Examples: 1KB is 1e3 bytes, 1MB is 1e6, 1GB is 1e9, 1TB is 1e12 etc.
     """
-    hash = models.CharField(max_length=63, blank=True, null=True)
-    """Hash (md5)."""
-    key = models.CharField(max_length=255, blank=True, null=True)
+    hash = models.CharField(max_length=86, db_index=True, null=True, default=None)
+    """Hash of file content. 86 base64 chars allow to store 64 bytes, 512 bits."""
+    key = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Storage key, the relative path within the storage location."""
-    run = models.ForeignKey(Run, models.DO_NOTHING, blank=True, null=True, related_name="outputs")
+    run = models.ForeignKey(Run, models.DO_NOTHING, related_name="outputs", null=True)
     """:class:`~lamindb.Run` that created the `file`."""
-    transform = models.ForeignKey(Transform, models.DO_NOTHING, blank=True, null=True)
+    transform = models.ForeignKey(Transform, models.DO_NOTHING, related_name="files", null=True)
     """:class:`~lamindb.Transform` whose run created the `file`."""
-    storage: "Storage" = models.ForeignKey(Storage, models.DO_NOTHING)
+    storage: "Storage" = models.ForeignKey(Storage, models.DO_NOTHING, related_name="files")
     """:class:`~lamindb.Storage` location of `file`, see `.path()` for full path."""
     # folders from Folders.files
     # features from Features.files
     # input_of from Run.inputs
-    created_at = models.DateTimeField(auto_now_add=True)
-    updated_at = models.DateTimeField(auto_now=True)
-    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id)
+    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    """Time of creation of record."""
+    updated_at = models.DateTimeField(auto_now=True, db_index=True)
+    """Time of last update to record."""
+    created_by = models.ForeignKey(User, models.DO_NOTHING, default=current_user_id, related_name="created_files")
+    """Creator of record."""
 
     class Meta:
         managed = True
         unique_together = (("storage", "key"),)
 
     def path(self) -> Union[Path, UPath]:
         """Path on storage."""
@@ -425,15 +495,15 @@
     # likely needs an arg `key`
     def replace(
         self,
         data: Union[PathLike, DataLike],
         run: Optional[Run] = None,
         format: Optional[str] = None,
     ) -> None:
-        """Replace data object."""
+        """Replace file content."""
         from lamindb._file import get_file_kwargs_from_data
 
         if isinstance(data, (Path, str)):
             name_to_pass = None
         else:
             name_to_pass = self.name
```

### Comparing `lamindb_setup-0.46a4/lnschema-core/noxfile.py` & `lamindb_setup-0.46a5/lnschema-core/noxfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 
 import nox
-import requests  # type: ignore
+import requests  # type: ignore  # noqa
 from laminci import move_built_docs_to_docs_slash_project_slug, upload_docs_artifact
 from laminci.nox import build_docs, login_testuser1, run_pre_commit, run_pytest  # noqa
 
 nox.options.default_venv_backend = "none"
 
 
 @nox.session
@@ -13,18 +13,18 @@
     run_pre_commit(session)
 
 
 @nox.session
 def install(session: nox.Session) -> None:
     session.run(*"pip install --no-deps .[django]".split())
     session.run(*"git clone --no-single-branch --depth 1 https://github.com/laminlabs/lamindb".split())
-    response = requests.get("https://github.com/laminlabs/lamindb/tree/cleanup")
-    if response.status_code < 400:
-        with session.chdir("./lamindb"):
-            session.run(*"git switch cleanup".split())
+    # response = requests.get("https://github.com/laminlabs/lamindb/tree/cleanup")
+    # if response.status_code < 400:
+    #     with session.chdir("./lamindb"):
+    #         session.run(*"git switch cleanup".split())
     if sys.platform.startswith("linux"):  # remove version pin when running on CI
         session.run(*"sed -i /lnschema_core/d ./lamindb/pyproject.toml".split())
     session.run(*"pip install ./lamindb[aws,test]".split())
 
 
 @nox.session()
 def build(session: nox.Session) -> None:
```

### Comparing `lamindb_setup-0.46a4/lnschema-core/pyproject.toml` & `lamindb_setup-0.46a5/lnschema-core/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/noxfile.py` & `lamindb_setup-0.46a5/noxfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,20 +26,23 @@
 
 @nox.session
 @nox.parametrize(
     "group",
     ["unit", "docs"],
 )
 def install(session: nox.Session, group: str) -> None:
-    session.run(*"pip install bionty".split())
-    session.run(*"pip install --no-deps lnschema_bionty".split())
+    session.run(*"pip install git+https://github.com/laminlabs/bionty".split())
     session.run(
-        *"pip install --no-deps git+https://github.com/laminlabs/lnschema-lamin1"
+        *"pip install --no-deps git+https://github.com/laminlabs/lnschema-bionty"
         .split()
     )
+    # session.run(
+    #     *"pip install --no-deps git+https://github.com/laminlabs/lnschema-lamin1"
+    #     .split()
+    # )
     # install lnschema-core from sub-module
     session.run(*"pip install --no-deps ./lnschema-core".split())
     # install lamindb-setup without deps
     session.run(*"pip install .[aws,test]".split())
 
 
 @nox.session
```

### Comparing `lamindb_setup-0.46a4/pyproject.toml` & `lamindb_setup-0.46a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/tests/test_bionty.py` & `lamindb_setup-0.46a5/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/tests/test_init_instance.py` & `lamindb_setup-0.46a5/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/tests/test_load_instance.py` & `lamindb_setup-0.46a5/tests/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.46a4/PKG-INFO` & `lamindb_setup-0.46a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.46a4
+Version: 0.46a5
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnhub_rest==0.9.10
 Requires-Dist: sqlmodel
 Requires-Dist: lnschema_core>=0.35a1
 Requires-Dist: lamin_logger>=0.3.3
```

